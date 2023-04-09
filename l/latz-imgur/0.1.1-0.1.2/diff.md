# Comparing `tmp/latz_imgur-0.1.1.tar.gz` & `tmp/latz_imgur-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latz_imgur-0.1.1.tar", max compression
+gzip compressed data, was "latz_imgur-0.1.2.tar", max compression
```

## Comparing `latz_imgur-0.1.1.tar` & `latz_imgur-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2022-12-28 16:22:03.152191 latz_imgur-0.1.1/LICENSE
--rw-r--r--   0        0        0       69 2022-12-28 16:22:03.152435 latz_imgur-0.1.1/README.md
--rw-r--r--   0        0        0        0 2022-12-28 16:22:55.031380 latz_imgur-0.1.1/latz_imgur/__init__.py
--rw-r--r--   0        0        0      123 2023-03-26 12:29:57.282398 latz_imgur-0.1.1/latz_imgur/__version__.py
--rw-r--r--   0        0        0     2386 2023-04-01 05:43:58.972773 latz_imgur-0.1.1/latz_imgur/main.py
--rw-r--r--   0        0        0      649 2023-04-01 05:49:37.385753 latz_imgur-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      864 1970-01-01 00:00:00.000000 latz_imgur-0.1.1/setup.py
--rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 latz_imgur-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-28 16:22:03.152191 latz_imgur-0.1.2/LICENSE
+-rw-r--r--   0        0        0       69 2022-12-28 16:22:03.152435 latz_imgur-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2022-12-28 16:22:55.031380 latz_imgur-0.1.2/latz_imgur/__init__.py
+-rw-r--r--   0        0        0      123 2023-04-09 08:53:52.201894 latz_imgur-0.1.2/latz_imgur/__version__.py
+-rw-r--r--   0        0        0     2409 2023-04-09 08:35:20.512946 latz_imgur-0.1.2/latz_imgur/main.py
+-rw-r--r--   0        0        0      650 2023-04-09 09:06:03.881845 latz_imgur-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      867 1970-01-01 00:00:00.000000 latz_imgur-0.1.2/setup.py
+-rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 latz_imgur-0.1.2/PKG-INFO
```

### Comparing `latz_imgur-0.1.1/LICENSE` & `latz_imgur-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `latz_imgur-0.1.1/latz_imgur/main.py` & `latz_imgur-0.1.2/latz_imgur/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import urllib.parse
 
 import httpx
-from pydantic import BaseModel, Field
-from latz.image import ImageSearchResultSet, ImageSearchResult
+from pydantic import BaseModel, SecretStr, Field
+from latz.image import ImageSearchResult
 from latz.plugins import hookimpl, SearchBackendHook
 from latz.exceptions import SearchBackendError
 
 #: Name of the plugin that will be referenced in our configuration
 PLUGIN_NAME = "imgur"
 
 #: Base URL for the Imgur API
@@ -43,36 +43,38 @@
 
     if not isinstance(json_data, dict):
         raise SearchBackendError("Received malformed response from search backend")
 
     return json_data
 
 
-async def search(client, config, query: str) -> ImageSearchResultSet:
+async def search(client, config, query: str) -> tuple[ImageSearchResult, ...]:
+    """
+    Search function that retrieves results from the Imgur API
+    """
+    access_key = config.search_backend_settings.imgur.access_key
+
     client.headers = httpx.Headers(
         {
-            "Authorization": f"Client-ID {config.search_backend_settings.imgur.access_key}"
+            "Authorization": f"Client-ID {access_key}"
         }
     )
     json_data = await _get(client, SEARCH_ENDPOINT, query)
 
-    search_results = tuple(
+    return tuple(
         ImageSearchResult(
             url=record_image.get("link"),
             width=record_image.get("width"),
-            height=record_image.get("height")
+            height=record_image.get("height"),
+            search_backend=PLUGIN_NAME
         )
         for record in json_data.get("data", tuple())
         for record_image in record.get("images", tuple())
     )
 
-    return ImageSearchResultSet(
-        search_results, len(search_results), search_backend=PLUGIN_NAME
-    )
-
 
 @hookimpl
 def search_backend():
     """
     Registers our Imgur image API backend
     """
     return SearchBackendHook(
```

### Comparing `latz_imgur-0.1.1/pyproject.toml` & `latz_imgur-0.1.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "latz-imgur"
-version = "0.1.1"
+version = "0.1.2"
 description = "Imgur plugin for the popular latz image search CLI tool"
 authors = ["Travis Hathaway <travis.j.hathaway@gmail.com>"]
 license = "GPUv3"
 readme = "README.md"
 packages = [{include = "latz_imgur"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
-latz = "0.2.0"
-pydantic = "^1.10.4"
-httpx = "^0.23.1"
+python = "^3.8.1"
+latz = "0.2.1"
+pydantic = "^1.10.7"
+httpx = "^0.23.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 darker = "^1.6.0"
 mypy = "^0.991"
 flake8 = "^6.0.0"
 pyupgrade = "^3.3.1"
```

### Comparing `latz_imgur-0.1.1/setup.py` & `latz_imgur-0.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 packages = \
 ['latz_imgur']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['httpx>=0.23.1,<0.24.0', 'latz==0.2.0', 'pydantic>=1.10.4,<2.0.0']
+['httpx>=0.23.3,<0.24.0', 'latz==0.2.1', 'pydantic>=1.10.7,<2.0.0']
 
 entry_points = \
 {'latz': ['imgur = latz_imgur.main']}
 
 setup_kwargs = {
     'name': 'latz-imgur',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Imgur plugin for the popular latz image search CLI tool',
     'long_description': '# latz-imgur\nImgur plugin for the popular latz image search CLI tool\n',
     'author': 'Travis Hathaway',
     'author_email': 'travis.j.hathaway@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.8.1,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `latz_imgur-0.1.1/PKG-INFO` & `latz_imgur-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: latz-imgur
-Version: 0.1.1
+Version: 0.1.2
 Summary: Imgur plugin for the popular latz image search CLI tool
 License: GPUv3
 Author: Travis Hathaway
 Author-email: travis.j.hathaway@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: httpx (>=0.23.1,<0.24.0)
-Requires-Dist: latz (==0.2.0)
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
+Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: latz (==0.2.1)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Description-Content-Type: text/markdown
 
 # latz-imgur
 Imgur plugin for the popular latz image search CLI tool
```

