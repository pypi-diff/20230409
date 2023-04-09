# Comparing `tmp/kavk_api-0.9.7.2.tar.gz` & `tmp/kavk_api-0.9.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kavk_api-0.9.7.2.tar", max compression
+gzip compressed data, was "kavk_api-0.9.7.3.tar", max compression
```

## Comparing `kavk_api-0.9.7.2.tar` & `kavk_api-0.9.7.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1066 2023-04-08 11:31:33.141480 kavk_api-0.9.7.2/LICENSE
--rw-r--r--   0        0        0     1251 2023-04-08 11:46:12.307389 kavk_api-0.9.7.2/README.rst
--rw-r--r--   0        0        0       51 2023-04-08 11:31:33.141480 kavk_api-0.9.7.2/kavk_api/__init__.py
--rw-r--r--   0        0        0     3192 2023-04-08 15:49:21.388876 kavk_api-0.9.7.2/kavk_api/bot_longpoll.py
--rw-r--r--   0        0        0    10766 2023-04-08 11:31:33.141480 kavk_api-0.9.7.2/kavk_api/enums.py
--rw-r--r--   0        0        0      341 2023-04-08 11:31:33.141480 kavk_api-0.9.7.2/kavk_api/exceptions.py
--rw-r--r--   0        0        0     4037 2023-04-08 11:31:33.141480 kavk_api-0.9.7.2/kavk_api/kavk_api.py
--rw-r--r--   0        0        0     7917 2023-04-08 11:31:33.142480 kavk_api-0.9.7.2/kavk_api/longpoll.py
--rw-r--r--   0        0        0     2941 2023-04-08 11:31:33.142480 kavk_api-0.9.7.2/kavk_api/types/base.py
--rw-r--r--   0        0        0     8143 2023-04-08 12:49:15.273996 kavk_api-0.9.7.2/kavk_api/types/bot_events.py
--rw-r--r--   0        0        0     5024 2023-04-08 11:31:33.142480 kavk_api-0.9.7.2/kavk_api/types/event_objects.py
--rw-r--r--   0        0        0   194565 2023-04-08 11:31:33.143480 kavk_api-0.9.7.2/kavk_api/types/methods.py
--rw-r--r--   0        0        0   144553 2023-04-08 11:31:33.144480 kavk_api-0.9.7.2/kavk_api/types/objects.py
--rw-r--r--   0        0        0    43554 2023-04-08 11:31:33.145480 kavk_api-0.9.7.2/kavk_api/types/responses.py
--rw-r--r--   0        0        0      123 2023-04-08 11:31:33.145480 kavk_api-0.9.7.2/kavk_api/utils.py
--rw-r--r--   0        0        0      423 2023-04-08 15:49:45.003873 kavk_api-0.9.7.2/pyproject.toml
--rw-r--r--   0        0        0     1689 1970-01-01 00:00:00.000000 kavk_api-0.9.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-08 11:31:33.141480 kavk_api-0.9.7.3/LICENSE
+-rw-r--r--   0        0        0     1251 2023-04-08 11:46:12.307389 kavk_api-0.9.7.3/README.rst
+-rw-r--r--   0        0        0       51 2023-04-08 11:31:33.141480 kavk_api-0.9.7.3/kavk_api/__init__.py
+-rw-r--r--   0        0        0     3192 2023-04-08 15:49:21.388876 kavk_api-0.9.7.3/kavk_api/bot_longpoll.py
+-rw-r--r--   0        0        0    10766 2023-04-08 11:31:33.141480 kavk_api-0.9.7.3/kavk_api/enums.py
+-rw-r--r--   0        0        0      341 2023-04-08 11:31:33.141480 kavk_api-0.9.7.3/kavk_api/exceptions.py
+-rw-r--r--   0        0        0     4037 2023-04-08 11:31:33.141480 kavk_api-0.9.7.3/kavk_api/kavk_api.py
+-rw-r--r--   0        0        0     7917 2023-04-08 11:31:33.142480 kavk_api-0.9.7.3/kavk_api/longpoll.py
+-rw-r--r--   0        0        0     3773 2023-04-08 19:28:05.512515 kavk_api-0.9.7.3/kavk_api/types/base.py
+-rw-r--r--   0        0        0     8143 2023-04-09 07:57:29.029583 kavk_api-0.9.7.3/kavk_api/types/bot_events.py
+-rw-r--r--   0        0        0     5024 2023-04-09 07:57:45.848583 kavk_api-0.9.7.3/kavk_api/types/event_objects.py
+-rw-r--r--   0        0        0   202079 2023-04-08 18:52:13.418738 kavk_api-0.9.7.3/kavk_api/types/methods.py
+-rw-r--r--   0        0        0   144553 2023-04-08 11:31:33.144480 kavk_api-0.9.7.3/kavk_api/types/objects.py
+-rw-r--r--   0        0        0    43554 2023-04-08 11:31:33.145480 kavk_api-0.9.7.3/kavk_api/types/responses.py
+-rw-r--r--   0        0        0      123 2023-04-08 11:31:33.145480 kavk_api-0.9.7.3/kavk_api/utils.py
+-rw-r--r--   0        0        0      423 2023-04-09 07:58:26.451582 kavk_api-0.9.7.3/pyproject.toml
+-rw-r--r--   0        0        0     1689 1970-01-01 00:00:00.000000 kavk_api-0.9.7.3/PKG-INFO
```

### Comparing `kavk_api-0.9.7.2/LICENSE` & `kavk_api-0.9.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.2/README.rst` & `kavk_api-0.9.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.2/kavk_api/bot_longpoll.py` & `kavk_api-0.9.7.3/kavk_api/bot_longpoll.py`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.2/kavk_api/enums.py` & `kavk_api-0.9.7.3/kavk_api/enums.py`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.2/kavk_api/kavk_api.py` & `kavk_api-0.9.7.3/kavk_api/kavk_api.py`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.2/kavk_api/longpoll.py` & `kavk_api-0.9.7.3/kavk_api/longpoll.py`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.2/kavk_api/types/bot_events.py` & `kavk_api-0.9.7.3/kavk_api/types/bot_events.py`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.2/kavk_api/types/event_objects.py` & `kavk_api-0.9.7.3/kavk_api/types/event_objects.py`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.2/kavk_api/types/objects.py` & `kavk_api-0.9.7.3/kavk_api/types/objects.py`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.2/kavk_api/types/responses.py` & `kavk_api-0.9.7.3/kavk_api/types/responses.py`

 * *Files identical despite different names*

### Comparing `kavk_api-0.9.7.2/PKG-INFO` & `kavk_api-0.9.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kavk-api
-Version: 0.9.7.2
+Version: 0.9.7.3
 Summary: 
 License: MIT
 Author: Kravandir
 Author-email: kravandir@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

