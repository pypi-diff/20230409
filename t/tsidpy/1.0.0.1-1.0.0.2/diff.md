# Comparing `tmp/tsidpy-1.0.0.1.tar.gz` & `tmp/tsidpy-1.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsidpy-1.0.0.1.tar", last modified: Sun Apr  9 01:00:32 2023, max compression
+gzip compressed data, was "tsidpy-1.0.0.2.tar", last modified: Sun Apr  9 01:32:04 2023, max compression
```

## Comparing `tsidpy-1.0.0.1.tar` & `tsidpy-1.0.0.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 luis       (504) staff       (20)        0 2023-04-09 01:00:32.772892 tsidpy-1.0.0.1/
--rw-r--r--   0 luis       (504) staff       (20)    10120 2023-04-09 01:00:32.772514 tsidpy-1.0.0.1/PKG-INFO
--rw-r--r--   0 luis       (504) staff       (20)     9823 2023-04-09 00:59:25.000000 tsidpy-1.0.0.1/README.md
--rw-r--r--   0 luis       (504) staff       (20)       38 2023-04-09 01:00:32.772983 tsidpy-1.0.0.1/setup.cfg
--rw-r--r--   0 luis       (504) staff       (20)      604 2023-04-09 01:00:03.000000 tsidpy-1.0.0.1/setup.py
-drwxr-xr-x   0 luis       (504) staff       (20)        0 2023-04-09 01:00:32.769824 tsidpy-1.0.0.1/tsidpy/
--rw-r--r--   0 luis       (504) staff       (20)       51 2023-04-08 23:04:41.000000 tsidpy-1.0.0.1/tsidpy/__init__.py
--rw-r--r--   0 luis       (504) staff       (20)      690 2023-04-07 23:41:36.000000 tsidpy-1.0.0.1/tsidpy/basen.py
--rw-r--r--   0 luis       (504) staff       (20)    14728 2023-04-09 00:00:39.000000 tsidpy-1.0.0.1/tsidpy/tsid.py
-drwxr-xr-x   0 luis       (504) staff       (20)        0 2023-04-09 01:00:32.771963 tsidpy-1.0.0.1/tsidpy.egg-info/
--rw-r--r--   0 luis       (504) staff       (20)    10120 2023-04-09 01:00:32.000000 tsidpy-1.0.0.1/tsidpy.egg-info/PKG-INFO
--rw-r--r--   0 luis       (504) staff       (20)      188 2023-04-09 01:00:32.000000 tsidpy-1.0.0.1/tsidpy.egg-info/SOURCES.txt
--rw-r--r--   0 luis       (504) staff       (20)        1 2023-04-09 01:00:32.000000 tsidpy-1.0.0.1/tsidpy.egg-info/dependency_links.txt
--rw-r--r--   0 luis       (504) staff       (20)        7 2023-04-09 01:00:32.000000 tsidpy-1.0.0.1/tsidpy.egg-info/top_level.txt
+drwxr-xr-x   0 luis       (504) staff       (20)        0 2023-04-09 01:32:04.435378 tsidpy-1.0.0.2/
+-rw-r--r--   0 luis       (504) staff       (20)     1066 2023-04-09 01:27:26.000000 tsidpy-1.0.0.2/LICENSE
+-rw-r--r--   0 luis       (504) staff       (20)    10340 2023-04-09 01:32:04.434939 tsidpy-1.0.0.2/PKG-INFO
+-rw-r--r--   0 luis       (504) staff       (20)     9823 2023-04-09 00:59:25.000000 tsidpy-1.0.0.2/README.md
+-rw-r--r--   0 luis       (504) staff       (20)      594 2023-04-09 01:31:53.000000 tsidpy-1.0.0.2/pyproject.toml
+-rw-r--r--   0 luis       (504) staff       (20)       38 2023-04-09 01:32:04.435485 tsidpy-1.0.0.2/setup.cfg
+drwxr-xr-x   0 luis       (504) staff       (20)        0 2023-04-09 01:32:04.430499 tsidpy-1.0.0.2/src/
+drwxr-xr-x   0 luis       (504) staff       (20)        0 2023-04-09 01:32:04.432743 tsidpy-1.0.0.2/src/tsidpy/
+-rw-r--r--   0 luis       (504) staff       (20)       51 2023-04-08 23:04:41.000000 tsidpy-1.0.0.2/src/tsidpy/__init__.py
+-rw-r--r--   0 luis       (504) staff       (20)      690 2023-04-07 23:41:36.000000 tsidpy-1.0.0.2/src/tsidpy/basen.py
+-rw-r--r--   0 luis       (504) staff       (20)    14728 2023-04-09 00:00:39.000000 tsidpy-1.0.0.2/src/tsidpy/tsid.py
+drwxr-xr-x   0 luis       (504) staff       (20)        0 2023-04-09 01:32:04.434396 tsidpy-1.0.0.2/src/tsidpy.egg-info/
+-rw-r--r--   0 luis       (504) staff       (20)    10340 2023-04-09 01:32:04.000000 tsidpy-1.0.0.2/src/tsidpy.egg-info/PKG-INFO
+-rw-r--r--   0 luis       (504) staff       (20)      230 2023-04-09 01:32:04.000000 tsidpy-1.0.0.2/src/tsidpy.egg-info/SOURCES.txt
+-rw-r--r--   0 luis       (504) staff       (20)        1 2023-04-09 01:32:04.000000 tsidpy-1.0.0.2/src/tsidpy.egg-info/dependency_links.txt
+-rw-r--r--   0 luis       (504) staff       (20)        7 2023-04-09 01:32:04.000000 tsidpy-1.0.0.2/src/tsidpy.egg-info/top_level.txt
```

### Comparing `tsidpy-1.0.0.1/PKG-INFO` & `tsidpy-1.0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: tsidpy
-Version: 1.0.0.1
+Version: 1.0.0.2
 Summary: A Python library for generating Time-Sorted Unique Identifiers (TSID)
-Home-page: https://github.com/luismedel/tsid-python
-Maintainer: Luis Medel
-Maintainer-email: luis@luismedel.com
-License: MIT
+Author-email: Luis Medel <luis@luismedel.com>
+Project-URL: Homepage, https://github.com/luismedel/tsid-python
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # tsid-python
 
 A Python library for generating Time-Sorted Unique Identifiers (TSID) as defined in <https://github.com/f4b6a3/tsid-creator>.
 
 This library is a port of the original Java code by [Fabio Lima](https://github.com/fabiolimace).
```

### Comparing `tsidpy-1.0.0.1/README.md` & `tsidpy-1.0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tsidpy-1.0.0.1/tsidpy/basen.py` & `tsidpy-1.0.0.2/src/tsidpy/basen.py`

 * *Files identical despite different names*

### Comparing `tsidpy-1.0.0.1/tsidpy/tsid.py` & `tsidpy-1.0.0.2/src/tsidpy/tsid.py`

 * *Files identical despite different names*

### Comparing `tsidpy-1.0.0.1/tsidpy.egg-info/PKG-INFO` & `tsidpy-1.0.0.2/src/tsidpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: tsidpy
-Version: 1.0.0.1
+Version: 1.0.0.2
 Summary: A Python library for generating Time-Sorted Unique Identifiers (TSID)
-Home-page: https://github.com/luismedel/tsid-python
-Maintainer: Luis Medel
-Maintainer-email: luis@luismedel.com
-License: MIT
+Author-email: Luis Medel <luis@luismedel.com>
+Project-URL: Homepage, https://github.com/luismedel/tsid-python
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # tsid-python
 
 A Python library for generating Time-Sorted Unique Identifiers (TSID) as defined in <https://github.com/f4b6a3/tsid-creator>.
 
 This library is a port of the original Java code by [Fabio Lima](https://github.com/fabiolimace).
```

