# Comparing `tmp/katalytic-pkg-0.1.1.tar.gz` & `tmp/katalytic-pkg-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-pkg-0.1.1.tar", last modified: Sat Apr  8 14:25:13 2023, max compression
+gzip compressed data, was "katalytic-pkg-0.2.0.tar", last modified: Sun Apr  9 04:07:02 2023, max compression
```

## Comparing `katalytic-pkg-0.1.1.tar` & `katalytic-pkg-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-08 14:25:13.153405 katalytic-pkg-0.1.1/
--rw-rw-r--   0 wip       (1000) wip       (1000)     1066 2023-04-07 08:03:04.000000 katalytic-pkg-0.1.1/LICENSE.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)     2815 2023-04-08 14:25:13.153405 katalytic-pkg-0.1.1/PKG-INFO
--rw-rw-r--   0 wip       (1000) wip       (1000)      877 2023-04-07 08:03:04.000000 katalytic-pkg-0.1.1/README.md
--rw-rw-r--   0 wip       (1000) wip       (1000)      881 2023-04-08 14:04:29.000000 katalytic-pkg-0.1.1/pyproject.toml
--rw-rw-r--   0 wip       (1000) wip       (1000)       38 2023-04-08 14:25:13.153405 katalytic-pkg-0.1.1/setup.cfg
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-08 14:25:13.149405 katalytic-pkg-0.1.1/src/
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-08 14:25:13.149405 katalytic-pkg-0.1.1/src/katalytic/
--rw-rw-r--   0 wip       (1000) wip       (1000)     4073 2023-04-08 13:53:10.000000 katalytic-pkg-0.1.1/src/katalytic/pkg.py
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-08 14:25:13.153405 katalytic-pkg-0.1.1/src/katalytic_pkg.egg-info/
--rw-rw-r--   0 wip       (1000) wip       (1000)     2815 2023-04-08 14:25:13.000000 katalytic-pkg-0.1.1/src/katalytic_pkg.egg-info/PKG-INFO
--rw-rw-r--   0 wip       (1000) wip       (1000)      239 2023-04-08 14:25:13.000000 katalytic-pkg-0.1.1/src/katalytic_pkg.egg-info/SOURCES.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)        1 2023-04-08 14:25:13.000000 katalytic-pkg-0.1.1/src/katalytic_pkg.egg-info/dependency_links.txt
--rw-rw-r--   0 wip       (1000) wip       (1000)       10 2023-04-08 14:25:13.000000 katalytic-pkg-0.1.1/src/katalytic_pkg.egg-info/top_level.txt
-drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-08 14:25:13.153405 katalytic-pkg-0.1.1/tests/
--rw-rw-r--   0 wip       (1000) wip       (1000)     2604 2023-04-08 13:56:04.000000 katalytic-pkg-0.1.1/tests/test_pkg.py
+drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 04:07:02.544979 katalytic-pkg-0.2.0/
+-rw-rw-r--   0 wip       (1000) wip       (1000)     1066 2023-04-07 08:03:04.000000 katalytic-pkg-0.2.0/LICENSE.txt
+-rw-rw-r--   0 wip       (1000) wip       (1000)     2815 2023-04-09 04:07:02.544979 katalytic-pkg-0.2.0/PKG-INFO
+-rw-rw-r--   0 wip       (1000) wip       (1000)      877 2023-04-07 08:03:04.000000 katalytic-pkg-0.2.0/README.md
+-rw-rw-r--   0 wip       (1000) wip       (1000)      881 2023-04-09 04:01:05.000000 katalytic-pkg-0.2.0/pyproject.toml
+-rw-rw-r--   0 wip       (1000) wip       (1000)       38 2023-04-09 04:07:02.544979 katalytic-pkg-0.2.0/setup.cfg
+drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 04:07:02.544979 katalytic-pkg-0.2.0/src/
+drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 04:07:02.544979 katalytic-pkg-0.2.0/src/katalytic/
+-rw-rw-r--   0 wip       (1000) wip       (1000)     4091 2023-04-09 03:58:18.000000 katalytic-pkg-0.2.0/src/katalytic/pkg.py
+drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 04:07:02.544979 katalytic-pkg-0.2.0/src/katalytic_pkg.egg-info/
+-rw-rw-r--   0 wip       (1000) wip       (1000)     2815 2023-04-09 04:07:02.000000 katalytic-pkg-0.2.0/src/katalytic_pkg.egg-info/PKG-INFO
+-rw-rw-r--   0 wip       (1000) wip       (1000)      239 2023-04-09 04:07:02.000000 katalytic-pkg-0.2.0/src/katalytic_pkg.egg-info/SOURCES.txt
+-rw-rw-r--   0 wip       (1000) wip       (1000)        1 2023-04-09 04:07:02.000000 katalytic-pkg-0.2.0/src/katalytic_pkg.egg-info/dependency_links.txt
+-rw-rw-r--   0 wip       (1000) wip       (1000)       10 2023-04-09 04:07:02.000000 katalytic-pkg-0.2.0/src/katalytic_pkg.egg-info/top_level.txt
+drwxrwxr-x   0 wip       (1000) wip       (1000)        0 2023-04-09 04:07:02.544979 katalytic-pkg-0.2.0/tests/
+-rw-rw-r--   0 wip       (1000) wip       (1000)     2604 2023-04-08 13:56:04.000000 katalytic-pkg-0.2.0/tests/test_pkg.py
```

### Comparing `katalytic-pkg-0.1.1/LICENSE.txt` & `katalytic-pkg-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.1.1/PKG-INFO` & `katalytic-pkg-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-pkg
-Version: 0.1.1
+Version: 0.2.0
 Summary: This plugin provides some metaprogramming magic for the other katalytic plugins
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 License: Copyright 2023 - present, Valentin Neagu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `katalytic-pkg-0.1.1/README.md` & `katalytic-pkg-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-pkg-0.1.1/pyproject.toml` & `katalytic-pkg-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "katalytic-pkg"
-version = "0.1.1"
+version = "0.2.0"
 description = "This plugin provides some metaprogramming magic for the other katalytic plugins"
 
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 requires-python = ">=3.6"
 
 classifiers = [
```

### Comparing `katalytic-pkg-0.1.1/src/katalytic/pkg.py` & `katalytic-pkg-0.2.0/src/katalytic/pkg.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,23 +31,23 @@
                 yield p2
                 if Path(f'{p2}/METADATA').is_file():
                     yield p2
             elif p2.endswith('.egg-info') and Path(f'{p2}/PKG-INFO').is_file():
                 yield p2
 
 
-def get_version(name, pkg):  # pragma: no cover -- I can't test all branches at the same time
+def get_version(dunder_name):  # pragma: no cover -- I can't test all branches at the same time
     if sys.version_info >= (3, 8):
         from importlib import metadata
-        version = metadata.version(name.replace('.', '-'))
+        version = metadata.version(dunder_name.replace('.', '-'))
         version_info = tuple(map(int, version.split('.')))
         return version, version_info
 
     version = None
-    for p in __find_paths(pkg):
+    for p in __find_paths(dunder_name.split('.')[0]):
         if p.endswith('.dist-info'):
             version = re.search(r'\w+-(\d+\.\d+\.\d+)', p)
             if version:
                 version = version.group(1)
                 break
 
         if p.endswith('.dist-info/METADATA'):
@@ -68,15 +68,15 @@
     # Nothing worked, but I would rather not raise an exception.
     # The package can be used without the version
     # This could happen if the package is installed on python 3.6
     # python 3.8 works fine
     return version, version_info
 
 
-__version__, __version_info__ = get_version(__name__, __package__)
+__version__, __version_info__ = get_version(__name__)
 
 
 def _get_stacktrace(e):
     return ''.join(traceback.format_exception(None, e, e.__traceback__))
 
 
 def _check(name, group):
```

### Comparing `katalytic-pkg-0.1.1/src/katalytic_pkg.egg-info/PKG-INFO` & `katalytic-pkg-0.2.0/src/katalytic_pkg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-pkg
-Version: 0.1.1
+Version: 0.2.0
 Summary: This plugin provides some metaprogramming magic for the other katalytic plugins
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 License: Copyright 2023 - present, Valentin Neagu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `katalytic-pkg-0.1.1/tests/test_pkg.py` & `katalytic-pkg-0.2.0/tests/test_pkg.py`

 * *Files identical despite different names*

