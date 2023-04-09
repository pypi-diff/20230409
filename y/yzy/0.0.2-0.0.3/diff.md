# Comparing `tmp/yzy-0.0.2.tar.gz` & `tmp/yzy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yzy-0.0.2.tar", last modified: Sun Apr  2 13:06:06 2023, max compression
+gzip compressed data, was "yzy-0.0.3.tar", last modified: Sun Apr  9 03:08:48 2023, max compression
```

## Comparing `yzy-0.0.2.tar` & `yzy-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-04-02 13:06:06.529929 yzy-0.0.2/
--rw-r--r--   0 yzy        (501) staff       (20)     1073 2023-04-02 11:39:35.000000 yzy-0.0.2/LICENSE
--rw-r--r--   0 yzy        (501) staff       (20)      711 2023-04-02 13:06:06.529798 yzy-0.0.2/PKG-INFO
--rw-r--r--   0 yzy        (501) staff       (20)      234 2023-04-02 13:00:34.000000 yzy-0.0.2/README.md
--rw-r--r--   0 yzy        (501) staff       (20)      550 2023-04-02 13:05:47.000000 yzy-0.0.2/pyproject.toml
--rw-r--r--   0 yzy        (501) staff       (20)       38 2023-04-02 13:06:06.529974 yzy-0.0.2/setup.cfg
-drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-04-02 13:06:06.527479 yzy-0.0.2/src/
-drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-04-02 13:06:06.528833 yzy-0.0.2/src/yzy/
--rw-r--r--   0 yzy        (501) staff       (20)        0 2023-04-02 11:41:50.000000 yzy-0.0.2/src/yzy/__init__.py
--rwx------   0 yzy        (501) staff       (20)     3793 2023-04-02 12:34:56.000000 yzy-0.0.2/src/yzy/file2md.py
--rwx------   0 yzy        (501) staff       (20)     2933 2023-03-29 09:30:46.000000 yzy-0.0.2/src/yzy/id2md.py
-drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-04-02 13:06:06.529562 yzy-0.0.2/src/yzy.egg-info/
--rw-r--r--   0 yzy        (501) staff       (20)      711 2023-04-02 13:06:06.000000 yzy-0.0.2/src/yzy.egg-info/PKG-INFO
--rw-r--r--   0 yzy        (501) staff       (20)      212 2023-04-02 13:06:06.000000 yzy-0.0.2/src/yzy.egg-info/SOURCES.txt
--rw-r--r--   0 yzy        (501) staff       (20)        1 2023-04-02 13:06:06.000000 yzy-0.0.2/src/yzy.egg-info/dependency_links.txt
--rw-r--r--   0 yzy        (501) staff       (20)        4 2023-04-02 13:06:06.000000 yzy-0.0.2/src/yzy.egg-info/top_level.txt
+drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-04-09 03:08:48.506116 yzy-0.0.3/
+-rw-r--r--   0 yzy        (501) staff       (20)     1073 2023-04-02 11:39:35.000000 yzy-0.0.3/LICENSE
+-rw-r--r--   0 yzy        (501) staff       (20)      767 2023-04-09 03:08:48.505964 yzy-0.0.3/PKG-INFO
+-rw-r--r--   0 yzy        (501) staff       (20)      288 2023-04-09 03:08:26.000000 yzy-0.0.3/README.md
+-rw-r--r--   0 yzy        (501) staff       (20)      552 2023-04-09 03:07:19.000000 yzy-0.0.3/pyproject.toml
+-rw-r--r--   0 yzy        (501) staff       (20)       38 2023-04-09 03:08:48.506177 yzy-0.0.3/setup.cfg
+drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-04-09 03:08:48.503448 yzy-0.0.3/src/
+drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-04-09 03:08:48.505056 yzy-0.0.3/src/yzy/
+-rw-r--r--   0 yzy        (501) staff       (20)        0 2023-04-02 11:41:50.000000 yzy-0.0.3/src/yzy/__init__.py
+-rwx------   0 yzy        (501) staff       (20)     5697 2023-04-09 03:05:07.000000 yzy-0.0.3/src/yzy/arxiv.py
+-rwx------   0 yzy        (501) staff       (20)     3793 2023-04-02 12:34:56.000000 yzy-0.0.3/src/yzy/file2md.py
+-rwx------   0 yzy        (501) staff       (20)     2933 2023-03-29 09:30:46.000000 yzy-0.0.3/src/yzy/id2md.py
+drwxr-xr-x   0 yzy        (501) staff       (20)        0 2023-04-09 03:08:48.505730 yzy-0.0.3/src/yzy.egg-info/
+-rw-r--r--   0 yzy        (501) staff       (20)      767 2023-04-09 03:08:48.000000 yzy-0.0.3/src/yzy.egg-info/PKG-INFO
+-rw-r--r--   0 yzy        (501) staff       (20)      229 2023-04-09 03:08:48.000000 yzy-0.0.3/src/yzy.egg-info/SOURCES.txt
+-rw-r--r--   0 yzy        (501) staff       (20)        1 2023-04-09 03:08:48.000000 yzy-0.0.3/src/yzy.egg-info/dependency_links.txt
+-rw-r--r--   0 yzy        (501) staff       (20)        4 2023-04-09 03:08:48.000000 yzy-0.0.3/src/yzy.egg-info/top_level.txt
```

### Comparing `yzy-0.0.2/LICENSE` & `yzy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yzy-0.0.2/PKG-INFO` & `yzy-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: yzy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Utils
 Author-email: Zhiyuan Yang <im.crazyang@gmail.com>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://github.com/yzy1996/Python-Code
+Project-URL: Bug Tracker, https://github.com/yzy1996/Python-Code/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -16,17 +16,23 @@
 
 各种工具
 
 
 
 ## Support
 
+- **arxiv.py**: combined
 - **id2md.py**: input arxiv id and then get the markdown format output.
 - **file2md.py**: input foldername containing papers and then get the markdown format output.
 
 ```
 python -m yzy.id2md
+
+python yzy.arxiv.id2md()
 ```
 
 
 
 
+
+
+
```

### Comparing `yzy-0.0.2/pyproject.toml` & `yzy-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yzy"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Zhiyuan Yang", email="im.crazyang@gmail.com" },
 ]
 description = "Utils"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/pypa/sampleproject"
-"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
+"Homepage" = "https://github.com/yzy1996/Python-Code"
+"Bug Tracker" = "https://github.com/yzy1996/Python-Code/issues"
```

### Comparing `yzy-0.0.2/src/yzy/file2md.py` & `yzy-0.0.3/src/yzy/file2md.py`

 * *Files identical despite different names*

### Comparing `yzy-0.0.2/src/yzy/id2md.py` & `yzy-0.0.3/src/yzy/id2md.py`

 * *Files identical despite different names*

### Comparing `yzy-0.0.2/src/yzy.egg-info/PKG-INFO` & `yzy-0.0.3/src/yzy.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: yzy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Utils
 Author-email: Zhiyuan Yang <im.crazyang@gmail.com>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://github.com/yzy1996/Python-Code
+Project-URL: Bug Tracker, https://github.com/yzy1996/Python-Code/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -16,17 +16,23 @@
 
 各种工具
 
 
 
 ## Support
 
+- **arxiv.py**: combined
 - **id2md.py**: input arxiv id and then get the markdown format output.
 - **file2md.py**: input foldername containing papers and then get the markdown format output.
 
 ```
 python -m yzy.id2md
+
+python yzy.arxiv.id2md()
 ```
 
 
 
 
+
+
+
```

