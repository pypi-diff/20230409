# Comparing `tmp/naruno_remote_app-0.53.0.tar.gz` & `tmp/naruno_remote_app-0.54.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naruno_remote_app-0.53.0.tar", last modified: Tue Apr  4 12:12:05 2023, max compression
+gzip compressed data, was "naruno_remote_app-0.54.0.tar", last modified: Sat Apr  8 23:33:50 2023, max compression
```

## Comparing `naruno_remote_app-0.53.0.tar` & `naruno_remote_app-0.54.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:12:05.406749 naruno_remote_app-0.53.0/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-04 12:12:05.406749 naruno_remote_app-0.53.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:12:05.406749 naruno_remote_app-0.53.0/naruno_remote_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-04 12:12:05.000000 naruno_remote_app-0.53.0/naruno_remote_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-04 12:12:05.000000 naruno_remote_app-0.53.0/naruno_remote_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 12:12:05.000000 naruno_remote_app-0.53.0/naruno_remote_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 12:12:05.000000 naruno_remote_app-0.53.0/naruno_remote_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-04 12:12:05.000000 naruno_remote_app-0.53.0/naruno_remote_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 12:12:05.000000 naruno_remote_app-0.53.0/naruno_remote_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 12:12:05.406749 naruno_remote_app-0.53.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-04 12:11:44.000000 naruno_remote_app-0.53.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:50.214379 naruno_remote_app-0.54.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-08 23:33:50.214379 naruno_remote_app-0.54.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 23:33:50.214379 naruno_remote_app-0.54.0/naruno_remote_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-08 23:33:50.000000 naruno_remote_app-0.54.0/naruno_remote_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-08 23:33:50.000000 naruno_remote_app-0.54.0/naruno_remote_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 23:33:50.000000 naruno_remote_app-0.54.0/naruno_remote_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 23:33:50.000000 naruno_remote_app-0.54.0/naruno_remote_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-08 23:33:50.000000 naruno_remote_app-0.54.0/naruno_remote_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 23:33:50.000000 naruno_remote_app-0.54.0/naruno_remote_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 23:33:50.214379 naruno_remote_app-0.54.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-08 23:33:31.000000 naruno_remote_app-0.54.0/setup.py
```

### Comparing `naruno_remote_app-0.53.0/setup.py` & `naruno_remote_app-0.54.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from setuptools import setup
 
 setup(
     name="naruno_remote_app",
-    version="0.53.0",
+    version="0.54.0",
     description="""This is a tool for apps on Naruno""",
     url="https://docs.naruno.org/",
     author="Naruno Developers",
     author_email="onur.atakan.ulusoy@naruno.org",
     license="MPL-2.0",
     install_requires="""
 requests==2.28.2
-naruno_api==0.53.0
+naruno_api==0.54.0
 """,
     python_requires=">=3.8",
     zip_safe=False,
 )
```

