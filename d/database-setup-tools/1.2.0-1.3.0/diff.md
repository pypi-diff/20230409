# Comparing `tmp/database_setup_tools-1.2.0.tar.gz` & `tmp/database_setup_tools-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_setup_tools-1.2.0.tar", max compression
+gzip compressed data, was "database_setup_tools-1.3.0.tar", max compression
```

## Comparing `database_setup_tools-1.2.0.tar` & `database_setup_tools-1.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-04-04 06:49:31.063943 database_setup_tools-1.2.0/LICENSE
--rw-r--r--   0        0        0     2579 2023-04-04 06:49:31.063943 database_setup_tools-1.2.0/README.md
--rw-r--r--   0        0        0       20 2023-04-04 06:49:43.920120 database_setup_tools-1.2.0/database_setup_tools/__init__.py
--rw-r--r--   0        0        0     2601 2023-04-04 06:49:31.063943 database_setup_tools-1.2.0/database_setup_tools/session_manager.py
--rw-r--r--   0        0        0     3809 2023-04-04 06:49:31.063943 database_setup_tools-1.2.0/database_setup_tools/setup.py
--rw-r--r--   0        0        0      953 2023-04-04 06:49:43.924120 database_setup_tools-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3215 1970-01-01 00:00:00.000000 database_setup_tools-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-09 10:35:41.748398 database_setup_tools-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2579 2023-04-09 10:35:41.748398 database_setup_tools-1.3.0/README.md
+-rw-r--r--   0        0        0       20 2023-04-09 10:35:52.520576 database_setup_tools-1.3.0/database_setup_tools/__init__.py
+-rw-r--r--   0        0        0     2646 2023-04-09 10:35:41.748398 database_setup_tools-1.3.0/database_setup_tools/session_manager.py
+-rw-r--r--   0        0        0     4067 2023-04-09 10:35:41.748398 database_setup_tools-1.3.0/database_setup_tools/setup.py
+-rw-r--r--   0        0        0      955 2023-04-09 10:35:52.520576 database_setup_tools-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3215 1970-01-01 00:00:00.000000 database_setup_tools-1.3.0/PKG-INFO
```

### Comparing `database_setup_tools-1.2.0/LICENSE` & `database_setup_tools-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `database_setup_tools-1.2.0/README.md` & `database_setup_tools-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `database_setup_tools-1.2.0/database_setup_tools/session_manager.py` & `database_setup_tools-1.3.0/database_setup_tools/session_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import threading
 from functools import cached_property
-from typing import Generator, Optional
+from typing import Any, Generator, Optional
 
 from sqlalchemy import create_engine
 from sqlalchemy.engine import Engine
 from sqlalchemy.orm import Session, sessionmaker
 from sqlalchemy.orm.scoping import scoped_session
 
 
@@ -17,33 +17,33 @@
     def __new__(cls, *args, **kwargs):
         if not cls._get_cached_instance(args, kwargs):
             with cls._lock:
                 if not cls._get_cached_instance(args, kwargs):
                     cls._instances.append((super(cls, cls).__new__(cls), (args, kwargs)))
         return cls._get_cached_instance(args, kwargs)
 
-    def __init__(self, database_uri: str, **kwargs):
+    def __init__(self, database_uri: str, **engine_options: dict[str, Any]):
         """Session Manager constructor
 
         Args:
             database_uri (str): The URI of the database to manage sessions for
 
         Keyword Args:
-            **kwargs: Keyword arguments to pass to the engine
+            **engine_options: Keyword arguments to pass to the engine
 
             postgresql:
                 pool_size (int): The maximum number of connections to the database
                 max_overflow (int): The maximum number of connections to the database
                 pre_ping (bool): Whether to ping the database before each connection, may fix connection issues
         """
         if not isinstance(database_uri, str):
             raise TypeError("database_uri must be a string")
 
         self._database_uri = database_uri
-        self._engine = self._get_engine(**kwargs)
+        self._engine = self._get_engine(**engine_options)
         self._session_factory = sessionmaker(self.engine)
         self._Session = scoped_session(self._session_factory)
 
     @cached_property
     def database_uri(self) -> str:
         """Getter for the database URI"""
         return self._database_uri
```

### Comparing `database_setup_tools-1.2.0/database_setup_tools/setup.py` & `database_setup_tools-1.3.0/database_setup_tools/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import threading
-from typing import List, Optional
+from typing import Any, List, Optional, Union
 
 import sqlalchemy_utils
 from sqlalchemy import MetaData, Table
-from sqlmodel import SQLModel
+from sqlmodel.main import SQLModel, SQLModelMetaclass
 
 from database_setup_tools.session_manager import SessionManager
 
 
 class DatabaseSetup:
     """Create the database and the tables if not done yet"""
 
@@ -17,30 +17,33 @@
     def __new__(cls, *args, **kwargs):
         if not cls._get_cached_instance(args, kwargs):
             with cls._lock:
                 if not cls._get_cached_instance(args, kwargs):
                     cls._instances.append((super(cls, cls).__new__(cls), (args, kwargs)))
         return cls._get_cached_instance(args, kwargs)
 
-    def __init__(self, model_metadata: MetaData, database_uri: str):
+    def __init__(self, model_metadata: MetaData, database_uri: str, **engine_options: dict[str, Any]):
         """Set up a database based on its URI and metadata. Will not overwrite existing data.
 
         Args:
             model_metadata (Metadata): The metadata of the models to create the tables for
             database_uri (str): The URI of the database to create the tables for
 
+        Keyword Args:
+            **engine_options: Keyword arguments to pass to the engine
         """
         if not isinstance(model_metadata, MetaData):
             raise TypeError("model_metadata must be a MetaData")
 
         if not isinstance(database_uri, str):
             raise TypeError("database_uri must be a string")
 
         self._model_metadata = model_metadata
         self._database_uri = database_uri
+        self._engine_options = engine_options
         self.create_database()
 
     @property
     def model_metadata(self) -> MetaData:
         """Getter for the model metadata
 
         Returns:
@@ -51,15 +54,15 @@
     @property
     def session_manager(self) -> SessionManager:
         """Getter for the session manager
 
         Returns:
             SessionManager: The session manager
         """
-        return SessionManager(database_uri=self.database_uri)
+        return SessionManager(database_uri=self.database_uri, **self._engine_options)
 
     @property
     def database_uri(self) -> str:
         """Getter for the database URI
 
         Returns:
             str: The database URI
@@ -81,15 +84,15 @@
         """Create the database and the tables if not done yet"""
         if not sqlalchemy_utils.database_exists(self.database_uri):
             sqlalchemy_utils.create_database(self.database_uri)
             self.model_metadata.create_all(self.session_manager.engine)
             return True
         return False
 
-    def truncate(self, tables: Optional[List[SQLModel]] = None):
+    def truncate(self, tables: Optional[List[Union[SQLModel, SQLModelMetaclass]]] = None):
         """Truncate all tables in the database"""
         tables_to_truncate: List[Table] = self.model_metadata.sorted_tables
         if tables is not None:
             table_names = [table.__tablename__ for table in tables]
             tables_to_truncate = filter(lambda table: table.name in table_names, tables_to_truncate)
 
         session = next(self.session_manager.get_session())
```

### Comparing `database_setup_tools-1.2.0/pyproject.toml` & `database_setup_tools-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "database-setup-tools"
-version = "1.2.0"
+version = "1.3.0"
 description = "Tools to easily setup databases opinionated towards FastAPI and SQLModel"
 authors = ["Jonas Scholl <jonas@code-specialist.com>", "Yannic Schröer <yannic@code-specialist.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "database_setup_tools" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 sqlalchemy = "^1.4.41"
 sqlalchemy-utils = ">=0.38.3,<0.41.0"
 
 [tool.poetry.dev-dependencies]
-black = "23.1.0"
-sqlmodel = "0.0.8"
+black = "23.3.0"
+sqlmodel = "^0.0.8"
 psycopg2-binary = "^2.9.5"
 pytest-cov = "^4.0.0"
 pytest = "7.2.0"
-httpx = "0.23.1"
+httpx = "^0.23.1"
 mockito = "^1.4.0"
 pytest-mockito = "^0.0.4"
 pre-commit = "^3.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `database_setup_tools-1.2.0/PKG-INFO` & `database_setup_tools-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-setup-tools
-Version: 1.2.0
+Version: 1.3.0
 Summary: Tools to easily setup databases opinionated towards FastAPI and SQLModel
 License: MIT
 Author: Jonas Scholl
 Author-email: jonas@code-specialist.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

