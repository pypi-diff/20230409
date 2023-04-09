# Comparing `tmp/kiwigrad-0.13.tar.gz` & `tmp/kiwigrad-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwigrad-0.13.tar", last modified: Sun Apr  9 09:10:50 2023, max compression
+gzip compressed data, was "kiwigrad-0.14.tar", last modified: Sun Apr  9 09:16:04 2023, max compression
```

## Comparing `kiwigrad-0.13.tar` & `kiwigrad-0.14.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-09 09:10:50.682289 kiwigrad-0.13/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.13/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       22 2023-04-08 12:11:45.000000 kiwigrad-0.13/MANIFEST.in
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1933 2023-04-09 09:10:50.681616 kiwigrad-0.13/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      177 2023-04-03 14:22:56.000000 kiwigrad-0.13/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-09 09:10:50.679361 kiwigrad-0.13/kiwigrad/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      313 2023-04-09 09:09:43.000000 kiwigrad-0.13/kiwigrad/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     5274 2023-04-08 16:31:22.000000 kiwigrad-0.13/kiwigrad/engine.pyx
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      969 2023-04-08 12:31:36.000000 kiwigrad-0.13/kiwigrad/graph.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2940 2023-04-09 08:38:37.000000 kiwigrad-0.13/kiwigrad/nn.pyx
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-09 09:10:50.681021 kiwigrad-0.13/kiwigrad.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1933 2023-04-09 09:10:50.000000 kiwigrad-0.13/kiwigrad.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      278 2023-04-09 09:10:50.000000 kiwigrad-0.13/kiwigrad.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-09 09:10:50.000000 kiwigrad-0.13/kiwigrad.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-09 09:10:50.000000 kiwigrad-0.13/kiwigrad.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-09 09:10:50.000000 kiwigrad-0.13/kiwigrad.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      666 2023-04-09 09:09:54.000000 kiwigrad-0.13/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-09 09:10:50.682461 kiwigrad-0.13/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-09 09:16:04.596362 kiwigrad-0.14/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.14/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       22 2023-04-08 12:11:45.000000 kiwigrad-0.14/MANIFEST.in
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1933 2023-04-09 09:16:04.595938 kiwigrad-0.14/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      177 2023-04-03 14:22:56.000000 kiwigrad-0.14/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-09 09:16:04.593205 kiwigrad-0.14/kiwigrad/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      452 2023-04-09 09:15:05.000000 kiwigrad-0.14/kiwigrad/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     5274 2023-04-08 16:31:22.000000 kiwigrad-0.14/kiwigrad/engine.pyx
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      969 2023-04-08 12:31:36.000000 kiwigrad-0.14/kiwigrad/graph.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2940 2023-04-09 08:38:37.000000 kiwigrad-0.14/kiwigrad/nn.pyx
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-09 09:16:04.595509 kiwigrad-0.14/kiwigrad.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1933 2023-04-09 09:16:04.000000 kiwigrad-0.14/kiwigrad.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      278 2023-04-09 09:16:04.000000 kiwigrad-0.14/kiwigrad.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-09 09:16:04.000000 kiwigrad-0.14/kiwigrad.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-09 09:16:04.000000 kiwigrad-0.14/kiwigrad.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-09 09:16:04.000000 kiwigrad-0.14/kiwigrad.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      666 2023-04-09 09:15:11.000000 kiwigrad-0.14/pyproject.toml
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-09 09:16:04.596520 kiwigrad-0.14/setup.cfg
```

### Comparing `kiwigrad-0.13/LICENSE` & `kiwigrad-0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.13/PKG-INFO` & `kiwigrad-0.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwigrad
-Version: 0.13
+Version: 0.14
 Summary: Mini deep learning framework
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `kiwigrad-0.13/kiwigrad/engine.pyx` & `kiwigrad-0.14/kiwigrad/engine.pyx`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.13/kiwigrad/graph.py` & `kiwigrad-0.14/kiwigrad/graph.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.13/kiwigrad/nn.pyx` & `kiwigrad-0.14/kiwigrad/nn.pyx`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.13/kiwigrad.egg-info/PKG-INFO` & `kiwigrad-0.14/kiwigrad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwigrad
-Version: 0.13
+Version: 0.14
 Summary: Mini deep learning framework
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `kiwigrad-0.13/pyproject.toml` & `kiwigrad-0.14/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kiwigrad"
-version = "0.13"
+version = "0.14"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Mini deep learning framework"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

