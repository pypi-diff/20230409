# Comparing `tmp/flet_route-0.2.0.tar.gz` & `tmp/flet_route-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_route-0.2.0.tar", last modified: Sun Apr  9 09:50:54 2023, max compression
+gzip compressed data, was "flet_route-0.2.1.tar", last modified: Sun Apr  9 10:29:51 2023, max compression
```

## Comparing `flet_route-0.2.0.tar` & `flet_route-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 saurabh   (1000) saurabh   (1001)        0 2023-04-09 09:50:54.562102 flet_route-0.2.0/
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)     1072 2023-03-09 16:43:16.000000 flet_route-0.2.0/LICENSE
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)     1103 2023-04-09 09:50:54.562102 flet_route-0.2.0/PKG-INFO
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)      620 2023-04-09 09:44:19.000000 flet_route-0.2.0/README.md
-drwxr-xr-x   0 saurabh   (1000) saurabh   (1001)        0 2023-04-09 09:50:54.561102 flet_route-0.2.0/flet_route/
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)      128 2023-04-02 00:50:24.000000 flet_route-0.2.0/flet_route/__init__.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)      646 2023-04-02 01:06:15.000000 flet_route-0.2.0/flet_route/basket.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)      405 2023-04-02 00:45:42.000000 flet_route-0.2.0/flet_route/not_found_view.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)      716 2023-04-02 01:09:18.000000 flet_route-0.2.0/flet_route/params.py
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)     4177 2023-04-06 16:28:44.000000 flet_route-0.2.0/flet_route/routing.py
-drwxr-xr-x   0 saurabh   (1000) saurabh   (1001)        0 2023-04-09 09:50:54.562102 flet_route-0.2.0/flet_route.egg-info/
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)     1103 2023-04-09 09:50:54.000000 flet_route-0.2.0/flet_route.egg-info/PKG-INFO
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)      278 2023-04-09 09:50:54.000000 flet_route-0.2.0/flet_route.egg-info/SOURCES.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)        1 2023-04-09 09:50:54.000000 flet_route-0.2.0/flet_route.egg-info/dependency_links.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)       11 2023-04-09 09:50:54.000000 flet_route-0.2.0/flet_route.egg-info/top_level.txt
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)       38 2023-04-09 09:50:54.562102 flet_route-0.2.0/setup.cfg
--rw-r--r--   0 saurabh   (1000) saurabh   (1001)      753 2023-04-09 09:44:30.000000 flet_route-0.2.0/setup.py
+drwxr-xr-x   0 saurabh   (1000) saurabh   (1001)        0 2023-04-09 10:29:51.641134 flet_route-0.2.1/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)     1072 2023-03-09 16:43:16.000000 flet_route-0.2.1/LICENSE
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)     1131 2023-04-09 10:29:51.640134 flet_route-0.2.1/PKG-INFO
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)      648 2023-04-09 10:28:42.000000 flet_route-0.2.1/README.md
+drwxr-xr-x   0 saurabh   (1000) saurabh   (1001)        0 2023-04-09 10:29:51.639134 flet_route-0.2.1/flet_route/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)      128 2023-04-02 00:50:24.000000 flet_route-0.2.1/flet_route/__init__.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)      646 2023-04-02 01:06:15.000000 flet_route-0.2.1/flet_route/basket.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)      405 2023-04-02 00:45:42.000000 flet_route-0.2.1/flet_route/not_found_view.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)      716 2023-04-02 01:09:18.000000 flet_route-0.2.1/flet_route/params.py
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)     4177 2023-04-06 16:28:44.000000 flet_route-0.2.1/flet_route/routing.py
+drwxr-xr-x   0 saurabh   (1000) saurabh   (1001)        0 2023-04-09 10:29:51.640134 flet_route-0.2.1/flet_route.egg-info/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)     1131 2023-04-09 10:29:51.000000 flet_route-0.2.1/flet_route.egg-info/PKG-INFO
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)      278 2023-04-09 10:29:51.000000 flet_route-0.2.1/flet_route.egg-info/SOURCES.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)        1 2023-04-09 10:29:51.000000 flet_route-0.2.1/flet_route.egg-info/dependency_links.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)       11 2023-04-09 10:29:51.000000 flet_route-0.2.1/flet_route.egg-info/top_level.txt
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)       38 2023-04-09 10:29:51.641134 flet_route-0.2.1/setup.cfg
+-rw-r--r--   0 saurabh   (1000) saurabh   (1001)      753 2023-04-09 10:28:52.000000 flet_route-0.2.1/setup.py
```

### Comparing `flet_route-0.2.0/LICENSE` & `flet_route-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_route-0.2.0/PKG-INFO` & `flet_route-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet_route
-Version: 0.2.0
+Version: 0.2.1
 Summary: This makes it easy to manage multiple views with dynamic routing.
 Home-page: https://github.com/saurabhwadekar/flet_route
 Author: Saurabh Wadekar [ INDIA ]
 Maintainer: Saurabh Wadekar
 Maintainer-email: saurabhwadekar420@gmail.com
 License: MIT
 Keywords: flet,routing,flet_route,routes,flet app,flet-route,flet simple routing
@@ -24,15 +24,15 @@
 ```
 
 ## Upgradation
 ```
 pip install flet-route --upgrade
 ```
 
-#### [📖 Read the documentation ](https://link-url-here.org)
+#### [📖 Read the documentation ](https://saurabhwadekar.github.io/flet-route-doc/flow/)
 
 
 ## Author
 
 <b>Name :</b> Saurabh Wadekar<br>
 <b>Email :</b> saurabhwadekar420@gmail.com<br>
 <b>County :</b> 🇮🇳INDIA🇮🇳<br>
```

### Comparing `flet_route-0.2.0/README.md` & `flet_route-0.2.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ```
 
 ## Upgradation
 ```
 pip install flet-route --upgrade
 ```
 
-#### [📖 Read the documentation ](https://link-url-here.org)
+#### [📖 Read the documentation ](https://saurabhwadekar.github.io/flet-route-doc/flow/)
 
 
 ## Author
 
 <b>Name :</b> Saurabh Wadekar<br>
 <b>Email :</b> saurabhwadekar420@gmail.com<br>
 <b>County :</b> 🇮🇳INDIA🇮🇳<br>
```

### Comparing `flet_route-0.2.0/flet_route/basket.py` & `flet_route-0.2.1/flet_route/basket.py`

 * *Files identical despite different names*

### Comparing `flet_route-0.2.0/flet_route/params.py` & `flet_route-0.2.1/flet_route/params.py`

 * *Files identical despite different names*

### Comparing `flet_route-0.2.0/flet_route/routing.py` & `flet_route-0.2.1/flet_route/routing.py`

 * *Files identical despite different names*

### Comparing `flet_route-0.2.0/flet_route.egg-info/PKG-INFO` & `flet_route-0.2.1/flet_route.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flet-route
-Version: 0.2.0
+Version: 0.2.1
 Summary: This makes it easy to manage multiple views with dynamic routing.
 Home-page: https://github.com/saurabhwadekar/flet_route
 Author: Saurabh Wadekar [ INDIA ]
 Maintainer: Saurabh Wadekar
 Maintainer-email: saurabhwadekar420@gmail.com
 License: MIT
 Keywords: flet,routing,flet_route,routes,flet app,flet-route,flet simple routing
@@ -24,15 +24,15 @@
 ```
 
 ## Upgradation
 ```
 pip install flet-route --upgrade
 ```
 
-#### [📖 Read the documentation ](https://link-url-here.org)
+#### [📖 Read the documentation ](https://saurabhwadekar.github.io/flet-route-doc/flow/)
 
 
 ## Author
 
 <b>Name :</b> Saurabh Wadekar<br>
 <b>Email :</b> saurabhwadekar420@gmail.com<br>
 <b>County :</b> 🇮🇳INDIA🇮🇳<br>
```

### Comparing `flet_route-0.2.0/setup.py` & `flet_route-0.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name = "flet_route",
-    version = "0.2.0",
+    version = "0.2.1",
     author="Saurabh Wadekar [ INDIA ]",
     packages=["flet_route"],
     license="MIT",
     requires=["flet","repath"],
     maintainer="Saurabh Wadekar",
     maintainer_email="saurabhwadekar420@gmail.com",
     keywords=["flet","routing","flet_route","routes","flet app","flet-route","flet simple routing"],
```

