# Comparing `tmp/database_setup_tools-1.3.0.tar.gz` & `tmp/database_setup_tools-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_setup_tools-1.3.0.tar", max compression
+gzip compressed data, was "database_setup_tools-1.3.1.tar", max compression
```

## Comparing `database_setup_tools-1.3.0.tar` & `database_setup_tools-1.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-04-09 10:35:41.748398 database_setup_tools-1.3.0/LICENSE
--rw-r--r--   0        0        0     2579 2023-04-09 10:35:41.748398 database_setup_tools-1.3.0/README.md
--rw-r--r--   0        0        0       20 2023-04-09 10:35:52.520576 database_setup_tools-1.3.0/database_setup_tools/__init__.py
--rw-r--r--   0        0        0     2646 2023-04-09 10:35:41.748398 database_setup_tools-1.3.0/database_setup_tools/session_manager.py
--rw-r--r--   0        0        0     4067 2023-04-09 10:35:41.748398 database_setup_tools-1.3.0/database_setup_tools/setup.py
--rw-r--r--   0        0        0      955 2023-04-09 10:35:52.520576 database_setup_tools-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3215 1970-01-01 00:00:00.000000 database_setup_tools-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-09 15:43:15.706477 database_setup_tools-1.3.1/LICENSE
+-rw-r--r--   0        0        0     2579 2023-04-09 15:43:15.706477 database_setup_tools-1.3.1/README.md
+-rw-r--r--   0        0        0      147 2023-04-09 15:43:25.122341 database_setup_tools-1.3.1/database_setup_tools/__init__.py
+-rw-r--r--   0        0        0     2646 2023-04-09 15:43:15.706477 database_setup_tools-1.3.1/database_setup_tools/session_manager.py
+-rw-r--r--   0        0        0     4067 2023-04-09 15:43:15.706477 database_setup_tools-1.3.1/database_setup_tools/setup.py
+-rw-r--r--   0        0        0      955 2023-04-09 15:43:25.122341 database_setup_tools-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3215 1970-01-01 00:00:00.000000 database_setup_tools-1.3.1/PKG-INFO
```

### Comparing `database_setup_tools-1.3.0/LICENSE` & `database_setup_tools-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `database_setup_tools-1.3.0/README.md` & `database_setup_tools-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `database_setup_tools-1.3.0/database_setup_tools/session_manager.py` & `database_setup_tools-1.3.1/database_setup_tools/session_manager.py`

 * *Files identical despite different names*

### Comparing `database_setup_tools-1.3.0/database_setup_tools/setup.py` & `database_setup_tools-1.3.1/database_setup_tools/setup.py`

 * *Files identical despite different names*

### Comparing `database_setup_tools-1.3.0/pyproject.toml` & `database_setup_tools-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "database-setup-tools"
-version = "1.3.0"
+version = "1.3.1"
 description = "Tools to easily setup databases opinionated towards FastAPI and SQLModel"
 authors = ["Jonas Scholl <jonas@code-specialist.com>", "Yannic Schröer <yannic@code-specialist.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "database_setup_tools" }]
 
 [tool.poetry.dependencies]
```

### Comparing `database_setup_tools-1.3.0/PKG-INFO` & `database_setup_tools-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-setup-tools
-Version: 1.3.0
+Version: 1.3.1
 Summary: Tools to easily setup databases opinionated towards FastAPI and SQLModel
 License: MIT
 Author: Jonas Scholl
 Author-email: jonas@code-specialist.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

