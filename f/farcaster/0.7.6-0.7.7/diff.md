# Comparing `tmp/farcaster-0.7.6.tar.gz` & `tmp/farcaster-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "farcaster-0.7.6.tar", max compression
+gzip compressed data, was "farcaster-0.7.7.tar", max compression
```

## Comparing `farcaster-0.7.6.tar` & `farcaster-0.7.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1084 2023-04-03 20:33:47.263429 farcaster-0.7.6/LICENSE
--rw-r--r--   0        0        0     4755 2023-04-03 20:33:47.263429 farcaster-0.7.6/README.md
--rw-r--r--   0        0        0      479 2023-04-03 20:33:47.267429 farcaster-0.7.6/farcaster/__init__.py
--rw-r--r--   0        0        0    37309 2023-04-03 20:33:47.267429 farcaster-0.7.6/farcaster/client.py
--rw-r--r--   0        0        0      516 2023-04-03 20:33:47.267429 farcaster-0.7.6/farcaster/config.py
--rw-r--r--   0        0        0    14393 2023-04-03 20:33:47.267429 farcaster-0.7.6/farcaster/models.py
--rw-r--r--   0        0        0        0 2023-04-03 20:33:47.267429 farcaster-0.7.6/farcaster/py.typed
--rw-r--r--   0        0        0        0 2023-04-03 20:33:47.267429 farcaster-0.7.6/farcaster/utils/__init__.py
--rw-r--r--   0        0        0     4797 2023-04-03 20:33:47.267429 farcaster-0.7.6/farcaster/utils/stream_generator.py
--rw-r--r--   0        0        0     3985 2023-04-03 20:33:47.267429 farcaster-0.7.6/pyproject.toml
--rw-r--r--   0        0        0     6228 1970-01-01 00:00:00.000000 farcaster-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-09 17:35:25.675298 farcaster-0.7.7/LICENSE
+-rw-r--r--   0        0        0     4755 2023-04-09 17:35:25.675298 farcaster-0.7.7/README.md
+-rw-r--r--   0        0        0      479 2023-04-09 17:35:25.679298 farcaster-0.7.7/farcaster/__init__.py
+-rw-r--r--   0        0        0    37303 2023-04-09 17:35:25.679298 farcaster-0.7.7/farcaster/client.py
+-rw-r--r--   0        0        0      516 2023-04-09 17:35:25.679298 farcaster-0.7.7/farcaster/config.py
+-rw-r--r--   0        0        0    14393 2023-04-09 17:35:25.679298 farcaster-0.7.7/farcaster/models.py
+-rw-r--r--   0        0        0        0 2023-04-09 17:35:25.679298 farcaster-0.7.7/farcaster/py.typed
+-rw-r--r--   0        0        0        0 2023-04-09 17:35:25.679298 farcaster-0.7.7/farcaster/utils/__init__.py
+-rw-r--r--   0        0        0     4797 2023-04-09 17:35:25.679298 farcaster-0.7.7/farcaster/utils/stream_generator.py
+-rw-r--r--   0        0        0     3985 2023-04-09 17:35:25.679298 farcaster-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0     6228 1970-01-01 00:00:00.000000 farcaster-0.7.7/PKG-INFO
```

### Comparing `farcaster-0.7.6/LICENSE` & `farcaster-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `farcaster-0.7.6/README.md` & `farcaster-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `farcaster-0.7.6/farcaster/client.py` & `farcaster-0.7.7/farcaster/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
     def get_healthcheck(self) -> bool:
         """Check if API is up and running
 
         Returns:
             bool: Status of the API
         """
-        response = self.session.get("https://api.farcaster.xyz/healthcheck")
+        response = self.session.get("https://api.warpcast.com/healthcheck")
         return response.ok
 
     def get_asset(self, token_id: int) -> AssetResult:
         """Get asset information
 
         Args:
             token_id (int): token ID
@@ -196,15 +196,15 @@
 
         Returns:
             TokenResult: _description_
         """
         header = self.generate_custody_auth_header(auth_params)
         body = AuthPutRequest(params=auth_params)
         response = requests.put(
-            "https://api.farcaster.xyz/v2/auth",
+            self.config.base_path + "auth",
             json=body.dict(by_alias=True, exclude_none=True),
             headers={"Authorization": header},
         ).json()
         return AuthPutResponse(**response).result
 
     def delete_auth(self) -> StatusContent:
         """Delete an access token
```

### Comparing `farcaster-0.7.6/farcaster/config.py` & `farcaster-0.7.7/farcaster/config.py`

 * *Files identical despite different names*

### Comparing `farcaster-0.7.6/farcaster/models.py` & `farcaster-0.7.7/farcaster/models.py`

 * *Files identical despite different names*

### Comparing `farcaster-0.7.6/farcaster/utils/stream_generator.py` & `farcaster-0.7.7/farcaster/utils/stream_generator.py`

 * *Files identical despite different names*

### Comparing `farcaster-0.7.6/pyproject.toml` & `farcaster-0.7.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "farcaster"
-version = "0.7.6"
+version = "0.7.7"
 description = "farcaster-py is a Python SDK for the Farcaster Protocol"
 readme = "README.md"
 authors = ["Andreessen Horowitz <crypto-engineering@a16z.com>"]
 license = "MIT"
 repository = "https://github.com/a16z/farcaster-py"
 homepage = "https://github.com/a16z/farcaster-py"
 
@@ -59,15 +59,15 @@
 pytest-dependency = "^0.5.1"
 pytest-html = "^3.1.1"
 pytest-cov = "^4.0.0"
 pytest-recording = "^0.12.1"
 docconvert = "^2.0.0"
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.0.5"
-mkdocstrings = ">=0.19.1,<0.21.0"
+mkdocstrings = ">=0.19.1,<0.22.0"
 mkdocstrings-python = "^0.8.3"
 pillow = "^9.4.0"
 cairosvg = "^2.6.0"
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py310"]
```

### Comparing `farcaster-0.7.6/PKG-INFO` & `farcaster-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: farcaster
-Version: 0.7.6
+Version: 0.7.7
 Summary: farcaster-py is a Python SDK for the Farcaster Protocol
 Home-page: https://github.com/a16z/farcaster-py
 License: MIT
 Author: Andreessen Horowitz
 Author-email: crypto-engineering@a16z.com
 Requires-Python: >3.7.1,<3.11
 Classifier: Development Status :: 3 - Alpha
```

