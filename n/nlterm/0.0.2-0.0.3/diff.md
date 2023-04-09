# Comparing `tmp/nlterm-0.0.2.tar.gz` & `tmp/nlterm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlterm-0.0.2.tar", last modified: Sun Apr  9 05:55:04 2023, max compression
+gzip compressed data, was "nlterm-0.0.3.tar", last modified: Sun Apr  9 06:03:02 2023, max compression
```

## Comparing `nlterm-0.0.2.tar` & `nlterm-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-09 05:55:04.294525 nlterm-0.0.2/
--rw-r--r--   0 tom       (1000) tom       (1000)      657 2023-04-09 05:55:04.294525 nlterm-0.0.2/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      354 2023-04-09 05:44:20.000000 nlterm-0.0.2/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-09 05:55:04.294525 nlterm-0.0.2/nlterm/
--rw-r--r--   0 tom       (1000) tom       (1000)       55 2023-04-09 05:36:57.000000 nlterm-0.0.2/nlterm/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3666 2023-04-09 05:50:41.000000 nlterm-0.0.2/nlterm/lib.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-09 05:55:04.294525 nlterm-0.0.2/nlterm.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)      657 2023-04-09 05:55:04.000000 nlterm-0.0.2/nlterm.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)      239 2023-04-09 05:55:04.000000 nlterm-0.0.2/nlterm.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-04-09 05:55:04.000000 nlterm-0.0.2/nlterm.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       39 2023-04-09 05:55:04.000000 nlterm-0.0.2/nlterm.egg-info/entry_points.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        7 2023-04-09 05:55:04.000000 nlterm-0.0.2/nlterm.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        7 2023-04-09 05:55:04.000000 nlterm-0.0.2/nlterm.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)      388 2023-04-09 05:54:36.000000 nlterm-0.0.2/pyproject.toml
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-04-09 05:55:04.294525 nlterm-0.0.2/setup.cfg
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-09 06:03:02.284502 nlterm-0.0.3/
+-rw-r--r--   0 tom       (1000) tom       (1000)      832 2023-04-09 06:03:02.284502 nlterm-0.0.3/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      529 2023-04-09 05:58:01.000000 nlterm-0.0.3/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-09 06:03:02.284502 nlterm-0.0.3/nlterm/
+-rw-r--r--   0 tom       (1000) tom       (1000)       55 2023-04-09 05:36:57.000000 nlterm-0.0.3/nlterm/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3686 2023-04-09 06:01:47.000000 nlterm-0.0.3/nlterm/lib.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-09 06:03:02.284502 nlterm-0.0.3/nlterm.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)      832 2023-04-09 06:03:02.000000 nlterm-0.0.3/nlterm.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)      239 2023-04-09 06:03:02.000000 nlterm-0.0.3/nlterm.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-04-09 06:03:02.000000 nlterm-0.0.3/nlterm.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       39 2023-04-09 06:03:02.000000 nlterm-0.0.3/nlterm.egg-info/entry_points.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       16 2023-04-09 06:03:02.000000 nlterm-0.0.3/nlterm.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        7 2023-04-09 06:03:02.000000 nlterm-0.0.3/nlterm.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)      400 2023-04-09 06:02:25.000000 nlterm-0.0.3/pyproject.toml
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-04-09 06:03:02.284502 nlterm-0.0.3/setup.cfg
```

### Comparing `nlterm-0.0.2/PKG-INFO` & `nlterm-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlterm
-Version: 0.0.2
+Version: 0.0.3
 Summary: Terminal with ChatGPT integration
 Author-email: Tom Shen <me@tomshen.io>
 Project-URL: homepage, https://github.com/tsunrise/nlterm
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
@@ -13,20 +13,35 @@
 # Install
 ```
 pip install nlterm
 ```
 
 # Example
 
+- Example 1
 ````
 > nlterm
 Instruction: reorgnize this folder to like a pypi project. That is I need to put scripts in `src` folder, and have a basic `pyproject.toml`
 ````
 This is the output:
 ````
 ```
 mkdir src
 mv *.py src
 touch pyproject.toml
 ```
-Execute? (y/n): y
+Execute? (y/n): 
+````
+
+- Example 2
+````
+> nlterm
+Instruction: Install the whl file
+````
+
+This is the output:
+````
+```
+pip install nlterm-0.0.2-py3-none-any.whl
+```
+Execute? (y/n): 
 ````
```

### Comparing `nlterm-0.0.2/nlterm/lib.py` & `nlterm-0.0.3/nlterm/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,17 @@
         ls.extend(files)
     return ls
 
 def get_os():
     """
     Get the OS name.
     """
-    return os.uname().sysname
+    import platform
+    return platform.system()
+
 
 def get_username():
     """
     Get the username.
     """
     return os.environ.get("USER")
```

### Comparing `nlterm-0.0.2/nlterm.egg-info/PKG-INFO` & `nlterm-0.0.3/nlterm.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlterm
-Version: 0.0.2
+Version: 0.0.3
 Summary: Terminal with ChatGPT integration
 Author-email: Tom Shen <me@tomshen.io>
 Project-URL: homepage, https://github.com/tsunrise/nlterm
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
@@ -13,20 +13,35 @@
 # Install
 ```
 pip install nlterm
 ```
 
 # Example
 
+- Example 1
 ````
 > nlterm
 Instruction: reorgnize this folder to like a pypi project. That is I need to put scripts in `src` folder, and have a basic `pyproject.toml`
 ````
 This is the output:
 ````
 ```
 mkdir src
 mv *.py src
 touch pyproject.toml
 ```
-Execute? (y/n): y
+Execute? (y/n): 
+````
+
+- Example 2
+````
+> nlterm
+Instruction: Install the whl file
+````
+
+This is the output:
+````
+```
+pip install nlterm-0.0.2-py3-none-any.whl
+```
+Execute? (y/n): 
 ````
```

