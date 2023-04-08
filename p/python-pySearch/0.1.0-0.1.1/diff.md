# Comparing `tmp/python-pySearch-0.1.0.tar.gz` & `tmp/python-pySearch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-pySearch-0.1.0.tar", last modified: Sat Apr  8 20:47:19 2023, max compression
+gzip compressed data, was "python-pySearch-0.1.1.tar", last modified: Sat Apr  8 22:30:45 2023, max compression
```

## Comparing `python-pySearch-0.1.0.tar` & `python-pySearch-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 20:47:19.816768 python-pySearch-0.1.0/
--rw-rw-r--   0 root         (0) root         (0)    11357 2023-04-07 19:54:46.000000 python-pySearch-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1849 2023-04-08 20:47:19.816768 python-pySearch-0.1.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      944 2023-04-07 20:55:50.000000 python-pySearch-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 20:47:19.816768 python-pySearch-0.1.0/python-pySearch/
--rw-rw-r--   0 root         (0) root         (0)    11466 2023-04-07 19:42:17.000000 python-pySearch-0.1.0/python-pySearch/pySearch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 20:47:19.816768 python-pySearch-0.1.0/python_pySearch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1849 2023-04-08 20:47:19.000000 python-pySearch-0.1.0/python_pySearch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      210 2023-04-08 20:47:19.000000 python-pySearch-0.1.0/python_pySearch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-08 20:47:19.000000 python-pySearch-0.1.0/python_pySearch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-08 20:47:19.000000 python-pySearch-0.1.0/python_pySearch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-08 20:47:19.816768 python-pySearch-0.1.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1124 2023-04-08 20:46:11.000000 python-pySearch-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 22:30:45.264662 python-pySearch-0.1.1/
+-rw-rw-r--   0 root         (0) root         (0)    11357 2023-04-07 19:54:46.000000 python-pySearch-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-04-08 22:30:45.264662 python-pySearch-0.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      902 2023-04-08 22:13:42.000000 python-pySearch-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 22:30:45.264662 python-pySearch-0.1.1/python-pySearch/
+-rw-rw-r--   0 root         (0) root         (0)       22 2023-04-08 22:11:01.000000 python-pySearch-0.1.1/python-pySearch/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11466 2023-04-07 19:42:17.000000 python-pySearch-0.1.1/python-pySearch/pySearch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-08 22:30:45.264662 python-pySearch-0.1.1/python_pySearch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-04-08 22:30:45.000000 python-pySearch-0.1.1/python_pySearch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      238 2023-04-08 22:30:45.000000 python-pySearch-0.1.1/python_pySearch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-08 22:30:45.000000 python-pySearch-0.1.1/python_pySearch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-08 22:30:45.000000 python-pySearch-0.1.1/python_pySearch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-08 22:30:45.264662 python-pySearch-0.1.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1099 2023-04-08 22:20:47.000000 python-pySearch-0.1.1/setup.py
```

### Comparing `python-pySearch-0.1.0/LICENSE` & `python-pySearch-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-pySearch-0.1.0/PKG-INFO` & `python-pySearch-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-pySearch
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package to search on the internet from your code.
 Home-page: UNKNOWN
 Author: Huzaifa Asim
 Author-email: huzaifaasim017@outlook.com
 Maintainer: HunerOn
 Maintainer-email: toyoureply@gmail.com
 License: UNKNOWN
@@ -22,32 +22,29 @@
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pySearch
 pySearch is a Python package that enables seamless searching across popular online platforms directly from your code.
 
-version: `0.1.0`
+version: `0.1.1`
 
 ## Installation
-windows: `pip install pySearch`
-linux: `sudo pip3 install pySearch`
+- Windows: `pip install python-pySearch`
+- Linux: `sudo pip3 install python-pySearch`
 
 ## Developers
 - Huzaifa Asim ([@huzaifaasim017](https://github.com/huzaifaasim017))
 
 ## Contact
 If you have any questions or suggestions, please feel free to reach out to us at toyoureply@gmail.com or through [GitHub issues](https://github.com/huneron/pySearch/issues).
 
 ## Review
 We would love to hear your feedback on our projects! please leave a review [here](https://huneron.site/contact).
 
-## Last Update
-Last updated on: Friday, 8 April 2023 (GMT)
-
 ## LICENSE
 This project is licensed under the [Apache License 2.0](https://github.com/huneron/pySearch/blob/main/LICENSE) to ensure that it remains free and open for everyone.
 
 ---
 
 Created with :heart: by Team [HunerOn](https://huneroncodes.blogspot.com/)
```

### Comparing `python-pySearch-0.1.0/README.md` & `python-pySearch-0.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 # pySearch
 pySearch is a Python package that enables seamless searching across popular online platforms directly from your code.
 
-version: `0.1.0`
+version: `0.1.1`
 
 ## Installation
-windows: `pip install pySearch`
-linux: `sudo pip3 install pySearch`
+- Windows: `pip install python-pySearch`
+- Linux: `sudo pip3 install python-pySearch`
 
 ## Developers
 - Huzaifa Asim ([@huzaifaasim017](https://github.com/huzaifaasim017))
 
 ## Contact
 If you have any questions or suggestions, please feel free to reach out to us at toyoureply@gmail.com or through [GitHub issues](https://github.com/huneron/pySearch/issues).
 
 ## Review
 We would love to hear your feedback on our projects! please leave a review [here](https://huneron.site/contact).
 
-## Last Update
-Last updated on: Friday, 8 April 2023 (GMT)
-
 ## LICENSE
 This project is licensed under the [Apache License 2.0](https://github.com/huneron/pySearch/blob/main/LICENSE) to ensure that it remains free and open for everyone.
 
 ---
 
 Created with :heart: by Team [HunerOn](https://huneroncodes.blogspot.com/)
```

### Comparing `python-pySearch-0.1.0/python-pySearch/pySearch.py` & `python-pySearch-0.1.1/python-pySearch/pySearch.py`

 * *Files identical despite different names*

### Comparing `python-pySearch-0.1.0/python_pySearch.egg-info/PKG-INFO` & `python-pySearch-0.1.1/python_pySearch.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-pySearch
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package to search on the internet from your code.
 Home-page: UNKNOWN
 Author: Huzaifa Asim
 Author-email: huzaifaasim017@outlook.com
 Maintainer: HunerOn
 Maintainer-email: toyoureply@gmail.com
 License: UNKNOWN
@@ -22,32 +22,29 @@
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pySearch
 pySearch is a Python package that enables seamless searching across popular online platforms directly from your code.
 
-version: `0.1.0`
+version: `0.1.1`
 
 ## Installation
-windows: `pip install pySearch`
-linux: `sudo pip3 install pySearch`
+- Windows: `pip install python-pySearch`
+- Linux: `sudo pip3 install python-pySearch`
 
 ## Developers
 - Huzaifa Asim ([@huzaifaasim017](https://github.com/huzaifaasim017))
 
 ## Contact
 If you have any questions or suggestions, please feel free to reach out to us at toyoureply@gmail.com or through [GitHub issues](https://github.com/huneron/pySearch/issues).
 
 ## Review
 We would love to hear your feedback on our projects! please leave a review [here](https://huneron.site/contact).
 
-## Last Update
-Last updated on: Friday, 8 April 2023 (GMT)
-
 ## LICENSE
 This project is licensed under the [Apache License 2.0](https://github.com/huneron/pySearch/blob/main/LICENSE) to ensure that it remains free and open for everyone.
 
 ---
 
 Created with :heart: by Team [HunerOn](https://huneroncodes.blogspot.com/)
```

### Comparing `python-pySearch-0.1.0/setup.py` & `python-pySearch-0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='python-pySearch',
-    version='0.1.0',
+    version='0.1.1',
     description='A Python package to search on the internet from your code.',
     maintainer='HunerOn',
     maintainer_email='toyoureply@gmail.com',
     author='Huzaifa Asim',
     author_email='huzaifaasim017@outlook.com',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['python-pySearch'],
     py_modules=['python-pySearch'],
-    install_requires=[],
     classifiers=[
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Internet :: WWW/HTTP',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

