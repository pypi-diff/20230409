# Comparing `tmp/exbetapi-2.4.0.tar.gz` & `tmp/exbetapi-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exbetapi-2.4.0.tar", max compression
+gzip compressed data, was "exbetapi-2.4.1.tar", max compression
```

## Comparing `exbetapi-2.4.0.tar` & `exbetapi-2.4.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      143 2023-03-18 21:33:38.525160 exbetapi-2.4.0/exbetapi/__init__.py
--rw-r--r--   0        0        0    18143 2023-03-18 21:33:38.525160 exbetapi-2.4.0/exbetapi/api.py
--rw-r--r--   0        0        0     4850 2023-03-18 21:33:38.525160 exbetapi-2.4.0/exbetapi/cli.py
--rw-r--r--   0        0        0      390 2023-03-18 21:33:38.525160 exbetapi-2.4.0/exbetapi/exceptions.py
--rw-r--r--   0        0        0     1726 2023-03-18 21:33:57.157202 exbetapi-2.4.0/pyproject.toml
--rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 exbetapi-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-04-09 19:19:28.035202 exbetapi-2.4.1/exbetapi/__init__.py
+-rw-r--r--   0        0        0    18167 2023-04-09 19:19:28.035202 exbetapi-2.4.1/exbetapi/api.py
+-rw-r--r--   0        0        0     4850 2023-04-09 19:19:28.035202 exbetapi-2.4.1/exbetapi/cli.py
+-rw-r--r--   0        0        0      390 2023-04-09 19:19:28.035202 exbetapi-2.4.1/exbetapi/exceptions.py
+-rw-r--r--   0        0        0     1726 2023-04-09 19:19:50.188093 exbetapi-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 exbetapi-2.4.1/PKG-INFO
```

### Comparing `exbetapi-2.4.0/exbetapi/api.py` & `exbetapi-2.4.1/exbetapi/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
                 and task.get("info")
             ):
                 task["info"] = eval(task.get("info", "{}"))
                 return task
             time.sleep(self._SLEEPTIME)
             cnt += 1
             if cnt > 3 * self._BLOCKTIME / self._SLEEPTIME:
-                raise ExecutionError("Inform admins")
+                raise ExecutionError(f"Inform admins {task_id}: {str(task)}")
 
     @staticmethod
     def _obtain_task_results(task):  # pragma: no cover
         """A task contains information about the operations performed. Extract
         those
         """
         results = task["info"].get("operation_results")
```

### Comparing `exbetapi-2.4.0/exbetapi/cli.py` & `exbetapi-2.4.1/exbetapi/cli.py`

 * *Files identical despite different names*

### Comparing `exbetapi-2.4.0/pyproject.toml` & `exbetapi-2.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "exbetapi"
-version = "2.4.0"
+version = "2.4.1"
 description = "Python Bindings for Trading API for exbet.io"
 authors = ["Python Development Team <py@exbet.io>"]
 homepage = "https://github.com/exbet/python-exbetapi"
 repository = "https://github.com/exbet/python-exbetapi"
 documentation = "https://python-exbetapi.rtfd.io"
 
 [tool.poetry.urls]
```

### Comparing `exbetapi-2.4.0/PKG-INFO` & `exbetapi-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exbetapi
-Version: 2.4.0
+Version: 2.4.1
 Summary: Python Bindings for Trading API for exbet.io
 Home-page: https://github.com/exbet/python-exbetapi
 Author: Python Development Team
 Author-email: py@exbet.io
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

