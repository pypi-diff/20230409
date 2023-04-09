# Comparing `tmp/hexa-0.0.2.tar.gz` & `tmp/hexa-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexa-0.0.2.tar", last modified: Sun Apr  9 13:09:51 2023, max compression
+gzip compressed data, was "hexa-0.0.3.tar", last modified: Sun Apr  9 13:21:23 2023, max compression
```

## Comparing `hexa-0.0.2.tar` & `hexa-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-04-09 13:09:51.036707 hexa-0.0.2/
--rw-r--r--   0 anderson  (1000) anderson  (1000)      409 2023-04-09 13:09:51.036707 hexa-0.0.2/PKG-INFO
-drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-04-09 13:09:51.033374 hexa-0.0.2/hexa/
--rw-r--r--   0 anderson  (1000) anderson  (1000)        9 2023-04-09 13:04:54.000000 hexa-0.0.2/hexa/__init__.py
-drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-04-09 13:09:51.036707 hexa-0.0.2/hexa.egg-info/
--rw-r--r--   0 anderson  (1000) anderson  (1000)      409 2023-04-09 13:09:51.000000 hexa-0.0.2/hexa.egg-info/PKG-INFO
--rw-r--r--   0 anderson  (1000) anderson  (1000)      143 2023-04-09 13:09:51.000000 hexa-0.0.2/hexa.egg-info/SOURCES.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)        1 2023-04-09 13:09:51.000000 hexa-0.0.2/hexa.egg-info/dependency_links.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)        5 2023-04-09 13:09:51.000000 hexa-0.0.2/hexa.egg-info/top_level.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)      514 2023-04-09 13:09:15.000000 hexa-0.0.2/pyproject.toml
--rw-r--r--   0 anderson  (1000) anderson  (1000)       38 2023-04-09 13:09:51.036707 hexa-0.0.2/setup.cfg
+drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-04-09 13:21:23.546751 hexa-0.0.3/
+-rw-r--r--   0 anderson  (1000) anderson  (1000)      409 2023-04-09 13:21:23.546751 hexa-0.0.3/PKG-INFO
+drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-04-09 13:21:23.546751 hexa-0.0.3/hexa/
+-rw-r--r--   0 anderson  (1000) anderson  (1000)        9 2023-04-09 13:04:54.000000 hexa-0.0.3/hexa/__init__.py
+drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-04-09 13:21:23.546751 hexa-0.0.3/hexa.egg-info/
+-rw-r--r--   0 anderson  (1000) anderson  (1000)      409 2023-04-09 13:21:23.000000 hexa-0.0.3/hexa.egg-info/PKG-INFO
+-rw-r--r--   0 anderson  (1000) anderson  (1000)      170 2023-04-09 13:21:23.000000 hexa-0.0.3/hexa.egg-info/SOURCES.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)        1 2023-04-09 13:21:23.000000 hexa-0.0.3/hexa.egg-info/dependency_links.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       17 2023-04-09 13:21:23.000000 hexa-0.0.3/hexa.egg-info/requires.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)        5 2023-04-09 13:21:23.000000 hexa-0.0.3/hexa.egg-info/top_level.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)      573 2023-04-09 13:21:15.000000 hexa-0.0.3/pyproject.toml
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       38 2023-04-09 13:21:23.546751 hexa-0.0.3/setup.cfg
```

### Comparing `hexa-0.0.2/pyproject.toml` & `hexa-0.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [project]
 name = "hexa"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Andrew Dunai", email="a@dun.ai" },
 ]
 description = "Hexagonal Architecture with Domain Driven Design"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "pydantic==1.10.4",  # Typed models
+]
 
 [project.urls]
 "Homepage" = "https://github.com/and3rson/hexa"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
```

