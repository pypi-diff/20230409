# Comparing `tmp/django-muid-1.0.3.tar.gz` & `tmp/django-muid-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-muid-1.0.3.tar", last modified: Sun Apr  9 19:07:42 2023, max compression
+gzip compressed data, was "django-muid-1.0.4.tar", last modified: Sun Apr  9 19:10:24 2023, max compression
```

## Comparing `django-muid-1.0.3.tar` & `django-muid-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 angelcamelot   (502) staff       (20)        0 2023-04-09 19:07:42.893980 django-muid-1.0.3/
--rw-r--r--   0 angelcamelot   (502) staff       (20)      831 2023-04-09 17:23:13.000000 django-muid-1.0.3/CONTRIBUTING.md
--rw-r--r--   0 angelcamelot   (502) staff       (20)      991 2023-04-09 17:28:06.000000 django-muid-1.0.3/LICENSE.md
--rw-r--r--   0 angelcamelot   (502) staff       (20)       60 2023-04-09 17:13:32.000000 django-muid-1.0.3/MANIFEST.in
--rw-r--r--   0 angelcamelot   (502) staff       (20)     2124 2023-04-09 19:07:42.893687 django-muid-1.0.3/PKG-INFO
--rw-r--r--   0 angelcamelot   (502) staff       (20)     1596 2023-04-09 18:56:41.000000 django-muid-1.0.3/README.md
-drwxr-xr-x   0 angelcamelot   (502) staff       (20)        0 2023-04-09 19:07:42.891404 django-muid-1.0.3/django_muid/
--rw-r--r--   0 angelcamelot   (502) staff       (20)       89 2023-04-09 19:07:07.000000 django-muid-1.0.3/django_muid/__init__.py
--rw-r--r--   0 angelcamelot   (502) staff       (20)     1423 2023-04-09 19:06:55.000000 django-muid-1.0.3/django_muid/fields.py
--rw-r--r--   0 angelcamelot   (502) staff       (20)     6189 2023-04-09 19:02:53.000000 django-muid-1.0.3/django_muid/muid.py
--rw-r--r--   0 angelcamelot   (502) staff       (20)      382 2023-04-09 19:06:32.000000 django-muid-1.0.3/django_muid/validators.py
-drwxr-xr-x   0 angelcamelot   (502) staff       (20)        0 2023-04-09 19:07:42.893290 django-muid-1.0.3/django_muid.egg-info/
--rw-r--r--   0 angelcamelot   (502) staff       (20)     2124 2023-04-09 19:07:42.000000 django-muid-1.0.3/django_muid.egg-info/PKG-INFO
--rw-r--r--   0 angelcamelot   (502) staff       (20)      323 2023-04-09 19:07:42.000000 django-muid-1.0.3/django_muid.egg-info/SOURCES.txt
--rw-r--r--   0 angelcamelot   (502) staff       (20)        1 2023-04-09 19:07:42.000000 django-muid-1.0.3/django_muid.egg-info/dependency_links.txt
--rw-r--r--   0 angelcamelot   (502) staff       (20)       23 2023-04-09 19:07:42.000000 django-muid-1.0.3/django_muid.egg-info/requires.txt
--rw-r--r--   0 angelcamelot   (502) staff       (20)       12 2023-04-09 19:07:42.000000 django-muid-1.0.3/django_muid.egg-info/top_level.txt
--rw-r--r--   0 angelcamelot   (502) staff       (20)       38 2023-04-09 19:07:42.894073 django-muid-1.0.3/setup.cfg
--rw-r--r--   0 angelcamelot   (502) staff       (20)      767 2023-04-09 19:07:38.000000 django-muid-1.0.3/setup.py
+drwxr-xr-x   0 angelcamelot   (502) staff       (20)        0 2023-04-09 19:10:24.582708 django-muid-1.0.4/
+-rw-r--r--   0 angelcamelot   (502) staff       (20)      831 2023-04-09 17:23:13.000000 django-muid-1.0.4/CONTRIBUTING.md
+-rw-r--r--   0 angelcamelot   (502) staff       (20)      991 2023-04-09 17:28:06.000000 django-muid-1.0.4/LICENSE.md
+-rw-r--r--   0 angelcamelot   (502) staff       (20)       60 2023-04-09 17:13:32.000000 django-muid-1.0.4/MANIFEST.in
+-rw-r--r--   0 angelcamelot   (502) staff       (20)     2124 2023-04-09 19:10:24.582307 django-muid-1.0.4/PKG-INFO
+-rw-r--r--   0 angelcamelot   (502) staff       (20)     1596 2023-04-09 18:56:41.000000 django-muid-1.0.4/README.md
+drwxr-xr-x   0 angelcamelot   (502) staff       (20)        0 2023-04-09 19:10:24.577978 django-muid-1.0.4/django_muid/
+-rw-r--r--   0 angelcamelot   (502) staff       (20)       92 2023-04-09 19:10:17.000000 django-muid-1.0.4/django_muid/__init__.py
+-rw-r--r--   0 angelcamelot   (502) staff       (20)     1425 2023-04-09 19:10:09.000000 django-muid-1.0.4/django_muid/fields.py
+-rw-r--r--   0 angelcamelot   (502) staff       (20)     6189 2023-04-09 19:02:53.000000 django-muid-1.0.4/django_muid/muid.py
+-rw-r--r--   0 angelcamelot   (502) staff       (20)      383 2023-04-09 19:09:57.000000 django-muid-1.0.4/django_muid/validators.py
+drwxr-xr-x   0 angelcamelot   (502) staff       (20)        0 2023-04-09 19:10:24.581475 django-muid-1.0.4/django_muid.egg-info/
+-rw-r--r--   0 angelcamelot   (502) staff       (20)     2124 2023-04-09 19:10:24.000000 django-muid-1.0.4/django_muid.egg-info/PKG-INFO
+-rw-r--r--   0 angelcamelot   (502) staff       (20)      323 2023-04-09 19:10:24.000000 django-muid-1.0.4/django_muid.egg-info/SOURCES.txt
+-rw-r--r--   0 angelcamelot   (502) staff       (20)        1 2023-04-09 19:10:24.000000 django-muid-1.0.4/django_muid.egg-info/dependency_links.txt
+-rw-r--r--   0 angelcamelot   (502) staff       (20)       23 2023-04-09 19:10:24.000000 django-muid-1.0.4/django_muid.egg-info/requires.txt
+-rw-r--r--   0 angelcamelot   (502) staff       (20)       12 2023-04-09 19:10:24.000000 django-muid-1.0.4/django_muid.egg-info/top_level.txt
+-rw-r--r--   0 angelcamelot   (502) staff       (20)       38 2023-04-09 19:10:24.582869 django-muid-1.0.4/setup.cfg
+-rw-r--r--   0 angelcamelot   (502) staff       (20)      767 2023-04-09 19:09:49.000000 django-muid-1.0.4/setup.py
```

### Comparing `django-muid-1.0.3/CONTRIBUTING.md` & `django-muid-1.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-muid-1.0.3/LICENSE.md` & `django-muid-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-muid-1.0.3/PKG-INFO` & `django-muid-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-muid
-Version: 1.0.3
+Version: 1.0.4
 Summary: MUID field for Django
 Home-page: https://github.com/angelcamelot/django-muid
 Author: Angel Camelot
 Author-email: dupeyron.camelot@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-muid-1.0.3/README.md` & `django-muid-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `django-muid-1.0.3/django_muid/fields.py` & `django-muid-1.0.4/django_muid/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.db.models import Field
-from muid import MUID
-from validators import muid_validator
+from .muid import MUID
+from .validators import muid_validator
 
 class MUIDField(Field):
     description = "MUID field"
 
     def __init__(self, *args, **kwargs):
         kwargs.setdefault('max_length', 16)
         super().__init__(*args, **kwargs)
```

### Comparing `django-muid-1.0.3/django_muid/muid.py` & `django-muid-1.0.4/django_muid/muid.py`

 * *Files identical despite different names*

### Comparing `django-muid-1.0.3/django_muid.egg-info/PKG-INFO` & `django-muid-1.0.4/django_muid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-muid
-Version: 1.0.3
+Version: 1.0.4
 Summary: MUID field for Django
 Home-page: https://github.com/angelcamelot/django-muid
 Author: Angel Camelot
 Author-email: dupeyron.camelot@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-muid-1.0.3/setup.py` & `django-muid-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="django-muid",
-    version="1.0.3",
+    version="1.0.4",
     description="MUID field for Django",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/angelcamelot/django-muid",
     author="Angel Camelot",
     author_email="dupeyron.camelot@gmail.com",
     packages=find_packages(),
```

