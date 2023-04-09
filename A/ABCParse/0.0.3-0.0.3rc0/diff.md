# Comparing `tmp/ABCParse-0.0.3.tar.gz` & `tmp/ABCParse-0.0.3rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ABCParse-0.0.3.tar", last modified: Sun Apr  9 05:01:46 2023, max compression
+gzip compressed data, was "ABCParse-0.0.3rc0.tar", last modified: Sun Apr  9 04:45:15 2023, max compression
```

## Comparing `ABCParse-0.0.3.tar` & `ABCParse-0.0.3rc0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 05:01:46.718174 ABCParse-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 05:01:46.718174 ABCParse-0.0.3/ABCParse/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-09 05:01:37.000000 ABCParse-0.0.3/ABCParse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-09 05:01:37.000000 ABCParse-0.0.3/ABCParse/_abc_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-09 05:01:37.000000 ABCParse-0.0.3/ABCParse/_function_kwargs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 05:01:46.718174 ABCParse-0.0.3/ABCParse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-09 05:01:46.000000 ABCParse-0.0.3/ABCParse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-09 05:01:46.000000 ABCParse-0.0.3/ABCParse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 05:01:46.000000 ABCParse-0.0.3/ABCParse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 05:01:46.000000 ABCParse-0.0.3/ABCParse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-09 05:01:37.000000 ABCParse-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-09 05:01:46.718174 ABCParse-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-09 05:01:37.000000 ABCParse-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 05:01:46.718174 ABCParse-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-09 05:01:37.000000 ABCParse-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:45:15.028167 ABCParse-0.0.3rc0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:45:15.028167 ABCParse-0.0.3rc0/ABCParse/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-09 04:45:05.000000 ABCParse-0.0.3rc0/ABCParse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-09 04:45:05.000000 ABCParse-0.0.3rc0/ABCParse/_abc_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-09 04:45:05.000000 ABCParse-0.0.3rc0/ABCParse/_function_kwargs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:45:15.028167 ABCParse-0.0.3rc0/ABCParse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-09 04:45:14.000000 ABCParse-0.0.3rc0/ABCParse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-09 04:45:14.000000 ABCParse-0.0.3rc0/ABCParse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 04:45:14.000000 ABCParse-0.0.3rc0/ABCParse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 04:45:14.000000 ABCParse-0.0.3rc0/ABCParse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-09 04:45:05.000000 ABCParse-0.0.3rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-09 04:45:15.028167 ABCParse-0.0.3rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-09 04:45:05.000000 ABCParse-0.0.3rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 04:45:15.028167 ABCParse-0.0.3rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-09 04:45:05.000000 ABCParse-0.0.3rc0/setup.py
```

### Comparing `ABCParse-0.0.3/ABCParse/_abc_parse.py` & `ABCParse-0.0.3rc0/ABCParse/_abc_parse.py`

 * *Files identical despite different names*

### Comparing `ABCParse-0.0.3/ABCParse/_function_kwargs.py` & `ABCParse-0.0.3rc0/ABCParse/_function_kwargs.py`

 * *Files identical despite different names*

### Comparing `ABCParse-0.0.3/ABCParse.egg-info/PKG-INFO` & `ABCParse-0.0.3rc0/ABCParse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ABCParse
-Version: 0.0.3
+Version: 0.0.3rc0
 Summary: A better base class to automatically parse local args.
 Author: Michael E. Vinyard
 Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ABCParse-0.0.3/LICENSE` & `ABCParse-0.0.3rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `ABCParse-0.0.3/PKG-INFO` & `ABCParse-0.0.3rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ABCParse
-Version: 0.0.3
+Version: 0.0.3rc0
 Summary: A better base class to automatically parse local args.
 Author: Michael E. Vinyard
 Author-email: mvinyard@broadinstitute.org
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ABCParse-0.0.3/README.md` & `ABCParse-0.0.3rc0/README.md`

 * *Files identical despite different names*

### Comparing `ABCParse-0.0.3/setup.py` & `ABCParse-0.0.3rc0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 import os
 import sys
 
 
 setuptools.setup(
     name="ABCParse",
-    version="0.0.3",
+    version="0.0.3rc0",
     python_requires=">3.7.0",
     author="Michael E. Vinyard",
     author_email="mvinyard@broadinstitute.org",
     url=None,
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="A better base class to automatically parse local args.",
```

