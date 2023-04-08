# Comparing `tmp/datastructuresLionelHandEricM-0.2.tar.gz` & `tmp/datastructuresLionelHandEricM-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datastructuresLionelHandEricM-0.2.tar", last modified: Sat Apr  8 22:00:23 2023, max compression
+gzip compressed data, was "datastructuresLionelHandEricM-0.3.tar", last modified: Sat Apr  8 22:17:54 2023, max compression
```

## Comparing `datastructuresLionelHandEricM-0.2.tar` & `datastructuresLionelHandEricM-0.3.tar`

### file list

```diff
@@ -1,10 +1,12 @@
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-08 22:00:23.644148 datastructuresLionelHandEricM-0.2/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-03-29 13:29:16.000000 datastructuresLionelHandEricM-0.2/.DS_Store
--rw-r--r--   0 lionelhasan   (501) staff       (20)      263 2023-04-08 22:00:23.643978 datastructuresLionelHandEricM-0.2/PKG-INFO
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-08 22:00:23.643773 datastructuresLionelHandEricM-0.2/datastructuresLionelHandEricM.egg-info/
--rw-r--r--   0 lionelhasan   (501) staff       (20)      263 2023-04-08 22:00:23.000000 datastructuresLionelHandEricM-0.2/datastructuresLionelHandEricM.egg-info/PKG-INFO
--rw-r--r--   0 lionelhasan   (501) staff       (20)      230 2023-04-08 22:00:23.000000 datastructuresLionelHandEricM-0.2/datastructuresLionelHandEricM.egg-info/SOURCES.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-08 22:00:23.000000 datastructuresLionelHandEricM-0.2/datastructuresLionelHandEricM.egg-info/dependency_links.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)       30 2023-04-08 22:00:23.000000 datastructuresLionelHandEricM-0.2/datastructuresLionelHandEricM.egg-info/top_level.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)       38 2023-04-08 22:00:23.644196 datastructuresLionelHandEricM-0.2/setup.cfg
--rw-r--r--   0 lionelhasan   (501) staff       (20)      340 2023-04-08 22:00:21.000000 datastructuresLionelHandEricM-0.2/setup.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-08 22:17:54.519631 datastructuresLionelHandEricM-0.3/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-03-29 13:29:16.000000 datastructuresLionelHandEricM-0.3/.DS_Store
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      263 2023-04-08 22:17:54.519494 datastructuresLionelHandEricM-0.3/PKG-INFO
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-08 22:17:54.518827 datastructuresLionelHandEricM-0.3/datastructuresLionelHandEricM/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-08 21:25:35.000000 datastructuresLionelHandEricM-0.3/datastructuresLionelHandEricM/__init__.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-08 22:17:54.519315 datastructuresLionelHandEricM-0.3/datastructuresLionelHandEricM.egg-info/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      263 2023-04-08 22:17:54.000000 datastructuresLionelHandEricM-0.3/datastructuresLionelHandEricM.egg-info/PKG-INFO
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      272 2023-04-08 22:17:54.000000 datastructuresLionelHandEricM-0.3/datastructuresLionelHandEricM.egg-info/SOURCES.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-08 22:17:54.000000 datastructuresLionelHandEricM-0.3/datastructuresLionelHandEricM.egg-info/dependency_links.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)       30 2023-04-08 22:17:54.000000 datastructuresLionelHandEricM-0.3/datastructuresLionelHandEricM.egg-info/top_level.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)       38 2023-04-08 22:17:54.519675 datastructuresLionelHandEricM-0.3/setup.cfg
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      340 2023-04-08 22:17:52.000000 datastructuresLionelHandEricM-0.3/setup.py
```

### Comparing `datastructuresLionelHandEricM-0.2/.DS_Store` & `datastructuresLionelHandEricM-0.3/.DS_Store`

 * *Files identical despite different names*

