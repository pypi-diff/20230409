# Comparing `tmp/sspeedup-0.5.0.tar.gz` & `tmp/sspeedup-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sspeedup-0.5.0.tar", max compression
+gzip compressed data, was "sspeedup-0.6.0.tar", max compression
```

## Comparing `sspeedup-0.5.0.tar` & `sspeedup-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1063 2023-02-11 14:43:18.500251 sspeedup-0.5.0/LICENSE
--rw-r--r--   0        0        0      225 2023-02-28 22:37:56.096629 sspeedup-0.5.0/README.md
--rw-r--r--   0        0        0     1257 2023-04-04 22:57:25.287162 sspeedup-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1940 2023-04-04 22:57:25.287162 sspeedup-0.5.0/sspeedup/api.py
--rw-r--r--   0        0        0      651 2023-02-28 22:37:56.103296 sspeedup-0.5.0/sspeedup/cache/timeout.py
--rw-r--r--   0        0        0     3223 2023-04-04 22:57:25.287162 sspeedup-0.5.0/sspeedup/colorful_print.py
--rw-r--r--   0        0        0      334 2023-03-03 22:38:05.439511 sspeedup-0.5.0/sspeedup/dict_helper.py
--rw-r--r--   0        0        0    12985 2023-03-17 09:06:31.863741 sspeedup-0.5.0/sspeedup/logging/run_logger.py
--rw-r--r--   0        0        0      686 2023-03-03 22:38:05.439511 sspeedup-0.5.0/sspeedup/make_qrcode.py
--rw-r--r--   0        0        0      594 2023-04-04 22:57:25.287162 sspeedup-0.5.0/sspeedup/pywebio/callbacks.py
--rw-r--r--   0        0        0      332 2023-04-04 22:57:25.290494 sspeedup-0.5.0/sspeedup/require.py
--rw-r--r--   0        0        0      168 2023-03-07 22:21:34.412596 sspeedup-0.5.0/sspeedup/retry/__init__.py
--rw-r--r--   0        0        0     1664 2023-04-04 22:57:25.290494 sspeedup-0.5.0/sspeedup/retry/deco.py
--rw-r--r--   0        0        0      168 2023-03-07 22:21:34.412596 sspeedup-0.5.0/sspeedup/retry/event.py
--rw-r--r--   0        0        0      623 2023-04-04 22:57:25.290494 sspeedup-0.5.0/sspeedup/retry/policy.py
--rw-r--r--   0        0        0     2219 2023-04-04 22:57:25.290494 sspeedup-0.5.0/sspeedup/time_helper.py
--rw-r--r--   0        0        0     2332 2023-02-28 22:37:56.103296 sspeedup-0.5.0/sspeedup/word_split/_base.py
--rw-r--r--   0        0        0     5155 2023-02-28 22:37:56.109963 sspeedup-0.5.0/sspeedup/word_split/jieba.py
--rw-r--r--   0        0        0     1436 1970-01-01 00:00:00.000000 sspeedup-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-02-11 14:43:18.500251 sspeedup-0.6.0/LICENSE
+-rw-r--r--   0        0        0      225 2023-02-28 22:37:56.096629 sspeedup-0.6.0/README.md
+-rw-r--r--   0        0        0     1257 2023-04-08 23:07:04.719413 sspeedup-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2311 2023-04-08 23:07:04.719413 sspeedup-0.6.0/sspeedup/api.py
+-rw-r--r--   0        0        0      651 2023-02-28 22:37:56.103296 sspeedup-0.6.0/sspeedup/cache/timeout.py
+-rw-r--r--   0        0        0     3223 2023-04-04 22:57:25.287162 sspeedup-0.6.0/sspeedup/colorful_print.py
+-rw-r--r--   0        0        0      334 2023-03-03 22:38:05.439511 sspeedup-0.6.0/sspeedup/dict_helper.py
+-rw-r--r--   0        0        0    12985 2023-03-17 09:06:31.863741 sspeedup-0.6.0/sspeedup/logging/run_logger.py
+-rw-r--r--   0        0        0      686 2023-03-03 22:38:05.439511 sspeedup-0.6.0/sspeedup/make_qrcode.py
+-rw-r--r--   0        0        0      594 2023-04-04 22:57:25.287162 sspeedup-0.6.0/sspeedup/pywebio/callbacks.py
+-rw-r--r--   0        0        0      332 2023-04-04 22:57:25.290494 sspeedup-0.6.0/sspeedup/require.py
+-rw-r--r--   0        0        0      168 2023-03-07 22:21:34.412596 sspeedup-0.6.0/sspeedup/retry/__init__.py
+-rw-r--r--   0        0        0     1664 2023-04-04 22:57:25.290494 sspeedup-0.6.0/sspeedup/retry/deco.py
+-rw-r--r--   0        0        0      168 2023-03-07 22:21:34.412596 sspeedup-0.6.0/sspeedup/retry/event.py
+-rw-r--r--   0        0        0      623 2023-04-04 22:57:25.290494 sspeedup-0.6.0/sspeedup/retry/policy.py
+-rw-r--r--   0        0        0     2219 2023-04-04 22:57:25.290494 sspeedup-0.6.0/sspeedup/time_helper.py
+-rw-r--r--   0        0        0     2332 2023-02-28 22:37:56.103296 sspeedup-0.6.0/sspeedup/word_split/_base.py
+-rw-r--r--   0        0        0     5155 2023-02-28 22:37:56.109963 sspeedup-0.6.0/sspeedup/word_split/jieba.py
+-rw-r--r--   0        0        0     1436 1970-01-01 00:00:00.000000 sspeedup-0.6.0/PKG-INFO
```

### Comparing `sspeedup-0.5.0/LICENSE` & `sspeedup-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sspeedup-0.5.0/pyproject.toml` & `sspeedup-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sspeedup"
-version = "0.5.0"
+version = "0.6.0"
 description = "开发工具箱"
 authors = ["yezi <yehaowei20060411@qq.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/FHU-yezi/sspeedup"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `sspeedup-0.5.0/sspeedup/cache/timeout.py` & `sspeedup-0.6.0/sspeedup/cache/timeout.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.5.0/sspeedup/colorful_print.py` & `sspeedup-0.6.0/sspeedup/colorful_print.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.5.0/sspeedup/logging/run_logger.py` & `sspeedup-0.6.0/sspeedup/logging/run_logger.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.5.0/sspeedup/make_qrcode.py` & `sspeedup-0.6.0/sspeedup/make_qrcode.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.5.0/sspeedup/pywebio/callbacks.py` & `sspeedup-0.6.0/sspeedup/pywebio/callbacks.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.5.0/sspeedup/retry/deco.py` & `sspeedup-0.6.0/sspeedup/retry/deco.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.5.0/sspeedup/retry/policy.py` & `sspeedup-0.6.0/sspeedup/retry/policy.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.5.0/sspeedup/time_helper.py` & `sspeedup-0.6.0/sspeedup/time_helper.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.5.0/sspeedup/word_split/_base.py` & `sspeedup-0.6.0/sspeedup/word_split/_base.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.5.0/sspeedup/word_split/jieba.py` & `sspeedup-0.6.0/sspeedup/word_split/jieba.py`

 * *Files identical despite different names*

### Comparing `sspeedup-0.5.0/PKG-INFO` & `sspeedup-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sspeedup
-Version: 0.5.0
+Version: 0.6.0
 Summary: 开发工具箱
 Home-page: https://github.com/FHU-yezi/sspeedup
 License: MIT
 Author: yezi
 Author-email: yehaowei20060411@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

