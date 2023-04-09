# Comparing `tmp/ddcci_plasmoid_backend-0.1.0.tar.gz` & `tmp/ddcci_plasmoid_backend-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddcci_plasmoid_backend-0.1.0.tar", max compression
+gzip compressed data, was "ddcci_plasmoid_backend-0.1.1.tar", max compression
```

## Comparing `ddcci_plasmoid_backend-0.1.0.tar` & `ddcci_plasmoid_backend-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1276 2023-04-09 11:20:03.343482 ddcci_plasmoid_backend-0.1.0/ddcci_plasmoid_backend/__init__.py
--rw-r--r--   0        0        0     2484 2023-04-09 13:52:00.246495 ddcci_plasmoid_backend-0.1.0/ddcci_plasmoid_backend/__main__.py
--rw-r--r--   0        0        0     3053 2023-04-09 11:37:36.411064 ddcci_plasmoid_backend-0.1.0/ddcci_plasmoid_backend/ddcci.py
--rw-r--r--   0        0        0     2426 2023-04-08 18:58:49.286640 ddcci_plasmoid_backend-0.1.0/ddcci_plasmoid_backend/ddcutil_parser.py
--rw-r--r--   0        0        0      400 2023-04-09 10:41:45.605341 ddcci_plasmoid_backend-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 ddcci_plasmoid_backend-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1276 2023-04-09 11:20:03.343482 ddcci_plasmoid_backend-0.1.1/ddcci_plasmoid_backend/__init__.py
+-rw-r--r--   0        0        0     2718 2023-04-09 16:12:30.293937 ddcci_plasmoid_backend-0.1.1/ddcci_plasmoid_backend/__main__.py
+-rw-r--r--   0        0        0     3053 2023-04-09 11:37:36.411064 ddcci_plasmoid_backend-0.1.1/ddcci_plasmoid_backend/ddcci.py
+-rw-r--r--   0        0        0     2426 2023-04-08 18:58:49.286640 ddcci_plasmoid_backend-0.1.1/ddcci_plasmoid_backend/ddcutil_parser.py
+-rw-r--r--   0        0        0      400 2023-04-09 16:10:53.377359 ddcci_plasmoid_backend-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 ddcci_plasmoid_backend-0.1.1/PKG-INFO
```

### Comparing `ddcci_plasmoid_backend-0.1.0/ddcci_plasmoid_backend/__init__.py` & `ddcci_plasmoid_backend-0.1.1/ddcci_plasmoid_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `ddcci_plasmoid_backend-0.1.0/ddcci_plasmoid_backend/__main__.py` & `ddcci_plasmoid_backend-0.1.1/ddcci_plasmoid_backend/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import logging
 import subprocess
 import sys
 import tempfile
 from importlib.metadata import version
 from pathlib import Path
+import os
 from typing import NoReturn
 
 import fasteners
 
 from ddcci_plasmoid_backend import arguments
 from ddcci_plasmoid_backend import ddcci
 
@@ -29,15 +30,17 @@
 if __name__ == '__main__':
     logger.debug(f'Command: {arguments["command"]}')
 
     if arguments['command'] == 'version':
         print(version('ddcci-plasmoid-backend'))
         sys.exit(0)
 
-    with fasteners.InterProcessLock(Path(tempfile.gettempdir()) / 'ddcci_plasmoid_backend.lock'):
+    # include the username in the lock file. Otherwise, if user A creates a lock, user B may not have the permissions
+    # to access the lock file and this program will fail until the lock file is deleted.
+    with fasteners.InterProcessLock(Path(tempfile.gettempdir()) / f'ddcci_plasmoid_backend-{os.getlogin()}.lock'):
         if arguments['command'] == 'detect':
             try:
                 result = asyncio.run(ddcci.detect())
             except subprocess.CalledProcessError as err:
                 handle_error(err)
 
             # Remove objects that are errors
```

### Comparing `ddcci_plasmoid_backend-0.1.0/ddcci_plasmoid_backend/ddcci.py` & `ddcci_plasmoid_backend-0.1.1/ddcci_plasmoid_backend/ddcci.py`

 * *Files identical despite different names*

### Comparing `ddcci_plasmoid_backend-0.1.0/ddcci_plasmoid_backend/ddcutil_parser.py` & `ddcci_plasmoid_backend-0.1.1/ddcci_plasmoid_backend/ddcutil_parser.py`

 * *Files identical despite different names*

