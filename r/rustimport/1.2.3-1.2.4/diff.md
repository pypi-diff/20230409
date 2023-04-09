# Comparing `tmp/rustimport-1.2.3.tar.gz` & `tmp/rustimport-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rustimport-1.2.3.tar", last modified: Sat Apr  8 12:40:23 2023, max compression
+gzip compressed data, was "rustimport-1.2.4.tar", last modified: Sun Apr  9 14:33:55 2023, max compression
```

## Comparing `rustimport-1.2.3.tar` & `rustimport-1.2.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:40:23.835553 rustimport-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-08 12:40:14.000000 rustimport-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-08 12:40:14.000000 rustimport-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-04-08 12:40:23.835553 rustimport-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-04-08 12:40:14.000000 rustimport-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 12:40:14.000000 rustimport-1.2.3/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:40:23.835553 rustimport-1.2.3/rustimport/
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-04-08 12:40:14.000000 rustimport-1.2.3/rustimport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-04-08 12:40:14.000000 rustimport-1.2.3/rustimport/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-08 12:40:14.000000 rustimport-1.2.3/rustimport/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-08 12:40:14.000000 rustimport-1.2.3/rustimport/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-08 12:40:14.000000 rustimport-1.2.3/rustimport/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-08 12:40:14.000000 rustimport-1.2.3/rustimport/find.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-08 12:40:14.000000 rustimport-1.2.3/rustimport/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    12584 2023-04-08 12:40:14.000000 rustimport-1.2.3/rustimport/importable.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-08 12:40:14.000000 rustimport-1.2.3/rustimport/load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:40:23.835553 rustimport-1.2.3/rustimport/pre_processing/
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-08 12:40:14.000000 rustimport-1.2.3/rustimport/pre_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-08 12:40:14.000000 rustimport-1.2.3/rustimport/pre_processing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-08 12:40:14.000000 rustimport-1.2.3/rustimport/pre_processing/pyo3_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-08 12:40:14.000000 rustimport-1.2.3/rustimport/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:40:23.835553 rustimport-1.2.3/rustimport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-04-08 12:40:23.000000 rustimport-1.2.3/rustimport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-08 12:40:23.000000 rustimport-1.2.3/rustimport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 12:40:23.000000 rustimport-1.2.3/rustimport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 12:40:23.000000 rustimport-1.2.3/rustimport.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-08 12:40:23.000000 rustimport-1.2.3/rustimport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-08 12:40:23.000000 rustimport-1.2.3/rustimport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 12:40:23.835553 rustimport-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-08 12:40:14.000000 rustimport-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:40:23.835553 rustimport-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-08 12:40:14.000000 rustimport-1.2.3/tests/run_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-04-08 12:40:14.000000 rustimport-1.2.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-08 12:40:14.000000 rustimport-1.2.3/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:33:55.872160 rustimport-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-09 14:33:44.000000 rustimport-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-09 14:33:44.000000 rustimport-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-04-09 14:33:55.872160 rustimport-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-04-09 14:33:44.000000 rustimport-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 14:33:44.000000 rustimport-1.2.4/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:33:55.872160 rustimport-1.2.4/rustimport/
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12584 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/importable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:33:55.872160 rustimport-1.2.4/rustimport/pre_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/pre_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/pre_processing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/pre_processing/pyo3_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:33:55.872160 rustimport-1.2.4/rustimport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-04-09 14:33:55.000000 rustimport-1.2.4/rustimport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-09 14:33:55.000000 rustimport-1.2.4/rustimport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:33:55.000000 rustimport-1.2.4/rustimport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:33:55.000000 rustimport-1.2.4/rustimport.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-09 14:33:55.000000 rustimport-1.2.4/rustimport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 14:33:55.000000 rustimport-1.2.4/rustimport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 14:33:55.872160 rustimport-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-09 14:33:44.000000 rustimport-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:33:55.872160 rustimport-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-09 14:33:44.000000 rustimport-1.2.4/tests/run_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-04-09 14:33:44.000000 rustimport-1.2.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-09 14:33:44.000000 rustimport-1.2.4/tests/test_examples.py
```

### Comparing `rustimport-1.2.3/LICENSE` & `rustimport-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.3/PKG-INFO` & `rustimport-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustimport
-Version: 1.2.3
+Version: 1.2.4
 Summary: Import Rust files directly from Python!
 Home-page: https://github.com/mityax/rustimport
 Author: mityax
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `rustimport-1.2.3/README.md` & `rustimport-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.3/rustimport/__init__.py` & `rustimport-1.2.4/rustimport/__init__.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.3/rustimport/__main__.py` & `rustimport-1.2.4/rustimport/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,14 @@
              "name ends with \".rs\", a single-file extension is created, otherwise, a crate will be set up.",
     )
     new_parser.add_argument("path")
 
     args = parser.parse_args(raw_args[1:])
 
     ch = logging.StreamHandler()
-    ch.setLevel(logging.DEBUG)
     ch.setFormatter(CLILoggingFormatter())
 
     if args.quiet:
         logging.basicConfig(level=logging.CRITICAL, handlers=[ch])
     elif args.verbose:
         logging.basicConfig(level=logging.DEBUG, handlers=[ch])
     else:
```

### Comparing `rustimport-1.2.3/rustimport/checksum.py` & `rustimport-1.2.4/rustimport/checksum.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.3/rustimport/compiler.py` & `rustimport-1.2.4/rustimport/compiler.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.3/rustimport/error_handling.py` & `rustimport-1.2.4/rustimport/error_handling.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.3/rustimport/find.py` & `rustimport-1.2.4/rustimport/find.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.3/rustimport/import_hook.py` & `rustimport-1.2.4/rustimport/import_hook.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             self.__running = False
 
 
 class Loader(importlib.abc.Loader):
     def __init__(self, importable: Importable):
         self.__importable = importable
 
-    def create_module(self, spec: ModuleSpec) -> types.ModuleType | None:
+    def create_module(self, spec: ModuleSpec) -> Optional[types.ModuleType]:
         if should_rebuild(self.__importable):
             self.__importable.build(release=settings.compile_release_binaries)
         return self.__importable.load()
 
     def exec_module(self, module: types.ModuleType) -> None:
         pass
```

### Comparing `rustimport-1.2.3/rustimport/importable.py` & `rustimport-1.2.4/rustimport/importable.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.3/rustimport/load.py` & `rustimport-1.2.4/rustimport/load.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.3/rustimport/pre_processing/__init__.py` & `rustimport-1.2.4/rustimport/pre_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.3/rustimport/pre_processing/base.py` & `rustimport-1.2.4/rustimport/pre_processing/base.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.3/rustimport/pre_processing/pyo3_template.py` & `rustimport-1.2.4/rustimport/pre_processing/pyo3_template.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.3/rustimport/settings.py` & `rustimport-1.2.4/rustimport/settings.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.3/rustimport.egg-info/PKG-INFO` & `rustimport-1.2.4/rustimport.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustimport
-Version: 1.2.3
+Version: 1.2.4
 Summary: Import Rust files directly from Python!
 Home-page: https://github.com/mityax/rustimport
 Author: mityax
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `rustimport-1.2.3/rustimport.egg-info/SOURCES.txt` & `rustimport-1.2.4/rustimport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.3/setup.py` & `rustimport-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.3/tests/test_cli.py` & `rustimport-1.2.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.3/tests/test_examples.py` & `rustimport-1.2.4/tests/test_examples.py`

 * *Files identical despite different names*

