# Comparing `tmp/vidis_algorithms_api-0.3.1.tar.gz` & `tmp/vidis_algorithms_api-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vidis_algorithms_api-0.3.1.tar", last modified: Fri Apr  7 07:15:43 2023, max compression
+gzip compressed data, was "vidis_algorithms_api-0.3.2.tar", last modified: Sun Apr  9 12:53:05 2023, max compression
```

## Comparing `vidis_algorithms_api-0.3.1.tar` & `vidis_algorithms_api-0.3.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 07:15:43.572188 vidis_algorithms_api-0.3.1/
--rw-r--r--   0 root         (0) root         (0)      383 2023-04-07 07:15:43.572188 vidis_algorithms_api-0.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1370 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 07:15:43.568188 vidis_algorithms_api-0.3.1/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 07:15:43.572188 vidis_algorithms_api-0.3.1/examples/dummy_example/
--rw-rw-rw-   0 root         (0) root         (0)      528 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.1/examples/dummy_example/algorithm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 07:15:43.572188 vidis_algorithms_api-0.3.1/examples/neural_network/
--rw-rw-rw-   0 root         (0) root         (0)     3626 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.1/examples/neural_network/algorithm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 07:15:43.572188 vidis_algorithms_api-0.3.1/examples/neural_network/model/
--rw-rw-rw-   0 root         (0) root         (0)     3737 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.1/examples/neural_network/model/model.py
--rw-rw-rw-   0 root         (0) root         (0)      471 2023-04-07 07:06:59.000000 vidis_algorithms_api-0.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-07 07:15:43.572188 vidis_algorithms_api-0.3.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      654 2023-04-07 07:06:59.000000 vidis_algorithms_api-0.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 07:15:43.572188 vidis_algorithms_api-0.3.1/vidis_algorithms_api/
--rw-rw-rw-   0 root         (0) root         (0)      568 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.1/vidis_algorithms_api/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     1091 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.1/vidis_algorithms_api/Task.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-04-07 07:06:59.000000 vidis_algorithms_api-0.3.1/vidis_algorithms_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 07:15:43.572188 vidis_algorithms_api-0.3.1/vidis_algorithms_api/core/
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.1/vidis_algorithms_api/core/Settings.py
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.1/vidis_algorithms_api/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 07:15:43.572188 vidis_algorithms_api-0.3.1/vidis_algorithms_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      383 2023-04-07 07:15:43.000000 vidis_algorithms_api-0.3.1/vidis_algorithms_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      531 2023-04-07 07:15:43.000000 vidis_algorithms_api-0.3.1/vidis_algorithms_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 07:15:43.000000 vidis_algorithms_api-0.3.1/vidis_algorithms_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-04-07 07:15:43.000000 vidis_algorithms_api-0.3.1/vidis_algorithms_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-04-07 07:15:43.000000 vidis_algorithms_api-0.3.1/vidis_algorithms_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:53:05.099517 vidis_algorithms_api-0.3.2/
+-rw-r--r--   0 root         (0) root         (0)      383 2023-04-09 12:53:05.099517 vidis_algorithms_api-0.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1370 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:53:05.099517 vidis_algorithms_api-0.3.2/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:53:05.099517 vidis_algorithms_api-0.3.2/examples/dummy_example/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-09 12:49:15.000000 vidis_algorithms_api-0.3.2/examples/dummy_example/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      528 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.2/examples/dummy_example/algorithm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:53:05.099517 vidis_algorithms_api-0.3.2/examples/neural_network/
+-rw-rw-rw-   0 root         (0) root         (0)     3626 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.2/examples/neural_network/algorithm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:53:05.099517 vidis_algorithms_api-0.3.2/examples/neural_network/model/
+-rw-rw-rw-   0 root         (0) root         (0)     3737 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.2/examples/neural_network/model/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      471 2023-04-09 12:49:15.000000 vidis_algorithms_api-0.3.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 12:53:05.099517 vidis_algorithms_api-0.3.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      666 2023-04-09 12:49:15.000000 vidis_algorithms_api-0.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:53:05.099517 vidis_algorithms_api-0.3.2/vidis_algorithms_api/
+-rw-rw-rw-   0 root         (0) root         (0)      568 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.2/vidis_algorithms_api/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.2/vidis_algorithms_api/Task.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-04-07 07:06:59.000000 vidis_algorithms_api-0.3.2/vidis_algorithms_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:53:05.099517 vidis_algorithms_api-0.3.2/vidis_algorithms_api/core/
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.2/vidis_algorithms_api/core/Settings.py
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-04-06 10:48:38.000000 vidis_algorithms_api-0.3.2/vidis_algorithms_api/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 12:53:05.099517 vidis_algorithms_api-0.3.2/vidis_algorithms_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      383 2023-04-09 12:53:05.000000 vidis_algorithms_api-0.3.2/vidis_algorithms_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      566 2023-04-09 12:53:05.000000 vidis_algorithms_api-0.3.2/vidis_algorithms_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 12:53:05.000000 vidis_algorithms_api-0.3.2/vidis_algorithms_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-04-09 12:53:05.000000 vidis_algorithms_api-0.3.2/vidis_algorithms_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-04-09 12:53:05.000000 vidis_algorithms_api-0.3.2/vidis_algorithms_api.egg-info/top_level.txt
```

### Comparing `vidis_algorithms_api-0.3.1/README.md` & `vidis_algorithms_api-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `vidis_algorithms_api-0.3.1/examples/dummy_example/algorithm.py` & `vidis_algorithms_api-0.3.2/examples/dummy_example/algorithm.py`

 * *Files identical despite different names*

### Comparing `vidis_algorithms_api-0.3.1/examples/neural_network/algorithm.py` & `vidis_algorithms_api-0.3.2/examples/neural_network/algorithm.py`

 * *Files identical despite different names*

### Comparing `vidis_algorithms_api-0.3.1/examples/neural_network/model/model.py` & `vidis_algorithms_api-0.3.2/examples/neural_network/model/model.py`

 * *Files identical despite different names*

### Comparing `vidis_algorithms_api-0.3.1/setup.py` & `vidis_algorithms_api-0.3.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 requirements = [
     'pydantic==1.10.2',
     'loguru==0.6.0',
     'numpy==1.24.1',
-    'celery==5.2.7',
+    'celery[amqp,redis]==5.2.7',
 ]
 
 with open('README.md', 'r') as f:
     description = f.read()
 
 
 def setup_package():
-    __version__ = '0.3.1'
+    __version__ = '0.3.2'
     url = 'https://github.com/Banayaki'
 
     setup(name='vidis_algorithms_api',
           description=description,
           version=__version__,
           url=url,
           license='MIT',
```

### Comparing `vidis_algorithms_api-0.3.1/vidis_algorithms_api/Main.py` & `vidis_algorithms_api-0.3.2/vidis_algorithms_api/Main.py`

 * *Files identical despite different names*

### Comparing `vidis_algorithms_api-0.3.1/vidis_algorithms_api/Task.py` & `vidis_algorithms_api-0.3.2/vidis_algorithms_api/Task.py`

 * *Files identical despite different names*

### Comparing `vidis_algorithms_api-0.3.1/vidis_algorithms_api.egg-info/SOURCES.txt` & `vidis_algorithms_api-0.3.2/vidis_algorithms_api.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 pyproject.toml
 setup.py
+examples/dummy_example/__init__.py
 examples/dummy_example/algorithm.py
 examples/neural_network/algorithm.py
 examples/neural_network/model/model.py
 vidis_algorithms_api/Main.py
 vidis_algorithms_api/Task.py
 vidis_algorithms_api/__init__.py
 vidis_algorithms_api.egg-info/PKG-INFO
```

