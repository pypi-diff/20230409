# Comparing `tmp/interactive-score-editor-0.1.2.tar.gz` & `tmp/interactive-score-editor-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactive-score-editor-0.1.2.tar", last modified: Sun Mar 26 07:46:51 2023, max compression
+gzip compressed data, was "interactive-score-editor-0.1.3.tar", last modified: Sun Apr  9 04:41:00 2023, max compression
```

## Comparing `interactive-score-editor-0.1.2.tar` & `interactive-score-editor-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 sadigulcelik   (501) staff       (20)        0 2023-03-26 07:46:51.318625 interactive-score-editor-0.1.2/
--rw-r--r--   0 sadigulcelik   (501) staff       (20)      292 2023-03-26 07:41:05.000000 interactive-score-editor-0.1.2/.bumpversion.cfg
--rw-r--r--   0 sadigulcelik   (501) staff       (20)     1580 2023-03-26 06:22:15.000000 interactive-score-editor-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 sadigulcelik   (501) staff       (20)    11357 2023-02-18 22:04:57.000000 interactive-score-editor-0.1.2/LICENSE
--rw-r--r--   0 sadigulcelik   (501) staff       (20)      461 2023-03-25 01:37:30.000000 interactive-score-editor-0.1.2/MANIFEST.in
--rw-r--r--   0 sadigulcelik   (501) staff       (20)     1913 2023-03-26 06:37:35.000000 interactive-score-editor-0.1.2/Makefile
--rw-r--r--   0 sadigulcelik   (501) staff       (20)    16198 2023-03-26 07:46:51.318400 interactive-score-editor-0.1.2/PKG-INFO
--rw-r--r--   0 sadigulcelik   (501) staff       (20)     2828 2023-03-26 07:41:05.000000 interactive-score-editor-0.1.2/README.md
--rw-r--r--   0 sadigulcelik   (501) staff       (20)     1893 2023-03-26 07:41:05.000000 interactive-score-editor-0.1.2/pyproject.toml
--rw-r--r--   0 sadigulcelik   (501) staff       (20)       38 2023-03-26 07:46:51.318674 interactive-score-editor-0.1.2/setup.cfg
--rw-r--r--   0 sadigulcelik   (501) staff       (20)       39 2023-03-25 01:37:30.000000 interactive-score-editor-0.1.2/setup.py
-drwxr-xr-x   0 sadigulcelik   (501) staff       (20)        0 2023-03-26 07:46:51.317093 interactive-score-editor-0.1.2/src/
--rw-r--r--   0 sadigulcelik   (501) staff       (20)     9659 2023-03-26 05:43:04.000000 interactive-score-editor-0.1.2/src/Base.py
--rw-r--r--   0 sadigulcelik   (501) staff       (20)       22 2023-03-26 07:41:05.000000 interactive-score-editor-0.1.2/src/__init__.py
-drwxr-xr-x   0 sadigulcelik   (501) staff       (20)        0 2023-03-26 07:46:51.317899 interactive-score-editor-0.1.2/src/interactive_score_editor.egg-info/
--rw-r--r--   0 sadigulcelik   (501) staff       (20)    16198 2023-03-26 07:46:51.000000 interactive-score-editor-0.1.2/src/interactive_score_editor.egg-info/PKG-INFO
--rw-r--r--   0 sadigulcelik   (501) staff       (20)      420 2023-03-26 07:46:51.000000 interactive-score-editor-0.1.2/src/interactive_score_editor.egg-info/SOURCES.txt
--rw-r--r--   0 sadigulcelik   (501) staff       (20)        1 2023-03-26 07:46:51.000000 interactive-score-editor-0.1.2/src/interactive_score_editor.egg-info/dependency_links.txt
--rw-r--r--   0 sadigulcelik   (501) staff       (20)      213 2023-03-26 07:46:51.000000 interactive-score-editor-0.1.2/src/interactive_score_editor.egg-info/requires.txt
--rw-r--r--   0 sadigulcelik   (501) staff       (20)       20 2023-03-26 07:46:51.000000 interactive-score-editor-0.1.2/src/interactive_score_editor.egg-info/top_level.txt
-drwxr-xr-x   0 sadigulcelik   (501) staff       (20)        0 2023-03-26 07:46:51.318040 interactive-score-editor-0.1.2/src/tests/
--rw-r--r--   0 sadigulcelik   (501) staff       (20)     4892 2023-03-26 05:43:04.000000 interactive-score-editor-0.1.2/src/tests/test_all.py
-drwxr-xr-x   0 sadigulcelik   (501) staff       (20)        0 2023-03-26 07:46:51.318172 interactive-score-editor-0.1.2/temp/
--rw-r--r--   0 sadigulcelik   (501) staff       (20)       18 2023-03-25 01:37:30.000000 interactive-score-editor-0.1.2/temp/TESTING.md
+drwxr-xr-x   0 sadigulcelik   (501) staff       (20)        0 2023-04-09 04:41:00.067897 interactive-score-editor-0.1.3/
+-rw-r--r--   0 sadigulcelik   (501) staff       (20)      292 2023-04-09 04:40:28.000000 interactive-score-editor-0.1.3/.bumpversion.cfg
+-rw-r--r--   0 sadigulcelik   (501) staff       (20)     1580 2023-04-03 04:33:04.000000 interactive-score-editor-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0 sadigulcelik   (501) staff       (20)    11357 2023-04-03 04:33:04.000000 interactive-score-editor-0.1.3/LICENSE
+-rw-r--r--   0 sadigulcelik   (501) staff       (20)      461 2023-04-09 04:40:28.000000 interactive-score-editor-0.1.3/MANIFEST.in
+-rw-r--r--   0 sadigulcelik   (501) staff       (20)     1913 2023-04-09 04:40:28.000000 interactive-score-editor-0.1.3/Makefile
+-rw-r--r--   0 sadigulcelik   (501) staff       (20)    16411 2023-04-09 04:41:00.067708 interactive-score-editor-0.1.3/PKG-INFO
+-rw-r--r--   0 sadigulcelik   (501) staff       (20)     3041 2023-04-09 04:40:28.000000 interactive-score-editor-0.1.3/README.md
+-rw-r--r--   0 sadigulcelik   (501) staff       (20)     1893 2023-04-09 04:40:28.000000 interactive-score-editor-0.1.3/pyproject.toml
+-rw-r--r--   0 sadigulcelik   (501) staff       (20)       38 2023-04-09 04:41:00.067938 interactive-score-editor-0.1.3/setup.cfg
+-rw-r--r--   0 sadigulcelik   (501) staff       (20)       39 2023-04-03 04:33:04.000000 interactive-score-editor-0.1.3/setup.py
+drwxr-xr-x   0 sadigulcelik   (501) staff       (20)        0 2023-04-09 04:41:00.066513 interactive-score-editor-0.1.3/src/
+-rw-r--r--   0 sadigulcelik   (501) staff       (20)     9659 2023-04-09 04:40:28.000000 interactive-score-editor-0.1.3/src/Base.py
+-rw-r--r--   0 sadigulcelik   (501) staff       (20)       22 2023-04-09 04:40:28.000000 interactive-score-editor-0.1.3/src/__init__.py
+drwxr-xr-x   0 sadigulcelik   (501) staff       (20)        0 2023-04-09 04:41:00.067162 interactive-score-editor-0.1.3/src/interactive_score_editor.egg-info/
+-rw-r--r--   0 sadigulcelik   (501) staff       (20)    16411 2023-04-09 04:41:00.000000 interactive-score-editor-0.1.3/src/interactive_score_editor.egg-info/PKG-INFO
+-rw-r--r--   0 sadigulcelik   (501) staff       (20)      420 2023-04-09 04:41:00.000000 interactive-score-editor-0.1.3/src/interactive_score_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 sadigulcelik   (501) staff       (20)        1 2023-04-09 04:41:00.000000 interactive-score-editor-0.1.3/src/interactive_score_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 sadigulcelik   (501) staff       (20)      213 2023-04-09 04:41:00.000000 interactive-score-editor-0.1.3/src/interactive_score_editor.egg-info/requires.txt
+-rw-r--r--   0 sadigulcelik   (501) staff       (20)       20 2023-04-09 04:41:00.000000 interactive-score-editor-0.1.3/src/interactive_score_editor.egg-info/top_level.txt
+drwxr-xr-x   0 sadigulcelik   (501) staff       (20)        0 2023-04-09 04:41:00.067306 interactive-score-editor-0.1.3/src/tests/
+-rw-r--r--   0 sadigulcelik   (501) staff       (20)     4892 2023-04-09 04:40:28.000000 interactive-score-editor-0.1.3/src/tests/test_all.py
+drwxr-xr-x   0 sadigulcelik   (501) staff       (20)        0 2023-04-09 04:41:00.067444 interactive-score-editor-0.1.3/temp/
+-rw-r--r--   0 sadigulcelik   (501) staff       (20)       18 2023-04-09 04:40:28.000000 interactive-score-editor-0.1.3/temp/TESTING.md
```

### Comparing `interactive-score-editor-0.1.2/CONTRIBUTING.md` & `interactive-score-editor-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `interactive-score-editor-0.1.2/LICENSE` & `interactive-score-editor-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `interactive-score-editor-0.1.2/Makefile` & `interactive-score-editor-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `interactive-score-editor-0.1.2/PKG-INFO` & `interactive-score-editor-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interactive-score-editor
-Version: 0.1.2
+Version: 0.1.3
 Summary: Interactive Score Editor
 Author-email: Sadi Gulcelik <sg3790@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -208,16 +208,26 @@
 Project-URL: repository, https://github.com/sadigulcelik/interactive-score-editor
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
+
+## This package has been renamed as [isedit](https://pypi.org/project/isedit/)
+
+<br>
+<br>
+
 # Interactive Score Editor
+
+
+
 A python library that combines score editing tools with audio output.<br>
+[![PyPI](https://img.shields.io/pypi/v/interactive-score-editor)](https://pypi.org/project/interactive-score-editor/)
 [![Build Status](https://github.com/sadigulcelik/interactive-score-editor/actions/workflows/build.yml/badge.svg)](https://github.com/sadigulcelik/interactive-score-editor/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/sadigulcelik/interactive-score-editor/branch/main/graph/badge.svg?token=Y3YYB6AYD1)](https://codecov.io/gh/sadigulcelik/interactive-score-editor)
 ![image](https://img.shields.io/badge/license-Apache--2.0-brightgreen)
 ![image](https://img.shields.io/github/issues/sadigulcelik/interactive-score-editor)
 
 ## Overview
```

### Comparing `interactive-score-editor-0.1.2/README.md` & `interactive-score-editor-0.1.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,19 @@
+
+## This package has been renamed as [isedit](https://pypi.org/project/isedit/)
+
+<br>
+<br>
+
 # Interactive Score Editor
+
+
+
 A python library that combines score editing tools with audio output.<br>
+[![PyPI](https://img.shields.io/pypi/v/interactive-score-editor)](https://pypi.org/project/interactive-score-editor/)
 [![Build Status](https://github.com/sadigulcelik/interactive-score-editor/actions/workflows/build.yml/badge.svg)](https://github.com/sadigulcelik/interactive-score-editor/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/sadigulcelik/interactive-score-editor/branch/main/graph/badge.svg?token=Y3YYB6AYD1)](https://codecov.io/gh/sadigulcelik/interactive-score-editor)
 ![image](https://img.shields.io/badge/license-Apache--2.0-brightgreen)
 ![image](https://img.shields.io/github/issues/sadigulcelik/interactive-score-editor)
 
 ## Overview
```

### Comparing `interactive-score-editor-0.1.2/pyproject.toml` & `interactive-score-editor-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "interactive-score-editor"
 authors = [{name = "Sadi Gulcelik", email = "sg3790@columbia.edu"}]
 description="Interactive Score Editor"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 requires-python = ">=3.7"
 
 dependencies = []
 
 classifiers = [
     "Programming Language :: Python :: 3.10",
 ]
```

### Comparing `interactive-score-editor-0.1.2/src/Base.py` & `interactive-score-editor-0.1.3/src/Base.py`

 * *Files identical despite different names*

### Comparing `interactive-score-editor-0.1.2/src/interactive_score_editor.egg-info/PKG-INFO` & `interactive-score-editor-0.1.3/src/interactive_score_editor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interactive-score-editor
-Version: 0.1.2
+Version: 0.1.3
 Summary: Interactive Score Editor
 Author-email: Sadi Gulcelik <sg3790@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -208,16 +208,26 @@
 Project-URL: repository, https://github.com/sadigulcelik/interactive-score-editor
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
+
+## This package has been renamed as [isedit](https://pypi.org/project/isedit/)
+
+<br>
+<br>
+
 # Interactive Score Editor
+
+
+
 A python library that combines score editing tools with audio output.<br>
+[![PyPI](https://img.shields.io/pypi/v/interactive-score-editor)](https://pypi.org/project/interactive-score-editor/)
 [![Build Status](https://github.com/sadigulcelik/interactive-score-editor/actions/workflows/build.yml/badge.svg)](https://github.com/sadigulcelik/interactive-score-editor/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/sadigulcelik/interactive-score-editor/branch/main/graph/badge.svg?token=Y3YYB6AYD1)](https://codecov.io/gh/sadigulcelik/interactive-score-editor)
 ![image](https://img.shields.io/badge/license-Apache--2.0-brightgreen)
 ![image](https://img.shields.io/github/issues/sadigulcelik/interactive-score-editor)
 
 ## Overview
```

### Comparing `interactive-score-editor-0.1.2/src/tests/test_all.py` & `interactive-score-editor-0.1.3/src/tests/test_all.py`

 * *Files identical despite different names*

