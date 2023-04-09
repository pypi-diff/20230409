# Comparing `tmp/earthquakepy-0.3.10.tar.gz` & `tmp/earthquakepy-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthquakepy-0.3.10.tar", last modified: Sun Apr  9 18:31:56 2023, max compression
+gzip compressed data, was "earthquakepy-0.3.8.tar", last modified: Fri Apr  7 10:02:24 2023, max compression
```

## Comparing `earthquakepy-0.3.10.tar` & `earthquakepy-0.3.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:31:56.028988 earthquakepy-0.3.10/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-09 18:31:47.000000 earthquakepy-0.3.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-09 18:31:56.028988 earthquakepy-0.3.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-09 18:31:47.000000 earthquakepy-0.3.10/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:31:56.028988 earthquakepy-0.3.10/earthquakepy/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-09 18:31:47.000000 earthquakepy-0.3.10/earthquakepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-04-09 18:31:47.000000 earthquakepy-0.3.10/earthquakepy/ims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-04-09 18:31:47.000000 earthquakepy-0.3.10/earthquakepy/multidof.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-09 18:31:47.000000 earthquakepy-0.3.10/earthquakepy/opensees_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-09 18:31:47.000000 earthquakepy-0.3.10/earthquakepy/opensees_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-09 18:31:47.000000 earthquakepy-0.3.10/earthquakepy/responseMdof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-09 18:31:47.000000 earthquakepy-0.3.10/earthquakepy/responseSdof.py
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-09 18:31:47.000000 earthquakepy-0.3.10/earthquakepy/singledof.py
--rw-r--r--   0 runner    (1001) docker     (123)    20974 2023-04-09 18:31:47.000000 earthquakepy-0.3.10/earthquakepy/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-04-09 18:31:47.000000 earthquakepy-0.3.10/earthquakepy/tsReaders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:31:56.028988 earthquakepy-0.3.10/earthquakepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-09 18:31:56.000000 earthquakepy-0.3.10/earthquakepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-09 18:31:56.000000 earthquakepy-0.3.10/earthquakepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 18:31:56.000000 earthquakepy-0.3.10/earthquakepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-09 18:31:56.000000 earthquakepy-0.3.10/earthquakepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-09 18:31:56.000000 earthquakepy-0.3.10/earthquakepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 18:31:56.028988 earthquakepy-0.3.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-09 18:31:47.000000 earthquakepy-0.3.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:02:24.295559 earthquakepy-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-07 10:02:15.000000 earthquakepy-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-07 10:02:24.295559 earthquakepy-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-07 10:02:15.000000 earthquakepy-0.3.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:02:24.295559 earthquakepy-0.3.8/earthquakepy/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-07 10:02:15.000000 earthquakepy-0.3.8/earthquakepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-04-07 10:02:15.000000 earthquakepy-0.3.8/earthquakepy/ims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-04-07 10:02:15.000000 earthquakepy-0.3.8/earthquakepy/multidof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-07 10:02:15.000000 earthquakepy-0.3.8/earthquakepy/opensees_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-07 10:02:15.000000 earthquakepy-0.3.8/earthquakepy/opensees_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-07 10:02:15.000000 earthquakepy-0.3.8/earthquakepy/responseMdof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-07 10:02:15.000000 earthquakepy-0.3.8/earthquakepy/responseSdof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-07 10:02:15.000000 earthquakepy-0.3.8/earthquakepy/singledof.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20957 2023-04-07 10:02:15.000000 earthquakepy-0.3.8/earthquakepy/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-04-07 10:02:15.000000 earthquakepy-0.3.8/earthquakepy/tsReaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:02:24.295559 earthquakepy-0.3.8/earthquakepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-07 10:02:24.000000 earthquakepy-0.3.8/earthquakepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-07 10:02:24.000000 earthquakepy-0.3.8/earthquakepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 10:02:24.000000 earthquakepy-0.3.8/earthquakepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 10:02:24.000000 earthquakepy-0.3.8/earthquakepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-07 10:02:24.000000 earthquakepy-0.3.8/earthquakepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 10:02:24.295559 earthquakepy-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-07 10:02:15.000000 earthquakepy-0.3.8/setup.py
```

### Comparing `earthquakepy-0.3.10/LICENSE` & `earthquakepy-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `earthquakepy-0.3.10/PKG-INFO` & `earthquakepy-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthquakepy
-Version: 0.3.10
+Version: 0.3.8
 Summary: python library for earthquake engineers.
 Home-page: https://github.com/gauthamrdy/earthquakepy
 Author: Gautham Reddy, Digvijay Patankar
 Author-email: pgrddy@gmail.com, dbpatankar@gmail.com
 License: GNU GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `earthquakepy-0.3.10/earthquakepy/ims.py` & `earthquakepy-0.3.8/earthquakepy/ims.py`

 * *Files identical despite different names*

### Comparing `earthquakepy-0.3.10/earthquakepy/multidof.py` & `earthquakepy-0.3.8/earthquakepy/multidof.py`

 * *Files identical despite different names*

### Comparing `earthquakepy-0.3.10/earthquakepy/opensees_classes.py` & `earthquakepy-0.3.8/earthquakepy/opensees_classes.py`

 * *Files identical despite different names*

### Comparing `earthquakepy-0.3.10/earthquakepy/opensees_helper.py` & `earthquakepy-0.3.8/earthquakepy/opensees_helper.py`

 * *Files identical despite different names*

### Comparing `earthquakepy-0.3.10/earthquakepy/responseSdof.py` & `earthquakepy-0.3.8/earthquakepy/responseSdof.py`

 * *Files identical despite different names*

### Comparing `earthquakepy-0.3.10/earthquakepy/singledof.py` & `earthquakepy-0.3.8/earthquakepy/singledof.py`

 * *Files identical despite different names*

### Comparing `earthquakepy-0.3.10/earthquakepy/timeseries.py` & `earthquakepy-0.3.8/earthquakepy/timeseries.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Define various classes to store timeseries and similar objects."""
 import numpy as np
 from scipy.integrate import trapz, cumtrapz
 import matplotlib.pyplot as plt
 # import matplotlib as mpl
-from earthquakepy.singledof import Sdof  # , SdofNL
+from .singledof import Sdof  # , SdofNL
 from scipy.fftpack import fft, fftfreq
 
 np.set_printoptions(threshold=50)
 
 
 class TimeSeries:
     """
@@ -21,15 +21,15 @@
         Define TimeSeries object.
 
         Parameters
         ----------
         t: (scalar or 1D array) time step (if scalar) or time axis (if 1D array)
         y: (1D array) ordinates
         """
-        if type(t) in [int, float, np.int_, np.float_]:
+        if (type(t) == float) or (type(t) == int):
             t = np.arange(t, len(y) * t + 0.1 * t, t)
         self.t = t
         self.y = y
         self.npts = len(self.t)
         self.dt = self.t[1] - self.t[0]
         self.component = " "
         self.duration = self.t[-1]
```

### Comparing `earthquakepy-0.3.10/earthquakepy/tsReaders.py` & `earthquakepy-0.3.8/earthquakepy/tsReaders.py`

 * *Files identical despite different names*

### Comparing `earthquakepy-0.3.10/earthquakepy.egg-info/PKG-INFO` & `earthquakepy-0.3.8/earthquakepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthquakepy
-Version: 0.3.10
+Version: 0.3.8
 Summary: python library for earthquake engineers.
 Home-page: https://github.com/gauthamrdy/earthquakepy
 Author: Gautham Reddy, Digvijay Patankar
 Author-email: pgrddy@gmail.com, dbpatankar@gmail.com
 License: GNU GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `earthquakepy-0.3.10/setup.py` & `earthquakepy-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 
 setup(
     name="earthquakepy",
-    version="0.3.10",
+    version="0.3.8",
     description="python library for earthquake engineers.",
     long_description = (this_directory / "README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/gauthamrdy/earthquakepy",
     author="Gautham Reddy, Digvijay Patankar",
     author_email="pgrddy@gmail.com, dbpatankar@gmail.com",
     license="GNU GPLv3",
```

