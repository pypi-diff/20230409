# Comparing `tmp/bingai-0.0.5.tar.gz` & `tmp/bingai-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bingai-0.0.5.tar", last modified: Sun Apr  9 06:36:47 2023, max compression
+gzip compressed data, was "bingai-0.0.6.tar", last modified: Sun Apr  9 06:38:30 2023, max compression
```

## Comparing `bingai-0.0.5.tar` & `bingai-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:36:47.136246 bingai-0.0.5/
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 05:57:49.000000 bingai-0.0.5/LICENSE
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      452 2023-04-09 06:36:47.135795 bingai-0.0.5/PKG-INFO
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)       18 2023-04-09 06:24:43.000000 bingai-0.0.5/README.md
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      546 2023-04-09 06:35:07.000000 bingai-0.0.5/pyproject.toml
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)       38 2023-04-09 06:36:47.136296 bingai-0.0.5/setup.cfg
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:36:47.125892 bingai-0.0.5/src/
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:36:47.129755 bingai-0.0.5/src/bingai/
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)       32 2023-04-09 06:36:04.000000 bingai-0.0.5/src/bingai/__init__.py
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)    15462 2023-04-09 06:18:06.000000 bingai-0.0.5/src/bingai/edge.py
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)     2939 2023-04-09 06:36:08.000000 bingai-0.0.5/src/bingai/main.py
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:36:47.133834 bingai-0.0.5/src/bingai.egg-info/
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      452 2023-04-09 06:36:47.000000 bingai-0.0.5/src/bingai.egg-info/PKG-INFO
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      262 2023-04-09 06:36:47.000000 bingai-0.0.5/src/bingai.egg-info/SOURCES.txt
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        1 2023-04-09 06:36:47.000000 bingai-0.0.5/src/bingai.egg-info/dependency_links.txt
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        9 2023-04-09 06:36:47.000000 bingai-0.0.5/src/bingai.egg-info/requires.txt
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        7 2023-04-09 06:36:47.000000 bingai-0.0.5/src/bingai.egg-info/top_level.txt
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:38:30.180306 bingai-0.0.6/
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 05:57:49.000000 bingai-0.0.6/LICENSE
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      452 2023-04-09 06:38:30.178340 bingai-0.0.6/PKG-INFO
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)       18 2023-04-09 06:24:43.000000 bingai-0.0.6/README.md
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      546 2023-04-09 06:38:17.000000 bingai-0.0.6/pyproject.toml
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)       38 2023-04-09 06:38:30.180420 bingai-0.0.6/setup.cfg
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:38:30.169498 bingai-0.0.6/src/
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:38:30.173720 bingai-0.0.6/src/bingai/
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)       52 2023-04-09 06:37:53.000000 bingai-0.0.6/src/bingai/__init__.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)    15462 2023-04-09 06:18:06.000000 bingai-0.0.6/src/bingai/edge.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)     2940 2023-04-09 06:37:59.000000 bingai-0.0.6/src/bingai/main.py
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:38:30.177811 bingai-0.0.6/src/bingai.egg-info/
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      452 2023-04-09 06:38:30.000000 bingai-0.0.6/src/bingai.egg-info/PKG-INFO
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      262 2023-04-09 06:38:30.000000 bingai-0.0.6/src/bingai.egg-info/SOURCES.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        1 2023-04-09 06:38:30.000000 bingai-0.0.6/src/bingai.egg-info/dependency_links.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        9 2023-04-09 06:38:30.000000 bingai-0.0.6/src/bingai.egg-info/requires.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        7 2023-04-09 06:38:30.000000 bingai-0.0.6/src/bingai.egg-info/top_level.txt
```

### Comparing `bingai-0.0.5/pyproject.toml` & `bingai-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bingai"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Gautam Veldanda", email="gautamveldanda@gmail.com" },
 ]
 description = "Bing API for ChatGPT"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `bingai-0.0.5/src/bingai/edge.py` & `bingai-0.0.6/src/bingai/edge.py`

 * *Files identical despite different names*

### Comparing `bingai-0.0.5/src/bingai/main.py` & `bingai-0.0.6/src/bingai/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import asyncio
 import re
 import os
 from selenium.webdriver import Edge, Chrome, Firefox
 from selenium.webdriver.common.by import By
 from selenium.webdriver.chrome.options import Options
-from edge import Chatbot, ConversationStyle
+from .edge import Chatbot, ConversationStyle
 
 class ChatbotSession:
     def __init__(self, email, password, browser='edge', headless=True):
         self.email = email
         self.password = password
         self.browser = browser
         self.headless = headless
```

