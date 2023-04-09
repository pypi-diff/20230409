# Comparing `tmp/k-amino.py-1.1.0.tar.gz` & `tmp/k-amino.py-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k-amino.py-1.1.0.tar", last modified: Sun Apr  9 01:21:22 2023, max compression
+gzip compressed data, was "k-amino.py-1.1.1.tar", last modified: Sun Apr  9 03:04:53 2023, max compression
```

## Comparing `k-amino.py-1.1.0.tar` & `k-amino.py-1.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 01:21:22.345925 k-amino.py-1.1.0/
--rw-rw-rw-   0        0        0      586 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     2143 2023-04-09 01:21:22.346931 k-amino.py-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1596 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 01:21:22.243178 k-amino.py-1.1.0/k_amino/
--rw-rw-rw-   0        0        0      872 2023-04-09 01:09:36.000000 k-amino.py-1.1.0/k_amino/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 01:21:22.278179 k-amino.py-1.1.0/k_amino/k_async/
--rw-rw-rw-   0        0        0      122 2023-04-09 01:08:06.000000 k-amino.py-1.1.0/k_amino/k_async/__init__.py
--rw-rw-rw-   0        0        0     3922 2023-04-07 02:03:55.000000 k-amino.py-1.1.0/k_amino/k_async/acm.py
--rw-rw-rw-   0        0        0     1950 2023-04-07 03:16:23.000000 k-amino.py-1.1.0/k_amino/k_async/bot.py
--rw-rw-rw-   0        0        0    31693 2023-04-07 03:34:54.000000 k-amino.py-1.1.0/k_amino/k_async/client.py
--rw-rw-rw-   0        0        0    46342 2023-04-07 02:21:35.000000 k-amino.py-1.1.0/k_amino/k_async/local.py
--rw-rw-rw-   0        0        0    24649 2023-04-07 03:42:28.000000 k-amino.py-1.1.0/k_amino/k_async/sockets.py
-drwxrwxrwx   0        0        0        0 2023-04-09 01:21:22.295180 k-amino.py-1.1.0/k_amino/k_sync/
--rw-rw-rw-   0        0        0      102 2023-04-09 01:08:25.000000 k-amino.py-1.1.0/k_amino/k_sync/__init__.py
--rw-rw-rw-   0        0        0     3751 2023-04-07 01:34:38.000000 k-amino.py-1.1.0/k_amino/k_sync/acm.py
--rw-rw-rw-   0        0        0     1912 2023-04-09 01:12:28.000000 k-amino.py-1.1.0/k_amino/k_sync/bot.py
--rw-rw-rw-   0        0        0    30339 2023-04-07 01:34:43.000000 k-amino.py-1.1.0/k_amino/k_sync/client.py
--rw-rw-rw-   0        0        0    45169 2023-04-07 01:37:06.000000 k-amino.py-1.1.0/k_amino/k_sync/local.py
--rw-rw-rw-   0        0        0    23210 2023-04-09 01:13:33.000000 k-amino.py-1.1.0/k_amino/k_sync/sockets.py
-drwxrwxrwx   0        0        0        0 2023-04-09 01:21:22.311192 k-amino.py-1.1.0/k_amino/lib/
--rw-rw-rw-   0        0        0       95 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_amino/lib/__init__.py
--rw-rw-rw-   0        0        0     2803 2023-04-07 05:28:51.000000 k-amino.py-1.1.0/k_amino/lib/async_sessions.py
--rw-rw-rw-   0        0        0     8314 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_amino/lib/exception.py
--rw-rw-rw-   0        0        0     1986 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_amino/lib/headers.py
--rw-rw-rw-   0        0        0   198102 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_amino/lib/objects.py
--rw-rw-rw-   0        0        0     2422 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_amino/lib/sessions.py
--rw-rw-rw-   0        0        0     1244 2023-04-09 01:09:13.000000 k-amino.py-1.1.0/k_amino/lib/util.py
-drwxrwxrwx   0        0        0        0 2023-04-09 01:21:22.264180 k-amino.py-1.1.0/k_amino.py.egg-info/
--rw-rw-rw-   0        0        0     2143 2023-04-09 01:21:21.000000 k-amino.py-1.1.0/k_amino.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      926 2023-04-09 01:21:22.000000 k-amino.py-1.1.0/k_amino.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 01:21:21.000000 k-amino.py-1.1.0/k_amino.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-04-09 01:21:21.000000 k-amino.py-1.1.0/k_amino.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-09 01:21:21.000000 k-amino.py-1.1.0/k_amino.py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-09 01:21:22.328926 k-amino.py-1.1.0/k_asyncOld/
--rw-rw-rw-   0        0        0       79 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_asyncOld/__init__.py
--rw-rw-rw-   0        0        0     5940 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_asyncOld/acm.py
--rw-rw-rw-   0        0        0    40417 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_asyncOld/client.py
-drwxrwxrwx   0        0        0        0 2023-04-09 01:21:22.342913 k-amino.py-1.1.0/k_asyncOld/lib/
--rw-rw-rw-   0        0        0       95 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_asyncOld/lib/__init__.py
--rw-rw-rw-   0        0        0     8314 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_asyncOld/lib/exception.py
--rw-rw-rw-   0        0        0     1631 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_asyncOld/lib/headers.py
--rw-rw-rw-   0        0        0   198118 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_asyncOld/lib/objects.py
--rw-rw-rw-   0        0        0      768 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_asyncOld/lib/util.py
--rw-rw-rw-   0        0        0    55364 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_asyncOld/local.py
--rw-rw-rw-   0        0        0    24930 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_asyncOld/sockets.py
--rw-rw-rw-   0        0        0       42 2023-04-09 01:21:22.350917 k-amino.py-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1363 2023-04-07 01:13:01.000000 k-amino.py-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:53.905399 k-amino.py-1.1.1/
+-rw-rw-rw-   0        0        0      586 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2143 2023-04-09 03:04:53.906408 k-amino.py-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1596 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:53.798383 k-amino.py-1.1.1/k_amino/
+-rw-rw-rw-   0        0        0      872 2023-04-09 02:59:46.000000 k-amino.py-1.1.1/k_amino/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:53.839376 k-amino.py-1.1.1/k_amino/k_async/
+-rw-rw-rw-   0        0        0      122 2023-04-09 01:08:06.000000 k-amino.py-1.1.1/k_amino/k_async/__init__.py
+-rw-rw-rw-   0        0        0     3922 2023-04-07 02:03:55.000000 k-amino.py-1.1.1/k_amino/k_async/acm.py
+-rw-rw-rw-   0        0        0     1950 2023-04-07 03:16:23.000000 k-amino.py-1.1.1/k_amino/k_async/bot.py
+-rw-rw-rw-   0        0        0    31693 2023-04-07 03:34:54.000000 k-amino.py-1.1.1/k_amino/k_async/client.py
+-rw-rw-rw-   0        0        0    46342 2023-04-09 02:54:55.000000 k-amino.py-1.1.1/k_amino/k_async/local.py
+-rw-rw-rw-   0        0        0    24649 2023-04-07 03:42:28.000000 k-amino.py-1.1.1/k_amino/k_async/sockets.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:53.855377 k-amino.py-1.1.1/k_amino/k_sync/
+-rw-rw-rw-   0        0        0      102 2023-04-09 01:08:25.000000 k-amino.py-1.1.1/k_amino/k_sync/__init__.py
+-rw-rw-rw-   0        0        0     3751 2023-04-07 01:34:38.000000 k-amino.py-1.1.1/k_amino/k_sync/acm.py
+-rw-rw-rw-   0        0        0     1912 2023-04-09 01:12:28.000000 k-amino.py-1.1.1/k_amino/k_sync/bot.py
+-rw-rw-rw-   0        0        0    30339 2023-04-07 01:34:43.000000 k-amino.py-1.1.1/k_amino/k_sync/client.py
+-rw-rw-rw-   0        0        0    45202 2023-04-09 02:51:09.000000 k-amino.py-1.1.1/k_amino/k_sync/local.py
+-rw-rw-rw-   0        0        0    23210 2023-04-09 01:13:33.000000 k-amino.py-1.1.1/k_amino/k_sync/sockets.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:53.872420 k-amino.py-1.1.1/k_amino/lib/
+-rw-rw-rw-   0        0        0       95 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_amino/lib/__init__.py
+-rw-rw-rw-   0        0        0     2803 2023-04-07 05:28:51.000000 k-amino.py-1.1.1/k_amino/lib/async_sessions.py
+-rw-rw-rw-   0        0        0     8314 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_amino/lib/exception.py
+-rw-rw-rw-   0        0        0     1986 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_amino/lib/headers.py
+-rw-rw-rw-   0        0        0   198102 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_amino/lib/objects.py
+-rw-rw-rw-   0        0        0     2422 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_amino/lib/sessions.py
+-rw-rw-rw-   0        0        0     1244 2023-04-09 01:09:13.000000 k-amino.py-1.1.1/k_amino/lib/util.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:53.822385 k-amino.py-1.1.1/k_amino.py.egg-info/
+-rw-rw-rw-   0        0        0     2143 2023-04-09 03:04:53.000000 k-amino.py-1.1.1/k_amino.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      926 2023-04-09 03:04:53.000000 k-amino.py-1.1.1/k_amino.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 03:04:53.000000 k-amino.py-1.1.1/k_amino.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2023-04-09 03:04:53.000000 k-amino.py-1.1.1/k_amino.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-09 03:04:53.000000 k-amino.py-1.1.1/k_amino.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:53.888385 k-amino.py-1.1.1/k_asyncOld/
+-rw-rw-rw-   0        0        0       79 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_asyncOld/__init__.py
+-rw-rw-rw-   0        0        0     5940 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_asyncOld/acm.py
+-rw-rw-rw-   0        0        0    40417 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_asyncOld/client.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:04:53.903376 k-amino.py-1.1.1/k_asyncOld/lib/
+-rw-rw-rw-   0        0        0       95 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_asyncOld/lib/__init__.py
+-rw-rw-rw-   0        0        0     8314 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_asyncOld/lib/exception.py
+-rw-rw-rw-   0        0        0     1631 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_asyncOld/lib/headers.py
+-rw-rw-rw-   0        0        0   198118 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_asyncOld/lib/objects.py
+-rw-rw-rw-   0        0        0      768 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_asyncOld/lib/util.py
+-rw-rw-rw-   0        0        0    55364 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_asyncOld/local.py
+-rw-rw-rw-   0        0        0    24930 2023-03-17 22:23:53.000000 k-amino.py-1.1.1/k_asyncOld/sockets.py
+-rw-rw-rw-   0        0        0       42 2023-04-09 03:04:53.910426 k-amino.py-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1381 2023-04-09 02:57:52.000000 k-amino.py-1.1.1/setup.py
```

### Comparing `k-amino.py-1.1.0/LICENSE` & `k-amino.py-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/PKG-INFO` & `k-amino.py-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k-amino.py
-Version: 1.1.0
+Version: 1.1.1
 Summary: Amino Bots with python!
 Home-page: https://github.com/kwel999/KAmino
 Download-URL: https://github.com/kwel999/KAmino/archive/refs/heads/main.zip
 Author: KWEL
 Author-email: itskwel999@gmail.com
 License: Apache
 Keywords: api,python,python3,python3.x,KWEL,kwel999,kwel.py,Amino,kamino,kamino pyK-Amino,kamino,kamino,kamino-bot,kamino-bots,kamino-bot,ndc,narvii.apps,aminoapps,kamino-py,kamino,kamino-bot,narvii
```

### Comparing `k-amino.py-1.1.0/README.md` & `k-amino.py-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_amino/__init__.py` & `k-amino.py-1.1.1/k_amino/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .k_async.acm import AsyncAcm
 from .k_async.client import AsyncClient
 from .k_async.local import AsyncSubClient
 # from .k_async.sockets import *
 from .k_async.bot import AsyncBot
 
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 
 __newest__ = loads(get("https://pypi.python.org/pypi/k-amino.py/json").text)["info"]["version"]
 
 if __version__ != __newest__:
     print(f"\033[1;31;38mk_amino New Version!: {__newest__} (You are using {__version__})\033[1;36;33m\nDiscord server: \"https://discord.gg/zd8gyFJquT\"\033[1;0m")
 else:
```

### Comparing `k-amino.py-1.1.0/k_amino/k_async/acm.py` & `k-amino.py-1.1.1/k_amino/k_async/acm.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_amino/k_async/bot.py` & `k-amino.py-1.1.1/k_amino/k_async/bot.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_amino/k_async/client.py` & `k-amino.py-1.1.1/k_amino/k_async/client.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_amino/k_async/local.py` & `k-amino.py-1.1.1/k_amino/k_async/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -1120,15 +1120,15 @@
             raise TypeError("choose a certain type to report")
 
         req = await self.postRequest(f"/x{self.comId}/s/flag", data)
         return Json(req)
 
     async def send_active_time(self, tz: int = int(-timezones // 1000), timers: list = None):
         data = {
-            "userActiveTimeChunkList": [timers if timers else {"start": int(timestamp()), "end": int(timestamp() + 300)}],
+            "userActiveTimeChunkList": timers if timers else [{"start": int(timestamp()), "end": int(timestamp() + 300)}],
             "timestamp": int(timestamp() * 1000),
             "optInAdsFlags": 2147483647,
             "timezone": tz,
         }
 
         req = await self.postRequest(
             f"/x{self.comId}/s/community/stats/user-active-time", data, minify=True
```

### Comparing `k-amino.py-1.1.0/k_amino/k_async/sockets.py` & `k-amino.py-1.1.1/k_amino/k_async/sockets.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_amino/k_sync/acm.py` & `k-amino.py-1.1.1/k_amino/k_sync/acm.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_amino/k_sync/bot.py` & `k-amino.py-1.1.1/k_amino/k_sync/bot.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_amino/k_sync/client.py` & `k-amino.py-1.1.1/k_amino/k_sync/client.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_amino/k_sync/local.py` & `k-amino.py-1.1.1/k_amino/k_sync/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -1117,18 +1117,18 @@
             data["objectId"] = wikiId
             data["objectType"] = 2
         else:
             raise TypeError("choose a certain type to report")
 
         req = self.postRequest(f"/x{self.comId}/s/flag", data)
         return Json(req)
-
+#thanks to V¡ktor#9475 for ideas
     def send_active_time(self, tz: int = int(-timezones // 1000), timers: list = None):
         data = {
-            "userActiveTimeChunkList": [timers if timers else {"start": int(timestamp()), "end": int(timestamp() + 300)}],
+            "userActiveTimeChunkList": timers if timers else [{"start": int(timestamp()), "end": int(timestamp() + 300)}],
             "timestamp": int(timestamp() * 1000),
             "optInAdsFlags": 2147483647,
             "timezone": tz,
         }
 
         req = self.postRequest(
             f"/x{self.comId}/s/community/stats/user-active-time", data, minify=True
```

### Comparing `k-amino.py-1.1.0/k_amino/k_sync/sockets.py` & `k-amino.py-1.1.1/k_amino/k_sync/sockets.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_amino/lib/async_sessions.py` & `k-amino.py-1.1.1/k_amino/lib/async_sessions.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_amino/lib/exception.py` & `k-amino.py-1.1.1/k_amino/lib/exception.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_amino/lib/headers.py` & `k-amino.py-1.1.1/k_amino/lib/headers.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_amino/lib/objects.py` & `k-amino.py-1.1.1/k_amino/lib/objects.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_amino/lib/sessions.py` & `k-amino.py-1.1.1/k_amino/lib/sessions.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_amino/lib/util.py` & `k-amino.py-1.1.1/k_amino/lib/util.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_amino.py.egg-info/PKG-INFO` & `k-amino.py-1.1.1/k_amino.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k-amino.py
-Version: 1.1.0
+Version: 1.1.1
 Summary: Amino Bots with python!
 Home-page: https://github.com/kwel999/KAmino
 Download-URL: https://github.com/kwel999/KAmino/archive/refs/heads/main.zip
 Author: KWEL
 Author-email: itskwel999@gmail.com
 License: Apache
 Keywords: api,python,python3,python3.x,KWEL,kwel999,kwel.py,Amino,kamino,kamino pyK-Amino,kamino,kamino,kamino-bot,kamino-bots,kamino-bot,ndc,narvii.apps,aminoapps,kamino-py,kamino,kamino-bot,narvii
```

### Comparing `k-amino.py-1.1.0/k_amino.py.egg-info/SOURCES.txt` & `k-amino.py-1.1.1/k_amino.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_asyncOld/acm.py` & `k-amino.py-1.1.1/k_asyncOld/acm.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_asyncOld/client.py` & `k-amino.py-1.1.1/k_asyncOld/client.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_asyncOld/lib/exception.py` & `k-amino.py-1.1.1/k_asyncOld/lib/exception.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_asyncOld/lib/headers.py` & `k-amino.py-1.1.1/k_asyncOld/lib/headers.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_asyncOld/lib/objects.py` & `k-amino.py-1.1.1/k_asyncOld/lib/objects.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_asyncOld/lib/util.py` & `k-amino.py-1.1.1/k_asyncOld/lib/util.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_asyncOld/local.py` & `k-amino.py-1.1.1/k_asyncOld/local.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/k_asyncOld/sockets.py` & `k-amino.py-1.1.1/k_asyncOld/sockets.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.1.0/setup.py` & `k-amino.py-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         "kamino",
         "kamino-bot",
         "narvii",
     ],
     include_package_data=True,
     install_requires=[
         "JSON_minify",
+        "httpx",
         "setuptools",
         "aiohttp",
         "websocket-client==1.3.1",
         "websockets",
         "ujson",
         "requests",
         "easy-events==2.8.2"
```

