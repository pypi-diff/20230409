# Comparing `tmp/sqlmodel_repository-1.0.0.tar.gz` & `tmp/sqlmodel_repository-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmodel_repository-1.0.0.tar", max compression
+gzip compressed data, was "sqlmodel_repository-1.0.1.tar", max compression
```

## Comparing `sqlmodel_repository-1.0.0.tar` & `sqlmodel_repository-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     5575 2023-04-09 10:58:27.814587 sqlmodel_repository-1.0.0/README.md
--rw-r--r--   0        0        0     1501 2023-04-09 10:58:47.490261 sqlmodel_repository-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       20 2023-04-09 10:58:47.490261 sqlmodel_repository-1.0.0/sqlmodel_repository/__init__.py
--rw-r--r--   0        0        0     7762 2023-04-09 10:58:27.818587 sqlmodel_repository-1.0.0/sqlmodel_repository/base_repository.py
--rw-r--r--   0        0        0      167 2023-04-09 10:58:27.818587 sqlmodel_repository-1.0.0/sqlmodel_repository/entity.py
--rw-r--r--   0        0        0      589 2023-04-09 10:58:27.818587 sqlmodel_repository-1.0.0/sqlmodel_repository/exceptions.py
--rw-r--r--   0        0        0     5842 2023-04-09 10:58:27.818587 sqlmodel_repository-1.0.0/sqlmodel_repository/repository.py
--rw-r--r--   0        0        0     6189 1970-01-01 00:00:00.000000 sqlmodel_repository-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     5575 2023-04-09 15:36:30.440790 sqlmodel_repository-1.0.1/README.md
+-rw-r--r--   0        0        0     1501 2023-04-09 15:36:53.925351 sqlmodel_repository-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      199 2023-04-09 15:36:53.921350 sqlmodel_repository-1.0.1/sqlmodel_repository/__init__.py
+-rw-r--r--   0        0        0     7762 2023-04-09 15:36:30.440790 sqlmodel_repository-1.0.1/sqlmodel_repository/base_repository.py
+-rw-r--r--   0        0        0      167 2023-04-09 15:36:30.440790 sqlmodel_repository-1.0.1/sqlmodel_repository/entity.py
+-rw-r--r--   0        0        0      589 2023-04-09 15:36:30.440790 sqlmodel_repository-1.0.1/sqlmodel_repository/exceptions.py
+-rw-r--r--   0        0        0     5842 2023-04-09 15:36:30.440790 sqlmodel_repository-1.0.1/sqlmodel_repository/repository.py
+-rw-r--r--   0        0        0     6189 1970-01-01 00:00:00.000000 sqlmodel_repository-1.0.1/PKG-INFO
```

### Comparing `sqlmodel_repository-1.0.0/README.md` & `sqlmodel_repository-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlmodel_repository-1.0.0/pyproject.toml` & `sqlmodel_repository-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.poetry]
 authors = ["Jonas Scholl <jonas@code-specialist.com>", "Yannic Schröer <yannic@code-specialist.com>"]
 description = "Repository pattern implementation for SQLModel (SQLAlchemy)"
 license = "MIT"
 name = "sqlmodel-repository"
 readme = "README.md"
-version = "1.0.0"
+version = "1.0.1"
 
 [tool.poetry.dependencies]
 database-setup-tools = "1.3.0"
 python = "^3.9"
 sqlmodel = "^0.0.8"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `sqlmodel_repository-1.0.0/sqlmodel_repository/base_repository.py` & `sqlmodel_repository-1.0.1/sqlmodel_repository/base_repository.py`

 * *Files identical despite different names*

### Comparing `sqlmodel_repository-1.0.0/sqlmodel_repository/exceptions.py` & `sqlmodel_repository-1.0.1/sqlmodel_repository/exceptions.py`

 * *Files identical despite different names*

### Comparing `sqlmodel_repository-1.0.0/sqlmodel_repository/repository.py` & `sqlmodel_repository-1.0.1/sqlmodel_repository/repository.py`

 * *Files identical despite different names*

### Comparing `sqlmodel_repository-1.0.0/PKG-INFO` & `sqlmodel_repository-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmodel-repository
-Version: 1.0.0
+Version: 1.0.1
 Summary: Repository pattern implementation for SQLModel (SQLAlchemy)
 License: MIT
 Author: Jonas Scholl
 Author-email: jonas@code-specialist.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

