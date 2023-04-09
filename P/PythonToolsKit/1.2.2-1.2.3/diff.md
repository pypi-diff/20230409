# Comparing `tmp/PythonToolsKit-1.2.2.tar.gz` & `tmp/PythonToolsKit-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonToolsKit-1.2.2.tar", last modified: Thu Feb  2 18:51:19 2023, max compression
+gzip compressed data, was "PythonToolsKit-1.2.3.tar", last modified: Sun Apr  9 12:17:42 2023, max compression
```

## Comparing `PythonToolsKit-1.2.2.tar` & `PythonToolsKit-1.2.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-02 18:51:19.925362 PythonToolsKit-1.2.2/
--rw-r--r--   0 kali      (1000) kali      (1000)    35149 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/LICENSE.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       27 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)    15504 2023-02-02 18:51:19.925362 PythonToolsKit-1.2.2/PKG-INFO
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-02 18:51:19.925362 PythonToolsKit-1.2.2/PythonToolsKit/
--rw-r--r--   0 kali      (1000) kali      (1000)    14047 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/Arguments.py
--rw-r--r--   0 kali      (1000) kali      (1000)     8544 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/Characters.py
--rw-r--r--   0 kali      (1000) kali      (1000)    27309 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/Colors.py
--rw-r--r--   0 kali      (1000) kali      (1000)    42825 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/DataAnalysis.py
--rwxr-x---   0 kali      (1000) kali      (1000)    18433 2023-02-02 18:17:36.000000 PythonToolsKit-1.2.2/PythonToolsKit/DebugEncoding.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5865 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/Dict.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4454 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/DictObject.py
--rw-r--r--   0 kali      (1000) kali      (1000)    11285 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/Encodings.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2665 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/Function.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3705 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/GetFile.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3814 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/GetPass.py
--rw-r--r--   0 kali      (1000) kali      (1000)    19640 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/GetType.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2404 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/Import.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5264 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/Json.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3237 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/List.py
--rw-r--r--   0 kali      (1000) kali      (1000)     8596 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/Logs.py
--rw-r--r--   0 kali      (1000) kali      (1000)    16573 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/OrdDict.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5353 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/PrintF.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3394 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/Process.py
--rw-r--r--   0 kali      (1000) kali      (1000)     6193 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/Random.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2490 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/RecursionDebug.py
--rw-r--r--   0 kali      (1000) kali      (1000)    18332 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/Report.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4888 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/ScapyTools.py
--rw-r--r--   0 kali      (1000) kali      (1000)     7137 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/StringF.py
--rw-r--r--   0 kali      (1000) kali      (1000)    15551 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/Terminal.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1106 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/TestArguments.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4712 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/TestTimeout.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3098 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/Thread.py
--rw-r--r--   0 kali      (1000) kali      (1000)     7868 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/Timeout.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3264 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/Tuple.py
--rw-r--r--   0 kali      (1000) kali      (1000)    10022 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/WindowsTerminal.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1641 2023-02-02 18:51:14.000000 PythonToolsKit-1.2.2/PythonToolsKit/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5949 2023-01-02 14:42:11.000000 PythonToolsKit-1.2.2/PythonToolsKit/urlopen.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-02-02 18:51:19.925362 PythonToolsKit-1.2.2/PythonToolsKit.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)    15504 2023-02-02 18:51:19.000000 PythonToolsKit-1.2.2/PythonToolsKit.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1135 2023-02-02 18:51:19.000000 PythonToolsKit-1.2.2/PythonToolsKit.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-02-02 18:51:19.000000 PythonToolsKit-1.2.2/PythonToolsKit.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      112 2023-02-02 18:51:19.000000 PythonToolsKit-1.2.2/PythonToolsKit.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-02-02 18:51:19.000000 PythonToolsKit-1.2.2/PythonToolsKit.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)    10968 2023-02-02 18:41:01.000000 PythonToolsKit-1.2.2/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-02-02 18:51:19.925362 PythonToolsKit-1.2.2/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     6693 2023-02-02 18:28:03.000000 PythonToolsKit-1.2.2/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-09 12:17:42.365424 PythonToolsKit-1.2.3/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35149 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/LICENSE.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       27 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)    15504 2023-04-09 12:17:42.365424 PythonToolsKit-1.2.3/PKG-INFO
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-09 12:17:42.365424 PythonToolsKit-1.2.3/PythonToolsKit/
+-rw-r--r--   0 kali      (1000) kali      (1000)    14047 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Arguments.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     8544 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Characters.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    27309 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Colors.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    43063 2023-04-09 12:17:05.000000 PythonToolsKit-1.2.3/PythonToolsKit/DataAnalysis.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    18433 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/DebugEncoding.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5865 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Dict.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4454 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/DictObject.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    11285 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Encodings.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2665 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Function.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3705 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/GetFile.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3814 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/GetPass.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    19640 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/GetType.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2404 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Import.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5264 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Json.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3237 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/List.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     8596 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Logs.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    16573 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/OrdDict.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5353 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/PrintF.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3394 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Process.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     6193 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Random.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2490 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/RecursionDebug.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    18332 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Report.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4888 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/ScapyTools.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     7137 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/StringF.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    15551 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Terminal.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1106 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/TestArguments.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4712 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/TestTimeout.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3098 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Thread.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     7868 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Timeout.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3264 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/Tuple.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    10022 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/WindowsTerminal.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1641 2023-04-09 12:16:27.000000 PythonToolsKit-1.2.3/PythonToolsKit/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5949 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/PythonToolsKit/urlopen.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-09 12:17:42.365424 PythonToolsKit-1.2.3/PythonToolsKit.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)    15504 2023-04-09 12:17:42.000000 PythonToolsKit-1.2.3/PythonToolsKit.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     1135 2023-04-09 12:17:42.000000 PythonToolsKit-1.2.3/PythonToolsKit.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-09 12:17:42.000000 PythonToolsKit-1.2.3/PythonToolsKit.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      112 2023-04-09 12:17:42.000000 PythonToolsKit-1.2.3/PythonToolsKit.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-04-09 12:17:42.000000 PythonToolsKit-1.2.3/PythonToolsKit.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)    10968 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-09 12:17:42.365424 PythonToolsKit-1.2.3/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     6693 2023-04-09 11:42:16.000000 PythonToolsKit-1.2.3/setup.py
```

### Comparing `PythonToolsKit-1.2.2/LICENSE.txt` & `PythonToolsKit-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PKG-INFO` & `PythonToolsKit-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToolsKit
-Version: 1.2.2
+Version: 1.2.3
 Summary: This package implements tools to build python package and tools.
 Home-page: https://github.com/mauricelambert/PythonToolsKit
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/Arguments.py` & `PythonToolsKit-1.2.3/PythonToolsKit/Arguments.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/Characters.py` & `PythonToolsKit-1.2.3/PythonToolsKit/Characters.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/Colors.py` & `PythonToolsKit-1.2.3/PythonToolsKit/Colors.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/DataAnalysis.py` & `PythonToolsKit-1.2.3/PythonToolsKit/DataAnalysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 ###################
 #    This package implements tools to build python package and tools.
-#    Copyright (C) 2022  Maurice Lambert
+#    Copyright (C) 2022, 2023  Maurice Lambert
 
 #    This program is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
 #    (at your option) any later version.
 
 #    This program is distributed in the hope that it will be useful,
@@ -367,15 +367,15 @@
 __description__ = """
 This package implements tools to build python package and tools.
 """
 license = "GPL-3.0 License"
 __url__ = "https://github.com/mauricelambert/PythonToolsKit"
 
 copyright = """
-PythonToolsKit  Copyright (C) 2022  Maurice Lambert
+PythonToolsKit  Copyright (C) 2022, 2023  Maurice Lambert
 This program comes with ABSOLUTELY NO WARRANTY.
 This is free software, and you are welcome to redistribute it
 under certain conditions.
 """
 __license__ = license
 __copyright__ = copyright
 
@@ -1327,15 +1327,19 @@
             values,
             *args,
             color=color,
             tick_label=keys,
             **kwargs,
         )
         title(chart_title)
-        plot.get_figure().canvas.parent().setWindowTitle("DataAnalysis chart")
+        canvas = plot.get_figure().canvas
+        if get_parent := getattr(canvas, "parent", None):
+            get_parent().setWindowTitle("DataAnalysis chart - " + argv[0])
+        elif manager := getattr(canvas, "manager", None):
+            manager.window.title("DataAnalysis chart - " + argv[0])
         show()
 
 
 if not PYPLOT:
     del DataAnalysis.statistictypes_chart
     del DataAnalysis.show_chart
     del DataAnalysis.valuetypes_counters_chart
```

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/DebugEncoding.py` & `PythonToolsKit-1.2.3/PythonToolsKit/DebugEncoding.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/Dict.py` & `PythonToolsKit-1.2.3/PythonToolsKit/Dict.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/DictObject.py` & `PythonToolsKit-1.2.3/PythonToolsKit/DictObject.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/Encodings.py` & `PythonToolsKit-1.2.3/PythonToolsKit/Encodings.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/Function.py` & `PythonToolsKit-1.2.3/PythonToolsKit/Function.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/GetFile.py` & `PythonToolsKit-1.2.3/PythonToolsKit/GetFile.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/GetPass.py` & `PythonToolsKit-1.2.3/PythonToolsKit/GetPass.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/GetType.py` & `PythonToolsKit-1.2.3/PythonToolsKit/GetType.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/Import.py` & `PythonToolsKit-1.2.3/PythonToolsKit/Import.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/Json.py` & `PythonToolsKit-1.2.3/PythonToolsKit/Json.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/List.py` & `PythonToolsKit-1.2.3/PythonToolsKit/List.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/Logs.py` & `PythonToolsKit-1.2.3/PythonToolsKit/Logs.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/OrdDict.py` & `PythonToolsKit-1.2.3/PythonToolsKit/OrdDict.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/PrintF.py` & `PythonToolsKit-1.2.3/PythonToolsKit/PrintF.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/Process.py` & `PythonToolsKit-1.2.3/PythonToolsKit/Process.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/Random.py` & `PythonToolsKit-1.2.3/PythonToolsKit/Random.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/RecursionDebug.py` & `PythonToolsKit-1.2.3/PythonToolsKit/RecursionDebug.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/Report.py` & `PythonToolsKit-1.2.3/PythonToolsKit/Report.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/ScapyTools.py` & `PythonToolsKit-1.2.3/PythonToolsKit/ScapyTools.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/StringF.py` & `PythonToolsKit-1.2.3/PythonToolsKit/StringF.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/Terminal.py` & `PythonToolsKit-1.2.3/PythonToolsKit/Terminal.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/TestArguments.py` & `PythonToolsKit-1.2.3/PythonToolsKit/TestArguments.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/TestTimeout.py` & `PythonToolsKit-1.2.3/PythonToolsKit/TestTimeout.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/Thread.py` & `PythonToolsKit-1.2.3/PythonToolsKit/Thread.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/Timeout.py` & `PythonToolsKit-1.2.3/PythonToolsKit/Timeout.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/Tuple.py` & `PythonToolsKit-1.2.3/PythonToolsKit/Tuple.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/WindowsTerminal.py` & `PythonToolsKit-1.2.3/PythonToolsKit/WindowsTerminal.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/__init__.py` & `PythonToolsKit-1.2.3/PythonToolsKit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ###################
 
 """
 This package implements tools to build python package and tools.
 """
 
-__version__ = "1.2.2"
+__version__ = "1.2.3"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements tools to build python package and tools.
 """
```

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit/urlopen.py` & `PythonToolsKit-1.2.3/PythonToolsKit/urlopen.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit.egg-info/PKG-INFO` & `PythonToolsKit-1.2.3/PythonToolsKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToolsKit
-Version: 1.2.2
+Version: 1.2.3
 Summary: This package implements tools to build python package and tools.
 Home-page: https://github.com/mauricelambert/PythonToolsKit
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `PythonToolsKit-1.2.2/PythonToolsKit.egg-info/SOURCES.txt` & `PythonToolsKit-1.2.3/PythonToolsKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/README.md` & `PythonToolsKit-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.2/setup.py` & `PythonToolsKit-1.2.3/setup.py`

 * *Files identical despite different names*

