# Comparing `tmp/erutils-1.2.2.2.tar.gz` & `tmp/Erutils-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erutils-1.2.2.2.tar", last modified: Sat Apr  1 07:40:18 2023, max compression
+gzip compressed data, was "Erutils-1.3.0.tar", last modified: Sun Apr  9 18:01:41 2023, max compression
```

## Comparing `erutils-1.2.2.2.tar` & `Erutils-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 07:40:18.659895 erutils-1.2.2.2/
--rw-rw-rw-   0        0        0     1864 2023-04-01 07:40:18.658896 erutils-1.2.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1262 2023-03-31 13:01:16.000000 erutils-1.2.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-01 07:40:18.626905 erutils-1.2.2.2/erutils/
--rw-rw-rw-   0        0        0      631 2023-03-16 17:34:01.000000 erutils-1.2.2.2/erutils/__init__.py
--rw-rw-rw-   0        0        0      169 2023-03-04 18:12:30.000000 erutils-1.2.2.2/erutils/__main__.py
--rw-rw-rw-   0        0        0       69 2023-03-25 19:08:12.000000 erutils-1.2.2.2/erutils/config.py
--rw-rw-rw-   0        0        0    32172 2023-03-16 17:38:36.000000 erutils-1.2.2.2/erutils/lightning.py
--rw-rw-rw-   0        0        0     3485 2023-03-25 19:08:12.000000 erutils-1.2.2.2/erutils/loggers.py
--rw-rw-rw-   0        0        0    48407 2023-04-01 07:38:28.000000 erutils-1.2.2.2/erutils/nn.py
--rw-rw-rw-   0        0        0    13359 2023-03-31 12:56:45.000000 erutils-1.2.2.2/erutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-01 07:40:18.656896 erutils-1.2.2.2/erutils.egg-info/
--rw-rw-rw-   0        0        0     1864 2023-04-01 07:40:18.000000 erutils-1.2.2.2/erutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-04-01 07:40:18.000000 erutils-1.2.2.2/erutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-01 07:40:18.000000 erutils-1.2.2.2/erutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-04-01 07:40:18.000000 erutils-1.2.2.2/erutils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-12-21 19:40:03.000000 erutils-1.2.2.2/erutils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      213 2023-04-01 07:40:18.000000 erutils-1.2.2.2/erutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-01 07:40:18.000000 erutils-1.2.2.2/erutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1044 2023-04-01 07:39:57.000000 erutils-1.2.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-01 07:40:18.659895 erutils-1.2.2.2/setup.cfg
--rw-rw-rw-   0        0        0      684 2023-04-01 07:39:45.000000 erutils-1.2.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 18:01:41.652065 Erutils-1.3.0/
+drwxrwxrwx   0        0        0        0 2023-04-09 18:01:41.634993 Erutils-1.3.0/Erutils/
+-rw-rw-rw-   0        0        0      631 2023-04-09 17:44:30.000000 Erutils-1.3.0/Erutils/__init__.py
+-rw-rw-rw-   0        0        0      169 2023-04-09 17:44:30.000000 Erutils-1.3.0/Erutils/__main__.py
+-rw-rw-rw-   0        0        0       69 2023-04-09 17:44:30.000000 Erutils-1.3.0/Erutils/config.py
+-rw-rw-rw-   0        0        0    32172 2023-04-09 17:44:30.000000 Erutils-1.3.0/Erutils/lightning.py
+-rw-rw-rw-   0        0        0     3485 2023-04-09 17:44:30.000000 Erutils-1.3.0/Erutils/loggers.py
+-rw-rw-rw-   0        0        0    48407 2023-04-09 17:44:30.000000 Erutils-1.3.0/Erutils/nn.py
+-rw-rw-rw-   0        0        0    13359 2023-04-09 17:44:30.000000 Erutils-1.3.0/Erutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-09 18:01:41.644487 Erutils-1.3.0/Erutils.egg-info/
+-rw-rw-rw-   0        0        0     3075 2023-04-09 18:01:41.000000 Erutils-1.3.0/Erutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-04-09 18:01:41.000000 Erutils-1.3.0/Erutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 18:01:41.000000 Erutils-1.3.0/Erutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-04-09 18:01:41.000000 Erutils-1.3.0/Erutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-09 18:01:41.000000 Erutils-1.3.0/Erutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3075 2023-04-09 18:01:41.645487 Erutils-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2355 2023-04-09 17:59:20.000000 Erutils-1.3.0/README.md
+-rw-rw-rw-   0        0        0      601 2023-04-09 17:44:30.000000 Erutils-1.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-09 18:01:41.652065 Erutils-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1249 2023-04-09 18:01:29.000000 Erutils-1.3.0/setup.py
```

### Comparing `erutils-1.2.2.2/erutils/__init__.py` & `Erutils-1.3.0/Erutils/__init__.py`

 * *Files identical despite different names*

### Comparing `erutils-1.2.2.2/erutils/lightning.py` & `Erutils-1.3.0/Erutils/lightning.py`

 * *Files identical despite different names*

### Comparing `erutils-1.2.2.2/erutils/loggers.py` & `Erutils-1.3.0/Erutils/loggers.py`

 * *Files identical despite different names*

### Comparing `erutils-1.2.2.2/erutils/nn.py` & `Erutils-1.3.0/Erutils/nn.py`

 * *Files identical despite different names*

### Comparing `erutils-1.2.2.2/erutils/utils.py` & `Erutils-1.3.0/Erutils/utils.py`

 * *Files identical despite different names*

