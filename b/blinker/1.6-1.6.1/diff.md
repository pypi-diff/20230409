# Comparing `tmp/blinker-1.6.tar.gz` & `tmp/blinker-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ubuntu/blinker/dist/.tmp-lozju9bg/blinker-1.6.tar", last modified: Sun Apr  2 14:03:50 2023, max compression
+gzip compressed data, was "/home/ubuntu/blinker/dist/.tmp-tx6nq4mi/blinker-1.6.1.tar", last modified: Sun Apr  9 15:26:19 2023, max compression
```

## Comparing `blinker-1.6.tar` & `blinker-1.6.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-02 14:03:50.818531 blinker-1.6/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2503 2023-04-02 13:58:17.000000 blinker-1.6/CHANGES.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1054 2023-04-02 13:58:17.000000 blinker-1.6/LICENSE.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      127 2023-04-02 13:58:17.000000 blinker-1.6/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1962 2023-04-02 14:03:50.818531 blinker-1.6/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      990 2023-04-02 13:58:17.000000 blinker-1.6/README.rst
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-02 14:03:50.738525 blinker-1.6/docs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      634 2023-04-02 13:58:17.000000 blinker-1.6/docs/Makefile
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-02 14:03:50.738525 blinker-1.6/docs/_static/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3627 2023-04-02 13:58:17.000000 blinker-1.6/docs/_static/blinker-named.png
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1195 2023-04-02 13:58:17.000000 blinker-1.6/docs/conf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9761 2023-04-02 13:58:17.000000 blinker-1.6/docs/index.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      765 2023-04-02 13:58:17.000000 blinker-1.6/docs/make.bat
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1895 2023-04-02 13:58:17.000000 blinker-1.6/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-02 14:03:50.818531 blinker-1.6/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-02 14:03:50.658519 blinker-1.6/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-02 14:03:50.738525 blinker-1.6/src/blinker/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      407 2023-04-02 13:58:17.000000 blinker-1.6/src/blinker/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9081 2023-04-02 13:58:17.000000 blinker-1.6/src/blinker/_saferef.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3997 2023-04-02 13:58:17.000000 blinker-1.6/src/blinker/_utilities.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20317 2023-04-02 13:58:17.000000 blinker-1.6/src/blinker/base.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-02 13:58:17.000000 blinker-1.6/src/blinker/py.typed
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-02 14:03:50.738525 blinker-1.6/src/blinker.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1962 2023-04-02 14:03:50.000000 blinker-1.6/src/blinker.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      535 2023-04-02 14:03:50.000000 blinker-1.6/src/blinker.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-02 14:03:50.000000 blinker-1.6/src/blinker.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       18 2023-04-02 14:03:50.000000 blinker-1.6/src/blinker.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-04-02 14:03:50.000000 blinker-1.6/src/blinker.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-02 14:03:50.818531 blinker-1.6/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-04-02 13:58:17.000000 blinker-1.6/tests/test_context.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3747 2023-04-02 13:58:17.000000 blinker-1.6/tests/test_saferef.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12962 2023-04-02 13:58:17.000000 blinker-1.6/tests/test_signals.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      451 2023-04-02 13:58:17.000000 blinker-1.6/tests/test_utilities.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      591 2023-04-02 13:58:17.000000 blinker-1.6/tox.ini
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-09 15:26:19.289915 blinker-1.6.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2752 2023-04-09 15:23:14.000000 blinker-1.6.1/CHANGES.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1054 2023-04-02 13:58:17.000000 blinker-1.6.1/LICENSE.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      127 2023-04-02 13:58:17.000000 blinker-1.6.1/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1964 2023-04-09 15:26:19.289915 blinker-1.6.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      990 2023-04-02 13:58:17.000000 blinker-1.6.1/README.rst
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-09 15:26:19.289915 blinker-1.6.1/docs/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      634 2023-04-02 13:58:17.000000 blinker-1.6.1/docs/Makefile
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-09 15:26:19.289915 blinker-1.6.1/docs/_static/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3627 2023-04-02 13:58:17.000000 blinker-1.6.1/docs/_static/blinker-named.png
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1195 2023-04-02 13:58:17.000000 blinker-1.6.1/docs/conf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9761 2023-04-02 13:58:17.000000 blinker-1.6.1/docs/index.rst
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      765 2023-04-02 13:58:17.000000 blinker-1.6.1/docs/make.bat
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1871 2023-04-09 15:23:14.000000 blinker-1.6.1/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-09 15:26:19.289915 blinker-1.6.1/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-09 15:26:19.289915 blinker-1.6.1/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-09 15:26:19.289915 blinker-1.6.1/src/blinker/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      409 2023-04-09 15:23:14.000000 blinker-1.6.1/src/blinker/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9081 2023-04-02 13:58:17.000000 blinker-1.6.1/src/blinker/_saferef.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3997 2023-04-02 13:58:17.000000 blinker-1.6.1/src/blinker/_utilities.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20317 2023-04-02 13:58:17.000000 blinker-1.6.1/src/blinker/base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-02 13:58:17.000000 blinker-1.6.1/src/blinker/py.typed
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-09 15:26:19.289915 blinker-1.6.1/src/blinker.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1964 2023-04-09 15:26:19.000000 blinker-1.6.1/src/blinker.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      535 2023-04-09 15:26:19.000000 blinker-1.6.1/src/blinker.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-09 15:26:19.000000 blinker-1.6.1/src/blinker.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-04-09 15:26:19.000000 blinker-1.6.1/src/blinker.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2023-04-09 15:26:19.000000 blinker-1.6.1/src/blinker.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-09 15:26:19.289915 blinker-1.6.1/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1053 2023-04-02 13:58:17.000000 blinker-1.6.1/tests/test_context.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3747 2023-04-02 13:58:17.000000 blinker-1.6.1/tests/test_saferef.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12962 2023-04-02 13:58:17.000000 blinker-1.6.1/tests/test_signals.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      451 2023-04-02 13:58:17.000000 blinker-1.6.1/tests/test_utilities.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      591 2023-04-02 13:58:17.000000 blinker-1.6.1/tox.ini
```

### Comparing `blinker-1.6/CHANGES.rst` & `blinker-1.6.1/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Version 1.6.1
+-------------
+
+Released 2023-04-09
+
+-   Ensure that py.typed is present in the distributions (to enable other
+    projects to use blinker's typing).
+-   Require typing-extensions > 4.2 to ensure it includes
+    ParamSpec. :issue:`90`
+
 Version 1.6
 -----------
 
 Released 2023-04-02
 
 -   Add a muted context manager to temporarily turn off a
     signal. :pr:`84`
```

### Comparing `blinker-1.6/LICENSE.rst` & `blinker-1.6.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `blinker-1.6/PKG-INFO` & `blinker-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blinker
-Version: 1.6
+Version: 1.6.1
 Summary: Fast, simple object-to-object and broadcast signaling
 Author-email: Jason Kirtland <jek@discorporate.us>
 Maintainer-email: Pallets Ecosystem <contact@palletsprojects.com>
 License: MIT License
 Project-URL: Homepage, https://blinker.readthedocs.io
 Project-URL: Documentation, https://blinker.readthedocs.io
 Project-URL: Source Code, https://github.com/pallets-eco/blinker/
```

### Comparing `blinker-1.6/README.rst` & `blinker-1.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `blinker-1.6/docs/Makefile` & `blinker-1.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `blinker-1.6/docs/_static/blinker-named.png` & `blinker-1.6.1/docs/_static/blinker-named.png`

 * *Files identical despite different names*

### Comparing `blinker-1.6/docs/conf.py` & `blinker-1.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blinker-1.6/docs/index.rst` & `blinker-1.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blinker-1.6/docs/make.bat` & `blinker-1.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `blinker-1.6/pyproject.toml` & `blinker-1.6.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Topic :: Software Development :: Libraries",
 ]
 requires-python = ">= 3.7"
 dynamic = ["version"]
-dependencies = ["typing-extensions"]
+dependencies = ["typing-extensions>=4.2"]
 
 [project.urls]
 Homepage = "https://blinker.readthedocs.io"
 Documentation = "https://blinker.readthedocs.io"
 "Source Code" = "https://github.com/pallets-eco/blinker/"
 "Issue Tracker" = "https://github.com/pallets-eco/blinker/issues/"
 Chat = "https://discord.gg/pallets"
@@ -56,15 +56,14 @@
 warn_unused_configs = true
 warn_unused_ignores = true
 warn_return_any = true
 #warn_unreachable = True
 
 [tool.setuptools]
 license-files = ["LICENSE.rst"]
-include-package-data = false
 
 [tool.setuptools.dynamic]
 version = {attr = "blinker.__version__"}
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 testpaths = ["tests"]
```

### Comparing `blinker-1.6/src/blinker/_saferef.py` & `blinker-1.6.1/src/blinker/_saferef.py`

 * *Files identical despite different names*

### Comparing `blinker-1.6/src/blinker/_utilities.py` & `blinker-1.6.1/src/blinker/_utilities.py`

 * *Files identical despite different names*

### Comparing `blinker-1.6/src/blinker/base.py` & `blinker-1.6.1/src/blinker/base.py`

 * *Files identical despite different names*

### Comparing `blinker-1.6/src/blinker.egg-info/PKG-INFO` & `blinker-1.6.1/src/blinker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blinker
-Version: 1.6
+Version: 1.6.1
 Summary: Fast, simple object-to-object and broadcast signaling
 Author-email: Jason Kirtland <jek@discorporate.us>
 Maintainer-email: Pallets Ecosystem <contact@palletsprojects.com>
 License: MIT License
 Project-URL: Homepage, https://blinker.readthedocs.io
 Project-URL: Documentation, https://blinker.readthedocs.io
 Project-URL: Source Code, https://github.com/pallets-eco/blinker/
```

### Comparing `blinker-1.6/src/blinker.egg-info/SOURCES.txt` & `blinker-1.6.1/src/blinker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blinker-1.6/tests/test_context.py` & `blinker-1.6.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `blinker-1.6/tests/test_saferef.py` & `blinker-1.6.1/tests/test_saferef.py`

 * *Files identical despite different names*

### Comparing `blinker-1.6/tests/test_signals.py` & `blinker-1.6.1/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `blinker-1.6/tox.ini` & `blinker-1.6.1/tox.ini`

 * *Files identical despite different names*

