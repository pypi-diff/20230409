# Comparing `tmp/selenextra-0.3.tar.gz` & `tmp/selenextra-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenextra-0.3.tar", last modified: Sun Apr  9 06:13:44 2023, max compression
+gzip compressed data, was "selenextra-0.4.tar", last modified: Sun Apr  9 06:31:11 2023, max compression
```

## Comparing `selenextra-0.3.tar` & `selenextra-0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 06:13:44.770141 selenextra-0.3/
--rw-rw-rw-   0        0        0    35823 2023-04-09 06:10:21.000000 selenextra-0.3/LICENSE
--rw-rw-rw-   0        0        0      625 2023-04-09 06:13:44.769143 selenextra-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       93 2023-04-09 06:10:21.000000 selenextra-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 06:13:44.762163 selenextra-0.3/selenextra/
--rw-rw-rw-   0        0        0     3701 2023-04-09 06:12:23.000000 selenextra-0.3/selenextra/__init__.py
--rw-rw-rw-   0        0        0       46 2023-04-09 06:10:21.000000 selenextra-0.3/selenextra/exceptions.py
--rw-rw-rw-   0        0        0     1239 2023-04-09 06:10:21.000000 selenextra-0.3/selenextra/patcher.py
--rw-rw-rw-   0        0        0     5149 2023-04-09 06:10:21.000000 selenextra-0.3/selenextra/typer.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:13:44.768146 selenextra-0.3/selenextra.egg-info/
--rw-rw-rw-   0        0        0      625 2023-04-09 06:13:44.000000 selenextra-0.3/selenextra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-04-09 06:13:44.000000 selenextra-0.3/selenextra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 06:13:44.000000 selenextra-0.3/selenextra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-09 06:13:44.000000 selenextra-0.3/selenextra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-09 06:13:44.000000 selenextra-0.3/selenextra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 06:13:44.770141 selenextra-0.3/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-04-09 06:12:34.000000 selenextra-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:31:11.081256 selenextra-0.4/
+-rw-rw-rw-   0        0        0    35823 2023-04-09 06:25:50.000000 selenextra-0.4/LICENSE
+-rw-rw-rw-   0        0        0      625 2023-04-09 06:31:11.081256 selenextra-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       93 2023-04-09 06:25:50.000000 selenextra-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 06:31:11.074275 selenextra-0.4/selenextra/
+-rw-rw-rw-   0        0        0     3820 2023-04-09 06:30:26.000000 selenextra-0.4/selenextra/__init__.py
+-rw-rw-rw-   0        0        0       46 2023-04-09 06:25:50.000000 selenextra-0.4/selenextra/exceptions.py
+-rw-rw-rw-   0        0        0     1239 2023-04-09 06:25:50.000000 selenextra-0.4/selenextra/patcher.py
+-rw-rw-rw-   0        0        0     5149 2023-04-09 06:25:50.000000 selenextra-0.4/selenextra/typer.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:31:11.080259 selenextra-0.4/selenextra.egg-info/
+-rw-rw-rw-   0        0        0      625 2023-04-09 06:31:10.000000 selenextra-0.4/selenextra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-04-09 06:31:11.000000 selenextra-0.4/selenextra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 06:31:10.000000 selenextra-0.4/selenextra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-09 06:31:10.000000 selenextra-0.4/selenextra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-09 06:31:10.000000 selenextra-0.4/selenextra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 06:31:11.081256 selenextra-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      798 2023-04-09 06:30:37.000000 selenextra-0.4/setup.py
```

### Comparing `selenextra-0.3/LICENSE` & `selenextra-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `selenextra-0.3/PKG-INFO` & `selenextra-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 0.3
+Version: 0.4
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `selenextra-0.3/selenextra/__init__.py` & `selenextra-0.4/selenextra/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 import random as rnd
 import time
 import os
 import json
 
 
 class ChromeDriver(Chrome):
+    CONNECTION_TIMEOUT = 30
+
     def __init__(self, **kwargs) -> None:
         driver_executable_path = kwargs.get('driver_executable_path', None)
 
         self.can_delete_executable = not driver_executable_path
         self.custom_patcher = CustomPatcher(
             executable_path=driver_executable_path,
             force=kwargs.get('patcher_force_close', False),
@@ -45,15 +47,19 @@
 
         return '; '.join(cookies) + ';'
 
     def get_browser_ip(self) -> str:
         self.get('https://httpbin.org/ip')
 
         try:
-            request = self.wait_for_request('/ip')
+            request = self.wait_for_request(
+                pat='/ip',
+                timeout=self.CONNECTION_TIMEOUT
+            )
+
             if not request.response.status_code == 200:
                 raise RequestException("Request failed with status code: {}".format(
                     request.response.status_code))
         except Exception as e:
             raise RequestException("Failed to retrieve IP: {}".format(str(e)))
 
         try:
```

### Comparing `selenextra-0.3/selenextra/patcher.py` & `selenextra-0.4/selenextra/patcher.py`

 * *Files identical despite different names*

### Comparing `selenextra-0.3/selenextra/typer.py` & `selenextra-0.4/selenextra/typer.py`

 * *Files identical despite different names*

### Comparing `selenextra-0.3/selenextra.egg-info/PKG-INFO` & `selenextra-0.4/selenextra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 0.3
+Version: 0.4
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `selenextra-0.3/setup.py` & `selenextra-0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='selenextra',
-    version='0.3',
+    version='0.4',
     description='Bringing additional features to Selenium',
     author='Tat Nguyen Van',
     author_email='nguyenvantat1182002@gmail.com',
     url='https://github.com/nguyenvantat1182002/SeleneXtra',
     packages=find_packages(),
     install_requires=[
         'scipy',
```

