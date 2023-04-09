# Comparing `tmp/katalytic-files-0.3.1.tar.gz` & `tmp/katalytic-files-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-files-0.3.1.tar", last modified: Sat Apr  8 16:39:30 2023, max compression
+gzip compressed data, was "katalytic-files-0.3.2.tar", last modified: Sun Apr  9 06:14:04 2023, max compression
```

## Comparing `katalytic-files-0.3.1.tar` & `katalytic-files-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-08 16:39:30.309463 katalytic-files-0.3.1/
--rw-rw-r--   0 wip       (1000) wip       (1000)     1066 2023-04-06 18:07:34.000000 katalytic-files-0.3.1/LICENSE.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)     3352 2023-04-08 16:39:30.309463 katalytic-files-0.3.1/PKG-INFO
--rw-rw-r--   0 wip       (1000) wip       (1000)     1224 2023-04-06 18:07:34.000000 katalytic-files-0.3.1/README.md
--rw-rw-r--   0 wip       (1000) wip       (1000)     1081 2023-04-08 16:32:07.000000 katalytic-files-0.3.1/pyproject.toml
--rw-rw-r--   0 wip       (1000) wip       (1000)       38 2023-04-08 16:39:30.309463 katalytic-files-0.3.1/setup.cfg
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-08 16:39:30.305463 katalytic-files-0.3.1/src/
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-08 16:39:30.309463 katalytic-files-0.3.1/src/katalytic/
--rw-rw-r--   0 wip       (1000) wip       (1000)    10925 2023-04-08 16:31:34.000000 katalytic-files-0.3.1/src/katalytic/files.py
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-08 16:39:30.309463 katalytic-files-0.3.1/src/katalytic_files.egg-info/
--rw-rw-r--   0 wip       (1000) wip       (1000)     3352 2023-04-08 16:39:30.000000 katalytic-files-0.3.1/src/katalytic_files.egg-info/PKG-INFO
--rw-rw-r--   0 wip       (1000) wip       (1000)      293 2023-04-08 16:39:30.000000 katalytic-files-0.3.1/src/katalytic_files.egg-info/SOURCES.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)        1 2023-04-08 16:39:30.000000 katalytic-files-0.3.1/src/katalytic_files.egg-info/dependency_links.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)       35 2023-04-08 16:39:30.000000 katalytic-files-0.3.1/src/katalytic_files.egg-info/requires.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)       10 2023-04-08 16:39:30.000000 katalytic-files-0.3.1/src/katalytic_files.egg-info/top_level.txt
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-08 16:39:30.309463 katalytic-files-0.3.1/tests/
--rw-rw-r--   0 wip       (1000) wip       (1000)    39656 2023-04-06 18:07:34.000000 katalytic-files-0.3.1/tests/test_files.py
+drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 06:14:04.797819 katalytic-files-0.3.2/
+-rw-rw-r--   0 wip       (1000) wip       (1000)     1066 2023-04-06 18:07:34.000000 katalytic-files-0.3.2/LICENSE.txt
+-rw-rw-r--   0 wip       (1000) wip       (1000)     3352 2023-04-09 06:14:04.797819 katalytic-files-0.3.2/PKG-INFO
+-rw-rw-r--   0 wip       (1000) wip       (1000)     1224 2023-04-06 18:07:34.000000 katalytic-files-0.3.2/README.md
+-rw-rw-r--   0 wip       (1000) wip       (1000)     1081 2023-04-09 04:47:14.000000 katalytic-files-0.3.2/pyproject.toml
+-rw-rw-r--   0 wip       (1000) wip       (1000)       38 2023-04-09 06:14:04.797819 katalytic-files-0.3.2/setup.cfg
+drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 06:14:04.797819 katalytic-files-0.3.2/src/
+drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 06:14:04.797819 katalytic-files-0.3.2/src/katalytic/
+-rw-rw-r--   0 wip       (1000) wip       (1000)    10912 2023-04-09 04:16:13.000000 katalytic-files-0.3.2/src/katalytic/files.py
+drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 06:14:04.797819 katalytic-files-0.3.2/src/katalytic_files.egg-info/
+-rw-rw-r--   0 wip       (1000) wip       (1000)     3352 2023-04-09 06:14:04.000000 katalytic-files-0.3.2/src/katalytic_files.egg-info/PKG-INFO
+-rw-rw-r--   0 wip       (1000) wip       (1000)      293 2023-04-09 06:14:04.000000 katalytic-files-0.3.2/src/katalytic_files.egg-info/SOURCES.txt
+-rw-rw-r--   0 wip       (1000) wip       (1000)        1 2023-04-09 06:14:04.000000 katalytic-files-0.3.2/src/katalytic_files.egg-info/dependency_links.txt
+-rw-rw-r--   0 wip       (1000) wip       (1000)       35 2023-04-09 06:14:04.000000 katalytic-files-0.3.2/src/katalytic_files.egg-info/requires.txt
+-rw-rw-r--   0 wip       (1000) wip       (1000)       10 2023-04-09 06:14:04.000000 katalytic-files-0.3.2/src/katalytic_files.egg-info/top_level.txt
+drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 06:14:04.797819 katalytic-files-0.3.2/tests/
+-rw-rw-r--   0 wip       (1000) wip       (1000)    39656 2023-04-06 18:07:34.000000 katalytic-files-0.3.2/tests/test_files.py
```

### Comparing `katalytic-files-0.3.1/LICENSE.txt` & `katalytic-files-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.1/PKG-INFO` & `katalytic-files-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-files
-Version: 0.3.1
+Version: 0.3.2
 Summary: This plugin adds utilities for working with files to the katalytic namespace
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 License: Copyright 2023 - present, Valentin Neagu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `katalytic-files-0.3.1/README.md` & `katalytic-files-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-files-0.3.1/pyproject.toml` & `katalytic-files-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "katalytic-files"
-version = "0.3.1"
+version = "0.3.2"
 description = "This plugin adds utilities for working with files to the katalytic namespace"
 
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 requires-python = ">=3.6"
 dependencies = [
-	"katalytic-pkg>=0.1.1",
+	"katalytic-pkg>=0.2.0",
 ]
 
 classifiers = [
 	"Development Status :: 4 - Beta",
 	"Intended Audience :: Developers",
 	"Intended Audience :: System Administrators",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `katalytic-files-0.3.1/src/katalytic/files.py` & `katalytic-files-0.3.2/src/katalytic/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import itertools
 import re
 import shutil
 from pathlib import Path
 
 from katalytic.pkg import get_version
 
-__version__, __version_info__ = get_version(__name__, __package__)
+__version__, __version_info__ = get_version(__name__)
 
 
 def clear_dir(path, *, create_missing=True):
     """This function is not named "empty_dir" to avoid confusing it with "is_dir_empty"."""
     if not isinstance(create_missing, bool):
         raise TypeError(f'<create_missing> expects False or True. Got {type(create_missing)}')
```

### Comparing `katalytic-files-0.3.1/src/katalytic_files.egg-info/PKG-INFO` & `katalytic-files-0.3.2/src/katalytic_files.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-files
-Version: 0.3.1
+Version: 0.3.2
 Summary: This plugin adds utilities for working with files to the katalytic namespace
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 License: Copyright 2023 - present, Valentin Neagu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `katalytic-files-0.3.1/tests/test_files.py` & `katalytic-files-0.3.2/tests/test_files.py`

 * *Files identical despite different names*

