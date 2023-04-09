# Comparing `tmp/reacher-0.3.3-py2.py3-none-any.whl.zip` & `tmp/reacher-0.3.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 6282 bytes, number of entries: 6
+Zip file size: 7496 bytes, number of entries: 6
 -rw-rw-r--  2.0 unx       52 b- defN 23-Mar-26 10:19 reacher/__init__.py
--rw-rw-r--  2.0 unx    12629 b- defN 23-Apr-04 15:56 reacher/reacher.py
--rw-rw-r--  2.0 unx     5438 b- defN 23-Apr-04 16:01 reacher-0.3.3.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Apr-04 16:01 reacher-0.3.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Apr-04 16:01 reacher-0.3.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      448 b- defN 23-Apr-04 16:01 reacher-0.3.3.dist-info/RECORD
-6 files, 18685 bytes uncompressed, 5474 bytes compressed:  70.7%
+-rw-rw-r--  2.0 unx    18371 b- defN 23-Apr-09 11:12 reacher/reacher.py
+-rw-rw-r--  2.0 unx     6362 b- defN 23-Apr-09 11:15 reacher-0.3.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Apr-09 11:15 reacher-0.3.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Apr-09 11:15 reacher-0.3.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      448 b- defN 23-Apr-09 11:15 reacher-0.3.4.dist-info/RECORD
+6 files, 25351 bytes uncompressed, 6688 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: reacher/__init__.py
 Comment: 
 
 Filename: reacher/reacher.py
 Comment: 
 
-Filename: reacher-0.3.3.dist-info/METADATA
+Filename: reacher-0.3.4.dist-info/METADATA
 Comment: 
 
-Filename: reacher-0.3.3.dist-info/WHEEL
+Filename: reacher-0.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: reacher-0.3.3.dist-info/top_level.txt
+Filename: reacher-0.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: reacher-0.3.3.dist-info/RECORD
+Filename: reacher-0.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## reacher/reacher.py

```diff
@@ -5,29 +5,38 @@
 from typing import List
 import os
 from paramiko import AutoAddPolicy, RSAKey, SSHClient
 from paramiko.auth_handler import AuthenticationException, SSHException
 from scp import SCPClient, SCPException
 import logging
 import shutil
+import socket
+import select
+try:
+    import SocketServer
+except ImportError:
+    import socketserver as SocketServer
+
 
 class RemoteClient:
     """Client to interact with a remote host via SSH & SCP."""
 
     def __init__(
         self,
         host: str,
         user: str,
-        password: str,
         ssh_key_filepath: str,
+        port: int = 22,
+        password: str = None,
     ):
         self.host = host
         self.user = user
         self.password = password
         self.ssh_key_filepath = ssh_key_filepath
+        self.port = port
         self.client = None
         self._upload_ssh_key()
 
     @property
     def connection(self):
         try:
             client = SSHClient()
@@ -35,14 +44,15 @@
             client.set_missing_host_key_policy(AutoAddPolicy())
             client.connect(
                 self.host,
                 username=self.user,
                 password=self.password,
                 key_filename=self.ssh_key_filepath,
                 timeout=5000,
+                port=self.port,
             )
             return client
         except AuthenticationException as e:
             logging.error(
                 f"AuthenticationException occurred; did you remember to generate an SSH key? {e}"
             )
         except Exception as e:
@@ -148,152 +158,263 @@
 
         stderr.channel.recv_exit_status()
         for line in stderr.readlines():
             print(line)
 
         return response
 
-
 class Reacher(object):
 
+    ARTIFACATS_PATH = "artifacts"
+    LOGS_PATH = "logs"
+
     WORKSPACE_PATH = "~/.reacher"
     BUILD_PATH = ""
 
-    CON_WORKSPACE_PATH = "/workspace"
-    CON_ARTIFACATS_PATH = "artifacts"
-    CON_LOGS_PATH = "logs"
-
-    MOUNTED = [
-        CON_ARTIFACATS_PATH,
-        CON_LOGS_PATH
-    ]
-
     def __init__(
         self,
         build_name: str,
-        image_name: str,
-        build_context: str,
         client: RemoteClient = None,
         host: str = None,
+        port: int = 22,
         user: str = None,
         password: str = None,
         ssh_key_filepath: str = None
     ):
 
         if client is None:
 
             assert (
                 host is not None
                 and user is not None
-                and password is not None
                 and ssh_key_filepath is not None
             )
 
             client = RemoteClient(
                 host=host,
                 user=user,
                 password=password,
                 ssh_key_filepath=ssh_key_filepath,
+                port=port,
             )
 
         self._client = client
+    
+        self._port_forwarding = PortForwarding(client=self._client)
+
         self._build_name = build_name
-        self._image_name = image_name
-        self._build_context = build_context 
     
     @property
     def workspace_path(self):
 
         return os.path.join("/home", self._client.user, ".reacher")
+    
+    def add_port_forward(self, remote_port: int, local_port: int):
+        
+        self._port_forwarding.add_port_forward(remote_port, local_port)
 
     @property
     def build_path(self):
 
         return os.path.join(self.workspace_path, self._build_name)
 
     @property
     def log_path(self):
 
         return os.path.join(
             self.workspace_path,
             self._build_name,
-            Reacher.CON_LOGS_PATH
+            Reacher.LOGS_PATH
         )
 
     @property
     def artifact_path(self):
 
         return os.path.join(
             self.workspace_path,
             self._build_name,
-            Reacher.CON_ARTIFACATS_PATH
+            Reacher.ARTIFACATS_PATH
         )
 
     def _setup_remote(self):
 
         self._client.execute_command(
             f"mkdir -p {self.build_path} && mkdir -p {self.artifact_path} && mkdir -p {self.log_path}"
         )
 
-        self._client.upload_dir(
-            self._build_context,
-            self.build_path,
-        )
-
     def clear(self):
 
         self._client.execute_command(
             f"rm -rf {self.build_path}", suppress=True,
         )
 
-        if self.is_running:
-            self._client.execute_command(
-                f"docker stop {self._build_name}", suppress=True,
-            )
-
-        if self.exists:
-            self._client.execute_command(
-                f"docker rm {self._build_name}", suppress=True,
-            )
-
         self._setup_remote()
 
     @property
     def artifacts(self):
 
         r = self._client.execute_command(
-            f"ls -1 {self.artifact_path}",
-            suppress=True,
+            f"ls -R {self.artifact_path}",
+            suppress=False,
         )
 
-        r = r.replace("\n", "").split("\r")
-
-        r = [x for x in r if (isinstance(x, str) and x != "")]
-
-        return r
-
     def get_artifact(self, artifact: str, destination: str = None):
 
         self._client.download_file(
             os.path.join(self.artifact_path, artifact),
             (
                 destination if destination is not None else 
-                os.path.join(".reacher", self._build_name, Reacher.CON_ARTIFACATS_PATH)
+                os.path.join(".reacher", self._build_name, Reacher.ARTIFACATS_PATH)
             )
         )
 
     def put_artifact(self, artifact: str):
 
         self._client.upload_dir(artifact, self.artifact_path)
 
     def get_all_artifact(self, destination: str = None):
 
         for artifact in self.artifacts:
             self.get_artifact(artifact, destination)
 
+    def _wrap_command_in_screen(self, command: str, named_session: str = None):
+
+        named_session = named_session if named_session is not None else uuid.uuid4()
+
+        return f"screen -S {named_session} {command}"
+
+    def execute_command(
+        self,
+        command,
+        stream: bool = True,
+        suppress: bool = False,
+        named_session: str = None,
+        wrap_in_screen: bool = False,
+    ):  
+
+        if wrap_in_screen or named_session is not None:
+            command = self._wrap_command_in_screen(command, named_session=named_session)
+
+        command = f"cd {self.build_path} && {command}"
+
+        return self._client.execute_command(
+            command,
+            stream=stream,
+            suppress=suppress,
+        )
+
+    def execute(
+        self,
+        file: str = None,
+        command: str = None,
+        context_folder: str = None,
+        named_session: str = None,
+    ):  
+
+        tmp_path = os.path.join(self.build_path, "src")
+        self._client.execute_command(f"mkdir -p {tmp_path}")
+
+        if file is not None:
+            print("uploading file")
+            self._client.upload_dir(file, self.build_path)
+        print("uploading file done")
+        if context_folder is not None:
+            e = context_folder.split("/")[-1]
+            print(e)
+            intermidiate = os.path.join(self.build_path, "trash0")
+            self._client.upload_dir(context_folder, intermidiate)
+            self.execute_command(
+                f"mv {intermidiate}/{e}/* {self.build_path} && rm -r {intermidiate} && rm -r {intermidiate}/{e}",
+                wrap_in_screen=False,
+            )
+
+        #self._client.execute_command(f"rm -r {tmp_path}")
+        
+        self.execute_command(
+            command,
+            named_session=named_session,
+            wrap_in_screen=True
+        )
+
+    def list_named_sessions(self):
+
+        self.execute_command(f"screen -list")
+
+    def attach_named_session(self, named_session: str):
+
+        self.execute_command(f"screen -r -d {named_session}")
+
+    def kill_named_session(self, named_session: str):
+
+        self.execute_command(f"screen -X -S {named_session} quit")
+
+    def setup(
+        self,
+    ):
+
+        self.clear()
+
+class ReacherDocker(Reacher):
+
+    CON_WORKSPACE_PATH = "/workspace"
+
+    MOUNTED = [
+        Reacher.ARTIFACATS_PATH,
+        Reacher.LOGS_PATH
+    ]
+
+    def __init__(
+        self,
+        build_name: str,
+        image_name: str,
+        build_context: str,
+        client: RemoteClient = None,
+        host: str = None,
+        port: int = 22,
+        user: str = None,
+        password: str = None,
+        ssh_key_filepath: str = None
+    ):
+
+        super().__init__(
+            build_name=build_name,
+            client=client,
+            host=host,
+            port=port,
+            user=user,
+            password=password,
+            ssh_key_filepath=ssh_key_filepath
+        )
+
+        self._image_name = image_name
+        self._build_context = build_context 
+
+    def _setup_remote(self):
+
+        super()._setup_remote()
+
+        self._client.upload_dir(
+            self._build_context,
+            self.build_path,
+        )
+
+    def clear(self):
+
+        if self.is_running:
+            self._client.execute_command(
+                f"docker stop {self._build_name}", suppress=True,
+            )
+
+        if self.exists:
+            self._client.execute_command(
+                f"docker rm {self._build_name}", suppress=True,
+            )
+
+        super().clear()
+
     def build(self):
 
         self.clear()
 
         self._client.execute_command(
             f"docker build -t {self._build_name} {os.path.join(self.build_path, self._build_context)}",
             stream=True,
@@ -305,16 +426,15 @@
         stream: bool = True,
         suppress: bool = False,
         named_session: str = None,
         wrap_in_screen: bool = False,
     ):  
 
         if wrap_in_screen or named_session is not None:
-            named_session = named_session if named_session is not None else uuid.uuid4()
-            command = f"screen -S {named_session} {command}"
+            command = self._wrap_command_in_screen(command, named_session=named_session)
 
         command = f"docker exec -it {self._build_name} {command}"
 
         return self._client.execute_command(
             command,
             stream=stream,
             suppress=suppress,
@@ -365,31 +485,20 @@
             )
 
         self._client.execute_command(
             f"docker cp {tmp_path}/. {self._build_name}:/{Reacher.CON_WORKSPACE_PATH}"
         )
 
         self._client.execute_command(f"rm -r {tmp_path}")
-        
-        if file is not None:
-            command = command if command is not None else f"python {file}"
-        
-        self.execute_command(command, named_session=named_session, wrap_in_screen=True)
-
-    def list_named_sessions(self):
-
-        self.execute_command(f"screen -list")
-
-    def attach_named_session(self, named_session: str):
-
-        self.execute_command(f"screen -r -d {named_session}")
-
-    def kill_named_session(self, named_session: str):
 
-        self.execute_command(f"screen -X -S {named_session} quit")
+        self.execute_command(
+            command,
+            named_session=named_session,
+            wrap_in_screen=True
+        )
 
     def setup(
         self,
         ports: List[int] = None,
         envs: Dict[str, str] = None,
         command: str = "sleep infinity",
         gpu: bool = False,
@@ -400,27 +509,25 @@
         extra_args = ""
 
         if gpu:
             extra_args = "--runtime=nvidia --gpus all"
 
         ctx = f"docker run -dt {extra_args} -w {Reacher.CON_WORKSPACE_PATH} --name {self._build_name}"
 
-        ctx = f"{ctx} -v {self.artifact_path}:{Reacher.CON_WORKSPACE_PATH}/{Reacher.CON_ARTIFACATS_PATH}"
-        ctx = f"{ctx} -v  {self.log_path}:{Reacher.CON_WORKSPACE_PATH}/{Reacher.CON_LOGS_PATH}"
+        ctx = f"{ctx} -v {self.artifact_path}:{Reacher.CON_WORKSPACE_PATH}/{Reacher.ARTIFACATS_PATH}"
+        ctx = f"{ctx} -v  {self.log_path}:{Reacher.CON_WORKSPACE_PATH}/{Reacher.LOGS_PATH}"
 
         if ports is not None:
             for p in ports:
                 ctx = f"{ctx} -p {p}:{p}"
 
         if envs is not None:
             for k, v in envs.items():
                 ctx = f"{ctx} -e {k}={v}"
 
-        path = os.path.join(self.build_path, self._build_context, "logging-driver-config.json")
-
         ctx = f"{ctx} {self._image_name} {command}"
 
         self._client.execute_command(ctx)
 
         # Install screen in container
         self.execute_command(
             "apt-get -y install screen",
@@ -443,8 +550,117 @@
                 'docker ps -a --format {{.Names}}', suppress=True,
         ).replace("\r", "").split("\n")
 
         return self._build_name in r
 
     if __name__ == "__main__":
 
-        pass
+        pass
+
+class ForwardServer(SocketServer.ThreadingTCPServer):
+    daemon_threads = True
+    allow_reuse_address = True
+
+class Handler(SocketServer.BaseRequestHandler):
+    
+    def handle(self):
+        try:
+            chan = self.ssh_transport.open_channel(
+                "direct-tcpip",
+                (self.chain_host, self.chain_port),
+                self.request.getpeername(),
+            )
+        except Exception as e:
+            print(
+                "Incoming request to %s:%d failed: %s"
+                % (self.chain_host, self.chain_port, repr(e))
+            )
+            return
+        if chan is None:
+            print(
+                "Incoming request to %s:%d was rejected by the SSH server."
+                % (self.chain_host, self.chain_port)
+            )
+            return
+
+        print(
+            "Connected!  Tunnel open %r -> %r -> %r"
+            % (
+                self.request.getpeername(),
+                chan.getpeername(),
+                (self.chain_host, self.chain_port),
+            )
+        )
+        while True:
+            r, w, x = select.select([self.request, chan], [], [])
+            if self.request in r:
+                data = self.request.recv(1024)
+                if len(data) == 0:
+                    break
+                chan.send(data)
+            if chan in r:
+                data = chan.recv(1024)
+                if len(data) == 0:
+                    break
+                self.request.send(data)
+
+        peername = self.request.getpeername()
+        chan.close()
+        self.request.close()
+        print("Tunnel closed from %r" % (peername,))
+
+
+def forward_tunnel(local_port, remote_host, remote_port, transport):
+    # this is a little convoluted, but lets me configure things for the Handler
+    # object.  (SocketServer doesn't give Handlers any way to access the outer
+    # server normally.)
+    class SubHander(Handler):
+        chain_host = remote_host
+        chain_port = remote_port
+        ssh_transport = transport
+
+    ForwardServer(("", local_port), SubHander).serve_forever()
+    
+    
+import threading
+    
+class PortForwarding(object):
+    
+    def __init__(
+        self,
+        host: str = None,
+        user: str = None,
+        ssh_port: int = 22,
+        ssh_key_file_path: str = None,
+        password: str = None,
+        client: RemoteClient = None
+    ):
+        
+        if client is None:
+        
+            self._client = RemoteClient(
+                host=host,
+                user=user,
+                password=password,
+                ssh_key_file_path=ssh_key_file_path,
+                port=ssh_port,
+            )
+            
+        else:
+            
+            self._client = client
+
+        self._threads = []
+    
+    def add_port_forward(self, remote_port: int, local_port: int):
+        
+        transport = self._client.connection.get_transport()
+        
+        x = threading.Thread(
+            target=forward_tunnel,
+            args=(local_port, self._client.host, remote_port, transport),
+            daemon=True
+        )
+        
+        self._threads.append(x)
+        
+        self._threads[-1].start()
```

## Comparing `reacher-0.3.3.dist-info/METADATA` & `reacher-0.3.4.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,73 @@
 Metadata-Version: 2.1
 Name: reacher
-Version: 0.3.3
+Version: 0.3.4
 Summary: A tool for reaching out to remote machine - excecute code and collect artificats
 Home-page: https://github.com/johannes-skog/reacher
 Author: johannes skog
 Author-email: johannes.skog.unsec@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: scp
 Requires-Dist: paramiko
 
 # Reacher
 
-From your local machine, Reacher will,
+From your local machine, ReacherDocker will,
 
 + build a docker image on the remote (docker must already be installed and ssh enabled) according to specifications
 + set up container on the remote with port port-forwarding and enviroment variables 
 + execute your local code on the remote, in the container, with printouts shown as your were running it locally
 + upload/download files from the container to your local machine
 
+and for your local machine, Reacher will,
+
++ execute your local code on the remote, with printouts shown as your were running it locally
++ upload/download files from the remote to your local machine
 
 # Getting started...
 
 To get started,
 
 ```bash
 pip install reacher
 pip install python-dotenv
 ```
 
 First we must setup a connection to the remote, RemoteClient will create a ssh connection between the local and remote machine.
 
 ```python
-from reacher.reacher import Reacher, RemoteClient
+from reacher.reacher import Reacher, ReacherDocker, RemoteClient
 from dotenv import dotenv_values
 config = dotenv_values()  # take environment variables from .env.
 client = RemoteClient(
     host=config["HOST"],
     user=config["USER"],
     password=config["PASSWORD"],
     ssh_key_filepath=config["SSH_KEY_PATH"]
 )
 ```
 
-the connection is sent to Reacher together with the name of the image that we want to build and the name of the container.
+the connection is sent to ReacherDocker together with the name of the image that we want to build and the name of the container.
 
 ```python
-reacher = Reacher(
+reacher = ReacherDocker(
     client=client,
     build_name="base",
     image_name="base",
     build_context="dockercontext"
 )
 ```
 
 or send in the aruments for RemoteClient direcly to Reacher
 
 ```python
-reacher = Reacher(
+reacher = ReacherDocker(
     client=client,
     build_name="base",
     image_name="base",
     build_context="dockercontext",
     host=config["HOST"],
     user=config["USER"],
     password=config["PASSWORD"],
@@ -74,15 +78,15 @@
 build_context should contain everything for building the docker image on the remote. It might look like,
 
 ```bash
 $ ls dockercontext/
 Dockerfile  requirements.txt
 ```
 
-Once Reacher has been setup we can build the image on the remote. Reacher will send the build_context to the remote and
+Once ReacherDocker has been setup we can build the image on the remote. ReacherDocker will send the build_context to the remote and
 trigger docker to build an image according to the specifications in the Dockerfile
 
 ```python
 reacher.build()
 
 [+] Building 0.0s (0/1)                                                         
 [+] Building 0.2s (2/3)                                                         
@@ -96,14 +100,36 @@
 
 and thereafter we can setup the docker container. Reacher will make sure this container is running until we have explicitly deleted it.
 
 ```python
 reacher.setup(ports=[8888, 6666], envs=dotenv_values(".env"))
 ```
 
+If you want to execute the code direcly on the remote, not in a container, go for Reacher. Reacher will use the remote enviroment, as is, when executing the commands.
+
+```python
+reacher = Reacher(
+    build_name="base",
+    host=config["HOST"],
+    user=config["USER"],
+    password=config["PASSWORD"],
+    ssh_key_filepath=config["SSH_KEY_PATH"]
+)
+```
+
+# Port-forwarding between remote and local
+
+If you want to access some service on the remote, you can forward the traffic on the ports of the remote to the local machine.
+
+```python
+reacher.add_port_forward(remote_port=6006, local_port=5998)
+```
+
+this will spin of a seperate daemon thread handling the port-forwading.
+
 # Running code on the remote 
 
 ## Running a code-snippet 
 
 Now we have built the docker image on the remote and have a container ready to execute whatever code that we want to run.
 
 A "Hello World" test can be triggered from a notebook.
```

