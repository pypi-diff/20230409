# Comparing `tmp/RcToolBox-0.0.2.tar.gz` & `tmp/RcToolBox-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RcToolBox-0.0.2.tar", last modified: Tue Apr  4 21:05:07 2023, max compression
+gzip compressed data, was "RcToolBox-0.0.3.tar", last modified: Sun Apr  9 10:38:53 2023, max compression
```

## Comparing `RcToolBox-0.0.2.tar` & `RcToolBox-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,24 @@
-drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-04 21:05:07.962109 RcToolBox-0.0.2/
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      231 2023-04-04 21:05:07.960529 RcToolBox-0.0.2/PKG-INFO
-drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-04 21:05:07.932942 RcToolBox-0.0.2/RcToolBox/
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        0 2023-03-07 20:28:07.000000 RcToolBox-0.0.2/RcToolBox/__init__.py
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     2222 2023-04-04 21:00:33.000000 RcToolBox-0.0.2/RcToolBox/basic_op.py
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     4937 2023-03-30 14:01:14.000000 RcToolBox-0.0.2/RcToolBox/dataset_op.py
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     3781 2023-04-04 20:53:19.000000 RcToolBox-0.0.2/RcToolBox/nifti_op.py
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     4412 2023-04-01 22:32:30.000000 RcToolBox-0.0.2/RcToolBox/pandas_op.py
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      918 2023-03-30 09:36:47.000000 RcToolBox-0.0.2/RcToolBox/xeon_op.py
-drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-04 21:05:07.955544 RcToolBox-0.0.2/RcToolBox.egg-info/
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      231 2023-04-04 21:05:06.000000 RcToolBox-0.0.2/RcToolBox.egg-info/PKG-INFO
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      306 2023-04-04 21:05:06.000000 RcToolBox-0.0.2/RcToolBox.egg-info/SOURCES.txt
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        1 2023-04-04 21:05:06.000000 RcToolBox-0.0.2/RcToolBox.egg-info/dependency_links.txt
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)       45 2023-04-04 21:05:06.000000 RcToolBox-0.0.2/RcToolBox.egg-info/requires.txt
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)       10 2023-04-04 21:05:06.000000 RcToolBox-0.0.2/RcToolBox.egg-info/top_level.txt
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)       38 2023-04-04 21:05:07.963216 RcToolBox-0.0.2/setup.cfg
--rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      808 2023-04-04 21:03:36.000000 RcToolBox-0.0.2/setup.py
+drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-09 10:38:53.618720 RcToolBox-0.0.3/
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      223 2023-04-09 10:38:53.617127 RcToolBox-0.0.3/PKG-INFO
+drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-09 10:38:53.565690 RcToolBox-0.0.3/RcToolBox/
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        0 2023-03-07 20:28:07.000000 RcToolBox-0.0.3/RcToolBox/__init__.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     2222 2023-04-04 21:00:33.000000 RcToolBox-0.0.3/RcToolBox/basic_op.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     6647 2023-04-09 10:37:05.000000 RcToolBox-0.0.3/RcToolBox/dataset_op.py
+drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-09 10:38:53.597955 RcToolBox-0.0.3/RcToolBox/draw/
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-05 11:05:14.000000 RcToolBox-0.0.3/RcToolBox/draw/__init__.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     2614 2023-04-09 10:09:08.000000 RcToolBox-0.0.3/RcToolBox/draw/df_plot.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     3737 2023-04-06 22:20:13.000000 RcToolBox-0.0.3/RcToolBox/nifti_op.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     4412 2023-04-01 22:32:30.000000 RcToolBox-0.0.3/RcToolBox/pandas_op.py
+drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-09 10:38:53.611976 RcToolBox-0.0.3/RcToolBox/segmentation/
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-05 11:05:02.000000 RcToolBox-0.0.3/RcToolBox/segmentation/__init__.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     2832 2023-04-09 10:37:38.000000 RcToolBox-0.0.3/RcToolBox/segmentation/evaluation.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)     1704 2023-04-09 10:07:40.000000 RcToolBox-0.0.3/RcToolBox/segmentation/metric.py
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      928 2023-04-09 10:06:45.000000 RcToolBox-0.0.3/RcToolBox/xeon_op.py
+drwxr-xr-x   0 rgao     (286349) lkeb-hpc (159106)        0 2023-04-09 10:38:53.589137 RcToolBox-0.0.3/RcToolBox.egg-info/
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      223 2023-04-09 10:38:53.000000 RcToolBox-0.0.3/RcToolBox.egg-info/PKG-INFO
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      464 2023-04-09 10:38:53.000000 RcToolBox-0.0.3/RcToolBox.egg-info/SOURCES.txt
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)        1 2023-04-09 10:38:53.000000 RcToolBox-0.0.3/RcToolBox.egg-info/dependency_links.txt
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)       68 2023-04-09 10:38:53.000000 RcToolBox-0.0.3/RcToolBox.egg-info/requires.txt
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)       10 2023-04-09 10:38:53.000000 RcToolBox-0.0.3/RcToolBox.egg-info/top_level.txt
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)       38 2023-04-09 10:38:53.619935 RcToolBox-0.0.3/setup.cfg
+-rw-r--r--   0 rgao     (286349) lkeb-hpc (159106)      840 2023-04-09 10:37:18.000000 RcToolBox-0.0.3/setup.py
```

### Comparing `RcToolBox-0.0.2/RcToolBox/basic_op.py` & `RcToolBox-0.0.3/RcToolBox/basic_op.py`

 * *Files identical despite different names*

### Comparing `RcToolBox-0.0.2/RcToolBox/nifti_op.py` & `RcToolBox-0.0.3/RcToolBox/nifti_op.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,70 +3,72 @@
 import SimpleITK as sitk
 import numpy as np
 import vtk
 import os
 import fastremap
 
 def load_nifti(nifti_file, load_image=True, load_info=True):
+
     img_itk = sitk.ReadImage(nifti_file)
     origin, spacing, direction = img_itk.GetOrigin(), img_itk.GetSpacing(), img_itk.GetDirection()
     img_npy = None
     if load_image:
         img_npy = sitk.GetArrayFromImage(img_itk)
     if load_info:
         if img_npy is not None:
             return img_npy, origin, spacing, direction
         else:
             return origin, spacing, direction
     else:
         return img_npy
 
 
-def npy2nifti(npy, template_nifit_file, dst_file=None, mode=None):
+def npy2nifti(npy, template_nifit_file, dst_file):
     """
 
     Args:
         mode:
         nifti_file:
         numpy: could be npy file or array
         dst_file:
 
     Returns:
 
     """
-    if template_nifit_file.endswith('.nii.gz'):
-        origin, spacing, direction = load_nifti(template_nifit_file, False)
-        if not isinstance(npy, np.ndarray):
-            npy = np.load(npy)
-        if len(npy.shape) == 5 or len(npy.shape) == 4:
-            npy = np.squeeze(npy)
-        new_itk = sitk.GetImageFromArray(npy, isVector=False)
-        new_itk.SetOrigin(origin)
-        if mode == 'homogeneous':
-            new_itk.SetSpacing(np.array([1.0, 1.0, 1.0]))
-        else:
-            new_itk.SetSpacing(spacing)
-        new_itk.SetDirection(direction)
-        if dst_file is None:
-            dst_file = template_nifit_file.replace('.nii.gz', '_process.nii.gz')
-        sitk.WriteImage(new_itk, dst_file)
+    
+    assert isinstance(npy, np.ndarray) and template_nifit_file.endswith('.nii.gz') and dst_file.endswith('.nii.gz')
+    
+    
+    origin, spacing, direction = load_nifti(template_nifit_file, False)
+    if not isinstance(npy, np.ndarray):
+        npy = np.load(npy)
+    if len(npy.shape) == 5 or len(npy.shape) == 4:
+        npy = np.squeeze(npy)
+    new_itk = sitk.GetImageFromArray(npy, isVector=False)
+    new_itk.SetOrigin(origin)
+    new_itk.SetSpacing(spacing)
+    new_itk.SetDirection(direction)
+    if dst_file is None:
+        dst_file = template_nifit_file.replace('.nii.gz', '_process.nii.gz')
+    sitk.WriteImage(new_itk, dst_file)
 
 
 def nifti2mesh(nifti_file, label, dst_file=None):
+    
     """
     Read a nifti file including a binary map of a segmented organ with label id = label.
     Convert it to a smoothed mesh of type stl.
     filename_nii     : Input nifti binary map
     filename_stl     : Output mesh name in stl format
     label            : segmented label id
     """
 
     # read the file
     reader = vtk.vtkNIFTIImageReader()
-    reader.SetFileName(filename_nii)
+    reader.SetFileName(nifti_file)
     reader.Update()
 
     # apply marching cube surface generation
     surf = vtk.vtkDiscreteMarchingCubes()
     surf.SetInputConnection(reader.GetOutputPort())
     surf.SetValue(0, label)  # use surf.GenerateValues function if more than one contour is available in the file
     surf.Update()
@@ -90,15 +92,17 @@
     writer.SetInputConnection(smoother.GetOutputPort())
     writer.SetFileTypeToASCII()
     if dst_file is None:
         dst_file = nifti_file.replace('.nii.gz', '.stl')
     writer.SetFileName(dst_file)
     writer.Write()
 
-def get_nifti_mask_bbox(mask_npy, return_mask=False, return_coord=True):
+def get_mask_bbox(mask_npy, return_mask=False, return_coord=True):
+    
+    assert isinstance(mask_npy, np.ndarray)
     # Return a dictionary of point cloud, key is the label id, value is the point cloud
     ptc_m = fastremap.point_cloud(mask_npy)
     ptc = np.vstack([ptc_m[key] for key in ptc_m.keys()])
     min_z, max_z = fastremap.minmax(ptc[:, 0])
     min_y, max_y = fastremap.minmax(ptc[:, 1])
     min_x, max_x = fastremap.minmax(ptc[:, 2])
```

### Comparing `RcToolBox-0.0.2/RcToolBox/pandas_op.py` & `RcToolBox-0.0.3/RcToolBox/pandas_op.py`

 * *Files identical despite different names*

### Comparing `RcToolBox-0.0.2/RcToolBox/xeon_op.py` & `RcToolBox-0.0.3/RcToolBox/xeon_op.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # from multiprocessing import Pool
 from pathos.multiprocessing import ProcessingPool as Pool
-from basic_op import sprint
+from RcToolBox.basic_op import sprint
 
 """ 
 Here we use pathos.multiprocessing. Unlike python's multiprocessing module, 
 pathos.multiprocessing can directly utilize functions that require multiple arguments
 """
 
 def hardcore_process(function, *args, num_workers=4):
```

### Comparing `RcToolBox-0.0.2/setup.py` & `RcToolBox-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages            
 
 setup(
     name = "RcToolBox",      # 这里是pip项目发布的名称
-    version = "0.0.2",  # 版本号，数值大的会优先被pip
+    version = "0.0.3",  # 版本号，数值大的会优先被pip
     keywords = ["pip", "RcToolBox"],			# 关键字
     description = "RC personal ToolBox",	# 描述
     long_description = "RC personal ToolBox",
     license = "MIT Licence",		# 许可证
 
     url = "",     #项目相关文件地址，一般是github项目地址即可
     author = "RC",			# 作者
     author_email = "yilingyaomeng@gmail.com",
 
     packages = find_packages(),
     include_package_data = True,
     platforms = "any",
-    install_requires = ["numpy", "PyYAML", "SimpleITK", "Pathos", "seaborn", "pandas"]          #这个项目依赖的第三方库
+    install_requires = ["numpy", "PyYAML", "SimpleITK", "Pathos", "seaborn", "pandas", "fastremap", "openpyxl", "vtk"]          #这个项目依赖的第三方库
 )
```

