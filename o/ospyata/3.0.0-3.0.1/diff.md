# Comparing `tmp/ospyata-3.0.0.tar.gz` & `tmp/ospyata-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ospyata-3.0.0.tar", last modified: Sat Apr  8 05:37:30 2023, max compression
+gzip compressed data, was "ospyata-3.0.1.tar", last modified: Sun Apr  9 04:55:10 2023, max compression
```

## Comparing `ospyata-3.0.0.tar` & `ospyata-3.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 aero      (1000) aero      (1000)        0 2023-04-08 05:37:30.202722 ospyata-3.0.0/
--rw-r--r--   0 aero      (1000) aero      (1000)     1074 2023-04-07 15:48:06.000000 ospyata-3.0.0/LICENSE
--rw-r--r--   0 aero      (1000) aero      (1000)     3045 2023-04-08 05:37:30.203722 ospyata-3.0.0/PKG-INFO
--rw-r--r--   0 aero      (1000) aero      (1000)     2188 2023-04-07 15:48:06.000000 ospyata-3.0.0/README.md
--rw-r--r--   0 aero      (1000) aero      (1000)       74 2023-04-08 05:37:30.203722 ospyata-3.0.0/setup.cfg
--rw-r--r--   0 aero      (1000) aero      (1000)     1548 2023-04-08 04:31:43.000000 ospyata-3.0.0/setup.py
-drwxr-xr-x   0 aero      (1000) aero      (1000)        0 2023-04-08 05:37:30.198722 ospyata-3.0.0/src/
-drwxr-xr-x   0 aero      (1000) aero      (1000)        0 2023-04-08 05:37:30.200722 ospyata-3.0.0/src/ospyata/
--rw-r--r--   0 aero      (1000) aero      (1000)      241 2023-04-07 15:48:06.000000 ospyata-3.0.0/src/ospyata/__init__.py
--rw-r--r--   0 aero      (1000) aero      (1000)      180 2023-04-07 16:12:04.000000 ospyata-3.0.0/src/ospyata/__version__.py
--rw-r--r--   0 aero      (1000) aero      (1000)     3164 2023-04-08 04:55:21.000000 ospyata-3.0.0/src/ospyata/osmata.py
-drwxr-xr-x   0 aero      (1000) aero      (1000)        0 2023-04-08 05:37:30.202722 ospyata-3.0.0/src/ospyata.egg-info/
--rw-r--r--   0 aero      (1000) aero      (1000)     3045 2023-04-08 05:37:30.000000 ospyata-3.0.0/src/ospyata.egg-info/PKG-INFO
--rw-r--r--   0 aero      (1000) aero      (1000)      283 2023-04-08 05:37:30.000000 ospyata-3.0.0/src/ospyata.egg-info/SOURCES.txt
--rw-r--r--   0 aero      (1000) aero      (1000)        1 2023-04-08 05:37:30.000000 ospyata-3.0.0/src/ospyata.egg-info/dependency_links.txt
--rw-r--r--   0 aero      (1000) aero      (1000)       11 2023-04-08 05:37:30.000000 ospyata-3.0.0/src/ospyata.egg-info/requires.txt
--rw-r--r--   0 aero      (1000) aero      (1000)        8 2023-04-08 05:37:30.000000 ospyata-3.0.0/src/ospyata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:55:10.065797 ospyata-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-09 04:55:00.000000 ospyata-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-09 04:55:10.065797 ospyata-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-09 04:55:00.000000 ospyata-3.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-09 04:55:10.065797 ospyata-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-09 04:55:00.000000 ospyata-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:55:10.065797 ospyata-3.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:55:10.065797 ospyata-3.0.1/src/ospyata/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-09 04:55:00.000000 ospyata-3.0.1/src/ospyata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-09 04:55:00.000000 ospyata-3.0.1/src/ospyata/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-09 04:55:00.000000 ospyata-3.0.1/src/ospyata/osmata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 04:55:10.065797 ospyata-3.0.1/src/ospyata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-09 04:55:10.000000 ospyata-3.0.1/src/ospyata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-09 04:55:10.000000 ospyata-3.0.1/src/ospyata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 04:55:10.000000 ospyata-3.0.1/src/ospyata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 04:55:10.000000 ospyata-3.0.1/src/ospyata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 04:55:10.000000 ospyata-3.0.1/src/ospyata.egg-info/top_level.txt
```

### Comparing `ospyata-3.0.0/LICENSE` & `ospyata-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ospyata-3.0.0/PKG-INFO` & `ospyata-3.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: ospyata
-Version: 3.0.0
+Version: 3.0.1
 Summary: Python library for the open source bookmark app Osmata.
 Home-page: https://github.com/aerocyber/ospyata
 Author: aerocyber
 License: MIT License
 Project-URL: Bug Reports, https://github.com/aerocyber/ospyata/issues
 Project-URL: Source, https://github.com/aerocyber/ospyata/
 Keywords: osmata,development,osmata-bindings,osmata-python-bindings,bookmarks
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.11, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ospyata
```

### Comparing `ospyata-3.0.0/README.md` & `ospyata-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ospyata-3.0.0/setup.py` & `ospyata-3.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,27 +15,26 @@
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 
 setup(
     name='ospyata',
     license="MIT License",
-    version='3.0.0',
+    version='3.0.1',
     description='Python library for the open source bookmark app Osmata.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/aerocyber/ospyata',
     author='aerocyber',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3 :: Only',
     ],
     keywords='osmata, development, osmata-bindings, osmata-python-bindings, bookmarks',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     python_requires='>=3.11, <4',
     install_requires=['validators'],
```

### Comparing `ospyata-3.0.0/src/ospyata/osmata.py` & `ospyata-3.0.1/src/ospyata/osmata.py`

 * *Files identical despite different names*

### Comparing `ospyata-3.0.0/src/ospyata.egg-info/PKG-INFO` & `ospyata-3.0.1/src/ospyata.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: ospyata
-Version: 3.0.0
+Version: 3.0.1
 Summary: Python library for the open source bookmark app Osmata.
 Home-page: https://github.com/aerocyber/ospyata
 Author: aerocyber
 License: MIT License
 Project-URL: Bug Reports, https://github.com/aerocyber/ospyata/issues
 Project-URL: Source, https://github.com/aerocyber/ospyata/
 Keywords: osmata,development,osmata-bindings,osmata-python-bindings,bookmarks
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.11, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ospyata
```

