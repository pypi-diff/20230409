# Comparing `tmp/dankware-3.3.3.tar.gz` & `tmp/dankware-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dankware-3.3.3.tar", last modified: Sat Apr  8 09:44:45 2023, max compression
+gzip compressed data, was "dankware-3.3.4.tar", last modified: Sun Apr  9 09:25:53 2023, max compression
```

## Comparing `dankware-3.3.3.tar` & `dankware-3.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 09:44:45.517176 dankware-3.3.3/
--rw-rw-rw-   0        0        0     1085 2023-02-11 12:53:16.000000 dankware-3.3.3/LICENSE
--rw-rw-rw-   0        0        0    14097 2023-04-08 09:44:45.516178 dankware-3.3.3/PKG-INFO
--rw-rw-rw-   0        0        0    13217 2023-03-29 08:26:24.000000 dankware-3.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 09:44:45.510667 dankware-3.3.3/dankware/
--rw-rw-rw-   0        0        0    46578 2023-04-08 09:43:25.000000 dankware-3.3.3/dankware/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 09:44:45.515178 dankware-3.3.3/dankware.egg-info/
--rw-rw-rw-   0        0        0    14097 2023-04-08 09:44:45.000000 dankware-3.3.3/dankware.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-04-08 09:44:45.000000 dankware-3.3.3/dankware.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 09:44:45.000000 dankware-3.3.3/dankware.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-08 09:44:45.000000 dankware-3.3.3/dankware.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-08 09:44:45.000000 dankware-3.3.3/dankware.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 09:44:45.517176 dankware-3.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1132 2023-04-08 09:43:46.000000 dankware-3.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 09:25:53.121963 dankware-3.3.4/
+-rw-rw-rw-   0        0        0     1085 2023-02-11 12:53:16.000000 dankware-3.3.4/LICENSE
+-rw-rw-rw-   0        0        0    14134 2023-04-09 09:25:53.119362 dankware-3.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    13217 2023-03-29 08:26:24.000000 dankware-3.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 09:25:53.114362 dankware-3.3.4/dankware/
+-rw-rw-rw-   0        0        0    46597 2023-04-09 09:00:17.000000 dankware-3.3.4/dankware/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 09:25:53.119362 dankware-3.3.4/dankware.egg-info/
+-rw-rw-rw-   0        0        0    14134 2023-04-09 09:25:53.000000 dankware-3.3.4/dankware.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-04-09 09:25:53.000000 dankware-3.3.4/dankware.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 09:25:53.000000 dankware-3.3.4/dankware.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-09 09:25:53.000000 dankware-3.3.4/dankware.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-09 09:25:53.000000 dankware-3.3.4/dankware.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 09:25:53.121963 dankware-3.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1478 2023-04-09 09:10:13.000000 dankware-3.3.4/setup.py
```

### Comparing `dankware-3.3.3/LICENSE` & `dankware-3.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dankware-3.3.3/PKG-INFO` & `dankware-3.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: dankware
-Version: 3.3.3
-Summary: Python module with various features.
+Version: 3.3.4
+Summary: Python package with various features!
 Home-page: https://github.com/SirDank/dankware
 Author: SirDank
 Author-email: SirDankenstein@protonmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/SirDank/dankware
 Project-URL: Bug Tracker, https://github.com/SirDank/dankware/issues
-Keywords: dank,dankware,multithread,gradient,fade,registry key,error traceback,random ip,github scraper,splash screen
+Keywords: dank,dankware,multithread,gradient,fade,registry key,error traceback,random ip generator,github scraper,splash screen,hide window,file selector
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development
```

### Comparing `dankware-3.3.3/README.md` & `dankware-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `dankware-3.3.3/dankware/__init__.py` & `dankware-3.3.4/dankware/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -824,15 +824,15 @@
     from tkinter import Tk
     from tkinter.filedialog import askopenfilename
 
     root = Tk()
     root.withdraw()
     if icon_path: root.iconbitmap(icon_path)
     file_path = askopenfilename(title=title)
-    return file_path
+    return file_path.replace("/", "\\")
 
 # --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def cls() -> None: 
     
     """
     Clear screen for multi-os
```

### Comparing `dankware-3.3.3/dankware.egg-info/PKG-INFO` & `dankware-3.3.4/dankware.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: dankware
-Version: 3.3.3
-Summary: Python module with various features.
+Version: 3.3.4
+Summary: Python package with various features!
 Home-page: https://github.com/SirDank/dankware
 Author: SirDank
 Author-email: SirDankenstein@protonmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/SirDank/dankware
 Project-URL: Bug Tracker, https://github.com/SirDank/dankware/issues
-Keywords: dank,dankware,multithread,gradient,fade,registry key,error traceback,random ip,github scraper,splash screen
+Keywords: dank,dankware,multithread,gradient,fade,registry key,error traceback,random ip generator,github scraper,splash screen,hide window,file selector
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development
```

