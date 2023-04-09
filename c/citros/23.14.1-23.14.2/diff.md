# Comparing `tmp/citros-23.14.1.tar.gz` & `tmp/citros-23.14.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citros-23.14.1.tar", last modified: Tue Apr  4 07:41:10 2023, max compression
+gzip compressed data, was "citros-23.14.2.tar", last modified: Sun Apr  9 08:05:34 2023, max compression
```

## Comparing `citros-23.14.1.tar` & `citros-23.14.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:41:10.158820 citros-23.14.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-04 07:40:52.000000 citros-23.14.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-04 07:41:10.158820 citros-23.14.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-04 07:40:52.000000 citros-23.14.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:41:10.154820 citros-23.14.1/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-04 07:40:52.000000 citros-23.14.1/bin/citros
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:41:10.154820 citros-23.14.1/citros/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-04 07:40:52.000000 citros-23.14.1/citros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-04 07:40:52.000000 citros-23.14.1/citros/citros.py
--rw-r--r--   0 runner    (1001) docker     (123)    13261 2023-04-04 07:40:52.000000 citros-23.14.1/citros/citros_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-04 07:40:52.000000 citros-23.14.1/citros/citros_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-04-04 07:40:52.000000 citros-23.14.1/citros/citros_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-04 07:40:52.000000 citros-23.14.1/citros/citros_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-04-04 07:40:52.000000 citros-23.14.1/citros/citros_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-04 07:40:52.000000 citros-23.14.1/citros/citros_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:41:10.154820 citros-23.14.1/citros/launches/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-04 07:40:52.000000 citros-23.14.1/citros/launches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-04-04 07:40:52.000000 citros-23.14.1/citros/launches/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:41:10.154820 citros-23.14.1/citros/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-04 07:40:52.000000 citros-23.14.1/citros/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-04 07:40:52.000000 citros-23.14.1/citros/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-04 07:40:52.000000 citros-23.14.1/citros/logger/logger_pg_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:41:10.154820 citros-23.14.1/citros/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-04 07:40:52.000000 citros-23.14.1/citros/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-04 07:40:52.000000 citros-23.14.1/citros/parsers/parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-04-04 07:40:52.000000 citros-23.14.1/citros/parsers/parser_ros2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:41:10.158820 citros-23.14.1/citros/rosbag/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-04 07:40:52.000000 citros-23.14.1/citros/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-04 07:40:52.000000 citros-23.14.1/citros/rosbag/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-04 07:40:52.000000 citros-23.14.1/citros/rosbag/reader_mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-04 07:40:52.000000 citros-23.14.1/citros/rosbag/reader_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:41:10.154820 citros-23.14.1/citros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-04 07:41:10.000000 citros-23.14.1/citros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-04 07:41:10.000000 citros-23.14.1/citros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 07:41:10.000000 citros-23.14.1/citros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-04 07:41:10.000000 citros-23.14.1/citros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-04 07:41:10.000000 citros-23.14.1/citros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-04 07:40:52.000000 citros-23.14.1/citros_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 07:41:10.158820 citros-23.14.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-04 07:40:52.000000 citros-23.14.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:41:10.158820 citros-23.14.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 07:40:52.000000 citros-23.14.1/tests/test_parse_ros_project.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 07:40:52.000000 citros-23.14.1/tests/test_uplosd_to_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:34.586971 citros-23.14.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 08:05:17.000000 citros-23.14.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-09 08:05:34.586971 citros-23.14.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-09 08:05:17.000000 citros-23.14.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:34.582971 citros-23.14.2/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-09 08:05:17.000000 citros-23.14.2/bin/citros
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:34.582971 citros-23.14.2/citros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-09 08:05:17.000000 citros-23.14.2/citros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-09 08:05:17.000000 citros-23.14.2/citros/citros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-04-09 08:05:17.000000 citros-23.14.2/citros/citros_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-09 08:05:17.000000 citros-23.14.2/citros/citros_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-04-09 08:05:17.000000 citros-23.14.2/citros/citros_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-09 08:05:17.000000 citros-23.14.2/citros/citros_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-04-09 08:05:17.000000 citros-23.14.2/citros/citros_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-09 08:05:17.000000 citros-23.14.2/citros/citros_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:34.582971 citros-23.14.2/citros/launches/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-09 08:05:17.000000 citros-23.14.2/citros/launches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-04-09 08:05:17.000000 citros-23.14.2/citros/launches/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:34.582971 citros-23.14.2/citros/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-09 08:05:17.000000 citros-23.14.2/citros/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-09 08:05:17.000000 citros-23.14.2/citros/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-09 08:05:17.000000 citros-23.14.2/citros/logger/logger_pg_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:34.582971 citros-23.14.2/citros/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-09 08:05:17.000000 citros-23.14.2/citros/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-09 08:05:17.000000 citros-23.14.2/citros/parsers/parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-04-09 08:05:17.000000 citros-23.14.2/citros/parsers/parser_ros2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:34.586971 citros-23.14.2/citros/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-09 08:05:17.000000 citros-23.14.2/citros/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-09 08:05:17.000000 citros-23.14.2/citros/rosbag/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-09 08:05:17.000000 citros-23.14.2/citros/rosbag/reader_mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-09 08:05:17.000000 citros-23.14.2/citros/rosbag/reader_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:34.582971 citros-23.14.2/citros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-09 08:05:34.000000 citros-23.14.2/citros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-09 08:05:34.000000 citros-23.14.2/citros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 08:05:34.000000 citros-23.14.2/citros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-09 08:05:34.000000 citros-23.14.2/citros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-09 08:05:34.000000 citros-23.14.2/citros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-09 08:05:17.000000 citros-23.14.2/citros_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 08:05:34.586971 citros-23.14.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-09 08:05:17.000000 citros-23.14.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:34.586971 citros-23.14.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:17.000000 citros-23.14.2/tests/test_parse_ros_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:05:17.000000 citros-23.14.2/tests/test_uplosd_to_server.py
```

### Comparing `citros-23.14.1/LICENSE` & `citros-23.14.2/LICENSE`

 * *Files identical despite different names*

### Comparing `citros-23.14.1/PKG-INFO` & `citros-23.14.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.14.1
+Version: 23.14.2
 Summary: A cli entypoint for citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.14.1/README.md` & `citros-23.14.2/README.md`

 * *Files identical despite different names*

### Comparing `citros-23.14.1/bin/citros` & `citros-23.14.2/bin/citros`

 * *Files identical despite different names*

### Comparing `citros-23.14.1/citros/__init__.py` & `citros-23.14.2/citros/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.1/citros/citros.py` & `citros-23.14.2/citros/citros.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.1/citros/citros_bag.py` & `citros-23.14.2/citros/citros_bag.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from pathlib import Path
 import traceback
 import datetime 
 import json
 import yaml
 import os
 
-from .rosbag import BagReader
+# from .rosbag import BagReader
+from .rosbag import BagReaderSQL
 
 ###########################
 #           BAGd
 ###########################  
 class citros_bag():
     def __init__(self, citros):     
         self.citros = citros
@@ -157,35 +158,37 @@
                 # print(postgres_insert_query, record_to_insert)
                 
                 cursor.execute(postgres_insert_query, record_to_insert)                                                        
                 connection.commit()                                 
             
             #####################
             # Uploading data
-            #####################             
-            bagReader = BagReader()                        
-            print(f"[{datetime.datetime.now()}] + read_messages", flush=True)
-            buffer = bagReader.read_messages(path_to_bag, simulation_run_id)            
-            print(f"[{datetime.datetime.now()}] - read_messages", flush=True)            
-            buffer.seek(0, os.SEEK_END)
-            size = buffer.tell()                
-            buffer.seek(0)
-            print(f"[{datetime.datetime.now()}] SET search_path TO data_bucket", flush=True)                                             
-            cursor.execute(f'SET search_path TO data_bucket')
-            print(f"[{datetime.datetime.now()}] inserting buffer size:", size, flush=True)                                             
-            cursor.copy_from(buffer, batch_run_id, sep=chr(0x1E), columns=['sid', 'rid', 'time', 'topic', 'type', 'data'])
-            print(f"[{datetime.datetime.now()}] after copy_from", flush=True)                 
-            connection.commit()                   
-            print(f"[{datetime.datetime.now()}] --- done", flush=True)                     
-            return True, f"success, uploaded [{path_to_metadata}],[{path_to_bag}] to Postgres. [size: {size}]", None                
+            #####################  
+            print(f"[{datetime.datetime.now()}] +++ uploading bag to PG", flush=True)
+            bagReader = BagReaderSQL()
+            total_size = 0
+            for buffer in bagReader.read_messages(path_to_bag, simulation_run_id):
+                # print(f"[{datetime.datetime.now()}] + read_messages", flush=True)
+                size = buffer.seek(0, os.SEEK_END)
+                size = buffer.tell()
+                total_size = total_size + size
+                buffer.seek(0)
+                cursor.execute(f'SET search_path TO data_bucket')                
+                cursor.copy_from(buffer, batch_run_id, sep=chr(0x1E), columns=['sid', 'rid', 'time', 'topic', 'type', 'data'])
+                print(f"[{datetime.datetime.now()}] \tinserting buffer size: { (size / 1024 ) / 1024 } MB", flush=True)                
+                # buffer.truncate(0)
+                # buffer.seek(0)
+                # buffer.close()
+                connection.commit()
+            print(f"[{datetime.datetime.now()}] --- done uploading to PG", flush=True)
+            return True, f"success, uploaded [{path_to_metadata}],[{path_to_bag}] to Postgres. [size: {(total_size / 1024)/1024} MB]", None
         except (Exception, psycopg2.Error) as error:
-            print(f"[{datetime.datetime.now()}] Failed to insert record into table, aboring uploading to PG DB.", error)               
+            print(f"[{datetime.datetime.now()}] Failed to insert record into table, aboring uploading to PG DB.", error) 
             print(traceback.format_exc())
-            return False, "go exception from pgdb" , error       
-
+            return False, "go exception from pgdb", error
         finally:
             # closing database connection.
             if connection:
                 cursor.close()
                 connection.close()
                 print(f"[{datetime.datetime.now()}] PostgreSQL connection is closed")
```

### Comparing `citros-23.14.1/citros/citros_batch.py` & `citros-23.14.2/citros/citros_batch.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.1/citros/citros_events.py` & `citros-23.14.2/citros/citros_events.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.1/citros/citros_integration.py` & `citros-23.14.2/citros/citros_integration.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.1/citros/citros_params.py` & `citros-23.14.2/citros/citros_params.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.1/citros/citros_utils.py` & `citros-23.14.2/citros/citros_utils.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.1/citros/launches/__init__.py` & `citros-23.14.2/citros/launches/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.1/citros/launches/launch.py` & `citros-23.14.2/citros/launches/launch.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.1/citros/logger/__init__.py` & `citros-23.14.2/citros/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.1/citros/logger/logger.py` & `citros-23.14.2/citros/logger/logger.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.1/citros/logger/logger_pg_handler.py` & `citros-23.14.2/citros/logger/logger_pg_handler.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.1/citros/parsers/__init__.py` & `citros-23.14.2/citros/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.1/citros/parsers/parser_ros2.py` & `citros-23.14.2/citros/parsers/parser_ros2.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,23 +114,24 @@
             "maintainer_email": maintainer_email,
             "description": description,
             "license": license,
             "nodes": nodes
         }
     
     def get_project_packages(self, project_path, workspace=""):                
-        self.log.debug(f"get_project_packages {project_path}/{workspace}")
+        self.log.debug(f" + get_project_packages {project_path}/{workspace}")
         
         package_paths = glob.glob(f"{project_path}/src/[!ros2.*]*")                
         if workspace != "":
             package_paths = glob.glob(f"{project_path}/{workspace}/src/*") + package_paths            
                         
         packages = []
         for package_path in package_paths:            
             # package_py = f"{'/'.join(package_path.split('/')[:-1])}/setup.py"
+            self.log.debug(f"package_path: {package_path}")
             
             parsed_data = None     
             try:
                 parsed_data = self.parse_xml(package_path)
             except Exception as e:
                 print(f"{package_path} doesn't contain xml, probably not a package. skipping.")
                 continue
@@ -142,14 +143,15 @@
                 
             elif parsed_data["build_type"] == "ament_cmake":          
                 temp = self.parse_makefile(package_path)
                 parsed_data["nodes"] = temp["nodes"]
                 parsed_data["cmake"] = temp["cmake"]                
                 
             else:
+                self.log.exception(f"Method {parsed_data['build_type']} not allowed")
                 raise Exception(f"Method {parsed_data['build_type']} not allowed")
 
             node_parameters = {}
             try:
                 path_to_config =  f"{package_path}/config/params.yaml"            
                 with open(path_to_config, 'r') as config_file:
                     config = yaml.full_load(config_file)
```

### Comparing `citros-23.14.1/citros/rosbag/__init__.py` & `citros-23.14.2/citros/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.1/citros/rosbag/reader_base.py` & `citros-23.14.2/citros/rosbag/reader_base.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.1/citros/rosbag/reader_mcap.py` & `citros-23.14.2/citros/rosbag/reader_mcap.py`

 * *Files identical despite different names*

### Comparing `citros-23.14.1/citros.egg-info/PKG-INFO` & `citros-23.14.2/citros.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.14.1
+Version: 23.14.2
 Summary: A cli entypoint for citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.14.1/citros.egg-info/SOURCES.txt` & `citros-23.14.2/citros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citros-23.14.1/setup.py` & `citros-23.14.2/setup.py`

 * *Files identical despite different names*

