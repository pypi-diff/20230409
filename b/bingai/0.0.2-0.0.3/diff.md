# Comparing `tmp/bingai-0.0.2.tar.gz` & `tmp/bingai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bingai-0.0.2.tar", last modified: Sun Apr  9 06:26:33 2023, max compression
+gzip compressed data, was "bingai-0.0.3.tar", last modified: Sun Apr  9 06:29:45 2023, max compression
```

## Comparing `bingai-0.0.2.tar` & `bingai-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:26:33.387233 bingai-0.0.2/
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 05:57:49.000000 bingai-0.0.2/LICENSE
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      452 2023-04-09 06:26:33.386878 bingai-0.0.2/PKG-INFO
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)       18 2023-04-09 06:24:43.000000 bingai-0.0.2/README.md
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      426 2023-04-09 06:26:23.000000 bingai-0.0.2/pyproject.toml
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)       38 2023-04-09 06:26:33.387273 bingai-0.0.2/setup.cfg
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:26:33.375414 bingai-0.0.2/src/
-drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:26:33.386386 bingai-0.0.2/src/bingai.egg-info/
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      452 2023-04-09 06:26:33.000000 bingai-0.0.2/src/bingai.egg-info/PKG-INFO
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)      194 2023-04-09 06:26:33.000000 bingai-0.0.2/src/bingai.egg-info/SOURCES.txt
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)        1 2023-04-09 06:26:33.000000 bingai-0.0.2/src/bingai.egg-info/dependency_links.txt
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)       12 2023-04-09 06:26:33.000000 bingai-0.0.2/src/bingai.egg-info/top_level.txt
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)     2939 2023-04-09 06:18:14.000000 bingai-0.0.2/src/bingai.py
--rw-r--r--   0 gautam_veldanda   (501) staff       (20)    15462 2023-04-09 06:18:06.000000 bingai-0.0.2/src/edge.py
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:29:45.471113 bingai-0.0.3/
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 05:57:49.000000 bingai-0.0.3/LICENSE
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      452 2023-04-09 06:29:45.470553 bingai-0.0.3/PKG-INFO
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)       18 2023-04-09 06:24:43.000000 bingai-0.0.3/README.md
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      461 2023-04-09 06:29:37.000000 bingai-0.0.3/pyproject.toml
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)       38 2023-04-09 06:29:45.471176 bingai-0.0.3/setup.cfg
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:29:45.466702 bingai-0.0.3/src/
+drwxr-xr-x   0 gautam_veldanda   (501) staff       (20)        0 2023-04-09 06:29:45.469730 bingai-0.0.3/src/bingai.egg-info/
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      452 2023-04-09 06:29:45.000000 bingai-0.0.3/src/bingai.egg-info/PKG-INFO
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)      227 2023-04-09 06:29:45.000000 bingai-0.0.3/src/bingai.egg-info/SOURCES.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        1 2023-04-09 06:29:45.000000 bingai-0.0.3/src/bingai.egg-info/dependency_links.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)        9 2023-04-09 06:29:45.000000 bingai-0.0.3/src/bingai.egg-info/requires.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)       12 2023-04-09 06:29:45.000000 bingai-0.0.3/src/bingai.egg-info/top_level.txt
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)     2939 2023-04-09 06:18:14.000000 bingai-0.0.3/src/bingai.py
+-rw-r--r--   0 gautam_veldanda   (501) staff       (20)    15462 2023-04-09 06:18:06.000000 bingai-0.0.3/src/edge.py
```

### Comparing `bingai-0.0.2/src/bingai.py` & `bingai-0.0.3/src/bingai.py`

 * *Files identical despite different names*

### Comparing `bingai-0.0.2/src/edge.py` & `bingai-0.0.3/src/edge.py`

 * *Files identical despite different names*

