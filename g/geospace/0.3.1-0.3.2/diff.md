# Comparing `tmp/geospace-0.3.1.tar.gz` & `tmp/geospace-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geospace-0.3.1.tar", last modified: Sun Apr  9 14:26:21 2023, max compression
+gzip compressed data, was "geospace-0.3.2.tar", last modified: Sun Apr  9 15:26:58 2023, max compression
```

## Comparing `geospace-0.3.1.tar` & `geospace-0.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 14:26:21.802782 geospace-0.3.1/
--rw-rw-rw-   0        0        0     1055 2021-03-21 14:06:09.000000 geospace-0.3.1/LICENSE
--rw-rw-rw-   0        0        0       25 2021-03-20 14:22:17.000000 geospace-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1294 2023-04-09 14:26:21.802782 geospace-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      582 2021-03-20 14:45:55.000000 geospace-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 14:26:21.797584 geospace-0.3.1/geospace/
--rw-rw-rw-   0        0        0      449 2023-03-11 18:48:26.000000 geospace-0.3.1/geospace/__init__.py
--rw-rw-rw-   0        0        0      992 2022-12-21 15:03:51.000000 geospace-0.3.1/geospace/_const.py
--rw-rw-rw-   0        0        0     4333 2022-11-26 11:21:06.000000 geospace-0.3.1/geospace/boundary.py
--rw-rw-rw-   0        0        0     8356 2023-03-08 17:18:47.000000 geospace-0.3.1/geospace/gee_export.py
--rw-rw-rw-   0        0        0     4248 2023-03-11 20:27:20.000000 geospace-0.3.1/geospace/map_calc.py
--rw-rw-rw-   0        0        0     1557 2022-12-21 14:22:31.000000 geospace-0.3.1/geospace/projection.py
--rw-rw-rw-   0        0        0     1240 2022-11-26 11:21:06.000000 geospace-0.3.1/geospace/ras_to_shp.py
--rw-rw-rw-   0        0        0     5931 2023-03-26 19:18:15.000000 geospace-0.3.1/geospace/raster.py
--rw-rw-rw-   0        0        0     5489 2022-11-26 11:21:06.000000 geospace-0.3.1/geospace/shape.py
--rw-rw-rw-   0        0        0     6206 2023-03-09 06:56:05.000000 geospace-0.3.1/geospace/shp_to_ras.py
--rw-rw-rw-   0        0        0     6363 2022-11-26 11:46:00.000000 geospace-0.3.1/geospace/spatial_calc.py
--rw-rw-rw-   0        0        0     6405 2023-03-26 19:17:45.000000 geospace-0.3.1/geospace/utils.py
--rw-rw-rw-   0        0        0     8848 2023-03-09 08:03:41.000000 geospace-0.3.1/geospace/zonal_stats.py
-drwxrwxrwx   0        0        0        0 2023-04-09 14:26:21.801759 geospace-0.3.1/geospace.egg-info/
--rw-rw-rw-   0        0        0     1294 2023-04-09 14:26:21.000000 geospace-0.3.1/geospace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      475 2023-04-09 14:26:21.000000 geospace-0.3.1/geospace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 14:26:21.000000 geospace-0.3.1/geospace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-09 14:26:21.000000 geospace-0.3.1/geospace.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-09 14:26:21.000000 geospace-0.3.1/geospace.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 14:26:21.802782 geospace-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     3987 2023-04-09 14:25:42.000000 geospace-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 15:26:58.667079 geospace-0.3.2/
+-rw-rw-rw-   0        0        0     1055 2021-03-21 14:06:09.000000 geospace-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0       25 2021-03-20 14:22:17.000000 geospace-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1294 2023-04-09 15:26:58.667079 geospace-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      582 2021-03-20 14:45:55.000000 geospace-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 15:26:58.662079 geospace-0.3.2/geospace/
+-rw-rw-rw-   0        0        0      449 2023-03-20 09:13:43.000000 geospace-0.3.2/geospace/__init__.py
+-rw-rw-rw-   0        0        0     1028 2023-03-21 08:26:55.000000 geospace-0.3.2/geospace/_const.py
+-rw-rw-rw-   0        0        0     4333 2023-03-20 09:13:43.000000 geospace-0.3.2/geospace/boundary.py
+-rw-rw-rw-   0        0        0     8356 2023-03-20 09:13:43.000000 geospace-0.3.2/geospace/gee_export.py
+-rw-rw-rw-   0        0        0     4248 2023-03-20 09:13:43.000000 geospace-0.3.2/geospace/map_calc.py
+-rw-rw-rw-   0        0        0     1557 2023-03-20 09:13:43.000000 geospace-0.3.2/geospace/projection.py
+-rw-rw-rw-   0        0        0     1240 2023-03-20 09:13:43.000000 geospace-0.3.2/geospace/ras_to_shp.py
+-rw-rw-rw-   0        0        0     5931 2023-04-09 15:26:08.000000 geospace-0.3.2/geospace/raster.py
+-rw-rw-rw-   0        0        0     5489 2023-03-20 09:13:43.000000 geospace-0.3.2/geospace/shape.py
+-rw-rw-rw-   0        0        0     6206 2023-03-20 09:13:43.000000 geospace-0.3.2/geospace/shp_to_ras.py
+-rw-rw-rw-   0        0        0     6363 2023-03-20 09:13:43.000000 geospace-0.3.2/geospace/spatial_calc.py
+-rw-rw-rw-   0        0        0     6405 2023-04-09 15:26:01.000000 geospace-0.3.2/geospace/utils.py
+-rw-rw-rw-   0        0        0     8848 2023-03-20 09:13:43.000000 geospace-0.3.2/geospace/zonal_stats.py
+drwxrwxrwx   0        0        0        0 2023-04-09 15:26:58.666080 geospace-0.3.2/geospace.egg-info/
+-rw-rw-rw-   0        0        0     1294 2023-04-09 15:26:58.000000 geospace-0.3.2/geospace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      475 2023-04-09 15:26:58.000000 geospace-0.3.2/geospace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 15:26:58.000000 geospace-0.3.2/geospace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-09 15:26:58.000000 geospace-0.3.2/geospace.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-09 15:26:58.000000 geospace-0.3.2/geospace.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 15:26:58.667079 geospace-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     3987 2023-04-09 15:26:40.000000 geospace-0.3.2/setup.py
```

### Comparing `geospace-0.3.1/LICENSE` & `geospace-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geospace-0.3.1/PKG-INFO` & `geospace-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geospace
-Version: 0.3.1
+Version: 0.3.2
 Summary: Geospatial processing library based on GDAL and Google Earth Engine
 Home-page: https://github.com/xiejx5/geospace
 Author: Cody James
 Author-email: xiejx5@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `geospace-0.3.1/README.md` & `geospace-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `geospace-0.3.1/geospace/_const.py` & `geospace-0.3.2/geospace/_const.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 WGS84 = "EPSG:4326"
 
 # creation options
 CREATION = ['BIGTIFF=YES', 'TILED=YES', 'NUM_THREADS=ALL_CPUS',
             'COMPRESS=ZSTD', 'PREDICTOR=1', 'ZSTD_LEVEL=1']
 
 # mapping between gdal type and ogr field type
-TYPE_MAP = {'uint8': gdal.GDT_Byte,
+TYPE_MAP = {'bool': gdal.GDT_Byte,
+            'uint8': gdal.GDT_Byte,
             'int8': gdal.GDT_Byte,
             'uint16': gdal.GDT_UInt16,
             'int16': gdal.GDT_Int16,
             'uint32': gdal.GDT_UInt32,
             'int32': gdal.GDT_Int32,
             'float32': gdal.GDT_Float32,
             'float64': gdal.GDT_Float64,
```

### Comparing `geospace-0.3.1/geospace/boundary.py` & `geospace-0.3.2/geospace/boundary.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.1/geospace/gee_export.py` & `geospace-0.3.2/geospace/gee_export.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.1/geospace/map_calc.py` & `geospace-0.3.2/geospace/map_calc.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.1/geospace/projection.py` & `geospace-0.3.2/geospace/projection.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.1/geospace/ras_to_shp.py` & `geospace-0.3.2/geospace/ras_to_shp.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.1/geospace/raster.py` & `geospace-0.3.2/geospace/raster.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.1/geospace/shape.py` & `geospace-0.3.2/geospace/shape.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.1/geospace/shp_to_ras.py` & `geospace-0.3.2/geospace/shp_to_ras.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.1/geospace/spatial_calc.py` & `geospace-0.3.2/geospace/spatial_calc.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.1/geospace/utils.py` & `geospace-0.3.2/geospace/utils.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.1/geospace/zonal_stats.py` & `geospace-0.3.2/geospace/zonal_stats.py`

 * *Files identical despite different names*

### Comparing `geospace-0.3.1/geospace.egg-info/PKG-INFO` & `geospace-0.3.2/geospace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geospace
-Version: 0.3.1
+Version: 0.3.2
 Summary: Geospatial processing library based on GDAL and Google Earth Engine
 Home-page: https://github.com/xiejx5/geospace
 Author: Cody James
 Author-email: xiejx5@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `geospace-0.3.1/setup.py` & `geospace-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'geospace'
 DESCRIPTION = 'Geospatial processing library based on GDAL and Google Earth Engine'
 URL = 'https://github.com/xiejx5/geospace'
 EMAIL = 'xiejx5@gmail.com'
 AUTHOR = 'Cody James'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.3.1'
+VERSION = '0.3.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'numpy', 'gdal', 'tqdm'
 ]
 
 # What packages are optional?
```

