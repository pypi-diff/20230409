# Comparing `tmp/mss-7.0.1.tar.gz` & `tmp/mss-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mss-7.0.1.tar", last modified: Thu Oct 27 07:09:44 2022, max compression
+gzip compressed data, was "mss-8.0.0.tar", last modified: Sun Apr  9 17:14:33 2023, max compression
```

## Comparing `mss-7.0.1.tar` & `mss-8.0.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2022-10-27 07:09:44.272235 mss-7.0.1/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1093 2022-10-27 01:34:09.000000 mss-7.0.1/LICENSE
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       88 2022-10-27 01:33:30.000000 mss-7.0.1/MANIFEST.in
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3515 2022-10-27 07:09:44.272235 mss-7.0.1/PKG-INFO
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2177 2022-10-27 03:56:49.000000 mss-7.0.1/README.rst
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2022-10-27 07:09:44.268235 mss-7.0.1/mss/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      940 2022-10-27 07:07:58.000000 mss-7.0.1/mss/__init__.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2542 2022-10-27 02:27:00.000000 mss-7.0.1/mss/__main__.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     6282 2022-10-27 02:53:45.000000 mss-7.0.1/mss/base.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     7573 2022-10-27 03:36:12.000000 mss-7.0.1/mss/darwin.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      342 2022-10-27 02:27:00.000000 mss-7.0.1/mss/exception.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      911 2022-10-27 02:36:50.000000 mss-7.0.1/mss/factory.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    13875 2022-10-27 03:36:12.000000 mss-7.0.1/mss/linux.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      416 2022-10-27 02:52:39.000000 mss-7.0.1/mss/models.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3971 2022-10-27 03:01:03.000000 mss-7.0.1/mss/screenshot.py
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2022-10-27 07:09:44.268235 mss-7.0.1/mss/tests/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1566 2022-10-27 02:10:59.000000 mss-7.0.1/mss/tests/bench_bgra2rgb.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1327 2022-10-27 02:11:02.000000 mss-7.0.1/mss/tests/bench_general.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1635 2022-10-27 03:26:38.000000 mss-7.0.1/mss/tests/conftest.py
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2022-10-27 07:09:44.268235 mss-7.0.1/mss/tests/res/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)  3145728 2022-10-27 01:33:30.000000 mss-7.0.1/mss/tests/res/monitor-1024x768.raw
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      501 2022-10-27 02:10:55.000000 mss-7.0.1/mss/tests/test_bgra_to_rgb.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      487 2022-10-27 02:11:13.000000 mss-7.0.1/mss/tests/test_cls_image.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      744 2022-10-27 02:11:16.000000 mss-7.0.1/mss/tests/test_find_monitors.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1526 2022-10-27 02:11:20.000000 mss-7.0.1/mss/tests/test_get_pixels.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3320 2022-10-27 02:11:26.000000 mss-7.0.1/mss/tests/test_gnu_linux.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     5142 2022-10-27 02:27:00.000000 mss-7.0.1/mss/tests/test_implementation.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3003 2022-10-27 03:41:43.000000 mss-7.0.1/mss/tests/test_leaks.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1719 2022-10-27 02:12:18.000000 mss-7.0.1/mss/tests/test_macos.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1815 2022-10-27 02:12:23.000000 mss-7.0.1/mss/tests/test_save.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      579 2022-10-27 03:58:54.000000 mss-7.0.1/mss/tests/test_setup.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2248 2022-10-27 02:12:40.000000 mss-7.0.1/mss/tests/test_third_party.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1913 2022-10-27 02:12:46.000000 mss-7.0.1/mss/tests/test_tools.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1866 2022-10-27 02:12:50.000000 mss-7.0.1/mss/tests/test_windows.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1942 2022-10-27 02:36:30.000000 mss-7.0.1/mss/tools.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     9306 2022-10-27 03:36:12.000000 mss-7.0.1/mss/windows.py
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2022-10-27 07:09:44.268235 mss-7.0.1/mss.egg-info/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3515 2022-10-27 07:09:44.000000 mss-7.0.1/mss.egg-info/PKG-INFO
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      843 2022-10-27 07:09:44.000000 mss-7.0.1/mss.egg-info/SOURCES.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        1 2022-10-27 07:09:44.000000 mss-7.0.1/mss.egg-info/dependency_links.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       42 2022-10-27 07:09:44.000000 mss-7.0.1/mss.egg-info/entry_points.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        1 2022-10-27 07:07:11.000000 mss-7.0.1/mss.egg-info/not-zip-safe
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        4 2022-10-27 07:09:44.000000 mss-7.0.1/mss.egg-info/top_level.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1764 2022-10-27 07:09:44.272235 mss-7.0.1/setup.cfg
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       39 2022-10-27 01:33:30.000000 mss-7.0.1/setup.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 17:14:33.609279 mss-8.0.0/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1093 2023-01-01 09:58:18.000000 mss-8.0.0/LICENSE
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       88 2021-08-03 16:40:06.000000 mss-8.0.0/MANIFEST.in
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3578 2023-04-09 17:14:33.609279 mss-8.0.0/PKG-INFO
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2199 2023-04-09 16:24:40.000000 mss-8.0.0/README.rst
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 17:14:33.601280 mss-8.0.0/mss/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      940 2023-04-08 11:57:14.000000 mss-8.0.0/mss/__init__.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2646 2023-04-09 16:40:38.000000 mss-8.0.0/mss/__main__.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     8606 2023-04-09 16:24:40.000000 mss-8.0.0/mss/base.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     7513 2023-04-09 16:24:40.000000 mss-8.0.0/mss/darwin.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      368 2023-04-09 16:24:40.000000 mss-8.0.0/mss/exception.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      911 2023-01-01 09:57:58.000000 mss-8.0.0/mss/factory.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    14900 2023-04-09 16:31:22.000000 mss-8.0.0/mss/linux.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      416 2023-01-01 09:57:58.000000 mss-8.0.0/mss/models.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3859 2023-04-09 16:24:40.000000 mss-8.0.0/mss/screenshot.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 17:14:33.605280 mss-8.0.0/mss/tests/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1566 2023-01-01 09:57:58.000000 mss-8.0.0/mss/tests/bench_bgra2rgb.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1327 2023-01-01 09:57:58.000000 mss-8.0.0/mss/tests/bench_general.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1382 2023-04-08 11:57:14.000000 mss-8.0.0/mss/tests/conftest.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 17:14:33.605280 mss-8.0.0/mss/tests/res/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)  3145728 2021-08-03 16:40:06.000000 mss-8.0.0/mss/tests/res/monitor-1024x768.raw
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      501 2023-01-01 09:57:58.000000 mss-8.0.0/mss/tests/test_bgra_to_rgb.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      573 2023-04-08 11:57:14.000000 mss-8.0.0/mss/tests/test_cls_image.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      863 2023-04-08 11:57:14.000000 mss-8.0.0/mss/tests/test_find_monitors.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1777 2023-04-08 11:57:14.000000 mss-8.0.0/mss/tests/test_get_pixels.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     5383 2023-04-09 16:24:40.000000 mss-8.0.0/mss/tests/test_gnu_linux.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     5505 2023-04-08 11:57:14.000000 mss-8.0.0/mss/tests/test_implementation.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1242 2023-04-09 16:24:40.000000 mss-8.0.0/mss/tests/test_issue_220.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3530 2023-04-08 11:57:14.000000 mss-8.0.0/mss/tests/test_leaks.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1719 2023-01-01 09:57:58.000000 mss-8.0.0/mss/tests/test_macos.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2242 2023-04-08 11:57:14.000000 mss-8.0.0/mss/tests/test_save.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      666 2023-04-08 11:57:14.000000 mss-8.0.0/mss/tests/test_setup.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2475 2023-04-08 11:57:14.000000 mss-8.0.0/mss/tests/test_third_party.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1969 2023-04-08 11:57:14.000000 mss-8.0.0/mss/tests/test_tools.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1866 2023-01-01 09:57:58.000000 mss-8.0.0/mss/tests/test_windows.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1928 2023-04-09 16:24:40.000000 mss-8.0.0/mss/tools.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     9290 2023-04-09 16:24:40.000000 mss-8.0.0/mss/windows.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 17:14:33.605280 mss-8.0.0/mss.egg-info/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3578 2023-04-09 17:14:33.000000 mss-8.0.0/mss.egg-info/PKG-INFO
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      871 2023-04-09 17:14:33.000000 mss-8.0.0/mss.egg-info/SOURCES.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        1 2023-04-09 17:14:33.000000 mss-8.0.0/mss.egg-info/dependency_links.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       42 2023-04-09 17:14:33.000000 mss-8.0.0/mss.egg-info/entry_points.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        1 2023-04-08 11:57:57.000000 mss-8.0.0/mss.egg-info/not-zip-safe
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        4 2023-04-09 17:14:33.000000 mss-8.0.0/mss.egg-info/top_level.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1865 2023-04-09 17:14:33.609279 mss-8.0.0/setup.cfg
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       39 2021-08-03 16:40:06.000000 mss-8.0.0/setup.py
```

### Comparing `mss-7.0.1/LICENSE` & `mss-8.0.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 MIT License
-Copyright (c) 2016-2022, Mickaël 'Tiger-222' Schoentgen
+Copyright (c) 2013-2023, Mickaël 'Tiger-222' Schoentgen
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `mss-7.0.1/PKG-INFO` & `mss-8.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 Metadata-Version: 2.1
 Name: mss
-Version: 7.0.1
+Version: 8.0.0
 Summary: An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 Home-page: https://github.com/BoboTiG/python-mss
 Author: Mickaël 'Tiger-222' Schoentgen
 Author-email: contact@tiger-222.fr
 License: MIT
 Project-URL: Documentation, https://python-mss.readthedocs.io
 Project-URL: Source, https://github.com/BoboTiG/python-mss
 Project-URL: Tracker, https://github.com/BoboTiG/python-mss/issues
 Keywords: screen,screenshot,screencapture,screengrab
 Platform: Darwin
 Platform: Linux
 Platform: Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics :: Capture :: Screen Capture
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Python MSS
 ==========
 
-.. image:: https://travis-ci.org/BoboTiG/python-mss.svg?branch=master
-    :target: https://travis-ci.org/BoboTiG/python-mss
-.. image:: https://ci.appveyor.com/api/projects/status/72dik18r6b746mb0?svg=true
-    :target: https://ci.appveyor.com/project/BoboTiG/python-mss
-.. image:: https://img.shields.io/badge/say-thanks-ff69b4.svg
-    :target: https://saythanks.io/to/BoboTiG
-.. image:: https://pepy.tech/badge/mss
-    :target: https://pepy.tech/project/mss
-.. image:: https://anaconda.org/conda-forge/python-mss/badges/installer/conda.svg
+.. image:: https://badge.fury.io/py/mss.svg
+    :target: https://pypi.org/project/mss/
+.. image:: https://anaconda.org/conda-forge/python-mss/badges/version.svg
     :target: https://anaconda.org/conda-forge/python-mss
+.. image:: https://github.com/BoboTiG/python-mss/actions/workflows/tests.yml/badge.svg?branch=master
+    :target: https://github.com/BoboTiG/python-mss/actions/workflows/tests.yml
+.. image:: https://static.pepy.tech/personalized-badge/mss?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
+    :target: https://pepy.tech/project/mss
 
 
 .. code-block:: python
 
     from mss import mss
 
     # The simplest use, save a screen shot of the 1st monitor
     with mss() as sct:
         sct.shot()
 
 
 An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 
-- **Python 3.5+** and PEP8 compliant, no dependency, thread-safe;
+- **Python 3.8+** and PEP8 compliant, no dependency, thread-safe;
 - very basic, it will grab one screen shot by monitor or a screen shot of all monitors and save it to a PNG file;
 - but you can use PIL and benefit from all its formats (or add yours directly);
 - integrate well with Numpy and OpenCV;
 - it could be easily embedded into games and other software which require fast and platform optimized methods to grab screen shots (like AI, Computer Vision);
 - get the `source code on GitHub <https://github.com/BoboTiG/python-mss>`_;
 - learn with a `bunch of examples <https://python-mss.readthedocs.io/examples.html>`_;
 - you can `report a bug <https://github.com/BoboTiG/python-mss/issues>`_;
@@ -79,12 +77,13 @@
 Or you can install it with conda::
 
     conda install -c conda-forge python-mss
 
 Maintenance
 -----------
 
-For the maintainers, here are commands to upload a new release:
+For the maintainers, here are commands to upload a new release::
 
+    rm -rf build dist
     python -m build --sdist --wheel
     twine check dist/*
     twine upload dist/*
```

### Comparing `mss-7.0.1/README.rst` & `mss-8.0.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Python MSS
 ==========
 
-.. image:: https://travis-ci.org/BoboTiG/python-mss.svg?branch=master
-    :target: https://travis-ci.org/BoboTiG/python-mss
-.. image:: https://ci.appveyor.com/api/projects/status/72dik18r6b746mb0?svg=true
-    :target: https://ci.appveyor.com/project/BoboTiG/python-mss
-.. image:: https://img.shields.io/badge/say-thanks-ff69b4.svg
-    :target: https://saythanks.io/to/BoboTiG
-.. image:: https://pepy.tech/badge/mss
-    :target: https://pepy.tech/project/mss
-.. image:: https://anaconda.org/conda-forge/python-mss/badges/installer/conda.svg
+.. image:: https://badge.fury.io/py/mss.svg
+    :target: https://pypi.org/project/mss/
+.. image:: https://anaconda.org/conda-forge/python-mss/badges/version.svg
     :target: https://anaconda.org/conda-forge/python-mss
+.. image:: https://github.com/BoboTiG/python-mss/actions/workflows/tests.yml/badge.svg?branch=master
+    :target: https://github.com/BoboTiG/python-mss/actions/workflows/tests.yml
+.. image:: https://static.pepy.tech/personalized-badge/mss?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
+    :target: https://pepy.tech/project/mss
 
 
 .. code-block:: python
 
     from mss import mss
 
     # The simplest use, save a screen shot of the 1st monitor
     with mss() as sct:
         sct.shot()
 
 
 An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 
-- **Python 3.5+** and PEP8 compliant, no dependency, thread-safe;
+- **Python 3.8+** and PEP8 compliant, no dependency, thread-safe;
 - very basic, it will grab one screen shot by monitor or a screen shot of all monitors and save it to a PNG file;
 - but you can use PIL and benefit from all its formats (or add yours directly);
 - integrate well with Numpy and OpenCV;
 - it could be easily embedded into games and other software which require fast and platform optimized methods to grab screen shots (like AI, Computer Vision);
 - get the `source code on GitHub <https://github.com/BoboTiG/python-mss>`_;
 - learn with a `bunch of examples <https://python-mss.readthedocs.io/examples.html>`_;
 - you can `report a bug <https://github.com/BoboTiG/python-mss/issues>`_;
@@ -47,12 +45,13 @@
 Or you can install it with conda::
 
     conda install -c conda-forge python-mss
 
 Maintenance
 -----------
 
-For the maintainers, here are commands to upload a new release:
+For the maintainers, here are commands to upload a new release::
 
+    rm -rf build dist
     python -m build --sdist --wheel
     twine check dist/*
     twine upload dist/*
```

### Comparing `mss-7.0.1/mss/__init__.py` & `mss-8.0.0/mss/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 You can always get the latest version of this module at:
     https://github.com/BoboTiG/python-mss
 If that URL should fail, try contacting the author.
 """
 from .exception import ScreenShotError
 from .factory import mss
 
-__version__ = "7.0.1"
+__version__ = "8.0.0"
 __author__ = "Mickaël 'Tiger-222' Schoentgen"
 __copyright__ = """
-Copyright (c) 2013-2022, Mickaël 'Tiger-222' Schoentgen
+Copyright (c) 2013-2023, Mickaël 'Tiger-222' Schoentgen
 
 Permission to use, copy, modify, and distribute this software and its
 documentation for any purpose and without fee or royalty is hereby
 granted, provided that the above copyright notice appear in all copies
 and that both that copyright notice and this permission notice appear
 in supporting documentation or portions thereof, including
 modifications, that you make.
```

### Comparing `mss-7.0.1/mss/__main__.py` & `mss-8.0.0/mss/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 This is part of the MSS Python's module.
 Source: https://github.com/BoboTiG/python-mss
 """
 import os.path
 from argparse import ArgumentParser
-from typing import List, Optional
+from typing import List
 
 from . import __version__
 from .exception import ScreenShotError
 from .factory import mss
 from .tools import to_png
 
 
-def main(args: Optional[List[str]] = None) -> int:
+def main(args: List[str], /) -> int:
     """Main logic."""
 
     cli_args = ArgumentParser()
     cli_args.add_argument(
         "-c",
         "--coordinates",
         default="",
@@ -27,20 +27,17 @@
         "-l",
         "--level",
         default=6,
         type=int,
         choices=list(range(10)),
         help="the PNG compression level",
     )
-    cli_args.add_argument(
-        "-m", "--monitor", default=0, type=int, help="the monitor to screen shot"
-    )
-    cli_args.add_argument(
-        "-o", "--output", default="monitor-{mon}.png", help="the output file name"
-    )
+    cli_args.add_argument("-m", "--monitor", default=0, type=int, help="the monitor to screen shot")
+    cli_args.add_argument("-o", "--output", default="monitor-{mon}.png", help="the output file name")
+    cli_args.add_argument("--with-cursor", default=False, action="store_true", help="include the cursor")
     cli_args.add_argument(
         "-q",
         "--quiet",
         default=False,
         action="store_true",
         help="do not print created files",
     )
@@ -61,15 +58,15 @@
             "width": int(width),
             "height": int(height),
         }
         if options.output == "monitor-{mon}.png":
             kwargs["output"] = "sct-{top}x{left}_{width}x{height}.png"
 
     try:
-        with mss() as sct:
+        with mss(with_cursor=options.with_cursor) as sct:
             if options.coordinates:
                 output = kwargs["output"].format(**kwargs["mon"])
                 sct_img = sct.grab(kwargs["mon"])
                 to_png(sct_img.rgb, sct_img.size, level=options.level, output=output)
                 if not options.quiet:
                     print(os.path.realpath(output))
             else:
@@ -77,11 +74,11 @@
                     if not options.quiet:
                         print(os.path.realpath(file_name))
             return 0
     except ScreenShotError:
         return 1
 
 
-if __name__ == "__main__":
+if __name__ == "__main__":  # pragma: nocover
     import sys
 
     sys.exit(main(sys.argv[1:]))
```

### Comparing `mss-7.0.1/mss/base.py` & `mss-8.0.0/mss/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,33 +14,47 @@
 
 lock = Lock()
 
 
 class MSSBase(metaclass=ABCMeta):
     """This class will be overloaded by a system specific one."""
 
-    __slots__ = {"_monitors", "cls_image", "compression_level"}
+    __slots__ = {"_monitors", "cls_image", "compression_level", "with_cursor"}
 
-    def __init__(self) -> None:
+    def __init__(
+        self,
+        /,
+        *,
+        compression_level: int = 6,
+        display: Optional[Union[bytes, str]] = None,  # Linux only
+        max_displays: int = 32,  # Mac only
+        with_cursor: bool = False,
+    ) -> None:
+        # pylint: disable=unused-argument
         self.cls_image: Type[ScreenShot] = ScreenShot
-        self.compression_level = 6
+        self.compression_level = compression_level
+        self.with_cursor = with_cursor
         self._monitors: Monitors = []
 
     def __enter__(self) -> "MSSBase":
         """For the cool call `with MSS() as mss:`."""
 
         return self
 
     def __exit__(self, *_: Any) -> None:
         """For the cool call `with MSS() as mss:`."""
 
         self.close()
 
     @abstractmethod
-    def _grab_impl(self, monitor: Monitor) -> ScreenShot:
+    def _cursor_impl(self) -> Optional[ScreenShot]:
+        """Retrieve all cursor data. Pixels have to be RGB."""
+
+    @abstractmethod
+    def _grab_impl(self, monitor: Monitor, /) -> ScreenShot:
         """
         Retrieve all pixels from a monitor. Pixels have to be RGB.
         That method has to be run using a threading lock.
         """
 
     @abstractmethod
     def _monitors_impl(self) -> None:
@@ -48,15 +62,15 @@
         Get positions of monitors (has to be run using a threading lock).
         It must populate self._monitors.
         """
 
     def close(self) -> None:
         """Clean-up."""
 
-    def grab(self, monitor: Union[Monitor, Tuple[int, int, int, int]]) -> ScreenShot:
+    def grab(self, monitor: Union[Monitor, Tuple[int, int, int, int]], /) -> ScreenShot:
         """
         Retrieve screen pixels for a given monitor.
 
         Note: *monitor* can be a tuple like the one PIL.Image.grab() accepts.
 
         :param monitor: The coordinates and size of the box to capture.
                         See :meth:`monitors <monitors>` for object details.
@@ -69,15 +83,19 @@
                 "left": monitor[0],
                 "top": monitor[1],
                 "width": monitor[2] - monitor[0],
                 "height": monitor[3] - monitor[1],
             }
 
         with lock:
-            return self._grab_impl(monitor)
+            screenshot = self._grab_impl(monitor)
+            if self.with_cursor:
+                cursor = self._cursor_impl()
+                screenshot = self._merge(screenshot, cursor)  # type: ignore[arg-type]
+            return screenshot
 
     @property
     def monitors(self) -> Monitors:
         """
         Get positions of all monitors.
         If the monitor has rotation, you have to deal with it
         inside this method.
@@ -100,17 +118,19 @@
             with lock:
                 self._monitors_impl()
 
         return self._monitors
 
     def save(
         self,
+        /,
+        *,
         mon: int = 0,
         output: str = "monitor-{mon}.png",
-        callback: Callable[[str], None] = None,
+        callback: Optional[Callable[[str], None]] = None,
     ) -> Iterator[str]:
         """
         Grab a screen shot and save it to a file.
 
         :param int mon: The monitor to screen shot (default=0).
                         -1: grab one screen shot of all monitors
                          0: grab one screen shot by monitor
@@ -150,40 +170,88 @@
                 yield fname
         else:
             # A screen shot of all monitors together or
             # a screen shot of the monitor N.
             mon = 0 if mon == -1 else mon
             try:
                 monitor = monitors[mon]
-            except IndexError:
-                # pylint: disable=raise-missing-from
-                raise ScreenShotError(f"Monitor {mon!r} does not exist.")
+            except IndexError as exc:
+                raise ScreenShotError(f"Monitor {mon!r} does not exist.") from exc
 
             output = output.format(mon=mon, date=datetime.now(), **monitor)
             if callable(callback):
                 callback(output)
             sct = self.grab(monitor)
             to_png(sct.rgb, sct.size, level=self.compression_level, output=output)
             yield output
 
-    def shot(self, **kwargs: Any) -> str:
+    def shot(self, /, **kwargs: Any) -> str:
         """
         Helper to save the screen shot of the 1st monitor, by default.
         You can pass the same arguments as for ``save``.
         """
 
         kwargs["mon"] = kwargs.get("mon", 1)
         return next(self.save(**kwargs))
 
     @staticmethod
+    def _merge(screenshot: ScreenShot, cursor: ScreenShot, /) -> ScreenShot:
+        """Create composite image by blending screenshot and mouse cursor."""
+
+        # pylint: disable=too-many-locals,invalid-name
+
+        (cx, cy), (cw, ch) = cursor.pos, cursor.size
+        (x, y), (w, h) = screenshot.pos, screenshot.size
+
+        cx2, cy2 = cx + cw, cy + ch
+        x2, y2 = x + w, y + h
+
+        overlap = cx < x2 and cx2 > x and cy < y2 and cy2 > y
+        if not overlap:
+            return screenshot
+
+        screen_data = screenshot.raw
+        cursor_data = cursor.raw
+
+        cy, cy2 = (cy - y) * 4, (cy2 - y2) * 4
+        cx, cx2 = (cx - x) * 4, (cx2 - x2) * 4
+        start_count_y = -cy if cy < 0 else 0
+        start_count_x = -cx if cx < 0 else 0
+        stop_count_y = ch * 4 - max(cy2, 0)
+        stop_count_x = cw * 4 - max(cx2, 0)
+        rgb = range(3)
+
+        for count_y in range(start_count_y, stop_count_y, 4):
+            pos_s = (count_y + cy) * w + cx
+            pos_c = count_y * cw
+
+            for count_x in range(start_count_x, stop_count_x, 4):
+                spos = pos_s + count_x
+                cpos = pos_c + count_x
+                alpha = cursor_data[cpos + 3]
+
+                if not alpha:
+                    continue
+
+                if alpha == 255:
+                    screen_data[spos : spos + 3] = cursor_data[cpos : cpos + 3]
+                else:
+                    alpha = alpha / 255
+                    for i in rgb:
+                        screen_data[spos + i] = int(cursor_data[cpos + i] * alpha + screen_data[spos + i] * (1 - alpha))
+
+        return screenshot
+
+    @staticmethod
     def _cfactory(
         attr: Any,
         func: str,
         argtypes: List[Any],
         restype: Any,
+        /,
         errcheck: Optional[Callable] = None,
     ) -> None:
         """Factory to create a ctypes function and automatically manage errors."""
 
         meth = getattr(attr, func)
         meth.argtypes = argtypes
         meth.restype = restype
```

### Comparing `mss-7.0.1/mss/darwin.py` & `mss-8.0.0/mss/darwin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,17 @@
 """
 This is part of the MSS Python's module.
 Source: https://github.com/BoboTiG/python-mss
 """
 import ctypes
 import ctypes.util
 import sys
-from ctypes import (
-    POINTER,
-    Structure,
-    c_double,
-    c_float,
-    c_int32,
-    c_ubyte,
-    c_uint32,
-    c_uint64,
-    c_void_p,
-)
+from ctypes import POINTER, Structure, c_double, c_float, c_int32, c_ubyte, c_uint32, c_uint64, c_void_p
 from platform import mac_ver
-from typing import Any, Type, Union
+from typing import Any, Optional, Type, Union
 
 from .base import MSSBase
 from .exception import ScreenShotError
 from .models import CFunctions, Monitor
 from .screenshot import ScreenShot, Size
 
 __all__ = ("MSS",)
@@ -72,48 +62,40 @@
     "CGDataProviderCopyData": ("core", [c_void_p], c_void_p),
     "CGDisplayBounds": ("core", [c_uint32], CGRect),
     "CGDisplayRotation": ("core", [c_uint32], c_float),
     "CFDataGetBytePtr": ("core", [c_void_p], c_void_p),
     "CFDataGetLength": ("core", [c_void_p], c_uint64),
     "CFRelease": ("core", [c_void_p], c_void_p),
     "CGDataProviderRelease": ("core", [c_void_p], c_void_p),
-    "CGGetActiveDisplayList": (
-        "core",
-        [c_uint32, POINTER(c_uint32), POINTER(c_uint32)],
-        c_int32,
-    ),
+    "CGGetActiveDisplayList": ("core", [c_uint32, POINTER(c_uint32), POINTER(c_uint32)], c_int32),
     "CGImageGetBitsPerPixel": ("core", [c_void_p], int),
     "CGImageGetBytesPerRow": ("core", [c_void_p], int),
     "CGImageGetDataProvider": ("core", [c_void_p], c_void_p),
     "CGImageGetHeight": ("core", [c_void_p], int),
     "CGImageGetWidth": ("core", [c_void_p], int),
     "CGRectStandardize": ("core", [CGRect], CGRect),
     "CGRectUnion": ("core", [CGRect, CGRect], CGRect),
-    "CGWindowListCreateImage": (
-        "core",
-        [CGRect, c_uint32, c_uint32, c_uint32],
-        c_void_p,
-    ),
+    "CGWindowListCreateImage": ("core", [CGRect, c_uint32, c_uint32, c_uint32], c_void_p),
 }
 
 
 class MSS(MSSBase):
     """
     Multiple ScreenShots implementation for macOS.
     It uses intensively the CoreGraphics library.
     """
 
     __slots__ = {"core", "max_displays"}
 
-    def __init__(self, **_: Any) -> None:
+    def __init__(self, /, **kwargs: Any) -> None:
         """macOS initialisations."""
 
-        super().__init__()
+        super().__init__(**kwargs)
 
-        self.max_displays = 32
+        self.max_displays = kwargs.get("max_displays", 32)
 
         self._init_library()
         self._set_cfunctions()
 
     def _init_library(self) -> None:
         """Load the CoreGraphics library."""
         version = float(".".join(mac_ver()[0].split(".")[:2]))
@@ -130,20 +112,15 @@
 
     def _set_cfunctions(self) -> None:
         """Set all ctypes functions and attach them to attributes."""
 
         cfactory = self._cfactory
         attrs = {"core": self.core}
         for func, (attr, argtypes, restype) in CFUNCTIONS.items():
-            cfactory(
-                attr=attrs[attr],
-                func=func,
-                argtypes=argtypes,
-                restype=restype,
-            )
+            cfactory(attrs[attr], func, argtypes, restype)
 
     def _monitors_impl(self) -> None:
         """Get positions of monitors. It will populate self._monitors."""
 
         int_ = int
         core = self.core
 
@@ -152,17 +129,15 @@
         # using CGRectUnion.  Else we will end with infinite values.
         all_monitors = CGRect()
         self._monitors.append({})
 
         # Each monitor
         display_count = c_uint32(0)
         active_displays = (c_uint32 * self.max_displays)()
-        core.CGGetActiveDisplayList(
-            self.max_displays, active_displays, ctypes.byref(display_count)
-        )
+        core.CGGetActiveDisplayList(self.max_displays, active_displays, ctypes.byref(display_count))
         rotations = {0.0: "normal", 90.0: "right", -90.0: "left"}
         for idx in range(display_count.value):
             display = active_displays[idx]
             rect = core.CGDisplayBounds(display)
             rect = core.CGRectStandardize(rect)
             width, height = rect.size.width, rect.size.height
             rot = core.CGDisplayRotation(display)
@@ -184,23 +159,21 @@
         self._monitors[0] = {
             "left": int_(all_monitors.origin.x),
             "top": int_(all_monitors.origin.y),
             "width": int_(all_monitors.size.width),
             "height": int_(all_monitors.size.height),
         }
 
-    def _grab_impl(self, monitor: Monitor) -> ScreenShot:
+    def _grab_impl(self, monitor: Monitor, /) -> ScreenShot:
         """Retrieve all pixels from a monitor. Pixels have to be RGB."""
 
         # pylint: disable=too-many-locals
 
         core = self.core
-        rect = CGRect(
-            (monitor["left"], monitor["top"]), (monitor["width"], monitor["height"])
-        )
+        rect = CGRect((monitor["left"], monitor["top"]), (monitor["width"], monitor["height"]))
 
         image_ref = core.CGWindowListCreateImage(rect, 1, 0, 0)
         if not image_ref:
             raise ScreenShotError("CoreGraphics.CGWindowListCreateImage() failed.")
 
         width = core.CGImageGetWidth(image_ref)
         height = core.CGImageGetHeight(image_ref)
@@ -228,7 +201,11 @@
         finally:
             if prov:
                 core.CGDataProviderRelease(prov)
             if copy_data:
                 core.CFRelease(copy_data)
 
         return self.cls_image(data, monitor, size=Size(width, height))
+
+    def _cursor_impl(self) -> Optional[ScreenShot]:
+        """Retrieve all cursor data. Pixels have to be RGB."""
+        return None
```

### Comparing `mss-7.0.1/mss/factory.py` & `mss-8.0.0/mss/factory.py`

 * *Files identical despite different names*

### Comparing `mss-7.0.1/mss/linux.py` & `mss-8.0.0/mss/linux.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 """
 This is part of the MSS Python's module.
 Source: https://github.com/BoboTiG/python-mss
 """
-import contextlib
-import ctypes
-import ctypes.util
 import os
-import threading
+from contextlib import suppress
 from ctypes import (
     CFUNCTYPE,
     POINTER,
     Structure,
+    byref,
     c_char_p,
     c_int,
     c_int32,
     c_long,
+    c_short,
     c_ubyte,
     c_uint,
     c_uint32,
     c_ulong,
     c_ushort,
     c_void_p,
+    cast,
+    cdll,
+    create_string_buffer,
 )
-from types import SimpleNamespace
-from typing import Any, Dict, Optional, Tuple, Union
+from ctypes.util import find_library
+from threading import current_thread, local
+from typing import Any, Tuple
 
 from .base import MSSBase, lock
 from .exception import ScreenShotError
 from .models import CFunctions, Monitor
 from .screenshot import ScreenShot
 
 __all__ = ("MSS",)
 
 
-ERROR = SimpleNamespace(details=None)
 PLAINMASK = 0x00FFFFFF
 ZPIXMAP = 2
 
 
 class Display(Structure):
     """
     Structure that serves as the connection to the X server
@@ -58,41 +60,32 @@
         ("error_code", c_ubyte),
         ("request_code", c_ubyte),
         ("minor_code", c_ubyte),
         ("resourceid", c_void_p),
     ]
 
 
-class XWindowAttributes(Structure):
-    """Attributes for the specified window."""
+class XFixesCursorImage(Structure):
+    """
+    Cursor structure.
+    /usr/include/X11/extensions/Xfixes.h
+    https://github.com/freedesktop/xorg-libXfixes/blob/libXfixes-6.0.0/include/X11/extensions/Xfixes.h#L96
+    """
 
     _fields_ = [
-        ("x", c_int32),
-        ("y", c_int32),
-        ("width", c_int32),
-        ("height", c_int32),
-        ("border_width", c_int32),
-        ("depth", c_int32),
-        ("visual", c_ulong),
-        ("root", c_ulong),
-        ("class", c_int32),
-        ("bit_gravity", c_int32),
-        ("win_gravity", c_int32),
-        ("backing_store", c_int32),
-        ("backing_planes", c_ulong),
-        ("backing_pixel", c_ulong),
-        ("save_under", c_int32),
-        ("colourmap", c_ulong),
-        ("mapinstalled", c_uint32),
-        ("map_state", c_uint32),
-        ("all_event_masks", c_ulong),
-        ("your_event_mask", c_ulong),
-        ("do_not_propagate_mask", c_ulong),
-        ("override_redirect", c_int32),
-        ("screen", c_ulong),
+        ("x", c_short),
+        ("y", c_short),
+        ("width", c_ushort),
+        ("height", c_ushort),
+        ("xhot", c_ushort),
+        ("yhot", c_ushort),
+        ("cursor_serial", c_ulong),
+        ("pixels", POINTER(c_ulong)),
+        ("atom", c_ulong),
+        ("name", c_char_p),
     ]
 
 
 class XImage(Structure):
     """
     Description of an image as it exists in the client's memory.
     https://tronche.com/gui/x/xlib/graphics/images.html
@@ -113,14 +106,33 @@
         ("bits_per_pixel", c_int),
         ("red_mask", c_ulong),
         ("green_mask", c_ulong),
         ("blue_mask", c_ulong),
     ]
 
 
+class XRRCrtcInfo(Structure):
+    """Structure that contains CRTC information."""
+
+    _fields_ = [
+        ("timestamp", c_ulong),
+        ("x", c_int),
+        ("y", c_int),
+        ("width", c_int),
+        ("height", c_int),
+        ("mode", c_long),
+        ("rotation", c_int),
+        ("noutput", c_int),
+        ("outputs", POINTER(c_long)),
+        ("rotations", c_ushort),
+        ("npossible", c_int),
+        ("possible", POINTER(c_long)),
+    ]
+
+
 class XRRModeInfo(Structure):
     """Voilà, voilà."""
 
 
 class XRRScreenResources(Structure):
     """
     Structure that contains arrays of XIDs that point to the
@@ -135,285 +147,259 @@
         ("noutput", c_int),
         ("outputs", POINTER(c_long)),
         ("nmode", c_int),
         ("modes", POINTER(XRRModeInfo)),
     ]
 
 
-class XRRCrtcInfo(Structure):
-    """Structure that contains CRTC information."""
+class XWindowAttributes(Structure):
+    """Attributes for the specified window."""
 
     _fields_ = [
-        ("timestamp", c_ulong),
-        ("x", c_int),
-        ("y", c_int),
-        ("width", c_int),
-        ("height", c_int),
-        ("mode", c_long),
-        ("rotation", c_int),
-        ("noutput", c_int),
-        ("outputs", POINTER(c_long)),
-        ("rotations", c_ushort),
-        ("npossible", c_int),
-        ("possible", POINTER(c_long)),
+        ("x", c_int32),
+        ("y", c_int32),
+        ("width", c_int32),
+        ("height", c_int32),
+        ("border_width", c_int32),
+        ("depth", c_int32),
+        ("visual", c_ulong),
+        ("root", c_ulong),
+        ("class", c_int32),
+        ("bit_gravity", c_int32),
+        ("win_gravity", c_int32),
+        ("backing_store", c_int32),
+        ("backing_planes", c_ulong),
+        ("backing_pixel", c_ulong),
+        ("save_under", c_int32),
+        ("colourmap", c_ulong),
+        ("mapinstalled", c_uint32),
+        ("map_state", c_uint32),
+        ("all_event_masks", c_ulong),
+        ("your_event_mask", c_ulong),
+        ("do_not_propagate_mask", c_ulong),
+        ("override_redirect", c_int32),
+        ("screen", c_ulong),
     ]
 
 
+_ERROR = {}
+_X11 = find_library("X11")
+_XFIXES = find_library("Xfixes")
+_XRANDR = find_library("Xrandr")
+
+
+@CFUNCTYPE(c_int, POINTER(Display), POINTER(Event))
+def _default_error_handler(display: Display, event: Event) -> int:
+    """
+    Specifies the default program's supplied error handler.
+    It's useful when exiting MSS to prevent letting `_error_handler()` as default handler.
+    Doing so would crash when using Tk/Tkinter, see issue #220.
+
+    Interesting technical stuff can be found here:
+        https://core.tcl-lang.org/tk/file?name=generic/tkError.c&ci=a527ef995862cb50
+        https://github.com/tcltk/tk/blob/b9cdafd83fe77499ff47fa373ce037aff3ae286a/generic/tkError.c
+    """
+    # pylint: disable=unused-argument
+    return 0  # pragma: nocover
+
+
 @CFUNCTYPE(c_int, POINTER(Display), POINTER(Event))
-def error_handler(_: Any, event: Any) -> int:
+def _error_handler(display: Display, event: Event) -> int:
     """Specifies the program's supplied error handler."""
+
+    # Get the specific error message
+    xlib = cdll.LoadLibrary(_X11)  # type: ignore[arg-type]
+    get_error = xlib.XGetErrorText
+    get_error.argtypes = [POINTER(Display), c_int, c_char_p, c_int]
+    get_error.restype = c_void_p
+
     evt = event.contents
-    ERROR.details = {
-        "type": evt.type,
-        "serial": evt.serial,
+    error = create_string_buffer(1024)
+    get_error(display, evt.error_code, error, len(error))
+
+    _ERROR[current_thread()] = {
+        "error": error.value.decode("utf-8"),
         "error_code": evt.error_code,
-        "request_code": evt.request_code,
         "minor_code": evt.minor_code,
+        "request_code": evt.request_code,
+        "serial": evt.serial,
+        "type": evt.type,
     }
+
     return 0
 
 
-def validate(
-    retval: int, func: Any, args: Tuple[Any, Any]
-) -> Optional[Tuple[Any, Any]]:
+def _validate(retval: int, func: Any, args: Tuple[Any, Any], /) -> Tuple[Any, Any]:
     """Validate the returned value of a Xlib or XRANDR function."""
 
-    if retval != 0 and not ERROR.details:
+    thread = current_thread()
+    if retval != 0 and thread not in _ERROR:
         return args
 
-    details = {"retval": retval, "args": args}
+    details = _ERROR.pop(thread, {})
     raise ScreenShotError(f"{func.__name__}() failed", details=details)
 
 
 # C functions that will be initialised later.
 # See https://tronche.com/gui/x/xlib/function-index.html for details.
 #
 # This is a dict:
 #    cfunction: (attr, argtypes, restype)
 #
-# Available attr: xlib, xrandr.
+# Available attr: xfixes, xlib, xrandr.
 #
 # Note: keep it sorted by cfunction.
 CFUNCTIONS: CFunctions = {
+    "XCloseDisplay": ("xlib", [POINTER(Display)], c_void_p),
     "XDefaultRootWindow": ("xlib", [POINTER(Display)], POINTER(XWindowAttributes)),
     "XDestroyImage": ("xlib", [POINTER(XImage)], c_void_p),
-    "XGetErrorText": ("xlib", [POINTER(Display), c_int, c_char_p, c_int], c_void_p),
+    "XFixesGetCursorImage": ("xfixes", [POINTER(Display)], POINTER(XFixesCursorImage)),
     "XGetImage": (
         "xlib",
-        [
-            POINTER(Display),
-            POINTER(Display),
-            c_int,
-            c_int,
-            c_uint,
-            c_uint,
-            c_ulong,
-            c_int,
-        ],
+        [POINTER(Display), POINTER(Display), c_int, c_int, c_uint, c_uint, c_ulong, c_int],
         POINTER(XImage),
     ),
-    "XGetWindowAttributes": (
-        "xlib",
-        [POINTER(Display), POINTER(XWindowAttributes), POINTER(XWindowAttributes)],
-        c_int,
-    ),
+    "XGetWindowAttributes": ("xlib", [POINTER(Display), POINTER(XWindowAttributes), POINTER(XWindowAttributes)], c_int),
     "XOpenDisplay": ("xlib", [c_char_p], POINTER(Display)),
-    "XQueryExtension": (
-        "xlib",
-        [
-            POINTER(Display),
-            c_char_p,
-            POINTER(c_int),
-            POINTER(c_int),
-            POINTER(c_int),
-        ],
-        c_uint,
-    ),
+    "XQueryExtension": ("xlib", [POINTER(Display), c_char_p, POINTER(c_int), POINTER(c_int), POINTER(c_int)], c_uint),
     "XRRFreeCrtcInfo": ("xrandr", [POINTER(XRRCrtcInfo)], c_void_p),
     "XRRFreeScreenResources": ("xrandr", [POINTER(XRRScreenResources)], c_void_p),
-    "XRRGetCrtcInfo": (
-        "xrandr",
-        [POINTER(Display), POINTER(XRRScreenResources), c_long],
-        POINTER(XRRCrtcInfo),
-    ),
-    "XRRGetScreenResources": (
-        "xrandr",
-        [POINTER(Display), POINTER(Display)],
-        POINTER(XRRScreenResources),
-    ),
-    "XRRGetScreenResourcesCurrent": (
-        "xrandr",
-        [POINTER(Display), POINTER(Display)],
-        POINTER(XRRScreenResources),
-    ),
+    "XRRGetCrtcInfo": ("xrandr", [POINTER(Display), POINTER(XRRScreenResources), c_long], POINTER(XRRCrtcInfo)),
+    "XRRGetScreenResources": ("xrandr", [POINTER(Display), POINTER(Display)], POINTER(XRRScreenResources)),
+    "XRRGetScreenResourcesCurrent": ("xrandr", [POINTER(Display), POINTER(Display)], POINTER(XRRScreenResources)),
     "XSetErrorHandler": ("xlib", [c_void_p], c_int),
 }
 
 
 class MSS(MSSBase):
     """
     Multiple ScreenShots implementation for GNU/Linux.
     It uses intensively the Xlib and its Xrandr extension.
     """
 
-    __slots__ = {"drawable", "root", "xlib", "xrandr"}
-
-    # A dict to maintain *display* values created by multiple threads.
-    _display_dict: Dict[threading.Thread, int] = {}
+    __slots__ = {"xfixes", "xlib", "xrandr", "_handles"}
 
-    def __init__(self, display: Optional[Union[bytes, str]] = None) -> None:
+    def __init__(self, /, **kwargs: Any) -> None:
         """GNU/Linux initialisations."""
 
-        super().__init__()
+        super().__init__(**kwargs)
 
+        display = kwargs.get("display", b"")
         if not display:
             try:
                 display = os.environ["DISPLAY"].encode("utf-8")
             except KeyError:
-                # pylint: disable=raise-missing-from
-                raise ScreenShotError("$DISPLAY not set.")
+                raise ScreenShotError("$DISPLAY not set.") from None
 
         if not isinstance(display, bytes):
             display = display.encode("utf-8")
 
         if b":" not in display:
             raise ScreenShotError(f"Bad display value: {display!r}.")
 
-        x11 = ctypes.util.find_library("X11")
-        if not x11:
+        if not _X11:
             raise ScreenShotError("No X11 library found.")
-        self.xlib = ctypes.cdll.LoadLibrary(x11)
+        self.xlib = cdll.LoadLibrary(_X11)
 
         # Install the error handler to prevent interpreter crashes:
         # any error will raise a ScreenShotError exception.
-        self.xlib.XSetErrorHandler(error_handler)
+        self.xlib.XSetErrorHandler(_error_handler)
 
-        xrandr = ctypes.util.find_library("Xrandr")
-        if not xrandr:
+        if not _XRANDR:
             raise ScreenShotError("No Xrandr extension found.")
-        self.xrandr = ctypes.cdll.LoadLibrary(xrandr)
+        self.xrandr = cdll.LoadLibrary(_XRANDR)
+
+        if self.with_cursor:
+            if _XFIXES:
+                self.xfixes = cdll.LoadLibrary(_XFIXES)
+            else:
+                self.with_cursor = False
 
         self._set_cfunctions()
 
-        self.root = self.xlib.XDefaultRootWindow(self._get_display(display))
+        self._handles = local()
+        self._handles.display = self.xlib.XOpenDisplay(display)
 
-        if not self.has_extension("RANDR"):
-            raise ScreenShotError("No Xrandr extension found.")
+        if not self._is_extension_enabled("RANDR"):
+            raise ScreenShotError("Xrandr not enabled.")
+
+        self._handles.root = self.xlib.XDefaultRootWindow(self._handles.display)
 
         # Fix for XRRGetScreenResources and XGetImage:
         #     expected LP_Display instance instead of LP_XWindowAttributes
-        self.drawable = ctypes.cast(self.root, POINTER(Display))
+        self._handles.drawable = cast(self._handles.root, POINTER(Display))
+
+    def close(self) -> None:
+        # Remove our error handler
+        self.xlib.XSetErrorHandler(_default_error_handler)
+
+        # Clean-up
+        if self._handles.display is not None:
+            self.xlib.XCloseDisplay(self._handles.display)
+            self._handles.display = None
+
+        # Also empty the error dict
+        _ERROR.clear()
 
-    def has_extension(self, extension: str) -> bool:
-        """Return True if the given *extension* is part of the extensions list of the server."""
+    def _is_extension_enabled(self, name: str, /) -> bool:
+        """Return True if the given *extension* is enabled on the server."""
         with lock:
             major_opcode_return = c_int()
             first_event_return = c_int()
             first_error_return = c_int()
 
             try:
                 self.xlib.XQueryExtension(
-                    self._get_display(),
-                    extension.encode("latin1"),
-                    ctypes.byref(major_opcode_return),
-                    ctypes.byref(first_event_return),
-                    ctypes.byref(first_error_return),
+                    self._handles.display,
+                    name.encode("latin1"),
+                    byref(major_opcode_return),
+                    byref(first_event_return),
+                    byref(first_error_return),
                 )
             except ScreenShotError:
                 return False
-            else:
-                return True
-
-    def _get_display(self, disp: Optional[bytes] = None) -> int:
-        """
-        Retrieve a thread-safe display from XOpenDisplay().
-        In multithreading, if the thread that creates *display* is dead, *display* will
-        no longer be valid to grab the screen. The *display* attribute is replaced
-        with *_display_dict* to maintain the *display* values in multithreading.
-        Since the current thread and main thread are always alive, reuse their
-        *display* value first.
-        """
-        cur_thread, main_thread = threading.current_thread(), threading.main_thread()
-        current_display = MSS._display_dict.get(cur_thread) or MSS._display_dict.get(
-            main_thread
-        )
-        if current_display:
-            display = current_display
-        else:
-            display = self.xlib.XOpenDisplay(disp)
-            MSS._display_dict[cur_thread] = display
-        return display
+            return True
 
     def _set_cfunctions(self) -> None:
         """Set all ctypes functions and attach them to attributes."""
 
         cfactory = self._cfactory
         attrs = {
+            "xfixes": getattr(self, "xfixes", None),
             "xlib": self.xlib,
             "xrandr": self.xrandr,
         }
         for func, (attr, argtypes, restype) in CFUNCTIONS.items():
-            with contextlib.suppress(AttributeError):
-                cfactory(
-                    attr=attrs[attr],
-                    errcheck=validate,
-                    func=func,
-                    argtypes=argtypes,
-                    restype=restype,
-                )
-
-    def get_error_details(self) -> Optional[Dict[str, Any]]:
-        """Get more information about the latest X server error."""
-
-        details: Dict[str, Any] = {}
-
-        if ERROR.details:
-            details = {"xerror_details": ERROR.details}
-            ERROR.details = None
-            xserver_error = ctypes.create_string_buffer(1024)
-            self.xlib.XGetErrorText(
-                self._get_display(),
-                details.get("xerror_details", {}).get("error_code", 0),
-                xserver_error,
-                len(xserver_error),
-            )
-            xerror = xserver_error.value.decode("utf-8")
-            if xerror != "0":
-                details["xerror"] = xerror
-
-        return details
+            with suppress(AttributeError):
+                errcheck = None if func == "XSetErrorHandler" else _validate
+                cfactory(attrs[attr], func, argtypes, restype, errcheck=errcheck)
 
     def _monitors_impl(self) -> None:
         """Get positions of monitors. It will populate self._monitors."""
 
-        display = self._get_display()
+        display = self._handles.display
         int_ = int
         xrandr = self.xrandr
 
         # All monitors
         gwa = XWindowAttributes()
-        self.xlib.XGetWindowAttributes(display, self.root, ctypes.byref(gwa))
+        self.xlib.XGetWindowAttributes(display, self._handles.root, byref(gwa))
         self._monitors.append(
-            {
-                "left": int_(gwa.x),
-                "top": int_(gwa.y),
-                "width": int_(gwa.width),
-                "height": int_(gwa.height),
-            }
+            {"left": int_(gwa.x), "top": int_(gwa.y), "width": int_(gwa.width), "height": int_(gwa.height)}
         )
 
         # Each monitor
         # A simple benchmark calling 10 times those 2 functions:
         # XRRGetScreenResources():        0.1755971429956844 s
         # XRRGetScreenResourcesCurrent(): 0.0039125580078689 s
         # The second is faster by a factor of 44! So try to use it first.
         try:
-            mon = xrandr.XRRGetScreenResourcesCurrent(display, self.drawable).contents
+            mon = xrandr.XRRGetScreenResourcesCurrent(display, self._handles.drawable).contents
         except AttributeError:
-            mon = xrandr.XRRGetScreenResources(display, self.drawable).contents
+            mon = xrandr.XRRGetScreenResources(display, self._handles.drawable).contents
 
         crtcs = mon.crtcs
         for idx in range(mon.ncrtc):
             crtc = xrandr.XRRGetCrtcInfo(display, mon, crtcs[idx]).contents
             if crtc.noutput == 0:
                 xrandr.XRRFreeCrtcInfo(crtc)
                 continue
@@ -425,38 +411,63 @@
                     "width": int_(crtc.width),
                     "height": int_(crtc.height),
                 }
             )
             xrandr.XRRFreeCrtcInfo(crtc)
         xrandr.XRRFreeScreenResources(mon)
 
-    def _grab_impl(self, monitor: Monitor) -> ScreenShot:
+    def _grab_impl(self, monitor: Monitor, /) -> ScreenShot:
         """Retrieve all pixels from a monitor. Pixels have to be RGB."""
 
         ximage = self.xlib.XGetImage(
-            self._get_display(),
-            self.drawable,
+            self._handles.display,
+            self._handles.drawable,
             monitor["left"],
             monitor["top"],
             monitor["width"],
             monitor["height"],
             PLAINMASK,
             ZPIXMAP,
         )
 
         try:
             bits_per_pixel = ximage.contents.bits_per_pixel
             if bits_per_pixel != 32:
-                raise ScreenShotError(
-                    f"[XImage] bits per pixel value not (yet?) implemented: {bits_per_pixel}."
-                )
+                raise ScreenShotError(f"[XImage] bits per pixel value not (yet?) implemented: {bits_per_pixel}.")
 
-            raw_data = ctypes.cast(
+            raw_data = cast(
                 ximage.contents.data,
                 POINTER(c_ubyte * monitor["height"] * monitor["width"] * 4),
             )
             data = bytearray(raw_data.contents)
         finally:
             # Free
             self.xlib.XDestroyImage(ximage)
 
         return self.cls_image(data, monitor)
+
+    def _cursor_impl(self) -> ScreenShot:
+        """Retrieve all cursor data. Pixels have to be RGB."""
+
+        # Read data of cursor/mouse-pointer
+        ximage = self.xfixes.XFixesGetCursorImage(self._handles.display)
+        if not (ximage and ximage.contents):
+            raise ScreenShotError("Cannot read XFixesGetCursorImage()")
+
+        cursor_img: XFixesCursorImage = ximage.contents
+        region = {
+            "left": cursor_img.x - cursor_img.xhot,
+            "top": cursor_img.y - cursor_img.yhot,
+            "width": cursor_img.width,
+            "height": cursor_img.height,
+        }
+
+        raw_data = cast(cursor_img.pixels, POINTER(c_ulong * region["height"] * region["width"]))
+        raw = bytearray(raw_data.contents)
+
+        data = bytearray(region["height"] * region["width"] * 4)
+        data[3::4] = raw[3::8]
+        data[2::4] = raw[2::8]
+        data[1::4] = raw[1::8]
+        data[::4] = raw[::8]
+
+        return self.cls_image(data, region)
```

### Comparing `mss-7.0.1/mss/screenshot.py` & `mss-8.0.0/mss/screenshot.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 
         A better name would have  been *Image*, but to prevent collisions
         with PIL.Image, it has been decided to use *ScreenShot*.
     """
 
     __slots__ = {"__pixels", "__rgb", "pos", "raw", "size"}
 
-    def __init__(
-        self, data: bytearray, monitor: Monitor, size: Optional[Size] = None
-    ) -> None:
+    def __init__(self, data: bytearray, monitor: Monitor, /, *, size: Optional[Size] = None) -> None:
         self.__pixels: Optional[Pixels] = None
         self.__rgb: Optional[bytes] = None
 
         #: Bytearray of the raw BGRA pixels retrieved by ctypes
         #: OS independent implementations.
         self.raw = data
 
@@ -53,17 +51,15 @@
             "version": 3,
             "shape": (self.height, self.width, 4),
             "typestr": "|u1",
             "data": self.raw,
         }
 
     @classmethod
-    def from_size(
-        cls: Type["ScreenShot"], data: bytearray, width: int, height: int
-    ) -> "ScreenShot":
+    def from_size(cls: Type["ScreenShot"], data: bytearray, width: int, height: int, /) -> "ScreenShot":
         """Instantiate a new class given only screen shot's data and size."""
         monitor = {"left": 0, "top": 0, "width": width, "height": height}
         return cls(data, monitor)
 
     @property
     def bgra(self) -> bytes:
         """BGRA values from the BGRA raw pixels."""
@@ -82,17 +78,15 @@
     @property
     def pixels(self) -> Pixels:
         """
         :return list: RGB tuples.
         """
 
         if not self.__pixels:
-            rgb_tuples: Iterator[Pixel] = zip(
-                self.raw[2::4], self.raw[1::4], self.raw[::4]
-            )
+            rgb_tuples: Iterator[Pixel] = zip(self.raw[2::4], self.raw[1::4], self.raw[::4])
             self.__pixels = list(zip(*[iter(rgb_tuples)] * self.width))  # type: ignore
 
         return self.__pixels
 
     @property
     def rgb(self) -> bytes:
         """
@@ -128,12 +122,9 @@
         :param int coord_x: The x coordinate.
         :param int coord_y: The y coordinate.
         :return tuple: The pixel value as (R, G, B).
         """
 
         try:
             return self.pixels[coord_y][coord_x]  # type: ignore
-        except IndexError:
-            # pylint: disable=raise-missing-from
-            raise ScreenShotError(
-                f"Pixel location ({coord_x}, {coord_y}) is out of range."
-            )
+        except IndexError as exc:
+            raise ScreenShotError(f"Pixel location ({coord_x}, {coord_y}) is out of range.") from exc
```

### Comparing `mss-7.0.1/mss/tests/bench_bgra2rgb.py` & `mss-8.0.0/mss/tests/bench_bgra2rgb.py`

 * *Files identical despite different names*

### Comparing `mss-7.0.1/mss/tests/bench_general.py` & `mss-8.0.0/mss/tests/bench_general.py`

 * *Files identical despite different names*

### Comparing `mss-7.0.1/mss/tests/conftest.py` & `mss-8.0.0/mss/tests/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
 This is part of the MSS Python's module.
 Source: https://github.com/BoboTiG/python-mss
 """
 import glob
 import os
+from pathlib import Path
 
 import pytest
 
-import mss
+from mss import mss
 
 
 @pytest.fixture(autouse=True)
 def no_warnings(recwarn):
     """Fail on warning."""
 
     yield
 
-    warnings = [
-        "{w.filename}:{w.lineno} {w.message}".format(w=warning) for warning in recwarn
-    ]
+    warnings = ["{w.filename}:{w.lineno} {w.message}".format(w=warning) for warning in recwarn]
     for warning in warnings:
         print(warning)
     assert not warnings
 
 
 def purge_files():
     """Remove all generated files from previous runs."""
@@ -37,37 +36,22 @@
 
 
 @pytest.fixture(scope="module", autouse=True)
 def before_tests(request):
     request.addfinalizer(purge_files)
 
 
-@pytest.fixture(scope="module")
-def sct():
-    try:
-        # `display` kwarg is only for GNU/Linux
-        return mss.mss(display=os.getenv("DISPLAY"))
-    except TypeError:
-        return mss.mss()
-
-
 @pytest.fixture(scope="session")
-def is_travis():
-    return "TRAVIS" in os.environ
+def raw() -> bytes:
+    file = Path(__file__).parent / "res" / "monitor-1024x768.raw"
+    return file.read_bytes()
 
 
 @pytest.fixture(scope="session")
-def raw():
-    here = os.path.dirname(__file__)
-    file = os.path.join(here, "res", "monitor-1024x768.raw")
-    with open(file, "rb") as f:
-        yield f.read()
-
-
-@pytest.fixture(scope="module")
-def pixel_ratio(sct):
+def pixel_ratio() -> int:
     """Get the pixel, used to adapt test checks."""
     # Grab a 1x1 screenshot
     region = {"top": 0, "left": 0, "width": 1, "height": 1}
 
-    # On macOS with Retina display, the width will be 2 instead of 1
-    return sct.grab(region).size[0]
+    with mss(display=os.getenv("DISPLAY")) as sct:
+        # On macOS with Retina display, the width will be 2 instead of 1
+        return sct.grab(region).size[0]
```

### Comparing `mss-7.0.1/mss/tests/res/monitor-1024x768.raw` & `mss-8.0.0/mss/tests/res/monitor-1024x768.raw`

 * *Files identical despite different names*

### Comparing `mss-7.0.1/mss/tests/test_get_pixels.py` & `mss-8.0.0/mss/tests/test_get_pixels.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 """
 This is part of the MSS Python's module.
 Source: https://github.com/BoboTiG/python-mss
 """
+import os
+
 import pytest
 
+from mss import mss
 from mss.base import ScreenShot
 from mss.exception import ScreenShotError
 
 
-def test_grab_monitor(sct):
-    for mon in sct.monitors:
-        image = sct.grab(mon)
-        assert isinstance(image, ScreenShot)
-        assert isinstance(image.raw, bytearray)
-        assert isinstance(image.rgb, bytes)
+def test_grab_monitor():
+    with mss(display=os.getenv("DISPLAY")) as sct:
+        for mon in sct.monitors:
+            image = sct.grab(mon)
+            assert isinstance(image, ScreenShot)
+            assert isinstance(image.raw, bytearray)
+            assert isinstance(image.rgb, bytes)
 
 
-def test_grab_part_of_screen(sct, pixel_ratio):
+def test_grab_part_of_screen(pixel_ratio):
     monitor = {"top": 160, "left": 160, "width": 160, "height": 160}
-    image = sct.grab(monitor)
+    with mss(display=os.getenv("DISPLAY")) as sct:
+        image = sct.grab(monitor)
     assert isinstance(image, ScreenShot)
     assert isinstance(image.raw, bytearray)
     assert isinstance(image.rgb, bytes)
     assert image.top == 160
     assert image.left == 160
     assert image.width == 160 * pixel_ratio
     assert image.height == 160 * pixel_ratio
 
 
-def test_grab_part_of_screen_rounded(sct, pixel_ratio):
+def test_grab_part_of_screen_rounded(pixel_ratio):
     monitor = {"top": 160, "left": 160, "width": 161, "height": 159}
-    image = sct.grab(monitor)
+    with mss(display=os.getenv("DISPLAY")) as sct:
+        image = sct.grab(monitor)
     assert isinstance(image, ScreenShot)
     assert isinstance(image.raw, bytearray)
     assert isinstance(image.rgb, bytes)
     assert image.top == 160
     assert image.left == 160
     assert image.width == 161 * pixel_ratio
     assert image.height == 159 * pixel_ratio
 
 
-def test_grab_individual_pixels(sct):
+def test_grab_individual_pixels():
     monitor = {"top": 160, "left": 160, "width": 222, "height": 42}
-    image = sct.grab(monitor)
+    with mss(display=os.getenv("DISPLAY")) as sct:
+        image = sct.grab(monitor)
     assert isinstance(image.pixel(0, 0), tuple)
     with pytest.raises(ScreenShotError):
         image.pixel(image.width + 1, 12)
```

### Comparing `mss-7.0.1/mss/tests/test_implementation.py` & `mss-8.0.0/mss/tests/test_implementation.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 """
 import os
 import os.path
 import platform
 
 import pytest
 
-import mss
 import mss.tools
+from mss import mss
 from mss.base import MSSBase
 from mss.exception import ScreenShotError
 from mss.screenshot import ScreenShot
 
 
 class MSS0(MSSBase):
     """Nothing implemented."""
@@ -38,48 +38,50 @@
 
 @pytest.mark.parametrize("cls", [MSS0, MSS1, MSS2])
 def test_incomplete_class(cls):
     with pytest.raises(TypeError):
         cls()
 
 
-def test_bad_monitor(sct):
-    with pytest.raises(ScreenShotError):
-        sct.grab(sct.shot(mon=222))
+def test_bad_monitor():
+    with mss(display=os.getenv("DISPLAY")) as sct:
+        with pytest.raises(ScreenShotError):
+            sct.shot(mon=222)
 
 
-def test_repr(sct, pixel_ratio):
+def test_repr(pixel_ratio):
     box = {"top": 0, "left": 0, "width": 10, "height": 10}
     expected_box = {
         "top": 0,
         "left": 0,
         "width": 10 * pixel_ratio,
         "height": 10 * pixel_ratio,
     }
-    img = sct.grab(box)
+    with mss(display=os.getenv("DISPLAY")) as sct:
+        img = sct.grab(box)
     ref = ScreenShot(bytearray(b"42"), expected_box)
     assert repr(img) == repr(ref)
 
 
 def test_factory(monkeypatch):
     # Current system
-    with mss.mss() as sct:
+    with mss() as sct:
         assert isinstance(sct, MSSBase)
 
     # Unknown
     monkeypatch.setattr(platform, "system", lambda: "Chuck Norris")
     with pytest.raises(ScreenShotError) as exc:
-        mss.mss()
+        mss()
     monkeypatch.undo()
 
     error = exc.value.args[0]
     assert error == "System 'chuck norris' not (yet?) implemented."
 
 
-def test_entry_point(capsys, sct):
+def test_entry_point(capsys):
     from datetime import datetime
 
     from mss.__main__ import main
 
     for opt in ("-m", "--monitor"):
         main([opt, "1"])
         out, _ = capsys.readouterr()
@@ -94,19 +96,20 @@
         assert os.path.isfile("monitor-1.png")
         os.remove("monitor-1.png")
 
     fmt = "sct-{width}x{height}.png"
     for opt in ("-o", "--out"):
         main([opt, fmt])
         out, _ = capsys.readouterr()
-        for monitor, line in zip(sct.monitors[1:], out.splitlines()):
-            filename = fmt.format(**monitor)
-            assert line.endswith(filename)
-            assert os.path.isfile(filename)
-            os.remove(filename)
+        with mss(display=os.getenv("DISPLAY")) as sct:
+            for monitor, line in zip(sct.monitors[1:], out.splitlines()):
+                filename = fmt.format(**monitor)
+                assert line.endswith(filename)
+                assert os.path.isfile(filename)
+                os.remove(filename)
 
     fmt = "sct_{mon}-{date:%Y-%m-%d}.png"
     for opt in ("-o", "--out"):
         main(["-m 1", opt, fmt])
         filename = fmt.format(mon=1, date=datetime.now())
         out, _ = capsys.readouterr()
         assert out.endswith(filename + "\n")
@@ -125,68 +128,70 @@
     coordinates = "2,12,40"
     for opt in ("-c", "--coordinates"):
         main([opt, coordinates])
         out, _ = capsys.readouterr()
         assert out == "Coordinates syntax: top, left, width, height\n"
 
 
-def test_grab_with_tuple(sct, pixel_ratio):
+def test_grab_with_tuple(pixel_ratio):
     left = 100
     top = 100
     right = 500
     lower = 500
     width = right - left  # 400px width
     height = lower - top  # 400px height
 
-    # PIL like
-    box = (left, top, right, lower)
-    im = sct.grab(box)
-    assert im.size == (width * pixel_ratio, height * pixel_ratio)
-
-    # MSS like
-    box2 = {"left": left, "top": top, "width": width, "height": height}
-    im2 = sct.grab(box2)
-    assert im.size == im2.size
-    assert im.pos == im2.pos
-    assert im.rgb == im2.rgb
-
-
-def test_grab_with_tuple_percents(sct, pixel_ratio):
-    monitor = sct.monitors[1]
-    left = monitor["left"] + monitor["width"] * 5 // 100  # 5% from the left
-    top = monitor["top"] + monitor["height"] * 5 // 100  # 5% from the top
-    right = left + 500  # 500px
-    lower = top + 500  # 500px
-    width = right - left
-    height = lower - top
-
-    # PIL like
-    box = (left, top, right, lower)
-    im = sct.grab(box)
-    assert im.size == (width * pixel_ratio, height * pixel_ratio)
-
-    # MSS like
-    box2 = {"left": left, "top": top, "width": width, "height": height}
-    im2 = sct.grab(box2)
-    assert im.size == im2.size
-    assert im.pos == im2.pos
-    assert im.rgb == im2.rgb
+    with mss(display=os.getenv("DISPLAY")) as sct:
+        # PIL like
+        box = (left, top, right, lower)
+        im = sct.grab(box)
+        assert im.size == (width * pixel_ratio, height * pixel_ratio)
+
+        # MSS like
+        box2 = {"left": left, "top": top, "width": width, "height": height}
+        im2 = sct.grab(box2)
+        assert im.size == im2.size
+        assert im.pos == im2.pos
+        assert im.rgb == im2.rgb
+
+
+def test_grab_with_tuple_percents(pixel_ratio):
+    with mss(display=os.getenv("DISPLAY")) as sct:
+        monitor = sct.monitors[1]
+        left = monitor["left"] + monitor["width"] * 5 // 100  # 5% from the left
+        top = monitor["top"] + monitor["height"] * 5 // 100  # 5% from the top
+        right = left + 500  # 500px
+        lower = top + 500  # 500px
+        width = right - left
+        height = lower - top
+
+        # PIL like
+        box = (left, top, right, lower)
+        im = sct.grab(box)
+        assert im.size == (width * pixel_ratio, height * pixel_ratio)
+
+        # MSS like
+        box2 = {"left": left, "top": top, "width": width, "height": height}
+        im2 = sct.grab(box2)
+        assert im.size == im2.size
+        assert im.pos == im2.pos
+        assert im.rgb == im2.rgb
 
 
 def test_thread_safety():
     """Regression test for issue #169."""
     import threading
     import time
 
     def record(check):
         """Record for one second."""
 
         start_time = time.time()
         while time.time() - start_time < 1:
-            with mss.mss() as sct:
+            with mss() as sct:
                 sct.grab(sct.monitors[1])
 
         check[threading.current_thread()] = True
 
     checkpoint = {}
     t1 = threading.Thread(target=record, args=(checkpoint,))
     t2 = threading.Thread(target=record, args=(checkpoint,))
```

### Comparing `mss-7.0.1/mss/tests/test_macos.py` & `mss-8.0.0/mss/tests/test_macos.py`

 * *Files identical despite different names*

### Comparing `mss-7.0.1/mss/tests/test_third_party.py` & `mss-8.0.0/mss/tests/test_third_party.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,72 +4,78 @@
 """
 import itertools
 import os
 import os.path
 
 import pytest
 
+from mss import mss
+
 try:
     import numpy
 except (ImportError, RuntimeError):
     # RuntimeError on Python 3.9 (macOS): Polyfit sanity test emitted a warning, ...
     numpy = None
 
 try:
     from PIL import Image
 except ImportError:
     Image = None
 
 
 @pytest.mark.skipif(numpy is None, reason="Numpy module not available.")
-def test_numpy(sct, pixel_ratio):
+def test_numpy(pixel_ratio):
     box = {"top": 0, "left": 0, "width": 10, "height": 10}
-    img = numpy.array(sct.grab(box))
+    with mss(display=os.getenv("DISPLAY")) as sct:
+        img = numpy.array(sct.grab(box))
     assert len(img) == 10 * pixel_ratio
 
 
 @pytest.mark.skipif(Image is None, reason="PIL module not available.")
-def test_pil(sct):
+def test_pil():
     width, height = 16, 16
     box = {"top": 0, "left": 0, "width": width, "height": height}
-    sct_img = sct.grab(box)
+    with mss(display=os.getenv("DISPLAY")) as sct:
+        sct_img = sct.grab(box)
 
     img = Image.frombytes("RGB", sct_img.size, sct_img.rgb)
     assert img.mode == "RGB"
     assert img.size == sct_img.size
 
     for x, y in itertools.product(range(width), range(height)):
         assert img.getpixel((x, y)) == sct_img.pixel(x, y)
 
     img.save("box.png")
     assert os.path.isfile("box.png")
 
 
 @pytest.mark.skipif(Image is None, reason="PIL module not available.")
-def test_pil_bgra(sct):
+def test_pil_bgra():
     width, height = 16, 16
     box = {"top": 0, "left": 0, "width": width, "height": height}
-    sct_img = sct.grab(box)
+    with mss(display=os.getenv("DISPLAY")) as sct:
+        sct_img = sct.grab(box)
 
     img = Image.frombytes("RGB", sct_img.size, sct_img.bgra, "raw", "BGRX")
     assert img.mode == "RGB"
     assert img.size == sct_img.size
 
     for x, y in itertools.product(range(width), range(height)):
         assert img.getpixel((x, y)) == sct_img.pixel(x, y)
 
     img.save("box-bgra.png")
     assert os.path.isfile("box-bgra.png")
 
 
 @pytest.mark.skipif(Image is None, reason="PIL module not available.")
-def test_pil_not_16_rounded(sct):
+def test_pil_not_16_rounded():
     width, height = 10, 10
     box = {"top": 0, "left": 0, "width": width, "height": height}
-    sct_img = sct.grab(box)
+    with mss(display=os.getenv("DISPLAY")) as sct:
+        sct_img = sct.grab(box)
 
     img = Image.frombytes("RGB", sct_img.size, sct_img.rgb)
     assert img.mode == "RGB"
     assert img.size == sct_img.size
 
     for x, y in itertools.product(range(width), range(height)):
         assert img.getpixel((x, y)) == sct_img.pixel(x, y)
```

### Comparing `mss-7.0.1/mss/tests/test_tools.py` & `mss-8.0.0/mss/tests/test_tools.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,35 +4,35 @@
 """
 import hashlib
 import os.path
 import zlib
 
 import pytest
 
+from mss import mss
 from mss.tools import to_png
 
 WIDTH = 10
 HEIGHT = 10
 MD5SUM = "055e615b74167c9bdfea16a00539450c"
 
 
-def test_bad_compression_level(sct):
-    sct.compression_level = 42
-    try:
+def test_bad_compression_level():
+    with mss(compression_level=42, display=os.getenv("DISPLAY")) as sct:
         with pytest.raises(zlib.error):
             sct.shot()
-    finally:
-        sct.compression_level = 6
 
 
-def test_compression_level(sct):
+def test_compression_level():
     data = b"rgb" * WIDTH * HEIGHT
     output = f"{WIDTH}x{HEIGHT}.png"
 
-    to_png(data, (WIDTH, HEIGHT), level=sct.compression_level, output=output)
+    with mss(display=os.getenv("DISPLAY")) as sct:
+        to_png(data, (WIDTH, HEIGHT), level=sct.compression_level, output=output)
+
     with open(output, "rb") as png:
         assert hashlib.md5(png.read()).hexdigest() == MD5SUM
 
 
 @pytest.mark.parametrize(
     "level, checksum",
     [
```

### Comparing `mss-7.0.1/mss/tests/test_windows.py` & `mss-8.0.0/mss/tests/test_windows.py`

 * *Files identical despite different names*

### Comparing `mss-7.0.1/mss/tools.py` & `mss-8.0.0/mss/tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 
 import os
 import struct
 import zlib
 from typing import Optional, Tuple
 
 
-def to_png(
-    data: bytes, size: Tuple[int, int], level: int = 6, output: Optional[str] = None
-) -> Optional[bytes]:
+def to_png(data: bytes, size: Tuple[int, int], /, *, level: int = 6, output: Optional[str] = None) -> Optional[bytes]:
     """
     Dump data to a PNG file.  If `output` is `None`, create no file but return
     the whole PNG data.
 
     :param bytes data: RGBRGB...RGB data.
     :param tuple size: The (width, height) pair.
     :param int level: PNG compression level.
@@ -25,17 +23,15 @@
 
     pack = struct.pack
     crc32 = zlib.crc32
 
     width, height = size
     line = width * 3
     png_filter = pack(">B", 0)
-    scanlines = b"".join(
-        [png_filter + data[y * line : y * line + line] for y in range(height)]
-    )
+    scanlines = b"".join([png_filter + data[y * line : y * line + line] for y in range(height)])
 
     magic = pack(">8B", 137, 80, 78, 71, 13, 10, 26, 10)
 
     # Header: size, marker, data, CRC32
     ihdr = [b"", b"IHDR", b"", b""]
     ihdr[2] = pack(">2I5B", width, height, 8, 2, 0, 0, 0)
     ihdr[3] = pack(">I", crc32(b"".join(ihdr[1:3])) & 0xFFFFFFFF)
```

### Comparing `mss-7.0.1/mss/windows.py` & `mss-8.0.0/mss/windows.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     LONG,
     LPARAM,
     LPRECT,
     RECT,
     UINT,
     WORD,
 )
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 from .base import MSSBase
 from .exception import ScreenShotError
 from .models import CFunctions, Monitor
 from .screenshot import ScreenShot
 
 __all__ = ("MSS",)
@@ -77,19 +77,15 @@
 CFUNCTIONS: CFunctions = {
     "BitBlt": ("gdi32", [HDC, INT, INT, INT, INT, HDC, INT, INT, DWORD], BOOL),
     "CreateCompatibleBitmap": ("gdi32", [HDC, INT, INT], HBITMAP),
     "CreateCompatibleDC": ("gdi32", [HDC], HDC),
     "DeleteObject": ("gdi32", [HGDIOBJ], INT),
     "EnumDisplayMonitors": ("user32", [HDC, c_void_p, MONITORNUMPROC, LPARAM], BOOL),
     "GetDeviceCaps": ("gdi32", [HWND, INT], INT),
-    "GetDIBits": (
-        "gdi32",
-        [HDC, HBITMAP, UINT, UINT, c_void_p, POINTER(BITMAPINFO), UINT],
-        BOOL,
-    ),
+    "GetDIBits": ("gdi32", [HDC, HBITMAP, UINT, UINT, c_void_p, POINTER(BITMAPINFO), UINT], BOOL),
     "GetSystemMetrics": ("user32", [INT], INT),
     "GetWindowDC": ("user32", [HWND], HDC),
     "SelectObject": ("gdi32", [HDC, HGDIOBJ], HGDIOBJ),
 }
 
 
 class MSS(MSSBase):
@@ -100,18 +96,18 @@
     # Class attributes instanced one time to prevent resource leaks.
     bmp = None
     memdc = None
 
     # A dict to maintain *srcdc* values created by multiple threads.
     _srcdc_dict: Dict[threading.Thread, int] = {}
 
-    def __init__(self, **_: Any) -> None:
+    def __init__(self, /, **kwargs: Any) -> None:
         """Windows initialisations."""
 
-        super().__init__()
+        super().__init__(**kwargs)
 
         self.user32 = ctypes.WinDLL("user32")
         self.gdi32 = ctypes.WinDLL("gdi32")
         self._set_cfunctions()
         self._set_dpi_awareness()
 
         self._bbox = {"height": 0, "width": 0}
@@ -135,20 +131,15 @@
 
         cfactory = self._cfactory
         attrs = {
             "gdi32": self.gdi32,
             "user32": self.user32,
         }
         for func, (attr, argtypes, restype) in CFUNCTIONS.items():
-            cfactory(
-                attr=attrs[attr],
-                func=func,
-                argtypes=argtypes,
-                restype=restype,
-            )
+            cfactory(attrs[attr], func, argtypes, restype)
 
     def _set_dpi_awareness(self) -> None:
         """Set DPI awareness to capture full screen on Hi-DPI monitors."""
 
         version = sys.getwindowsversion()[:2]  # pylint: disable=no-member
         if version >= (6, 3):
             # Windows 8.1+
@@ -166,17 +157,15 @@
         Retrieve a thread-safe HDC from GetWindowDC().
         In multithreading, if the thread that creates *srcdc* is dead, *srcdc* will
         no longer be valid to grab the screen. The *srcdc* attribute is replaced
         with *_srcdc_dict* to maintain the *srcdc* values in multithreading.
         Since the current thread and main thread are always alive, reuse their *srcdc* value first.
         """
         cur_thread, main_thread = threading.current_thread(), threading.main_thread()
-        current_srcdc = MSS._srcdc_dict.get(cur_thread) or MSS._srcdc_dict.get(
-            main_thread
-        )
+        current_srcdc = MSS._srcdc_dict.get(cur_thread) or MSS._srcdc_dict.get(main_thread)
         if current_srcdc:
             srcdc = current_srcdc
         else:
             srcdc = self.user32.GetWindowDC(0)
             MSS._srcdc_dict[cur_thread] = srcdc
         return srcdc
 
@@ -215,15 +204,15 @@
                 }
             )
             return 1
 
         callback = MONITORNUMPROC(_callback)
         user32.EnumDisplayMonitors(0, 0, callback, 0)
 
-    def _grab_impl(self, monitor: Monitor) -> ScreenShot:
+    def _grab_impl(self, monitor: Monitor, /) -> ScreenShot:
         """
         Retrieve all pixels from a monitor. Pixels have to be RGB.
 
         In the code, there are a few interesting things:
 
         [1] bmi.bmiHeader.biHeight = -height
 
@@ -271,14 +260,16 @@
             width,
             height,
             srcdc,
             monitor["left"],
             monitor["top"],
             SRCCOPY | CAPTUREBLT,
         )
-        bits = self.gdi32.GetDIBits(
-            memdc, MSS.bmp, 0, height, self._data, self._bmi, DIB_RGB_COLORS
-        )
+        bits = self.gdi32.GetDIBits(memdc, MSS.bmp, 0, height, self._data, self._bmi, DIB_RGB_COLORS)
         if bits != height:
             raise ScreenShotError("gdi32.GetDIBits() failed.")
 
         return self.cls_image(bytearray(self._data), monitor)
+
+    def _cursor_impl(self) -> Optional[ScreenShot]:
+        """Retrieve all cursor data. Pixels have to be RGB."""
+        return None
```

### Comparing `mss-7.0.1/mss.egg-info/PKG-INFO` & `mss-8.0.0/mss.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 Metadata-Version: 2.1
 Name: mss
-Version: 7.0.1
+Version: 8.0.0
 Summary: An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 Home-page: https://github.com/BoboTiG/python-mss
 Author: Mickaël 'Tiger-222' Schoentgen
 Author-email: contact@tiger-222.fr
 License: MIT
 Project-URL: Documentation, https://python-mss.readthedocs.io
 Project-URL: Source, https://github.com/BoboTiG/python-mss
 Project-URL: Tracker, https://github.com/BoboTiG/python-mss/issues
 Keywords: screen,screenshot,screencapture,screengrab
 Platform: Darwin
 Platform: Linux
 Platform: Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics :: Capture :: Screen Capture
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Python MSS
 ==========
 
-.. image:: https://travis-ci.org/BoboTiG/python-mss.svg?branch=master
-    :target: https://travis-ci.org/BoboTiG/python-mss
-.. image:: https://ci.appveyor.com/api/projects/status/72dik18r6b746mb0?svg=true
-    :target: https://ci.appveyor.com/project/BoboTiG/python-mss
-.. image:: https://img.shields.io/badge/say-thanks-ff69b4.svg
-    :target: https://saythanks.io/to/BoboTiG
-.. image:: https://pepy.tech/badge/mss
-    :target: https://pepy.tech/project/mss
-.. image:: https://anaconda.org/conda-forge/python-mss/badges/installer/conda.svg
+.. image:: https://badge.fury.io/py/mss.svg
+    :target: https://pypi.org/project/mss/
+.. image:: https://anaconda.org/conda-forge/python-mss/badges/version.svg
     :target: https://anaconda.org/conda-forge/python-mss
+.. image:: https://github.com/BoboTiG/python-mss/actions/workflows/tests.yml/badge.svg?branch=master
+    :target: https://github.com/BoboTiG/python-mss/actions/workflows/tests.yml
+.. image:: https://static.pepy.tech/personalized-badge/mss?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads
+    :target: https://pepy.tech/project/mss
 
 
 .. code-block:: python
 
     from mss import mss
 
     # The simplest use, save a screen shot of the 1st monitor
     with mss() as sct:
         sct.shot()
 
 
 An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 
-- **Python 3.5+** and PEP8 compliant, no dependency, thread-safe;
+- **Python 3.8+** and PEP8 compliant, no dependency, thread-safe;
 - very basic, it will grab one screen shot by monitor or a screen shot of all monitors and save it to a PNG file;
 - but you can use PIL and benefit from all its formats (or add yours directly);
 - integrate well with Numpy and OpenCV;
 - it could be easily embedded into games and other software which require fast and platform optimized methods to grab screen shots (like AI, Computer Vision);
 - get the `source code on GitHub <https://github.com/BoboTiG/python-mss>`_;
 - learn with a `bunch of examples <https://python-mss.readthedocs.io/examples.html>`_;
 - you can `report a bug <https://github.com/BoboTiG/python-mss/issues>`_;
@@ -79,12 +77,13 @@
 Or you can install it with conda::
 
     conda install -c conda-forge python-mss
 
 Maintenance
 -----------
 
-For the maintainers, here are commands to upload a new release:
+For the maintainers, here are commands to upload a new release::
 
+    rm -rf build dist
     python -m build --sdist --wheel
     twine check dist/*
     twine upload dist/*
```

### Comparing `mss-7.0.1/mss.egg-info/SOURCES.txt` & `mss-8.0.0/mss.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 mss/tests/conftest.py
 mss/tests/test_bgra_to_rgb.py
 mss/tests/test_cls_image.py
 mss/tests/test_find_monitors.py
 mss/tests/test_get_pixels.py
 mss/tests/test_gnu_linux.py
 mss/tests/test_implementation.py
+mss/tests/test_issue_220.py
 mss/tests/test_leaks.py
 mss/tests/test_macos.py
 mss/tests/test_save.py
 mss/tests/test_setup.py
 mss/tests/test_third_party.py
 mss/tests/test_tools.py
 mss/tests/test_windows.py
```

### Comparing `mss-7.0.1/setup.cfg` & `mss-8.0.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mss
-version = 7.0.1
+version = 8.0.0
 author = Mickaël 'Tiger-222' Schoentgen
 author_email = contact@tiger-222.fr
 description = An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/BoboTiG/python-mss
 home_page = https://pypi.org/project/mss/
@@ -16,57 +16,62 @@
 license = MIT
 license_files = 
 	LICENSE
 platforms = Darwin, Linux, Windows
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	License :: OSI Approved :: MIT License
+	Programming Language :: Python :: Implementation :: CPython
+	Programming Language :: Python :: Implementation :: PyPy
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Multimedia :: Graphics :: Capture :: Screen Capture
 	Topic :: Software Development :: Libraries
 
 [options]
 zip_safe = False
 include_package_data = True
 packages_dir = mss
 packages = find:
-python_requires = >=3.5
+python_requires = >=3.8
 
 [options.entry_points]
 console_scripts = 
 	mss = mss.__main__:main
 
+[coverage:run]
+omit = 
+	mss/tests/*
+
 [flake8]
 ignore = 
 	E203
 	W503
 max-line-length = 120
 
 [isort]
 multi_line_output = 3
 include_trailing_comma = True
 force_grid_wrap = 0
 use_parentheses = True
-line_length = 88
+line_length = 120
 
 [tool:pytest]
 addopts = 
 	--showlocals
 	--strict-markers
-	--failed-first
 	-r fE
 	-v
+	--cov=mss
+	--cov-report=term-missing
 	--force-flaky
 	--no-success-flaky-report
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

