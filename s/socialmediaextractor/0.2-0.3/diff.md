# Comparing `tmp/socialmediaextractor-0.2.tar.gz` & `tmp/socialmediaextractor-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socialmediaextractor-0.2.tar", last modified: Sun Apr  9 18:16:17 2023, max compression
+gzip compressed data, was "socialmediaextractor-0.3.tar", last modified: Sun Apr  9 18:33:56 2023, max compression
```

## Comparing `socialmediaextractor-0.2.tar` & `socialmediaextractor-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 irfan      (501) staff       (20)        0 2023-04-09 18:16:17.611066 socialmediaextractor-0.2/
--rw-r--r--   0 irfan      (501) staff       (20)      228 2023-04-09 18:16:17.610700 socialmediaextractor-0.2/PKG-INFO
--rw-r--r--   0 irfan      (501) staff       (20)      649 2023-04-09 18:14:52.000000 socialmediaextractor-0.2/README.md
--rw-r--r--   0 irfan      (501) staff       (20)       38 2023-04-09 18:16:17.611207 socialmediaextractor-0.2/setup.cfg
--rw-r--r--   0 irfan      (501) staff       (20)      357 2023-04-09 18:16:14.000000 socialmediaextractor-0.2/setup.py
-drwxr-xr-x   0 irfan      (501) staff       (20)        0 2023-04-09 18:16:17.610138 socialmediaextractor-0.2/socialmediaextractor.egg-info/
--rw-r--r--   0 irfan      (501) staff       (20)      228 2023-04-09 18:16:17.000000 socialmediaextractor-0.2/socialmediaextractor.egg-info/PKG-INFO
--rw-r--r--   0 irfan      (501) staff       (20)      237 2023-04-09 18:16:17.000000 socialmediaextractor-0.2/socialmediaextractor.egg-info/SOURCES.txt
--rw-r--r--   0 irfan      (501) staff       (20)        1 2023-04-09 18:16:17.000000 socialmediaextractor-0.2/socialmediaextractor.egg-info/dependency_links.txt
--rw-r--r--   0 irfan      (501) staff       (20)       24 2023-04-09 18:16:17.000000 socialmediaextractor-0.2/socialmediaextractor.egg-info/requires.txt
--rw-r--r--   0 irfan      (501) staff       (20)        1 2023-04-09 18:16:17.000000 socialmediaextractor-0.2/socialmediaextractor.egg-info/top_level.txt
+drwxr-xr-x   0 irfan      (501) staff       (20)        0 2023-04-09 18:33:56.901027 socialmediaextractor-0.3/
+-rw-r--r--   0 irfan      (501) staff       (20)     1086 2023-04-09 18:33:56.900719 socialmediaextractor-0.3/PKG-INFO
+-rw-r--r--   0 irfan      (501) staff       (20)      649 2023-04-09 18:14:52.000000 socialmediaextractor-0.3/README.md
+-rw-r--r--   0 irfan      (501) staff       (20)       38 2023-04-09 18:33:56.901171 socialmediaextractor-0.3/setup.cfg
+-rw-r--r--   0 irfan      (501) staff       (20)     1250 2023-04-09 18:33:50.000000 socialmediaextractor-0.3/setup.py
+drwxr-xr-x   0 irfan      (501) staff       (20)        0 2023-04-09 18:33:56.900170 socialmediaextractor-0.3/socialmediaextractor.egg-info/
+-rw-r--r--   0 irfan      (501) staff       (20)     1086 2023-04-09 18:33:56.000000 socialmediaextractor-0.3/socialmediaextractor.egg-info/PKG-INFO
+-rw-r--r--   0 irfan      (501) staff       (20)      237 2023-04-09 18:33:56.000000 socialmediaextractor-0.3/socialmediaextractor.egg-info/SOURCES.txt
+-rw-r--r--   0 irfan      (501) staff       (20)        1 2023-04-09 18:33:56.000000 socialmediaextractor-0.3/socialmediaextractor.egg-info/dependency_links.txt
+-rw-r--r--   0 irfan      (501) staff       (20)       24 2023-04-09 18:33:56.000000 socialmediaextractor-0.3/socialmediaextractor.egg-info/requires.txt
+-rw-r--r--   0 irfan      (501) staff       (20)        1 2023-04-09 18:33:56.000000 socialmediaextractor-0.3/socialmediaextractor.egg-info/top_level.txt
```

### Comparing `socialmediaextractor-0.2/README.md` & `socialmediaextractor-0.3/README.md`

 * *Files identical despite different names*

