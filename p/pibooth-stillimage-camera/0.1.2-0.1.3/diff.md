# Comparing `tmp/pibooth-stillimage-camera-0.1.2.tar.gz` & `tmp/pibooth-stillimage-camera-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pibooth-stillimage-camera-0.1.2.tar", last modified: Sun Apr  9 16:21:24 2023, max compression
+gzip compressed data, was "pibooth-stillimage-camera-0.1.3.tar", last modified: Sun Apr  9 19:22:48 2023, max compression
```

## Comparing `pibooth-stillimage-camera-0.1.2.tar` & `pibooth-stillimage-camera-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 gilou     (1000) gilou     (1000)        0 2023-04-09 16:21:24.046278 pibooth-stillimage-camera-0.1.2/
--rw-rw-r--   0 gilou     (1000) gilou     (1000)    34476 2023-04-09 10:19:41.000000 pibooth-stillimage-camera-0.1.2/LICENSE
--rw-rw-r--   0 gilou     (1000) gilou     (1000)     2077 2023-04-09 16:21:24.046278 pibooth-stillimage-camera-0.1.2/PKG-INFO
--rw-rw-r--   0 gilou     (1000) gilou     (1000)     1175 2023-04-09 16:08:24.000000 pibooth-stillimage-camera-0.1.2/README.md
-drwxrwxr-x   0 gilou     (1000) gilou     (1000)        0 2023-04-09 16:21:24.046278 pibooth-stillimage-camera-0.1.2/pibooth_stillimage_camera.egg-info/
--rw-rw-r--   0 gilou     (1000) gilou     (1000)     2077 2023-04-09 16:21:24.000000 pibooth-stillimage-camera-0.1.2/pibooth_stillimage_camera.egg-info/PKG-INFO
--rw-rw-r--   0 gilou     (1000) gilou     (1000)      357 2023-04-09 16:21:24.000000 pibooth-stillimage-camera-0.1.2/pibooth_stillimage_camera.egg-info/SOURCES.txt
--rw-rw-r--   0 gilou     (1000) gilou     (1000)        1 2023-04-09 16:21:24.000000 pibooth-stillimage-camera-0.1.2/pibooth_stillimage_camera.egg-info/dependency_links.txt
--rw-rw-r--   0 gilou     (1000) gilou     (1000)       64 2023-04-09 16:21:24.000000 pibooth-stillimage-camera-0.1.2/pibooth_stillimage_camera.egg-info/entry_points.txt
--rw-rw-r--   0 gilou     (1000) gilou     (1000)       14 2023-04-09 16:21:24.000000 pibooth-stillimage-camera-0.1.2/pibooth_stillimage_camera.egg-info/requires.txt
--rw-rw-r--   0 gilou     (1000) gilou     (1000)       26 2023-04-09 16:21:24.000000 pibooth-stillimage-camera-0.1.2/pibooth_stillimage_camera.egg-info/top_level.txt
--rw-rw-r--   0 gilou     (1000) gilou     (1000)     3182 2023-04-09 10:21:48.000000 pibooth-stillimage-camera-0.1.2/pibooth_stillimage_camera.py
--rw-rw-r--   0 gilou     (1000) gilou     (1000)     1126 2023-04-09 16:21:06.000000 pibooth-stillimage-camera-0.1.2/pyproject.toml
--rw-rw-r--   0 gilou     (1000) gilou     (1000)       38 2023-04-09 16:21:24.046278 pibooth-stillimage-camera-0.1.2/setup.cfg
+drwxrwxr-x   0 gilou     (1000) gilou     (1000)        0 2023-04-09 19:22:48.907290 pibooth-stillimage-camera-0.1.3/
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)    34476 2023-04-09 10:19:41.000000 pibooth-stillimage-camera-0.1.3/LICENSE
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)     2139 2023-04-09 19:22:48.907290 pibooth-stillimage-camera-0.1.3/PKG-INFO
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)     1175 2023-04-09 16:08:24.000000 pibooth-stillimage-camera-0.1.3/README.md
+drwxrwxr-x   0 gilou     (1000) gilou     (1000)        0 2023-04-09 19:22:48.907290 pibooth-stillimage-camera-0.1.3/pibooth_stillimage_camera.egg-info/
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)     2139 2023-04-09 19:22:48.000000 pibooth-stillimage-camera-0.1.3/pibooth_stillimage_camera.egg-info/PKG-INFO
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)      357 2023-04-09 19:22:48.000000 pibooth-stillimage-camera-0.1.3/pibooth_stillimage_camera.egg-info/SOURCES.txt
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)        1 2023-04-09 19:22:48.000000 pibooth-stillimage-camera-0.1.3/pibooth_stillimage_camera.egg-info/dependency_links.txt
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)       64 2023-04-09 19:22:48.000000 pibooth-stillimage-camera-0.1.3/pibooth_stillimage_camera.egg-info/entry_points.txt
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)       14 2023-04-09 19:22:48.000000 pibooth-stillimage-camera-0.1.3/pibooth_stillimage_camera.egg-info/requires.txt
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)       26 2023-04-09 19:22:48.000000 pibooth-stillimage-camera-0.1.3/pibooth_stillimage_camera.egg-info/top_level.txt
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)     3182 2023-04-09 17:28:06.000000 pibooth-stillimage-camera-0.1.3/pibooth_stillimage_camera.py
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)     1239 2023-04-09 19:20:30.000000 pibooth-stillimage-camera-0.1.3/pyproject.toml
+-rw-rw-r--   0 gilou     (1000) gilou     (1000)       38 2023-04-09 19:22:48.907290 pibooth-stillimage-camera-0.1.3/setup.cfg
```

### Comparing `pibooth-stillimage-camera-0.1.2/LICENSE` & `pibooth-stillimage-camera-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pibooth-stillimage-camera-0.1.2/PKG-INFO` & `pibooth-stillimage-camera-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: pibooth-stillimage-camera
-Version: 0.1.2
+Version: 0.1.3
 Summary: Dummy camera for pibooth, producing still images for testing
 License: AGPLv3
 Project-URL: Homepage, https://gitlab.com/wolface/wolfoto-project/pibooth-stillimage-camera
-Classifier: Development Status :: 4 - Beta
+Keywords: Raspberry Pi,camera,photobooth,pibooth
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pibooth-stillimage-camera-0.1.2/README.md` & `pibooth-stillimage-camera-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pibooth-stillimage-camera-0.1.2/pibooth_stillimage_camera.egg-info/PKG-INFO` & `pibooth-stillimage-camera-0.1.3/pibooth_stillimage_camera.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: pibooth-stillimage-camera
-Version: 0.1.2
+Version: 0.1.3
 Summary: Dummy camera for pibooth, producing still images for testing
 License: AGPLv3
 Project-URL: Homepage, https://gitlab.com/wolface/wolfoto-project/pibooth-stillimage-camera
-Classifier: Development Status :: 4 - Beta
+Keywords: Raspberry Pi,camera,photobooth,pibooth
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pibooth-stillimage-camera-0.1.2/pibooth_stillimage_camera.py` & `pibooth-stillimage-camera-0.1.3/pibooth_stillimage_camera.py`

 * *Files identical despite different names*

### Comparing `pibooth-stillimage-camera-0.1.2/pyproject.toml` & `pibooth-stillimage-camera-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 [project]
 name = "pibooth-stillimage-camera"
-version = "0.1.2"
+version = "0.1.3"
 description = "Dummy camera for pibooth, producing still images for testing"
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "AGPLv3" }
 classifiers = [
-    'Development Status :: 4 - Beta',
+    'Development Status :: 5 - Production/Stable',
     'Environment :: Other Environment',
     'Intended Audience :: Developers',
     'Intended Audience :: End Users/Desktop',
     'License :: OSI Approved :: GNU Affero General Public License v3',
     'Operating System :: POSIX :: Linux',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Natural Language :: English',
     'Topic :: Multimedia :: Graphics :: Capture :: Digital Camera',
 ]
+keywords = [
+	'Raspberry Pi',
+        'camera',
+        'photobooth',
+	'pibooth',
+]
 dependencies = [
 	"pibooth>2.0.0",
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/wolface/wolfoto-project/pibooth-stillimage-camera"
 
@@ -31,8 +37,8 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [tools.setuptools]
 py-modules = ["pibooth_stillimage_camera.py"]
-
+zip-safe = false
```

