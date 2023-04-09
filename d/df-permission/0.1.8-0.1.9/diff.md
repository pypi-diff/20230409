# Comparing `tmp/df-permission-0.1.8.tar.gz` & `tmp/df-permission-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "df-permission-0.1.8.tar", last modified: Sun Apr  9 11:14:56 2023, max compression
+gzip compressed data, was "df-permission-0.1.9.tar", last modified: Sun Apr  9 11:34:41 2023, max compression
```

## Comparing `df-permission-0.1.8.tar` & `df-permission-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 11:14:56.272813 df-permission-0.1.8/
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2576 2023-04-09 11:14:56.272813 df-permission-0.1.8/PKG-INFO
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2028 2023-04-08 07:51:02.000000 df-permission-0.1.8/README.md
-drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 11:14:56.272813 df-permission-0.1.8/df_permission/
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        0 2023-04-07 13:57:28.000000 df-permission-0.1.8/df_permission/__init__.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       63 2023-04-07 13:57:28.000000 df-permission-0.1.8/df_permission/admin.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)      157 2023-04-07 13:57:28.000000 df-permission-0.1.8/df_permission/apps.py
-drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 11:14:56.272813 df-permission-0.1.8/df_permission/management/
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        0 2023-04-07 13:57:28.000000 df-permission-0.1.8/df_permission/management/__init__.py
-drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 11:14:56.272813 df-permission-0.1.8/df_permission/management/commands/
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        0 2023-04-07 13:57:28.000000 df-permission-0.1.8/df_permission/management/commands/__init__.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2941 2023-04-08 08:35:02.000000 df-permission-0.1.8/df_permission/management/commands/generate_model_field_permissions.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2675 2023-04-09 10:27:35.000000 df-permission-0.1.8/df_permission/management/commands/generate_serializer_field_permissions.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       57 2023-04-07 13:57:28.000000 df-permission-0.1.8/df_permission/models.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     4857 2023-04-09 11:14:30.000000 df-permission-0.1.8/df_permission/permissions.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       60 2023-04-07 13:57:28.000000 df-permission-0.1.8/df_permission/tests.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       77 2023-04-07 13:57:28.000000 df-permission-0.1.8/df_permission/variables.py
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       63 2023-04-07 13:57:28.000000 df-permission-0.1.8/df_permission/views.py
-drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 11:14:56.272813 df-permission-0.1.8/df_permission.egg-info/
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2576 2023-04-09 11:14:56.000000 df-permission-0.1.8/df_permission.egg-info/PKG-INFO
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)      627 2023-04-09 11:14:56.000000 df-permission-0.1.8/df_permission.egg-info/SOURCES.txt
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        1 2023-04-09 11:14:56.000000 df-permission-0.1.8/df_permission.egg-info/dependency_links.txt
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       27 2023-04-09 11:14:56.000000 df-permission-0.1.8/df_permission.egg-info/requires.txt
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       14 2023-04-09 11:14:56.000000 df-permission-0.1.8/df_permission.egg-info/top_level.txt
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       38 2023-04-09 11:14:56.276814 df-permission-0.1.8/setup.cfg
--rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     1062 2023-04-09 11:14:42.000000 df-permission-0.1.8/setup.py
+drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 11:34:41.709388 df-permission-0.1.9/
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2716 2023-04-09 11:34:41.709388 df-permission-0.1.9/PKG-INFO
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2168 2023-04-09 11:31:49.000000 df-permission-0.1.9/README.md
+drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 11:34:41.709388 df-permission-0.1.9/df_permission/
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        0 2023-04-07 13:57:28.000000 df-permission-0.1.9/df_permission/__init__.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       63 2023-04-07 13:57:28.000000 df-permission-0.1.9/df_permission/admin.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)      157 2023-04-07 13:57:28.000000 df-permission-0.1.9/df_permission/apps.py
+drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 11:34:41.709388 df-permission-0.1.9/df_permission/management/
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        0 2023-04-07 13:57:28.000000 df-permission-0.1.9/df_permission/management/__init__.py
+drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 11:34:41.709388 df-permission-0.1.9/df_permission/management/commands/
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        0 2023-04-07 13:57:28.000000 df-permission-0.1.9/df_permission/management/commands/__init__.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2941 2023-04-08 08:35:02.000000 df-permission-0.1.9/df_permission/management/commands/generate_model_field_permissions.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2675 2023-04-09 10:27:35.000000 df-permission-0.1.9/df_permission/management/commands/generate_serializer_field_permissions.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       57 2023-04-07 13:57:28.000000 df-permission-0.1.9/df_permission/models.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     4857 2023-04-09 11:14:30.000000 df-permission-0.1.9/df_permission/permissions.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       60 2023-04-07 13:57:28.000000 df-permission-0.1.9/df_permission/tests.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       77 2023-04-07 13:57:28.000000 df-permission-0.1.9/df_permission/variables.py
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       63 2023-04-07 13:57:28.000000 df-permission-0.1.9/df_permission/views.py
+drwxrwxr-x   0 asliddin  (1000) asliddin  (1000)        0 2023-04-09 11:34:41.709388 df-permission-0.1.9/df_permission.egg-info/
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     2716 2023-04-09 11:34:41.000000 df-permission-0.1.9/df_permission.egg-info/PKG-INFO
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)      627 2023-04-09 11:34:41.000000 df-permission-0.1.9/df_permission.egg-info/SOURCES.txt
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)        1 2023-04-09 11:34:41.000000 df-permission-0.1.9/df_permission.egg-info/dependency_links.txt
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       27 2023-04-09 11:34:41.000000 df-permission-0.1.9/df_permission.egg-info/requires.txt
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       14 2023-04-09 11:34:41.000000 df-permission-0.1.9/df_permission.egg-info/top_level.txt
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)       38 2023-04-09 11:34:41.709388 df-permission-0.1.9/setup.cfg
+-rw-rw-r--   0 asliddin  (1000) asliddin  (1000)     1062 2023-04-09 11:33:44.000000 df-permission-0.1.9/setup.py
```

### Comparing `df-permission-0.1.8/PKG-INFO` & `df-permission-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: df-permission
-Version: 0.1.8
+Version: 0.1.9
 Summary: Django field permission package
 Author: Maxmudov Asliddin
 Author-email: <asliddin750750@gmail.com>
 Keywords: python,field,permission,field permission,django field
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -25,16 +25,22 @@
 INSTALLED_APPS = [
     ...,
     'df_permission'
 ]
 ```
 
 ### Generate permissions
+For model fields:
 ```text
-./manage.py generate_df_permissions
+./manage.py generate_model_field_permissions
+```
+
+For serializer fields (not include model fields):
+```text
+./manage.py generate_serializer_field_permissions
 ```
 
 ### Attributes
 
 `df_method`
 - Method of action
 - Valid values are `create`, `update`, `retrieve`, `list`, `destroy`
```

### Comparing `df-permission-0.1.8/README.md` & `df-permission-0.1.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,22 @@
 INSTALLED_APPS = [
     ...,
     'df_permission'
 ]
 ```
 
 ### Generate permissions
+For model fields:
 ```text
-./manage.py generate_df_permissions
+./manage.py generate_model_field_permissions
+```
+
+For serializer fields (not include model fields):
+```text
+./manage.py generate_serializer_field_permissions
 ```
 
 ### Attributes
 
 `df_method`
 - Method of action
 - Valid values are `create`, `update`, `retrieve`, `list`, `destroy`
```

### Comparing `df-permission-0.1.8/df_permission/management/commands/generate_model_field_permissions.py` & `df-permission-0.1.9/df_permission/management/commands/generate_model_field_permissions.py`

 * *Files identical despite different names*

### Comparing `df-permission-0.1.8/df_permission/management/commands/generate_serializer_field_permissions.py` & `df-permission-0.1.9/df_permission/management/commands/generate_serializer_field_permissions.py`

 * *Files identical despite different names*

### Comparing `df-permission-0.1.8/df_permission/permissions.py` & `df-permission-0.1.9/df_permission/permissions.py`

 * *Files identical despite different names*

### Comparing `df-permission-0.1.8/df_permission.egg-info/PKG-INFO` & `df-permission-0.1.9/df_permission.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: df-permission
-Version: 0.1.8
+Version: 0.1.9
 Summary: Django field permission package
 Author: Maxmudov Asliddin
 Author-email: <asliddin750750@gmail.com>
 Keywords: python,field,permission,field permission,django field
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -25,16 +25,22 @@
 INSTALLED_APPS = [
     ...,
     'df_permission'
 ]
 ```
 
 ### Generate permissions
+For model fields:
 ```text
-./manage.py generate_df_permissions
+./manage.py generate_model_field_permissions
+```
+
+For serializer fields (not include model fields):
+```text
+./manage.py generate_serializer_field_permissions
 ```
 
 ### Attributes
 
 `df_method`
 - Method of action
 - Valid values are `create`, `update`, `retrieve`, `list`, `destroy`
```

### Comparing `df-permission-0.1.8/df_permission.egg-info/SOURCES.txt` & `df-permission-0.1.9/df_permission.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `df-permission-0.1.8/setup.py` & `df-permission-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 DESCRIPTION = "Django field permission package"
 
 
 def read(f):
     return open(f, "r", encoding="utf-8").read()
```

