# Comparing `tmp/niklibpy-0.1.0.tar.gz` & `tmp/niklibpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niklibpy-0.1.0.tar", max compression
+gzip compressed data, was "niklibpy-0.1.1.tar", max compression
```

## Comparing `niklibpy-0.1.0.tar` & `niklibpy-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-04-09 09:48:57.610510 niklibpy-0.1.0/niklibpy/__init__.py
--rw-r--r--   0        0        0     1442 2023-04-09 09:49:23.256295 niklibpy-0.1.0/niklibpy/niklib.py
--rw-r--r--   0        0        0      260 2023-04-09 09:54:25.073500 niklibpy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 niklibpy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-04-09 09:59:16.284386 niklibpy-0.1.1/niklibpy/__init__.py
+-rw-r--r--   0        0        0     1473 2023-04-09 10:00:28.520242 niklibpy-0.1.1/niklibpy/niklib.py
+-rw-r--r--   0        0        0      260 2023-04-09 10:23:51.552186 niklibpy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      336 1970-01-01 00:00:00.000000 niklibpy-0.1.1/PKG-INFO
```

### Comparing `niklibpy-0.1.0/niklibpy/niklib.py` & `niklibpy-0.1.1/niklibpy/niklib.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import concurrent.futures
-import sys
 import warnings
 from functools import reduce
-from typing import Any, Callable
+from typing import Any, Callable, List
 
 
-def pmap(funcs, max_workers=2):
+def pmap(funcs: List[Callable], max_workers: int = 2) -> List[Any]:
     """Simple parallel map construction, using a thread pool executor.
 
     Feed it an array of functions, and it will execute them in parallel, returning
     the results in the same order as the input functions"""
     with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
         futures = {executor.submit(func): i for i, func in enumerate(funcs)}
         results = []
```

