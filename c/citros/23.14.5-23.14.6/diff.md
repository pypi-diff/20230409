# Comparing `tmp/citros-23.14.5.tar.gz` & `tmp/citros-23.14.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citros-23.14.5.tar", last modified: Sun Apr  9 08:38:22 2023, max compression
+gzip compressed data, was "citros-23.14.6.tar", last modified: Sun Apr  9 08:42:50 2023, max compression
```

## Comparing `citros-23.14.5.tar` & `citros-23.14.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:38:22.357019 citros-23.14.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 08:38:03.000000 citros-23.14.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-09 08:38:22.353019 citros-23.14.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-09 08:38:03.000000 citros-23.14.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:38:22.353019 citros-23.14.5/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-09 08:38:03.000000 citros-23.14.5/bin/citros
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:38:22.353019 citros-23.14.5/citros/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-09 08:38:03.000000 citros-23.14.5/citros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-09 08:38:03.000000 citros-23.14.5/citros/citros.py
--rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-04-09 08:38:03.000000 citros-23.14.5/citros/citros_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-09 08:38:03.000000 citros-23.14.5/citros/citros_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-04-09 08:38:03.000000 citros-23.14.5/citros/citros_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-09 08:38:03.000000 citros-23.14.5/citros/citros_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-04-09 08:38:03.000000 citros-23.14.5/citros/citros_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-09 08:38:03.000000 citros-23.14.5/citros/citros_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:38:22.353019 citros-23.14.5/citros/launches/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-09 08:38:03.000000 citros-23.14.5/citros/launches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-04-09 08:38:03.000000 citros-23.14.5/citros/launches/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:38:22.353019 citros-23.14.5/citros/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-09 08:38:03.000000 citros-23.14.5/citros/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-09 08:38:03.000000 citros-23.14.5/citros/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-09 08:38:03.000000 citros-23.14.5/citros/logger/logger_pg_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:38:22.353019 citros-23.14.5/citros/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-09 08:38:03.000000 citros-23.14.5/citros/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-09 08:38:03.000000 citros-23.14.5/citros/parsers/parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-04-09 08:38:03.000000 citros-23.14.5/citros/parsers/parser_ros2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:38:22.353019 citros-23.14.5/citros/rosbag/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-09 08:38:03.000000 citros-23.14.5/citros/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-09 08:38:03.000000 citros-23.14.5/citros/rosbag/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-09 08:38:03.000000 citros-23.14.5/citros/rosbag/reader_mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-09 08:38:03.000000 citros-23.14.5/citros/rosbag/reader_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:38:22.353019 citros-23.14.5/citros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-09 08:38:22.000000 citros-23.14.5/citros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-09 08:38:22.000000 citros-23.14.5/citros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 08:38:22.000000 citros-23.14.5/citros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-09 08:38:22.000000 citros-23.14.5/citros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-09 08:38:22.000000 citros-23.14.5/citros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-09 08:38:03.000000 citros-23.14.5/citros_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 08:38:22.357019 citros-23.14.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-09 08:38:03.000000 citros-23.14.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:38:22.353019 citros-23.14.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:38:03.000000 citros-23.14.5/tests/test_parse_ros_project.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:38:03.000000 citros-23.14.5/tests/test_uplosd_to_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:50.151061 citros-23.14.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 08:42:32.000000 citros-23.14.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-09 08:42:50.151061 citros-23.14.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-09 08:42:32.000000 citros-23.14.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:50.147061 citros-23.14.6/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-09 08:42:32.000000 citros-23.14.6/bin/citros
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:50.147061 citros-23.14.6/citros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-09 08:42:32.000000 citros-23.14.6/citros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-09 08:42:32.000000 citros-23.14.6/citros/citros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-04-09 08:42:32.000000 citros-23.14.6/citros/citros_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-09 08:42:32.000000 citros-23.14.6/citros/citros_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-04-09 08:42:32.000000 citros-23.14.6/citros/citros_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-09 08:42:32.000000 citros-23.14.6/citros/citros_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-04-09 08:42:32.000000 citros-23.14.6/citros/citros_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-09 08:42:32.000000 citros-23.14.6/citros/citros_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:50.147061 citros-23.14.6/citros/launches/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-09 08:42:32.000000 citros-23.14.6/citros/launches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-04-09 08:42:32.000000 citros-23.14.6/citros/launches/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:50.147061 citros-23.14.6/citros/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-09 08:42:32.000000 citros-23.14.6/citros/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-09 08:42:32.000000 citros-23.14.6/citros/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-09 08:42:32.000000 citros-23.14.6/citros/logger/logger_pg_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:50.147061 citros-23.14.6/citros/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-09 08:42:32.000000 citros-23.14.6/citros/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-09 08:42:32.000000 citros-23.14.6/citros/parsers/parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-04-09 08:42:32.000000 citros-23.14.6/citros/parsers/parser_ros2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:50.147061 citros-23.14.6/citros/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-09 08:42:32.000000 citros-23.14.6/citros/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-09 08:42:32.000000 citros-23.14.6/citros/rosbag/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-09 08:42:32.000000 citros-23.14.6/citros/rosbag/reader_mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-09 08:42:32.000000 citros-23.14.6/citros/rosbag/reader_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:50.147061 citros-23.14.6/citros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-09 08:42:50.000000 citros-23.14.6/citros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-09 08:42:50.000000 citros-23.14.6/citros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 08:42:50.000000 citros-23.14.6/citros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-09 08:42:50.000000 citros-23.14.6/citros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-09 08:42:50.000000 citros-23.14.6/citros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-09 08:42:32.000000 citros-23.14.6/citros_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 08:42:50.151061 citros-23.14.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-09 08:42:32.000000 citros-23.14.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:50.147061 citros-23.14.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:32.000000 citros-23.14.6/tests/test_parse_ros_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:42:32.000000 citros-23.14.6/tests/test_uplosd_to_server.py
```

### Comparing `citros-23.14.5/LICENSE` & `citros-23.14.6/LICENSE`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/PKG-INFO` & `citros-23.14.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.14.5
+Version: 23.14.6
 Summary: A cli entypoint for citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.14.5/README.md` & `citros-23.14.6/README.md`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/bin/citros` & `citros-23.14.6/bin/citros`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/citros/__init__.py` & `citros-23.14.6/citros/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/citros/citros.py` & `citros-23.14.6/citros/citros.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/citros/citros_bag.py` & `citros-23.14.6/citros/citros_bag.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/citros/citros_batch.py` & `citros-23.14.6/citros/citros_batch.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/citros/citros_events.py` & `citros-23.14.6/citros/citros_events.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/citros/citros_integration.py` & `citros-23.14.6/citros/citros_integration.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/citros/citros_params.py` & `citros-23.14.6/citros/citros_params.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/citros/citros_utils.py` & `citros-23.14.6/citros/citros_utils.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/citros/launches/__init__.py` & `citros-23.14.6/citros/launches/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/citros/launches/launch.py` & `citros-23.14.6/citros/launches/launch.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/citros/logger/__init__.py` & `citros-23.14.6/citros/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/citros/logger/logger.py` & `citros-23.14.6/citros/logger/logger.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/citros/logger/logger_pg_handler.py` & `citros-23.14.6/citros/logger/logger_pg_handler.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/citros/parsers/__init__.py` & `citros-23.14.6/citros/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/citros/parsers/parser_ros2.py` & `citros-23.14.6/citros/parsers/parser_ros2.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
             })
         return packages
 
     def get_project_launch_files(self, package_path, workspace=""):
         #TODO: check if done. 
         launch_paths = glob.glob(f"{package_path}/launch/*.py")
         if workspace != "":
-            launch_paths + glob.glob(f"{package_path}/{workspace}/src/[!ros2.*]*")
+            launch_paths + glob.glob(f"{package_path}/{workspace}/src/*.py")
         
         launch_paths = [p for p in launch_paths if 'ros2.' not in p]
         
         launche_files = []
         for launch_path in launch_paths:
             launche_files.append({                
                 "name": launch_path.split("/")[-1],
```

### Comparing `citros-23.14.5/citros/rosbag/__init__.py` & `citros-23.14.6/citros/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/citros/rosbag/reader_base.py` & `citros-23.14.6/citros/rosbag/reader_base.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/citros/rosbag/reader_mcap.py` & `citros-23.14.6/citros/rosbag/reader_mcap.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/citros/rosbag/reader_sqlite.py` & `citros-23.14.6/citros/rosbag/reader_sqlite.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/citros.egg-info/PKG-INFO` & `citros-23.14.6/citros.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.14.5
+Version: 23.14.6
 Summary: A cli entypoint for citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.14.5/citros.egg-info/SOURCES.txt` & `citros-23.14.6/citros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citros-23.14.5/setup.py` & `citros-23.14.6/setup.py`

 * *Files identical despite different names*

