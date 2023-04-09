# Comparing `tmp/bingai-0.0.7.tar.gz` & `tmp/bingai-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bingai-0.0.7.tar", last modified: Sun Apr  9 06:42:10 2023, max compression
+gzip compressed data, was "bingai-1.0.0.tar", last modified: Sun Apr  9 06:51:42 2023, max compression
```

## Comparing `bingai-0.0.7.tar` & `bingai-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:42:10.490909 bingai-0.0.7/
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 05:57:49.000000 bingai-0.0.7/LICENSE
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      452 2023-04-09 06:42:10.490599 bingai-0.0.7/PKG-INFO
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)       18 2023-04-09 06:24:43.000000 bingai-0.0.7/README.md
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      546 2023-04-09 06:41:52.000000 bingai-0.0.7/pyproject.toml
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)       38 2023-04-09 06:42:10.490959 bingai-0.0.7/setup.cfg
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:42:10.483048 bingai-0.0.7/src/
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:42:10.486626 bingai-0.0.7/src/bingai/
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)       52 2023-04-09 06:37:53.000000 bingai-0.0.7/src/bingai/__init__.py
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)    15462 2023-04-09 06:18:06.000000 bingai-0.0.7/src/bingai/edge.py
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)     3112 2023-04-09 06:41:42.000000 bingai-0.0.7/src/bingai/main.py
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:42:10.490124 bingai-0.0.7/src/bingai.egg-info/
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      452 2023-04-09 06:42:10.000000 bingai-0.0.7/src/bingai.egg-info/PKG-INFO
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      262 2023-04-09 06:42:10.000000 bingai-0.0.7/src/bingai.egg-info/SOURCES.txt
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        1 2023-04-09 06:42:10.000000 bingai-0.0.7/src/bingai.egg-info/dependency_links.txt
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        9 2023-04-09 06:42:10.000000 bingai-0.0.7/src/bingai.egg-info/requires.txt
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        7 2023-04-09 06:42:10.000000 bingai-0.0.7/src/bingai.egg-info/top_level.txt
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:51:42.761206 bingai-1.0.0/
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 05:57:49.000000 bingai-1.0.0/LICENSE
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      645 2023-04-09 06:51:42.760896 bingai-1.0.0/PKG-INFO
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      212 2023-04-09 06:51:25.000000 bingai-1.0.0/README.md
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      546 2023-04-09 06:51:03.000000 bingai-1.0.0/pyproject.toml
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)       38 2023-04-09 06:51:42.761269 bingai-1.0.0/setup.cfg
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:51:42.747043 bingai-1.0.0/src/
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:51:42.756750 bingai-1.0.0/src/bingai/
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)       49 2023-04-09 06:50:45.000000 bingai-1.0.0/src/bingai/__init__.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)    15462 2023-04-09 06:18:06.000000 bingai-1.0.0/src/bingai/edge.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)     3109 2023-04-09 06:50:45.000000 bingai-1.0.0/src/bingai/main.py
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:51:42.760347 bingai-1.0.0/src/bingai.egg-info/
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      645 2023-04-09 06:51:42.000000 bingai-1.0.0/src/bingai.egg-info/PKG-INFO
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      262 2023-04-09 06:51:42.000000 bingai-1.0.0/src/bingai.egg-info/SOURCES.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        1 2023-04-09 06:51:42.000000 bingai-1.0.0/src/bingai.egg-info/dependency_links.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        9 2023-04-09 06:51:42.000000 bingai-1.0.0/src/bingai.egg-info/requires.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        7 2023-04-09 06:51:42.000000 bingai-1.0.0/src/bingai.egg-info/top_level.txt
```

### Comparing `bingai-0.0.7/pyproject.toml` & `bingai-1.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bingai"
-version = "0.0.7"
+version = "1.0.0"
 authors = [
   { name="Gautam Veldanda", email="gautamveldanda@gmail.com" },
 ]
 description = "Bing API for ChatGPT"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `bingai-0.0.7/src/bingai/edge.py` & `bingai-1.0.0/src/bingai/edge.py`

 * *Files identical despite different names*

### Comparing `bingai-0.0.7/src/bingai/main.py` & `bingai-1.0.0/src/bingai/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 from selenium import webdriver
 from selenium.webdriver import Edge, Chrome, Firefox
 from selenium.webdriver.common.by import By
 from selenium.webdriver.chrome.options import Options
 from .edge import Chatbot, ConversationStyle
 
-class ChatbotSession:
+class BingSession:
     def __init__(self, email, password, browser='edge', headless=True):
         self.email = email
         self.password = password
         self.browser = browser
         self.headless = headless
         self.cookies_file = 'cookies.json'
         self.bot = None
```

