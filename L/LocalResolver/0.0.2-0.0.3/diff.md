# Comparing `tmp/LocalResolver-0.0.2.tar.gz` & `tmp/LocalResolver-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LocalResolver-0.0.2.tar", last modified: Thu Apr  6 20:40:40 2023, max compression
+gzip compressed data, was "LocalResolver-0.0.3.tar", last modified: Sun Apr  9 15:25:30 2023, max compression
```

## Comparing `LocalResolver-0.0.2.tar` & `LocalResolver-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-06 20:40:40.946742 LocalResolver-0.0.2/
--rw-r--r--   0 kali      (1000) kali      (1000)    35149 2023-04-06 19:27:34.000000 LocalResolver-0.0.2/LICENSE.txt
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-06 20:40:40.946742 LocalResolver-0.0.2/LocalResolver.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     2371 2023-04-06 20:40:40.000000 LocalResolver-0.0.2/LocalResolver.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      276 2023-04-06 20:40:40.000000 LocalResolver-0.0.2/LocalResolver.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-06 20:40:40.000000 LocalResolver-0.0.2/LocalResolver.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       59 2023-04-06 20:40:40.000000 LocalResolver-0.0.2/LocalResolver.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        6 2023-04-06 20:40:40.000000 LocalResolver-0.0.2/LocalResolver.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       14 2023-04-06 20:40:40.000000 LocalResolver-0.0.2/LocalResolver.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       27 2023-04-06 19:27:34.000000 LocalResolver-0.0.2/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)     2371 2023-04-06 20:40:40.946742 LocalResolver-0.0.2/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1174 2023-04-06 20:12:08.000000 LocalResolver-0.0.2/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-06 20:40:40.946742 LocalResolver-0.0.2/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1619 2023-04-06 20:40:36.000000 LocalResolver-0.0.2/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-09 15:25:30.393651 LocalResolver-0.0.3/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35149 2023-04-06 19:27:34.000000 LocalResolver-0.0.3/LICENSE.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-09 15:25:30.393651 LocalResolver-0.0.3/LocalResolver.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     2371 2023-04-09 15:25:30.000000 LocalResolver-0.0.3/LocalResolver.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      293 2023-04-09 15:25:30.000000 LocalResolver-0.0.3/LocalResolver.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-09 15:25:30.000000 LocalResolver-0.0.3/LocalResolver.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       59 2023-04-09 15:25:30.000000 LocalResolver-0.0.3/LocalResolver.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        6 2023-04-09 15:25:30.000000 LocalResolver-0.0.3/LocalResolver.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       14 2023-04-09 15:25:30.000000 LocalResolver-0.0.3/LocalResolver.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)     7561 2023-04-09 15:25:13.000000 LocalResolver-0.0.3/LocalResolver.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       27 2023-04-06 19:27:34.000000 LocalResolver-0.0.3/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)     2371 2023-04-09 15:25:30.393651 LocalResolver-0.0.3/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     1174 2023-04-06 20:12:08.000000 LocalResolver-0.0.3/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-09 15:25:30.393651 LocalResolver-0.0.3/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1619 2023-04-09 15:25:18.000000 LocalResolver-0.0.3/setup.py
```

### Comparing `LocalResolver-0.0.2/LICENSE.txt` & `LocalResolver-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `LocalResolver-0.0.2/LocalResolver.egg-info/PKG-INFO` & `LocalResolver-0.0.3/LocalResolver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LocalResolver
-Version: 0.0.2
+Version: 0.0.3
 Summary: This package implements local hostname resolver tool with scapy (using netbios and LLMNR query).
 Home-page: https://github.com/mauricelambert/LocalResolver
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `LocalResolver-0.0.2/PKG-INFO` & `LocalResolver-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LocalResolver
-Version: 0.0.2
+Version: 0.0.3
 Summary: This package implements local hostname resolver tool with scapy (using netbios and LLMNR query).
 Home-page: https://github.com/mauricelambert/LocalResolver
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `LocalResolver-0.0.2/README.md` & `LocalResolver-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `LocalResolver-0.0.2/setup.py` & `LocalResolver-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'LocalResolver',
-    version = "0.0.2",
+    version = "0.0.3",
     py_modules=["LocalResolver"],
     install_requires = ['scapy'],
     author = "Maurice Lambert", 
     author_email = "mauricelambert434@gmail.com",
     maintainer="Maurice Lambert",
     maintainer_email="mauricelambert434@gmail.com",
     description = "This package implements local hostname resolver tool with scapy (using netbios and LLMNR query).",
```

