# Comparing `tmp/lazylinop-1.0.7-py3-none-any.whl.zip` & `tmp/lazylinop-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 23369 bytes, number of entries: 8
--rw-r--r--  2.0 unx       71 b- defN 23-Apr-07 08:48 lazylinop/__init__.py
--rw-r--r--  2.0 unx    63971 b- defN 23-Apr-07 08:48 lazylinop/lazylinop.py
--rw-r--r--  2.0 unx    28887 b- defN 23-Apr-07 08:48 lazylinop/wip/lsignal.py
--rw-rw-rw-  2.0 unx     1434 b- defN 23-Apr-07 08:48 lazylinop-1.0.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     4769 b- defN 23-Apr-07 08:48 lazylinop-1.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 08:48 lazylinop-1.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-07 08:48 lazylinop-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      638 b- defN 23-Apr-07 08:48 lazylinop-1.0.7.dist-info/RECORD
-8 files, 99872 bytes uncompressed, 22259 bytes compressed:  77.7%
+Zip file size: 23368 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       71 b- defN 23-Apr-09 13:53 lazylinop/__init__.py
+-rw-r--r--  2.0 unx    63971 b- defN 23-Apr-09 13:53 lazylinop/lazylinop.py
+-rw-r--r--  2.0 unx    28887 b- defN 23-Apr-09 13:53 lazylinop/wip/lsignal.py
+-rw-rw-rw-  2.0 unx     1434 b- defN 23-Apr-09 13:53 lazylinop-1.0.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     4769 b- defN 23-Apr-09 13:53 lazylinop-1.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 13:53 lazylinop-1.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-09 13:53 lazylinop-1.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      638 b- defN 23-Apr-09 13:53 lazylinop-1.0.8.dist-info/RECORD
+8 files, 99872 bytes uncompressed, 22258 bytes compressed:  77.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: lazylinop/lazylinop.py
 Comment: 
 
 Filename: lazylinop/wip/lsignal.py
 Comment: 
 
-Filename: lazylinop-1.0.7.dist-info/LICENSE.txt
+Filename: lazylinop-1.0.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: lazylinop-1.0.7.dist-info/METADATA
+Filename: lazylinop-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: lazylinop-1.0.7.dist-info/WHEEL
+Filename: lazylinop-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: lazylinop-1.0.7.dist-info/top_level.txt
+Filename: lazylinop-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: lazylinop-1.0.7.dist-info/RECORD
+Filename: lazylinop-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lazylinop/__init__.py

```diff
@@ -1,3 +1,3 @@
 from . import lazylinop
 from .lazylinop import *
-__version__ = '1.0.7'
+__version__ = '1.0.8'
```

## Comparing `lazylinop-1.0.7.dist-info/LICENSE.txt` & `lazylinop-1.0.8.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `lazylinop-1.0.7.dist-info/METADATA` & `lazylinop-1.0.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazylinop
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package dedicated to lazy linear operators based on diverse backends/libraries.
 Author-email: Inria <remi.gribonval@inria.fr>, Pascal Carrivain <pascal.carrivain@inria.fr>, Simon Delamare <simon.delamare@ens-lyon.fr>, Hakim Hadj-Djilani <hakim.hadj-djilani@inria.fr>, Rémi Gribonval <remi.gribonval@inria.fr>
 License: Copyright 2023, Inria
         
         BSD License 2.0
         
         Redistribution and use in source and binary forms, with or without
```

## Comparing `lazylinop-1.0.7.dist-info/RECORD` & `lazylinop-1.0.8.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-lazylinop/__init__.py,sha256=jkoW-hMlCBfimmwlNVdpsqRS-kW18BbH4evCj8f75t0,71
+lazylinop/__init__.py,sha256=70evtjs6ZC9ldwx4Y2pZsSRawM7jxsvWdXnA9iA3-6c,71
 lazylinop/lazylinop.py,sha256=0vYzM13ttwSqHsYHaGsQWSEX2P80kbb6uxv1I3iZ3qc,63971
 lazylinop/wip/lsignal.py,sha256=c5EFZqgjYGmyReTyi2ftVr69vFhivSY0Sjn-9P8MQUM,28887
-lazylinop-1.0.7.dist-info/LICENSE.txt,sha256=jHt8qQXwxwsxIgSCZbFwPqQw3R1QWQK0JzZZ3PAwlU0,1434
-lazylinop-1.0.7.dist-info/METADATA,sha256=-bfrIudkqnL3H9Pf0wZLoWz8_HMK3zQGeWJ7f-tMcHQ,4769
-lazylinop-1.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-lazylinop-1.0.7.dist-info/top_level.txt,sha256=zq6N2WH1Vl_0zSzqC12W0Oil87_uMjD3sYhWGjRioIc,10
-lazylinop-1.0.7.dist-info/RECORD,,
+lazylinop-1.0.8.dist-info/LICENSE.txt,sha256=jHt8qQXwxwsxIgSCZbFwPqQw3R1QWQK0JzZZ3PAwlU0,1434
+lazylinop-1.0.8.dist-info/METADATA,sha256=fWHRQY8Q4DKlB6G4Ep1BV9-a-_O5Y3U5kVOwoSqXmoA,4769
+lazylinop-1.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+lazylinop-1.0.8.dist-info/top_level.txt,sha256=zq6N2WH1Vl_0zSzqC12W0Oil87_uMjD3sYhWGjRioIc,10
+lazylinop-1.0.8.dist-info/RECORD,,
```

