# Comparing `tmp/py-unused-deps-0.2.0.tar.gz` & `tmp/py-unused-deps-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-unused-deps-0.2.0.tar", last modified: Sun Jan 15 20:11:00 2023, max compression
+gzip compressed data, was "py-unused-deps-0.2.1.tar", last modified: Sun Apr  9 20:36:41 2023, max compression
```

## Comparing `py-unused-deps-0.2.0.tar` & `py-unused-deps-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 mjh       (1000) mjh       (1000)        0 2023-01-15 20:11:00.680663 py-unused-deps-0.2.0/
--rw-r--r--   0 mjh       (1000) mjh       (1000)    18092 2023-01-07 15:04:16.000000 py-unused-deps-0.2.0/LICENSE
--rw-r--r--   0 mjh       (1000) mjh       (1000)     5890 2023-01-15 20:11:00.680663 py-unused-deps-0.2.0/PKG-INFO
--rw-r--r--   0 mjh       (1000) mjh       (1000)     5224 2023-01-07 14:57:55.000000 py-unused-deps-0.2.0/README.md
-drwxr-xr-x   0 mjh       (1000) mjh       (1000)        0 2023-01-15 20:11:00.680663 py-unused-deps-0.2.0/py_unused_deps.egg-info/
--rw-r--r--   0 mjh       (1000) mjh       (1000)     5890 2023-01-15 20:11:00.000000 py-unused-deps-0.2.0/py_unused_deps.egg-info/PKG-INFO
--rw-r--r--   0 mjh       (1000) mjh       (1000)      496 2023-01-15 20:11:00.000000 py-unused-deps-0.2.0/py_unused_deps.egg-info/SOURCES.txt
--rw-r--r--   0 mjh       (1000) mjh       (1000)        1 2023-01-15 20:11:00.000000 py-unused-deps-0.2.0/py_unused_deps.egg-info/dependency_links.txt
--rw-r--r--   0 mjh       (1000) mjh       (1000)       57 2023-01-15 20:11:00.000000 py-unused-deps-0.2.0/py_unused_deps.egg-info/entry_points.txt
--rw-r--r--   0 mjh       (1000) mjh       (1000)       99 2023-01-15 20:11:00.000000 py-unused-deps-0.2.0/py_unused_deps.egg-info/requires.txt
--rw-r--r--   0 mjh       (1000) mjh       (1000)       12 2023-01-15 20:11:00.000000 py-unused-deps-0.2.0/py_unused_deps.egg-info/top_level.txt
--rw-r--r--   0 mjh       (1000) mjh       (1000)     1625 2023-01-15 20:11:00.680663 py-unused-deps-0.2.0/setup.cfg
--rw-r--r--   0 mjh       (1000) mjh       (1000)       38 2022-09-30 21:07:55.000000 py-unused-deps-0.2.0/setup.py
-drwxr-xr-x   0 mjh       (1000) mjh       (1000)        0 2023-01-15 20:11:00.680663 py-unused-deps-0.2.0/unused_deps/
--rw-r--r--   0 mjh       (1000) mjh       (1000)        9 2022-09-30 20:04:47.000000 py-unused-deps-0.2.0/unused_deps/__init__.py
--rw-r--r--   0 mjh       (1000) mjh       (1000)       91 2022-10-02 15:27:05.000000 py-unused-deps-0.2.0/unused_deps/__main__.py
--rw-r--r--   0 mjh       (1000) mjh       (1000)      356 2022-10-02 13:39:33.000000 py-unused-deps-0.2.0/unused_deps/compat.py
--rw-r--r--   0 mjh       (1000) mjh       (1000)     2291 2023-01-03 11:03:42.000000 py-unused-deps-0.2.0/unused_deps/config.py
--rw-r--r--   0 mjh       (1000) mjh       (1000)     2941 2022-12-16 22:04:00.000000 py-unused-deps-0.2.0/unused_deps/dist_info.py
--rw-r--r--   0 mjh       (1000) mjh       (1000)      559 2022-12-16 22:04:00.000000 py-unused-deps-0.2.0/unused_deps/errors.py
--rw-r--r--   0 mjh       (1000) mjh       (1000)     1526 2022-12-16 22:04:00.000000 py-unused-deps-0.2.0/unused_deps/files.py
--rw-r--r--   0 mjh       (1000) mjh       (1000)      728 2022-12-16 22:04:00.000000 py-unused-deps-0.2.0/unused_deps/import_finder.py
--rw-r--r--   0 mjh       (1000) mjh       (1000)     5540 2023-01-03 11:03:42.000000 py-unused-deps-0.2.0/unused_deps/main.py
--rw-r--r--   0 mjh       (1000) mjh       (1000)        0 2022-10-09 09:37:56.000000 py-unused-deps-0.2.0/unused_deps/py.typed
+drwxr-xr-x   0 mjh       (1000) mjh       (1000)        0 2023-04-09 20:36:41.323624 py-unused-deps-0.2.1/
+-rw-r--r--   0 mjh       (1000) mjh       (1000)    18092 2023-01-07 15:04:16.000000 py-unused-deps-0.2.1/LICENSE
+-rw-r--r--   0 mjh       (1000) mjh       (1000)     5952 2023-04-09 20:36:41.323624 py-unused-deps-0.2.1/PKG-INFO
+-rw-r--r--   0 mjh       (1000) mjh       (1000)     5224 2023-01-07 14:57:55.000000 py-unused-deps-0.2.1/README.md
+drwxr-xr-x   0 mjh       (1000) mjh       (1000)        0 2023-04-09 20:36:41.323624 py-unused-deps-0.2.1/py_unused_deps.egg-info/
+-rw-r--r--   0 mjh       (1000) mjh       (1000)     5952 2023-04-09 20:36:41.000000 py-unused-deps-0.2.1/py_unused_deps.egg-info/PKG-INFO
+-rw-r--r--   0 mjh       (1000) mjh       (1000)      496 2023-04-09 20:36:41.000000 py-unused-deps-0.2.1/py_unused_deps.egg-info/SOURCES.txt
+-rw-r--r--   0 mjh       (1000) mjh       (1000)        1 2023-04-09 20:36:41.000000 py-unused-deps-0.2.1/py_unused_deps.egg-info/dependency_links.txt
+-rw-r--r--   0 mjh       (1000) mjh       (1000)       57 2023-04-09 20:36:41.000000 py-unused-deps-0.2.1/py_unused_deps.egg-info/entry_points.txt
+-rw-r--r--   0 mjh       (1000) mjh       (1000)       99 2023-04-09 20:36:41.000000 py-unused-deps-0.2.1/py_unused_deps.egg-info/requires.txt
+-rw-r--r--   0 mjh       (1000) mjh       (1000)       12 2023-04-09 20:36:41.000000 py-unused-deps-0.2.1/py_unused_deps.egg-info/top_level.txt
+-rw-r--r--   0 mjh       (1000) mjh       (1000)     1682 2023-04-09 20:36:41.326957 py-unused-deps-0.2.1/setup.cfg
+-rw-r--r--   0 mjh       (1000) mjh       (1000)       38 2022-09-30 21:07:55.000000 py-unused-deps-0.2.1/setup.py
+drwxr-xr-x   0 mjh       (1000) mjh       (1000)        0 2023-04-09 20:36:41.323624 py-unused-deps-0.2.1/unused_deps/
+-rw-r--r--   0 mjh       (1000) mjh       (1000)        9 2022-09-30 20:04:47.000000 py-unused-deps-0.2.1/unused_deps/__init__.py
+-rw-r--r--   0 mjh       (1000) mjh       (1000)       91 2022-10-02 15:27:05.000000 py-unused-deps-0.2.1/unused_deps/__main__.py
+-rw-r--r--   0 mjh       (1000) mjh       (1000)      356 2022-10-02 13:39:33.000000 py-unused-deps-0.2.1/unused_deps/compat.py
+-rw-r--r--   0 mjh       (1000) mjh       (1000)     2291 2023-01-03 11:03:42.000000 py-unused-deps-0.2.1/unused_deps/config.py
+-rw-r--r--   0 mjh       (1000) mjh       (1000)     2941 2022-12-16 22:04:00.000000 py-unused-deps-0.2.1/unused_deps/dist_info.py
+-rw-r--r--   0 mjh       (1000) mjh       (1000)      559 2022-12-16 22:04:00.000000 py-unused-deps-0.2.1/unused_deps/errors.py
+-rw-r--r--   0 mjh       (1000) mjh       (1000)     1526 2022-12-16 22:04:00.000000 py-unused-deps-0.2.1/unused_deps/files.py
+-rw-r--r--   0 mjh       (1000) mjh       (1000)      728 2022-12-16 22:04:00.000000 py-unused-deps-0.2.1/unused_deps/import_finder.py
+-rw-r--r--   0 mjh       (1000) mjh       (1000)     5540 2023-01-03 11:03:42.000000 py-unused-deps-0.2.1/unused_deps/main.py
+-rw-r--r--   0 mjh       (1000) mjh       (1000)        0 2022-10-09 09:37:56.000000 py-unused-deps-0.2.1/unused_deps/py.typed
```

### Comparing `py-unused-deps-0.2.0/LICENSE` & `py-unused-deps-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-unused-deps-0.2.0/PKG-INFO` & `py-unused-deps-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: py-unused-deps
-Version: 0.2.0
+Version: 0.2.1
 Summary: Find unused dependencies
+Home-page: https://github.com/matthewhughes934/py-unused-deps
 Author: Matthew Hughes
 Author-email: matthewhughes934@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `py-unused-deps-0.2.0/README.md` & `py-unused-deps-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `py-unused-deps-0.2.0/py_unused_deps.egg-info/PKG-INFO` & `py-unused-deps-0.2.1/py_unused_deps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: py-unused-deps
-Version: 0.2.0
+Version: 0.2.1
 Summary: Find unused dependencies
+Home-page: https://github.com/matthewhughes934/py-unused-deps
 Author: Matthew Hughes
 Author-email: matthewhughes934@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `py-unused-deps-0.2.0/setup.cfg` & `py-unused-deps-0.2.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [metadata]
 name = py-unused-deps
-version = 0.2.0
+version = 0.2.1
 author = Matthew Hughes
 author_email = matthewhughes934@gmail.com
 description = Find unused dependencies
 long_description = file: README.md
 long_description_content_type = text/markdown
+url = https://github.com/matthewhughes934/py-unused-deps
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
```

### Comparing `py-unused-deps-0.2.0/unused_deps/config.py` & `py-unused-deps-0.2.1/unused_deps/config.py`

 * *Files identical despite different names*

### Comparing `py-unused-deps-0.2.0/unused_deps/dist_info.py` & `py-unused-deps-0.2.1/unused_deps/dist_info.py`

 * *Files identical despite different names*

### Comparing `py-unused-deps-0.2.0/unused_deps/errors.py` & `py-unused-deps-0.2.1/unused_deps/errors.py`

 * *Files identical despite different names*

### Comparing `py-unused-deps-0.2.0/unused_deps/files.py` & `py-unused-deps-0.2.1/unused_deps/files.py`

 * *Files identical despite different names*

### Comparing `py-unused-deps-0.2.0/unused_deps/import_finder.py` & `py-unused-deps-0.2.1/unused_deps/import_finder.py`

 * *Files identical despite different names*

### Comparing `py-unused-deps-0.2.0/unused_deps/main.py` & `py-unused-deps-0.2.1/unused_deps/main.py`

 * *Files identical despite different names*

