# Comparing `tmp/helperize-0.0.1.tar.gz` & `tmp/helperize-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helperize-0.0.1.tar", max compression
+gzip compressed data, was "helperize-0.0.4.tar", max compression
```

## Comparing `helperize-0.0.1.tar` & `helperize-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1074 2023-04-08 23:47:49.521257 helperize-0.0.1/LICENSE
--rw-r--r--   0        0        0      417 2023-04-09 00:11:02.766201 helperize-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-04-08 23:47:49.522516 helperize-0.0.1/helperize/__init__.py
--rw-r--r--   0        0        0        0 2023-04-08 23:47:49.522642 helperize-0.0.1/helperize/cli/__init__.py
--rw-r--r--   0        0        0      575 2023-04-08 23:56:07.793275 helperize-0.0.1/helperize/cli/cli.py
--rw-r--r--   0        0        0      230 2023-04-08 23:47:49.522883 helperize-0.0.1/helperize/interface.py
--rw-r--r--   0        0        0     1069 2023-04-08 23:47:49.523003 helperize-0.0.1/helperize/log.py
--rw-r--r--   0        0        0     1108 2023-04-09 00:11:25.263152 helperize-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 helperize-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-08 23:47:49.521257 helperize-0.0.4/LICENSE
+-rw-r--r--   0        0        0      417 2023-04-09 00:11:02.766201 helperize-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-08 23:47:49.522516 helperize-0.0.4/helperize/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-08 23:47:49.522642 helperize-0.0.4/helperize/cli/__init__.py
+-rw-r--r--   0        0        0      575 2023-04-08 23:56:07.793275 helperize-0.0.4/helperize/cli/cli.py
+-rw-r--r--   0        0        0      230 2023-04-08 23:47:49.522883 helperize-0.0.4/helperize/interface.py
+-rw-r--r--   0        0        0     1069 2023-04-08 23:47:49.523003 helperize-0.0.4/helperize/log.py
+-rw-r--r--   0        0        0     1108 2023-04-09 00:47:36.124632 helperize-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 helperize-0.0.4/PKG-INFO
```

### Comparing `helperize-0.0.1/LICENSE` & `helperize-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `helperize-0.0.1/helperize/cli/cli.py` & `helperize-0.0.4/helperize/cli/cli.py`

 * *Files identical despite different names*

### Comparing `helperize-0.0.1/helperize/log.py` & `helperize-0.0.4/helperize/log.py`

 * *Files identical despite different names*

### Comparing `helperize-0.0.1/pyproject.toml` & `helperize-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 authors = ["Michael Vogelsong <4020875+mjvogelsong@users.noreply.github.com>"]
 description = "Work with AI helpers that collaborate with you to build practical systems."
 license = "MIT"
 name = "helperize"
 readme = "README.md"
-version = "0.0.1"
+version = "0.0.4"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 rich = "^13.3.3"
 typer = "^0.7.0"
 
 [tool.poetry.group.lint.dependencies]
```

### Comparing `helperize-0.0.1/PKG-INFO` & `helperize-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helperize
-Version: 0.0.1
+Version: 0.0.4
 Summary: Work with AI helpers that collaborate with you to build practical systems.
 License: MIT
 Author: Michael Vogelsong
 Author-email: 4020875+mjvogelsong@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

