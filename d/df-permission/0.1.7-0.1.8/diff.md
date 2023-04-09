# Comparing `tmp/df-permission-0.1.7.tar.gz` & `tmp/df-permission-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "df-permission-0.1.7.tar", last modified: Sun Apr  9 10:46:15 2023, max compression
+gzip compressed data, was "df-permission-0.1.8.tar", last modified: Sun Apr  9 11:14:56 2023, max compression
```

## Comparing `df-permission-0.1.7.tar` & `df-permission-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 10:46:15.055793 df-permission-0.1.7/
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2576 2023-04-09 10:46:15.055793 df-permission-0.1.7/PKG-INFO
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2028 2023-04-08 07:51:02.000000 df-permission-0.1.7/README.md
-drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 10:46:15.051793 df-permission-0.1.7/df_permission/
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        0 2023-04-07 13:57:28.000000 df-permission-0.1.7/df_permission/__init__.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       63 2023-04-07 13:57:28.000000 df-permission-0.1.7/df_permission/admin.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)      157 2023-04-07 13:57:28.000000 df-permission-0.1.7/df_permission/apps.py
-drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 10:46:15.055793 df-permission-0.1.7/df_permission/management/
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        0 2023-04-07 13:57:28.000000 df-permission-0.1.7/df_permission/management/__init__.py
-drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 10:46:15.055793 df-permission-0.1.7/df_permission/management/commands/
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        0 2023-04-07 13:57:28.000000 df-permission-0.1.7/df_permission/management/commands/__init__.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2941 2023-04-08 08:35:02.000000 df-permission-0.1.7/df_permission/management/commands/generate_model_field_permissions.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2675 2023-04-09 10:27:35.000000 df-permission-0.1.7/df_permission/management/commands/generate_serializer_field_permissions.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       57 2023-04-07 13:57:28.000000 df-permission-0.1.7/df_permission/models.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     4447 2023-04-09 10:45:49.000000 df-permission-0.1.7/df_permission/permissions.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       60 2023-04-07 13:57:28.000000 df-permission-0.1.7/df_permission/tests.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       77 2023-04-07 13:57:28.000000 df-permission-0.1.7/df_permission/variables.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       63 2023-04-07 13:57:28.000000 df-permission-0.1.7/df_permission/views.py
-drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 10:46:15.051793 df-permission-0.1.7/df_permission.egg-info/
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2576 2023-04-09 10:46:14.000000 df-permission-0.1.7/df_permission.egg-info/PKG-INFO
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)      627 2023-04-09 10:46:14.000000 df-permission-0.1.7/df_permission.egg-info/SOURCES.txt
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        1 2023-04-09 10:46:14.000000 df-permission-0.1.7/df_permission.egg-info/dependency_links.txt
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       27 2023-04-09 10:46:14.000000 df-permission-0.1.7/df_permission.egg-info/requires.txt
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       14 2023-04-09 10:46:14.000000 df-permission-0.1.7/df_permission.egg-info/top_level.txt
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       38 2023-04-09 10:46:15.055793 df-permission-0.1.7/setup.cfg
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     1062 2023-04-09 10:46:04.000000 df-permission-0.1.7/setup.py
+drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 11:14:56.272813 df-permission-0.1.8/
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2576 2023-04-09 11:14:56.272813 df-permission-0.1.8/PKG-INFO
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2028 2023-04-08 07:51:02.000000 df-permission-0.1.8/README.md
+drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 11:14:56.272813 df-permission-0.1.8/df_permission/
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        0 2023-04-07 13:57:28.000000 df-permission-0.1.8/df_permission/__init__.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       63 2023-04-07 13:57:28.000000 df-permission-0.1.8/df_permission/admin.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)      157 2023-04-07 13:57:28.000000 df-permission-0.1.8/df_permission/apps.py
+drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 11:14:56.272813 df-permission-0.1.8/df_permission/management/
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        0 2023-04-07 13:57:28.000000 df-permission-0.1.8/df_permission/management/__init__.py
+drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 11:14:56.272813 df-permission-0.1.8/df_permission/management/commands/
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        0 2023-04-07 13:57:28.000000 df-permission-0.1.8/df_permission/management/commands/__init__.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2941 2023-04-08 08:35:02.000000 df-permission-0.1.8/df_permission/management/commands/generate_model_field_permissions.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2675 2023-04-09 10:27:35.000000 df-permission-0.1.8/df_permission/management/commands/generate_serializer_field_permissions.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       57 2023-04-07 13:57:28.000000 df-permission-0.1.8/df_permission/models.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     4857 2023-04-09 11:14:30.000000 df-permission-0.1.8/df_permission/permissions.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       60 2023-04-07 13:57:28.000000 df-permission-0.1.8/df_permission/tests.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       77 2023-04-07 13:57:28.000000 df-permission-0.1.8/df_permission/variables.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       63 2023-04-07 13:57:28.000000 df-permission-0.1.8/df_permission/views.py
+drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 11:14:56.272813 df-permission-0.1.8/df_permission.egg-info/
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2576 2023-04-09 11:14:56.000000 df-permission-0.1.8/df_permission.egg-info/PKG-INFO
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)      627 2023-04-09 11:14:56.000000 df-permission-0.1.8/df_permission.egg-info/SOURCES.txt
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        1 2023-04-09 11:14:56.000000 df-permission-0.1.8/df_permission.egg-info/dependency_links.txt
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       27 2023-04-09 11:14:56.000000 df-permission-0.1.8/df_permission.egg-info/requires.txt
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       14 2023-04-09 11:14:56.000000 df-permission-0.1.8/df_permission.egg-info/top_level.txt
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       38 2023-04-09 11:14:56.276814 df-permission-0.1.8/setup.cfg
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     1062 2023-04-09 11:14:42.000000 df-permission-0.1.8/setup.py
```

### Comparing `df-permission-0.1.7/PKG-INFO` & `df-permission-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: df-permission
-Version: 0.1.7
+Version: 0.1.8
 Summary: Django field permission package
 Author: Maxmudov Asliddin
 Author-email: <asliddin750750@gmail.com>
 Keywords: python,field,permission,field permission,django field
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `df-permission-0.1.7/README.md` & `df-permission-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `df-permission-0.1.7/df_permission/management/commands/generate_model_field_permissions.py` & `df-permission-0.1.8/df_permission/management/commands/generate_model_field_permissions.py`

 * *Files identical despite different names*

### Comparing `df-permission-0.1.7/df_permission/management/commands/generate_serializer_field_permissions.py` & `df-permission-0.1.8/df_permission/management/commands/generate_serializer_field_permissions.py`

 * *Files identical despite different names*

### Comparing `df-permission-0.1.7/df_permission/permissions.py` & `df-permission-0.1.8/df_permission/permissions.py`

 * *Files 10% similar despite different names*

```diff
@@ -100,17 +100,26 @@
         return str(model._meta.model_name).lower()
 
     def _get_required_perms(self, view, fields):
         """
         Required permissions for view
         """
         df_method = self._get_method(view)
-        df_model = self._get_model_name(view)
+        df_model_name = self._get_model_name(view)
+        df_model = self._get_model(view)
+        model_fields = df_model._meta.get_fields()
+        model_fields = [field.name for field in model_fields]
+        serializer = view.serializer_class.__name__.lower()
 
-        required_perms = [f'{df_method}--{df_model}--{field}' for field in fields]
+        required_perms = []
+        for field in fields:
+            if field not in model_fields:
+                required_perms.append(f'{df_method}--{serializer}--{field}')
+            else:
+                required_perms.append(f'{df_method}--{df_model_name}--{field}')
         return required_perms
 
     @staticmethod
     def _get_user_perms(request):
         return get_user_perms(request)
 
     @staticmethod
```

### Comparing `df-permission-0.1.7/df_permission.egg-info/PKG-INFO` & `df-permission-0.1.8/df_permission.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: df-permission
-Version: 0.1.7
+Version: 0.1.8
 Summary: Django field permission package
 Author: Maxmudov Asliddin
 Author-email: <asliddin750750@gmail.com>
 Keywords: python,field,permission,field permission,django field
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `df-permission-0.1.7/df_permission.egg-info/SOURCES.txt` & `df-permission-0.1.8/df_permission.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `df-permission-0.1.7/setup.py` & `df-permission-0.1.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.1.7"
+VERSION = "0.1.8"
 DESCRIPTION = "Django field permission package"
 
 
 def read(f):
     return open(f, "r", encoding="utf-8").read()
```

