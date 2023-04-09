# Comparing `tmp/dxsp-0.0.7.tar.gz` & `tmp/dxsp-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-0.0.7.tar", last modified: Sun Apr  9 12:50:43 2023, max compression
+gzip compressed data, was "dxsp-0.0.8.tar", last modified: Sun Apr  9 12:56:31 2023, max compression
```

## Comparing `dxsp-0.0.7.tar` & `dxsp-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:50:43.075862 dxsp-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-09 12:50:33.000000 dxsp-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-09 12:50:43.075862 dxsp-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-09 12:50:33.000000 dxsp-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:50:43.075862 dxsp-0.0.7/dxsp/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-09 12:50:33.000000 dxsp-0.0.7/dxsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-04-09 12:50:33.000000 dxsp-0.0.7/dxsp/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-09 12:50:33.000000 dxsp-0.0.7/dxsp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:50:43.075862 dxsp-0.0.7/dxsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-09 12:50:43.000000 dxsp-0.0.7/dxsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-09 12:50:43.000000 dxsp-0.0.7/dxsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 12:50:43.000000 dxsp-0.0.7/dxsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 12:50:43.000000 dxsp-0.0.7/dxsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-09 12:50:33.000000 dxsp-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 12:50:43.075862 dxsp-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:56:31.575496 dxsp-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-09 12:56:20.000000 dxsp-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-09 12:56:31.575496 dxsp-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-09 12:56:20.000000 dxsp-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:56:31.575496 dxsp-0.0.8/dxsp/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-09 12:56:20.000000 dxsp-0.0.8/dxsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-04-09 12:56:20.000000 dxsp-0.0.8/dxsp/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-09 12:56:20.000000 dxsp-0.0.8/dxsp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:56:31.575496 dxsp-0.0.8/dxsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-04-09 12:56:31.000000 dxsp-0.0.8/dxsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-09 12:56:31.000000 dxsp-0.0.8/dxsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 12:56:31.000000 dxsp-0.0.8/dxsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 12:56:31.000000 dxsp-0.0.8/dxsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-09 12:56:20.000000 dxsp-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 12:56:31.575496 dxsp-0.0.8/setup.cfg
```

### Comparing `dxsp-0.0.7/LICENSE` & `dxsp-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-0.0.7/PKG-INFO` & `dxsp-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 0.0.7
+Version: 0.0.8
 Summary: DXSP (DeX SwaP), A defi swap helper package. Easy peasy Swap.
 Author: MrAniki
 Project-URL: Homepage, https://github.com/mraniki/dxsp
 Project-URL: Bug Tracker, https://github.com/mraniki/dxsp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dxsp-0.0.7/README.md` & `dxsp-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-0.0.7/dxsp/main.py` & `dxsp-0.0.8/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-0.0.7/dxsp/utils.py` & `dxsp-0.0.8/dxsp/utils.py`

 * *Files identical despite different names*

### Comparing `dxsp-0.0.7/dxsp.egg-info/PKG-INFO` & `dxsp-0.0.8/dxsp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 0.0.7
+Version: 0.0.8
 Summary: DXSP (DeX SwaP), A defi swap helper package. Easy peasy Swap.
 Author: MrAniki
 Project-URL: Homepage, https://github.com/mraniki/dxsp
 Project-URL: Bug Tracker, https://github.com/mraniki/dxsp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dxsp-0.0.7/pyproject.toml` & `dxsp-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dxsp"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="MrAniki" },
 ]
 description = "DXSP (DeX SwaP), A defi swap helper package. Easy peasy Swap."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

