# Comparing `tmp/kiwigrad-0.0.9.tar.gz` & `tmp/kiwigrad-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwigrad-0.0.9.tar", last modified: Sun Apr  9 08:56:02 2023, max compression
+gzip compressed data, was "kiwigrad-0.1.tar", last modified: Sun Apr  9 09:01:09 2023, max compression
```

## Comparing `kiwigrad-0.0.9.tar` & `kiwigrad-0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-09 08:56:02.647848 kiwigrad-0.0.9/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.0.9/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       22 2023-04-08 12:11:45.000000 kiwigrad-0.0.9/MANIFEST.in
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1934 2023-04-09 08:56:02.647268 kiwigrad-0.0.9/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      177 2023-04-03 14:22:56.000000 kiwigrad-0.0.9/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-09 08:56:02.644779 kiwigrad-0.0.9/kiwigrad/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      352 2023-04-09 08:55:12.000000 kiwigrad-0.0.9/kiwigrad/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     5274 2023-04-08 16:31:22.000000 kiwigrad-0.0.9/kiwigrad/engine.pyx
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      969 2023-04-08 12:31:36.000000 kiwigrad-0.0.9/kiwigrad/graph.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2940 2023-04-09 08:38:37.000000 kiwigrad-0.0.9/kiwigrad/nn.pyx
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-09 08:56:02.646635 kiwigrad-0.0.9/kiwigrad.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1934 2023-04-09 08:56:02.000000 kiwigrad-0.0.9/kiwigrad.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      278 2023-04-09 08:56:02.000000 kiwigrad-0.0.9/kiwigrad.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-09 08:56:02.000000 kiwigrad-0.0.9/kiwigrad.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-09 08:56:02.000000 kiwigrad-0.0.9/kiwigrad.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-09 08:56:02.000000 kiwigrad-0.0.9/kiwigrad.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      667 2023-04-09 08:37:51.000000 kiwigrad-0.0.9/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-09 08:56:02.647981 kiwigrad-0.0.9/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-09 09:01:09.175132 kiwigrad-0.1/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.1/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       22 2023-04-08 12:11:45.000000 kiwigrad-0.1/MANIFEST.in
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1932 2023-04-09 09:01:09.174475 kiwigrad-0.1/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      177 2023-04-03 14:22:56.000000 kiwigrad-0.1/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-09 09:01:09.171839 kiwigrad-0.1/kiwigrad/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      405 2023-04-09 09:00:04.000000 kiwigrad-0.1/kiwigrad/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     5274 2023-04-08 16:31:22.000000 kiwigrad-0.1/kiwigrad/engine.pyx
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      969 2023-04-08 12:31:36.000000 kiwigrad-0.1/kiwigrad/graph.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2940 2023-04-09 08:38:37.000000 kiwigrad-0.1/kiwigrad/nn.pyx
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-09 09:01:09.173748 kiwigrad-0.1/kiwigrad.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1932 2023-04-09 09:01:09.000000 kiwigrad-0.1/kiwigrad.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      278 2023-04-09 09:01:09.000000 kiwigrad-0.1/kiwigrad.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-09 09:01:09.000000 kiwigrad-0.1/kiwigrad.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-09 09:01:09.000000 kiwigrad-0.1/kiwigrad.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-09 09:01:09.000000 kiwigrad-0.1/kiwigrad.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      665 2023-04-09 09:00:10.000000 kiwigrad-0.1/pyproject.toml
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-09 09:01:09.175344 kiwigrad-0.1/setup.cfg
```

### Comparing `kiwigrad-0.0.9/LICENSE` & `kiwigrad-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.0.9/PKG-INFO` & `kiwigrad-0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwigrad
-Version: 0.0.9
+Version: 0.1
 Summary: Mini deep learning framework
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `kiwigrad-0.0.9/kiwigrad/engine.pyx` & `kiwigrad-0.1/kiwigrad/engine.pyx`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.0.9/kiwigrad/graph.py` & `kiwigrad-0.1/kiwigrad/graph.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.0.9/kiwigrad/nn.pyx` & `kiwigrad-0.1/kiwigrad/nn.pyx`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.0.9/kiwigrad.egg-info/PKG-INFO` & `kiwigrad-0.1/kiwigrad.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwigrad
-Version: 0.0.9
+Version: 0.1
 Summary: Mini deep learning framework
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `kiwigrad-0.0.9/pyproject.toml` & `kiwigrad-0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kiwigrad"
-version = "0.0.9"
+version = "0.1"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Mini deep learning framework"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

