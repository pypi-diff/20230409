# Comparing `tmp/pyevsim-1.1.4.tar.gz` & `tmp/pyevsim-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyevsim-1.1.4.tar", last modified: Tue Nov  8 07:33:18 2022, max compression
+gzip compressed data, was "pyevsim-1.1.5.tar", last modified: Sun Apr  9 09:11:01 2023, max compression
```

## Comparing `pyevsim-1.1.4.tar` & `pyevsim-1.1.5.tar`

### file list

```diff
@@ -1,29 +1,24 @@
-drwxrwxr-x   0 cbchoi    (1000) cbchoi    (1000)        0 2022-11-08 07:33:18.181221 pyevsim-1.1.4/
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)     1070 2022-11-05 06:02:07.000000 pyevsim-1.1.4/LICENSE
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)      512 2022-11-08 07:33:18.181221 pyevsim-1.1.4/PKG-INFO
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)       55 2022-11-05 06:02:07.000000 pyevsim-1.1.4/README.md
-drwxrwxr-x   0 cbchoi    (1000) cbchoi    (1000)        0 2022-11-08 07:33:18.171221 pyevsim-1.1.4/examples/
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)        0 2022-11-05 06:02:07.000000 pyevsim-1.1.4/examples/__init__.py
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)     2219 2022-11-05 06:02:07.000000 pyevsim-1.1.4/examples/model_relay.py
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)     1592 2022-11-05 06:02:07.000000 pyevsim-1.1.4/examples/multi_thread.py
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)     1195 2022-11-05 06:02:07.000000 pyevsim-1.1.4/examples/periodic_exec.py
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)     2126 2022-11-05 06:02:07.000000 pyevsim-1.1.4/examples/port_example.py
-drwxrwxr-x   0 cbchoi    (1000) cbchoi    (1000)        0 2022-11-08 07:33:18.178221 pyevsim-1.1.4/pyevsim/
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)     1899 2022-11-05 06:02:07.000000 pyevsim-1.1.4/pyevsim/__init__.py
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)     3562 2022-11-05 06:02:07.000000 pyevsim-1.1.4/pyevsim/behavior_model.py
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)     2395 2022-11-05 06:02:07.000000 pyevsim-1.1.4/pyevsim/behavior_model_executor.py
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)      585 2022-11-05 06:02:07.000000 pyevsim-1.1.4/pyevsim/default_message_catcher.py
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)     2413 2022-11-05 06:02:07.000000 pyevsim-1.1.4/pyevsim/definition.py
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)     1749 2022-11-05 06:02:07.000000 pyevsim-1.1.4/pyevsim/structural_model.py
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)    14311 2022-11-08 07:29:06.000000 pyevsim-1.1.4/pyevsim/system_executor.py
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)      808 2022-11-05 06:02:07.000000 pyevsim-1.1.4/pyevsim/system_message.py
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)      701 2022-11-05 06:02:07.000000 pyevsim-1.1.4/pyevsim/system_object.py
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)     1471 2022-11-05 06:02:07.000000 pyevsim-1.1.4/pyevsim/system_simulator.py
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)      504 2022-11-05 06:02:07.000000 pyevsim-1.1.4/pyevsim/termination_manager.py
-drwxrwxr-x   0 cbchoi    (1000) cbchoi    (1000)        0 2022-11-08 07:33:18.180221 pyevsim-1.1.4/pyevsim.egg-info/
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)      512 2022-11-08 07:33:18.000000 pyevsim-1.1.4/pyevsim.egg-info/PKG-INFO
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)      574 2022-11-08 07:33:18.000000 pyevsim-1.1.4/pyevsim.egg-info/SOURCES.txt
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)        1 2022-11-08 07:33:18.000000 pyevsim-1.1.4/pyevsim.egg-info/dependency_links.txt
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)       17 2022-11-08 07:33:18.000000 pyevsim-1.1.4/pyevsim.egg-info/top_level.txt
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)       38 2022-11-08 07:33:18.182221 pyevsim-1.1.4/setup.cfg
--rw-rw-r--   0 cbchoi    (1000) cbchoi    (1000)      579 2022-11-08 07:32:56.000000 pyevsim-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 09:11:01.382464 pyevsim-1.1.5/
+-rw-rw-rw-   0        0        0     1091 2022-08-27 18:53:45.000000 pyevsim-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0      541 2023-04-09 09:11:01.382464 pyevsim-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       58 2022-08-27 18:53:45.000000 pyevsim-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 09:11:01.365463 pyevsim-1.1.5/pyevsim/
+-rw-rw-rw-   0        0        0     1950 2022-08-27 18:53:45.000000 pyevsim-1.1.5/pyevsim/__init__.py
+-rw-rw-rw-   0        0        0     3656 2023-04-09 08:46:51.000000 pyevsim-1.1.5/pyevsim/behavior_model.py
+-rw-rw-rw-   0        0        0     2477 2022-08-27 18:53:45.000000 pyevsim-1.1.5/pyevsim/behavior_model_executor.py
+-rw-rw-rw-   0        0        0      603 2022-08-27 18:53:45.000000 pyevsim-1.1.5/pyevsim/default_message_catcher.py
+-rw-rw-rw-   0        0        0     2496 2023-04-09 08:46:51.000000 pyevsim-1.1.5/pyevsim/definition.py
+-rw-rw-rw-   0        0        0     5884 2023-04-09 09:06:40.000000 pyevsim-1.1.5/pyevsim/gen.py
+-rw-rw-rw-   0        0        0     1796 2022-08-27 18:53:45.000000 pyevsim-1.1.5/pyevsim/structural_model.py
+-rw-rw-rw-   0        0        0    14720 2023-04-09 08:46:51.000000 pyevsim-1.1.5/pyevsim/system_executor.py
+-rw-rw-rw-   0        0        0      842 2022-08-27 18:53:45.000000 pyevsim-1.1.5/pyevsim/system_message.py
+-rw-rw-rw-   0        0        0      726 2022-08-27 18:53:45.000000 pyevsim-1.1.5/pyevsim/system_object.py
+-rw-rw-rw-   0        0        0     1524 2023-04-09 08:46:51.000000 pyevsim-1.1.5/pyevsim/system_simulator.py
+-rw-rw-rw-   0        0        0      524 2022-08-27 18:53:45.000000 pyevsim-1.1.5/pyevsim/termination_manager.py
+drwxrwxrwx   0        0        0        0 2023-04-09 09:11:01.380463 pyevsim-1.1.5/pyevsim.egg-info/
+-rw-rw-rw-   0        0        0      541 2023-04-09 09:11:01.000000 pyevsim-1.1.5/pyevsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-04-09 09:11:01.000000 pyevsim-1.1.5/pyevsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 09:11:01.000000 pyevsim-1.1.5/pyevsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-09 09:11:01.000000 pyevsim-1.1.5/pyevsim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 09:11:01.382464 pyevsim-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      596 2023-04-09 08:57:52.000000 pyevsim-1.1.5/setup.py
```

### Comparing `pyevsim-1.1.4/pyevsim/__init__.py` & `pyevsim-1.1.5/pyevsim/__init__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-#!/usr/bin/env python
-# 
-# A library that provides a Modeling & Simulation Environment for Discrete Event System Formalism
-#
-# MIT License
-# Copyright (C) 2020-2022
-# Changbeom Choi <me@cbchoi.info>
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-# 
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-# 
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-"""A library that provides a Modeling & Simulation Environment for Discrete Event System Formalism"""
-
-__author__ = "me@cbchoi.info"
-
-__all__ = [ 'behavior_model', 
-			'behavior_model_executor', 
-			'default_message_catcher', 
-			'definition',
-			'structural_model',
-			'system_executor', 
-			'system_message', 
-			'system_object', 
-			'system_simulator', 
-			'termination_manager']
-
-from .system_simulator import SystemSimulator
-from .behavior_model_executor import BehaviorModelExecutor
-from .system_message import SysMessage
-from .definition import (
-	Infinite,
-	AttributeType,
-	SimulationMode,
-	ModelType,
-	CoreModel,
-	SingletonType,
+#!/usr/bin/env python
+# 
+# A library that provides a Modeling & Simulation Environment for Discrete Event System Formalism
+#
+# MIT License
+# Copyright (C) 2020-2022
+# Changbeom Choi <me@cbchoi.info>
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+# 
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+# 
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+"""A library that provides a Modeling & Simulation Environment for Discrete Event System Formalism"""
+
+__author__ = "me@cbchoi.info"
+
+__all__ = [ 'behavior_model', 
+			'behavior_model_executor', 
+			'default_message_catcher', 
+			'definition',
+			'structural_model',
+			'system_executor', 
+			'system_message', 
+			'system_object', 
+			'system_simulator', 
+			'termination_manager']
+
+from .system_simulator import SystemSimulator
+from .behavior_model_executor import BehaviorModelExecutor
+from .system_message import SysMessage
+from .definition import (
+	Infinite,
+	AttributeType,
+	SimulationMode,
+	ModelType,
+	CoreModel,
+	SingletonType,
 	)
```

### Comparing `pyevsim-1.1.4/pyevsim/default_message_catcher.py` & `pyevsim-1.1.5/pyevsim/default_message_catcher.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from .behavior_model_executor import BehaviorModelExecutor
-from .system_message import SysMessage
-from .definition import *
-
-class DefaultMessageCatcher(BehaviorModelExecutor):
-    def __init__(self, instance_time, destruct_time, name, engine_name):
-        BehaviorModelExecutor.__init__(self, instance_time, destruct_time, name, engine_name)
-
-        self.init_state("IDLE")
-        self.insert_state("IDLE", Infinite)
-
-        self.insert_input_port("uncaught")
-
-    def ext_trans(self, port, msg):
-        data = msg.retrieve()
-
-    def time_advance(self):
-        return Infinite
+from .behavior_model_executor import BehaviorModelExecutor
+from .system_message import SysMessage
+from .definition import *
+
+class DefaultMessageCatcher(BehaviorModelExecutor):
+    def __init__(self, instance_time, destruct_time, name, engine_name):
+        BehaviorModelExecutor.__init__(self, instance_time, destruct_time, name, engine_name)
+
+        self.init_state("IDLE")
+        self.insert_state("IDLE", Infinite)
+
+        self.insert_input_port("uncaught")
+
+    def ext_trans(self, port, msg):
+        data = msg.retrieve()
+
+    def time_advance(self):
+        return Infinite
```

### Comparing `pyevsim-1.1.4/pyevsim/structural_model.py` & `pyevsim-1.1.5/pyevsim/structural_model.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from .definition import CoreModel, ModelType
-from collections import OrderedDict
-
-class StructuralModel(CoreModel):
-    def __init__(self, _name=""):
-        super(StructuralModel, self).__init__(_name, ModelType.STRUCTURAL)
-
-        self._models = []
-
-        self.external_input_coupling_map = {}
-        self.external_output_coupling_map = {}
-        self.internal_coupling_map = {}
-
-    def insert_model(self, model):
-        self._models.append(model)
-
-    def retrieve_models(self):
-        return self._models
-
-    def insert_external_input_coupling(self, src_port, internal_model, dst_port):
-        if (self, src_port) not in self.external_input_coupling_map:
-            self.external_input_coupling_map[(self, src_port)] = [(internal_model, dst_port)]
-        else:
-            self.external_input_coupling_map[(self, src_port)].append((internal_model, dst_port))
-
-    def insert_external_output_coupling(self, internal_model, src_port, dst_port):
-        self.external_output_coupling_map[(internal_model, src_port)] = (self, dst_port)
-        pass
-
-    def insert_internal_coupling(self, src_model, src_port, dst_model, dst_port):
-        if (src_model, src_port) not in self.internal_coupling_map:
-            self.internal_coupling_map[(src_model, src_port)] = [(dst_model, dst_port)]
-        else:
-            self.internal_coupling_map[(src_model, src_port)].append((dst_model, dst_port))
-        pass
-
-    def retrieve_external_input_coupling(self):
-        return self.external_input_coupling_map
-
-    def retrieve_external_output_coupling(self):
-        return self.external_output_coupling_map
-
-    def retrieve_internal_coupling(self):
-        return self.internal_coupling_map
-
-    def get_create_time(self):
-        return 0
+from .definition import CoreModel, ModelType
+from collections import OrderedDict
+
+class StructuralModel(CoreModel):
+    def __init__(self, _name=""):
+        super(StructuralModel, self).__init__(_name, ModelType.STRUCTURAL)
+
+        self._models = []
+
+        self.external_input_coupling_map = {}
+        self.external_output_coupling_map = {}
+        self.internal_coupling_map = {}
+
+    def insert_model(self, model):
+        self._models.append(model)
+
+    def retrieve_models(self):
+        return self._models
+
+    def insert_external_input_coupling(self, src_port, internal_model, dst_port):
+        if (self, src_port) not in self.external_input_coupling_map:
+            self.external_input_coupling_map[(self, src_port)] = [(internal_model, dst_port)]
+        else:
+            self.external_input_coupling_map[(self, src_port)].append((internal_model, dst_port))
+
+    def insert_external_output_coupling(self, internal_model, src_port, dst_port):
+        self.external_output_coupling_map[(internal_model, src_port)] = (self, dst_port)
+        pass
+
+    def insert_internal_coupling(self, src_model, src_port, dst_model, dst_port):
+        if (src_model, src_port) not in self.internal_coupling_map:
+            self.internal_coupling_map[(src_model, src_port)] = [(dst_model, dst_port)]
+        else:
+            self.internal_coupling_map[(src_model, src_port)].append((dst_model, dst_port))
+        pass
+
+    def retrieve_external_input_coupling(self):
+        return self.external_input_coupling_map
+
+    def retrieve_external_output_coupling(self):
+        return self.external_output_coupling_map
+
+    def retrieve_internal_coupling(self):
+        return self.internal_coupling_map
+
+    def get_create_time(self):
+        return 0
```

### Comparing `pyevsim-1.1.4/pyevsim/system_object.py` & `pyevsim-1.1.5/pyevsim/system_object.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import datetime
-
-class SysObject(object):
-    # Object ID which tracks the entire instantiated Objects
-    __GLOBAL_OBJECT_ID = 0
-
-    def __init__(self):
-        self.__created_time = datetime.datetime.now()
-        self.__object_id = SysObject.__GLOBAL_OBJECT_ID
-        SysObject.__GLOBAL_OBJECT_ID = SysObject.__GLOBAL_OBJECT_ID + 1
-
-    def __str__(self):
-        return "ID:%10d %s" % (self.__object_id, self.__created_time)
-
-    def set_req_time(self, global_time):
-        pass
-
-    def get_req_time(self):
-        pass
-
-    def __lt__(self, other):
-        return self.__object_id < other.__object_id
-
-    # added by cbchoi 2020-01-21
-    def get_obj_id(self):
+import datetime
+
+class SysObject(object):
+    # Object ID which tracks the entire instantiated Objects
+    __GLOBAL_OBJECT_ID = 0
+
+    def __init__(self):
+        self.__created_time = datetime.datetime.now()
+        self.__object_id = SysObject.__GLOBAL_OBJECT_ID
+        SysObject.__GLOBAL_OBJECT_ID = SysObject.__GLOBAL_OBJECT_ID + 1
+
+    def __str__(self):
+        return "ID:%10d %s" % (self.__object_id, self.__created_time)
+
+    def set_req_time(self, global_time):
+        pass
+
+    def get_req_time(self):
+        pass
+
+    def __lt__(self, other):
+        return self.__object_id < other.__object_id
+
+    # added by cbchoi 2020-01-21
+    def get_obj_id(self):
         return self.__object_id
```

