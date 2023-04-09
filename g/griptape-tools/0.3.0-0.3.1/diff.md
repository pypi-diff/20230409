# Comparing `tmp/griptape_tools-0.3.0.tar.gz` & `tmp/griptape_tools-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_tools-0.3.0.tar", max compression
+gzip compressed data, was "griptape_tools-0.3.1.tar", max compression
```

## Comparing `griptape_tools-0.3.0.tar` & `griptape_tools-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.3.0/LICENSE
--rw-r--r--   0        0        0      940 2023-04-06 20:56:04.343666 griptape_tools-0.3.0/README.md
--rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.3.0/griptape/__init__.py
--rw-r--r--   0        0        0      137 2023-04-07 15:29:21.691602 griptape_tools-0.3.0/griptape/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.3.0/griptape/tools/calculator/__init__.py
--rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.3.0/griptape/tools/calculator/manifest.yml
--rw-r--r--   0        0        0       20 2023-04-07 16:15:03.210825 griptape_tools-0.3.0/griptape/tools/calculator/requirements.txt
--rw-r--r--   0        0        0     1513 2023-04-09 16:48:43.512439 griptape_tools-0.3.0/griptape/tools/calculator/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.3.0/griptape/tools/google_search/__init__.py
--rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.3.0/griptape/tools/google_search/manifest.yml
--rw-r--r--   0        0        0       20 2023-04-07 16:15:03.213519 griptape_tools-0.3.0/griptape/tools/google_search/requirements.txt
--rw-r--r--   0        0        0     2436 2023-04-09 16:48:43.509967 griptape_tools-0.3.0/griptape/tools/google_search/tool.py
--rw-r--r--   0        0        0      525 2023-04-09 16:49:20.960108 griptape_tools-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 griptape_tools-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.3.1/LICENSE
+-rw-r--r--   0        0        0      940 2023-04-06 20:56:04.343666 griptape_tools-0.3.1/README.md
+-rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.3.1/griptape/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-07 15:29:21.691602 griptape_tools-0.3.1/griptape/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.3.1/griptape/tools/calculator/__init__.py
+-rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.3.1/griptape/tools/calculator/manifest.yml
+-rw-r--r--   0        0        0       20 2023-04-09 16:57:04.925786 griptape_tools-0.3.1/griptape/tools/calculator/requirements.txt
+-rw-r--r--   0        0        0     1513 2023-04-09 16:48:43.512439 griptape_tools-0.3.1/griptape/tools/calculator/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.3.1/griptape/tools/google_search/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.3.1/griptape/tools/google_search/manifest.yml
+-rw-r--r--   0        0        0       20 2023-04-09 16:57:04.927625 griptape_tools-0.3.1/griptape/tools/google_search/requirements.txt
+-rw-r--r--   0        0        0     2436 2023-04-09 16:48:43.509967 griptape_tools-0.3.1/griptape/tools/google_search/tool.py
+-rw-r--r--   0        0        0      525 2023-04-09 16:57:59.445954 griptape_tools-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 griptape_tools-0.3.1/PKG-INFO
```

### Comparing `griptape_tools-0.3.0/LICENSE` & `griptape_tools-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.3.0/README.md` & `griptape_tools-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.3.0/griptape/tools/calculator/tool.py` & `griptape_tools-0.3.1/griptape/tools/calculator/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.3.0/griptape/tools/google_search/tool.py` & `griptape_tools-0.3.1/griptape/tools/google_search/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.3.0/pyproject.toml` & `griptape_tools-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "griptape-tools"
-version = "0.3.0"
+version = "0.3.1"
 description = "Tools for the griptape-core package."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape-tools"
 
 packages = [
```

### Comparing `griptape_tools-0.3.0/PKG-INFO` & `griptape_tools-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griptape-tools
-Version: 0.3.0
+Version: 0.3.1
 Summary: Tools for the griptape-core package.
 Home-page: https://github.com/griptape-ai/griptape-tools
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

