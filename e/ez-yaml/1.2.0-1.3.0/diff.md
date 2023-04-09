# Comparing `tmp/ez_yaml-1.2.0.tar.gz` & `tmp/ez_yaml-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ez_yaml-1.2.0.tar", last modified: Fri Mar 11 16:29:24 2022, max compression
+gzip compressed data, was "ez_yaml-1.3.0.tar", last modified: Sun Apr  9 03:55:54 2023, max compression
```

## Comparing `ez_yaml-1.2.0.tar` & `ez_yaml-1.3.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-03-11 16:29:24.573257 ez_yaml-1.2.0/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      953 2022-03-11 16:29:24.572720 ez_yaml-1.2.0/PKG-INFO
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-03-11 16:29:24.566332 ez_yaml-1.2.0/ez_yaml/
--rw-r--r--   0 jeffhykin   (501) staff       (20)       30 2021-07-27 19:25:46.000000 ez_yaml-1.2.0/ez_yaml/__init__.py
--rw-r--r--   0 jeffhykin   (501) staff       (20)     6923 2022-03-11 16:28:24.000000 ez_yaml-1.2.0/ez_yaml/ez_yaml.py
-drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2022-03-11 16:29:24.571595 ez_yaml-1.2.0/ez_yaml.egg-info/
--rw-r--r--   0 jeffhykin   (501) staff       (20)      953 2022-03-11 16:29:24.000000 ez_yaml-1.2.0/ez_yaml.egg-info/PKG-INFO
--rw-r--r--   0 jeffhykin   (501) staff       (20)      201 2022-03-11 16:29:24.000000 ez_yaml-1.2.0/ez_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2022-03-11 16:29:24.000000 ez_yaml-1.2.0/ez_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       12 2022-03-11 16:29:24.000000 ez_yaml-1.2.0/ez_yaml.egg-info/requires.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)        8 2022-03-11 16:29:24.000000 ez_yaml-1.2.0/ez_yaml.egg-info/top_level.txt
--rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2022-03-11 16:29:24.573407 ez_yaml-1.2.0/setup.cfg
--rw-r--r--   0 jeffhykin   (501) staff       (20)     1276 2022-03-11 16:26:26.000000 ez_yaml-1.2.0/setup.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-09 03:55:54.806225 ez_yaml-1.3.0/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      718 2023-04-09 03:55:54.806084 ez_yaml-1.3.0/PKG-INFO
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-09 03:55:54.805158 ez_yaml-1.3.0/ez_yaml/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       30 2022-12-02 18:23:22.000000 ez_yaml-1.3.0/ez_yaml/__init__.py
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     6984 2023-04-09 03:54:41.000000 ez_yaml-1.3.0/ez_yaml/ez_yaml.py
+drwxr-xr-x   0 jeffhykin   (501) staff       (20)        0 2023-04-09 03:55:54.805880 ez_yaml-1.3.0/ez_yaml.egg-info/
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      718 2023-04-09 03:55:54.000000 ez_yaml-1.3.0/ez_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 jeffhykin   (501) staff       (20)      171 2023-04-09 03:55:54.000000 ez_yaml-1.3.0/ez_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        1 2023-04-09 03:55:54.000000 ez_yaml-1.3.0/ez_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)        8 2023-04-09 03:55:54.000000 ez_yaml-1.3.0/ez_yaml.egg-info/top_level.txt
+-rw-r--r--   0 jeffhykin   (501) staff       (20)       38 2023-04-09 03:55:54.806269 ez_yaml-1.3.0/setup.cfg
+-rw-r--r--   0 jeffhykin   (501) staff       (20)     1158 2023-04-09 03:44:06.000000 ez_yaml-1.3.0/setup.py
```

### Comparing `ez_yaml-1.2.0/PKG-INFO` & `ez_yaml-1.3.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: ez_yaml
-Version: 1.2.0
+Version: 1.3.0
 Summary: Straighforward wrapper around Ruamel Yaml
 Home-page: https://github.com/jeff-hykin/ez_yaml
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
-Description: # Install
-        
-        `pip install ez_yaml`
-        
-        # Use
-        
-        ```python
-        import ez_yaml
-        
-        # to_string(obj, options={})
-        ez_yaml.to_string({"thing": 1, "abc": [ 1,2,3 ]})
-        
-        # to_object(file_path, options={})
-        # to_object(string   , options={})
-        ez_yaml.to_object(string='''
-        
-        thing: 1
-        abc:
-            - 1
-            - 2
-            - 3
-        
-        ''')
-        
-        # to_file(obj, file_path, options={})
-        ez_yaml.to_file(
-            {"thing": 1, "abc": [ 1,2,3 ]},
-            file_path="./my_file.yaml",
-        )
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+
+# Install
+
+`pip install ez_yaml`
+
+# Use
+
+```python
+import ez_yaml
+
+# to_string(obj, options={})
+ez_yaml.to_string({"thing": 1, "abc": [ 1,2,3 ]})
+
+# to_object(file_path, options={})
+# to_object(string   , options={})
+ez_yaml.to_object(string='''
+
+thing: 1
+abc:
+    - 1
+    - 2
+    - 3
+
+''')
+
+# to_file(obj, file_path, options={})
+ez_yaml.to_file(
+    {"thing": 1, "abc": [ 1,2,3 ]},
+    file_path="./my_file.yaml",
+)
+
```

### Comparing `ez_yaml-1.2.0/ez_yaml/ez_yaml.py` & `ez_yaml-1.3.0/ez_yaml/ez_yaml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import ruamel.yaml
+from .__dependencies__ import ruamel 
+from .__dependencies__.ruamel import yaml
 from io import StringIO
 from pathlib import Path
 import os
 
 # setup loader (basically options)
 yaml = ruamel.yaml.YAML()
 yaml.version = (1, 2)
```

### Comparing `ez_yaml-1.2.0/ez_yaml.egg-info/PKG-INFO` & `ez_yaml-1.3.0/ez_yaml.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: ez-yaml
-Version: 1.2.0
+Version: 1.3.0
 Summary: Straighforward wrapper around Ruamel Yaml
 Home-page: https://github.com/jeff-hykin/ez_yaml
 Author: Jeff Hykin
 Author-email: jeff.hykin@gmail.com
 License: MIT
-Description: # Install
-        
-        `pip install ez_yaml`
-        
-        # Use
-        
-        ```python
-        import ez_yaml
-        
-        # to_string(obj, options={})
-        ez_yaml.to_string({"thing": 1, "abc": [ 1,2,3 ]})
-        
-        # to_object(file_path, options={})
-        # to_object(string   , options={})
-        ez_yaml.to_object(string='''
-        
-        thing: 1
-        abc:
-            - 1
-            - 2
-            - 3
-        
-        ''')
-        
-        # to_file(obj, file_path, options={})
-        ez_yaml.to_file(
-            {"thing": 1, "abc": [ 1,2,3 ]},
-            file_path="./my_file.yaml",
-        )
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+
+# Install
+
+`pip install ez_yaml`
+
+# Use
+
+```python
+import ez_yaml
+
+# to_string(obj, options={})
+ez_yaml.to_string({"thing": 1, "abc": [ 1,2,3 ]})
+
+# to_object(file_path, options={})
+# to_object(string   , options={})
+ez_yaml.to_object(string='''
+
+thing: 1
+abc:
+    - 1
+    - 2
+    - 3
+
+''')
+
+# to_file(obj, file_path, options={})
+ez_yaml.to_file(
+    {"thing": 1, "abc": [ 1,2,3 ]},
+    file_path="./my_file.yaml",
+)
+
```

### Comparing `ez_yaml-1.2.0/setup.py` & `ez_yaml-1.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,19 +22,15 @@
     description=package_info["description"],
     url=package_info["url"],
     author=package_info["author"],
     author_email=package_info["author_email"],
     license=package_info["license"],
     packages=[package_info["name"]],
     install_requires=[
-        "ruamel.yaml", # tested on 0.17.21"
-        # examples:
-        # 'aiohttp >= 3.7.4',
-        # 'python-socketio >= 5.3.0',
-        # 'requests == 2.26.0',
+        # "ruamel.yaml", # tested on 0.17.21"
     ],
     classifiers=[
         # examples:
         # 'Development Status :: 5 - Production/Stable',
         # 'Intended Audience :: Developers',
         # 'Programming Language :: Python',
         # "Programming Language :: Python :: 3",
```

