# Comparing `tmp/latz-0.2.0.tar.gz` & `tmp/latz-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latz-0.2.0.tar", max compression
+gzip compressed data, was "latz-0.2.1.tar", max compression
```

## Comparing `latz-0.2.0.tar` & `latz-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    35149 2022-12-26 15:23:51.948928 latz-0.2.0/LICENSE
--rw-r--r--   0        0        0     3660 2023-03-21 15:03:54.149100 latz-0.2.0/README.md
--rw-r--r--   0        0        0        0 2022-12-26 15:39:44.319136 latz-0.2.0/latz/__init__.py
--rw-r--r--   0        0        0       32 2022-12-26 17:26:42.986898 latz-0.2.0/latz/__main__.py
--rw-r--r--   0        0        0      114 2023-02-12 15:26:39.939864 latz-0.2.0/latz/__version__.py
--rw-r--r--   0        0        0     2248 2023-03-21 14:35:03.207031 latz-0.2.0/latz/cli.py
--rw-r--r--   0        0        0      125 2022-12-30 06:12:02.158385 latz-0.2.0/latz/commands/__init__.py
--rw-r--r--   0        0        0        0 2022-12-30 06:09:15.533001 latz-0.2.0/latz/commands/config/__init__.py
--rw-r--r--   0        0        0     1741 2023-03-21 14:55:55.633831 latz-0.2.0/latz/commands/config/commands.py
--rw-r--r--   0        0        0     5345 2023-03-21 14:35:03.207595 latz-0.2.0/latz/commands/config/validators.py
--rw-r--r--   0        0        0      931 2023-03-21 14:35:03.208321 latz-0.2.0/latz/commands/search.py
--rw-r--r--   0        0        0      158 2023-02-12 15:24:55.309271 latz-0.2.0/latz/config/__init__.py
--rw-r--r--   0        0        0     1320 2022-12-27 17:50:22.421504 latz-0.2.0/latz/config/errors.py
--rw-r--r--   0        0        0     5387 2023-02-12 15:18:41.160146 latz-0.2.0/latz/config/main.py
--rw-r--r--   0        0        0      478 2023-03-21 14:35:03.209075 latz-0.2.0/latz/config/models.py
--rw-r--r--   0        0        0      437 2023-03-21 14:51:42.094793 latz-0.2.0/latz/constants.py
--rw-r--r--   0        0        0      513 2023-03-21 14:35:03.209805 latz-0.2.0/latz/exceptions.py
--rw-r--r--   0        0        0     1159 2023-03-21 14:35:03.210081 latz-0.2.0/latz/fetch.py
--rw-r--r--   0        0        0     2047 2023-03-21 14:35:03.210550 latz-0.2.0/latz/image.py
--rw-r--r--   0        0        0       64 2023-03-21 14:35:03.211249 latz-0.2.0/latz/plugins/__init__.py
--rw-r--r--   0        0        0     2213 2023-03-21 15:47:31.187528 latz-0.2.0/latz/plugins/hookspec.py
--rw-r--r--   0        0        0        0 2022-12-27 16:56:40.900108 latz-0.2.0/latz/plugins/image/__init__.py
--rw-r--r--   0        0        0     1490 2023-03-21 14:35:03.212494 latz-0.2.0/latz/plugins/image/placeholder.py
--rw-r--r--   0        0        0     2585 2023-03-21 14:35:03.212904 latz-0.2.0/latz/plugins/image/unsplash.py
--rw-r--r--   0        0        0     5107 2023-03-21 14:35:03.213346 latz-0.2.0/latz/plugins/manager.py
--rw-r--r--   0        0        0        0 2023-01-14 11:48:02.530113 latz-0.2.0/latz/py.typed
--rw-r--r--   0        0        0      925 2023-03-21 15:48:57.945469 latz-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4846 1970-01-01 00:00:00.000000 latz-0.2.0/setup.py
--rw-r--r--   0        0        0     4411 1970-01-01 00:00:00.000000 latz-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-26 15:23:51.948928 latz-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3660 2023-03-21 15:03:54.149100 latz-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2022-12-26 15:39:44.319136 latz-0.2.1/latz/__init__.py
+-rw-r--r--   0        0        0       32 2022-12-26 17:26:42.986898 latz-0.2.1/latz/__main__.py
+-rw-r--r--   0        0        0      114 2023-04-09 08:55:39.013145 latz-0.2.1/latz/__version__.py
+-rw-r--r--   0        0        0     2248 2023-03-21 14:35:03.207031 latz-0.2.1/latz/cli.py
+-rw-r--r--   0        0        0      125 2022-12-30 06:12:02.158385 latz-0.2.1/latz/commands/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-30 06:09:15.533001 latz-0.2.1/latz/commands/config/__init__.py
+-rw-r--r--   0        0        0     1741 2023-03-21 14:55:55.633831 latz-0.2.1/latz/commands/config/commands.py
+-rw-r--r--   0        0        0     5345 2023-03-21 14:35:03.207595 latz-0.2.1/latz/commands/config/validators.py
+-rw-r--r--   0        0        0     1889 2023-04-09 08:26:25.323916 latz-0.2.1/latz/commands/search.py
+-rw-r--r--   0        0        0      158 2023-02-12 15:24:55.309271 latz-0.2.1/latz/config/__init__.py
+-rw-r--r--   0        0        0     1320 2022-12-27 17:50:22.421504 latz-0.2.1/latz/config/errors.py
+-rw-r--r--   0        0        0     5387 2023-02-12 15:18:41.160146 latz-0.2.1/latz/config/main.py
+-rw-r--r--   0        0        0      478 2023-03-21 14:35:03.209075 latz-0.2.1/latz/config/models.py
+-rw-r--r--   0        0        0      437 2023-03-21 14:51:42.094793 latz-0.2.1/latz/constants.py
+-rw-r--r--   0        0        0      513 2023-03-21 14:35:03.209805 latz-0.2.1/latz/exceptions.py
+-rw-r--r--   0        0        0     1159 2023-03-21 14:35:03.210081 latz-0.2.1/latz/fetch.py
+-rw-r--r--   0        0        0      360 2023-04-09 08:47:39.546148 latz-0.2.1/latz/image.py
+-rw-r--r--   0        0        0       64 2023-03-21 14:35:03.211249 latz-0.2.1/latz/plugins/__init__.py
+-rw-r--r--   0        0        0     2172 2023-04-09 08:58:53.235015 latz-0.2.1/latz/plugins/hookspec.py
+-rw-r--r--   0        0        0        0 2022-12-27 16:56:40.900108 latz-0.2.1/latz/plugins/image/__init__.py
+-rw-r--r--   0        0        0     1471 2023-04-09 08:58:53.235133 latz-0.2.1/latz/plugins/image/placeholder.py
+-rw-r--r--   0        0        0     2498 2023-04-09 08:58:04.271861 latz-0.2.1/latz/plugins/image/unsplash.py
+-rw-r--r--   0        0        0     5107 2023-04-08 13:53:04.757057 latz-0.2.1/latz/plugins/manager.py
+-rw-r--r--   0        0        0        0 2023-01-14 11:48:02.530113 latz-0.2.1/latz/py.typed
+-rw-r--r--   0        0        0      926 2023-04-09 08:50:21.255376 latz-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4849 1970-01-01 00:00:00.000000 latz-0.2.1/setup.py
+-rw-r--r--   0        0        0     4464 1970-01-01 00:00:00.000000 latz-0.2.1/PKG-INFO
```

### Comparing `latz-0.2.0/LICENSE` & `latz-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `latz-0.2.0/README.md` & `latz-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `latz-0.2.0/latz/cli.py` & `latz-0.2.1/latz/cli.py`

 * *Files identical despite different names*

### Comparing `latz-0.2.0/latz/commands/config/commands.py` & `latz-0.2.1/latz/commands/config/commands.py`

 * *Files identical despite different names*

### Comparing `latz-0.2.0/latz/commands/config/validators.py` & `latz-0.2.1/latz/commands/config/validators.py`

 * *Files identical despite different names*

### Comparing `latz-0.2.0/latz/config/errors.py` & `latz-0.2.1/latz/config/errors.py`

 * *Files identical despite different names*

### Comparing `latz-0.2.0/latz/config/main.py` & `latz-0.2.1/latz/config/main.py`

 * *Files identical despite different names*

### Comparing `latz-0.2.0/latz/exceptions.py` & `latz-0.2.1/latz/exceptions.py`

 * *Files identical despite different names*

### Comparing `latz-0.2.0/latz/fetch.py` & `latz-0.2.1/latz/fetch.py`

 * *Files identical despite different names*

### Comparing `latz-0.2.0/latz/plugins/hookspec.py` & `latz-0.2.1/latz/plugins/hookspec.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from collections.abc import Callable
 
 import httpx
 import pluggy  # type: ignore
 from pydantic import BaseModel
 
 from latz.constants import APP_NAME
-from latz.image import ImageSearchResultSet
+from latz.image import ImageSearchResult
 
 hookspec = pluggy.HookspecMarker(APP_NAME)
 hookimpl = pluggy.HookimplMarker(APP_NAME)
 
 
 class SearchBackendHook(NamedTuple):
     """
@@ -46,23 +46,24 @@
           "param_one": "value"
         }
       }
     }
     ```
     """
 
-    search: Callable[[httpx.AsyncClient, Any, str], Awaitable[ImageSearchResultSet]]
+    search: Callable[
+        [httpx.AsyncClient, Any, str], Awaitable[tuple[ImageSearchResult, ...]]
+    ]
     """
     Callable that implements the search hook.
     """
 
     config_fields: BaseModel
     """
-    Mapping defining the namespace for the config parameters, the pydantic
-    model to use and the default values it should contain.
+    Pydantic model that defines all the settings that this plugin needs.
 
     **Example:**
 
     ```python
 
     from pydantic import BaseModel, Field
```

### Comparing `latz-0.2.0/latz/plugins/image/placeholder.py` & `latz-0.2.1/latz/plugins/image/placeholder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,53 @@
 from typing import Literal
 from urllib.parse import urljoin
 
 from pydantic import BaseModel, Field
 
 from ...image import (
     ImageSearchResult,
-    ImageSearchResultSet,
 )
 from .. import hookimpl, SearchBackendHook
 
 #: Name of the plugin that will be referenced in our configuration
 PLUGIN_NAME = "placeholder"
 
 
 class PlaceholderBackendConfig(BaseModel):
     """
-    Unsplash requires the usage of an ``access_key`` and ``secret_key``
-    when using their API. We expose these settings here so users of the CLI
-    tool can use it.
+    Configuration for the placeholder backend. Currently only supports "bear"
+    or "kitten".
     """
 
     type: Literal["bear", "kitten"] = Field(
         default="kitten", description="The type of placeholder image links to use"
     )
 
 
-async def search(client, config, query: str) -> ImageSearchResultSet:
+async def search(client, config, query: str) -> tuple[ImageSearchResult, ...]:
+    """
+    Search function for placeholder backend. It only returns three pre-defined
+    search results. This is primarily meant for testing and demonstration purposes.
+    """
     placeholder_type = config.search_backend_settings.placeholder.type
     base_url = f"https://place{placeholder_type}.com"
     sizes = ((200, 300), (600, 500), (1000, 800))
 
-    results = tuple(
+    return tuple(
         ImageSearchResult(
             url=urljoin(base_url, f"{width}/{height}"),
             width=width,
             height=height,
+            search_backend=PLUGIN_NAME,
         )
         for width, height in sizes
     )
 
-    return ImageSearchResultSet(
-        results=results, total_number_results=len(results), search_backend=PLUGIN_NAME
-    )
-
 
 @hookimpl
 def search_backend():
     """
-    Registers our Unsplash image API backend
+    Registers our placeholder search backend
     """
     return SearchBackendHook(
-        name=PLUGIN_NAME,
-        search=search,
-        config_fields=PlaceholderBackendConfig(),
+        name=PLUGIN_NAME, search=search, config_fields=PlaceholderBackendConfig()
     )
```

### Comparing `latz-0.2.0/latz/plugins/image/unsplash.py` & `latz-0.2.1/latz/plugins/image/unsplash.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import urllib.parse
 
 import httpx
 from pydantic import BaseModel, Field
 
 from ...image import (
     ImageSearchResult,
-    ImageSearchResultSet,
 )
 from .. import hookimpl, SearchBackendHook
 from ...exceptions import SearchBackendError
 
 #: Name of the plugin that will be referenced in our configuration
 PLUGIN_NAME = "unsplash"
 
@@ -49,40 +48,36 @@
 
     if not isinstance(json_data, dict):
         raise SearchBackendError("Received malformed response from search backend")
 
     return json_data
 
 
-async def search(client: httpx.AsyncClient, config, query: str) -> ImageSearchResultSet:
+async def search(
+    client: httpx.AsyncClient, config, query: str
+) -> tuple[ImageSearchResult, ...]:
     """
-    Find images based on a `query` and return an `ImageSearchResultSet`
+    Find images based on a `query` and return a tuple of `ImageSearchResult` objects.
 
     :raises SearchBackendError: Encountered during problems querying the API
     """
-    client.headers = httpx.Headers(
-        {
-            "Authorization": f"Client-ID {config.search_backend_settings.unsplash.access_key}"
-        }
-    )
+    access_key = config.search_backend_settings.unsplash.access_key
+    client.headers = httpx.Headers({"Authorization": f"Client-ID {access_key}"})
     json_data = await _get(client, SEARCH_ENDPOINT, query)
 
-    search_results = tuple(
+    return tuple(
         ImageSearchResult(
             url=record.get("links", {}).get("download"),
             width=record.get("width"),
             height=record.get("height"),
+            search_backend=PLUGIN_NAME,
         )
         for record in json_data.get("results", tuple())
     )
 
-    return ImageSearchResultSet(
-        search_results, len(search_results), search_backend=PLUGIN_NAME
-    )
-
 
 @hookimpl
 def search_backend():
     """
     Registers our Unsplash image API backend
     """
     return SearchBackendHook(
```

### Comparing `latz-0.2.0/latz/plugins/manager.py` & `latz-0.2.1/latz/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `latz-0.2.0/pyproject.toml` & `latz-0.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "latz"
-version = "0.2.0"
+version = "0.2.1"
 description = "CLI Program for downloading images. Maybe by location too..."
 authors = ["Travis Hathaway <travis.j.hathaway@gmail.com>"]
 license = "GNU v3"
 readme = "README.md"
 packages = [
     { include = "latz" },
     { include = "latz/py.typed" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
-pydantic = "^1.10.2"
+python = "^3.8.1"
+pydantic = "^1.10.7"
 httpx = "^0.23.1"
 Pillow = "^9.3.0"
-rich = "^12.6.0"
+rich = "^13.3.3"
 rich-click = "^1.6.0"
 click = "^8.1.3"
 pluggy = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 darker = "^1.6.0"
```

### Comparing `latz-0.2.0/setup.py` & `latz-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,34 +15,34 @@
 modules = \
 ['py']
 install_requires = \
 ['Pillow>=9.3.0,<10.0.0',
  'click>=8.1.3,<9.0.0',
  'httpx>=0.23.1,<0.24.0',
  'pluggy>=1.0.0,<2.0.0',
- 'pydantic>=1.10.2,<2.0.0',
+ 'pydantic>=1.10.7,<2.0.0',
  'rich-click>=1.6.0,<2.0.0',
- 'rich>=12.6.0,<13.0.0']
+ 'rich>=13.3.3,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['latz = latz.cli:cli']}
 
 setup_kwargs = {
     'name': 'latz',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'CLI Program for downloading images. Maybe by location too...',
     'long_description': '# Overview\n\n[pluggy]: https://pluggy.readthedocs.io/en/stable/\n[click]: https://click.palletsprojects.com/\n[pydantic]: https://docs.pydantic.dev/\n[rich]: https://rich.readthedocs.io/\n[anaconda.org]: https://anaconda.org\n[latz-imgur]: https://github.com/travishathaway/latz-imgur\n[creating-plugins]: creating-plugins\n\nThis is a command line tool used for retrieving images from various image\nsearch backends (e.g. Unsplash, Google). This tool is primarily developed for educational purposes\nto show people how to develop plugin friendly Python applications. Furthermore,\nit is an example project that shows how to effectively pair a handful of\npopular Python libraries to write command line applications.\n\nTo facilitate our plugin architecture, the [pluggy][pluggy] library is used.\nOther libraries used include the following:\n\n- [click][click]: used for structuring the command line application 🖱 💻\n- [pydantic][pydantic]: used for handling configuration file validation 🗃\n- [rich][rich]: used for UX/UI elements and generally making the application more pretty 🌈\n\n### Why "latz"\n\n"latz" is short and easy to type! This is super important when writing CLI programs.\nI also might add a geolocation search feature, so it is a reference  to the word "latitude".\n\n## Quick Start\n\n### Installation\n\nlatz is available for install either on PyPI:\n\n```bash\n# Run from a new virtual environment\n$ pip install latz\n```\n\nor my own [anaconda.org][anaconda.org] channel:\n\n```bash\n$ conda create -n latz \'thath::latz\'\n```\n\nIf you are interested in tinkering around with the code yourself, you can also\nrun it locally:\n\n```bash\n$ git clone git@github.com:/travishathaway/latz.git\n$ cd latz\n# Create a virtual environment however you like..\n$ pip install -e .\n```\n\n### Usage\n\nLatz comes initially configured with the "unsplash" image search backend. To use this,\nyou will need to create an Unsplash account and create a test application. After getting\nyour "access_key", you can set this value by running this command:\n\n```bash\n$ latz config set search_backend_settings.unsplash.access_key=<YOUR_ACCESS_KEY>\n```\n\nOnce this is configured, you can search Unsplash for bunny pictures:\n\n```bash\n$ latz search "bunny"\n[\n    ImageSearchResultSet(\n        results=(\n            ImageSearchResult(\n                url=\'https://unsplash.com/photos/u_kMWN-BWyU/download?ixid=MnwzOTMwOTR8MHwxfHNlYXJjaHwxfHxidW5ueXxlbnwwfHx8fDE2Nzk0MTA2NzQ\',\n                width=3456,\n                height=5184\n            ),\n            # ... results truncated\n        ),\n        total_number_results=10,\n        search_backend=\'unsplash\'\n    )\n]\n```\n\n### Configuring\n\nThe configuration for latz is stored in your home direct and is in the JSON format.\nBelow is a what a default version of this configuration looks like:\n\n```json\n{\n  "search_backends": [\n    "unsplash"\n  ],\n  "search_backend_settings": {\n    "placeholder": {\n      "type": "kitten"\n    },\n    "unsplash": {\n      "access_key": "your-access-key"\n    }\n  }\n}\n```\n\n_Latz will also search in your current working directory for a `.latz.json` file and use this in your configuration.\nFiles in the current working directory will be prioritized over your home directory location._\n\nTo see other available image search backends, see [Available image search backends](#available-image-search-backends) below.\n\n### Available image search backends\n\nHere are a list of the available search backends:\n\n#### Built-in\n\n- "unsplash"\n- "placeholder"\n\n#### Third-party\n\n- [latz-imgur][latz-imgur]\n\n### How to extend and write your own image search backend\n\nPlease see the [creating plugins][creating-plugins] guide in the documentation.\n',
     'author': 'Travis Hathaway',
     'author_email': 'travis.j.hathaway@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'py_modules': modules,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.8.1,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `latz-0.2.0/PKG-INFO` & `latz-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: latz
-Version: 0.2.0
+Version: 0.2.1
 Summary: CLI Program for downloading images. Maybe by location too...
 License: GNU v3
 Author: Travis Hathaway
 Author-email: travis.j.hathaway@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.3.0,<10.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: httpx (>=0.23.1,<0.24.0)
 Requires-Dist: pluggy (>=1.0.0,<2.0.0)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
-Requires-Dist: rich (>=12.6.0,<13.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: rich (>=13.3.3,<14.0.0)
 Requires-Dist: rich-click (>=1.6.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Overview
 
 [pluggy]: https://pluggy.readthedocs.io/en/stable/
 [click]: https://click.palletsprojects.com/
```

