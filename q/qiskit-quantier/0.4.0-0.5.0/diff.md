# Comparing `tmp/qiskit_quantier-0.4.0.tar.gz` & `tmp/qiskit_quantier-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_quantier-0.4.0.tar", last modified: Sat Apr  8 22:03:22 2023, max compression
+gzip compressed data, was "qiskit_quantier-0.5.0.tar", last modified: Sat Apr  8 22:15:22 2023, max compression
```

## Comparing `qiskit_quantier-0.4.0.tar` & `qiskit_quantier-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-04-08 22:03:22.620358 qiskit_quantier-0.4.0/
--rw-r--r--   0 rustam     (501) staff       (20)      335 2023-04-08 22:03:22.620039 qiskit_quantier-0.4.0/PKG-INFO
--rw-r--r--   0 rustam     (501) staff       (20)       26 2023-04-08 21:37:34.000000 qiskit_quantier-0.4.0/README.md
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-04-08 22:03:22.618728 qiskit_quantier-0.4.0/qiskit_quantier.egg-info/
--rw-r--r--   0 rustam     (501) staff       (20)      335 2023-04-08 22:03:22.000000 qiskit_quantier-0.4.0/qiskit_quantier.egg-info/PKG-INFO
--rw-r--r--   0 rustam     (501) staff       (20)      233 2023-04-08 22:03:22.000000 qiskit_quantier-0.4.0/qiskit_quantier.egg-info/SOURCES.txt
--rw-r--r--   0 rustam     (501) staff       (20)        1 2023-04-08 22:03:22.000000 qiskit_quantier-0.4.0/qiskit_quantier.egg-info/dependency_links.txt
--rw-r--r--   0 rustam     (501) staff       (20)       18 2023-04-08 22:03:22.000000 qiskit_quantier-0.4.0/qiskit_quantier.egg-info/requires.txt
--rw-r--r--   0 rustam     (501) staff       (20)        9 2023-04-08 22:03:22.000000 qiskit_quantier-0.4.0/qiskit_quantier.egg-info/top_level.txt
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-04-08 22:03:22.619080 qiskit_quantier-0.4.0/quantier/
--rw-r--r--   0 rustam     (501) staff       (20)     1889 2023-04-08 21:16:12.000000 qiskit_quantier-0.4.0/quantier/quantier.py
--rw-r--r--   0 rustam     (501) staff       (20)       38 2023-04-08 22:03:22.620488 qiskit_quantier-0.4.0/setup.cfg
--rw-r--r--   0 rustam     (501) staff       (20)      661 2023-04-08 22:03:11.000000 qiskit_quantier-0.4.0/setup.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-04-08 22:15:22.936123 qiskit_quantier-0.5.0/
+-rw-r--r--   0 rustam     (501) staff       (20)      335 2023-04-08 22:15:22.935822 qiskit_quantier-0.5.0/PKG-INFO
+-rw-r--r--   0 rustam     (501) staff       (20)       26 2023-04-08 21:37:34.000000 qiskit_quantier-0.5.0/README.md
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-04-08 22:15:22.934195 qiskit_quantier-0.5.0/qiskit_quantier.egg-info/
+-rw-r--r--   0 rustam     (501) staff       (20)      335 2023-04-08 22:15:22.000000 qiskit_quantier-0.5.0/qiskit_quantier.egg-info/PKG-INFO
+-rw-r--r--   0 rustam     (501) staff       (20)      254 2023-04-08 22:15:22.000000 qiskit_quantier-0.5.0/qiskit_quantier.egg-info/SOURCES.txt
+-rw-r--r--   0 rustam     (501) staff       (20)        1 2023-04-08 22:15:22.000000 qiskit_quantier-0.5.0/qiskit_quantier.egg-info/dependency_links.txt
+-rw-r--r--   0 rustam     (501) staff       (20)       18 2023-04-08 22:15:22.000000 qiskit_quantier-0.5.0/qiskit_quantier.egg-info/requires.txt
+-rw-r--r--   0 rustam     (501) staff       (20)        9 2023-04-08 22:15:22.000000 qiskit_quantier-0.5.0/qiskit_quantier.egg-info/top_level.txt
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-04-08 22:15:22.934830 qiskit_quantier-0.5.0/quantier/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2023-04-08 22:13:24.000000 qiskit_quantier-0.5.0/quantier/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)     1889 2023-04-08 21:16:12.000000 qiskit_quantier-0.5.0/quantier/quantier.py
+-rw-r--r--   0 rustam     (501) staff       (20)       38 2023-04-08 22:15:22.936244 qiskit_quantier-0.5.0/setup.cfg
+-rw-r--r--   0 rustam     (501) staff       (20)      661 2023-04-08 22:14:17.000000 qiskit_quantier-0.5.0/setup.py
```

### Comparing `qiskit_quantier-0.4.0/quantier/quantier.py` & `qiskit_quantier-0.5.0/quantier/quantier.py`

 * *Files identical despite different names*

### Comparing `qiskit_quantier-0.4.0/setup.py` & `qiskit_quantier-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qiskit_quantier",
-    version="0.4.0",
+    version="0.5.0",
     description="A quantum provider for Qiskit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["quantier"],
     package_dir={"quantier": "quantier"},
     classifiers=[
         "Programming Language :: Python :: 3",
```

