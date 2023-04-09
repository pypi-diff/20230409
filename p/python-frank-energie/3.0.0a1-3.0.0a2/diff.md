# Comparing `tmp/python_frank_energie-3.0.0a1.tar.gz` & `tmp/python_frank_energie-3.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_frank_energie-3.0.0a1.tar", max compression
+gzip compressed data, was "python_frank_energie-3.0.0a2.tar", max compression
```

## Comparing `python_frank_energie-3.0.0a1.tar` & `python_frank_energie-3.0.0a2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11346 2023-03-31 19:15:54.688375 python_frank_energie-3.0.0a1/LICENSE
--rw-r--r--   0        0        0      325 2023-03-31 19:15:54.688375 python_frank_energie-3.0.0a1/README.md
--rw-r--r--   0        0        0     2340 2023-03-31 19:16:17.885936 python_frank_energie-3.0.0a1/pyproject.toml
--rw-r--r--   0        0        0      175 2023-03-31 19:15:54.692375 python_frank_energie-3.0.0a1/python_frank_energie/__init__.py
--rw-r--r--   0        0        0      257 2023-03-31 19:15:54.692375 python_frank_energie-3.0.0a1/python_frank_energie/exceptions.py
--rw-r--r--   0        0        0     5093 2023-03-31 19:15:54.692375 python_frank_energie-3.0.0a1/python_frank_energie/frank_energie.py
--rw-r--r--   0        0        0     5763 2023-03-31 19:15:54.692375 python_frank_energie-3.0.0a1/python_frank_energie/models.py
--rw-r--r--   0        0        0     1219 1970-01-01 00:00:00.000000 python_frank_energie-3.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-03-31 20:23:15.208961 python_frank_energie-3.0.0a2/LICENSE
+-rw-r--r--   0        0        0      325 2023-03-31 20:23:15.208961 python_frank_energie-3.0.0a2/README.md
+-rw-r--r--   0        0        0     2340 2023-03-31 20:23:35.157119 python_frank_energie-3.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-03-31 20:23:15.208961 python_frank_energie-3.0.0a2/python_frank_energie/__init__.py
+-rw-r--r--   0        0        0      257 2023-03-31 20:23:15.208961 python_frank_energie-3.0.0a2/python_frank_energie/exceptions.py
+-rw-r--r--   0        0        0     5080 2023-03-31 20:23:15.208961 python_frank_energie-3.0.0a2/python_frank_energie/frank_energie.py
+-rw-r--r--   0        0        0     5763 2023-03-31 20:23:15.208961 python_frank_energie-3.0.0a2/python_frank_energie/models.py
+-rw-r--r--   0        0        0     1219 1970-01-01 00:00:00.000000 python_frank_energie-3.0.0a2/PKG-INFO
```

### Comparing `python_frank_energie-3.0.0a1/LICENSE` & `python_frank_energie-3.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_frank_energie-3.0.0a1/pyproject.toml` & `python_frank_energie-3.0.0a2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-frank-energie"
-version = "3.0.0-alpha-1"
+version = "3.0.0-alpha-2"
 description = "Asynchronous Python client for the Frank Energie"
 authors = ["DCSBL"]
 maintainers = ["DCSBL"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://github.com/dcsbl/python-frank-energie"
 repository = "https://github.com/dcsbl/python-frank-energie"
```

### Comparing `python_frank_energie-3.0.0a1/python_frank_energie/frank_energie.py` & `python_frank_energie-3.0.0a2/python_frank_energie/frank_energie.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                 }
             """,
             "operationName": "Login",
             "variables": {"email": username, "password": password},
         }
 
         self._auth = Authentication.from_dict(await self._query(query))
-        return self._auth.refreshToken
+        return self._auth
 
     async def monthSummary(self) -> MonthSummary:
 
         if self._auth is None:
             raise AuthRequiredException
 
         query = {
```

### Comparing `python_frank_energie-3.0.0a1/python_frank_energie/models.py` & `python_frank_energie-3.0.0a2/python_frank_energie/models.py`

 * *Files identical despite different names*

### Comparing `python_frank_energie-3.0.0a1/PKG-INFO` & `python_frank_energie-3.0.0a2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-frank-energie
-Version: 3.0.0a1
+Version: 3.0.0a2
 Summary: Asynchronous Python client for the Frank Energie
 Home-page: https://github.com/dcsbl/python-frank-energie
 License: Apache-2.0
 Author: DCSBL
 Maintainer: DCSBL
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

