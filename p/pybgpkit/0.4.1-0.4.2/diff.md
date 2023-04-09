# Comparing `tmp/pybgpkit-0.4.1.tar.gz` & `tmp/pybgpkit-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybgpkit-0.4.1.tar", last modified: Thu Mar 30 23:11:03 2023, max compression
+gzip compressed data, was "pybgpkit-0.4.2.tar", last modified: Sun Apr  9 06:13:07 2023, max compression
```

## Comparing `pybgpkit-0.4.1.tar` & `pybgpkit-0.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mingwei    (501) staff       (20)        0 2023-03-30 23:11:03.324802 pybgpkit-0.4.1/
--rw-r--r--   0 mingwei    (501) staff       (20)     1063 2022-01-31 02:29:25.000000 pybgpkit-0.4.1/LICENSE
--rw-r--r--   0 mingwei    (501) staff       (20)     7643 2023-03-30 23:11:03.324679 pybgpkit-0.4.1/PKG-INFO
--rw-r--r--   0 mingwei    (501) staff       (20)     7389 2023-03-30 05:13:34.000000 pybgpkit-0.4.1/README.md
-drwxr-xr-x   0 mingwei    (501) staff       (20)        0 2023-03-30 23:11:03.323784 pybgpkit-0.4.1/bgpkit/
--rw-r--r--   0 mingwei    (501) staff       (20)       98 2022-04-05 23:11:20.000000 pybgpkit-0.4.1/bgpkit/__init__.py
--rw-r--r--   0 mingwei    (501) staff       (20)     2081 2022-04-27 15:55:01.000000 pybgpkit-0.4.1/bgpkit/bgpkit_broker.py
--rw-r--r--   0 mingwei    (501) staff       (20)       34 2022-04-27 15:54:49.000000 pybgpkit-0.4.1/bgpkit/bgpkit_parser.py
--rw-r--r--   0 mingwei    (501) staff       (20)     2012 2022-04-05 22:19:49.000000 pybgpkit-0.4.1/bgpkit/bgpkit_roas.py
--rw-r--r--   0 mingwei    (501) staff       (20)     1273 2022-04-27 15:56:16.000000 pybgpkit-0.4.1/bgpkit/test_integration.py
-drwxr-xr-x   0 mingwei    (501) staff       (20)        0 2023-03-30 23:11:03.324522 pybgpkit-0.4.1/pybgpkit.egg-info/
--rw-r--r--   0 mingwei    (501) staff       (20)     7643 2023-03-30 23:11:03.000000 pybgpkit-0.4.1/pybgpkit.egg-info/PKG-INFO
--rw-r--r--   0 mingwei    (501) staff       (20)      316 2023-03-30 23:11:03.000000 pybgpkit-0.4.1/pybgpkit.egg-info/SOURCES.txt
--rw-r--r--   0 mingwei    (501) staff       (20)        1 2023-03-30 23:11:03.000000 pybgpkit-0.4.1/pybgpkit.egg-info/dependency_links.txt
--rw-r--r--   0 mingwei    (501) staff       (20)       49 2023-03-30 23:11:03.000000 pybgpkit-0.4.1/pybgpkit.egg-info/requires.txt
--rw-r--r--   0 mingwei    (501) staff       (20)        7 2023-03-30 23:11:03.000000 pybgpkit-0.4.1/pybgpkit.egg-info/top_level.txt
--rw-r--r--   0 mingwei    (501) staff       (20)      103 2022-02-01 17:35:12.000000 pybgpkit-0.4.1/pyproject.toml
--rw-r--r--   0 mingwei    (501) staff       (20)       38 2023-03-30 23:11:03.324836 pybgpkit-0.4.1/setup.cfg
--rw-r--r--   0 mingwei    (501) staff       (20)      709 2023-03-30 23:09:37.000000 pybgpkit-0.4.1/setup.py
+drwxr-xr-x   0 mingwei    (501) staff       (20)        0 2023-04-09 06:13:07.501584 pybgpkit-0.4.2/
+-rw-r--r--   0 mingwei    (501) staff       (20)     1063 2022-01-31 02:29:25.000000 pybgpkit-0.4.2/LICENSE
+-rw-r--r--   0 mingwei    (501) staff       (20)     7643 2023-04-09 06:13:07.501472 pybgpkit-0.4.2/PKG-INFO
+-rw-r--r--   0 mingwei    (501) staff       (20)     7389 2023-03-30 05:13:34.000000 pybgpkit-0.4.2/README.md
+drwxr-xr-x   0 mingwei    (501) staff       (20)        0 2023-04-09 06:13:07.500617 pybgpkit-0.4.2/bgpkit/
+-rw-r--r--   0 mingwei    (501) staff       (20)       98 2022-04-05 23:11:20.000000 pybgpkit-0.4.2/bgpkit/__init__.py
+-rw-r--r--   0 mingwei    (501) staff       (20)     2081 2022-04-27 15:55:01.000000 pybgpkit-0.4.2/bgpkit/bgpkit_broker.py
+-rw-r--r--   0 mingwei    (501) staff       (20)       34 2022-04-27 15:54:49.000000 pybgpkit-0.4.2/bgpkit/bgpkit_parser.py
+-rw-r--r--   0 mingwei    (501) staff       (20)     2012 2022-04-05 22:19:49.000000 pybgpkit-0.4.2/bgpkit/bgpkit_roas.py
+-rw-r--r--   0 mingwei    (501) staff       (20)     1273 2022-04-27 15:56:16.000000 pybgpkit-0.4.2/bgpkit/test_integration.py
+drwxr-xr-x   0 mingwei    (501) staff       (20)        0 2023-04-09 06:13:07.501325 pybgpkit-0.4.2/pybgpkit.egg-info/
+-rw-r--r--   0 mingwei    (501) staff       (20)     7643 2023-04-09 06:13:07.000000 pybgpkit-0.4.2/pybgpkit.egg-info/PKG-INFO
+-rw-r--r--   0 mingwei    (501) staff       (20)      316 2023-04-09 06:13:07.000000 pybgpkit-0.4.2/pybgpkit.egg-info/SOURCES.txt
+-rw-r--r--   0 mingwei    (501) staff       (20)        1 2023-04-09 06:13:07.000000 pybgpkit-0.4.2/pybgpkit.egg-info/dependency_links.txt
+-rw-r--r--   0 mingwei    (501) staff       (20)       49 2023-04-09 06:13:07.000000 pybgpkit-0.4.2/pybgpkit.egg-info/requires.txt
+-rw-r--r--   0 mingwei    (501) staff       (20)        7 2023-04-09 06:13:07.000000 pybgpkit-0.4.2/pybgpkit.egg-info/top_level.txt
+-rw-r--r--   0 mingwei    (501) staff       (20)      103 2022-02-01 17:35:12.000000 pybgpkit-0.4.2/pyproject.toml
+-rw-r--r--   0 mingwei    (501) staff       (20)       38 2023-04-09 06:13:07.501617 pybgpkit-0.4.2/setup.cfg
+-rw-r--r--   0 mingwei    (501) staff       (20)      709 2023-04-09 06:12:48.000000 pybgpkit-0.4.2/setup.py
```

### Comparing `pybgpkit-0.4.1/LICENSE` & `pybgpkit-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybgpkit-0.4.1/PKG-INFO` & `pybgpkit-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybgpkit
-Version: 0.4.1
+Version: 0.4.2
 Summary: BGPKIT tools Python bindings
 Home-page: https://github.com/bgpkit/pybgpkit
 Author: Mingwei Zhang
 Author-email: mingwei@bgpkit.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pybgpkit-0.4.1/README.md` & `pybgpkit-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pybgpkit-0.4.1/bgpkit/bgpkit_broker.py` & `pybgpkit-0.4.2/bgpkit/bgpkit_broker.py`

 * *Files identical despite different names*

### Comparing `pybgpkit-0.4.1/bgpkit/bgpkit_roas.py` & `pybgpkit-0.4.2/bgpkit/bgpkit_roas.py`

 * *Files identical despite different names*

### Comparing `pybgpkit-0.4.1/bgpkit/test_integration.py` & `pybgpkit-0.4.2/bgpkit/test_integration.py`

 * *Files identical despite different names*

### Comparing `pybgpkit-0.4.1/pybgpkit.egg-info/PKG-INFO` & `pybgpkit-0.4.2/pybgpkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybgpkit
-Version: 0.4.1
+Version: 0.4.2
 Summary: BGPKIT tools Python bindings
 Home-page: https://github.com/bgpkit/pybgpkit
 Author: Mingwei Zhang
 Author-email: mingwei@bgpkit.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pybgpkit-0.4.1/setup.py` & `pybgpkit-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name='pybgpkit',
-    version='0.4.1',
+    version='0.4.2',
     description='BGPKIT tools Python bindings',
     url='https://github.com/bgpkit/pybgpkit',
     author='Mingwei Zhang',
     author_email='mingwei@bgpkit.com',
     packages=setuptools.find_packages(),
     include_package_data=True,
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         # available on pip
         'dataclasses_json',
-        'pybgpkit-parser==0.4.1',
+        'pybgpkit-parser==0.4.2',
         'requests',
     ]
 )
```

