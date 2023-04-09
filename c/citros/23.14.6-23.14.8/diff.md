# Comparing `tmp/citros-23.14.6.tar.gz` & `tmp/citros-23.14.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citros-23.14.6.tar", last modified: Sun Apr  9 08:42:50 2023, max compression
+gzip compressed data, was "citros-23.14.8.tar", last modified: Sun Apr  9 16:37:05 2023, max compression
```

## Comparing `citros-23.14.6.tar` & `citros-23.14.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:50.151061 citros-23.14.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 08:42:32.000000 citros-23.14.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-09 08:42:50.151061 citros-23.14.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-09 08:42:32.000000 citros-23.14.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:50.147061 citros-23.14.6/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-09 08:42:32.000000 citros-23.14.6/bin/citros
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:50.147061 citros-23.14.6/citros/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-09 08:42:32.000000 citros-23.14.6/citros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-09 08:42:32.000000 citros-23.14.6/citros/citros.py
--rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-04-09 08:42:32.000000 citros-23.14.6/citros/citros_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-09 08:42:32.000000 citros-23.14.6/citros/citros_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-04-09 08:42:32.000000 citros-23.14.6/citros/citros_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-09 08:42:32.000000 citros-23.14.6/citros/citros_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-04-09 08:42:32.000000 citros-23.14.6/citros/citros_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-09 08:42:32.000000 citros-23.14.6/citros/citros_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:50.147061 citros-23.14.6/citros/launches/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-09 08:42:32.000000 citros-23.14.6/citros/launches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-04-09 08:42:32.000000 citros-23.14.6/citros/launches/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:50.147061 citros-23.14.6/citros/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-09 08:42:32.000000 citros-23.14.6/citros/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-09 08:42:32.000000 citros-23.14.6/citros/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-09 08:42:32.000000 citros-23.14.6/citros/logger/logger_pg_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:50.147061 citros-23.14.6/citros/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-09 08:42:32.000000 citros-23.14.6/citros/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-09 08:42:32.000000 citros-23.14.6/citros/parsers/parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-04-09 08:42:32.000000 citros-23.14.6/citros/parsers/parser_ros2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:50.147061 citros-23.14.6/citros/rosbag/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-09 08:42:32.000000 citros-23.14.6/citros/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-09 08:42:32.000000 citros-23.14.6/citros/rosbag/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-09 08:42:32.000000 citros-23.14.6/citros/rosbag/reader_mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-09 08:42:32.000000 citros-23.14.6/citros/rosbag/reader_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:50.147061 citros-23.14.6/citros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-09 08:42:50.000000 citros-23.14.6/citros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-09 08:42:50.000000 citros-23.14.6/citros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 08:42:50.000000 citros-23.14.6/citros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-09 08:42:50.000000 citros-23.14.6/citros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-09 08:42:50.000000 citros-23.14.6/citros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-09 08:42:32.000000 citros-23.14.6/citros_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 08:42:50.151061 citros-23.14.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-09 08:42:32.000000 citros-23.14.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:50.147061 citros-23.14.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:32.000000 citros-23.14.6/tests/test_parse_ros_project.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:32.000000 citros-23.14.6/tests/test_uplosd_to_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:37:05.905102 citros-23.14.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 16:36:48.000000 citros-23.14.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-09 16:37:05.905102 citros-23.14.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-09 16:36:48.000000 citros-23.14.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:37:05.901101 citros-23.14.8/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-09 16:36:48.000000 citros-23.14.8/bin/citros
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:37:05.901101 citros-23.14.8/citros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-09 16:36:48.000000 citros-23.14.8/citros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-09 16:36:48.000000 citros-23.14.8/citros/citros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-04-09 16:36:48.000000 citros-23.14.8/citros/citros_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-09 16:36:48.000000 citros-23.14.8/citros/citros_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-04-09 16:36:48.000000 citros-23.14.8/citros/citros_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-09 16:36:48.000000 citros-23.14.8/citros/citros_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-04-09 16:36:48.000000 citros-23.14.8/citros/citros_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-09 16:36:48.000000 citros-23.14.8/citros/citros_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:37:05.901101 citros-23.14.8/citros/launches/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-09 16:36:48.000000 citros-23.14.8/citros/launches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-04-09 16:36:48.000000 citros-23.14.8/citros/launches/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:37:05.905102 citros-23.14.8/citros/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-09 16:36:48.000000 citros-23.14.8/citros/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-09 16:36:48.000000 citros-23.14.8/citros/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-09 16:36:48.000000 citros-23.14.8/citros/logger/logger_pg_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:37:05.905102 citros-23.14.8/citros/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-09 16:36:48.000000 citros-23.14.8/citros/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-09 16:36:48.000000 citros-23.14.8/citros/parsers/parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-04-09 16:36:48.000000 citros-23.14.8/citros/parsers/parser_ros2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:37:05.905102 citros-23.14.8/citros/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-09 16:36:48.000000 citros-23.14.8/citros/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-09 16:36:48.000000 citros-23.14.8/citros/rosbag/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-09 16:36:48.000000 citros-23.14.8/citros/rosbag/reader_mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-09 16:36:48.000000 citros-23.14.8/citros/rosbag/reader_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:37:05.901101 citros-23.14.8/citros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-09 16:37:05.000000 citros-23.14.8/citros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-09 16:37:05.000000 citros-23.14.8/citros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 16:37:05.000000 citros-23.14.8/citros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-09 16:37:05.000000 citros-23.14.8/citros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-09 16:37:05.000000 citros-23.14.8/citros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-09 16:36:48.000000 citros-23.14.8/citros_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 16:37:05.905102 citros-23.14.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-09 16:36:48.000000 citros-23.14.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:37:05.905102 citros-23.14.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 16:36:48.000000 citros-23.14.8/tests/test_parse_ros_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 16:36:48.000000 citros-23.14.8/tests/test_uplosd_to_server.py
```

### Comparing `citros-23.14.6/LICENSE` & `citros-23.14.8/LICENSE`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/PKG-INFO` & `citros-23.14.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.14.6
+Version: 23.14.8
 Summary: A cli entypoint for citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.14.6/README.md` & `citros-23.14.8/README.md`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/bin/citros` & `citros-23.14.8/bin/citros`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/citros/__init__.py` & `citros-23.14.8/citros/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/citros/citros.py` & `citros-23.14.8/citros/citros.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/citros/citros_bag.py` & `citros-23.14.8/citros/citros_bag.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/citros/citros_batch.py` & `citros-23.14.8/citros/citros_batch.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/citros/citros_events.py` & `citros-23.14.8/citros/citros_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                               headers={"Authorization": f"Bearer {self.citros._get_token()}"}
                             )              
             if resp.status_code != 200:
                 print(f"Error from sync_events: [{self.CITROS_EVENTS}], {resp.status_code}: {resp.reason}", resp)
                 # print("sync_events", self.CITROS_EVENTS, request_json)
                 return False   
         except Exception as e:
-            print(f"Error from sync_events: [{self.CITROS_EVENTS}], {e}", resp)
+            print(f"Error from sync_events: [{self.CITROS_EVENTS}], {e}")
             return False
         return True
```

### Comparing `citros-23.14.6/citros/citros_integration.py` & `citros-23.14.8/citros/citros_integration.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/citros/citros_params.py` & `citros-23.14.8/citros/citros_params.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/citros/citros_utils.py` & `citros-23.14.8/citros/citros_utils.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/citros/launches/__init__.py` & `citros-23.14.8/citros/launches/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/citros/launches/launch.py` & `citros-23.14.8/citros/launches/launch.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/citros/logger/__init__.py` & `citros-23.14.8/citros/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/citros/logger/logger.py` & `citros-23.14.8/citros/logger/logger.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/citros/logger/logger_pg_handler.py` & `citros-23.14.8/citros/logger/logger_pg_handler.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/citros/parsers/__init__.py` & `citros-23.14.8/citros/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/citros/parsers/parser_ros2.py` & `citros-23.14.8/citros/parsers/parser_ros2.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/citros/rosbag/__init__.py` & `citros-23.14.8/citros/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/citros/rosbag/reader_base.py` & `citros-23.14.8/citros/rosbag/reader_base.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/citros/rosbag/reader_mcap.py` & `citros-23.14.8/citros/rosbag/reader_mcap.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/citros/rosbag/reader_sqlite.py` & `citros-23.14.8/citros/rosbag/reader_sqlite.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/citros.egg-info/PKG-INFO` & `citros-23.14.8/citros.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.14.6
+Version: 23.14.8
 Summary: A cli entypoint for citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.14.6/citros.egg-info/SOURCES.txt` & `citros-23.14.8/citros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citros-23.14.6/setup.py` & `citros-23.14.8/setup.py`

 * *Files identical despite different names*

