# Comparing `tmp/picorm-0.1.1.tar.gz` & `tmp/picorm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picorm-0.1.1.tar", last modified: Sun Mar 19 15:32:09 2023, max compression
+gzip compressed data, was "picorm-0.1.4.tar", last modified: Sun Apr  9 14:53:54 2023, max compression
```

## Comparing `picorm-0.1.1.tar` & `picorm-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:32:09.674717 picorm-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-03-19 15:32:01.000000 picorm-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-03-19 15:32:09.674717 picorm-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-03-19 15:32:01.000000 picorm-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:32:09.674717 picorm-0.1.1/picorm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:32:09.674717 picorm-0.1.1/picorm/picorm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-03-19 15:32:09.000000 picorm-0.1.1/picorm/picorm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-19 15:32:09.000000 picorm-0.1.1/picorm/picorm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 15:32:09.000000 picorm-0.1.1/picorm/picorm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-19 15:32:09.000000 picorm-0.1.1/picorm/picorm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 15:32:09.674717 picorm-0.1.1/picorm/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 15:32:01.000000 picorm-0.1.1/picorm/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-03-19 15:32:01.000000 picorm-0.1.1/picorm/tests/test_storages.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 15:32:09.674717 picorm-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-03-19 15:32:01.000000 picorm-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:53:54.227563 picorm-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-09 14:53:43.000000 picorm-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-04-09 14:53:54.223563 picorm-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-04-09 14:53:43.000000 picorm-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:53:54.223563 picorm-0.1.4/picorm/
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-09 14:53:43.000000 picorm-0.1.4/picorm/FileStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-09 14:53:43.000000 picorm-0.1.4/picorm/SQLiteStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-09 14:53:43.000000 picorm-0.1.4/picorm/Storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-09 14:53:43.000000 picorm-0.1.4/picorm/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-09 14:53:43.000000 picorm-0.1.4/picorm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:53:54.223563 picorm-0.1.4/picorm/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 14:53:43.000000 picorm-0.1.4/picorm/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-04-09 14:53:43.000000 picorm-0.1.4/picorm/tests/test_storages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-09 14:53:43.000000 picorm-0.1.4/picorm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:53:54.223563 picorm-0.1.4/picorm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-04-09 14:53:54.000000 picorm-0.1.4/picorm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-09 14:53:54.000000 picorm-0.1.4/picorm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:53:54.000000 picorm-0.1.4/picorm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-09 14:53:54.000000 picorm-0.1.4/picorm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 14:53:54.227563 picorm-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-09 14:53:43.000000 picorm-0.1.4/setup.py
```

### Comparing `picorm-0.1.1/LICENSE` & `picorm-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `picorm-0.1.1/PKG-INFO` & `picorm-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picorm
-Version: 0.1.1
+Version: 0.1.4
 Summary: Small ORM with limited functions for multiple database engines for pet-projects
 Home-page: https://github.com/k5md/picorm
 Author: k5md
 Author-email: k-5md@yandex.ru
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/k5md/picorm/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `picorm-0.1.1/README.md` & `picorm-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `picorm-0.1.1/picorm/picorm.egg-info/PKG-INFO` & `picorm-0.1.4/picorm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picorm
-Version: 0.1.1
+Version: 0.1.4
 Summary: Small ORM with limited functions for multiple database engines for pet-projects
 Home-page: https://github.com/k5md/picorm
 Author: k5md
 Author-email: k-5md@yandex.ru
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/k5md/picorm/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `picorm-0.1.1/picorm/tests/test_storages.py` & `picorm-0.1.4/picorm/tests/test_storages.py`

 * *Files identical despite different names*

### Comparing `picorm-0.1.1/setup.py` & `picorm-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,13 @@
         "License :: OSI Approved :: %s" % __license__,
         "Operating System :: Microsoft :: Windows",
         "Operating System :: Unix",
         "Topic :: Utilities",
         "Topic :: Database",
         "Topic :: Database :: Front-Ends",
     ],
-    package_dir = { "": "picorm" },
-    packages = setuptools.find_packages(
-        where="picorm",
-    ),
+    package_dir = { ".": "picorm" },
+    packages = setuptools.find_packages(),
     python_requires = ">=3.7",
     install_requires=[],
     include_package_data = True,
 )
```

