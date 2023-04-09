# Comparing `tmp/raydl-0.0.6.tar.gz` & `tmp/raydl-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raydl-0.0.6.tar", last modified: Sat Apr  1 02:59:04 2023, max compression
+gzip compressed data, was "raydl-0.0.7.tar", last modified: Sun Apr  9 16:03:55 2023, max compression
```

## Comparing `raydl-0.0.6.tar` & `raydl-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-01 02:59:04.592290 raydl-0.0.6/
--rw-r--r--   0 rayw       (501) staff       (20)     1069 2023-01-24 10:36:02.000000 raydl-0.0.6/LICENSE
--rw-r--r--   0 rayw       (501) staff       (20)     1958 2023-04-01 02:59:04.592129 raydl-0.0.6/PKG-INFO
--rw-r--r--   0 rayw       (501) staff       (20)      227 2023-01-24 12:20:22.000000 raydl-0.0.6/README.md
--rw-r--r--   0 rayw       (501) staff       (20)     1736 2023-04-01 02:58:39.000000 raydl-0.0.6/pyproject.toml
--rw-r--r--   0 rayw       (501) staff       (20)       38 2023-04-01 02:59:04.592343 raydl-0.0.6/setup.cfg
--rw-r--r--   0 rayw       (501) staff       (20)       38 2023-01-24 12:50:45.000000 raydl-0.0.6/setup.py
-drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-01 02:59:04.587826 raydl-0.0.6/src/
-drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-01 02:59:04.590984 raydl-0.0.6/src/raydl/
--rw-r--r--   0 rayw       (501) staff       (20)      441 2023-04-01 02:58:39.000000 raydl-0.0.6/src/raydl/__init__.py
--rw-r--r--   0 rayw       (501) staff       (20)     3242 2023-03-29 17:49:47.000000 raydl-0.0.6/src/raydl/__main__.py
--rw-r--r--   0 rayw       (501) staff       (20)     1466 2023-01-31 03:35:05.000000 raydl-0.0.6/src/raydl/collect_env.py
--rw-r--r--   0 rayw       (501) staff       (20)    10843 2023-03-29 17:39:53.000000 raydl-0.0.6/src/raydl/image.py
--rw-r--r--   0 rayw       (501) staff       (20)     4339 2023-04-01 02:56:34.000000 raydl-0.0.6/src/raydl/initialization.py
--rw-r--r--   0 rayw       (501) staff       (20)    13850 2023-04-01 02:57:11.000000 raydl-0.0.6/src/raydl/sfdb.py
--rw-r--r--   0 rayw       (501) staff       (20)     5021 2023-03-29 15:02:33.000000 raydl-0.0.6/src/raydl/tensor.py
--rw-r--r--   0 rayw       (501) staff       (20)     2229 2023-02-25 16:45:04.000000 raydl-0.0.6/src/raydl/time.py
--rw-r--r--   0 rayw       (501) staff       (20)      705 2023-03-18 18:27:59.000000 raydl-0.0.6/src/raydl/utils.py
-drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-01 02:59:04.591857 raydl-0.0.6/src/raydl.egg-info/
--rw-r--r--   0 rayw       (501) staff       (20)     1958 2023-04-01 02:59:04.000000 raydl-0.0.6/src/raydl.egg-info/PKG-INFO
--rw-r--r--   0 rayw       (501) staff       (20)      396 2023-04-01 02:59:04.000000 raydl-0.0.6/src/raydl.egg-info/SOURCES.txt
--rw-r--r--   0 rayw       (501) staff       (20)        1 2023-04-01 02:59:04.000000 raydl-0.0.6/src/raydl.egg-info/dependency_links.txt
--rw-r--r--   0 rayw       (501) staff       (20)       37 2023-04-01 02:59:04.000000 raydl-0.0.6/src/raydl.egg-info/requires.txt
--rw-r--r--   0 rayw       (501) staff       (20)        6 2023-04-01 02:59:04.000000 raydl-0.0.6/src/raydl.egg-info/top_level.txt
+drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-09 16:03:55.585296 raydl-0.0.7/
+-rw-r--r--   0 rayw       (501) staff       (20)     1069 2023-01-24 10:36:02.000000 raydl-0.0.7/LICENSE
+-rw-r--r--   0 rayw       (501) staff       (20)     1958 2023-04-09 16:03:55.585139 raydl-0.0.7/PKG-INFO
+-rw-r--r--   0 rayw       (501) staff       (20)      227 2023-01-24 12:20:22.000000 raydl-0.0.7/README.md
+-rw-r--r--   0 rayw       (501) staff       (20)     1736 2023-04-09 16:03:34.000000 raydl-0.0.7/pyproject.toml
+-rw-r--r--   0 rayw       (501) staff       (20)       38 2023-04-09 16:03:55.585345 raydl-0.0.7/setup.cfg
+-rw-r--r--   0 rayw       (501) staff       (20)       38 2023-01-24 12:50:45.000000 raydl-0.0.7/setup.py
+drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-09 16:03:55.580953 raydl-0.0.7/src/
+drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-09 16:03:55.584117 raydl-0.0.7/src/raydl/
+-rw-r--r--   0 rayw       (501) staff       (20)      441 2023-04-09 16:03:34.000000 raydl-0.0.7/src/raydl/__init__.py
+-rw-r--r--   0 rayw       (501) staff       (20)     3242 2023-03-29 17:49:47.000000 raydl-0.0.7/src/raydl/__main__.py
+-rw-r--r--   0 rayw       (501) staff       (20)     1466 2023-01-31 03:35:05.000000 raydl-0.0.7/src/raydl/collect_env.py
+-rw-r--r--   0 rayw       (501) staff       (20)    12896 2023-04-09 16:01:01.000000 raydl-0.0.7/src/raydl/image.py
+-rw-r--r--   0 rayw       (501) staff       (20)     4339 2023-04-01 02:56:34.000000 raydl-0.0.7/src/raydl/initialization.py
+-rw-r--r--   0 rayw       (501) staff       (20)    13850 2023-04-01 02:57:11.000000 raydl-0.0.7/src/raydl/sfdb.py
+-rw-r--r--   0 rayw       (501) staff       (20)     5021 2023-03-29 15:02:33.000000 raydl-0.0.7/src/raydl/tensor.py
+-rw-r--r--   0 rayw       (501) staff       (20)     2229 2023-02-25 16:45:04.000000 raydl-0.0.7/src/raydl/time.py
+-rw-r--r--   0 rayw       (501) staff       (20)      705 2023-03-18 18:27:59.000000 raydl-0.0.7/src/raydl/utils.py
+drwxr-xr-x   0 rayw       (501) staff       (20)        0 2023-04-09 16:03:55.584923 raydl-0.0.7/src/raydl.egg-info/
+-rw-r--r--   0 rayw       (501) staff       (20)     1958 2023-04-09 16:03:55.000000 raydl-0.0.7/src/raydl.egg-info/PKG-INFO
+-rw-r--r--   0 rayw       (501) staff       (20)      396 2023-04-09 16:03:55.000000 raydl-0.0.7/src/raydl.egg-info/SOURCES.txt
+-rw-r--r--   0 rayw       (501) staff       (20)        1 2023-04-09 16:03:55.000000 raydl-0.0.7/src/raydl.egg-info/dependency_links.txt
+-rw-r--r--   0 rayw       (501) staff       (20)       37 2023-04-09 16:03:55.000000 raydl-0.0.7/src/raydl.egg-info/requires.txt
+-rw-r--r--   0 rayw       (501) staff       (20)        6 2023-04-09 16:03:55.000000 raydl-0.0.7/src/raydl.egg-info/top_level.txt
```

### Comparing `raydl-0.0.6/LICENSE` & `raydl-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `raydl-0.0.6/PKG-INFO` & `raydl-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raydl
-Version: 0.0.6
+Version: 0.0.7
 Summary: The library of utilities to help you deal with the deep learning in PyTorch.
 Author: Ray Wang
 License: MIT License
         
         Copyright (c) [2023] [Ray Wang]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `raydl-0.0.6/pyproject.toml` & `raydl-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "raydl"
-version = "0.0.6"
+version = "0.0.7"
 description = "The library of utilities to help you deal with the deep learning in PyTorch."
 readme = "README.md"
 authors = [{ name = "Ray Wang" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
@@ -51,15 +51,15 @@
 ignore = ["UP007", "C408", "B905"]
 line-length=119
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.bumpver]
-current_version = "0.0.6"
+current_version = "0.0.7"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `raydl-0.0.6/src/raydl/__main__.py` & `raydl-0.0.7/src/raydl/__main__.py`

 * *Files identical despite different names*

### Comparing `raydl-0.0.6/src/raydl/collect_env.py` & `raydl-0.0.7/src/raydl/collect_env.py`

 * *Files identical despite different names*

### Comparing `raydl-0.0.6/src/raydl/image.py` & `raydl-0.0.7/src/raydl/image.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import math
 import platform
 import warnings
 from pathlib import Path
 from typing import Iterable, Optional, Sequence, Union, cast
 
+import numpy as np
 import torch
 import torch.nn.functional as F
 import torchvision.transforms.functional
 from PIL import Image, ImageDraw, ImageFont
 from torchvision.utils import make_grid
 
 DEFAULT_FONT = "DejaVuSans.ttf" if platform.system() == "Linux" else "Arial.ttf"
@@ -264,7 +265,50 @@
     if isinstance(save_path, (str, Path)):
         save_path = Path(save_path)
         save_path = [save_path.with_name(f"{save_path.stem}_{i}{save_path.suffix}") for i in range(len(images))]
     assert len(save_path) >= len(images)
 
     for i in range(len(pil_images)):
         pil_images[i].save(save_path[i])
+
+
+def create_heatmap(
+    images: torch.Tensor,
+    range_min: Union[float, torch.Tensor, None] = None,
+    range_max: Union[float, torch.Tensor, None] = None,
+    scale_each: bool = False,
+    color_map: str = "jet",
+) -> torch.Tensor:
+    """
+    create heatmap from BxHxW tensor.
+    :param images: Tensor[BxHxW]
+    :param range_min: max value used to normalize the image. By default, min and max are computed from the tensor.
+    :param range_max: min value used to normalize the image. By default, min and max are computed from the tensor.
+    :param scale_each: If True, scale each image in the batch of images separately rather
+     than the (min, max) over all images. Default: False.
+    :param color_map: The colormap to apply, colormap from
+     https://docs.opencv.org/3.4/d3/d50/group__imgproc__colormap.html#ga9a805d8262bcbe273f16be9ea2055a65
+    :param return_tensor: if True, return Tensor[Bx3xHxW], otherwise return tuple of numpy.array(0-255)
+    :return:
+    """
+    device = images.device
+    assert images.dim() == 3
+    try:
+        import cv2
+
+        color_map = getattr(cv2, f"COLORMAP_{color_map.upper()}")
+    except AttributeError as e:
+        raise ValueError(f"invalid color_map {color_map}") from e
+
+    with torch.no_grad():
+        images = images.detach().clone().to(dtype=torch.float32, device=torch.device("cpu"))
+        if range_min is None:
+            range_min = images.amin(dim=[-1, -2], keepdim=True) if scale_each else images.amin()
+        if range_max is None:
+            range_max = images.amax(dim=[-1, -2], keepdim=True) if scale_each else images.amax()
+        heatmaps = []
+        for m in images.add_(-range_min).div_(range_max - range_min + 1e-5).clip_(0.0, 1.0):
+            heatmaps.append(cv2.applyColorMap(np.uint8(m.numpy() * 255), color_map))
+        heatmaps = torch.from_numpy(np.stack(heatmaps)).permute(0, 3, 1, 2)
+        # BGR -> RGB & [0, 255] -> [0, 1]
+        heatmaps = heatmaps[:, [2, 1, 0], :, :].contiguous().float().to(device) / 255
+        return heatmaps
```

### Comparing `raydl-0.0.6/src/raydl/initialization.py` & `raydl-0.0.7/src/raydl/initialization.py`

 * *Files identical despite different names*

### Comparing `raydl-0.0.6/src/raydl/sfdb.py` & `raydl-0.0.7/src/raydl/sfdb.py`

 * *Files identical despite different names*

### Comparing `raydl-0.0.6/src/raydl/tensor.py` & `raydl-0.0.7/src/raydl/tensor.py`

 * *Files identical despite different names*

### Comparing `raydl-0.0.6/src/raydl/time.py` & `raydl-0.0.7/src/raydl/time.py`

 * *Files identical despite different names*

### Comparing `raydl-0.0.6/src/raydl/utils.py` & `raydl-0.0.7/src/raydl/utils.py`

 * *Files identical despite different names*

### Comparing `raydl-0.0.6/src/raydl.egg-info/PKG-INFO` & `raydl-0.0.7/src/raydl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raydl
-Version: 0.0.6
+Version: 0.0.7
 Summary: The library of utilities to help you deal with the deep learning in PyTorch.
 Author: Ray Wang
 License: MIT License
         
         Copyright (c) [2023] [Ray Wang]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

