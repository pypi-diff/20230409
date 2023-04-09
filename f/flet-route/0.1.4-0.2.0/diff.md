# Comparing `tmp/flet_route-0.1.4.tar.gz` & `tmp/flet_route-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_route-0.1.4.tar", last modified: Sun Mar 12 15:36:25 2023, max compression
+gzip compressed data, was "flet_route-0.2.0.tar", last modified: Sun Apr  9 09:50:54 2023, max compression
```

## Comparing `flet_route-0.1.4.tar` & `flet_route-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 saurabh   (1000) saurabh   (1001)        0 2023-03-12 15:36:25.632063 flet_route-0.1.4/
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)     1072 2023-03-09 16:43:16.000000 flet_route-0.1.4/LICENSE
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)     6296 2023-03-12 15:36:25.631063 flet_route-0.1.4/PKG-INFO
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)     5813 2023-03-12 08:26:58.000000 flet_route-0.1.4/README.rst
-drwxr-xr-x   0 saurabh   (1000) saurabh   (1001)        0 2023-03-12 15:36:25.630063 flet_route-0.1.4/flet_route/
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)       74 2023-03-08 04:13:06.000000 flet_route-0.1.4/flet_route/__init__.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)      398 2023-03-08 04:42:33.000000 flet_route-0.1.4/flet_route/not_found_view.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)     2496 2023-03-12 07:19:04.000000 flet_route-0.1.4/flet_route/routing.py
-drwxr-xr-x   0 saurabh   (1000) saurabh   (1001)        0 2023-03-12 15:36:25.631063 flet_route-0.1.4/flet_route.egg-info/
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)     6296 2023-03-12 15:36:25.000000 flet_route-0.1.4/flet_route.egg-info/PKG-INFO
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)      237 2023-03-12 15:36:25.000000 flet_route-0.1.4/flet_route.egg-info/SOURCES.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)        1 2023-03-12 15:36:25.000000 flet_route-0.1.4/flet_route.egg-info/dependency_links.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)       11 2023-03-12 15:36:25.000000 flet_route-0.1.4/flet_route.egg-info/top_level.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)       38 2023-03-12 15:36:25.632063 flet_route-0.1.4/setup.cfg
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)      753 2023-03-12 15:36:11.000000 flet_route-0.1.4/setup.py
+drwxr-xr-x   0 saurabh   (1000) saurabh   (1001)        0 2023-04-09 09:50:54.562102 flet_route-0.2.0/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)     1072 2023-03-09 16:43:16.000000 flet_route-0.2.0/LICENSE
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)     1103 2023-04-09 09:50:54.562102 flet_route-0.2.0/PKG-INFO
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)      620 2023-04-09 09:44:19.000000 flet_route-0.2.0/README.md
+drwxr-xr-x   0 saurabh   (1000) saurabh   (1001)        0 2023-04-09 09:50:54.561102 flet_route-0.2.0/flet_route/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)      128 2023-04-02 00:50:24.000000 flet_route-0.2.0/flet_route/__init__.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)      646 2023-04-02 01:06:15.000000 flet_route-0.2.0/flet_route/basket.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)      405 2023-04-02 00:45:42.000000 flet_route-0.2.0/flet_route/not_found_view.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)      716 2023-04-02 01:09:18.000000 flet_route-0.2.0/flet_route/params.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)     4177 2023-04-06 16:28:44.000000 flet_route-0.2.0/flet_route/routing.py
+drwxr-xr-x   0 saurabh   (1000) saurabh   (1001)        0 2023-04-09 09:50:54.562102 flet_route-0.2.0/flet_route.egg-info/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)     1103 2023-04-09 09:50:54.000000 flet_route-0.2.0/flet_route.egg-info/PKG-INFO
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)      278 2023-04-09 09:50:54.000000 flet_route-0.2.0/flet_route.egg-info/SOURCES.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)        1 2023-04-09 09:50:54.000000 flet_route-0.2.0/flet_route.egg-info/dependency_links.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)       11 2023-04-09 09:50:54.000000 flet_route-0.2.0/flet_route.egg-info/top_level.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)       38 2023-04-09 09:50:54.562102 flet_route-0.2.0/setup.cfg
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)      753 2023-04-09 09:44:30.000000 flet_route-0.2.0/setup.py
```

### Comparing `flet_route-0.1.4/LICENSE` & `flet_route-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_route-0.1.4/setup.py` & `flet_route-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name = "flet_route",
-    version = "0.1.4",
+    version = "0.2.0",
     author="Saurabh Wadekar [ INDIA ]",
     packages=["flet_route"],
     license="MIT",
     requires=["flet","repath"],
     maintainer="Saurabh Wadekar",
     maintainer_email="saurabhwadekar420@gmail.com",
     keywords=["flet","routing","flet_route","routes","flet app","flet-route","flet simple routing"],
```

