# Comparing `tmp/tklinenums-1.6.tar.gz` & `tmp/tklinenums-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tklinenums-1.6.tar", last modified: Fri Apr  7 19:01:06 2023, max compression
+gzip compressed data, was "tklinenums-1.6.1.tar", last modified: Sun Apr  9 18:21:48 2023, max compression
```

## Comparing `tklinenums-1.6.tar` & `tklinenums-1.6.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:01:06.550646 tklinenums-1.6/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-07 19:01:06.550646 tklinenums-1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-07 19:00:50.000000 tklinenums-1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 19:01:06.550646 tklinenums-1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-07 19:00:50.000000 tklinenums-1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:01:06.546646 tklinenums-1.6/tklinenums/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 19:00:50.000000 tklinenums-1.6/tklinenums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-04-07 19:00:50.000000 tklinenums-1.6/tklinenums/tklinenums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 19:01:06.550646 tklinenums-1.6/tklinenums.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-07 19:01:06.000000 tklinenums-1.6/tklinenums.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-07 19:01:06.000000 tklinenums-1.6/tklinenums.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 19:01:06.000000 tklinenums-1.6/tklinenums.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-07 19:01:06.000000 tklinenums-1.6/tklinenums.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:48.515345 tklinenums-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-09 18:21:48.515345 tklinenums-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-09 18:21:29.000000 tklinenums-1.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 18:21:48.515345 tklinenums-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-09 18:21:29.000000 tklinenums-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:48.511345 tklinenums-1.6.1/tklinenums/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 18:21:29.000000 tklinenums-1.6.1/tklinenums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10852 2023-04-09 18:21:29.000000 tklinenums-1.6.1/tklinenums/tklinenums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:21:48.511345 tklinenums-1.6.1/tklinenums.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-09 18:21:48.000000 tklinenums-1.6.1/tklinenums.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-09 18:21:48.000000 tklinenums-1.6.1/tklinenums.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 18:21:48.000000 tklinenums-1.6.1/tklinenums.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 18:21:48.000000 tklinenums-1.6.1/tklinenums.egg-info/top_level.txt
```

### Comparing `tklinenums-1.6/PKG-INFO` & `tklinenums-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: tklinenums
-Version: 1.6
+Version: 1.6.1
 Summary: A simple Tkinter widget for displaying line numbers
 Home-page: https://github.com/Moosems/TkLineNums
 Author: Moosems
 Author-email: moosems.j@gmail.com
 Description-Content-Type: text/markdown
 
-# TkLineNums V.1.6
+# TkLineNums V.1.6.1
 
 TkLineNums is a simple line numbering widget for Tkinter. It supports ttk themes through the set_to_ttk_style method.
 
 ![img](https://github.com/Moosems/TkLineNums/raw/main/images/TkLineNumsPhoto.png)
 
 ## Features
```

### Comparing `tklinenums-1.6/README.md` & `tklinenums-1.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# TkLineNums V.1.6
+# TkLineNums V.1.6.1
 
 TkLineNums is a simple line numbering widget for Tkinter. It supports ttk themes through the set_to_ttk_style method.
 
 ![img](https://github.com/Moosems/TkLineNums/raw/main/images/TkLineNumsPhoto.png)
 
 ## Features
```

### Comparing `tklinenums-1.6/tklinenums/tklinenums.py` & `tklinenums-1.6.1/tklinenums/tklinenums.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,15 @@
 
     def set_font(self, font: tuple | Font | str | None) -> None:
         """Sets the font of the widget"""
         if isinstance(font, Font):
             self.font: Font = font
         elif isinstance(font, tuple):
             self.font: Font = Font(family=font[0], size=font[1])
-        elif isinstance(font, str):
+        elif isinstance(font, str) and not font.startswith("{"):
             self.font: Font = Font(name=font, exists=True)
         else:
             self.font: Font = Font(
                 family=" ".join(
                     (
                         font := self.textwidget["font"]
                         .replace("{", "")
```

### Comparing `tklinenums-1.6/tklinenums.egg-info/PKG-INFO` & `tklinenums-1.6.1/tklinenums.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: tklinenums
-Version: 1.6
+Version: 1.6.1
 Summary: A simple Tkinter widget for displaying line numbers
 Home-page: https://github.com/Moosems/TkLineNums
 Author: Moosems
 Author-email: moosems.j@gmail.com
 Description-Content-Type: text/markdown
 
-# TkLineNums V.1.6
+# TkLineNums V.1.6.1
 
 TkLineNums is a simple line numbering widget for Tkinter. It supports ttk themes through the set_to_ttk_style method.
 
 ![img](https://github.com/Moosems/TkLineNums/raw/main/images/TkLineNumsPhoto.png)
 
 ## Features
```

