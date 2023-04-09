# Comparing `tmp/selenextra-0.4.tar.gz` & `tmp/selenextra-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenextra-0.4.tar", last modified: Sun Apr  9 06:31:11 2023, max compression
+gzip compressed data, was "selenextra-0.5.tar", last modified: Sun Apr  9 06:37:08 2023, max compression
```

## Comparing `selenextra-0.4.tar` & `selenextra-0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 06:31:11.081256 selenextra-0.4/
--rw-rw-rw-   0        0        0    35823 2023-04-09 06:25:50.000000 selenextra-0.4/LICENSE
--rw-rw-rw-   0        0        0      625 2023-04-09 06:31:11.081256 selenextra-0.4/PKG-INFO
--rw-rw-rw-   0        0        0       93 2023-04-09 06:25:50.000000 selenextra-0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 06:31:11.074275 selenextra-0.4/selenextra/
--rw-rw-rw-   0        0        0     3820 2023-04-09 06:30:26.000000 selenextra-0.4/selenextra/__init__.py
--rw-rw-rw-   0        0        0       46 2023-04-09 06:25:50.000000 selenextra-0.4/selenextra/exceptions.py
--rw-rw-rw-   0        0        0     1239 2023-04-09 06:25:50.000000 selenextra-0.4/selenextra/patcher.py
--rw-rw-rw-   0        0        0     5149 2023-04-09 06:25:50.000000 selenextra-0.4/selenextra/typer.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:31:11.080259 selenextra-0.4/selenextra.egg-info/
--rw-rw-rw-   0        0        0      625 2023-04-09 06:31:10.000000 selenextra-0.4/selenextra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-04-09 06:31:11.000000 selenextra-0.4/selenextra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 06:31:10.000000 selenextra-0.4/selenextra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-09 06:31:10.000000 selenextra-0.4/selenextra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-09 06:31:10.000000 selenextra-0.4/selenextra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 06:31:11.081256 selenextra-0.4/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-04-09 06:30:37.000000 selenextra-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:37:08.002355 selenextra-0.5/
+-rw-rw-rw-   0        0        0    35823 2023-04-09 06:25:50.000000 selenextra-0.5/LICENSE
+-rw-rw-rw-   0        0        0      625 2023-04-09 06:37:08.002355 selenextra-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       93 2023-04-09 06:25:50.000000 selenextra-0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 06:37:07.991385 selenextra-0.5/selenextra/
+-rw-rw-rw-   0        0        0     4472 2023-04-09 06:36:28.000000 selenextra-0.5/selenextra/__init__.py
+-rw-rw-rw-   0        0        0       46 2023-04-09 06:25:50.000000 selenextra-0.5/selenextra/exceptions.py
+-rw-rw-rw-   0        0        0     1239 2023-04-09 06:25:50.000000 selenextra-0.5/selenextra/patcher.py
+-rw-rw-rw-   0        0        0     5149 2023-04-09 06:25:50.000000 selenextra-0.5/selenextra/typer.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:37:08.001359 selenextra-0.5/selenextra.egg-info/
+-rw-rw-rw-   0        0        0      625 2023-04-09 06:37:07.000000 selenextra-0.5/selenextra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-04-09 06:37:07.000000 selenextra-0.5/selenextra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 06:37:07.000000 selenextra-0.5/selenextra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-09 06:37:07.000000 selenextra-0.5/selenextra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-09 06:37:07.000000 selenextra-0.5/selenextra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 06:37:08.003353 selenextra-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      798 2023-04-09 06:36:34.000000 selenextra-0.5/setup.py
```

### Comparing `selenextra-0.4/LICENSE` & `selenextra-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `selenextra-0.4/PKG-INFO` & `selenextra-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 0.4
+Version: 0.5
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `selenextra-0.4/selenextra/__init__.py` & `selenextra-0.5/selenextra/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .typer import Typer
 from seleniumwire.undetected_chromedriver import Chrome, ChromeOptions
 from selenium.common.exceptions import TimeoutException
 from seleniumwire.request import Request, Response
-from typing import Union, Callable, Any
+from typing import Union, Callable, Any, List, Tuple
 from .patcher import CustomPatcher
 from .exceptions import *
 
 import re
 import random as rnd
 import time
 import os
@@ -102,14 +102,31 @@
             value = value.strip()
 
             self.add_cookie({'name': name, 'value': value})
 
         self.sleep_random_time(1, 2.5)
         self.refresh()
 
+    def find_first_matching_request(self, paths: List[Tuple[str, Callable[[Request], Any]]], timeout: Union[int, float] = 30) -> Any:
+        end_time = time.time() + timeout
+
+        while time.time() < end_time:
+            for item in paths:
+                path, callback = item
+
+                request = self.backend.storage.find(path)
+                if request is None:
+                    time.sleep(1/5)
+                    continue
+
+                return callback(request) if callback else request
+
+        raise TimeoutException(
+            'Could not find the requested item within the specified timeout')
+
     def remove_executable(self) -> None:
         if self.can_delete_executable:
             os.remove(self.custom_patcher.executable_path)
 
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
         super().__exit__(exc_type, exc_val, exc_tb)
         self.remove_executable()
```

### Comparing `selenextra-0.4/selenextra/patcher.py` & `selenextra-0.5/selenextra/patcher.py`

 * *Files identical despite different names*

### Comparing `selenextra-0.4/selenextra/typer.py` & `selenextra-0.5/selenextra/typer.py`

 * *Files identical despite different names*

### Comparing `selenextra-0.4/selenextra.egg-info/PKG-INFO` & `selenextra-0.5/selenextra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 0.4
+Version: 0.5
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `selenextra-0.4/setup.py` & `selenextra-0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='selenextra',
-    version='0.4',
+    version='0.5',
     description='Bringing additional features to Selenium',
     author='Tat Nguyen Van',
     author_email='nguyenvantat1182002@gmail.com',
     url='https://github.com/nguyenvantat1182002/SeleneXtra',
     packages=find_packages(),
     install_requires=[
         'scipy',
```

