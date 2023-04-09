# Comparing `tmp/pyxk-0.4.9.tar.gz` & `tmp/pyxk-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxk-0.4.9.tar", last modified: Sat Apr  8 12:34:36 2023, max compression
+gzip compressed data, was "pyxk-0.5.0.tar", last modified: Sun Apr  9 02:21:25 2023, max compression
```

## Comparing `pyxk-0.4.9.tar` & `pyxk-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-08 12:34:36.159032 pyxk-0.4.9/
--rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.4.9/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)      343 2023-04-08 12:34:36.159032 pyxk-0.4.9/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.4.9/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-08 12:34:36.159032 pyxk-0.4.9/pyxk/
--rw-rw----   0 root         (0) everybody  (9997)      702 2023-04-08 12:07:19.000000 pyxk-0.4.9/pyxk/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    10405 2023-04-08 12:33:28.000000 pyxk-0.4.9/pyxk/aclient.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-08 12:34:36.159032 pyxk-0.4.9/pyxk/aes/
--rw-rw----   0 root         (0) everybody  (9997)       79 2023-02-24 04:10:40.000000 pyxk-0.4.9/pyxk/aes/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     3639 2023-04-06 15:25:24.000000 pyxk-0.4.9/pyxk/aes/_fmtdata.py
--rw-rw----   0 root         (0) everybody  (9997)     4701 2023-04-06 15:27:39.000000 pyxk-0.4.9/pyxk/aes/cryptor.py
--rw-rw----   0 root         (0) everybody  (9997)      954 2023-03-15 06:04:12.000000 pyxk-0.4.9/pyxk/lazy_loader.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-08 12:34:36.159032 pyxk-0.4.9/pyxk/m3u8/
--rw-rw----   0 root         (0) everybody  (9997)       82 2023-03-16 14:08:36.000000 pyxk-0.4.9/pyxk/m3u8/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     8292 2023-03-16 12:13:38.000000 pyxk-0.4.9/pyxk/m3u8/_download.py
--rw-rw----   0 root         (0) everybody  (9997)     3199 2023-03-16 16:35:49.000000 pyxk-0.4.9/pyxk/m3u8/_entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)     7791 2023-03-16 16:35:32.000000 pyxk-0.4.9/pyxk/m3u8/_m3u8.py
--rw-rw----   0 root         (0) everybody  (9997)     4504 2023-03-17 04:00:18.000000 pyxk-0.4.9/pyxk/m3u8/_parser.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-08 12:34:36.159032 pyxk-0.4.9/pyxk/requests/
--rw-rw----   0 root         (0) everybody  (9997)      235 2023-04-06 15:53:39.000000 pyxk-0.4.9/pyxk/requests/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     5598 2023-04-06 16:07:00.000000 pyxk-0.4.9/pyxk/requests/_entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)     7514 2023-03-31 10:17:41.000000 pyxk-0.4.9/pyxk/requests/api.py
--rw-rw----   0 root         (0) everybody  (9997)    21859 2023-04-06 15:20:21.000000 pyxk-0.4.9/pyxk/requests/sessions.py
--rw-rw----   0 root         (0) everybody  (9997)    12202 2023-04-06 16:00:37.000000 pyxk-0.4.9/pyxk/utils.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-08 12:34:36.159032 pyxk-0.4.9/pyxk.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      343 2023-04-08 12:34:35.000000 pyxk-0.4.9/pyxk.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      539 2023-04-08 12:34:36.000000 pyxk-0.4.9/pyxk.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-08 12:34:35.000000 pyxk-0.4.9/pyxk.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       91 2023-04-08 12:34:35.000000 pyxk-0.4.9/pyxk.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       55 2023-04-08 12:34:35.000000 pyxk-0.4.9/pyxk.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        5 2023-04-08 12:34:35.000000 pyxk-0.4.9/pyxk.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-08 12:34:36.159032 pyxk-0.4.9/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      916 2023-04-08 12:34:26.000000 pyxk-0.4.9/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 02:21:25.194990 pyxk-0.5.0/
+-rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:05.000000 pyxk-0.5.0/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)      343 2023-04-09 02:21:25.194990 pyxk-0.5.0/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)        4 2023-03-31 15:33:16.000000 pyxk-0.5.0/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 02:21:25.184990 pyxk-0.5.0/pyxk/
+-rw-rw----   0 root         (0) everybody  (9997)      702 2023-04-08 12:07:19.000000 pyxk-0.5.0/pyxk/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    10882 2023-04-08 18:09:14.000000 pyxk-0.5.0/pyxk/aclient.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 02:21:25.194990 pyxk-0.5.0/pyxk/aes/
+-rw-rw----   0 root         (0) everybody  (9997)       79 2023-02-24 04:10:40.000000 pyxk-0.5.0/pyxk/aes/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     3639 2023-04-06 15:25:24.000000 pyxk-0.5.0/pyxk/aes/_fmtdata.py
+-rw-rw----   0 root         (0) everybody  (9997)     4701 2023-04-06 15:27:39.000000 pyxk-0.5.0/pyxk/aes/cryptor.py
+-rw-rw----   0 root         (0) everybody  (9997)      954 2023-03-15 06:04:12.000000 pyxk-0.5.0/pyxk/lazy_loader.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 02:21:25.194990 pyxk-0.5.0/pyxk/m3u8/
+-rw-rw----   0 root         (0) everybody  (9997)       82 2023-03-16 14:08:36.000000 pyxk-0.5.0/pyxk/m3u8/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     8292 2023-03-16 12:13:38.000000 pyxk-0.5.0/pyxk/m3u8/_download.py
+-rw-rw----   0 root         (0) everybody  (9997)     3199 2023-03-16 16:35:49.000000 pyxk-0.5.0/pyxk/m3u8/_entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)     7791 2023-03-16 16:35:32.000000 pyxk-0.5.0/pyxk/m3u8/_m3u8.py
+-rw-rw----   0 root         (0) everybody  (9997)     4504 2023-03-17 04:00:18.000000 pyxk-0.5.0/pyxk/m3u8/_parser.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 02:21:25.194990 pyxk-0.5.0/pyxk/requests/
+-rw-rw----   0 root         (0) everybody  (9997)      235 2023-04-06 15:53:39.000000 pyxk-0.5.0/pyxk/requests/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     5598 2023-04-06 16:07:00.000000 pyxk-0.5.0/pyxk/requests/_entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)     7514 2023-03-31 10:17:41.000000 pyxk-0.5.0/pyxk/requests/api.py
+-rw-rw----   0 root         (0) everybody  (9997)    21859 2023-04-06 15:20:21.000000 pyxk-0.5.0/pyxk/requests/sessions.py
+-rw-rw----   0 root         (0) everybody  (9997)    12202 2023-04-06 16:00:37.000000 pyxk-0.5.0/pyxk/utils.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-09 02:21:25.184990 pyxk-0.5.0/pyxk.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      343 2023-04-09 02:21:25.000000 pyxk-0.5.0/pyxk.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      539 2023-04-09 02:21:25.000000 pyxk-0.5.0/pyxk.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-09 02:21:25.000000 pyxk-0.5.0/pyxk.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       91 2023-04-09 02:21:25.000000 pyxk-0.5.0/pyxk.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       55 2023-04-09 02:21:25.000000 pyxk-0.5.0/pyxk.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        5 2023-04-09 02:21:25.000000 pyxk-0.5.0/pyxk.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-09 02:21:25.194990 pyxk-0.5.0/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      916 2023-04-09 02:20:57.000000 pyxk-0.5.0/setup.py
```

### Comparing `pyxk-0.4.9/LICENSE` & `pyxk-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxk-0.4.9/pyxk/__init__.py` & `pyxk-0.5.0/pyxk/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.4.9/pyxk/aclient.py` & `pyxk-0.5.0/pyxk/aclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,54 +53,68 @@
     async def start(self):
         """运行开始之前调用"""
 
     async def stop(self):
         """运行完成之后调用"""
 
     @classmethod
-    def run(cls) -> tuple:
+    def run(cls) -> typing.Union[object, list]:
         """类方法: 协程入口 run, 应该从这里开始
 
         Return: ClientSession, [..., ...]
         返回值: 当前类的实例化, 协程运行结果列表
         """
         # Event loop
         loop = asyncio.new_event_loop()
         asyncio.set_event_loop(loop)
         # Instance
         self: ClientSession = cls(loop=loop)
         result: list = self._loop.run_until_complete(self.async_start())
+        # close event loop
+        if isinstance(self._loop, AbstractEventLoop):
+            self._loop.close()
         return self, result
 
     async def async_start(self):
         try:
-            # Event loop
-            if not isinstance(self._loop, asyncio.AbstractEventLoop):
+            # event loop
+            if (
+                not isinstance(self._loop, AbstractEventLoop)
+                or self._loop.is_closed() is True
+            ):
                 self._loop = asyncio.get_event_loop()
+                asyncio.set_event_loop(self._loop)
+            # create aiohttp.ClientSession
+            if not (
+                isinstance(self._session, Session)
+                and self._session.closed is False
+            ):
+                self._session = await self.create_client_session()
 
-            # Create aiohttp.ClientSession
-            if not isinstance(self._session, Session):
-                self._session = Session(
-                    loop=self._loop,
-                    headers=self.merge_headers(),
-                    **self.merge_aiohttp_kwargs()
-                )
             # run - self.open
             await self.start()
             result: list = await self.start_request()
         finally:
             await self.async_close()
         return result
 
     async def async_close(self):
         await self.stop()
-        # Close aiohttp.ClientSession
+        # close aiohttp.ClientSession
         if isinstance(self._session, Session):
             await self._session.close()
 
+    async def create_client_session(self):
+        "创建 aiohttp.ClientSession"
+        return Session(loop=self._loop, headers=self.merge_headers(), **self.merge_aiohttp_kwargs())
+
+    @property
+    def loop(self) -> AbstractEventLoop:
+        return self._loop
+
     def merge_headers(self) -> CIMultiDict:
         """aiohttp.ClientSession Headers"""
         user_agent = self.user_agent if isinstance(self.user_agent, str) else get_user_agent("android")
         headers = CIMultiDict(self.headers or {})
         headers.setdefault("User-Agent", user_agent)
         return headers
```

### Comparing `pyxk-0.4.9/pyxk/aes/_fmtdata.py` & `pyxk-0.5.0/pyxk/aes/_fmtdata.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.4.9/pyxk/aes/cryptor.py` & `pyxk-0.5.0/pyxk/aes/cryptor.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.4.9/pyxk/lazy_loader.py` & `pyxk-0.5.0/pyxk/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.4.9/pyxk/m3u8/_download.py` & `pyxk-0.5.0/pyxk/m3u8/_download.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.4.9/pyxk/m3u8/_entry_point.py` & `pyxk-0.5.0/pyxk/m3u8/_entry_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.4.9/pyxk/m3u8/_m3u8.py` & `pyxk-0.5.0/pyxk/m3u8/_m3u8.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.4.9/pyxk/m3u8/_parser.py` & `pyxk-0.5.0/pyxk/m3u8/_parser.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.4.9/pyxk/requests/_entry_point.py` & `pyxk-0.5.0/pyxk/requests/_entry_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.4.9/pyxk/requests/api.py` & `pyxk-0.5.0/pyxk/requests/api.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.4.9/pyxk/requests/sessions.py` & `pyxk-0.5.0/pyxk/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.4.9/pyxk/utils.py` & `pyxk-0.5.0/pyxk/utils.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.4.9/pyxk.egg-info/SOURCES.txt` & `pyxk-0.5.0/pyxk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxk-0.4.9/setup.py` & `pyxk-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyxk",
-    version="0.4.9",
+    version="0.5.0",
     author="xiek",
     install_requires=[
         "requests",
         "pycryptodome",
         "rich",
         "m3u8",
         "aiohttp",
```

