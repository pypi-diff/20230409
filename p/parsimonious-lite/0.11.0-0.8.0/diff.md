# Comparing `tmp/parsimonious-lite-0.11.0.tar.gz` & `tmp/parsimonious-lite-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsimonious-lite-0.11.0.tar", last modified: Sun Apr  9 06:08:44 2023, max compression
+gzip compressed data, was "parsimonious-lite-0.8.0.tar", last modified: Sun Apr  9 05:59:19 2023, max compression
```

## Comparing `parsimonious-lite-0.11.0.tar` & `parsimonious-lite-0.8.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-09 06:08:44.091988 parsimonious-lite-0.11.0/
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     1053 2023-04-01 17:33:54.000000 parsimonious-lite-0.11.0/LICENSE
--rw-r--r--   0 stormslivkoff   (502) staff       (20)       35 2023-04-01 17:33:54.000000 parsimonious-lite-0.11.0/MANIFEST.in
--rw-r--r--   0 stormslivkoff   (502) staff       (20)      963 2023-04-09 06:08:44.091776 parsimonious-lite-0.11.0/PKG-INFO
--rw-r--r--   0 stormslivkoff   (502) staff       (20)    19543 2023-04-01 17:47:34.000000 parsimonious-lite-0.11.0/README.rst
-drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-09 06:08:44.089136 parsimonious-lite-0.11.0/parsimonious_lite/
--rw-r--r--   0 stormslivkoff   (502) staff       (20)      436 2023-04-01 17:48:53.000000 parsimonious-lite-0.11.0/parsimonious_lite/__init__.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     3768 2023-04-01 17:46:45.000000 parsimonious-lite-0.11.0/parsimonious_lite/exceptions.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)    16522 2023-04-01 17:49:11.000000 parsimonious-lite-0.11.0/parsimonious_lite/expressions.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)    19456 2023-04-01 17:47:16.000000 parsimonious-lite-0.11.0/parsimonious_lite/grammar.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)    13187 2023-04-01 17:48:07.000000 parsimonious-lite-0.11.0/parsimonious_lite/nodes.py
-drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-09 06:08:44.091545 parsimonious-lite-0.11.0/parsimonious_lite/tests/
--rw-r--r--   0 stormslivkoff   (502) staff       (20)        0 2023-04-01 17:33:54.000000 parsimonious-lite-0.11.0/parsimonious_lite/tests/__init__.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     3244 2023-04-01 17:47:40.000000 parsimonious-lite-0.11.0/parsimonious_lite/tests/benchmarks.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     1595 2023-04-01 17:37:26.000000 parsimonious-lite-0.11.0/parsimonious_lite/tests/test_benchmarks.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)    12231 2023-04-01 17:49:27.000000 parsimonious-lite-0.11.0/parsimonious_lite/tests/test_expressions.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)    17696 2023-04-01 17:48:44.000000 parsimonious-lite-0.11.0/parsimonious_lite/tests/test_grammar.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     5851 2023-04-01 17:48:17.000000 parsimonious-lite-0.11.0/parsimonious_lite/tests/test_nodes.py
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     1161 2023-04-01 17:37:26.000000 parsimonious-lite-0.11.0/parsimonious_lite/utils.py
-drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-09 06:08:44.090202 parsimonious-lite-0.11.0/parsimonious_lite.egg-info/
--rw-r--r--   0 stormslivkoff   (502) staff       (20)      963 2023-04-09 06:08:44.000000 parsimonious-lite-0.11.0/parsimonious_lite.egg-info/PKG-INFO
--rw-r--r--   0 stormslivkoff   (502) staff       (20)      660 2023-04-09 06:08:44.000000 parsimonious-lite-0.11.0/parsimonious_lite.egg-info/SOURCES.txt
--rw-r--r--   0 stormslivkoff   (502) staff       (20)        1 2023-04-09 06:08:44.000000 parsimonious-lite-0.11.0/parsimonious_lite.egg-info/dependency_links.txt
--rw-r--r--   0 stormslivkoff   (502) staff       (20)       11 2023-04-09 06:08:44.000000 parsimonious-lite-0.11.0/parsimonious_lite.egg-info/requires.txt
--rw-r--r--   0 stormslivkoff   (502) staff       (20)       18 2023-04-09 06:08:44.000000 parsimonious-lite-0.11.0/parsimonious_lite.egg-info/top_level.txt
--rw-r--r--   0 stormslivkoff   (502) staff       (20)       38 2023-04-09 06:08:44.092050 parsimonious-lite-0.11.0/setup.cfg
--rw-r--r--   0 stormslivkoff   (502) staff       (20)     1515 2023-04-09 06:06:23.000000 parsimonious-lite-0.11.0/setup.py
+drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-09 05:59:19.327074 parsimonious-lite-0.8.0/
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     1053 2023-04-01 17:33:54.000000 parsimonious-lite-0.8.0/LICENSE
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)       35 2023-04-01 17:33:54.000000 parsimonious-lite-0.8.0/MANIFEST.in
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)      962 2023-04-09 05:59:19.326924 parsimonious-lite-0.8.0/PKG-INFO
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)    19543 2023-04-01 17:47:34.000000 parsimonious-lite-0.8.0/README.rst
+drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-09 05:59:19.324895 parsimonious-lite-0.8.0/parsimonious_lite/
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)      436 2023-04-01 17:48:53.000000 parsimonious-lite-0.8.0/parsimonious_lite/__init__.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     3768 2023-04-01 17:46:45.000000 parsimonious-lite-0.8.0/parsimonious_lite/exceptions.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)    16522 2023-04-01 17:49:11.000000 parsimonious-lite-0.8.0/parsimonious_lite/expressions.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)    19456 2023-04-01 17:47:16.000000 parsimonious-lite-0.8.0/parsimonious_lite/grammar.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)    13187 2023-04-01 17:48:07.000000 parsimonious-lite-0.8.0/parsimonious_lite/nodes.py
+drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-09 05:59:19.326709 parsimonious-lite-0.8.0/parsimonious_lite/tests/
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)        0 2023-04-01 17:33:54.000000 parsimonious-lite-0.8.0/parsimonious_lite/tests/__init__.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     3244 2023-04-01 17:47:40.000000 parsimonious-lite-0.8.0/parsimonious_lite/tests/benchmarks.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     1595 2023-04-01 17:37:26.000000 parsimonious-lite-0.8.0/parsimonious_lite/tests/test_benchmarks.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)    12231 2023-04-01 17:49:27.000000 parsimonious-lite-0.8.0/parsimonious_lite/tests/test_expressions.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)    17696 2023-04-01 17:48:44.000000 parsimonious-lite-0.8.0/parsimonious_lite/tests/test_grammar.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     5851 2023-04-01 17:48:17.000000 parsimonious-lite-0.8.0/parsimonious_lite/tests/test_nodes.py
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     1161 2023-04-01 17:37:26.000000 parsimonious-lite-0.8.0/parsimonious_lite/utils.py
+drwxr-xr-x   0 stormslivkoff   (502) staff       (20)        0 2023-04-09 05:59:19.325802 parsimonious-lite-0.8.0/parsimonious_lite.egg-info/
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)      962 2023-04-09 05:59:19.000000 parsimonious-lite-0.8.0/parsimonious_lite.egg-info/PKG-INFO
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)      660 2023-04-09 05:59:19.000000 parsimonious-lite-0.8.0/parsimonious_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)        1 2023-04-09 05:59:19.000000 parsimonious-lite-0.8.0/parsimonious_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)       11 2023-04-09 05:59:19.000000 parsimonious-lite-0.8.0/parsimonious_lite.egg-info/requires.txt
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)       18 2023-04-09 05:59:19.000000 parsimonious-lite-0.8.0/parsimonious_lite.egg-info/top_level.txt
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)       38 2023-04-09 05:59:19.327117 parsimonious-lite-0.8.0/setup.cfg
+-rw-r--r--   0 stormslivkoff   (502) staff       (20)     1514 2023-04-01 17:46:54.000000 parsimonious-lite-0.8.0/setup.py
```

### Comparing `parsimonious-lite-0.11.0/LICENSE` & `parsimonious-lite-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parsimonious-lite-0.11.0/PKG-INFO` & `parsimonious-lite-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsimonious-lite
-Version: 0.11.0
+Version: 0.8.0
 Summary: lite fork of parsimonious 0.8.0 for compatibility with python 3.11
 Keywords: parse,parser,parsing,peg,packrat,grammar,language
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `parsimonious-lite-0.11.0/README.rst` & `parsimonious-lite-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `parsimonious-lite-0.11.0/parsimonious_lite/exceptions.py` & `parsimonious-lite-0.8.0/parsimonious_lite/exceptions.py`

 * *Files identical despite different names*

### Comparing `parsimonious-lite-0.11.0/parsimonious_lite/expressions.py` & `parsimonious-lite-0.8.0/parsimonious_lite/expressions.py`

 * *Files identical despite different names*

### Comparing `parsimonious-lite-0.11.0/parsimonious_lite/grammar.py` & `parsimonious-lite-0.8.0/parsimonious_lite/grammar.py`

 * *Files identical despite different names*

### Comparing `parsimonious-lite-0.11.0/parsimonious_lite/nodes.py` & `parsimonious-lite-0.8.0/parsimonious_lite/nodes.py`

 * *Files identical despite different names*

### Comparing `parsimonious-lite-0.11.0/parsimonious_lite/tests/benchmarks.py` & `parsimonious-lite-0.8.0/parsimonious_lite/tests/benchmarks.py`

 * *Files identical despite different names*

### Comparing `parsimonious-lite-0.11.0/parsimonious_lite/tests/test_benchmarks.py` & `parsimonious-lite-0.8.0/parsimonious_lite/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `parsimonious-lite-0.11.0/parsimonious_lite/tests/test_expressions.py` & `parsimonious-lite-0.8.0/parsimonious_lite/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `parsimonious-lite-0.11.0/parsimonious_lite/tests/test_grammar.py` & `parsimonious-lite-0.8.0/parsimonious_lite/tests/test_grammar.py`

 * *Files identical despite different names*

### Comparing `parsimonious-lite-0.11.0/parsimonious_lite/tests/test_nodes.py` & `parsimonious-lite-0.8.0/parsimonious_lite/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `parsimonious-lite-0.11.0/parsimonious_lite/utils.py` & `parsimonious-lite-0.8.0/parsimonious_lite/utils.py`

 * *Files identical despite different names*

### Comparing `parsimonious-lite-0.11.0/parsimonious_lite.egg-info/PKG-INFO` & `parsimonious-lite-0.8.0/parsimonious_lite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsimonious-lite
-Version: 0.11.0
+Version: 0.8.0
 Summary: lite fork of parsimonious 0.8.0 for compatibility with python 3.11
 Keywords: parse,parser,parsing,peg,packrat,grammar,language
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `parsimonious-lite-0.11.0/parsimonious_lite.egg-info/SOURCES.txt` & `parsimonious-lite-0.8.0/parsimonious_lite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parsimonious-lite-0.11.0/setup.py` & `parsimonious-lite-0.8.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from io import open
 from setuptools import setup, find_packages
 
 long_description=open('README.rst', 'r', encoding='utf8').read()
 
 setup(
     name='parsimonious-lite',
-    version='0.11.0',
+    version='0.8.0',
     description='lite fork of parsimonious 0.8.0 for compatibility with python 3.11',
     packages=find_packages(exclude=['ez_setup']),
     tests_require=['nose'],
     test_suite='nose.collector',
     include_package_data=True,
     install_requires=['six>=1.9.0'],
     classifiers=[
```

