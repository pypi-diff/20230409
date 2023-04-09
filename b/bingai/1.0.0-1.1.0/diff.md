# Comparing `tmp/bingai-1.0.0.tar.gz` & `tmp/bingai-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bingai-1.0.0.tar", last modified: Sun Apr  9 06:51:42 2023, max compression
+gzip compressed data, was "bingai-1.1.0.tar", last modified: Sun Apr  9 07:00:45 2023, max compression
```

## Comparing `bingai-1.0.0.tar` & `bingai-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:51:42.761206 bingai-1.0.0/
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 05:57:49.000000 bingai-1.0.0/LICENSE
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      645 2023-04-09 06:51:42.760896 bingai-1.0.0/PKG-INFO
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      212 2023-04-09 06:51:25.000000 bingai-1.0.0/README.md
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      546 2023-04-09 06:51:03.000000 bingai-1.0.0/pyproject.toml
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)       38 2023-04-09 06:51:42.761269 bingai-1.0.0/setup.cfg
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:51:42.747043 bingai-1.0.0/src/
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:51:42.756750 bingai-1.0.0/src/bingai/
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)       49 2023-04-09 06:50:45.000000 bingai-1.0.0/src/bingai/__init__.py
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)    15462 2023-04-09 06:18:06.000000 bingai-1.0.0/src/bingai/edge.py
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)     3109 2023-04-09 06:50:45.000000 bingai-1.0.0/src/bingai/main.py
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:51:42.760347 bingai-1.0.0/src/bingai.egg-info/
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      645 2023-04-09 06:51:42.000000 bingai-1.0.0/src/bingai.egg-info/PKG-INFO
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      262 2023-04-09 06:51:42.000000 bingai-1.0.0/src/bingai.egg-info/SOURCES.txt
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        1 2023-04-09 06:51:42.000000 bingai-1.0.0/src/bingai.egg-info/dependency_links.txt
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        9 2023-04-09 06:51:42.000000 bingai-1.0.0/src/bingai.egg-info/requires.txt
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        7 2023-04-09 06:51:42.000000 bingai-1.0.0/src/bingai.egg-info/top_level.txt
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 07:00:45.660881 bingai-1.1.0/
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 05:57:49.000000 bingai-1.1.0/LICENSE
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      845 2023-04-09 07:00:45.660214 bingai-1.1.0/PKG-INFO
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      412 2023-04-09 07:00:19.000000 bingai-1.1.0/README.md
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      546 2023-04-09 07:00:27.000000 bingai-1.1.0/pyproject.toml
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)       38 2023-04-09 07:00:45.660984 bingai-1.1.0/setup.cfg
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 07:00:45.645224 bingai-1.1.0/src/
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 07:00:45.655987 bingai-1.1.0/src/bingai/
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)       49 2023-04-09 06:50:45.000000 bingai-1.1.0/src/bingai/__init__.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)    15462 2023-04-09 06:18:06.000000 bingai-1.1.0/src/bingai/edge.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)     3109 2023-04-09 06:50:45.000000 bingai-1.1.0/src/bingai/main.py
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 07:00:45.659557 bingai-1.1.0/src/bingai.egg-info/
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      845 2023-04-09 07:00:45.000000 bingai-1.1.0/src/bingai.egg-info/PKG-INFO
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      262 2023-04-09 07:00:45.000000 bingai-1.1.0/src/bingai.egg-info/SOURCES.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        1 2023-04-09 07:00:45.000000 bingai-1.1.0/src/bingai.egg-info/dependency_links.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        9 2023-04-09 07:00:45.000000 bingai-1.1.0/src/bingai.egg-info/requires.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        7 2023-04-09 07:00:45.000000 bingai-1.1.0/src/bingai.egg-info/top_level.txt
```

### Comparing `bingai-1.0.0/pyproject.toml` & `bingai-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bingai"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Gautam Veldanda", email="gautamveldanda@gmail.com" },
 ]
 description = "Bing API for ChatGPT"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `bingai-1.0.0/src/bingai/edge.py` & `bingai-1.1.0/src/bingai/edge.py`

 * *Files identical despite different names*

### Comparing `bingai-1.0.0/src/bingai/main.py` & `bingai-1.1.0/src/bingai/main.py`

 * *Files identical despite different names*

