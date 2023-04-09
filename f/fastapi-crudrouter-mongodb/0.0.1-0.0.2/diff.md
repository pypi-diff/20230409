# Comparing `tmp/fastapi-crudrouter-mongodb-0.0.1.tar.gz` & `tmp/fastapi-crudrouter-mongodb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-crudrouter-mongodb-0.0.1.tar", last modified: Sun Apr  9 19:28:05 2023, max compression
+gzip compressed data, was "fastapi-crudrouter-mongodb-0.0.2.tar", last modified: Sun Apr  9 19:50:13 2023, max compression
```

## Comparing `fastapi-crudrouter-mongodb-0.0.1.tar` & `fastapi-crudrouter-mongodb-0.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 19:28:05.690905 fastapi-crudrouter-mongodb-0.0.1/
--rw-r--r--   0 pierro    (1000) pierro    (1000)     1070 2023-04-09 10:32:33.000000 fastapi-crudrouter-mongodb-0.0.1/LICENSE
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     4296 2023-04-09 19:28:05.690905 fastapi-crudrouter-mongodb-0.0.1/PKG-INFO
--rw-r--r--   0 pierro    (1000) pierro    (1000)     2934 2023-04-09 12:10:04.000000 fastapi-crudrouter-mongodb-0.0.1/README.md
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 19:28:05.690905 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)      278 2023-04-09 19:27:52.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/__init__.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 19:28:05.690905 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)      177 2023-04-09 11:15:45.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/__init__.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 19:28:05.690905 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/models/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)      134 2023-04-09 10:58:04.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/models/CRUDEmbed.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)      384 2023-04-09 10:54:52.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/models/CRUDLookup.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)      191 2023-04-09 11:09:33.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/models/__init__.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     1145 2023-04-09 10:50:18.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/models/mongo_model.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)      400 2023-04-09 10:50:03.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/models/mongo_object_id_model.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 19:28:05.690905 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     6252 2023-04-09 11:26:20.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/CRUDRouter.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     1464 2023-04-09 10:51:15.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/CRUDRouterFactory.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     1960 2023-04-09 10:51:15.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/CRUDRouterRepository.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)      220 2023-04-09 11:17:14.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/__init__.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 19:28:05.690905 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/embed/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     5101 2023-04-09 11:00:10.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouter.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     1433 2023-04-09 10:59:36.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterFactory.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     3148 2023-04-09 10:58:18.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterRepository.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)       82 2023-04-09 11:18:46.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/embed/__init__.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 19:28:05.690905 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/lookup/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     6480 2023-04-09 10:57:21.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouter.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     1439 2023-04-09 10:53:17.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterFactory.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     3730 2023-04-09 10:57:30.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterRepository.py
--rw-rw-r--   0 pierro    (1000) pierro    (1000)       86 2023-04-09 11:18:20.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/lookup/__init__.py
-drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 19:28:05.690905 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb.egg-info/
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     4296 2023-04-09 19:28:05.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb.egg-info/PKG-INFO
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     1398 2023-04-09 19:28:05.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb.egg-info/SOURCES.txt
--rw-rw-r--   0 pierro    (1000) pierro    (1000)        1 2023-04-09 19:28:05.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb.egg-info/dependency_links.txt
--rw-rw-r--   0 pierro    (1000) pierro    (1000)       28 2023-04-09 19:28:05.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb.egg-info/requires.txt
--rw-rw-r--   0 pierro    (1000) pierro    (1000)       27 2023-04-09 19:28:05.000000 fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb.egg-info/top_level.txt
--rw-rw-r--   0 pierro    (1000) pierro    (1000)       38 2023-04-09 19:28:05.690905 fastapi-crudrouter-mongodb-0.0.1/setup.cfg
--rw-rw-r--   0 pierro    (1000) pierro    (1000)     1717 2023-04-09 19:27:56.000000 fastapi-crudrouter-mongodb-0.0.1/setup.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 19:50:13.487852 fastapi-crudrouter-mongodb-0.0.2/
+-rw-r--r--   0 pierro    (1000) pierro    (1000)     1070 2023-04-09 10:32:33.000000 fastapi-crudrouter-mongodb-0.0.2/LICENSE
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     4394 2023-04-09 19:50:13.487852 fastapi-crudrouter-mongodb-0.0.2/PKG-INFO
+-rw-r--r--   0 pierro    (1000) pierro    (1000)     3032 2023-04-09 19:48:39.000000 fastapi-crudrouter-mongodb-0.0.2/README.md
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 19:50:13.483852 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)      278 2023-04-09 19:49:45.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/__init__.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 19:50:13.483852 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)      177 2023-04-09 11:15:45.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/__init__.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 19:50:13.487852 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/models/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)      134 2023-04-09 10:58:04.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/models/CRUDEmbed.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)      384 2023-04-09 10:54:52.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/models/CRUDLookup.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)      191 2023-04-09 11:09:33.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/models/__init__.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     1145 2023-04-09 10:50:18.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/models/mongo_model.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)      400 2023-04-09 10:50:03.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/models/mongo_object_id_model.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 19:50:13.487852 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     6253 2023-04-09 19:39:43.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/CRUDRouter.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     1464 2023-04-09 10:51:15.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/CRUDRouterFactory.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     1963 2023-04-09 19:40:02.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/CRUDRouterRepository.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)      220 2023-04-09 11:17:14.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/__init__.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 19:50:13.487852 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/embed/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     5101 2023-04-09 11:00:10.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouter.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     1433 2023-04-09 10:59:36.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterFactory.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     3148 2023-04-09 10:58:18.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterRepository.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)       82 2023-04-09 11:18:46.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/embed/__init__.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 19:50:13.487852 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/lookup/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     6480 2023-04-09 10:57:21.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouter.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     1432 2023-04-09 19:40:37.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterFactory.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     3730 2023-04-09 10:57:30.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterRepository.py
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)       86 2023-04-09 11:18:20.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/lookup/__init__.py
+drwxrwxr-x   0 pierro    (1000) pierro    (1000)        0 2023-04-09 19:50:13.483852 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb.egg-info/
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     4394 2023-04-09 19:50:13.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb.egg-info/PKG-INFO
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     1398 2023-04-09 19:50:13.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb.egg-info/SOURCES.txt
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)        1 2023-04-09 19:50:13.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb.egg-info/dependency_links.txt
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)       31 2023-04-09 19:50:13.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb.egg-info/requires.txt
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)       27 2023-04-09 19:50:13.000000 fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb.egg-info/top_level.txt
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)       38 2023-04-09 19:50:13.487852 fastapi-crudrouter-mongodb-0.0.2/setup.cfg
+-rw-rw-r--   0 pierro    (1000) pierro    (1000)     1720 2023-04-09 19:49:50.000000 fastapi-crudrouter-mongodb-0.0.2/setup.py
```

### Comparing `fastapi-crudrouter-mongodb-0.0.1/LICENSE` & `fastapi-crudrouter-mongodb-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.1/PKG-INFO` & `fastapi-crudrouter-mongodb-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-crudrouter-mongodb
-Version: 0.0.1
+Version: 0.0.2
 Summary: A dynamic FastAPI router that automatically creates CRUD routes for your mongodb models
 Home-page: https://github.com/pierrod/fastapi-crudrouter-mongodb
 Author: Pierre DUVEAU
 Author-email: 
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Internet
@@ -58,18 +58,22 @@
 ```
 
 ## Basic Usage
 
 I will provide more examples in the future, but for now, here is a basic example of how to use the FastAPI CRUDRouter for Mongodb.
 
 ```python
+from datetime import datetime
+from typing import List, Optional, Union
 from fastapi import FastAPI
-from fastapi_crudrouter_mongodb import CRUDRouter, CRUDLookup, MongoModel, MongoObjectId
+from pydantic import Field
+from fastapi_crudrouter_mongodb import CRUDRouter, MongoModel, MongoObjectId, CRUDLookup
 import motor.motor_asyncio
 
+
 # Database connection using motor 
 client = motor.motor_asyncio.AsyncIOMotorClient(
     "mongodb://localhost:27017/local")
 
 db = client.local
 
 # Models
@@ -113,15 +117,14 @@
     prefix="/users",
     tags=["users"],
 )
 
 # Instantiating the FastAPI app
 app = FastAPI()
 app.include_router(users_controller)
-
 ```
 
 ## OpenAPI Support
 
 By default, all routes generated by the CRUDRouter will be documented according to OpenAPI spec.
 
 Below are the default routes created by the CRUDRouter shown in the generated OpenAPI documentation.
```

### Comparing `fastapi-crudrouter-mongodb-0.0.1/README.md` & `fastapi-crudrouter-mongodb-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,18 +28,22 @@
 ```
 
 ## Basic Usage
 
 I will provide more examples in the future, but for now, here is a basic example of how to use the FastAPI CRUDRouter for Mongodb.
 
 ```python
+from datetime import datetime
+from typing import List, Optional, Union
 from fastapi import FastAPI
-from fastapi_crudrouter_mongodb import CRUDRouter, CRUDLookup, MongoModel, MongoObjectId
+from pydantic import Field
+from fastapi_crudrouter_mongodb import CRUDRouter, MongoModel, MongoObjectId, CRUDLookup
 import motor.motor_asyncio
 
+
 # Database connection using motor 
 client = motor.motor_asyncio.AsyncIOMotorClient(
     "mongodb://localhost:27017/local")
 
 db = client.local
 
 # Models
@@ -83,15 +87,14 @@
     prefix="/users",
     tags=["users"],
 )
 
 # Instantiating the FastAPI app
 app = FastAPI()
 app.include_router(users_controller)
-
 ```
 
 ## OpenAPI Support
 
 By default, all routes generated by the CRUDRouter will be documented according to OpenAPI spec.
 
 Below are the default routes created by the CRUDRouter shown in the generated OpenAPI documentation.
```

### Comparing `fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/models/mongo_model.py` & `fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/models/mongo_model.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/CRUDRouter.py` & `fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/CRUDRouter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Callable, List
 
 from fastapi import HTTPException
-from CRUDRouterFactory import CRUDRouterFactory
+from .CRUDRouterFactory import CRUDRouterFactory
 from . import CRUDRouterRepository
 from .embed.CRUDEmbedRouter import CRUDEmbedRouter
 from .lookup.CRUDLookupRouter import CRUDLookupRouter
 from ..models.CRUDEmbed import CRUDEmbed
 from ..models.CRUDLookup import CRUDLookup
 from ..models.mongo_model import MongoModel
```

### Comparing `fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/CRUDRouterFactory.py` & `fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/CRUDRouterFactory.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/CRUDRouterRepository.py` & `fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/CRUDRouterRepository.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from bson import ObjectId
-from utils.mongo_model import MongoModel
+from ..models.mongo_model import MongoModel
 
 
 async def get_all(db, model: MongoModel, collection_name) -> list:
     """
     Get all documents from the database
     """
     documents = []
```

### Comparing `fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouter.py` & `fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouter.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterFactory.py` & `fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterFactory.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterRepository.py` & `fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/embed/CRUDEmbedRouterRepository.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouter.py` & `fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouter.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterFactory.py` & `fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterFactory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Callable
 from fastapi import APIRouter
 
-from utils.CRUDRouterFactory import CRUDRouterFactory
-from utils.lookup.CRUDLookup import CRUDLookup
+from ..CRUDRouterFactory import CRUDRouterFactory
+from ...models.CRUDLookup import CRUDLookup
 
 class CRUDLookupRouterFactory(APIRouter):
 
     def __init__(self, parent_router: CRUDRouterFactory, child_args: CRUDLookup, *args, **kwargs):
         self.parent_router = parent_router
         self.child_args = child_args
```

### Comparing `fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterRepository.py` & `fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb/core/router/lookup/CRUDLookupRouterRepository.py`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb.egg-info/PKG-INFO` & `fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-crudrouter-mongodb
-Version: 0.0.1
+Version: 0.0.2
 Summary: A dynamic FastAPI router that automatically creates CRUD routes for your mongodb models
 Home-page: https://github.com/pierrod/fastapi-crudrouter-mongodb
 Author: Pierre DUVEAU
 Author-email: 
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Internet
@@ -58,18 +58,22 @@
 ```
 
 ## Basic Usage
 
 I will provide more examples in the future, but for now, here is a basic example of how to use the FastAPI CRUDRouter for Mongodb.
 
 ```python
+from datetime import datetime
+from typing import List, Optional, Union
 from fastapi import FastAPI
-from fastapi_crudrouter_mongodb import CRUDRouter, CRUDLookup, MongoModel, MongoObjectId
+from pydantic import Field
+from fastapi_crudrouter_mongodb import CRUDRouter, MongoModel, MongoObjectId, CRUDLookup
 import motor.motor_asyncio
 
+
 # Database connection using motor 
 client = motor.motor_asyncio.AsyncIOMotorClient(
     "mongodb://localhost:27017/local")
 
 db = client.local
 
 # Models
@@ -113,15 +117,14 @@
     prefix="/users",
     tags=["users"],
 )
 
 # Instantiating the FastAPI app
 app = FastAPI()
 app.include_router(users_controller)
-
 ```
 
 ## OpenAPI Support
 
 By default, all routes generated by the CRUDRouter will be documented according to OpenAPI spec.
 
 Below are the default routes created by the CRUDRouter shown in the generated OpenAPI documentation.
```

### Comparing `fastapi-crudrouter-mongodb-0.0.1/fastapi_crudrouter_mongodb.egg-info/SOURCES.txt` & `fastapi-crudrouter-mongodb-0.0.2/fastapi_crudrouter_mongodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi-crudrouter-mongodb-0.0.1/setup.py` & `fastapi-crudrouter-mongodb-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="fastapi-crudrouter-mongodb",
-    version="0.0.1",
+    version="0.0.2",
     author="Pierre DUVEAU",
     author_email="",
     description="A dynamic FastAPI router that automatically creates CRUD routes for your mongodb models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pierrod/fastapi-crudrouter-mongodb",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "fastapi",
         "pydantic",
-        "bson",
+        "pymongo",
         "motor"
     ],
     classifiers=[
         "Operating System :: OS Independent",
         "Development Status :: 3 - Alpha",
         "Topic :: Internet",
         "Topic :: Internet :: WWW/HTTP",
```

