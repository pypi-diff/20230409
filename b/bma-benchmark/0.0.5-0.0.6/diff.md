# Comparing `tmp/bma_benchmark-0.0.5.tar.gz` & `tmp/bma_benchmark-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bma_benchmark-0.0.5.tar", last modified: Sun Apr  2 16:37:15 2023, max compression
+gzip compressed data, was "bma_benchmark-0.0.6.tar", last modified: Sun Apr  9 00:52:57 2023, max compression
```

## Comparing `bma_benchmark-0.0.5.tar` & `bma_benchmark-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-02 16:37:15.800594 bma_benchmark-0.0.5/
--rw-r--r--   0 divisor   (1000) root         (0)     1066 2023-04-01 17:20:56.000000 bma_benchmark-0.0.5/LICENSE
--rw-r--r--   0 divisor   (1000) root         (0)     2873 2023-04-02 16:37:15.796594 bma_benchmark-0.0.5/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)     2369 2023-04-01 18:30:25.000000 bma_benchmark-0.0.5/README.md
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-02 16:37:15.796594 bma_benchmark-0.0.5/bma_benchmark/
--rw-r--r--   0 divisor   (1000) root         (0)     8239 2023-04-02 16:37:10.000000 bma_benchmark-0.0.5/bma_benchmark/__init__.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-02 16:37:15.796594 bma_benchmark-0.0.5/bma_benchmark.egg-info/
--rw-r--r--   0 divisor   (1000) root         (0)     2873 2023-04-02 16:37:15.000000 bma_benchmark-0.0.5/bma_benchmark.egg-info/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      236 2023-04-02 16:37:15.000000 bma_benchmark-0.0.5/bma_benchmark.egg-info/SOURCES.txt
--rw-r--r--   0 divisor   (1000) root         (0)        1 2023-04-02 16:37:15.000000 bma_benchmark-0.0.5/bma_benchmark.egg-info/dependency_links.txt
--rw-r--r--   0 divisor   (1000) root         (0)       40 2023-04-02 16:37:15.000000 bma_benchmark-0.0.5/bma_benchmark.egg-info/requires.txt
--rw-r--r--   0 divisor   (1000) root         (0)       14 2023-04-02 16:37:15.000000 bma_benchmark-0.0.5/bma_benchmark.egg-info/top_level.txt
--rw-r--r--   0 divisor   (1000) root         (0)       38 2023-04-02 16:37:15.800594 bma_benchmark-0.0.5/setup.cfg
--rw-r--r--   0 divisor   (1000) root         (0)      793 2023-04-02 16:37:10.000000 bma_benchmark-0.0.5/setup.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-09 00:52:57.109502 bma_benchmark-0.0.6/
+-rw-r--r--   0 divisor   (1000) root         (0)     1066 2023-04-01 17:20:56.000000 bma_benchmark-0.0.6/LICENSE
+-rw-r--r--   0 divisor   (1000) root         (0)     3382 2023-04-09 00:52:57.109502 bma_benchmark-0.0.6/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)     2878 2023-04-09 00:52:13.000000 bma_benchmark-0.0.6/README.md
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-09 00:52:57.109502 bma_benchmark-0.0.6/bin/
+-rwxr-xr-x   0 divisor   (1000) root         (0)      765 2023-04-09 00:47:51.000000 bma_benchmark-0.0.6/bin/bma-benchmark
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-09 00:52:57.109502 bma_benchmark-0.0.6/bma_benchmark/
+-rw-r--r--   0 divisor   (1000) root         (0)     9665 2023-04-09 00:52:53.000000 bma_benchmark-0.0.6/bma_benchmark/__init__.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-04-09 00:52:57.109502 bma_benchmark-0.0.6/bma_benchmark.egg-info/
+-rw-r--r--   0 divisor   (1000) root         (0)     3382 2023-04-09 00:52:57.000000 bma_benchmark-0.0.6/bma_benchmark.egg-info/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      254 2023-04-09 00:52:57.000000 bma_benchmark-0.0.6/bma_benchmark.egg-info/SOURCES.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        1 2023-04-09 00:52:57.000000 bma_benchmark-0.0.6/bma_benchmark.egg-info/dependency_links.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       40 2023-04-09 00:52:57.000000 bma_benchmark-0.0.6/bma_benchmark.egg-info/requires.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       14 2023-04-09 00:52:57.000000 bma_benchmark-0.0.6/bma_benchmark.egg-info/top_level.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       38 2023-04-09 00:52:57.109502 bma_benchmark-0.0.6/setup.cfg
+-rw-r--r--   0 divisor   (1000) root         (0)      828 2023-04-09 00:52:53.000000 bma_benchmark-0.0.6/setup.py
```

### Comparing `bma_benchmark-0.0.5/LICENSE` & `bma_benchmark-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bma_benchmark-0.0.5/PKG-INFO` & `bma_benchmark-0.0.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: bma_benchmark
-Version: 0.0.5
-Summary: Python benchmark tool
-Home-page: https://github.com/alttch/bma-benchmark-py
-Author: Bohemia Automation / Altertech
-Author-email: div@altertech.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: System :: Benchmark
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # bma-benchmark-py
 
 Python benchmark library
 
 <img src="https://img.shields.io/pypi/v/bma-benchmark.svg" /> <img src="https://img.shields.io/badge/license-MIT-green" /> <img src="https://img.shields.io/badge/python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8-blue.svg" />
 
 
@@ -121,8 +105,26 @@
 my_bench = Benchmark()
 
 @my_bench
 def bench():
     pass
 ```
 
+## Storing results from multiple benchmarks
+
+Run a benchmark script with "OUT" OS variable:
+
+```shell
+OUT=b1.json python script.py
+```
+
+The benchmark result will be saved into "b1.json" file. After, multiple
+benchmarks can be combined into a single table with "bma-benchmark" console
+tool:
+
+```shell
+bma-benchmark b1.json b2.json
+```
 
+The tool automatically adds benchmark prefixes as "FILE_NAME.". It also has got
+options to specify precision, units etc. (run "bma-benchmark -h" to get list of
+all options)
```

### Comparing `bma_benchmark-0.0.5/README.md` & `bma_benchmark-0.0.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: bma_benchmark
+Version: 0.0.6
+Summary: Python benchmark tool
+Home-page: https://github.com/alttch/bma-benchmark-py
+Author: Bohemia Automation / Altertech
+Author-email: div@altertech.com
+License: MIT
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: System :: Benchmark
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # bma-benchmark-py
 
 Python benchmark library
 
 <img src="https://img.shields.io/pypi/v/bma-benchmark.svg" /> <img src="https://img.shields.io/badge/license-MIT-green" /> <img src="https://img.shields.io/badge/python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8-blue.svg" />
 
 
@@ -104,7 +120,29 @@
 
 my_bench = Benchmark()
 
 @my_bench
 def bench():
     pass
 ```
+
+## Storing results from multiple benchmarks
+
+Run a benchmark script with "OUT" OS variable:
+
+```shell
+OUT=b1.json python script.py
+```
+
+The benchmark result will be saved into "b1.json" file. After, multiple
+benchmarks can be combined into a single table with "bma-benchmark" console
+tool:
+
+```shell
+bma-benchmark b1.json b2.json
+```
+
+The tool automatically adds benchmark prefixes as "FILE_NAME.". It also has got
+options to specify precision, units etc. (run "bma-benchmark -h" to get list of
+all options)
+
+
```

### Comparing `bma_benchmark-0.0.5/bma_benchmark/__init__.py` & `bma_benchmark-0.0.6/bma_benchmark/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python3
 
-__version__ = '0.0.5'
+__version__ = '0.0.6'
 
 import time
 import json
 import os
 import subprocess
 
 from collections import OrderedDict
+from pathlib import Path
 
 
 def _get_multiplier(units):
     if units == 's':
         return 1
     elif units == 'ms':
         return 1_000
@@ -61,15 +62,15 @@
         multiplier = _get_multiplier(units)
         if print_result:
             from rapidtables import format_table, FORMAT_GENERATOR_COLS
             from neotermcolor import colored, cprint
         result = []
         base_elapsed = None
         for target in self.targets:
-            if print_result:
+            if print_result and target.kind in ['func', 'sub']:
                 spacer = '-' * 4
                 cprint(f'{spacer} {target.kind} {target.name} {spacer}',
                        color='grey')
             if target.kind == 'func':
                 op_start = time.perf_counter()
                 call_elapsed_min = None
                 call_elapsed_max = None
@@ -117,14 +118,34 @@
                         row['max'] = sub_row['max']
                         row['avg'] = sub_row['sec'] / number
                         row['sec'] = sub_row['sec']
                         row['iters/s'] = f'{round(number / row["sec"]):_}'
                         result.append(row)
                         if self.base == sub_row['name']:
                             base_elapsed = sub_row['sec']
+            elif target.kind == 'file':
+                p = Path(target.name)
+                with open(p) as fh:
+                    sub_result = json.load(fh)
+                    sub_number = sub_result['number']
+                    for sub_row in sub_result['result']:
+                        row = OrderedDict()
+                        row['name'] = f'{p.stem}.{sub_row["name"]}'
+                        row['min'] = sub_row['min']
+                        row['max'] = sub_row['max']
+                        row['avg'] = sub_row['sec'] / sub_number
+                        row['sec'] = sub_row['sec']
+                        if self.base == row['name']:
+                            base_elapsed = row['sec']
+                        row['iters/s'] = f'{round(sub_number / row["sec"]):_}'
+                        result.append(row)
+        fout = os.getenv('OUT')
+        if fout:
+            with open(fout, 'w') as fh:
+                json.dump(dict(result=result, number=number), fh)
         for row in result:
             if _full and base_elapsed:
                 if row['name'] == self.base:
                     row['diff'] = ''
                     row['diff_col'] = None
                 else:
                     if base_elapsed < row['sec']:
@@ -172,14 +193,18 @@
                 print(colored(r[3], color='white'), end=spacer)
                 print(colored(r[4], color='blue'), end=spacer)
                 if len(r) == 7:
                     print(colored(r[5], color='yellow'), end=spacer)
                     print(colored(r[6], color=diff_col[i]))
                 else:
                     print(colored(r[5], color='yellow'))
+        if fout:
+            print()
+            print(f'The result has been saved into',
+                  colored(fout, color='cyan', attrs='bold'))
         return result
 
     def __call__(self, f=None, **kwargs):
 
         def inner(f):
             self.append(f, **kwargs)
 
@@ -214,14 +239,24 @@
 
         Args:
             path: command path
         """
         target = Target(path, kind='sub', name=path)
         self.targets.append(target)
 
+    def append_file(self, path):
+        """
+        Append results from a file
+
+        Args:
+            path: file path
+        """
+        target = Target(path, kind='file', name=path)
+        self.targets.append(target)
+
     def sub(self):
         """
         Must be called method in sub-scripts
         """
         print(
             json.dumps(
                 dict(result=self.run(number=int(
```

### Comparing `bma_benchmark-0.0.5/bma_benchmark.egg-info/PKG-INFO` & `bma_benchmark-0.0.6/bma_benchmark.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bma-benchmark
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python benchmark tool
 Home-page: https://github.com/alttch/bma-benchmark-py
 Author: Bohemia Automation / Altertech
 Author-email: div@altertech.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -121,8 +121,28 @@
 my_bench = Benchmark()
 
 @my_bench
 def bench():
     pass
 ```
 
+## Storing results from multiple benchmarks
+
+Run a benchmark script with "OUT" OS variable:
+
+```shell
+OUT=b1.json python script.py
+```
+
+The benchmark result will be saved into "b1.json" file. After, multiple
+benchmarks can be combined into a single table with "bma-benchmark" console
+tool:
+
+```shell
+bma-benchmark b1.json b2.json
+```
+
+The tool automatically adds benchmark prefixes as "FILE_NAME.". It also has got
+options to specify precision, units etc. (run "bma-benchmark -h" to get list of
+all options)
+
```

### Comparing `bma_benchmark-0.0.5/setup.py` & `bma_benchmark-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.5'
+__version__ = '0.0.6'
 
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
@@ -13,13 +13,14 @@
     description='Python benchmark tool',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/alttch/bma-benchmark-py',
     packages=setuptools.find_packages(),
     license='MIT',
     install_requires=['rapidtables>=0.1.11', 'neotermcolor>=2.0.8'],
+    scripts=['bin/bma-benchmark'],
     classifiers=(
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Topic :: Software Development :: Libraries',
         'Topic :: System :: Benchmark',
     ))
```

