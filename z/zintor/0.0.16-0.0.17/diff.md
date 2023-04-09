# Comparing `tmp/zintor-0.0.16.tar.gz` & `tmp/zintor-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zintor-0.0.16.tar", last modified: Wed Mar 29 02:05:02 2023, max compression
+gzip compressed data, was "zintor-0.0.17.tar", last modified: Sun Apr  9 15:10:19 2023, max compression
```

## Comparing `zintor-0.0.16.tar` & `zintor-0.0.17.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-03-29 02:05:02.849058 zintor-0.0.16/
--rw-r--r--   0 dzung     (1000) dzung     (1000)      383 2023-03-29 02:05:02.849058 zintor-0.0.16/PKG-INFO
--rw-r--r--   0 dzung     (1000) dzung     (1000)       38 2023-03-29 02:05:02.849058 zintor-0.0.16/setup.cfg
--rw-r--r--   0 dzung     (1000) dzung     (1000)     1362 2023-03-29 02:04:59.000000 zintor-0.0.16/setup.py
-drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-03-29 02:05:02.849058 zintor-0.0.16/zintor/
-drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-03-29 02:05:02.849058 zintor-0.0.16/zintor/src/
-drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-03-29 02:05:02.849058 zintor-0.0.16/zintor/src/zintor.egg-info/
--rw-r--r--   0 dzung     (1000) dzung     (1000)      383 2023-03-29 02:05:02.000000 zintor-0.0.16/zintor/src/zintor.egg-info/PKG-INFO
--rw-r--r--   0 dzung     (1000) dzung     (1000)      233 2023-03-29 02:05:02.000000 zintor-0.0.16/zintor/src/zintor.egg-info/SOURCES.txt
--rw-r--r--   0 dzung     (1000) dzung     (1000)        1 2023-03-29 02:05:02.000000 zintor-0.0.16/zintor/src/zintor.egg-info/dependency_links.txt
--rw-r--r--   0 dzung     (1000) dzung     (1000)       74 2023-03-29 02:05:02.000000 zintor-0.0.16/zintor/src/zintor.egg-info/requires.txt
--rw-r--r--   0 dzung     (1000) dzung     (1000)        7 2023-03-29 02:05:02.000000 zintor-0.0.16/zintor/src/zintor.egg-info/top_level.txt
--rw-r--r--   0 dzung     (1000) dzung     (1000)     3171 2023-03-29 01:39:43.000000 zintor-0.0.16/zintor/src/zintor.py
+drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-04-09 15:10:19.594263 zintor-0.0.17/
+-rw-r--r--   0 dzung     (1000) dzung     (1000)      383 2023-04-09 15:10:19.594263 zintor-0.0.17/PKG-INFO
+-rw-r--r--   0 dzung     (1000) dzung     (1000)       38 2023-04-09 15:10:19.594263 zintor-0.0.17/setup.cfg
+-rw-r--r--   0 dzung     (1000) dzung     (1000)     1362 2023-04-09 15:10:14.000000 zintor-0.0.17/setup.py
+drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-04-09 15:10:19.584263 zintor-0.0.17/zintor/
+drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-04-09 15:10:19.584263 zintor-0.0.17/zintor/src/
+drwxr-xr-x   0 dzung     (1000) dzung     (1000)        0 2023-04-09 15:10:19.594263 zintor-0.0.17/zintor/src/zintor.egg-info/
+-rw-r--r--   0 dzung     (1000) dzung     (1000)      383 2023-04-09 15:10:19.000000 zintor-0.0.17/zintor/src/zintor.egg-info/PKG-INFO
+-rw-r--r--   0 dzung     (1000) dzung     (1000)      233 2023-04-09 15:10:19.000000 zintor-0.0.17/zintor/src/zintor.egg-info/SOURCES.txt
+-rw-r--r--   0 dzung     (1000) dzung     (1000)        1 2023-04-09 15:10:19.000000 zintor-0.0.17/zintor/src/zintor.egg-info/dependency_links.txt
+-rw-r--r--   0 dzung     (1000) dzung     (1000)       74 2023-04-09 15:10:19.000000 zintor-0.0.17/zintor/src/zintor.egg-info/requires.txt
+-rw-r--r--   0 dzung     (1000) dzung     (1000)        7 2023-04-09 15:10:19.000000 zintor-0.0.17/zintor/src/zintor.egg-info/top_level.txt
+-rw-r--r--   0 dzung     (1000) dzung     (1000)     3130 2023-04-09 15:09:12.000000 zintor-0.0.17/zintor/src/zintor.py
```

### Comparing `zintor-0.0.16/setup.py` & `zintor-0.0.17/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="zintor",                             # This is the name of the package
-    version="0.0.16",                        # The initial release version
+    version="0.0.17",                        # The initial release version
     author="__Async__",                     # Full name of the author
     description="Python Admin Package",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `zintor-0.0.16/zintor/src/zintor.py` & `zintor-0.0.17/zintor/src/zintor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os.path as op
 from uuid import uuid4
 
 from flask import url_for, g, redirect, render_template, request
 from flask import has_app_context
 from flask_admin import Admin, AdminIndexView, helpers, expose
+from flask_admin.actions import action
 from flask_admin.model.form import InlineFormAdmin
 from flask_admin.contrib.sqla.filters import BaseSQLAFilter
 from flask_admin.contrib.sqla.filters import FilterEqual, BooleanEqualFilter
 from flask_sqlalchemy import SQLAlchemy
 from markupsafe import Markup
 from werkzeug.utils import secure_filename
 from werkzeug.security import generate_password_hash, check_password_hash
@@ -33,16 +34,14 @@
 class BaseView(ModelView):
     column_list = ('id', 'created_at', 'updated_at')
     column_labels = dict(
         id='#',
         created_at='登録日時',
         updated_at='更新日時',
     )
-    def is_accessible(self):
-        return login.current_user.is_authenticated
 
 class BaseInlineView(InlineFormAdmin):
     pass
 
 class ImageView(ModelView):
     def _list_thumbnail(view, context, model, name):
         if not model.path:
```

