# Comparing `tmp/porteratzolibs-0.1.1.tar.gz` & `tmp/porteratzolibs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "porteratzolibs-0.1.1.tar", last modified: Sun Apr  9 03:57:34 2023, max compression
+gzip compressed data, was "porteratzolibs-0.1.2.tar", last modified: Sun Apr  9 04:01:55 2023, max compression
```

## Comparing `porteratzolibs-0.1.1.tar` & `porteratzolibs-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,40 @@
-drwxrwxr-x   0 omar      (1000) omar      (1000)        0 2023-04-09 03:57:34.730241 porteratzolibs-0.1.1/
--rw-rw-r--   0 omar      (1000) omar      (1000)     1067 2023-03-22 05:37:34.000000 porteratzolibs-0.1.1/LICENSE
--rw-rw-r--   0 omar      (1000) omar      (1000)      349 2023-04-09 03:57:34.730241 porteratzolibs-0.1.1/PKG-INFO
--rw-rw-r--   0 omar      (1000) omar      (1000)       45 2023-04-09 03:56:03.000000 porteratzolibs-0.1.1/README.md
-drwxrwxr-x   0 omar      (1000) omar      (1000)        0 2023-04-09 03:57:34.730241 porteratzolibs-0.1.1/porteratzolibs.egg-info/
--rw-rw-r--   0 omar      (1000) omar      (1000)      349 2023-04-09 03:57:34.000000 porteratzolibs-0.1.1/porteratzolibs.egg-info/PKG-INFO
--rw-rw-r--   0 omar      (1000) omar      (1000)      215 2023-04-09 03:57:34.000000 porteratzolibs-0.1.1/porteratzolibs.egg-info/SOURCES.txt
--rw-rw-r--   0 omar      (1000) omar      (1000)        1 2023-04-09 03:57:34.000000 porteratzolibs-0.1.1/porteratzolibs.egg-info/dependency_links.txt
--rw-rw-r--   0 omar      (1000) omar      (1000)       45 2023-04-09 03:57:34.000000 porteratzolibs-0.1.1/porteratzolibs.egg-info/requires.txt
--rw-rw-r--   0 omar      (1000) omar      (1000)       15 2023-04-09 03:57:34.000000 porteratzolibs-0.1.1/porteratzolibs.egg-info/top_level.txt
--rw-rw-r--   0 omar      (1000) omar      (1000)       38 2023-04-09 03:57:34.730241 porteratzolibs-0.1.1/setup.cfg
--rw-rw-r--   0 omar      (1000) omar      (1000)      661 2023-04-09 03:57:30.000000 porteratzolibs-0.1.1/setup.py
+drwxrwxr-x   0 omar      (1000) omar      (1000)        0 2023-04-09 04:01:55.227228 porteratzolibs-0.1.2/
+-rw-rw-r--   0 omar      (1000) omar      (1000)     1067 2023-03-22 05:37:34.000000 porteratzolibs-0.1.2/LICENSE
+drwxrwxr-x   0 omar      (1000) omar      (1000)        0 2023-04-09 04:01:55.227228 porteratzolibs-0.1.2/Legacy/
+-rwxrwxrwx   0 omar      (1000) omar      (1000)    26663 2023-01-05 01:20:20.000000 porteratzolibs-0.1.2/Legacy/ARUSTUFF.py
+-rwxrwxrwx   0 omar      (1000) omar      (1000)    15114 2023-01-05 02:27:25.000000 porteratzolibs-0.1.2/Legacy/Corners.py
+-rwxrwxrwx   0 omar      (1000) omar      (1000)     5143 2023-01-05 01:20:20.000000 porteratzolibs-0.1.2/Legacy/LIDARFileSearch.py
+-rwxrwxrwx   0 omar      (1000) omar      (1000)     6784 2023-01-05 01:20:20.000000 porteratzolibs-0.1.2/Legacy/Legacy.py
+-rwxrwxrwx   0 omar      (1000) omar      (1000)    15375 2023-01-05 01:20:20.000000 porteratzolibs-0.1.2/Legacy/ModelsV2.py
+-rwxrwxrwx   0 omar      (1000) omar      (1000)    30009 2023-04-09 03:56:03.000000 porteratzolibs-0.1.2/Legacy/Plane.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)     9273 2023-01-05 02:37:36.000000 porteratzolibs-0.1.2/Legacy/VelLoader.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)        0 2023-04-09 04:01:32.000000 porteratzolibs-0.1.2/Legacy/__init__.py
+-rwxrwxr-x   0 omar      (1000) omar      (1000)    10941 2023-04-09 03:56:03.000000 porteratzolibs-0.1.2/Legacy/py_util.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)      349 2023-04-09 04:01:55.227228 porteratzolibs-0.1.2/PKG-INFO
+-rw-rw-r--   0 omar      (1000) omar      (1000)       45 2023-04-09 03:56:03.000000 porteratzolibs-0.1.2/README.md
+drwxrwxr-x   0 omar      (1000) omar      (1000)        0 2023-04-09 04:01:55.227228 porteratzolibs-0.1.2/porteratzolibs/
+drwxrwxr-x   0 omar      (1000) omar      (1000)        0 2023-04-09 04:01:55.227228 porteratzolibs-0.1.2/porteratzolibs/Misc/
+-rwxrwxrwx   0 omar      (1000) omar      (1000)     2914 2023-03-22 05:39:05.000000 porteratzolibs-0.1.2/porteratzolibs/Misc/CameraStuff.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)        0 2023-01-05 22:25:54.000000 porteratzolibs-0.1.2/porteratzolibs/Misc/__init__.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)     1682 2023-03-22 05:39:51.000000 porteratzolibs-0.1.2/porteratzolibs/Misc/geometry.py
+-rwxrwxr-x   0 omar      (1000) omar      (1000)     6057 2023-03-22 05:39:18.000000 porteratzolibs-0.1.2/porteratzolibs/Misc/tictoc.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)     3835 2023-01-05 22:37:05.000000 porteratzolibs-0.1.2/porteratzolibs/Misc/transforms.py
+drwxrwxr-x   0 omar      (1000) omar      (1000)        0 2023-04-09 04:01:55.227228 porteratzolibs-0.1.2/porteratzolibs/ThreeDProcessing/
+-rwxrwxr-x   0 omar      (1000) omar      (1000)     3192 2023-04-09 03:56:03.000000 porteratzolibs-0.1.2/porteratzolibs/ThreeDProcessing/ThreeDPreocessing.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)        0 2023-01-05 22:25:53.000000 porteratzolibs-0.1.2/porteratzolibs/ThreeDProcessing/__init__.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)    14206 2023-01-05 20:25:15.000000 porteratzolibs-0.1.2/porteratzolibs/ThreeDProcessing/pclpy_utils.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)        0 2023-04-09 04:00:10.000000 porteratzolibs-0.1.2/porteratzolibs/__init__.py
+drwxrwxr-x   0 omar      (1000) omar      (1000)        0 2023-04-09 04:01:55.227228 porteratzolibs-0.1.2/porteratzolibs/visualization_o3d/
+-rw-rw-r--   0 omar      (1000) omar      (1000)        0 2023-01-05 22:25:52.000000 porteratzolibs-0.1.2/porteratzolibs/visualization_o3d/__init__.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)     1975 2023-04-09 03:56:03.000000 porteratzolibs-0.1.2/porteratzolibs/visualization_o3d/create_geometries.py
+-rw-rw-r--   0 omar      (1000) omar      (1000)     4842 2023-04-09 03:56:03.000000 porteratzolibs-0.1.2/porteratzolibs/visualization_o3d/open3d_pointsetClass.py
+-rwxrwxrwx   0 omar      (1000) omar      (1000)      730 2023-01-10 03:47:28.000000 porteratzolibs-0.1.2/porteratzolibs/visualization_o3d/open3d_utils.py
+-rwxrwxrwx   0 omar      (1000) omar      (1000)    12070 2023-04-09 03:56:03.000000 porteratzolibs-0.1.2/porteratzolibs/visualization_o3d/open3dvis.py
+drwxrwxr-x   0 omar      (1000) omar      (1000)        0 2023-04-09 04:01:55.227228 porteratzolibs-0.1.2/porteratzolibs.egg-info/
+-rw-rw-r--   0 omar      (1000) omar      (1000)      349 2023-04-09 04:01:55.000000 porteratzolibs-0.1.2/porteratzolibs.egg-info/PKG-INFO
+-rw-rw-r--   0 omar      (1000) omar      (1000)      972 2023-04-09 04:01:55.000000 porteratzolibs-0.1.2/porteratzolibs.egg-info/SOURCES.txt
+-rw-rw-r--   0 omar      (1000) omar      (1000)        1 2023-04-09 04:01:55.000000 porteratzolibs-0.1.2/porteratzolibs.egg-info/dependency_links.txt
+-rw-rw-r--   0 omar      (1000) omar      (1000)       45 2023-04-09 04:01:55.000000 porteratzolibs-0.1.2/porteratzolibs.egg-info/requires.txt
+-rw-rw-r--   0 omar      (1000) omar      (1000)       22 2023-04-09 04:01:55.000000 porteratzolibs-0.1.2/porteratzolibs.egg-info/top_level.txt
+-rw-rw-r--   0 omar      (1000) omar      (1000)       38 2023-04-09 04:01:55.227228 porteratzolibs-0.1.2/setup.cfg
+-rw-rw-r--   0 omar      (1000) omar      (1000)      687 2023-04-09 04:01:50.000000 porteratzolibs-0.1.2/setup.py
```

### Comparing `porteratzolibs-0.1.1/LICENSE` & `porteratzolibs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `porteratzolibs-0.1.1/setup.py` & `porteratzolibs-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+import setuptools
 from setuptools import setup
 
 setup(
     name='porteratzolibs',
-    version='0.1.1',    
+    version='0.1.2',    
     description='Collection of utils',
     url='https://github.com/porteratzo/porteratzolibs',
     author='Omar Montoya',
     author_email='omar.alfonso.montoya@hotmail.com',
     license='MIT License',
-    packages=['porteratzolibs'],
+    packages=setuptools.find_packages(),
     install_requires=['matplotlib',
                       'numpy', 
                       'open3d',
                       'pandas',
                       'opencv-python',                    
                       ],
```

