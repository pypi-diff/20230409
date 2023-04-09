# Comparing `tmp/fudgeo-0.3.8-py3-none-any.whl.zip` & `tmp/fudgeo-0.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 19761 bytes, number of entries: 12
--rw-r--r--  2.0 unx      117 b- defN 23-Mar-28 18:21 fudgeo/__init__.py
+Zip file size: 19764 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      117 b- defN 23-Mar-28 23:34 fudgeo/__init__.py
 -rw-r--r--  2.0 unx     2457 b- defN 23-Mar-12 04:11 fudgeo/constant.py
 -rw-r--r--  2.0 unx     1157 b- defN 23-Jan-04 21:53 fudgeo/enumeration.py
 -rw-r--r--  2.0 unx    62026 b- defN 23-Mar-12 04:11 fudgeo/geometry.py
--rw-r--r--  2.0 unx    17613 b- defN 23-Mar-28 18:17 fudgeo/geopkg.py
+-rw-r--r--  2.0 unx    17613 b- defN 23-Mar-28 23:35 fudgeo/geopkg.py
 -rw-r--r--  2.0 unx     2795 b- defN 23-Mar-12 04:11 fudgeo/geopkg.sql
--rw-r--r--  2.0 unx     7506 b- defN 23-Mar-28 18:17 fudgeo/sql.py
--rw-r--r--  2.0 unx     1088 b- defN 23-Mar-28 18:22 fudgeo-0.3.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     9095 b- defN 23-Mar-28 18:22 fudgeo-0.3.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-28 18:22 fudgeo-0.3.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Mar-28 18:22 fudgeo-0.3.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      901 b- defN 23-Mar-28 18:22 fudgeo-0.3.8.dist-info/RECORD
-12 files, 104854 bytes uncompressed, 18277 bytes compressed:  82.6%
+-rw-r--r--  2.0 unx     7506 b- defN 23-Mar-28 18:25 fudgeo/sql.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-Mar-28 23:40 fudgeo-0.3.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9095 b- defN 23-Mar-28 23:40 fudgeo-0.3.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Mar-28 23:40 fudgeo-0.3.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Mar-28 23:40 fudgeo-0.3.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      901 b- defN 23-Mar-28 23:40 fudgeo-0.3.9.dist-info/RECORD
+12 files, 104854 bytes uncompressed, 18280 bytes compressed:  82.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: fudgeo/geopkg.sql
 Comment: 
 
 Filename: fudgeo/sql.py
 Comment: 
 
-Filename: fudgeo-0.3.8.dist-info/LICENSE
+Filename: fudgeo-0.3.9.dist-info/LICENSE
 Comment: 
 
-Filename: fudgeo-0.3.8.dist-info/METADATA
+Filename: fudgeo-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: fudgeo-0.3.8.dist-info/WHEEL
+Filename: fudgeo-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: fudgeo-0.3.8.dist-info/top_level.txt
+Filename: fudgeo-0.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: fudgeo-0.3.8.dist-info/RECORD
+Filename: fudgeo-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fudgeo/__init__.py

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 """
 Package Initialization
 """
 
 
-__version__ = '0.3.8'
+__version__ = '0.3.9'
 
 
 if __name__ == '__main__':
     pass
```

## fudgeo/geopkg.py

```diff
@@ -514,15 +514,15 @@
     @property
     def escaped_name(self) -> str:
         """
         Escaped Name, only adds quotes if needed
         """
         name = self.name
         if name.upper() in KEYWORDS:
-            name = f"'{name}'"
+            name = f'"{name}"'
         return name
     # End escaped_name property
 
     def __repr__(self) -> str:
         """
         String representation
         """
```

## Comparing `fudgeo-0.3.8.dist-info/LICENSE` & `fudgeo-0.3.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fudgeo-0.3.8.dist-info/METADATA` & `fudgeo-0.3.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fudgeo
-Version: 0.3.8
+Version: 0.3.9
 Summary: GeoPackage support from Python.  fudgeo is a simple package for creating OGC GeoPackages, Feature Classes, Tables, and geometries (read and write).
 Author-email: "Integrated Informatics Inc." <contact@integrated-informatics.com>
 License: MIT License
         
         Copyright (c) 2021-2023 Integrated Informatics Inc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

