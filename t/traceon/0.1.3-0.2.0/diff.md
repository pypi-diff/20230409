# Comparing `tmp/traceon-0.1.3.tar.gz` & `tmp/traceon-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traceon-0.1.3.tar", last modified: Mon Mar 27 08:41:11 2023, max compression
+gzip compressed data, was "traceon-0.2.0.tar", last modified: Sun Apr  9 21:05:32 2023, max compression
```

## Comparing `traceon-0.1.3.tar` & `traceon-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-03-27 08:41:11.539927 traceon-0.1.3/
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)    34524 2023-03-21 09:42:58.000000 traceon-0.1.3/LICENSE.txt
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)       27 2023-03-21 10:12:12.000000 traceon-0.1.3/MANIFEST.in
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     3313 2023-03-27 08:41:11.539927 traceon-0.1.3/PKG-INFO
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     2223 2023-03-23 15:56:28.000000 traceon-0.1.3/README.md
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)       38 2023-03-27 08:41:11.539927 traceon-0.1.3/setup.cfg
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     1435 2023-03-27 08:40:23.000000 traceon-0.1.3/setup.py
-drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-03-27 08:41:11.531927 traceon-0.1.3/traceon/
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     2752 2023-03-21 09:42:58.000000 traceon-0.1.3/traceon/__init__.py
-drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-03-27 08:41:11.535927 traceon-0.1.3/traceon/backend/
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)    15501 2023-03-22 16:16:27.000000 traceon-0.1.3/traceon/backend/__init__.py
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)    31964 2023-03-22 16:23:54.000000 traceon-0.1.3/traceon/backend/traceon-backend.c
-drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-03-27 08:41:11.539927 traceon-0.1.3/traceon/data/
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)  1023104 2023-03-21 09:42:58.000000 traceon-0.1.3/traceon/data/radial-series-3D-theta-dependent-coefficients.npy
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     8128 2023-03-21 09:42:58.000000 traceon-0.1.3/traceon/data/radial-series-3D-thetas.npy
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     7718 2023-03-21 09:42:58.000000 traceon-0.1.3/traceon/excitation.py
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)    13563 2023-03-23 10:28:01.000000 traceon-0.1.3/traceon/geometry.py
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     7611 2023-03-27 06:56:38.000000 traceon-0.1.3/traceon/plotting.py
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)    24908 2023-03-21 15:40:27.000000 traceon-0.1.3/traceon/solver.py
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     8192 2023-03-21 09:42:58.000000 traceon-0.1.3/traceon/tracing.py
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     2204 2023-03-26 19:25:41.000000 traceon-0.1.3/traceon/util.py
-drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-03-27 08:41:11.535927 traceon-0.1.3/traceon.egg-info/
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)     3313 2023-03-27 08:41:11.000000 traceon-0.1.3/traceon.egg-info/PKG-INFO
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)      497 2023-03-27 08:41:11.000000 traceon-0.1.3/traceon.egg-info/SOURCES.txt
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)        1 2023-03-27 08:41:11.000000 traceon-0.1.3/traceon.egg-info/dependency_links.txt
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)       48 2023-03-27 08:41:11.000000 traceon-0.1.3/traceon.egg-info/requires.txt
--rw-r--r--   0 leonvv    (1000) leonvv    (1000)        8 2023-03-27 08:41:11.000000 traceon-0.1.3/traceon.egg-info/top_level.txt
+drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-04-09 21:05:32.803852 traceon-0.2.0/
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)    34524 2023-03-21 09:42:58.000000 traceon-0.2.0/LICENSE.txt
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)       27 2023-04-09 12:34:12.000000 traceon-0.2.0/MANIFEST.in
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     3542 2023-04-09 21:05:32.803852 traceon-0.2.0/PKG-INFO
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     2380 2023-04-09 12:34:12.000000 traceon-0.2.0/README.md
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)       38 2023-04-09 21:05:32.803852 traceon-0.2.0/setup.cfg
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     1435 2023-04-09 21:04:38.000000 traceon-0.2.0/setup.py
+drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-04-09 21:05:32.799852 traceon-0.2.0/traceon/
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     2764 2023-04-09 13:50:35.000000 traceon-0.2.0/traceon/__init__.py
+drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-04-09 21:05:32.799852 traceon-0.2.0/traceon/backend/
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)    16334 2023-04-09 21:01:54.000000 traceon-0.2.0/traceon/backend/__init__.py
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)    43174 2023-04-09 20:53:56.000000 traceon-0.2.0/traceon/backend/traceon-backend.c
+drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-04-09 21:05:32.803852 traceon-0.2.0/traceon/data/
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)  1023104 2023-04-09 12:34:12.000000 traceon-0.2.0/traceon/data/radial-series-3D-theta-dependent-coefficients.npy
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     8128 2023-04-09 12:34:12.000000 traceon-0.2.0/traceon/data/radial-series-3D-thetas.npy
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     8406 2023-04-09 13:45:50.000000 traceon-0.2.0/traceon/excitation.py
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)    13830 2023-04-09 13:28:24.000000 traceon-0.2.0/traceon/geometry.py
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     6781 2023-04-09 13:28:24.000000 traceon-0.2.0/traceon/plotting.py
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)    26699 2023-04-09 13:41:52.000000 traceon-0.2.0/traceon/solver.py
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     8192 2023-04-09 12:34:12.000000 traceon-0.2.0/traceon/tracing.py
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     2204 2023-04-09 12:34:12.000000 traceon-0.2.0/traceon/util.py
+drwxr-xr-x   0 leonvv    (1000) leonvv    (1000)        0 2023-04-09 21:05:32.799852 traceon-0.2.0/traceon.egg-info/
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)     3542 2023-04-09 21:05:32.000000 traceon-0.2.0/traceon.egg-info/PKG-INFO
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)      497 2023-04-09 21:05:32.000000 traceon-0.2.0/traceon.egg-info/SOURCES.txt
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)        1 2023-04-09 21:05:32.000000 traceon-0.2.0/traceon.egg-info/dependency_links.txt
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)       48 2023-04-09 21:05:32.000000 traceon-0.2.0/traceon.egg-info/requires.txt
+-rw-r--r--   0 leonvv    (1000) leonvv    (1000)        8 2023-04-09 21:05:32.000000 traceon-0.2.0/traceon.egg-info/top_level.txt
```

### Comparing `traceon-0.1.3/LICENSE.txt` & `traceon-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `traceon-0.1.3/PKG-INFO` & `traceon-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traceon
-Version: 0.1.3
+Version: 0.2.0
 Summary: Solver and tracer for electrostatic problems
 Home-page: https://github.com/leon-vv/Traceon
 Author: Léon van Velzen
 Author-email: leonvanvelzen@protonmail.com
 License: AGPLv3
 Project-URL: Documentation, https://leon.science/traceon
 Project-URL: Code, https://github.com/leon-vv/traceon
@@ -17,35 +17,44 @@
         
         ## Documentation
         
         [Examples](https://github.com/leon-vv/Traceon/tree/main/examples)
         
         [API documentation](https://leon.science/traceon/index.html)
         
+        ## Citation
+        
+        Please cite the software as follows:
+        
+        ```
+        L.B. van Velzen. Traceon software (version 0.1.3). 2023. https://doi.org/10.5281/zenodo.7773697
+        ```
+        
+        ## Installation
+        
+        Install using the Python package manager:
+        ```
+        pip install traceon
+        ```
+        
+        The installation is known to work on Linux and Windows. Please reach out to me if you have any installation problems.
+        
         ## Validations
         
         To ensure the accuracy of the package, different problems from the literature have been analyzed using this software. See [/validation](https://github.com/leon-vv/Traceon/tree/main/validation) directory for more information. The validations can easily be executed from the command line, for example:
         ```bash
         python3 ./validation/edwards2007.py --help
         python3 ./validation/capacitance-sphere.py --help
         etc...
         ```
         
         ## License
         
         [AGPLv3](https://www.gnu.org/licenses/agpl-3.0.en.html)
         
-        ## Installation
-        
-        Install using the Python package manager:
-        ```
-        pip install traceon
-        ```
-        
-        The installation is known to work on Linux and Windows. Please reach out to me if you have any installation problems.
         
         ## Help! I have a problem!
         
         Don't worry. You can reach me.
         
         [Open an issue](https://github.com/leon-vv/Traceon/issues)
```

### Comparing `traceon-0.1.3/README.md` & `traceon-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,35 +6,44 @@
 
 ## Documentation
 
 [Examples](https://github.com/leon-vv/Traceon/tree/main/examples)
 
 [API documentation](https://leon.science/traceon/index.html)
 
+## Citation
+
+Please cite the software as follows:
+
+```
+L.B. van Velzen. Traceon software (version 0.1.3). 2023. https://doi.org/10.5281/zenodo.7773697
+```
+
+## Installation
+
+Install using the Python package manager:
+```
+pip install traceon
+```
+
+The installation is known to work on Linux and Windows. Please reach out to me if you have any installation problems.
+
 ## Validations
 
 To ensure the accuracy of the package, different problems from the literature have been analyzed using this software. See [/validation](https://github.com/leon-vv/Traceon/tree/main/validation) directory for more information. The validations can easily be executed from the command line, for example:
 ```bash
 python3 ./validation/edwards2007.py --help
 python3 ./validation/capacitance-sphere.py --help
 etc...
 ```
 
 ## License
 
 [AGPLv3](https://www.gnu.org/licenses/agpl-3.0.en.html)
 
-## Installation
-
-Install using the Python package manager:
-```
-pip install traceon
-```
-
-The installation is known to work on Linux and Windows. Please reach out to me if you have any installation problems.
 
 ## Help! I have a problem!
 
 Don't worry. You can reach me.
 
 [Open an issue](https://github.com/leon-vv/Traceon/issues)
```

### Comparing `traceon-0.1.3/setup.py` & `traceon-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 backend_extension = Extension(
     name='traceon.backend.traceon_backend',
     sources=['traceon/backend/traceon-backend.c'],
     **compiler_kwargs)
 
 setup(
     name='traceon',
-    version='0.1.3',
+    version='0.2.0',
     description='Solver and tracer for electrostatic problems',
     url='https://github.com/leon-vv/Traceon',
     author='Léon van Velzen',
     author_email='leonvanvelzen@protonmail.com',
     keywords=['boundary element method', 'BEM', 'electrostatic', 'electromagnetic', 'electron microscope', 'electron', 'tracing', 'particle', 'tracer', 'electron optics'],
     license='AGPLv3',
     ext_modules=[backend_extension],
```

### Comparing `traceon-0.1.3/traceon/__init__.py` & `traceon-0.2.0/traceon/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Welcome!
 
-Traceon is a general software package for numerical
-charged particle optics. The heart of the package is an implementation of the Boundary Element
-Method (BEM) to efficiently compute electrostatic fields. Currently radial symmetry and general
-three dimensional geometries are supported. In both symmetries very accuracute and efficient radial
-series interpolation can be used to make electron tracing very fast. The resulting electron trajectories
-can be used to determine the aberrations of optical components under study.
+Traceon is a general software package used for numerical electron optics. Its main feature is the implementation of the Boundary Element Method (BEM) to quickly calculate the surface charge distribution.
+The program supports both radial symmetry and general three-dimensional geometries. 
+Electron tracing can be done very quickly using accurate radial series interpolation in both geometries.
+The electron trajectories obtained can help determine the aberrations of the optical components under study.
 
 If you have any issues using the package, please open an issue on the [Traceon Github page](https://github.com/leon-vv/Traceon).
 
 The software is currently distributed under the `AGPLv3` license. 
 
 # Usage
 
@@ -50,11 +48,12 @@
 in the formulas for the potential (and thus also in the formulas for the electric field) the actual \( \\sigma \) values themselves are never computed.
 
 """
 
 __pdoc__ = {}
 __pdoc__['traceon.util'] = False
 __pdoc__['traceon.backend'] = False
+__pdoc__['traceon.data'] = False
 __pdoc__['traceon.tracing.Tracer.__call__'] = True
```

### Comparing `traceon-0.1.3/traceon/backend/__init__.py` & `traceon-0.2.0/traceon/backend/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,16 @@
     backend_lib = C.cdll.LoadLibrary(global_path)
 
 
 TRACING_BLOCK_SIZE = C.c_size_t.in_dll(backend_lib, 'TRACING_BLOCK_SIZE').value
 
 DERIV_2D_MAX = C.c_int.in_dll(backend_lib, 'DERIV_2D_MAX_SYM').value
 
+N_QUAD_2D = C.c_int.in_dll(backend_lib, 'N_QUAD_2D_SYM').value
+
 NU_MAX = C.c_int.in_dll(backend_lib, 'NU_MAX_SYM').value
 M_MAX = C.c_int.in_dll(backend_lib, 'M_MAX_SYM').value
 
 # Pass numpy array to C
 def arr(*args, dtype=np.float64, **kwargs):
     return ndpointer(*args, dtype=dtype, flags=('C_CONTIGUOUS', 'ALIGNED'), **kwargs);
 
@@ -58,51 +60,53 @@
 
 integration_cb_2d = C.CFUNCTYPE(dbl, dbl, dbl, dbl, dbl, vp)
 integration_cb_3d = C.CFUNCTYPE(dbl, dbl, dbl, dbl, dbl, dbl, dbl, vp)
 field_fun = C.CFUNCTYPE(None, C.POINTER(dbl), C.POINTER(dbl), vp);
 
 vertices = arr(ndim=3)
 lines = arr(ndim=3)
-charges = arr(ndim=1)
+charges_3d = arr(ndim=1)
+charges_2d = arr(ndim=2)
 z_values = arr(ndim=1)
 
 bounds = arr(shape=(3, 2))
 
 times_block = arr(shape=(TRACING_BLOCK_SIZE,))
 tracing_block = arr(shape=(TRACING_BLOCK_SIZE, 6))
 
 backend_functions = {
     'ellipk' : (dbl, dbl),
     'ellipe': (dbl, dbl),
     'normal_2d': (None, v2, v2, v2),
-    'line_integral': (dbl, v2, v2, v2, integration_cb_2d, C.c_void_p),
     'normal_3d': (None, v3, v3, v3),
     'triangle_integral': (dbl, v3, v3, v3, v3, integration_cb_3d, C.c_void_p),
     'trace_particle': (sz, times_block, tracing_block, field_fun, bounds, dbl, vp),
     'potential_radial_ring': (dbl, dbl, dbl, dbl, dbl, vp), 
     'dr1_potential_radial_ring': (dbl, dbl, dbl, dbl, dbl, vp), 
     'dz1_potential_radial_ring': (dbl, dbl, dbl, dbl, dbl, vp), 
-    'axial_derivatives_radial_ring': (None, arr(ndim=2), lines, charges, sz, z_values, sz),
-    'potential_radial': (dbl, v3, vertices, charges, sz),
+    'axial_derivatives_radial_ring': (None, arr(ndim=2), lines, charges_2d, sz, z_values, sz),
+    'potential_radial': (dbl, v3, vertices, charges_2d, sz),
     'potential_radial_derivs': (dbl, v2, z_values, arr(ndim=3), sz),
-    'field_radial': (None, v3, v3, vertices, charges, sz),
-    'trace_particle_radial': (sz, times_block, tracing_block, bounds, dbl, vertices, charges, sz),
+    'charge_radial': (dbl, arr(ndim=2), arr(ndim=1)),
+    'field_radial': (None, v3, v3, vertices, charges_2d, sz),
+    'trace_particle_radial': (sz, times_block, tracing_block, bounds, dbl, vertices, charges_2d, sz),
     'field_radial_derivs': (None, v3, v3, z_values, arr(ndim=3), sz),
     'trace_particle_radial_derivs': (sz, times_block, tracing_block, bounds, dbl, z_values, arr(ndim=3), sz),
     'dx1_potential_3d_point': (dbl, dbl, dbl, dbl, dbl, dbl, dbl, vp),
     'dy1_potential_3d_point': (dbl, dbl, dbl, dbl, dbl, dbl, dbl, vp),
     'dz1_potential_3d_point': (dbl, dbl, dbl, dbl, dbl, dbl, dbl, vp),
     'potential_3d_point': (dbl, dbl, dbl, dbl, dbl, dbl, dbl, vp),
-    'axial_coefficients_3d': (None, vertices, charges, sz, z_values, arr(ndim=4), sz, arr(ndim=1), arr(ndim=4), sz),
-    'potential_3d': (dbl, v3, vertices, charges, sz),
+    'axial_coefficients_3d': (None, vertices, charges_3d, sz, z_values, arr(ndim=4), sz, arr(ndim=1), arr(ndim=4), sz),
+    'potential_3d': (dbl, v3, vertices, charges_3d, sz),
     'potential_3d_derivs': (dbl, v3, z_values, arr(ndim=5), sz),
-    'field_3d': (None, v3, v3, vertices, charges, sz),
-    'trace_particle_3d': (sz, times_block, tracing_block, bounds, dbl, vertices, charges, sz),
+    'field_3d': (None, v3, v3, vertices, charges_3d, sz),
+    'trace_particle_3d': (sz, times_block, tracing_block, bounds, dbl, vertices, charges_3d, sz),
     'field_3d_derivs': (None, v3, v3, z_values, arr(ndim=5), sz),
     'trace_particle_3d_derivs': (sz, times_block, tracing_block, bounds, dbl, z_values, arr(ndim=5), sz),
+    'add_floating_conductor_constraints_radial': (None, arr(ndim=2), lines, sz, arr(dtype=np.int64), sz, sz),
     'fill_matrix_radial': (None, arr(ndim=2), lines, arr(dtype=C.c_uint8, ndim=1), arr(ndim=1), sz, sz, C.c_int, C.c_int),
     'fill_matrix_3d': (None, arr(ndim=2), vertices, arr(dtype=C.c_uint8, ndim=1), arr(ndim=1), sz, sz, C.c_int, C.c_int),
     'xy_plane_intersection_2d': (C.c_bool, arr(ndim=2), sz, arr(shape=(4,)), dbl),
     'xy_plane_intersection_3d': (C.c_bool, arr(ndim=2), sz, arr(shape=(6,)), dbl)
 }
 
 
@@ -140,18 +144,14 @@
 
 # Remove the last argument, which is usually a void pointer to optional data
 # passed to the function. In Python we don't need this functionality
 # as we can simply use closures.
 def remove_arg(fun):
     return lambda *args: fun(*args[:-1])
 
-def line_integral(point, v1, v2, callback):
-    assert point.shape == (2,) and v1.shape == (2,) and v2.shape == (2,)
-    return backend_lib.line_integral(point, v1, v2, integration_cb_2d(remove_arg(callback)), None)
-
 def normal_3d(p1, p2, p3):
     normal = np.zeros( (3,) )
     backend_lib.normal_2d(p1, p2, normal)
     return normal
    
 def triangle_integral(point, v1, v2, v3, callback):
     assert point.shape == (3,) and v1.shape == (3,) and v2.shape == (3,) and v3.shape == (3,)
@@ -218,15 +218,16 @@
 def trace_particle(position, velocity, field, bounds, atol):
     bounds = np.array(bounds)
     
     return trace_particle_wrapper(position, velocity,
         lambda T, P: backend_lib.trace_particle(T, P, wrap_field_fun(field), bounds, atol, None))
 
 def trace_particle_radial(position, velocity, bounds, atol, vertices, charges):
-    assert vertices.shape == (len(charges), 2, 3)
+    assert vertices.shape == (len(charges), 4, 3)
+    assert charges.shape == (len(charges), N_QUAD_2D)
     bounds = np.array(bounds)
     
     if bounds.shape[0] == 2:
         bounds = np.array([bounds[0], bounds[1], [-1.0, 0.0]])
      
     times, positions = trace_particle_wrapper(position, velocity,
         lambda T, P: backend_lib.trace_particle_radial(T, P, bounds, atol, vertices, charges, len(charges)))
@@ -259,46 +260,55 @@
     assert velocity.shape == (3,)
     assert coeffs.shape == (len(z)-1, 2, NU_MAX, M_MAX, 4)
     bounds = np.array(bounds)
      
     return trace_particle_wrapper(position, velocity,
         lambda T, P: backend_lib.trace_particle_3d_derivs(T, P, bounds, atol, z, coeffs, len(z)))
 
-potential_radial_ring = remove_arg(backend_lib.potential_radial_ring)
-dr1_potential_radial_ring = remove_arg(backend_lib.dr1_potential_radial_ring)
-dz1_potential_radial_ring = remove_arg(backend_lib.dz1_potential_radial_ring)
+potential_radial_ring = lambda *args: backend_lib.potential_radial_ring(*args, None)
+dr1_potential_radial_ring = lambda *args: backend_lib.dr1_potential_radial_ring(*args, None)
+dz1_potential_radial_ring = lambda *args: backend_lib.dz1_potential_radial_ring(*args, None)
 
 def axial_derivatives_radial_ring(z, lines, charges):
     derivs = np.zeros( (z.size, DERIV_2D_MAX) )
-    assert lines.shape[1] == 2 and lines.shape[2] == 3
+    assert lines.shape == (len(charges), 4, 3)
     assert len(lines) == len(charges)
+    assert charges.shape == (len(charges), N_QUAD_2D)
     
     backend_lib.axial_derivatives_radial_ring(derivs, lines, charges, len(lines), z, len(z))
     return derivs
 
 def potential_radial(point, vertices, charges):
     point = _vec_2d_to_3d(point)
-    assert vertices.shape == (len(charges), 2, 3)
+    assert vertices.shape == (len(charges), 4, 3)
+    assert charges.shape == (len(vertices), N_QUAD_2D)
     return backend_lib.potential_radial(point, vertices, charges, len(charges))
 
 def potential_radial_derivs(point, z, coeffs):
     assert coeffs.shape == (len(z)-1, DERIV_2D_MAX, 6)
     return backend_lib.potential_radial_derivs(point, z, coeffs, len(z))
 
+def charge_radial(vertices, charges):
+    assert vertices.shape == (len(charges), 3)
+    assert charges.shape == (len(vertices),)
+
+    return backend_lib.charge_radial(vertices, charges)
+
 def field_radial(point, vertices, charges):
     point = _vec_2d_to_3d(point)
-    assert vertices.shape == (len(charges), 2, 3)
+    assert vertices.shape == (len(charges), 4, 3)
+    assert charges.shape == (len(charges), N_QUAD_2D)
      
     field = np.zeros( (3,) )
     backend_lib.field_radial(point, field, vertices, charges, len(charges))
     return field[:2]
 
 def field_radial_derivs(point, z, coeffs):
     point = _vec_2d_to_3d(point)
-    assert coeffs.shape == (len(z), DERIV_2D_MAX, 6)
+    assert coeffs.shape == (len(z)-1, DERIV_2D_MAX, 6)
     field = np.zeros( (3,) )
     backend_lib.field_radial_derivs(point, field, z, coeffs, len(z))
     return field[:2]
 
 dx1_potential_3d_point = remove_arg(backend_lib.dx1_potential_3d_point)
 dy1_potential_3d_point = remove_arg(backend_lib.dy1_potential_3d_point)
 dz1_potential_3d_point = remove_arg(backend_lib.dz1_potential_3d_point)
@@ -319,39 +329,49 @@
 def potential_3d(point, vertices, charges):
     assert vertices.shape == (len(charges), 3, 3)
     assert point.shape == (3,)
      
     return backend_lib.potential_3d(point, vertices, charges, len(charges))
 
 def potential_3d_derivs(point, z, coeffs):
-    assert coeffs.shape == (len(z), NU_MAX, M_MAX, 4)
+    assert coeffs.shape == (len(z)-1, NU_MAX, M_MAX, 4)
     assert point.shape == (3,)
     
     return backend_lib.potential_3d_derivs(point, z, coeffs, len(z))
 
 def field_3d(point, vertices, charges):
     assert vertices.shape == (len(charges), 3, 3)
     assert point.shape == (3,)
 
     field = np.zeros( (3,) )
     backend_lib.field_3d(point, field, vertices, charges, len(vertices))
     return field
 
 def field_3d_derivs(point, z, coeffs):
     assert point.shape == (3,)
-    assert coeffs.shape == (len(z), NU_MAX, M_MAX, 4)
+    assert coeffs.shape == (len(z)-1, NU_MAX, M_MAX, 4)
 
     field = np.zeros( (3,) )
     backend_lib.field_3d_derivs(point, field, z, coeffs, len(z))
 
+def add_floating_conductor_constraints_radial(matrix, vertices, indices, row):
+    N_matrix = matrix.shape[0]
+    assert all(N_QUAD_2D*i < N_matrix for i in indices)
+    assert matrix.shape[0] == matrix.shape[1]
+
+    return backend_lib.add_floating_conductor_constraints_radial(matrix, vertices, N_matrix, indices.astype(np.int64), len(indices), row)
+
+
 def fill_matrix_radial(matrix, lines, excitation_types, excitation_values, start_index, end_index):
     N = len(lines)
+    N_quad = N_QUAD_2D*N
+    
     # Due to floating conductor constraints the matrix might actually be bigger than NxN
-    assert matrix.shape[0] >= N and matrix.shape[1] >= N and matrix.shape[0] == matrix.shape[1]
-    assert lines.shape == (N, 2, 3)
+    assert matrix.shape[0] >= N_quad and matrix.shape[1] >= N_quad and matrix.shape[0] == matrix.shape[1]
+    assert lines.shape == (N, 4, 3)
     assert excitation_types.shape == (N,)
     assert excitation_values.shape == (N,)
     assert 0 <= start_index < N and 0 <= end_index < N and start_index < end_index
      
     backend_lib.fill_matrix_radial(matrix, lines, excitation_types, excitation_values, N, matrix.shape[0], start_index, end_index)
 
 def fill_matrix_3d(matrix, vertices, excitation_types, excitation_values, start_index, end_index):
```

### Comparing `traceon-0.1.3/traceon/data/radial-series-3D-theta-dependent-coefficients.npy` & `traceon-0.2.0/traceon/data/radial-series-3D-theta-dependent-coefficients.npy`

 * *Files identical despite different names*

### Comparing `traceon-0.1.3/traceon/data/radial-series-3D-thetas.npy` & `traceon-0.2.0/traceon/data/radial-series-3D-thetas.npy`

 * *Files identical despite different names*

### Comparing `traceon-0.1.3/traceon/excitation.py` & `traceon-0.2.0/traceon/excitation.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 
 from enum import IntEnum
 
 import numpy as np
 
 from .geometry import Symmetry
+from .backend import N_QUAD_2D
 
 class ExcitationType(IntEnum):
     """Possible excitation that can be applied to elements of the geometry. See the methods of `Excitation` for documentation."""
     VOLTAGE_FIXED = 1
     VOLTAGE_FUN = 2
     DIELECTRIC = 3
     FLOATING_CONDUCTOR = 4
@@ -102,15 +103,15 @@
             assert name in self.electrodes
             self.excitation_types[name] = (ExcitationType.FLOATING_CONDUCTOR, charge)
      
     def _get_element_type(self):
         if self.mesh.symmetry == Symmetry.THREE_D:
             return 'triangle'
         else:
-            return 'line'
+            return 'line4'
     
         
     def _split_for_superposition(self):
         
         # Names that have a fixed voltage excitation, not equal to 0.0
         types = self.excitation_types
         non_zero_fixed = [n for n, (t, v) in types.items() if t == ExcitationType.VOLTAGE_FIXED and v != 0.0]
@@ -141,16 +142,18 @@
 
     def get_active_elements(self):
         """Get elements in the mesh that are active, in the sense that
         an excitation to them has been applied. 
     
         Returns
         --------
-        A tuple of two elements: (points, names). points is a Numpy array of shape (N, 2, 3) in the case of 2D and (N, 3, 3) in the case of 3D. \
+        A tuple of two elements: (points, names). points is a Numpy array of shape (N, 4, 3) in the case of 2D and (N, 3, 3) in the case of 3D. \
         This array contains the vertices of the line elements or the triangles. \
+        Multiple points per line elements are used in the case of 2D since higher order BEM is employed, in which the true position on the line \
+        element is given by a polynomial interpolation of the points. \
         names is a dictionary, the keys being the names of the physical groups mentioned by this excitation, \
         while the values are Numpy arrays of indices that can be used to index the points array.
         """
         type_ = self._get_element_type()
         mesh = self.mesh.mesh
         vertices = mesh.cells_dict[type_] # Indices making up the lines and triangles
         inactive = np.full(len(vertices), True)
@@ -175,11 +178,22 @@
         --------
         int, giving the number of elements. """
         type_ = self._get_element_type()
         mesh = self.mesh.mesh
         
         return sum(len(mesh.cell_sets_dict[n][type_]) for n in self.excitation_types.keys())
 
+    def get_number_of_matrix_elements(self):
+        
+        Nfloating = len([name for name, (type_, _) in self.excitation_types.items() if type_ == ExcitationType.FLOATING_CONDUCTOR])
+        Nelem = self.get_number_of_active_elements()
+         
+        if self.mesh.symmetry == Symmetry.RADIAL:
+            return Nelem*N_QUAD_2D + Nfloating
+        elif self.mesh.symmetry == Symmetry.THREE_D:
+            return Nelem + Nfloating
+
+
```

### Comparing `traceon-0.1.3/traceon/geometry.py` & `traceon-0.2.0/traceon/geometry.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pygmsh import *
 import gmsh
 from enum import Enum
 
 import pickle
 
 from .util import Saveable
+from .backend import N_QUAD_2D
 
 
 def revolve_around_optical_axis(geom, elements, factor=1.0):
     """
     Revolve geometry elements around the optical axis. Useful when you
     want to generate 3D geometries from a cylindrically symmetric 2D geometry.
     
@@ -66,17 +67,17 @@
 
     def __str__(self):
         if self == Symmetry.RADIAL:
             return 'radial'
         elif self == Symmetry.THREE_D:
             return '3d'
 
-class Geometry(occ.Geometry):
+class Geometry(geo.Geometry):
     """
-    Small wrapper class around pygmsh.occ.Geometry which itself is a small wrapper around the powerful GMSH library.
+    Small wrapper class around pygmsh.geo.Geometry which itself is a small wrapper around the powerful GMSH library.
     See the GMSH and pygmsh documentation to learn how to build any 2D or 3D geometry. This class makes it easier to control
     the mesh size (using the _mesh size factor_) and optionally allows to scale the mesh size with the distance from the optical
     axis. It also add support for multiple calls to the `add_physical` method with the same name.
     
     Parameters
     ---------
     symmetry: Symmetry
@@ -123,43 +124,48 @@
             self._physical_queue[name].extend(entities)
         else:
             self._physical_queue[name] = entities
 
     def generate_mesh(self, *args, **kwargs):
         """
         Generate the mesh, determining the mesh dimension (line elements or triangles) from the
-        supplied symmetry. The arguments are passed directly to `pygmsh.occ.Geometry.generate_mesh`.
+        supplied symmetry. The arguments are passed directly to `pygmsh.geo.Geometry.generate_mesh`.
         
         Returns
         -------
         `Mesh`
 
         """
         for label, entities in self._physical_queue.items():
             super().add_physical(entities, label)
           
         if self.size_from_distance:
             self.set_mesh_size_callback(self._mesh_size_callback)
         
         dim = 2 if self.symmetry == Symmetry.THREE_D else 1
+
+        if dim == 1:
+            gmsh.option.setNumber('Mesh.ElementOrder', 3)
+        else:
+            gmsh.option.setNumber('Mesh.ElementOrder', 1)
         
         return Mesh(super().generate_mesh(dim=dim, *args, **kwargs), self.symmetry)
 
     def set_mesh_size_factor(self, factor):
         """
         Set the mesh size factor. Which simply scales with the total number of elements in the mesh.
         
         Parameters
         ----------
         factor : float
             The mesh size factor to use. 
         
         """
         if self.symmetry == Symmetry.RADIAL:
-            gmsh.option.setNumber('Mesh.MeshSizeFactor', 1/factor)
+            gmsh.option.setNumber('Mesh.MeshSizeFactor', 1/factor * N_QUAD_2D)
         elif self.symmetry == Symmetry.THREE_D:
             # GMSH seems to produce meshes which contain way more elements for 3D geometries
             # with the same mesh factor. This is confusing for users and therefore we arbtrarily
             # incrase the mesh size to roughly correspond with the 2D number of elements.
             gmsh.option.setNumber('Mesh.MeshSizeFactor', 4*sqrt(1/factor))
 
     def set_minimum_mesh_size(self, size):
@@ -211,27 +217,30 @@
 
         """
         return list(self.mesh.cell_sets_dict.keys())
     
     def __str__(self):
         physicals = self.mesh.cell_sets_dict.keys()
         physical_names = ', '.join(physicals)
-        type_ = 'line' if self.symmetry != Symmetry.THREE_D else 'triangle'
+        type_ = 'line4' if self.symmetry != Symmetry.THREE_D else 'triangle'
         physical_nums = ', '.join([str(len(self.mesh.cell_sets_dict[n][type_])) for n in physicals])
         
         cells_type = ['point'] + [str(c.type) for c in self.mesh.cells]
         cells_count = [len(self.mesh.points)] + [len(c) for c in self.mesh.cells]
         
         return f'<Traceon Mesh {self.symmetry},\n' \
             f'\tPhysical groups: {physical_names}\n' \
             f'\tElements in physical groups: {physical_nums}\n' \
             f'\tNumber of.. \n\t    ' \
             + '\n\t    '.join([f'{t}: \t{c}' for t, c in zip(cells_type, cells_count)]) \
             + '>'
 
+    def write_gmsh(self, filename):
+        self.mesh.write(filename)
+
 
         #return f'<Traceon Mesh with {len(self.mesh.points)} points, ', '.join(self.mesh.cell_sets_dict.keys()))
         #return str(self.mesh) + ' (metadata: ' + str(self.metadata) + ')'
 
 class MEMSStack(Geometry):
     """Geometry consisting of a stack of MEMS fabricated elements. This geometry is modelled using a stack
     of rectangularly shaped elements with a variable spacing in between. Useful when doing calculations on MEMS fabricated
@@ -317,15 +326,15 @@
         self._current_z += thickness
         
         return cl
     
     def generate_mesh(self, *args, **kwargs):
         """
         Generate the mesh, determining the mesh dimension (line elements or triangles) from the
-        supplied `revolve_factor`. The arguments are passed directly to `pygmsh.occ.Geometry.generate_mesh`.
+        supplied `revolve_factor`. The arguments are passed directly to `pygmsh.geo.Geometry.generate_mesh`.
         
         Returns
         -------
         `Mesh`
 
         """
         # Enclose on right
```

### Comparing `traceon-0.1.3/traceon/plotting.py` & `traceon-0.2.0/traceon/plotting.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,32 +2,31 @@
 to show the line and triangle meshes generated by Traceon."""
 
 import matplotlib.tri as mtri
 import matplotlib.pyplot as plt
 from matplotlib.collections import LineCollection
 from scipy.interpolate import *
 import numpy as np
-import vedo
 
 from . import backend
 
 def _create_point_to_physical_dict(mesh):
     d = {}
     
     for k, v in mesh.cell_sets_dict.items():
         
         if 'triangle' in v: 
             for p in mesh.cells_dict['triangle'][v['triangle']]:
                 a, b, c = p
                 d[a], d[b], d[c] = k, k, k
         
-        if 'line' in v:
-            for l in mesh.cells_dict['line'][v['line']]:
-                a, b = l
-                d[a], d[b] = k, k
+        if 'line4' in v:
+            for l in mesh.cells_dict['line4'][v['line4']]:
+                a, b, c, e = l
+                d[a], d[b], d[c], d[e] = k, k, k, k
      
     return d
 
 # Taken from
 # https://stackoverflow.com/questions/13685386/matplotlib-equal-unit-length-with-equal-aspect-ratio-z-axis-is-not-equal-to
 def _set_axes_equal(ax):
     """Set 3D plot axes to equal scale.
@@ -44,45 +43,14 @@
     x, y, z = np.mean(limits, axis=1)
     radius = 0.5 * np.max(np.abs(limits[:, 1] - limits[:, 0]))
     ax.set_xlim3d([x - radius, x + radius])
     ax.set_ylim3d([y - radius, y + radius])
     ax.set_zlim3d([z - radius, z + radius])
 
 def plot_triangle_mesh(mesh, show_legend=True, **colors):
-    
-    dict_ = _create_point_to_physical_dict(mesh)
-    triangles = mesh.cells_dict['triangle']
-     
-    triangles_to_plot = []
-    colors_ = []
-     
-    for (A, B, C) in triangles:
-        color = '#CCC'
-        
-        if A in dict_ and B in dict_ and C in dict_:
-            phys1, phys2, phys3 = dict_[A], dict_[B], dict_[C]
-            if phys1 == phys2 and phys2 == phys3 and phys1 in colors:
-                color = colors[phys1]
-         
-        triangles_to_plot.append( [A, B, C] )
-        colors_.append(color)
-    
-    colors_, triangles_to_plot = np.array(colors_), np.array(triangles_to_plot)
-    plotter = vedo.Plotter()
-    
-    for c in set(colors_):
-        mask = colors_ == c
-        vm = vedo.Mesh([mesh.points, triangles_to_plot[mask]], c)
-        vm.linecolor('black').linewidth(1)
-        plotter += vm
-    
-    vedo.show(plotter, viewup='z', axes=True)
-
-'''
-def plot_triangle_mesh(mesh, show_legend=True, **colors):
     """Show a 3D mesh (mesh consisting of many triangles).
 
     Parameters
     ----------
     mesh: meshio mesh
         The mesh to show.
 
@@ -141,15 +109,14 @@
             plt.plot([], [], label=l, color=c)
         plt.legend(loc='upper left')
      
     plt.xlabel('x (mm)')
     plt.ylabel('y (mm)')
     ax.set_zlabel('z (mm)')
     plt.show()
-'''
 
 
 def plot_line_mesh(mesh, trajectory=None, show_legend=True, **colors):
     """Show a 2D mesh (mesh consisting of many line elements).
     
     Parameters
     ---------
@@ -166,32 +133,33 @@
         physical group names, while the values can be any color understood by matplotlib.
     """
     plt.figure(figsize=(10, 13))
     plt.rcParams.update({'font.size': 17})
     plt.gca().set_aspect('equal')
      
     dict_ = _create_point_to_physical_dict(mesh)
-    lines = mesh.cells_dict['line']
-
+    lines = mesh.cells_dict['line4']
+    
     to_plot_x = []
     to_plot_y = []
     colors_ = []
     
-    for (A, B) in lines:
-        color = '#CCC'
-
-        if A in dict_ and B in dict_:
-            phys1, phys2 = dict_[A], dict_[B]
-            if phys1 == phys2 and phys1 in colors:
-                color = colors[phys1]
-         
-        p1, p2 = mesh.points[A], mesh.points[B]
-        to_plot_x.append( [p1[0], p2[0]] )
-        to_plot_y.append( [p1[1], p2[1]] )
-        colors_.append(color)
+    for (P1, P2, P3, P4) in lines:
+        for A, B in [(P1, P3), (P3, P4), (P4, P2)]:
+            color = '#CCC'
+
+            if A in dict_ and B in dict_:
+                phys1, phys2 = dict_[A], dict_[B]
+                if phys1 == phys2 and phys1 in colors:
+                    color = colors[phys1]
+            
+            p1, p2 = mesh.points[A], mesh.points[B]
+            to_plot_x.append( [p1[0], p2[0]] )
+            to_plot_y.append( [p1[1], p2[1]] )
+            colors_.append(color)
      
     colors_ = np.array(colors_)
      
     for c in set(colors_):
         mask = colors_ == c
         plt.plot(np.array(to_plot_x)[mask].T, np.array(to_plot_y)[mask].T, color=c, linewidth=2)
         plt.scatter(np.array(to_plot_x)[mask].T, np.array(to_plot_y)[mask].T, color=c, s=15)
```

### Comparing `traceon-0.1.3/traceon/solver.py` & `traceon-0.2.0/traceon/solver.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 import math as m
 import time
 from threading import Thread
 import os.path as path
 
 import numpy as np
 from scipy.interpolate import CubicSpline, BPoly, PPoly
+from scipy.special import legendre
+from scipy.integrate import quad
 
 from . import geometry as G
 from . import excitation as E
 from . import backend
 from . import util
 
 FACTOR_AXIAL_DERIV_SAMPLING_2D = 0.2
@@ -66,39 +68,50 @@
 theta0 = thetas[0]
 dtheta = thetas[1]-thetas[0]
 
 thetas_interpolation_coefficients = np.load(coefficients_file)
 
 assert thetas_interpolation_coefficients.shape == (thetas.size-1, backend.NU_MAX, backend.M_MAX, 4)
 
+def _get_N_quad(exc):
+    if exc.mesh.symmetry == G.Symmetry.RADIAL:
+        return backend.N_QUAD_2D
+    elif exc.mesh.symmetry == G.Symmetry.THREE_D:
+        return 1
+
 def _get_floating_conductor_names(exc):
     return [n for n, (t, v) in exc.excitation_types.items() if t == E.ExcitationType.FLOATING_CONDUCTOR]
 
 def _excitation_to_right_hand_side(excitation, vertices, names):
     floating_names = _get_floating_conductor_names(excitation)
      
     N_floating = len(floating_names)
     N_lines = len(vertices)
-    N_matrix = N_lines + N_floating # Every floating conductor adds one constraint
+    N_quad = _get_N_quad(excitation)
+    N_matrix = N_quad*N_lines + N_floating # Every floating conductor adds one constraint
 
     F = np.zeros( (N_matrix) )
      
     for name, indices in names.items():
         type_, value  = excitation.excitation_types[name]
+
+        all_indices = np.concatenate( [N_quad*indices + i for i in range(N_quad)] )
          
         if type_ == E.ExcitationType.VOLTAGE_FIXED:
-            F[indices] = value
+            F[all_indices] = value
         elif type_ == E.ExcitationType.VOLTAGE_FUN:
             for i in indices:
                 points = vertices[i]
                 middle = np.average(points, axis=0)
-                F[i] = value(*middle)
+                for q in range(N_quad):
+                    # TODO: use higher order BEM?
+                    F[N_quad*i + q] = value(*middle)
         elif type_ == E.ExcitationType.DIELECTRIC or \
                 type_ == E.ExcitationType.FLOATING_CONDUCTOR:
-            F[indices] = 0
+            F[all_indices] = 0
     
     # See comments in _add_floating_conductor_constraints_to_matrix
     for i, f in enumerate(floating_names):
         F[-N_floating+i] = excitation.excitation_types[f][1]
      
     assert np.all(np.isfinite(F))
     return F
@@ -115,75 +128,87 @@
 
 def _add_floating_conductor_constraints_to_matrix(matrix, vertices, names, excitation):
     floating = _get_floating_conductor_names(excitation)
     N_matrix = matrix.shape[0]
     assert matrix.shape == (N_matrix, N_matrix)
      
     for i, f in enumerate(floating):
-        for index in names[f]:
-            # An extra unknown voltage is added to the matrix for every floating conductor.
-            # The column related to this unknown voltage is positioned at the rightmost edge of the matrix.
-            # If multiple floating conductors are present the column lives at -len(floating) + i
-            matrix[ index, -len(floating) + i] = -1
-            # The unknown voltage is determined by the constraint on the total charge of the conductor.
-            # This constraint lives at the bottom edge of the matrix.
-            # The surface area of the respective line element (or triangle) is multiplied by the surface charge (unknown)
-            # to arrive at the total specified charge (right hand side).
-            element = vertices[index]
-            matrix[ -len(floating) + i, index] = _area(excitation.mesh.symmetry, element)
+        if excitation.mesh.symmetry == G.Symmetry.THREE_D: 
+            for index in names[f]:
+                # An extra unknown voltage is added to the matrix for every floating conductor.
+                # The column related to this unknown voltage is positioned at the rightmost edge of the matrix.
+                # If multiple floating conductors are present the column lives at -len(floating) + i
+                matrix[ index, -len(floating) + i] = -1
+                # The unknown voltage is determined by the constraint on the total charge of the conductor.
+                # This constraint lives at the bottom edge of the matrix.
+                # The surface area of the respective line element (or triangle) is multiplied by the surface charge (unknown)
+                # to arrive at the total specified charge (right hand side).
+                element = vertices[index]
+                matrix[ -len(floating) + i, index] = _area(excitation.mesh.symmetry, element)
+        elif excitation.mesh.symmetry == G.Symmetry.RADIAL:
+            indices = names[f]
+            backend.add_floating_conductor_constraints_radial(matrix, vertices, indices, i)
+                
 
 def _excitation_to_matrix(excitation, vertices, names):
     floating_names = _get_floating_conductor_names(excitation)
     
     N_floating = len(floating_names)
     N_lines = len(vertices)
-    N_matrix = N_lines + N_floating # Every floating conductor adds one constraint
+    N_quad = _get_N_quad(excitation)
+    N_matrix = N_quad*N_lines + N_floating # Every floating conductor adds one constraint
      
     excitation_types = np.zeros(N_lines, dtype=np.uint8)
     excitation_values = np.zeros(N_lines)
     
     for n, indices in names.items():
         excitation_types[indices] = int( excitation.excitation_types[n][0] )
         
         if excitation.excitation_types[n][0] == E.ExcitationType.DIELECTRIC:
             excitation_values[indices] = excitation.excitation_types[n][1]
      
     assert np.all(excitation_types != 0)
      
-    print(f'Total number of elements: {N_lines}, symmetry: {excitation.mesh.symmetry}')
-     
     st = time.time()
-    
     matrix = np.zeros( (N_matrix, N_matrix) )
+    print(f'Number of elements: {N_lines}, size of matrix: {N_matrix} ({matrix.nbytes/1e6:.0f} MB), symmetry: {excitation.mesh.symmetry}')
+     
     fill_fun = backend.fill_matrix_radial if excitation.mesh.symmetry != G.Symmetry.THREE_D else backend.fill_matrix_3d
-
+    
     def fill_matrix_rows(rows):
         fill_fun(matrix, vertices, excitation_types, excitation_values, rows[0], rows[-1])
     
     util.split_collect(fill_matrix_rows, np.arange(N_lines))    
-      
+
+    # Fill the difficult self voltages
+    print(f'Time for building matrix: {(time.time()-st)*1000:.0f} ms')
+     
     assert np.all(np.isfinite(matrix))
     
     _add_floating_conductor_constraints_to_matrix(matrix, vertices, names, excitation)
-    print(f'Time for building matrix: {(time.time()-st)*1000:.0f} ms')
         
     return matrix
 
 
 def _charges_to_field(excitation, charges, vertices, names):
     floating_names = _get_floating_conductor_names(excitation)
     N_floating = len(floating_names)
-    assert len(charges) == len(vertices) + N_floating
+    N_quad = _get_N_quad(excitation)
+     
+    assert len(charges) == N_quad*len(vertices) + N_floating
     
     floating_voltages = {n:charges[-N_floating+i] for i, n in enumerate(floating_names)}
     if N_floating > 0:
         charges = charges[:-N_floating]
      
-    assert len(charges) == len(vertices)
-      
+    assert len(charges) == N_quad*len(vertices)
+
+    if N_quad > 1:
+        charges = np.reshape(charges, (len(vertices), N_quad))
+     
     field_class = FieldRadialBEM if excitation.mesh.symmetry != G.Symmetry.THREE_D else Field3D_BEM
     return field_class(vertices, charges, floating_voltages=floating_voltages)
     
 
 def solve_bem(excitation, superposition=False):
     """
     Solve for the charges on the surface of the geometry by using the Boundary Element Method (BEM) and taking
@@ -211,15 +236,14 @@
     """
     
     vertices, names = excitation.get_active_elements()
      
     if not superposition:
         matrix = _excitation_to_matrix(excitation, vertices, names)
         F = _excitation_to_right_hand_side(excitation, vertices, names)
-        
         st = time.time()
         charges = np.linalg.solve(matrix, F)
         assert np.all(np.isfinite(charges))
         print(f'Time for solving matrix: {(time.time()-st)*1000:.0f} ms')
 
         return _charges_to_field(excitation, charges, vertices, names)
      
@@ -313,15 +337,15 @@
 
 class FieldRadialBEM(FieldBEM):
     """A radially symmetric electrostatic field. The field is a result of the surface charges as computed by the
     `solve_bem` function. See the comments in `FieldBEM`."""
     
     def __init__(self, vertices, charges, floating_voltages={}):
         super().__init__(vertices, charges, floating_voltages)
-        assert vertices.shape == (len(charges), 2, 3)
+        assert vertices.shape == (len(charges), 4, 3)
         
     def field_at_point(self, point):
         """
         Compute the electric field, \( \\vec{E} = -\\nabla \phi \)
         
         Parameters
         ----------
@@ -398,14 +422,32 @@
         st = time.time()
         derivs = np.concatenate(util.split_collect(self.get_axial_potential_derivatives, z), axis=0)
         coeffs = _quintic_spline_coefficients(z, derivs.T)
         print(f'Computing derivative interpolation took {(time.time()-st)*1000:.2f} ms ({len(z)} items)')
         
         return FieldRadialAxial(z, coeffs)
 
+    def _charge_on_index(self, i):
+        return backend.charge_radial(self.vertices[i], self.charges[i])
+
+    def charge_on_elements(self, indices):
+        """Compute the sum of the charges present on the elements with the given indices. To
+        get the total charge of a physical group use `names['name']` for indices where `names` 
+        is returned by `traceon.excitation.Excitation.get_active_elements()`.
+
+        Parameters
+        ----------
+        indices: (N,) array of int
+            indices of the elements contributing to the charge sum. 
+         
+        Returns
+        -------
+        The sum of the charge. See the note about units on the front page."""
+        return sum(self._charge_on_index(i) for i in indices)
+
 class Field3D_BEM(FieldBEM):
     """An electrostatic field resulting from a general 3D geometry. The field is a result of the surface charges as computed by the
     `solve_bem` function. See the comments in `FieldBEM`."""
      
     def __init__(self, vertices, charges, floating_voltages={}):
         super().__init__(vertices, charges, floating_voltages)
         assert vertices.shape == (len(charges), 3, 3)
```

### Comparing `traceon-0.1.3/traceon/tracing.py` & `traceon-0.2.0/traceon/tracing.py`

 * *Files identical despite different names*

### Comparing `traceon-0.1.3/traceon/util.py` & `traceon-0.2.0/traceon/util.py`

 * *Files identical despite different names*

### Comparing `traceon-0.1.3/traceon.egg-info/PKG-INFO` & `traceon-0.2.0/traceon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traceon
-Version: 0.1.3
+Version: 0.2.0
 Summary: Solver and tracer for electrostatic problems
 Home-page: https://github.com/leon-vv/Traceon
 Author: Léon van Velzen
 Author-email: leonvanvelzen@protonmail.com
 License: AGPLv3
 Project-URL: Documentation, https://leon.science/traceon
 Project-URL: Code, https://github.com/leon-vv/traceon
@@ -17,35 +17,44 @@
         
         ## Documentation
         
         [Examples](https://github.com/leon-vv/Traceon/tree/main/examples)
         
         [API documentation](https://leon.science/traceon/index.html)
         
+        ## Citation
+        
+        Please cite the software as follows:
+        
+        ```
+        L.B. van Velzen. Traceon software (version 0.1.3). 2023. https://doi.org/10.5281/zenodo.7773697
+        ```
+        
+        ## Installation
+        
+        Install using the Python package manager:
+        ```
+        pip install traceon
+        ```
+        
+        The installation is known to work on Linux and Windows. Please reach out to me if you have any installation problems.
+        
         ## Validations
         
         To ensure the accuracy of the package, different problems from the literature have been analyzed using this software. See [/validation](https://github.com/leon-vv/Traceon/tree/main/validation) directory for more information. The validations can easily be executed from the command line, for example:
         ```bash
         python3 ./validation/edwards2007.py --help
         python3 ./validation/capacitance-sphere.py --help
         etc...
         ```
         
         ## License
         
         [AGPLv3](https://www.gnu.org/licenses/agpl-3.0.en.html)
         
-        ## Installation
-        
-        Install using the Python package manager:
-        ```
-        pip install traceon
-        ```
-        
-        The installation is known to work on Linux and Windows. Please reach out to me if you have any installation problems.
         
         ## Help! I have a problem!
         
         Don't worry. You can reach me.
         
         [Open an issue](https://github.com/leon-vv/Traceon/issues)
```

