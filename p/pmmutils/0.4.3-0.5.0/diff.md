# Comparing `tmp/pmmutils-0.4.3.tar.gz` & `tmp/pmmutils-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmmutils-0.4.3.tar", last modified: Mon Mar 27 13:38:16 2023, max compression
+gzip compressed data, was "pmmutils-0.5.0.tar", last modified: Sun Apr  9 18:41:03 2023, max compression
```

## Comparing `pmmutils-0.4.3.tar` & `pmmutils-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:38:16.374852 pmmutils-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-27 13:38:02.000000 pmmutils-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-03-27 13:38:16.374852 pmmutils-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-03-27 13:38:02.000000 pmmutils-0.4.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:38:16.374852 pmmutils-0.4.3/pmmutils/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-27 13:38:02.000000 pmmutils-0.4.3/pmmutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-03-27 13:38:02.000000 pmmutils-0.4.3/pmmutils/args.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-27 13:38:02.000000 pmmutils-0.4.3/pmmutils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22188 2023-03-27 13:38:02.000000 pmmutils-0.4.3/pmmutils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    31561 2023-03-27 13:38:02.000000 pmmutils-0.4.3/pmmutils/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-03-27 13:38:02.000000 pmmutils-0.4.3/pmmutils/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-03-27 13:38:02.000000 pmmutils-0.4.3/pmmutils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 13:38:16.374852 pmmutils-0.4.3/pmmutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-03-27 13:38:16.000000 pmmutils-0.4.3/pmmutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-27 13:38:16.000000 pmmutils-0.4.3/pmmutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 13:38:16.000000 pmmutils-0.4.3/pmmutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-27 13:38:16.000000 pmmutils-0.4.3/pmmutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-27 13:38:16.000000 pmmutils-0.4.3/pmmutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 13:38:16.374852 pmmutils-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-03-27 13:38:02.000000 pmmutils-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:41:03.981987 pmmutils-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-09 18:40:50.000000 pmmutils-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-09 18:41:03.981987 pmmutils-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-09 18:40:50.000000 pmmutils-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:41:03.981987 pmmutils-0.5.0/pmmutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-09 18:40:50.000000 pmmutils-0.5.0/pmmutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-04-09 18:40:50.000000 pmmutils-0.5.0/pmmutils/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-09 18:40:50.000000 pmmutils-0.5.0/pmmutils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22188 2023-04-09 18:40:50.000000 pmmutils-0.5.0/pmmutils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31561 2023-04-09 18:40:50.000000 pmmutils-0.5.0/pmmutils/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-09 18:40:50.000000 pmmutils-0.5.0/pmmutils/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-09 18:40:50.000000 pmmutils-0.5.0/pmmutils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:41:03.981987 pmmutils-0.5.0/pmmutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-09 18:41:03.000000 pmmutils-0.5.0/pmmutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-09 18:41:03.000000 pmmutils-0.5.0/pmmutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 18:41:03.000000 pmmutils-0.5.0/pmmutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-09 18:41:03.000000 pmmutils-0.5.0/pmmutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 18:41:03.000000 pmmutils-0.5.0/pmmutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 18:41:03.981987 pmmutils-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-09 18:40:50.000000 pmmutils-0.5.0/setup.py
```

### Comparing `pmmutils-0.4.3/LICENSE` & `pmmutils-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pmmutils-0.4.3/PKG-INFO` & `pmmutils-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmmutils
-Version: 0.4.3
+Version: 0.5.0
 Summary: Util Methods for PMM
 Home-page: https://github.com/meisnate12/pmmutils
 Author: Nathan Taggart
 Author-email: meisnate12@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/meisnate12/pmmutils
 Project-URL: Funding, https://github.com/sponsors/meisnate12
```

### Comparing `pmmutils-0.4.3/README.rst` & `pmmutils-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `pmmutils-0.4.3/pmmutils/__init__.py` & `pmmutils-0.5.0/pmmutils/__init__.py`

 * *Files identical despite different names*

### Comparing `pmmutils-0.4.3/pmmutils/args.py` & `pmmutils-0.5.0/pmmutils/args.py`

 * *Files identical despite different names*

### Comparing `pmmutils-0.4.3/pmmutils/logging.py` & `pmmutils-0.5.0/pmmutils/logging.py`

 * *Files identical despite different names*

### Comparing `pmmutils-0.4.3/pmmutils/schedule.py` & `pmmutils-0.5.0/pmmutils/schedule.py`

 * *Files identical despite different names*

### Comparing `pmmutils-0.4.3/pmmutils/util.py` & `pmmutils-0.5.0/pmmutils/util.py`

 * *Files identical despite different names*

### Comparing `pmmutils-0.4.3/pmmutils/yaml.py` & `pmmutils-0.5.0/pmmutils/yaml.py`

 * *Files identical despite different names*

### Comparing `pmmutils-0.4.3/pmmutils.egg-info/PKG-INFO` & `pmmutils-0.5.0/pmmutils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmmutils
-Version: 0.4.3
+Version: 0.5.0
 Summary: Util Methods for PMM
 Home-page: https://github.com/meisnate12/pmmutils
 Author: Nathan Taggart
 Author-email: meisnate12@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/meisnate12/pmmutils
 Project-URL: Funding, https://github.com/sponsors/meisnate12
```

### Comparing `pmmutils-0.4.3/setup.py` & `pmmutils-0.5.0/setup.py`

 * *Files identical despite different names*

