# Comparing `tmp/myplotlib-1.0.3.tar.gz` & `tmp/myplotlib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myplotlib-1.0.3.tar", last modified: Fri Mar 10 19:22:11 2023, max compression
+gzip compressed data, was "myplotlib-1.1.0.tar", last modified: Sun Apr  9 21:28:29 2023, max compression
```

## Comparing `myplotlib-1.0.3.tar` & `myplotlib-1.1.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 hakobyan (1051207734) 1832971548        0 2023-03-10 19:22:11.624892 myplotlib-1.0.3/
--rw-r--r--   0 hakobyan (1051207734) 1832971548     1500 2023-03-10 19:09:07.000000 myplotlib-1.0.3/LICENSE
--rw-r--r--   0 hakobyan (1051207734) 1832971548       76 2023-03-10 19:09:07.000000 myplotlib-1.0.3/MANIFEST.in
--rw-r--r--   0 hakobyan (1051207734) 1832971548     1910 2023-03-10 19:22:11.625025 myplotlib-1.0.3/PKG-INFO
--rw-r--r--   0 hakobyan (1051207734) 1832971548     1542 2023-03-10 19:19:08.000000 myplotlib-1.0.3/README.md
-drwxr-xr-x   0 hakobyan (1051207734) 1832971548        0 2023-03-10 19:22:11.603144 myplotlib-1.0.3/myplotlib/
--rw-r--r--   0 hakobyan (1051207734) 1832971548     2441 2023-03-10 19:19:35.000000 myplotlib-1.0.3/myplotlib/__init__.py
-drwxr-xr-x   0 hakobyan (1051207734) 1832971548        0 2023-03-10 19:22:11.607789 myplotlib-1.0.3/myplotlib/assets/
-drwxr-xr-x   0 hakobyan (1051207734) 1832971548        0 2023-03-10 19:22:11.610486 myplotlib-1.0.3/myplotlib/assets/colormaps/
--rw-r--r--   0 hakobyan (1051207734) 1832971548    76725 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/colormaps/bipolar.csv
--rw-r--r--   0 hakobyan (1051207734) 1832971548     6679 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/colormaps/fire.csv
--rw-r--r--   0 hakobyan (1051207734) 1832971548     9996 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/colormaps/idl.csv
--rw-r--r--   0 hakobyan (1051207734) 1832971548    38400 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/colormaps/sunrise.csv
--rw-r--r--   0 hakobyan (1051207734) 1832971548    38400 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/colormaps/thermal.csv
--rw-r--r--   0 hakobyan (1051207734) 1832971548    38400 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/colormaps/vanilla.csv
--rw-r--r--   0 hakobyan (1051207734) 1832971548      682 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/fancy.dark.mplstyle
--rw-r--r--   0 hakobyan (1051207734) 1832971548      491 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/fancy.light.mplstyle
-drwxr-xr-x   0 hakobyan (1051207734) 1832971548        0 2023-03-10 19:22:11.623785 myplotlib-1.0.3/myplotlib/assets/fonts/
--rwxr-xr-x   0 hakobyan (1051207734) 1832971548   244278 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/fonts/AppleChancery.ttf
--rw-r--r--   0 hakobyan (1051207734) 1832971548   601316 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/fonts/EBGaramond-Bold.ttf
--rw-r--r--   0 hakobyan (1051207734) 1832971548   567300 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/fonts/EBGaramond-BoldItalic.ttf
--rw-r--r--   0 hakobyan (1051207734) 1832971548   600940 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/fonts/EBGaramond-ExtraBold.ttf
--rw-r--r--   0 hakobyan (1051207734) 1832971548   566936 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/fonts/EBGaramond-ExtraBoldItalic.ttf
--rw-r--r--   0 hakobyan (1051207734) 1832971548   564280 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/fonts/EBGaramond-Italic.ttf
--rw-r--r--   0 hakobyan (1051207734) 1832971548   601412 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/fonts/EBGaramond-Medium.ttf
--rw-r--r--   0 hakobyan (1051207734) 1832971548   566872 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/fonts/EBGaramond-MediumItalic.ttf
--rw-r--r--   0 hakobyan (1051207734) 1832971548   599076 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/fonts/EBGaramond-Regular.ttf
--rw-r--r--   0 hakobyan (1051207734) 1832971548   601652 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/fonts/EBGaramond-SemiBold.ttf
--rw-r--r--   0 hakobyan (1051207734) 1832971548   567528 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/fonts/EBGaramond-SemiBoldItalic.ttf
--rwxr-xr-x   0 hakobyan (1051207734) 1832971548    44328 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/fonts/HersheyTex-Book.otf
--rwxr-xr-x   0 hakobyan (1051207734) 1832971548    31664 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/fonts/HersheyTex-Light.otf
--rw-r--r--   0 hakobyan (1051207734) 1832971548      663 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/hershey.dark.mplstyle
--rw-r--r--   0 hakobyan (1051207734) 1832971548      492 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/hershey.light.mplstyle
--rw-r--r--   0 hakobyan (1051207734) 1832971548      481 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/mono.dark.mplstyle
--rw-r--r--   0 hakobyan (1051207734) 1832971548      290 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/assets/mono.light.mplstyle
--rw-r--r--   0 hakobyan (1051207734) 1832971548    12462 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/plots.py
--rw-r--r--   0 hakobyan (1051207734) 1832971548     6014 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/tests.py
-drwxr-xr-x   0 hakobyan (1051207734) 1832971548        0 2023-03-10 19:22:11.624575 myplotlib-1.0.3/myplotlib/tools/
--rw-r--r--   0 hakobyan (1051207734) 1832971548        0 2023-03-10 19:09:07.000000 myplotlib-1.0.3/myplotlib/tools/__init__.py
--rw-r--r--   0 hakobyan (1051207734) 1832971548     3080 2023-03-10 19:15:11.000000 myplotlib-1.0.3/myplotlib/tools/lic.py
-drwxr-xr-x   0 hakobyan (1051207734) 1832971548        0 2023-03-10 19:22:11.605579 myplotlib-1.0.3/myplotlib.egg-info/
--rw-r--r--   0 hakobyan (1051207734) 1832971548     1910 2023-03-10 19:22:11.000000 myplotlib-1.0.3/myplotlib.egg-info/PKG-INFO
--rw-r--r--   0 hakobyan (1051207734) 1832971548     1420 2023-03-10 19:22:11.000000 myplotlib-1.0.3/myplotlib.egg-info/SOURCES.txt
--rw-r--r--   0 hakobyan (1051207734) 1832971548        1 2023-03-10 19:22:11.000000 myplotlib-1.0.3/myplotlib.egg-info/dependency_links.txt
--rw-r--r--   0 hakobyan (1051207734) 1832971548       37 2023-03-10 19:22:11.000000 myplotlib-1.0.3/myplotlib.egg-info/requires.txt
--rw-r--r--   0 hakobyan (1051207734) 1832971548       10 2023-03-10 19:22:11.000000 myplotlib-1.0.3/myplotlib.egg-info/top_level.txt
--rw-r--r--   0 hakobyan (1051207734) 1832971548        1 2023-03-10 19:13:54.000000 myplotlib-1.0.3/myplotlib.egg-info/zip-safe
--rw-r--r--   0 hakobyan (1051207734) 1832971548       86 2023-03-10 19:09:07.000000 myplotlib-1.0.3/pyproject.toml
--rw-r--r--   0 hakobyan (1051207734) 1832971548      664 2023-03-10 19:22:11.625642 myplotlib-1.0.3/setup.cfg
+drwxr-xr-x   0 hayk      (1000) hayk      (1000)        0 2023-04-09 21:28:29.930756 myplotlib-1.1.0/
+-rw-r--r--   0 hayk      (1000) hayk      (1000)     1500 2023-03-04 21:33:25.000000 myplotlib-1.1.0/LICENSE
+-rw-r--r--   0 hayk      (1000) hayk      (1000)       76 2023-03-04 21:25:07.000000 myplotlib-1.1.0/MANIFEST.in
+-rw-r--r--   0 hayk      (1000) hayk      (1000)     1623 2023-04-09 21:28:29.930756 myplotlib-1.1.0/PKG-INFO
+-rw-r--r--   0 hayk      (1000) hayk      (1000)     1255 2023-04-09 20:55:59.000000 myplotlib-1.1.0/README.md
+drwxr-xr-x   0 hayk      (1000) hayk      (1000)        0 2023-04-09 21:28:29.920756 myplotlib-1.1.0/myplotlib/
+-rw-r--r--   0 hayk      (1000) hayk      (1000)     2441 2023-04-09 21:28:19.000000 myplotlib-1.1.0/myplotlib/__init__.py
+drwxr-xr-x   0 hayk      (1000) hayk      (1000)        0 2023-04-09 21:28:29.920756 myplotlib-1.1.0/myplotlib/assets/
+drwxr-xr-x   0 hayk      (1000) hayk      (1000)        0 2023-04-09 21:28:29.930756 myplotlib-1.1.0/myplotlib/assets/colormaps/
+-rw-r--r--   0 hayk      (1000) hayk      (1000)    76725 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/colormaps/bipolar.csv
+-rw-r--r--   0 hayk      (1000) hayk      (1000)    76800 2023-04-09 21:17:19.000000 myplotlib-1.1.0/myplotlib/assets/colormaps/colt.csv
+-rw-r--r--   0 hayk      (1000) hayk      (1000)     6679 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/colormaps/fire.csv
+-rw-r--r--   0 hayk      (1000) hayk      (1000)     9996 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/colormaps/idl.csv
+-rw-r--r--   0 hayk      (1000) hayk      (1000)    38400 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/colormaps/sunrise.csv
+-rw-r--r--   0 hayk      (1000) hayk      (1000)    38400 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/colormaps/thermal.csv
+-rw-r--r--   0 hayk      (1000) hayk      (1000)    38400 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/colormaps/vanilla.csv
+-rw-r--r--   0 hayk      (1000) hayk      (1000)      682 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/fancy.dark.mplstyle
+-rw-r--r--   0 hayk      (1000) hayk      (1000)      491 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/fancy.light.mplstyle
+drwxr-xr-x   0 hayk      (1000) hayk      (1000)        0 2023-04-09 21:28:29.930756 myplotlib-1.1.0/myplotlib/assets/fonts/
+-rwxr-xr-x   0 hayk      (1000) hayk      (1000)   244278 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/fonts/AppleChancery.ttf
+-rw-r--r--   0 hayk      (1000) hayk      (1000)   601316 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/fonts/EBGaramond-Bold.ttf
+-rw-r--r--   0 hayk      (1000) hayk      (1000)   567300 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/fonts/EBGaramond-BoldItalic.ttf
+-rw-r--r--   0 hayk      (1000) hayk      (1000)   600940 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/fonts/EBGaramond-ExtraBold.ttf
+-rw-r--r--   0 hayk      (1000) hayk      (1000)   566936 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/fonts/EBGaramond-ExtraBoldItalic.ttf
+-rw-r--r--   0 hayk      (1000) hayk      (1000)   564280 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/fonts/EBGaramond-Italic.ttf
+-rw-r--r--   0 hayk      (1000) hayk      (1000)   601412 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/fonts/EBGaramond-Medium.ttf
+-rw-r--r--   0 hayk      (1000) hayk      (1000)   566872 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/fonts/EBGaramond-MediumItalic.ttf
+-rw-r--r--   0 hayk      (1000) hayk      (1000)   599076 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/fonts/EBGaramond-Regular.ttf
+-rw-r--r--   0 hayk      (1000) hayk      (1000)   601652 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/fonts/EBGaramond-SemiBold.ttf
+-rw-r--r--   0 hayk      (1000) hayk      (1000)   567528 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/fonts/EBGaramond-SemiBoldItalic.ttf
+-rwxr-xr-x   0 hayk      (1000) hayk      (1000)    44328 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/fonts/HersheyTex-Book.otf
+-rwxr-xr-x   0 hayk      (1000) hayk      (1000)    31664 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/fonts/HersheyTex-Light.otf
+-rw-r--r--   0 hayk      (1000) hayk      (1000)      663 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/hershey.dark.mplstyle
+-rw-r--r--   0 hayk      (1000) hayk      (1000)      492 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/hershey.light.mplstyle
+-rw-r--r--   0 hayk      (1000) hayk      (1000)      481 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/mono.dark.mplstyle
+-rw-r--r--   0 hayk      (1000) hayk      (1000)      290 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/assets/mono.light.mplstyle
+-rw-r--r--   0 hayk      (1000) hayk      (1000)    12462 2023-03-04 21:30:05.000000 myplotlib-1.1.0/myplotlib/plots.py
+-rw-r--r--   0 hayk      (1000) hayk      (1000)     6012 2023-04-09 20:55:23.000000 myplotlib-1.1.0/myplotlib/tests.py
+drwxr-xr-x   0 hayk      (1000) hayk      (1000)        0 2023-04-09 21:28:29.930756 myplotlib-1.1.0/myplotlib/tools/
+-rw-r--r--   0 hayk      (1000) hayk      (1000)        0 2023-03-04 21:25:07.000000 myplotlib-1.1.0/myplotlib/tools/__init__.py
+-rw-r--r--   0 hayk      (1000) hayk      (1000)     2938 2023-04-09 21:11:56.000000 myplotlib-1.1.0/myplotlib/tools/lic.py
+drwxr-xr-x   0 hayk      (1000) hayk      (1000)        0 2023-04-09 21:28:29.920756 myplotlib-1.1.0/myplotlib.egg-info/
+-rw-r--r--   0 hayk      (1000) hayk      (1000)     1623 2023-04-09 21:28:29.000000 myplotlib-1.1.0/myplotlib.egg-info/PKG-INFO
+-rw-r--r--   0 hayk      (1000) hayk      (1000)     1456 2023-04-09 21:28:29.000000 myplotlib-1.1.0/myplotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 hayk      (1000) hayk      (1000)        1 2023-04-09 21:28:29.000000 myplotlib-1.1.0/myplotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 hayk      (1000) hayk      (1000)       54 2023-04-09 21:28:29.000000 myplotlib-1.1.0/myplotlib.egg-info/requires.txt
+-rw-r--r--   0 hayk      (1000) hayk      (1000)       10 2023-04-09 21:28:29.000000 myplotlib-1.1.0/myplotlib.egg-info/top_level.txt
+-rw-r--r--   0 hayk      (1000) hayk      (1000)        1 2023-03-04 21:34:48.000000 myplotlib-1.1.0/myplotlib.egg-info/zip-safe
+-rw-r--r--   0 hayk      (1000) hayk      (1000)       86 2023-03-04 21:25:07.000000 myplotlib-1.1.0/pyproject.toml
+-rw-r--r--   0 hayk      (1000) hayk      (1000)      682 2023-04-09 21:28:29.930756 myplotlib-1.1.0/setup.cfg
```

### Comparing `myplotlib-1.0.3/LICENSE` & `myplotlib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/PKG-INFO` & `myplotlib-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 Metadata-Version: 2.1
 Name: myplotlib
-Version: 1.0.3
+Version: 1.1.0
 Summary: `matplotlib` binder with custom styles and routines for fast plotting
 Home-page: https://github.com/haykh/myplotlib
 Author: morninbru
 Author-email: haykh.astro@gmail.com
 License: BSD 3-Clause License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # `myplotlib`
 
 `matplotlib` binder with custom styles and routines for fast plotting. see [previews of available styles](https://github.com/haykh/myplotlib/tree/master/previews#readme).
 
-> _Note_: `numba` support in line-integral-convolution algorithm has been temporarily removed due to incompatibility with `python` 3.11; see [issue](https://github.com/numba/numba/issues/8304). Because of this the line integral convolution algorithm is quite slow and not recommended for usage.
-
 ### installation
 
 ```shell
 pip install myplotlib
 ```
 
 ### usage
 
 ```python
 # initialize style:
 import myplotlib
 myplotlib.load(style=..., flavor=...)
-# style can be [`fancy` | `mono` | `hershey`]
-# flavor can be [`light` | `dark`]
-# if not specified defaults to `style = 'main', flavor = 'light'`
+# style can be [None | `fancy` | `mono` | `hershey`]
+# flavor can be [None | `light` | `dark`]
+# if not specified defaults to `style = None, flavor = None`
 
 # auxiliary functions for plotting:
 import myplotlib.plots as myplt
 # type for docstring:
 myplt?
 
 # preview custom styles with built-in functions
```

### Comparing `myplotlib-1.0.3/README.md` & `myplotlib-1.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # `myplotlib`
 
 `matplotlib` binder with custom styles and routines for fast plotting. see [previews of available styles](https://github.com/haykh/myplotlib/tree/master/previews#readme).
 
-> _Note_: `numba` support in line-integral-convolution algorithm has been temporarily removed due to incompatibility with `python` 3.11; see [issue](https://github.com/numba/numba/issues/8304). Because of this the line integral convolution algorithm is quite slow and not recommended for usage.
-
 ### installation
 
 ```shell
 pip install myplotlib
 ```
 
 ### usage
 
 ```python
 # initialize style:
 import myplotlib
 myplotlib.load(style=..., flavor=...)
-# style can be [`fancy` | `mono` | `hershey`]
-# flavor can be [`light` | `dark`]
-# if not specified defaults to `style = 'main', flavor = 'light'`
+# style can be [None | `fancy` | `mono` | `hershey`]
+# flavor can be [None | `light` | `dark`]
+# if not specified defaults to `style = None, flavor = None`
 
 # auxiliary functions for plotting:
 import myplotlib.plots as myplt
 # type for docstring:
 myplt?
 
 # preview custom styles with built-in functions
```

### Comparing `myplotlib-1.0.3/myplotlib/__init__.py` & `myplotlib-1.1.0/myplotlib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pkg_resources
 
-__version__ = "1.0.3"
+__version__ = "1.1.0"
 
 CUSTOM_CMAPS = []
 
 
 def __RGBToPyCmap(rgbdata):
     import numpy as np
```

### Comparing `myplotlib-1.0.3/myplotlib/assets/colormaps/bipolar.csv` & `myplotlib-1.1.0/myplotlib/assets/colormaps/bipolar.csv`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/assets/colormaps/fire.csv` & `myplotlib-1.1.0/myplotlib/assets/colormaps/fire.csv`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/assets/colormaps/idl.csv` & `myplotlib-1.1.0/myplotlib/assets/colormaps/idl.csv`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/assets/colormaps/sunrise.csv` & `myplotlib-1.1.0/myplotlib/assets/colormaps/sunrise.csv`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/assets/colormaps/thermal.csv` & `myplotlib-1.1.0/myplotlib/assets/colormaps/thermal.csv`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/assets/colormaps/vanilla.csv` & `myplotlib-1.1.0/myplotlib/assets/colormaps/vanilla.csv`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/assets/fancy.dark.mplstyle` & `myplotlib-1.1.0/myplotlib/assets/fancy.dark.mplstyle`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/assets/fonts/AppleChancery.ttf` & `myplotlib-1.1.0/myplotlib/assets/fonts/AppleChancery.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/assets/fonts/EBGaramond-Bold.ttf` & `myplotlib-1.1.0/myplotlib/assets/fonts/EBGaramond-Bold.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/assets/fonts/EBGaramond-BoldItalic.ttf` & `myplotlib-1.1.0/myplotlib/assets/fonts/EBGaramond-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/assets/fonts/EBGaramond-ExtraBold.ttf` & `myplotlib-1.1.0/myplotlib/assets/fonts/EBGaramond-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/assets/fonts/EBGaramond-ExtraBoldItalic.ttf` & `myplotlib-1.1.0/myplotlib/assets/fonts/EBGaramond-ExtraBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/assets/fonts/EBGaramond-Italic.ttf` & `myplotlib-1.1.0/myplotlib/assets/fonts/EBGaramond-Italic.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/assets/fonts/EBGaramond-Medium.ttf` & `myplotlib-1.1.0/myplotlib/assets/fonts/EBGaramond-Medium.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/assets/fonts/EBGaramond-MediumItalic.ttf` & `myplotlib-1.1.0/myplotlib/assets/fonts/EBGaramond-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/assets/fonts/EBGaramond-Regular.ttf` & `myplotlib-1.1.0/myplotlib/assets/fonts/EBGaramond-Regular.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/assets/fonts/EBGaramond-SemiBold.ttf` & `myplotlib-1.1.0/myplotlib/assets/fonts/EBGaramond-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/assets/fonts/EBGaramond-SemiBoldItalic.ttf` & `myplotlib-1.1.0/myplotlib/assets/fonts/EBGaramond-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/assets/fonts/HersheyTex-Book.otf` & `myplotlib-1.1.0/myplotlib/assets/fonts/HersheyTex-Book.otf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/assets/fonts/HersheyTex-Light.otf` & `myplotlib-1.1.0/myplotlib/assets/fonts/HersheyTex-Light.otf`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/assets/hershey.dark.mplstyle` & `myplotlib-1.1.0/myplotlib/assets/hershey.dark.mplstyle`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/plots.py` & `myplotlib-1.1.0/myplotlib/plots.py`

 * *Files identical despite different names*

### Comparing `myplotlib-1.0.3/myplotlib/tests.py` & `myplotlib-1.1.0/myplotlib/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         for (x, y) in vortices
         if -extra_factor < x < extra_factor and -extra_factor < y < extra_factor
     ]
     sx, sy = (1000, 1000)
     xs = np.linspace(-1, 1, sx).astype(np.float64)[None, :]
     ys = np.linspace(-1, 1, sy).astype(np.float64)[:, None]
     vectors = np.zeros((sx, sy, 2), dtype=np.float64)
-    for (x, y) in vortices:
+    for x, y in vortices:
         rsq = (xs - x) ** 2 + (ys - y) ** 2
         vectors[..., 0] += (ys - y) / rsq
         vectors[..., 1] += -(xs - x) / rsq
     myplt.plotVectorField(
         ax,
         xs,
         ys,
```

### Comparing `myplotlib-1.0.3/myplotlib/tools/lic.py` & `myplotlib-1.1.0/myplotlib/tools/lic.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,34 +2,30 @@
 # Credits to Patrick Crumley (@pcrumley)
 # https://github.com/pcrumley/tristanUtils/blob/master/src/lic_NUMBA.py
 # . . . . .
 
 # A NUMBA based implementation of the code found here:
 # https://scipy-cookbook.readthedocs.io/items/LineIntegralConvolution.html
 
-# NOTE [3-10-2023]:
-# | NUMBA support temporarily disabled due to incompatibility with python 3.11
-
 import numpy as np
-from numpy import ones
-# from numba import jit, guvectorize, float64, int32
+from numba import jit
 
 
 def generate_kernel(klen):
     kernel = np.sin(np.arange(klen) * np.pi / klen)
     return kernel.astype(np.float64)
 
 
 def generate_texture(shape, seed=None):
     if seed is not None:
         np.random.seed(seed)
     return np.random.rand(*shape).astype(np.float64)
 
 
-# @jit
+@jit(nopython=False)
 def advance(vx, vy, xyArr, fxfyArr, w, h):
     if vx >= 0:
         tx = (1 - fxfyArr[1]) / vx
     else:
         tx = -fxfyArr[1] / vx
     if vy >= 0:
         ty = (1 - fxfyArr[0]) / vy
@@ -57,15 +53,15 @@
         xyArr[1] = 0  # FIXME: other boundary conditions?
     if xyArr[0] < 0:
         xyArr[0] = 0  # FIXME: other boundary conditions?
     if xyArr[0] >= h:
         xyArr[0] = h - 1  # FIXME: other boundary conditions?
 
 
-# @jit(nopython=True)
+@jit(nopython=True)
 def line_integral_convolution(vx, vy, texture, kernel):
     h = vx.shape[0]
     w = vx.shape[1]
     kernellen = kernel.shape[0]
     if h != vy.shape[0] or w != vy.shape[1]:
         raise ValueError("Vx and Vy must the same shape")
     if h != texture.shape[0] or w != texture.shape[1]:
```

### Comparing `myplotlib-1.0.3/myplotlib.egg-info/PKG-INFO` & `myplotlib-1.1.0/myplotlib.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 Metadata-Version: 2.1
 Name: myplotlib
-Version: 1.0.3
+Version: 1.1.0
 Summary: `matplotlib` binder with custom styles and routines for fast plotting
 Home-page: https://github.com/haykh/myplotlib
 Author: morninbru
 Author-email: haykh.astro@gmail.com
 License: BSD 3-Clause License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # `myplotlib`
 
 `matplotlib` binder with custom styles and routines for fast plotting. see [previews of available styles](https://github.com/haykh/myplotlib/tree/master/previews#readme).
 
-> _Note_: `numba` support in line-integral-convolution algorithm has been temporarily removed due to incompatibility with `python` 3.11; see [issue](https://github.com/numba/numba/issues/8304). Because of this the line integral convolution algorithm is quite slow and not recommended for usage.
-
 ### installation
 
 ```shell
 pip install myplotlib
 ```
 
 ### usage
 
 ```python
 # initialize style:
 import myplotlib
 myplotlib.load(style=..., flavor=...)
-# style can be [`fancy` | `mono` | `hershey`]
-# flavor can be [`light` | `dark`]
-# if not specified defaults to `style = 'main', flavor = 'light'`
+# style can be [None | `fancy` | `mono` | `hershey`]
+# flavor can be [None | `light` | `dark`]
+# if not specified defaults to `style = None, flavor = None`
 
 # auxiliary functions for plotting:
 import myplotlib.plots as myplt
 # type for docstring:
 myplt?
 
 # preview custom styles with built-in functions
```

### Comparing `myplotlib-1.0.3/myplotlib.egg-info/SOURCES.txt` & `myplotlib-1.1.0/myplotlib.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 myplotlib/assets/fancy.dark.mplstyle
 myplotlib/assets/fancy.light.mplstyle
 myplotlib/assets/hershey.dark.mplstyle
 myplotlib/assets/hershey.light.mplstyle
 myplotlib/assets/mono.dark.mplstyle
 myplotlib/assets/mono.light.mplstyle
 myplotlib/assets/colormaps/bipolar.csv
+myplotlib/assets/colormaps/colt.csv
 myplotlib/assets/colormaps/fire.csv
 myplotlib/assets/colormaps/idl.csv
 myplotlib/assets/colormaps/sunrise.csv
 myplotlib/assets/colormaps/thermal.csv
 myplotlib/assets/colormaps/vanilla.csv
 myplotlib/assets/fonts/AppleChancery.ttf
 myplotlib/assets/fonts/EBGaramond-Bold.ttf
```

### Comparing `myplotlib-1.0.3/setup.cfg` & `myplotlib-1.1.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 zip_safe = True
 python_requires = >=3.6
 packages = find:
 include_package_data = True
 install_requires = 
 	matplotlib>=3.0.0
 	numpy
+	numba==0.57.0rc1
 
 [options.package_data]
 myplotlib = assets/colormaps/*.csv, fonts/*.ttf, *.mplstyle
 
 [options.extras_require]
 dev = 
 	black
```

