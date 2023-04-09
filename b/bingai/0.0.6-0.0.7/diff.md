# Comparing `tmp/bingai-0.0.6.tar.gz` & `tmp/bingai-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bingai-0.0.6.tar", last modified: Sun Apr  9 06:38:30 2023, max compression
+gzip compressed data, was "bingai-0.0.7.tar", last modified: Sun Apr  9 06:42:10 2023, max compression
```

## Comparing `bingai-0.0.6.tar` & `bingai-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:38:30.180306 bingai-0.0.6/
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 05:57:49.000000 bingai-0.0.6/LICENSE
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      452 2023-04-09 06:38:30.178340 bingai-0.0.6/PKG-INFO
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)       18 2023-04-09 06:24:43.000000 bingai-0.0.6/README.md
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      546 2023-04-09 06:38:17.000000 bingai-0.0.6/pyproject.toml
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)       38 2023-04-09 06:38:30.180420 bingai-0.0.6/setup.cfg
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:38:30.169498 bingai-0.0.6/src/
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:38:30.173720 bingai-0.0.6/src/bingai/
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)       52 2023-04-09 06:37:53.000000 bingai-0.0.6/src/bingai/__init__.py
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)    15462 2023-04-09 06:18:06.000000 bingai-0.0.6/src/bingai/edge.py
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)     2940 2023-04-09 06:37:59.000000 bingai-0.0.6/src/bingai/main.py
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:38:30.177811 bingai-0.0.6/src/bingai.egg-info/
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      452 2023-04-09 06:38:30.000000 bingai-0.0.6/src/bingai.egg-info/PKG-INFO
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      262 2023-04-09 06:38:30.000000 bingai-0.0.6/src/bingai.egg-info/SOURCES.txt
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        1 2023-04-09 06:38:30.000000 bingai-0.0.6/src/bingai.egg-info/dependency_links.txt
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        9 2023-04-09 06:38:30.000000 bingai-0.0.6/src/bingai.egg-info/requires.txt
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        7 2023-04-09 06:38:30.000000 bingai-0.0.6/src/bingai.egg-info/top_level.txt
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:42:10.490909 bingai-0.0.7/
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 05:57:49.000000 bingai-0.0.7/LICENSE
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      452 2023-04-09 06:42:10.490599 bingai-0.0.7/PKG-INFO
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)       18 2023-04-09 06:24:43.000000 bingai-0.0.7/README.md
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      546 2023-04-09 06:41:52.000000 bingai-0.0.7/pyproject.toml
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)       38 2023-04-09 06:42:10.490959 bingai-0.0.7/setup.cfg
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:42:10.483048 bingai-0.0.7/src/
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:42:10.486626 bingai-0.0.7/src/bingai/
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)       52 2023-04-09 06:37:53.000000 bingai-0.0.7/src/bingai/__init__.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)    15462 2023-04-09 06:18:06.000000 bingai-0.0.7/src/bingai/edge.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)     3112 2023-04-09 06:41:42.000000 bingai-0.0.7/src/bingai/main.py
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:42:10.490124 bingai-0.0.7/src/bingai.egg-info/
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      452 2023-04-09 06:42:10.000000 bingai-0.0.7/src/bingai.egg-info/PKG-INFO
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      262 2023-04-09 06:42:10.000000 bingai-0.0.7/src/bingai.egg-info/SOURCES.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        1 2023-04-09 06:42:10.000000 bingai-0.0.7/src/bingai.egg-info/dependency_links.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        9 2023-04-09 06:42:10.000000 bingai-0.0.7/src/bingai.egg-info/requires.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        7 2023-04-09 06:42:10.000000 bingai-0.0.7/src/bingai.egg-info/top_level.txt
```

### Comparing `bingai-0.0.6/pyproject.toml` & `bingai-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bingai"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Gautam Veldanda", email="gautamveldanda@gmail.com" },
 ]
 description = "Bing API for ChatGPT"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `bingai-0.0.6/src/bingai/edge.py` & `bingai-0.0.7/src/bingai/edge.py`

 * *Files identical despite different names*

### Comparing `bingai-0.0.6/src/bingai/main.py` & `bingai-0.0.7/src/bingai/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import time
 import json
 import asyncio
 import re
 import os
+from selenium import webdriver
 from selenium.webdriver import Edge, Chrome, Firefox
 from selenium.webdriver.common.by import By
 from selenium.webdriver.chrome.options import Options
 from .edge import Chatbot, ConversationStyle
 
 class ChatbotSession:
     def __init__(self, email, password, browser='edge', headless=True):
@@ -25,17 +26,20 @@
             driver = Chrome()
         elif self.browser == 'firefox':
             driver = Firefox()
         else:
             raise ValueError(f"Invalid browser specified: {self.browser}")
 
         # Configure options
+        edgeOptions = webdriver.EdgeOptions()
+        edgeOptions.headless = self.headless
         options = Options()
         if self.headless:
             options.add_argument("--headless")
+            options.add_argument('--disable-gpu')
 
         # Navigate to the login page and enter email
         driver.get('https://login.live.com/')
         email_input = driver.find_element(By.NAME, 'loginfmt')
         email_input.send_keys(self.email)
         driver.find_element(By.ID, 'idSIButton9').click()
         time.sleep(3)
```

