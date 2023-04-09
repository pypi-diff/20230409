# Comparing `tmp/reacher-0.3.5-py2.py3-none-any.whl.zip` & `tmp/reacher-0.3.6-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 7503 bytes, number of entries: 6
+Zip file size: 7852 bytes, number of entries: 6
 -rw-rw-r--  2.0 unx       52 b- defN 23-Mar-26 10:19 reacher/__init__.py
--rw-rw-r--  2.0 unx    18487 b- defN 23-Apr-09 12:20 reacher/reacher.py
--rw-rw-r--  2.0 unx     6457 b- defN 23-Apr-09 12:23 reacher-0.3.5.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Apr-09 12:23 reacher-0.3.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Apr-09 12:23 reacher-0.3.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      448 b- defN 23-Apr-09 12:23 reacher-0.3.5.dist-info/RECORD
-6 files, 25562 bytes uncompressed, 6695 bytes compressed:  73.8%
+-rw-rw-r--  2.0 unx    19000 b- defN 23-Apr-09 13:33 reacher/reacher.py
+-rw-rw-r--  2.0 unx     6932 b- defN 23-Apr-09 13:45 reacher-0.3.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Apr-09 13:45 reacher-0.3.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Apr-09 13:45 reacher-0.3.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      448 b- defN 23-Apr-09 13:45 reacher-0.3.6.dist-info/RECORD
+6 files, 26550 bytes uncompressed, 7044 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: reacher/__init__.py
 Comment: 
 
 Filename: reacher/reacher.py
 Comment: 
 
-Filename: reacher-0.3.5.dist-info/METADATA
+Filename: reacher-0.3.6.dist-info/METADATA
 Comment: 
 
-Filename: reacher-0.3.5.dist-info/WHEEL
+Filename: reacher-0.3.6.dist-info/WHEEL
 Comment: 
 
-Filename: reacher-0.3.5.dist-info/top_level.txt
+Filename: reacher-0.3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: reacher-0.3.5.dist-info/RECORD
+Filename: reacher-0.3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## reacher/reacher.py

```diff
@@ -1,25 +1,31 @@
+
 import os
-from typing import List, Dict
+from typing import List, Dict, Union
 import uuid
 from os import system
 from typing import List
 import os
 from paramiko import AutoAddPolicy, RSAKey, SSHClient
 from paramiko.auth_handler import AuthenticationException, SSHException
 from scp import SCPClient, SCPException
 import logging
 import shutil
 import socket
 import select
+import sys
+
 try:
     import SocketServer
 except ImportError:
     import socketserver as SocketServer
 
+# Define progress callback that prints the current percentage completed for the file
+def progress4(filename, size, sent, peername):
+    sys.stdout.write("(%s:%s) %s's progress: %.2f%%   \r" % (peername[0], peername[1], filename, float(sent)/float(size)*100) )
 
 class RemoteClient:
     """Client to interact with a remote host via SSH & SCP."""
 
     def __init__(
         self,
         host: str,
@@ -57,15 +63,15 @@
             )
         except Exception as e:
             logging.error(f"Unexpected error occurred while connecting to host: {e}")
 
     @property
     def scp(self) -> SCPClient:
         conn = self.connection
-        return SCPClient(conn.get_transport())
+        return SCPClient(conn.get_transport(), progress4=progress4)
 
     def _get_ssh_key(self):
         try:
             self.ssh_key = RSAKey.from_private_key_file(self.ssh_key_filepath)
             logging.info(f"Found SSH key at self {self.ssh_key_filepath}")
             return self.ssh_key
         except SSHException as e:
@@ -104,23 +110,15 @@
         except Exception as e:
             logging.error(f"Unexpected exception during bulk upload: {e}")
 
     def download_file(self, remote_filepath: str, local_path: str):
 
         os.makedirs(local_path, exist_ok=True)
 
-        file_name = remote_filepath.split("/")[-1]
-        
-        self.scp.get(remote_filepath)
-
-        # shutil.move only overwrites if the destination is absolut
-        shutil.move(
-            os.path.abspath(file_name),
-            os.path.join(os.path.abspath(local_path), file_name)
-        )
+        self.scp.get(remote_filepath, local_path=local_path, recursive=True)
 
     def execute_command(self, command: str, stream: bool = False, suppress: bool = False):
 
         stdin, stdout, stderr = self.connection.exec_command(command, get_pty=True)
 
         stdout._set_mode('rb')
 
@@ -231,54 +229,73 @@
 
         return os.path.join(
             self.workspace_path,
             self._build_name,
             Reacher.ARTIFACATS_PATH
         )
 
-    def _setup_remote(self):
+    def setup(self):
 
         self._client.execute_command(
             f"mkdir -p {self.build_path} && mkdir -p {self.artifact_path} && mkdir -p {self.log_path}"
         )
 
     def clear(self):
 
         self._client.execute_command(
             f"rm -rf {self.build_path}", suppress=True,
         )
 
-        self._setup_remote()
+        self.setup()
 
-    @property
-    def artifacts(self):
+    def ls(self, folder: str = None):
+
+        if folder is None:
+            folder = self.build_path
+        else:
+            folder = os.path.join(self.build_path, folder)
 
         r = self._client.execute_command(
-            f"ls -R {self.artifact_path}",
+            f"find {folder} -print",
             suppress=False,
         )
 
-    def get_artifact(self, artifact: str, destination: str = None):
+    def put(self, path: str, destination_folder: str = None):
+        
+        if destination_folder is None:
+            destination_folder = self.build_path
+        else:
+            destination_folder = os.path.join(self.build_path, destination_folder)
 
-        self._client.download_file(
-            os.path.join(self.artifact_path, artifact),
-            (
-                destination if destination is not None else 
-                os.path.join(".reacher", self._build_name, Reacher.ARTIFACATS_PATH)
-            )
-        )
+        if not isinstance(path, list):
+            path = [path]
 
-    def put_artifact(self, artifact: str):
+        for p in path:
+            self._client.upload_dir(p, destination_folder)
 
-        self._client.upload_dir(artifact, self.artifact_path)
+    def get(self, path: Union[List[str], str], destination_folder: str = None):
 
-    def get_all_artifact(self, destination: str = None):
+        if destination_folder is None:
+            destination_folder = os.path.join(".reacher", self._build_name)
 
-        for artifact in self.artifacts:
-            self.get_artifact(artifact, destination)
+        if not isinstance(path, list):
+            path = [path]
+
+        for p in path:
+            self._client.download_file(os.path.join(self.build_path, p), destination_folder)
+
+    @property
+    def artifacts(self):
+        self.ls(self.artifact_path)
+
+    def get_artifact(self, artifact: str, destination: str = None):
+        self.get(os.path.join(self.artifact_path, artifact), destination)
+
+    def put_artifact(self, artifact: str):
+        self.put(artifact, self.artifact_path)
 
     def _wrap_command_in_screen(self, command: str, named_session: str = None):
 
         named_session = named_session if named_session is not None else uuid.uuid4()
 
         return f"screen -S {named_session} {command}"
 
@@ -287,29 +304,29 @@
         command,
         stream: bool = True,
         suppress: bool = False,
         named_session: str = None,
         wrap_in_screen: bool = False,
     ):  
 
-        if wrap_in_screen or named_session is not None:
+        if wrap_in_screen:
             command = self._wrap_command_in_screen(command, named_session=named_session)
 
         command = f"cd {self.build_path} && {command}"
 
         return self._client.execute_command(
             command,
             stream=stream,
             suppress=suppress,
         )
 
     def execute(
         self,
+        command: str,
         file: str = None,
-        command: str = None,
         context_folder: str = None,
         named_session: str = None,
     ):  
 
         if file is not None:
             self._client.upload_dir(file, self.build_path)
         if context_folder is not None:
@@ -317,40 +334,32 @@
             intermidiate = os.path.join(self.build_path, "trash0")
             self._client.upload_dir(context_folder, intermidiate)
             self.execute_command(
                 f"mv {intermidiate}/{e}/* {self.build_path} && rm -r {intermidiate}",
                 wrap_in_screen=False,
             )
 
-        #self._client.execute_command(f"rm -r {tmp_path}")
-        
         self.execute_command(
             command,
             named_session=named_session,
-            wrap_in_screen=True
+            wrap_in_screen=True,
         )
 
     def list_named_sessions(self):
 
         self.execute_command(f"screen -list")
 
     def attach_named_session(self, named_session: str):
 
         self.execute_command(f"screen -r -d {named_session}")
 
     def kill_named_session(self, named_session: str):
 
         self.execute_command(f"screen -X -S {named_session} quit")
 
-    def setup(
-        self,
-    ):
-
-        self.clear()
-
 class ReacherDocker(Reacher):
 
     CON_WORKSPACE_PATH = "/workspace"
 
     MOUNTED = [
         Reacher.ARTIFACATS_PATH,
         Reacher.LOGS_PATH
@@ -450,16 +459,16 @@
 
         if len(ls) > 0:
             cmd = f"rm -r {' '.join(ls)}"
             self.execute_command(cmd)
 
     def execute(
         self,
+        command: str,
         file: str = None,
-        command: str = None,
         context_folder: str = None,
         named_session: str = None,
         clear_container: bool = False,
     ):  
 
         if clear_container:
             self._clear_container()
```

## Comparing `reacher-0.3.5.dist-info/METADATA` & `reacher-0.3.6.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reacher
-Version: 0.3.5
+Version: 0.3.6
 Summary: A tool for reaching out to remote machine - excecute code and collect artificats
 Home-page: https://github.com/johannes-skog/reacher
 Author: johannes skog
 Author-email: johannes.skog.unsec@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -122,14 +122,41 @@
 
 ```python
 reacher.add_port_forward(remote_port=6006, local_port=5998, paramiko=True)
 ```
 
 this will spin of a seperate daemon thread handling the port-forwading. Set paramiko to False to trigger a system call for the port forwarding instead.
 
+
+# Put and getting files
+
+Supports list of files or single files
+
+```python
+reacher.put(["setup.py", "build.sh", "reacher"], <destination>)
+```
+
+default destination is root directory of the build.
+
+```python
+reacher.get(["setup.py", "build.sh", "reacher"], <destination>)
+```
+
+default destination is ```.reacher/build_name```, relative your local path.
+
+Use ```reacher.ls(base_path)``` to list files on the remote.
+
+# Running commands on the remote 
+
+```python
+reacher.execute_command("ls", wrap_in_screen=True, named_session="test")
+```
+
+wrap the command in a screen if running something that you want make persistent. If named_session is not specified an unique id will be created for the sesssion.
+
 # Running code on the remote 
 
 ## Running a code-snippet 
 
 Now we have built the docker image on the remote and have a container ready to execute whatever code that we want to run.
 
 A "Hello World" test can be triggered from a notebook.
@@ -216,12 +243,7 @@
 
 Successfully copied 3.584kB to base://workspace
 
 Hello from class Dependency
 [screen is terminating]
 ```
 
-## Generate artifact 
-
-In many cases we want to run some code on the remote and afterwards collect some artifacts.
-
-Everything that is saved in the artifact directory will be available for us to download to the local machine.
```

