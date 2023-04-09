# Comparing `tmp/geetiles-0.1.3.tar.gz` & `tmp/geetiles-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geetiles-0.1.3.tar", last modified: Tue Mar 21 21:37:29 2023, max compression
+gzip compressed data, was "geetiles-0.1.4.tar", last modified: Sun Apr  9 18:47:40 2023, max compression
```

## Comparing `geetiles-0.1.3.tar` & `geetiles-0.1.4.tar`

### file list

```diff
@@ -1,37 +1,44 @@
-drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-03-21 21:37:29.648157 geetiles-0.1.3/
--rw-rw-r--   0 rlx       (1000) rlx       (1000)      104 2023-03-17 14:46:38.000000 geetiles-0.1.3/.gitignore
--rw-rw-r--   0 rlx       (1000) rlx       (1000)     1074 2023-03-17 14:46:38.000000 geetiles-0.1.3/LICENSE.txt
--rw-rw-r--   0 rlx       (1000) rlx       (1000)     6685 2023-03-21 21:37:29.648157 geetiles-0.1.3/PKG-INFO
--rw-rw-r--   0 rlx       (1000) rlx       (1000)     6389 2023-03-21 21:35:34.000000 geetiles-0.1.3/README.md
-drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-03-21 21:37:29.608157 geetiles-0.1.3/data/
--rw-rw-r--   0 rlx       (1000) rlx       (1000)     1879 2023-03-21 14:53:07.000000 geetiles-0.1.3/data/luxembourg.README.txt
--rw-rw-r--   0 rlx       (1000) rlx       (1000)    13885 2023-03-17 14:46:38.000000 geetiles-0.1.3/data/luxembourg.wkt
-drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-03-21 21:37:29.608157 geetiles-0.1.3/geetiles/
--rw-rw-r--   0 rlx       (1000) rlx       (1000)      220 2023-03-17 14:46:38.000000 geetiles-0.1.3/geetiles/__init__.py
--rw-rw-r--   0 rlx       (1000) rlx       (1000)    17370 2023-03-21 19:58:14.000000 geetiles-0.1.3/geetiles/cmds.py
--rw-rw-r--   0 rlx       (1000) rlx       (1000)     9284 2023-03-19 04:44:24.000000 geetiles-0.1.3/geetiles/gee.py
--rw-rw-r--   0 rlx       (1000) rlx       (1000)    12157 2023-03-21 16:26:23.000000 geetiles-0.1.3/geetiles/main.py
--rw-rw-r--   0 rlx       (1000) rlx       (1000)    23807 2023-03-21 14:25:34.000000 geetiles-0.1.3/geetiles/partitions.py
--rw-rw-r--   0 rlx       (1000) rlx       (1000)     4211 2023-03-21 14:26:41.000000 geetiles-0.1.3/geetiles/utils.py
-drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-03-21 21:37:29.608157 geetiles-0.1.3/geetiles.egg-info/
--rw-rw-r--   0 rlx       (1000) rlx       (1000)     6685 2023-03-21 21:37:29.000000 geetiles-0.1.3/geetiles.egg-info/PKG-INFO
--rw-rw-r--   0 rlx       (1000) rlx       (1000)      712 2023-03-21 21:37:29.000000 geetiles-0.1.3/geetiles.egg-info/SOURCES.txt
--rw-rw-r--   0 rlx       (1000) rlx       (1000)        1 2023-03-21 21:37:29.000000 geetiles-0.1.3/geetiles.egg-info/dependency_links.txt
--rw-rw-r--   0 rlx       (1000) rlx       (1000)       44 2023-03-21 21:37:29.000000 geetiles-0.1.3/geetiles.egg-info/entry_points.txt
--rw-rw-r--   0 rlx       (1000) rlx       (1000)        1 2023-03-17 14:51:57.000000 geetiles-0.1.3/geetiles.egg-info/not-zip-safe
--rw-rw-r--   0 rlx       (1000) rlx       (1000)       91 2023-03-21 21:37:29.000000 geetiles-0.1.3/geetiles.egg-info/requires.txt
--rw-rw-r--   0 rlx       (1000) rlx       (1000)        9 2023-03-21 21:37:29.000000 geetiles-0.1.3/geetiles.egg-info/top_level.txt
--rw-rw-r--   0 rlx       (1000) rlx       (1000)       56 2023-03-17 14:46:38.000000 geetiles-0.1.3/howto-publish.txt
-drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-03-21 21:37:29.640157 geetiles-0.1.3/imgs/
--rw-rw-r--   0 rlx       (1000) rlx       (1000)    82153 2023-03-19 05:37:33.000000 geetiles-0.1.3/imgs/dataframe.png
--rw-rw-r--   0 rlx       (1000) rlx       (1000)   366561 2023-03-17 14:46:38.000000 geetiles-0.1.3/imgs/landcover.png
--rw-rw-r--   0 rlx       (1000) rlx       (1000)   310721 2023-03-19 05:20:29.000000 geetiles-0.1.3/imgs/luxembourg-bands-communes.png
--rw-rw-r--   0 rlx       (1000) rlx       (1000)   306508 2023-03-19 05:14:46.000000 geetiles-0.1.3/imgs/luxembourg-bands.png
--rw-r--r--   0 rlx       (1000) rlx       (1000)  1664553 2023-03-21 21:33:01.000000 geetiles-0.1.3/imgs/luxembourg-communes-random5k.png
--rw-rw-r--   0 rlx       (1000) rlx       (1000)   959795 2023-03-17 14:46:38.000000 geetiles-0.1.3/imgs/luxembourg-communes.png
--rw-rw-r--   0 rlx       (1000) rlx       (1000)   863339 2023-03-17 14:46:38.000000 geetiles-0.1.3/imgs/luxembourg-random-5k.png
--rw-r--r--   0 rlx       (1000) rlx       (1000)  1182265 2023-03-21 21:34:06.000000 geetiles-0.1.3/imgs/luxembourg-splits.png
--rw-rw-r--   0 rlx       (1000) rlx       (1000)  1642194 2023-03-17 14:46:38.000000 geetiles-0.1.3/imgs/luxgrid.png
--rw-rw-r--   0 rlx       (1000) rlx       (1000)  1287337 2023-03-17 14:46:38.000000 geetiles-0.1.3/imgs/sentinel2.png
--rw-rw-r--   0 rlx       (1000) rlx       (1000)      385 2023-03-21 21:37:29.648157 geetiles-0.1.3/setup.cfg
--rw-rw-r--   0 rlx       (1000) rlx       (1000)      713 2023-03-17 15:10:29.000000 geetiles-0.1.3/setup.py
+drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-04-09 18:47:40.617351 geetiles-0.1.4/
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      104 2023-03-17 14:46:38.000000 geetiles-0.1.4/.gitignore
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)     1074 2023-03-17 14:46:38.000000 geetiles-0.1.4/LICENSE.txt
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)     6263 2023-04-09 18:47:40.617351 geetiles-0.1.4/PKG-INFO
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)     5967 2023-04-09 18:46:01.000000 geetiles-0.1.4/README.md
+drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-04-09 18:47:40.557350 geetiles-0.1.4/data/
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)     1879 2023-03-21 14:53:07.000000 geetiles-0.1.4/data/luxembourg.README.txt
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)    13885 2023-03-17 14:46:38.000000 geetiles-0.1.4/data/luxembourg.wkt
+drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-04-09 18:47:40.561350 geetiles-0.1.4/geetiles/
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      220 2023-03-17 14:46:38.000000 geetiles-0.1.4/geetiles/__init__.py
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)    18581 2023-04-09 18:46:01.000000 geetiles-0.1.4/geetiles/cmds.py
+drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-04-09 18:47:40.561350 geetiles-0.1.4/geetiles/defs/
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      430 2023-04-09 18:46:01.000000 geetiles-0.1.4/geetiles/defs/esaworldcover.py
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      983 2023-04-09 18:46:01.000000 geetiles-0.1.4/geetiles/defs/humanpop2015.py
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)     1064 2023-04-09 18:46:01.000000 geetiles-0.1.4/geetiles/defs/sentinel2rgbmedian2020.py
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      438 2023-04-09 18:46:01.000000 geetiles-0.1.4/geetiles/defs/soilphbenelux.py
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      417 2023-04-09 18:46:01.000000 geetiles-0.1.4/geetiles/defs/soilphcolombia.py
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      659 2023-04-09 18:46:01.000000 geetiles-0.1.4/geetiles/defs/treecover2020.py
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)     9284 2023-03-19 04:44:24.000000 geetiles-0.1.4/geetiles/gee.py
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)    11745 2023-04-09 18:46:01.000000 geetiles-0.1.4/geetiles/main.py
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)    24339 2023-04-09 18:46:01.000000 geetiles-0.1.4/geetiles/partitions.py
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)     6889 2023-04-09 18:46:01.000000 geetiles-0.1.4/geetiles/utils.py
+drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-04-09 18:47:40.561350 geetiles-0.1.4/geetiles.egg-info/
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)     6263 2023-04-09 18:47:40.000000 geetiles-0.1.4/geetiles.egg-info/PKG-INFO
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      907 2023-04-09 18:47:40.000000 geetiles-0.1.4/geetiles.egg-info/SOURCES.txt
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)        1 2023-04-09 18:47:40.000000 geetiles-0.1.4/geetiles.egg-info/dependency_links.txt
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)       44 2023-04-09 18:47:40.000000 geetiles-0.1.4/geetiles.egg-info/entry_points.txt
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)        1 2023-03-17 14:51:57.000000 geetiles-0.1.4/geetiles.egg-info/not-zip-safe
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)       91 2023-04-09 18:47:40.000000 geetiles-0.1.4/geetiles.egg-info/requires.txt
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)        9 2023-04-09 18:47:40.000000 geetiles-0.1.4/geetiles.egg-info/top_level.txt
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)       56 2023-03-17 14:46:38.000000 geetiles-0.1.4/howto-publish.txt
+drwxrwxr-x   0 rlx       (1000) rlx       (1000)        0 2023-04-09 18:47:40.609351 geetiles-0.1.4/imgs/
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)    82153 2023-03-19 05:37:33.000000 geetiles-0.1.4/imgs/dataframe.png
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)   366561 2023-03-17 14:46:38.000000 geetiles-0.1.4/imgs/landcover.png
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)   310721 2023-03-19 05:20:29.000000 geetiles-0.1.4/imgs/luxembourg-bands-communes.png
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)   306508 2023-03-19 05:14:46.000000 geetiles-0.1.4/imgs/luxembourg-bands.png
+-rw-r--r--   0 rlx       (1000) rlx       (1000)  1664553 2023-03-21 21:33:01.000000 geetiles-0.1.4/imgs/luxembourg-communes-random5k.png
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)   959795 2023-03-17 14:46:38.000000 geetiles-0.1.4/imgs/luxembourg-communes.png
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)   863339 2023-03-17 14:46:38.000000 geetiles-0.1.4/imgs/luxembourg-random-5k.png
+-rw-r--r--   0 rlx       (1000) rlx       (1000)  1182265 2023-03-21 21:34:06.000000 geetiles-0.1.4/imgs/luxembourg-splits.png
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)  1642194 2023-03-17 14:46:38.000000 geetiles-0.1.4/imgs/luxgrid.png
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)  1287337 2023-03-17 14:46:38.000000 geetiles-0.1.4/imgs/sentinel2.png
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      385 2023-04-09 18:47:40.617351 geetiles-0.1.4/setup.cfg
+-rw-rw-r--   0 rlx       (1000) rlx       (1000)      713 2023-03-17 15:10:29.000000 geetiles-0.1.4/setup.py
```

### Comparing `geetiles-0.1.3/LICENSE.txt` & `geetiles-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.3/PKG-INFO` & `geetiles-0.1.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: geetiles
-Version: 0.1.3
-Summary: download Google Earth Engine datasets to tiles as geotiff arrays
-Home-page: https://github.com/rramosp/geetiles
-Author: raul ramos
-Author-email: raul.ramos@udea.edu.co
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # geetiles
 
 ## download Google Earth Engine datasets to tiles as geotiff arrays
 
 Uses the [Google Earth Engine High Volume Endpoint](https://developers.google.com/earth-engine/cloud/highvolume) which, according to the documentation:
 
 > This service is designed to support a much larger number of simultaneous requests per user, but provides less caching, so it's best for small queries that don't involve any sort of aggregation (like fetching tiles from pre-built images).
@@ -31,24 +21,24 @@
 this generates file `./lux_partitions_aschips_14c55eb7d417f.geojson`. Use a tool such as [QGIS](https://qgis.org/) to view it.
 
 <center><img src='imgs/luxgrid.png' width=800></center>
 
 
 ### 2. download tiles
 
-    geet download --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson  --gee_image_pycode sentinel2-rgb-median-2020 --pixels_lonlat [100,100] --skip_if_exists
+    geet download --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson  --dataset_def sentinel2-rgb-median-2020 --pixels_lonlat [100,100] --skip_if_exists
 
 
 this fills the folder `lux_partitions_aschips_14c55eb7d417f/sentinel2-rgb-median-2020` with RGB geotiff images of size 100x100 pixels.
 
-If using `sentinel2-rgb-median-2020` as `gee_image_pycode`, which is an alias to [Sentinel-2 MSI Level 2-A](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S2_SR) GEE dataset, taking the median of the cloudless chips over the year 2020.
+If using `sentinel2-rgb-median-2020` as `dataset_def`, which is an alias to [Sentinel-2 MSI Level 2-A](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S2_SR) GEE dataset, taking the median of the cloudless chips over the year 2020.
 
 <center><img src='imgs/sentinel2.png' width=800></center>
 
-If using `esa-world-cover` as `gee_image_pycode`, which is an alias to [ESA WorldCover 10m v100](https://developers.google.com/earth-engine/datasets/catalog/ESA_WorldCover_v100) GEE dataset.
+If using `esa-world-cover` as `dataset_def`, which is an alias to [ESA WorldCover 10m v100](https://developers.google.com/earth-engine/datasets/catalog/ESA_WorldCover_v100) GEE dataset.
 
 <center><img src='imgs/landcover.png' width=800></center>
 
 
 ## Other usages
 
 ### Other ways to create the set of tiles (shapes) 
@@ -64,32 +54,17 @@
       geet select --orig_shapefile COMM_RG_01M_2016_4326.zip --aoi_wkt_file luxembourg.wkt --tiles_name communes --aoi_name lux --dest_dir .
 
 <center><img src='imgs/luxembourg-communes-random5k.png' width=600></center>
 
 
 ### Using your own code to define the GEE source image object.
 
-    geet download --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson  --gee_image_pycode crops.py --dataset_name crop --pixels_lonlat [100,100] --skip_if_exists --skip_confirm --n_processes 20
-
-assuming the file `crops.py` contains the following code
-
-        import ee
-
-        def get_ee_image():
-            return ee.Image('USGS/GFSAD1000_V1')\
-                     .select('landcover')\
-                     .visualize(min=0.0, max=5.0,
-                                palette = ['black', 'orange', 'brown', 
-                                           '02a50f', 'green', 'yellow'])
-
-        def get_dataset_name():
-            return 'crops'
-
+    geet download --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson  --dataset_def crops.py --pixels_lonlat [100,100] --skip_if_exists --skip_confirm --n_processes 20
 
-The `crops.py` will be saved under the destination folder for reference. The destination folder is created alongside the `tiles-file`.
+where `crops.py` contains a python `class DatasetDefinition` following the structure of the predefined ones under `defs`.  The files `crops.py` will be saved under the destination folder for reference. The destination folder is created alongside the `tiles_file`.
 
 ### Split geometries in train, test, val using geographic bands
 
 With a certain angle
 
     geet split --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson --nbands 8 --train_pct .5 --test_pct 0.3 --val_pct 0.2  --angle 0.78
 
@@ -110,15 +85,15 @@
 
 With respect to a dataset downloaded with segmentation labels.
 
     geet lp.compute --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson --dataset_name esa-world-cover
 
 We can also add the label proportions of the coarser tile in which each chip is embedded. First, we need to download the labels for each coarser tile from GEE.
 
-    geet download --tiles_file lux_partitions_communes_1a471c686e053.geojson  --gee_image_pycode esa-world-cover  --meters_per_pixel 20  --skip_if_exists 
+    geet download --tiles_file lux_partitions_communes_1a471c686e053.geojson  --dataset_def esa-world-cover  --meters_per_pixel 20  --skip_if_exists 
 
 then, compute the label proportions at this coarser tiles:
 
     geet lp.compute --tiles_file lux_partitions_communes_1a471c686e053.geojson --dataset_name esa-world-cover
 
 and then compute the label proportions from the coarser tiles.
 
@@ -129,13 +104,13 @@
 <img src='imgs/dataframe.png' width=800>
 
 
 ### Creating a dataset to share it
 
 This will create a zip file, with a pickle per chip containing a dictionary with the chip image, label and proportions.
 
-    geet zip.dataset --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson --foreign_tiles_file lux_partitions_communes_1a471c686e053.geojson --images_dataset_name sentinel2-rgb-median-2020 --labels_dataset_name esa-world-cover --readme_file README.txt  --label_map [10,20,30,40,50,60,70,80,90,95,100]
+    geet zip.dataset --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson --foreign_tiles_file lux_partitions_communes_1a471c686e053.geojson --images_dataset_def sentinel2-rgb-median-2020 --labels_dataset_def esa-world-cover --readme_file README.txt
 
 ### Some notes
 
 - the hash codes in the name files are computed using the participating geometries. This ensures that changing geometries do not override each other(such as for random partitions, or a wkt with slightly different coordinates).
 - the splits are saved both as a column in the corresponding `tiles_file` (which is a `geojson`) and in a separte `csv` file. This is to enable fast loading from `csv` (as loading from `geojson` might take a while, especially for large dataset).
```

### Comparing `geetiles-0.1.3/README.md` & `geetiles-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: geetiles
+Version: 0.1.4
+Summary: download Google Earth Engine datasets to tiles as geotiff arrays
+Home-page: https://github.com/rramosp/geetiles
+Author: raul ramos
+Author-email: raul.ramos@udea.edu.co
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # geetiles
 
 ## download Google Earth Engine datasets to tiles as geotiff arrays
 
 Uses the [Google Earth Engine High Volume Endpoint](https://developers.google.com/earth-engine/cloud/highvolume) which, according to the documentation:
 
 > This service is designed to support a much larger number of simultaneous requests per user, but provides less caching, so it's best for small queries that don't involve any sort of aggregation (like fetching tiles from pre-built images).
@@ -21,24 +31,24 @@
 this generates file `./lux_partitions_aschips_14c55eb7d417f.geojson`. Use a tool such as [QGIS](https://qgis.org/) to view it.
 
 <center><img src='imgs/luxgrid.png' width=800></center>
 
 
 ### 2. download tiles
 
-    geet download --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson  --gee_image_pycode sentinel2-rgb-median-2020 --pixels_lonlat [100,100] --skip_if_exists
+    geet download --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson  --dataset_def sentinel2-rgb-median-2020 --pixels_lonlat [100,100] --skip_if_exists
 
 
 this fills the folder `lux_partitions_aschips_14c55eb7d417f/sentinel2-rgb-median-2020` with RGB geotiff images of size 100x100 pixels.
 
-If using `sentinel2-rgb-median-2020` as `gee_image_pycode`, which is an alias to [Sentinel-2 MSI Level 2-A](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S2_SR) GEE dataset, taking the median of the cloudless chips over the year 2020.
+If using `sentinel2-rgb-median-2020` as `dataset_def`, which is an alias to [Sentinel-2 MSI Level 2-A](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S2_SR) GEE dataset, taking the median of the cloudless chips over the year 2020.
 
 <center><img src='imgs/sentinel2.png' width=800></center>
 
-If using `esa-world-cover` as `gee_image_pycode`, which is an alias to [ESA WorldCover 10m v100](https://developers.google.com/earth-engine/datasets/catalog/ESA_WorldCover_v100) GEE dataset.
+If using `esa-world-cover` as `dataset_def`, which is an alias to [ESA WorldCover 10m v100](https://developers.google.com/earth-engine/datasets/catalog/ESA_WorldCover_v100) GEE dataset.
 
 <center><img src='imgs/landcover.png' width=800></center>
 
 
 ## Other usages
 
 ### Other ways to create the set of tiles (shapes) 
@@ -54,32 +64,17 @@
       geet select --orig_shapefile COMM_RG_01M_2016_4326.zip --aoi_wkt_file luxembourg.wkt --tiles_name communes --aoi_name lux --dest_dir .
 
 <center><img src='imgs/luxembourg-communes-random5k.png' width=600></center>
 
 
 ### Using your own code to define the GEE source image object.
 
-    geet download --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson  --gee_image_pycode crops.py --dataset_name crop --pixels_lonlat [100,100] --skip_if_exists --skip_confirm --n_processes 20
-
-assuming the file `crops.py` contains the following code
-
-        import ee
-
-        def get_ee_image():
-            return ee.Image('USGS/GFSAD1000_V1')\
-                     .select('landcover')\
-                     .visualize(min=0.0, max=5.0,
-                                palette = ['black', 'orange', 'brown', 
-                                           '02a50f', 'green', 'yellow'])
-
-        def get_dataset_name():
-            return 'crops'
-
+    geet download --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson  --dataset_def crops.py --pixels_lonlat [100,100] --skip_if_exists --skip_confirm --n_processes 20
 
-The `crops.py` will be saved under the destination folder for reference. The destination folder is created alongside the `tiles-file`.
+where `crops.py` contains a python `class DatasetDefinition` following the structure of the predefined ones under `defs`.  The files `crops.py` will be saved under the destination folder for reference. The destination folder is created alongside the `tiles_file`.
 
 ### Split geometries in train, test, val using geographic bands
 
 With a certain angle
 
     geet split --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson --nbands 8 --train_pct .5 --test_pct 0.3 --val_pct 0.2  --angle 0.78
 
@@ -100,15 +95,15 @@
 
 With respect to a dataset downloaded with segmentation labels.
 
     geet lp.compute --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson --dataset_name esa-world-cover
 
 We can also add the label proportions of the coarser tile in which each chip is embedded. First, we need to download the labels for each coarser tile from GEE.
 
-    geet download --tiles_file lux_partitions_communes_1a471c686e053.geojson  --gee_image_pycode esa-world-cover  --meters_per_pixel 20  --skip_if_exists 
+    geet download --tiles_file lux_partitions_communes_1a471c686e053.geojson  --dataset_def esa-world-cover  --meters_per_pixel 20  --skip_if_exists 
 
 then, compute the label proportions at this coarser tiles:
 
     geet lp.compute --tiles_file lux_partitions_communes_1a471c686e053.geojson --dataset_name esa-world-cover
 
 and then compute the label proportions from the coarser tiles.
 
@@ -119,13 +114,13 @@
 <img src='imgs/dataframe.png' width=800>
 
 
 ### Creating a dataset to share it
 
 This will create a zip file, with a pickle per chip containing a dictionary with the chip image, label and proportions.
 
-    geet zip.dataset --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson --foreign_tiles_file lux_partitions_communes_1a471c686e053.geojson --images_dataset_name sentinel2-rgb-median-2020 --labels_dataset_name esa-world-cover --readme_file README.txt  --label_map [10,20,30,40,50,60,70,80,90,95,100]
+    geet zip.dataset --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson --foreign_tiles_file lux_partitions_communes_1a471c686e053.geojson --images_dataset_def sentinel2-rgb-median-2020 --labels_dataset_def esa-world-cover --readme_file README.txt
 
 ### Some notes
 
 - the hash codes in the name files are computed using the participating geometries. This ensures that changing geometries do not override each other(such as for random partitions, or a wkt with slightly different coordinates).
 - the splits are saved both as a column in the corresponding `tiles_file` (which is a `geojson`) and in a separte `csv` file. This is to enable fast loading from `csv` (as loading from `geojson` might take a while, especially for large dataset).
```

### Comparing `geetiles-0.1.3/data/luxembourg.README.txt` & `geetiles-0.1.4/data/luxembourg.README.txt`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.3/data/luxembourg.wkt` & `geetiles-0.1.4/data/luxembourg.wkt`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.3/geetiles/cmds.py` & `geetiles-0.1.4/geetiles/cmds.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import numpy as np
 import shapely as sh
 from joblib import delayed
 from pyproj import CRS
 from progressbar import progressbar as pbar
 from skimage.io import imread
 import pickle
-from zipfile import ZipFile
+from zipfile import ZipFile, ZIP_DEFLATED
 
 
 from . import partitions
 from . import utils
 
 epsg4326 = utils.epsg4326
 
@@ -37,50 +37,54 @@
     else:
         p.split_per_partitions(nbands=nbands, angle=angle, 
                             train_pct=train_pct, test_pct=test_pct, val_pct=val_pct, 
                             other_partitions_id=foreign_tiles_name)
     p.save_splits()
 
 def label_proportions_compute(tiles_file, 
-                              dataset_name):
+                              labels_dataset_def):
     
+    label_dataset_definition = utils.get_dataset_definition(labels_dataset_def)
+    print ("loading tiles from", tiles_file, flush=True)
     p = partitions.PartitionSet.from_file(tiles_file)
     print(f"computing proportions for {len(p.data)} partitions")
-    p.add_proportions(dataset_name, n_jobs=1, transform_label_fn=lambda x: str(int(x)))
+    p.add_proportions(label_dataset_definition, n_jobs=1)
     print ("done!")
 
 def label_proportions_from_foreign(tiles_file,
                                    foreign_tiles_file,
-                                   dataset_name):
+                                   labels_dataset_def):
+
+    label_dataset_definition = utils.get_dataset_definition(labels_dataset_def)
+
     print ("loading primary tiles from", tiles_file, flush=True)
     p = partitions.PartitionSet.from_file(tiles_file)
     print ("loading foreign tiles from", foreign_tiles_file, flush=True)
     t = partitions.PartitionSet.from_file(foreign_tiles_file) 
     print ("intersecting geometries and computing label proportions from foreign tiles", flush=True)
-    p.add_foreign_proportions(dataset_name, t)    
+    p.add_foreign_proportions(label_dataset_definition, t)    
     print ("done!")
 
 
 def intersect_with_foreign(tiles_file, foreign_tiles_file):
     print ("loading primary tiles from", tiles_file, flush=True)
     p = partitions.PartitionSet.from_file(tiles_file)
     print ("loading foreign tiles from", foreign_tiles_file, flush=True)
     t = partitions.PartitionSet.from_file(foreign_tiles_file) 
     print ("intersecting geometries with foreign tiles", flush=True)
     p.add_foreign_partition(t)    
     print ("done!")
 
 
 def download(tiles_file, 
-             gee_image_pycode, 
+             dataset_def, 
              pixels_lonlat, meters_per_pixel, 
              max_downloads,
              shuffle,
              skip_if_exists,
-             dtype,
              ee_auth_mode,
              n_processes,
              skip_confirm=False):
     
     # sanity check
     if (pixels_lonlat is None and meters_per_pixel is None) or\
        (pixels_lonlat is not None and meters_per_pixel is not None):
@@ -92,19 +96,22 @@
             pixels_lonlat = [int(i) for i in pixels_lonlat]
             if not len(pixels_lonlat)==2:
                 raise Exception
         except:
             raise ValueError("'pixels_lonlat' must be a tuple of two ints such as --pixels_lonlat [100,100]")
 
 
+    dataset_definition = utils.get_dataset_definition(dataset_def)
+    dtype = dataset_definition.get_dtype()
+
     print (f"""
 using the following download specficication
 
 tiles_file:        {tiles_file}
-gee_image_pycode   {gee_image_pycode}
+dataset_def        {dataset_def}
 pixels_lonlat      {pixels_lonlat}
 meters_per_pixel   {meters_per_pixel}
 max_downloads      {max_downloads}
 shuffle            {shuffle}
 skip_if_exists     {skip_if_exists}
 dtype              {dtype}
 ee_auth_mode       {ee_auth_mode}
@@ -136,62 +143,28 @@
             ee.Authenticate(auth_mode = 'notebook')
         
     else:
         ee.Authenticate(auth_mode = ee_auth_mode)
 
     ee.Initialize()
 
-    # define gee image object
-    if gee_image_pycode == 'sentinel2-rgb-median-2020':
-        def maskS2clouds(image):
-            qa = image.select('MSK_CLDPRB')
-            mask = qa.lt(5)
-            return image.updateMask(mask)
-
-        gee_image = ee.ImageCollection('COPERNICUS/S2_SR_HARMONIZED')\
-                        .filterDate('2020-01-01', '2020-12-31')\
-                        .map(maskS2clouds)\
-                        .select('B4', 'B3', 'B2')\
-                        .median()\
-                        .visualize(min=0, max=4000)
-        
-        dataset_name = gee_image_pycode
-        
-    elif gee_image_pycode == 'esa-world-cover':
-        gee_image = ee.ImageCollection("ESA/WorldCover/v100").first()
-        dataset_name = gee_image_pycode
-        
-    elif os.path.isfile(gee_image_pycode):
-        print (f"evaluating python code at {gee_image_pycode}")
-        pyfname = gee_image_pycode
-        gee_image_pycode = open(pyfname).read()
-        try:
-            exec(gee_image_pycode, globals())
-            gee_image = get_ee_image()
-            dataset_name = get_dataset_name()
-        except Exception as e:
-            print ("--------------------------------------")
-            print (f"error executing your code at {pyfname}")
-            print ("--------------------------------------")
-            raise e
-        
-    else:
-        raise ValueError(f"file {gee_image_pycode} not found")
-        
+    gee_image = dataset_definition.get_gee_image()
+    dataset_name = dataset_definition.get_dataset_name()
+
     print ("-----------------------------------------------")
     print (f"dataset name is '{dataset_name}'")
     print ("-----------------------------------------------")
     # download the tiles
     p = partitions.PartitionSet.from_file(tiles_file)
 
     # save gee_image_codestr
     dest_dir = p.get_downloaded_tiles_dest_dir(dataset_name)
     os.makedirs(dest_dir, exist_ok=True)
-    with open(f"{dest_dir}.gee_image_pycode.py", "w") as f:
-        f.write(gee_image_pycode)
+    with open(f"{dest_dir}.dataset_def.py", "w") as f:
+        f.write(dataset_def)
 
     p.download_gee_tiles(gee_image, dataset_name, 
                          meters_per_pixel = meters_per_pixel, 
                          pixels_lonlat = pixels_lonlat,
                          dtype = dtype, 
                          shuffle = shuffle,
                          skip_if_exists = skip_if_exists,
@@ -295,158 +268,197 @@
 def select_partitions(orig_shapefile, aoi_wkt_file, aoi_name, tiles_name, dest_dir):
     """
     selects the geometries in 'orig_shafile' that have some intersention with aoi,
     assigns them an identifier and saves them in a new file.
     """
     print ("reading orig shapefile", flush=True)
     parts = gpd.read_file(orig_shapefile)
-
     if not  parts.crs == epsg4326:
            raise ValueError("'orig_shapefile' must be in epsg4326, lon/lat degrees "+\
                             f"but found \n{parts.crs}")
     
     with open(aoi_wkt_file, "r") as f:
         aoi = wkt.loads(f.read()) 
     
     print ("selecting geometries", flush=True)
     parts = [p for p in pbar(parts.geometry) if p.intersects(aoi)]
+    if len(parts)==0:
+        raise ValueError("no intersecting geometries found")
     # very small intersections probably are cause by numerical approximations
     # on the borders of the aoi
     parts = [p for p in parts if p.intersection(aoi).area>1e-5]
     
     parts = gpd.GeoDataFrame({'geometry': parts}, crs = CRS.from_epsg(4326))
+    parts.to_file("/tmp/bb.geojson", driver='GeoJSON')
     parts = partitions.PartitionSet(aoi_name, data=parts)
     print ()
     parts.save_as(dest_dir, tiles_name)
 
     return parts
 
 def zip_dataset(tiles_file, 
                 foreign_tiles_file,
-                images_dataset_name, 
-                labels_dataset_name, 
-                label_map,
+                images_dataset_def, 
+                labels_dataset_def, 
                 readme_file):
     
 
-    try:
-        label_map = eval(label_map)
-        label_map = [int(i) for i in label_map]
-    except:
-        raise ValueError("'label_map' must be a list of ints such as --label_map [10,20,95,100]")
-
-    if not 0 in label_map:
-        print ("adding class 0 to label map")
-        label_map = [0] + label_map
+    images_dataset = utils.get_dataset_definition(images_dataset_def)
+    images_dataset_name = images_dataset.get_dataset_name()
+
+    if labels_dataset_def is not None:
+        labels_dataset = utils.get_dataset_definition(labels_dataset_def)
+        labels_dataset_name = labels_dataset.get_dataset_name()
+    else:
+        labels_dataset_def = None
+        labels_dataset_name = None
 
-    labelmap = {str(i):j for i,j in enumerate(label_map)}
-    print ("using label map", labelmap)
 
     basedir = os.path.dirname(tiles_file)
     if basedir == "":
         basedir = "."
     filebase, _ = os.path.splitext(tiles_file)
     aoi_name = os.path.basename(tiles_file).split("_")[0]
     splits_file = f'{basedir}/{filebase}_splits.csv'
     expanded_file = f'{basedir}/{filebase}_expanded.geojson'
     destination_dir = f"{basedir}/{aoi_name}_{images_dataset_name}"
     if labels_dataset_name is not None:
         destination_dir += f"_{labels_dataset_name}"
 
-    s = foreign_tiles_file
-    foreign_tiles_name = s[s.find('_partitions_')+len('_partitions_'):].split("_")[0]
-
+    if foreign_tiles_file is not None:
+        s = foreign_tiles_file
+        foreign_tiles_name = s[s.find('_partitions_')+len('_partitions_'):].split("_")[0]
+    else:
+        foreign_tiles_name = None
+        
     print ("preparing folders")
     os.makedirs(f"{destination_dir}/data", exist_ok=True)
 
     def remove_hash(filename):
         filebase, extension = os.path.splitext(filename)
         if filebase.endswith('_splits'):
             r = "_".join(filebase.split("_")[:-2])+"_splits"+extension
         elif filebase.endswith('_expanded'):
             r = "_".join(filebase.split("_")[:-2])+"_expanded"+extension
         else:
             r = "_".join(filebase.split("_")[:-1])+extension            
         return r
     
-    print ("creating extended file for easy visualization of label proportions")
+    print ("creating expanded file for easy visualization of label proportions")
     p = partitions.PartitionSet.from_file(tiles_file)
     p.expand_proportions()
 
     # copy files
+    print ("copying metadata files")
     for filename in [tiles_file, foreign_tiles_file, splits_file, expanded_file]:
         if filename is not None and os.path.isfile(filename):
-            shutil.copyfile(f"{filename}", f"{destination_dir}/{remove_hash(os.path.basename(filename))}")
-
-    # splits file is just call 'splits.csv'
-    for filename in [splits_file]:
-        if filename is not None and os.path.isfile(filename):
-            shutil.copyfile(f"{filename}", f"{destination_dir}/splits.csv")
-
+            dest_file = f"{destination_dir}/{remove_hash(os.path.basename(filename))}"
+            if dest_file.endswith('splits.csv'):
+                # splits file is just called 'splits.csv'
+                dest_file = f"{destination_dir}/splits.csv"
+
+            shutil.copyfile(f"{filename}", dest_file)
+
+            # remove columns from other datasets in tiles file
+            if filename == tiles_file:
+                m = gpd.read_file(dest_file)
+                remove_columns = [c for c in m.columns if '_proportions' in c and labels_dataset_name is not None and not labels_dataset_name in c]
+                if len(remove_columns)>0:
+                    print ("removing data from other label datasets")
+                    m = m[[c for c in m.columns if not c in remove_columns]]
+                    m.to_file(dest_file, driver='GeoJSON')
 
     if readme_file is not None:
         shutil.copyfile(readme_file, f"{destination_dir}/README.txt")
 
-
-
-    labelmapi = {str(v):k for k,v in labelmap.items()}
-
-    def maplabel(label):
-
-        mlabel = np.zeros_like(label)
-        for v1,v2 in labelmapi.items():
-            mlabel[label==int(v1)] = v2
-
-        return mlabel
-    
-    def map_proportions(proportions):
-        return {str(labelmapi[str(k1)]): v1 for k1,v1 in proportions.items()}
-
     print ("reading tiles file")
     # read chip definitions
     c = gpd.read_file(tiles_file)
     # gather imgs, labels and proportions 
     partitionset_dir = os.path.splitext(f"{basedir}/{tiles_file}")[0]
+    n_skipped_chips = 0
+    n_included_chips = 0
+
+    included_chipids = []
+
     for _,i in pbar(c.iterrows(), max_value=len(c)):
         r = {}
         img_filename   = f"{partitionset_dir}/{images_dataset_name}/{i.identifier}.tif"
-        label_filename = f"{partitionset_dir}/{labels_dataset_name}/{i.identifier}.tif"
+        if labels_dataset_name is not None:
+            label_filename = f"{partitionset_dir}/{labels_dataset_name}/{i.identifier}.tif"
         if os.path.exists(img_filename):
+
             img = imread(img_filename).astype(np.int16)
-            label = imread(label_filename).astype(np.int16)
-            label = maplabel(label)
+            if 'map_values' in dir(images_dataset):
+                img = images_dataset.map_values(img)
+            
             coords = np.r_[i.geometry.envelope.boundary.coords]
             center_latlon = coords.mean(axis=0)[::-1]
             cmax = coords.max(axis=0)[::-1]
             cmin = coords.min(axis=0)[::-1]
             nw = np.r_[cmax[0], cmin[1]]
             se = np.r_[cmin[0], cmax[1]]    
 
-            r['chipmean'] = img
+            r['chip'] = img
             r['chip_id'] = i.identifier
-            r['label'] = label
             r['center_latlon'] = center_latlon
             r['corners'] = { 'nw': nw, 'se': se }
             
-            props = {}
-            props['partitions_aschip'] = map_proportions(i[f'{labels_dataset_name}_proportions'].copy())
-
-            props[f'partitions_{foreign_tiles_name}'] = i[f'{labels_dataset_name}_proportions_at_{foreign_tiles_name}'].copy()
-            props[f'partitions_{foreign_tiles_name}'] = map_proportions(props[f'partitions_{foreign_tiles_name}'])
-
-            r['label_proportions'] = props
-            with open(f"{destination_dir}/data/{i.identifier}.pkl", "wb") as f:
-                pickle.dump(r, f)
+            if labels_dataset_name is not None and os.path.exists(label_filename):
+                label = imread(label_filename).astype(np.int16)
+                if 'map_values' in dir(labels_dataset):
+                    label = labels_dataset.map_values(label)
+
+                r['label'] = label
+                props = {}
+                if f'{labels_dataset_name}_proportions' in i.keys():
+                    props['partitions_aschip'] = i[f'{labels_dataset_name}_proportions'].copy()
+
+                if foreign_tiles_name is not None and f'foreignid_{foreign_tiles_name}' in i.keys():
+                    props[f'partitions_{foreign_tiles_name}'] = i[f'{labels_dataset_name}_proportions_at_{foreign_tiles_name}'].copy()
+                    props[f'foreignid_{foreign_tiles_name}'] = i[f'foreignid_{foreign_tiles_name}']
+
+                if len(props)>0:
+                    r['label_proportions'] = props
+
+            if labels_dataset is None or\
+               'include_chip_in_dataset' not in dir(labels_dataset) or \
+               labels_dataset.include_chip_in_dataset(r):
+                with open(f"{destination_dir}/data/{i.identifier}.pkl", "wb") as f:
+                    pickle.dump(r, f)
+                n_included_chips += 1
+                included_chipids.append(r['chip_id'])
+            else:
+                n_skipped_chips += 1
+
+    print (f"including {n_included_chips} chips, and skipped {n_skipped_chips}")
+
+    # remove usused chips from metadata files
+    if n_included_chips < len(c):
+        chip_metafiles = [i for i in os.listdir(destination_dir) if 'aschip' in i]
+        for filename in chip_metafiles:
+            print ("removing unused chips from", filename, flush=True)
+            filename = f"{destination_dir}/{filename}"
+            if filename.endswith("splits.csv"):
+                f = pd.read_csv(filename)
+                f = f[f.identifier.isin(included_chipids)]
+                f.to_csv(filename, index=False)
+            elif filename.endswith(".geojson"):
+                f = gpd.read_file(filename)
+                f = f[f.identifier.isin(included_chipids)]
+                f.to_file(filename, driver='GeoJSON')
+            else:
+                continue
 
     # create zip file
     print ("zipping all content")
 
     # Create object of ZipFile
     zipfile = f"{destination_dir}.zip"
-    with ZipFile(zipfile, 'w') as zip_object:
+    with ZipFile(zipfile, 'w', compression=ZIP_DEFLATED, compresslevel=9) as zip_object:
         # Traverse all files in directory
         for folder_name, sub_folders, file_names in os.walk(destination_dir):
             for filename in file_names:
                 # Create filepath of files in directory
                 file_path = os.path.join(folder_name, filename)
                 # Add files to zip file
                 zip_object.write(file_path, file_path)
```

### Comparing `geetiles-0.1.3/geetiles/gee.py` & `geetiles-0.1.4/geetiles/gee.py`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.3/geetiles/main.py` & `geetiles-0.1.4/geetiles/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,54 +23,52 @@
     sel_parser.add_argument('--orig_shapefile', required=True, type=str, help='the shapefile with the geometries to select')
     sel_parser.add_argument('--aoi_name', required=True, type=str, help='the name of the AOI, used to name the resulting file')
     sel_parser.add_argument('--dest_dir', required=True, type=str, help='the folder to store the resulting file')
     sel_parser.add_argument('--tiles_name', required=True, type=str, help='a name for the selected geometries, used to name the resulting file')
 
     dwn_parser = subparsers.add_parser('download', help='downloads tiles from gee.')
     dwn_parser.add_argument('--tiles_file', required=True, type=str, help='output file produced by grid, random or select commands. It requires columns "geometry" and "identifier", and be in crs epsg4326. Downloaded tiles will be stored as geotiffs alongside in the same folder.')
-    dwn_parser.add_argument('--gee_image_pycode', required=True, type=str, help="A file with python code defining a function named get_ee_image that returns a gee Image object, and a function get_dataset_name returning a string. Can also be the string 'sentinel2-rgb-median-2020' or 'esa-world-cover' for built-in definitions")
+    dwn_parser.add_argument('--dataset_def', required=True, type=str, help="A file with python code defining a class with the dataset definition. See files under defs/ for examples . Can also be the string 'sentinel2-rgb-median-2020' or 'esa-world-cover' for built-in definitions")
     dwn_parser.add_argument('--pixels_lonlat', default=None, type=str, help='a tuple, if set, the tile will have this exact size in pixels, regardless the physical size. For instance --pixels_lonlat [100,100]')
     dwn_parser.add_argument('--meters_per_pixel', default=None, type=int, help='an int, if set, the tile pixel size will be computed to match the requested meters per pixel. You must use exactly one of --meters_per_pixel or --pixels_lonlat.')
     dwn_parser.add_argument('--max_downloads', default=None, type=str, help='max number of tiles to download.')
     dwn_parser.add_argument('--shuffle', default=False, action='store_true', help='if set, the order of tile downloading will be shuffled.')
     dwn_parser.add_argument('--skip_if_exists', default=False, action='store_true', help='if set, tiles already existing in the destination folder will not be downloaded.')
     dwn_parser.add_argument('--skip_confirm', default=False, action='store_true', help='if set, proceeds with no user confirmation.')
-    dwn_parser.add_argument('--dtype', default='uint8', type=str, help='numeric data type to store the images.')
     dwn_parser.add_argument('--ee_auth_mode', default=None, type=str, help='gee auth mode, see https://developers.google.com/earth-engine/apidocs/ee-authenticate.')
     dwn_parser.add_argument('--n_processes', default=10, type=int, help='number of parallel processes.')
 
     int_parser = subparsers.add_parser('intersect', help='for each tile, it gets the largest tile id from another set intersecting it.')
     int_parser.add_argument('--tiles_file', required=True, type=str, help='output file produced by grid, random or select commands. It requires columns "geometry" and "identifier", and be in crs epsg4326.')
     int_parser.add_argument('--foreign_tiles_file', required=True, type=str, help='the other tile set.')
 
     lpc_parser = subparsers.add_parser('lp.compute', help='computes labels proportions from downloaded dataset.')
     lpc_parser.add_argument('--tiles_file', required=True, type=str, help='output file produced by grid, random or select commands. It requires columns "geometry" and "identifier", and be in crs epsg4326.')
-    lpc_parser.add_argument('--dataset_name', required=True, type=str, help='name for the downloaded dataset to use. Must be a dataset with integer pixels denoting classes or labels.')
+    lpc_parser.add_argument('--labels_dataset_def', required=True, type=str, help='the dataset definition for which to compute proportions. Must have been downloaded previously. See "download --dataset-def".')
 
     lpf_parser = subparsers.add_parser('lp.from_foreign', help='computes labels proportions from another geometry partition on the same area by interseting geometries.')
     lpf_parser.add_argument('--tiles_file', required=True, type=str, help='output file produced by grid, random or select commands. It requires columns "geometry" and "identifier", and be in crs epsg4326.')
     lpf_parser.add_argument('--foreign_tiles_file', required=True, type=str, help='the tiles file from which labels will be taken to compute proportions by intersecting geometries.')
-    lpf_parser.add_argument('--dataset_name', required=True, type=str, help='name for the downloaded dataset to use on foreign_tiles_file. Must be a dataset with integer pixels denoting classes or labels.')
+    lpf_parser.add_argument('--labels_dataset_def', required=True, type=str, help='the dataset definition for which to compute proportions. Must have been downloaded previously. See "download --dataset-def".')
 
     split_parser = subparsers.add_parser('split', help='splits geometries in train, test and val with contiguous bands.')
     split_parser.add_argument('--tiles_file', required=True, type=str, help='output file produced by grid, random or select commands. It requires columns "geometry" and "identifier", and be in crs epsg4326.')
     split_parser.add_argument('--nbands', required=True, type=int, help='the number of bands to create.')
     split_parser.add_argument('--angle', required=True, type=float, help='angle to use for the bands, in [-1.5707,1.5707] = [-pi/2, pi/2].')
     split_parser.add_argument('--train_pct', required=True, type=float, help='percentage of train data, in [0,1].')
     split_parser.add_argument('--test_pct', required=True, type=float, help='percentage of test data, in [0,1].')
     split_parser.add_argument('--val_pct', required=True, type=float, help='percentage of validation data, in [0,1].')
     split_parser.add_argument('--foreign_tiles_name', required=False, default=None, type=str, help='add a split that keeps tiles within coarser foreign tiles together in the same split. Must have run lp.from_foreign before.')
 
     zip_parser = subparsers.add_parser('zip.dataset', help='assembles chips into pkls and zips all data.')
     zip_parser.add_argument('--tiles_file', required=True, type=str, help='output file produced by grid, random or select commands.')
     zip_parser.add_argument('--foreign_tiles_file', default=None, required=False, type=str, help='the tiles file from which foreign label proportions were computed.')
-    zip_parser.add_argument('--images_dataset_name', required=True, type=str, help="name of the dataset with images downloaded following the geometry of 'tiles_file'.")
-    zip_parser.add_argument('--labels_dataset_name', default=None, required=False, type=str, help="name of the dataset with labels downloaded following the geometry of 'tiles_file'.")
+    zip_parser.add_argument('--images_dataset_def', required=True, type=str, help="name of the dataset or python file used to download tiles (see 'dataset_def' in 'download').")
+    zip_parser.add_argument('--labels_dataset_def', default=None, required=False, type=str, help="name of the dataset or python file used to download tiles (see 'dataset_def' in 'download').")
     zip_parser.add_argument('--readme_file', default=None, required=False, type=str, help="name of the README.txt file to add to the zip file.")
-    zip_parser.add_argument('--label_map', required=True, type=str, help="a list of class ids present in the labels dataset to be mapped to the sequence [0,1,..] in the resulting zipped dataset")
 
     print ("-----------------------------------------------------------")
     print (f"Google Earth Engine dataset extractor utility {__version__}")
     print ("-----------------------------------------------------------")
     print ()
     args = parser.parse_args()
     if args.cmd == 'grid':
@@ -97,21 +95,20 @@
                           dest_dir       = args.dest_dir)
         
     elif args.cmd == 'download':
 
         print ("downloading tiles from GEE")
         try:
             download(   tiles_file        = args.tiles_file, 
-                        gee_image_pycode  = args.gee_image_pycode, 
+                        dataset_def       = args.dataset_def, 
                         pixels_lonlat     = args.pixels_lonlat, 
                         meters_per_pixel  = args.meters_per_pixel, 
                         max_downloads     = args.max_downloads,
                         shuffle           = args.shuffle,
                         skip_if_exists    = args.skip_if_exists,
-                        dtype             = args.dtype,
                         ee_auth_mode      = args.ee_auth_mode,
                         skip_confirm      = args.skip_confirm, 
                         n_processes       = args.n_processes
                     )
         except ValueError as e:
             print ("ERROR.", e)
             quit(-1)
@@ -120,21 +117,21 @@
         print ("computing intersections with foreign tiles")
         intersect_with_foreign(tiles_file         = args.tiles_file,
                                foreign_tiles_file = args.foreign_tiles_file)
 
     elif args.cmd == 'lp.compute':
         print ("computing proportions")
         label_proportions_compute(tiles_file = args.tiles_file, 
-                                  dataset_name = args.dataset_name)      
+                                  labels_dataset_def = args.labels_dataset_def)      
 
     elif args.cmd == 'lp.from_foreign':
         print ("computing proportions from foreign tiles")
         label_proportions_from_foreign(tiles_file         = args.tiles_file,
                                        foreign_tiles_file = args.foreign_tiles_file,
-                                       dataset_name       = args.dataset_name)  
+                                       labels_dataset_def = args.labels_dataset_def)  
         
     elif args.cmd == 'split':
         print ("splitting bands")
         split(tiles_file         = args.tiles_file, 
               nbands             = args.nbands, 
               angle              = args.angle,
               train_pct          = args.train_pct, 
@@ -142,11 +139,10 @@
               val_pct            = args.val_pct,
               foreign_tiles_name = args.foreign_tiles_name)
         
     elif args.cmd == 'zip.dataset':
         print ("zipping dataset")
         zip_dataset(tiles_file          = args.tiles_file, 
                     foreign_tiles_file  = args.foreign_tiles_file,
-                    images_dataset_name = args.images_dataset_name, 
-                    labels_dataset_name = args.labels_dataset_name, 
-                    label_map           = args.label_map,
+                    images_dataset_def  = args.images_dataset_def, 
+                    labels_dataset_def  = args.labels_dataset_def, 
                     readme_file         = args.readme_file)
```

### Comparing `geetiles-0.1.3/geetiles/partitions.py` & `geetiles-0.1.4/geetiles/partitions.py`

 * *Files 7% similar despite different names*

```diff
@@ -225,46 +225,50 @@
         """
         cols_proportions = [i for i in self.data.columns if "_proportions" in i]
         if len(cols_proportions)==0:
             print ("no proportions found in", self.origin_file)
             return
         
         for col in cols_proportions:
+            #self.data = self.data[[c for c in self.data.columns if not c.startswith(f"{col}__")]]
             self.data = utils.expand_dict_column(self.data, col)
             
         f,ext = os.path.splitext(self.origin_file)
         expanded_fname = f'{f}_expanded{ext}'
         self.data.to_file(expanded_fname, driver='GeoJSON')
         print ("saved expanded file to", expanded_fname)
 
-    def add_proportions(self, image_collection_name, n_jobs=5, transform_label_fn=lambda x: x):
+    def add_proportions(self, labels_dataset_def, n_jobs=5):
         """
         adds proportions from an image collection with the same geometry (such when this partitionset
         is an rgb image collection and image_collection_name contains segmentation masks)
         """
         def f(identifier, geometry):
             proportions = Partition(partitionset = self, 
                                     identifier = identifier, 
                                     geometry = geometry, 
                                     crs = self.data.crs).compute_proportions_from_raster(
-                                                                image_collection_name,
-                                                                transform_label_fn = transform_label_fn,
+                                                                labels_dataset_def
                                                             )
             return proportions
-
-        r = utils.mParallel(n_jobs=n_jobs, verbose=30)(delayed(f)(i.identifier, i.geometry) for i in self.data.itertuples())
-        self.data[f"{image_collection_name}_proportions"] = r
+        
+        if n_jobs==1:
+            r = [f(i.identifier, i.geometry) for i in pbar(self.data.itertuples(), max_value=len(self.data))]
+        else:
+            r = utils.mParallel(n_jobs=n_jobs, verbose=30)(delayed(f)(i.identifier, i.geometry) for i in self.data.itertuples())
+        self.data[f"{labels_dataset_def.get_dataset_name()}_proportions"] = r
         print()
         self.save()
 
-    def add_foreign_proportions(self, image_collection_name, foreign_partitionset):
+    def add_foreign_proportions(self, label_dataset_definition, foreign_partitionset):
         """
         add class proportions of the geometries of this partitionset when embedded in a coarser partitionset.
         see Partition.compute_foreign_proportions below
         """
+        image_collection_name = label_dataset_definition.get_dataset_name()
         parts = self.get_partitions()
         proportions = []
         foreign_ids = []
         for part in pbar(parts):
             foreign_proportions, foreign_identifier = part.compute_foreign_proportions(image_collection_name, foreign_partitionset)
             #proportions.append({'partition_id': foreign_identifier, 
             #                    'proportions': foreign_proportions})
@@ -398,23 +402,35 @@
 
     def get_tif(self, image_collection_name):
         basedir = self.partitionset_dir + "/" + image_collection_name
         filename = f"{basedir}/{self.identifier}.tif"
         img = imread(filename)
         return img
     
-    def compute_proportions_from_raster(self, image_collection_name, transform_label_fn=lambda x: x):
+    def compute_proportions_from_raster(self, labels_dataset_def):
+
+        # retrieve label array from disk
+        image_collection_name = labels_dataset_def.get_dataset_name()
         basedir = self.partitionset_dir + "/" + image_collection_name
         filename = f"{basedir}/{self.identifier}.tif"
         img = imread(filename)
+
+        # map image values according to dataset definition
+        img = labels_dataset_def.map_values(img)
+
+        # account for proportions only within the geometry 
+        # (in case it does not match the rectangular image)
         mask = utils.get_binary_mask(self.geometry, img.shape)
         img = img[mask==1]
-        r = {transform_label_fn(k):v for k,v in zip(*np.unique(img, return_counts=True))}        
+
+        # compute proportions
+        r = {k:v for k,v in zip(*np.unique(img, return_counts=True))}        
         total = sum(r.values())
-        r = {k:v/total for k,v in r.items()}
+        r = {str(k):v/total for k,v in r.items()}
+
         return r
     
     def compute_foreign_partition(self, foreign_partition_set):
         """
         returns the id of the foreign partition (geometry) intersecting this one
         """        
         t = foreign_partition_set
```

### Comparing `geetiles-0.1.3/geetiles.egg-info/PKG-INFO` & `geetiles-0.1.4/geetiles.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geetiles
-Version: 0.1.3
+Version: 0.1.4
 Summary: download Google Earth Engine datasets to tiles as geotiff arrays
 Home-page: https://github.com/rramosp/geetiles
 Author: raul ramos
 Author-email: raul.ramos@udea.edu.co
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -31,24 +31,24 @@
 this generates file `./lux_partitions_aschips_14c55eb7d417f.geojson`. Use a tool such as [QGIS](https://qgis.org/) to view it.
 
 <center><img src='imgs/luxgrid.png' width=800></center>
 
 
 ### 2. download tiles
 
-    geet download --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson  --gee_image_pycode sentinel2-rgb-median-2020 --pixels_lonlat [100,100] --skip_if_exists
+    geet download --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson  --dataset_def sentinel2-rgb-median-2020 --pixels_lonlat [100,100] --skip_if_exists
 
 
 this fills the folder `lux_partitions_aschips_14c55eb7d417f/sentinel2-rgb-median-2020` with RGB geotiff images of size 100x100 pixels.
 
-If using `sentinel2-rgb-median-2020` as `gee_image_pycode`, which is an alias to [Sentinel-2 MSI Level 2-A](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S2_SR) GEE dataset, taking the median of the cloudless chips over the year 2020.
+If using `sentinel2-rgb-median-2020` as `dataset_def`, which is an alias to [Sentinel-2 MSI Level 2-A](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S2_SR) GEE dataset, taking the median of the cloudless chips over the year 2020.
 
 <center><img src='imgs/sentinel2.png' width=800></center>
 
-If using `esa-world-cover` as `gee_image_pycode`, which is an alias to [ESA WorldCover 10m v100](https://developers.google.com/earth-engine/datasets/catalog/ESA_WorldCover_v100) GEE dataset.
+If using `esa-world-cover` as `dataset_def`, which is an alias to [ESA WorldCover 10m v100](https://developers.google.com/earth-engine/datasets/catalog/ESA_WorldCover_v100) GEE dataset.
 
 <center><img src='imgs/landcover.png' width=800></center>
 
 
 ## Other usages
 
 ### Other ways to create the set of tiles (shapes) 
@@ -64,32 +64,17 @@
       geet select --orig_shapefile COMM_RG_01M_2016_4326.zip --aoi_wkt_file luxembourg.wkt --tiles_name communes --aoi_name lux --dest_dir .
 
 <center><img src='imgs/luxembourg-communes-random5k.png' width=600></center>
 
 
 ### Using your own code to define the GEE source image object.
 
-    geet download --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson  --gee_image_pycode crops.py --dataset_name crop --pixels_lonlat [100,100] --skip_if_exists --skip_confirm --n_processes 20
+    geet download --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson  --dataset_def crops.py --pixels_lonlat [100,100] --skip_if_exists --skip_confirm --n_processes 20
 
-assuming the file `crops.py` contains the following code
-
-        import ee
-
-        def get_ee_image():
-            return ee.Image('USGS/GFSAD1000_V1')\
-                     .select('landcover')\
-                     .visualize(min=0.0, max=5.0,
-                                palette = ['black', 'orange', 'brown', 
-                                           '02a50f', 'green', 'yellow'])
-
-        def get_dataset_name():
-            return 'crops'
-
-
-The `crops.py` will be saved under the destination folder for reference. The destination folder is created alongside the `tiles-file`.
+where `crops.py` contains a python `class DatasetDefinition` following the structure of the predefined ones under `defs`.  The files `crops.py` will be saved under the destination folder for reference. The destination folder is created alongside the `tiles_file`.
 
 ### Split geometries in train, test, val using geographic bands
 
 With a certain angle
 
     geet split --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson --nbands 8 --train_pct .5 --test_pct 0.3 --val_pct 0.2  --angle 0.78
 
@@ -110,15 +95,15 @@
 
 With respect to a dataset downloaded with segmentation labels.
 
     geet lp.compute --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson --dataset_name esa-world-cover
 
 We can also add the label proportions of the coarser tile in which each chip is embedded. First, we need to download the labels for each coarser tile from GEE.
 
-    geet download --tiles_file lux_partitions_communes_1a471c686e053.geojson  --gee_image_pycode esa-world-cover  --meters_per_pixel 20  --skip_if_exists 
+    geet download --tiles_file lux_partitions_communes_1a471c686e053.geojson  --dataset_def esa-world-cover  --meters_per_pixel 20  --skip_if_exists 
 
 then, compute the label proportions at this coarser tiles:
 
     geet lp.compute --tiles_file lux_partitions_communes_1a471c686e053.geojson --dataset_name esa-world-cover
 
 and then compute the label proportions from the coarser tiles.
 
@@ -129,13 +114,13 @@
 <img src='imgs/dataframe.png' width=800>
 
 
 ### Creating a dataset to share it
 
 This will create a zip file, with a pickle per chip containing a dictionary with the chip image, label and proportions.
 
-    geet zip.dataset --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson --foreign_tiles_file lux_partitions_communes_1a471c686e053.geojson --images_dataset_name sentinel2-rgb-median-2020 --labels_dataset_name esa-world-cover --readme_file README.txt  --label_map [10,20,30,40,50,60,70,80,90,95,100]
+    geet zip.dataset --tiles_file lux_partitions_aschips_14c55eb7d417f.geojson --foreign_tiles_file lux_partitions_communes_1a471c686e053.geojson --images_dataset_def sentinel2-rgb-median-2020 --labels_dataset_def esa-world-cover --readme_file README.txt
 
 ### Some notes
 
 - the hash codes in the name files are computed using the participating geometries. This ensures that changing geometries do not override each other(such as for random partitions, or a wkt with slightly different coordinates).
 - the splits are saved both as a column in the corresponding `tiles_file` (which is a `geojson`) and in a separte `csv` file. This is to enable fast loading from `csv` (as loading from `geojson` might take a while, especially for large dataset).
```

### Comparing `geetiles-0.1.3/geetiles.egg-info/SOURCES.txt` & `geetiles-0.1.4/geetiles.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 geetiles.egg-info/PKG-INFO
 geetiles.egg-info/SOURCES.txt
 geetiles.egg-info/dependency_links.txt
 geetiles.egg-info/entry_points.txt
 geetiles.egg-info/not-zip-safe
 geetiles.egg-info/requires.txt
 geetiles.egg-info/top_level.txt
+geetiles/defs/esaworldcover.py
+geetiles/defs/humanpop2015.py
+geetiles/defs/sentinel2rgbmedian2020.py
+geetiles/defs/soilphbenelux.py
+geetiles/defs/soilphcolombia.py
+geetiles/defs/treecover2020.py
 imgs/dataframe.png
 imgs/landcover.png
 imgs/luxembourg-bands-communes.png
 imgs/luxembourg-bands.png
 imgs/luxembourg-communes-random5k.png
 imgs/luxembourg-communes.png
 imgs/luxembourg-random-5k.png
```

### Comparing `geetiles-0.1.3/imgs/dataframe.png` & `geetiles-0.1.4/imgs/dataframe.png`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.3/imgs/landcover.png` & `geetiles-0.1.4/imgs/landcover.png`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.3/imgs/luxembourg-bands-communes.png` & `geetiles-0.1.4/imgs/luxembourg-bands-communes.png`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.3/imgs/luxembourg-bands.png` & `geetiles-0.1.4/imgs/luxembourg-bands.png`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.3/imgs/luxembourg-communes-random5k.png` & `geetiles-0.1.4/imgs/luxembourg-communes-random5k.png`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.3/imgs/luxembourg-communes.png` & `geetiles-0.1.4/imgs/luxembourg-communes.png`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.3/imgs/luxembourg-random-5k.png` & `geetiles-0.1.4/imgs/luxembourg-random-5k.png`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.3/imgs/luxembourg-splits.png` & `geetiles-0.1.4/imgs/luxembourg-splits.png`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.3/imgs/luxgrid.png` & `geetiles-0.1.4/imgs/luxgrid.png`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.3/imgs/sentinel2.png` & `geetiles-0.1.4/imgs/sentinel2.png`

 * *Files identical despite different names*

### Comparing `geetiles-0.1.3/setup.py` & `geetiles-0.1.4/setup.py`

 * *Files identical despite different names*

