# Comparing `tmp/jacktrade-0.1.0.tar.gz` & `tmp/jacktrade-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jacktrade-0.1.0.tar", last modified: Sun Apr  9 13:30:35 2023, max compression
+gzip compressed data, was "jacktrade-0.1.1.tar", last modified: Sun Apr  9 15:19:01 2023, max compression
```

## Comparing `jacktrade-0.1.0.tar` & `jacktrade-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 13:30:35.216949 jacktrade-0.1.0/
--rw-rw-rw-   0        0        0     1077 2023-02-11 18:38:48.000000 jacktrade-0.1.0/LICENSE.md
--rw-rw-rw-   0        0        0     4665 2023-04-09 13:30:35.215951 jacktrade-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2948 2023-04-09 13:28:41.000000 jacktrade-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 13:30:35.198996 jacktrade-0.1.0/jacktrade/
--rw-rw-rw-   0        0        0        0 2023-02-12 13:53:20.000000 jacktrade-0.1.0/jacktrade/__init__.py
--rw-rw-rw-   0        0        0     2325 2023-04-08 14:04:50.000000 jacktrade-0.1.0/jacktrade/benchmark.py
--rw-rw-rw-   0        0        0     3665 2023-04-09 13:07:22.000000 jacktrade-0.1.0/jacktrade/collections.py
--rw-rw-rw-   0        0        0     2486 2023-04-08 15:30:12.000000 jacktrade-0.1.0/jacktrade/multicore.py
--rw-rw-rw-   0        0        0      662 2023-04-08 16:09:02.000000 jacktrade-0.1.0/jacktrade/pickler.py
-drwxrwxrwx   0        0        0        0 2023-04-09 13:30:35.205017 jacktrade-0.1.0/jacktrade.egg-info/
--rw-rw-rw-   0        0        0     4665 2023-04-09 13:30:35.000000 jacktrade-0.1.0/jacktrade.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-04-09 13:30:35.000000 jacktrade-0.1.0/jacktrade.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 13:30:35.000000 jacktrade-0.1.0/jacktrade.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-09 13:30:35.000000 jacktrade-0.1.0/jacktrade.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      677 2023-04-08 17:33:40.000000 jacktrade-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-09 13:30:35.216949 jacktrade-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-09 13:30:35.213957 jacktrade-0.1.0/tests/
--rw-rw-rw-   0        0        0     1891 2023-04-08 14:04:02.000000 jacktrade-0.1.0/tests/test_benchmark.py
--rw-rw-rw-   0        0        0     4132 2023-04-09 13:07:18.000000 jacktrade-0.1.0/tests/test_collections.py
--rw-rw-rw-   0        0        0     3232 2023-04-09 12:49:59.000000 jacktrade-0.1.0/tests/test_multicore.py
--rw-rw-rw-   0        0        0      608 2023-04-08 16:08:21.000000 jacktrade-0.1.0/tests/test_pickler.py
--rw-rw-rw-   0        0        0      180 2023-04-08 14:13:05.000000 jacktrade-0.1.0/tests/test_template.py
+drwxrwxrwx   0        0        0        0 2023-04-09 15:19:01.564228 jacktrade-0.1.1/
+-rw-rw-rw-   0        0        0     1077 2023-02-11 18:38:48.000000 jacktrade-0.1.1/LICENSE.md
+-rw-rw-rw-   0        0        0     5227 2023-04-09 15:19:01.563190 jacktrade-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3455 2023-04-09 15:08:47.000000 jacktrade-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 15:19:01.544274 jacktrade-0.1.1/jacktrade/
+-rw-rw-rw-   0        0        0        0 2023-02-12 13:53:20.000000 jacktrade-0.1.1/jacktrade/__init__.py
+-rw-rw-rw-   0        0        0     2300 2023-04-09 15:05:56.000000 jacktrade-0.1.1/jacktrade/benchmark.py
+-rw-rw-rw-   0        0        0     3665 2023-04-09 13:07:22.000000 jacktrade-0.1.1/jacktrade/collections.py
+-rw-rw-rw-   0        0        0     2486 2023-04-08 15:30:12.000000 jacktrade-0.1.1/jacktrade/multicore.py
+-rw-rw-rw-   0        0        0      662 2023-04-08 16:09:02.000000 jacktrade-0.1.1/jacktrade/pickler.py
+drwxrwxrwx   0        0        0        0 2023-04-09 15:19:01.552219 jacktrade-0.1.1/jacktrade.egg-info/
+-rw-rw-rw-   0        0        0     5227 2023-04-09 15:19:01.000000 jacktrade-0.1.1/jacktrade.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2023-04-09 15:19:01.000000 jacktrade-0.1.1/jacktrade.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 15:19:01.000000 jacktrade-0.1.1/jacktrade.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-09 15:19:01.000000 jacktrade-0.1.1/jacktrade.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      727 2023-04-09 14:59:59.000000 jacktrade-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-09 15:19:01.565183 jacktrade-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-09 15:19:01.561195 jacktrade-0.1.1/tests/
+-rw-rw-rw-   0        0        0     1891 2023-04-08 14:04:02.000000 jacktrade-0.1.1/tests/test_benchmark.py
+-rw-rw-rw-   0        0        0     4132 2023-04-09 13:07:18.000000 jacktrade-0.1.1/tests/test_collections.py
+-rw-rw-rw-   0        0        0     3232 2023-04-09 12:49:59.000000 jacktrade-0.1.1/tests/test_multicore.py
+-rw-rw-rw-   0        0        0      608 2023-04-08 16:08:21.000000 jacktrade-0.1.1/tests/test_pickler.py
+-rw-rw-rw-   0        0        0      180 2023-04-08 14:13:05.000000 jacktrade-0.1.1/tests/test_template.py
```

### Comparing `jacktrade-0.1.0/LICENSE.md` & `jacktrade-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jacktrade-0.1.0/PKG-INFO` & `jacktrade-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jacktrade
-Version: 0.1.0
+Version: 0.1.1
 Summary: A collection of commonly used Python utilities.
 Author-email: Mario Zaja <mzaja0@gmail.com>
 License: MIT License
         
         Copyright (c) 2023, Mario Zaja
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -12,41 +12,49 @@
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Project-URL: Homepage, https://github.com/mzaja/jacktrade
 Project-URL: Bug Tracker, https://github.com/mzaja/jacktrade/issues
 Keywords: utils,utilities
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# Jacktrade
-**Jack of all trades, master of none** - a collection of commonly used Python utilities. The package consists of the following submodules:
+# jacktrade
+[![test](https://github.com/mzaja/jacktrade/actions/workflows/test.yml/badge.svg)](https://github.com/mzaja/jacktrade/actions/workflows/test.yml) [![Coverage Status](https://coveralls.io/repos/github/mzaja/jacktrade/badge.svg?branch=main)](https://coveralls.io/github/mzaja/jacktrade?branch=main) [![PyPI version](https://badge.fury.io/py/jacktrade.svg)](https://badge.fury.io/py/jacktrade) ![License](https://img.shields.io/github/license/mzaja/jacktrade)
 
-- [Jacktrade](#jacktrade)
-  - [Benchmark](#benchmark)
-  - [Collections](#collections)
-  - [Multicore](#multicore)
-  - [Pickler](#pickler)
+**Jack of all trades, master of none** - a collection of commonly used Python utilities. Install using:
+```
+pip install jacktrade
+```
+
+The package consists of the following submodules:
+
+- [Benchmark](#benchmark)
+- [Collections](#collections)
+- [Multicore](#multicore)
+- [Pickler](#pickler)
 
 ## Benchmark
 Contains a `CodeTimer` class which is used to elegantly and precisely time a piece of code:
 ```py
 from jacktrade.benchmark import CodeTimer
 from time import sleep
 
 with CodeTimer() as ct:
     # Enter code to time here
-    sleep(0.1)  # Simulate a piece of code
+    sleep(0.1)  # Simulates a piece of code
 
-# "Code execution took 100 ms." gets printed out.
+# Prints: "Code execution took 100 ms."
+(ct.ns, ct.us, ct.ms. ct.s)  # Access code duration in nano/micro/milli/seconds.
 ```
 
 ## Collections
 Contains utility functions for working with collections, namely dictionaries and iterables. Usage examples include:
 ```py
 from jacktrade.collections import *
 
@@ -55,30 +63,28 @@
 flatten_dict(dict_data)             # Returns: [1, 2]
 get_first_dict_item(dict_data)      # Returns: ("a", 1)
 get_first_dict_key(dict_data)       # Returns: "a"
 get_first_dict_value(dict_data)     # Returns: 1
 
 # Iterable utilities
 list_data = [1, 2, [3, 4], 5, 6]
-flatten_list(list_data)                     # Returns: [1, 2, 3, 4, 5, 6]
-list(chunkify(list_data, chunk_size=2))     # Returns: [[1, 2], [[3, 4], 5], [6]]
-list(limit_iterator(list_data, limit=3))    # Returns: [1, 2, [3, 4]]
+flatten_list(list_data)             # Returns: [1, 2, 3, 4, 5, 6]
+chunkify(list_data, chunk_size=2)   # Yields: [1, 2], [[3, 4], 5], [6]
+limit_iterator(list_data, limit=3)  # Yields: 1, 2, [3, 4]
 ```
 
 ## Multicore
 Provides an elegant and memory-efficient way to process data using multiple cores. The main advantage of using `do_multicore_work` function over manually using `concurrent.futures` or `multiprocessing` modules is that new jobs are only submitted for execution when a CPU core is available. This optimises CPU and RAM usage. Using the aforementioned modules directly, it is all too easy to inadvarently cause memory leaks and crash the interpreter (if not the whole system).
 
 Usage example (does not work in the interactive interpreter):
 ```py
 from jacktrade.multicore import do_multicore_work
 
 def worker(first, second) -> tuple:
-    """
-    Receives two arguments and returns them as a tuple.
-    """
+    """Receives two arguments and returns them as a tuple."""
     return (first, second)
 
 def worker_done_callback(future):
     """Called whenever a worker process terminates and returns a result."""
     print(future.result())
 
 if __name__ == "__main__":
```

### Comparing `jacktrade-0.1.0/README.md` & `jacktrade-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,34 @@
-# Jacktrade
-**Jack of all trades, master of none** - a collection of commonly used Python utilities. The package consists of the following submodules:
+# jacktrade
+[![test](https://github.com/mzaja/jacktrade/actions/workflows/test.yml/badge.svg)](https://github.com/mzaja/jacktrade/actions/workflows/test.yml) [![Coverage Status](https://coveralls.io/repos/github/mzaja/jacktrade/badge.svg?branch=main)](https://coveralls.io/github/mzaja/jacktrade?branch=main) [![PyPI version](https://badge.fury.io/py/jacktrade.svg)](https://badge.fury.io/py/jacktrade) ![License](https://img.shields.io/github/license/mzaja/jacktrade)
 
-- [Jacktrade](#jacktrade)
-  - [Benchmark](#benchmark)
-  - [Collections](#collections)
-  - [Multicore](#multicore)
-  - [Pickler](#pickler)
+**Jack of all trades, master of none** - a collection of commonly used Python utilities. Install using:
+```
+pip install jacktrade
+```
+
+The package consists of the following submodules:
+
+- [Benchmark](#benchmark)
+- [Collections](#collections)
+- [Multicore](#multicore)
+- [Pickler](#pickler)
 
 ## Benchmark
 Contains a `CodeTimer` class which is used to elegantly and precisely time a piece of code:
 ```py
 from jacktrade.benchmark import CodeTimer
 from time import sleep
 
 with CodeTimer() as ct:
     # Enter code to time here
-    sleep(0.1)  # Simulate a piece of code
+    sleep(0.1)  # Simulates a piece of code
 
-# "Code execution took 100 ms." gets printed out.
+# Prints: "Code execution took 100 ms."
+(ct.ns, ct.us, ct.ms. ct.s)  # Access code duration in nano/micro/milli/seconds.
 ```
 
 ## Collections
 Contains utility functions for working with collections, namely dictionaries and iterables. Usage examples include:
 ```py
 from jacktrade.collections import *
 
@@ -30,30 +37,28 @@
 flatten_dict(dict_data)             # Returns: [1, 2]
 get_first_dict_item(dict_data)      # Returns: ("a", 1)
 get_first_dict_key(dict_data)       # Returns: "a"
 get_first_dict_value(dict_data)     # Returns: 1
 
 # Iterable utilities
 list_data = [1, 2, [3, 4], 5, 6]
-flatten_list(list_data)                     # Returns: [1, 2, 3, 4, 5, 6]
-list(chunkify(list_data, chunk_size=2))     # Returns: [[1, 2], [[3, 4], 5], [6]]
-list(limit_iterator(list_data, limit=3))    # Returns: [1, 2, [3, 4]]
+flatten_list(list_data)             # Returns: [1, 2, 3, 4, 5, 6]
+chunkify(list_data, chunk_size=2)   # Yields: [1, 2], [[3, 4], 5], [6]
+limit_iterator(list_data, limit=3)  # Yields: 1, 2, [3, 4]
 ```
 
 ## Multicore
 Provides an elegant and memory-efficient way to process data using multiple cores. The main advantage of using `do_multicore_work` function over manually using `concurrent.futures` or `multiprocessing` modules is that new jobs are only submitted for execution when a CPU core is available. This optimises CPU and RAM usage. Using the aforementioned modules directly, it is all too easy to inadvarently cause memory leaks and crash the interpreter (if not the whole system).
 
 Usage example (does not work in the interactive interpreter):
 ```py
 from jacktrade.multicore import do_multicore_work
 
 def worker(first, second) -> tuple:
-    """
-    Receives two arguments and returns them as a tuple.
-    """
+    """Receives two arguments and returns them as a tuple."""
     return (first, second)
 
 def worker_done_callback(future):
     """Called whenever a worker process terminates and returns a result."""
     print(future.result())
 
 if __name__ == "__main__":
```

### Comparing `jacktrade-0.1.0/jacktrade/benchmark.py` & `jacktrade-0.1.1/jacktrade/benchmark.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,16 +35,15 @@
         self.s = -1
 
     def __enter__(self):
         self.start = time.perf_counter_ns()
         return self
 
     def __exit__(self, exc_type, exc_value, exc_tb):
-        finish = time.perf_counter_ns()
-        self.ns = finish - self.start
+        self.ns = time.perf_counter_ns() - self.start
         self.us = self.ns / 1e3
         self.ms = self.ns / 1e6
         self.s = self.ns / 1e9
         if not self._no_print:
             print(
                 f"Code execution took {self._format_time(self.ns, self._min_digits)}."
             )
```

### Comparing `jacktrade-0.1.0/jacktrade/collections.py` & `jacktrade-0.1.1/jacktrade/collections.py`

 * *Files identical despite different names*

### Comparing `jacktrade-0.1.0/jacktrade/multicore.py` & `jacktrade-0.1.1/jacktrade/multicore.py`

 * *Files identical despite different names*

### Comparing `jacktrade-0.1.0/jacktrade/pickler.py` & `jacktrade-0.1.1/jacktrade/pickler.py`

 * *Files identical despite different names*

### Comparing `jacktrade-0.1.0/jacktrade.egg-info/PKG-INFO` & `jacktrade-0.1.1/jacktrade.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jacktrade
-Version: 0.1.0
+Version: 0.1.1
 Summary: A collection of commonly used Python utilities.
 Author-email: Mario Zaja <mzaja0@gmail.com>
 License: MIT License
         
         Copyright (c) 2023, Mario Zaja
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -12,41 +12,49 @@
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Project-URL: Homepage, https://github.com/mzaja/jacktrade
 Project-URL: Bug Tracker, https://github.com/mzaja/jacktrade/issues
 Keywords: utils,utilities
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# Jacktrade
-**Jack of all trades, master of none** - a collection of commonly used Python utilities. The package consists of the following submodules:
+# jacktrade
+[![test](https://github.com/mzaja/jacktrade/actions/workflows/test.yml/badge.svg)](https://github.com/mzaja/jacktrade/actions/workflows/test.yml) [![Coverage Status](https://coveralls.io/repos/github/mzaja/jacktrade/badge.svg?branch=main)](https://coveralls.io/github/mzaja/jacktrade?branch=main) [![PyPI version](https://badge.fury.io/py/jacktrade.svg)](https://badge.fury.io/py/jacktrade) ![License](https://img.shields.io/github/license/mzaja/jacktrade)
 
-- [Jacktrade](#jacktrade)
-  - [Benchmark](#benchmark)
-  - [Collections](#collections)
-  - [Multicore](#multicore)
-  - [Pickler](#pickler)
+**Jack of all trades, master of none** - a collection of commonly used Python utilities. Install using:
+```
+pip install jacktrade
+```
+
+The package consists of the following submodules:
+
+- [Benchmark](#benchmark)
+- [Collections](#collections)
+- [Multicore](#multicore)
+- [Pickler](#pickler)
 
 ## Benchmark
 Contains a `CodeTimer` class which is used to elegantly and precisely time a piece of code:
 ```py
 from jacktrade.benchmark import CodeTimer
 from time import sleep
 
 with CodeTimer() as ct:
     # Enter code to time here
-    sleep(0.1)  # Simulate a piece of code
+    sleep(0.1)  # Simulates a piece of code
 
-# "Code execution took 100 ms." gets printed out.
+# Prints: "Code execution took 100 ms."
+(ct.ns, ct.us, ct.ms. ct.s)  # Access code duration in nano/micro/milli/seconds.
 ```
 
 ## Collections
 Contains utility functions for working with collections, namely dictionaries and iterables. Usage examples include:
 ```py
 from jacktrade.collections import *
 
@@ -55,30 +63,28 @@
 flatten_dict(dict_data)             # Returns: [1, 2]
 get_first_dict_item(dict_data)      # Returns: ("a", 1)
 get_first_dict_key(dict_data)       # Returns: "a"
 get_first_dict_value(dict_data)     # Returns: 1
 
 # Iterable utilities
 list_data = [1, 2, [3, 4], 5, 6]
-flatten_list(list_data)                     # Returns: [1, 2, 3, 4, 5, 6]
-list(chunkify(list_data, chunk_size=2))     # Returns: [[1, 2], [[3, 4], 5], [6]]
-list(limit_iterator(list_data, limit=3))    # Returns: [1, 2, [3, 4]]
+flatten_list(list_data)             # Returns: [1, 2, 3, 4, 5, 6]
+chunkify(list_data, chunk_size=2)   # Yields: [1, 2], [[3, 4], 5], [6]
+limit_iterator(list_data, limit=3)  # Yields: 1, 2, [3, 4]
 ```
 
 ## Multicore
 Provides an elegant and memory-efficient way to process data using multiple cores. The main advantage of using `do_multicore_work` function over manually using `concurrent.futures` or `multiprocessing` modules is that new jobs are only submitted for execution when a CPU core is available. This optimises CPU and RAM usage. Using the aforementioned modules directly, it is all too easy to inadvarently cause memory leaks and crash the interpreter (if not the whole system).
 
 Usage example (does not work in the interactive interpreter):
 ```py
 from jacktrade.multicore import do_multicore_work
 
 def worker(first, second) -> tuple:
-    """
-    Receives two arguments and returns them as a tuple.
-    """
+    """Receives two arguments and returns them as a tuple."""
     return (first, second)
 
 def worker_done_callback(future):
     """Called whenever a worker process terminates and returns a result."""
     print(future.result())
 
 if __name__ == "__main__":
```

### Comparing `jacktrade-0.1.0/tests/test_benchmark.py` & `jacktrade-0.1.1/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `jacktrade-0.1.0/tests/test_collections.py` & `jacktrade-0.1.1/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `jacktrade-0.1.0/tests/test_multicore.py` & `jacktrade-0.1.1/tests/test_multicore.py`

 * *Files identical despite different names*

### Comparing `jacktrade-0.1.0/tests/test_pickler.py` & `jacktrade-0.1.1/tests/test_pickler.py`

 * *Files identical despite different names*

