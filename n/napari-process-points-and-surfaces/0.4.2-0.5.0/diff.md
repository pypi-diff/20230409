# Comparing `tmp/napari-process-points-and-surfaces-0.4.2.tar.gz` & `tmp/napari-process-points-and-surfaces-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-process-points-and-surfaces-0.4.2.tar", last modified: Thu Mar 23 16:12:23 2023, max compression
+gzip compressed data, was "napari-process-points-and-surfaces-0.5.0.tar", last modified: Sun Apr  9 16:16:24 2023, max compression
```

## Comparing `napari-process-points-and-surfaces-0.4.2.tar` & `napari-process-points-and-surfaces-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 16:12:23.332702 napari-process-points-and-surfaces-0.4.2/
--rw-rw-rw-   0        0        0     1545 2022-12-11 08:10:39.000000 napari-process-points-and-surfaces-0.4.2/LICENSE
--rw-rw-rw-   0        0        0      123 2022-12-11 08:10:39.000000 napari-process-points-and-surfaces-0.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     9507 2023-03-23 16:12:23.332702 napari-process-points-and-surfaces-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     8109 2023-03-23 15:24:47.000000 napari-process-points-and-surfaces-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-23 16:12:23.270195 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/
--rw-rw-rw-   0        0        0    26930 2023-03-23 16:12:05.000000 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/__init__.py
--rw-rw-rw-   0        0        0    13148 2023-02-19 09:36:16.000000 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/_quantification.py
--rw-rw-rw-   0        0        0    11721 2023-02-18 13:24:12.000000 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/_surface_annotation_widget.py
-drwxrwxrwx   0        0        0        0 2023-03-23 16:12:23.301449 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/_tests/
--rw-rw-rw-   0        0        0        0 2022-12-11 08:10:40.000000 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/_tests/__init__.py
--rw-rw-rw-   0        0        0     5024 2023-02-19 08:46:50.000000 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/_tests/test_function.py
--rw-rw-rw-   0        0        0       39 2023-02-18 11:11:52.000000 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/_tests/test_open3d.py
--rw-rw-rw-   0        0        0     7024 2023-03-23 16:12:05.000000 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/_tests/test_vedo_functions.py
--rw-rw-rw-   0        0        0      622 2023-02-18 11:18:34.000000 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/_utils.py
--rw-rw-rw-   0        0        0    22814 2023-03-23 16:12:05.000000 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/_vedo.py
-drwxrwxrwx   0        0        0        0 2023-03-23 16:12:23.332702 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/data/
--rw-rw-rw-   0        0        0  3138605 2022-12-11 08:10:40.000000 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/data/bun_zipper.ply
--rw-rw-rw-   0        0        0      377 2022-12-11 08:10:40.000000 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/data/bun_zipper_stanford_bunny_source.txt
--rw-rw-rw-   0        0        0   126537 2023-02-18 13:24:12.000000 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/data/gastruloid.ply
--rw-rw-rw-   0        0        0      224 2023-02-18 13:24:12.000000 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/data/gastruloid_source.txt
--rw-rw-rw-   0        0        0    54920 2022-12-11 08:10:40.000000 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/data/knot.ply
--rw-rw-rw-   0        0        0     1205 2022-12-11 08:10:40.000000 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/data/knot_license.md
-drwxrwxrwx   0        0        0        0 2023-03-23 16:12:23.285821 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces.egg-info/
--rw-rw-rw-   0        0        0     9507 2023-03-23 16:12:23.000000 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1259 2023-03-23 16:12:23.000000 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 16:12:23.000000 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-03-23 16:12:23.000000 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      206 2023-03-23 16:12:23.000000 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces.egg-info/requires.txt
--rw-rw-rw-   0        0        0       35 2023-03-23 16:12:23.000000 napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      393 2023-03-04 22:21:28.000000 napari-process-points-and-surfaces-0.4.2/requirements.txt
--rw-rw-rw-   0        0        0     1778 2023-03-23 16:12:23.332702 napari-process-points-and-surfaces-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0      114 2022-12-11 08:10:40.000000 napari-process-points-and-surfaces-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:16:24.716839 napari-process-points-and-surfaces-0.5.0/
+-rw-rw-rw-   0        0        0     1545 2022-12-11 08:10:39.000000 napari-process-points-and-surfaces-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0      123 2022-12-11 08:10:39.000000 napari-process-points-and-surfaces-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9507 2023-04-09 16:16:24.716839 napari-process-points-and-surfaces-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8109 2023-03-23 15:24:47.000000 napari-process-points-and-surfaces-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 16:16:24.593262 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/
+-rw-rw-rw-   0        0        0    28662 2023-04-09 16:15:51.000000 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/__init__.py
+-rw-rw-rw-   0        0        0    13469 2023-04-09 16:15:25.000000 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/_quantification.py
+-rw-rw-rw-   0        0        0    11721 2023-02-18 13:24:12.000000 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/_surface_annotation_widget.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:16:24.651273 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/_tests/
+-rw-rw-rw-   0        0        0        0 2022-12-11 08:10:40.000000 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/_tests/__init__.py
+-rw-rw-rw-   0        0        0     5122 2023-04-09 16:15:25.000000 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/_tests/test_function.py
+-rw-rw-rw-   0        0        0       39 2023-02-18 11:11:52.000000 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/_tests/test_open3d.py
+-rw-rw-rw-   0        0        0     7024 2023-03-23 16:12:05.000000 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/_tests/test_vedo_functions.py
+-rw-rw-rw-   0        0        0     3117 2023-04-09 16:15:25.000000 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/_utils.py
+-rw-rw-rw-   0        0        0    25319 2023-04-09 16:15:25.000000 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/_vedo.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:16:24.714834 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/data/
+-rw-rw-rw-   0        0        0  3138605 2022-12-11 08:10:40.000000 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/data/bun_zipper.ply
+-rw-rw-rw-   0        0        0      377 2022-12-11 08:10:40.000000 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/data/bun_zipper_stanford_bunny_source.txt
+-rw-rw-rw-   0        0        0   126537 2023-02-18 13:24:12.000000 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/data/gastruloid.ply
+-rw-rw-rw-   0        0        0      224 2023-02-18 13:24:12.000000 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/data/gastruloid_source.txt
+-rw-rw-rw-   0        0        0    54920 2022-12-11 08:10:40.000000 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/data/knot.ply
+-rw-rw-rw-   0        0        0     1205 2022-12-11 08:10:40.000000 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/data/knot_license.md
+drwxrwxrwx   0        0        0        0 2023-04-09 16:16:24.642391 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces.egg-info/
+-rw-rw-rw-   0        0        0     9507 2023-04-09 16:16:24.000000 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1259 2023-04-09 16:16:24.000000 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 16:16:24.000000 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-04-09 16:16:24.000000 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      206 2023-04-09 16:16:24.000000 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       35 2023-04-09 16:16:24.000000 napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      393 2023-03-04 22:21:28.000000 napari-process-points-and-surfaces-0.5.0/requirements.txt
+-rw-rw-rw-   0        0        0     1778 2023-04-09 16:16:24.719846 napari-process-points-and-surfaces-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      114 2022-12-11 08:10:40.000000 napari-process-points-and-surfaces-0.5.0/setup.py
```

### Comparing `napari-process-points-and-surfaces-0.4.2/LICENSE` & `napari-process-points-and-surfaces-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-process-points-and-surfaces-0.4.2/PKG-INFO` & `napari-process-points-and-surfaces-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-process-points-and-surfaces
-Version: 0.4.2
+Version: 0.5.0
 Summary: Process and analyze surfaces using open3d and vedo in napari
 Home-page: https://github.com/haesleinhuepf/napari-process-points-and-surfaces
 Author: Robert Haase, Johannes Soltwedel
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/napari-process-points-and-surfaces/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/napari-process-points-and-surfaces#README.md
```

### Comparing `napari-process-points-and-surfaces-0.4.2/README.md` & `napari-process-points-and-surfaces-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/__init__.py` & `napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version__ = "0.4.2"
+__version__ = "0.5.0"
 __common_alias__ = "nppas"
 
 import warnings
 
 
 from napari_plugin_engine import napari_hook_implementation
 from napari_tools_menu import register_function, register_action
@@ -129,14 +129,17 @@
 def labels_to_centroids(labels_data:"napari.types.LabelsData", viewer:"napari.Viewer" = None) -> "napari.types.PointsData":
     """Determine centroids from all labels and store them as points.
 
     Parameters
     ----------
     labels_data:napari.types.LabelsData
     """
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
+
     from skimage.measure import regionprops
 
     statistics = regionprops(labels_data)
     centroids = [s.centroid for s in statistics]
     return centroids
 
 
@@ -152,14 +155,16 @@
 
     Parameters
     ----------
     points_data:napari.types.PointsData
     as_large_as_image:napari.types.ImageData
         An image to specify the size of the output image. This image will not be overwritten.
     """
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
 
     labels_stack = np.zeros(as_large_as_image.shape, dtype=int)
     for i, p in enumerate(points_data):
         if len(labels_stack.shape) == 3:
             labels_stack[int(p[0] + 0.5), int(p[1] + 0.5), int(p[2] + 0.5)] = i + 1
         elif len(labels_stack.shape) == 2:
             labels_stack[int(p[0] + 0.5), int(p[1] + 0.5)] = i + 1
@@ -194,14 +199,16 @@
     viewer: napari.Viewer, optional
 
     Returns
     -------
     binary_image:ImageData
     """
     import vedo
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
 
     my_mesh = vedo.mesh.Mesh((surface[0], surface[1]))
     vertices = my_mesh.points()  # get coordinates of surface vertices
 
     # get bounding box of mesh
     boundaries_l = np.min(vertices + 0.5, axis=0).astype(int)
     boundaries_r = np.max(vertices + 0.5, axis=0).astype(int)
@@ -216,44 +223,62 @@
         binary_image = my_mesh.binarize().tonumpy().astype(int)
 
     return np.asarray(binary_image > 0).astype(int)
 
 
 @register_function(menu="Surfaces > Create surface from any label (marching cubes, scikit-image, nppas)")
 @time_slicer
-def label_to_surface(labels: "napari.types.LabelsData", label_id: int = 1) -> "napari.types.SurfaceData":
+def label_to_surface(labels: "napari.types.LabelsData", label_id: int = 1, viewer: "napari.Viewer" = None) -> "napari.types.SurfaceData":
     """
     Turn a single label out of a label image into a surface using the marching cubes algorithm
 
     Parameters
     ----------
     labels_data:napari.types.LabelsData
     label_id: int
     """
     from skimage.measure import marching_cubes
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
 
     binary = np.asarray(labels == label_id)
 
     vertices, faces, normals, values = marching_cubes(binary, 0)
 
-    return remove_duplicate_vertices(SurfaceTuple((vertices, faces, values)))
+    result = remove_duplicate_vertices(SurfaceTuple((vertices, faces, values)))
+
+    # invert faces to make sure lighting works
+    return invert_faces(result)
+
+
+@register_function(menu="Surfaces > Invert faces (reverse, vedo, nppas)")
+@time_slicer
+def invert_faces(surface: "napari.types.SurfaceData", viewer: "napari.Viewer" = None) -> "napari.types.SurfaceData":
+    """
+    Invert faces (turn inside outside), which might make sense for visualization purposes such as lightning.
+    """
+    mesh = to_vedo_mesh(surface)
+    mesh.reverse()
+    return to_napari_surface_data(mesh)
 
 
 @register_function(menu="Surfaces > Create surface from all labels (marching cubes, scikit-image, nppas)")
 @time_slicer
-def all_labels_to_surface(labels: "napari.types.LabelsData") -> "napari.types.SurfaceData":
+def all_labels_to_surface(labels: "napari.types.LabelsData", viewer: "napari.Viewer" = None) -> "napari.types.SurfaceData":
     """
     Turn a set of labels into a surface using the marching cubes algorithm
 
     Parameters
     ----------
     labels_data:napari.types.LabelsData
     """
     import vedo
     from skimage.measure import marching_cubes
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
 
     # convert to numpy in case it's not (clesperanto, dask, ...)
     labels = np.asarray(labels)
 
     # Create a surface for every label
     mesh_list = []
     for label in np.unique(labels)[:-1]:
@@ -268,23 +293,26 @@
     #(mesh.points(), np.asarray(mesh.faces()), mesh.pointdata['OriginalMeshID'])
 
 # alias
 marching_cubes = all_labels_to_surface
 
 @register_function(menu="Surfaces > Create surface from largest label (marching cubes, scikit-image, nppas)")
 @time_slicer
-def largest_label_to_surface(labels: "napari.types.LabelsData") -> "napari.types.SurfaceData":
+def largest_label_to_surface(labels: "napari.types.LabelsData", viewer: "napari.Viewer" = None) -> "napari.types.SurfaceData":
     """
     Turn the largest label in a label image into a surface using the marching cubes algorithm
 
     Parameters
     ----------
     labels_data:napari.types.LabelsData
     """
     from skimage.measure import regionprops
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
+
     statistics = regionprops(labels)
 
     label_index = np.argmax([r.area for r in statistics])
     labels_list = [r.label for r in statistics]
     label = labels_list[label_index]
 
     return label_to_surface(labels, label)
@@ -708,7 +736,27 @@
 def _check_open3d():
     try:
         import open3d
         return True
     except:
         warnings.warn("Open3D is not installed. Follow the instructions here: http://www.open3d.org/docs/release/introduction.html#python-quick-start")
     return False
+
+
+@register_function(menu="Surfaces > Flip (vedo, nppas)")
+def flip(surface: "napari.types.SurfaceData", flip_x:bool=True, flip_y:bool=True, flip_z:bool=True, viewer: "napari.Viewer" = None) -> "napari.types.SurfaceData":
+    import numpy as np
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
+
+    surface = [f.copy() for f in surface]
+
+    coordinates = surface[0]
+    if flip_x:
+        coordinates[:,-1] = coordinates[:,-1] * -1 + np.max(coordinates[:,-1])
+    if flip_y:
+        coordinates[:,-2] = coordinates[:,-2] * -1 + np.max(coordinates[:,-2])
+    if flip_z:
+        coordinates[:,-3] = coordinates[:,-3] * -1 + np.max(coordinates[:,-3])
+
+    surface[0] = coordinates
+    return surface
```

### Comparing `napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/_quantification.py` & `napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/_quantification.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,18 +79,21 @@
     Gauss_Curvature = 0
     Mean_Curvature = 1
     Maximum_Curvature = 2
     Minimum_Curvature = 3
 
 
 @register_function(menu="Measurement maps > Surface quality (vedo, nppas)")
-def add_quality(surface: "napari.types.SurfaceData", quality_id: Quality = Quality.MIN_ANGLE) -> "napari.types.SurfaceData":
+def add_quality(surface: "napari.types.SurfaceData", quality_id: Quality = Quality.MIN_ANGLE, viewer: "napari.Viewer" = None) -> "napari.types.SurfaceData":
     from ._vedo import to_vedo_mesh
     import vedo
     from ._vedo import SurfaceTuple
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
+
     mesh = vedo.mesh.Mesh((surface[0], surface[1]))
     if not isinstance(quality_id, int):
         quality_id = quality_id.value
 
     if quality_id < 1000:
         mesh.compute_quality(quality_id)
 
@@ -223,37 +226,44 @@
     from napari_skimage_regionprops import add_table
     add_table(surface_layer, napari_viewer)
 
 
 @register_function(menu="Measurement maps > Surface curvature (vedo, nppas)")
 def add_curvature_scalars(surface: "napari.types.SurfaceData",
                           curvature_id: Curvature = Curvature.Gauss_Curvature,
+                          viewer: "napari.Viewer" = None
                           ) -> "napari.types.SurfaceData":
     """
     Determine the surface curvature using vedo built-in functions.
     
     This function determines surface curvature using the built-in methods of
     the vedo library.
 
     Parameters
     ----------
     surface : "napari.types.SurfaceData"
         3-Tuple of (points, faces, values)
     curvature_id : Union[Curvature, int] optional
         Method to be used: 0-gaussian, 1-mean, 2-max, 3-min curvature. The
         default is 0 (gaussian).
+    viewer : napari.Viewer, optional
+        makes light follow the camera in the given viewer
+
     Returns
     -------
     "napari.types.SurfaceData"
         3-tuple consisting of (points, faces, values)
         
     See also
     --------
     Vedo curvature: https://vedo.embl.es/autodocs/content/vedo/mesh.html?highlight=curvature#vedo.mesh.Mesh.addCurvatureScalars
     """
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
+
     import vedo
     from ._vedo import SurfaceTuple
 
     mesh = vedo.mesh.Mesh((surface[0], surface[1]))    
     if isinstance(curvature_id, int):
         used_method = curvature_id
     else:
```

### Comparing `napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/_surface_annotation_widget.py` & `napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/_surface_annotation_widget.py`

 * *Files identical despite different names*

### Comparing `napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/_tests/test_function.py` & `napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/_tests/test_function.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,17 @@
             surface_from_point_cloud_alpha_shape,\
             surface_from_point_cloud_ball_pivoting,\
             all_labels_to_surface,\
             label_to_surface,\
             largest_label_to_surface,\
             add_quality,\
             Quality,\
-            fill_holes
+            fill_holes, \
+            invert_faces, \
+            flip
 
     from skimage.data import cells3d
     nuclei = cells3d()[:, 1, 60:120, 30:80]
 
     from skimage.measure import label
     labels = label(nuclei > 20000)
 
@@ -51,14 +53,17 @@
     points_to_labels(points, labels)
     surface = points_to_convex_hull_surface(points)
     surface = fill_holes(surface)
     surface_from_point_cloud_ball_pivoting(points)
     surface_from_point_cloud_alpha_shape(points)
     add_quality(surface, Quality.SKEW)
 
+    invert_faces(surface)
+    flip(surface)
+
 def test_something2():
     from .._vedo import (to_vedo_mesh,
                          to_vedo_points,
                          to_napari_surface_data,
                          to_napari_points_data,
                          smooth_surface,
                          _subdivide_loop_vedo,
```

### Comparing `napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/_tests/test_vedo_functions.py` & `napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/_tests/test_vedo_functions.py`

 * *Files identical despite different names*

### Comparing `napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/_vedo.py` & `napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/_vedo.py`

 * *Files 10% similar despite different names*

```diff
@@ -135,173 +135,200 @@
 
 def _hide_vtk_warnings():
     from vtkmodules.vtkCommonCore import vtkObject
     vtkObject.GlobalWarningDisplayOff()
 
 
 @register_function(menu="Surfaces > Convex hull (vedo, nppas)")
-def create_convex_hull_from_surface(surface: "napari.types.SurfaceData") -> "napari.types.SurfaceData":
+def create_convex_hull_from_surface(surface: "napari.types.SurfaceData", viewer: "napari.Viewer" = None) -> "napari.types.SurfaceData":
     """Determine the convex hull of a surface
 
     Parameters
     ----------
     surface:napari.types.SurfaceData
+    viewer : napari.Viewer, optional
+        makes light follow the camera in the given viewer
+
 
     See Also
     --------
     ..[0] https://vedo.embl.es/autodocs/content/vedo/shapes.html#vedo.shapes.ConvexHull
     """
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
+
     mesh = to_vedo_mesh(surface)
 
     import vedo
     convex_hull_mesh = vedo.shapes.ConvexHull(mesh)
 
     return to_napari_surface_data(convex_hull_mesh)
 
 
 @register_function(menu="Surfaces > Remove duplicate vertices (vedo, nppas)")
-def remove_duplicate_vertices(surface: "napari.types.SurfaceData") -> "napari.types.SurfaceData":
+def remove_duplicate_vertices(surface: "napari.types.SurfaceData", viewer: "napari.Viewer" = None) -> "napari.types.SurfaceData":
     """
     Clean a surface mesh (i.e., remove duplicate faces & vertices).
 
     See Also
     --------
     ..[0] https://vedo.embl.es/docs/vedo/pointcloud.html#Points.clean
     
     """
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
+
     mesh = to_vedo_mesh(surface)
     clean_mesh = mesh.clean()
 
     return to_napari_surface_data(clean_mesh)
 
 
 @register_function(menu="Surfaces > Connected components labeling (vedo, nppas)")
-def connected_component_labeling(surface: "napari.types.SurfaceData") -> "napari.types.SurfaceData":
+def connected_component_labeling(surface: "napari.types.SurfaceData", viewer: "napari.Viewer" = None) -> "napari.types.SurfaceData":
     """
     Determine the connected components of a surface mesh.
 
     See Also
     --------
     ..[0] https://vedo.embl.es/docs/vedo/mesh.html#Mesh.compute_connectivity
     """
     from ._quantification import set_vertex_values
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
 
     mesh = to_vedo_mesh(surface)
     mesh.compute_connectivity()
     region_id = mesh.pointdata["RegionId"]
 
     mesh_out = to_napari_surface_data(mesh)
     mesh_out = set_vertex_values(mesh_out, region_id)
 
     return mesh_out
 
 
 @register_function(menu="Surfaces > Smooth (moving least squares, vedo, nppas)")
 def smooth_surface_moving_least_squares_2d(surface: "napari.types.SurfaceData",
-                                           smoothing_factor: float = 0.2) -> "napari.types.SurfaceData":
+                                           smoothing_factor: float = 0.2,
+                                           viewer: "napari.Viewer" = None) -> "napari.types.SurfaceData":
     """Apply a moving least squares approach to smooth a surface
 
     See Also
     --------
     ..[0] https://vedo.embl.es/autodocs/content/vedo/vedo/pointcloud.html#Points.smooth_mls_2d
     """
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
 
     mesh = to_vedo_mesh(surface)
 
     smooth_mesh = mesh.smooth_mls_2d(f=smoothing_factor)
 
     return to_napari_surface_data(smooth_mesh)
 
 
 @register_function(menu="Surfaces > Smooth (moving least squares with radius, vedo, nppas)")
 def smooth_surface_moving_least_squares_2d_radius(surface: "napari.types.SurfaceData",
                                                   smoothing_factor: float = 0.2,
-                                                  radius: float = 0.2) -> "napari.types.SurfaceData":
+                                                  radius: float = 0.2,
+                                                  viewer: "napari.Viewer" = None) -> "napari.types.SurfaceData":
     """Apply a moving least squares approach to smooth a surface. 
     
     The radius is used to determine the number of points to use for the smoothing.
 
     See Also
     --------
     ..[0] https://vedo.embl.es/autodocs/content/vedo/vedo/pointcloud.html#Points.smooth_mls_2d
     """
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
 
     mesh = to_vedo_mesh(surface)
 
     smooth_mesh = mesh.smooth_mls_2d(f=smoothing_factor, radius=radius)
 
     return to_napari_surface_data(smooth_mesh)
 
 
 @register_function(menu="Points > Smooth (moving least squares, vedo, nppas)")
 def smooth_pointcloud_moving_least_squares_2d(pointcloud: "napari.types.PointsData",
-                                              smoothing_factor: float = 0.2) -> "napari.types.PointsData":
+                                              smoothing_factor: float = 0.2,
+                                              viewer: "napari.Viewer" = None) -> "napari.types.PointsData":
     """Apply a moving least squares approach to smooth a point cloud.
 
     See Also
     --------
     ..[0] https://vedo.embl.es/autodocs/content/vedo/vedo/pointcloud.html#Points.smooth_mls_2d
     """
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
 
     points = to_vedo_points(pointcloud)
 
     smooth_points = points.smooth_mls_2d(f=smoothing_factor)
 
     return to_napari_points_data(smooth_points)
 
 
 @register_function(menu="Points > Smooth (moving least squares radius, vedo, nppas)")
 def smooth_pointcloud_moving_least_squares_2d_radius(pointcloud: "napari.types.PointsData",
                                                      smoothing_factor: float = 0.2,
-                                                     radius=2) -> "napari.types.PointsData":
+                                                     radius: float = 2,
+                                                     viewer: "napari.Viewer" = None) -> "napari.types.PointsData":
     """Apply a moving least squares approach to smooth a point cloud.
 
     The radius is used to determine the number of points to use for the smoothing.
 
     See Also
     --------
     ..[0] https://vedo.embl.es/autodocs/content/vedo/vedo/pointcloud.html#Points.smooth_mls_2d
     """
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
 
     points = to_vedo_points(pointcloud)
 
     smooth_points = points.smooth_mls_2d(f=smoothing_factor, radius=radius)
 
     return to_napari_points_data(smooth_points)
 
 
 @register_function(menu="Surfaces > Smooth (Windowed Sinc, vedo, nppas)")
 def smooth_surface(surface: "napari.types.SurfaceData",
                    number_of_iterations: int = 15,
                    pass_band: float = 0.1,
                    edge_angle: float = 15,
                    feature_angle: float = 60,
-                   boundary: bool = False
+                   boundary: bool = False,
+                   viewer: "napari.Viewer" = None
                    ) -> "napari.types.SurfaceData":
     """Smooth a surface using a Windowed Sinc kernel.
 
     See Also
     --------
     ..[0] https://vedo.embl.es/docs/vedo/mesh.html#Mesh.smooth
     """
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
 
     mesh = to_vedo_mesh(surface)
 
     smooth_mesh = mesh.smooth(niter=number_of_iterations,
                               pass_band=pass_band,
                               edge_angle=edge_angle,
                               feature_angle=feature_angle,
                               boundary=boundary)
 
     return to_napari_surface_data(smooth_mesh)
 
 
 #@register_function(menu="Surfaces > Subdivide loop (vedo, nppas)")
 def _subdivide_loop_vedo(surface: "napari.types.SurfaceData",
-                         number_of_iterations: int = 1
+                         number_of_iterations: int = 1,
+                         viewer: "napari.Viewer" = None
                          ) -> "napari.types.SurfaceData":
     """
     Make a mesh more detailed by subdividing in a loop.
 
     This increases the number of faces on the surface simply by subdividing
     each triangle into four new triangles.
 
@@ -311,22 +338,26 @@
     number_of_iterations:int
 
     See Also
     --------
     ..[0] https://vedo.embl.es/docs/vedo/mesh.html#Mesh.subdivide
     ..[1] https://vtk.org/doc/nightly/html/classvtkLoopSubdivisionFilter.html
     """
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
+
     mesh_in = to_vedo_mesh(surface)
     mesh_out = mesh_in.subdivide(number_of_iterations, method=0)
     return to_napari_surface_data(mesh_out)
 
 
 #@register_function(menu="Surfaces > Subdivide linear (vedo, nppas)")
 def _subdivide_linear(surface: "napari.types.SurfaceData",
-                      number_of_iterations: int = 1
+                      number_of_iterations: int = 1,
+                      viewer: "napari.Viewer" = None
                       ) -> "napari.types.SurfaceData":
     """
     Make a mesh more detailed by linear subdivision.
 
     The position of the created triangles is determined by a
     linear interpolation method and is thus slower than the
     loop subdivision algorithm.
@@ -337,23 +368,27 @@
     number_of_iterations:int
 
     See Also
     --------
     ..[0] https://vedo.embl.es/docs/vedo/mesh.html#Mesh.subdivide
     ..[1] https://vtk.org/doc/nightly/html/classvtkLinearSubdivisionFilter.html
     """
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
+
     mesh_in = to_vedo_mesh(surface)
     mesh_out = mesh_in.subdivide(number_of_iterations, method=1)
     return to_napari_surface_data(mesh_out)
 
 
 @register_function(menu="Surfaces > Subdivide adaptive (vedo, nppas)")
 def subdivide_adaptive(surface: "napari.types.SurfaceData",
                        number_of_iterations: int = 1,
-                       maximum_edge_length: float = 0.
+                       maximum_edge_length: float = 0,
+                       viewer: "napari.Viewer" = None
                        ) -> "napari.types.SurfaceData":
     """
     Make a mesh more detailed by adaptive subdivision.
 
     Each triangle is split into a set of new triangles based
     on a given maximum edge length or triangle area. If the 
     `maximum_edge_length` parameter is set to 0, then the 
@@ -365,28 +400,32 @@
     number_of_iterations:int
 
     See Also
     --------
     ..[0] https://vedo.embl.es/docs/vedo/mesh.html#Mesh.subdivide
     ..[1] https://vtk.org/doc/nightly/html/classvtkAdaptiveSubdivisionFilter.html
     """
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
+
     mesh_in = to_vedo_mesh(surface)
 
     if maximum_edge_length == 0:
         maximum_edge_length = mesh_in.diagonal_size(
         ) / np.sqrt(mesh_in._data.GetNumberOfPoints()) / number_of_iterations
 
     mesh_out = mesh_in.subdivide(
         number_of_iterations, method=2, mel=maximum_edge_length)
     return to_napari_surface_data(mesh_out)
 
 
 # @register_function(menu="Surfaces > Subdivide butterfly (vedo, nppas)")
 def _subdivide_butterfly(surface: "napari.types.SurfaceData",
-                         number_of_iterations: int = 1
+                         number_of_iterations: int = 1,
+                         viewer: "napari.Viewer" = None
                          ) -> "napari.types.SurfaceData":
     """
     Make a mesh more detailed by adaptive subdivision.
 
     Each triangle is split into a set of new triangles based
     on an 8-point butterfly scheme.
 
@@ -397,44 +436,52 @@
 
     See Also
     --------
     ..[0] https://vedo.embl.es/docs/vedo/mesh.html#Mesh.subdivide
     ..[1] https://vtk.org/doc/nightly/html/classvtkButterflySubdivisionFilter.html
     ..[2] Zorin et al. "Interpolating Subdivisions for Meshes with Arbitrary Topology," Computer Graphics Proceedings, Annual Conference Series, 1996, ACM SIGGRAPH, pp.189-192
     """
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
+
     mesh_in = to_vedo_mesh(surface)
     mesh_out = mesh_in.subdivide(number_of_iterations, method=3)
     return to_napari_surface_data(mesh_out)
 
 
 @register_function(menu="Surfaces > Subdivide centroid (vedo, nppas)")
 def subdivide_centroid(surface: "napari.types.SurfaceData",
-                         number_of_iterations: int = 1
+                         number_of_iterations: int = 1,
+                         viewer: "napari.Viewer" = None
                          ) -> "napari.types.SurfaceData":
     """
     Make a mesh more detailed by centroid-based subdivision.
 
     Parameters
     ----------
     surface:napari.types.SurfaceData
     number_of_iterations:int, optional
 
     See Also
     --------
     ..[0] https://vedo.embl.es/docs/vedo/mesh.html#Mesh.subdivide
     """
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
+
     mesh_in = to_vedo_mesh(surface)
     mesh_out = mesh_in.subdivide(number_of_iterations, method=4)
     return to_napari_surface_data(mesh_out)
 
 
 @register_function(menu="Surfaces > Decimate surface (quadric, vedo, nppas)")
 def decimate_quadric(surface: "napari.types.SurfaceData",
                      fraction: float = 0.5,
-                     number_of_vertices: int = None
+                     number_of_vertices: int = None,
+                     viewer: "napari.Viewer" = None
                     ) -> "napari.types.SurfaceData":
     """
     Reduce numbers of vertices of a surface to a given fraction.
 
     Parameters
     ----------
     surface:napari.types.SurfaceData
@@ -447,23 +494,27 @@
     -------
     SurfaceData
 
     See Also
     --------
     ..[0] https://vedo.embl.es/autodocs/content/vedo/vedo/mesh.html#Mesh.decimate
     """
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
+
     mesh_in = to_vedo_mesh(surface)
     mesh_out = mesh_in.decimate(method='quadric', fraction=fraction, n=number_of_vertices)
     return to_napari_surface_data(mesh_out)
 
 
 @register_function(menu="Surfaces > Decimate surface (pro, vedo, nppas)")
 def decimate_pro(surface: "napari.types.SurfaceData",
                      fraction: float = 0.5,
-                     number_of_vertices: int = None
+                     number_of_vertices: int = None,
+                     viewer: "napari.Viewer" = None
                     ) -> "napari.types.SurfaceData":
     """
     Reduce numbers of vertices of a surface to a given fraction.
 
     Parameters
     ----------
     surface:napari.types.SurfaceData
@@ -476,71 +527,79 @@
     -------
     SurfaceData
 
     See Also
     --------
     ..[0] https://vedo.embl.es/autodocs/content/vedo/vedo/mesh.html#Mesh.decimate
     """
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
+
     mesh_in = to_vedo_mesh(surface)
     mesh_out = mesh_in.decimate(method='pro', fraction=fraction, n=number_of_vertices)
     return to_napari_surface_data(mesh_out)
 
 
 @register_function(menu="Points > Create points from surface (vedo, nppas)")
-def sample_points_from_surface(surface: "napari.types.SurfaceData", distance_fraction: float = 0.01) -> "napari.types.PointsData":
+def sample_points_from_surface(surface: "napari.types.SurfaceData", distance_fraction: float = 0.01, viewer: "napari.Viewer" = None) -> "napari.types.PointsData":
     """Sample points from a surface
 
     Parameters
     ----------
     surface:napari.types.SurfaceData
     distance_fraction:float
         the smaller the distance, the more points
 
     See Also
     --------
     ..[0] https://vedo.embl.es/docs/vedo/pointcloud.html#Points.subsample
     """
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
 
     mesh_in = to_vedo_mesh(surface)
 
     point_cloud = mesh_in.subsample(fraction=distance_fraction)
 
     result = to_napari_points_data(point_cloud)
     return result
 
 
 @register_function(menu="Points > Subsample points (vedo, nppas)")
-def subsample_points(points_data: "napari.types.PointsData", distance_fraction: float = 0.01) -> "napari.types.PointsData":
+def subsample_points(points_data: "napari.types.PointsData", distance_fraction: float = 0.01, viewer: "napari.Viewer" = None) -> "napari.types.PointsData":
     """Subsample points
 
     Parameters
     ----------
     points_data:napari.types.PointsData
     distance_fraction:float
         the smaller the distance, the more points
 
     See Also
     --------
     ..[0] https://vedo.embl.es/docs/vedo/pointcloud.html#Points.subsample
     """
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
 
     mesh_in = to_vedo_points(points_data)
 
     point_cloud = mesh_in.subsample(fraction=distance_fraction)
 
     result = to_napari_points_data(point_cloud)
     return result
 
 
 @register_function(menu="Surfaces > Create surface from pointcloud (flying edges, vedo, nppas)")
 def reconstruct_surface_from_pointcloud(point_cloud: "napari.types.PointsData",
                                         number_of_sampling_voxels: int = 100,
                                         point_influence_radius: float = 0.1,
                                         padding: float = 0.05,
-                                        fill_holes: bool = True) -> "napari.types.SurfaceData":
+                                        fill_holes: bool = True,
+                                        viewer: "napari.Viewer" = None) -> "napari.types.SurfaceData":
     """Reconstruct a surface from a point cloud.
 
     Parameters
     ----------
     point_cloud:napari.types.PointsData
     number_of_sampling_voxels: int, optional
         number of voxels in each direction to sample the surface
@@ -548,20 +607,22 @@
     point_influence_radius: float, optional
         radius of influence of each point.
         Smaller values generally improve performance markedly.
     padding: float, optional
         increase by this fraction the bounding box
     fill_holes: bool, optional
         fill holes in the surface
-    
 
     See Also
     --------
     ..[0] https://vedo.embl.es/docs/vedo/pointcloud.html#Points.reconstruct_surface
     """
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
+
     point_cloud = to_vedo_points(point_cloud)
     mesh_out = point_cloud.reconstruct_surface(
         dims=(number_of_sampling_voxels) * 3,
         radius=point_influence_radius,
         padding=padding,
         hole_filling=fill_holes)
 
@@ -571,48 +632,54 @@
                          " parameters. Try to increase the number of " +
                          "sampling voxels or the point influence radius.")
 
     return mesh_out
 
 
 @register_function(menu="Surfaces > Convex hull of points (vedo, nppas)")
-def create_convex_hull_from_points(points_data: "napari.types.PointsData") -> "napari.types.SurfaceData":
+def create_convex_hull_from_points(points_data: "napari.types.PointsData",
+                                   viewer: "napari.Viewer" = None) -> "napari.types.SurfaceData":
     """Determine the convex hull surface of a list of points
 
     Parameters
     ----------
     points_data:napari.types.PointsData
 
     See Also
     --------
     ..[0] https://vedo.embl.es/autodocs/content/vedo/shapes.html#vedo.shapes.ConvexHull
     """
     import vedo
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
 
     point_cloud = to_vedo_points(points_data)
     mesh_out = vedo.shapes.ConvexHull(point_cloud)
 
     return to_napari_surface_data(mesh_out)
 
 
 @register_function(menu="Surfaces > Fill holes (vedo, nppas)")
-def fill_holes_in_surface(surface: "napari.types.SurfaceData", size_limit: float = 100) -> "napari.types.SurfaceData":
+def fill_holes_in_surface(surface: "napari.types.SurfaceData", size_limit: float = 100, viewer: "napari.Viewer" = None) -> "napari.types.SurfaceData":
     """
     Fill holes in a surface up to a specified size.
 
     Parameters
     ----------
     surface : napari.layers.Surface
     size_limit : float, optional
         Size limit to hole-filling. The default is 100.
 
     See also
     --------
     ..[0] https://vedo.embl.es/docs/vedo/mesh.html#Mesh.fillHoles
     """
+    from ._utils import _init_viewer
+    _init_viewer(viewer)
+
     mesh = to_vedo_mesh((surface[0], surface[1]))
     mesh.fill_holes(size=size_limit)
 
     return to_napari_surface_data(mesh)
 
 
 def show(surface, zoom: float = 1, azimuth: float = 0, elevation: float = 0, cmap:str = 'viridis'):
```

#### html2text {}

```diff
@@ -57,205 +57,229 @@
 ", ] return "\n".join(all) def to_napari_surface_data(vedo_mesh, values=None):
 if values is None: return SurfaceTuple((vedo_mesh.points(), np.asarray
 (vedo_mesh.faces()))) else: return SurfaceTuple((vedo_mesh.points(), np.asarray
 (vedo_mesh.faces()), values)) def to_napari_points_data(vedo_points): return
 vedo_points.points() def _hide_vtk_warnings(): from vtkmodules.vtkCommonCore
 import vtkObject vtkObject.GlobalWarningDisplayOff() @register_function
 (menu="Surfaces > Convex hull (vedo, nppas)") def
-create_convex_hull_from_surface(surface: "napari.types.SurfaceData") -
-> "napari.types.SurfaceData": """Determine the convex hull of a surface
-Parameters ---------- surface:napari.types.SurfaceData See Also -------- ..[0]
-https://vedo.embl.es/autodocs/content/vedo/shapes.html#vedo.shapes.ConvexHull
-""" mesh = to_vedo_mesh(surface) import vedo convex_hull_mesh =
-vedo.shapes.ConvexHull(mesh) return to_napari_surface_data(convex_hull_mesh)
+create_convex_hull_from_surface(surface: "napari.types.SurfaceData", viewer:
+"napari.Viewer" = None) -> "napari.types.SurfaceData": """Determine the convex
+hull of a surface Parameters ---------- surface:napari.types.SurfaceData viewer
+: napari.Viewer, optional makes light follow the camera in the given viewer See
+Also -------- ..[0] https://vedo.embl.es/autodocs/content/vedo/
+shapes.html#vedo.shapes.ConvexHull """ from ._utils import _init_viewer
+_init_viewer(viewer) mesh = to_vedo_mesh(surface) import vedo convex_hull_mesh
+= vedo.shapes.ConvexHull(mesh) return to_napari_surface_data(convex_hull_mesh)
 @register_function(menu="Surfaces > Remove duplicate vertices (vedo, nppas)")
-def remove_duplicate_vertices(surface: "napari.types.SurfaceData") -
-> "napari.types.SurfaceData": """ Clean a surface mesh (i.e., remove duplicate
-faces & vertices). See Also -------- ..[0] https://vedo.embl.es/docs/vedo/
-pointcloud.html#Points.clean """ mesh = to_vedo_mesh(surface) clean_mesh =
+def remove_duplicate_vertices(surface: "napari.types.SurfaceData", viewer:
+"napari.Viewer" = None) -> "napari.types.SurfaceData": """ Clean a surface mesh
+(i.e., remove duplicate faces & vertices). See Also -------- ..[0] https://
+vedo.embl.es/docs/vedo/pointcloud.html#Points.clean """ from ._utils import
+_init_viewer _init_viewer(viewer) mesh = to_vedo_mesh(surface) clean_mesh =
 mesh.clean() return to_napari_surface_data(clean_mesh) @register_function
 (menu="Surfaces > Connected components labeling (vedo, nppas)") def
-connected_component_labeling(surface: "napari.types.SurfaceData") -
-> "napari.types.SurfaceData": """ Determine the connected components of a
-surface mesh. See Also -------- ..[0] https://vedo.embl.es/docs/vedo/
-mesh.html#Mesh.compute_connectivity """ from ._quantification import
-set_vertex_values mesh = to_vedo_mesh(surface) mesh.compute_connectivity()
+connected_component_labeling(surface: "napari.types.SurfaceData", viewer:
+"napari.Viewer" = None) -> "napari.types.SurfaceData": """ Determine the
+connected components of a surface mesh. See Also -------- ..[0] https://
+vedo.embl.es/docs/vedo/mesh.html#Mesh.compute_connectivity """ from
+._quantification import set_vertex_values from ._utils import _init_viewer
+_init_viewer(viewer) mesh = to_vedo_mesh(surface) mesh.compute_connectivity()
 region_id = mesh.pointdata["RegionId"] mesh_out = to_napari_surface_data(mesh)
 mesh_out = set_vertex_values(mesh_out, region_id) return mesh_out
 @register_function(menu="Surfaces > Smooth (moving least squares, vedo,
 nppas)") def smooth_surface_moving_least_squares_2d(surface:
-"napari.types.SurfaceData", smoothing_factor: float = 0.2) -
-> "napari.types.SurfaceData": """Apply a moving least squares approach to
-smooth a surface See Also -------- ..[0] https://vedo.embl.es/autodocs/content/
-vedo/vedo/pointcloud.html#Points.smooth_mls_2d """ mesh = to_vedo_mesh(surface)
-smooth_mesh = mesh.smooth_mls_2d(f=smoothing_factor) return
+"napari.types.SurfaceData", smoothing_factor: float = 0.2, viewer:
+"napari.Viewer" = None) -> "napari.types.SurfaceData": """Apply a moving least
+squares approach to smooth a surface See Also -------- ..[0] https://
+vedo.embl.es/autodocs/content/vedo/vedo/pointcloud.html#Points.smooth_mls_2d
+""" from ._utils import _init_viewer _init_viewer(viewer) mesh = to_vedo_mesh
+(surface) smooth_mesh = mesh.smooth_mls_2d(f=smoothing_factor) return
 to_napari_surface_data(smooth_mesh) @register_function(menu="Surfaces > Smooth
 (moving least squares with radius, vedo, nppas)") def
 smooth_surface_moving_least_squares_2d_radius(surface:
-"napari.types.SurfaceData", smoothing_factor: float = 0.2, radius: float = 0.2)
--> "napari.types.SurfaceData": """Apply a moving least squares approach to
-smooth a surface. The radius is used to determine the number of points to use
-for the smoothing. See Also -------- ..[0] https://vedo.embl.es/autodocs/
-content/vedo/vedo/pointcloud.html#Points.smooth_mls_2d """ mesh = to_vedo_mesh
-(surface) smooth_mesh = mesh.smooth_mls_2d(f=smoothing_factor, radius=radius)
-return to_napari_surface_data(smooth_mesh) @register_function(menu="Points >
-Smooth (moving least squares, vedo, nppas)") def
+"napari.types.SurfaceData", smoothing_factor: float = 0.2, radius: float = 0.2,
+viewer: "napari.Viewer" = None) -> "napari.types.SurfaceData": """Apply a
+moving least squares approach to smooth a surface. The radius is used to
+determine the number of points to use for the smoothing. See Also -------- ..
+[0] https://vedo.embl.es/autodocs/content/vedo/vedo/
+pointcloud.html#Points.smooth_mls_2d """ from ._utils import _init_viewer
+_init_viewer(viewer) mesh = to_vedo_mesh(surface) smooth_mesh =
+mesh.smooth_mls_2d(f=smoothing_factor, radius=radius) return
+to_napari_surface_data(smooth_mesh) @register_function(menu="Points > Smooth
+(moving least squares, vedo, nppas)") def
 smooth_pointcloud_moving_least_squares_2d(pointcloud:
-"napari.types.PointsData", smoothing_factor: float = 0.2) -
-> "napari.types.PointsData": """Apply a moving least squares approach to smooth
-a point cloud. See Also -------- ..[0] https://vedo.embl.es/autodocs/content/
-vedo/vedo/pointcloud.html#Points.smooth_mls_2d """ points = to_vedo_points
-(pointcloud) smooth_points = points.smooth_mls_2d(f=smoothing_factor) return
-to_napari_points_data(smooth_points) @register_function(menu="Points > Smooth
-(moving least squares radius, vedo, nppas)") def
-smooth_pointcloud_moving_least_squares_2d_radius(pointcloud:
-"napari.types.PointsData", smoothing_factor: float = 0.2, radius=2) -
-> "napari.types.PointsData": """Apply a moving least squares approach to smooth
-a point cloud. The radius is used to determine the number of points to use for
-the smoothing. See Also -------- ..[0] https://vedo.embl.es/autodocs/content/
-vedo/vedo/pointcloud.html#Points.smooth_mls_2d """ points = to_vedo_points
-(pointcloud) smooth_points = points.smooth_mls_2d(f=smoothing_factor,
-radius=radius) return to_napari_points_data(smooth_points) @register_function
-(menu="Surfaces > Smooth (Windowed Sinc, vedo, nppas)") def smooth_surface
-(surface: "napari.types.SurfaceData", number_of_iterations: int = 15,
-pass_band: float = 0.1, edge_angle: float = 15, feature_angle: float = 60,
-boundary: bool = False ) -> "napari.types.SurfaceData": """Smooth a surface
-using a Windowed Sinc kernel. See Also -------- ..[0] https://vedo.embl.es/
-docs/vedo/mesh.html#Mesh.smooth """ mesh = to_vedo_mesh(surface) smooth_mesh =
-mesh.smooth(niter=number_of_iterations, pass_band=pass_band,
-edge_angle=edge_angle, feature_angle=feature_angle, boundary=boundary) return
-to_napari_surface_data(smooth_mesh) #@register_function(menu="Surfaces >
-Subdivide loop (vedo, nppas)") def _subdivide_loop_vedo(surface:
-"napari.types.SurfaceData", number_of_iterations: int = 1 ) -
-> "napari.types.SurfaceData": """ Make a mesh more detailed by subdividing in a
-loop. This increases the number of faces on the surface simply by subdividing
-each triangle into four new triangles. Parameters ---------- surface:
-napari.types.SurfaceData number_of_iterations:int See Also -------- ..[0]
-https://vedo.embl.es/docs/vedo/mesh.html#Mesh.subdivide ..[1] https://vtk.org/
-doc/nightly/html/classvtkLoopSubdivisionFilter.html """ mesh_in = to_vedo_mesh
-(surface) mesh_out = mesh_in.subdivide(number_of_iterations, method=0) return
-to_napari_surface_data(mesh_out) #@register_function(menu="Surfaces > Subdivide
-linear (vedo, nppas)") def _subdivide_linear(surface:
-"napari.types.SurfaceData", number_of_iterations: int = 1 ) -
+"napari.types.PointsData", smoothing_factor: float = 0.2, viewer:
+"napari.Viewer" = None) -> "napari.types.PointsData": """Apply a moving least
+squares approach to smooth a point cloud. See Also -------- ..[0] https://
+vedo.embl.es/autodocs/content/vedo/vedo/pointcloud.html#Points.smooth_mls_2d
+""" from ._utils import _init_viewer _init_viewer(viewer) points =
+to_vedo_points(pointcloud) smooth_points = points.smooth_mls_2d
+(f=smoothing_factor) return to_napari_points_data(smooth_points)
+@register_function(menu="Points > Smooth (moving least squares radius, vedo,
+nppas)") def smooth_pointcloud_moving_least_squares_2d_radius(pointcloud:
+"napari.types.PointsData", smoothing_factor: float = 0.2, radius: float = 2,
+viewer: "napari.Viewer" = None) -> "napari.types.PointsData": """Apply a moving
+least squares approach to smooth a point cloud. The radius is used to determine
+the number of points to use for the smoothing. See Also -------- ..[0] https://
+vedo.embl.es/autodocs/content/vedo/vedo/pointcloud.html#Points.smooth_mls_2d
+""" from ._utils import _init_viewer _init_viewer(viewer) points =
+to_vedo_points(pointcloud) smooth_points = points.smooth_mls_2d
+(f=smoothing_factor, radius=radius) return to_napari_points_data(smooth_points)
+@register_function(menu="Surfaces > Smooth (Windowed Sinc, vedo, nppas)") def
+smooth_surface(surface: "napari.types.SurfaceData", number_of_iterations: int =
+15, pass_band: float = 0.1, edge_angle: float = 15, feature_angle: float = 60,
+boundary: bool = False, viewer: "napari.Viewer" = None ) -
+> "napari.types.SurfaceData": """Smooth a surface using a Windowed Sinc kernel.
+See Also -------- ..[0] https://vedo.embl.es/docs/vedo/mesh.html#Mesh.smooth
+""" from ._utils import _init_viewer _init_viewer(viewer) mesh = to_vedo_mesh
+(surface) smooth_mesh = mesh.smooth(niter=number_of_iterations,
+pass_band=pass_band, edge_angle=edge_angle, feature_angle=feature_angle,
+boundary=boundary) return to_napari_surface_data(smooth_mesh)
+#@register_function(menu="Surfaces > Subdivide loop (vedo, nppas)") def
+_subdivide_loop_vedo(surface: "napari.types.SurfaceData", number_of_iterations:
+int = 1, viewer: "napari.Viewer" = None ) -> "napari.types.SurfaceData": """
+Make a mesh more detailed by subdividing in a loop. This increases the number
+of faces on the surface simply by subdividing each triangle into four new
+triangles. Parameters ---------- surface:napari.types.SurfaceData
+number_of_iterations:int See Also -------- ..[0] https://vedo.embl.es/docs/
+vedo/mesh.html#Mesh.subdivide ..[1] https://vtk.org/doc/nightly/html/
+classvtkLoopSubdivisionFilter.html """ from ._utils import _init_viewer
+_init_viewer(viewer) mesh_in = to_vedo_mesh(surface) mesh_out =
+mesh_in.subdivide(number_of_iterations, method=0) return to_napari_surface_data
+(mesh_out) #@register_function(menu="Surfaces > Subdivide linear (vedo,
+nppas)") def _subdivide_linear(surface: "napari.types.SurfaceData",
+number_of_iterations: int = 1, viewer: "napari.Viewer" = None ) -
 > "napari.types.SurfaceData": """ Make a mesh more detailed by linear
 subdivision. The position of the created triangles is determined by a linear
 interpolation method and is thus slower than the loop subdivision algorithm.
 Parameters ---------- surface:napari.types.SurfaceData number_of_iterations:int
 See Also -------- ..[0] https://vedo.embl.es/docs/vedo/mesh.html#Mesh.subdivide
 ..[1] https://vtk.org/doc/nightly/html/classvtkLinearSubdivisionFilter.html """
-mesh_in = to_vedo_mesh(surface) mesh_out = mesh_in.subdivide
-(number_of_iterations, method=1) return to_napari_surface_data(mesh_out)
-@register_function(menu="Surfaces > Subdivide adaptive (vedo, nppas)") def
-subdivide_adaptive(surface: "napari.types.SurfaceData", number_of_iterations:
-int = 1, maximum_edge_length: float = 0. ) -> "napari.types.SurfaceData": """
+from ._utils import _init_viewer _init_viewer(viewer) mesh_in = to_vedo_mesh
+(surface) mesh_out = mesh_in.subdivide(number_of_iterations, method=1) return
+to_napari_surface_data(mesh_out) @register_function(menu="Surfaces > Subdivide
+adaptive (vedo, nppas)") def subdivide_adaptive(surface:
+"napari.types.SurfaceData", number_of_iterations: int = 1, maximum_edge_length:
+float = 0, viewer: "napari.Viewer" = None ) -> "napari.types.SurfaceData": """
 Make a mesh more detailed by adaptive subdivision. Each triangle is split into
 a set of new triangles based on a given maximum edge length or triangle area.
 If the `maximum_edge_length` parameter is set to 0, then the parameter will be
 estimated automatically. Parameters ---------- surface:napari.types.SurfaceData
 number_of_iterations:int See Also -------- ..[0] https://vedo.embl.es/docs/
 vedo/mesh.html#Mesh.subdivide ..[1] https://vtk.org/doc/nightly/html/
-classvtkAdaptiveSubdivisionFilter.html """ mesh_in = to_vedo_mesh(surface) if
-maximum_edge_length == 0: maximum_edge_length = mesh_in.diagonal_size( ) /
-np.sqrt(mesh_in._data.GetNumberOfPoints()) / number_of_iterations mesh_out =
+classvtkAdaptiveSubdivisionFilter.html """ from ._utils import _init_viewer
+_init_viewer(viewer) mesh_in = to_vedo_mesh(surface) if maximum_edge_length ==
+0: maximum_edge_length = mesh_in.diagonal_size( ) / np.sqrt
+(mesh_in._data.GetNumberOfPoints()) / number_of_iterations mesh_out =
 mesh_in.subdivide( number_of_iterations, method=2, mel=maximum_edge_length)
 return to_napari_surface_data(mesh_out) # @register_function(menu="Surfaces >
 Subdivide butterfly (vedo, nppas)") def _subdivide_butterfly(surface:
-"napari.types.SurfaceData", number_of_iterations: int = 1 ) -
-> "napari.types.SurfaceData": """ Make a mesh more detailed by adaptive
-subdivision. Each triangle is split into a set of new triangles based on an 8-
-point butterfly scheme. Parameters ---------- surface:napari.types.SurfaceData
-number_of_iterations:int See Also -------- ..[0] https://vedo.embl.es/docs/
-vedo/mesh.html#Mesh.subdivide ..[1] https://vtk.org/doc/nightly/html/
-classvtkButterflySubdivisionFilter.html ..[2] Zorin et al. "Interpolating
-Subdivisions for Meshes with Arbitrary Topology," Computer Graphics
-Proceedings, Annual Conference Series, 1996, ACM SIGGRAPH, pp.189-192 """
-mesh_in = to_vedo_mesh(surface) mesh_out = mesh_in.subdivide
-(number_of_iterations, method=3) return to_napari_surface_data(mesh_out)
-@register_function(menu="Surfaces > Subdivide centroid (vedo, nppas)") def
-subdivide_centroid(surface: "napari.types.SurfaceData", number_of_iterations:
-int = 1 ) -> "napari.types.SurfaceData": """ Make a mesh more detailed by
-centroid-based subdivision. Parameters ---------- surface:
-napari.types.SurfaceData number_of_iterations:int, optional See Also -------
-- ..[0] https://vedo.embl.es/docs/vedo/mesh.html#Mesh.subdivide """ mesh_in =
+"napari.types.SurfaceData", number_of_iterations: int = 1, viewer:
+"napari.Viewer" = None ) -> "napari.types.SurfaceData": """ Make a mesh more
+detailed by adaptive subdivision. Each triangle is split into a set of new
+triangles based on an 8-point butterfly scheme. Parameters ---------- surface:
+napari.types.SurfaceData number_of_iterations:int See Also -------- ..[0]
+https://vedo.embl.es/docs/vedo/mesh.html#Mesh.subdivide ..[1] https://vtk.org/
+doc/nightly/html/classvtkButterflySubdivisionFilter.html ..[2] Zorin et al.
+"Interpolating Subdivisions for Meshes with Arbitrary Topology," Computer
+Graphics Proceedings, Annual Conference Series, 1996, ACM SIGGRAPH, pp.189-192
+""" from ._utils import _init_viewer _init_viewer(viewer) mesh_in =
 to_vedo_mesh(surface) mesh_out = mesh_in.subdivide(number_of_iterations,
-method=4) return to_napari_surface_data(mesh_out) @register_function
-(menu="Surfaces > Decimate surface (quadric, vedo, nppas)") def
-decimate_quadric(surface: "napari.types.SurfaceData", fraction: float = 0.5,
-number_of_vertices: int = None ) -> "napari.types.SurfaceData": """ Reduce
-numbers of vertices of a surface to a given fraction. Parameters ---------
-- surface:napari.types.SurfaceData fraction: float, optional reduce the number
-of vertices in the surface to the given fraction (0...1, default 0.5)
+method=3) return to_napari_surface_data(mesh_out) @register_function
+(menu="Surfaces > Subdivide centroid (vedo, nppas)") def subdivide_centroid
+(surface: "napari.types.SurfaceData", number_of_iterations: int = 1, viewer:
+"napari.Viewer" = None ) -> "napari.types.SurfaceData": """ Make a mesh more
+detailed by centroid-based subdivision. Parameters ---------- surface:
+napari.types.SurfaceData number_of_iterations:int, optional See Also -------
+- ..[0] https://vedo.embl.es/docs/vedo/mesh.html#Mesh.subdivide """ from
+._utils import _init_viewer _init_viewer(viewer) mesh_in = to_vedo_mesh
+(surface) mesh_out = mesh_in.subdivide(number_of_iterations, method=4) return
+to_napari_surface_data(mesh_out) @register_function(menu="Surfaces > Decimate
+surface (quadric, vedo, nppas)") def decimate_quadric(surface:
+"napari.types.SurfaceData", fraction: float = 0.5, number_of_vertices: int =
+None, viewer: "napari.Viewer" = None ) -> "napari.types.SurfaceData": """
+Reduce numbers of vertices of a surface to a given fraction. Parameters -------
+--- surface:napari.types.SurfaceData fraction: float, optional reduce the
+number of vertices in the surface to the given fraction (0...1, default 0.5)
 number_of_vertices:int, optional overwrites fraction in case specified Returns
 ------- SurfaceData See Also -------- ..[0] https://vedo.embl.es/autodocs/
-content/vedo/vedo/mesh.html#Mesh.decimate """ mesh_in = to_vedo_mesh(surface)
-mesh_out = mesh_in.decimate(method='quadric', fraction=fraction,
-n=number_of_vertices) return to_napari_surface_data(mesh_out)
-@register_function(menu="Surfaces > Decimate surface (pro, vedo, nppas)") def
-decimate_pro(surface: "napari.types.SurfaceData", fraction: float = 0.5,
-number_of_vertices: int = None ) -> "napari.types.SurfaceData": """ Reduce
-numbers of vertices of a surface to a given fraction. Parameters ---------
-- surface:napari.types.SurfaceData fraction: float, optional reduce the number
-of vertices in the surface to the given fraction (0...1, default 0.5)
+content/vedo/vedo/mesh.html#Mesh.decimate """ from ._utils import _init_viewer
+_init_viewer(viewer) mesh_in = to_vedo_mesh(surface) mesh_out =
+mesh_in.decimate(method='quadric', fraction=fraction, n=number_of_vertices)
+return to_napari_surface_data(mesh_out) @register_function(menu="Surfaces >
+Decimate surface (pro, vedo, nppas)") def decimate_pro(surface:
+"napari.types.SurfaceData", fraction: float = 0.5, number_of_vertices: int =
+None, viewer: "napari.Viewer" = None ) -> "napari.types.SurfaceData": """
+Reduce numbers of vertices of a surface to a given fraction. Parameters -------
+--- surface:napari.types.SurfaceData fraction: float, optional reduce the
+number of vertices in the surface to the given fraction (0...1, default 0.5)
 number_of_vertices:int, optional overwrites fraction in case specified Returns
 ------- SurfaceData See Also -------- ..[0] https://vedo.embl.es/autodocs/
-content/vedo/vedo/mesh.html#Mesh.decimate """ mesh_in = to_vedo_mesh(surface)
-mesh_out = mesh_in.decimate(method='pro', fraction=fraction,
-n=number_of_vertices) return to_napari_surface_data(mesh_out)
-@register_function(menu="Points > Create points from surface (vedo, nppas)")
-def sample_points_from_surface(surface: "napari.types.SurfaceData",
-distance_fraction: float = 0.01) -> "napari.types.PointsData": """Sample points
-from a surface Parameters ---------- surface:napari.types.SurfaceData
+content/vedo/vedo/mesh.html#Mesh.decimate """ from ._utils import _init_viewer
+_init_viewer(viewer) mesh_in = to_vedo_mesh(surface) mesh_out =
+mesh_in.decimate(method='pro', fraction=fraction, n=number_of_vertices) return
+to_napari_surface_data(mesh_out) @register_function(menu="Points > Create
+points from surface (vedo, nppas)") def sample_points_from_surface(surface:
+"napari.types.SurfaceData", distance_fraction: float = 0.01, viewer:
+"napari.Viewer" = None) -> "napari.types.PointsData": """Sample points from a
+surface Parameters ---------- surface:napari.types.SurfaceData
 distance_fraction:float the smaller the distance, the more points See Also ----
 ---- ..[0] https://vedo.embl.es/docs/vedo/pointcloud.html#Points.subsample """
-mesh_in = to_vedo_mesh(surface) point_cloud = mesh_in.subsample
-(fraction=distance_fraction) result = to_napari_points_data(point_cloud) return
-result @register_function(menu="Points > Subsample points (vedo, nppas)") def
-subsample_points(points_data: "napari.types.PointsData", distance_fraction:
-float = 0.01) -> "napari.types.PointsData": """Subsample points Parameters ----
------- points_data:napari.types.PointsData distance_fraction:float the smaller
-the distance, the more points See Also -------- ..[0] https://vedo.embl.es/
-docs/vedo/pointcloud.html#Points.subsample """ mesh_in = to_vedo_points
+from ._utils import _init_viewer _init_viewer(viewer) mesh_in = to_vedo_mesh
+(surface) point_cloud = mesh_in.subsample(fraction=distance_fraction) result =
+to_napari_points_data(point_cloud) return result @register_function
+(menu="Points > Subsample points (vedo, nppas)") def subsample_points
+(points_data: "napari.types.PointsData", distance_fraction: float = 0.01,
+viewer: "napari.Viewer" = None) -> "napari.types.PointsData": """Subsample
+points Parameters ---------- points_data:napari.types.PointsData
+distance_fraction:float the smaller the distance, the more points See Also ----
+---- ..[0] https://vedo.embl.es/docs/vedo/pointcloud.html#Points.subsample """
+from ._utils import _init_viewer _init_viewer(viewer) mesh_in = to_vedo_points
 (points_data) point_cloud = mesh_in.subsample(fraction=distance_fraction)
 result = to_napari_points_data(point_cloud) return result @register_function
 (menu="Surfaces > Create surface from pointcloud (flying edges, vedo, nppas)")
 def reconstruct_surface_from_pointcloud(point_cloud: "napari.types.PointsData",
 number_of_sampling_voxels: int = 100, point_influence_radius: float = 0.1,
-padding: float = 0.05, fill_holes: bool = True) -> "napari.types.SurfaceData":
-"""Reconstruct a surface from a point cloud. Parameters ---------- point_cloud:
-napari.types.PointsData number_of_sampling_voxels: int, optional number of
-voxels in each direction to sample the surface Can be used to control
-reconstruction precision. point_influence_radius: float, optional radius of
-influence of each point. Smaller values generally improve performance markedly.
-padding: float, optional increase by this fraction the bounding box fill_holes:
-bool, optional fill holes in the surface See Also -------- ..[0] https://
-vedo.embl.es/docs/vedo/pointcloud.html#Points.reconstruct_surface """
-point_cloud = to_vedo_points(point_cloud) mesh_out =
+padding: float = 0.05, fill_holes: bool = True, viewer: "napari.Viewer" = None)
+-> "napari.types.SurfaceData": """Reconstruct a surface from a point cloud.
+Parameters ---------- point_cloud:napari.types.PointsData
+number_of_sampling_voxels: int, optional number of voxels in each direction to
+sample the surface Can be used to control reconstruction precision.
+point_influence_radius: float, optional radius of influence of each point.
+Smaller values generally improve performance markedly. padding: float, optional
+increase by this fraction the bounding box fill_holes: bool, optional fill
+holes in the surface See Also -------- ..[0] https://vedo.embl.es/docs/vedo/
+pointcloud.html#Points.reconstruct_surface """ from ._utils import _init_viewer
+_init_viewer(viewer) point_cloud = to_vedo_points(point_cloud) mesh_out =
 point_cloud.reconstruct_surface( dims=(number_of_sampling_voxels) * 3,
 radius=point_influence_radius, padding=padding, hole_filling=fill_holes)
 mesh_out = to_napari_surface_data(mesh_out) if len(mesh_out[1]) == 0: raise
 ValueError("No surface could be reconstructed with the given" + " parameters.
 Try to increase the number of " + "sampling voxels or the point influence
 radius.") return mesh_out @register_function(menu="Surfaces > Convex hull of
 points (vedo, nppas)") def create_convex_hull_from_points(points_data:
-"napari.types.PointsData") -> "napari.types.SurfaceData": """Determine the
-convex hull surface of a list of points Parameters ---------- points_data:
-napari.types.PointsData See Also -------- ..[0] https://vedo.embl.es/autodocs/
-content/vedo/shapes.html#vedo.shapes.ConvexHull """ import vedo point_cloud =
-to_vedo_points(points_data) mesh_out = vedo.shapes.ConvexHull(point_cloud)
-return to_napari_surface_data(mesh_out) @register_function(menu="Surfaces >
-Fill holes (vedo, nppas)") def fill_holes_in_surface(surface:
-"napari.types.SurfaceData", size_limit: float = 100) -
-> "napari.types.SurfaceData": """ Fill holes in a surface up to a specified
-size. Parameters ---------- surface : napari.layers.Surface size_limit : float,
-optional Size limit to hole-filling. The default is 100. See also -------- ..
-[0] https://vedo.embl.es/docs/vedo/mesh.html#Mesh.fillHoles """ mesh =
-to_vedo_mesh((surface[0], surface[1])) mesh.fill_holes(size=size_limit) return
-to_napari_surface_data(mesh) def show(surface, zoom: float = 1, azimuth: float
-= 0, elevation: float = 0, cmap:str = 'viridis'): """ Visualizes a surface
-mesh, e.g. in Jupyter Notebooks. Parameters ---------- zoom: float, optional >
-1: Zoom in < 1: Zoom out azimuth: float, optional angle in degrees for turning
-the view direction elevation: float, optional angle in degrees for turning the
-view direction cmap: str, optional colormap for visualization of values See
-also -------- https://vedo.embl.es/autodocs/content/vedo/vedo/
-plotter.html#Plotter """ from vedo import Plotter mesh = to_vedo_mesh((surface
-[0], surface[1])) if len(surface) > 2: mesh.cmap(cmap, surface[2]) plt =
-Plotter() plt.show(mesh, zoom=zoom, azimuth=azimuth, elevation=elevation)
+"napari.types.PointsData", viewer: "napari.Viewer" = None) -
+> "napari.types.SurfaceData": """Determine the convex hull surface of a list of
+points Parameters ---------- points_data:napari.types.PointsData See Also -----
+--- ..[0] https://vedo.embl.es/autodocs/content/vedo/
+shapes.html#vedo.shapes.ConvexHull """ import vedo from ._utils import
+_init_viewer _init_viewer(viewer) point_cloud = to_vedo_points(points_data)
+mesh_out = vedo.shapes.ConvexHull(point_cloud) return to_napari_surface_data
+(mesh_out) @register_function(menu="Surfaces > Fill holes (vedo, nppas)") def
+fill_holes_in_surface(surface: "napari.types.SurfaceData", size_limit: float =
+100, viewer: "napari.Viewer" = None) -> "napari.types.SurfaceData": """ Fill
+holes in a surface up to a specified size. Parameters ---------- surface :
+napari.layers.Surface size_limit : float, optional Size limit to hole-filling.
+The default is 100. See also -------- ..[0] https://vedo.embl.es/docs/vedo/
+mesh.html#Mesh.fillHoles """ from ._utils import _init_viewer _init_viewer
+(viewer) mesh = to_vedo_mesh((surface[0], surface[1])) mesh.fill_holes
+(size=size_limit) return to_napari_surface_data(mesh) def show(surface, zoom:
+float = 1, azimuth: float = 0, elevation: float = 0, cmap:str = 'viridis'): """
+Visualizes a surface mesh, e.g. in Jupyter Notebooks. Parameters ---------
+- zoom: float, optional > 1: Zoom in < 1: Zoom out azimuth: float, optional
+angle in degrees for turning the view direction elevation: float, optional
+angle in degrees for turning the view direction cmap: str, optional colormap
+for visualization of values See also -------- https://vedo.embl.es/autodocs/
+content/vedo/vedo/plotter.html#Plotter """ from vedo import Plotter mesh =
+to_vedo_mesh((surface[0], surface[1])) if len(surface) > 2: mesh.cmap(cmap,
+surface[2]) plt = Plotter() plt.show(mesh, zoom=zoom, azimuth=azimuth,
+elevation=elevation)
```

### Comparing `napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/data/bun_zipper.ply` & `napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/data/bun_zipper.ply`

 * *Files identical despite different names*

### Comparing `napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/data/gastruloid.ply` & `napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/data/gastruloid.ply`

 * *Files identical despite different names*

### Comparing `napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/data/knot.ply` & `napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/data/knot.ply`

 * *Files identical despite different names*

### Comparing `napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces/data/knot_license.md` & `napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces/data/knot_license.md`

 * *Files identical despite different names*

### Comparing `napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces.egg-info/PKG-INFO` & `napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-process-points-and-surfaces
-Version: 0.4.2
+Version: 0.5.0
 Summary: Process and analyze surfaces using open3d and vedo in napari
 Home-page: https://github.com/haesleinhuepf/napari-process-points-and-surfaces
 Author: Robert Haase, Johannes Soltwedel
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/napari-process-points-and-surfaces/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/napari-process-points-and-surfaces#README.md
```

### Comparing `napari-process-points-and-surfaces-0.4.2/napari_process_points_and_surfaces.egg-info/SOURCES.txt` & `napari-process-points-and-surfaces-0.5.0/napari_process_points_and_surfaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-process-points-and-surfaces-0.4.2/setup.cfg` & `napari-process-points-and-surfaces-0.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6170 6172 692d 7072 6f63 6573   = napari-proces
 00000020: 732d 706f 696e 7473 2d61 6e64 2d73 7572  s-points-and-sur
 00000030: 6661 6365 730d 0a76 6572 7369 6f6e 203d  faces..version =
-00000040: 2030 2e34 2e32 0d0a 6175 7468 6f72 203d   0.4.2..author =
+00000040: 2030 2e35 2e30 0d0a 6175 7468 6f72 203d   0.5.0..author =
 00000050: 2052 6f62 6572 7420 4861 6173 652c 204a   Robert Haase, J
 00000060: 6f68 616e 6e65 7320 536f 6c74 7765 6465  ohannes Soltwede
 00000070: 6c0d 0a61 7574 686f 725f 656d 6169 6c20  l..author_email 
 00000080: 3d20 726f 6265 7274 2e68 6161 7365 4074  = robert.haase@t
 00000090: 752d 6472 6573 6465 6e2e 6465 0d0a 7572  u-dresden.de..ur
 000000a0: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 000000b0: 7562 2e63 6f6d 2f68 6165 736c 6569 6e68  ub.com/haesleinh
```

