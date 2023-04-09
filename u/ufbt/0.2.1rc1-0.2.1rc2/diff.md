# Comparing `tmp/ufbt-0.2.1rc1.tar.gz` & `tmp/ufbt-0.2.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufbt-0.2.1rc1.tar", last modified: Sat Apr  8 22:53:28 2023, max compression
+gzip compressed data, was "ufbt-0.2.1rc2.tar", last modified: Sun Apr  9 12:59:58 2023, max compression
```

## Comparing `ufbt-0.2.1rc1.tar` & `ufbt-0.2.1rc2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:53:28.441876 ufbt-0.2.1rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-08 22:53:28.441876 ufbt-0.2.1rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-08 22:53:15.000000 ufbt-0.2.1rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-08 22:53:15.000000 ufbt-0.2.1rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 22:53:28.441876 ufbt-0.2.1rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:53:28.441876 ufbt-0.2.1rc1/ufbt/
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-08 22:53:15.000000 ufbt-0.2.1rc1/ufbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-08 22:53:15.000000 ufbt-0.2.1rc1/ufbt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25093 2023-04-08 22:53:15.000000 ufbt-0.2.1rc1/ufbt/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:53:28.441876 ufbt-0.2.1rc1/ufbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-08 22:53:28.000000 ufbt-0.2.1rc1/ufbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-08 22:53:28.000000 ufbt-0.2.1rc1/ufbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 22:53:28.000000 ufbt-0.2.1rc1/ufbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-08 22:53:28.000000 ufbt-0.2.1rc1/ufbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-08 22:53:28.000000 ufbt-0.2.1rc1/ufbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:59:58.982588 ufbt-0.2.1rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-04-09 12:59:47.000000 ufbt-0.2.1rc2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-09 12:59:58.982588 ufbt-0.2.1rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-09 12:59:47.000000 ufbt-0.2.1rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-09 12:59:47.000000 ufbt-0.2.1rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 12:59:58.982588 ufbt-0.2.1rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:59:58.982588 ufbt-0.2.1rc2/ufbt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-09 12:59:47.000000 ufbt-0.2.1rc2/ufbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-09 12:59:47.000000 ufbt-0.2.1rc2/ufbt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25878 2023-04-09 12:59:47.000000 ufbt-0.2.1rc2/ufbt/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:59:58.982588 ufbt-0.2.1rc2/ufbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-09 12:59:58.000000 ufbt-0.2.1rc2/ufbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-09 12:59:58.000000 ufbt-0.2.1rc2/ufbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 12:59:58.000000 ufbt-0.2.1rc2/ufbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-09 12:59:58.000000 ufbt-0.2.1rc2/ufbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 12:59:58.000000 ufbt-0.2.1rc2/ufbt.egg-info/top_level.txt
```

### Comparing `ufbt-0.2.1rc1/PKG-INFO` & `ufbt-0.2.1rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufbt
-Version: 0.2.1rc1
+Version: 0.2.1rc2
 Summary: uFBT - micro Flipper Build Tool. Tool for building and developing applications (.fap) for Flipper Zero and its device family.
 Author-email: "Flipper Devices Inc." <pypi@flipperdevices.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: documentation, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: repository, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: issues, https://github.com/flipperdevices/flipperzero-ufbt/issues
@@ -19,14 +19,15 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
 # uFBT - micro Flipper Build Tool
 
 uFBT is a cross-platform tool for building applications for [Flipper Zero](https://flipperzero.one/). It is a simplified version of [Flipper Build Tool (FBT)](https://github.com/flipperdevices/flipperzero-firmware/blob/dev/documentation/fbt.md).
 
 uFBT enables basic development tasks for Flipper Zero, such as building and debugging applications, flashing firmware, creating VSCode development configurations. It uses prebuilt binaries and libraries, so you don't need to build [the whole firmware](https://github.com/flipperdevices/flipperzero-firmware) to compile and debug your application for Flipper.
```

### Comparing `ufbt-0.2.1rc1/README.md` & `ufbt-0.2.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.1rc1/pyproject.toml` & `ufbt-0.2.1rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.1rc1/ufbt/bootstrap.py` & `ufbt-0.2.1rc2/ufbt/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,25 @@
-###
-# Bootstrap script for uFBT. Deploys SDK and metadata.
-###
+#
+# Bootstrap script for uFBT. Deploys the SDK and metadata.
+# This file is part of uFBT <https://github.com/flipperdevices/flipperzero-ufbt>
+# Copyright (C) 2022-2023 Flipper Devices Inc.
+#
+#     This program is free software: you can redistribute it and/or modify
+#     it under the terms of the GNU General Public License as published by
+#     the Free Software Foundation, either version 3 of the License, or
+#     (at your option) any later version.
+#
+#     This program is distributed in the hope that it will be useful,
+#     but WITHOUT ANY WARRANTY; without even the implied warranty of
+#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#     GNU General Public License for more details.
+#
+#     You should have received a copy of the GNU General Public License
+#     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+#
 
 import argparse
 import enum
 import json
 import logging
 import os
 import re
@@ -698,20 +713,20 @@
             state_data.update({"error": "SDK is not deployed"})
 
         if key := args.status_key:
             if key not in state_data:
                 log.error(f"Unknown status key {key}")
                 return 1
             if args.json:
-                print(json.dumps(state_data[key], indent=4))
+                print(json.dumps(state_data[key]))
             else:
                 print(state_data.get(key, ""))
         else:
             if args.json:
-                print(json.dumps(state_data, indent=4))
+                print(json.dumps(state_data))
             else:
                 for key, value in state_data.items():
                     log.info(f"{self.STATUS_FIELDS[key]:<15} {value}")
 
         return 1 if state_data.get("error") else 0
```

### Comparing `ufbt-0.2.1rc1/ufbt.egg-info/PKG-INFO` & `ufbt-0.2.1rc2/ufbt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufbt
-Version: 0.2.1rc1
+Version: 0.2.1rc2
 Summary: uFBT - micro Flipper Build Tool. Tool for building and developing applications (.fap) for Flipper Zero and its device family.
 Author-email: "Flipper Devices Inc." <pypi@flipperdevices.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: documentation, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: repository, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: issues, https://github.com/flipperdevices/flipperzero-ufbt/issues
@@ -19,14 +19,15 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
 # uFBT - micro Flipper Build Tool
 
 uFBT is a cross-platform tool for building applications for [Flipper Zero](https://flipperzero.one/). It is a simplified version of [Flipper Build Tool (FBT)](https://github.com/flipperdevices/flipperzero-firmware/blob/dev/documentation/fbt.md).
 
 uFBT enables basic development tasks for Flipper Zero, such as building and debugging applications, flashing firmware, creating VSCode development configurations. It uses prebuilt binaries and libraries, so you don't need to build [the whole firmware](https://github.com/flipperdevices/flipperzero-firmware) to compile and debug your application for Flipper.
```

