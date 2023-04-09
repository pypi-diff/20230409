# Comparing `tmp/vajirayana-0.0.1.tar.gz` & `tmp/vajirayana-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vajirayana-0.0.1.tar", last modified: Sun Apr  9 14:24:10 2023, max compression
+gzip compressed data, was "vajirayana-0.0.2.tar", last modified: Sun Apr  9 14:34:12 2023, max compression
```

## Comparing `vajirayana-0.0.1.tar` & `vajirayana-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 hrnph     (1000) hrnph     (1000)        0 2023-04-09 14:24:10.533081 vajirayana-0.0.1/
--rw-r--r--   0 hrnph     (1000) hrnph     (1000)      576 2023-04-09 14:24:10.533081 vajirayana-0.0.1/PKG-INFO
--rw-r--r--   0 hrnph     (1000) hrnph     (1000)      132 2023-04-09 12:29:16.000000 vajirayana-0.0.1/README.md
--rw-r--r--   0 hrnph     (1000) hrnph     (1000)       38 2023-04-09 14:24:10.533081 vajirayana-0.0.1/setup.cfg
--rw-r--r--   0 hrnph     (1000) hrnph     (1000)     1013 2023-04-09 14:23:49.000000 vajirayana-0.0.1/setup.py
-drwxr-xr-x   0 hrnph     (1000) hrnph     (1000)        0 2023-04-09 14:24:10.530081 vajirayana-0.0.1/vajirayana/
--rw-r--r--   0 hrnph     (1000) hrnph     (1000)       27 2023-04-09 14:20:59.000000 vajirayana-0.0.1/vajirayana/__init__.py
--rw-r--r--   0 hrnph     (1000) hrnph     (1000)     2200 2023-04-09 12:20:50.000000 vajirayana-0.0.1/vajirayana/scraper.py
-drwxr-xr-x   0 hrnph     (1000) hrnph     (1000)        0 2023-04-09 14:24:10.532081 vajirayana-0.0.1/vajirayana.egg-info/
--rw-r--r--   0 hrnph     (1000) hrnph     (1000)      576 2023-04-09 14:24:10.000000 vajirayana-0.0.1/vajirayana.egg-info/PKG-INFO
--rw-r--r--   0 hrnph     (1000) hrnph     (1000)      232 2023-04-09 14:24:10.000000 vajirayana-0.0.1/vajirayana.egg-info/SOURCES.txt
--rw-r--r--   0 hrnph     (1000) hrnph     (1000)        1 2023-04-09 14:24:10.000000 vajirayana-0.0.1/vajirayana.egg-info/dependency_links.txt
--rw-r--r--   0 hrnph     (1000) hrnph     (1000)       42 2023-04-09 14:24:10.000000 vajirayana-0.0.1/vajirayana.egg-info/requires.txt
--rw-r--r--   0 hrnph     (1000) hrnph     (1000)       11 2023-04-09 14:24:10.000000 vajirayana-0.0.1/vajirayana.egg-info/top_level.txt
+drwxr-xr-x   0 hrnph     (1000) hrnph     (1000)        0 2023-04-09 14:34:12.633110 vajirayana-0.0.2/
+-rw-r--r--   0 hrnph     (1000) hrnph     (1000)     1056 2023-04-09 14:29:25.000000 vajirayana-0.0.2/LICENSE.md
+-rw-r--r--   0 hrnph     (1000) hrnph     (1000)      601 2023-04-09 14:34:12.633110 vajirayana-0.0.2/PKG-INFO
+-rw-r--r--   0 hrnph     (1000) hrnph     (1000)      376 2023-04-09 14:33:47.000000 vajirayana-0.0.2/README.md
+-rw-r--r--   0 hrnph     (1000) hrnph     (1000)      106 2023-04-09 14:34:12.634110 vajirayana-0.0.2/setup.cfg
+-rw-r--r--   0 hrnph     (1000) hrnph     (1000)     1013 2023-04-09 14:34:09.000000 vajirayana-0.0.2/setup.py
+drwxr-xr-x   0 hrnph     (1000) hrnph     (1000)        0 2023-04-09 14:34:12.631110 vajirayana-0.0.2/vajirayana/
+-rw-r--r--   0 hrnph     (1000) hrnph     (1000)       27 2023-04-09 14:20:59.000000 vajirayana-0.0.2/vajirayana/__init__.py
+-rw-r--r--   0 hrnph     (1000) hrnph     (1000)     2200 2023-04-09 12:20:50.000000 vajirayana-0.0.2/vajirayana/scraper.py
+drwxr-xr-x   0 hrnph     (1000) hrnph     (1000)        0 2023-04-09 14:34:12.633110 vajirayana-0.0.2/vajirayana.egg-info/
+-rw-r--r--   0 hrnph     (1000) hrnph     (1000)      601 2023-04-09 14:34:12.000000 vajirayana-0.0.2/vajirayana.egg-info/PKG-INFO
+-rw-r--r--   0 hrnph     (1000) hrnph     (1000)      253 2023-04-09 14:34:12.000000 vajirayana-0.0.2/vajirayana.egg-info/SOURCES.txt
+-rw-r--r--   0 hrnph     (1000) hrnph     (1000)        1 2023-04-09 14:34:12.000000 vajirayana-0.0.2/vajirayana.egg-info/dependency_links.txt
+-rw-r--r--   0 hrnph     (1000) hrnph     (1000)       42 2023-04-09 14:34:12.000000 vajirayana-0.0.2/vajirayana.egg-info/requires.txt
+-rw-r--r--   0 hrnph     (1000) hrnph     (1000)       11 2023-04-09 14:34:12.000000 vajirayana-0.0.2/vajirayana.egg-info/top_level.txt
```

### Comparing `vajirayana-0.0.1/PKG-INFO` & `vajirayana-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: vajirayana
-Version: 0.0.1
+Version: 0.0.2
 Summary: an unofficial python API interface for Vajirayana
 Author: hrnph
 Author-email: hrnph@protonmail.com
 Keywords: python,api,scraper,vajirayana,vajirayana-scraper
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+License-File: LICENSE.md
 
 Vajirayana Scraper an unofficial python API interface for Vajirayana
```

### Comparing `vajirayana-0.0.1/setup.py` & `vajirayana-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'an unofficial python API interface for Vajirayana'
 LONG_DESCRIPTION = 'Vajirayana Scraper an unofficial python API interface for Vajirayana'
 
 # Setting up
 setup(
         name="vajirayana", 
         version=VERSION,
```

### Comparing `vajirayana-0.0.1/vajirayana/scraper.py` & `vajirayana-0.0.2/vajirayana/scraper.py`

 * *Files identical despite different names*

### Comparing `vajirayana-0.0.1/vajirayana.egg-info/PKG-INFO` & `vajirayana-0.0.2/vajirayana.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: vajirayana
-Version: 0.0.1
+Version: 0.0.2
 Summary: an unofficial python API interface for Vajirayana
 Author: hrnph
 Author-email: hrnph@protonmail.com
 Keywords: python,api,scraper,vajirayana,vajirayana-scraper
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+License-File: LICENSE.md
 
 Vajirayana Scraper an unofficial python API interface for Vajirayana
```

