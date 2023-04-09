# Comparing `tmp/metaseg-0.3.1.tar.gz` & `tmp/metaseg-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.3.1.tar", last modified: Sat Apr  8 23:50:19 2023, max compression
+gzip compressed data, was "metaseg-0.3.3.tar", last modified: Sun Apr  9 10:31:28 2023, max compression
```

## Comparing `metaseg-0.3.1.tar` & `metaseg-0.3.3.tar`

### file list

```diff
@@ -1,37 +1,40 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-08 23:50:19.536091 metaseg-0.3.1/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.3.1/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.3.1/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1777 2023-04-08 23:50:19.536091 metaseg-0.3.1/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1503 2023-04-08 23:49:11.000000 metaseg-0.3.1/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-08 23:50:19.519424 metaseg-0.3.1/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      492 2023-04-08 23:50:05.000000 metaseg-0.3.1/metaseg/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-08 23:50:13.000000 metaseg-0.3.1/metaseg/app.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15117 2023-04-07 13:09:43.000000 metaseg-0.3.1/metaseg/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-06 18:52:09.000000 metaseg-0.3.1/metaseg/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3686 2023-04-08 23:50:13.000000 metaseg-0.3.1/metaseg/demo.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-08 23:50:19.526091 metaseg-0.3.1/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.3.1/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.3.1/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.3.1/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.3.1/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.3.1/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.3.1/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.3.1/metaseg/modeling/transformer.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-06 18:52:09.000000 metaseg-0.3.1/metaseg/predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-08 23:50:19.532757 metaseg-0.3.1/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      310 2023-04-08 23:50:14.000000 metaseg-0.3.1/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.3.1/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)      518 2023-04-08 23:50:13.000000 metaseg-0.3.1/metaseg/utils/data_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-08 17:15:08.000000 metaseg-0.3.1/metaseg/utils/file_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.3.1/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.3.1/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-08 23:50:19.522757 metaseg-0.3.1/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1777 2023-04-08 23:50:19.000000 metaseg-0.3.1/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      730 2023-04-08 23:50:19.000000 metaseg-0.3.1/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-08 23:50:19.000000 metaseg-0.3.1/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      226 2023-04-08 23:50:19.000000 metaseg-0.3.1/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-08 23:50:19.000000 metaseg-0.3.1/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.3.1/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      139 2023-04-08 09:21:23.000000 metaseg-0.3.1/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-08 23:50:19.539424 metaseg-0.3.1/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.3.1/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:31:28.379747 metaseg-0.3.3/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.3.3/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.3.3/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2122 2023-04-09 10:31:28.379747 metaseg-0.3.3/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1848 2023-04-09 10:31:02.000000 metaseg-0.3.3/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:31:28.369747 metaseg-0.3.3/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      562 2023-04-09 10:28:45.000000 metaseg-0.3.3/metaseg/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3686 2023-04-09 10:19:56.000000 metaseg-0.3.3/metaseg/auto_mask_demo.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15117 2023-04-07 13:09:43.000000 metaseg-0.3.3/metaseg/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-06 18:52:09.000000 metaseg-0.3.3/metaseg/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2309 2023-04-09 10:27:56.000000 metaseg-0.3.3/metaseg/manuel_mask_demo.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:31:28.373081 metaseg-0.3.3/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.3.3/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.3.3/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.3.3/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.3.3/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.3.3/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.3.3/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.3.3/metaseg/modeling/transformer.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-06 18:52:09.000000 metaseg-0.3.3/metaseg/predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:31:28.376414 metaseg-0.3.3/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      310 2023-04-09 10:19:56.000000 metaseg-0.3.3/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.3.3/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      518 2023-04-09 10:19:56.000000 metaseg-0.3.3/metaseg/utils/data_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-08 17:15:08.000000 metaseg-0.3.3/metaseg/utils/file_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.3.3/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.3.3/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:31:28.376414 metaseg-0.3.3/metaseg/webapp/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:19:56.000000 metaseg-0.3.3/metaseg/webapp/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-09 10:19:56.000000 metaseg-0.3.3/metaseg/webapp/app.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:31:28.373081 metaseg-0.3.3/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2122 2023-04-09 10:31:28.000000 metaseg-0.3.3/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      802 2023-04-09 10:31:28.000000 metaseg-0.3.3/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-09 10:31:28.000000 metaseg-0.3.3/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      226 2023-04-09 10:31:28.000000 metaseg-0.3.3/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-09 10:31:28.000000 metaseg-0.3.3/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.3.3/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      139 2023-04-08 09:21:23.000000 metaseg-0.3.3/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-09 10:31:28.379747 metaseg-0.3.3/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.3.3/setup.py
```

### Comparing `metaseg-0.3.1/LICENSE` & `metaseg-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.1/PKG-INFO` & `metaseg-0.3.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.3.1
+Version: 0.3.3
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -37,31 +37,44 @@
 
 # If gpu memory is not enough, reduce the points_per_side and points_per_batch.
 
 # For image
 
 autoseg_image = SegAutoMaskGenerator().save_image(
     source="image.jpg",
-    model_type="vit_l",
+    model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=0,
 )
 
 # For video
 
 autoseg_video = SegAutoMaskGenerator().save_video(
     source="video.mp4",
-    model_type="vit_l",
+    model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=1000,
 )
+
+# For manuel box selection
+from metaseg import SegManualMaskGenerator
+
+seg_manual_mask_generator = SegManualMaskGenerator().save_image(
+    source="image.jpg",
+    model_type="vit_l", # vit_l, vit_h, vit_b
+    x0=100,
+    y0=100,
+    x1=200,
+    y1=200,
+)
 ```
 
 # Extra Features
 
 - [x] Support for video files
 - [x] Support for pip installation
 - [x] Support for web application
+- [x] Support for box to polygon conversion
 - [x] Support for automatic download model weights
```

#### html2text {}

```diff
@@ -1,18 +1,23 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.3.1 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.3.3 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskGenerator # If
 gpu memory is not enough, reduce the points_per_side and points_per_batch. #
 For image autoseg_image = SegAutoMaskGenerator().save_image
-( source="image.jpg", model_type="vit_l", points_per_side=16,
-points_per_batch=64, min_area=0, ) # For video autoseg_video =
-SegAutoMaskGenerator().save_video( source="video.mp4", model_type="vit_l",
-points_per_side=16, points_per_batch=64, min_area=1000, ) ``` # Extra Features
-- [x] Support for video files - [x] Support for pip installation - [x] Support
-for web application - [x] Support for automatic download model weights
+( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b
+points_per_side=16, points_per_batch=64, min_area=0, ) # For video
+autoseg_video = SegAutoMaskGenerator().save_video( source="video.mp4",
+model_type="vit_l", # vit_l, vit_h, vit_b points_per_side=16,
+points_per_batch=64, min_area=1000, ) # For manuel box selection from metaseg
+import SegManualMaskGenerator seg_manual_mask_generator =
+SegManualMaskGenerator().save_image( source="image.jpg", model_type="vit_l", #
+vit_l, vit_h, vit_b x0=100, y0=100, x1=200, y1=200, ) ``` # Extra Features -
+[x] Support for video files - [x] Support for pip installation - [x] Support
+for web application - [x] Support for box to polygon conversion - [x] Support
+for automatic download model weights
```

### Comparing `metaseg-0.3.1/README.md` & `metaseg-0.3.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -25,31 +25,44 @@
 
 # If gpu memory is not enough, reduce the points_per_side and points_per_batch.
 
 # For image
 
 autoseg_image = SegAutoMaskGenerator().save_image(
     source="image.jpg",
-    model_type="vit_l",
+    model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=0,
 )
 
 # For video
 
 autoseg_video = SegAutoMaskGenerator().save_video(
     source="video.mp4",
-    model_type="vit_l",
+    model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=1000,
 )
+
+# For manuel box selection
+from metaseg import SegManualMaskGenerator
+
+seg_manual_mask_generator = SegManualMaskGenerator().save_image(
+    source="image.jpg",
+    model_type="vit_l", # vit_l, vit_h, vit_b
+    x0=100,
+    y0=100,
+    x1=200,
+    y1=200,
+)
 ```
 
 # Extra Features
 
 - [x] Support for video files
 - [x] Support for pip installation
 - [x] Support for web application
+- [x] Support for box to polygon conversion
 - [x] Support for automatic download model weights
```

#### html2text {}

```diff
@@ -2,13 +2,18 @@
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskGenerator # If
 gpu memory is not enough, reduce the points_per_side and points_per_batch. #
 For image autoseg_image = SegAutoMaskGenerator().save_image
-( source="image.jpg", model_type="vit_l", points_per_side=16,
-points_per_batch=64, min_area=0, ) # For video autoseg_video =
-SegAutoMaskGenerator().save_video( source="video.mp4", model_type="vit_l",
-points_per_side=16, points_per_batch=64, min_area=1000, ) ``` # Extra Features
-- [x] Support for video files - [x] Support for pip installation - [x] Support
-for web application - [x] Support for automatic download model weights
+( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b
+points_per_side=16, points_per_batch=64, min_area=0, ) # For video
+autoseg_video = SegAutoMaskGenerator().save_video( source="video.mp4",
+model_type="vit_l", # vit_l, vit_h, vit_b points_per_side=16,
+points_per_batch=64, min_area=1000, ) # For manuel box selection from metaseg
+import SegManualMaskGenerator seg_manual_mask_generator =
+SegManualMaskGenerator().save_image( source="image.jpg", model_type="vit_l", #
+vit_l, vit_h, vit_b x0=100, y0=100, x1=200, y1=200, ) ``` # Extra Features -
+[x] Support for video files - [x] Support for pip installation - [x] Support
+for web application - [x] Support for box to polygon conversion - [x] Support
+for automatic download model weights
```

### Comparing `metaseg-0.3.1/metaseg/app.py` & `metaseg-0.3.3/metaseg/webapp/app.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.1/metaseg/automatic_mask_generator.py` & `metaseg-0.3.3/metaseg/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.1/metaseg/build_sam.py` & `metaseg-0.3.3/metaseg/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.1/metaseg/demo.py` & `metaseg-0.3.3/metaseg/auto_mask_demo.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.1/metaseg/modeling/common.py` & `metaseg-0.3.3/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.1/metaseg/modeling/image_encoder.py` & `metaseg-0.3.3/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.1/metaseg/modeling/mask_decoder.py` & `metaseg-0.3.3/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.1/metaseg/modeling/prompt_encoder.py` & `metaseg-0.3.3/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.1/metaseg/modeling/sam.py` & `metaseg-0.3.3/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.1/metaseg/modeling/transformer.py` & `metaseg-0.3.3/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.1/metaseg/predictor.py` & `metaseg-0.3.3/metaseg/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.1/metaseg/utils/amg.py` & `metaseg-0.3.3/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.1/metaseg/utils/data_utils.py` & `metaseg-0.3.3/metaseg/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.1/metaseg/utils/file_utils.py` & `metaseg-0.3.3/metaseg/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.1/metaseg/utils/onnx.py` & `metaseg-0.3.3/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.1/metaseg/utils/transforms.py` & `metaseg-0.3.3/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.1/metaseg.egg-info/PKG-INFO` & `metaseg-0.3.3/metaseg.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.3.1
+Version: 0.3.3
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -37,31 +37,44 @@
 
 # If gpu memory is not enough, reduce the points_per_side and points_per_batch.
 
 # For image
 
 autoseg_image = SegAutoMaskGenerator().save_image(
     source="image.jpg",
-    model_type="vit_l",
+    model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=0,
 )
 
 # For video
 
 autoseg_video = SegAutoMaskGenerator().save_video(
     source="video.mp4",
-    model_type="vit_l",
+    model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=1000,
 )
+
+# For manuel box selection
+from metaseg import SegManualMaskGenerator
+
+seg_manual_mask_generator = SegManualMaskGenerator().save_image(
+    source="image.jpg",
+    model_type="vit_l", # vit_l, vit_h, vit_b
+    x0=100,
+    y0=100,
+    x1=200,
+    y1=200,
+)
 ```
 
 # Extra Features
 
 - [x] Support for video files
 - [x] Support for pip installation
 - [x] Support for web application
+- [x] Support for box to polygon conversion
 - [x] Support for automatic download model weights
```

#### html2text {}

```diff
@@ -1,18 +1,23 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.3.1 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.3.3 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskGenerator # If
 gpu memory is not enough, reduce the points_per_side and points_per_batch. #
 For image autoseg_image = SegAutoMaskGenerator().save_image
-( source="image.jpg", model_type="vit_l", points_per_side=16,
-points_per_batch=64, min_area=0, ) # For video autoseg_video =
-SegAutoMaskGenerator().save_video( source="video.mp4", model_type="vit_l",
-points_per_side=16, points_per_batch=64, min_area=1000, ) ``` # Extra Features
-- [x] Support for video files - [x] Support for pip installation - [x] Support
-for web application - [x] Support for automatic download model weights
+( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b
+points_per_side=16, points_per_batch=64, min_area=0, ) # For video
+autoseg_video = SegAutoMaskGenerator().save_video( source="video.mp4",
+model_type="vit_l", # vit_l, vit_h, vit_b points_per_side=16,
+points_per_batch=64, min_area=1000, ) # For manuel box selection from metaseg
+import SegManualMaskGenerator seg_manual_mask_generator =
+SegManualMaskGenerator().save_image( source="image.jpg", model_type="vit_l", #
+vit_l, vit_h, vit_b x0=100, y0=100, x1=200, y1=200, ) ``` # Extra Features -
+[x] Support for video files - [x] Support for pip installation - [x] Support
+for web application - [x] Support for box to polygon conversion - [x] Support
+for automatic download model weights
```

### Comparing `metaseg-0.3.1/metaseg.egg-info/SOURCES.txt` & `metaseg-0.3.3/metaseg.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 metaseg/__init__.py
-metaseg/app.py
+metaseg/auto_mask_demo.py
 metaseg/automatic_mask_generator.py
 metaseg/build_sam.py
-metaseg/demo.py
+metaseg/manuel_mask_demo.py
 metaseg/predictor.py
 metaseg.egg-info/PKG-INFO
 metaseg.egg-info/SOURCES.txt
 metaseg.egg-info/dependency_links.txt
 metaseg.egg-info/requires.txt
 metaseg.egg-info/top_level.txt
 metaseg/modeling/__init__.py
@@ -24,8 +24,10 @@
 metaseg/modeling/sam.py
 metaseg/modeling/transformer.py
 metaseg/utils/__init__.py
 metaseg/utils/amg.py
 metaseg/utils/data_utils.py
 metaseg/utils/file_utils.py
 metaseg/utils/onnx.py
-metaseg/utils/transforms.py
+metaseg/utils/transforms.py
+metaseg/webapp/__init__.py
+metaseg/webapp/app.py
```

### Comparing `metaseg-0.3.1/setup.py` & `metaseg-0.3.3/setup.py`

 * *Files identical despite different names*

