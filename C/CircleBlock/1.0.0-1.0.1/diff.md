# Comparing `tmp/CircleBlock-1.0.0.tar.gz` & `tmp/CircleBlock-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CircleBlock-1.0.0.tar", last modified: Sun Apr  9 07:38:46 2023, max compression
+gzip compressed data, was "CircleBlock-1.0.1.tar", last modified: Sun Apr  9 07:57:31 2023, max compression
```

## Comparing `CircleBlock-1.0.0.tar` & `CircleBlock-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 07:38:46.306737 CircleBlock-1.0.0/
--rw-r--r--   0 phil       (501) staff       (20)      364 2023-04-09 05:40:57.000000 CircleBlock-1.0.0/CHANGELOG.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 07:38:46.305802 CircleBlock-1.0.0/CircleBlock.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      603 2023-04-09 07:38:46.000000 CircleBlock-1.0.0/CircleBlock.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      355 2023-04-09 07:38:46.000000 CircleBlock-1.0.0/CircleBlock.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-09 07:38:46.000000 CircleBlock-1.0.0/CircleBlock.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       47 2023-04-09 07:38:46.000000 CircleBlock-1.0.0/CircleBlock.egg-info/entry_points.txt
--rw-r--r--   0 phil       (501) staff       (20)       22 2023-04-09 07:38:46.000000 CircleBlock-1.0.0/CircleBlock.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-09 07:38:46.000000 CircleBlock-1.0.0/CircleBlock.egg-info/top_level.txt
--rw-r--r--   0 phil       (501) staff       (20)     1939 2023-04-09 05:38:11.000000 CircleBlock-1.0.0/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      152 2023-04-09 06:09:13.000000 CircleBlock-1.0.0/MANIFEST.in
--rw-r--r--   0 phil       (501) staff       (20)      603 2023-04-09 07:38:46.306588 CircleBlock-1.0.0/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     1959 2023-04-09 07:29:41.000000 CircleBlock-1.0.0/README.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 07:38:46.306378 CircleBlock-1.0.0/circleblock/
--rw-r--r--   0 phil       (501) staff       (20)     4904 2023-04-09 07:03:29.000000 CircleBlock-1.0.0/circleblock/changer.py
--rw-r--r--   0 phil       (501) staff       (20)     3421 2023-04-09 07:02:41.000000 CircleBlock-1.0.0/circleblock/circleblock.py
--rw-r--r--   0 phil       (501) staff       (20)      845 2023-04-09 06:58:59.000000 CircleBlock-1.0.0/circleblock/cli.py
--rw-r--r--   0 phil       (501) staff       (20)     1197 2023-04-09 06:12:22.000000 CircleBlock-1.0.0/circleblock/watcher.py
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-04-09 07:38:46.306789 CircleBlock-1.0.0/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)      920 2023-04-09 06:15:26.000000 CircleBlock-1.0.0/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 07:57:31.293069 CircleBlock-1.0.1/
+-rw-r--r--   0 phil       (501) staff       (20)      364 2023-04-09 05:40:57.000000 CircleBlock-1.0.1/CHANGELOG.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 07:57:31.292235 CircleBlock-1.0.1/CircleBlock.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      603 2023-04-09 07:57:31.000000 CircleBlock-1.0.1/CircleBlock.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      355 2023-04-09 07:57:31.000000 CircleBlock-1.0.1/CircleBlock.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-09 07:57:31.000000 CircleBlock-1.0.1/CircleBlock.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       36 2023-04-09 07:57:31.000000 CircleBlock-1.0.1/CircleBlock.egg-info/entry_points.txt
+-rw-r--r--   0 phil       (501) staff       (20)       22 2023-04-09 07:57:31.000000 CircleBlock-1.0.1/CircleBlock.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-09 07:57:31.000000 CircleBlock-1.0.1/CircleBlock.egg-info/top_level.txt
+-rw-r--r--   0 phil       (501) staff       (20)     1939 2023-04-09 05:38:11.000000 CircleBlock-1.0.1/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      152 2023-04-09 06:09:13.000000 CircleBlock-1.0.1/MANIFEST.in
+-rw-r--r--   0 phil       (501) staff       (20)      603 2023-04-09 07:57:31.292940 CircleBlock-1.0.1/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     1959 2023-04-09 07:29:41.000000 CircleBlock-1.0.1/README.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 07:57:31.292771 CircleBlock-1.0.1/circleblock/
+-rw-r--r--   0 phil       (501) staff       (20)     4904 2023-04-09 07:03:29.000000 CircleBlock-1.0.1/circleblock/changer.py
+-rw-r--r--   0 phil       (501) staff       (20)     3421 2023-04-09 07:02:41.000000 CircleBlock-1.0.1/circleblock/circleblock.py
+-rw-r--r--   0 phil       (501) staff       (20)      833 2023-04-09 07:49:56.000000 CircleBlock-1.0.1/circleblock/cli.py
+-rw-r--r--   0 phil       (501) staff       (20)     1197 2023-04-09 06:12:22.000000 CircleBlock-1.0.1/circleblock/watcher.py
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-04-09 07:57:31.293113 CircleBlock-1.0.1/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)      909 2023-04-09 07:55:28.000000 CircleBlock-1.0.1/setup.py
```

### Comparing `CircleBlock-1.0.0/CircleBlock.egg-info/PKG-INFO` & `CircleBlock-1.0.1/CircleBlock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CircleBlock
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python package for creating circle-themed block diagrams
 Author: phil
 Author-email: eightynine01@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CircleBlock-1.0.0/LICENSE` & `CircleBlock-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.0/PKG-INFO` & `CircleBlock-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CircleBlock
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python package for creating circle-themed block diagrams
 Author: phil
 Author-email: eightynine01@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CircleBlock-1.0.0/README.md` & `CircleBlock-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.0/circleblock/changer.py` & `CircleBlock-1.0.1/circleblock/changer.py`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.0/circleblock/circleblock.py` & `CircleBlock-1.0.1/circleblock/circleblock.py`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.0/circleblock/cli.py` & `CircleBlock-1.0.1/circleblock/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import click
 
-from circleblock.circleblock import start_circleblock
+from circleblock import start_circleblock
 
 
 @click.group(name='ccbk')
 def cli():
     pass
```

### Comparing `CircleBlock-1.0.0/circleblock/watcher.py` & `CircleBlock-1.0.1/circleblock/watcher.py`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.0/setup.py` & `CircleBlock-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CircleBlock',
-    version='1.0.0',
+    version='1.0.1',
     description='Python package for creating circle-themed block diagrams',
     author='phil',
     author_email='eightynine01@gmail.com',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'watchdog',
@@ -22,11 +22,11 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     python_requires='>=3.6',
     entry_points={
         'console_scripts': [
-            'ccbk=circleblock.cli:start'
+            'ccbk=.cli:start'
         ]
     }
 )
```

