# Comparing `tmp/flet_pyodide-0.6.0.dev1293.tar.gz` & `tmp/flet_pyodide-0.6.0.dev1294.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_pyodide-0.6.0.dev1293.tar", max compression
+gzip compressed data, was "flet_pyodide-0.6.0.dev1294.tar", max compression
```

## Comparing `flet_pyodide-0.6.0.dev1293.tar` & `flet_pyodide-0.6.0.dev1294.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2264 2023-04-07 16:29:36.673248 flet_pyodide-0.6.0.dev1293/README.md
--rw-r--r--   0        0        0      644 2023-04-07 16:30:17.857266 flet_pyodide-0.6.0.dev1293/pyproject.toml
--rw-r--r--   0        0        0      101 2023-04-07 16:29:36.677248 flet_pyodide-0.6.0.dev1293/src/flet/__init__.py
--rw-r--r--   0        0        0     2377 2023-04-07 16:29:36.677248 flet_pyodide-0.6.0.dev1293/src/flet/flet.py
--rw-r--r--   0        0        0       55 2023-04-07 16:29:36.677248 flet_pyodide-0.6.0.dev1293/src/flet/matplotlib_chart.py
--rw-r--r--   0        0        0       47 2023-04-07 16:29:36.677248 flet_pyodide-0.6.0.dev1293/src/flet/plotly_chart.py
--rw-r--r--   0        0        0     3861 2023-04-07 16:29:36.677248 flet_pyodide-0.6.0.dev1293/src/flet/pyodide_connection.py
--rw-r--r--   0        0        0      103 2023-04-07 16:30:17.293266 flet_pyodide-0.6.0.dev1293/src/flet/version.py
--rw-r--r--   0        0        0     3007 1970-01-01 00:00:00.000000 flet_pyodide-0.6.0.dev1293/PKG-INFO
+-rw-r--r--   0        0        0     2264 2023-04-09 01:08:32.293865 flet_pyodide-0.6.0.dev1294/README.md
+-rw-r--r--   0        0        0      644 2023-04-09 01:09:04.303828 flet_pyodide-0.6.0.dev1294/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-04-09 01:08:32.293865 flet_pyodide-0.6.0.dev1294/src/flet/__init__.py
+-rw-r--r--   0        0        0     2377 2023-04-09 01:08:32.293865 flet_pyodide-0.6.0.dev1294/src/flet/flet.py
+-rw-r--r--   0        0        0       55 2023-04-09 01:08:32.293865 flet_pyodide-0.6.0.dev1294/src/flet/matplotlib_chart.py
+-rw-r--r--   0        0        0       47 2023-04-09 01:08:32.293865 flet_pyodide-0.6.0.dev1294/src/flet/plotly_chart.py
+-rw-r--r--   0        0        0     3861 2023-04-09 01:08:32.293865 flet_pyodide-0.6.0.dev1294/src/flet/pyodide_connection.py
+-rw-r--r--   0        0        0      103 2023-04-09 01:09:03.635800 flet_pyodide-0.6.0.dev1294/src/flet/version.py
+-rw-r--r--   0        0        0     3007 1970-01-01 00:00:00.000000 flet_pyodide-0.6.0.dev1294/PKG-INFO
```

### Comparing `flet_pyodide-0.6.0.dev1293/README.md` & `flet_pyodide-0.6.0.dev1294/README.md`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.6.0.dev1293/pyproject.toml` & `flet_pyodide-0.6.0.dev1294/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-pyodide"
-version = "0.6.0.dev1293"
+version = "0.6.0.dev1294"
 description = "Flet for Pyodide - build standalone SPA in Python with Flutter UI."
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet", from = "src" },
@@ -12,15 +12,15 @@
 
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
-flet-core = "0.6.0.dev1293"
+flet-core = "0.6.0.dev1294"
 python = "^3.9"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
```

### Comparing `flet_pyodide-0.6.0.dev1293/src/flet/flet.py` & `flet_pyodide-0.6.0.dev1294/src/flet/flet.py`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.6.0.dev1293/src/flet/pyodide_connection.py` & `flet_pyodide-0.6.0.dev1294/src/flet/pyodide_connection.py`

 * *Files identical despite different names*

### Comparing `flet_pyodide-0.6.0.dev1293/PKG-INFO` & `flet_pyodide-0.6.0.dev1294/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: flet-pyodide
-Version: 0.6.0.dev1293
+Version: 0.6.0.dev1294
 Summary: Flet for Pyodide - build standalone SPA in Python with Flutter UI.
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: flet-core (==0.6.0.dev1293)
+Requires-Dist: flet-core (==0.6.0.dev1294)
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
 Project-URL: repository, https://github.com/flet-dev/flet
 Description-Content-Type: text/markdown
 
 # Flet for Pyodide - build standalone Single-Page Applications (SPA) in Python with Flutter UI
```

