# Comparing `tmp/kdot-0.0.1.tar.gz` & `tmp/kdot-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kdot-0.0.1.tar", last modified: Sun Apr  9 21:46:07 2023, max compression
+gzip compressed data, was "kdot-0.0.3.tar", last modified: Sun Apr  9 21:56:32 2023, max compression
```

## Comparing `kdot-0.0.1.tar` & `kdot-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:46:07.904280 kdot-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-09 21:45:58.000000 kdot-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-09 21:46:07.904280 kdot-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-09 21:45:58.000000 kdot-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:46:07.904280 kdot-0.0.1/kdot/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-09 21:45:58.000000 kdot-0.0.1/kdot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-09 21:45:58.000000 kdot-0.0.1/kdot/kdot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:46:07.904280 kdot-0.0.1/kdot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-09 21:46:07.000000 kdot-0.0.1/kdot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-09 21:46:07.000000 kdot-0.0.1/kdot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 21:46:07.000000 kdot-0.0.1/kdot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 21:46:07.000000 kdot-0.0.1/kdot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 21:46:07.904280 kdot-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-09 21:45:58.000000 kdot-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:56:32.176102 kdot-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-09 21:56:22.000000 kdot-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-09 21:56:32.176102 kdot-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-09 21:56:22.000000 kdot-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:56:32.176102 kdot-0.0.3/kdot/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-09 21:56:22.000000 kdot-0.0.3/kdot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:56:32.176102 kdot-0.0.3/kdot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-09 21:56:32.000000 kdot-0.0.3/kdot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-09 21:56:32.000000 kdot-0.0.3/kdot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 21:56:32.000000 kdot-0.0.3/kdot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 21:56:32.000000 kdot-0.0.3/kdot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 21:56:32.176102 kdot-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-09 21:56:22.000000 kdot-0.0.3/setup.py
```

### Comparing `kdot-0.0.1/LICENSE` & `kdot-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kdot-0.0.1/setup.py` & `kdot-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.1"
+VERSION = "0.0.3"
 DESCRIPTION = "A anti skid package"
 LONG_DESCRIPTION = (
     "A package that makes it easy to add anti skid to all of your (my) repos"
 )
 
 setup(
     name="kdot",
```

