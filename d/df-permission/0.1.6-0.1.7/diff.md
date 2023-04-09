# Comparing `tmp/df-permission-0.1.6.tar.gz` & `tmp/df-permission-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "df-permission-0.1.6.tar", last modified: Sun Apr  9 10:31:06 2023, max compression
+gzip compressed data, was "df-permission-0.1.7.tar", last modified: Sun Apr  9 10:46:15 2023, max compression
```

## Comparing `df-permission-0.1.6.tar` & `df-permission-0.1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 10:31:06.838408 df-permission-0.1.6/
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2576 2023-04-09 10:31:06.838408 df-permission-0.1.6/PKG-INFO
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2028 2023-04-08 07:51:02.000000 df-permission-0.1.6/README.md
-drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 10:31:06.838408 df-permission-0.1.6/df_permission/
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        0 2023-04-07 13:57:28.000000 df-permission-0.1.6/df_permission/__init__.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       63 2023-04-07 13:57:28.000000 df-permission-0.1.6/df_permission/admin.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)      157 2023-04-07 13:57:28.000000 df-permission-0.1.6/df_permission/apps.py
-drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 10:31:06.838408 df-permission-0.1.6/df_permission/management/
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        0 2023-04-07 13:57:28.000000 df-permission-0.1.6/df_permission/management/__init__.py
-drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 10:31:06.838408 df-permission-0.1.6/df_permission/management/commands/
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        0 2023-04-07 13:57:28.000000 df-permission-0.1.6/df_permission/management/commands/__init__.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2941 2023-04-08 08:35:02.000000 df-permission-0.1.6/df_permission/management/commands/generate_model_field_permissions.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2675 2023-04-09 10:27:35.000000 df-permission-0.1.6/df_permission/management/commands/generate_serializer_field_permissions.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       57 2023-04-07 13:57:28.000000 df-permission-0.1.6/df_permission/models.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     4294 2023-04-08 07:49:58.000000 df-permission-0.1.6/df_permission/permissions.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       60 2023-04-07 13:57:28.000000 df-permission-0.1.6/df_permission/tests.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       77 2023-04-07 13:57:28.000000 df-permission-0.1.6/df_permission/variables.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       63 2023-04-07 13:57:28.000000 df-permission-0.1.6/df_permission/views.py
-drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 10:31:06.838408 df-permission-0.1.6/df_permission.egg-info/
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2576 2023-04-09 10:31:06.000000 df-permission-0.1.6/df_permission.egg-info/PKG-INFO
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)      627 2023-04-09 10:31:06.000000 df-permission-0.1.6/df_permission.egg-info/SOURCES.txt
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        1 2023-04-09 10:31:06.000000 df-permission-0.1.6/df_permission.egg-info/dependency_links.txt
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       27 2023-04-09 10:31:06.000000 df-permission-0.1.6/df_permission.egg-info/requires.txt
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       14 2023-04-09 10:31:06.000000 df-permission-0.1.6/df_permission.egg-info/top_level.txt
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       38 2023-04-09 10:31:06.838408 df-permission-0.1.6/setup.cfg
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     1062 2023-04-09 10:30:14.000000 df-permission-0.1.6/setup.py
+drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 10:46:15.055793 df-permission-0.1.7/
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2576 2023-04-09 10:46:15.055793 df-permission-0.1.7/PKG-INFO
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2028 2023-04-08 07:51:02.000000 df-permission-0.1.7/README.md
+drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 10:46:15.051793 df-permission-0.1.7/df_permission/
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        0 2023-04-07 13:57:28.000000 df-permission-0.1.7/df_permission/__init__.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       63 2023-04-07 13:57:28.000000 df-permission-0.1.7/df_permission/admin.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)      157 2023-04-07 13:57:28.000000 df-permission-0.1.7/df_permission/apps.py
+drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 10:46:15.055793 df-permission-0.1.7/df_permission/management/
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        0 2023-04-07 13:57:28.000000 df-permission-0.1.7/df_permission/management/__init__.py
+drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 10:46:15.055793 df-permission-0.1.7/df_permission/management/commands/
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        0 2023-04-07 13:57:28.000000 df-permission-0.1.7/df_permission/management/commands/__init__.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2941 2023-04-08 08:35:02.000000 df-permission-0.1.7/df_permission/management/commands/generate_model_field_permissions.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2675 2023-04-09 10:27:35.000000 df-permission-0.1.7/df_permission/management/commands/generate_serializer_field_permissions.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       57 2023-04-07 13:57:28.000000 df-permission-0.1.7/df_permission/models.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     4447 2023-04-09 10:45:49.000000 df-permission-0.1.7/df_permission/permissions.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       60 2023-04-07 13:57:28.000000 df-permission-0.1.7/df_permission/tests.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       77 2023-04-07 13:57:28.000000 df-permission-0.1.7/df_permission/variables.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       63 2023-04-07 13:57:28.000000 df-permission-0.1.7/df_permission/views.py
+drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 10:46:15.051793 df-permission-0.1.7/df_permission.egg-info/
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2576 2023-04-09 10:46:14.000000 df-permission-0.1.7/df_permission.egg-info/PKG-INFO
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)      627 2023-04-09 10:46:14.000000 df-permission-0.1.7/df_permission.egg-info/SOURCES.txt
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        1 2023-04-09 10:46:14.000000 df-permission-0.1.7/df_permission.egg-info/dependency_links.txt
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       27 2023-04-09 10:46:14.000000 df-permission-0.1.7/df_permission.egg-info/requires.txt
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       14 2023-04-09 10:46:14.000000 df-permission-0.1.7/df_permission.egg-info/top_level.txt
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       38 2023-04-09 10:46:15.055793 df-permission-0.1.7/setup.cfg
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     1062 2023-04-09 10:46:04.000000 df-permission-0.1.7/setup.py
```

### Comparing `df-permission-0.1.6/PKG-INFO` & `df-permission-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: df-permission
-Version: 0.1.6
+Version: 0.1.7
 Summary: Django field permission package
 Author: Maxmudov Asliddin
 Author-email: <asliddin750750@gmail.com>
 Keywords: python,field,permission,field permission,django field
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `df-permission-0.1.6/README.md` & `df-permission-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `df-permission-0.1.6/df_permission/management/commands/generate_model_field_permissions.py` & `df-permission-0.1.7/df_permission/management/commands/generate_model_field_permissions.py`

 * *Files identical despite different names*

### Comparing `df-permission-0.1.6/df_permission/management/commands/generate_serializer_field_permissions.py` & `df-permission-0.1.7/df_permission/management/commands/generate_serializer_field_permissions.py`

 * *Files identical despite different names*

### Comparing `df-permission-0.1.6/df_permission/permissions.py` & `df-permission-0.1.7/df_permission/permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,18 +45,21 @@
         """
         if hasattr(view, 'df_fields'):
             fields = view.df_fields
         elif hasattr(view, 'get_serializer'):
             serializer = view.get_serializer()
             serializer_fields = list(serializer.fields.keys())
 
-            model_fields = self._get_model_fields(view)
-
-            # get fields only available in model
-            fields = [field for field in serializer_fields if field in model_fields]
+            # version >= 0.1.6 (available for serializer fields)
+            fields = serializer_fields
+            # version < 0.1.6
+            # model_fields = self._get_model_fields(view)
+            #
+            # # get fields only available in model
+            # fields = [field for field in serializer_fields if field in model_fields]
         else:
             raise AttributeError('df_fields is required')
 
         return fields
 
     @staticmethod
     def _get_method(view):
```

### Comparing `df-permission-0.1.6/df_permission.egg-info/PKG-INFO` & `df-permission-0.1.7/df_permission.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: df-permission
-Version: 0.1.6
+Version: 0.1.7
 Summary: Django field permission package
 Author: Maxmudov Asliddin
 Author-email: <asliddin750750@gmail.com>
 Keywords: python,field,permission,field permission,django field
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `df-permission-0.1.6/df_permission.egg-info/SOURCES.txt` & `df-permission-0.1.7/df_permission.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `df-permission-0.1.6/setup.py` & `df-permission-0.1.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.1.6"
+VERSION = "0.1.7"
 DESCRIPTION = "Django field permission package"
 
 
 def read(f):
     return open(f, "r", encoding="utf-8").read()
```

