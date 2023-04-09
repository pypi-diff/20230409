# Comparing `tmp/opsgenielib-0.0.8.tar.gz` & `tmp/opsgenielib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opsgenielib-0.0.8.tar", last modified: Tue May 28 10:52:27 2019, max compression
+gzip compressed data, was "dist/opsgenielib-0.0.9.tar", last modified: Tue May 28 11:45:35 2019, max compression
```

## Comparing `opsgenielib-0.0.8.tar` & `opsgenielib-0.0.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)        0 2019-05-28 10:52:27.000000 opsgenielib-0.0.8/
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)        5 2019-05-28 10:51:39.000000 opsgenielib-0.0.8/.VERSION
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)      171 2019-05-25 15:26:32.000000 opsgenielib-0.0.8/AUTHORS.rst
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)     1292 2019-05-26 18:22:31.000000 opsgenielib-0.0.8/CONTRIBUTING.rst
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)       97 2019-04-12 08:57:45.000000 opsgenielib-0.0.8/HISTORY.rst
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)     1063 2019-04-12 08:57:45.000000 opsgenielib-0.0.8/LICENSE
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)      396 2019-05-26 18:22:22.000000 opsgenielib-0.0.8/MANIFEST.in
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)     3503 2019-05-28 10:52:27.000000 opsgenielib-0.0.8/PKG-INFO
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      546 2019-05-26 18:01:17.000000 opsgenielib-0.0.8/Pipfile
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)    28043 2019-05-28 10:52:26.000000 opsgenielib-0.0.8/Pipfile.lock
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)     2265 2019-05-26 18:22:10.000000 opsgenielib-0.0.8/README.rst
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      901 2019-05-26 18:21:56.000000 opsgenielib-0.0.8/USAGE.rst
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      538 2019-05-28 10:52:26.000000 opsgenielib-0.0.8/dev-requirements.txt
-drwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)        0 2019-05-28 10:52:27.000000 opsgenielib-0.0.8/docs/
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)     6782 2019-05-26 18:22:26.000000 opsgenielib-0.0.8/docs/Makefile
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)       28 2019-04-12 08:57:45.000000 opsgenielib-0.0.8/docs/authors.rst
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)     8917 2019-05-26 18:21:52.000000 opsgenielib-0.0.8/docs/conf.py
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)       33 2019-04-12 08:57:45.000000 opsgenielib-0.0.8/docs/contributing.rst
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)       28 2019-04-12 08:57:45.000000 opsgenielib-0.0.8/docs/history.rst
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)      507 2019-05-26 18:22:29.000000 opsgenielib-0.0.8/docs/index.rst
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)       33 2019-04-12 08:57:45.000000 opsgenielib-0.0.8/docs/installation.rst
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)       27 2019-04-12 08:57:45.000000 opsgenielib-0.0.8/docs/readme.rst
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)       26 2019-04-12 08:57:45.000000 opsgenielib-0.0.8/docs/usage.rst
-drwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)        0 2019-05-28 10:52:27.000000 opsgenielib-0.0.8/opsgenielib/
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)        5 2019-05-28 10:52:26.000000 opsgenielib-0.0.8/opsgenielib/.VERSION
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)      171 2019-05-28 10:52:26.000000 opsgenielib-0.0.8/opsgenielib/AUTHORS.rst
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)     1292 2019-05-28 10:52:26.000000 opsgenielib-0.0.8/opsgenielib/CONTRIBUTING.rst
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)       97 2019-05-28 10:52:26.000000 opsgenielib-0.0.8/opsgenielib/HISTORY.rst
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)     1063 2019-05-28 10:52:26.000000 opsgenielib-0.0.8/opsgenielib/LICENSE
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      546 2019-05-28 10:52:26.000000 opsgenielib-0.0.8/opsgenielib/Pipfile
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)    28043 2019-05-28 10:52:26.000000 opsgenielib-0.0.8/opsgenielib/Pipfile.lock
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)     2265 2019-05-28 10:52:26.000000 opsgenielib-0.0.8/opsgenielib/README.rst
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      901 2019-05-28 10:52:26.000000 opsgenielib-0.0.8/opsgenielib/USAGE.rst
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)     1976 2019-05-26 18:22:20.000000 opsgenielib-0.0.8/opsgenielib/__init__.py
-drwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)        0 2019-05-28 10:52:27.000000 opsgenielib-0.0.8/opsgenielib/__pycache__/
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      823 2019-05-26 19:51:55.000000 opsgenielib-0.0.8/opsgenielib/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      930 2019-05-22 17:54:55.000000 opsgenielib-0.0.8/opsgenielib/__pycache__/_version.cpython-37.pyc
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)    20422 2019-05-27 08:40:27.000000 opsgenielib-0.0.8/opsgenielib/__pycache__/opsgenielib.cpython-37.pyc
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      851 2019-05-26 19:51:56.000000 opsgenielib-0.0.8/opsgenielib/__pycache__/opsgenielibexceptions.cpython-37.pyc
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)     2108 2019-04-12 08:57:45.000000 opsgenielib-0.0.8/opsgenielib/_version.py
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      538 2019-05-28 10:52:26.000000 opsgenielib-0.0.8/opsgenielib/dev-requirements.txt
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)    23952 2019-05-28 10:51:22.000000 opsgenielib-0.0.8/opsgenielib/opsgenielib.py
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)     1801 2019-05-26 18:22:14.000000 opsgenielib-0.0.8/opsgenielib/opsgenielibexceptions.py
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      363 2019-05-28 10:52:26.000000 opsgenielib-0.0.8/opsgenielib/requirements.txt
-drwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)        0 2019-05-28 10:52:27.000000 opsgenielib-0.0.8/opsgenielib.egg-info/
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)     3503 2019-05-28 10:52:26.000000 opsgenielib-0.0.8/opsgenielib.egg-info/PKG-INFO
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)     1117 2019-05-28 10:52:26.000000 opsgenielib-0.0.8/opsgenielib.egg-info/SOURCES.txt
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)        1 2019-05-28 10:52:26.000000 opsgenielib-0.0.8/opsgenielib.egg-info/dependency_links.txt
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)        1 2019-05-26 18:29:30.000000 opsgenielib-0.0.8/opsgenielib.egg-info/not-zip-safe
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)       30 2019-05-28 10:52:26.000000 opsgenielib-0.0.8/opsgenielib.egg-info/requires.txt
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)       12 2019-05-28 10:52:26.000000 opsgenielib-0.0.8/opsgenielib.egg-info/top_level.txt
--rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      363 2019-05-28 10:52:26.000000 opsgenielib-0.0.8/requirements.txt
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)      151 2019-05-28 10:52:27.000000 opsgenielib-0.0.8/setup.cfg
--rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)     1933 2019-05-26 18:41:34.000000 opsgenielib-0.0.8/setup.py
+drwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)        0 2019-05-28 11:45:35.000000 opsgenielib-0.0.9/
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)        5 2019-05-28 11:44:21.000000 opsgenielib-0.0.9/.VERSION
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)      171 2019-05-25 15:26:32.000000 opsgenielib-0.0.9/AUTHORS.rst
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)     1292 2019-05-26 18:22:31.000000 opsgenielib-0.0.9/CONTRIBUTING.rst
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)       97 2019-04-12 08:57:45.000000 opsgenielib-0.0.9/HISTORY.rst
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)     1063 2019-04-12 08:57:45.000000 opsgenielib-0.0.9/LICENSE
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)      396 2019-05-26 18:22:22.000000 opsgenielib-0.0.9/MANIFEST.in
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)     3503 2019-05-28 11:45:35.000000 opsgenielib-0.0.9/PKG-INFO
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      546 2019-05-26 18:01:17.000000 opsgenielib-0.0.9/Pipfile
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)    28043 2019-05-28 11:45:34.000000 opsgenielib-0.0.9/Pipfile.lock
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)     2265 2019-05-26 18:22:10.000000 opsgenielib-0.0.9/README.rst
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      901 2019-05-26 18:21:56.000000 opsgenielib-0.0.9/USAGE.rst
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      538 2019-05-28 11:45:34.000000 opsgenielib-0.0.9/dev-requirements.txt
+drwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)        0 2019-05-28 11:45:35.000000 opsgenielib-0.0.9/docs/
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)     6782 2019-05-26 18:22:26.000000 opsgenielib-0.0.9/docs/Makefile
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)       28 2019-04-12 08:57:45.000000 opsgenielib-0.0.9/docs/authors.rst
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)     8917 2019-05-26 18:21:52.000000 opsgenielib-0.0.9/docs/conf.py
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)       33 2019-04-12 08:57:45.000000 opsgenielib-0.0.9/docs/contributing.rst
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)       28 2019-04-12 08:57:45.000000 opsgenielib-0.0.9/docs/history.rst
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)      507 2019-05-26 18:22:29.000000 opsgenielib-0.0.9/docs/index.rst
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)       33 2019-04-12 08:57:45.000000 opsgenielib-0.0.9/docs/installation.rst
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)       27 2019-04-12 08:57:45.000000 opsgenielib-0.0.9/docs/readme.rst
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)       26 2019-04-12 08:57:45.000000 opsgenielib-0.0.9/docs/usage.rst
+drwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)        0 2019-05-28 11:45:35.000000 opsgenielib-0.0.9/opsgenielib/
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)        5 2019-05-28 11:45:34.000000 opsgenielib-0.0.9/opsgenielib/.VERSION
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)      171 2019-05-28 11:45:34.000000 opsgenielib-0.0.9/opsgenielib/AUTHORS.rst
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)     1292 2019-05-28 11:45:34.000000 opsgenielib-0.0.9/opsgenielib/CONTRIBUTING.rst
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)       97 2019-05-28 11:45:34.000000 opsgenielib-0.0.9/opsgenielib/HISTORY.rst
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)     1063 2019-05-28 11:45:34.000000 opsgenielib-0.0.9/opsgenielib/LICENSE
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      546 2019-05-28 11:45:34.000000 opsgenielib-0.0.9/opsgenielib/Pipfile
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)    28043 2019-05-28 11:45:34.000000 opsgenielib-0.0.9/opsgenielib/Pipfile.lock
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)     2265 2019-05-28 11:45:34.000000 opsgenielib-0.0.9/opsgenielib/README.rst
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      901 2019-05-28 11:45:34.000000 opsgenielib-0.0.9/opsgenielib/USAGE.rst
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)     1976 2019-05-26 18:22:20.000000 opsgenielib-0.0.9/opsgenielib/__init__.py
+drwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)        0 2019-05-28 11:45:35.000000 opsgenielib-0.0.9/opsgenielib/__pycache__/
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      823 2019-05-26 19:51:55.000000 opsgenielib-0.0.9/opsgenielib/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      930 2019-05-22 17:54:55.000000 opsgenielib-0.0.9/opsgenielib/__pycache__/_version.cpython-37.pyc
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)    20422 2019-05-27 08:40:27.000000 opsgenielib-0.0.9/opsgenielib/__pycache__/opsgenielib.cpython-37.pyc
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      851 2019-05-26 19:51:56.000000 opsgenielib-0.0.9/opsgenielib/__pycache__/opsgenielibexceptions.cpython-37.pyc
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)     2108 2019-04-12 08:57:45.000000 opsgenielib-0.0.9/opsgenielib/_version.py
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      538 2019-05-28 11:45:34.000000 opsgenielib-0.0.9/opsgenielib/dev-requirements.txt
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)    23938 2019-05-28 11:44:35.000000 opsgenielib-0.0.9/opsgenielib/opsgenielib.py
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)     1801 2019-05-26 18:22:14.000000 opsgenielib-0.0.9/opsgenielib/opsgenielibexceptions.py
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      363 2019-05-28 11:45:34.000000 opsgenielib-0.0.9/opsgenielib/requirements.txt
+drwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)        0 2019-05-28 11:45:35.000000 opsgenielib-0.0.9/opsgenielib.egg-info/
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)     3503 2019-05-28 11:45:35.000000 opsgenielib-0.0.9/opsgenielib.egg-info/PKG-INFO
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)     1117 2019-05-28 11:45:35.000000 opsgenielib-0.0.9/opsgenielib.egg-info/SOURCES.txt
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)        1 2019-05-28 11:45:35.000000 opsgenielib-0.0.9/opsgenielib.egg-info/dependency_links.txt
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)        1 2019-05-26 18:29:30.000000 opsgenielib-0.0.9/opsgenielib.egg-info/not-zip-safe
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)       30 2019-05-28 11:45:35.000000 opsgenielib-0.0.9/opsgenielib.egg-info/requires.txt
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)       12 2019-05-28 11:45:35.000000 opsgenielib-0.0.9/opsgenielib.egg-info/top_level.txt
+-rw-r--r--   0 yhoorneman (839247727) SBP\Domain Users (450652656)      363 2019-05-28 11:45:34.000000 opsgenielib-0.0.9/requirements.txt
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)      151 2019-05-28 11:45:35.000000 opsgenielib-0.0.9/setup.cfg
+-rwxr-xr-x   0 yhoorneman (839247727) SBP\Domain Users (450652656)     1933 2019-05-26 18:41:34.000000 opsgenielib-0.0.9/setup.py
```

### Comparing `opsgenielib-0.0.8/CONTRIBUTING.rst` & `opsgenielib-0.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/LICENSE` & `opsgenielib-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/PKG-INFO` & `opsgenielib-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: opsgenielib
-Version: 0.0.8
+Version: 0.0.9
 Summary: opsgenielib
 Home-page: https://sbp.gitlab.schubergphilis.com/Services/SaaS/Dummy/opsgenielib
 Author: Yorick Hoorneman
 Author-email: yhoorneman@schubergphilis.com
 License: MIT
 Description: ===========
         opsgenielib
```

### Comparing `opsgenielib-0.0.8/Pipfile` & `opsgenielib-0.0.9/Pipfile`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/Pipfile.lock` & `opsgenielib-0.0.9/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/README.rst` & `opsgenielib-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/USAGE.rst` & `opsgenielib-0.0.9/USAGE.rst`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/dev-requirements.txt` & `opsgenielib-0.0.9/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/docs/Makefile` & `opsgenielib-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/docs/conf.py` & `opsgenielib-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/opsgenielib/CONTRIBUTING.rst` & `opsgenielib-0.0.9/opsgenielib/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/opsgenielib/LICENSE` & `opsgenielib-0.0.9/opsgenielib/LICENSE`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/opsgenielib/Pipfile` & `opsgenielib-0.0.9/opsgenielib/Pipfile`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/opsgenielib/Pipfile.lock` & `opsgenielib-0.0.9/opsgenielib/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/opsgenielib/README.rst` & `opsgenielib-0.0.9/opsgenielib/README.rst`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/opsgenielib/USAGE.rst` & `opsgenielib-0.0.9/opsgenielib/USAGE.rst`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/opsgenielib/__init__.py` & `opsgenielib-0.0.9/opsgenielib/__init__.py`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/opsgenielib/__pycache__/__init__.cpython-37.pyc` & `opsgenielib-0.0.9/opsgenielib/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/opsgenielib/__pycache__/_version.cpython-37.pyc` & `opsgenielib-0.0.9/opsgenielib/__pycache__/_version.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/opsgenielib/__pycache__/opsgenielib.cpython-37.pyc` & `opsgenielib-0.0.9/opsgenielib/__pycache__/opsgenielib.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/opsgenielib/__pycache__/opsgenielibexceptions.cpython-37.pyc` & `opsgenielib-0.0.9/opsgenielib/__pycache__/opsgenielibexceptions.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/opsgenielib/_version.py` & `opsgenielib-0.0.9/opsgenielib/_version.py`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/opsgenielib/dev-requirements.txt` & `opsgenielib-0.0.9/opsgenielib/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/opsgenielib/opsgenielib.py` & `opsgenielib-0.0.9/opsgenielib/opsgenielib.py`

 * *Files 0% similar despite different names*

```diff
@@ -548,15 +548,15 @@
             },
             "startDate": f"{start_date}",
             "endDate": f"{end_date}"
         }
         self._logger.debug('Making a call to "%s"', url)
         response = self._session.post(url, json=payload)
         response.raise_for_status()
-        return response.json()
+        return response
 
     def set_override_scheduled(self, team_name, start_date, end_date, user):
         """Overrides the on-call user of an opsgenie team, based on the team name.
 
         Note:
         Start and End date format example: 2019-03-15T14:34:09Z.
         opsgenie uses UTC, time entered might be different.
@@ -573,8 +573,8 @@
             },
             "startDate": f"{start_date_utc}",
             "endDate": f"{end_date_utc}"
         }
         self._logger.debug('Making a call to "%s"', url)
         response = self._session.post(url, json=payload)
         response.raise_for_status()
-        return response.json()
+        return response
```

### Comparing `opsgenielib-0.0.8/opsgenielib/opsgenielibexceptions.py` & `opsgenielib-0.0.9/opsgenielib/opsgenielibexceptions.py`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/opsgenielib.egg-info/PKG-INFO` & `opsgenielib-0.0.9/opsgenielib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: opsgenielib
-Version: 0.0.8
+Version: 0.0.9
 Summary: opsgenielib
 Home-page: https://sbp.gitlab.schubergphilis.com/Services/SaaS/Dummy/opsgenielib
 Author: Yorick Hoorneman
 Author-email: yhoorneman@schubergphilis.com
 License: MIT
 Description: ===========
         opsgenielib
```

### Comparing `opsgenielib-0.0.8/opsgenielib.egg-info/SOURCES.txt` & `opsgenielib-0.0.9/opsgenielib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opsgenielib-0.0.8/setup.py` & `opsgenielib-0.0.9/setup.py`

 * *Files identical despite different names*

