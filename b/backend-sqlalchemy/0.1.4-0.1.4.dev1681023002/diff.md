# Comparing `tmp/backend_sqlalchemy-0.1.4.tar.gz` & `tmp/backend_sqlalchemy-0.1.4.dev1681023002.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend_sqlalchemy-0.1.4.tar", max compression
+gzip compressed data, was "backend_sqlalchemy-0.1.4.dev1681023002.tar", max compression
```

## Comparing `backend_sqlalchemy-0.1.4.tar` & `backend_sqlalchemy-0.1.4.dev1681023002.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      291 2023-04-09 06:53:30.854019 backend_sqlalchemy-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-04-09 06:53:30.854019 backend_sqlalchemy-0.1.4/backend_sqlalchemy/__init__.py
--rw-r--r--   0        0        0      248 2023-04-09 06:53:30.854019 backend_sqlalchemy-0.1.4/backend_sqlalchemy/main.py
--rw-r--r--   0        0        0     1400 2023-04-09 06:53:47.714198 backend_sqlalchemy-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1506 1970-01-01 00:00:00.000000 backend_sqlalchemy-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      291 2023-04-09 06:49:43.038254 backend_sqlalchemy-0.1.4.dev1681023002/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 06:49:43.038254 backend_sqlalchemy-0.1.4.dev1681023002/backend_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      248 2023-04-09 06:49:43.038254 backend_sqlalchemy-0.1.4.dev1681023002/backend_sqlalchemy/main.py
+-rw-r--r--   0        0        0     1415 2023-04-09 06:50:03.518454 backend_sqlalchemy-0.1.4.dev1681023002/pyproject.toml
+-rw-r--r--   0        0        0     1520 1970-01-01 00:00:00.000000 backend_sqlalchemy-0.1.4.dev1681023002/PKG-INFO
```

### Comparing `backend_sqlalchemy-0.1.4/pyproject.toml` & `backend_sqlalchemy-0.1.4.dev1681023002/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "backend-sqlalchemy"
 packages = [{include = "backend_sqlalchemy"}]
-version = "0.1.4"
+version = "0.1.4.dev.1681023002"
 description = "Core for SQLAlchemy"
 authors = ["Martin More <martinmore@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["sqlalchemy", "python", "backend"]
 
 homepage = "https://example.com/"
```

### Comparing `backend_sqlalchemy-0.1.4/PKG-INFO` & `backend_sqlalchemy-0.1.4.dev1681023002/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend-sqlalchemy
-Version: 0.1.4
+Version: 0.1.4.dev1681023002
 Summary: Core for SQLAlchemy
 Home-page: https://example.com/
 License: MIT
 Keywords: sqlalchemy,python,backend
 Author: Martin More
 Author-email: martinmore@gmail.com
 Requires-Python: >=3.10,<4.0
```

