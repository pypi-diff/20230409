# Comparing `tmp/bugs-chart.py-1.0.1.tar.gz` & `tmp/bugs-chart.py-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bugs-chart.py-1.0.1.tar", last modified: Sun Apr  9 05:08:20 2023, max compression
+gzip compressed data, was "bugs-chart.py-1.0.2.tar", last modified: Sun Apr  9 05:11:59 2023, max compression
```

## Comparing `bugs-chart.py-1.0.1.tar` & `bugs-chart.py-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jieunpark   (501) staff       (20)        0 2023-04-09 05:08:20.732907 bugs-chart.py-1.0.1/
--rw-r--r--   0 jieunpark   (501) staff       (20)     1074 2023-04-09 04:50:14.000000 bugs-chart.py-1.0.1/LICENSE
--rw-r--r--   0 jieunpark   (501) staff       (20)      252 2023-04-09 05:08:20.732803 bugs-chart.py-1.0.1/PKG-INFO
--rw-r--r--   0 jieunpark   (501) staff       (20)     1561 2023-04-09 04:49:16.000000 bugs-chart.py-1.0.1/README.md
--rw-r--r--   0 jieunpark   (501) staff       (20)     4439 2023-04-09 04:58:38.000000 bugs-chart.py-1.0.1/bugs.py
-drwxr-xr-x   0 jieunpark   (501) staff       (20)        0 2023-04-09 05:08:20.732637 bugs-chart.py-1.0.1/bugs_chart.py.egg-info/
--rw-r--r--   0 jieunpark   (501) staff       (20)      252 2023-04-09 05:08:20.000000 bugs-chart.py-1.0.1/bugs_chart.py.egg-info/PKG-INFO
--rw-r--r--   0 jieunpark   (501) staff       (20)      218 2023-04-09 05:08:20.000000 bugs-chart.py-1.0.1/bugs_chart.py.egg-info/SOURCES.txt
--rw-r--r--   0 jieunpark   (501) staff       (20)        1 2023-04-09 05:08:20.000000 bugs-chart.py-1.0.1/bugs_chart.py.egg-info/dependency_links.txt
--rw-r--r--   0 jieunpark   (501) staff       (20)       17 2023-04-09 05:08:20.000000 bugs-chart.py-1.0.1/bugs_chart.py.egg-info/requires.txt
--rw-r--r--   0 jieunpark   (501) staff       (20)        5 2023-04-09 05:08:20.000000 bugs-chart.py-1.0.1/bugs_chart.py.egg-info/top_level.txt
--rw-r--r--   0 jieunpark   (501) staff       (20)       38 2023-04-09 05:08:20.732947 bugs-chart.py-1.0.1/setup.cfg
--rw-r--r--   0 jieunpark   (501) staff       (20)      449 2023-04-09 05:07:31.000000 bugs-chart.py-1.0.1/setup.py
+drwxr-xr-x   0 jieunpark   (501) staff       (20)        0 2023-04-09 05:11:59.498734 bugs-chart.py-1.0.2/
+-rw-r--r--   0 jieunpark   (501) staff       (20)     1074 2023-04-09 04:50:14.000000 bugs-chart.py-1.0.2/LICENSE
+-rw-r--r--   0 jieunpark   (501) staff       (20)     1855 2023-04-09 05:11:59.498634 bugs-chart.py-1.0.2/PKG-INFO
+-rw-r--r--   0 jieunpark   (501) staff       (20)     1561 2023-04-09 04:49:16.000000 bugs-chart.py-1.0.2/README.md
+-rw-r--r--   0 jieunpark   (501) staff       (20)     4439 2023-04-09 04:58:38.000000 bugs-chart.py-1.0.2/bugs.py
+drwxr-xr-x   0 jieunpark   (501) staff       (20)        0 2023-04-09 05:11:59.498471 bugs-chart.py-1.0.2/bugs_chart.py.egg-info/
+-rw-r--r--   0 jieunpark   (501) staff       (20)     1855 2023-04-09 05:11:59.000000 bugs-chart.py-1.0.2/bugs_chart.py.egg-info/PKG-INFO
+-rw-r--r--   0 jieunpark   (501) staff       (20)      218 2023-04-09 05:11:59.000000 bugs-chart.py-1.0.2/bugs_chart.py.egg-info/SOURCES.txt
+-rw-r--r--   0 jieunpark   (501) staff       (20)        1 2023-04-09 05:11:59.000000 bugs-chart.py-1.0.2/bugs_chart.py.egg-info/dependency_links.txt
+-rw-r--r--   0 jieunpark   (501) staff       (20)       17 2023-04-09 05:11:59.000000 bugs-chart.py-1.0.2/bugs_chart.py.egg-info/requires.txt
+-rw-r--r--   0 jieunpark   (501) staff       (20)        5 2023-04-09 05:11:59.000000 bugs-chart.py-1.0.2/bugs_chart.py.egg-info/top_level.txt
+-rw-r--r--   0 jieunpark   (501) staff       (20)       38 2023-04-09 05:11:59.498770 bugs-chart.py-1.0.2/setup.cfg
+-rw-r--r--   0 jieunpark   (501) staff       (20)      539 2023-04-09 05:10:37.000000 bugs-chart.py-1.0.2/setup.py
```

### Comparing `bugs-chart.py-1.0.1/LICENSE` & `bugs-chart.py-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bugs-chart.py-1.0.1/README.md` & `bugs-chart.py-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bugs-chart.py-1.0.1/bugs.py` & `bugs-chart.py-1.0.2/bugs.py`

 * *Files identical despite different names*

