# Comparing `tmp/aiofauna-0.0.5.tar.gz` & `tmp/aiofauna-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiofauna-0.0.5.tar", max compression
+gzip compressed data, was "aiofauna-0.0.6.tar", max compression
```

## Comparing `aiofauna-0.0.5.tar` & `aiofauna-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1062 2023-04-04 09:22:52.727508 aiofauna-0.0.5/aiofauna/__init__.py
--rw-r--r--   0        0        0     7640 2023-04-04 08:57:41.715281 aiofauna-0.0.5/aiofauna/application.py
--rw-r--r--   0        0        0     4881 2023-04-04 06:35:42.759624 aiofauna-0.0.5/aiofauna/client.py
--rw-r--r--   0        0        0      493 2023-04-04 07:02:54.142000 aiofauna-0.0.5/aiofauna/deprecated.py
--rw-r--r--   0        0        0     8215 2023-04-04 07:02:53.605804 aiofauna-0.0.5/aiofauna/errors.py
--rw-r--r--   0        0        0     1598 2023-04-04 08:59:31.698896 aiofauna-0.0.5/aiofauna/helpers.py
--rw-r--r--   0        0        0     5537 2023-04-04 08:01:04.804127 aiofauna-0.0.5/aiofauna/json.py
--rw-r--r--   0        0        0     5617 2023-04-02 02:01:28.305641 aiofauna-0.0.5/aiofauna/objects.py
--rw-r--r--   0        0        0    15335 2023-04-04 07:02:51.919994 aiofauna-0.0.5/aiofauna/odm.py
--rw-r--r--   0        0        0     2624 2023-04-04 08:57:42.050368 aiofauna-0.0.5/aiofauna/page.py
--rw-r--r--   0        0        0    41509 2023-04-02 02:01:30.987614 aiofauna-0.0.5/aiofauna/query.py
--rw-r--r--   0        0        0     1132 2023-04-04 08:55:57.371956 aiofauna-0.0.5/LICENSE
--rw-r--r--   0        0        0      589 2023-04-04 09:22:50.912134 aiofauna-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      804 2023-04-04 09:23:22.165978 aiofauna-0.0.5/setup.py
--rw-r--r--   0        0        0      708 2023-04-04 09:23:22.165978 aiofauna-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-09 15:51:15.849095 aiofauna-0.0.6/aiofauna/__init__.py
+-rw-r--r--   0        0        0     7816 2023-04-09 15:50:09.852936 aiofauna-0.0.6/aiofauna/application.py
+-rw-r--r--   0        0        0     4881 2023-04-09 00:48:46.949196 aiofauna-0.0.6/aiofauna/client.py
+-rw-r--r--   0        0        0      493 2023-04-04 07:02:54.142000 aiofauna-0.0.6/aiofauna/deprecated.py
+-rw-r--r--   0        0        0     8215 2023-04-09 15:50:12.700726 aiofauna-0.0.6/aiofauna/errors.py
+-rw-r--r--   0        0        0     2408 2023-04-09 02:06:01.350775 aiofauna-0.0.6/aiofauna/helpers.py
+-rw-r--r--   0        0        0     6724 2023-04-09 00:48:44.968530 aiofauna-0.0.6/aiofauna/json.py
+-rw-r--r--   0        0        0     1303 2023-04-09 01:04:59.396687 aiofauna-0.0.6/aiofauna/meta.py
+-rw-r--r--   0        0        0     5777 2023-04-09 14:32:34.125477 aiofauna-0.0.6/aiofauna/objects.py
+-rw-r--r--   0        0        0    15335 2023-04-04 07:02:51.919994 aiofauna-0.0.6/aiofauna/odm.py
+-rw-r--r--   0        0        0     2624 2023-04-04 08:57:42.050368 aiofauna-0.0.6/aiofauna/page.py
+-rw-r--r--   0        0        0    41509 2023-04-02 02:01:30.987614 aiofauna-0.0.6/aiofauna/query.py
+-rw-r--r--   0        0        0     1132 2023-04-04 08:55:57.371956 aiofauna-0.0.6/LICENSE
+-rw-r--r--   0        0        0      589 2023-04-09 15:50:57.314237 aiofauna-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      804 2023-04-09 15:51:34.315973 aiofauna-0.0.6/setup.py
+-rw-r--r--   0        0        0      708 2023-04-09 15:51:34.315973 aiofauna-0.0.6/PKG-INFO
```

### Comparing `aiofauna-0.0.5/aiofauna/__init__.py` & `aiofauna-0.0.6/aiofauna/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 README.md
 """
 
-__version__ = "0.0.5"
-__author__ = "aiolibs"
+__version__ = "0.0.6"
+__author__ = "obahamonde"
 __license__ = "MIT"
 
 import asyncio
 from time import perf_counter
 from datetime import datetime, date, time, timedelta
 from typing import Any, AsyncGenerator, Callable, Dict, List, Optional, Union
 from uuid import UUID, uuid4
```

### Comparing `aiofauna-0.0.5/aiofauna/application.py` & `aiofauna-0.0.6/aiofauna/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,18 @@
     Application,
     AppRunner,
     TCPSite,
     Request,
     Response,
     json_response
 )
+from aiohttp import ClientSession
 from typing import Callable, Coroutine
 from functools import wraps
-
+from aiofauna.meta import parse_to_response
 
 class App(Application):
     """
     
     This module defines the App class, which is a subclass of the aiohttp.web.Application class.
     The App class provides a simple way to create web applications with Jinja2 templates.
 
@@ -64,18 +65,16 @@
             Callable: The decorator function.
         """
 
         def decorator(func):
             @wraps(func)
             def wrapper(*args, **kwargs):
                 return func(*args, **kwargs)
-
-            self.add_route(method, path, wrapper, **kwargs)
+            self.router.add_route(method, path, wrapper, **kwargs)
             return wrapper
-
         return decorator
 
     def get(self, path: str, **kwargs):
 
         """
         
         Decorator to define a GET route and its corresponding handler function.
@@ -235,15 +234,15 @@
         
             Callable: The decorator function.
             
         """
 
         return self.route("TRACE", path, **kwargs)
 
-    def add_route(self, method: str, path: str, func: Callable, **kwargs):
+    def add(self, method: str, path: str, func: Callable, **kwargs):
 
         """
         
         Add a route and its corresponding handler function.
         
         Args:
             method (str): The HTTP method for the route (e.g., "GET", "POST").
@@ -252,29 +251,33 @@
             **kwargs: Additional keyword arguments for the route.
             
         """
 
         self.router.add_route(method, path, func, **kwargs)
         return self
 
-    async def listen(self, host: str = "0.0.0.0", port: int = 8080, **kwargs):
+    async def listen(self, host:bool=False, port: int = 8000, **kwargs):
 
         """
         
         Starts Listening for requests.
         
         Args:
         
             host (str): The host to listen on.
             
             port (int): The port to listen on.
             
             **kwargs: Additional keyword arguments for the server.
             
         """
-
+        if not host:
+            _host = "localhost"
+        _host = "0.0.0.0"
         runner = AppRunner(self, **kwargs)
         await runner.setup()
-        site = TCPSite(runner, host, port)
+        site = TCPSite(runner, _host, port)
         await site.start()
         while True:
             await asyncio.sleep(1)
+            
+
```

### Comparing `aiofauna-0.0.5/aiofauna/client.py` & `aiofauna-0.0.6/aiofauna/client.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.5/aiofauna/errors.py` & `aiofauna-0.0.6/aiofauna/errors.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.5/aiofauna/objects.py` & `aiofauna-0.0.6/aiofauna/objects.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 """
 Types used in queries and responses.
 See the `docs <https://app.fauna.com/documentation/reference/queryapi#simple-type>`__.
 """
 from datetime import datetime
-
-# pylint: disable=redefined-builtin
 from iso8601 import parse_date
 from aiofauna.deprecated import deprecated
 from aiofauna.query import Expr
 
-
 class Ref(Expr):
     """
-  FaunaDB ref. See the `docs <https://app.fauna.com/documentation/reference/queryapi#special-type>`__.
-
-  A simple wrapper around a string which can be extracted using ``ref.value``.
-  Queries that require a Ref will not work if you just pass in a string.
-  """
+    ```python
+    Ref(id, cls=None, db=None)
+    ```
+    A reference to a document in a collection or index.
+    
+    :param id: The document's ID.
+    :param cls: The collection or index class.
+    :param db: The database.
+
+    `Ref` 
+    
+    Is a special type in FaunaDB. It is used to represent a document in a collection or index.
+    
+    It is serialized to JSON as an object with the `@ref` key. Passing the `id` to the response. 
+    
+    """
 
     def __init__(self, id, cls=None, db=None):
         if id is None:
             raise ValueError("The Ref must have an id.")
 
         value = {"id": id}
```

### Comparing `aiofauna-0.0.5/aiofauna/odm.py` & `aiofauna-0.0.6/aiofauna/odm.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.5/aiofauna/page.py` & `aiofauna-0.0.6/aiofauna/page.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.5/aiofauna/query.py` & `aiofauna-0.0.6/aiofauna/query.py`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.5/LICENSE` & `aiofauna-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiofauna-0.0.5/pyproject.toml` & `aiofauna-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiofauna"
-version = "0.0.5"
+version = "0.0.6"
 description = "A developer friendly yet versatile asynchronous Object-Document Mapper for FaunaDB"
 authors = ["Oscar Bahamonde <oscar.bahamonde.dev@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pydantic = {extras = ["dotenv","email"], version = "^1.10.7"}
 aiohttp = "^3.8.4"
```

### Comparing `aiofauna-0.0.5/setup.py` & `aiofauna-0.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 {'': ['*']}
 
 install_requires = \
 ['Jinja2>=3.1.2,<4.0.0',
  'aiohttp-sse>=2.1.0,<3.0.0',
  'aiohttp>=3.8.4,<4.0.0',
  'iso8601>=1.1.0,<2.0.0',
- 'pydantic[dotenv,email]>=1.10.7,<2.0.0']
+ 'pydantic[email,dotenv]>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'aiofauna',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': 'A developer friendly yet versatile asynchronous Object-Document Mapper for FaunaDB',
     'long_description': None,
     'author': 'Oscar Bahamonde',
     'author_email': 'oscar.bahamonde.dev@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `aiofauna-0.0.5/PKG-INFO` & `aiofauna-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: aiofauna
-Version: 0.0.5
+Version: 0.0.6
 Summary: A developer friendly yet versatile asynchronous Object-Document Mapper for FaunaDB
 Author: Oscar Bahamonde
 Author-email: oscar.bahamonde.dev@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: aiohttp-sse (>=2.1.0,<3.0.0)
 Requires-Dist: iso8601 (>=1.1.0,<2.0.0)
-Requires-Dist: pydantic[dotenv,email] (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic[email,dotenv] (>=1.10.7,<2.0.0)
```

