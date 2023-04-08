# Comparing `tmp/zuela-0.2.0.tar.gz` & `tmp/zuela-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zuela-0.2.0.tar", last modified: Sat Apr  8 22:29:08 2023, max compression
+gzip compressed data, was "zuela-0.3.0.tar", last modified: Sat Apr  8 23:05:35 2023, max compression
```

## Comparing `zuela-0.2.0.tar` & `zuela-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 22:29:08.219066 zuela-0.2.0/
--rw-rw-rw-   0        0        0      691 2023-04-08 22:29:08.219066 zuela-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0        4 2023-04-08 22:06:19.000000 zuela-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-08 22:29:08.220071 zuela-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1332 2023-04-08 22:29:02.000000 zuela-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 22:29:08.198060 zuela-0.2.0/zuela/
--rw-rw-rw-   0        0        0       67 2023-04-08 22:28:13.000000 zuela-0.2.0/zuela/__init__.py
--rw-rw-rw-   0        0        0      288 2023-04-08 22:02:33.000000 zuela-0.2.0/zuela/multiplication.py
-drwxrwxrwx   0        0        0        0 2023-04-08 22:29:08.217061 zuela-0.2.0/zuela.egg-info/
--rw-rw-rw-   0        0        0      691 2023-04-08 22:29:08.000000 zuela-0.2.0/zuela.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-04-08 22:29:08.000000 zuela-0.2.0/zuela.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 22:29:08.000000 zuela-0.2.0/zuela.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-08 22:29:08.000000 zuela-0.2.0/zuela.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-08 22:29:08.000000 zuela-0.2.0/zuela.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-08 23:05:35.244354 zuela-0.3.0/
+-rw-rw-rw-   0        0        0      691 2023-04-08 23:05:35.243340 zuela-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2023-04-08 22:06:19.000000 zuela-0.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-08 23:05:35.244354 zuela-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1332 2023-04-08 22:39:23.000000 zuela-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 23:05:35.200334 zuela-0.3.0/zuela/
+-rw-rw-rw-   0        0        0     6943 2023-04-08 23:05:23.000000 zuela-0.3.0/zuela/__init__.py
+-rw-rw-rw-   0        0        0      288 2023-04-08 22:02:33.000000 zuela-0.3.0/zuela/multiplication.py
+drwxrwxrwx   0        0        0        0 2023-04-08 23:05:35.241333 zuela-0.3.0/zuela.egg-info/
+-rw-rw-rw-   0        0        0      691 2023-04-08 23:05:35.000000 zuela-0.3.0/zuela.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-04-08 23:05:35.000000 zuela-0.3.0/zuela.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 23:05:35.000000 zuela-0.3.0/zuela.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-08 23:05:35.000000 zuela-0.3.0/zuela.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-08 23:05:35.000000 zuela-0.3.0/zuela.egg-info/top_level.txt
```

### Comparing `zuela-0.2.0/PKG-INFO` & `zuela-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zuela
-Version: 0.2.0
+Version: 0.3.0
 Summary: Demo library
 Home-page: https://medium-multiply.readthedocs.io/
 Author: Joffrey Bienvenu
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `zuela-0.2.0/setup.py` & `zuela-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="zuela",
-    version="0.2.0",
+    version="0.3.0",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://medium-multiply.readthedocs.io/",
     author="Joffrey Bienvenu",
     author_email="example@email.com",
     license="MIT",
```

### Comparing `zuela-0.2.0/zuela.egg-info/PKG-INFO` & `zuela-0.3.0/zuela.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zuela
-Version: 0.2.0
+Version: 0.3.0
 Summary: Demo library
 Home-page: https://medium-multiply.readthedocs.io/
 Author: Joffrey Bienvenu
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

