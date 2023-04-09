# Comparing `tmp/pyllicagram-1.6.tar.gz` & `tmp/pyllicagram-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyllicagram-1.6.tar", last modified: Sun Apr  9 16:34:53 2023, max compression
+gzip compressed data, was "dist/pyllicagram-1.7.tar", last modified: Sun Apr  9 16:49:29 2023, max compression
```

## Comparing `pyllicagram-1.6.tar` & `pyllicagram-1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 16:34:53.934602 pyllicagram-1.6/
--rw-r--r--   0 benoit2c   (501) staff       (20)      274 2023-04-09 16:34:53.933713 pyllicagram-1.6/PKG-INFO
--rw-r--r--   0 benoit2c   (501) staff       (20)     4137 2022-12-07 10:30:33.000000 pyllicagram-1.6/README.md
--rw-r--r--   0 benoit2c   (501) staff       (20)       38 2023-04-09 16:34:53.934862 pyllicagram-1.6/setup.cfg
--rw-r--r--   0 benoit2c   (501) staff       (20)      404 2023-04-09 16:34:49.000000 pyllicagram-1.6/setup.py
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 16:34:53.925773 pyllicagram-1.6/src/
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 16:34:53.927466 pyllicagram-1.6/src/pyllicagram/
--rw-r--r--   0 benoit2c   (501) staff       (20)     2421 2022-12-07 10:30:33.000000 pyllicagram-1.6/src/pyllicagram/__init__.py
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 16:34:53.932542 pyllicagram-1.6/src/pyllicagram.egg-info/
--rw-r--r--   0 benoit2c   (501) staff       (20)      274 2023-04-09 16:34:53.000000 pyllicagram-1.6/src/pyllicagram.egg-info/PKG-INFO
--rw-r--r--   0 benoit2c   (501) staff       (20)      240 2023-04-09 16:34:53.000000 pyllicagram-1.6/src/pyllicagram.egg-info/SOURCES.txt
--rw-r--r--   0 benoit2c   (501) staff       (20)        1 2023-04-09 16:34:53.000000 pyllicagram-1.6/src/pyllicagram.egg-info/dependency_links.txt
--rw-r--r--   0 benoit2c   (501) staff       (20)        7 2023-04-09 16:34:53.000000 pyllicagram-1.6/src/pyllicagram.egg-info/requires.txt
--rw-r--r--   0 benoit2c   (501) staff       (20)       12 2023-04-09 16:34:53.000000 pyllicagram-1.6/src/pyllicagram.egg-info/top_level.txt
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 16:49:29.373391 pyllicagram-1.7/
+-rw-r--r--   0 benoit2c   (501) staff       (20)      274 2023-04-09 16:49:29.372666 pyllicagram-1.7/PKG-INFO
+-rw-r--r--   0 benoit2c   (501) staff       (20)     4137 2023-04-09 16:45:51.000000 pyllicagram-1.7/README.md
+-rw-r--r--   0 benoit2c   (501) staff       (20)       38 2023-04-09 16:49:29.373631 pyllicagram-1.7/setup.cfg
+-rw-r--r--   0 benoit2c   (501) staff       (20)      404 2023-04-09 16:48:38.000000 pyllicagram-1.7/setup.py
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 16:49:29.368091 pyllicagram-1.7/src/
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 16:49:29.369439 pyllicagram-1.7/src/pyllicagram/
+-rw-r--r--   0 benoit2c   (501) staff       (20)     2421 2023-04-09 16:45:51.000000 pyllicagram-1.7/src/pyllicagram/__init__.py
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 16:49:29.371902 pyllicagram-1.7/src/pyllicagram.egg-info/
+-rw-r--r--   0 benoit2c   (501) staff       (20)      274 2023-04-09 16:49:29.000000 pyllicagram-1.7/src/pyllicagram.egg-info/PKG-INFO
+-rw-r--r--   0 benoit2c   (501) staff       (20)      240 2023-04-09 16:49:29.000000 pyllicagram-1.7/src/pyllicagram.egg-info/SOURCES.txt
+-rw-r--r--   0 benoit2c   (501) staff       (20)        1 2023-04-09 16:49:29.000000 pyllicagram-1.7/src/pyllicagram.egg-info/dependency_links.txt
+-rw-r--r--   0 benoit2c   (501) staff       (20)        7 2023-04-09 16:49:29.000000 pyllicagram-1.7/src/pyllicagram.egg-info/requires.txt
+-rw-r--r--   0 benoit2c   (501) staff       (20)       12 2023-04-09 16:49:29.000000 pyllicagram-1.7/src/pyllicagram.egg-info/top_level.txt
```

### Comparing `pyllicagram-1.6/README.md` & `pyllicagram-1.7/README.md`

 * *Files identical despite different names*

### Comparing `pyllicagram-1.6/src/pyllicagram/__init__.py` & `pyllicagram-1.7/src/pyllicagram/__init__.py`

 * *Files identical despite different names*

