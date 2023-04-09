# Comparing `tmp/gridworks_proactor-0.1.5.tar.gz` & `tmp/gridworks_proactor-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_proactor-0.1.5.tar", max compression
+gzip compressed data, was "gridworks_proactor-0.1.6.tar", max compression
```

## Comparing `gridworks_proactor-0.1.5.tar` & `gridworks_proactor-0.1.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1070 2023-03-29 21:43:31.717474 gridworks_proactor-0.1.5/LICENSE
--rw-r--r--   0        0        0     2615 2023-03-29 21:43:43.881518 gridworks_proactor-0.1.5/README.md
--rw-r--r--   0        0        0     2357 2023-03-29 21:43:43.881518 gridworks_proactor-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2119 2023-03-29 21:43:31.717474 gridworks_proactor-0.1.5/src/gwproactor/__init__.py
--rw-r--r--   0        0        0     1610 2023-03-29 21:43:31.717474 gridworks_proactor-0.1.5/src/gwproactor/config/__init__.py
--rw-r--r--   0        0        0     4109 2023-03-29 21:43:31.717474 gridworks_proactor-0.1.5/src/gwproactor/config/logging.py
--rw-r--r--   0        0        0      373 2023-03-29 21:43:31.717474 gridworks_proactor-0.1.5/src/gwproactor/config/mqtt.py
--rw-r--r--   0        0        0     3107 2023-03-29 21:43:31.717474 gridworks_proactor-0.1.5/src/gwproactor/config/paths.py
--rw-r--r--   0        0        0      596 2023-03-29 21:43:31.717474 gridworks_proactor-0.1.5/src/gwproactor/config/proactor_settings.py
--rw-r--r--   0        0        0    16041 2023-03-29 21:43:31.717474 gridworks_proactor-0.1.5/src/gwproactor/link_state.py
--rw-r--r--   0        0        0     5557 2023-03-29 21:43:31.717474 gridworks_proactor-0.1.5/src/gwproactor/logger.py
--rw-r--r--   0        0        0     4184 2023-03-29 21:43:31.717474 gridworks_proactor-0.1.5/src/gwproactor/logging_setup.py
--rw-r--r--   0        0        0     7715 2023-03-29 21:43:31.717474 gridworks_proactor-0.1.5/src/gwproactor/message.py
--rw-r--r--   0        0        0    11137 2023-03-29 21:43:31.717474 gridworks_proactor-0.1.5/src/gwproactor/mqtt.py
--rw-r--r--   0        0        0    13287 2023-03-29 21:43:31.717474 gridworks_proactor-0.1.5/src/gwproactor/persister.py
--rw-r--r--   0        0        0    35665 2023-03-29 21:43:31.717474 gridworks_proactor-0.1.5/src/gwproactor/proactor_implementation.py
--rw-r--r--   0        0        0     3448 2023-03-29 21:43:31.717474 gridworks_proactor-0.1.5/src/gwproactor/proactor_interface.py
--rw-r--r--   0        0        0     2645 2023-03-29 21:43:31.717474 gridworks_proactor-0.1.5/src/gwproactor/problems.py
--rw-r--r--   0        0        0        0 2023-03-29 21:43:31.717474 gridworks_proactor-0.1.5/src/gwproactor/py.typed
--rw-r--r--   0        0        0     3714 2023-03-29 21:43:31.717474 gridworks_proactor-0.1.5/src/gwproactor/stats.py
--rw-r--r--   0        0        0     9207 2023-03-29 21:43:31.717474 gridworks_proactor-0.1.5/src/gwproactor/sync_thread.py
--rw-r--r--   0        0        0     6070 2023-03-29 21:43:31.721474 gridworks_proactor-0.1.5/src/gwproactor/watchdog.py
--rw-r--r--   0        0        0     1053 2023-03-29 21:43:31.721474 gridworks_proactor-0.1.5/src/gwproactor_test/__init__.py
--rw-r--r--   0        0        0     6615 2023-03-29 21:43:31.721474 gridworks_proactor-0.1.5/src/gwproactor_test/clean.py
--rw-r--r--   0        0        0     6836 2023-03-29 21:43:31.721474 gridworks_proactor-0.1.5/src/gwproactor_test/comm_test_helper.py
--rw-r--r--   0        0        0    20076 2023-03-29 21:43:31.721474 gridworks_proactor-0.1.5/src/gwproactor_test/config/hardware-layout.json
--rw-r--r--   0        0        0      807 2023-03-29 21:43:31.721474 gridworks_proactor-0.1.5/src/gwproactor_test/dummies/__init__.py
--rw-r--r--   0        0        0      187 2023-03-29 21:43:31.721474 gridworks_proactor-0.1.5/src/gwproactor_test/dummies/child/__init__.py
--rw-r--r--   0        0        0      401 2023-03-29 21:43:31.721474 gridworks_proactor-0.1.5/src/gwproactor_test/dummies/child/config.py
--rw-r--r--   0        0        0     2558 2023-03-29 21:43:31.721474 gridworks_proactor-0.1.5/src/gwproactor_test/dummies/child/dummy.py
--rw-r--r--   0        0        0      195 2023-03-29 21:43:31.721474 gridworks_proactor-0.1.5/src/gwproactor_test/dummies/names.py
--rw-r--r--   0        0        0      193 2023-03-29 21:43:31.721474 gridworks_proactor-0.1.5/src/gwproactor_test/dummies/parent/__init__.py
--rw-r--r--   0        0        0     1021 2023-03-29 21:43:31.721474 gridworks_proactor-0.1.5/src/gwproactor_test/dummies/parent/config.py
--rw-r--r--   0        0        0     2199 2023-03-29 21:43:31.721474 gridworks_proactor-0.1.5/src/gwproactor_test/dummies/parent/dummy.py
--rw-r--r--   0        0        0     2388 2023-03-29 21:43:31.721474 gridworks_proactor-0.1.5/src/gwproactor_test/logger_guard.py
--rw-r--r--   0        0        0     9437 2023-03-29 21:43:31.721474 gridworks_proactor-0.1.5/src/gwproactor_test/proactor_recorder.py
--rw-r--r--   0        0        0    46715 2023-03-29 21:43:43.881518 gridworks_proactor-0.1.5/src/gwproactor_test/proactor_test_collections.py
--rw-r--r--   0        0        0     2936 2023-03-29 21:43:31.721474 gridworks_proactor-0.1.5/src/gwproactor_test/wait.py
--rw-r--r--   0        0        0     4150 1970-01-01 00:00:00.000000 gridworks_proactor-0.1.5/setup.py
--rw-r--r--   0        0        0     3844 1970-01-01 00:00:00.000000 gridworks_proactor-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-09 21:04:05.219174 gridworks_proactor-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2615 2023-04-09 21:04:05.219174 gridworks_proactor-0.1.6/README.md
+-rw-r--r--   0        0        0     2357 2023-04-09 21:04:27.243353 gridworks_proactor-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2119 2023-04-09 21:04:05.219174 gridworks_proactor-0.1.6/src/gwproactor/__init__.py
+-rw-r--r--   0        0        0     1610 2023-04-09 21:04:05.219174 gridworks_proactor-0.1.6/src/gwproactor/config/__init__.py
+-rw-r--r--   0        0        0     4109 2023-04-09 21:04:05.219174 gridworks_proactor-0.1.6/src/gwproactor/config/logging.py
+-rw-r--r--   0        0        0      373 2023-04-09 21:04:05.219174 gridworks_proactor-0.1.6/src/gwproactor/config/mqtt.py
+-rw-r--r--   0        0        0     3107 2023-04-09 21:04:05.219174 gridworks_proactor-0.1.6/src/gwproactor/config/paths.py
+-rw-r--r--   0        0        0      596 2023-04-09 21:04:05.219174 gridworks_proactor-0.1.6/src/gwproactor/config/proactor_settings.py
+-rw-r--r--   0        0        0    16041 2023-04-09 21:04:05.219174 gridworks_proactor-0.1.6/src/gwproactor/link_state.py
+-rw-r--r--   0        0        0     5557 2023-04-09 21:04:05.219174 gridworks_proactor-0.1.6/src/gwproactor/logger.py
+-rw-r--r--   0        0        0     4184 2023-04-09 21:04:05.219174 gridworks_proactor-0.1.6/src/gwproactor/logging_setup.py
+-rw-r--r--   0        0        0     7718 2023-04-09 21:04:27.243353 gridworks_proactor-0.1.6/src/gwproactor/message.py
+-rw-r--r--   0        0        0    11137 2023-04-09 21:04:05.219174 gridworks_proactor-0.1.6/src/gwproactor/mqtt.py
+-rw-r--r--   0        0        0    13287 2023-04-09 21:04:05.219174 gridworks_proactor-0.1.6/src/gwproactor/persister.py
+-rw-r--r--   0        0        0    35518 2023-04-09 21:04:27.243353 gridworks_proactor-0.1.6/src/gwproactor/proactor_implementation.py
+-rw-r--r--   0        0        0     3448 2023-04-09 21:04:05.219174 gridworks_proactor-0.1.6/src/gwproactor/proactor_interface.py
+-rw-r--r--   0        0        0     2645 2023-04-09 21:04:05.219174 gridworks_proactor-0.1.6/src/gwproactor/problems.py
+-rw-r--r--   0        0        0        0 2023-04-09 21:04:05.219174 gridworks_proactor-0.1.6/src/gwproactor/py.typed
+-rw-r--r--   0        0        0     3714 2023-04-09 21:04:05.219174 gridworks_proactor-0.1.6/src/gwproactor/stats.py
+-rw-r--r--   0        0        0     9207 2023-04-09 21:04:05.219174 gridworks_proactor-0.1.6/src/gwproactor/sync_thread.py
+-rw-r--r--   0        0        0     6070 2023-04-09 21:04:05.219174 gridworks_proactor-0.1.6/src/gwproactor/watchdog.py
+-rw-r--r--   0        0        0     1053 2023-04-09 21:04:05.219174 gridworks_proactor-0.1.6/src/gwproactor_test/__init__.py
+-rw-r--r--   0        0        0     6615 2023-04-09 21:04:05.223175 gridworks_proactor-0.1.6/src/gwproactor_test/clean.py
+-rw-r--r--   0        0        0     6836 2023-04-09 21:04:05.223175 gridworks_proactor-0.1.6/src/gwproactor_test/comm_test_helper.py
+-rw-r--r--   0        0        0    20076 2023-04-09 21:04:05.223175 gridworks_proactor-0.1.6/src/gwproactor_test/config/hardware-layout.json
+-rw-r--r--   0        0        0      807 2023-04-09 21:04:05.223175 gridworks_proactor-0.1.6/src/gwproactor_test/dummies/__init__.py
+-rw-r--r--   0        0        0      187 2023-04-09 21:04:05.223175 gridworks_proactor-0.1.6/src/gwproactor_test/dummies/child/__init__.py
+-rw-r--r--   0        0        0      401 2023-04-09 21:04:05.223175 gridworks_proactor-0.1.6/src/gwproactor_test/dummies/child/config.py
+-rw-r--r--   0        0        0     2558 2023-04-09 21:04:05.223175 gridworks_proactor-0.1.6/src/gwproactor_test/dummies/child/dummy.py
+-rw-r--r--   0        0        0      195 2023-04-09 21:04:05.223175 gridworks_proactor-0.1.6/src/gwproactor_test/dummies/names.py
+-rw-r--r--   0        0        0      193 2023-04-09 21:04:05.223175 gridworks_proactor-0.1.6/src/gwproactor_test/dummies/parent/__init__.py
+-rw-r--r--   0        0        0     1021 2023-04-09 21:04:05.223175 gridworks_proactor-0.1.6/src/gwproactor_test/dummies/parent/config.py
+-rw-r--r--   0        0        0     2199 2023-04-09 21:04:05.223175 gridworks_proactor-0.1.6/src/gwproactor_test/dummies/parent/dummy.py
+-rw-r--r--   0        0        0     2388 2023-04-09 21:04:05.223175 gridworks_proactor-0.1.6/src/gwproactor_test/logger_guard.py
+-rw-r--r--   0        0        0     9437 2023-04-09 21:04:05.223175 gridworks_proactor-0.1.6/src/gwproactor_test/proactor_recorder.py
+-rw-r--r--   0        0        0    46715 2023-04-09 21:04:05.223175 gridworks_proactor-0.1.6/src/gwproactor_test/proactor_test_collections.py
+-rw-r--r--   0        0        0     2936 2023-04-09 21:04:05.223175 gridworks_proactor-0.1.6/src/gwproactor_test/wait.py
+-rw-r--r--   0        0        0     4150 1970-01-01 00:00:00.000000 gridworks_proactor-0.1.6/setup.py
+-rw-r--r--   0        0        0     3844 1970-01-01 00:00:00.000000 gridworks_proactor-0.1.6/PKG-INFO
```

### Comparing `gridworks_proactor-0.1.5/LICENSE` & `gridworks_proactor-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/README.md` & `gridworks_proactor-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/pyproject.toml` & `gridworks_proactor-0.1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-proactor"
-version = "0.1.5"
+version = "0.1.6"
 description = "Gridworks Proactor"
 authors = ["Jessica Millar <jmillar@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-proactor"
 repository = "https://github.com/thegridelectric/gridworks-proactor"
 documentation = "https://gridworks-proactor.readthedocs.io"
```

### Comparing `gridworks_proactor-0.1.5/src/gwproactor/__init__.py` & `gridworks_proactor-0.1.6/src/gwproactor/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor/config/__init__.py` & `gridworks_proactor-0.1.6/src/gwproactor/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor/config/logging.py` & `gridworks_proactor-0.1.6/src/gwproactor/config/logging.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor/config/paths.py` & `gridworks_proactor-0.1.6/src/gwproactor/config/paths.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor/config/proactor_settings.py` & `gridworks_proactor-0.1.6/src/gwproactor/config/proactor_settings.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor/link_state.py` & `gridworks_proactor-0.1.6/src/gwproactor/link_state.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor/logger.py` & `gridworks_proactor-0.1.6/src/gwproactor/logger.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor/logging_setup.py` & `gridworks_proactor-0.1.6/src/gwproactor/logging_setup.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor/message.py` & `gridworks_proactor-0.1.6/src/gwproactor/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,8 +288,8 @@
 
 
 class DBGEvent(EventBase):
     Command: DBGPayload
     Path: str = ""
     Count: int = 0
     Msg: str = ""
-    TypeName: Literal["gridworks.event.scada-dbg"] = "gridworks.event.proactor.dbg"
+    TypeName: Literal["gridworks.event.proactor.dbg"] = "gridworks.event.proactor.dbg"
```

### Comparing `gridworks_proactor-0.1.5/src/gwproactor/mqtt.py` & `gridworks_proactor-0.1.6/src/gwproactor/mqtt.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor/persister.py` & `gridworks_proactor-0.1.6/src/gwproactor/persister.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor/proactor_implementation.py` & `gridworks_proactor-0.1.6/src/gwproactor/proactor_implementation.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,22 +320,18 @@
     def _apply_ack_timeout(self, transition: Transition) -> Ok:
         self._logger.path("++Proactor._apply_ack_timeout")
         path_dbg = 0
         if transition.deactivated():
             path_dbg |= 0x00000001
             self.generate_event(ResponseTimeoutEvent(PeerName=transition.link_name))
             self._logger.comm_event(str(transition))
-            if transition.recv_deactivated():
+            self._derived_recv_deactivated(transition)
+            for message_id in list(self._acks.keys()):
                 path_dbg |= 0x00000002
-                self._derived_recv_deactivated(transition)
-                for message_id in list(self._acks.keys()):
-                    path_dbg |= 0x00000004
-                    self._process_ack_result(
-                        message_id, AckWaitSummary.connection_failure
-                    )
+                self._process_ack_result(message_id, AckWaitSummary.connection_failure)
         self._logger.path("--Proactor._apply_ack_timeout path:0x%08X", path_dbg)
         return Ok()
 
     def _process_ack_result(self, message_id: str, reason: AckWaitSummary):
         self._logger.path("++Proactor._process_ack_result  %s", message_id)
         path_dbg = 0
         wait_info = self._cancel_ack_timer(message_id)
```

### Comparing `gridworks_proactor-0.1.5/src/gwproactor/proactor_interface.py` & `gridworks_proactor-0.1.6/src/gwproactor/proactor_interface.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor/problems.py` & `gridworks_proactor-0.1.6/src/gwproactor/problems.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor/stats.py` & `gridworks_proactor-0.1.6/src/gwproactor/stats.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor/sync_thread.py` & `gridworks_proactor-0.1.6/src/gwproactor/sync_thread.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor/watchdog.py` & `gridworks_proactor-0.1.6/src/gwproactor/watchdog.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor_test/__init__.py` & `gridworks_proactor-0.1.6/src/gwproactor_test/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor_test/clean.py` & `gridworks_proactor-0.1.6/src/gwproactor_test/clean.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor_test/comm_test_helper.py` & `gridworks_proactor-0.1.6/src/gwproactor_test/comm_test_helper.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor_test/config/hardware-layout.json` & `gridworks_proactor-0.1.6/src/gwproactor_test/config/hardware-layout.json`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor_test/dummies/__init__.py` & `gridworks_proactor-0.1.6/src/gwproactor_test/dummies/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor_test/dummies/child/dummy.py` & `gridworks_proactor-0.1.6/src/gwproactor_test/dummies/child/dummy.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor_test/dummies/parent/config.py` & `gridworks_proactor-0.1.6/src/gwproactor_test/dummies/parent/config.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor_test/dummies/parent/dummy.py` & `gridworks_proactor-0.1.6/src/gwproactor_test/dummies/parent/dummy.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor_test/logger_guard.py` & `gridworks_proactor-0.1.6/src/gwproactor_test/logger_guard.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor_test/proactor_recorder.py` & `gridworks_proactor-0.1.6/src/gwproactor_test/proactor_recorder.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor_test/proactor_test_collections.py` & `gridworks_proactor-0.1.6/src/gwproactor_test/proactor_test_collections.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/src/gwproactor_test/wait.py` & `gridworks_proactor-0.1.6/src/gwproactor_test/wait.py`

 * *Files identical despite different names*

### Comparing `gridworks_proactor-0.1.5/setup.py` & `gridworks_proactor-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
  'xdg>=6.0.0,<7.0.0']
 
 extras_require = \
 {'tests': ['pytest>=7.2.0,<8.0.0', 'pytest-asyncio>=0.20.3,<0.21.0']}
 
 setup_kwargs = {
     'name': 'gridworks-proactor',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'Gridworks Proactor',
     'long_description': "# Gridworks Proactor\n\n[![PyPI](https://img.shields.io/pypi/v/gridworks-proactor.svg)][pypi status]\n[![Status](https://img.shields.io/pypi/status/gridworks-proactor.svg)][pypi status]\n[![Python Version](https://img.shields.io/pypi/pyversions/gridworks-proactor)][pypi status]\n[![License](https://img.shields.io/pypi/l/gridworks-proactor)][license]\n\n[![Read the documentation at https://gridworks-proactor.readthedocs.io/](https://img.shields.io/readthedocs/gridworks-proactor/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/thegridelectric/gridworks-proactor/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/thegridelectric/gridworks-proactor/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi status]: https://pypi.org/project/gridworks-proactor/\n[read the docs]: https://gridworks-proactor.readthedocs.io/\n[tests]: https://github.com/thegridelectric/gridworks-proactor/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/thegridelectric/gridworks-proactor\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n- TODO\n\n## Requirements\n\n- TODO\n\n## Installation\n\nYou can install _Gridworks Proactor_ via [pip] from [PyPI]:\n\n```console\n$ pip install gridworks-proactor\n```\n\n## Usage\n\nPlease see the [Command-line Reference] for details.\n\n## Contributing\n\nContributions are very welcome. In order to develop, do this:\n\n```console\n$ poetry install --all-extras\n```\n\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Gridworks Proactor_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/thegridelectric/gridworks-proactor/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/thegridelectric/gridworks-proactor/blob/main/LICENSE\n[contributor guide]: https://github.com/thegridelectric/gridworks-proactor/blob/main/CONTRIBUTING.md\n[command-line reference]: https://gridworks-proactor.readthedocs.io/en/latest/usage.html\n",
     'author': 'Jessica Millar',
     'author_email': 'jmillar@gridworks-consulting.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/thegridelectric/gridworks-proactor',
```

### Comparing `gridworks_proactor-0.1.5/PKG-INFO` & `gridworks_proactor-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks-proactor
-Version: 0.1.5
+Version: 0.1.6
 Summary: Gridworks Proactor
 Home-page: https://github.com/thegridelectric/gridworks-proactor
 License: MIT
 Author: Jessica Millar
 Author-email: jmillar@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

