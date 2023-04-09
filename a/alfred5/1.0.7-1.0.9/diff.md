# Comparing `tmp/alfred5-1.0.7.tar.gz` & `tmp/alfred5-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred5-1.0.7.tar", last modified: Mon Feb 20 20:00:02 2023, max compression
+gzip compressed data, was "alfred5-1.0.9.tar", last modified: Sun Apr  9 03:30:45 2023, max compression
```

## Comparing `alfred5-1.0.7.tar` & `alfred5-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 20:00:02.525087 alfred5-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-02-20 19:59:49.000000 alfred5-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-20 19:59:49.000000 alfred5-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-02-20 20:00:02.525087 alfred5-1.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 20:00:02.525087 alfred5-1.0.7/alfred5/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-20 19:59:49.000000 alfred5-1.0.7/alfred5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-02-20 19:59:49.000000 alfred5-1.0.7/alfred5/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 20:00:02.525087 alfred5-1.0.7/alfred5/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    25511 2023-02-20 19:59:49.000000 alfred5-1.0.7/alfred5/icons/error.png
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-02-20 19:59:49.000000 alfred5-1.0.7/alfred5/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 20:00:02.525087 alfred5-1.0.7/alfred5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-02-20 20:00:02.000000 alfred5-1.0.7/alfred5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-20 20:00:02.000000 alfred5-1.0.7/alfred5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 20:00:02.000000 alfred5-1.0.7/alfred5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 20:00:02.000000 alfred5-1.0.7/alfred5.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-20 20:00:02.000000 alfred5-1.0.7/alfred5.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-20 20:00:02.000000 alfred5-1.0.7/alfred5.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 20:00:02.525087 alfred5-1.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-02-20 19:59:49.000000 alfred5-1.0.7/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 20:00:02.525087 alfred5-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-02-20 19:59:49.000000 alfred5-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 20:00:02.525087 alfred5-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 19:59:49.000000 alfred5-1.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-20 19:59:49.000000 alfred5-1.0.7/tests/test_snippets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:30:45.533282 alfred5-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-09 03:30:36.000000 alfred5-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-09 03:30:36.000000 alfred5-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-09 03:30:45.533282 alfred5-1.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:30:45.529282 alfred5-1.0.9/alfred5/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-09 03:30:36.000000 alfred5-1.0.9/alfred5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-04-09 03:30:36.000000 alfred5-1.0.9/alfred5/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-09 03:30:36.000000 alfred5-1.0.9/alfred5/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:30:45.533282 alfred5-1.0.9/alfred5/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    35477 2023-04-09 03:30:36.000000 alfred5-1.0.9/alfred5/icons/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-09 03:30:36.000000 alfred5-1.0.9/alfred5/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:30:45.533282 alfred5-1.0.9/alfred5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-09 03:30:45.000000 alfred5-1.0.9/alfred5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-09 03:30:45.000000 alfred5-1.0.9/alfred5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 03:30:45.000000 alfred5-1.0.9/alfred5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 03:30:45.000000 alfred5-1.0.9/alfred5.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-09 03:30:45.000000 alfred5-1.0.9/alfred5.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-09 03:30:45.000000 alfred5-1.0.9/alfred5.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:30:45.533282 alfred5-1.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-09 03:30:36.000000 alfred5-1.0.9/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 03:30:45.533282 alfred5-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-09 03:30:36.000000 alfred5-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:30:45.533282 alfred5-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 03:30:36.000000 alfred5-1.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-09 03:30:36.000000 alfred5-1.0.9/tests/test_snippets.py
```

### Comparing `alfred5-1.0.7/LICENSE` & `alfred5-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alfred5-1.0.7/PKG-INFO` & `alfred5-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred5
-Version: 1.0.7
+Version: 1.0.9
 Summary: Simple python wrapper for alfred workflow / snippets
 Home-page: https://github.com/yedhrab/alfred5
 Author: Yunus Emre Ak
 Author-email: yemreak.com@gmail.com
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/yedhrab/alfred5/
 Project-URL: Documentation, https://github.com/yedhrab/alfred5/wiki
```

### Comparing `alfred5-1.0.7/alfred5/client.py` & `alfred5-1.0.9/alfred5/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from shutil import copy2, move
 from tempfile import TemporaryDirectory
 from zipfile import ZIP_DEFLATED, ZipFile
 from ruamel.yaml import load as yaml_load, dump as yaml_dump
 from plistlib import load as plist_load
 from .models import SNIPPET_INFO_TEMPLATE, Result, Snippet, yaml
 from typing import NoReturn
+from .errors import WorkflowError
 
 
 class SnippetClient:
     snippets: list[Snippet]
 
     def __init__(self) -> None:
         self.snippets: list[Snippet] = []
@@ -136,17 +137,20 @@
         ```
         """
         client = cls()
         try:
             run(func(client))
             client.response()
         except Exception as e:
-            client.error_response(
-                title=str(e), subtitle=format_exc().strip().split("\n")[-1]
-            )
+            if isinstance(e, WorkflowError):
+                client.error_response(title=e.title, subtitle=e.subtitle)
+            else:
+                client.error_response(
+                    title=str(e), subtitle=format_exc().strip().split("\n")[-1]
+                )
 
     def add_result(
         self,
         title: str,
         subtitle: str = "",
         icon_path: str | Path | None = None,
         arg: str = "",
```

### Comparing `alfred5-1.0.7/alfred5/models.py` & `alfred5-1.0.9/alfred5/models.py`

 * *Files identical despite different names*

### Comparing `alfred5-1.0.7/alfred5.egg-info/PKG-INFO` & `alfred5-1.0.9/alfred5.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred5
-Version: 1.0.7
+Version: 1.0.9
 Summary: Simple python wrapper for alfred workflow / snippets
 Home-page: https://github.com/yedhrab/alfred5
 Author: Yunus Emre Ak
 Author-email: yemreak.com@gmail.com
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/yedhrab/alfred5/
 Project-URL: Documentation, https://github.com/yedhrab/alfred5/wiki
```

### Comparing `alfred5-1.0.7/docs/README.md` & `alfred5-1.0.9/docs/README.md`

 * *Files identical despite different names*

### Comparing `alfred5-1.0.7/setup.py` & `alfred5-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from glob import glob
 from os.path import basename, splitext
 from setuptools import find_packages, setup
 from pathlib import Path
 
-VERSION = "1.0.7"
+VERSION = "1.0.9"
 README_PATH = "docs/README.md"
 USERNAME = "yedhrab"
 REPOSITORY = "alfred5"
 
 setup(
     name=REPOSITORY,
     version=VERSION,
```

