# Comparing `tmp/aiopyarr-22.9.0.tar.gz` & `tmp/aiopyarr-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopyarr-22.9.0.tar", last modified: Tue Sep 27 22:23:07 2022, max compression
+gzip compressed data, was "aiopyarr-23.4.0.tar", last modified: Sun Apr  9 01:01:00 2023, max compression
```

## Comparing `aiopyarr-22.9.0.tar` & `aiopyarr-23.4.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 22:23:07.936025 aiopyarr-22.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2324 2022-09-27 22:23:07.936025 aiopyarr-22.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1545 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 22:23:07.932025 aiopyarr-22.9.0/aiopyarr/
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/const.py
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    24668 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/lidarr_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 22:23:07.936025 aiopyarr-22.9.0/aiopyarr/models/
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4047 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/models/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/models/const.py
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/models/host_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)    14021 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/models/lidarr.py
--rw-r--r--   0 runner    (1001) docker     (121)     6662 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/models/lidarr_common.py
--rw-r--r--   0 runner    (1001) docker     (121)    10521 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/models/radarr.py
--rw-r--r--   0 runner    (1001) docker     (121)     7562 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/models/radarr_common.py
--rw-r--r--   0 runner    (1001) docker     (121)    15461 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/models/readarr.py
--rw-r--r--   0 runner    (1001) docker     (121)    18230 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/models/readarr_common.py
--rw-r--r--   0 runner    (1001) docker     (121)    14410 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/models/request.py
--rw-r--r--   0 runner    (1001) docker     (121)    52800 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/models/request_common.py
--rw-r--r--   0 runner    (1001) docker     (121)    12084 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/models/sonarr.py
--rw-r--r--   0 runner    (1001) docker     (121)     6998 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/models/sonarr_common.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    23605 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/radarr_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    27576 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/readarr_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    38654 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/request_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    24643 2022-09-27 22:23:00.000000 aiopyarr-22.9.0/aiopyarr/sonarr_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 22:23:07.932025 aiopyarr-22.9.0/aiopyarr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2324 2022-09-27 22:23:07.000000 aiopyarr-22.9.0/aiopyarr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      833 2022-09-27 22:23:07.000000 aiopyarr-22.9.0/aiopyarr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 22:23:07.000000 aiopyarr-22.9.0/aiopyarr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-27 22:23:07.000000 aiopyarr-22.9.0/aiopyarr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-27 22:23:07.000000 aiopyarr-22.9.0/aiopyarr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-09-27 22:23:07.936025 aiopyarr-22.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-09-27 22:23:07.000000 aiopyarr-22.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:01:00.313641 aiopyarr-23.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-09 01:01:00.313641 aiopyarr-23.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:01:00.305641 aiopyarr-23.4.0/aiopyarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24668 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/lidarr_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:01:00.309641 aiopyarr-23.4.0/aiopyarr/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/models/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/models/host_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14053 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/models/lidarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/models/lidarr_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/models/radarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/models/radarr_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/models/readarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/models/readarr_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14410 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53089 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/models/request_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/models/sonarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/models/sonarr_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23605 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/radarr_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27582 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/readarr_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38679 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/request_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24643 2023-04-09 01:00:50.000000 aiopyarr-23.4.0/aiopyarr/sonarr_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 01:01:00.305641 aiopyarr-23.4.0/aiopyarr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-09 01:01:00.000000 aiopyarr-23.4.0/aiopyarr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-09 01:01:00.000000 aiopyarr-23.4.0/aiopyarr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 01:01:00.000000 aiopyarr-23.4.0/aiopyarr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-09 01:01:00.000000 aiopyarr-23.4.0/aiopyarr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 01:01:00.000000 aiopyarr-23.4.0/aiopyarr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-09 01:01:00.313641 aiopyarr-23.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-09 01:00:58.000000 aiopyarr-23.4.0/setup.py
```

### Comparing `aiopyarr-22.9.0/LICENSE` & `aiopyarr-23.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopyarr-22.9.0/PKG-INFO` & `aiopyarr-23.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopyarr
-Version: 22.9.0
+Version: 23.4.0
 Summary: An Asynchronous Lidarr, Radarr, Readarr, Sonarr APIs for Python.
 Home-page: https://github.com/tkdrob/aiopyarr
 Author: Robert Hillis
 Author-email: tkdrob4390@yahoo.com
 License: MIT license
 Keywords: aiopyarr,radarr,sonarr,plex
 Classifier: Intended Audience :: Developers
```

### Comparing `aiopyarr-22.9.0/README.md` & `aiopyarr-23.4.0/README.md`

 * *Files identical despite different names*

### Comparing `aiopyarr-22.9.0/aiopyarr/const.py` & `aiopyarr-23.4.0/aiopyarr/const.py`

 * *Files identical despite different names*

### Comparing `aiopyarr-22.9.0/aiopyarr/exceptions.py` & `aiopyarr-23.4.0/aiopyarr/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiopyarr-22.9.0/aiopyarr/lidarr_client.py` & `aiopyarr-23.4.0/aiopyarr/lidarr_client.py`

 * *Files identical despite different names*

### Comparing `aiopyarr-22.9.0/aiopyarr/models/base.py` & `aiopyarr-23.4.0/aiopyarr/models/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """PyArr base model."""
 from __future__ import annotations
 
 from dataclasses import dataclass
 from datetime import date, datetime
 from enum import Enum
-from re import search
 from typing import Any
 
+import ciso8601
+
 from ..const import ATTR_DATA
 from .const import (
     CONVERT_TO_BOOL,
     CONVERT_TO_DATE,
     CONVERT_TO_DATETIME,
     CONVERT_TO_ENUM,
     CONVERT_TO_FLOAT,
@@ -22,29 +23,25 @@
 def get_datetime(
     _input: datetime | str | None, utc: bool = False
 ) -> datetime | str | int | None:
     """Convert input to datetime object."""
     if isinstance(_input, str):
         if _input.isnumeric():
             return int(_input)
-        if res := search(r"(\d+-\d{2}-\d{2})T?(\d{2}:\d{2}:\d{2})?\.*((.*)Z)?", _input):
-            if res.group(2):
-                _input = f"{res.group(1)}{res.group(2)}{f'{res.group(4)}000000'[:6]}"
-                if utc:
-                    return datetime.strptime(f"{_input}+00:00", "%Y-%m-%d%H:%M:%S%f%z")
-                return datetime.strptime(_input, "%Y-%m-%d%H:%M:%S%f")
-            return datetime.strptime(_input, "%Y-%m-%d")
+        if utc:
+            return ciso8601.parse_datetime(_input)
+        return ciso8601.parse_datetime_as_naive(_input)
     return _input
 
 
-def get_date(_input: datetime | str | None) -> date | str | int | None:
+def get_date(_input: datetime | str | None) -> date | None:
     """Convert input to date object."""
     if (result := get_datetime(_input)) and isinstance(result, datetime):
         return result.date()
-    return result
+    return None
 
 
 def get_enum_value(val: str) -> str | Enum:
     """Convert input to the correct enum."""
     for protocol in ProtocolType:
         if (
             val.isnumeric()
@@ -127,9 +124,9 @@
         return {
             k: v
             if isinstance(v, bool)
             else str(v)
             if k in CONVERT_TO_INTEGER
             else toraw(v)
             for k, v in self.__dict__.items()
-            if k != "basedata"
+            if k != ATTR_DATA
         }
```

### Comparing `aiopyarr-22.9.0/aiopyarr/models/const.py` & `aiopyarr-23.4.0/aiopyarr/models/const.py`

 * *Files identical despite different names*

### Comparing `aiopyarr-22.9.0/aiopyarr/models/host_configuration.py` & `aiopyarr-23.4.0/aiopyarr/models/host_configuration.py`

 * *Files identical despite different names*

### Comparing `aiopyarr-22.9.0/aiopyarr/models/lidarr.py` & `aiopyarr-23.4.0/aiopyarr/models/lidarr.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,14 +310,15 @@
     albumId: int
     artist: type[_LidarrArtist] = field(default=_LidarrArtist)
     artistId: int
     downloadForced: bool
 
     def __post_init__(self):
         """Post init."""
+        super().__post_init__()
         self.album = _LidarrQueueItemAlbum(self.album)
         self.artist = _LidarrArtist(self.artist)
         self.quality = _Quality(self.quality)
         self.statusMessages = [_StatusMessage(x) for x in self.statusMessages or []]
 
 
 @dataclass(init=False)
```

### Comparing `aiopyarr-22.9.0/aiopyarr/models/lidarr_common.py` & `aiopyarr-23.4.0/aiopyarr/models/lidarr_common.py`

 * *Files identical despite different names*

### Comparing `aiopyarr-22.9.0/aiopyarr/models/radarr.py` & `aiopyarr-23.4.0/aiopyarr/models/radarr.py`

 * *Files identical despite different names*

### Comparing `aiopyarr-22.9.0/aiopyarr/models/radarr_common.py` & `aiopyarr-23.4.0/aiopyarr/models/radarr_common.py`

 * *Files identical despite different names*

### Comparing `aiopyarr-22.9.0/aiopyarr/models/readarr.py` & `aiopyarr-23.4.0/aiopyarr/models/readarr.py`

 * *Files identical despite different names*

### Comparing `aiopyarr-22.9.0/aiopyarr/models/readarr_common.py` & `aiopyarr-23.4.0/aiopyarr/models/readarr_common.py`

 * *Files identical despite different names*

### Comparing `aiopyarr-22.9.0/aiopyarr/models/request.py` & `aiopyarr-23.4.0/aiopyarr/models/request.py`

 * *Files identical despite different names*

### Comparing `aiopyarr-22.9.0/aiopyarr/models/request_common.py` & `aiopyarr-23.4.0/aiopyarr/models/request_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 @dataclass(init=False)
 class _Common4(BaseModel):
     """Common attributes."""
 
     downloadClient: str
     downloadId: str
-    estimatedCompletionTime: datetime
+    estimatedCompletionTime: datetime | None = None
     indexer: str
     outputPath: str
 
 
 @dataclass(init=False)
 class _Common5(BaseModel):
     """Common attributes."""
@@ -149,19 +149,28 @@
     id: int
     protocol: ProtocolType
     quality: type[_Quality] = field(default=_Quality)
     size: int
     sizeleft: int
     status: str
     statusMessages: list[_StatusMessage] | None = None
-    timeleft: str
+    timeleft: str | None = None
     title: str
-    trackedDownloadState: str
+    trackedDownloadState: str = "downloading"
     trackedDownloadStatus: str
 
+    def __post_init__(self):
+        """Post init."""
+        if (
+            hasattr(self, "sizeleft")
+            and self.sizeleft > 0
+            and self.timeleft == "00:00:00"
+        ):
+            self.trackedDownloadState = "stopped"
+
 
 @dataclass(init=False)
 class _Common9(BaseModel):
     """Common attributes."""
 
     certification: str
     genres: list[str]
```

### Comparing `aiopyarr-22.9.0/aiopyarr/models/sonarr.py` & `aiopyarr-23.4.0/aiopyarr/models/sonarr.py`

 * *Files identical despite different names*

### Comparing `aiopyarr-22.9.0/aiopyarr/models/sonarr_common.py` & `aiopyarr-23.4.0/aiopyarr/models/sonarr_common.py`

 * *Files identical despite different names*

### Comparing `aiopyarr-22.9.0/aiopyarr/radarr_client.py` & `aiopyarr-23.4.0/aiopyarr/radarr_client.py`

 * *Files identical despite different names*

### Comparing `aiopyarr-22.9.0/aiopyarr/readarr_client.py` & `aiopyarr-23.4.0/aiopyarr/readarr_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,15 +380,15 @@
 
     async def async_lookup_book(
         self, term: str, booktype: ReadarrBookTypes = ReadarrBookTypes.ISBN
     ) -> list[ReadarrBookLookup]:
         """Search for new books using a term, goodreads ID, isbn or asin."""
         return await self._async_request(
             "book/lookup",
-            params={TERM: f"{booktype}:{term}"},
+            params={TERM: f"{booktype.value}:{term}"},
             datatype=ReadarrBookLookup,
         )
 
     async def async_add_bookshelf(
         self, data: ReadarrBookshelf
     ) -> ReadarrBookshelf:  # verify
         """Add a bookshelf to the database."""
```

### Comparing `aiopyarr-22.9.0/aiopyarr/request_client.py` & `aiopyarr-23.4.0/aiopyarr/request_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Shared API."""
 # pylint: disable=too-many-lines
 from __future__ import annotations
 
 import asyncio
 from copy import copy
 from re import search
-from typing import Any, Text
+from typing import Any
 
 from aiohttp.client import ClientError, ClientSession, ClientTimeout
+import orjson
 
 from .const import (
     ALL,
     ATTR_DATA,
     HEADERS,
     HEADERS_JS,
     IS_VALID,
@@ -151,22 +152,21 @@
         """Send API request."""
         url = self._host.api_url(command)
         try:
             request = await self._session.request(
                 method=method.value,
                 url=url,
                 params=params,
-                json=toraw(data),
+                data=orjson.dumps(toraw(data)),
                 headers=self._headers,
                 timeout=ClientTimeout(self._request_timeout),
                 ssl=self._host.verify_ssl,
             )
 
             if request.status >= 400:
-
                 if request.status == 401:
                     raise ArrAuthenticationException(self, request)
                 if request.status == 404:
                     raise ArrResourceNotFound(self, request)
                 raise ArrConnectionException(
                     self,
                     f"Request for '{url}' failed with status code '{request.status}'",
@@ -331,23 +331,23 @@
             f"command/{commandid}", method=HTTPMethod.DELETE
         )
 
     async def async_get_log_file(self) -> list[LogFile]:
         """Get log file."""
         return await self._async_request("log/file", datatype=LogFile)
 
-    async def async_get_log_file_content(self, file: str) -> Text:
+    async def async_get_log_file_content(self, file: str) -> str:
         """Get log file content."""
         return await self._async_request(f"log/file/{file}")
 
     async def async_get_log_file_updates(self) -> list[LogFile]:
         """Get log file updates."""
         return await self._async_request("log/file/update", datatype=LogFile)
 
-    async def async_get_log_file_update_content(self, file: str) -> Text:
+    async def async_get_log_file_update_content(self, file: str) -> str:
         """Get log file update content."""
         return await self._async_request(f"log/file/update/{file}")
 
     async def async_get_system_status(self) -> SystemStatus:
         """Get information about system status."""
         return await self._async_request("system/status", datatype=SystemStatus)
 
@@ -737,15 +737,15 @@
             _val = "album/" if alt else "artist/"
         elif hasattr(self, "async_get_authors"):
             _val = "author/" if alt else "book/"
         _imgsize = f"-{val}" if size is not ImageSize.LARGE else ""
         _imgsize = "" if hasattr(self, "async_get_albums") else _imgsize
 
         _ext = "png" if imagetype == ImageType.LOGO else "jpg"
-        cmd = f"mediacover/{_val}{imageid}/{imagetype}{_imgsize}.{_ext}"
+        cmd = f"mediacover/{_val}{imageid}/{imagetype.value}{_imgsize}.{_ext}"
         return await self._async_request(cmd)
 
     async def async_mark_failed(self, recordid: int) -> None:
         """Mark a history item as failed."""
         return await self._async_request(
             f"history/failed/{recordid}", method=HTTPMethod.POST
         )
```

### Comparing `aiopyarr-22.9.0/aiopyarr/sonarr_client.py` & `aiopyarr-23.4.0/aiopyarr/sonarr_client.py`

 * *Files identical despite different names*

### Comparing `aiopyarr-22.9.0/aiopyarr.egg-info/PKG-INFO` & `aiopyarr-23.4.0/aiopyarr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopyarr
-Version: 22.9.0
+Version: 23.4.0
 Summary: An Asynchronous Lidarr, Radarr, Readarr, Sonarr APIs for Python.
 Home-page: https://github.com/tkdrob/aiopyarr
 Author: Robert Hillis
 Author-email: tkdrob4390@yahoo.com
 License: MIT license
 Keywords: aiopyarr,radarr,sonarr,plex
 Classifier: Intended Audience :: Developers
```

### Comparing `aiopyarr-22.9.0/aiopyarr.egg-info/SOURCES.txt` & `aiopyarr-23.4.0/aiopyarr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiopyarr-22.9.0/setup.py` & `aiopyarr-23.4.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="aiopyarr",
-    version="22.9.0",
+    version="23.4.0",
     author="Robert Hillis",
     author_email="tkdrob4390@yahoo.com",
     description="An Asynchronous Lidarr, Radarr, Readarr, Sonarr APIs for Python.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/tkdrob/aiopyarr",
     package_data={"aiopyarr": ["py.typed"]},
```

