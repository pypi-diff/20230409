# Comparing `tmp/Colors and Styles-1.0.0.tar.gz` & `tmp/Colors and Styles-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Colors and Styles-1.0.0.tar", last modified: Sun Apr  9 01:45:06 2023, max compression
+gzip compressed data, was "Colors and Styles-1.0.1.tar", last modified: Sun Apr  9 01:53:16 2023, max compression
```

## Comparing `Colors and Styles-1.0.0.tar` & `Colors and Styles-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-09 01:45:06.876901 Colors and Styles-1.0.0/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-09 01:45:06.864901 Colors and Styles-1.0.0/Colors-and-Styles/
--rw-r--r--   0 runner    (1000) runner    (1000)      158 2023-04-09 01:14:49.000000 Colors and Styles-1.0.0/Colors-and-Styles/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2625 2023-04-09 01:14:27.000000 Colors and Styles-1.0.0/Colors-and-Styles/color.py
--rw-r--r--   0 runner    (1000) runner    (1000)      460 2023-04-09 01:14:39.000000 Colors and Styles-1.0.0/Colors-and-Styles/style.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-09 01:45:06.872901 Colors and Styles-1.0.0/Colors_and_Styles.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     3076 2023-04-09 01:45:06.000000 Colors and Styles-1.0.0/Colors_and_Styles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      293 2023-04-09 01:45:06.000000 Colors and Styles-1.0.0/Colors_and_Styles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-09 01:45:06.000000 Colors and Styles-1.0.0/Colors_and_Styles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-09 01:45:06.000000 Colors and Styles-1.0.0/Colors_and_Styles.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     1069 2023-04-09 01:17:29.000000 Colors and Styles-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1000) runner    (1000)     3076 2023-04-09 01:45:06.872901 Colors and Styles-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     2365 2023-04-09 01:32:38.000000 Colors and Styles-1.0.0/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      473 2023-01-20 17:56:39.000000 Colors and Styles-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-09 01:45:06.876901 Colors and Styles-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      890 2023-04-09 01:37:24.000000 Colors and Styles-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-09 01:53:16.852119 Colors and Styles-1.0.1/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-09 01:53:16.848119 Colors and Styles-1.0.1/Colors-and-Styles/
+-rw-r--r--   0 runner    (1000) runner    (1000)      158 2023-04-09 01:14:49.000000 Colors and Styles-1.0.1/Colors-and-Styles/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2625 2023-04-09 01:14:27.000000 Colors and Styles-1.0.1/Colors-and-Styles/color.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      460 2023-04-09 01:14:39.000000 Colors and Styles-1.0.1/Colors-and-Styles/style.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-09 01:53:16.848119 Colors and Styles-1.0.1/Colors_and_Styles.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3155 2023-04-09 01:53:16.000000 Colors and Styles-1.0.1/Colors_and_Styles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      293 2023-04-09 01:53:16.000000 Colors and Styles-1.0.1/Colors_and_Styles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-09 01:53:16.000000 Colors and Styles-1.0.1/Colors_and_Styles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       18 2023-04-09 01:53:16.000000 Colors and Styles-1.0.1/Colors_and_Styles.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     1069 2023-04-09 01:17:29.000000 Colors and Styles-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)     3155 2023-04-09 01:53:16.848119 Colors and Styles-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     2365 2023-04-09 01:32:38.000000 Colors and Styles-1.0.1/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      473 2023-01-20 17:56:39.000000 Colors and Styles-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-09 01:53:16.852119 Colors and Styles-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      890 2023-04-09 01:52:25.000000 Colors and Styles-1.0.1/setup.py
```

### Comparing `Colors and Styles-1.0.0/Colors-and-Styles/color.py` & `Colors and Styles-1.0.1/Colors-and-Styles/color.py`

 * *Files identical despite different names*

### Comparing `Colors and Styles-1.0.0/Colors_and_Styles.egg-info/PKG-INFO` & `Colors and Styles-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Colors-and-Styles
-Version: 1.0.0
+Name: Colors and Styles
+Version: 1.0.1
 Summary: A basic package that makes it easy to add color and styles to your terminal.
 Author: QwertyQwerty
 Author-email: personqwertyperson88@gmail.com
 License: MIT
 Keywords: color,style,ansi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -63,10 +63,14 @@
 ```python
 print(f"{Style.BOLD}This text is bold.{Style.RESET}")
 ```
 
 
 # Change Log
 
-## 0.0.1 (4/8/2023)
+## 1.0.1 (4/8/2023)
+
+- Really really small update that does nothing important
+
+## 1.0.0 (4/8/2023)
 
 - First release
```

### Comparing `Colors and Styles-1.0.0/LICENSE.txt` & `Colors and Styles-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Colors and Styles-1.0.0/PKG-INFO` & `Colors and Styles-1.0.1/Colors_and_Styles.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Colors and Styles
-Version: 1.0.0
+Name: Colors-and-Styles
+Version: 1.0.1
 Summary: A basic package that makes it easy to add color and styles to your terminal.
 Author: QwertyQwerty
 Author-email: personqwertyperson88@gmail.com
 License: MIT
 Keywords: color,style,ansi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -63,10 +63,14 @@
 ```python
 print(f"{Style.BOLD}This text is bold.{Style.RESET}")
 ```
 
 
 # Change Log
 
-## 0.0.1 (4/8/2023)
+## 1.0.1 (4/8/2023)
+
+- Really really small update that does nothing important
+
+## 1.0.0 (4/8/2023)
 
 - First release
```

### Comparing `Colors and Styles-1.0.0/README.md` & `Colors and Styles-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `Colors and Styles-1.0.0/setup.py` & `Colors and Styles-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Colors and Styles',
-    version='1.0.0',
+    version='1.0.1',
     description='A basic package that makes it easy to add color and styles to your terminal.',
     long_description_content_type="text/markdown",
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.md').read(),
     author='QwertyQwerty',
     author_email='personqwertyperson88@gmail.com',
     license='MIT', 
     keywords=['color', 'style', 'ansi'],
```

