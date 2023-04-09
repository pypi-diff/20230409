# Comparing `tmp/synth_mapping_helper-1.1.0.tar.gz` & `tmp/synth_mapping_helper-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synth_mapping_helper-1.1.0.tar", last modified: Sun Apr  9 17:16:00 2023, max compression
+gzip compressed data, was "synth_mapping_helper-1.1.1.tar", last modified: Sun Apr  9 17:27:56 2023, max compression
```

## Comparing `synth_mapping_helper-1.1.0.tar` & `synth_mapping_helper-1.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:16:00.862068 synth_mapping_helper-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-09 17:16:00.862068 synth_mapping_helper-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 17:16:00.862068 synth_mapping_helper-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:16:00.862068 synth_mapping_helper-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:16:00.862068 synth_mapping_helper-1.1.0/src/synth_mapping_helper/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25631 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    26636 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper/companion.py
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper/finalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper/movement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper/pattern_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper/rails.py
--rw-r--r--   0 runner    (1001) docker     (123)    16398 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper/synth_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:16:00.862068 synth_mapping_helper-1.1.0/src/synth_mapping_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-09 17:16:00.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-09 17:16:00.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:16:00.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-09 17:16:00.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-09 17:16:00.000000 synth_mapping_helper-1.1.0/src/synth_mapping_helper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:16:00.862068 synth_mapping_helper-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-09 17:15:44.000000 synth_mapping_helper-1.1.0/tests/test_synth_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:27:56.592177 synth_mapping_helper-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-09 17:27:56.592177 synth_mapping_helper-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 17:27:56.592177 synth_mapping_helper-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:27:56.592177 synth_mapping_helper-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:27:56.592177 synth_mapping_helper-1.1.1/src/synth_mapping_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25631 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26636 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper/companion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper/movement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper/pattern_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper/rails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16429 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper/synth_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:27:56.592177 synth_mapping_helper-1.1.1/src/synth_mapping_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-09 17:27:56.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-09 17:27:56.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:27:56.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-09 17:27:56.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-09 17:27:56.000000 synth_mapping_helper-1.1.1/src/synth_mapping_helper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:27:56.592177 synth_mapping_helper-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-09 17:27:46.000000 synth_mapping_helper-1.1.1/tests/test_synth_format.py
```

### Comparing `synth_mapping_helper-1.1.0/LICENSE` & `synth_mapping_helper-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.1.0/PKG-INFO` & `synth_mapping_helper-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synth_mapping_helper
-Version: 1.1.0
+Version: 1.1.1
 Summary: Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard
 Home-page: https://github.com/adosikas/synth_mapping_helper
 Author: adosikas
 Author-email: 
 Project-URL: Documentation, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Bug Reports, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Source Code, https://github.com/adosikas/synth_mapping_helper
```

### Comparing `synth_mapping_helper-1.1.0/README.md` & `synth_mapping_helper-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.1.0/setup.py` & `synth_mapping_helper-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.1.0/src/synth_mapping_helper/cli.py` & `synth_mapping_helper-1.1.1/src/synth_mapping_helper/cli.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.1.0/src/synth_mapping_helper/companion.py` & `synth_mapping_helper-1.1.1/src/synth_mapping_helper/companion.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.1.0/src/synth_mapping_helper/finalize.py` & `synth_mapping_helper-1.1.1/src/synth_mapping_helper/finalize.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.1.0/src/synth_mapping_helper/movement.py` & `synth_mapping_helper-1.1.1/src/synth_mapping_helper/movement.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.1.0/src/synth_mapping_helper/pattern_generation.py` & `synth_mapping_helper-1.1.1/src/synth_mapping_helper/pattern_generation.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.1.0/src/synth_mapping_helper/rails.py` & `synth_mapping_helper-1.1.1/src/synth_mapping_helper/rails.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.1.0/src/synth_mapping_helper/synth_format.py` & `synth_mapping_helper-1.1.1/src/synth_mapping_helper/synth_format.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #/usr/bin/env python3
 from io import BytesIO
 import dataclasses
 import json
 from pathlib import Path
+from typing import Union
 from zipfile import ZipFile
 
 import numpy as np
 import pyperclip
 
 # For simplicity, we exclusively use grid coordinates (x, y) and use measures for time (z)
 # These values are only needed to convert to / from the format the game uses
@@ -134,15 +135,15 @@
     def merge(self, other: "DataContainer") -> None:
         for t in NOTE_TYPES:
             self_notes = getattr(self, t)
             other_notes = getattr(other, t)
             setattr(self, t, self_notes | other_notes)
         self.walls |= other.walls
 
-    def get_object_dict(self, type_name: str) -> SINGLE_COLOR_NOTES | WALLS:
+    def get_object_dict(self, type_name: str) -> Union[SINGLE_COLOR_NOTES, WALLS]:
         if type_name in NOTE_TYPES:
             return getattr(self, type_name)
         wall_type = WALL_TYPES[type_name][0]
         return {
             time_index: wall
             for time_index, wall in sorted(self.walls.items())
             if wall[0, 3] == wall_type
```

### Comparing `synth_mapping_helper-1.1.0/src/synth_mapping_helper/utils.py` & `synth_mapping_helper-1.1.1/src/synth_mapping_helper/utils.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.1.0/src/synth_mapping_helper.egg-info/PKG-INFO` & `synth_mapping_helper-1.1.1/src/synth_mapping_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synth-mapping-helper
-Version: 1.1.0
+Version: 1.1.1
 Summary: Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard
 Home-page: https://github.com/adosikas/synth_mapping_helper
 Author: adosikas
 Author-email: 
 Project-URL: Documentation, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Bug Reports, https://github.com/adosikas/synth_mapping_helper
 Project-URL: Source Code, https://github.com/adosikas/synth_mapping_helper
```

### Comparing `synth_mapping_helper-1.1.0/src/synth_mapping_helper.egg-info/SOURCES.txt` & `synth_mapping_helper-1.1.1/src/synth_mapping_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

