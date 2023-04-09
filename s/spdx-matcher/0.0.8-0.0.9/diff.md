# Comparing `tmp/spdx_matcher-0.0.8.tar.gz` & `tmp/spdx_matcher-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spdx_matcher-0.0.8.tar", last modified: Sat Mar 18 08:33:45 2023, max compression
+gzip compressed data, was "spdx_matcher-0.0.9.tar", last modified: Sat Mar 18 09:19:19 2023, max compression
```

## Comparing `spdx_matcher-0.0.8.tar` & `spdx_matcher-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-03-18 08:33:45.305604 spdx_matcher-0.0.8/
--rw-r--r--   0 mike       (501) staff       (20)    28689 2023-03-18 05:22:17.000000 spdx_matcher-0.0.8/LICENSE.txt
--rw-r--r--   0 mike       (501) staff       (20)    50329 2023-03-18 08:33:45.305208 spdx_matcher-0.0.8/PKG-INFO
--rw-r--r--   0 mike       (501) staff       (20)    18638 2023-03-18 05:20:36.000000 spdx_matcher-0.0.8/README.md
--rw-r--r--   0 mike       (501) staff       (20)     5255 2023-03-18 08:32:35.000000 spdx_matcher-0.0.8/pyproject.toml
--rw-r--r--   0 mike       (501) staff       (20)       38 2023-03-18 08:33:45.305703 spdx_matcher-0.0.8/setup.cfg
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-03-18 08:33:45.279986 spdx_matcher-0.0.8/src/
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-03-18 08:33:45.282413 spdx_matcher-0.0.8/src/spdx_matcher/
--rw-r--r--   0 mike       (501) staff       (20)    25042 2023-03-17 06:43:58.000000 spdx_matcher-0.0.8/src/spdx_matcher/__init__.py
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-03-18 08:33:45.304095 spdx_matcher-0.0.8/src/spdx_matcher/_pyinstaller/
--rw-r--r--   0 mike       (501) staff       (20)       72 2023-03-18 08:07:01.000000 spdx_matcher-0.0.8/src/spdx_matcher/_pyinstaller/__init__.py
--rw-r--r--   0 mike       (501) staff       (20)      127 2023-03-18 08:07:01.000000 spdx_matcher-0.0.8/src/spdx_matcher/_pyinstaller/hook-spdx_matcher.py
--rw-r--r--   0 mike       (501) staff       (20)  9481047 2023-03-16 20:37:30.000000 spdx_matcher-0.0.8/src/spdx_matcher/spdxCache.json
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-03-18 08:33:45.303259 spdx_matcher-0.0.8/src/spdx_matcher.egg-info/
--rw-r--r--   0 mike       (501) staff       (20)    50329 2023-03-18 08:33:45.000000 spdx_matcher-0.0.8/src/spdx_matcher.egg-info/PKG-INFO
--rw-r--r--   0 mike       (501) staff       (20)      459 2023-03-18 08:33:45.000000 spdx_matcher-0.0.8/src/spdx_matcher.egg-info/SOURCES.txt
--rw-r--r--   0 mike       (501) staff       (20)        1 2023-03-18 08:33:45.000000 spdx_matcher-0.0.8/src/spdx_matcher.egg-info/dependency_links.txt
--rw-r--r--   0 mike       (501) staff       (20)      145 2023-03-18 08:33:45.000000 spdx_matcher-0.0.8/src/spdx_matcher.egg-info/entry_points.txt
--rw-r--r--   0 mike       (501) staff       (20)       45 2023-03-18 08:33:45.000000 spdx_matcher-0.0.8/src/spdx_matcher.egg-info/requires.txt
--rw-r--r--   0 mike       (501) staff       (20)       13 2023-03-18 08:33:45.000000 spdx_matcher-0.0.8/src/spdx_matcher.egg-info/top_level.txt
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-03-18 08:33:45.304537 spdx_matcher-0.0.8/tests/
--rw-r--r--   0 mike       (501) staff       (20)    11724 2023-03-17 05:57:30.000000 spdx_matcher-0.0.8/tests/test_spdx_matcher.py
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-03-18 09:19:19.955612 spdx_matcher-0.0.9/
+-rw-r--r--   0 mike       (501) staff       (20)    28689 2023-03-18 05:22:17.000000 spdx_matcher-0.0.9/LICENSE.txt
+-rw-r--r--   0 mike       (501) staff       (20)    50329 2023-03-18 09:19:19.955225 spdx_matcher-0.0.9/PKG-INFO
+-rw-r--r--   0 mike       (501) staff       (20)    18638 2023-03-18 05:20:36.000000 spdx_matcher-0.0.9/README.md
+-rw-r--r--   0 mike       (501) staff       (20)     5254 2023-03-18 09:17:55.000000 spdx_matcher-0.0.9/pyproject.toml
+-rw-r--r--   0 mike       (501) staff       (20)       38 2023-03-18 09:19:19.955709 spdx_matcher-0.0.9/setup.cfg
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-03-18 09:19:19.932323 spdx_matcher-0.0.9/src/
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-03-18 09:19:19.934728 spdx_matcher-0.0.9/src/spdx_matcher/
+-rw-r--r--   0 mike       (501) staff       (20)    25042 2023-03-17 06:43:58.000000 spdx_matcher-0.0.9/src/spdx_matcher/__init__.py
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-03-18 09:19:19.954104 spdx_matcher-0.0.9/src/spdx_matcher/_pyinstaller/
+-rw-r--r--   0 mike       (501) staff       (20)       72 2023-03-18 08:07:01.000000 spdx_matcher-0.0.9/src/spdx_matcher/_pyinstaller/__init__.py
+-rw-r--r--   0 mike       (501) staff       (20)      127 2023-03-18 08:07:01.000000 spdx_matcher-0.0.9/src/spdx_matcher/_pyinstaller/hook-spdx_matcher.py
+-rw-r--r--   0 mike       (501) staff       (20)  9481047 2023-03-16 20:37:30.000000 spdx_matcher-0.0.9/src/spdx_matcher/spdxCache.json
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-03-18 09:19:19.953297 spdx_matcher-0.0.9/src/spdx_matcher.egg-info/
+-rw-r--r--   0 mike       (501) staff       (20)    50329 2023-03-18 09:19:19.000000 spdx_matcher-0.0.9/src/spdx_matcher.egg-info/PKG-INFO
+-rw-r--r--   0 mike       (501) staff       (20)      459 2023-03-18 09:19:19.000000 spdx_matcher-0.0.9/src/spdx_matcher.egg-info/SOURCES.txt
+-rw-r--r--   0 mike       (501) staff       (20)        1 2023-03-18 09:19:19.000000 spdx_matcher-0.0.9/src/spdx_matcher.egg-info/dependency_links.txt
+-rw-r--r--   0 mike       (501) staff       (20)      144 2023-03-18 09:19:19.000000 spdx_matcher-0.0.9/src/spdx_matcher.egg-info/entry_points.txt
+-rw-r--r--   0 mike       (501) staff       (20)       45 2023-03-18 09:19:19.000000 spdx_matcher-0.0.9/src/spdx_matcher.egg-info/requires.txt
+-rw-r--r--   0 mike       (501) staff       (20)       13 2023-03-18 09:19:19.000000 spdx_matcher-0.0.9/src/spdx_matcher.egg-info/top_level.txt
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-03-18 09:19:19.954531 spdx_matcher-0.0.9/tests/
+-rw-r--r--   0 mike       (501) staff       (20)    11724 2023-03-17 05:57:30.000000 spdx_matcher-0.0.9/tests/test_spdx_matcher.py
```

### Comparing `spdx_matcher-0.0.8/LICENSE.txt` & `spdx_matcher-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spdx_matcher-0.0.8/PKG-INFO` & `spdx_matcher-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spdx_matcher
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package that enables extracting licenses from free text using spdx license matching algorithm
 Author-email: Mike Moore <z_z_zebra@yahoo.com>
 Maintainer-email: Mike Moore <z_z_zebra@yahoo.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `spdx_matcher-0.0.8/README.md` & `spdx_matcher-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `spdx_matcher-0.0.8/pyproject.toml` & `spdx_matcher-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "spdx_matcher"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.8"  # Required
+version = "0.0.9"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "A package that enables extracting licenses from free text using spdx license matching algorithm"  # Optional
 
 readme = "README.md" # Optional
@@ -116,15 +116,15 @@
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 [tool.setuptools]
 package-data = {"spdx_matcher" = ["spdxCache.json"]}
 
 [project.entry-points."spdx_matcher"]
-pyinstaller40 = "spdx_matcher.__pyinstaller:get_hook_dirs"
+pyinstaller40 = "spdx_matcher._pyinstaller:get_hook_dirs"
 
 [tool.black]
 line-length = 88
 
 [build-system]
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
```

### Comparing `spdx_matcher-0.0.8/src/spdx_matcher/__init__.py` & `spdx_matcher-0.0.9/src/spdx_matcher/__init__.py`

 * *Files identical despite different names*

### Comparing `spdx_matcher-0.0.8/src/spdx_matcher/spdxCache.json` & `spdx_matcher-0.0.9/src/spdx_matcher/spdxCache.json`

 * *Files identical despite different names*

### Comparing `spdx_matcher-0.0.8/src/spdx_matcher.egg-info/PKG-INFO` & `spdx_matcher-0.0.9/src/spdx_matcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spdx-matcher
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package that enables extracting licenses from free text using spdx license matching algorithm
 Author-email: Mike Moore <z_z_zebra@yahoo.com>
 Maintainer-email: Mike Moore <z_z_zebra@yahoo.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `spdx_matcher-0.0.8/tests/test_spdx_matcher.py` & `spdx_matcher-0.0.9/tests/test_spdx_matcher.py`

 * *Files identical despite different names*

