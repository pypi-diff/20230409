# Comparing `tmp/backend_sqlalchemy-0.1.3.tar.gz` & `tmp/backend_sqlalchemy-0.1.4.dev1681023002.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend_sqlalchemy-0.1.3.tar", max compression
+gzip compressed data, was "backend_sqlalchemy-0.1.4.dev1681023002.tar", max compression
```

## Comparing `backend_sqlalchemy-0.1.3.tar` & `backend_sqlalchemy-0.1.4.dev1681023002.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      197 2023-04-08 18:08:33.435244 backend_sqlalchemy-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-04-08 18:08:33.435244 backend_sqlalchemy-0.1.3/backend_sqlalchemy/__init__.py
--rw-r--r--   0        0        0      179 2023-04-08 18:08:33.435244 backend_sqlalchemy-0.1.3/backend_sqlalchemy/main.py
--rw-r--r--   0        0        0     1400 2023-04-08 18:08:59.204162 backend_sqlalchemy-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1412 1970-01-01 00:00:00.000000 backend_sqlalchemy-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      291 2023-04-09 06:49:43.038254 backend_sqlalchemy-0.1.4.dev1681023002/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 06:49:43.038254 backend_sqlalchemy-0.1.4.dev1681023002/backend_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      248 2023-04-09 06:49:43.038254 backend_sqlalchemy-0.1.4.dev1681023002/backend_sqlalchemy/main.py
+-rw-r--r--   0        0        0     1415 2023-04-09 06:50:03.518454 backend_sqlalchemy-0.1.4.dev1681023002/pyproject.toml
+-rw-r--r--   0        0        0     1520 1970-01-01 00:00:00.000000 backend_sqlalchemy-0.1.4.dev1681023002/PKG-INFO
```

### Comparing `backend_sqlalchemy-0.1.3/pyproject.toml` & `backend_sqlalchemy-0.1.4.dev1681023002/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "backend-sqlalchemy"
 packages = [{include = "backend_sqlalchemy"}]
-version = "0.1.3"
+version = "0.1.4.dev.1681023002"
 description = "Core for SQLAlchemy"
 authors = ["Martin More <martinmore@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["sqlalchemy", "python", "backend"]
 
 homepage = "https://example.com/"
```

### Comparing `backend_sqlalchemy-0.1.3/PKG-INFO` & `backend_sqlalchemy-0.1.4.dev1681023002/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend-sqlalchemy
-Version: 0.1.3
+Version: 0.1.4.dev1681023002
 Summary: Core for SQLAlchemy
 Home-page: https://example.com/
 License: MIT
 Keywords: sqlalchemy,python,backend
 Author: Martin More
 Author-email: martinmore@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -27,7 +27,13 @@
 Description-Content-Type: text/markdown
 
 # Backend SQLAlchemy
 
 
 [![codecov](https://codecov.io/gh/martinmore-team/backend-sqlalchemy/branch/main/graph/badge.svg?token=XJER9LZAZV)](https://codecov.io/gh/martinmore-team/backend-sqlalchemy)
 
+
+## Tests
+
+- poetry run coverage run -m pytest --showlocals -vv
+- poetry run coverage xml -i
+
```

