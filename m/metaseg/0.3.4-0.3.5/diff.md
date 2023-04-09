# Comparing `tmp/metaseg-0.3.4.tar.gz` & `tmp/metaseg-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.3.4.tar", last modified: Sun Apr  9 13:58:50 2023, max compression
+gzip compressed data, was "metaseg-0.3.5.tar", last modified: Sun Apr  9 14:15:24 2023, max compression
```

## Comparing `metaseg-0.3.4.tar` & `metaseg-0.3.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:58:50.585914 metaseg-0.3.4/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.3.4/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.3.4/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2144 2023-04-09 13:58:50.585914 metaseg-0.3.4/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1870 2023-04-09 13:44:17.000000 metaseg-0.3.4/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:58:50.565914 metaseg-0.3.4/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      556 2023-04-09 13:58:07.000000 metaseg-0.3.4/metaseg/__init__.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:58:50.579248 metaseg-0.3.4/metaseg/generator/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:51:55.000000 metaseg-0.3.4/metaseg/generator/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-09 13:58:07.000000 metaseg-0.3.4/metaseg/generator/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-06 18:52:09.000000 metaseg-0.3.4/metaseg/generator/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-06 18:52:09.000000 metaseg-0.3.4/metaseg/generator/predictor.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5580 2023-04-09 13:58:07.000000 metaseg-0.3.4/metaseg/mask_predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:58:50.582581 metaseg-0.3.4/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.3.4/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.3.4/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.3.4/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.3.4/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.3.4/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.3.4/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.3.4/metaseg/modeling/transformer.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:58:50.585914 metaseg-0.3.4/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      310 2023-04-09 10:19:56.000000 metaseg-0.3.4/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.3.4/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)      518 2023-04-09 10:19:56.000000 metaseg-0.3.4/metaseg/utils/data_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-08 17:15:08.000000 metaseg-0.3.4/metaseg/utils/file_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.3.4/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.3.4/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:58:50.585914 metaseg-0.3.4/metaseg/webapp/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:19:56.000000 metaseg-0.3.4/metaseg/webapp/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-09 10:19:56.000000 metaseg-0.3.4/metaseg/webapp/app.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:58:50.572581 metaseg-0.3.4/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2144 2023-04-09 13:58:50.000000 metaseg-0.3.4/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      834 2023-04-09 13:58:50.000000 metaseg-0.3.4/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-09 13:58:50.000000 metaseg-0.3.4/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      226 2023-04-09 13:58:50.000000 metaseg-0.3.4/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-09 13:58:50.000000 metaseg-0.3.4/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.3.4/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      139 2023-04-08 09:21:23.000000 metaseg-0.3.4/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-09 13:58:50.585914 metaseg-0.3.4/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.3.4/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 14:15:24.909224 metaseg-0.3.5/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.3.5/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.3.5/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2125 2023-04-09 14:15:24.909224 metaseg-0.3.5/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1851 2023-04-09 14:07:11.000000 metaseg-0.3.5/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 14:15:24.899224 metaseg-0.3.5/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      556 2023-04-09 14:02:26.000000 metaseg-0.3.5/metaseg/__init__.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 14:15:24.899224 metaseg-0.3.5/metaseg/generator/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:51:55.000000 metaseg-0.3.5/metaseg/generator/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-09 13:58:07.000000 metaseg-0.3.5/metaseg/generator/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-06 18:52:09.000000 metaseg-0.3.5/metaseg/generator/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-06 18:52:09.000000 metaseg-0.3.5/metaseg/generator/predictor.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5580 2023-04-09 13:58:07.000000 metaseg-0.3.5/metaseg/mask_predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 14:15:24.902557 metaseg-0.3.5/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.3.5/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.3.5/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.3.5/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.3.5/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.3.5/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.3.5/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.3.5/metaseg/modeling/transformer.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 14:15:24.905890 metaseg-0.3.5/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      310 2023-04-09 10:19:56.000000 metaseg-0.3.5/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.3.5/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      518 2023-04-09 10:19:56.000000 metaseg-0.3.5/metaseg/utils/data_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-08 17:15:08.000000 metaseg-0.3.5/metaseg/utils/file_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.3.5/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.3.5/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 14:15:24.909224 metaseg-0.3.5/metaseg/webapp/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:19:56.000000 metaseg-0.3.5/metaseg/webapp/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-09 10:19:56.000000 metaseg-0.3.5/metaseg/webapp/app.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 14:15:24.899224 metaseg-0.3.5/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2125 2023-04-09 14:15:24.000000 metaseg-0.3.5/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      834 2023-04-09 14:15:24.000000 metaseg-0.3.5/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-09 14:15:24.000000 metaseg-0.3.5/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      226 2023-04-09 14:15:24.000000 metaseg-0.3.5/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-09 14:15:24.000000 metaseg-0.3.5/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.3.5/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      139 2023-04-08 09:21:23.000000 metaseg-0.3.5/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-09 14:15:24.909224 metaseg-0.3.5/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.3.5/setup.py
```

### Comparing `metaseg-0.3.4/LICENSE` & `metaseg-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.4/PKG-INFO` & `metaseg-0.3.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.3.4
+Version: 0.3.5
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -28,42 +28,41 @@
 ### Installation
 ```bash
 pip install metaseg
 ```
 
 ### Usage
 ```python
-from metaseg import SegAutoMaskGenerator
+from metaseg import SegAutoMaskPredictor, SegManualMaskPredictor
 
 # If gpu memory is not enough, reduce the points_per_side and points_per_batch.
 
 # For image
 
-autoseg_image = SegAutoMaskGenerator().save_image(
+autoseg_image = SegAutoMaskPredictor().save_image(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=0,
 )
 
 # For video
 
-autoseg_video = SegAutoMaskGenerator().save_video(
+autoseg_video = SegAutoMaskPredictor().save_video(
     source="video.mp4",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=1000,
 )
 
 # For manuel box selection
-from metaseg import SegManualMaskGenerator
 
-seg_manual_mask_generator = SegManualMaskGenerator().save_image(
+seg_manual_mask_generator = SegManualMaskPredictor().save_image(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     x0=100,
     y0=100,
     x1=200,
     y1=200,
 )
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.3.4 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.3.5 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
-metaseg ``` ### Usage ```python from metaseg import SegAutoMaskGenerator # If
-gpu memory is not enough, reduce the points_per_side and points_per_batch. #
-For image autoseg_image = SegAutoMaskGenerator().save_image
-( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b
-points_per_side=16, points_per_batch=64, min_area=0, ) # For video
-autoseg_video = SegAutoMaskGenerator().save_video( source="video.mp4",
-model_type="vit_l", # vit_l, vit_h, vit_b points_per_side=16,
-points_per_batch=64, min_area=1000, ) # For manuel box selection from metaseg
-import SegManualMaskGenerator seg_manual_mask_generator =
-SegManualMaskGenerator().save_image( source="image.jpg", model_type="vit_l", #
-vit_l, vit_h, vit_b x0=100, y0=100, x1=200, y1=200, ) ``` # Extra Features -
-[x] Support for video files - [x] Support for pip installation - [x] Support
-for web application - [x] Support for box to polygon conversion - [x] Support
-for automatic download model weights
+metaseg ``` ### Usage ```python from metaseg import SegAutoMaskPredictor,
+SegManualMaskPredictor # If gpu memory is not enough, reduce the
+points_per_side and points_per_batch. # For image autoseg_image =
+SegAutoMaskPredictor().save_image( source="image.jpg", model_type="vit_l", #
+vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0, ) #
+For video autoseg_video = SegAutoMaskPredictor().save_video
+( source="video.mp4", model_type="vit_l", # vit_l, vit_h, vit_b
+points_per_side=16, points_per_batch=64, min_area=1000, ) # For manuel box
+selection seg_manual_mask_generator = SegManualMaskPredictor().save_image
+( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b x0=100, y0=100,
+x1=200, y1=200, ) ``` # Extra Features - [x] Support for video files - [x]
+Support for pip installation - [x] Support for web application - [x] Support
+for box to polygon conversion - [x] Support for automatic download model
+weights
```

### Comparing `metaseg-0.3.4/README.md` & `metaseg-0.3.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -16,42 +16,41 @@
 ### Installation
 ```bash
 pip install metaseg
 ```
 
 ### Usage
 ```python
-from metaseg import SegAutoMaskGenerator
+from metaseg import SegAutoMaskPredictor, SegManualMaskPredictor
 
 # If gpu memory is not enough, reduce the points_per_side and points_per_batch.
 
 # For image
 
-autoseg_image = SegAutoMaskGenerator().save_image(
+autoseg_image = SegAutoMaskPredictor().save_image(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=0,
 )
 
 # For video
 
-autoseg_video = SegAutoMaskGenerator().save_video(
+autoseg_video = SegAutoMaskPredictor().save_video(
     source="video.mp4",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=1000,
 )
 
 # For manuel box selection
-from metaseg import SegManualMaskGenerator
 
-seg_manual_mask_generator = SegManualMaskGenerator().save_image(
+seg_manual_mask_generator = SegManualMaskPredictor().save_image(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     x0=100,
     y0=100,
     x1=200,
     y1=200,
 )
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
-metaseg ``` ### Usage ```python from metaseg import SegAutoMaskGenerator # If
-gpu memory is not enough, reduce the points_per_side and points_per_batch. #
-For image autoseg_image = SegAutoMaskGenerator().save_image
-( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b
-points_per_side=16, points_per_batch=64, min_area=0, ) # For video
-autoseg_video = SegAutoMaskGenerator().save_video( source="video.mp4",
-model_type="vit_l", # vit_l, vit_h, vit_b points_per_side=16,
-points_per_batch=64, min_area=1000, ) # For manuel box selection from metaseg
-import SegManualMaskGenerator seg_manual_mask_generator =
-SegManualMaskGenerator().save_image( source="image.jpg", model_type="vit_l", #
-vit_l, vit_h, vit_b x0=100, y0=100, x1=200, y1=200, ) ``` # Extra Features -
-[x] Support for video files - [x] Support for pip installation - [x] Support
-for web application - [x] Support for box to polygon conversion - [x] Support
-for automatic download model weights
+metaseg ``` ### Usage ```python from metaseg import SegAutoMaskPredictor,
+SegManualMaskPredictor # If gpu memory is not enough, reduce the
+points_per_side and points_per_batch. # For image autoseg_image =
+SegAutoMaskPredictor().save_image( source="image.jpg", model_type="vit_l", #
+vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0, ) #
+For video autoseg_video = SegAutoMaskPredictor().save_video
+( source="video.mp4", model_type="vit_l", # vit_l, vit_h, vit_b
+points_per_side=16, points_per_batch=64, min_area=1000, ) # For manuel box
+selection seg_manual_mask_generator = SegManualMaskPredictor().save_image
+( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b x0=100, y0=100,
+x1=200, y1=200, ) ``` # Extra Features - [x] Support for video files - [x]
+Support for pip installation - [x] Support for web application - [x] Support
+for box to polygon conversion - [x] Support for automatic download model
+weights
```

### Comparing `metaseg-0.3.4/metaseg/__init__.py` & `metaseg-0.3.5/metaseg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 # LICENSE file in the root directory of this source tree.
 
 from metaseg.generator.automatic_mask_generator import SamAutomaticMaskGenerator
 from metaseg.generator.build_sam import build_sam, build_sam_vit_b, build_sam_vit_h, build_sam_vit_l, sam_model_registry
 from metaseg.generator.predictor import SamPredictor
 from metaseg.mask_predictor import SegAutoMaskPredictor, SegManualMaskPredictor
 
-__version__ = "0.3.4"
+__version__ = "0.3.5"
```

### Comparing `metaseg-0.3.4/metaseg/generator/automatic_mask_generator.py` & `metaseg-0.3.5/metaseg/generator/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.4/metaseg/generator/build_sam.py` & `metaseg-0.3.5/metaseg/generator/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.4/metaseg/generator/predictor.py` & `metaseg-0.3.5/metaseg/generator/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.4/metaseg/mask_predictor.py` & `metaseg-0.3.5/metaseg/mask_predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.4/metaseg/modeling/common.py` & `metaseg-0.3.5/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.4/metaseg/modeling/image_encoder.py` & `metaseg-0.3.5/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.4/metaseg/modeling/mask_decoder.py` & `metaseg-0.3.5/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.4/metaseg/modeling/prompt_encoder.py` & `metaseg-0.3.5/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.4/metaseg/modeling/sam.py` & `metaseg-0.3.5/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.4/metaseg/modeling/transformer.py` & `metaseg-0.3.5/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.4/metaseg/utils/amg.py` & `metaseg-0.3.5/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.4/metaseg/utils/data_utils.py` & `metaseg-0.3.5/metaseg/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.4/metaseg/utils/file_utils.py` & `metaseg-0.3.5/metaseg/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.4/metaseg/utils/onnx.py` & `metaseg-0.3.5/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.4/metaseg/utils/transforms.py` & `metaseg-0.3.5/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.4/metaseg/webapp/app.py` & `metaseg-0.3.5/metaseg/webapp/app.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.4/metaseg.egg-info/PKG-INFO` & `metaseg-0.3.5/metaseg.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.3.4
+Version: 0.3.5
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -28,42 +28,41 @@
 ### Installation
 ```bash
 pip install metaseg
 ```
 
 ### Usage
 ```python
-from metaseg import SegAutoMaskGenerator
+from metaseg import SegAutoMaskPredictor, SegManualMaskPredictor
 
 # If gpu memory is not enough, reduce the points_per_side and points_per_batch.
 
 # For image
 
-autoseg_image = SegAutoMaskGenerator().save_image(
+autoseg_image = SegAutoMaskPredictor().save_image(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=0,
 )
 
 # For video
 
-autoseg_video = SegAutoMaskGenerator().save_video(
+autoseg_video = SegAutoMaskPredictor().save_video(
     source="video.mp4",
     model_type="vit_l", # vit_l, vit_h, vit_b
     points_per_side=16, 
     points_per_batch=64,
     min_area=1000,
 )
 
 # For manuel box selection
-from metaseg import SegManualMaskGenerator
 
-seg_manual_mask_generator = SegManualMaskGenerator().save_image(
+seg_manual_mask_generator = SegManualMaskPredictor().save_image(
     source="image.jpg",
     model_type="vit_l", # vit_l, vit_h, vit_b
     x0=100,
     y0=100,
     x1=200,
     y1=200,
 )
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.3.4 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.3.5 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
-metaseg ``` ### Usage ```python from metaseg import SegAutoMaskGenerator # If
-gpu memory is not enough, reduce the points_per_side and points_per_batch. #
-For image autoseg_image = SegAutoMaskGenerator().save_image
-( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b
-points_per_side=16, points_per_batch=64, min_area=0, ) # For video
-autoseg_video = SegAutoMaskGenerator().save_video( source="video.mp4",
-model_type="vit_l", # vit_l, vit_h, vit_b points_per_side=16,
-points_per_batch=64, min_area=1000, ) # For manuel box selection from metaseg
-import SegManualMaskGenerator seg_manual_mask_generator =
-SegManualMaskGenerator().save_image( source="image.jpg", model_type="vit_l", #
-vit_l, vit_h, vit_b x0=100, y0=100, x1=200, y1=200, ) ``` # Extra Features -
-[x] Support for video files - [x] Support for pip installation - [x] Support
-for web application - [x] Support for box to polygon conversion - [x] Support
-for automatic download model weights
+metaseg ``` ### Usage ```python from metaseg import SegAutoMaskPredictor,
+SegManualMaskPredictor # If gpu memory is not enough, reduce the
+points_per_side and points_per_batch. # For image autoseg_image =
+SegAutoMaskPredictor().save_image( source="image.jpg", model_type="vit_l", #
+vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0, ) #
+For video autoseg_video = SegAutoMaskPredictor().save_video
+( source="video.mp4", model_type="vit_l", # vit_l, vit_h, vit_b
+points_per_side=16, points_per_batch=64, min_area=1000, ) # For manuel box
+selection seg_manual_mask_generator = SegManualMaskPredictor().save_image
+( source="image.jpg", model_type="vit_l", # vit_l, vit_h, vit_b x0=100, y0=100,
+x1=200, y1=200, ) ``` # Extra Features - [x] Support for video files - [x]
+Support for pip installation - [x] Support for web application - [x] Support
+for box to polygon conversion - [x] Support for automatic download model
+weights
```

### Comparing `metaseg-0.3.4/metaseg.egg-info/SOURCES.txt` & `metaseg-0.3.5/metaseg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.4/setup.py` & `metaseg-0.3.5/setup.py`

 * *Files identical despite different names*

