# Comparing `tmp/reacher-0.3.6-py2.py3-none-any.whl.zip` & `tmp/reacher-0.3.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 7852 bytes, number of entries: 6
+Zip file size: 7938 bytes, number of entries: 6
 -rw-rw-r--  2.0 unx       52 b- defN 23-Mar-26 10:19 reacher/__init__.py
--rw-rw-r--  2.0 unx    19000 b- defN 23-Apr-09 13:33 reacher/reacher.py
--rw-rw-r--  2.0 unx     6932 b- defN 23-Apr-09 13:45 reacher-0.3.6.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Apr-09 13:45 reacher-0.3.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Apr-09 13:45 reacher-0.3.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      448 b- defN 23-Apr-09 13:45 reacher-0.3.6.dist-info/RECORD
-6 files, 26550 bytes uncompressed, 7044 bytes compressed:  73.5%
+-rw-rw-r--  2.0 unx    19620 b- defN 23-Apr-09 17:16 reacher/reacher.py
+-rw-rw-r--  2.0 unx     6932 b- defN 23-Apr-09 17:55 reacher-0.3.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Apr-09 17:55 reacher-0.3.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Apr-09 17:55 reacher-0.3.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      448 b- defN 23-Apr-09 17:55 reacher-0.3.7.dist-info/RECORD
+6 files, 27170 bytes uncompressed, 7130 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: reacher/__init__.py
 Comment: 
 
 Filename: reacher/reacher.py
 Comment: 
 
-Filename: reacher-0.3.6.dist-info/METADATA
+Filename: reacher-0.3.7.dist-info/METADATA
 Comment: 
 
-Filename: reacher-0.3.6.dist-info/WHEEL
+Filename: reacher-0.3.7.dist-info/WHEEL
 Comment: 
 
-Filename: reacher-0.3.6.dist-info/top_level.txt
+Filename: reacher-0.3.7.dist-info/top_level.txt
 Comment: 
 
-Filename: reacher-0.3.6.dist-info/RECORD
+Filename: reacher-0.3.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## reacher/reacher.py

```diff
@@ -164,14 +164,20 @@
 
     ARTIFACATS_PATH = "artifacts"
     LOGS_PATH = "logs"
 
     WORKSPACE_PATH = "~/.reacher"
     BUILD_PATH = ""
 
+    EXCLUDES = [
+        ".git",
+        ".__pycache__",
+        "logs",
+    ]
+
     def __init__(
         self,
         build_name: str,
         client: RemoteClient = None,
         host: str = None,
         port: int = 22,
         user: str = None,
@@ -243,25 +249,30 @@
 
         self._client.execute_command(
             f"rm -rf {self.build_path}", suppress=True,
         )
 
         self.setup()
 
-    def ls(self, folder: str = None):
+    def ls(self, folder: str = None, supress: bool = False):
 
         if folder is None:
             folder = self.build_path
         else:
             folder = os.path.join(self.build_path, folder)
 
-        r = self._client.execute_command(
+        r = self.execute_command(
             f"find {folder} -print",
-            suppress=False,
-        )
+            suppress=supress,
+            stream=False,
+        ).replace("\n", "").split("\r")
+
+        r = [x for x in r if x != "" and x != "."]
+
+        return r
 
     def put(self, path: str, destination_folder: str = None):
         
         if destination_folder is None:
             destination_folder = self.build_path
         else:
             destination_folder = os.path.join(self.build_path, destination_folder)
@@ -358,15 +369,15 @@
 
 class ReacherDocker(Reacher):
 
     CON_WORKSPACE_PATH = "/workspace"
 
     MOUNTED = [
         Reacher.ARTIFACATS_PATH,
-        Reacher.LOGS_PATH
+        Reacher.LOGS_PATH, 
     ]
 
     def __init__(
         self,
         build_name: str,
         image_name: str,
         build_context: str,
@@ -410,14 +421,29 @@
         if self.exists:
             self._client.execute_command(
                 f"docker rm {self._build_name}", suppress=True,
             )
 
         super().clear()
 
+    def ls(self, folder: str = None, supress: bool = False):
+
+        if folder is None:
+            folder = "."
+
+        r = self.execute_command(
+            f"find {folder} -print",
+            suppress=supress,
+            stream=False,
+        ).replace("\n", "").split("\r")
+
+        r = [x for x in r if x != "" and x != "."]
+
+        return r
+
     def build(self):
 
         self.clear()
 
         self._client.execute_command(
             f"docker build -t {self._build_name} {os.path.join(self.build_path, self._build_context)}",
             stream=True,
@@ -439,43 +465,41 @@
 
         return self._client.execute_command(
             command,
             stream=stream,
             suppress=suppress,
         )
 
-    def _clear_container(self):
+    def clear_container(self):
 
-        ls = self.execute_command("ls", stream=False, suppress=True)
+        files = self.ls(supress=True)
+        files_pruned = []
 
-        ls = " ".join(ls).split()   
-
-        ls = [
-            x.strip('\n').strip('\r').replace("\t", '') for x in ls
-        ]
-
-        ls = [
-            x for x in ls if (x not in Reacher.MOUNTED)
-        ]
-
-        if len(ls) > 0:
-            cmd = f"rm -r {' '.join(ls)}"
+        for x in files:
+            if any([f in x for f in self.MOUNTED]):
+                continue
+            if x == "" or x == "." or x == "..":
+                continue
+            files_pruned.append(x)
+        
+        if len(files_pruned) > 0:
+            cmd = f"rm -r {' '.join(files_pruned)}"
             self.execute_command(cmd)
 
     def execute(
         self,
         command: str,
         file: str = None,
         context_folder: str = None,
         named_session: str = None,
         clear_container: bool = False,
     ):  
 
         if clear_container:
-            self._clear_container()
+            self.clear_container()
 
         tmp_path = os.path.join(self.build_path, "src")
         self._client.execute_command(f"mkdir -p {tmp_path}")
 
         if file is not None:
             self._client.upload_dir(file, tmp_path)
         
@@ -484,15 +508,15 @@
             intermidiate = os.path.join(self.build_path, "trash0")
             self._client.upload_dir(context_folder, intermidiate)
             self._client.execute_command(
                 f"mv {intermidiate}/{e}/* {tmp_path} && rm -r {intermidiate}"
             )
 
         self._client.execute_command(
-            f"docker cp {tmp_path}/. {self._build_name}:/{Reacher.CON_WORKSPACE_PATH}"
+            f"docker cp {tmp_path}/. {self._build_name}:/{ReacherDocker.CON_WORKSPACE_PATH}"
         )
 
         self._client.execute_command(f"rm -r {tmp_path}")
 
         self.execute_command(
             command,
             named_session=named_session,
@@ -510,18 +534,18 @@
         self.clear()
 
         extra_args = ""
 
         if gpu:
             extra_args = "--runtime=nvidia --gpus all"
 
-        ctx = f"docker run -dt {extra_args} -w {Reacher.CON_WORKSPACE_PATH} --name {self._build_name}"
+        ctx = f"docker run -dt {extra_args} -w {ReacherDocker.CON_WORKSPACE_PATH} --name {self._build_name}"
 
-        ctx = f"{ctx} -v {self.artifact_path}:{Reacher.CON_WORKSPACE_PATH}/{Reacher.ARTIFACATS_PATH}"
-        ctx = f"{ctx} -v  {self.log_path}:{Reacher.CON_WORKSPACE_PATH}/{Reacher.LOGS_PATH}"
+        ctx = f"{ctx} -v {self.artifact_path}:{ReacherDocker.CON_WORKSPACE_PATH}/{Reacher.ARTIFACATS_PATH}"
+        ctx = f"{ctx} -v  {self.log_path}:{ReacherDocker.CON_WORKSPACE_PATH}/{Reacher.LOGS_PATH}"
 
         if ports is not None:
             for p in ports:
                 ctx = f"{ctx} -p {p}:{p}"
 
         if envs is not None:
             for k, v in envs.items():
```

## Comparing `reacher-0.3.6.dist-info/METADATA` & `reacher-0.3.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reacher
-Version: 0.3.6
+Version: 0.3.7
 Summary: A tool for reaching out to remote machine - excecute code and collect artificats
 Home-page: https://github.com/johannes-skog/reacher
 Author: johannes skog
 Author-email: johannes.skog.unsec@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

