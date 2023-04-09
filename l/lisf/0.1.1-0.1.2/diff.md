# Comparing `tmp/lisf-0.1.1.tar.gz` & `tmp/lisf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lisf-0.1.1.tar", max compression
+gzip compressed data, was "lisf-0.1.2.tar", max compression
```

## Comparing `lisf-0.1.1.tar` & `lisf-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2372 2023-04-05 21:50:19.240538 lisf-0.1.1/lisf.py
--rw-r--r--   0        0        0      244 2023-04-05 21:53:43.416797 lisf-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 lisf-0.1.1/setup.py
--rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 lisf-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2336 2023-04-09 18:17:29.905578 lisf-0.1.2/lisf.py
+-rw-r--r--   0        0        0      424 2023-04-09 18:51:14.046125 lisf-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      532 1970-01-01 00:00:00.000000 lisf-0.1.2/setup.py
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 lisf-0.1.2/PKG-INFO
```

### Comparing `lisf-0.1.1/lisf.py` & `lisf-0.1.2/lisf.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from contextlib import contextmanager
 import sys
 import types
-
+from asgiref import sync
 
 nothing = object()
 
 
 class Module(types.ModuleType):
     _cache = {}
     _lazy_loaders = {}
 
     def register_loader(self, key, lazy_loader, rewrite=False):
         current_loader = self._lazy_loaders.get(key, None)
         assert callable(lazy_loader)
-        if current_loader is not None:
-            assert rewrite is False, 'already registered'
-            if rewrite is not True:
-                return lazy_loader
         assert rewrite is True or current_loader is None
+        if sync.iscoroutinefunction(lazy_loader):
+            lazy_loader = sync.async_to_sync(lazy_loader)
         self._lazy_loaders[key] = lazy_loader
         return current_loader
 
     def get(self, key):
         try:
             value = self._cache[key]
         except KeyError:
```

