# Comparing `tmp/wilderness-0.1.8.tar.gz` & `tmp/wilderness-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wilderness-0.1.8.tar", last modified: Wed Aug 31 21:39:40 2022, max compression
+gzip compressed data, was "wilderness-0.1.9.tar", last modified: Fri Jan 13 21:15:24 2023, max compression
```

## Comparing `wilderness-0.1.8.tar` & `wilderness-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,75 @@
-drwxr-xr-x   0 gertjan   (1000) gertjan   (1000)        0 2022-08-31 21:39:40.772495 wilderness-0.1.8/
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)     1071 2021-11-05 22:40:06.000000 wilderness-0.1.8/LICENSE
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)     3536 2022-08-31 21:39:40.772495 wilderness-0.1.8/PKG-INFO
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)     2795 2022-04-13 20:14:49.000000 wilderness-0.1.8/README.md
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)      210 2021-11-03 15:04:45.000000 wilderness-0.1.8/pyproject.toml
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)       38 2022-08-31 21:39:40.772495 wilderness-0.1.8/setup.cfg
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)     2745 2022-01-31 00:22:33.000000 wilderness-0.1.8/setup.py
-drwxr-xr-x   0 gertjan   (1000) gertjan   (1000)        0 2022-08-31 21:39:40.772495 wilderness-0.1.8/wilderness/
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)      278 2022-02-12 22:47:46.000000 wilderness-0.1.8/wilderness/__init__.py
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)       88 2022-08-31 21:35:21.000000 wilderness-0.1.8/wilderness/__version__.py
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)     2078 2022-04-25 21:17:26.000000 wilderness-0.1.8/wilderness/_argparse.py
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)    18221 2022-06-25 20:38:24.000000 wilderness-0.1.8/wilderness/application.py
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)     3253 2022-06-25 20:37:58.000000 wilderness-0.1.8/wilderness/command.py
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)     6316 2022-06-25 20:39:05.000000 wilderness-0.1.8/wilderness/documentable.py
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)     6167 2022-04-01 22:29:51.000000 wilderness-0.1.8/wilderness/formatter.py
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)     1860 2022-06-25 19:30:50.000000 wilderness-0.1.8/wilderness/group.py
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)     2545 2022-08-31 21:33:28.000000 wilderness-0.1.8/wilderness/help.py
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)     7558 2022-08-31 21:33:28.000000 wilderness-0.1.8/wilderness/manpages.py
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)       27 2021-11-10 15:58:13.000000 wilderness-0.1.8/wilderness/py.typed
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)     2149 2022-04-25 22:44:18.000000 wilderness-0.1.8/wilderness/tester.py
-drwxr-xr-x   0 gertjan   (1000) gertjan   (1000)        0 2022-08-31 21:39:40.772495 wilderness-0.1.8/wilderness.egg-info/
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)     3536 2022-08-31 21:39:39.000000 wilderness-0.1.8/wilderness.egg-info/PKG-INFO
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)      518 2022-08-31 21:39:40.000000 wilderness-0.1.8/wilderness.egg-info/SOURCES.txt
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)        1 2022-08-31 21:39:39.000000 wilderness-0.1.8/wilderness.egg-info/dependency_links.txt
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)        1 2022-08-31 21:34:42.000000 wilderness-0.1.8/wilderness.egg-info/not-zip-safe
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)      104 2022-08-31 21:39:40.000000 wilderness-0.1.8/wilderness.egg-info/requires.txt
--rw-r--r--   0 gertjan   (1000) gertjan   (1000)       11 2022-08-31 21:39:40.000000 wilderness-0.1.8/wilderness.egg-info/top_level.txt
+drwxr-xr-x   0 gertjan   (1000) gertjan   (1000)        0 2023-01-13 21:15:24.501674 wilderness-0.1.9/
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     1071 2021-11-05 22:40:06.000000 wilderness-0.1.9/LICENSE
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)      218 2023-01-13 21:15:06.000000 wilderness-0.1.9/MANIFEST.in
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     2787 2022-06-25 20:39:05.000000 wilderness-0.1.9/Makefile
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     3536 2023-01-13 21:15:24.501674 wilderness-0.1.9/PKG-INFO
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     2795 2022-04-13 20:14:49.000000 wilderness-0.1.9/README.md
+drwxr-xr-x   0 gertjan   (1000) gertjan   (1000)        0 2023-01-13 21:15:24.498341 wilderness-0.1.9/docs/
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)      745 2022-04-25 22:05:28.000000 wilderness-0.1.9/docs/CHANGELOG.rst
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)      629 2022-04-25 22:05:28.000000 wilderness-0.1.9/docs/Makefile
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     3052 2022-04-25 22:05:28.000000 wilderness-0.1.9/docs/README.rst
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)       29 2021-11-14 14:51:25.000000 wilderness-0.1.9/docs/_changelog.rst
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)       26 2021-11-14 14:51:14.000000 wilderness-0.1.9/docs/_readme.rst
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     1966 2021-11-14 14:57:36.000000 wilderness-0.1.9/docs/conf.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)      259 2021-11-14 14:52:45.000000 wilderness-0.1.9/docs/index.rst
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)      799 2021-11-14 14:50:51.000000 wilderness-0.1.9/docs/make.bat
+drwxr-xr-x   0 gertjan   (1000) gertjan   (1000)        0 2023-01-13 21:15:24.498341 wilderness-0.1.9/docs/source/
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)      103 2022-04-25 21:59:09.000000 wilderness-0.1.9/docs/source/modules.rst
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     1338 2022-04-25 21:59:09.000000 wilderness-0.1.9/docs/source/wilderness.rst
+drwxr-xr-x   0 gertjan   (1000) gertjan   (1000)        0 2023-01-13 21:15:24.498341 wilderness-0.1.9/examples/
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     1130 2021-11-06 21:01:45.000000 wilderness-0.1.9/examples/README.md
+drwxr-xr-x   0 gertjan   (1000) gertjan   (1000)        0 2023-01-13 21:15:24.498341 wilderness-0.1.9/examples/fakedf/
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     1153 2021-11-10 19:07:55.000000 wilderness-0.1.9/examples/fakedf/README.md
+drwxr-xr-x   0 gertjan   (1000) gertjan   (1000)        0 2023-01-13 21:15:24.498341 wilderness-0.1.9/examples/fakedf/fakedf/
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)        0 2021-11-06 16:48:31.000000 wilderness-0.1.9/examples/fakedf/fakedf/__init__.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)      166 2021-11-06 21:21:26.000000 wilderness-0.1.9/examples/fakedf/fakedf/__main__.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)       47 2021-11-06 16:52:34.000000 wilderness-0.1.9/examples/fakedf/fakedf/__version__.py
+drwxr-xr-x   0 gertjan   (1000) gertjan   (1000)        0 2023-01-13 21:15:24.498341 wilderness-0.1.9/examples/fakedf/fakedf/console/
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)      101 2021-11-06 21:21:26.000000 wilderness-0.1.9/examples/fakedf/fakedf/console/__init__.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     3328 2021-11-06 21:21:26.000000 wilderness-0.1.9/examples/fakedf/fakedf/console/_docs.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     4029 2021-11-06 23:19:24.000000 wilderness-0.1.9/examples/fakedf/fakedf/console/application.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     3110 2021-11-14 23:09:32.000000 wilderness-0.1.9/examples/fakedf/setup.py
+drwxr-xr-x   0 gertjan   (1000) gertjan   (1000)        0 2023-01-13 21:15:24.498341 wilderness-0.1.9/examples/fakegit/
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)      345 2021-11-10 19:08:27.000000 wilderness-0.1.9/examples/fakegit/README.md
+drwxr-xr-x   0 gertjan   (1000) gertjan   (1000)        0 2023-01-13 21:15:24.501674 wilderness-0.1.9/examples/fakegit/fakegit/
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)        0 2021-10-24 22:32:34.000000 wilderness-0.1.9/examples/fakegit/fakegit/__init__.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)      166 2021-11-05 22:14:42.000000 wilderness-0.1.9/examples/fakegit/fakegit/__main__.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)       47 2021-11-04 11:14:27.000000 wilderness-0.1.9/examples/fakegit/fakegit/__version__.py
+drwxr-xr-x   0 gertjan   (1000) gertjan   (1000)        0 2023-01-13 21:15:24.501674 wilderness-0.1.9/examples/fakegit/fakegit/console/
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)      167 2021-11-05 22:25:16.000000 wilderness-0.1.9/examples/fakegit/fakegit/console/__init__.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     7379 2021-11-06 19:52:29.000000 wilderness-0.1.9/examples/fakegit/fakegit/console/application.py
+drwxr-xr-x   0 gertjan   (1000) gertjan   (1000)        0 2023-01-13 21:15:24.501674 wilderness-0.1.9/examples/fakegit/fakegit/console/commands/
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)      229 2021-11-05 22:16:33.000000 wilderness-0.1.9/examples/fakegit/fakegit/console/commands/__init__.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)    18913 2022-02-12 22:47:46.000000 wilderness-0.1.9/examples/fakegit/fakegit/console/commands/clone.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     2875 2022-02-12 22:47:46.000000 wilderness-0.1.9/examples/fakegit/fakegit/console/commands/commit.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     1681 2022-02-12 22:53:04.000000 wilderness-0.1.9/examples/fakegit/fakegit/console/commands/fetch.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     9596 2022-02-12 22:47:46.000000 wilderness-0.1.9/examples/fakegit/fakegit/console/commands/init.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     3115 2021-11-14 23:09:32.000000 wilderness-0.1.9/examples/fakegit/setup.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)      210 2021-11-03 15:04:45.000000 wilderness-0.1.9/pyproject.toml
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)       38 2023-01-13 21:15:24.501674 wilderness-0.1.9/setup.cfg
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     2745 2022-01-31 00:22:33.000000 wilderness-0.1.9/setup.py
+drwxr-xr-x   0 gertjan   (1000) gertjan   (1000)        0 2023-01-13 21:15:24.501674 wilderness-0.1.9/tests/
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)        0 2022-04-25 22:38:33.000000 wilderness-0.1.9/tests/__init__.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     3804 2023-01-13 20:51:47.000000 wilderness-0.1.9/tests/test_application.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     4082 2022-04-25 21:26:23.000000 wilderness-0.1.9/tests/test_formatter.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     2843 2022-06-25 19:33:47.000000 wilderness-0.1.9/tests/test_group.py
+drwxr-xr-x   0 gertjan   (1000) gertjan   (1000)        0 2023-01-13 21:15:24.501674 wilderness-0.1.9/wilderness/
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)      278 2022-02-12 22:47:46.000000 wilderness-0.1.9/wilderness/__init__.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)       88 2023-01-13 21:09:29.000000 wilderness-0.1.9/wilderness/__version__.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     2078 2022-04-25 21:17:26.000000 wilderness-0.1.9/wilderness/_argparse.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)    18231 2023-01-13 20:58:25.000000 wilderness-0.1.9/wilderness/application.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     3243 2023-01-13 20:57:21.000000 wilderness-0.1.9/wilderness/command.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     6316 2022-06-25 20:39:05.000000 wilderness-0.1.9/wilderness/documentable.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     6167 2022-04-01 22:29:51.000000 wilderness-0.1.9/wilderness/formatter.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     1860 2022-06-25 19:30:50.000000 wilderness-0.1.9/wilderness/group.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     2545 2023-01-13 20:51:47.000000 wilderness-0.1.9/wilderness/help.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     7558 2023-01-13 20:51:47.000000 wilderness-0.1.9/wilderness/manpages.py
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)       27 2021-11-10 15:58:13.000000 wilderness-0.1.9/wilderness/py.typed
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     2149 2022-04-25 22:44:18.000000 wilderness-0.1.9/wilderness/tester.py
+drwxr-xr-x   0 gertjan   (1000) gertjan   (1000)        0 2023-01-13 21:15:24.501674 wilderness-0.1.9/wilderness.egg-info/
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     3536 2023-01-13 21:15:24.000000 wilderness-0.1.9/wilderness.egg-info/PKG-INFO
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)     1631 2023-01-13 21:15:24.000000 wilderness-0.1.9/wilderness.egg-info/SOURCES.txt
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)        1 2023-01-13 21:15:24.000000 wilderness-0.1.9/wilderness.egg-info/dependency_links.txt
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)        1 2023-01-13 21:09:05.000000 wilderness-0.1.9/wilderness.egg-info/not-zip-safe
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)      104 2023-01-13 21:15:24.000000 wilderness-0.1.9/wilderness.egg-info/requires.txt
+-rw-r--r--   0 gertjan   (1000) gertjan   (1000)       11 2023-01-13 21:15:24.000000 wilderness-0.1.9/wilderness.egg-info/top_level.txt
```

### Comparing `wilderness-0.1.8/LICENSE` & `wilderness-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wilderness-0.1.8/PKG-INFO` & `wilderness-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wilderness
-Version: 0.1.8
+Version: 0.1.9
 Summary: Easy multi-level command line applications with man pages
 Home-page: https://github.com/GjjvdBurg/wilderness
 Author: Gertjan van den Burg
 Author-email: gertjanvandenburg@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `wilderness-0.1.8/README.md` & `wilderness-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `wilderness-0.1.8/setup.py` & `wilderness-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `wilderness-0.1.8/wilderness/_argparse.py` & `wilderness-0.1.9/wilderness/_argparse.py`

 * *Files identical despite different names*

### Comparing `wilderness-0.1.8/wilderness/application.py` & `wilderness-0.1.9/wilderness/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -541,15 +541,15 @@
 
         # epilog
         formatter.add_text(self._epilog)
 
         # determine help from format above
         return formatter.format_help()
 
-    def print_help(self, file: TextIO = None):
+    def print_help(self, file: Optional[TextIO] = None):
         """Print the command line help text for the application
 
         Parameters
         ----------
         file : Optional[TextIO]
             The file to which to write the help text. If omitted, the help text
             will be written to sys.stdout.
```

### Comparing `wilderness-0.1.8/wilderness/command.py` & `wilderness-0.1.9/wilderness/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 class Command(DocumentableMixin, metaclass=abc.ABCMeta):
     def __init__(
         self,
         name: str,
         title: Optional[str] = None,
         description: Optional[str] = None,
-        add_help: Optional[bool] = True,
+        add_help: bool = True,
         extra_sections: Optional[Dict[str, str]] = None,
         options_prolog: Optional[str] = None,
         options_epilog: Optional[str] = None,
     ):
         super().__init__(
             description=description,
             extra_sections=extra_sections,
```

### Comparing `wilderness-0.1.8/wilderness/documentable.py` & `wilderness-0.1.9/wilderness/documentable.py`

 * *Files identical despite different names*

### Comparing `wilderness-0.1.8/wilderness/formatter.py` & `wilderness-0.1.9/wilderness/formatter.py`

 * *Files identical despite different names*

### Comparing `wilderness-0.1.8/wilderness/group.py` & `wilderness-0.1.9/wilderness/group.py`

 * *Files identical despite different names*

### Comparing `wilderness-0.1.8/wilderness/help.py` & `wilderness-0.1.9/wilderness/help.py`

 * *Files identical despite different names*

### Comparing `wilderness-0.1.8/wilderness/manpages.py` & `wilderness-0.1.9/wilderness/manpages.py`

 * *Files identical despite different names*

### Comparing `wilderness-0.1.8/wilderness/tester.py` & `wilderness-0.1.9/wilderness/tester.py`

 * *Files identical despite different names*

### Comparing `wilderness-0.1.8/wilderness.egg-info/PKG-INFO` & `wilderness-0.1.9/wilderness.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wilderness
-Version: 0.1.8
+Version: 0.1.9
 Summary: Easy multi-level command line applications with man pages
 Home-page: https://github.com/GjjvdBurg/wilderness
 Author: Gertjan van den Burg
 Author-email: gertjanvandenburg@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

