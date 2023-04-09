# Comparing `tmp/k-amino.py-1.1.1.tar.gz` & `tmp/k-amino.py-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k-amino.py-1.1.1.tar", last modified: Sun Apr  9 03:04:53 2023, max compression
+gzip compressed data, was "k-amino.py-1.1.2.tar", last modified: Sun Apr  9 11:22:10 2023, max compression
```

## Comparing `k-amino.py-1.1.1.tar` & `k-amino.py-1.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 03:04:53.905399 k-amino.py-1.1.1/
--rw-rw-rw-   0        0        0      586 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     2143 2023-04-09 03:04:53.906408 k-amino.py-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1596 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 03:04:53.798383 k-amino.py-1.1.1/k_amino/
--rw-rw-rw-   0        0        0      872 2023-04-09 02:59:46.000000 k-amino.py-1.1.1/k_amino/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 03:04:53.839376 k-amino.py-1.1.1/k_amino/k_async/
--rw-rw-rw-   0        0        0      122 2023-04-09 01:08:06.000000 k-amino.py-1.1.1/k_amino/k_async/__init__.py
--rw-rw-rw-   0        0        0     3922 2023-04-07 02:03:55.000000 k-amino.py-1.1.1/k_amino/k_async/acm.py
--rw-rw-rw-   0        0        0     1950 2023-04-07 03:16:23.000000 k-amino.py-1.1.1/k_amino/k_async/bot.py
--rw-rw-rw-   0        0        0    31693 2023-04-07 03:34:54.000000 k-amino.py-1.1.1/k_amino/k_async/client.py
--rw-rw-rw-   0        0        0    46342 2023-04-09 02:54:55.000000 k-amino.py-1.1.1/k_amino/k_async/local.py
--rw-rw-rw-   0        0        0    24649 2023-04-07 03:42:28.000000 k-amino.py-1.1.1/k_amino/k_async/sockets.py
-drwxrwxrwx   0        0        0        0 2023-04-09 03:04:53.855377 k-amino.py-1.1.1/k_amino/k_sync/
--rw-rw-rw-   0        0        0      102 2023-04-09 01:08:25.000000 k-amino.py-1.1.1/k_amino/k_sync/__init__.py
--rw-rw-rw-   0        0        0     3751 2023-04-07 01:34:38.000000 k-amino.py-1.1.1/k_amino/k_sync/acm.py
--rw-rw-rw-   0        0        0     1912 2023-04-09 01:12:28.000000 k-amino.py-1.1.1/k_amino/k_sync/bot.py
--rw-rw-rw-   0        0        0    30339 2023-04-07 01:34:43.000000 k-amino.py-1.1.1/k_amino/k_sync/client.py
--rw-rw-rw-   0        0        0    45202 2023-04-09 02:51:09.000000 k-amino.py-1.1.1/k_amino/k_sync/local.py
--rw-rw-rw-   0        0        0    23210 2023-04-09 01:13:33.000000 k-amino.py-1.1.1/k_amino/k_sync/sockets.py
-drwxrwxrwx   0        0        0        0 2023-04-09 03:04:53.872420 k-amino.py-1.1.1/k_amino/lib/
--rw-rw-rw-   0        0        0       95 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_amino/lib/__init__.py
--rw-rw-rw-   0        0        0     2803 2023-04-07 05:28:51.000000 k-amino.py-1.1.1/k_amino/lib/async_sessions.py
--rw-rw-rw-   0        0        0     8314 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_amino/lib/exception.py
--rw-rw-rw-   0        0        0     1986 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_amino/lib/headers.py
--rw-rw-rw-   0        0        0   198102 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_amino/lib/objects.py
--rw-rw-rw-   0        0        0     2422 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_amino/lib/sessions.py
--rw-rw-rw-   0        0        0     1244 2023-04-09 01:09:13.000000 k-amino.py-1.1.1/k_amino/lib/util.py
-drwxrwxrwx   0        0        0        0 2023-04-09 03:04:53.822385 k-amino.py-1.1.1/k_amino.py.egg-info/
--rw-rw-rw-   0        0        0     2143 2023-04-09 03:04:53.000000 k-amino.py-1.1.1/k_amino.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      926 2023-04-09 03:04:53.000000 k-amino.py-1.1.1/k_amino.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 03:04:53.000000 k-amino.py-1.1.1/k_amino.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2023-04-09 03:04:53.000000 k-amino.py-1.1.1/k_amino.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-09 03:04:53.000000 k-amino.py-1.1.1/k_amino.py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-09 03:04:53.888385 k-amino.py-1.1.1/k_asyncOld/
--rw-rw-rw-   0        0        0       79 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_asyncOld/__init__.py
--rw-rw-rw-   0        0        0     5940 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_asyncOld/acm.py
--rw-rw-rw-   0        0        0    40417 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_asyncOld/client.py
-drwxrwxrwx   0        0        0        0 2023-04-09 03:04:53.903376 k-amino.py-1.1.1/k_asyncOld/lib/
--rw-rw-rw-   0        0        0       95 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_asyncOld/lib/__init__.py
--rw-rw-rw-   0        0        0     8314 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_asyncOld/lib/exception.py
--rw-rw-rw-   0        0        0     1631 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_asyncOld/lib/headers.py
--rw-rw-rw-   0        0        0   198118 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_asyncOld/lib/objects.py
--rw-rw-rw-   0        0        0      768 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_asyncOld/lib/util.py
--rw-rw-rw-   0        0        0    55364 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_asyncOld/local.py
--rw-rw-rw-   0        0        0    24930 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_asyncOld/sockets.py
--rw-rw-rw-   0        0        0       42 2023-04-09 03:04:53.910426 k-amino.py-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1381 2023-04-09 02:57:52.000000 k-amino.py-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 11:22:10.468340 k-amino.py-1.1.2/
+-rw-rw-rw-   0        0        0      586 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2143 2023-04-09 11:22:10.468340 k-amino.py-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1596 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 11:22:10.347353 k-amino.py-1.1.2/k_amino/
+-rw-rw-rw-   0        0        0      872 2023-04-09 11:22:00.000000 k-amino.py-1.1.2/k_amino/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 11:22:10.390340 k-amino.py-1.1.2/k_amino/k_async/
+-rw-rw-rw-   0        0        0      122 2023-04-09 03:38:43.000000 k-amino.py-1.1.2/k_amino/k_async/__init__.py
+-rw-rw-rw-   0        0        0     3922 2023-04-07 02:03:55.000000 k-amino.py-1.1.2/k_amino/k_async/acm.py
+-rw-rw-rw-   0        0        0     1950 2023-04-07 03:16:23.000000 k-amino.py-1.1.2/k_amino/k_async/bot.py
+-rw-rw-rw-   0        0        0    31693 2023-04-07 03:34:54.000000 k-amino.py-1.1.2/k_amino/k_async/client.py
+-rw-rw-rw-   0        0        0    46342 2023-04-09 02:54:55.000000 k-amino.py-1.1.2/k_amino/k_async/local.py
+-rw-rw-rw-   0        0        0    24690 2023-04-09 11:21:26.000000 k-amino.py-1.1.2/k_amino/k_async/sockets.py
+drwxrwxrwx   0        0        0        0 2023-04-09 11:22:10.409341 k-amino.py-1.1.2/k_amino/k_sync/
+-rw-rw-rw-   0        0        0      102 2023-04-09 01:08:25.000000 k-amino.py-1.1.2/k_amino/k_sync/__init__.py
+-rw-rw-rw-   0        0        0     3751 2023-04-07 01:34:38.000000 k-amino.py-1.1.2/k_amino/k_sync/acm.py
+-rw-rw-rw-   0        0        0     1912 2023-04-09 01:12:28.000000 k-amino.py-1.1.2/k_amino/k_sync/bot.py
+-rw-rw-rw-   0        0        0    30339 2023-04-07 01:34:43.000000 k-amino.py-1.1.2/k_amino/k_sync/client.py
+-rw-rw-rw-   0        0        0    45202 2023-04-09 02:51:09.000000 k-amino.py-1.1.2/k_amino/k_sync/local.py
+-rw-rw-rw-   0        0        0    23210 2023-04-09 01:13:33.000000 k-amino.py-1.1.2/k_amino/k_sync/sockets.py
+drwxrwxrwx   0        0        0        0 2023-04-09 11:22:10.431340 k-amino.py-1.1.2/k_amino/lib/
+-rw-rw-rw-   0        0        0       95 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_amino/lib/__init__.py
+-rw-rw-rw-   0        0        0     2803 2023-04-07 05:28:51.000000 k-amino.py-1.1.2/k_amino/lib/async_sessions.py
+-rw-rw-rw-   0        0        0     8314 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_amino/lib/exception.py
+-rw-rw-rw-   0        0        0     1986 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_amino/lib/headers.py
+-rw-rw-rw-   0        0        0   198102 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_amino/lib/objects.py
+-rw-rw-rw-   0        0        0     2422 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_amino/lib/sessions.py
+-rw-rw-rw-   0        0        0     1688 2023-04-09 07:16:48.000000 k-amino.py-1.1.2/k_amino/lib/util.py
+drwxrwxrwx   0        0        0        0 2023-04-09 11:22:10.370341 k-amino.py-1.1.2/k_amino.py.egg-info/
+-rw-rw-rw-   0        0        0     2143 2023-04-09 11:22:09.000000 k-amino.py-1.1.2/k_amino.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      926 2023-04-09 11:22:10.000000 k-amino.py-1.1.2/k_amino.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 11:22:09.000000 k-amino.py-1.1.2/k_amino.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-04-09 11:22:09.000000 k-amino.py-1.1.2/k_amino.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-09 11:22:09.000000 k-amino.py-1.1.2/k_amino.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 11:22:10.447341 k-amino.py-1.1.2/k_asyncOld/
+-rw-rw-rw-   0        0        0       79 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_asyncOld/__init__.py
+-rw-rw-rw-   0        0        0     5940 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_asyncOld/acm.py
+-rw-rw-rw-   0        0        0    40417 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_asyncOld/client.py
+drwxrwxrwx   0        0        0        0 2023-04-09 11:22:10.465344 k-amino.py-1.1.2/k_asyncOld/lib/
+-rw-rw-rw-   0        0        0       95 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_asyncOld/lib/__init__.py
+-rw-rw-rw-   0        0        0     8314 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_asyncOld/lib/exception.py
+-rw-rw-rw-   0        0        0     1631 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_asyncOld/lib/headers.py
+-rw-rw-rw-   0        0        0   198118 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_asyncOld/lib/objects.py
+-rw-rw-rw-   0        0        0      768 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_asyncOld/lib/util.py
+-rw-rw-rw-   0        0        0    55364 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_asyncOld/local.py
+-rw-rw-rw-   0        0        0    24930 2023-03-17 22:23:53.000000 k-amino.py-1.1.2/k_asyncOld/sockets.py
+-rw-rw-rw-   0        0        0       42 2023-04-09 11:22:10.473342 k-amino.py-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1381 2023-04-09 02:57:52.000000 k-amino.py-1.1.2/setup.py
```

### Comparing `k-amino.py-1.1.1/LICENSE` & `k-amino.py-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/PKG-INFO` & `k-amino.py-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k-amino.py
-Version: 1.1.1
+Version: 1.1.2
 Summary: Amino Bots with python!
 Home-page: https://github.com/kwel999/KAmino
 Download-URL: https://github.com/kwel999/KAmino/archive/refs/heads/main.zip
 Author: KWEL
 Author-email: itskwel999@gmail.com
 License: Apache
 Keywords: api,python,python3,python3.x,KWEL,kwel999,kwel.py,Amino,kamino,kamino pyK-Amino,kamino,kamino,kamino-bot,kamino-bots,kamino-bot,ndc,narvii.apps,aminoapps,kamino-py,kamino,kamino-bot,narvii
```

### Comparing `k-amino.py-1.1.1/README.md` & `k-amino.py-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_amino/__init__.py` & `k-amino.py-1.1.2/k_amino/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .k_async.acm import AsyncAcm
 from .k_async.client import AsyncClient
 from .k_async.local import AsyncSubClient
 # from .k_async.sockets import *
 from .k_async.bot import AsyncBot
 
 
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 
 __newest__ = loads(get("https://pypi.python.org/pypi/k-amino.py/json").text)["info"]["version"]
 
 if __version__ != __newest__:
     print(f"\033[1;31;38mk_amino New Version!: {__newest__} (You are using {__version__})\033[1;36;33m\nDiscord server: \"https://discord.gg/zd8gyFJquT\"\033[1;0m")
 else:
```

### Comparing `k-amino.py-1.1.1/k_amino/k_async/acm.py` & `k-amino.py-1.1.2/k_amino/k_async/acm.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_amino/k_async/bot.py` & `k-amino.py-1.1.2/k_amino/k_async/bot.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_amino/k_async/client.py` & `k-amino.py-1.1.2/k_amino/k_async/client.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_amino/k_async/local.py` & `k-amino.py-1.1.2/k_amino/k_async/local.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_amino/k_async/sockets.py` & `k-amino.py-1.1.2/k_amino/k_async/sockets.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,19 @@
 import asyncio
 
 from ..lib import *
 from ..lib.objects import *
 from .bot import AsyncBot as Bot
 from easy_events import AsyncEvents
 
-asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+try:
+    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+except Exception:
+    pass
+
 
 class AsyncCallbacks(Bot):
     def __init__(self, is_bot: bool = False, prefix: str = "!"):
         Bot.__init__(self, prefix=prefix)
 
         # if the user want to use the script as a bot
         self.is_bot = is_bot
```

### Comparing `k-amino.py-1.1.1/k_amino/k_sync/acm.py` & `k-amino.py-1.1.2/k_amino/k_sync/acm.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_amino/k_sync/bot.py` & `k-amino.py-1.1.2/k_amino/k_sync/bot.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_amino/k_sync/client.py` & `k-amino.py-1.1.2/k_amino/k_sync/client.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_amino/k_sync/local.py` & `k-amino.py-1.1.2/k_amino/k_sync/local.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_amino/k_sync/sockets.py` & `k-amino.py-1.1.2/k_amino/k_sync/sockets.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_amino/lib/async_sessions.py` & `k-amino.py-1.1.2/k_amino/lib/async_sessions.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_amino/lib/exception.py` & `k-amino.py-1.1.2/k_amino/lib/exception.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_amino/lib/headers.py` & `k-amino.py-1.1.2/k_amino/lib/headers.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_amino/lib/objects.py` & `k-amino.py-1.1.2/k_amino/lib/objects.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_amino/lib/sessions.py` & `k-amino.py-1.1.2/k_amino/lib/sessions.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_amino/lib/util.py` & `k-amino.py-1.1.2/k_amino/lib/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from base64 import b64encode, urlsafe_b64decode
 from time import time as timestamp
 from typing import Dict, List
 import base64
 import hashlib
 import hmac
 from uuid import uuid4
 
@@ -40,7 +41,19 @@
         } for _ in range(total // 300)
     ] + [
         {
             'start': int(timestamp()),
             'end': int(timestamp() + total % 300)
         }
     ]
+
+
+def decode_sid(sid: str) -> dict:
+    return json.loads(urlsafe_b64decode(sid + "=" * (4 - len(sid) % 4))[1:-20])
+
+def sid_to_uid(SID: str) -> str: return decode_sid(SID)["2"]
+
+def sid_to_ip_address(SID: str) -> str: return decode_sid(SID)["4"]
+
+def sid_created_time(SID: str) -> str: return decode_sid(SID)["5"]
+
+def sid_to_client_type(SID: str) -> str: return decode_sid(SID)["6"]
```

### Comparing `k-amino.py-1.1.1/k_amino.py.egg-info/PKG-INFO` & `k-amino.py-1.1.2/k_amino.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k-amino.py
-Version: 1.1.1
+Version: 1.1.2
 Summary: Amino Bots with python!
 Home-page: https://github.com/kwel999/KAmino
 Download-URL: https://github.com/kwel999/KAmino/archive/refs/heads/main.zip
 Author: KWEL
 Author-email: itskwel999@gmail.com
 License: Apache
 Keywords: api,python,python3,python3.x,KWEL,kwel999,kwel.py,Amino,kamino,kamino pyK-Amino,kamino,kamino,kamino-bot,kamino-bots,kamino-bot,ndc,narvii.apps,aminoapps,kamino-py,kamino,kamino-bot,narvii
```

### Comparing `k-amino.py-1.1.1/k_amino.py.egg-info/SOURCES.txt` & `k-amino.py-1.1.2/k_amino.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_asyncOld/acm.py` & `k-amino.py-1.1.2/k_asyncOld/acm.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_asyncOld/client.py` & `k-amino.py-1.1.2/k_asyncOld/client.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_asyncOld/lib/exception.py` & `k-amino.py-1.1.2/k_asyncOld/lib/exception.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_asyncOld/lib/headers.py` & `k-amino.py-1.1.2/k_asyncOld/lib/headers.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_asyncOld/lib/objects.py` & `k-amino.py-1.1.2/k_asyncOld/lib/objects.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_asyncOld/lib/util.py` & `k-amino.py-1.1.2/k_asyncOld/lib/util.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_asyncOld/local.py` & `k-amino.py-1.1.2/k_asyncOld/local.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/k_asyncOld/sockets.py` & `k-amino.py-1.1.2/k_asyncOld/sockets.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.1/setup.py` & `k-amino.py-1.1.2/setup.py`

 * *Files identical despite different names*

