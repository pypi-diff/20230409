# Comparing `tmp/python-switchbot-2.3.0.tar.gz` & `tmp/python-switchbot-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-switchbot-2.3.0.tar", last modified: Mon Mar 27 09:30:00 2023, max compression
+gzip compressed data, was "python-switchbot-2.3.1.tar", last modified: Sun Apr  9 05:36:36 2023, max compression
```

## Comparing `python-switchbot-2.3.0.tar` & `python-switchbot-2.3.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 09:30:00.653019 python-switchbot-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-27 09:29:52.000000 python-switchbot-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-03-27 09:30:00.653019 python-switchbot-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-03-27 09:29:52.000000 python-switchbot-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-27 09:29:52.000000 python-switchbot-2.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 09:30:00.653019 python-switchbot-2.3.0/python_switchbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-03-27 09:30:00.000000 python-switchbot-2.3.0/python_switchbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-27 09:30:00.000000 python-switchbot-2.3.0/python_switchbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 09:30:00.000000 python-switchbot-2.3.0/python_switchbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-27 09:30:00.000000 python-switchbot-2.3.0/python_switchbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-27 09:30:00.000000 python-switchbot-2.3.0/python_switchbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-27 09:30:00.653019 python-switchbot-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 09:29:52.000000 python-switchbot-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 09:30:00.653019 python-switchbot-2.3.0/switchbot/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-03-27 09:29:52.000000 python-switchbot-2.3.0/switchbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-03-27 09:29:52.000000 python-switchbot-2.3.0/switchbot/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-03-27 09:29:52.000000 python-switchbot-2.3.0/switchbot/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-03-27 09:29:52.000000 python-switchbot-2.3.0/switchbot/remotes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 05:36:36.434328 python-switchbot-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-09 05:36:27.000000 python-switchbot-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-09 05:36:36.434328 python-switchbot-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-09 05:36:27.000000 python-switchbot-2.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-09 05:36:27.000000 python-switchbot-2.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 05:36:36.430328 python-switchbot-2.3.1/python_switchbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-09 05:36:36.000000 python-switchbot-2.3.1/python_switchbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-09 05:36:36.000000 python-switchbot-2.3.1/python_switchbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 05:36:36.000000 python-switchbot-2.3.1/python_switchbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-09 05:36:36.000000 python-switchbot-2.3.1/python_switchbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 05:36:36.000000 python-switchbot-2.3.1/python_switchbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-09 05:36:36.434328 python-switchbot-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 05:36:27.000000 python-switchbot-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 05:36:36.434328 python-switchbot-2.3.1/switchbot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-09 05:36:27.000000 python-switchbot-2.3.1/switchbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-09 05:36:27.000000 python-switchbot-2.3.1/switchbot/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-09 05:36:27.000000 python-switchbot-2.3.1/switchbot/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-09 05:36:27.000000 python-switchbot-2.3.1/switchbot/remotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-09 05:36:27.000000 python-switchbot-2.3.1/switchbot/scene.py
```

### Comparing `python-switchbot-2.3.0/LICENSE` & `python-switchbot-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-switchbot-2.3.0/PKG-INFO` & `python-switchbot-2.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-switchbot
-Version: 2.3.0
+Version: 2.3.1
 Summary: A Python library to control SwitchBot devices connected to SwitchBot Hub
 Home-page: https://github.com/jonghwanhyeon/python-switchbot
 Author: Jonghwan Hyeon
 Author-email: jonghwanhyeon93@gmail.com
 License: MIT
 Keywords: switchbot
 Classifier: Development Status :: 4 - Beta
@@ -93,7 +93,21 @@
 # To send supported commands,
 remote.command('swing')
 remote.command('low_speed')
 
 # To send custom commands,
 remote.command('MyCustomCommand', customize=True)
 ```
+
+### Scenes
+```python
+# To list all infra red remotes
+scenes = switchbot.scenes()
+for scene in scenes:
+    print(scene)
+
+# If you already know a remote id:
+scene = switchbot.scene(id='')
+
+# To execute scene
+scene.execute()
+```
```

### Comparing `python-switchbot-2.3.0/README.md` & `python-switchbot-2.3.1/python_switchbot.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: python-switchbot
+Version: 2.3.1
+Summary: A Python library to control SwitchBot devices connected to SwitchBot Hub
+Home-page: https://github.com/jonghwanhyeon/python-switchbot
+Author: Jonghwan Hyeon
+Author-email: jonghwanhyeon93@gmail.com
+License: MIT
+Keywords: switchbot
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Home Automation
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # python-switchbot
 A Python library to control SwitchBot devices connected to SwitchBot Hub
 
 ## Requirements
 - Python 3.7+
 - [A SwitchBot Token](https://github.com/OpenWonderLabs/SwitchBotAPI#getting-started)
 
@@ -75,7 +93,21 @@
 # To send supported commands,
 remote.command('swing')
 remote.command('low_speed')
 
 # To send custom commands,
 remote.command('MyCustomCommand', customize=True)
 ```
+
+### Scenes
+```python
+# To list all infra red remotes
+scenes = switchbot.scenes()
+for scene in scenes:
+    print(scene)
+
+# If you already know a remote id:
+scene = switchbot.scene(id='')
+
+# To execute scene
+scene.execute()
+```
```

### Comparing `python-switchbot-2.3.0/setup.cfg` & `python-switchbot-2.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-switchbot-2.3.0/switchbot/__init__.py` & `python-switchbot-2.3.1/switchbot/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import uuid
 from typing import List
 
 from switchbot.client import SwitchBotClient
 from switchbot.devices import Device
 from switchbot.remotes import Remote
+from switchbot.scene import Scene
 
-__version__ = "2.3.0"
+__version__ = "2.3.1"
 
 
 class SwitchBot:
     def __init__(self, token: str, secret: str):
         self.client = SwitchBotClient(token, secret, nonce=str(uuid.uuid4()))
 
     def devices(self) -> List[Device]:
@@ -37,7 +38,17 @@
         ]
 
     def remote(self, id: str) -> Remote:
         for remote in self.remotes():
             if remote.id == id:
                 return remote
         raise ValueError(f"Unknown remote {id}")
+
+    def scenes(self) -> List[Scene]:
+        response = self.client.get("scenes")
+        return [Scene(client=self.client, id=scene["scene_id"], **scene) for scene in response["body"]]
+
+    def scene(self, id: str) -> Scene:
+        for scene in self.scenes():
+            if scene.id == id:
+                return scene
+        raise ValueError(f"Unknown scene {id}")
```

### Comparing `python-switchbot-2.3.0/switchbot/client.py` & `python-switchbot-2.3.1/switchbot/client.py`

 * *Files identical despite different names*

### Comparing `python-switchbot-2.3.0/switchbot/devices.py` & `python-switchbot-2.3.1/switchbot/devices.py`

 * *Files identical despite different names*

### Comparing `python-switchbot-2.3.0/switchbot/remotes.py` & `python-switchbot-2.3.1/switchbot/remotes.py`

 * *Files identical despite different names*

