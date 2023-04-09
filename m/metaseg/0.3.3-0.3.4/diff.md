# Comparing `tmp/metaseg-0.3.3.tar.gz` & `tmp/metaseg-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.3.3.tar", last modified: Sun Apr  9 10:31:28 2023, max compression
+gzip compressed data, was "metaseg-0.3.4.tar", last modified: Sun Apr  9 13:58:50 2023, max compression
```

## Comparing `metaseg-0.3.3.tar` & `metaseg-0.3.4.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:31:28.379747 metaseg-0.3.3/
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.3.3/LICENSE
--rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.3.3/MANIFEST.in
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2122 2023-04-09 10:31:28.379747 metaseg-0.3.3/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1848 2023-04-09 10:31:02.000000 metaseg-0.3.3/README.md
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:31:28.369747 metaseg-0.3.3/metaseg/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      562 2023-04-09 10:28:45.000000 metaseg-0.3.3/metaseg/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3686 2023-04-09 10:19:56.000000 metaseg-0.3.3/metaseg/auto_mask_demo.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    15117 2023-04-07 13:09:43.000000 metaseg-0.3.3/metaseg/automatic_mask_generator.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-06 18:52:09.000000 metaseg-0.3.3/metaseg/build_sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2309 2023-04-09 10:27:56.000000 metaseg-0.3.3/metaseg/manuel_mask_demo.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:31:28.373081 metaseg-0.3.3/metaseg/modeling/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.3.3/metaseg/modeling/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.3.3/metaseg/modeling/common.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.3.3/metaseg/modeling/image_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.3.3/metaseg/modeling/mask_decoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.3.3/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.3.3/metaseg/modeling/sam.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.3.3/metaseg/modeling/transformer.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-06 18:52:09.000000 metaseg-0.3.3/metaseg/predictor.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:31:28.376414 metaseg-0.3.3/metaseg/utils/
--rw-r--r--   0 kadir     (1000) kadir     (1001)      310 2023-04-09 10:19:56.000000 metaseg-0.3.3/metaseg/utils/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.3.3/metaseg/utils/amg.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)      518 2023-04-09 10:19:56.000000 metaseg-0.3.3/metaseg/utils/data_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-08 17:15:08.000000 metaseg-0.3.3/metaseg/utils/file_utils.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.3.3/metaseg/utils/onnx.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.3.3/metaseg/utils/transforms.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:31:28.376414 metaseg-0.3.3/metaseg/webapp/
--rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:19:56.000000 metaseg-0.3.3/metaseg/webapp/__init__.py
--rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-09 10:19:56.000000 metaseg-0.3.3/metaseg/webapp/app.py
-drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:31:28.373081 metaseg-0.3.3/metaseg.egg-info/
--rw-r--r--   0 kadir     (1000) kadir     (1001)     2122 2023-04-09 10:31:28.000000 metaseg-0.3.3/metaseg.egg-info/PKG-INFO
--rw-r--r--   0 kadir     (1000) kadir     (1001)      802 2023-04-09 10:31:28.000000 metaseg-0.3.3/metaseg.egg-info/SOURCES.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-09 10:31:28.000000 metaseg-0.3.3/metaseg.egg-info/dependency_links.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      226 2023-04-09 10:31:28.000000 metaseg-0.3.3/metaseg.egg-info/requires.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-09 10:31:28.000000 metaseg-0.3.3/metaseg.egg-info/top_level.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.3.3/pyproject.toml
--rw-r--r--   0 kadir     (1000) kadir     (1001)      139 2023-04-08 09:21:23.000000 metaseg-0.3.3/requirements.txt
--rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-09 10:31:28.379747 metaseg-0.3.3/setup.cfg
--rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.3.3/setup.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:58:50.585914 metaseg-0.3.4/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11357 2023-04-06 18:52:09.000000 metaseg-0.3.4/LICENSE
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       24 2023-04-06 18:52:09.000000 metaseg-0.3.4/MANIFEST.in
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2144 2023-04-09 13:58:50.585914 metaseg-0.3.4/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1870 2023-04-09 13:44:17.000000 metaseg-0.3.4/README.md
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:58:50.565914 metaseg-0.3.4/metaseg/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      556 2023-04-09 13:58:07.000000 metaseg-0.3.4/metaseg/__init__.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:58:50.579248 metaseg-0.3.4/metaseg/generator/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:51:55.000000 metaseg-0.3.4/metaseg/generator/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    15127 2023-04-09 13:58:07.000000 metaseg-0.3.4/metaseg/generator/automatic_mask_generator.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2936 2023-04-06 18:52:09.000000 metaseg-0.3.4/metaseg/generator/build_sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    11570 2023-04-06 18:52:09.000000 metaseg-0.3.4/metaseg/generator/predictor.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5580 2023-04-09 13:58:07.000000 metaseg-0.3.4/metaseg/mask_predictor.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:58:50.582581 metaseg-0.3.4/metaseg/modeling/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      465 2023-04-07 18:10:29.000000 metaseg-0.3.4/metaseg/modeling/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1479 2023-04-07 18:08:09.000000 metaseg-0.3.4/metaseg/modeling/common.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    14341 2023-04-07 18:08:22.000000 metaseg-0.3.4/metaseg/modeling/image_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     6540 2023-04-07 18:08:12.000000 metaseg-0.3.4/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8596 2023-04-07 18:08:19.000000 metaseg-0.3.4/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     7273 2023-04-07 18:08:31.000000 metaseg-0.3.4/metaseg/modeling/sam.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     8332 2023-04-07 18:08:16.000000 metaseg-0.3.4/metaseg/modeling/transformer.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:58:50.585914 metaseg-0.3.4/metaseg/utils/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      310 2023-04-09 10:19:56.000000 metaseg-0.3.4/metaseg/utils/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)    12621 2023-04-06 18:52:09.000000 metaseg-0.3.4/metaseg/utils/amg.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      518 2023-04-09 10:19:56.000000 metaseg-0.3.4/metaseg/utils/data_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1231 2023-04-08 17:15:08.000000 metaseg-0.3.4/metaseg/utils/file_utils.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     5743 2023-04-06 18:52:09.000000 metaseg-0.3.4/metaseg/utils/onnx.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     3874 2023-04-06 18:52:09.000000 metaseg-0.3.4/metaseg/utils/transforms.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:58:50.585914 metaseg-0.3.4/metaseg/webapp/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        0 2023-04-09 10:19:56.000000 metaseg-0.3.4/metaseg/webapp/__init__.py
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     4495 2023-04-09 10:19:56.000000 metaseg-0.3.4/metaseg/webapp/app.py
+drwxr-xr-x   0 kadir     (1000) kadir     (1001)        0 2023-04-09 13:58:50.572581 metaseg-0.3.4/metaseg.egg-info/
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     2144 2023-04-09 13:58:50.000000 metaseg-0.3.4/metaseg.egg-info/PKG-INFO
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      834 2023-04-09 13:58:50.000000 metaseg-0.3.4/metaseg.egg-info/SOURCES.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        1 2023-04-09 13:58:50.000000 metaseg-0.3.4/metaseg.egg-info/dependency_links.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      226 2023-04-09 13:58:50.000000 metaseg-0.3.4/metaseg.egg-info/requires.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)        8 2023-04-09 13:58:50.000000 metaseg-0.3.4/metaseg.egg-info/top_level.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)       80 2023-04-06 18:52:09.000000 metaseg-0.3.4/pyproject.toml
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      139 2023-04-08 09:21:23.000000 metaseg-0.3.4/requirements.txt
+-rw-r--r--   0 kadir     (1000) kadir     (1001)      430 2023-04-09 13:58:50.585914 metaseg-0.3.4/setup.cfg
+-rw-r--r--   0 kadir     (1000) kadir     (1001)     1529 2023-04-06 18:52:10.000000 metaseg-0.3.4/setup.py
```

### Comparing `metaseg-0.3.3/LICENSE` & `metaseg-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.3/PKG-INFO` & `metaseg-0.3.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.3.3
+Version: 0.3.4
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -15,21 +15,20 @@
      MetaSeg: Packaged version of the Segment Anything repository
 </h2>
 <div>
     <img width="1000" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.2.2/metaseg_demo.gif">
 </div>
     <a href="https://pepy.tech/project/metaseg"><img src="https://pepy.tech/badge/metaseg" alt="downloads"></a>
     <a href="https://badge.fury.io/py/metaseg"><img src="https://badge.fury.io/py/metaseg.svg" alt="pypi version"></a>
-    <a href="https://huggingface.co/spaces/ArtGAN/metaseg-webui"><img src="https://img.shields.io/badge/%20HuggingFace%20-Demo-blue.svg" alt="HuggingFace Spaces"></a>
+    <a href="https://huggingface.co/spaces/ArtGAN/metaseg-webui"><img src="https://huggingface.co/datasets/huggingface/badges/raw/main/open-in-hf-spaces-sm.svg" alt="HuggingFace Spaces"></a>
 
 </div>
 
 This repo is a packaged version of the [segment-anything](https://github.com/facebookresearch/segment-anything) model.
 
-
 ### Installation
 ```bash
 pip install metaseg
 ```
 
 ### Usage
 ```python
@@ -65,15 +64,14 @@
     model_type="vit_l", # vit_l, vit_h, vit_b
     x0=100,
     y0=100,
     x1=200,
     y1=200,
 )
 ```
-
 # Extra Features
 
 - [x] Support for video files
 - [x] Support for pip installation
 - [x] Support for web application
 - [x] Support for box to polygon conversion
 - [x] Support for automatic download model weights
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.3.3 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.3.4 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
```

### Comparing `metaseg-0.3.3/README.md` & `metaseg-0.3.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,20 @@
      MetaSeg: Packaged version of the Segment Anything repository
 </h2>
 <div>
     <img width="1000" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.2.2/metaseg_demo.gif">
 </div>
     <a href="https://pepy.tech/project/metaseg"><img src="https://pepy.tech/badge/metaseg" alt="downloads"></a>
     <a href="https://badge.fury.io/py/metaseg"><img src="https://badge.fury.io/py/metaseg.svg" alt="pypi version"></a>
-    <a href="https://huggingface.co/spaces/ArtGAN/metaseg-webui"><img src="https://img.shields.io/badge/%20HuggingFace%20-Demo-blue.svg" alt="HuggingFace Spaces"></a>
+    <a href="https://huggingface.co/spaces/ArtGAN/metaseg-webui"><img src="https://huggingface.co/datasets/huggingface/badges/raw/main/open-in-hf-spaces-sm.svg" alt="HuggingFace Spaces"></a>
 
 </div>
 
 This repo is a packaged version of the [segment-anything](https://github.com/facebookresearch/segment-anything) model.
 
-
 ### Installation
 ```bash
 pip install metaseg
 ```
 
 ### Usage
 ```python
@@ -53,15 +52,14 @@
     model_type="vit_l", # vit_l, vit_h, vit_b
     x0=100,
     y0=100,
     x1=200,
     y1=200,
 )
 ```
-
 # Extra Features
 
 - [x] Support for video files
 - [x] Support for pip installation
 - [x] Support for web application
 - [x] Support for box to polygon conversion
 - [x] Support for automatic download model weights
```

### Comparing `metaseg-0.3.3/metaseg/automatic_mask_generator.py` & `metaseg-0.3.4/metaseg/generator/automatic_mask_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 from typing import Any, Dict, List, Optional, Tuple
 
 import numpy as np
 import torch
 from torchvision.ops.boxes import batched_nms, box_area  # type: ignore
 
+from metaseg.generator.predictor import SamPredictor
 from metaseg.modeling import Sam
-from metaseg.predictor import SamPredictor
 from metaseg.utils.amg import (
     MaskData,
     area_from_rle,
     batch_iterator,
     batched_mask_to_box,
     box_xyxy_to_xywh,
     build_all_layer_point_grids,
```

### Comparing `metaseg-0.3.3/metaseg/build_sam.py` & `metaseg-0.3.4/metaseg/generator/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.3/metaseg/modeling/common.py` & `metaseg-0.3.4/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.3/metaseg/modeling/image_encoder.py` & `metaseg-0.3.4/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.3/metaseg/modeling/mask_decoder.py` & `metaseg-0.3.4/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.3/metaseg/modeling/prompt_encoder.py` & `metaseg-0.3.4/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.3/metaseg/modeling/sam.py` & `metaseg-0.3.4/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.3/metaseg/modeling/transformer.py` & `metaseg-0.3.4/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.3/metaseg/predictor.py` & `metaseg-0.3.4/metaseg/generator/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.3/metaseg/utils/amg.py` & `metaseg-0.3.4/metaseg/utils/amg.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.3/metaseg/utils/data_utils.py` & `metaseg-0.3.4/metaseg/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.3/metaseg/utils/file_utils.py` & `metaseg-0.3.4/metaseg/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.3/metaseg/utils/onnx.py` & `metaseg-0.3.4/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.3/metaseg/utils/transforms.py` & `metaseg-0.3.4/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.3/metaseg/webapp/app.py` & `metaseg-0.3.4/metaseg/webapp/app.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.3.3/metaseg.egg-info/PKG-INFO` & `metaseg-0.3.4/metaseg.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.3.3
+Version: 0.3.4
 Home-page: https://github.com/kadirnar/segment-anything-pip
 Author: kadirnar
 License: Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
@@ -15,21 +15,20 @@
      MetaSeg: Packaged version of the Segment Anything repository
 </h2>
 <div>
     <img width="1000" alt="teaser" src="https://github.com/kadirnar/segment-anything-pip/releases/download/v0.2.2/metaseg_demo.gif">
 </div>
     <a href="https://pepy.tech/project/metaseg"><img src="https://pepy.tech/badge/metaseg" alt="downloads"></a>
     <a href="https://badge.fury.io/py/metaseg"><img src="https://badge.fury.io/py/metaseg.svg" alt="pypi version"></a>
-    <a href="https://huggingface.co/spaces/ArtGAN/metaseg-webui"><img src="https://img.shields.io/badge/%20HuggingFace%20-Demo-blue.svg" alt="HuggingFace Spaces"></a>
+    <a href="https://huggingface.co/spaces/ArtGAN/metaseg-webui"><img src="https://huggingface.co/datasets/huggingface/badges/raw/main/open-in-hf-spaces-sm.svg" alt="HuggingFace Spaces"></a>
 
 </div>
 
 This repo is a packaged version of the [segment-anything](https://github.com/facebookresearch/segment-anything) model.
 
-
 ### Installation
 ```bash
 pip install metaseg
 ```
 
 ### Usage
 ```python
@@ -65,15 +64,14 @@
     model_type="vit_l", # vit_l, vit_h, vit_b
     x0=100,
     y0=100,
     x1=200,
     y1=200,
 )
 ```
-
 # Extra Features
 
 - [x] Support for video files
 - [x] Support for pip installation
 - [x] Support for web application
 - [x] Support for box to polygon conversion
 - [x] Support for automatic download model weights
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.3.3 Home-page: https://
+Metadata-Version: 2.1 Name: metaseg Version: 0.3.4 Home-page: https://
 github.com/kadirnar/segment-anything-pip Author: kadirnar License: Apache-2.0
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 all Provides-Extra: dev License-File: LICENSE
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                 [downloads] [pypi_version] [HuggingFace_Spaces]
 This repo is a packaged version of the [segment-anything](https://github.com/
```

### Comparing `metaseg-0.3.3/metaseg.egg-info/SOURCES.txt` & `metaseg-0.3.4/metaseg.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 metaseg/__init__.py
-metaseg/auto_mask_demo.py
-metaseg/automatic_mask_generator.py
-metaseg/build_sam.py
-metaseg/manuel_mask_demo.py
-metaseg/predictor.py
+metaseg/mask_predictor.py
 metaseg.egg-info/PKG-INFO
 metaseg.egg-info/SOURCES.txt
 metaseg.egg-info/dependency_links.txt
 metaseg.egg-info/requires.txt
 metaseg.egg-info/top_level.txt
+metaseg/generator/__init__.py
+metaseg/generator/automatic_mask_generator.py
+metaseg/generator/build_sam.py
+metaseg/generator/predictor.py
 metaseg/modeling/__init__.py
 metaseg/modeling/common.py
 metaseg/modeling/image_encoder.py
 metaseg/modeling/mask_decoder.py
 metaseg/modeling/prompt_encoder.py
 metaseg/modeling/sam.py
 metaseg/modeling/transformer.py
```

### Comparing `metaseg-0.3.3/setup.py` & `metaseg-0.3.4/setup.py`

 * *Files identical despite different names*

