# Comparing `tmp/Uname_sridhar-0.0.3.tar.gz` & `tmp/Uname_sridhar-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Uname_sridhar-0.0.3.tar", last modified: Sun Apr  9 02:09:07 2023, max compression
+gzip compressed data, was "Uname_sridhar-0.0.4.tar", last modified: Sun Apr  9 02:24:26 2023, max compression
```

## Comparing `Uname_sridhar-0.0.3.tar` & `Uname_sridhar-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-09 02:09:07.001916 Uname_sridhar-0.0.3/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      590 2023-04-09 02:09:07.001916 Uname_sridhar-0.0.3/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      267 2023-04-09 01:42:28.000000 Uname_sridhar-0.0.3/README.md
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-09 02:09:07.001916 Uname_sridhar-0.0.3/Uname_sridhar.egg-info/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      590 2023-04-09 02:09:06.000000 Uname_sridhar-0.0.3/Uname_sridhar.egg-info/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      236 2023-04-09 02:09:06.000000 Uname_sridhar-0.0.3/Uname_sridhar.egg-info/SOURCES.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-04-09 02:09:06.000000 Uname_sridhar-0.0.3/Uname_sridhar.egg-info/dependency_links.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       46 2023-04-09 02:09:06.000000 Uname_sridhar-0.0.3/Uname_sridhar.egg-info/entry_points.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        5 2023-04-09 02:09:06.000000 Uname_sridhar-0.0.3/Uname_sridhar.egg-info/top_level.txt
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-09 02:09:07.001916 Uname_sridhar-0.0.3/main/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-09 01:42:29.000000 Uname_sridhar-0.0.3/main/__init__.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1318 2023-04-09 01:42:30.000000 Uname_sridhar-0.0.3/main/main.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-09 02:09:07.001916 Uname_sridhar-0.0.3/setup.cfg
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      633 2023-04-09 02:08:30.000000 Uname_sridhar-0.0.3/setup.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-09 02:24:25.996666 Uname_sridhar-0.0.4/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      594 2023-04-09 02:24:25.996666 Uname_sridhar-0.0.4/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      271 2023-04-09 02:23:20.000000 Uname_sridhar-0.0.4/README.md
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-09 02:24:25.996666 Uname_sridhar-0.0.4/Uname_sridhar.egg-info/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      594 2023-04-09 02:24:25.000000 Uname_sridhar-0.0.4/Uname_sridhar.egg-info/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      236 2023-04-09 02:24:25.000000 Uname_sridhar-0.0.4/Uname_sridhar.egg-info/SOURCES.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-04-09 02:24:25.000000 Uname_sridhar-0.0.4/Uname_sridhar.egg-info/dependency_links.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       46 2023-04-09 02:24:25.000000 Uname_sridhar-0.0.4/Uname_sridhar.egg-info/entry_points.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        5 2023-04-09 02:24:25.000000 Uname_sridhar-0.0.4/Uname_sridhar.egg-info/top_level.txt
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-09 02:24:25.996666 Uname_sridhar-0.0.4/main/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-09 01:42:29.000000 Uname_sridhar-0.0.4/main/__init__.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1318 2023-04-09 01:42:30.000000 Uname_sridhar-0.0.4/main/main.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-09 02:24:25.996666 Uname_sridhar-0.0.4/setup.cfg
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      633 2023-04-09 02:24:05.000000 Uname_sridhar-0.0.4/setup.py
```

### Comparing `Uname_sridhar-0.0.3/PKG-INFO` & `Uname_sridhar-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Uname_sridhar
-Version: 0.0.3
+Version: 0.0.4
 Summary: Get Information About Current Linux Kernel With Python
 Home-page: https://git.selfmade.ninja/SRIDHARDSCV/package_uname_command
 Author: Sridhar
 Author-email: dcsvsridhar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -23,12 +23,12 @@
 
 
 
 #### Usage
 
 To get all available info about Linux Commands and Type of Linux Commands
 ```
- Uname [Option..]
+ Uname_cli [Option..]
 
 ```
```

### Comparing `Uname_sridhar-0.0.3/Uname_sridhar.egg-info/PKG-INFO` & `Uname_sridhar-0.0.4/Uname_sridhar.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Uname-sridhar
-Version: 0.0.3
+Version: 0.0.4
 Summary: Get Information About Current Linux Kernel With Python
 Home-page: https://git.selfmade.ninja/SRIDHARDSCV/package_uname_command
 Author: Sridhar
 Author-email: dcsvsridhar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -23,12 +23,12 @@
 
 
 
 #### Usage
 
 To get all available info about Linux Commands and Type of Linux Commands
 ```
- Uname [Option..]
+ Uname_cli [Option..]
 
 ```
```

### Comparing `Uname_sridhar-0.0.3/main/main.py` & `Uname_sridhar-0.0.4/main/main.py`

 * *Files identical despite different names*

### Comparing `Uname_sridhar-0.0.3/setup.py` & `Uname_sridhar-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='Uname_sridhar',
-    version='0.0.3',
+    version='0.0.4',
     author='Sridhar',
     author_email='dcsvsridhar@gmail.com',
     description='Get Information About Current Linux Kernel With Python',
     packages=find_packages(),
     url='https://git.selfmade.ninja/SRIDHARDSCV/package_uname_command',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

