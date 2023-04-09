# Comparing `tmp/tensorscout-2.2.0.tar.gz` & `tmp/tensorscout-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorscout-2.2.0.tar", max compression
+gzip compressed data, was "tensorscout-2.3.0.tar", max compression
```

## Comparing `tensorscout-2.2.0.tar` & `tensorscout-2.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1077 2022-05-25 22:13:34.760586 tensorscout-2.2.0/LICENSE
--rw-r--r--   0        0        0     1019 2023-04-03 22:00:18.346311 tensorscout-2.2.0/README.md
--rw-r--r--   0        0        0      460 2023-04-09 15:56:57.577035 tensorscout-2.2.0/pyproject.toml
--rw-r--r--   0        0        0       30 2023-04-02 04:18:08.970296 tensorscout-2.2.0/tensorscout/__init__.py
--rwxr-xr-x   0        0        0     7010 2023-04-09 17:28:41.933779 tensorscout-2.2.0/tensorscout/main.py
--rw-r--r--   0        0        0     1816 1970-01-01 00:00:00.000000 tensorscout-2.2.0/setup.py
--rw-r--r--   0        0        0     1796 1970-01-01 00:00:00.000000 tensorscout-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2022-05-25 22:13:34.760586 tensorscout-2.3.0/LICENSE
+-rw-r--r--   0        0        0     1019 2023-04-03 22:00:18.346311 tensorscout-2.3.0/README.md
+-rw-r--r--   0        0        0      460 2023-04-09 20:22:21.978086 tensorscout-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-04-02 04:18:08.970296 tensorscout-2.3.0/tensorscout/__init__.py
+-rwxr-xr-x   0        0        0     5463 2023-04-09 19:57:13.122902 tensorscout-2.3.0/tensorscout/main.py
+-rw-r--r--   0        0        0     1816 1970-01-01 00:00:00.000000 tensorscout-2.3.0/setup.py
+-rw-r--r--   0        0        0     1796 1970-01-01 00:00:00.000000 tensorscout-2.3.0/PKG-INFO
```

### Comparing `tensorscout-2.2.0/LICENSE` & `tensorscout-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorscout-2.2.0/README.md` & `tensorscout-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tensorscout-2.2.0/setup.py` & `tensorscout-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'numpy>=1.24.2,<2.0.0',
  'pathos>=0.3.0,<0.4.0',
  'scipy>=1.10.1,<2.0.0',
  'timethis>=0.1.1,<0.2.0']
 
 setup_kwargs = {
     'name': 'tensorscout',
-    'version': '2.2.0',
+    'version': '2.3.0',
     'description': 'A Python library for tensor operations powered by parallel processing',
     'long_description': '# tensorscout\n\n[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](https://raw.githubusercontent.com/andrewrgarcia/tensorscout/main/LICENSE)\n[![Documentation Status](https://readthedocs.org/projects/tensorscout/badge/?version=latest)](https://tensorscout.readthedocs.io/en/latest/?badge=latest)\n\nA Python library for tensor operations powered by parallel processing.\n\n<a href="https://tensorscout.readthedocs.io"><img src="https://raw.githubusercontent.com/andrewrgarcia/tensorscout/main/icon_scout.png" width="400"></a>\n\n\n## Installation\n\n```ruby\npip install tensorscout\n```\n\nIt is recommended you run voxelmap using a `virtualenv` virtual environment. To do so, follow the below simple protocol to create the virtual environment, run it, and install the package there:\n\n```ruby \nvirtualenv venv\nsource venv/bin/activate\npip install tensorscout\n```\nTo exit the virtual environment, simply type `deactivate`. To access it at any other time again, enter with the above `source venv...` command. \n',
     'author': 'andrewrgarcia',
     'author_email': 'garcia.gtr@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['tensorscout'] package_data = \ {'': ['*']} install_requires = \
 ['matplotlib>=3.7.1,<4.0.0', 'numpy>=1.24.2,<2.0.0', 'pathos>=0.3.0,<0.4.0',
 'scipy>=1.10.1,<2.0.0', 'timethis>=0.1.1,<0.2.0'] setup_kwargs = { 'name':
-'tensorscout', 'version': '2.2.0', 'description': 'A Python library for tensor
+'tensorscout', 'version': '2.3.0', 'description': 'A Python library for tensor
 operations powered by parallel processing', 'long_description': '#
 tensorscout\n\n[![License](http://img.shields.io/:license-mit-
 blue.svg?style=flat-square)](https://raw.githubusercontent.com/andrewrgarcia/
 tensorscout/main/LICENSE)\n[![Documentation Status](https://readthedocs.org/
 projects/tensorscout/badge/?version=latest)](https://
 tensorscout.readthedocs.io/en/latest/?badge=latest)\n\nA Python library for
 tensor operations powered by parallel processing.\n\n[https://
```

### Comparing `tensorscout-2.2.0/PKG-INFO` & `tensorscout-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorscout
-Version: 2.2.0
+Version: 2.3.0
 Summary: A Python library for tensor operations powered by parallel processing
 License: MIT
 Author: andrewrgarcia
 Author-email: garcia.gtr@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensorscout Version: 2.2.0 Summary: A Python
+Metadata-Version: 2.1 Name: tensorscout Version: 2.3.0 Summary: A Python
 library for tensor operations powered by parallel processing License: MIT
 Author: andrewrgarcia Author-email: garcia.gtr@gmail.com Requires-Python:
 >=3.8,<3.12 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-Dist: numpy
```

