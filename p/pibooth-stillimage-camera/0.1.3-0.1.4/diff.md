# Comparing `tmp/pibooth-stillimage-camera-0.1.3.tar.gz` & `tmp/pibooth-stillimage-camera-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pibooth-stillimage-camera-0.1.3.tar", last modified: Sun Apr  9 19:22:48 2023, max compression
+gzip compressed data, was "pibooth-stillimage-camera-0.1.4.tar", last modified: Sun Apr  9 21:13:28 2023, max compression
```

## Comparing `pibooth-stillimage-camera-0.1.3.tar` & `pibooth-stillimage-camera-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 gilou     (1000) gilou     (1000)        0 2023-04-09 19:22:48.907290 pibooth-stillimage-camera-0.1.3/
--rw-rw-r--   0 gilou     (1000) gilou     (1000)    34476 2023-04-09 10:19:41.000000 pibooth-stillimage-camera-0.1.3/LICENSE
--rw-rw-r--   0 gilou     (1000) gilou     (1000)     2139 2023-04-09 19:22:48.907290 pibooth-stillimage-camera-0.1.3/PKG-INFO
--rw-rw-r--   0 gilou     (1000) gilou     (1000)     1175 2023-04-09 16:08:24.000000 pibooth-stillimage-camera-0.1.3/README.md
-drwxrwxr-x   0 gilou     (1000) gilou     (1000)        0 2023-04-09 19:22:48.907290 pibooth-stillimage-camera-0.1.3/pibooth_stillimage_camera.egg-info/
--rw-rw-r--   0 gilou     (1000) gilou     (1000)     2139 2023-04-09 19:22:48.000000 pibooth-stillimage-camera-0.1.3/pibooth_stillimage_camera.egg-info/PKG-INFO
--rw-rw-r--   0 gilou     (1000) gilou     (1000)      357 2023-04-09 19:22:48.000000 pibooth-stillimage-camera-0.1.3/pibooth_stillimage_camera.egg-info/SOURCES.txt
--rw-rw-r--   0 gilou     (1000) gilou     (1000)        1 2023-04-09 19:22:48.000000 pibooth-stillimage-camera-0.1.3/pibooth_stillimage_camera.egg-info/dependency_links.txt
--rw-rw-r--   0 gilou     (1000) gilou     (1000)       64 2023-04-09 19:22:48.000000 pibooth-stillimage-camera-0.1.3/pibooth_stillimage_camera.egg-info/entry_points.txt
--rw-rw-r--   0 gilou     (1000) gilou     (1000)       14 2023-04-09 19:22:48.000000 pibooth-stillimage-camera-0.1.3/pibooth_stillimage_camera.egg-info/requires.txt
--rw-rw-r--   0 gilou     (1000) gilou     (1000)       26 2023-04-09 19:22:48.000000 pibooth-stillimage-camera-0.1.3/pibooth_stillimage_camera.egg-info/top_level.txt
--rw-rw-r--   0 gilou     (1000) gilou     (1000)     3182 2023-04-09 17:28:06.000000 pibooth-stillimage-camera-0.1.3/pibooth_stillimage_camera.py
--rw-rw-r--   0 gilou     (1000) gilou     (1000)     1239 2023-04-09 19:20:30.000000 pibooth-stillimage-camera-0.1.3/pyproject.toml
--rw-rw-r--   0 gilou     (1000) gilou     (1000)       38 2023-04-09 19:22:48.907290 pibooth-stillimage-camera-0.1.3/setup.cfg
+drwxrwxr-x   0 gilou     (1000) gilou     (1000)        0 2023-04-09 21:13:28.358734 pibooth-stillimage-camera-0.1.4/
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)    34476 2023-04-09 10:19:41.000000 pibooth-stillimage-camera-0.1.4/LICENSE
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)     2139 2023-04-09 21:13:28.358734 pibooth-stillimage-camera-0.1.4/PKG-INFO
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)     1175 2023-04-09 16:08:24.000000 pibooth-stillimage-camera-0.1.4/README.md
+drwxrwxr-x   0 gilou     (1000) gilou     (1000)        0 2023-04-09 21:13:28.358734 pibooth-stillimage-camera-0.1.4/pibooth_stillimage_camera.egg-info/
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)     2139 2023-04-09 21:13:28.000000 pibooth-stillimage-camera-0.1.4/pibooth_stillimage_camera.egg-info/PKG-INFO
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)      405 2023-04-09 21:13:28.000000 pibooth-stillimage-camera-0.1.4/pibooth_stillimage_camera.egg-info/SOURCES.txt
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)        1 2023-04-09 21:13:28.000000 pibooth-stillimage-camera-0.1.4/pibooth_stillimage_camera.egg-info/dependency_links.txt
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)       64 2023-04-09 21:13:28.000000 pibooth-stillimage-camera-0.1.4/pibooth_stillimage_camera.egg-info/entry_points.txt
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)        1 2023-04-09 21:11:00.000000 pibooth-stillimage-camera-0.1.4/pibooth_stillimage_camera.egg-info/not-zip-safe
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)       14 2023-04-09 21:13:28.000000 pibooth-stillimage-camera-0.1.4/pibooth_stillimage_camera.egg-info/requires.txt
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)       26 2023-04-09 21:13:28.000000 pibooth-stillimage-camera-0.1.4/pibooth_stillimage_camera.egg-info/top_level.txt
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)     3182 2023-04-09 21:03:55.000000 pibooth-stillimage-camera-0.1.4/pibooth_stillimage_camera.py
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)     1326 2023-04-09 21:13:22.000000 pibooth-stillimage-camera-0.1.4/pyproject.toml
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)       38 2023-04-09 21:13:28.358734 pibooth-stillimage-camera-0.1.4/setup.cfg
```

### Comparing `pibooth-stillimage-camera-0.1.3/LICENSE` & `pibooth-stillimage-camera-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pibooth-stillimage-camera-0.1.3/PKG-INFO` & `pibooth-stillimage-camera-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pibooth-stillimage-camera
-Version: 0.1.3
+Version: 0.1.4
 Summary: Dummy camera for pibooth, producing still images for testing
 License: AGPLv3
 Project-URL: Homepage, https://gitlab.com/wolface/wolfoto-project/pibooth-stillimage-camera
 Keywords: Raspberry Pi,camera,photobooth,pibooth
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `pibooth-stillimage-camera-0.1.3/README.md` & `pibooth-stillimage-camera-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pibooth-stillimage-camera-0.1.3/pibooth_stillimage_camera.egg-info/PKG-INFO` & `pibooth-stillimage-camera-0.1.4/pibooth_stillimage_camera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pibooth-stillimage-camera
-Version: 0.1.3
+Version: 0.1.4
 Summary: Dummy camera for pibooth, producing still images for testing
 License: AGPLv3
 Project-URL: Homepage, https://gitlab.com/wolface/wolfoto-project/pibooth-stillimage-camera
 Keywords: Raspberry Pi,camera,photobooth,pibooth
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `pibooth-stillimage-camera-0.1.3/pibooth_stillimage_camera.py` & `pibooth-stillimage-camera-0.1.4/pibooth_stillimage_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import pibooth
 
 from pibooth.utils import LOGGER
 from pibooth import fonts
 from pibooth.camera.base import BaseCamera
 
-__version__ = "0.1.0"
+__version__ = "0.1.4"
 
 class SiCamera(BaseCamera):
     """Dummy camera, showing a still image, for tests"""
     def __init__(self, camera_proxy=None, background_color='pink', foreground_color='black'):
         self.dummy_text = "Still image for tests"
         self.dummy_background = background_color
         self.dummy_foreground = foreground_color
```

### Comparing `pibooth-stillimage-camera-0.1.3/pyproject.toml` & `pibooth-stillimage-camera-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pibooth-stillimage-camera"
-version = "0.1.3"
+dynamic = ["version"]
 description = "Dummy camera for pibooth, producing still images for testing"
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "AGPLv3" }
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Other Environment',
@@ -35,10 +35,13 @@
 "pibooth_stillimage_camera" = "pibooth_stillimage_camera"
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
-[tools.setuptools]
-py-modules = ["pibooth_stillimage_camera.py"]
+[tool.setuptools]
+py-modules = ["pibooth_stillimage_camera"]
 zip-safe = false
+
+[tool.setuptools.dynamic]
+version = {attr = "pibooth_stillimage_camera.__version__" }
```

