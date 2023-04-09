# Comparing `tmp/wg_utilities-3.1.0.tar.gz` & `tmp/wg_utilities-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wg_utilities-3.1.0.tar", max compression
+gzip compressed data, was "wg_utilities-3.1.1.tar", max compression
```

## Comparing `wg_utilities-3.1.0.tar` & `wg_utilities-3.1.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1069 2023-04-08 17:47:26.186761 wg_utilities-3.1.0/LICENSE
--rw-r--r--   0        0        0     1520 2023-04-08 17:47:26.186761 wg_utilities-3.1.0/README.md
--rw-r--r--   0        0        0     4830 2023-04-08 17:47:26.190761 wg_utilities-3.1.0/pyproject.toml
--rw-r--r--   0        0        0      280 2023-04-08 17:47:26.254762 wg_utilities-3.1.0/wg_utilities/__init__.py
--rw-r--r--   0        0        0      140 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/api/__init__.py
--rw-r--r--   0        0        0     7384 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/api/temp_auth_server.py
--rw-r--r--   0        0        0      560 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/__init__.py
--rw-r--r--   0        0        0     4962 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/_google.py
--rw-r--r--   0        0        0    10359 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/_spotify_types.py
--rw-r--r--   0        0        0    24659 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/google_calendar.py
--rw-r--r--   0        0        0    56685 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/google_drive.py
--rw-r--r--   0        0        0     7142 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/google_fit.py
--rw-r--r--   0        0        0    14065 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/google_photos.py
--rw-r--r--   0        0        0    16193 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/monzo.py
--rw-r--r--   0        0        0    24945 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/oauth_client.py
--rw-r--r--   0        0        0    49741 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/spotify.py
--rw-r--r--   0        0        0    21403 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/clients/truelayer.py
--rw-r--r--   0        0        0      126 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/devices/__init__.py
--rw-r--r--   0        0        0      119 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/devices/dht22/__init__.py
--rwxr-xr-x   0        0        0     6589 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/devices/dht22/dht22_lib.py
--rw-r--r--   0        0        0     1129 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/devices/epd/__init__.py
--rw-r--r--   0        0        0     7042 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/devices/epd/epd7in5_v2.py
--rw-r--r--   0        0        0     5993 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/devices/epd/epdconfig.py
--rw-r--r--   0        0        0      138 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/devices/yamaha_yas_209/__init__.py
--rw-r--r--   0        0        0    36226 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
--rw-r--r--   0        0        0     5401 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/exceptions/__init__.py
--rw-r--r--   0        0        0      803 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/functions/__init__.py
--rw-r--r--   0        0        0     4595 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/functions/_functions.py
--rw-r--r--   0        0        0     1287 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/functions/datetime_helpers.py
--rw-r--r--   0        0        0     2024 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/functions/file_management.py
--rw-r--r--   0        0        0     8851 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/functions/json.py
--rw-r--r--   0        0        0     1386 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/functions/processes.py
--rw-r--r--   0        0        0     1106 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/functions/string_manipulation.py
--rw-r--r--   0        0        0     1586 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/functions/xml.py
--rw-r--r--   0        0        0     7258 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/loggers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/py.typed
--rw-r--r--   0        0        0      167 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/testing/__init__.py
--rw-r--r--   0        0        0     5257 2023-04-08 17:47:26.258762 wg_utilities-3.1.0/wg_utilities/testing/_custom_mocks.py
--rw-r--r--   0        0        0     3336 1970-01-01 00:00:00.000000 wg_utilities-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-09 17:34:11.075225 wg_utilities-3.1.1/LICENSE
+-rw-r--r--   0        0        0     1520 2023-04-09 17:34:11.075225 wg_utilities-3.1.1/README.md
+-rw-r--r--   0        0        0     4855 2023-04-09 17:34:11.075225 wg_utilities-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-04-09 17:34:11.155226 wg_utilities-3.1.1/wg_utilities/__init__.py
+-rw-r--r--   0        0        0      140 2023-04-09 17:34:11.155226 wg_utilities-3.1.1/wg_utilities/api/__init__.py
+-rw-r--r--   0        0        0     7384 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/api/temp_auth_server.py
+-rw-r--r--   0        0        0      560 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/__init__.py
+-rw-r--r--   0        0        0     4962 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/_google.py
+-rw-r--r--   0        0        0    10359 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/_spotify_types.py
+-rw-r--r--   0        0        0    24659 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/google_calendar.py
+-rw-r--r--   0        0        0    56685 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/google_drive.py
+-rw-r--r--   0        0        0     7142 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/google_fit.py
+-rw-r--r--   0        0        0    14065 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/google_photos.py
+-rw-r--r--   0        0        0    16193 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/monzo.py
+-rw-r--r--   0        0        0    24945 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/oauth_client.py
+-rw-r--r--   0        0        0    49741 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/spotify.py
+-rw-r--r--   0        0        0    21403 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/clients/truelayer.py
+-rw-r--r--   0        0        0      126 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/devices/__init__.py
+-rw-r--r--   0        0        0      119 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/devices/dht22/__init__.py
+-rwxr-xr-x   0        0        0     6589 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/devices/dht22/dht22_lib.py
+-rw-r--r--   0        0        0     1129 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/devices/epd/__init__.py
+-rw-r--r--   0        0        0     7042 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/devices/epd/epd7in5_v2.py
+-rw-r--r--   0        0        0     5993 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/devices/epd/epdconfig.py
+-rw-r--r--   0        0        0      138 2023-04-09 17:34:11.159226 wg_utilities-3.1.1/wg_utilities/devices/yamaha_yas_209/__init__.py
+-rw-r--r--   0        0        0    36348 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
+-rw-r--r--   0        0        0     5401 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/exceptions/__init__.py
+-rw-r--r--   0        0        0      803 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/functions/__init__.py
+-rw-r--r--   0        0        0     4595 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/functions/_functions.py
+-rw-r--r--   0        0        0     1287 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/functions/datetime_helpers.py
+-rw-r--r--   0        0        0     2024 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/functions/file_management.py
+-rw-r--r--   0        0        0     8851 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/functions/json.py
+-rw-r--r--   0        0        0     1386 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/functions/processes.py
+-rw-r--r--   0        0        0     1106 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/functions/string_manipulation.py
+-rw-r--r--   0        0        0     1586 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/functions/xml.py
+-rw-r--r--   0        0        0     7258 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/loggers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/py.typed
+-rw-r--r--   0        0        0      167 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/testing/__init__.py
+-rw-r--r--   0        0        0     5257 2023-04-09 17:34:11.163226 wg_utilities-3.1.1/wg_utilities/testing/_custom_mocks.py
+-rw-r--r--   0        0        0     3336 1970-01-01 00:00:00.000000 wg_utilities-3.1.1/PKG-INFO
```

### Comparing `wg_utilities-3.1.0/LICENSE` & `wg_utilities-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/README.md` & `wg_utilities-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/pyproject.toml` & `wg_utilities-3.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wg-utilities"
-version = "3.1.0"
+version = "3.1.1"
 description = "Loads of useful stuff for the things I do :)"
 
 authors = ["Will Garside <worgarside@gmail.com>"]
 include = ["wg_utilities/py.typed"]
 license = "MIT"
 maintainers = ["Will Garside <worgarside@gmail.com>"]
 packages = [{ include = "wg_utilities" }]
@@ -27,25 +27,24 @@
 pigpio = { version = "*", optional = true }
 pillow = { version = "*", optional = true }
 pydantic = { version = "*", optional = true }
 pyjwt = { version = "~=2.6.0", optional = true }
 python-dotenv = { version = "*", optional = true }
 pytz = ">=2022.1"
 requests = { version = ">=2.26.0", optional = true }
-"rpi.gpio" = { version = "*", markers = "sys_platform == 'linux'" , optional = true }
+"rpi.gpio" = { version = "*", markers = "sys_platform == 'linux'",  optional = true }
 spidev = { version = "*", markers = "sys_platform == 'linux'", optional = true  }
 strenum = { version = "*", optional = true }
 tzlocal = { version = "*", optional = true }
 xmltodict = { version = "*", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 pylint = "*"
 pre-commit = "*"
-twine = "==4.0.2"
 mypy = "*"
 types-requests = "*"
 types-tzlocal = "*"
 boto3-stubs = "*"
 lxml-stubs = "*"
 types-setuptools = "*"
 pycln = "*"
@@ -134,14 +133,17 @@
     "mocked_operation_lookup: allows setting the mocks in the `mb3c` fixture",
     "upnp_value_path: file with content to set as the value in a `upnp_state_variable` fixture",
 ]
 
 [tool.coverage.report]
 exclude_lines = ["pragma: no cover", "def __repr__", "def __str__", "@overload"]
 
+[tool.coverage.run]
+relative_files = true
+
 [tool.mypy]
 ignore_missing_imports = true
 exclude = ["_local_sandbox"]
 show_error_codes = true
 plugins = 'pydantic.mypy'
 follow_imports = "silent"
 warn_redundant_casts = true
```

### Comparing `wg_utilities-3.1.0/wg_utilities/api/temp_auth_server.py` & `wg_utilities-3.1.1/wg_utilities/api/temp_auth_server.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/clients/__init__.py` & `wg_utilities-3.1.1/wg_utilities/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/clients/_google.py` & `wg_utilities-3.1.1/wg_utilities/clients/_google.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/clients/_spotify_types.py` & `wg_utilities-3.1.1/wg_utilities/clients/_spotify_types.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/clients/google_calendar.py` & `wg_utilities-3.1.1/wg_utilities/clients/google_calendar.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/clients/google_drive.py` & `wg_utilities-3.1.1/wg_utilities/clients/google_drive.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/clients/google_fit.py` & `wg_utilities-3.1.1/wg_utilities/clients/google_fit.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/clients/google_photos.py` & `wg_utilities-3.1.1/wg_utilities/clients/google_photos.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/clients/monzo.py` & `wg_utilities-3.1.1/wg_utilities/clients/monzo.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/clients/oauth_client.py` & `wg_utilities-3.1.1/wg_utilities/clients/oauth_client.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/clients/spotify.py` & `wg_utilities-3.1.1/wg_utilities/clients/spotify.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/clients/truelayer.py` & `wg_utilities-3.1.1/wg_utilities/clients/truelayer.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/devices/dht22/dht22_lib.py` & `wg_utilities-3.1.1/wg_utilities/devices/dht22/dht22_lib.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/devices/epd/__init__.py` & `wg_utilities-3.1.1/wg_utilities/devices/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/devices/epd/epd7in5_v2.py` & `wg_utilities-3.1.1/wg_utilities/devices/epd/epd7in5_v2.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/devices/epd/epdconfig.py` & `wg_utilities-3.1.1/wg_utilities/devices/epd/epdconfig.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py` & `wg_utilities-3.1.1/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from asyncio import new_event_loop, run
 from asyncio import sleep as async_sleep
 from collections.abc import Callable, Coroutine, Mapping, Sequence
 from datetime import datetime, timedelta
 from enum import Enum
 from functools import wraps
 from logging import DEBUG, getLogger
+from re import compile as re_compile
 from textwrap import dedent
 from threading import Thread
 from time import sleep, strptime
 from typing import Any, Literal, TypedDict, TypeVar
 
 from async_upnp_client.aiohttp import AiohttpNotifyServer, AiohttpRequester
 from async_upnp_client.client import UpnpDevice, UpnpService, UpnpStateVariable
@@ -868,19 +869,22 @@
 
         Parse a dictionary where some values are/could be XML strings, and unpack
         the XML into JSON within the dict
 
         Args:
             xml_dict (dict): the dictionary to parse
         """
+
+        pattern = re_compile(r"&(?!(amp|apos|lt|gt|quot);)")
+
         traverse_dict(
             xml_dict,
             target_type=str,
             target_processor_func=lambda val, dict_key=None, list_index=None: parse_xml(
-                val, attr_prefix="", cdata_key="text"
+                pattern.sub("&amp;", val), attr_prefix="", cdata_key="text"
             ),
             single_keys_to_remove=["val", "DIDL-Lite"],
         )
 
     # TODO: @on_exception()
     def pause(self) -> None:
         """Pause the current media."""
```

### Comparing `wg_utilities-3.1.0/wg_utilities/exceptions/__init__.py` & `wg_utilities-3.1.1/wg_utilities/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/functions/__init__.py` & `wg_utilities-3.1.1/wg_utilities/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/functions/_functions.py` & `wg_utilities-3.1.1/wg_utilities/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/functions/datetime_helpers.py` & `wg_utilities-3.1.1/wg_utilities/functions/datetime_helpers.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/functions/file_management.py` & `wg_utilities-3.1.1/wg_utilities/functions/file_management.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/functions/json.py` & `wg_utilities-3.1.1/wg_utilities/functions/json.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/functions/processes.py` & `wg_utilities-3.1.1/wg_utilities/functions/processes.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/functions/string_manipulation.py` & `wg_utilities-3.1.1/wg_utilities/functions/string_manipulation.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/functions/xml.py` & `wg_utilities-3.1.1/wg_utilities/functions/xml.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/loggers/__init__.py` & `wg_utilities-3.1.1/wg_utilities/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/wg_utilities/testing/_custom_mocks.py` & `wg_utilities-3.1.1/wg_utilities/testing/_custom_mocks.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.1.0/PKG-INFO` & `wg_utilities-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wg-utilities
-Version: 3.1.0
+Version: 3.1.1
 Summary: Loads of useful stuff for the things I do :)
 Home-page: https://github.com/worgarside/wg-utilities
 License: MIT
 Author: Will Garside
 Author-email: worgarside@gmail.com
 Maintainer: Will Garside
 Maintainer-email: worgarside@gmail.com
```

