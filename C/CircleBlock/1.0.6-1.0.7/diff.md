# Comparing `tmp/CircleBlock-1.0.6.tar.gz` & `tmp/CircleBlock-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CircleBlock-1.0.6.tar", last modified: Sun Apr  9 16:48:20 2023, max compression
+gzip compressed data, was "CircleBlock-1.0.7.tar", last modified: Sun Apr  9 17:09:26 2023, max compression
```

## Comparing `CircleBlock-1.0.6.tar` & `CircleBlock-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 16:48:20.226320 CircleBlock-1.0.6/
--rw-r--r--   0 phil       (501) staff       (20)      411 2023-04-09 16:48:10.000000 CircleBlock-1.0.6/CHANGELOG.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 16:48:20.225623 CircleBlock-1.0.6/CircleBlock.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-09 16:48:20.000000 CircleBlock-1.0.6/CircleBlock.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      328 2023-04-09 16:48:20.000000 CircleBlock-1.0.6/CircleBlock.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-09 16:48:20.000000 CircleBlock-1.0.6/CircleBlock.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       45 2023-04-09 16:48:20.000000 CircleBlock-1.0.6/CircleBlock.egg-info/entry_points.txt
--rw-r--r--   0 phil       (501) staff       (20)       25 2023-04-09 16:48:20.000000 CircleBlock-1.0.6/CircleBlock.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-09 16:48:20.000000 CircleBlock-1.0.6/CircleBlock.egg-info/top_level.txt
--rw-r--r--   0 phil       (501) staff       (20)     1939 2023-04-09 05:38:11.000000 CircleBlock-1.0.6/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      152 2023-04-09 14:19:08.000000 CircleBlock-1.0.6/MANIFEST.in
--rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-09 16:48:20.226189 CircleBlock-1.0.6/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     2601 2023-04-09 09:32:22.000000 CircleBlock-1.0.6/README.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 16:48:20.226011 CircleBlock-1.0.6/circleblock/
--rw-r--r--   0 phil       (501) staff       (20)     4729 2023-04-09 16:45:25.000000 CircleBlock-1.0.6/circleblock/changer.py
--rw-r--r--   0 phil       (501) staff       (20)     3156 2023-04-09 14:52:09.000000 CircleBlock-1.0.6/circleblock/cli.py
--rw-r--r--   0 phil       (501) staff       (20)      983 2023-04-09 13:59:02.000000 CircleBlock-1.0.6/circleblock/watcher.py
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-04-09 16:48:20.226372 CircleBlock-1.0.6/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)     1021 2023-04-09 16:47:41.000000 CircleBlock-1.0.6/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 17:09:26.560352 CircleBlock-1.0.7/
+-rw-r--r--   0 phil       (501) staff       (20)      411 2023-04-09 17:08:56.000000 CircleBlock-1.0.7/CHANGELOG.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 17:09:26.559402 CircleBlock-1.0.7/CircleBlock.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-09 17:09:26.000000 CircleBlock-1.0.7/CircleBlock.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      364 2023-04-09 17:09:26.000000 CircleBlock-1.0.7/CircleBlock.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-04-09 17:09:26.000000 CircleBlock-1.0.7/CircleBlock.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       57 2023-04-09 17:09:26.000000 CircleBlock-1.0.7/CircleBlock.egg-info/entry_points.txt
+-rw-r--r--   0 phil       (501) staff       (20)       25 2023-04-09 17:09:26.000000 CircleBlock-1.0.7/CircleBlock.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)       12 2023-04-09 17:09:26.000000 CircleBlock-1.0.7/CircleBlock.egg-info/top_level.txt
+-rw-r--r--   0 phil       (501) staff       (20)     1939 2023-04-09 05:38:11.000000 CircleBlock-1.0.7/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      152 2023-04-09 17:08:22.000000 CircleBlock-1.0.7/MANIFEST.in
+-rw-r--r--   0 phil       (501) staff       (20)      705 2023-04-09 17:09:26.560139 CircleBlock-1.0.7/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     2601 2023-04-09 09:32:22.000000 CircleBlock-1.0.7/README.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-09 17:09:26.559945 CircleBlock-1.0.7/circleblock/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2023-04-09 17:05:19.000000 CircleBlock-1.0.7/circleblock/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     4729 2023-04-09 16:45:25.000000 CircleBlock-1.0.7/circleblock/changer.py
+-rw-r--r--   0 phil       (501) staff       (20)     3120 2023-04-09 17:08:08.000000 CircleBlock-1.0.7/circleblock/circleblock_cli.py
+-rw-r--r--   0 phil       (501) staff       (20)      983 2023-04-09 13:59:02.000000 CircleBlock-1.0.7/circleblock/watcher.py
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-04-09 17:09:26.560398 CircleBlock-1.0.7/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)     1033 2023-04-09 17:08:51.000000 CircleBlock-1.0.7/setup.py
```

### Comparing `CircleBlock-1.0.6/CircleBlock.egg-info/PKG-INFO` & `CircleBlock-1.0.7/CircleBlock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CircleBlock
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python package for creating circle-themed block diagrams
 Author: phil
 Author-email: eightynine01@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CircleBlock-1.0.6/LICENSE` & `CircleBlock-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.6/PKG-INFO` & `CircleBlock-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CircleBlock
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python package for creating circle-themed block diagrams
 Author: phil
 Author-email: eightynine01@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CircleBlock-1.0.6/README.md` & `CircleBlock-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.6/circleblock/changer.py` & `CircleBlock-1.0.7/circleblock/changer.py`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.6/circleblock/cli.py` & `CircleBlock-1.0.7/circleblock/circleblock_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import enum
 import os
 import signal
-import sys
 
 import typer
 
 from daemonize import Daemonize
 
 from .changer import InitFileUpdater
 from .watcher import FileWatcher
@@ -93,9 +92,9 @@
 @app.command(help='Initialize CircleBlock')
 def init(ctx: typer.Context) -> None:
     cb: CircleBlock = ctx.obj['cb'] or CircleBlock(ctx.obj['project_root'])
     cb.updater.initialize_all_init_files()
 
 
 if __name__ == '__main__':
-    app(prog_name='circleblock', help_option_names=['--help'])
+    app(help_option_names=['--help'])
```

### Comparing `CircleBlock-1.0.6/circleblock/watcher.py` & `CircleBlock-1.0.7/circleblock/watcher.py`

 * *Files identical despite different names*

### Comparing `CircleBlock-1.0.6/setup.py` & `CircleBlock-1.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CircleBlock',
-    version='1.0.6',
+    version='1.0.7',
     description='Python package for creating circle-themed block diagrams',
     author='phil',
     author_email='eightynine01@gmail.com',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'watchdog',
@@ -24,11 +24,11 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
     python_requires='>=3.6',
     entry_points={
         'console_scripts': [
-            'ccbk=circleblock.cli:app'
+            'ccbk=circleblock.circleblock_cli:app'
         ]
     }
 )
```

