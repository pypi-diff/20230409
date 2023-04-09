# Comparing `tmp/zuela-0.4.0.tar.gz` & `tmp/zuela-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zuela-0.4.0.tar", last modified: Sun Apr  9 19:15:25 2023, max compression
+gzip compressed data, was "zuela-0.5.0.tar", last modified: Sun Apr  9 19:58:00 2023, max compression
```

## Comparing `zuela-0.4.0.tar` & `zuela-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 19:15:25.966050 zuela-0.4.0/
--rw-rw-rw-   0        0        0      691 2023-04-09 19:15:25.966050 zuela-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0        4 2023-04-08 22:06:19.000000 zuela-0.4.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-09 19:15:25.967050 zuela-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1337 2023-04-09 19:13:48.000000 zuela-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 19:15:25.913051 zuela-0.4.0/zuela/
--rw-rw-rw-   0        0        0     7199 2023-04-09 19:14:31.000000 zuela-0.4.0/zuela/__init__.py
--rw-rw-rw-   0        0        0      288 2023-04-09 19:14:31.000000 zuela-0.4.0/zuela/multiplication.py
-drwxrwxrwx   0        0        0        0 2023-04-09 19:15:25.964062 zuela-0.4.0/zuela.egg-info/
--rw-rw-rw-   0        0        0      691 2023-04-09 19:15:25.000000 zuela-0.4.0/zuela.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-04-09 19:15:25.000000 zuela-0.4.0/zuela.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 19:15:25.000000 zuela-0.4.0/zuela.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-09 19:15:25.000000 zuela-0.4.0/zuela.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-09 19:15:25.000000 zuela-0.4.0/zuela.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 19:58:00.601758 zuela-0.5.0/
+-rw-rw-rw-   0        0        0      691 2023-04-09 19:58:00.600762 zuela-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2023-04-08 22:06:19.000000 zuela-0.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-09 19:58:00.601758 zuela-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1355 2023-04-09 19:57:43.000000 zuela-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 19:58:00.572758 zuela-0.5.0/zuela/
+-rw-rw-rw-   0        0        0     7199 2023-04-09 19:14:31.000000 zuela-0.5.0/zuela/__init__.py
+-rw-rw-rw-   0        0        0      288 2023-04-09 19:14:31.000000 zuela-0.5.0/zuela/multiplication.py
+drwxrwxrwx   0        0        0        0 2023-04-09 19:58:00.599758 zuela-0.5.0/zuela.egg-info/
+-rw-rw-rw-   0        0        0      691 2023-04-09 19:58:00.000000 zuela-0.5.0/zuela.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-04-09 19:58:00.000000 zuela-0.5.0/zuela.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 19:58:00.000000 zuela-0.5.0/zuela.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-04-09 19:58:00.000000 zuela-0.5.0/zuela.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-09 19:58:00.000000 zuela-0.5.0/zuela.egg-info/top_level.txt
```

### Comparing `zuela-0.4.0/PKG-INFO` & `zuela-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zuela
-Version: 0.4.0
+Version: 0.5.0
 Summary: Demo library
 Home-page: https://medium-multiply.readthedocs.io/
 Author: Joffrey Bienvenu
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `zuela-0.4.0/setup.py` & `zuela-0.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 
 # To use a consistent encoding
 from codecs import open
 from os import path
 
+print('TEST'*10)
 
 # The directory containing this file
 HERE = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="zuela",
-    version="0.4.0",
+    version="0.5.0",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://medium-multiply.readthedocs.io/",
     author="Joffrey Bienvenu",
     author_email="example@email.com",
     license="MIT",
```

### Comparing `zuela-0.4.0/zuela/__init__.py` & `zuela-0.5.0/zuela/__init__.py`

 * *Files identical despite different names*

### Comparing `zuela-0.4.0/zuela.egg-info/PKG-INFO` & `zuela-0.5.0/zuela.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zuela
-Version: 0.4.0
+Version: 0.5.0
 Summary: Demo library
 Home-page: https://medium-multiply.readthedocs.io/
 Author: Joffrey Bienvenu
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

