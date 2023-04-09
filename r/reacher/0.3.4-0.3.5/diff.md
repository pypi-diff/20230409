# Comparing `tmp/reacher-0.3.4-py2.py3-none-any.whl.zip` & `tmp/reacher-0.3.5-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 7496 bytes, number of entries: 6
+Zip file size: 7503 bytes, number of entries: 6
 -rw-rw-r--  2.0 unx       52 b- defN 23-Mar-26 10:19 reacher/__init__.py
--rw-rw-r--  2.0 unx    18371 b- defN 23-Apr-09 11:12 reacher/reacher.py
--rw-rw-r--  2.0 unx     6362 b- defN 23-Apr-09 11:15 reacher-0.3.4.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Apr-09 11:15 reacher-0.3.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Apr-09 11:15 reacher-0.3.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      448 b- defN 23-Apr-09 11:15 reacher-0.3.4.dist-info/RECORD
-6 files, 25351 bytes uncompressed, 6688 bytes compressed:  73.6%
+-rw-rw-r--  2.0 unx    18487 b- defN 23-Apr-09 12:20 reacher/reacher.py
+-rw-rw-r--  2.0 unx     6457 b- defN 23-Apr-09 12:23 reacher-0.3.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Apr-09 12:23 reacher-0.3.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Apr-09 12:23 reacher-0.3.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      448 b- defN 23-Apr-09 12:23 reacher-0.3.5.dist-info/RECORD
+6 files, 25562 bytes uncompressed, 6695 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: reacher/__init__.py
 Comment: 
 
 Filename: reacher/reacher.py
 Comment: 
 
-Filename: reacher-0.3.4.dist-info/METADATA
+Filename: reacher-0.3.5.dist-info/METADATA
 Comment: 
 
-Filename: reacher-0.3.4.dist-info/WHEEL
+Filename: reacher-0.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: reacher-0.3.4.dist-info/top_level.txt
+Filename: reacher-0.3.5.dist-info/top_level.txt
 Comment: 
 
-Filename: reacher-0.3.4.dist-info/RECORD
+Filename: reacher-0.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## reacher/reacher.py

```diff
@@ -43,15 +43,15 @@
             client.load_system_host_keys()
             client.set_missing_host_key_policy(AutoAddPolicy())
             client.connect(
                 self.host,
                 username=self.user,
                 password=self.password,
                 key_filename=self.ssh_key_filepath,
-                timeout=5000,
+                timeout=10000,
                 port=self.port,
             )
             return client
         except AuthenticationException as e:
             logging.error(
                 f"AuthenticationException occurred; did you remember to generate an SSH key? {e}"
             )
@@ -204,17 +204,17 @@
         self._build_name = build_name
     
     @property
     def workspace_path(self):
 
         return os.path.join("/home", self._client.user, ".reacher")
     
-    def add_port_forward(self, remote_port: int, local_port: int):
+    def add_port_forward(self, remote_port: int, local_port: int, paramiko: bool = True):
         
-        self._port_forwarding.add_port_forward(remote_port, local_port)
+        self._port_forwarding.add_port_forward(remote_port, local_port, paramiko)
 
     @property
     def build_path(self):
 
         return os.path.join(self.workspace_path, self._build_name)
 
     @property
@@ -306,28 +306,22 @@
         self,
         file: str = None,
         command: str = None,
         context_folder: str = None,
         named_session: str = None,
     ):  
 
-        tmp_path = os.path.join(self.build_path, "src")
-        self._client.execute_command(f"mkdir -p {tmp_path}")
-
         if file is not None:
-            print("uploading file")
             self._client.upload_dir(file, self.build_path)
-        print("uploading file done")
         if context_folder is not None:
             e = context_folder.split("/")[-1]
-            print(e)
             intermidiate = os.path.join(self.build_path, "trash0")
             self._client.upload_dir(context_folder, intermidiate)
             self.execute_command(
-                f"mv {intermidiate}/{e}/* {self.build_path} && rm -r {intermidiate} && rm -r {intermidiate}/{e}",
+                f"mv {intermidiate}/{e}/* {self.build_path} && rm -r {intermidiate}",
                 wrap_in_screen=False,
             )
 
         #self._client.execute_command(f"rm -r {tmp_path}")
         
         self.execute_command(
             command,
@@ -606,37 +600,45 @@
         peername = self.request.getpeername()
         chan.close()
         self.request.close()
         print("Tunnel closed from %r" % (peername,))
 
 
 def forward_tunnel(local_port, remote_host, remote_port, transport):
-    # this is a little convoluted, but lets me configure things for the Handler
-    # object.  (SocketServer doesn't give Handlers any way to access the outer
-    # server normally.)
+
     class SubHander(Handler):
         chain_host = remote_host
         chain_port = remote_port
         ssh_transport = transport
 
     ForwardServer(("", local_port), SubHander).serve_forever()
     
+
+def forward_tunnel_system(
+        local_port,
+        remote_port,
+        client,
+):
+
+    command = f"ssh -L {local_port}:localhost:{remote_port} -N {client.user}@{client.host} -p {client.port}"
+    
+    os.system(command)
     
 import threading
     
 class PortForwarding(object):
     
     def __init__(
         self,
         host: str = None,
         user: str = None,
         ssh_port: int = 22,
         ssh_key_file_path: str = None,
         password: str = None,
-        client: RemoteClient = None
+        client: RemoteClient = None,
     ):
         
         if client is None:
         
             self._client = RemoteClient(
                 host=host,
                 user=user,
@@ -647,20 +649,30 @@
             
         else:
             
             self._client = client
 
         self._threads = []
     
-    def add_port_forward(self, remote_port: int, local_port: int):
+    def add_port_forward(self, remote_port: int, local_port: int, paramiko: bool = True):
         
-        transport = self._client.connection.get_transport()
-        
-        x = threading.Thread(
-            target=forward_tunnel,
-            args=(local_port, self._client.host, remote_port, transport),
-            daemon=True
-        )
+        if paramiko:
+
+            transport = self._client.connection.get_transport()
         
+            x = threading.Thread(
+                target=forward_tunnel,
+                args=(local_port, self._client.host, remote_port, transport),
+                daemon=True
+            )
+
+        else:
+                
+            x = threading.Thread(
+                target=forward_tunnel_system,
+                args=(local_port, remote_port, self._client),
+                daemon=True
+            )
+
         self._threads.append(x)
         
         self._threads[-1].start()
```

## Comparing `reacher-0.3.4.dist-info/METADATA` & `reacher-0.3.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reacher
-Version: 0.3.4
+Version: 0.3.5
 Summary: A tool for reaching out to remote machine - excecute code and collect artificats
 Home-page: https://github.com/johannes-skog/reacher
 Author: johannes skog
 Author-email: johannes.skog.unsec@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -117,18 +117,18 @@
 ```
 
 # Port-forwarding between remote and local
 
 If you want to access some service on the remote, you can forward the traffic on the ports of the remote to the local machine.
 
 ```python
-reacher.add_port_forward(remote_port=6006, local_port=5998)
+reacher.add_port_forward(remote_port=6006, local_port=5998, paramiko=True)
 ```
 
-this will spin of a seperate daemon thread handling the port-forwading.
+this will spin of a seperate daemon thread handling the port-forwading. Set paramiko to False to trigger a system call for the port forwarding instead.
 
 # Running code on the remote 
 
 ## Running a code-snippet 
 
 Now we have built the docker image on the remote and have a container ready to execute whatever code that we want to run.
```

