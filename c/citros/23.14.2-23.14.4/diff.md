# Comparing `tmp/citros-23.14.2.tar.gz` & `tmp/citros-23.14.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citros-23.14.2.tar", last modified: Sun Apr  9 08:05:34 2023, max compression
+gzip compressed data, was "citros-23.14.4.tar", last modified: Sun Apr  9 08:34:38 2023, max compression
```

## Comparing `citros-23.14.2.tar` & `citros-23.14.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:34.586971 citros-23.14.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 08:05:17.000000 citros-23.14.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-09 08:05:34.586971 citros-23.14.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-09 08:05:17.000000 citros-23.14.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:34.582971 citros-23.14.2/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-09 08:05:17.000000 citros-23.14.2/bin/citros
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:34.582971 citros-23.14.2/citros/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-09 08:05:17.000000 citros-23.14.2/citros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-09 08:05:17.000000 citros-23.14.2/citros/citros.py
--rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-04-09 08:05:17.000000 citros-23.14.2/citros/citros_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-09 08:05:17.000000 citros-23.14.2/citros/citros_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-04-09 08:05:17.000000 citros-23.14.2/citros/citros_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-09 08:05:17.000000 citros-23.14.2/citros/citros_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-04-09 08:05:17.000000 citros-23.14.2/citros/citros_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-09 08:05:17.000000 citros-23.14.2/citros/citros_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:34.582971 citros-23.14.2/citros/launches/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-09 08:05:17.000000 citros-23.14.2/citros/launches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-04-09 08:05:17.000000 citros-23.14.2/citros/launches/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:34.582971 citros-23.14.2/citros/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-09 08:05:17.000000 citros-23.14.2/citros/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-09 08:05:17.000000 citros-23.14.2/citros/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-09 08:05:17.000000 citros-23.14.2/citros/logger/logger_pg_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:34.582971 citros-23.14.2/citros/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-09 08:05:17.000000 citros-23.14.2/citros/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-09 08:05:17.000000 citros-23.14.2/citros/parsers/parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-04-09 08:05:17.000000 citros-23.14.2/citros/parsers/parser_ros2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:34.586971 citros-23.14.2/citros/rosbag/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-09 08:05:17.000000 citros-23.14.2/citros/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-09 08:05:17.000000 citros-23.14.2/citros/rosbag/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-09 08:05:17.000000 citros-23.14.2/citros/rosbag/reader_mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-09 08:05:17.000000 citros-23.14.2/citros/rosbag/reader_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:34.582971 citros-23.14.2/citros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-09 08:05:34.000000 citros-23.14.2/citros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-09 08:05:34.000000 citros-23.14.2/citros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 08:05:34.000000 citros-23.14.2/citros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-09 08:05:34.000000 citros-23.14.2/citros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-09 08:05:34.000000 citros-23.14.2/citros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-09 08:05:17.000000 citros-23.14.2/citros_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 08:05:34.586971 citros-23.14.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-09 08:05:17.000000 citros-23.14.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:34.586971 citros-23.14.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:17.000000 citros-23.14.2/tests/test_parse_ros_project.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:17.000000 citros-23.14.2/tests/test_uplosd_to_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:34:38.912022 citros-23.14.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 08:34:24.000000 citros-23.14.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-09 08:34:38.912022 citros-23.14.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-09 08:34:24.000000 citros-23.14.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:34:38.900022 citros-23.14.4/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-09 08:34:24.000000 citros-23.14.4/bin/citros
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:34:38.904022 citros-23.14.4/citros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-09 08:34:24.000000 citros-23.14.4/citros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-09 08:34:24.000000 citros-23.14.4/citros/citros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-04-09 08:34:24.000000 citros-23.14.4/citros/citros_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-09 08:34:24.000000 citros-23.14.4/citros/citros_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-04-09 08:34:24.000000 citros-23.14.4/citros/citros_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-09 08:34:24.000000 citros-23.14.4/citros/citros_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-04-09 08:34:24.000000 citros-23.14.4/citros/citros_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-09 08:34:24.000000 citros-23.14.4/citros/citros_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:34:38.908022 citros-23.14.4/citros/launches/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-09 08:34:24.000000 citros-23.14.4/citros/launches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-04-09 08:34:24.000000 citros-23.14.4/citros/launches/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:34:38.908022 citros-23.14.4/citros/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-09 08:34:24.000000 citros-23.14.4/citros/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-09 08:34:24.000000 citros-23.14.4/citros/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-09 08:34:24.000000 citros-23.14.4/citros/logger/logger_pg_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:34:38.908022 citros-23.14.4/citros/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-09 08:34:24.000000 citros-23.14.4/citros/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-09 08:34:24.000000 citros-23.14.4/citros/parsers/parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-04-09 08:34:24.000000 citros-23.14.4/citros/parsers/parser_ros2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:34:38.908022 citros-23.14.4/citros/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-09 08:34:24.000000 citros-23.14.4/citros/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-09 08:34:24.000000 citros-23.14.4/citros/rosbag/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-09 08:34:24.000000 citros-23.14.4/citros/rosbag/reader_mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-09 08:34:24.000000 citros-23.14.4/citros/rosbag/reader_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:34:38.904022 citros-23.14.4/citros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-09 08:34:38.000000 citros-23.14.4/citros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-09 08:34:38.000000 citros-23.14.4/citros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 08:34:38.000000 citros-23.14.4/citros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-09 08:34:38.000000 citros-23.14.4/citros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-09 08:34:38.000000 citros-23.14.4/citros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-09 08:34:24.000000 citros-23.14.4/citros_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 08:34:38.912022 citros-23.14.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-09 08:34:24.000000 citros-23.14.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:34:38.912022 citros-23.14.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:34:24.000000 citros-23.14.4/tests/test_parse_ros_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:34:24.000000 citros-23.14.4/tests/test_uplosd_to_server.py
```

### Comparing `citros-23.14.2/LICENSE` & `citros-23.14.4/LICENSE`

 * *Files identical despite different names*

### Comparing `citros-23.14.2/PKG-INFO` & `citros-23.14.4/citros/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,21 @@
-Metadata-Version: 2.1
-Name: citros
-Version: 23.14.2
-Summary: A cli entypoint for citros system.
-Home-page: http://pypi.python.org/pypi/citros_cli/
-Author: vovacooper
-Author-email: vova@lulav.space
-License: LICENSE.txt
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-```python
 # ==============================================
-#   ██████╗██╗████████╗██████╗  ██████╗ ███████╗
-#  ██╔════╝██║╚══██╔══╝██╔══██╗██╔═══██╗██╔════╝
-#  ██║     ██║   ██║   ██████╔╝██║   ██║███████╗
-#  ██║     ██║   ██║   ██╔══██╗██║   ██║╚════██║
-#  ╚██████╗██║   ██║   ██║  ██║╚██████╔╝███████║
-#   ╚═════╝╚═╝   ╚═╝   ╚═╝  ╚═╝ ╚═════╝ ╚══════╝                                        
+#  ██████╗██╗████████╗██████╗  ██████╗ ███████╗
+# ██╔════╝██║╚══██╔══╝██╔══██╗██╔═══██╗██╔════╝
+# ██║     ██║   ██║   ██████╔╝██║   ██║███████╗
+# ██║     ██║   ██║   ██╔══██╗██║   ██║╚════██║
+# ╚██████╗██║   ██║   ██║  ██║╚██████╔╝███████║
+#  ╚═════╝╚═╝   ╚═╝   ╚═╝  ╚═╝ ╚═════╝ ╚══════╝                                        
 # ==============================================
-```
-# CiTROS CLI
 
-# description:
+from .citros import Citros
+
+__all__ = [
+        'Citros'
+]
 
-the CiTROS cli will run by the user. 
-inside the ros-project folder. 
+__version__ = "unknown"
+try:
+    from citros_meta import __version__,__author__,__author_email__,__copyright__,__description__,__license__,__title__,__url__
+except ImportError:
+    # We're running in a tree that doesn't have a _version.py, so we don't know what our version is.
+    pass
```

### Comparing `citros-23.14.2/README.md` & `citros-23.14.4/citros/launches/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,61 @@
-00000000: 6060 6070 7974 686f 6e0a 2320 3d3d 3d3d  ```python.# ====
+00000000: 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  # ==============
 00000010: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00000020: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000030: 3d3d 3d3d 3d3d 3d3d 3d3d 0a23 2020 20e2  ==========.#   .
-00000040: 9688 e296 88e2 9688 e296 88e2 9688 e296  ................
-00000050: 88e2 9597 e296 88e2 9688 e295 97e2 9688  ................
-00000060: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
-00000070: 9688 e296 88e2 9597 e296 88e2 9688 e296  ................
-00000080: 88e2 9688 e296 88e2 9688 e295 9720 20e2  .............  .
-00000090: 9688 e296 88e2 9688 e296 88e2 9688 e296  ................
-000000a0: 88e2 9597 20e2 9688 e296 88e2 9688 e296  .... ...........
-000000b0: 88e2 9688 e296 88e2 9688 e295 970a 2320  ..............# 
-000000c0: 20e2 9688 e296 88e2 9594 e295 90e2 9590   ...............
-000000d0: e295 90e2 9590 e295 9de2 9688 e296 88e2  ................
-000000e0: 9591 e295 9ae2 9590 e295 90e2 9688 e296  ................
-000000f0: 88e2 9594 e295 90e2 9590 e295 9de2 9688  ................
-00000100: e296 88e2 9594 e295 90e2 9590 e296 88e2  ................
-00000110: 9688 e295 97e2 9688 e296 88e2 9594 e295  ................
-00000120: 90e2 9590 e295 90e2 9688 e296 88e2 9597  ................
-00000130: e296 88e2 9688 e295 94e2 9590 e295 90e2  ................
-00000140: 9590 e295 90e2 959d 0a23 2020 e296 88e2  .........#  ....
-00000150: 9688 e295 9120 2020 2020 e296 88e2 9688  .....     ......
-00000160: e295 9120 2020 e296 88e2 9688 e295 9120  ...   ......... 
-00000170: 2020 e296 88e2 9688 e296 88e2 9688 e296    ..............
-00000180: 88e2 9688 e295 94e2 959d e296 88e2 9688  ................
-00000190: e295 9120 2020 e296 88e2 9688 e295 91e2  ...   ..........
-000001a0: 9688 e296 88e2 9688 e296 88e2 9688 e296  ................
-000001b0: 88e2 9688 e295 970a 2320 20e2 9688 e296  ........#  .....
-000001c0: 88e2 9591 2020 2020 20e2 9688 e296 88e2  ....     .......
-000001d0: 9591 2020 20e2 9688 e296 88e2 9591 2020  ..   .........  
-000001e0: 20e2 9688 e296 88e2 9594 e295 90e2 9590   ...............
-000001f0: e296 88e2 9688 e295 97e2 9688 e296 88e2  ................
-00000200: 9591 2020 20e2 9688 e296 88e2 9591 e295  ..   ...........
-00000210: 9ae2 9590 e295 90e2 9590 e295 90e2 9688  ................
-00000220: e296 88e2 9591 0a23 2020 e295 9ae2 9688  .......#  ......
-00000230: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
-00000240: 9597 e296 88e2 9688 e295 9120 2020 e296  ...........   ..
-00000250: 88e2 9688 e295 9120 2020 e296 88e2 9688  .......   ......
-00000260: e295 9120 20e2 9688 e296 88e2 9591 e295  ...  ...........
-00000270: 9ae2 9688 e296 88e2 9688 e296 88e2 9688  ................
-00000280: e296 88e2 9594 e295 9de2 9688 e296 88e2  ................
-00000290: 9688 e296 88e2 9688 e296 88e2 9688 e295  ................
-000002a0: 910a 2320 2020 e295 9ae2 9590 e295 90e2  ..#   ..........
-000002b0: 9590 e295 90e2 9590 e295 9de2 959a e295  ................
-000002c0: 90e2 959d 2020 20e2 959a e295 90e2 959d  ....   .........
-000002d0: 2020 20e2 959a e295 90e2 959d 2020 e295     .........  ..
-000002e0: 9ae2 9590 e295 9d20 e295 9ae2 9590 e295  ....... ........
-000002f0: 90e2 9590 e295 90e2 9590 e295 9d20 e295  ............. ..
-00000300: 9ae2 9590 e295 90e2 9590 e295 90e2 9590  ................
-00000310: e295 90e2 959d 2020 2020 2020 2020 2020  ......          
-00000320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000330: 2020 2020 2020 2020 2020 2020 2020 0a23                .#
-00000340: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
-00000350: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000360: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
-00000370: 6060 600a 2320 4369 5452 4f53 2043 4c49  ```.# CiTROS CLI
-00000380: 0a0a 2320 6465 7363 7269 7074 696f 6e3a  ..# description:
-00000390: 0a0a 7468 6520 4369 5452 4f53 2063 6c69  ..the CiTROS cli
-000003a0: 2077 696c 6c20 7275 6e20 6279 2074 6865   will run by the
-000003b0: 2075 7365 722e 200a 696e 7369 6465 2074   user. .inside t
-000003c0: 6865 2072 6f73 2d70 726f 6a65 6374 2066  he ros-project f
-000003d0: 6f6c 6465 722e 200a                      older. .
+00000030: 0a23 2020 e296 88e2 9688 e296 88e2 9688  .#  ............
+00000040: e296 88e2 9688 e295 97e2 9688 e296 88e2  ................
+00000050: 9597 e296 88e2 9688 e296 88e2 9688 e296  ................
+00000060: 88e2 9688 e296 88e2 9688 e295 97e2 9688  ................
+00000070: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
+00000080: 9597 2020 e296 88e2 9688 e296 88e2 9688  ..  ............
+00000090: e296 88e2 9688 e295 9720 e296 88e2 9688  ......... ......
+000000a0: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
+000000b0: 9597 0a23 20e2 9688 e296 88e2 9594 e295  ...# ...........
+000000c0: 90e2 9590 e295 90e2 9590 e295 9de2 9688  ................
+000000d0: e296 88e2 9591 e295 9ae2 9590 e295 90e2  ................
+000000e0: 9688 e296 88e2 9594 e295 90e2 9590 e295  ................
+000000f0: 9de2 9688 e296 88e2 9594 e295 90e2 9590  ................
+00000100: e296 88e2 9688 e295 97e2 9688 e296 88e2  ................
+00000110: 9594 e295 90e2 9590 e295 90e2 9688 e296  ................
+00000120: 88e2 9597 e296 88e2 9688 e295 94e2 9590  ................
+00000130: e295 90e2 9590 e295 90e2 959d 0a23 20e2  .............# .
+00000140: 9688 e296 88e2 9591 2020 2020 20e2 9688  ........     ...
+00000150: e296 88e2 9591 2020 20e2 9688 e296 88e2  ......   .......
+00000160: 9591 2020 20e2 9688 e296 88e2 9688 e296  ..   ...........
+00000170: 88e2 9688 e296 88e2 9594 e295 9de2 9688  ................
+00000180: e296 88e2 9591 2020 20e2 9688 e296 88e2  ......   .......
+00000190: 9591 e296 88e2 9688 e296 88e2 9688 e296  ................
+000001a0: 88e2 9688 e296 88e2 9597 0a23 20e2 9688  ...........# ...
+000001b0: e296 88e2 9591 2020 2020 20e2 9688 e296  ......     .....
+000001c0: 88e2 9591 2020 20e2 9688 e296 88e2 9591  ....   .........
+000001d0: 2020 20e2 9688 e296 88e2 9594 e295 90e2     .............
+000001e0: 9590 e296 88e2 9688 e295 97e2 9688 e296  ................
+000001f0: 88e2 9591 2020 20e2 9688 e296 88e2 9591  ....   .........
+00000200: e295 9ae2 9590 e295 90e2 9590 e295 90e2  ................
+00000210: 9688 e296 88e2 9591 0a23 20e2 959a e296  .........# .....
+00000220: 88e2 9688 e296 88e2 9688 e296 88e2 9688  ................
+00000230: e295 97e2 9688 e296 88e2 9591 2020 20e2  ............   .
+00000240: 9688 e296 88e2 9591 2020 20e2 9688 e296  ........   .....
+00000250: 88e2 9591 2020 e296 88e2 9688 e295 91e2  ....  ..........
+00000260: 959a e296 88e2 9688 e296 88e2 9688 e296  ................
+00000270: 88e2 9688 e295 94e2 959d e296 88e2 9688  ................
+00000280: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
+00000290: 9591 0a23 2020 e295 9ae2 9590 e295 90e2  ...#  ..........
+000002a0: 9590 e295 90e2 9590 e295 9de2 959a e295  ................
+000002b0: 90e2 959d 2020 20e2 959a e295 90e2 959d  ....   .........
+000002c0: 2020 20e2 959a e295 90e2 959d 2020 e295     .........  ..
+000002d0: 9ae2 9590 e295 9d20 e295 9ae2 9590 e295  ....... ........
+000002e0: 90e2 9590 e295 90e2 9590 e295 9d20 e295  ............. ..
+000002f0: 9ae2 9590 e295 90e2 9590 e295 90e2 9590  ................
+00000300: e295 90e2 959d 2020 2020 2020 2020 2020  ......          
+00000310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000320: 2020 2020 2020 2020 2020 2020 2020 0a23                .#
+00000330: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
+00000340: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000350: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
+00000360: 0a66 726f 6d20 2e6c 6175 6e63 6820 696d  .from .launch im
+00000370: 706f 7274 2067 656e 6572 6174 655f 6c61  port generate_la
+00000380: 756e 6368 5f64 6573 6372 6970 7469 6f6e  unch_description
+00000390: 0a0a 5f5f 616c 6c5f 5f20 3d20 5b0a 2020  ..__all__ = [.  
+000003a0: 2020 2020 2020 2767 6574 5f6c 6f67 6765        'get_logge
+000003b0: 7227 2c0a 2020 2020 2020 2020 2773 746f  r',.        'sto
+000003c0: 705f 6c6f 6767 6572 270a 5d0a            p_logger'.].
```

### Comparing `citros-23.14.2/bin/citros` & `citros-23.14.4/bin/citros`

 * *Files identical despite different names*

### Comparing `citros-23.14.2/citros/__init__.py` & `citros-23.14.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,29 @@
+Metadata-Version: 2.1
+Name: citros
+Version: 23.14.4
+Summary: A cli entypoint for citros system.
+Home-page: http://pypi.python.org/pypi/citros_cli/
+Author: vovacooper
+Author-email: vova@lulav.space
+License: LICENSE.txt
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+```python
 # ==============================================
-#  ██████╗██╗████████╗██████╗  ██████╗ ███████╗
-# ██╔════╝██║╚══██╔══╝██╔══██╗██╔═══██╗██╔════╝
-# ██║     ██║   ██║   ██████╔╝██║   ██║███████╗
-# ██║     ██║   ██║   ██╔══██╗██║   ██║╚════██║
-# ╚██████╗██║   ██║   ██║  ██║╚██████╔╝███████║
-#  ╚═════╝╚═╝   ╚═╝   ╚═╝  ╚═╝ ╚═════╝ ╚══════╝                                        
+#   ██████╗██╗████████╗██████╗  ██████╗ ███████╗
+#  ██╔════╝██║╚══██╔══╝██╔══██╗██╔═══██╗██╔════╝
+#  ██║     ██║   ██║   ██████╔╝██║   ██║███████╗
+#  ██║     ██║   ██║   ██╔══██╗██║   ██║╚════██║
+#  ╚██████╗██║   ██║   ██║  ██║╚██████╔╝███████║
+#   ╚═════╝╚═╝   ╚═╝   ╚═╝  ╚═╝ ╚═════╝ ╚══════╝                                        
 # ==============================================
+```
+# CiTROS CLI
 
-from .citros import Citros
+[![Publish CITROS_CLI to PyPI / GitHub](https://github.com/lulav/citros_cli/actions/workflows/release_to_pypi.yaml/badge.svg)](https://github.com/lulav/citros_cli/actions/workflows/release_to_pypi.yaml)
 
-__all__ = [
-        'Citros'
-]
+# description:
 
-__version__ = "unknown"
-try:
-    from citros_meta import __version__,__author__,__author_email__,__copyright__,__description__,__license__,__title__,__url__
-except ImportError:
-    # We're running in a tree that doesn't have a _version.py, so we don't know what our version is.
-    pass
+the CiTROS cli will run by the user. 
+inside the ros-project folder.
```

### Comparing `citros-23.14.2/citros/citros.py` & `citros-23.14.4/citros/citros.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.2/citros/citros_bag.py` & `citros-23.14.4/citros/citros_bag.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.2/citros/citros_batch.py` & `citros-23.14.4/citros/citros_batch.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.2/citros/citros_events.py` & `citros-23.14.4/citros/citros_events.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.2/citros/citros_integration.py` & `citros-23.14.4/citros/citros_integration.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.2/citros/citros_params.py` & `citros-23.14.4/citros/citros_params.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.2/citros/citros_utils.py` & `citros-23.14.4/citros/citros_utils.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.2/citros/launches/__init__.py` & `citros-23.14.4/citros/logger/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,13 +3,14 @@
 # ██╔════╝██║╚══██╔══╝██╔══██╗██╔═══██╗██╔════╝
 # ██║     ██║   ██║   ██████╔╝██║   ██║███████╗
 # ██║     ██║   ██║   ██╔══██╗██║   ██║╚════██║
 # ╚██████╗██║   ██║   ██║  ██║╚██████╔╝███████║
 #  ╚═════╝╚═╝   ╚═╝   ╚═╝  ╚═╝ ╚═════╝ ╚══════╝                                        
 # ==============================================
 
-from .launch import generate_launch_description
+from .logger import get_logger
+# , stop_logger
 
 __all__ = [
         'get_logger',
-        'stop_logger'
+        # 'stop_logger'
 ]
```

### Comparing `citros-23.14.2/citros/launches/launch.py` & `citros-23.14.4/citros/launches/launch.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.2/citros/logger/__init__.py` & `citros-23.14.4/citros/rosbag/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 # ██╔════╝██║╚══██╔══╝██╔══██╗██╔═══██╗██╔════╝
 # ██║     ██║   ██║   ██████╔╝██║   ██║███████╗
 # ██║     ██║   ██║   ██╔══██╗██║   ██║╚════██║
 # ╚██████╗██║   ██║   ██║  ██║╚██████╔╝███████║
 #  ╚═════╝╚═╝   ╚═╝   ╚═╝  ╚═╝ ╚═════╝ ╚══════╝                                        
 # ==============================================
 
-from .logger import get_logger
-# , stop_logger
+# from .citros import Citros
+
+
+from .reader_base import BagReader
+from .reader_mcap import BagReaderMcap
+from .reader_sqlite import BagReaderSQL
 
 __all__ = [
-        'get_logger',
-        # 'stop_logger'
+        'BagReader',
+        'BagReaderMcap',
+        'BagReaderSQL'
 ]
```

### Comparing `citros-23.14.2/citros/logger/logger.py` & `citros-23.14.4/citros/logger/logger.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.2/citros/logger/logger_pg_handler.py` & `citros-23.14.4/citros/logger/logger_pg_handler.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.2/citros/parsers/__init__.py` & `citros-23.14.4/citros/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.2/citros/parsers/parser_ros2.py` & `citros-23.14.4/citros/parsers/parser_ros2.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,18 +116,20 @@
             "license": license,
             "nodes": nodes
         }
     
     def get_project_packages(self, project_path, workspace=""):                
         self.log.debug(f" + get_project_packages {project_path}/{workspace}")
         
-        package_paths = glob.glob(f"{project_path}/src/[!ros2.*]*")                
+        package_paths = glob.glob(f"{project_path}/src/*")                
         if workspace != "":
             package_paths = glob.glob(f"{project_path}/{workspace}/src/*") + package_paths            
-                        
+        
+        package_paths = [p for p in package_paths if 'ros2.' in p]
+        
         packages = []
         for package_path in package_paths:            
             # package_py = f"{'/'.join(package_path.split('/')[:-1])}/setup.py"
             self.log.debug(f"package_path: {package_path}")
             
             parsed_data = None     
             try:
```

### Comparing `citros-23.14.2/citros/rosbag/__init__.py` & `citros-23.14.4/citros.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,29 @@
+Metadata-Version: 2.1
+Name: citros
+Version: 23.14.4
+Summary: A cli entypoint for citros system.
+Home-page: http://pypi.python.org/pypi/citros_cli/
+Author: vovacooper
+Author-email: vova@lulav.space
+License: LICENSE.txt
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+```python
 # ==============================================
-#  ██████╗██╗████████╗██████╗  ██████╗ ███████╗
-# ██╔════╝██║╚══██╔══╝██╔══██╗██╔═══██╗██╔════╝
-# ██║     ██║   ██║   ██████╔╝██║   ██║███████╗
-# ██║     ██║   ██║   ██╔══██╗██║   ██║╚════██║
-# ╚██████╗██║   ██║   ██║  ██║╚██████╔╝███████║
-#  ╚═════╝╚═╝   ╚═╝   ╚═╝  ╚═╝ ╚═════╝ ╚══════╝                                        
+#   ██████╗██╗████████╗██████╗  ██████╗ ███████╗
+#  ██╔════╝██║╚══██╔══╝██╔══██╗██╔═══██╗██╔════╝
+#  ██║     ██║   ██║   ██████╔╝██║   ██║███████╗
+#  ██║     ██║   ██║   ██╔══██╗██║   ██║╚════██║
+#  ╚██████╗██║   ██║   ██║  ██║╚██████╔╝███████║
+#   ╚═════╝╚═╝   ╚═╝   ╚═╝  ╚═╝ ╚═════╝ ╚══════╝                                        
 # ==============================================
+```
+# CiTROS CLI
 
-# from .citros import Citros
-
+[![Publish CITROS_CLI to PyPI / GitHub](https://github.com/lulav/citros_cli/actions/workflows/release_to_pypi.yaml/badge.svg)](https://github.com/lulav/citros_cli/actions/workflows/release_to_pypi.yaml)
 
-from .reader_base import BagReader
-from .reader_mcap import BagReaderMcap
-from .reader_sqlite import BagReaderSQL
+# description:
 
-__all__ = [
-        'BagReader',
-        'BagReaderMcap',
-        'BagReaderSQL'
-]
+the CiTROS cli will run by the user. 
+inside the ros-project folder.
```

### Comparing `citros-23.14.2/citros/rosbag/reader_base.py` & `citros-23.14.4/citros/rosbag/reader_base.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.2/citros/rosbag/reader_mcap.py` & `citros-23.14.4/citros/rosbag/reader_mcap.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.2/citros/rosbag/reader_sqlite.py` & `citros-23.14.4/citros/rosbag/reader_sqlite.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.2/citros.egg-info/PKG-INFO` & `citros-23.14.4/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,80 +1,75 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6369 7472  : 2.1.Name: citr
-00000020: 6f73 0a56 6572 7369 6f6e 3a20 3233 2e31  os.Version: 23.1
-00000030: 342e 320a 5375 6d6d 6172 793a 2041 2063  4.2.Summary: A c
-00000040: 6c69 2065 6e74 7970 6f69 6e74 2066 6f72  li entypoint for
-00000050: 2063 6974 726f 7320 7379 7374 656d 2e0a   citros system..
-00000060: 486f 6d65 2d70 6167 653a 2068 7474 703a  Home-page: http:
-00000070: 2f2f 7079 7069 2e70 7974 686f 6e2e 6f72  //pypi.python.or
-00000080: 672f 7079 7069 2f63 6974 726f 735f 636c  g/pypi/citros_cl
-00000090: 692f 0a41 7574 686f 723a 2076 6f76 6163  i/.Author: vovac
-000000a0: 6f6f 7065 720a 4175 7468 6f72 2d65 6d61  ooper.Author-ema
-000000b0: 696c 3a20 766f 7661 406c 756c 6176 2e73  il: vova@lulav.s
-000000c0: 7061 6365 0a4c 6963 656e 7365 3a20 4c49  pace.License: LI
-000000d0: 4345 4e53 452e 7478 740a 4465 7363 7269  CENSE.txt.Descri
-000000e0: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
-000000f0: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-00000100: 6e0a 4c69 6365 6e73 652d 4669 6c65 3a20  n.License-File: 
-00000110: 4c49 4345 4e53 450a 0a60 6060 7079 7468  LICENSE..```pyth
-00000120: 6f6e 0a23 203d 3d3d 3d3d 3d3d 3d3d 3d3d  on.# ===========
-00000130: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000140: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000150: 3d3d 3d0a 2320 2020 e296 88e2 9688 e296  ===.#   ........
-00000160: 88e2 9688 e296 88e2 9688 e295 97e2 9688  ................
-00000170: e296 88e2 9597 e296 88e2 9688 e296 88e2  ................
-00000180: 9688 e296 88e2 9688 e296 88e2 9688 e295  ................
-00000190: 97e2 9688 e296 88e2 9688 e296 88e2 9688  ................
-000001a0: e296 88e2 9597 2020 e296 88e2 9688 e296  ......  ........
-000001b0: 88e2 9688 e296 88e2 9688 e295 9720 e296  ............. ..
-000001c0: 88e2 9688 e296 88e2 9688 e296 88e2 9688  ................
-000001d0: e296 88e2 9597 0a23 2020 e296 88e2 9688  .......#  ......
-000001e0: e295 94e2 9590 e295 90e2 9590 e295 90e2  ................
-000001f0: 959d e296 88e2 9688 e295 91e2 959a e295  ................
-00000200: 90e2 9590 e296 88e2 9688 e295 94e2 9590  ................
-00000210: e295 90e2 959d e296 88e2 9688 e295 94e2  ................
-00000220: 9590 e295 90e2 9688 e296 88e2 9597 e296  ................
-00000230: 88e2 9688 e295 94e2 9590 e295 90e2 9590  ................
-00000240: e296 88e2 9688 e295 97e2 9688 e296 88e2  ................
-00000250: 9594 e295 90e2 9590 e295 90e2 9590 e295  ................
-00000260: 9d0a 2320 20e2 9688 e296 88e2 9591 2020  ..#  .........  
-00000270: 2020 20e2 9688 e296 88e2 9591 2020 20e2     .........   .
-00000280: 9688 e296 88e2 9591 2020 20e2 9688 e296  ........   .....
-00000290: 88e2 9688 e296 88e2 9688 e296 88e2 9594  ................
-000002a0: e295 9de2 9688 e296 88e2 9591 2020 20e2  ............   .
-000002b0: 9688 e296 88e2 9591 e296 88e2 9688 e296  ................
-000002c0: 88e2 9688 e296 88e2 9688 e296 88e2 9597  ................
-000002d0: 0a23 2020 e296 88e2 9688 e295 9120 2020  .#  .........   
-000002e0: 2020 e296 88e2 9688 e295 9120 2020 e296    .........   ..
-000002f0: 88e2 9688 e295 9120 2020 e296 88e2 9688  .......   ......
-00000300: e295 94e2 9590 e295 90e2 9688 e296 88e2  ................
-00000310: 9597 e296 88e2 9688 e295 9120 2020 e296  ...........   ..
-00000320: 88e2 9688 e295 91e2 959a e295 90e2 9590  ................
-00000330: e295 90e2 9590 e296 88e2 9688 e295 910a  ................
-00000340: 2320 20e2 959a e296 88e2 9688 e296 88e2  #  .............
-00000350: 9688 e296 88e2 9688 e295 97e2 9688 e296  ................
-00000360: 88e2 9591 2020 20e2 9688 e296 88e2 9591  ....   .........
-00000370: 2020 20e2 9688 e296 88e2 9591 2020 e296     .........  ..
-00000380: 88e2 9688 e295 91e2 959a e296 88e2 9688  ................
-00000390: e296 88e2 9688 e296 88e2 9688 e295 94e2  ................
-000003a0: 959d e296 88e2 9688 e296 88e2 9688 e296  ................
-000003b0: 88e2 9688 e296 88e2 9591 0a23 2020 20e2  ...........#   .
-000003c0: 959a e295 90e2 9590 e295 90e2 9590 e295  ................
-000003d0: 90e2 959d e295 9ae2 9590 e295 9d20 2020  .............   
-000003e0: e295 9ae2 9590 e295 9d20 2020 e295 9ae2  .........   ....
-000003f0: 9590 e295 9d20 20e2 959a e295 90e2 959d  .....  .........
-00000400: 20e2 959a e295 90e2 9590 e295 90e2 9590   ...............
-00000410: e295 90e2 959d 20e2 959a e295 90e2 9590  ...... .........
-00000420: e295 90e2 9590 e295 90e2 9590 e295 9d20  ............... 
-00000430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000450: 2020 2020 2020 200a 2320 3d3d 3d3d 3d3d         .# ======
-00000460: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000470: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000480: 3d3d 3d3d 3d3d 3d3d 0a60 6060 0a23 2043  ========.```.# C
-00000490: 6954 524f 5320 434c 490a 0a23 2064 6573  iTROS CLI..# des
-000004a0: 6372 6970 7469 6f6e 3a0a 0a74 6865 2043  cription:..the C
-000004b0: 6954 524f 5320 636c 6920 7769 6c6c 2072  iTROS cli will r
-000004c0: 756e 2062 7920 7468 6520 7573 6572 2e20  un by the user. 
-000004d0: 0a69 6e73 6964 6520 7468 6520 726f 732d  .inside the ros-
-000004e0: 7072 6f6a 6563 7420 666f 6c64 6572 2e20  project folder. 
-000004f0: 0a                                       .
+00000000: 6060 6070 7974 686f 6e0a 2320 3d3d 3d3d  ```python.# ====
+00000010: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000020: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000030: 3d3d 3d3d 3d3d 3d3d 3d3d 0a23 2020 20e2  ==========.#   .
+00000040: 9688 e296 88e2 9688 e296 88e2 9688 e296  ................
+00000050: 88e2 9597 e296 88e2 9688 e295 97e2 9688  ................
+00000060: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
+00000070: 9688 e296 88e2 9597 e296 88e2 9688 e296  ................
+00000080: 88e2 9688 e296 88e2 9688 e295 9720 20e2  .............  .
+00000090: 9688 e296 88e2 9688 e296 88e2 9688 e296  ................
+000000a0: 88e2 9597 20e2 9688 e296 88e2 9688 e296  .... ...........
+000000b0: 88e2 9688 e296 88e2 9688 e295 970a 2320  ..............# 
+000000c0: 20e2 9688 e296 88e2 9594 e295 90e2 9590   ...............
+000000d0: e295 90e2 9590 e295 9de2 9688 e296 88e2  ................
+000000e0: 9591 e295 9ae2 9590 e295 90e2 9688 e296  ................
+000000f0: 88e2 9594 e295 90e2 9590 e295 9de2 9688  ................
+00000100: e296 88e2 9594 e295 90e2 9590 e296 88e2  ................
+00000110: 9688 e295 97e2 9688 e296 88e2 9594 e295  ................
+00000120: 90e2 9590 e295 90e2 9688 e296 88e2 9597  ................
+00000130: e296 88e2 9688 e295 94e2 9590 e295 90e2  ................
+00000140: 9590 e295 90e2 959d 0a23 2020 e296 88e2  .........#  ....
+00000150: 9688 e295 9120 2020 2020 e296 88e2 9688  .....     ......
+00000160: e295 9120 2020 e296 88e2 9688 e295 9120  ...   ......... 
+00000170: 2020 e296 88e2 9688 e296 88e2 9688 e296    ..............
+00000180: 88e2 9688 e295 94e2 959d e296 88e2 9688  ................
+00000190: e295 9120 2020 e296 88e2 9688 e295 91e2  ...   ..........
+000001a0: 9688 e296 88e2 9688 e296 88e2 9688 e296  ................
+000001b0: 88e2 9688 e295 970a 2320 20e2 9688 e296  ........#  .....
+000001c0: 88e2 9591 2020 2020 20e2 9688 e296 88e2  ....     .......
+000001d0: 9591 2020 20e2 9688 e296 88e2 9591 2020  ..   .........  
+000001e0: 20e2 9688 e296 88e2 9594 e295 90e2 9590   ...............
+000001f0: e296 88e2 9688 e295 97e2 9688 e296 88e2  ................
+00000200: 9591 2020 20e2 9688 e296 88e2 9591 e295  ..   ...........
+00000210: 9ae2 9590 e295 90e2 9590 e295 90e2 9688  ................
+00000220: e296 88e2 9591 0a23 2020 e295 9ae2 9688  .......#  ......
+00000230: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
+00000240: 9597 e296 88e2 9688 e295 9120 2020 e296  ...........   ..
+00000250: 88e2 9688 e295 9120 2020 e296 88e2 9688  .......   ......
+00000260: e295 9120 20e2 9688 e296 88e2 9591 e295  ...  ...........
+00000270: 9ae2 9688 e296 88e2 9688 e296 88e2 9688  ................
+00000280: e296 88e2 9594 e295 9de2 9688 e296 88e2  ................
+00000290: 9688 e296 88e2 9688 e296 88e2 9688 e295  ................
+000002a0: 910a 2320 2020 e295 9ae2 9590 e295 90e2  ..#   ..........
+000002b0: 9590 e295 90e2 9590 e295 9de2 959a e295  ................
+000002c0: 90e2 959d 2020 20e2 959a e295 90e2 959d  ....   .........
+000002d0: 2020 20e2 959a e295 90e2 959d 2020 e295     .........  ..
+000002e0: 9ae2 9590 e295 9d20 e295 9ae2 9590 e295  ....... ........
+000002f0: 90e2 9590 e295 90e2 9590 e295 9d20 e295  ............. ..
+00000300: 9ae2 9590 e295 90e2 9590 e295 90e2 9590  ................
+00000310: e295 90e2 959d 2020 2020 2020 2020 2020  ......          
+00000320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000330: 2020 2020 2020 2020 2020 2020 2020 0a23                .#
+00000340: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
+00000350: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000360: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
+00000370: 6060 600a 2320 4369 5452 4f53 2043 4c49  ```.# CiTROS CLI
+00000380: 0a0a 5b21 5b50 7562 6c69 7368 2043 4954  ..[![Publish CIT
+00000390: 524f 535f 434c 4920 746f 2050 7950 4920  ROS_CLI to PyPI 
+000003a0: 2f20 4769 7448 7562 5d28 6874 7470 733a  / GitHub](https:
+000003b0: 2f2f 6769 7468 7562 2e63 6f6d 2f6c 756c  //github.com/lul
+000003c0: 6176 2f63 6974 726f 735f 636c 692f 6163  av/citros_cli/ac
+000003d0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+000003e0: 7265 6c65 6173 655f 746f 5f70 7970 692e  release_to_pypi.
+000003f0: 7961 6d6c 2f62 6164 6765 2e73 7667 295d  yaml/badge.svg)]
+00000400: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000410: 636f 6d2f 6c75 6c61 762f 6369 7472 6f73  com/lulav/citros
+00000420: 5f63 6c69 2f61 6374 696f 6e73 2f77 6f72  _cli/actions/wor
+00000430: 6b66 6c6f 7773 2f72 656c 6561 7365 5f74  kflows/release_t
+00000440: 6f5f 7079 7069 2e79 616d 6c29 0a0a 2320  o_pypi.yaml)..# 
+00000450: 6465 7363 7269 7074 696f 6e3a 0a0a 7468  description:..th
+00000460: 6520 4369 5452 4f53 2063 6c69 2077 696c  e CiTROS cli wil
+00000470: 6c20 7275 6e20 6279 2074 6865 2075 7365  l run by the use
+00000480: 722e 200a 696e 7369 6465 2074 6865 2072  r. .inside the r
+00000490: 6f73 2d70 726f 6a65 6374 2066 6f6c 6465  os-project folde
+000004a0: 722e 200a                                r. .
```

### Comparing `citros-23.14.2/citros.egg-info/SOURCES.txt` & `citros-23.14.4/citros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citros-23.14.2/setup.py` & `citros-23.14.4/setup.py`

 * *Files identical despite different names*

