# Comparing `tmp/selenextra-0.2.tar.gz` & `tmp/selenextra-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenextra-0.2.tar", last modified: Fri Apr  7 13:51:08 2023, max compression
+gzip compressed data, was "selenextra-0.3.tar", last modified: Sun Apr  9 06:13:44 2023, max compression
```

## Comparing `selenextra-0.2.tar` & `selenextra-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 13:51:08.525787 selenextra-0.2/
--rw-rw-rw-   0        0        0    35823 2023-04-07 13:48:48.000000 selenextra-0.2/LICENSE
--rw-rw-rw-   0        0        0      625 2023-04-07 13:51:08.524789 selenextra-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       57 2023-04-07 13:48:48.000000 selenextra-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 13:51:08.518805 selenextra-0.2/selenextra/
--rw-rw-rw-   0        0        0     3740 2023-04-07 13:48:48.000000 selenextra-0.2/selenextra/__init__.py
--rw-rw-rw-   0        0        0       46 2023-04-07 13:48:48.000000 selenextra-0.2/selenextra/exceptions.py
--rw-rw-rw-   0        0        0     1239 2023-04-07 13:48:48.000000 selenextra-0.2/selenextra/patcher.py
--rw-rw-rw-   0        0        0     5149 2023-04-07 13:48:48.000000 selenextra-0.2/selenextra/typer.py
-drwxrwxrwx   0        0        0        0 2023-04-07 13:51:08.524789 selenextra-0.2/selenextra.egg-info/
--rw-rw-rw-   0        0        0      625 2023-04-07 13:51:08.000000 selenextra-0.2/selenextra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-04-07 13:51:08.000000 selenextra-0.2/selenextra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 13:51:08.000000 selenextra-0.2/selenextra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-07 13:51:08.000000 selenextra-0.2/selenextra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-07 13:51:08.000000 selenextra-0.2/selenextra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 13:51:08.525787 selenextra-0.2/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-04-07 13:49:28.000000 selenextra-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:13:44.770141 selenextra-0.3/
+-rw-rw-rw-   0        0        0    35823 2023-04-09 06:10:21.000000 selenextra-0.3/LICENSE
+-rw-rw-rw-   0        0        0      625 2023-04-09 06:13:44.769143 selenextra-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       93 2023-04-09 06:10:21.000000 selenextra-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 06:13:44.762163 selenextra-0.3/selenextra/
+-rw-rw-rw-   0        0        0     3701 2023-04-09 06:12:23.000000 selenextra-0.3/selenextra/__init__.py
+-rw-rw-rw-   0        0        0       46 2023-04-09 06:10:21.000000 selenextra-0.3/selenextra/exceptions.py
+-rw-rw-rw-   0        0        0     1239 2023-04-09 06:10:21.000000 selenextra-0.3/selenextra/patcher.py
+-rw-rw-rw-   0        0        0     5149 2023-04-09 06:10:21.000000 selenextra-0.3/selenextra/typer.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:13:44.768146 selenextra-0.3/selenextra.egg-info/
+-rw-rw-rw-   0        0        0      625 2023-04-09 06:13:44.000000 selenextra-0.3/selenextra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-04-09 06:13:44.000000 selenextra-0.3/selenextra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 06:13:44.000000 selenextra-0.3/selenextra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-09 06:13:44.000000 selenextra-0.3/selenextra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-09 06:13:44.000000 selenextra-0.3/selenextra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 06:13:44.770141 selenextra-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      798 2023-04-09 06:12:34.000000 selenextra-0.3/setup.py
```

### Comparing `selenextra-0.2/LICENSE` & `selenextra-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `selenextra-0.2/PKG-INFO` & `selenextra-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 0.2
+Version: 0.3
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `selenextra-0.2/selenextra/__init__.py` & `selenextra-0.3/selenextra/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from .typer import Typer
+from seleniumwire.undetected_chromedriver import Chrome, ChromeOptions
 from selenium.common.exceptions import TimeoutException
 from seleniumwire.request import Request, Response
 from typing import Union, Callable, Any
 from .patcher import CustomPatcher
 from .exceptions import *
 
 import re
 import random as rnd
 import time
 import os
 import json
-import seleniumwire.undetected_chromedriver as webdriver
 
-ChromeOptions = webdriver.ChromeOptions
 
-
-class ChromeDriver(webdriver.Chrome):
+class ChromeDriver(Chrome):
     def __init__(self, **kwargs) -> None:
         driver_executable_path = kwargs.get('driver_executable_path', None)
 
         self.can_delete_executable = not driver_executable_path
         self.custom_patcher = CustomPatcher(
             executable_path=driver_executable_path,
             force=kwargs.get('patcher_force_close', False),
```

### Comparing `selenextra-0.2/selenextra/patcher.py` & `selenextra-0.3/selenextra/patcher.py`

 * *Files identical despite different names*

### Comparing `selenextra-0.2/selenextra/typer.py` & `selenextra-0.3/selenextra/typer.py`

 * *Files identical despite different names*

### Comparing `selenextra-0.2/selenextra.egg-info/PKG-INFO` & `selenextra-0.3/selenextra.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 0.2
+Version: 0.3
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

