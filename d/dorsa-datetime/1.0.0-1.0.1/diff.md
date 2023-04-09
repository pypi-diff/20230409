# Comparing `tmp/dorsa_datetime-1.0.0.tar.gz` & `tmp/dorsa_datetime-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dorsa_datetime-1.0.0.tar", last modified: Sat Apr  8 10:38:37 2023, max compression
+gzip compressed data, was "dorsa_datetime-1.0.1.tar", last modified: Sun Apr  9 06:59:31 2023, max compression
```

## Comparing `dorsa_datetime-1.0.0.tar` & `dorsa_datetime-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-08 10:38:37.191464 dorsa_datetime-1.0.0/
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)    10175 2023-04-07 08:19:35.000000 dorsa_datetime-1.0.0/LICENSE.txt
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1890 2023-04-08 10:38:37.191464 dorsa_datetime-1.0.0/PKG-INFO
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1033 2023-04-07 13:03:26.000000 dorsa_datetime-1.0.0/README.md
-drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-08 10:38:37.191464 dorsa_datetime-1.0.0/dorsa_datetime/
--rw-r--r--   0 reyhane   (1000) reyhane   (1000)      162 2023-04-08 09:55:51.000000 dorsa_datetime-1.0.0/dorsa_datetime/__init__.py
--rw-r--r--   0 reyhane   (1000) reyhane   (1000)     3457 2023-04-07 11:41:55.000000 dorsa_datetime-1.0.0/dorsa_datetime/datetime_funcs.py
-drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-08 10:38:37.191464 dorsa_datetime-1.0.0/dorsa_datetime.egg-info/
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1890 2023-04-08 10:38:37.000000 dorsa_datetime-1.0.0/dorsa_datetime.egg-info/PKG-INFO
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)      289 2023-04-08 10:38:37.000000 dorsa_datetime-1.0.0/dorsa_datetime.egg-info/SOURCES.txt
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)        1 2023-04-08 10:38:37.000000 dorsa_datetime-1.0.0/dorsa_datetime.egg-info/dependency_links.txt
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)        9 2023-04-08 10:38:37.000000 dorsa_datetime-1.0.0/dorsa_datetime.egg-info/requires.txt
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       15 2023-04-08 10:38:37.000000 dorsa_datetime-1.0.0/dorsa_datetime.egg-info/top_level.txt
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       79 2023-04-08 10:38:37.195463 dorsa_datetime-1.0.0/setup.cfg
--rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1734 2023-04-08 10:37:02.000000 dorsa_datetime-1.0.0/setup.py
+drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-09 06:59:31.266029 dorsa_datetime-1.0.1/
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)    10175 2023-04-07 08:19:35.000000 dorsa_datetime-1.0.1/LICENSE.txt
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1890 2023-04-09 06:59:31.266029 dorsa_datetime-1.0.1/PKG-INFO
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1033 2023-04-07 13:03:26.000000 dorsa_datetime-1.0.1/README.md
+drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-09 06:59:31.266029 dorsa_datetime-1.0.1/dorsa_datetime/
+-rw-r--r--   0 reyhane   (1000) reyhane   (1000)      162 2023-04-08 09:55:51.000000 dorsa_datetime-1.0.1/dorsa_datetime/__init__.py
+-rw-r--r--   0 reyhane   (1000) reyhane   (1000)     3457 2023-04-09 06:23:40.000000 dorsa_datetime-1.0.1/dorsa_datetime/datetime_funcs.py
+drwxrwxr-x   0 reyhane   (1000) reyhane   (1000)        0 2023-04-09 06:59:31.266029 dorsa_datetime-1.0.1/dorsa_datetime.egg-info/
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1890 2023-04-09 06:59:31.000000 dorsa_datetime-1.0.1/dorsa_datetime.egg-info/PKG-INFO
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)      289 2023-04-09 06:59:31.000000 dorsa_datetime-1.0.1/dorsa_datetime.egg-info/SOURCES.txt
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)        1 2023-04-09 06:59:31.000000 dorsa_datetime-1.0.1/dorsa_datetime.egg-info/dependency_links.txt
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       13 2023-04-09 06:59:31.000000 dorsa_datetime-1.0.1/dorsa_datetime.egg-info/requires.txt
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       15 2023-04-09 06:59:31.000000 dorsa_datetime-1.0.1/dorsa_datetime.egg-info/top_level.txt
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)       79 2023-04-09 06:59:31.266029 dorsa_datetime-1.0.1/setup.cfg
+-rw-rw-r--   0 reyhane   (1000) reyhane   (1000)     1738 2023-04-09 06:58:29.000000 dorsa_datetime-1.0.1/setup.py
```

### Comparing `dorsa_datetime-1.0.0/LICENSE.txt` & `dorsa_datetime-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dorsa_datetime-1.0.0/PKG-INFO` & `dorsa_datetime-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorsa_datetime
-Version: 1.0.0
+Version: 1.0.1
 Summary: Find current date and time
 Home-page: https://github.com/DORSA-co/modules/tree/main/DORSA_DateTime
 Author: Dorsa-co
 Author-email: info@dorsa-co.ir
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/DORSA-co/modules/tree/main/DORSA_DateTime/issues
 Keywords: pypi,dorsa_datetime,tutorial
```

### Comparing `dorsa_datetime-1.0.0/README.md` & `dorsa_datetime-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dorsa_datetime-1.0.0/dorsa_datetime/datetime_funcs.py` & `dorsa_datetime-1.0.1/dorsa_datetime/datetime_funcs.py`

 * *Files identical despite different names*

### Comparing `dorsa_datetime-1.0.0/dorsa_datetime.egg-info/PKG-INFO` & `dorsa_datetime-1.0.1/dorsa_datetime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorsa-datetime
-Version: 1.0.0
+Version: 1.0.1
 Summary: Find current date and time
 Home-page: https://github.com/DORSA-co/modules/tree/main/DORSA_DateTime
 Author: Dorsa-co
 Author-email: info@dorsa-co.ir
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/DORSA-co/modules/tree/main/DORSA_DateTime/issues
 Keywords: pypi,dorsa_datetime,tutorial
```

### Comparing `dorsa_datetime-1.0.0/setup.py` & `dorsa_datetime-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 # Reads the content of your README.md into a variable to be used in the setup below
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='dorsa_datetime',                           # should match the package folder
     packages=['dorsa_datetime'],                     # should match the package folder
-    version='1.0.0',                                # important for updates
+    version='1.0.1',                                # important for updates
     license='Apache License 2.0',                                  # should match your chosen license
     description='Find current date and time',
     long_description=long_description,              # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='Dorsa-co',
     author_email='info@dorsa-co.ir',
     url='https://github.com/DORSA-co/modules/tree/main/DORSA_DateTime', 
     project_urls = {                                # Optional
         "Bug Tracker": "https://github.com/DORSA-co/modules/tree/main/DORSA_DateTime/issues"
     },
-    install_requires=['requests'],                  # list all packages that your package uses
+    install_requires=['persiantools'],                  # list all packages that your package uses
     keywords=["pypi", "dorsa_datetime", "tutorial"], # descriptive meta-data
     classifiers=[                                   # https://pypi.org/classifiers
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Documentation',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
```

