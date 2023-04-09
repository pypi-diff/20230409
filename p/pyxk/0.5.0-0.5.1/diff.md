# Comparing `tmp/pyxk-0.5.0.tar.gz` & `tmp/pyxk-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxk-0.5.0.tar", last modified: Sun Apr  9 02:21:25 2023, max compression
+gzip compressed data, was "pyxk-0.5.1.tar", last modified: Sun Apr  9 12:40:04 2023, max compression
```

## Comparing `pyxk-0.5.0.tar` & `pyxk-0.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 02:21:25.194990 pyxk-0.5.0/
--rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.5.0/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)      343 2023-04-09 02:21:25.194990 pyxk-0.5.0/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.5.0/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 02:21:25.184990 pyxk-0.5.0/pyxk/
--rw-rw----   0 root         (0) everybody  (9997)      702 2023-04-08 12:07:19.000000 pyxk-0.5.0/pyxk/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    10882 2023-04-08 18:09:14.000000 pyxk-0.5.0/pyxk/aclient.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 02:21:25.194990 pyxk-0.5.0/pyxk/aes/
--rw-rw----   0 root         (0) everybody  (9997)       79 2023-02-24 04:10:40.000000 pyxk-0.5.0/pyxk/aes/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3639 2023-04-06 15:25:24.000000 pyxk-0.5.0/pyxk/aes/_fmtdata.py
--rw-rw----   0 root         (0) everybody  (9997)     4701 2023-04-06 15:27:39.000000 pyxk-0.5.0/pyxk/aes/cryptor.py
--rw-rw----   0 root         (0) everybody  (9997)      954 2023-03-15 06:04:12.000000 pyxk-0.5.0/pyxk/lazy_loader.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 02:21:25.194990 pyxk-0.5.0/pyxk/m3u8/
--rw-rw----   0 root         (0) everybody  (9997)       82 2023-03-16 14:08:36.000000 pyxk-0.5.0/pyxk/m3u8/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     8292 2023-03-16 12:13:38.000000 pyxk-0.5.0/pyxk/m3u8/_download.py
--rw-rw----   0 root         (0) everybody  (9997)     3199 2023-03-16 16:35:49.000000 pyxk-0.5.0/pyxk/m3u8/_entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)     7791 2023-03-16 16:35:32.000000 pyxk-0.5.0/pyxk/m3u8/_m3u8.py
--rw-rw----   0 root         (0) everybody  (9997)     4504 2023-03-17 04:00:18.000000 pyxk-0.5.0/pyxk/m3u8/_parser.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 02:21:25.194990 pyxk-0.5.0/pyxk/requests/
--rw-rw----   0 root         (0) everybody  (9997)      235 2023-04-06 15:53:39.000000 pyxk-0.5.0/pyxk/requests/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     5598 2023-04-06 16:07:00.000000 pyxk-0.5.0/pyxk/requests/_entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)     7514 2023-03-31 10:17:41.000000 pyxk-0.5.0/pyxk/requests/api.py
--rw-rw----   0 root         (0) everybody  (9997)    21859 2023-04-06 15:20:21.000000 pyxk-0.5.0/pyxk/requests/sessions.py
--rw-rw----   0 root         (0) everybody  (9997)    12202 2023-04-06 16:00:37.000000 pyxk-0.5.0/pyxk/utils.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 02:21:25.184990 pyxk-0.5.0/pyxk.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      343 2023-04-09 02:21:25.000000 pyxk-0.5.0/pyxk.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      539 2023-04-09 02:21:25.000000 pyxk-0.5.0/pyxk.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-09 02:21:25.000000 pyxk-0.5.0/pyxk.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       91 2023-04-09 02:21:25.000000 pyxk-0.5.0/pyxk.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       55 2023-04-09 02:21:25.000000 pyxk-0.5.0/pyxk.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        5 2023-04-09 02:21:25.000000 pyxk-0.5.0/pyxk.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-09 02:21:25.194990 pyxk-0.5.0/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      916 2023-04-09 02:20:57.000000 pyxk-0.5.0/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 12:40:04.368316 pyxk-0.5.1/
+-rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.5.1/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)      343 2023-04-09 12:40:04.368316 pyxk-0.5.1/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.5.1/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 12:40:04.358316 pyxk-0.5.1/pyxk/
+-rw-rw----   0 root         (0) everybody  (9997)      701 2023-04-09 12:39:02.000000 pyxk-0.5.1/pyxk/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    11004 2023-04-09 12:38:52.000000 pyxk-0.5.1/pyxk/aclient.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 12:40:04.358316 pyxk-0.5.1/pyxk/aes/
+-rw-rw----   0 root         (0) everybody  (9997)       79 2023-02-24 04:10:40.000000 pyxk-0.5.1/pyxk/aes/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3639 2023-04-06 15:25:24.000000 pyxk-0.5.1/pyxk/aes/_fmtdata.py
+-rw-rw----   0 root         (0) everybody  (9997)     4701 2023-04-06 15:27:39.000000 pyxk-0.5.1/pyxk/aes/cryptor.py
+-rw-rw----   0 root         (0) everybody  (9997)      954 2023-03-15 06:04:12.000000 pyxk-0.5.1/pyxk/lazy_loader.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 12:40:04.358316 pyxk-0.5.1/pyxk/m3u8/
+-rw-rw----   0 root         (0) everybody  (9997)       82 2023-03-16 14:08:36.000000 pyxk-0.5.1/pyxk/m3u8/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     8292 2023-03-16 12:13:38.000000 pyxk-0.5.1/pyxk/m3u8/_download.py
+-rw-rw----   0 root         (0) everybody  (9997)     3199 2023-03-16 16:35:49.000000 pyxk-0.5.1/pyxk/m3u8/_entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)     7791 2023-03-16 16:35:32.000000 pyxk-0.5.1/pyxk/m3u8/_m3u8.py
+-rw-rw----   0 root         (0) everybody  (9997)     4504 2023-03-17 04:00:18.000000 pyxk-0.5.1/pyxk/m3u8/_parser.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 12:40:04.368316 pyxk-0.5.1/pyxk/requests/
+-rw-rw----   0 root         (0) everybody  (9997)      235 2023-04-06 15:53:39.000000 pyxk-0.5.1/pyxk/requests/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     5598 2023-04-06 16:07:00.000000 pyxk-0.5.1/pyxk/requests/_entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)     7514 2023-03-31 10:17:41.000000 pyxk-0.5.1/pyxk/requests/api.py
+-rw-rw----   0 root         (0) everybody  (9997)    21859 2023-04-06 15:20:21.000000 pyxk-0.5.1/pyxk/requests/sessions.py
+-rw-rw----   0 root         (0) everybody  (9997)    12202 2023-04-06 16:00:37.000000 pyxk-0.5.1/pyxk/utils.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 12:40:04.358316 pyxk-0.5.1/pyxk.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      343 2023-04-09 12:40:04.000000 pyxk-0.5.1/pyxk.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      539 2023-04-09 12:40:04.000000 pyxk-0.5.1/pyxk.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-09 12:40:04.000000 pyxk-0.5.1/pyxk.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       91 2023-04-09 12:40:04.000000 pyxk-0.5.1/pyxk.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       55 2023-04-09 12:40:04.000000 pyxk-0.5.1/pyxk.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        5 2023-04-09 12:40:04.000000 pyxk-0.5.1/pyxk.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-09 12:40:04.368316 pyxk-0.5.1/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      916 2023-04-09 12:40:00.000000 pyxk-0.5.1/setup.py
```

### Comparing `pyxk-0.5.0/LICENSE` & `pyxk-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.0/pyxk/__init__.py` & `pyxk-0.5.1/pyxk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,12 +28,12 @@
     put,
     request,
     wget,
     Session,
 )
 from pyxk.lazy_loader import LazyLoader
 from pyxk.aclient import (
-    ClientSession,
+    AsyncSession,
     default_live,
     default_progress_columns,
     default_download_progress_columns
 )
```

### Comparing `pyxk-0.5.0/pyxk/aclient.py` & `pyxk-0.5.1/pyxk/aclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 rich_box = LazyLoader("rich_box", globals(), "rich.box")
 rich_panel = LazyLoader("rich_panel", globals(), "rich.panel")
 rich_table = LazyLoader("rich_table", globals(), "rich.table")
 rich_console = LazyLoader("rich_console", globals(), "rich.console")
 
 
 
-class ClientSession:
+class AsyncSession:
 
     limit: int = 16
     timeout: typing.Union[int, float, dict] = {
         "total": 8,
         "connect": None,
         "sock_read": None,
         "sock_connect": None
@@ -53,25 +53,27 @@
     async def start(self):
         """运行开始之前调用"""
 
     async def stop(self):
         """运行完成之后调用"""
 
     @classmethod
-    def run(cls) -> typing.Union[object, list]:
+    def run(cls, **kwargs) -> typing.Union[object, list]:
         """类方法: 协程入口 run, 应该从这里开始
 
         Return: ClientSession, [..., ...]
         返回值: 当前类的实例化, 协程运行结果列表
         """
         # Event loop
-        loop = asyncio.new_event_loop()
-        asyncio.set_event_loop(loop)
+        if not isinstance(kwargs.get("loop", None), AbstractEventLoop):
+            loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(loop)
+            kwargs["loop"] = loop
         # Instance
-        self: ClientSession = cls(loop=loop)
+        self: ClientSession = cls(**kwargs)
         result: list = self._loop.run_until_complete(self.async_start())
         # close event loop
         if isinstance(self._loop, AbstractEventLoop):
             self._loop.close()
         return self, result
 
     async def async_start(self):
```

### Comparing `pyxk-0.5.0/pyxk/aes/_fmtdata.py` & `pyxk-0.5.1/pyxk/aes/_fmtdata.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.0/pyxk/aes/cryptor.py` & `pyxk-0.5.1/pyxk/aes/cryptor.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.0/pyxk/lazy_loader.py` & `pyxk-0.5.1/pyxk/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.0/pyxk/m3u8/_download.py` & `pyxk-0.5.1/pyxk/m3u8/_download.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.0/pyxk/m3u8/_entry_point.py` & `pyxk-0.5.1/pyxk/m3u8/_entry_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.0/pyxk/m3u8/_m3u8.py` & `pyxk-0.5.1/pyxk/m3u8/_m3u8.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.0/pyxk/m3u8/_parser.py` & `pyxk-0.5.1/pyxk/m3u8/_parser.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.0/pyxk/requests/_entry_point.py` & `pyxk-0.5.1/pyxk/requests/_entry_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.0/pyxk/requests/api.py` & `pyxk-0.5.1/pyxk/requests/api.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.0/pyxk/requests/sessions.py` & `pyxk-0.5.1/pyxk/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.0/pyxk/utils.py` & `pyxk-0.5.1/pyxk/utils.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.0/pyxk.egg-info/SOURCES.txt` & `pyxk-0.5.1/pyxk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxk-0.5.0/setup.py` & `pyxk-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyxk",
-    version="0.5.0",
+    version="0.5.1",
     author="xiek",
     install_requires=[
         "requests",
         "pycryptodome",
         "rich",
         "m3u8",
         "aiohttp",
```

