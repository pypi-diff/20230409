# Comparing `tmp/primegenerators-0.0.1.tar.gz` & `tmp/primegenerators-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "primegenerators-0.0.1.tar", max compression
+gzip compressed data, was "primegenerators-0.0.2.tar", max compression
```

## Comparing `primegenerators-0.0.1.tar` & `primegenerators-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1998 2023-04-09 02:10:28.000000 primegenerators-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-04-02 23:21:14.000000 primegenerators-0.0.1/primegenerators/__init__.py
--rw-r--r--   0        0        0     1298 2023-04-09 02:08:48.000000 primegenerators-0.0.1/primegenerators/__main__.py
--rw-r--r--   0        0        0        0 2023-04-02 23:06:40.000000 primegenerators-0.0.1/primegenerators/generators/__init__.py
--rw-r--r--   0        0        0      166 2023-04-04 03:37:36.000000 primegenerators-0.0.1/primegenerators/generators/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2851 2023-04-09 02:09:48.000000 primegenerators-0.0.1/primegenerators/generators/__pycache__/eratosthenes_generator.cpython-310.pyc
--rw-r--r--   0        0        0      828 2023-04-09 01:10:38.000000 primegenerators-0.0.1/primegenerators/generators/__pycache__/factory.cpython-310.pyc
--rw-r--r--   0        0        0     2184 2023-04-09 01:39:58.000000 primegenerators-0.0.1/primegenerators/generators/__pycache__/prime_generator.cpython-310.pyc
--rw-r--r--   0        0        0     2875 2023-04-09 02:08:46.000000 primegenerators-0.0.1/primegenerators/generators/eratosthenes_generator.py
--rw-r--r--   0        0        0      628 2023-04-09 01:10:38.000000 primegenerators-0.0.1/primegenerators/generators/factory.py
--rw-r--r--   0        0        0     1566 2023-04-09 01:35:08.000000 primegenerators-0.0.1/primegenerators/generators/prime_generator.py
--rw-r--r--   0        0        0      407 2023-04-09 02:10:28.000000 primegenerators-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 primegenerators-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1979 2023-04-09 02:16:02.000000 primegenerators-0.0.2/README.md
+-rw-r--r--   0        0        0       61 2023-04-09 02:16:02.000000 primegenerators-0.0.2/primegenerators/__init__.py
+-rw-r--r--   0        0        0     1279 2023-04-09 02:30:34.000000 primegenerators-0.0.2/primegenerators/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-02 23:06:40.000000 primegenerators-0.0.2/primegenerators/generators/__init__.py
+-rw-r--r--   0        0        0      166 2023-04-04 03:37:36.000000 primegenerators-0.0.2/primegenerators/generators/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2851 2023-04-09 02:09:48.000000 primegenerators-0.0.2/primegenerators/generators/__pycache__/eratosthenes_generator.cpython-310.pyc
+-rw-r--r--   0        0        0      828 2023-04-09 01:10:38.000000 primegenerators-0.0.2/primegenerators/generators/__pycache__/factory.cpython-310.pyc
+-rw-r--r--   0        0        0     2184 2023-04-09 01:39:58.000000 primegenerators-0.0.2/primegenerators/generators/__pycache__/prime_generator.cpython-310.pyc
+-rw-r--r--   0        0        0     2875 2023-04-09 02:08:46.000000 primegenerators-0.0.2/primegenerators/generators/eratosthenes_generator.py
+-rw-r--r--   0        0        0      628 2023-04-09 01:10:38.000000 primegenerators-0.0.2/primegenerators/generators/factory.py
+-rw-r--r--   0        0        0     1566 2023-04-09 01:35:08.000000 primegenerators-0.0.2/primegenerators/generators/prime_generator.py
+-rw-r--r--   0        0        0      699 2023-04-09 04:32:16.000000 primegenerators-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2724 1970-01-01 00:00:00.000000 primegenerators-0.0.2/PKG-INFO
```

### Comparing `primegenerators-0.0.1/README.md` & `primegenerators-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ```
 
 ## Python Library
 
 The prime generator should be created using the factory method, e.g.:
 
 ```python
-from primegenerators.generators.factory import get_generator
+from primegenerators import get_generator
 
 # Details elided
 
 generator = get_generator("eratosthenes")
 
 for index, prime in enumerate(generator.primes()):
     sys.stdout.write(str(prime))
```

### Comparing `primegenerators-0.0.1/primegenerators/__main__.py` & `primegenerators-0.0.2/primegenerators/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 import sys
 from enum import Enum
 
-from primegenerators.generators.factory import get_generator
+from primegenerators import get_generator
 
 
 class OutputFormat(Enum):
     TEXT = 1
     JSON = 2
     CSV = 3
```

### Comparing `primegenerators-0.0.1/primegenerators/generators/__pycache__/eratosthenes_generator.cpython-310.pyc` & `primegenerators-0.0.2/primegenerators/generators/__pycache__/eratosthenes_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `primegenerators-0.0.1/primegenerators/generators/__pycache__/factory.cpython-310.pyc` & `primegenerators-0.0.2/primegenerators/generators/__pycache__/factory.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `primegenerators-0.0.1/primegenerators/generators/__pycache__/prime_generator.cpython-310.pyc` & `primegenerators-0.0.2/primegenerators/generators/__pycache__/prime_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `primegenerators-0.0.1/primegenerators/generators/eratosthenes_generator.py` & `primegenerators-0.0.2/primegenerators/generators/eratosthenes_generator.py`

 * *Files identical despite different names*

### Comparing `primegenerators-0.0.1/primegenerators/generators/factory.py` & `primegenerators-0.0.2/primegenerators/generators/factory.py`

 * *Files identical despite different names*

### Comparing `primegenerators-0.0.1/primegenerators/generators/prime_generator.py` & `primegenerators-0.0.2/primegenerators/generators/prime_generator.py`

 * *Files identical despite different names*

### Comparing `primegenerators-0.0.1/PKG-INFO` & `primegenerators-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 Metadata-Version: 2.1
 Name: primegenerators
-Version: 0.0.1
-Summary: A library of prime number generators and analyzers
+Version: 0.0.2
+Summary: A library of prime number generators and analyzers, that also has a command-line interface
+License: Apache-2.0
+Keywords: prime,numbers,generator,cli
 Author: big-jr
 Author-email: githubcomms@softwarepragmatism.com
 Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 
 # PrimeGenerators - Prime Number Generation and Utilities
 
 ## Command Line Interface
 
 The prime generator can be run from the command line. The output can be piped or redirected to a separate file or process.
@@ -29,15 +36,15 @@
 ```
 
 ## Python Library
 
 The prime generator should be created using the factory method, e.g.:
 
 ```python
-from primegenerators.generators.factory import get_generator
+from primegenerators import get_generator
 
 # Details elided
 
 generator = get_generator("eratosthenes")
 
 for index, prime in enumerate(generator.primes()):
     sys.stdout.write(str(prime))
```

