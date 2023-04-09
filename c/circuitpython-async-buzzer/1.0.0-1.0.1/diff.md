# Comparing `tmp/circuitpython-async-buzzer-1.0.0.tar.gz` & `tmp/circuitpython-async-buzzer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-async-buzzer-1.0.0.tar", last modified: Sun Apr  9 13:04:41 2023, max compression
+gzip compressed data, was "circuitpython-async-buzzer-1.0.1.tar", last modified: Sun Apr  9 13:10:44 2023, max compression
```

## Comparing `circuitpython-async-buzzer-1.0.0.tar` & `circuitpython-async-buzzer-1.0.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:04:41.699340 circuitpython-async-buzzer-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:04:41.691340 circuitpython-async-buzzer-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:04:41.695340 circuitpython-async-buzzer-1.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:04:41.695340 circuitpython-async-buzzer-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:04:41.695340 circuitpython-async-buzzer-1.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-09 13:04:41.695340 circuitpython-async-buzzer-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-09 13:04:34.000000 circuitpython-async-buzzer-1.0.0/async_buzzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:04:41.695340 circuitpython-async-buzzer-1.0.0/circuitpython_async_buzzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-09 13:04:41.000000 circuitpython-async-buzzer-1.0.0/circuitpython_async_buzzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-09 13:04:41.000000 circuitpython-async-buzzer-1.0.0/circuitpython_async_buzzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 13:04:41.000000 circuitpython-async-buzzer-1.0.0/circuitpython_async_buzzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-09 13:04:41.000000 circuitpython-async-buzzer-1.0.0/circuitpython_async_buzzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-09 13:04:41.000000 circuitpython-async-buzzer-1.0.0/circuitpython_async_buzzer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:04:41.695340 circuitpython-async-buzzer-1.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:04:41.695340 circuitpython-async-buzzer-1.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:04:41.695340 circuitpython-async-buzzer-1.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-09 13:04:34.000000 circuitpython-async-buzzer-1.0.0/examples/async_buzzer_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-09 13:04:34.000000 circuitpython-async-buzzer-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-09 13:04:23.000000 circuitpython-async-buzzer-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 13:04:41.699340 circuitpython-async-buzzer-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:10:43.998399 circuitpython-async-buzzer-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:10:43.994399 circuitpython-async-buzzer-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:10:43.994399 circuitpython-async-buzzer-1.0.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:10:43.998399 circuitpython-async-buzzer-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:10:43.998399 circuitpython-async-buzzer-1.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-04-09 13:10:43.998399 circuitpython-async-buzzer-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-09 13:10:35.000000 circuitpython-async-buzzer-1.0.1/async_buzzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:10:43.998399 circuitpython-async-buzzer-1.0.1/circuitpython_async_buzzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-04-09 13:10:43.000000 circuitpython-async-buzzer-1.0.1/circuitpython_async_buzzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-09 13:10:43.000000 circuitpython-async-buzzer-1.0.1/circuitpython_async_buzzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 13:10:43.000000 circuitpython-async-buzzer-1.0.1/circuitpython_async_buzzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-09 13:10:43.000000 circuitpython-async-buzzer-1.0.1/circuitpython_async_buzzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-09 13:10:43.000000 circuitpython-async-buzzer-1.0.1/circuitpython_async_buzzer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:10:43.998399 circuitpython-async-buzzer-1.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:10:43.998399 circuitpython-async-buzzer-1.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:10:43.998399 circuitpython-async-buzzer-1.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-09 13:10:35.000000 circuitpython-async-buzzer-1.0.1/examples/async_buzzer_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-09 13:10:35.000000 circuitpython-async-buzzer-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-09 13:10:27.000000 circuitpython-async-buzzer-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 13:10:43.998399 circuitpython-async-buzzer-1.0.1/setup.cfg
```

### Comparing `circuitpython-async-buzzer-1.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-async-buzzer-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-async-buzzer-1.0.0/.github/workflows/release_gh.yml` & `circuitpython-async-buzzer-1.0.1/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-async-buzzer-1.0.0/.gitignore` & `circuitpython-async-buzzer-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-async-buzzer-1.0.0/.pre-commit-config.yaml` & `circuitpython-async-buzzer-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-async-buzzer-1.0.0/.pylintrc` & `circuitpython-async-buzzer-1.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-async-buzzer-1.0.0/CODE_OF_CONDUCT.md` & `circuitpython-async-buzzer-1.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-async-buzzer-1.0.0/LICENSE` & `circuitpython-async-buzzer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-async-buzzer-1.0.0/LICENSES/CC-BY-4.0.txt` & `circuitpython-async-buzzer-1.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-async-buzzer-1.0.0/LICENSES/MIT.txt` & `circuitpython-async-buzzer-1.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-async-buzzer-1.0.0/LICENSES/Unlicense.txt` & `circuitpython-async-buzzer-1.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-async-buzzer-1.0.0/PKG-INFO` & `circuitpython-async-buzzer-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-async-buzzer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Play simple tunes on a piezo buzzer asynchronously
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_async_buzzer
 Keywords: adafruit,blinka,circuitpython,micropython,async_buzzer,asyncio,buzzer,piezo,music,tune,alert,async,asynchronous
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -44,14 +44,15 @@
 
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
+* `CircuitPython asyncio module <https://github.com/adafruit/Adafruit_CircuitPython_asyncio>`_
 
 Installing from PyPI
 =====================
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/circuitpython-async-buzzer/>`_.
 To install for current user:
```

### Comparing `circuitpython-async-buzzer-1.0.0/README.rst` & `circuitpython-async-buzzer-1.0.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
+* `CircuitPython asyncio module <https://github.com/adafruit/Adafruit_CircuitPython_asyncio>`_
 
 Installing from PyPI
 =====================
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/circuitpython-async-buzzer/>`_.
 To install for current user:
```

### Comparing `circuitpython-async-buzzer-1.0.0/async_buzzer.py` & `circuitpython-async-buzzer-1.0.1/async_buzzer.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,26 +19,29 @@
 * This works with passive piezo transducers.
 
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 
+* CircuitPython asyncio module:
+  https://github.com/adafruit/Adafruit_CircuitPython_asyncio
+
 """
 try:
     from typing import Optional, Union, Tuple, Sequence, List
     import pwmio
 except ImportError:
     pass
 
 import asyncio
 from collections import namedtuple
 
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __repo__ = "https://github.com/furbrain/CircuitPython_async_buzzer.git"
 
 
 Note = namedtuple("Note", ("freq", "duration"))
 
 
 class Buzzer:
```

### Comparing `circuitpython-async-buzzer-1.0.0/circuitpython_async_buzzer.egg-info/PKG-INFO` & `circuitpython-async-buzzer-1.0.1/circuitpython_async_buzzer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-async-buzzer
-Version: 1.0.0
+Version: 1.0.1
 Summary: Play simple tunes on a piezo buzzer asynchronously
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/furbrain/CircuitPython_async_buzzer
 Keywords: adafruit,blinka,circuitpython,micropython,async_buzzer,asyncio,buzzer,piezo,music,tune,alert,async,asynchronous
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -44,14 +44,15 @@
 
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
+* `CircuitPython asyncio module <https://github.com/adafruit/Adafruit_CircuitPython_asyncio>`_
 
 Installing from PyPI
 =====================
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/circuitpython-async-buzzer/>`_.
 To install for current user:
```

### Comparing `circuitpython-async-buzzer-1.0.0/circuitpython_async_buzzer.egg-info/SOURCES.txt` & `circuitpython-async-buzzer-1.0.1/circuitpython_async_buzzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-async-buzzer-1.0.0/docs/_static/favicon.ico` & `circuitpython-async-buzzer-1.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-async-buzzer-1.0.0/docs/conf.py` & `circuitpython-async-buzzer-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-async-buzzer-1.0.0/docs/index.rst` & `circuitpython-async-buzzer-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-async-buzzer-1.0.0/examples/async_buzzer_simpletest.py` & `circuitpython-async-buzzer-1.0.1/examples/async_buzzer_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-async-buzzer-1.0.0/pyproject.toml` & `circuitpython-async-buzzer-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-async-buzzer"
 description = "Play simple tunes on a piezo buzzer asynchronously"
-version = "1.0.0"
+version = "1.0.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/furbrain/CircuitPython_async_buzzer"}
 keywords = [
     "adafruit",
```

