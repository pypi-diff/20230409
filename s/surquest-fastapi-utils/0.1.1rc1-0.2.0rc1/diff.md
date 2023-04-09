# Comparing `tmp/surquest_fastapi_utils-0.1.1rc1.tar.gz` & `tmp/surquest_fastapi_utils-0.2.0rc1.tar.gz`

## Comparing `surquest_fastapi_utils-0.1.1rc1.tar` & `surquest_fastapi_utils-0.2.0rc1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/package.base.dockerfile
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/.github/workflows/release.yml
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/.github/workflows/test.yml
--rw-r--r--   0        0        0    43478 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/assets/img/logs.png
--rw-r--r--   0        0        0    66316 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/assets/img/trace.png
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/schemas/responses/__init__.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/schemas/responses/base.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/schemas/responses/info.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/schemas/responses/message.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/schemas/responses/metadata.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/schemas/responses/responses.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/schemas/responses/status.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/utils/__init__.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/utils/args.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/utils/route.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/utils/GCP/GCP.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/utils/GCP/__init__.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/utils/GCP/catcher.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/utils/GCP/formatter.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/utils/GCP/http_context.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/utils/GCP/logging.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/utils/GCP/middleware.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/utils/GCP/tracer.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/test/pytest.ini
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/test/utils/test_catcher.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/LICENSE
--rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/README.md
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/pyproject.toml
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.1.1rc1/PKG-INFO
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/package.base.dockerfile
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/.github/workflows/test.yml
+-rw-r--r--   0        0        0    43478 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/assets/img/logs.png
+-rw-r--r--   0        0        0    66316 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/assets/img/trace.png
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/schemas/responses/__init__.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/schemas/responses/base.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/schemas/responses/info.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/schemas/responses/message.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/schemas/responses/metadata.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/schemas/responses/responses.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/schemas/responses/status.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/__init__.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/args.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/route.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/GCP.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/__init__.py
+-rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/catcher.py
+-rw-r--r--   0        0        0     6329 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/formatter.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/http_context.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/logging.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/middleware.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/tracer.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/test/pytest.ini
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/test/utils/test_catcher.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/LICENSE
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/README.md
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     5245 2020-02-02 00:00:00.000000 surquest_fastapi_utils-0.2.0rc1/PKG-INFO
```

### Comparing `surquest_fastapi_utils-0.1.1rc1/package.base.dockerfile` & `surquest_fastapi_utils-0.2.0rc1/package.base.dockerfile`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.1.1rc1/.github/workflows/release.yml` & `surquest_fastapi_utils-0.2.0rc1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.1.1rc1/.github/workflows/test.yml` & `surquest_fastapi_utils-0.2.0rc1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.1.1rc1/assets/img/logs.png` & `surquest_fastapi_utils-0.2.0rc1/assets/img/logs.png`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.1.1rc1/assets/img/trace.png` & `surquest_fastapi_utils-0.2.0rc1/assets/img/trace.png`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/schemas/responses/metadata.py` & `surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/schemas/responses/metadata.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/schemas/responses/responses.py` & `surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/schemas/responses/responses.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/utils/args.py` & `surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/args.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/utils/route.py` & `surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/route.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/utils/GCP/catcher.py` & `surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/catcher.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # import external modules
 import os
 from fastapi import Request
 from fastapi.exceptions import RequestValidationError
 from starlette.exceptions import HTTPException as StarletteHTTPException
-from traceback import format_exc
+import traceback
 
 from surquest.fastapi.schemas.responses import Response, Message
 
 from .logging import Logger
 from .http_context import (
     HTTP_REQUEST_CONTEXT,
     CLOUD_TRACE_CONTEXT
@@ -29,49 +29,53 @@
 
 
 class Catcher:
 
     OUPS = "Oups, something went wrong"
 
     @classmethod
-    def catch_internal_error(
+    async def catch_internal_error(
             cls,
             request: Request,
             exc: BaseException
     ):
 
-        ctx = {"trace": CLOUD_TRACE_CONTEXT.get()}
+        tb = traceback.format_exc(chain=False).split("\n")
 
-        # if run in production return only the error message + trace
-        if os.getenv('ENVIRONMENT', 'dev').lower() not in ['prod', 'production']:
+        ctx = {
+            "trace": CLOUD_TRACE_CONTEXT.get()
+        }
 
-            # if is not production return the full traceback
-            ctx["traceback"] =  str(format_exc()).split("\n")
+        if os.getenv("ENV", "DEV").upper() not in ["PROD", "PRODUCTION"] or \
+            os.getenv("ENVIRONMENT", "DEV").upper() not in ["PROD", "PRODUCTION"]:
+
+            ctx["traceback"] = tb
 
         message = Message(
             msg=F"{str(exc)} ({type(exc).__name__})",
             type="SERVER.ERROR",
             ctx=ctx,
         )
 
         Logger.error(
             F"{str(exc)} ({type(exc).__name__})",
             extra={
                 "error": message.dict(exclude_none=True),
-                "request": HTTP_REQUEST_CONTEXT.get()
+                "request": HTTP_REQUEST_CONTEXT.get(),
+                "traceback": tb
             }
         )
 
         return Response.set(
             status_code=500,
             errors=[message]
         )
 
     @classmethod
-    def catch_validation_error(
+    async def catch_validation_error(
             cls,
             request: Request,
             exc: RequestValidationError
     ):
         errors = []
 
         for error in exc.errors():
@@ -94,15 +98,15 @@
 
         return Response.set(
             status_code=422,
             errors=errors
         )
 
     @classmethod
-    def catch_http_exception(
+    async def catch_http_exception(
             cls,
             request: Request,
             exc: StarletteHTTPException
     ):
 
         message = Message(
             msg=getattr(exc, "detail", f"Not Found: ({request.url})"),
```

### Comparing `surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/utils/GCP/http_context.py` & `surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/http_context.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/utils/GCP/logging.py` & `surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/logging.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/utils/GCP/middleware.py` & `surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/middleware.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         try:
 
             response = await call_next(request)
             return response
 
         except BaseException as exc:
 
-            return Catcher.catch_internal_error(request, exc)
+            return await Catcher.catch_internal_error(request, exc)
 
 class LoggingMiddleware(BaseHTTPMiddleware):
 
     def __init__(self, app):
         super().__init__(app)
 
     @staticmethod
@@ -56,15 +56,15 @@
         try:
 
             response = await call_next(request)
             return response
 
         except BaseException as exc:
 
-            return Catcher.catch_internal_error(request, exc)
+            return await Catcher.catch_internal_error(request, exc)
 
 
 class DBMiddleware(BaseHTTPMiddleware):
 
     def __init__(self, app, db=None, ):
         super().__init__(app)
         self.db = db
@@ -81,12 +81,12 @@
             request.state.db_engine = self.db.get_engine()
 
             response = await call_next(request)
             return response
 
         except BaseException as exc:
 
-            return Catcher.catch_internal_error(request, exc)
+            return await Catcher.catch_internal_error(request, exc)
 
         finally:
 
             request.state.db_engine.dispose()
```

### Comparing `surquest_fastapi_utils-0.1.1rc1/surquest/fastapi/utils/GCP/tracer.py` & `surquest_fastapi_utils-0.2.0rc1/surquest/fastapi/utils/GCP/tracer.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.1.1rc1/test/utils/test_catcher.py` & `surquest_fastapi_utils-0.2.0rc1/test/utils/test_catcher.py`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.1.1rc1/.gitignore` & `surquest_fastapi_utils-0.2.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.1.1rc1/LICENSE` & `surquest_fastapi_utils-0.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `surquest_fastapi_utils-0.1.1rc1/README.md` & `surquest_fastapi_utils-0.2.0rc1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 # Introduction
 
 This project provides collection of utilities for smooth integration of FastAPI framework with Google Cloud Platform services as logging and tracing.
 
 The key features of this project are:
 
-* Logging to Stackdriver
-* Tracing to Stackdriver
+* Logging to Cloud Logging
+* Tracing to Cloud Logging
+* Error Reporting via Cloud Logging
 * Custom middleware for configuration of logging
 * Custom exception handlers treating HTTP and validation exceptions
 * Custom routes for documentation and favicon
 * Custom responses with statuses `success`, `warning` and `error` and standardized error messages
 
 # Quick Start
```

### Comparing `surquest_fastapi_utils-0.1.1rc1/pyproject.toml` & `surquest_fastapi_utils-0.2.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "surquest-fastapi-utils"
-version = "0.1.1rc1"
+version = "0.2.0rc1"
 description = "This project provides collection of utilities for FastAPI framework as: Catcher, Middleware, etc."
 authors = [
     {name= "Michal Švarc", email= "michal.svarc@surquest.com"}
 ]
 readme = "README.md"
 dependencies = [
     "fastapi >= 0.81.0",
```

### Comparing `surquest_fastapi_utils-0.1.1rc1/PKG-INFO` & `surquest_fastapi_utils-0.2.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surquest-fastapi-utils
-Version: 0.1.1rc1
+Version: 0.2.0rc1
 Summary: This project provides collection of utilities for FastAPI framework as: Catcher, Middleware, etc.
 Project-URL: Homepage, https://github.com/surquest/python-fastapi-utils
 Project-URL: Bug Tracker, https://github.com/surquest/python-fastapi-utils/issues
 Author-email: Michal Švarc <michal.svarc@surquest.com>
 License-File: LICENSE
 Requires-Dist: fastapi>=0.81.0
 Requires-Dist: google-cloud-logging>=3.1.0
@@ -22,16 +22,17 @@
 
 # Introduction
 
 This project provides collection of utilities for smooth integration of FastAPI framework with Google Cloud Platform services as logging and tracing.
 
 The key features of this project are:
 
-* Logging to Stackdriver
-* Tracing to Stackdriver
+* Logging to Cloud Logging
+* Tracing to Cloud Logging
+* Error Reporting via Cloud Logging
 * Custom middleware for configuration of logging
 * Custom exception handlers treating HTTP and validation exceptions
 * Custom routes for documentation and favicon
 * Custom responses with statuses `success`, `warning` and `error` and standardized error messages
 
 # Quick Start
```

