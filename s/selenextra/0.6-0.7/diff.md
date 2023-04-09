# Comparing `tmp/selenextra-0.6.tar.gz` & `tmp/selenextra-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenextra-0.6.tar", last modified: Sun Apr  9 06:42:18 2023, max compression
+gzip compressed data, was "selenextra-0.7.tar", last modified: Sun Apr  9 09:30:21 2023, max compression
```

## Comparing `selenextra-0.6.tar` & `selenextra-0.7.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 06:42:18.878799 selenextra-0.6/
--rw-rw-rw-   0        0        0    35823 2023-04-09 06:25:50.000000 selenextra-0.6/LICENSE
--rw-rw-rw-   0        0        0      625 2023-04-09 06:42:18.877801 selenextra-0.6/PKG-INFO
--rw-rw-rw-   0        0        0       93 2023-04-09 06:25:50.000000 selenextra-0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 06:42:18.869823 selenextra-0.6/selenextra/
--rw-rw-rw-   0        0        0     4561 2023-04-09 06:41:48.000000 selenextra-0.6/selenextra/__init__.py
--rw-rw-rw-   0        0        0       46 2023-04-09 06:25:50.000000 selenextra-0.6/selenextra/exceptions.py
--rw-rw-rw-   0        0        0     1239 2023-04-09 06:25:50.000000 selenextra-0.6/selenextra/patcher.py
--rw-rw-rw-   0        0        0     5149 2023-04-09 06:25:50.000000 selenextra-0.6/selenextra/typer.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:42:18.876804 selenextra-0.6/selenextra.egg-info/
--rw-rw-rw-   0        0        0      625 2023-04-09 06:42:18.000000 selenextra-0.6/selenextra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-04-09 06:42:18.000000 selenextra-0.6/selenextra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 06:42:18.000000 selenextra-0.6/selenextra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-09 06:42:18.000000 selenextra-0.6/selenextra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-09 06:42:18.000000 selenextra-0.6/selenextra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 06:42:18.878799 selenextra-0.6/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-04-09 06:41:56.000000 selenextra-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 09:30:21.626941 selenextra-0.7/
+-rw-rw-rw-   0        0        0    35823 2023-04-09 08:30:10.000000 selenextra-0.7/LICENSE
+-rw-rw-rw-   0        0        0   247181 2023-03-28 09:22:26.000000 selenextra-0.7/LICENSE.chromedriver
+-rw-rw-rw-   0        0        0      625 2023-04-09 09:30:21.625944 selenextra-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       93 2023-04-09 08:30:10.000000 selenextra-0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 09:30:21.619958 selenextra-0.7/selenextra/
+-rw-rw-rw-   0        0        0     4440 2023-04-09 09:27:39.000000 selenextra-0.7/selenextra/__init__.py
+-rw-rw-rw-   0        0        0       46 2023-04-09 08:30:10.000000 selenextra-0.7/selenextra/exceptions.py
+-rw-rw-rw-   0        0        0     1239 2023-04-09 08:30:10.000000 selenextra-0.7/selenextra/patcher.py
+-rw-rw-rw-   0        0        0     5149 2023-04-09 08:30:10.000000 selenextra-0.7/selenextra/typer.py
+drwxrwxrwx   0        0        0        0 2023-04-09 09:30:21.625944 selenextra-0.7/selenextra.egg-info/
+-rw-rw-rw-   0        0        0      625 2023-04-09 09:30:21.000000 selenextra-0.7/selenextra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-04-09 09:30:21.000000 selenextra-0.7/selenextra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 09:30:21.000000 selenextra-0.7/selenextra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-09 09:30:21.000000 selenextra-0.7/selenextra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-09 09:30:21.000000 selenextra-0.7/selenextra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 09:30:21.626941 selenextra-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      798 2023-04-09 09:27:45.000000 selenextra-0.7/setup.py
```

### Comparing `selenextra-0.6/LICENSE` & `selenextra-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `selenextra-0.6/PKG-INFO` & `selenextra-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 0.6
+Version: 0.7
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `selenextra-0.6/selenextra/__init__.py` & `selenextra-0.7/selenextra/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 from .typer import Typer
-from seleniumwire.undetected_chromedriver import Chrome, ChromeOptions
+from undetected_chromedriver import ChromeOptions
+from seleniumwire.undetected_chromedriver import Chrome
 from selenium.common.exceptions import TimeoutException
 from seleniumwire.request import Request, Response
 from typing import Union, Callable, Any, List, Tuple
 from .patcher import CustomPatcher
 from .exceptions import *
 
 import re
 import random as rnd
 import time
-import os
 import json
 
 
 class ChromeDriver(Chrome):
     CONNECTION_TIMEOUT = 30
 
     def __init__(self, **kwargs) -> None:
-        driver_executable_path = kwargs.get('driver_executable_path', None)
-
-        self.can_delete_executable = not driver_executable_path
         self.custom_patcher = CustomPatcher(
-            executable_path=driver_executable_path,
+            executable_path=kwargs.get('driver_executable_path', None),
             force=kwargs.get('patcher_force_close', False),
             version_main=kwargs.get('version_main', None)
         )
 
         self.custom_patcher.auto()
 
         release = self.custom_patcher.fetch_release_number()
@@ -66,32 +63,43 @@
             body = request.response.body.decode('utf-8')
             data = json.loads(body)
         except:
             return None
 
         return data['origin']
 
-    def process_requests(self, callback: Callable[[Request, Response], Any], timeout: Union[int, float] = 30) -> Any:
+    def callback_with_timeout(self, callback: Callable[[Tuple], Any], params: tuple, timeout: Union[int, float] = 30) -> Any:
         end_time = time.time() + timeout
 
         while time.time() < end_time:
-            for request in self.requests:
-                if not request.response:
-                    continue
-
-                response = request.response
-                result = callback(request, response)
+            result = callback(*params)
 
-                if not result:
-                    continue
+            if not result:
+                continue
 
-                return result
+            return result
 
         raise TimeoutException(
-            'Request processing timed out after the specified timeout period.')
+            f'Callback execution timed out: {callback.__name__}')
+
+    def _process_requests(self, callback: Callable[[Request, Response], Any]) -> Any:
+        for request in self.requests:
+            if not request.response:
+                continue
+
+            response = request.response
+            result = callback(request, response)
+
+            if not result:
+                continue
+
+            return result
+
+    def process_requests(self, callback: Callable[[Request, Response], Any], timeout: Union[int, float] = 30) -> Any:
+        return self.callback_with_timeout(self._process_requests, (callback,), timeout)
 
     def sleep_random_time(self, a: Union[int, float], b: Union[int, float]) -> None:
         time.sleep(round(rnd.uniform(a, b), 1))
 
     def add_cookie_string(self, cookie_string: str) -> None:
         cookie_regex = re.compile(r"([^=]+)=([^;]+)?;")
         cookies = cookie_regex.findall(cookie_string)
@@ -102,39 +110,24 @@
             value = value.strip()
 
             self.add_cookie({'name': name, 'value': value})
 
         self.sleep_random_time(1, 2.5)
         self.refresh()
 
-    def find_first_matching_request(self, paths: List[Tuple[str, Callable[[Request], Any]]], timeout: Union[int, float] = 30) -> Any:
-        end_time = time.time() + timeout
-
-        while time.time() < end_time:
-            for item in paths:
-                path, callback = item
-
-                request = self.backend.storage.find(path)
-                if request is None:
-                    time.sleep(1/5)
-                    continue
+    def _find_first_matching_request(self, paths: List[Tuple[str, Callable[[Request], Any]]]) -> Any:
+        for item in paths:
+            path, callback = item
+
+            request = self.backend.storage.find(path)
+            if request is None:
+                time.sleep(1/5)
+                continue
 
-                return callback(request) if callback else request
+            return callback(request) if callback else request
 
-        raise TimeoutException(
-            'Could not find the requested item within the specified timeout')
-
-    def remove_executable(self) -> None:
-        if self.can_delete_executable:
-            os.remove(self.custom_patcher.executable_path)
+    def find_first_matching_request(self, paths: List[Tuple[str, Callable[[Request], Any]]], timeout: Union[int, float] = 30) -> Any:
+        return self.callback_with_timeout(self._find_first_matching_request, (paths, ), timeout)
 
     def quit(self) -> None:
         super().quit()
-        self.remove_executable()
-
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
-        super().__exit__(exc_type, exc_val, exc_tb)
-        self.remove_executable()
-
-    def __del__(self) -> None:
-        super().__del__()
-        self.remove_executable()
+        self.custom_patcher = None
```

### Comparing `selenextra-0.6/selenextra/patcher.py` & `selenextra-0.7/selenextra/patcher.py`

 * *Files identical despite different names*

### Comparing `selenextra-0.6/selenextra/typer.py` & `selenextra-0.7/selenextra/typer.py`

 * *Files identical despite different names*

### Comparing `selenextra-0.6/selenextra.egg-info/PKG-INFO` & `selenextra-0.7/selenextra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 0.6
+Version: 0.7
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `selenextra-0.6/setup.py` & `selenextra-0.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='selenextra',
-    version='0.6',
+    version='0.7',
     description='Bringing additional features to Selenium',
     author='Tat Nguyen Van',
     author_email='nguyenvantat1182002@gmail.com',
     url='https://github.com/nguyenvantat1182002/SeleneXtra',
     packages=find_packages(),
     install_requires=[
         'scipy',
```

