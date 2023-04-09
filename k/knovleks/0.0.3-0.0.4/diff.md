# Comparing `tmp/knovleks-0.0.3.tar.gz` & `tmp/knovleks-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knovleks-0.0.3.tar", last modified: Sat Oct  1 12:20:59 2022, max compression
+gzip compressed data, was "knovleks-0.0.4.tar", last modified: Sun Apr  9 14:15:03 2023, max compression
```

## Comparing `knovleks-0.0.3.tar` & `knovleks-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 loris     (1000) loris     (1000)        0 2022-10-01 12:20:59.726262 knovleks-0.0.3/
--rw-rw-r--   0 loris     (1000) loris     (1000)    11341 2022-06-11 12:02:50.000000 knovleks-0.0.3/LICENSE
--rw-r--r--   0 loris     (1000) loris     (1000)     1877 2022-10-01 12:20:59.726262 knovleks-0.0.3/PKG-INFO
--rw-rw-r--   0 loris     (1000) loris     (1000)     1686 2022-06-24 22:40:19.000000 knovleks-0.0.3/README.md
-drwxr-xr-x   0 loris     (1000) loris     (1000)        0 2022-10-01 12:20:59.725262 knovleks-0.0.3/knovleks/
--rw-rw-r--   0 loris     (1000) loris     (1000)        0 2022-06-11 17:08:25.000000 knovleks-0.0.3/knovleks/__init__.py
--rw-rw-r--   0 loris     (1000) loris     (1000)     4247 2022-06-24 22:48:05.000000 knovleks-0.0.3/knovleks/__main__.py
-drwxr-xr-x   0 loris     (1000) loris     (1000)        0 2022-10-01 12:20:59.726262 knovleks-0.0.3/knovleks/document_types/
--rw-rw-r--   0 loris     (1000) loris     (1000)      124 2022-06-11 13:57:13.000000 knovleks-0.0.3/knovleks/document_types/__init__.py
--rw-rw-r--   0 loris     (1000) loris     (1000)      291 2022-06-11 14:09:48.000000 knovleks-0.0.3/knovleks/document_types/note_document.py
--rw-rw-r--   0 loris     (1000) loris     (1000)      647 2022-06-24 22:50:07.000000 knovleks-0.0.3/knovleks/document_types/pdf_document.py
--rw-rw-r--   0 loris     (1000) loris     (1000)      587 2022-06-12 12:40:09.000000 knovleks-0.0.3/knovleks/document_types/website_document.py
--rw-rw-r--   0 loris     (1000) loris     (1000)      887 2022-06-12 13:18:36.000000 knovleks-0.0.3/knovleks/idocument_type.py
--rw-rw-r--   0 loris     (1000) loris     (1000)     9875 2022-06-24 22:17:36.000000 knovleks-0.0.3/knovleks/knovleks.py
--rw-rw-r--   0 loris     (1000) loris     (1000)     6871 2022-06-12 13:22:30.000000 knovleks-0.0.3/knovleks/tui.py
-drwxr-xr-x   0 loris     (1000) loris     (1000)        0 2022-10-01 12:20:59.725262 knovleks-0.0.3/knovleks.egg-info/
--rw-rw-r--   0 loris     (1000) loris     (1000)     1877 2022-10-01 12:20:59.000000 knovleks-0.0.3/knovleks.egg-info/PKG-INFO
--rw-rw-r--   0 loris     (1000) loris     (1000)      503 2022-10-01 12:20:59.000000 knovleks-0.0.3/knovleks.egg-info/SOURCES.txt
--rw-rw-r--   0 loris     (1000) loris     (1000)        1 2022-10-01 12:20:59.000000 knovleks-0.0.3/knovleks.egg-info/dependency_links.txt
--rw-rw-r--   0 loris     (1000) loris     (1000)       51 2022-10-01 12:20:59.000000 knovleks-0.0.3/knovleks.egg-info/entry_points.txt
--rw-rw-r--   0 loris     (1000) loris     (1000)       86 2022-10-01 12:20:59.000000 knovleks-0.0.3/knovleks.egg-info/requires.txt
--rw-rw-r--   0 loris     (1000) loris     (1000)        9 2022-10-01 12:20:59.000000 knovleks-0.0.3/knovleks.egg-info/top_level.txt
--rw-rw-r--   0 loris     (1000) loris     (1000)       81 2022-06-11 19:10:53.000000 knovleks-0.0.3/pyproject.toml
--rw-rw-r--   0 loris     (1000) loris     (1000)      621 2022-10-01 12:20:59.726262 knovleks-0.0.3/setup.cfg
+drwxr-xr-x   0 loris     (1000) loris     (1000)        0 2023-04-09 14:15:03.826116 knovleks-0.0.4/
+-rw-rw-r--   0 loris     (1000) loris     (1000)    11341 2022-06-11 12:02:50.000000 knovleks-0.0.4/LICENSE
+-rw-r--r--   0 loris     (1000) loris     (1000)     1877 2023-04-09 14:15:03.826116 knovleks-0.0.4/PKG-INFO
+-rw-rw-r--   0 loris     (1000) loris     (1000)     1686 2022-06-24 22:40:19.000000 knovleks-0.0.4/README.md
+drwxr-xr-x   0 loris     (1000) loris     (1000)        0 2023-04-09 14:15:03.824116 knovleks-0.0.4/knovleks/
+-rw-rw-r--   0 loris     (1000) loris     (1000)        0 2022-06-11 17:08:25.000000 knovleks-0.0.4/knovleks/__init__.py
+-rw-rw-r--   0 loris     (1000) loris     (1000)     4247 2022-06-24 22:48:05.000000 knovleks-0.0.4/knovleks/__main__.py
+drwxr-xr-x   0 loris     (1000) loris     (1000)        0 2023-04-09 14:15:03.825116 knovleks-0.0.4/knovleks/document_types/
+-rw-rw-r--   0 loris     (1000) loris     (1000)      124 2022-06-11 13:57:13.000000 knovleks-0.0.4/knovleks/document_types/__init__.py
+-rw-rw-r--   0 loris     (1000) loris     (1000)      291 2022-06-11 14:09:48.000000 knovleks-0.0.4/knovleks/document_types/note_document.py
+-rw-rw-r--   0 loris     (1000) loris     (1000)      647 2022-06-24 22:50:07.000000 knovleks-0.0.4/knovleks/document_types/pdf_document.py
+-rw-rw-r--   0 loris     (1000) loris     (1000)      587 2022-06-12 12:40:09.000000 knovleks-0.0.4/knovleks/document_types/website_document.py
+-rw-rw-r--   0 loris     (1000) loris     (1000)      887 2022-06-12 13:18:36.000000 knovleks-0.0.4/knovleks/idocument_type.py
+-rw-rw-r--   0 loris     (1000) loris     (1000)     9875 2022-06-24 22:17:36.000000 knovleks-0.0.4/knovleks/knovleks.py
+-rw-rw-r--   0 loris     (1000) loris     (1000)     6871 2022-06-12 13:22:30.000000 knovleks-0.0.4/knovleks/tui.py
+drwxr-xr-x   0 loris     (1000) loris     (1000)        0 2023-04-09 14:15:03.825116 knovleks-0.0.4/knovleks.egg-info/
+-rw-rw-r--   0 loris     (1000) loris     (1000)     1877 2023-04-09 14:15:03.000000 knovleks-0.0.4/knovleks.egg-info/PKG-INFO
+-rw-rw-r--   0 loris     (1000) loris     (1000)      518 2023-04-09 14:15:03.000000 knovleks-0.0.4/knovleks.egg-info/SOURCES.txt
+-rw-rw-r--   0 loris     (1000) loris     (1000)        1 2023-04-09 14:15:03.000000 knovleks-0.0.4/knovleks.egg-info/dependency_links.txt
+-rw-rw-r--   0 loris     (1000) loris     (1000)       51 2023-04-09 14:15:03.000000 knovleks-0.0.4/knovleks.egg-info/entry_points.txt
+-rw-rw-r--   0 loris     (1000) loris     (1000)       86 2023-04-09 14:15:03.000000 knovleks-0.0.4/knovleks.egg-info/requires.txt
+-rw-rw-r--   0 loris     (1000) loris     (1000)        9 2023-04-09 14:15:03.000000 knovleks-0.0.4/knovleks.egg-info/top_level.txt
+-rw-rw-r--   0 loris     (1000) loris     (1000)       81 2022-06-11 19:10:53.000000 knovleks-0.0.4/pyproject.toml
+-rw-rw-r--   0 loris     (1000) loris     (1000)      621 2023-04-09 14:15:03.826116 knovleks-0.0.4/setup.cfg
+drwxr-xr-x   0 loris     (1000) loris     (1000)        0 2023-04-09 14:15:03.826116 knovleks-0.0.4/tests/
+-rw-rw-r--   0 loris     (1000) loris     (1000)     8288 2022-06-11 17:19:58.000000 knovleks-0.0.4/tests/tests.py
```

### Comparing `knovleks-0.0.3/LICENSE` & `knovleks-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `knovleks-0.0.3/PKG-INFO` & `knovleks-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knovleks
-Version: 0.0.3
+Version: 0.0.4
 Author: Loris Reiff
 Author-email: loris.reiff@liblor.ch
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Knovleks
```

### Comparing `knovleks-0.0.3/README.md` & `knovleks-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `knovleks-0.0.3/knovleks/__main__.py` & `knovleks-0.0.4/knovleks/__main__.py`

 * *Files identical despite different names*

### Comparing `knovleks-0.0.3/knovleks/document_types/pdf_document.py` & `knovleks-0.0.4/knovleks/document_types/pdf_document.py`

 * *Files identical despite different names*

### Comparing `knovleks-0.0.3/knovleks/document_types/website_document.py` & `knovleks-0.0.4/knovleks/document_types/website_document.py`

 * *Files identical despite different names*

### Comparing `knovleks-0.0.3/knovleks/idocument_type.py` & `knovleks-0.0.4/knovleks/idocument_type.py`

 * *Files identical despite different names*

### Comparing `knovleks-0.0.3/knovleks/knovleks.py` & `knovleks-0.0.4/knovleks/knovleks.py`

 * *Files identical despite different names*

### Comparing `knovleks-0.0.3/knovleks/tui.py` & `knovleks-0.0.4/knovleks/tui.py`

 * *Files identical despite different names*

### Comparing `knovleks-0.0.3/knovleks.egg-info/PKG-INFO` & `knovleks-0.0.4/knovleks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knovleks
-Version: 0.0.3
+Version: 0.0.4
 Author: Loris Reiff
 Author-email: loris.reiff@liblor.ch
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Knovleks
```

### Comparing `knovleks-0.0.3/setup.cfg` & `knovleks-0.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [metadata]
 name = knovleks
-version = 0.0.3
+version = 0.0.4
 author = Loris Reiff
 author_email = loris.reiff@liblor.ch
 license = Apache 2.0
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 packages = find:
 install_requires = 
-	PyMuPDF==1.20.2
+	PyMuPDF==1.21.1
 	newspaper3k==0.2.8
 	click==8.1.3
 	textual==0.1.18
 	textual-inputs==0.2.6
 
 [options.entry_points]
 console_scripts =
```

