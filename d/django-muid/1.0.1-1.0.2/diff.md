# Comparing `tmp/django-muid-1.0.1.tar.gz` & `tmp/django-muid-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-muid-1.0.1.tar", last modified: Sun Apr  9 18:40:53 2023, max compression
+gzip compressed data, was "django-muid-1.0.2.tar", last modified: Sun Apr  9 18:57:01 2023, max compression
```

## Comparing `django-muid-1.0.1.tar` & `django-muid-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 angelcamelot   (502) staff       (20)        0 2023-04-09 18:40:53.122532 django-muid-1.0.1/
--rw-r--r--   0 angelcamelot   (502) staff       (20)      831 2023-04-09 17:23:13.000000 django-muid-1.0.1/CONTRIBUTING.md
--rw-r--r--   0 angelcamelot   (502) staff       (20)      991 2023-04-09 17:28:06.000000 django-muid-1.0.1/LICENSE.md
--rw-r--r--   0 angelcamelot   (502) staff       (20)       60 2023-04-09 17:13:32.000000 django-muid-1.0.1/MANIFEST.in
--rw-r--r--   0 angelcamelot   (502) staff       (20)     2130 2023-04-09 18:40:53.122282 django-muid-1.0.1/PKG-INFO
--rw-r--r--   0 angelcamelot   (502) staff       (20)     1602 2023-04-09 17:31:47.000000 django-muid-1.0.1/README.md
-drwxr-xr-x   0 angelcamelot   (502) staff       (20)        0 2023-04-09 18:40:53.120601 django-muid-1.0.1/django-muid/
--rw-r--r--   0 angelcamelot   (502) staff       (20)       92 2023-04-09 17:10:16.000000 django-muid-1.0.1/django-muid/__init__.py
--rw-r--r--   0 angelcamelot   (502) staff       (20)     1425 2023-04-09 17:11:53.000000 django-muid-1.0.1/django-muid/fields.py
--rw-r--r--   0 angelcamelot   (502) staff       (20)        0 2023-04-09 17:08:54.000000 django-muid-1.0.1/django-muid/muid.py
--rw-r--r--   0 angelcamelot   (502) staff       (20)      383 2023-04-09 17:10:32.000000 django-muid-1.0.1/django-muid/validators.py
-drwxr-xr-x   0 angelcamelot   (502) staff       (20)        0 2023-04-09 18:40:53.121955 django-muid-1.0.1/django_muid.egg-info/
--rw-r--r--   0 angelcamelot   (502) staff       (20)     2130 2023-04-09 18:40:53.000000 django-muid-1.0.1/django_muid.egg-info/PKG-INFO
--rw-r--r--   0 angelcamelot   (502) staff       (20)      323 2023-04-09 18:40:53.000000 django-muid-1.0.1/django_muid.egg-info/SOURCES.txt
--rw-r--r--   0 angelcamelot   (502) staff       (20)        1 2023-04-09 18:40:53.000000 django-muid-1.0.1/django_muid.egg-info/dependency_links.txt
--rw-r--r--   0 angelcamelot   (502) staff       (20)       23 2023-04-09 18:40:53.000000 django-muid-1.0.1/django_muid.egg-info/requires.txt
--rw-r--r--   0 angelcamelot   (502) staff       (20)       12 2023-04-09 18:40:53.000000 django-muid-1.0.1/django_muid.egg-info/top_level.txt
--rw-r--r--   0 angelcamelot   (502) staff       (20)       38 2023-04-09 18:40:53.122618 django-muid-1.0.1/setup.cfg
--rw-r--r--   0 angelcamelot   (502) staff       (20)      909 2023-04-09 18:39:04.000000 django-muid-1.0.1/setup.py
+drwxr-xr-x   0 angelcamelot   (502) staff       (20)        0 2023-04-09 18:57:01.901017 django-muid-1.0.2/
+-rw-r--r--   0 angelcamelot   (502) staff       (20)      831 2023-04-09 17:23:13.000000 django-muid-1.0.2/CONTRIBUTING.md
+-rw-r--r--   0 angelcamelot   (502) staff       (20)      991 2023-04-09 17:28:06.000000 django-muid-1.0.2/LICENSE.md
+-rw-r--r--   0 angelcamelot   (502) staff       (20)       60 2023-04-09 17:13:32.000000 django-muid-1.0.2/MANIFEST.in
+-rw-r--r--   0 angelcamelot   (502) staff       (20)     2124 2023-04-09 18:57:01.900603 django-muid-1.0.2/PKG-INFO
+-rw-r--r--   0 angelcamelot   (502) staff       (20)     1596 2023-04-09 18:56:41.000000 django-muid-1.0.2/README.md
+drwxr-xr-x   0 angelcamelot   (502) staff       (20)        0 2023-04-09 18:57:01.897518 django-muid-1.0.2/django_muid/
+-rw-r--r--   0 angelcamelot   (502) staff       (20)       92 2023-04-09 17:10:16.000000 django-muid-1.0.2/django_muid/__init__.py
+-rw-r--r--   0 angelcamelot   (502) staff       (20)     1425 2023-04-09 17:11:53.000000 django-muid-1.0.2/django_muid/fields.py
+-rw-r--r--   0 angelcamelot   (502) staff       (20)        0 2023-04-09 17:08:54.000000 django-muid-1.0.2/django_muid/muid.py
+-rw-r--r--   0 angelcamelot   (502) staff       (20)      383 2023-04-09 17:10:32.000000 django-muid-1.0.2/django_muid/validators.py
+drwxr-xr-x   0 angelcamelot   (502) staff       (20)        0 2023-04-09 18:57:01.899930 django-muid-1.0.2/django_muid.egg-info/
+-rw-r--r--   0 angelcamelot   (502) staff       (20)     2124 2023-04-09 18:57:01.000000 django-muid-1.0.2/django_muid.egg-info/PKG-INFO
+-rw-r--r--   0 angelcamelot   (502) staff       (20)      323 2023-04-09 18:57:01.000000 django-muid-1.0.2/django_muid.egg-info/SOURCES.txt
+-rw-r--r--   0 angelcamelot   (502) staff       (20)        1 2023-04-09 18:57:01.000000 django-muid-1.0.2/django_muid.egg-info/dependency_links.txt
+-rw-r--r--   0 angelcamelot   (502) staff       (20)       23 2023-04-09 18:57:01.000000 django-muid-1.0.2/django_muid.egg-info/requires.txt
+-rw-r--r--   0 angelcamelot   (502) staff       (20)       12 2023-04-09 18:57:01.000000 django-muid-1.0.2/django_muid.egg-info/top_level.txt
+-rw-r--r--   0 angelcamelot   (502) staff       (20)       38 2023-04-09 18:57:01.901150 django-muid-1.0.2/setup.cfg
+-rw-r--r--   0 angelcamelot   (502) staff       (20)      767 2023-04-09 18:56:28.000000 django-muid-1.0.2/setup.py
```

### Comparing `django-muid-1.0.1/CONTRIBUTING.md` & `django-muid-1.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-muid-1.0.1/LICENSE.md` & `django-muid-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-muid-1.0.1/PKG-INFO` & `django-muid-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: django-muid
-Version: 1.0.1
+Version: 1.0.2
 Summary: MUID field for Django
 Home-page: https://github.com/angelcamelot/django-muid
 Author: Angel Camelot
 Author-email: dupeyron.camelot@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# Django MUID 1.0.0
+# Django MUID
     
 [![Build Status](https://travis-ci.org/bradleyayers/django-muid.svg?branch=master)](https://travis-ci.org/bradleyayers/django-muid)
 [![Coverage Status](https://coveralls.io/repos/github/bradleyayers/django-muid/badge.svg?branch=master)](https://coveralls.io/github/bradleyayers/django-muid?branch=master)
 [![PyPI version](https://badge.fury.io/py/django-muid.svg)](https://badge.fury.io/py/django-muid)
 [![PyPI](https://img.shields.io/pypi/pyversions/django-muid.svg)](https://pypi.python.org/pypi/django-muid)
 [![PyPI](https://img.shields.io/pypi/l/django-muid.svg)](https://pypi.python.org/pypi/django-muid)
```

### Comparing `django-muid-1.0.1/README.md` & `django-muid-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Django MUID 1.0.0
+# Django MUID
     
 [![Build Status](https://travis-ci.org/bradleyayers/django-muid.svg?branch=master)](https://travis-ci.org/bradleyayers/django-muid)
 [![Coverage Status](https://coveralls.io/repos/github/bradleyayers/django-muid/badge.svg?branch=master)](https://coveralls.io/github/bradleyayers/django-muid?branch=master)
 [![PyPI version](https://badge.fury.io/py/django-muid.svg)](https://badge.fury.io/py/django-muid)
 [![PyPI](https://img.shields.io/pypi/pyversions/django-muid.svg)](https://pypi.python.org/pypi/django-muid)
 [![PyPI](https://img.shields.io/pypi/l/django-muid.svg)](https://pypi.python.org/pypi/django-muid)
```

### Comparing `django-muid-1.0.1/django-muid/fields.py` & `django-muid-1.0.2/django_muid/fields.py`

 * *Files identical despite different names*

### Comparing `django-muid-1.0.1/django_muid.egg-info/PKG-INFO` & `django-muid-1.0.2/django_muid.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: django-muid
-Version: 1.0.1
+Version: 1.0.2
 Summary: MUID field for Django
 Home-page: https://github.com/angelcamelot/django-muid
 Author: Angel Camelot
 Author-email: dupeyron.camelot@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# Django MUID 1.0.0
+# Django MUID
     
 [![Build Status](https://travis-ci.org/bradleyayers/django-muid.svg?branch=master)](https://travis-ci.org/bradleyayers/django-muid)
 [![Coverage Status](https://coveralls.io/repos/github/bradleyayers/django-muid/badge.svg?branch=master)](https://coveralls.io/github/bradleyayers/django-muid?branch=master)
 [![PyPI version](https://badge.fury.io/py/django-muid.svg)](https://badge.fury.io/py/django-muid)
 [![PyPI](https://img.shields.io/pypi/pyversions/django-muid.svg)](https://pypi.python.org/pypi/django-muid)
 [![PyPI](https://img.shields.io/pypi/l/django-muid.svg)](https://pypi.python.org/pypi/django-muid)
```

### Comparing `django-muid-1.0.1/setup.py` & `django-muid-1.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="django-muid",
-    version="1.0.1",
+    version="1.0.2",
     description="MUID field for Django",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/angelcamelot/django-muid",
     author="Angel Camelot",
     author_email="dupeyron.camelot@gmail.com",
     packages=find_packages(),
@@ -19,12 +19,8 @@
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
     ],
     python_requires=">=3.6",
-    package_data={
-        "django-muid": ['django_muid-1.0.0.tar.gz', 'django_muid-1.0.0.tar.gz.asc'],
-    },
-    include_package_data=True,
 )
```

