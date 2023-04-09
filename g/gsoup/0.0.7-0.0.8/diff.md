# Comparing `tmp/gsoup-0.0.7.tar.gz` & `tmp/gsoup-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsoup-0.0.7.tar", last modified: Mon Feb 20 06:54:06 2023, max compression
+gzip compressed data, was "gsoup-0.0.8.tar", last modified: Sun Apr  9 14:09:34 2023, max compression
```

## Comparing `gsoup-0.0.7.tar` & `gsoup-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 yotam     (1003) yotam     (1003)        0 2023-02-20 06:54:06.778624 gsoup-0.0.7/
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     1088 2022-11-18 02:40:35.000000 gsoup-0.0.7/LICENSE
--rw-rw-r--   0 yotam     (1003) yotam     (1003)       45 2022-12-05 04:54:57.000000 gsoup-0.0.7/MANIFEST.in
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     3154 2023-02-20 06:54:06.778624 gsoup-0.0.7/PKG-INFO
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     1392 2023-02-15 10:00:37.000000 gsoup-0.0.7/README.md
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     1210 2023-02-20 06:52:31.000000 gsoup-0.0.7/pyproject.toml
--rw-rw-r--   0 yotam     (1003) yotam     (1003)       38 2023-02-20 06:54:06.778624 gsoup-0.0.7/setup.cfg
-drwxrwxr-x   0 yotam     (1003) yotam     (1003)        0 2023-02-20 06:54:06.774624 gsoup-0.0.7/src/
-drwxrwxr-x   0 yotam     (1003) yotam     (1003)        0 2023-02-20 06:54:06.778624 gsoup-0.0.7/src/gsoup/
--rwx------   0 yotam     (1003) yotam     (1003)   343980 2012-02-17 04:17:40.000000 gsoup-0.0.7/src/gsoup/FreeMono.ttf
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     2104 2023-02-20 06:52:31.000000 gsoup-0.0.7/src/gsoup/__init__.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)    22849 2023-02-15 10:16:38.000000 gsoup-0.0.7/src/gsoup/core.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     7842 2022-12-14 08:18:43.000000 gsoup-0.0.7/src/gsoup/geometry_advanced.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)    14890 2023-02-15 10:00:37.000000 gsoup-0.0.7/src/gsoup/geometry_basic.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)    16801 2023-02-14 06:40:54.000000 gsoup-0.0.7/src/gsoup/gsoup_io.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)    17186 2023-02-20 06:51:15.000000 gsoup-0.0.7/src/gsoup/image.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)    17647 2023-02-14 06:40:54.000000 gsoup-0.0.7/src/gsoup/procam.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     8162 2023-01-27 03:19:31.000000 gsoup-0.0.7/src/gsoup/sphere_trace.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     9104 2023-02-17 14:37:19.000000 gsoup-0.0.7/src/gsoup/structures.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)    10012 2023-02-17 13:20:00.000000 gsoup-0.0.7/src/gsoup/video.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     7393 2023-02-17 14:37:19.000000 gsoup-0.0.7/src/gsoup/viewer.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     6260 2023-02-20 06:51:15.000000 gsoup-0.0.7/src/gsoup/viewer_drivers.py
-drwxrwxr-x   0 yotam     (1003) yotam     (1003)        0 2023-02-20 06:54:06.778624 gsoup-0.0.7/src/gsoup.egg-info/
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     3154 2023-02-20 06:54:06.000000 gsoup-0.0.7/src/gsoup.egg-info/PKG-INFO
--rw-rw-r--   0 yotam     (1003) yotam     (1003)      528 2023-02-20 06:54:06.000000 gsoup-0.0.7/src/gsoup.egg-info/SOURCES.txt
--rw-rw-r--   0 yotam     (1003) yotam     (1003)        1 2023-02-20 06:54:06.000000 gsoup-0.0.7/src/gsoup.egg-info/dependency_links.txt
--rw-rw-r--   0 yotam     (1003) yotam     (1003)      110 2023-02-20 06:54:06.000000 gsoup-0.0.7/src/gsoup.egg-info/requires.txt
--rw-rw-r--   0 yotam     (1003) yotam     (1003)        6 2023-02-20 06:54:06.000000 gsoup-0.0.7/src/gsoup.egg-info/top_level.txt
-drwxrwxr-x   0 yotam     (1003) yotam     (1003)        0 2023-02-20 06:54:06.778624 gsoup-0.0.7/tests/
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     8881 2023-02-20 06:51:15.000000 gsoup-0.0.7/tests/test_basic.py
+drwxrwxr-x   0 yotam     (1003) yotam     (1003)        0 2023-04-09 14:09:34.404677 gsoup-0.0.8/
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)     1088 2022-11-18 02:40:35.000000 gsoup-0.0.8/LICENSE
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)       45 2022-12-05 04:54:57.000000 gsoup-0.0.8/MANIFEST.in
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)     3154 2023-04-09 14:09:34.400678 gsoup-0.0.8/PKG-INFO
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)     1392 2023-02-15 10:00:37.000000 gsoup-0.0.8/README.md
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)     1210 2023-04-09 14:09:07.000000 gsoup-0.0.8/pyproject.toml
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)       38 2023-04-09 14:09:34.404677 gsoup-0.0.8/setup.cfg
+drwxrwxr-x   0 yotam     (1003) yotam     (1003)        0 2023-04-09 14:09:34.396678 gsoup-0.0.8/src/
+drwxrwxr-x   0 yotam     (1003) yotam     (1003)        0 2023-04-09 14:09:34.400678 gsoup-0.0.8/src/gsoup/
+-rwx------   0 yotam     (1003) yotam     (1003)   343980 2012-02-17 04:17:40.000000 gsoup-0.0.8/src/gsoup/FreeMono.ttf
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)     2370 2023-04-09 14:09:07.000000 gsoup-0.0.8/src/gsoup/__init__.py
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)    26648 2023-04-09 12:29:27.000000 gsoup-0.0.8/src/gsoup/core.py
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)     7842 2022-12-14 08:18:43.000000 gsoup-0.0.8/src/gsoup/geometry_advanced.py
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)    14710 2023-03-11 12:33:08.000000 gsoup-0.0.8/src/gsoup/geometry_basic.py
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)    16714 2023-03-11 13:26:05.000000 gsoup-0.0.8/src/gsoup/gsoup_io.py
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)    22251 2023-03-21 09:44:07.000000 gsoup-0.0.8/src/gsoup/image.py
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)    18798 2023-03-11 12:33:36.000000 gsoup-0.0.8/src/gsoup/procam.py
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)     8189 2023-02-28 10:40:05.000000 gsoup-0.0.8/src/gsoup/sphere_trace.py
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)     9104 2023-02-17 14:37:19.000000 gsoup-0.0.8/src/gsoup/structures.py
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)    10012 2023-02-17 13:20:00.000000 gsoup-0.0.8/src/gsoup/video.py
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)     7409 2023-03-10 03:21:59.000000 gsoup-0.0.8/src/gsoup/viewer.py
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)     6542 2023-03-10 03:21:59.000000 gsoup-0.0.8/src/gsoup/viewer_drivers.py
+drwxrwxr-x   0 yotam     (1003) yotam     (1003)        0 2023-04-09 14:09:34.400678 gsoup-0.0.8/src/gsoup.egg-info/
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)     3154 2023-04-09 14:09:34.000000 gsoup-0.0.8/src/gsoup.egg-info/PKG-INFO
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)      528 2023-04-09 14:09:34.000000 gsoup-0.0.8/src/gsoup.egg-info/SOURCES.txt
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)        1 2023-04-09 14:09:34.000000 gsoup-0.0.8/src/gsoup.egg-info/dependency_links.txt
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)      110 2023-04-09 14:09:34.000000 gsoup-0.0.8/src/gsoup.egg-info/requires.txt
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)        6 2023-04-09 14:09:34.000000 gsoup-0.0.8/src/gsoup.egg-info/top_level.txt
+drwxrwxr-x   0 yotam     (1003) yotam     (1003)        0 2023-04-09 14:09:34.400678 gsoup-0.0.8/tests/
+-rw-rw-r--   0 yotam     (1003) yotam     (1003)    14734 2023-04-09 08:06:28.000000 gsoup-0.0.8/tests/test_basic.py
```

### Comparing `gsoup-0.0.7/LICENSE` & `gsoup-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gsoup-0.0.7/PKG-INFO` & `gsoup-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsoup
-Version: 0.0.7
+Version: 0.0.8
 Summary: A geoemtry & graphics library with focus on clarity rather than performance.
 Author-email: Yotam Erel <erelyotam@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Yotam Erel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gsoup-0.0.7/README.md` & `gsoup-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gsoup-0.0.7/pyproject.toml` & `gsoup-0.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gsoup"
-version = "0.0.7"
+version = "0.0.8"
 description = "A geoemtry & graphics library with focus on clarity rather than performance."
 readme = "README.md"
 authors = [{ name = "Yotam Erel", email = "erelyotam@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -29,15 +29,15 @@
 build = ["build", "twine"]
 dev = ["bumpver", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/yoterel/gsoup"
 
 [tool.bumpver]
-current_version = "0.0.7"
+current_version = "0.0.8"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `gsoup-0.0.7/src/gsoup/FreeMono.ttf` & `gsoup-0.0.8/src/gsoup/FreeMono.ttf`

 * *Files identical despite different names*

### Comparing `gsoup-0.0.7/src/gsoup/__init__.py` & `gsoup-0.0.8/src/gsoup/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,35 @@
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 
 from .core import (
+    is_np,
     broadcast_batch,
     to_hom,
     homogenize,
+    look_at_torch,
+    look_at_np,
     compose_rt,
     to_44,
     to_34,
-    look_at_np,
     to_np,
     to_numpy,
     to_torch,
     to_8b,
     to_float,
     rotx,
     roty,
     rotz,
     map_range,
     create_random_cameras_on_unit_sphere,
+    random_vectors_on_sphere,
     opengl_c2w_to_opencv_c2w,
     opencv_c2w_to_opengl_c2w,
+    opencv_intrinsics_from_opengl_project,
     opengl_project_from_opencv_intrinsics,
+    perspective_projection,
     vec2skew,
     batch_vec2skew,
     rotvec2mat,
     batch_rotvec2mat,
     random_qvec,
     qvec2mat,
     batch_qvec2mat,
@@ -70,26 +75,32 @@
 )
 
 from .image import (
     alpha_compose,
     draw_text_on_image,
     draw_gizmo_on_image,
     merge_figures_with_line,
+    generate_checkerboard,
     generate_voronoi_diagram,
     generate_gray_gradient,
     generate_dot_pattern,
     generate_stripe_pattern,
     generate_concentric_circles,
     generate_lollipop_pattern,
     interpolate_single_channel,
     interpolate_multi_channel,
     image_grid,
     resize_images_naive,
+    adjust_contrast_brightness,
     change_brightness,
-    change_contrast
+    linear_to_srgb,
+    srgb_to_linear,
+    pad_image_to_res,
+    mask_regions,
+    crop_center
 )
 
 from .video import (
     get_video_info,
     get_frame_timestamps,
     load_video,
     save_video,
```

### Comparing `gsoup-0.0.7/src/gsoup/core.py` & `gsoup-0.0.8/src/gsoup/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,58 @@
 import torch
 import numpy as np
 from PIL import Image
 
+def is_np(x):
+    """
+    checks if x is a numpy array or torch tensor (will raise an error if x is neither)
+    :param x: object to check
+    :return: True if x is a numpy array, False if x is a torch tensor
+    """
+    if type(x) == np.ndarray:
+        return True
+    elif type(x) == torch.Tensor:
+        return False
+    else:
+        raise ValueError("input must be torch.Tensor or np.ndarray")
+
 def to_hom(x):
     """
     converts a vector to homogeneous coordinates
     :param x: nxc numpy array
     :return: nxc+1 numpy array
     """
-    if type(x) == torch.Tensor:
-        if x.ndim == 1:
-            return torch.cat((x, torch.ones(1, device=x.device)))
-        else:
-            return torch.cat((x, torch.ones(x.shape[0], 1, device=x.device)), dim=-1)
-    elif type(x) == np.ndarray:
+    if is_np(x):
         if x.ndim == 1:
             return np.concatenate((x, np.array([1], dtype=x.dtype)))
         else:
             return np.concatenate((x, np.ones((x.shape[0], 1), dtype=x.dtype)), axis=-1)
     else:
-        raise ValueError("x must be torch.Tensor or np.ndarray")
+        if x.ndim == 1:
+            return torch.cat((x, torch.ones(1, device=x.device)))
+        else:
+            return torch.cat((x, torch.ones(x.shape[0], 1, device=x.device)), dim=-1)
 
 def homogenize(x, keepdim=False):
     """
     normalizes a homogeneous vector by dividing by the last coordinate
     :param x: nx3 numpy array
     :return: nx4 numpy array
     """
     x = (x / x[..., -1:])
     if not keepdim:
         x = x[..., :-1]
     return x
 
 def normalize(x, eps=1e-7):
-    if type(x) == torch.Tensor:
-        return x / (torch.norm(x, dim=-1, keepdim=True) + eps)
-    elif type(x) == np.ndarray:
+
+    if is_np(x):
         return x / (np.linalg.norm(x, axis=-1, keepdims=True) + eps)
+    else:
+        return x / (torch.norm(x, dim=-1, keepdim=True) + eps)
 
 
 def broadcast_batch(*args):
     """
     broadcast a list of arrays to the same shape on the batch dimension
     assumes first dimension is batch unless ndim = 1 for all inputs (but then does not broadcast)
     :param args: list of arrays
@@ -85,23 +97,21 @@
     :param mat: dimsx3x4 numpy array (dims can be any number of dims including 0)
     :return: dimsx4x4 numpy array
     """
     if mat.shape[-2:] == (4, 4):
         return mat
     if mat.shape[-2:] != (3, 4):
         raise ValueError("mat must be 3x4")
-    if type(mat) == torch.Tensor:
-        to_cat = torch.zeros((*mat.shape[:-2], 1, 4), dtype=mat.dtype, device=mat.device)
-        to_cat[..., -1] = 1
-        new_mat = torch.cat((mat, to_cat), dim=-2)
-    elif type(mat) == np.ndarray:
+    if is_np(mat):
         to_cat = np.broadcast_to(np.array([0, 0, 0, 1]), (*mat.shape[:-2], 1, 4))
         new_mat = np.concatenate((mat, to_cat), axis=-2)
     else:
-        raise ValueError("mat must be torch.Tensor or np.ndarray")
+        to_cat = torch.zeros((*mat.shape[:-2], 1, 4), dtype=mat.dtype, device=mat.device)
+        to_cat[..., -1] = 1
+        new_mat = torch.cat((mat, to_cat), dim=-2)
     return new_mat
 
 def to_34(mat: np.array):
     """
     converts a 4x4 to a 3x4 matrix by removeing the last row
     :param mat: 4x4 numpy array
     :return: 3x4 numpy array
@@ -111,67 +121,64 @@
             raise ValueError("mat must be 4x4")
         return mat[:, :-1, :]
     else:
         if mat.shape != (4, 4):
             raise ValueError("mat must be 4x4")
         return mat[:-1, :]
 
-def look_at_np(from_, to_, up_, openGL=False):
+def look_at_np(eye, at, up, opengl=False):
     """
     returns a batch of look_at transforms 4x4 (camera->world, the inverse of a ModelView matrix)
     will broadcast upon batch dimension if necessary.
-    :param from_: n x 3 from vectors in world space
-    :param to_: n x 3 at vector in world space
-    :param up_: n x 3 up vector in world space
-    :param is_openGL: if True, output will be in opengl coordinates (z backward, y up) otherwise (z forward, y down)
+    :param eye: n x 3 from vectors in world space
+    :param at: n x 3 at vector in world space
+    :param up: n x 3 up vector in world space
+    :param opengl: if True, output will be in OpenGL coordinates (z backward, y up) otherwise (z forward, y down)
     :return: n x 4 x 4 transformation matrices (camera->world, the inverse of a ModelView matrix)
     """
-    from_, to_, up_ = broadcast_batch(from_, to_, up_)
-    forward = to_ - from_
+    eye, at, up = broadcast_batch(eye, at, up)
+    forward = at - eye
     forward = forward / np.linalg.norm(forward, axis=-1, keepdims=True)
-    right = np.cross(forward, up_)
+    right = np.cross(forward, up)
     right = right / np.linalg.norm(right, axis=-1, keepdims=True)
     up = np.cross(forward, right)
     up = up / np.linalg.norm(up, axis=-1, keepdims=True)
     rot = np.concatenate((right[..., None], up[..., None], forward[..., None]), axis=-1)
-    c2w = np.concatenate((rot, from_[..., None]), axis=-1)
-    c2w = to_44(c2w)
-    if openGL:
-        c2w[:, :, 1] *= -1
-        c2w[:, :, 2] *= -1
+    c2w = compose_rt(rot, eye, square=True)
+    if opengl:
+        c2w = opencv_c2w_to_opengl_c2w(c2w)
     return c2w
 
 def look_at_torch(
         eye:torch.Tensor, #3
         at:torch.Tensor, #3
         up:torch.Tensor, #3
-        device:torch.device,
-        openGL:bool=False
+        opengl:bool=False
     ) -> torch.Tensor: #4,4
     """
-    creates a lookat transform matrix (OpenCV convention)
+    creates a lookat transform matrix
     :param eye: where the camera is
     :param at: where the camera is looking
     :param up: the up vector of world space
-    :param device: the device to put the matrix on
+    :param opengl: if True, output will be in OpenGL coordinates (z backward, y up) otherwise (z forward, y down)
     :return: 4x4 lookat transform matrix
     """
-    if openGL:
-        z = (eye - at).type(torch.float32).to(device)
-    else:
-        z = (at - eye).type(torch.float32).to(device)
+    # todo batch support
+    z = (at - eye).type(torch.float32)
     z /= torch.norm(z)
-    x = torch.cross(up, z).type(torch.float32).to(device)
+    x = torch.cross(z, up).type(torch.float32)
     x /= torch.norm(x)
-    y = torch.cross(z, x).type(torch.float32).to(device)
+    y = torch.cross(z, x).type(torch.float32)
     y /= torch.norm(y)
-    T = torch.eye(4, device=device)
-    T[:3,:3] = torch.stack([x,y,z],dim=1)
-    T[:3,3] = eye
-    return T
+    c2w = torch.eye(4, device=z.device)
+    c2w[:3,:3] = torch.stack([x,y,z],dim=1)
+    c2w[:3,3] = eye
+    if opengl:
+        c2w = opencv_c2w_to_opengl_c2w(c2w)
+    return c2w
 
 def orthographic_projection(l, r, b, t, n, f):
     """
     creates an orthographic projection matrix (OpenGL convention)
     :param l: left
     :param r: right
     :param b: bottom
@@ -229,32 +236,50 @@
     return np.array([[sx, 0, a, 0],
                       [ 0,sy, b, 0],
                       [ 0, 0, c, d],
                       [ 0, 0,-1, 0]])
 
 def opengl_project_from_opencv_intrinsics(opencv_intrinsics, width, height, near=0.1, far=100.0):
     """
-    given a matrix K from opencv, returns the corresponding projection matrix for opengl ("Eye/Camera/View space -> Clip Space")
-    :param opencv_project: 3x3 projection matrix from opencv
+    given a matrix K from opencv, returns the corresponding projection matrix for OpenGL ("Eye/Camera/View space -> Clip Space")
+    :param opencv_intrinsics: 3x3 intrinsics matrix from opencv
     :param width: width of the image
     :param height: height of the image
     :param near: near plane
     :param far: far plane
-    :return: 4x4 projection matrix for opengl (note: column major)
+    :return: 4x4 projection matrix for OpenGL (note: column major)
     """
     fx = opencv_intrinsics[0, 0]
     fy = opencv_intrinsics[1, 1]
     cx = opencv_intrinsics[0, 2]
     cy = opencv_intrinsics[1, 2]
     opengl_mtx = np.array([[2*fx/width, 0.0, (width - 2*cx)/width, 0.0],
                            [0.0, -2*fy/height, (height - 2*cy)/height, 0.0],
                            [0.0, 0.0, (-far - near) / (far - near), -2.0*far*near/(far-near)],
                            [0.0, 0.0, -1.0, 0.0]])
     return opengl_mtx
 
+def opencv_intrinsics_from_opengl_project(opengl_project, width, height):
+    """
+    given a projection matrix from OpenGL ("Eye/Camera/View space -> Clip Space"), returns a matrix K for opencv
+    :param opengl_project: 4x4 projection matrix from OpenGL
+    :param width: width of the image
+    :param height: height of the image
+    :return: 3x3 intrinsics matrix for opencv
+    note: assumes camera center is middle of image
+    """
+    fx = opengl_project[0, 0] * width / 2
+    fy = opengl_project[1, 1] * height / 2
+    cx = width / 2
+    cy = height / 2
+    opencv_mtx = np.array([[fx, 0.0, cx],
+                           [0.0, fy, cy],
+                           [0.0, 0.0, 1]])
+    return opencv_mtx
+
 def opengl_c2w_to_opencv_c2w(opengl_transforms):
     """
     given a modelview matrix (World space->Eye/Camera/View space) where z is backward and y is up,
     converts its coordinate system to opencv convention (z forward, y down)
     :param opengl_transforms: 4x4 modelview matrix or batch of 4x4 modelview matrices
     :return: 4x4 modelview matrix in opencv convention
     """
@@ -266,38 +291,48 @@
         raise ValueError("transform must be 4x4 or batch of 4x4")
     my_transforms[:, :, 1] *= -1
     my_transforms[:, :, 2] *= -1
     return my_transforms.reshape(opengl_transforms.shape)
 
 def opencv_c2w_to_opengl_c2w(opencv_transform):
     """
-    converts coordinates of "vision" (opencv) to opengl coordinates by flipping y and z axes
+    converts coordinates of "vision" (opencv) to OpenGL coordinates by flipping y and z axes
     """
     return opengl_c2w_to_opencv_c2w(opencv_transform)
 
-def create_random_cameras_on_unit_sphere(n, r, device="cuda"):
+def create_random_cameras_on_unit_sphere(n_cams, radius, normal=None, opengl=False, device="cpu"):
     """
     creates a batch of world2view ("ModelView" matrix) and view2clip ("Projection" matrix) transforms on a unit sphere looking at the center
-    :param n: number of cameras
-    :param r: radius of the sphere
+    :param n_cams: number of cameras
+    :param radius: radius of the sphere
+    :param normal: if provided, only the hemisphere in the direction of the normal is sampled
+    :param opengl: if True, the coordinate system is converted to openGL convention (z backward, y up)
     :param device: device to put the tensors on
-    :return: world2view, view2clip
+    :return: world2view (world2cam), view2clip (requires further processing if opengl=False)
     """
-    locs = torch.randn((n, 3), device=device)
+    locs = torch.randn((n_cams, 3), device=device)
     locs = torch.nn.functional.normalize(locs, dim=1, eps=1e-6)
-    locs = locs * r
-    matrices = torch.empty((n, 4, 4), dtype=torch.float32, device=device)
+    if normal is not None:
+        if normal.ndim == 1:
+            normal = normal[None, :]
+        normal = torch.nn.functional.normalize(normal, dim=-1, eps=1e-6)
+        dot_product = (locs[:, None, :] @ normal[:, :, None]).squeeze()
+        locs[dot_product < 0] *= -1
+    locs = locs * radius
+    matrices = torch.empty((n_cams, 4, 4), dtype=torch.float32, device=device)
     for i in range(len(locs)):
         matrices[i] = look_at_torch(locs[i],
-                                       torch.zeros(3, dtype=torch.float32, device=device),
-                                       torch.tensor([0.,1.,0.], device=device),
-                                       device=device)
+                                    torch.zeros(3, dtype=torch.float32, device=device),
+                                    torch.tensor([0.,0.,1.], device=device),
+                                    opengl=opengl)
     v2w = matrices  # c2w
     w2v = torch.inverse(v2w)
-    v2c = torch.tensor(perspective_projection(), dtype=torch.float32, device=device)
+    v2c = perspective_projection()
+    v2c = np.tile(v2c[None, :], (n_cams, 1, 1))
+    v2c = torch.tensor(v2c, dtype=torch.float32, device=device)
     return w2v, v2c
 
 def to_np(arr: torch.Tensor):
     """
     converts a tensor to numpy array
     :param arr: tensor
     :return: numpy array
@@ -327,37 +362,69 @@
     :return: torch tensor
     """
     if dtype is None:
         return torch.tensor(arr, device=device)
     else:
         return torch.tensor(arr, dtype=dtype, device=device)
 
-def to_8b(x: np.array, clip=True):
-    """
-    convert a numpy (float, double) array to 8 bit
-    """
-    if x.dtype == np.float32 or x.dtype == np.float64:
-        if clip:
-            x = np.clip(x, 0, 1)
-        return (255 * x).astype(np.uint8)
-    elif x.dtype == np.uint8:
-        return x
-
-def to_float(x: np.array, clip=True):
-    """
-    convert a numpy (8bit) array to float
+def to_8b(x, clip=True):
     """
-    if x.dtype == np.uint8:
-        return x.astype(np.float32) / 255
-    elif x.dtype == np.float32:
-        if clip:
-            x = np.clip(x, 0, 1)
-        return x
+    convert an array (float, double) array to 8 bit
+    :param x: array
+    :param clip: if True, clips values to [0,1]
+    :return: 8 bit array
+    """
+    if is_np(x):
+        if x.dtype == np.float32 or x.dtype == np.float64:
+            if clip:
+                x = np.clip(x, 0, 1)
+            return (255 * x).round().astype(np.uint8)
+        elif x.dtype == bool:
+            return x.astype(np.uint8) * 255
+        elif x.dtype == np.uint8:
+            return x
     else:
-        raise ValueError("unsupported dtype")
+        if x.dtype == torch.float32 or x.dtype == torch.float64:
+            if clip:
+                x = torch.clamp(x, 0, 1)
+            return (255 * x).round().type(torch.uint8)
+        elif x.dtype == torch.bool:
+            return x.type(torch.uint8) * 255
+        elif x.dtype == torch.uint8:
+            return x
+
+def to_float(x, clip=True):
+    """
+    convert a 8bit or bool array to float
+    :param x: array
+    :param clip: if True, clips values to [0,1]
+    :return: float array
+    """
+    if is_np(x):
+        if x.dtype == np.uint8:
+            return x.astype(np.float32) / 255
+        elif x.dtype == np.float32:
+            if clip:
+                x = np.clip(x, 0, 1)
+            return x
+        elif x.dtype == bool:
+            return x.astype(np.float32)
+        else:
+            raise ValueError("unsupported dtype")
+    else:
+        if x.dtype == torch.uint8:
+            return x.to(torch.float32) / 255
+        elif x.dtype == torch.float32:
+            if clip:
+                x = torch.clamp(x, 0, 1)
+            return x
+        elif x.dtype == torch.bool:
+            return x.to(torch.float32)
+        else:
+            raise ValueError("unsupported dtype")
 
 def to_PIL(x: np.array):
     """
     convert a numpy float array to a PIL image
     """
     if x.ndim == 3:
         return Image.fromarray(to_8b(x))
@@ -388,56 +455,68 @@
     if s.shape[-1] != 3:
         raise ValueError("translation vector must be 3d")
     if s.ndim == 1:
         s = s[None, :]
     mat = np.diag(s)
     return to_44(mat)
 
-def sincos(a):
-    a = np.deg2rad(a)
+def sincos(a, degrees=True):
+    """
+    sin and cos of an angle
+    :param a: angle
+    :param degrees: if True, a is in degrees
+    """
+    if degrees:
+        a = np.deg2rad(a)
     return np.sin(a), np.cos(a)
 
 def rotate(a, r):
     """
-    creates a rotation matrix from an angle and an axis
+    creates a rotation matrix from an angle a and an axis of rotation r
     """
     s, c = sincos(a)
     r = normalize(r)
     nc = 1 - c
     x, y, z = r
     return np.array([[x*x*nc +   c, x*y*nc - z*s, x*z*nc + y*s, 0],
                       [y*x*nc + z*s, y*y*nc +   c, y*z*nc - x*s, 0],
                       [x*z*nc - y*s, y*z*nc + x*s, z*z*nc +   c, 0],
                       [           0,            0,            0, 1]])
 
-def rotx(a):
+def rotx(a, degrees=True):
     """
-    creates a rotation matrix around the x axis
+    creates a homogeneous 3D rotation matrix around the x axis
+    a: angle
+    degrees: if True, a is in degrees, else radians
     """
-    s, c = sincos(a)
+    s, c = sincos(a, degrees)
     return np.array([[1,0,0,0],
                       [0,c,-s,0],
                       [0,s,c,0],
                       [0,0,0,1]])
 
-def roty(a):
+def roty(a, degrees=True):
     """
-    creates a rotation matrix around the y axis
+    creates a homogeneous 3D rotation matrix around the y axis
+    a: angle
+    degrees: if True, a is in degrees, else radians
     """
-    s, c = sincos(a)
+    s, c = sincos(a, degrees)
     return np.array([[c,0,s,0],
                       [0,1,0,0],
                       [-s,0,c,0],
                       [0,0,0,1]])
 
-def rotz(a):
+def rotz(a, degrees=True):
     """
-    creates a rotation matrix around the z axis
+    creates a homogeneous 3D rotation matrix around the z axis
+    a: angle
+    degrees: if True, a is in degrees, else radians
     """
-    s, c = sincos(a)
+    s, c = sincos(a, degrees)
     return np.array([[c,-s,0,0],
                       [s,c,0,0],
                       [0,0,1,0],
                       [0,0,0,1]])
 
 def map_range(x, in_min, in_max, out_min, out_max):
     """
@@ -501,24 +580,43 @@
     # angle1 = torch.arccos(ortho.dot(r @ ortho))
     angle2 = torch.arccos((torch.trace(r) - 1) / 2)
     raise NotImplementedError("please verify this function implementation before usage")
     return rotvec * angle2
 
 def random_qvec(n: int):
     """
-    Generate random quaternions representing rotations
+    generate random quaternions representing rotations
     :param n: Number of quaternions in a batch to return.
     :return: Quaternions as tensor of shape (N, 4).
     """
     o = np.random.randn(n, 4)
     s = (o * o).sum(1)
     denom = np.copysign(np.sqrt(s), o[:, 0])[:, None]
     o = o / denom
     return o
 
+def random_vectors_on_sphere(n, normal=None, device="cpu"):
+    """
+    create a batch of uniformly distributed random unit vectors on a sphere
+    note: if normal is provided, returns random unit vectors on the hemisphere around the normal, but isn't uniform anymore.
+    :param n: number of vectors
+    :param normal: normals to orient the hemisphere (,3) or (n,3)
+    :param device: device to put the tensors on
+    :return: tensor of shape (n, 3)
+    """
+    locs = torch.randn((n, 3), device=device)
+    locs = torch.nn.functional.normalize(locs, dim=1, eps=1e-6)
+    if normal is not None:
+        if normal.ndim == 1:
+            normal = normal[None, :]
+        normal = torch.nn.functional.normalize(normal, dim=-1, eps=1e-6)
+        dot_product = (locs[:, None, :] @ normal[:, :, None]).squeeze()
+        locs[dot_product < 0] *= -1
+    return locs
+
 def qvec2mat(qvec):
     """
     Converts a quaternion to a rotation matrix
     :param qvec: tensor of size 4 where real part is first (a + bi + cj + dk) => (a, b, c, d)
     :return: rotation matrix 3x3
     """
     return batch_qvec2mat(qvec[None, :])[0]
@@ -531,22 +629,20 @@
     """
     if qvecs.shape[-1] != 4:
         raise ValueError("quaternions must be of shape (..., 4)")
     if qvecs.ndim == 1:
         qvecs = qvecs[None, :]
     if qvecs.ndim > 2:
         raise ValueError("quaternions must be of shape (..., 4)")
-    if type(qvecs) == torch.Tensor:
-        r, i, j, k = torch.unbind(qvecs, -1)
-        stacking_func = torch.stack
-    elif type(qvecs) == np.ndarray:
+    if is_np(qvecs):
         r, i, j, k = [x[0] for x in np.split(qvecs, 4, -1)]
         stacking_func = np.stack
     else:
-        raise ValueError("quaternions must be of type torch.Tensor or np.ndarray")
+        r, i, j, k = torch.unbind(qvecs, -1)
+        stacking_func = torch.stack
     two_s = 2.0 / (qvecs * qvecs).sum(-1)
     o = stacking_func([1 - two_s * (j * j + k * k),
                        two_s * (i * j - k * r),
                        two_s * (i * k + j * r),
                        two_s * (i * j + k * r),
                        1 - two_s * (i * i + k * k),
                        two_s * (j * k - i * r),
```

### Comparing `gsoup-0.0.7/src/gsoup/geometry_advanced.py` & `gsoup-0.0.8/src/gsoup/geometry_advanced.py`

 * *Files identical despite different names*

### Comparing `gsoup-0.0.7/src/gsoup/geometry_basic.py` & `gsoup-0.0.8/src/gsoup/geometry_basic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 import torch
 import numpy as np
+from .core import is_np
 
 def duplicate_faces(f):
     """
     duplicates *every* face in the mesh, with flipped orientation (and appends it to the end of the tensor)
     note: will transfer to CPU if necessary with current implementation
     :param f: faces of the mesh (Nx3)
     :return: faces of the mesh with duplicated faces
     """
-    if type(f) != np.ndarray:
-        new_faces = f.detach().cpu().numpy()
-    else:
+    if is_np(f):
         new_faces = f
+    else:
+        new_faces = f.detach().cpu().numpy()
     swapped_f = new_faces.copy()
     swapped_f[:, [1, 2]] = swapped_f[:, [2, 1]]
     f_new = np.concatenate([new_faces, swapped_f])
-    if type(f) != np.ndarray:
+    if not is_np(f):
         f_new = torch.tensor(f_new, dtype=f.dtype, device=f.device)
     return f_new
 
 def remove_duplicate_faces(f):
     """
     remove duplicate faces from a mesh
     note: will transfer to CPU if necessary with current implementation
     :param f: faces of the mesh (Nx3)
     :return: vertices and faces of the mesh without duplicate faces
     """
-    if type(f) != np.ndarray:
-        f_new = f.detach().cpu().numpy()
-    else:
+    if is_np(f):
         f_new = f
+    else:
+        f_new = f.detach().cpu().numpy()
     f_new = np.sort(f_new, axis=1)
     f_new = np.unique(f_new, axis=0)
-    if type(f) != np.ndarray:
+    if not is_np(f):
         f_new = torch.tensor(f_new, dtype=f.dtype, device=f.device)
     return f_new
     
 def get_aspect_ratio(v: torch.Tensor, f: torch.Tensor):
     """
     measure aspect ratio of all triangles using: (circumradius / 2inradius)
     aspect_ratio < 1 for illegal or degenerate triangle
@@ -70,30 +71,27 @@
     return face_areas
 
 def normalize_vertices(vertices, mode="unit_sphere"):
     """
     shift and resize mesh to fit into a bounding volume
     """
     eps = 1e-7
-    if type(vertices) == np.ndarray:
+    if is_np(vertices):
         vertices -= (vertices.min(axis=0) + vertices.max(axis=0)) / 2
         if mode == "unit_sphere":
             vertices = vertices / (np.linalg.norm(vertices, axis=-1).max() + eps)
         elif mode == "unit_cube":
             vertices = vertices / (np.abs(vertices).max(dim=-1) + eps)
             raise NotImplementedError
-        
-    elif type(vertices) == torch.Tensor:
+    else:
         if mode == "unit_sphere":
             vertices -= (vertices.min(dim=0)[0] + vertices.max(dim=0)[0]) / 2
             vertices = vertices / (torch.norm(vertices, dim=-1).max() + eps)
         elif mode == "unit_cube":
             raise NotImplementedError
-    else:
-        raise TypeError("vertices must be either np.ndarray or torch.Tensor")
     return vertices
 
 def calc_face_normals(vertices: torch.Tensor, faces: torch.Tensor, normalize: bool = False):
     """
     # V,3 first vertex may be unreferenced
     # F,3 long, first face may be all zeros
 
@@ -103,15 +101,15 @@
         / \     looking onto surface (in neg normal direction)
       c1---c2
     """
     full_vertices = vertices[faces]  # F,(3,3)
     v0, v1, v2 = full_vertices.unbind(dim=1)  # F,3
     face_normals = torch.cross(v1 - v0, v2 - v0, dim=1)  # F,3
     if normalize:
-        face_normals = torch.nn.functional.normalize(face_normals, eps=1e-6, dim=1)  # TODO inplace?
+        face_normals = torch.nn.functional.normalize(face_normals, eps=1e-6, dim=1)
     return face_normals  # F,3
 
 def calc_vertex_normals(vertices: torch.Tensor, faces: torch.Tensor, face_normals: torch.Tensor = None):
     """
     # V,3 first vertex may be unreferenced
     # F,3 long, first face may be all zero
     return # F,3, not normalized
@@ -144,15 +142,15 @@
     e0---->-o
     """
 
     F = faces.shape[0]
     # make full edges, lower vertex index first
     face_edges = torch.stack((faces, faces.roll(-1, 1)), dim=-1)  # F*3,3,2
     full_edges = face_edges.reshape(F * 3, 2)
-    sorted_edges, _ = full_edges.sort(dim=-1)  # F*3,2 TODO min/max faster?
+    sorted_edges, _ = full_edges.sort(dim=-1)  # F*3,2 todo min/max faster?
 
     # make unique edges
     edges, full_to_unique = torch.unique(input=sorted_edges, return_inverse=True, dim=0)  # (E,2),(F*3)
     E = edges.shape[0]
     face_to_edge = full_to_unique.reshape(F, 3)  # F,3
     if not with_edge_to_face:
         return edges, face_to_edge
```

### Comparing `gsoup-0.0.7/src/gsoup/gsoup_io.py` & `gsoup-0.0.8/src/gsoup/gsoup_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,58 +46,55 @@
     :param file_name: if provided, saves image with this name
     """
     if image.ndim == 2:
         image = image[..., None]
     if image.ndim != 3:
         raise ValueError("Image must be 2 or 3 dimensional")
     dst = Path(dst)
-    dst.parent.mkdir(parents=True, exist_ok=True)
     save_images(image[None, ...], dst.parent, [dst.name], force_grayscale)
 
 def save_images(images, dst, file_names: list = [], force_grayscale: bool = False, overwrite: bool = True):
     """
     saves images as png
     :param images: (b x H x W x C) tensor
-    :param dst: path to save images to
+    :param dst: path to save images to (will create folder if it does not exist)
     :param force_grayscale: if True, saves images as grayscale
     :param file_names: if provided, saves images with these names (list of length b)
     """
     if type(images) == torch.Tensor:
         images = to_np(images)
     if np.isnan(images).any():
         raise ValueError("Images must be finite")
-    if images.dtype == np.float32 or images.dtype == np.float64:
+    if images.dtype == np.float32 or images.dtype == np.float64 or images.dtype == bool:
         images = to_8b(images)
     if images.dtype != np.uint8:
-        raise ValueError("Images must be of type uint8 (or float32/64, but will be converted to uint8)")
+        raise ValueError("Images must be of type uint8 (or float32/64, which will be converted to uint8)")
     if images.ndim != 4:
         raise ValueError("Images must be of shape (b x H x W x C)")
     if file_names:
         if images.shape[0] != len(file_names):
             raise ValueError("Number of images and length of file names list must match")
         file_names = [Path(x).stem for x in file_names]  # remove suffix
+    dst = Path(dst)
+    dst.mkdir(parents=True, exist_ok=True)
     for i, image in enumerate(images):
         if force_grayscale or images.shape[-1] == 1:
             if images.shape[-1] == 3:
                 image = image.mean(axis=-1, keepdims=True).astype(np.uint8)
             pil_image = Image.fromarray(image[..., 0], mode="L")
         else:
             pil_image = Image.fromarray(image)
-        if file_names is not None:
+        if file_names:
             cur_dst = Path(dst, "{}.png".format(file_names[i]))
-            if not overwrite:
-                if cur_dst.exists():
-                    continue
-            pil_image.save(str(cur_dst))
         else:
             cur_dst = Path(dst, "{:05d}.png".format(i))
-            if not overwrite:
-                if cur_dst.exists():
-                    continue
-            pil_image.save(str(cur_dst))
+        if not overwrite:
+            if cur_dst.exists():
+                continue
+        pil_image.save(str(cur_dst))
 
 def load_image(path, to_float=False, channels_last=True, to_torch=False, device=None, resize_wh=None, as_grayscale=False):
     """
     loads an image from a single file
     :param path: path to file
     :param to_float: if True, converts image to float
     :param return_paths: if True, returns a list of file paths
@@ -304,15 +301,15 @@
     f = np.stack(faceList)
     if finite_flag and verbose:
         print("Warning: some vertices in file were not finite")
     # vn = np.stack(vertexNormalList)
     # vt = np.stack(vertexTextureList)
     return v, f #, vn, vt
 
-def save_obj(path: Path, vertices, faces):
+def save_obj(vertices, faces, path: Path):
     """"
     :param path: path to save obj file to
     :param vertices: (n x 3) tensor of vertices
     :param faces: (m x 3) tensor of vertex indices
     """
     path = Path(path)
     if path.suffix != ".obj":
@@ -335,41 +332,41 @@
         raise ValueError("Faces must be of type int32 / int64")
     with open(str(path), "w") as file:
         for v in vertices:
             file.write("v {} {} {}\n".format(v[0], v[1], v[2]))  # write vertices
         for f in faces:
             file.write("f {} {} {}\n".format(f[0] + 1, f[1] + 1, f[2] + 1))  # obj indices start at 1
 
-def save_ply(path: Path, vertices, faces):
+def save_ply(vertices, faces, path: Path):
     raise NotImplementedError
 
-def save_mesh(path, vertices, faces):
+def save_mesh(vertices, faces, path):
     """
     saves a mesh to a file
     :param path: path to save mesh to
     :param vertices: (n x 3) tensor of vertices
     :param faces: (m x 3) tensor of vertex indices
     """
     path = Path(path)
     if path.suffix not in [".obj"]:
         raise ValueError("Only .obj is supported")
     else:
         if path.suffix == ".obj":
-            save_obj(path, vertices, faces)
+            save_obj(vertices, faces, path)
         # elif path.suffix == ".ply":
         #     save_ply(path, vertices, faces)
 
-def save_pointcloud(path: Path, vertices):
+def save_pointcloud(vertices, path: Path):
     path = Path(path)
     if path.suffix != ".ply":
         raise ValueError("Only .ply are supported")
     else:
-        save_ply(path, vertices, None)
+        save_ply(vertices, None, path)
 
-def save_meshes(path, vertices, faces, file_names: list = []):
+def save_meshes(vertices, faces, path, file_names: list = []):
     """
     saves a list of meshes to a folder
     :param path: path to save meshes to
     :param vertices: (b x V x 3) tensor
     :param faces: (b x F x 3) tensor
     :param file_names: list of file names (of length b)
     """
@@ -379,10 +376,10 @@
         raise ValueError("Vertices and faces must have the same batch size")
     if file_names:
         if len(file_names) != vertices.shape[0]:
             raise ValueError("Number of file names must match batch size")
     path = Path(path)
     for i, (v, f) in enumerate(zip(vertices, faces)):
         if file_names:
-            save_mesh(path / "{}.obj".format(file_names[i]), v, f)
+            save_mesh(v, f, path / "{}.obj".format(file_names[i]))
         else:
-            save_mesh(path / "{:05d}.obj".format(i), v, f)
+            save_mesh(v, f, path / "{:05d}.obj".format(i))
```

### Comparing `gsoup-0.0.7/src/gsoup/image.py` & `gsoup-0.0.8/src/gsoup/image.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 import numpy as np
+import torch
 from PIL import Image, ImageDraw, ImageFont
 from scipy import interpolate, spatial
-from .core import to_8b, to_float, to_hom, homogenize, broadcast_batch, map_range
+from .core import to_8b, to_float, to_hom, homogenize, broadcast_batch, is_np
 from .structures import get_gizmo_coords
 from .gsoup_io import save_image
 
 def alpha_compose(images, bg_color=None):
     """
     composes a single or batch of RGBA images into a single or batch of RGB images
     :param image: b x H x W x 4 or H x W x 4
     :param bg_color: 3 or b x 3
     :return: b x H x W x 3 or H x W x 3
     """
-    if bg_color is None:
-        bg_color = np.array([0., 0., 0.]).astype(np.float32)
     if images.ndim != 3 and images.ndim != 4:
         raise ValueError("image must be 3 or 4 dimensional")
     if images.shape[-1] != 4:
         raise ValueError("image must have 4 channels")
-    if images.dtype != np.float32:
-        images = to_float(images)
+    if is_np(images):
+        if bg_color is None:
+            bg_color = np.array([0., 0., 0.]).astype(np.float32)
+        if images.dtype != np.float32:
+            images = to_float(images)
+    else:
+        if bg_color is None:
+            bg_color = torch.tensor([0., 0., 0.], dtype=images.dtype, device=images.device)
+        if images.dtype != torch.float32:
+            images = to_float(images)
     alpha = images[..., 3:4]
     rgb = images[..., :3]
     return alpha * rgb + (1 - alpha) * bg_color
 
 def draw_text_on_image(images, text_per_image, fill_white=True):
     """
     writes text on images given as np array (b x H x W x 3)
@@ -45,44 +52,42 @@
         text = text_per_image[i]
         ImageDraw.Draw(rgb).text((0, 0), text, fill=fill, font=font)
     rgbs = np.array([np.asarray(rgb) for rgb in rgbs])
     if is_float:
         rgbs = to_float(rgbs)
     return rgbs
 
-def draw_gizmo_on_image(np_images, w2c, isOpenGL=False, scale=.05):
+def draw_gizmo_on_image(np_images, w2c, opengl=False, scale=.05):
     """
     adds a gizmo to a batch of np images.
     note: will broadcast np_images and w2c against eachother.
     :param np_images: b x H x W x 3
     :param w2c: b x 3 x 4 w2c transforms (opencv conventions)
-    :param isOpenGL: if True, the w2c transforms are assumed to be in OpenGL conventions, else OpenCV conventions
+    :param opengl: if True, the w2c transforms are assumed to be in OpenGL conventions, else OpenCV conventions
+    for opengl, w2c should be a bx4x4 matrix converting from world to *CLIP* space.
     :param scale: scale of the gizmo
     :return: b x H x W x 3
     """
     new_images = []
     if np_images.ndim != 4:
         raise ValueError("np_images must be b x H x W x 3")
     if w2c.ndim != 3:
         raise ValueError("KRt must be b x 3 x 4")
     np_images, w2c = broadcast_batch(np_images, w2c)
     for i, np_image in enumerate(np_images):
         pil_image = Image.fromarray(to_8b(np_image))
         W, H = pil_image.size
-        # W, H = image.shape[1], image.shape[0]
         gizmo_cords, _, _ = get_gizmo_coords(scale)
-        gizmo_hom = to_hom(gizmo_cords)  #  = np.concatenate((gizmo_cords, np.ones_like(gizmo_cords[:, 0:1])), axis=-1)
+        gizmo_hom = to_hom(gizmo_cords)
         verts_clip = (w2c[i] @ gizmo_hom.T).T
-        verts_clip = homogenize(verts_clip) # verts_screen_xy = verts_screen[:, :2] / verts_screen[:, 2:3]
-        if isOpenGL:
-            raise NotImplementedError("OpenGL convention is not supported for now")
-            # if not (np.abs(verts_screen_xy[:, 2]) <= 1).all():
-            #    raise ValueError("OpenGL convention is not followed")
-            # verts_clip = verts_clip[:, :2]
-            # verts_screen = np.array([W, H]) * (verts_clip + 1) / 2
+        verts_clip = homogenize(verts_clip)
+        if opengl:
+            verts_clip = verts_clip[:, :2]
+            verts_screen = np.array([W, H]) * (verts_clip + 1) / 2
+            verts_screen[:, 1] *= -1
         else:
             verts_screen = verts_clip
         desired_loc = np.array([W - 40, H - 40])
         verts_screen += desired_loc - verts_screen[0]
         draw = ImageDraw.Draw(pil_image)
         draw.line((tuple(verts_screen[0]), tuple(verts_screen[1])), fill="red", width = 0)
         draw.line((tuple(verts_screen[0]), tuple(verts_screen[2])), fill="green", width = 0)
@@ -102,15 +107,14 @@
     :return: new (H x W x 3) numpy array with line in between
     """
     if img1.dtype != np.uint8:
         line_color = np.array(line_color) / 255
     else:
         line_color = np.array(line_color, dtype=np.uint8)
     combined = np.ascontiguousarray(np.broadcast_to(line_color, img1.shape))
-    # combined = np.ones_like(img1)*255
     y, x, _ = img1.shape
     yy, xx = np.mgrid[:y, :x]
     img1_positions = (xx-lower_intersection*x)*np.tan(angle)-line_width//2>(yy-y)
     img2_positions = (xx-lower_intersection*x)*np.tan(angle)+line_width//2<(yy-y)
     combined[img1_positions] = img1[img1_positions]
     combined[img2_positions] = img2[img2_positions]
     return combined
@@ -157,14 +161,28 @@
     for i in range(0, width, spacing):
         for j in range(0, height, spacing):
             img1.ellipse([i, j, i + radius*2, j + radius*2], fill=tuple(np.random.randint(0, 255, size=(3,))))
     if dst is not None:
         img.save(str(dst))
     return np.array(img)
 
+def generate_checkerboard(h, w, blocksize):
+    """
+    generates a checkerboard pattern
+    note: if blocksize is not a divisor of w or h, the pattern will have extra "crops" at the edges
+    :param h: height of the image
+    :param w: width of the image
+    :param blocksize: size of the squares
+    :return: (H x W x 1) numpy array (np.bool)
+    """
+    c0, c1 = 0, 1  # color of the squares, for binary these are just 0,1
+    tile = np.array([[c0, c1],[c1, c0]], dtype=np.bool).repeat(blocksize, axis=0).repeat(blocksize, axis=1)[..., None]
+    grid = np.tile(tile, ( h//(2*blocksize)+1, w//(2*blocksize)+1, 1))
+    return grid[:h,:w]
+
 def generate_stripe_pattern(height, width, background="black", direction="vert", thickness=5, spacing=50, dst=None):
     """
     generates an image with colored stripes in a certain direction
     :param height: height of the image
     :param width: width of the image
     :param background: background color
     :param direction: direction of the stripes ("vert", "hor", "both")
@@ -197,14 +215,15 @@
     generates an image with a lollipop pattern
     :param height: height of the image
     :param width: width of the image
     :param background: background color
     :param n: number of circles in the pattern
     :param m: number of lines in the pattern
     :param dst: if not None, the image is written to this path
+    :return: (H x W x 3) numpy array (uint8)
     """
     spacing_x = width // (2*n)
     spacing_y = height // (2*n)
     spacing_angle = 360 // m
     img = Image.new("RGB", (width, height), background)
     img1 = ImageDraw.Draw(img)
     for j in range(m):
@@ -353,56 +372,153 @@
     """
     if images.ndim != 4:
         raise ValueError("images must be a 4D array")
     if images.shape[1] != images.shape[2]:
         raise ValueError("images must be square")
     if not channels_last:
         raise NotImplementedError("only channels last is supported")
+    channels_size = images.shape[-1]
     input_size = np.array(images.shape[1:3])
     output_size = np.array([H, W])
     bin_size = input_size // output_size
     if mode == "max":
-        small_images = images.reshape((images.shape[0], output_size[0], bin_size[0], output_size[1], bin_size[1], 3)).max(4).max(2)
+        small_images = images.reshape((images.shape[0], output_size[0], bin_size[0], output_size[1], bin_size[1], channels_size)).max(4).max(2)
     elif mode == "mean":
-        small_images = images.reshape((images.shape[0], output_size[0], bin_size[0], output_size[1], bin_size[1], 3)).mean(4).mean(2)
-        small_images = small_images.astype(np.uint8)
+        small_images = images.reshape((images.shape[0], output_size[0], bin_size[0], output_size[1], bin_size[1], channels_size)).mean(4).mean(2)
+        if images.dtype == np.uint8:
+            small_images = small_images.astype(np.uint8)
     else:
         raise ValueError("mode must be one of 'max', 'mean'")
     return small_images
 
+def pad_image_to_res(images, res_h, res_w, bg_color=None):
+    """
+    pads a batch of numpy images to a specific resolution
+    :param image: numpy image b x h x w x c
+    :param res_h: height of the output image
+    :param res_w: width of the output image
+    :param bg_color: background color c (defaults to black)
+    :return: padded image b x res_h x res_w x c
+    """
+    if bg_color is None:
+        if is_np(images):
+            bg_color = np.zeros(images.shape[-1], dtype=images.dtype)
+        else:
+            bg_color = torch.zeros(images.shape[-1], dtype=images.dtype, device=images.device)
+    if images.ndim != 4:
+        raise ValueError("image must be a 4D array")
+    b, h, w, c = images.shape
+    if h > res_h or w > res_w:
+        raise ValueError("images dimensions is larger than the output resolution")
+    if h == res_h and w == res_w:
+        return images
+    if bg_color.shape[0] != c:
+        raise ValueError("background color must have the same number of channels as the image")
+    bg_color = bg_color[None, None, None, :]
+    if is_np(images):
+        output = np.zeros((b, res_h, res_w, c), dtype=images.dtype)
+    else:
+        output = torch.zeros((b, res_h, res_w, c), dtype=images.dtype, device=images.device)
+    output[:, :, :, :] = bg_color
+    corner_left = (res_w - w) // 2
+    corner_top = (res_h - h) // 2
+    output[:, corner_top:corner_top + h, corner_left:corner_left + w, :] = images
+    return output
+
+def crop_center(images, dst_h, dst_w):
+    """
+    crops a batch of images to a specific resolution, but the crop comes from the center of the image
+    :param image: numpy (or torch) array b x h x w x c
+    :param dst_h: height of the output image
+    :param dst_w: width of the output image
+    :return: cropped image b x dst_h x dst_w x c
+    """
+    if images.ndim != 4:
+        raise ValueError("image must be a 4D array")
+    _, h, w, _ = images.shape
+    if h < dst_h or w < dst_w:
+        raise ValueError("images dimensions is smaller than the output resolution")
+    if h == dst_h and w == dst_w:
+        return images
+    corner_left = (w - dst_w) // 2
+    corner_top = (h - dst_h) // 2
+    output = images[:, corner_top:corner_top + dst_h, corner_left:corner_left + dst_w, :]
+    return output
+
+def mask_regions(images, start_h, end_h, start_w, end_w):
+    """
+    masks a batch of numpy image with black background outside of region of interest (roi)
+    :param image: numpy image b x h x w x c
+    :param start_h: where does the roi height start
+    :param end_h: where does the roi height end
+    :param start_w: where does the roi width start
+    :param end_w: where does the roi width end
+    :return: masked image
+    """
+    if images.ndim != 4:
+        raise ValueError("image must be a 4D array")
+    _, h, w, _ = images.shape
+    if start_h < 0 or start_w < 0 or end_h > h or end_w > w:
+        raise ValueError("Values exceed image resolution")
+    output = np.zeros_like(images)
+    output[:, start_h:end_h, start_w:end_w, :] = images[start_h:end_h, start_w:end_w, :]
+    return output
+
+def adjust_contrast_brightness(img, alpha, beta=None):
+    """
+    adjusts image contrast and brightness using naive gain and bias factors
+    :param img: input image numpy array (n x h x w x 3), float values between 0 and 1
+    :param alpha: gain factor ("contrast") between 0 and inf
+    :param beta: bias factor ("brightness") between -inf and inf (but typically between -1 and 1)
+    :return: the new image
+    """
+    if img.dtype != np.float32:
+        raise ValueError("img must be a float32 numpy array (0-1)")
+    if beta is None:  # if beta is not provided, set to factor of alpha
+        beta = 0.5 - alpha / 2
+    new_img = img * alpha + beta
+    new_img[new_img < 0] = 0
+    new_img[new_img > 1] = 1
+    return new_img.astype(np.uint8)
+
 def change_brightness(input_img, brightness=0):
     """
-    changes brightness of an image
-    :param input_img the numpy image
+    changes brightness of an image or batch of images
+    :param input_img a numpy or torch tensor of float values between 0 and 1 (n x h x w x 3)
     :param brightness a number between -255 to 255 (0=no change)
     :return the new image
     """
+    if input_img.dtype != np.float32 and input_img.dtype != torch.float32:
+        raise ValueError("input_img must be a float32 array (0-1)")
     if brightness != 0:
         if brightness > 0:
             shadow = brightness
             highlight = 255
         else:
             shadow = 0
             highlight = 255 + brightness
         alpha_b = (highlight - shadow)/255
-        gamma_b = shadow
+        gamma_b = shadow / 255
     else:
         alpha_b = 1
         gamma_b = 0
     return input_img*alpha_b + gamma_b
 
-def change_contrast(input_img, contrast=127):
+def linear_to_srgb(linear):
     """
-    changes brightness of an image
-    :param input_img the numpy image
-    :param brightness a number between -127 to 127 (0=no change)
-    :return the new image
+    converts linear RGB to sRGB, see https://en.wikipedia.org/wiki/SRGB.
+    note: linear is expected to be in the range [0, 1]
     """
-    contrast = map_range(contrast, 0, 254, -127, 127)
-    if contrast != 0:
-        f = float(131 * (contrast + 127)) / (127 * (131 - contrast))
-        alpha_c = f
-        gamma_c = 127*(1-f)
-    else:
-        alpha_c = 1
-        gamma_c = 0
-    return input_img*alpha_c + gamma_c
+    eps = np.finfo(np.float32).eps
+    srgb0 = 323 / 25 * linear
+    srgb1 = (211 * np.maximum(eps, linear)**(5 / 12) - 11) / 200
+    return np.where(linear <= 0.0031308, srgb0, srgb1)
+
+def srgb_to_linear(srgb):
+    """
+    converts linear RGB to sRGB, see https://en.wikipedia.org/wiki/SRGB.
+    note: srgb is expected to be in the range [0, 1]
+    """
+    eps = np.finfo(np.float32).eps
+    linear0 = 25 / 323 * srgb
+    linear1 = np.maximum(eps, ((200 * srgb + 11) / (211)))**(12 / 5)
+    return np.where(srgb <= 0.04045, linear0, linear1)
```

### Comparing `gsoup-0.0.7/src/gsoup/procam.py` & `gsoup-0.0.8/src/gsoup/procam.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,74 @@
 import numpy as np
 import torch
 import cv2
 from .gsoup_io import save_image, save_images, load_images, load_image
+from .core import to_8b
 from .image import interpolate_multi_channel, change_brightness
 from pathlib import Path
 
 def warp_image(p2c, cam_image, cam_h=None, cam_w=None, output_path=None):
     """
+    todo: explain p2c structure
     given a 2D dense mapping between pixels from optical device 1 to optical device 2,
     warp an image from optical device 1 to optical device 2
     :param p2c: 2D dense mapping between pixels from optical device 1 to optical device 2
-    :param cam_image: path to image from optical device 1
+    :param cam_image: path to image from optical device 1, or float np array channels last, or pytorch tensor channels last
     :param cam_h: camera height, if not supplied assumes cam_image is in the correct dimensions in relation to p2c
     :param cam_w: camera width, if not supplied assumes cam_image is in the correct dimensions in relation to p2c
     :param output_path: path to save warped image to
+    :return: warped image np array uint8
     """
     if type(cam_image) == np.ndarray:
+        unwarped = torch.tensor(cam_image)
+    elif type(cam_image) == torch.Tensor:
         unwarped = cam_image
     else:
-        unwarped = load_image(cam_image, to_float=True, resize_wh=(cam_w, cam_h))
+        unwarped = load_image(cam_image, to_float=True, to_torch=True, resize_wh=(cam_w, cam_h))
+    if unwarped.dtype != torch.float32 and unwarped.dtype != torch.float64:
+        raise ValueError("cam_image must be float32 or float64")
+    if unwarped.ndim != 3:
+        raise ValueError("cam_image must be 3D")
+    if unwarped.shape[2] != 3:
+        raise ValueError("cam_image must be a channels last image.")
+    if cam_h is not None:
+        if unwarped.shape[0] != cam_h:
+            raise ValueError("cam_image must be of shape cam_h, cam_w, 3")
+    if cam_w is not None:
+        if unwarped.shape[1] != cam_w:
+            raise ValueError("cam_image must be of shape cam_h, cam_w, 3")
     #print(p2c.shape)
     #p2c = Image.open(Path(interpolated_p2c_path))
     if type(p2c) != np.ndarray:
-        p2c = np.load(p2c)
-    p2c = np.asarray(p2c)[:, :, :2]
+        p2c_data = np.load(p2c)
+    else:
+        p2c_data = p2c.copy()
+    p2c_data = np.asarray(p2c_data)[:, :, :2]
     #p2c = p2c/255
-    p2c[:, :, 0] = (p2c[:, :, 0] * 2) - 1
-    p2c[:, :, 1] = (p2c[:, :, 1] * 2) - 1
-    p2c[:, :, [1, 0]] = p2c[:, :, [0, 1]]
+    p2c_data[:, :, 0] = (p2c_data[:, :, 0] * 2) - 1
+    p2c_data[:, :, 1] = (p2c_data[:, :, 1] * 2) - 1
+    p2c_data[:, :, [1, 0]] = p2c_data[:, :, [0, 1]]
     # p2c = np.round(p2c).astype(np.int32)
-    grid = torch.tensor(p2c.astype(np.float32)).unsqueeze(0)
+    grid = torch.tensor(p2c_data.astype(np.float32)).unsqueeze(0)
     input = torch.tensor(unwarped).permute(2, 0, 1).unsqueeze(0)
     warped = torch.nn.functional.grid_sample(input, grid).squeeze().permute(1, 2, 0).numpy()
-    warped_int = (warped * 255).astype(np.uint8)
+    warped_int = to_8b(warped)
     if output_path is not None:
         output_path.parent.mkdir(exist_ok=True, parents=True)
         save_image(warped_int, output_path)
     return warped_int
 
 def generate_gray_code(height, width, step, output_dir=None):
     """
     generate gray code patterns for structured light scanning
     :param height: height of the pattern
     :param width: width of the pattern
     :param step: step size of the pattern (e.g. 2 means the patterns are half the resolution)
     :param output_dir: directory to save the patterns to
-    :return: list of patterns
+    :return: n x height x width array of patterns
     """
     gc_height = int((height-1)/step)+1
     gc_width = int((width-1)/step)+1
     graycode = cv2.structured_light_GrayCodePattern.create(gc_width, gc_height)
     patterns = graycode.generate()[1]
     # decrease pattern resolution
     exp_patterns = []
@@ -66,26 +85,27 @@
         output_dir = Path(output_dir)
         output_dir.mkdir(exist_ok=True, parents=True)
         file_names = ["pattern_{:02d}.png".format(i) for i in range(len(exp_patterns))]
         save_images(exp_patterns[..., None], output_dir, file_names=file_names)
     return exp_patterns
 
 def pix2pix_correspondence(proj_width, proj_height, step, captures,
-                           BLACKTHR = 2, WHITETHR = 30, output_dir=None, debug=False):
+                           BLACKTHR = 2, WHITETHR = 30, output_dir=None, verbose=True, debug=False):
     """
     finds dense pixel to pixel pix2pix_correspondence between a projector and a camera
     note: assumes gray code patterns used for projections were generated using generate_gray_code
     :param proj_width: width of projector
     :param proj_height: height of projector
     :param step: step factor used for gray code patterns (e.g. 2 means half resolution)
     :param captures: the actual n x cam_height x cam_width x 3 captured images, or a directory containing the images
     :param BLACKTHR: threshold for black pixels
     :param WHITETHR: threshold for white pixels
     :param output_dir: directory to save results to
-    :param debug: if True, saves debug images
+    :param verbose: if True, prints progress and status
+    :param debug: if True, saves debug images (must provide output_dir)
     """
     if output_dir is not None:
         output_dir = Path(output_dir)
         output_dir.mkdir(parents=True, exist_ok=True)
     # prep decoder
     gc_width = int((proj_width-1)/step)+1
     gc_height = int((proj_height-1)/step)+1
@@ -103,15 +123,16 @@
     white = imgs.pop()
     cam_height = white.shape[0]
     cam_width = white.shape[1]
     if debug:
         diff_pic = white.astype(np.uint64) - black.astype(np.uint64)
         diff_pic[diff_pic < 0] = 0
         save_image(diff_pic[..., None].astype(np.uint8), Path(output_dir, "white_black_diff.png"))
-        print('camera image size :', white.shape)
+        if verbose:
+            print('camera image size :', white.shape)
     # initialize
     viz_c2p = np.zeros((cam_height, cam_width, 3), np.float32)
     ragged_p2c = np.empty((proj_height, proj_width), dtype=object)
     for i in np.ndindex(ragged_p2c.shape): ragged_p2c[i] = []
     missing_values_c2p = np.ones((cam_height, cam_width), np.bool8)
     # c2p
     c2p_list = [] # [((cam x, y), (proj x, y))]
@@ -127,15 +148,16 @@
                 missing_values_c2p[y, x] = False
                 c2p_list.append(((x, y), fixed_pix))
     # p2c
     total_size = ragged_p2c.size
     counter = 0
     for i in range(proj_height):
         for j in range(proj_width):
-            print("{} / {}".format(counter, total_size), end="\r", flush=True)
+            if verbose:
+                print("{} / {}".format(counter, total_size), end="\r", flush=True)
             val = np.mean(ragged_p2c[i, j], dtype=np.float32, axis=0)
             if np.isnan(val).any():
                 val = np.zeros(2)
             else:
                 val = np.round(val).astype(np.int32)
             ragged_p2c[i, j] = val
             counter += 1
@@ -151,15 +173,16 @@
         np.save(Path(output_dir, "c2p.npy"), interpolated_c2p) 
         np.save(Path(output_dir, "p2c.npy"), interpolated_p2c) 
         if debug:
             save_image(interpolated_c2p, Path(output_dir, "interpolated_c2p.png"))
             save_image(interpolated_p2c, Path(output_dir, "interpolated_p2c.png"))
             save_image(viz_c2p, Path(output_dir, "c2p.png"))
             save_image(viz_p2c, Path(output_dir, "p2c.png"))
-            print('Amount of c2p correspondences :', len(c2p_list))
+            if verbose:
+                print('Amount of c2p correspondences :', len(c2p_list))
     return interpolated_c2p, interpolated_p2c
 
 def naive_color_compensate(target_image, all_white_image, all_black_image, cam_width, cam_height, brightness_decrease=-127, output_path=None, debug=False):
     """
     color compensate a projected image such that it appears closer to a target image from the perspective of a camera
     loosly based on "Embedded entertainment with smart projectors"
     :param target_image the desired image path from the perspective of the camera
```

### Comparing `gsoup-0.0.7/src/gsoup/sphere_trace.py` & `gsoup-0.0.8/src/gsoup/sphere_trace.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,16 +111,16 @@
     surface_normals = nn.functional.normalize(surface_normals, dim=-1)
     return surface_normals
 
 
 def generate_rays(w2v, v2c, resx=512, resy=512, device="cuda:0"):
     """
     generates batch of rays for a batch of cameras
-    :param w2v: world to view matrix
-    :param v2c: view to clip matrix
+    :param w2v: a batch of world to view matrices (nx4x4)
+    :param v2c: view to clip matrix (4x4)
     :param resx: resolution x
     :param resy: resolution y
     :param device: device
     """
     y_clip = (torch.arange(resy, dtype=torch.float32, device=device) / resy) * 2 - 1
     x_clip = (torch.arange(resx, dtype=torch.float32, device=device) / resx) * 2 - 1
     xy_clip = torch.stack(torch.meshgrid(x_clip, y_clip, indexing="ij"), dim=-1)
```

### Comparing `gsoup-0.0.7/src/gsoup/structures.py` & `gsoup-0.0.8/src/gsoup/structures.py`

 * *Files identical despite different names*

### Comparing `gsoup-0.0.7/src/gsoup/video.py` & `gsoup-0.0.8/src/gsoup/video.py`

 * *Files identical despite different names*

### Comparing `gsoup-0.0.7/src/gsoup/viewer.py` & `gsoup-0.0.8/src/gsoup/viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,19 +71,19 @@
             ps_pointcloud.add_vector_quantity("vecs", v,
                                             enabled=True,
                                             radius=0.002,
                                             length=0.1,
                                             color=(0.2, 0.5, 0.5))
         return ps_pointcloud
 
-    def register_camera(self, name, poses, edge_rad, group=True, alpha=1.0):
+    def register_camera(self, name, poses, edge_rad, group=True, alpha=1.0, scale=0.1):
         """
         register a camera structure to polyscope
         """
-        v_cam, e_cam, c_cam = structures.get_camera_coords()
+        v_cam, e_cam, c_cam = structures.get_camera_coords(scale)
         v_tot = []
         e_tot = []
         c_tot = []
         for i, pose in enumerate(poses):
             v = homogenize((pose @ to_hom(v_cam).T).T)
             if group:
                 v_tot.append(v)
```

### Comparing `gsoup-0.0.7/src/gsoup/viewer_drivers.py` & `gsoup-0.0.8/src/gsoup/viewer_drivers.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,17 +121,21 @@
     :param group_cameras: if true, accelerates view but groups camera as a single object
     :return:
     """
     gviewer.init(height=512, width=512)
     gviewer.ps.set_up_dir("z_up")
     edge_rad = 0.0005
     v_aabb, e_aabb, c_aabb = structures.get_aabb_coords()
-    ps_net = gviewer.ps.register_curve_network("aabb", v_aabb, e_aabb, radius=edge_rad)
-    ps_net.add_color_quantity("color", c_aabb, defined_on='edges', enabled=True)
-    gviewer.register_pointcloud("center_of_world", np.zeros((1, 3)), c=np.array([1., 1., 1.])[None, :], radius=0.005, mode="sphere")
+    aabb_network = gviewer.ps.register_curve_network("aabb", v_aabb, e_aabb, radius=edge_rad)
+    aabb_network.add_color_quantity("color", c_aabb, defined_on='edges', enabled=True)
+    v_gizmo, e_gizmo, c_gizmo = structures.get_gizmo_coords(0.1)
+    gizmo_network = gviewer.ps.register_curve_network("gizmo", v_gizmo, e_gizmo, radius=edge_rad)
+    gizmo_network.add_color_quantity("color", c_gizmo, defined_on='edges', enabled=True)
+    coa = np.zeros((1, 3))
+    gviewer.register_pointcloud("center_of_world", coa, c=np.array([1., 1., 1.])[None, :], radius=0.005, mode="sphere")
     if camera_poses is not None:
         v_tot, e_tot, c_tot = gviewer.register_camera("cameras", camera_poses, edge_rad, group_cameras)
     if meshes is not None:
         for i, mesh in enumerate(meshes):
             gviewer.register_mesh("mesh_{}".format(i), mesh[0], mesh[1], transparency=0.5)
     if pointclouds is not None:
         for i, pointcloud in enumerate(pointclouds):
```

### Comparing `gsoup-0.0.7/src/gsoup.egg-info/PKG-INFO` & `gsoup-0.0.8/src/gsoup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsoup
-Version: 0.0.7
+Version: 0.0.8
 Summary: A geoemtry & graphics library with focus on clarity rather than performance.
 Author-email: Yotam Erel <erelyotam@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Yotam Erel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gsoup-0.0.7/src/gsoup.egg-info/SOURCES.txt` & `gsoup-0.0.8/src/gsoup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

