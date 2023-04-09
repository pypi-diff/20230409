# Comparing `tmp/lupin-danquin-0.0.1.dev1.tar.gz` & `tmp/lupin-danquin-0.0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lupin-danquin-0.0.1.dev1.tar", last modified: Sun Apr  9 16:23:48 2023, max compression
+gzip compressed data, was "lupin-danquin-0.0.1.dev2.tar", last modified: Sun Apr  9 21:53:09 2023, max compression
```

## Comparing `lupin-danquin-0.0.1.dev1.tar` & `lupin-danquin-0.0.1.dev2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 16:23:48.352696 lupin-danquin-0.0.1.dev1/
--rw-rw-rw-   0        0        0     1093 2023-04-09 16:08:01.000000 lupin-danquin-0.0.1.dev1/LICENCE
--rw-rw-rw-   0        0        0      573 2023-04-09 16:23:48.352696 lupin-danquin-0.0.1.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     1010 2023-04-09 16:15:47.000000 lupin-danquin-0.0.1.dev1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 16:23:48.327161 lupin-danquin-0.0.1.dev1/lupin_danquin/
--rw-rw-rw-   0        0        0       28 2023-04-09 16:23:48.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/__init__.py
--rw-rw-rw-   0        0        0      825 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/check_coding_rules.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:23:48.348185 lupin-danquin-0.0.1.dev1/lupin_danquin/core/
--rw-rw-rw-   0        0        0        0 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/__init__.py
--rw-rw-rw-   0        0        0     4561 2023-04-07 13:23:10.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/application.py
--rw-rw-rw-   0        0        0      538 2023-04-09 15:14:35.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/external_resources.py
--rw-rw-rw-   0        0        0     1797 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/global_variable.py
--rw-rw-rw-   0        0        0       23 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/line_ended.py
--rw-rw-rw-   0        0        0     1173 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/local_variable.py
--rw-rw-rw-   0        0        0     1448 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/parameter.py
--rw-rw-rw-   0        0        0     4619 2023-04-09 15:14:46.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/program.py
--rw-rw-rw-   0        0        0      356 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/rules.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:23:48.349757 lupin-danquin-0.0.1.dev1/lupin_danquin/core/tools/
--rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/tools/__init__.py
--rw-rw-rw-   0        0        0      961 2023-04-09 15:57:16.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:23:48.351699 lupin-danquin-0.0.1.dev1/lupin_danquin/core/val3_doc_generator/
--rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/val3_doc_generator/__init__.py
--rw-rw-rw-   0        0        0     1363 2023-04-09 15:14:35.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py
--rw-rw-rw-   0        0        0     1461 2023-04-09 15:14:35.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/documentation_extraction.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:23:48.341183 lupin-danquin-0.0.1.dev1/lupin_danquin.egg-info/
--rw-rw-rw-   0        0        0      573 2023-04-09 16:23:48.000000 lupin-danquin-0.0.1.dev1/lupin_danquin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      845 2023-04-09 16:23:48.000000 lupin-danquin-0.0.1.dev1/lupin_danquin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 16:23:48.000000 lupin-danquin-0.0.1.dev1/lupin_danquin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-09 15:55:39.000000 lupin-danquin-0.0.1.dev1/lupin_danquin.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       89 2023-04-09 16:23:48.000000 lupin-danquin-0.0.1.dev1/lupin_danquin.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-09 16:23:48.000000 lupin-danquin-0.0.1.dev1/lupin_danquin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      828 2023-04-09 16:23:48.353696 lupin-danquin-0.0.1.dev1/setup.cfg
--rw-rw-rw-   0        0        0      172 2023-04-09 15:52:50.000000 lupin-danquin-0.0.1.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 21:53:09.715095 lupin-danquin-0.0.1.dev2/
+-rw-rw-rw-   0        0        0     1093 2023-04-09 16:27:22.000000 lupin-danquin-0.0.1.dev2/LICENCE
+-rw-rw-rw-   0        0        0      573 2023-04-09 21:53:09.715095 lupin-danquin-0.0.1.dev2/PKG-INFO
+-rw-rw-rw-   0        0        0     1010 2023-04-09 16:27:22.000000 lupin-danquin-0.0.1.dev2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 21:53:09.690273 lupin-danquin-0.0.1.dev2/lupin_danquin/
+-rw-rw-rw-   0        0        0       28 2023-04-09 21:53:09.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/__init__.py
+-rw-rw-rw-   0        0        0       78 2023-04-09 16:33:06.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/__main__.py
+-rw-rw-rw-   0        0        0      825 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/check_coding_rules.py
+drwxrwxrwx   0        0        0        0 2023-04-09 21:53:09.712093 lupin-danquin-0.0.1.dev2/lupin_danquin/core/
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/__init__.py
+-rw-rw-rw-   0        0        0     4561 2023-04-07 13:23:10.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/application.py
+-rw-rw-rw-   0        0        0     1797 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/global_variable.py
+-rw-rw-rw-   0        0        0       23 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/line_ended.py
+-rw-rw-rw-   0        0        0     1173 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/local_variable.py
+-rw-rw-rw-   0        0        0     1448 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/parameter.py
+-rw-rw-rw-   0        0        0     4619 2023-04-09 15:14:46.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/program.py
+-rw-rw-rw-   0        0        0      356 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/rules.py
+drwxrwxrwx   0        0        0        0 2023-04-09 21:53:09.713095 lupin-danquin-0.0.1.dev2/lupin_danquin/core/tools/
+-rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/tools/__init__.py
+-rw-rw-rw-   0        0        0     1917 2023-04-09 21:52:28.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-09 21:53:09.714095 lupin-danquin-0.0.1.dev2/lupin_danquin/core/val3_doc_generator/
+-rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/val3_doc_generator/__init__.py
+-rw-rw-rw-   0        0        0     3264 2023-04-09 17:28:09.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py
+-rw-rw-rw-   0        0        0     1441 2023-04-09 21:52:55.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/run.py
+drwxrwxrwx   0        0        0        0 2023-04-09 21:53:09.704784 lupin-danquin-0.0.1.dev2/lupin_danquin.egg-info/
+-rw-rw-rw-   0        0        0      573 2023-04-09 21:53:09.000000 lupin-danquin-0.0.1.dev2/lupin_danquin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      849 2023-04-09 21:53:09.000000 lupin-danquin-0.0.1.dev2/lupin_danquin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 21:53:09.000000 lupin-danquin-0.0.1.dev2/lupin_danquin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-09 21:53:09.000000 lupin-danquin-0.0.1.dev2/lupin_danquin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-09 16:34:59.000000 lupin-danquin-0.0.1.dev2/lupin_danquin.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       90 2023-04-09 21:53:09.000000 lupin-danquin-0.0.1.dev2/lupin_danquin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-09 21:53:09.000000 lupin-danquin-0.0.1.dev2/lupin_danquin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      906 2023-04-09 21:53:09.716094 lupin-danquin-0.0.1.dev2/setup.cfg
+-rw-rw-rw-   0        0        0      172 2023-04-09 16:27:22.000000 lupin-danquin-0.0.1.dev2/setup.py
```

### Comparing `lupin-danquin-0.0.1.dev1/LICENCE` & `lupin-danquin-0.0.1.dev2/LICENCE`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev1/PKG-INFO` & `lupin-danquin-0.0.1.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-danquin
-Version: 0.0.1.dev1
+Version: 0.0.1.dev2
 Summary: Testing - Documentation
 License: MIT License
 Keywords: documentation,testing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Documentation
```

### Comparing `lupin-danquin-0.0.1.dev1/README.md` & `lupin-danquin-0.0.1.dev2/README.md`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev1/lupin_danquin/check_coding_rules.py` & `lupin-danquin-0.0.1.dev2/lupin_danquin/check_coding_rules.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev1/lupin_danquin/core/application.py` & `lupin-danquin-0.0.1.dev2/lupin_danquin/core/application.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev1/lupin_danquin/core/global_variable.py` & `lupin-danquin-0.0.1.dev2/lupin_danquin/core/global_variable.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev1/lupin_danquin/core/local_variable.py` & `lupin-danquin-0.0.1.dev2/lupin_danquin/core/local_variable.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev1/lupin_danquin/core/parameter.py` & `lupin-danquin-0.0.1.dev2/lupin_danquin/core/parameter.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev1/lupin_danquin/core/program.py` & `lupin-danquin-0.0.1.dev2/lupin_danquin/core/program.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev1/lupin_danquin.egg-info/PKG-INFO` & `lupin-danquin-0.0.1.dev2/lupin_danquin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-danquin
-Version: 0.0.1.dev1
+Version: 0.0.1.dev2
 Summary: Testing - Documentation
 License: MIT License
 Keywords: documentation,testing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Documentation
```

### Comparing `lupin-danquin-0.0.1.dev1/lupin_danquin.egg-info/SOURCES.txt` & `lupin-danquin-0.0.1.dev2/lupin_danquin.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 LICENCE
 README.md
 setup.cfg
 setup.py
 lupin_danquin/__init__.py
+lupin_danquin/__main__.py
 lupin_danquin/check_coding_rules.py
-lupin_danquin/documentation_extraction.py
+lupin_danquin/run.py
 lupin_danquin.egg-info/PKG-INFO
 lupin_danquin.egg-info/SOURCES.txt
 lupin_danquin.egg-info/dependency_links.txt
+lupin_danquin.egg-info/entry_points.txt
 lupin_danquin.egg-info/not-zip-safe
 lupin_danquin.egg-info/requires.txt
 lupin_danquin.egg-info/top_level.txt
 lupin_danquin/core/__init__.py
 lupin_danquin/core/application.py
-lupin_danquin/core/external_resources.py
 lupin_danquin/core/global_variable.py
 lupin_danquin/core/line_ended.py
 lupin_danquin/core/local_variable.py
 lupin_danquin/core/parameter.py
 lupin_danquin/core/program.py
 lupin_danquin/core/rules.py
 lupin_danquin/core/tools/__init__.py
```

