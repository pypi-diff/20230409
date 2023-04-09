# Comparing `tmp/pohan-0.0.3.tar.gz` & `tmp/pohan-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pohan-0.0.3.tar", last modified: Sun Apr  9 05:48:11 2023, max compression
+gzip compressed data, was "pohan-0.0.4.tar", last modified: Sun Apr  9 06:59:21 2023, max compression
```

## Comparing `pohan-0.0.3.tar` & `pohan-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 05:48:11.807372 pohan-0.0.3/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 pohan-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2923 2023-04-09 05:48:11.807372 pohan-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2400 2023-04-08 15:58:00.000000 pohan-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 05:48:11.727238 pohan-0.0.3/pohan/
--rw-rw-rw-   0        0        0       25 2023-04-07 14:38:11.000000 pohan-0.0.3/pohan/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:48:11.783367 pohan-0.0.3/pohan/api/
--rw-rw-rw-   0        0        0       15 2023-04-07 16:46:51.000000 pohan-0.0.3/pohan/api/__init__.py
--rw-rw-rw-   0        0        0      276 2023-04-09 05:45:05.000000 pohan-0.0.3/pohan/api/普通话.py
--rw-rw-rw-   0        0        0      231 2023-04-07 14:40:42.000000 pohan-0.0.3/pohan/api/重庆话.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:48:11.787365 pohan-0.0.3/pohan/lib/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pohan-0.0.3/pohan/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:48:11.756368 pohan-0.0.3/pohan.egg-info/
--rw-rw-rw-   0        0        0     2923 2023-04-09 05:48:11.000000 pohan-0.0.3/pohan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-04-09 05:48:11.000000 pohan-0.0.3/pohan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 05:48:11.000000 pohan-0.0.3/pohan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-07 14:19:04.000000 pohan-0.0.3/pohan.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-04-09 05:48:11.000000 pohan-0.0.3/pohan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      688 2023-04-09 05:48:11.811370 pohan-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 pohan-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:48:11.804368 pohan-0.0.3/tests/
--rw-rw-rw-   0        0        0      181 2023-04-05 16:44:51.000000 pohan-0.0.3/tests/__init__.py
--rw-rw-rw-   0        0        0      392 2023-04-07 14:16:56.000000 pohan-0.0.3/tests/test_pohan.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:21.809289 pohan-0.0.4/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 pohan-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2923 2023-04-09 06:59:21.809289 pohan-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2400 2023-04-08 15:58:00.000000 pohan-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:21.765686 pohan-0.0.4/pohan/
+-rw-rw-rw-   0        0        0       25 2023-04-07 14:38:11.000000 pohan-0.0.4/pohan/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:21.799781 pohan-0.0.4/pohan/api/
+-rw-rw-rw-   0        0        0       15 2023-04-07 16:46:51.000000 pohan-0.0.4/pohan/api/__init__.py
+-rw-rw-rw-   0        0        0      545 2023-04-09 06:38:26.000000 pohan-0.0.4/pohan/api/普通话.py
+-rw-rw-rw-   0        0        0      342 2023-04-09 06:22:08.000000 pohan-0.0.4/pohan/api/重庆话.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:21.802770 pohan-0.0.4/pohan/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pohan-0.0.4/pohan/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:21.790723 pohan-0.0.4/pohan.egg-info/
+-rw-rw-rw-   0        0        0     2923 2023-04-09 06:59:21.000000 pohan-0.0.4/pohan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-04-09 06:59:21.000000 pohan-0.0.4/pohan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 06:59:21.000000 pohan-0.0.4/pohan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-07 14:19:04.000000 pohan-0.0.4/pohan.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-04-09 06:59:21.000000 pohan-0.0.4/pohan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      688 2023-04-09 06:59:21.811288 pohan-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 pohan-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:59:21.807288 pohan-0.0.4/tests/
+-rw-rw-rw-   0        0        0      181 2023-04-05 16:44:51.000000 pohan-0.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0      392 2023-04-07 14:16:56.000000 pohan-0.0.4/tests/test_pohan.py
```

### Comparing `pohan-0.0.3/LICENSE` & `pohan-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pohan-0.0.3/PKG-INFO` & `pohan-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pohan
-Version: 0.0.3
+Version: 0.0.4
 Summary: pip install pohan
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/pohan/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/pohan/blob/master/README.md
```

### Comparing `pohan-0.0.3/README.md` & `pohan-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pohan-0.0.3/pohan.egg-info/PKG-INFO` & `pohan-0.0.4/pohan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pohan
-Version: 0.0.3
+Version: 0.0.4
 Summary: pip install pohan
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/pohan/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/pohan/blob/master/README.md
```

### Comparing `pohan-0.0.3/setup.cfg` & `pohan-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f68 616e 0d0a 7665 7273 696f   = pohan..versio
-00000020: 6e20 3d20 302e 302e 330d 0a64 6573 6372  n = 0.0.3..descr
+00000020: 6e20 3d20 302e 302e 340d 0a64 6573 6372  n = 0.0.4..descr
 00000030: 6970 7469 6f6e 203d 2070 6970 2069 6e73  iption = pip ins
 00000040: 7461 6c6c 2070 6f68 616e 0d0a 6c6f 6e67  tall pohan..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
```

