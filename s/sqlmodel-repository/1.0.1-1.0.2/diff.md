# Comparing `tmp/sqlmodel_repository-1.0.1.tar.gz` & `tmp/sqlmodel_repository-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmodel_repository-1.0.1.tar", max compression
+gzip compressed data, was "sqlmodel_repository-1.0.2.tar", max compression
```

## Comparing `sqlmodel_repository-1.0.1.tar` & `sqlmodel_repository-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     5575 2023-04-09 15:36:30.440790 sqlmodel_repository-1.0.1/README.md
--rw-r--r--   0        0        0     1501 2023-04-09 15:36:53.925351 sqlmodel_repository-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      199 2023-04-09 15:36:53.921350 sqlmodel_repository-1.0.1/sqlmodel_repository/__init__.py
--rw-r--r--   0        0        0     7762 2023-04-09 15:36:30.440790 sqlmodel_repository-1.0.1/sqlmodel_repository/base_repository.py
--rw-r--r--   0        0        0      167 2023-04-09 15:36:30.440790 sqlmodel_repository-1.0.1/sqlmodel_repository/entity.py
--rw-r--r--   0        0        0      589 2023-04-09 15:36:30.440790 sqlmodel_repository-1.0.1/sqlmodel_repository/exceptions.py
--rw-r--r--   0        0        0     5842 2023-04-09 15:36:30.440790 sqlmodel_repository-1.0.1/sqlmodel_repository/repository.py
--rw-r--r--   0        0        0     6189 1970-01-01 00:00:00.000000 sqlmodel_repository-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-09 16:14:21.173404 sqlmodel_repository-1.0.2/LICENSE
+-rw-r--r--   0        0        0     5575 2023-04-09 16:14:21.173404 sqlmodel_repository-1.0.2/README.md
+-rw-r--r--   0        0        0     1502 2023-04-09 16:14:41.753399 sqlmodel_repository-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      199 2023-04-09 16:14:41.753399 sqlmodel_repository-1.0.2/sqlmodel_repository/__init__.py
+-rw-r--r--   0        0        0     7761 2023-04-09 16:14:21.177404 sqlmodel_repository-1.0.2/sqlmodel_repository/base_repository.py
+-rw-r--r--   0        0        0      167 2023-04-09 16:14:21.177404 sqlmodel_repository-1.0.2/sqlmodel_repository/entity.py
+-rw-r--r--   0        0        0      589 2023-04-09 16:14:21.177404 sqlmodel_repository-1.0.2/sqlmodel_repository/exceptions.py
+-rw-r--r--   0        0        0     5841 2023-04-09 16:14:21.177404 sqlmodel_repository-1.0.2/sqlmodel_repository/repository.py
+-rw-r--r--   0        0        0     6143 1970-01-01 00:00:00.000000 sqlmodel_repository-1.0.2/PKG-INFO
```

### Comparing `sqlmodel_repository-1.0.1/README.md` & `sqlmodel_repository-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sqlmodel_repository-1.0.1/pyproject.toml` & `sqlmodel_repository-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 [tool.poetry]
 authors = ["Jonas Scholl <jonas@code-specialist.com>", "Yannic Schröer <yannic@code-specialist.com>"]
 description = "Repository pattern implementation for SQLModel (SQLAlchemy)"
 license = "MIT"
 name = "sqlmodel-repository"
 readme = "README.md"
-version = "1.0.1"
+version = "1.0.2"
 
 [tool.poetry.dependencies]
-database-setup-tools = "1.3.0"
 python = "^3.9"
 sqlmodel = "^0.0.8"
 
 [tool.poetry.dev-dependencies]
 psycopg2-binary = "^2.9.5"
 pylint = "^2.15.8"
 pylint-quotes = "^0.2.3"
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
+database-setup-tools = "^1.3.1"
 
 [tool.pytest.ini_options]
 addopts = "-x -p no:warnings -v --cov-report=term-missing --cov-report=term --no-cov-on-fail --cov=sqlmodel_repository"
 
 [tool.black]
 line-length = 200
 target-version = ["py39", "py310", "py311"]
```

### Comparing `sqlmodel_repository-1.0.1/sqlmodel_repository/base_repository.py` & `sqlmodel_repository-1.0.2/sqlmodel_repository/base_repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from abc import ABC, abstractmethod
-
 from functools import lru_cache
 from typing import Generic, Type, TypeVar, get_args
 
 from sqlalchemy.orm import Session
 
 from sqlmodel_repository.entity import SQLModelEntity
 from sqlmodel_repository.exceptions import CouldNotCreateEntityException, CouldNotDeleteEntityException, EntityDoesNotPossessAttributeException, EntityNotFoundException
```

### Comparing `sqlmodel_repository-1.0.1/sqlmodel_repository/exceptions.py` & `sqlmodel_repository-1.0.2/sqlmodel_repository/exceptions.py`

 * *Files identical despite different names*

### Comparing `sqlmodel_repository-1.0.1/sqlmodel_repository/repository.py` & `sqlmodel_repository-1.0.2/sqlmodel_repository/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from abc import ABC
 from typing import List, TypeVar
 
-
 from sqlmodel import col
-from sqlmodel_repository.base_repository import BaseRepository
 
+from sqlmodel_repository.base_repository import BaseRepository
 from sqlmodel_repository.entity import SQLModelEntity
 from sqlmodel_repository.exceptions import EntityDoesNotPossessAttributeException
 
 GenericEntity = TypeVar("GenericEntity", bound=SQLModelEntity)
 
 
 class Repository(BaseRepository[GenericEntity], ABC):
```

### Comparing `sqlmodel_repository-1.0.1/PKG-INFO` & `sqlmodel_repository-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: sqlmodel-repository
-Version: 1.0.1
+Version: 1.0.2
 Summary: Repository pattern implementation for SQLModel (SQLAlchemy)
 License: MIT
 Author: Jonas Scholl
 Author-email: jonas@code-specialist.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: database-setup-tools (==1.3.0)
 Requires-Dist: sqlmodel (>=0.0.8,<0.0.9)
 Description-Content-Type: text/markdown
 
 # SQLModel Repository - Python Repository Pattern Implementation for SQLModel
 
 [![CodeQL](https://github.com/code-specialist/python-repository/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/code-specialist/python-repository/actions/workflows/github-code-scanning/codeql) [![Tests](https://github.com/code-specialist/python-repository/actions/workflows/test.yaml/badge.svg)](https://github.com/code-specialist/python-repository/actions/workflows/test.yaml)
```

