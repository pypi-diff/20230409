# Comparing `tmp/acr122u-websocket-1.0.1.tar.gz` & `tmp/acr122u-websocket-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acr122u-websocket-1.0.1.tar", last modified: Sat Apr  8 19:21:48 2023, max compression
+gzip compressed data, was "acr122u-websocket-1.1.0.tar", last modified: Sun Apr  9 14:20:09 2023, max compression
```

## Comparing `acr122u-websocket-1.0.1.tar` & `acr122u-websocket-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:21:48.099702 acr122u-websocket-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-08 19:21:39.000000 acr122u-websocket-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-08 19:21:48.099702 acr122u-websocket-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-08 19:21:39.000000 acr122u-websocket-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:21:48.099702 acr122u-websocket-1.0.1/acr122u_websocket/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-08 19:21:39.000000 acr122u-websocket-1.0.1/acr122u_websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-08 19:21:39.000000 acr122u-websocket-1.0.1/acr122u_websocket/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-08 19:21:39.000000 acr122u-websocket-1.0.1/acr122u_websocket/my_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-08 19:21:39.000000 acr122u-websocket-1.0.1/acr122u_websocket/reader_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:21:48.099702 acr122u-websocket-1.0.1/acr122u_websocket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-08 19:21:48.000000 acr122u-websocket-1.0.1/acr122u_websocket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-08 19:21:48.000000 acr122u-websocket-1.0.1/acr122u_websocket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 19:21:48.000000 acr122u-websocket-1.0.1/acr122u_websocket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-08 19:21:48.000000 acr122u-websocket-1.0.1/acr122u_websocket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-08 19:21:48.000000 acr122u-websocket-1.0.1/acr122u_websocket.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-08 19:21:39.000000 acr122u-websocket-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 19:21:48.099702 acr122u-websocket-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:20:09.231924 acr122u-websocket-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-09 14:19:56.000000 acr122u-websocket-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-09 14:20:09.231924 acr122u-websocket-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-09 14:19:56.000000 acr122u-websocket-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:20:09.227924 acr122u-websocket-1.1.0/acr122u_websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 14:19:56.000000 acr122u-websocket-1.1.0/acr122u_websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-09 14:19:56.000000 acr122u-websocket-1.1.0/acr122u_websocket/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-09 14:19:56.000000 acr122u-websocket-1.1.0/acr122u_websocket/my_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-09 14:19:56.000000 acr122u-websocket-1.1.0/acr122u_websocket/reader_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:20:09.231924 acr122u-websocket-1.1.0/acr122u_websocket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-09 14:20:09.000000 acr122u-websocket-1.1.0/acr122u_websocket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-09 14:20:09.000000 acr122u-websocket-1.1.0/acr122u_websocket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:20:09.000000 acr122u-websocket-1.1.0/acr122u_websocket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-09 14:20:09.000000 acr122u-websocket-1.1.0/acr122u_websocket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-09 14:20:09.000000 acr122u-websocket-1.1.0/acr122u_websocket.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-09 14:19:56.000000 acr122u-websocket-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 14:20:09.231924 acr122u-websocket-1.1.0/setup.cfg
```

### Comparing `acr122u-websocket-1.0.1/LICENSE` & `acr122u-websocket-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acr122u-websocket-1.0.1/pyproject.toml` & `acr122u-websocket-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "acr122u-websocket"
-version = "1.0.1"
+version = "1.1.0"
 description = "A webserver that connects to a acr122u and exposes it over websocket"
 readme = "README.md"
 authors = [{ name = "Robert van Dijk", email = "contact@robertvandijk.nl" }]
 license = { file = "pb" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
@@ -21,21 +21,22 @@
     'py-acr122u',
 ]
 requires-python = ">=3.11"
 
 [project.optional-dependencies]
 dev = [
     "bumpver",
+    "black",
 ]
 
 [project.urls]
 Homepage = "https://github.com/robertdijk/acr122u-websocket"
 
 [tool.bumpver]
-current_version = "1.0.1"
+current_version = "1.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

