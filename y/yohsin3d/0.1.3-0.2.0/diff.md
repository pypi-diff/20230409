# Comparing `tmp/yohsin3d-0.1.3.tar.gz` & `tmp/yohsin3d-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yohsin3d-0.1.3.tar", last modified: Wed Apr  5 23:35:39 2023, max compression
+gzip compressed data, was "yohsin3d-0.2.0.tar", last modified: Sun Apr  9 09:55:45 2023, max compression
```

## Comparing `yohsin3d-0.1.3.tar` & `yohsin3d-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:35:39.371183 yohsin3d-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-05 23:35:29.000000 yohsin3d-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-05 23:35:39.371183 yohsin3d-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-05 23:35:29.000000 yohsin3d-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 23:35:39.371183 yohsin3d-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-05 23:35:29.000000 yohsin3d-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:35:39.371183 yohsin3d-0.1.3/yohsin3d/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-05 23:35:29.000000 yohsin3d-0.1.3/yohsin3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:35:39.371183 yohsin3d-0.1.3/yohsin3d/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 23:35:29.000000 yohsin3d-0.1.3/yohsin3d/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-05 23:35:29.000000 yohsin3d-0.1.3/yohsin3d/core/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-05 23:35:29.000000 yohsin3d-0.1.3/yohsin3d/core/behavior.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:35:39.371183 yohsin3d-0.1.3/yohsin3d/core/body/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 23:35:29.000000 yohsin3d-0.1.3/yohsin3d/core/body/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-04-05 23:35:29.000000 yohsin3d-0.1.3/yohsin3d/core/body/body_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-04-05 23:35:29.000000 yohsin3d-0.1.3/yohsin3d/core/body/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-05 23:35:29.000000 yohsin3d-0.1.3/yohsin3d/core/body/nao_joint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:35:39.371183 yohsin3d-0.1.3/yohsin3d/core/network/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 23:35:29.000000 yohsin3d-0.1.3/yohsin3d/core/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-04-05 23:35:29.000000 yohsin3d-0.1.3/yohsin3d/core/network/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-05 23:35:29.000000 yohsin3d-0.1.3/yohsin3d/core/network/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:35:39.371183 yohsin3d-0.1.3/yohsin3d/core/world/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 23:35:29.000000 yohsin3d-0.1.3/yohsin3d/core/world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-05 23:35:29.000000 yohsin3d-0.1.3/yohsin3d/core/world/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-05 23:35:29.000000 yohsin3d-0.1.3/yohsin3d/core/world/world_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:35:39.371183 yohsin3d-0.1.3/yohsin3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-05 23:35:39.000000 yohsin3d-0.1.3/yohsin3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-05 23:35:39.000000 yohsin3d-0.1.3/yohsin3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 23:35:39.000000 yohsin3d-0.1.3/yohsin3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-05 23:35:39.000000 yohsin3d-0.1.3/yohsin3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.918965 yohsin3d-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-09 09:55:45.918965 yohsin3d-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 09:55:45.918965 yohsin3d-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.914965 yohsin3d-0.2.0/yohsin3d/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.914965 yohsin3d-0.2.0/yohsin3d/communicators/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/communicators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.914965 yohsin3d-0.2.0/yohsin3d/communicators/y3d_communicator/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/communicators/y3d_communicator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/communicators/y3d_communicator/bit_codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/communicators/y3d_communicator/communicator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.914965 yohsin3d-0.2.0/yohsin3d/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/behavior.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.914965 yohsin3d-0.2.0/yohsin3d/core/body/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/body/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/body/body_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/body/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/body/nao_joint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.918965 yohsin3d-0.2.0/yohsin3d/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/common/agent_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/common/ground_truth_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.918965 yohsin3d-0.2.0/yohsin3d/core/communicator/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/communicator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/communicator/base_communicator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.918965 yohsin3d-0.2.0/yohsin3d/core/localizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/localizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/localizer/base_localizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.918965 yohsin3d-0.2.0/yohsin3d/core/network/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/network/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/network/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/network/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.918965 yohsin3d-0.2.0/yohsin3d/core/world/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/world/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/core/world/world_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.918965 yohsin3d-0.2.0/yohsin3d/localizers/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/localizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-09 09:55:37.000000 yohsin3d-0.2.0/yohsin3d/localizers/ground_truth_localizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:55:45.914965 yohsin3d-0.2.0/yohsin3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-09 09:55:45.000000 yohsin3d-0.2.0/yohsin3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-09 09:55:45.000000 yohsin3d-0.2.0/yohsin3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 09:55:45.000000 yohsin3d-0.2.0/yohsin3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 09:55:45.000000 yohsin3d-0.2.0/yohsin3d.egg-info/top_level.txt
```

### Comparing `yohsin3d-0.1.3/LICENSE` & `yohsin3d-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yohsin3d-0.1.3/yohsin3d/core/agent.py` & `yohsin3d-0.2.0/yohsin3d/core/agent.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,57 @@
-from .network.server import Server
-from .behavior import Behavior
-import signal, sys, traceback
+import signal
+import sys
+import traceback
+
+from .network import Server
+from .body import AgentType
+from .behavior import BaseBehavior
 
 
 class Agent:
     def __init__(
         self,
         agent_num: int,
-        agent_type: int,
-        team_name: str = "FCYohsin",
+        team_name: str,
+        behavior: BaseBehavior,
+        agent_type: AgentType = 0,
         host_name: str = "localhost",
         global_port: int = 3100,
         monitor_port: int = 3200,
     ) -> None:
 
         self.team_name = team_name
         self.agent_num = agent_num
         self.agent_type = agent_type
+        self.spawned = False
 
-        self.nao_rsg = "rsg/agent/nao/nao.rsg" if agent_type == 0 else f"rsg/agent/nao/nao_hetero.rsg {agent_type}"
+        self.nao_rsg = "rsg/agent/nao/nao.rsg" if agent_type == AgentType.NAO else f"rsg/agent/nao/nao_hetero.rsg {int(agent_type)}"
 
         self.host_name = host_name
         self.agent_running = True
         self.global_port = global_port
         self.monitor_port = monitor_port
 
         self.global_socket = Server()
         self.monitor_socket = Server()
-        self.behavior: Behavior = Behavior(
-            team_name=self.team_name,
-            rsg=self.nao_rsg,
-            agent_type=self.agent_type,
-            agent_unum=self.agent_num,
-            start_coordinates=(0,0,0)
-        )
+        self.behavior: BaseBehavior = behavior
+        self.behavior.initialize(team_name)
 
     def done(self):
         self.global_socket.close()
         if self.monitor_port != -1:
             self.monitor_socket.close()
 
+    def setup_message(self):
+        print("Loading rsg: " + "(scene " + self.nao_rsg + ")")
+        return f"(scene {self.nao_rsg})"
+
+    def spawn_message(self):
+        return f"(init (unum {self.agent_num})(teamname {self.team_name}))"
+
     def run(self):
 
         behavior = self.behavior
         if behavior:
             try:
                 self.global_socket.connect(self.host_name, self.global_port)
                 if self.monitor_port != -1:
@@ -52,31 +60,38 @@
             except ConnectionRefusedError:
                 print("Connection Refused Error...")
                 print("Make sure you have the server running...")
                 self.done()
                 exit()
 
             print("Connection Established...")
-            self.global_socket.put_message(behavior.spawn_message())
+            self.global_socket.put_message(self.setup_message())
 
             while self.agent_running:
                 try:
                     msg_from_server = self.global_socket.get_message().decode('utf-8')
-                    msg_to_server = behavior.think(msg_from_server)
+                    msg_to_server = None
+                    if not self.spawned:
+                        msg_to_server = self.spawn_message()
+                        self.spawned = True
+                    else:
+                        msg_to_server = behavior.think(msg_from_server)
+
                     if msg_to_server is not None:
                         self.global_socket.put_message(msg_to_server)
                     if self.monitor_port != -1:
-                        self.monitor_socket.put_message(behavior.get_monitor_message())
+                        self.monitor_socket.put_message(
+                            behavior.get_monitor_message())
 
                 except Exception as e:
                     print(traceback.format_exc())
                     self.done()
                     exit()
 
     def start(self):
         def signal_handler(sig, _):
             print('\nExiting!')
             sys.exit(0)
 
         signal.signal(signal.SIGINT, signal_handler)
         self.run()
-        self.done()
+        self.done()
```

### Comparing `yohsin3d-0.1.3/yohsin3d/core/behavior.py` & `yohsin3d-0.2.0/yohsin3d/core/behavior.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,120 +1,125 @@
-from .body.body_model import *
-from .world.world_model import *
-from .network.parser import Parser
-
-class Behavior:
-
-    def __init__(self, team_name: str, rsg: str, agent_unum, agent_type, start_coordinates) -> None:
-        self.rsg = rsg
-        self.team_name = team_name
-        self.agent_unum = agent_unum
-        self.start_coordinates = start_coordinates
+from .body import *
+from .world import *
+from .localizer import BaseLocalizer
+from .network import Parser
+from .communicator import BaseCommunicator
+from .common import AgentLocation
 
+
+class BaseBehavior:
+
+    def __init__(self, beam_location: AgentLocation, localizer: BaseLocalizer = None, communicator: BaseCommunicator = None) -> None:
+        self.beam_location = beam_location
         self.monitor_msg = ""
-        self.spawn_init = False
         self.initialized = False
         self.init_beamed = False
-        self.respawning = False
+        self.localizer: BaseLocalizer = localizer
+        self.communicator: BaseCommunicator = communicator
 
-        self.world_model = WorldModel()
+    def initialize(self, team_name):
+        self.world_model = WorldModel(team_name)
         self.body_model = BodyModel(self.world_model)
 
         self.parser = Parser(world_model=self.world_model,
-                             body_model=self.body_model)
+                             body_model=self.body_model,
+                             communicator=self.communicator                             
+                             )
+        
+        
+        if self.communicator is not None:
+            self.communicator.initialize(self.world_model, self.localizer)
 
-    def spawn_message(self):
-        print("Loading rsg: " + "(scene " + self.rsg + ")")
-        return f"(scene {self.rsg})"
+        if self.localizer is not None:
+            self.localizer.initialize(self.world_model)
 
-    def beamable_playmode(self):
+    def can_rebeam(self):
         pm = self.world_model.get_playmode()
-        return pm == PlayModes.PM_BEFORE_KICK_OFF or pm == PlayModes.PM_GOAL_LEFT or pm == PlayModes.PM_GOAL_RIGHT
-
+        last_pm = self.world_model.get_last_playmode()
+        beamable_modes = [
+            PlayModes.BEFORE_KICK_OFF,
+            PlayModes.GOAL_LEFT,
+            PlayModes.GOAL_RIGHT,
+        ]
+        return pm in beamable_modes and pm != last_pm
 
     def beam_effector(self, x, y, z):
         return f"(beam {x} {y} {z})"
 
     def init_beam_effector(self):
-        x, y, z = self.start_coordinates
-        return self.beam_effector(x, y, z)
+        x, y = self.beam_location.position
+        return self.beam_effector(x, y, self.beam_location.orientation)
 
     def hj_effector(self, name, rate):
         return "({} {:.2f})".format(name, rate)
 
     def compose_action(self):
         message = ""
         for effector in EffectorJoints:
             torque = self.body_model.compute_torque(effector)
             effector_name = effector.to_string()
             message += self.hj_effector(effector_name, torque)
 
+        if self.communicator is not None:
+            message += self.communicator.make_say_message()
+
         return message
 
     def get_monitor_message(self):
         ret = self.monitor_msg
         self.monitor_msg = ""
         return ret
 
     def set_monitor_message(self, msg):
         self.monitor_msg = msg
 
-    def respawn(self):
-        self.init_beamed = False
-        self.initialized = False
-
     def initialize_body(self):
         self.body_model.set_initial_arm(BodyParts.ARM_LEFT)
         self.body_model.set_initial_arm(BodyParts.ARM_RIGHT)
         self.body_model.set_initial_leg(BodyParts.LEG_LEFT)
         self.body_model.set_initial_leg(BodyParts.LEG_RIGHT)
         self.body_model.set_initial_head()
 
-    def spawn_nao(self):
-        self.time_when_spawned = (self.world_model.get_time())
-        self.spawn_init = True
-        msg = "(playMode BeforeKickOff)"
-        self.set_monitor_message(msg)
-        return f"(init (unum {self.agent_unum})(teamname {self.team_name}))"
+    def __can_initialize(self):
+        return self.world_model.is_my_number_set() and self.world_model.is_side_set()
 
     def initialize_nao(self):
-        
-        if not self.world_model.get_unum_set(
-        ) or not self.world_model.get_side_set():
-            return None
 
         if not self.init_beamed:
             self.init_beamed = True
             return self.init_beam_effector()
-        else:
-            self.initialized = True
-            return None
 
+        if not self.__can_initialize() or self.initialized:
+            return
 
+        self.initialize_body()
+        self.initialized = True
+        return None
+    
     def think(self, message: str) -> str:
 
         parse_success = self.parser.parse(message)
-
         if not parse_success:
             print("Parser failed to parse message..")
 
-        if not self.spawn_init:
-            return self.spawn_nao()
+        message = self.initialize_nao()
+        if message is not None:
+            return message
+
+        if self.can_rebeam():
+            self.init_beamed = False
+
+        if self.localizer is not None:
+            self.localizer.update()
 
-        if not self.initialized:
-            message = self.initialize_nao()
-            if message is not None:
-                return message
-
-        if self.respawning:
-            self.respawning = False
-            self.respawn()
-        
         action = ""
         self.act()
-        action += self.compose_action()
 
+        if self.communicator is not None:
+            self.communicator.say()
+            self.communicator.hear()
+            
+        action += self.compose_action()
         return action
 
     def act(self):
-       pass
-    
+        raise NotImplementedError
```

### Comparing `yohsin3d-0.1.3/yohsin3d/core/body/body_model.py` & `yohsin3d-0.2.0/yohsin3d/core/body/body_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         if (arm == BodyParts.ARM_LEFT):
 
             self.set_target_angle(EffectorJoints.EFF_LA1, ang1)
             self.set_target_angle(EffectorJoints.EFF_LA2, ang2)
             self.set_target_angle(EffectorJoints.EFF_LA3, ang3)
             self.set_target_angle(EffectorJoints.EFF_LA4, ang4)
 
-        else:  # ARM_RIGHT
+        else:
 
             self.set_target_angle(EffectorJoints.EFF_RA1, ang1)
             self.set_target_angle(EffectorJoints.EFF_RA2, -ang2)
             self.set_target_angle(EffectorJoints.EFF_RA3, -ang3)
             self.set_target_angle(EffectorJoints.EFF_RA4, -ang4)
 
     def set_initial_leg(self, leg) -> bool:
@@ -158,8 +158,8 @@
             angle = effector.min_angle
 
         if abs(angle - current_angle) < effector.error_tolerance:
             return 0
         elif current_angle < angle:
             return math.radians(abs(angle - current_angle)) * gain
         elif current_angle > angle:
-            return -math.radians(abs(angle - current_angle)) * gain
+            return -math.radians(abs(angle - current_angle)) * gain
```

### Comparing `yohsin3d-0.1.3/yohsin3d/core/body/nao_joint.py` & `yohsin3d-0.2.0/yohsin3d/core/body/nao_joint.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,21 +11,20 @@
         self.current_angle = 0
         self.target_angle = 0
 
         self.error_tolerance = error_tolerance
 
         self.scale = 1.0
 
-
     def set_target_angle(self, angle):
 
         if (angle < self.min_angle):
             self.target_angle = self.min_angle
 
         elif (angle > self.max_angle):
             self.target_angle = self.max_angle
 
         else:
             self.target_angle = angle
 
     def update(self, angle):
-        self.current_angle = angle
+        self.current_angle = angle
```

### Comparing `yohsin3d-0.1.3/yohsin3d/core/network/parser.py` & `yohsin3d-0.2.0/yohsin3d/core/network/parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,81 +1,82 @@
 import re
 from typing import List
-from ..body.body_model import *
-from ..world.world_model import *
+from ..body import *
+from ..world import *
+from ..communicator import *
+from .constants import *
+
 
 class Parser:
 
     def __init__(self,
-                 world_model=None,
-                 body_model=None,
-                 team_name="test") -> None:
+                 world_model,
+                 body_model,
+                 communicator,
+                 ) -> None:
 
         self.world_model: WorldModel = world_model
         self.body_model: BodyModel = body_model
-        self.side = SIDE_LEFT
-        self.team_name = team_name
-
+        self.communicator: BaseCommunicator = communicator
+        
+        self.side = Sides.LEFT
 
     def tokenise(self, s) -> List[str]:
         string = re.sub(r'[\(\)]', ' ', s)
         result = re.split(r'\s+', string.strip())
         return result
 
     def __parser_helper(self, matching_string, string):
         match = re.search(fr'{matching_string}\s+([^\)\]]+)', string)
         if match:
             return match.group(1)
 
-
     def __parse_time(self, string):
         time = float(self.__parser_helper("now", string))
         self.world_model.set_time(time)
         self.world_model.increment_cycle()
         return time is not None
 
     def __parse_game_state(self, string):
 
         playmode_string = self.__parser_helper("pm", string)
-        playmode = playModeStringToEnum.get(playmode_string, None)
+        playmode = PlayModes(playmode_string)
+        self.world_model.set_last_playmode(self.world_model.get_playmode())
         self.world_model.set_playmode(playmode)
 
         gametime = float(self.__parser_helper("t", string))
         self.world_model.set_gametime(gametime)
 
-        if self.world_model.get_unum() is None:
+        if self.world_model.get_my_number() is None:
             unum = (self.__parser_helper("unum", string))
-            self.world_model.set_unum(int(unum) if unum else None)
-            self.world_model.set_unum_set(True)
+            self.world_model.set_my_number(int(unum) if unum else None)
 
         score_left = int(self.__parser_helper("sl", string))
         self.world_model.set_score_left(score_left)
 
         score_right = int(self.__parser_helper("sr", string))
         self.world_model.set_score_right(score_right)
 
-        if not self.world_model.get_side_set():
+        if not self.world_model.is_side_set():
             side = self.__parser_helper("team", string)
             if side is not None:
-                self.world_model.set_side(SIDE_LEFT if side == "left" else SIDE_RIGHT)
-                self.world_model.set_side_set(True)
+                self.world_model.set_side(
+                    Sides.LEFT if side == "left" else Sides.RIGHT)
 
         return True
 
-
     def __parse_gyro(self, string):
         rateX, rateY, rateZ = self.__get_xyz(string, "rt")
         self.body_model.set_gyro_rates((rateX, rateY, rateZ))
         return True
 
     def __get_xyz(self, string, start):
         x, y, z = self.__parser_helper(start, string).split()
         return float(x), float(y), float(z)
 
-
     def __parse_accelerometer(self, string):
         rateX, rateY, rateZ = self.__get_xyz(string, "a")
 
         #  Sometimes spurious (very high or NaN) readings come through. Clip them.
         spuriousThreshold = 20.0
         if ((abs(rateX) > spuriousThreshold)):
             rateX = 0
@@ -94,237 +95,273 @@
         #  Apply filter to raw accelerometer data
         K = 0.9
         lastAccel = self.body_model.get_accel_rates()
         correctedRateX = K * lastAccel[0] + (1 - K) * correctedRateX
         correctedRateY = K * lastAccel[1] + (1 - K) * correctedRateY
         correctedRateZ = K * lastAccel[2] + (1 - K) * correctedRateZ
 
-        self.body_model.set_accel_rates((correctedRateX, correctedRateY, correctedRateZ))
-
+        self.body_model.set_accel_rates(
+            (correctedRateX, correctedRateY, correctedRateZ))
 
     def __segment(self, string):
         return re.findall(r'\(([^()]*(?:\(([^()]*(?:\((?:[^()]*(?:\([^()]*\)[^()]*)*)\)[^()]*)*)\)[^()]*)*)\)', string)
 
-
     def __parse_hinge_joint(self, string):
         effector_name = joint_to_effector[self.__parser_helper("n", string)]
         effector_angle = float(self.__parser_helper("ax", string))
-        
+
         self.body_model.set_current_angle(effector_name, effector_angle)
         return True
 
-
     def __parse_FRP(self, str):
         name = self.__parser_helper("n", str)
         centreX, centreY, centreZ = self.__get_xyz(str, "c")
         forceX, forceY, forceZ = self.__get_xyz(str, "f")
-        self.world_model.force_resistance_perceptors[name] = [(centreX, centreY, centreZ),(forceX, forceY, forceZ)]
+        name = ForceResistancePerceptors(name)
+        self.world_model.force_resistance_perceptors[name] = [
+            (centreX, centreY, centreZ), (forceX, forceY, forceZ)]
         return True
 
     def __get_first(self, string):
         return re.search(r'^[^( ]+', string).group(0)
 
-
     def __parse_simple_vision_object(self, string):
         name = self.__get_first(string)
         x, y, z = self.__get_xyz(string, "pol")
+        name = VisibleObjects(name)
         self.world_model.simple_vision_objects[name] = (x, y, z)
         return True
 
-
-
     def __parse_line(self, string):
-
         '''
         Parse Line is not complete yet. There are multiple lines data coming from the server. We need to figure out how to 
         process that. 
-        
+
         TODO: Need to undderstand the concept of the lines
         '''
         tokens = self.tokenise(string)
 
         r = float(tokens[2])
         theta = float(tokens[3])
         phi = float(tokens[4])
 
         r2 = float(tokens[6])
         theta2 = float(tokens[7])
         phi2 = float(tokens[8])
 
-        self.world_model.complex_vision_objects['L'] = [(r, theta, phi), (r2, theta2, phi2)]
+        self.world_model.lines = [(r, theta, phi), (r2, theta2, phi2)]
         return True
 
-
     def __parse_player(self, string):
 
         valid = False
 
         tokens = self.tokenise(string)
-        valid = (len(tokens) == 30) # based on the assumption that the max characters in a team name will be 100
+        # based on the assumption that the max characters in a team name will be 100
+        valid = (len(tokens) == 30)
 
         if valid:
             agent_num = (tokens[4]).zfill(2)
             team_name = tokens[2]
 
-            player_info = {
-                    "head" : (float(tokens[7]), float(tokens[8]), float(tokens[9])),
-                    "rlowerarm" : (float(tokens[12]), float(tokens[13]), float(tokens[14])),
-                    "llowerarm" : (float(tokens[17]), float(tokens[18]), float(tokens[19])),
-                    "rfoot" : (float(tokens[22]), float(tokens[23]), float(tokens[24])),
-                    "lfoot" : (float(tokens[27]), float(tokens[28]), float(tokens[29]))
-                }
+            agent_num = int(agent_num)
 
-            if team_name == "FC-Yohsin":
-                self.world_model.complex_vision_objects[f"Yohsin{agent_num}"] = player_info
+            player_info = {
+                "head": (float(tokens[7]), float(tokens[8]), float(tokens[9])),
+                "rlowerarm": (float(tokens[12]), float(tokens[13]), float(tokens[14])),
+                "llowerarm": (float(tokens[17]), float(tokens[18]), float(tokens[19])),
+                "rfoot": (float(tokens[22]), float(tokens[23]), float(tokens[24])),
+                "lfoot": (float(tokens[27]), float(tokens[28]), float(tokens[29]))
+            }
+
+            if team_name == self.world_model.my_team_name:
+                self.world_model.teammate_info[agent_num].is_visible = True
+                self.world_model.teammate_info[agent_num].update_from_dict(player_info)
             else:
-                self.world_model.complex_vision_objects[f"Opponent{agent_num}"] = player_info
+                self.world_model.opponent_info[agent_num].is_visible = True
+                self.world_model.opponent_info[agent_num].update_from_dict(player_info)
 
         return valid
 
-
     def __reset_simple_non_visible_objects(self, string):
-        '''
-        This method resets the objects to None if they are not visible to the agent based on our latest message from the server
-        '''
-
-        for object in self.world_model.simple_vision_objects.keys():
-            if not re.search(f"[(]{object}\s", string):
+        for object in VisibleObjects:
+            if not re.search(f"[(]{object.value}\s", string):
                 self.world_model.simple_vision_objects[object] = None
 
-
-    def __reset_complex_non_visible_objects(self, string):
-        '''
-        This method resets the objects to None if they are not visible to the agent based on our latest message from the server
-        '''
-
-        for object in self.world_model.complex_vision_objects.keys():
-
-            if "FC-Yohsin" in object:
-                if not re.search(f"\(P\s\(team\sFC-Yohsin\s[(]id\s{int(object[len(object)-2:])}\)", string):
-                    self.world_model.complex_vision_objects[object] = None
-            elif "Opponent" in object:
-                if not re.search(f"\(P\s\(team\s.{1,100}\)\s\(id\s{int(object[len(object)-2:])}", string):
-                    self.world_model.complex_vision_objects[object] = None
-            else:
-                if not re.search("\(L\s", string):
-                    self.world_model.complex_vision_objects["L"] : None
-
-
-
-
+    def __is_player_visible(self, string, num, team):
+        regex = f"\(P\s+\(team\s+{team}\)\s+\(id\s+{num}\)"
+        return re.search(regex, string) is not None
+
+    def __reset_player_information(self, string):
+        for object in self.world_model.teammate_info.keys():
+            if not self.__is_player_visible(string, object, self.world_model.my_team_name):
+                self.world_model.teammate_info[object].is_visible = False
+
+        for object in self.world_model.opponent_info.keys():
+            if not self.__is_player_visible(string, object, self.world_model.opponent_team_name):
+                self.world_model.opponent_info[object].is_visible = False
 
     def __parse_position_groundtruth(self, string):
         tokens = self.tokenise(string)
-        self.world_model.set_position_groundtruth((float(tokens[1]), float(tokens[2]), float(tokens[3])))
+        self.world_model.set_position_groundtruth(
+            (float(tokens[1]), float(tokens[2]), float(tokens[3])))
 
     def __parse_orientation_groundtruth(self, string):
         tokens = self.tokenise(string)
         self.world_model.set_orientation_groundtruth(float(tokens[1]))
 
     def __parse_ball_position_groundtruth(self, string):
         tokens = self.tokenise(string)
-        self.world_model.set_ball_position_groundtruth((float(tokens[1]), float(tokens[2]), float(tokens[3])))
+        self.world_model.set_ball_position_groundtruth(
+            (float(tokens[1]), float(tokens[2]), float(tokens[3])))
 
     def __parse_see(self, string):
         valid = True
 
         self.__reset_simple_non_visible_objects(string=string)
-        self.__reset_complex_non_visible_objects(string=string)
+        self.__reset_player_information(string=string)
 
         str_segments = self.__segment(string)
 
         for segment in str_segments:
-            segment:str = segment[0].strip()
+            segment: str = segment[0].strip()
 
             # Goalpost
-            if(segment[0] == 'G'):
+            if (segment[0] == 'G'):
                 valid = self.__parse_simple_vision_object(segment) and valid
 
             # Flags
-            elif(segment[0] == 'F'):
+            elif (segment[0] == 'F'):
                 valid = self.__parse_simple_vision_object(segment) and valid
 
             # Ball
-            elif(segment[0] == 'B'):
+            elif (segment[0] == 'B'):
                 valid = self.__parse_simple_vision_object(segment) and valid
 
             # Player
-            elif(segment[0]== 'P'):
+            elif (segment[0] == 'P'):
                 self.__parse_player(segment)
 
             # My Position and My Orientation (Ground Truth)
-            elif (segment[0]== 'm'):
-                if (segment[:6].strip()== 'mypos'):
+            elif (segment[0] == 'm'):
+                if (segment[:6].strip() == 'mypos'):
                     self.__parse_position_groundtruth(segment)
 
                 if (segment[:8].strip() == 'myorien'):
                     self.__parse_orientation_groundtruth(segment)
 
-
             # GroundTruth Ball Position
-            elif (segment[0]== 'b'):
+            elif (segment[0] == 'b'):
                 if (segment[:8].strip() == 'ballpos'):
                     self.__parse_ball_position_groundtruth(segment)
 
             # See token (ignore)
-            elif  (segment[0]== 'S'):
+            elif (segment[0] == 'S'):
                 pass
 
             # Line
-            elif (segment[0] == 'L' ):
+            elif (segment[0] == 'L'):
                 valid = self.__parse_line(segment)
 
             else:
                 valid = False
 
-
         return valid
+    
 
 
+    def __parse_hear(self: 'Parser', string):
+
+        tokens = self.tokenise(string)
+        valid = False
+
+        heard_time = 0.0
+        is_self = False
+        message = ""
+
+        valid = len(tokens) == 5
+
+    
+        if not valid:
+            return valid
+
+        i = 1
+
+        if len(tokens) == 5:
+            team = tokens[i]
+            i+=1
+            if team != self.world_model.my_team_name:
+                self.world_model.opponent_team_name = team
+                return True
+
+        heard_time = float(tokens[i])
+
+        if tokens[i + 1] == "self":
+            is_self = True
+        else:
+            is_self = False
+        
+        i += 2
+
+        if i >= len(tokens):
+            return False
+
+        message = tokens[i]
+        delta_game_time = self.world_model.get_time() - self.world_model.get_gametime()
+        hear_game_time = heard_time + delta_game_time
+        orientation = tokens[3]
+
+        self.communicator.heard_message.update(
+            message=message,
+            heard_time=hear_game_time, 
+            team_name=team,
+            voice_orientation=orientation
+            )
+   
+        return valid
 
     def parse(self, string):
+
         valid = True
 
         inputSegments = self.__segment(string)
 
         for segment in inputSegments:
             segment: str = segment[0].strip()
 
             # Time
-            if (segment[0]== 't'):
+            if (segment[0] == 't'):
                 valid = self.__parse_time(segment) and valid
 
-
-            elif(segment[0] == 'G'):
+            elif (segment[0] == 'G'):
                 # GameState
-                if(segment[1] == 'S'):
+                if (segment[1] == 'S'):
                     valid = self.__parse_game_state(segment) and valid
 
                 # Gyro
                 else:
                     valid = self.__parse_gyro(segment) and valid
 
             # Hear #TODO
-            elif(segment[0] == 'h'):
-                pass
+            elif (segment[0] == 'h'):
+                valid = self.__parse_hear(segment) and valid
 
             # Hinge Joint
-            elif(segment[0] == 'H'):
+            elif (segment[0] == 'H'):
                 valid = self.__parse_hinge_joint(segment) and valid
 
-
             # See
-            elif(segment[0] == 'S'):
+            elif (segment[0] == 'S'):
                 valid = self.__parse_see(segment)
 
             # FRP
-            elif(segment[0] == 'F'):
+            elif (segment[0] == 'F'):
                 valid = self.__parse_FRP(segment) and valid
 
             # Accelerometer
-            elif(segment[0] == 'A'):
+            elif (segment[0] == 'A'):
                 valid = self.__parse_accelerometer(segment) and valid
 
             else:
                 valid = False
 
-        return True
+        return True
```

### Comparing `yohsin3d-0.1.3/yohsin3d/core/network/server.py` & `yohsin3d-0.2.0/yohsin3d/core/network/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-import struct, socket
-INT_SIZE = 4
+import struct
+import socket
+from .constants import *
+
 
 class Server:
     def __init__(self) -> None:
-        self.socket: socket.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        self.socket: socket.socket = socket.socket(
+            socket.AF_INET, socket.SOCK_STREAM)
 
     def connect(self, host, port):
         self.socket.connect((host, port))
 
     def recieve_message(self, length):
         buffer = b''
         bytesRead = 0
@@ -17,20 +20,20 @@
             buffer += nextBytes
 
         return buffer
 
     def get_message(self):
         length = struct.unpack("!I", self.recieve_message(INT_SIZE))[0]
         buffer = self.recieve_message(length)
-        return buffer 
+        return buffer
 
     def put_message(self, message: str):
         if len(message.strip()) == 0:
             return
-        
+
         # convert message to ASCII encoded byte string
         length = len(message)
         bmessage = bytes(message, 'ASCII')
 
         # send length of message
         lengthMessage = struct.pack("!I", length)
         bytesSent = 0
@@ -38,10 +41,9 @@
             bytesSent += self.socket.send(lengthMessage[bytesSent:])
 
         # send actual message
         bytesSent = 0
         while (bytesSent < length):
             bytesSent += self.socket.send(bmessage[bytesSent:])
 
-
     def close(self):
-        self.socket.close()
+        self.socket.close()
```

