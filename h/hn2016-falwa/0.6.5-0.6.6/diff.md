# Comparing `tmp/hn2016_falwa-0.6.5.tar.gz` & `tmp/hn2016_falwa-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hn2016_falwa-0.6.5.tar", last modified: Thu Mar  2 05:48:12 2023, max compression
+gzip compressed data, was "hn2016_falwa-0.6.6.tar", last modified: Sun Apr  9 19:51:08 2023, max compression
```

## Comparing `hn2016_falwa-0.6.5.tar` & `hn2016_falwa-0.6.6.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-03-02 05:48:12.000000 hn2016_falwa-0.6.5/
--rw-r--r--   0 claresyhuang   (501) staff       (20)     1462 2023-03-02 05:48:12.000000 hn2016_falwa-0.6.5/PKG-INFO
-drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-03-02 05:48:12.000000 hn2016_falwa-0.6.5/hn2016_falwa/
--rw-r--r--   0 claresyhuang   (501) staff       (20)      679 2023-03-02 05:43:47.000000 hn2016_falwa-0.6.5/hn2016_falwa/__init__.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)     4834 2022-08-28 04:26:39.000000 hn2016_falwa-0.6.5/hn2016_falwa/barotropic_field.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)     4853 2022-08-28 04:26:28.000000 hn2016_falwa-0.6.5/hn2016_falwa/basis.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)      335 2023-01-17 16:56:08.000000 hn2016_falwa-0.6.5/hn2016_falwa/constant.py
-drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-03-02 05:48:12.000000 hn2016_falwa-0.6.5/hn2016_falwa/f90_modules/
--rw-r--r--   0 claresyhuang   (501) staff       (20)     5000 2023-02-14 04:53:29.000000 hn2016_falwa-0.6.5/hn2016_falwa/f90_modules/compute_flux_dirinv.f90
--rw-r--r--   0 claresyhuang   (501) staff       (20)     5819 2023-02-14 04:53:29.000000 hn2016_falwa-0.6.5/hn2016_falwa/f90_modules/compute_lwa_and_barotropic_fluxes.f90
--rw-r--r--   0 claresyhuang   (501) staff       (20)     4592 2023-01-17 16:56:08.000000 hn2016_falwa-0.6.5/hn2016_falwa/f90_modules/compute_qref_and_fawa_first.f90
--rw-r--r--   0 claresyhuang   (501) staff       (20)     7231 2022-08-28 03:20:26.000000 hn2016_falwa-0.6.5/hn2016_falwa/f90_modules/compute_reference_states.f90
--rw-r--r--   0 claresyhuang   (501) staff       (20)     6105 2022-08-28 03:20:26.000000 hn2016_falwa-0.6.5/hn2016_falwa/f90_modules/interpolate_fields.f90
--rw-r--r--   0 claresyhuang   (501) staff       (20)     5625 2023-01-17 16:56:08.000000 hn2016_falwa-0.6.5/hn2016_falwa/f90_modules/interpolate_fields_dirinv.f90
--rw-r--r--   0 claresyhuang   (501) staff       (20)      905 2022-08-28 03:20:26.000000 hn2016_falwa-0.6.5/hn2016_falwa/f90_modules/matrix_after_inversion.f90
--rw-r--r--   0 claresyhuang   (501) staff       (20)     2353 2023-01-17 16:56:08.000000 hn2016_falwa-0.6.5/hn2016_falwa/f90_modules/matrix_b4_inversion.f90
--rw-r--r--   0 claresyhuang   (501) staff       (20)     2288 2022-08-28 03:20:26.000000 hn2016_falwa-0.6.5/hn2016_falwa/f90_modules/upward_sweep.f90
-drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-03-02 05:48:12.000000 hn2016_falwa-0.6.5/hn2016_falwa/legacy/
--rw-r--r--   0 claresyhuang   (501) staff       (20)        0 2021-08-14 20:06:09.000000 hn2016_falwa-0.6.5/hn2016_falwa/legacy/__init__.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)    20729 2021-08-14 20:06:33.000000 hn2016_falwa-0.6.5/hn2016_falwa/legacy/beta_version.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)    50300 2023-01-17 16:56:40.000000 hn2016_falwa-0.6.5/hn2016_falwa/oopinterface.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)     1161 2023-01-17 16:56:08.000000 hn2016_falwa-0.6.5/hn2016_falwa/plot_utilities.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)     3346 2022-08-30 03:28:00.000000 hn2016_falwa-0.6.5/hn2016_falwa/qgformalism.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)     9932 2022-08-28 04:25:37.000000 hn2016_falwa-0.6.5/hn2016_falwa/utilities.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)    23544 2022-08-28 04:25:29.000000 hn2016_falwa-0.6.5/hn2016_falwa/wrapper.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)    28059 2023-01-17 16:56:08.000000 hn2016_falwa-0.6.5/hn2016_falwa/xarrayinterface.py
-drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-03-02 05:48:12.000000 hn2016_falwa-0.6.5/hn2016_falwa.egg-info/
--rw-r--r--   0 claresyhuang   (501) staff       (20)     1462 2023-03-02 05:48:11.000000 hn2016_falwa-0.6.5/hn2016_falwa.egg-info/PKG-INFO
--rw-r--r--   0 claresyhuang   (501) staff       (20)     1202 2023-03-02 05:48:11.000000 hn2016_falwa-0.6.5/hn2016_falwa.egg-info/SOURCES.txt
--rw-r--r--   0 claresyhuang   (501) staff       (20)        1 2023-03-02 05:48:11.000000 hn2016_falwa-0.6.5/hn2016_falwa.egg-info/dependency_links.txt
--rw-r--r--   0 claresyhuang   (501) staff       (20)        1 2023-03-02 05:32:38.000000 hn2016_falwa-0.6.5/hn2016_falwa.egg-info/not-zip-safe
--rw-r--r--   0 claresyhuang   (501) staff       (20)       19 2023-03-02 05:48:11.000000 hn2016_falwa-0.6.5/hn2016_falwa.egg-info/requires.txt
--rw-r--r--   0 claresyhuang   (501) staff       (20)       19 2023-03-02 05:48:11.000000 hn2016_falwa-0.6.5/hn2016_falwa.egg-info/top_level.txt
--rw-r--r--   0 claresyhuang   (501) staff       (20)       38 2023-03-02 05:48:12.000000 hn2016_falwa-0.6.5/setup.cfg
--rw-r--r--   0 claresyhuang   (501) staff       (20)     3513 2023-03-02 05:43:47.000000 hn2016_falwa-0.6.5/setup.py
-drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-03-02 05:48:12.000000 hn2016_falwa-0.6.5/tests/
--rw-r--r--   0 claresyhuang   (501) staff       (20)        0 2020-03-01 18:39:03.000000 hn2016_falwa-0.6.5/tests/__init__.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)        1 2020-03-01 18:39:03.000000 hn2016_falwa-0.6.5/tests/conftest.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)     3839 2021-08-15 20:17:11.000000 hn2016_falwa-0.6.5/tests/test_barotropic_field.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)     2063 2020-03-01 18:39:03.000000 hn2016_falwa-0.6.5/tests/test_basis.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)    10170 2023-02-14 23:09:16.000000 hn2016_falwa-0.6.5/tests/test_oopinterface.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)     1167 2020-03-01 18:39:03.000000 hn2016_falwa-0.6.5/tests/test_utilities.py
--rw-r--r--   0 claresyhuang   (501) staff       (20)     5643 2022-08-28 03:20:26.000000 hn2016_falwa-0.6.5/tests/test_xarrayinterface.py
+drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-04-09 19:51:08.770943 hn2016_falwa-0.6.6/
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     1065 2020-03-01 18:38:08.000000 hn2016_falwa-0.6.6/LICENSE.txt
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     1320 2023-04-09 19:51:08.770639 hn2016_falwa-0.6.6/PKG-INFO
+drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-04-09 19:51:08.558964 hn2016_falwa-0.6.6/hn2016_falwa/
+-rw-r--r--   0 claresyhuang   (501) staff       (20)      679 2023-04-09 19:49:59.000000 hn2016_falwa-0.6.6/hn2016_falwa/__init__.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     4834 2022-08-28 04:26:39.000000 hn2016_falwa-0.6.6/hn2016_falwa/barotropic_field.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     4853 2022-08-28 04:26:28.000000 hn2016_falwa-0.6.6/hn2016_falwa/basis.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)      335 2023-01-17 16:56:08.000000 hn2016_falwa-0.6.6/hn2016_falwa/constant.py
+drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-04-09 19:51:08.647229 hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     5000 2023-02-14 04:53:29.000000 hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/compute_flux_dirinv.f90
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     5819 2023-02-14 04:53:29.000000 hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/compute_lwa_and_barotropic_fluxes.f90
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     4592 2023-01-17 16:56:08.000000 hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/compute_qref_and_fawa_first.f90
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     7231 2022-08-28 03:20:26.000000 hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/compute_reference_states.f90
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     6105 2022-08-28 03:20:26.000000 hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/interpolate_fields.f90
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     5625 2023-01-17 16:56:08.000000 hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/interpolate_fields_dirinv.f90
+-rw-r--r--   0 claresyhuang   (501) staff       (20)      905 2022-08-28 03:20:26.000000 hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/matrix_after_inversion.f90
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     2353 2023-01-17 16:56:08.000000 hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/matrix_b4_inversion.f90
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     2288 2022-08-28 03:20:26.000000 hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/upward_sweep.f90
+drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-04-09 19:51:08.662719 hn2016_falwa-0.6.6/hn2016_falwa/legacy/
+-rw-r--r--   0 claresyhuang   (501) staff       (20)        0 2021-08-14 20:06:09.000000 hn2016_falwa-0.6.6/hn2016_falwa/legacy/__init__.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)    20729 2021-08-14 20:06:33.000000 hn2016_falwa-0.6.6/hn2016_falwa/legacy/beta_version.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)    50300 2023-01-17 16:56:40.000000 hn2016_falwa-0.6.6/hn2016_falwa/oopinterface.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     1161 2023-01-17 16:56:08.000000 hn2016_falwa-0.6.6/hn2016_falwa/plot_utilities.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     3346 2022-08-30 03:28:00.000000 hn2016_falwa-0.6.6/hn2016_falwa/qgformalism.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     9932 2022-08-28 04:25:37.000000 hn2016_falwa-0.6.6/hn2016_falwa/utilities.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)    23544 2022-08-28 04:25:29.000000 hn2016_falwa-0.6.6/hn2016_falwa/wrapper.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)    28059 2023-01-17 16:56:08.000000 hn2016_falwa-0.6.6/hn2016_falwa/xarrayinterface.py
+drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-04-09 19:51:08.561802 hn2016_falwa-0.6.6/hn2016_falwa.egg-info/
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     1320 2023-04-09 19:51:08.000000 hn2016_falwa-0.6.6/hn2016_falwa.egg-info/PKG-INFO
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     1214 2023-04-09 19:51:08.000000 hn2016_falwa-0.6.6/hn2016_falwa.egg-info/SOURCES.txt
+-rw-r--r--   0 claresyhuang   (501) staff       (20)        1 2023-04-09 19:51:08.000000 hn2016_falwa-0.6.6/hn2016_falwa.egg-info/dependency_links.txt
+-rw-r--r--   0 claresyhuang   (501) staff       (20)        1 2023-04-09 19:51:08.000000 hn2016_falwa-0.6.6/hn2016_falwa.egg-info/not-zip-safe
+-rw-r--r--   0 claresyhuang   (501) staff       (20)       19 2023-04-09 19:51:08.000000 hn2016_falwa-0.6.6/hn2016_falwa.egg-info/requires.txt
+-rw-r--r--   0 claresyhuang   (501) staff       (20)       19 2023-04-09 19:51:08.000000 hn2016_falwa-0.6.6/hn2016_falwa.egg-info/top_level.txt
+-rw-r--r--   0 claresyhuang   (501) staff       (20)       38 2023-04-09 19:51:08.771025 hn2016_falwa-0.6.6/setup.cfg
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     3511 2023-04-09 19:49:59.000000 hn2016_falwa-0.6.6/setup.py
+drwxr-xr-x   0 claresyhuang   (501) staff       (20)        0 2023-04-09 19:51:08.761498 hn2016_falwa-0.6.6/tests/
+-rw-r--r--   0 claresyhuang   (501) staff       (20)        0 2020-03-01 18:39:03.000000 hn2016_falwa-0.6.6/tests/__init__.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)        1 2020-03-01 18:39:03.000000 hn2016_falwa-0.6.6/tests/conftest.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     3839 2021-08-15 20:17:11.000000 hn2016_falwa-0.6.6/tests/test_barotropic_field.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     2063 2020-03-01 18:39:03.000000 hn2016_falwa-0.6.6/tests/test_basis.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)    10170 2023-04-07 01:45:01.000000 hn2016_falwa-0.6.6/tests/test_oopinterface.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     1167 2020-03-01 18:39:03.000000 hn2016_falwa-0.6.6/tests/test_utilities.py
+-rw-r--r--   0 claresyhuang   (501) staff       (20)     5643 2022-08-28 03:20:26.000000 hn2016_falwa-0.6.6/tests/test_xarrayinterface.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hn2016_falwa-0.6.5/PKG-INFO` & `hn2016_falwa-0.6.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: hn2016_falwa
-Version: 0.6.5
+Version: 0.6.6
 Summary: python package to compute finite-amplitude local wave activity (Huang and Nakamura 2016, JAS)
 Home-page: https://github.com/csyhuang/hn2016_falwa
 Author: Clare S. Y. Huang
-Author-email: csyhuang@protonmail.com
+Author-email: csyhuang@uchicago.edu
 License: MIT
-Description: 
-            hn2016_falwa is a package that contains modules to compute the finite-amplitude
-            local wave activity (FALWA) and reference state (U_ref) in the following papers:
-            Huang and Nakamura (2016, JAS): http://dx.doi.org/10.1175/JAS-D-15-0194.1
-            Huang and Nakamura (2017, GRL): http://onlinelibrary.wiley.com/doi/10.1002/2017GL073760/full
-            Nakamura and Huang (2018, Science): https://doi.org/10.1126/science.aat0721
-            Neal et al (submitted to GRL.)
-        
-            The current version of the library handles calculation of FALWA in a spherical barotropic model and QGPV fields on 
-            isobaric surfaces.
-            
-            The functions in this library can compute the tracer equivalent-latitude relationship
-            proposed in Nakamura (1996) (Also, see Allen and Nakamura (2003)) and the (zonal mean)
-            finite-amplitude wave activity in spherical geometry as in Nakamura and Solomon (2010).
-            
-            Links:    
-            - Source code: http://github.com/csyhuang/hn2016_falwa/
-            
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+
+    hn2016_falwa is a package that contains modules to compute the finite-amplitude
+    local wave activity (FALWA) and reference state (U_ref) in the following papers:
+    Huang and Nakamura (2016, JAS): http://dx.doi.org/10.1175/JAS-D-15-0194.1
+    Huang and Nakamura (2017, GRL): http://onlinelibrary.wiley.com/doi/10.1002/2017GL073760/full
+    Nakamura and Huang (2018, Science): https://doi.org/10.1126/science.aat0721
+    Neal et al (submitted to GRL.)
+
+    The current version of the library handles calculation of FALWA in a spherical barotropic model and QGPV fields on 
+    isobaric surfaces.
+    
+    The functions in this library can compute the tracer equivalent-latitude relationship
+    proposed in Nakamura (1996) (Also, see Allen and Nakamura (2003)) and the (zonal mean)
+    finite-amplitude wave activity in spherical geometry as in Nakamura and Solomon (2010).
+    
+    Links:    
+    - Source code: http://github.com/csyhuang/hn2016_falwa/
+
```

### Comparing `hn2016_falwa-0.6.5/hn2016_falwa/__init__.py` & `hn2016_falwa-0.6.6/hn2016_falwa/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 ------------------------------------------
 File name: __init__.py
 Author: Clare Huang, Christopher Polster
 """
 
-__version__ = "0.6.5"
+__version__ = "0.6.6"
 from .interpolate_fields import interpolate_fields
 from .interpolate_fields_direct_inv import interpolate_fields_direct_inv
 from .compute_qref_and_fawa_first import compute_qref_and_fawa_first
 from .matrix_b4_inversion import matrix_b4_inversion
 from .matrix_after_inversion import matrix_after_inversion
 from .upward_sweep import upward_sweep
 from .compute_reference_states import compute_reference_states
```

### Comparing `hn2016_falwa-0.6.5/hn2016_falwa/barotropic_field.py` & `hn2016_falwa-0.6.6/hn2016_falwa/barotropic_field.py`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/hn2016_falwa/basis.py` & `hn2016_falwa-0.6.6/hn2016_falwa/basis.py`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/hn2016_falwa/f90_modules/compute_flux_dirinv.f90` & `hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/compute_flux_dirinv.f90`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/hn2016_falwa/f90_modules/compute_lwa_and_barotropic_fluxes.f90` & `hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/compute_lwa_and_barotropic_fluxes.f90`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/hn2016_falwa/f90_modules/compute_qref_and_fawa_first.f90` & `hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/compute_qref_and_fawa_first.f90`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/hn2016_falwa/f90_modules/compute_reference_states.f90` & `hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/compute_reference_states.f90`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/hn2016_falwa/f90_modules/interpolate_fields.f90` & `hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/interpolate_fields.f90`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/hn2016_falwa/f90_modules/interpolate_fields_dirinv.f90` & `hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/interpolate_fields_dirinv.f90`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/hn2016_falwa/f90_modules/matrix_after_inversion.f90` & `hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/matrix_after_inversion.f90`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/hn2016_falwa/f90_modules/matrix_b4_inversion.f90` & `hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/matrix_b4_inversion.f90`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/hn2016_falwa/f90_modules/upward_sweep.f90` & `hn2016_falwa-0.6.6/hn2016_falwa/f90_modules/upward_sweep.f90`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/hn2016_falwa/legacy/beta_version.py` & `hn2016_falwa-0.6.6/hn2016_falwa/legacy/beta_version.py`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/hn2016_falwa/oopinterface.py` & `hn2016_falwa-0.6.6/hn2016_falwa/oopinterface.py`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/hn2016_falwa/plot_utilities.py` & `hn2016_falwa-0.6.6/hn2016_falwa/plot_utilities.py`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/hn2016_falwa/qgformalism.py` & `hn2016_falwa-0.6.6/hn2016_falwa/qgformalism.py`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/hn2016_falwa/utilities.py` & `hn2016_falwa-0.6.6/hn2016_falwa/utilities.py`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/hn2016_falwa/wrapper.py` & `hn2016_falwa-0.6.6/hn2016_falwa/wrapper.py`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/hn2016_falwa/xarrayinterface.py` & `hn2016_falwa-0.6.6/hn2016_falwa/xarrayinterface.py`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/hn2016_falwa.egg-info/PKG-INFO` & `hn2016_falwa-0.6.6/hn2016_falwa.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: hn2016-falwa
-Version: 0.6.5
+Version: 0.6.6
 Summary: python package to compute finite-amplitude local wave activity (Huang and Nakamura 2016, JAS)
 Home-page: https://github.com/csyhuang/hn2016_falwa
 Author: Clare S. Y. Huang
-Author-email: csyhuang@protonmail.com
+Author-email: csyhuang@uchicago.edu
 License: MIT
-Description: 
-            hn2016_falwa is a package that contains modules to compute the finite-amplitude
-            local wave activity (FALWA) and reference state (U_ref) in the following papers:
-            Huang and Nakamura (2016, JAS): http://dx.doi.org/10.1175/JAS-D-15-0194.1
-            Huang and Nakamura (2017, GRL): http://onlinelibrary.wiley.com/doi/10.1002/2017GL073760/full
-            Nakamura and Huang (2018, Science): https://doi.org/10.1126/science.aat0721
-            Neal et al (submitted to GRL.)
-        
-            The current version of the library handles calculation of FALWA in a spherical barotropic model and QGPV fields on 
-            isobaric surfaces.
-            
-            The functions in this library can compute the tracer equivalent-latitude relationship
-            proposed in Nakamura (1996) (Also, see Allen and Nakamura (2003)) and the (zonal mean)
-            finite-amplitude wave activity in spherical geometry as in Nakamura and Solomon (2010).
-            
-            Links:    
-            - Source code: http://github.com/csyhuang/hn2016_falwa/
-            
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+
+    hn2016_falwa is a package that contains modules to compute the finite-amplitude
+    local wave activity (FALWA) and reference state (U_ref) in the following papers:
+    Huang and Nakamura (2016, JAS): http://dx.doi.org/10.1175/JAS-D-15-0194.1
+    Huang and Nakamura (2017, GRL): http://onlinelibrary.wiley.com/doi/10.1002/2017GL073760/full
+    Nakamura and Huang (2018, Science): https://doi.org/10.1126/science.aat0721
+    Neal et al (submitted to GRL.)
+
+    The current version of the library handles calculation of FALWA in a spherical barotropic model and QGPV fields on 
+    isobaric surfaces.
+    
+    The functions in this library can compute the tracer equivalent-latitude relationship
+    proposed in Nakamura (1996) (Also, see Allen and Nakamura (2003)) and the (zonal mean)
+    finite-amplitude wave activity in spherical geometry as in Nakamura and Solomon (2010).
+    
+    Links:    
+    - Source code: http://github.com/csyhuang/hn2016_falwa/
+
```

### Comparing `hn2016_falwa-0.6.5/hn2016_falwa.egg-info/SOURCES.txt` & `hn2016_falwa-0.6.6/hn2016_falwa.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 setup.py
 hn2016_falwa/__init__.py
 hn2016_falwa/barotropic_field.py
 hn2016_falwa/basis.py
 hn2016_falwa/constant.py
 hn2016_falwa/oopinterface.py
 hn2016_falwa/plot_utilities.py
```

### Comparing `hn2016_falwa-0.6.5/setup.py` & `hn2016_falwa-0.6.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,21 +56,21 @@
 
 ext9 = Extension(name='hn2016_falwa.compute_flux_dirinv',
                  sources=['hn2016_falwa/f90_modules/compute_flux_dirinv.f90'],
                  f2py_options=['--quiet'])
 
 setup(
     name='hn2016_falwa',
-    version='0.6.5',
+    version='0.6.6',
     description='python package to compute finite-amplitude local wave activity (Huang and Nakamura 2016, JAS)',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     url='https://github.com/csyhuang/hn2016_falwa',
     author='Clare S. Y. Huang',
-    author_email='csyhuang@protonmail.com',
+    author_email='csyhuang@uchicago.edu',
     license='MIT',
     packages=find_packages(),
     install_requires=['numpy', 'scipy', 'xarray'],
     setup_requires=['pytest-runner'],
     tests_require=['pytest'],
     test_suite="tests",
     ext_modules=[ext1, ext2, ext3, ext4, ext5, ext6, ext7, ext8, ext9],
```

### Comparing `hn2016_falwa-0.6.5/tests/test_barotropic_field.py` & `hn2016_falwa-0.6.6/tests/test_barotropic_field.py`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/tests/test_basis.py` & `hn2016_falwa-0.6.6/tests/test_basis.py`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/tests/test_oopinterface.py` & `hn2016_falwa-0.6.6/tests/test_oopinterface.py`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/tests/test_utilities.py` & `hn2016_falwa-0.6.6/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `hn2016_falwa-0.6.5/tests/test_xarrayinterface.py` & `hn2016_falwa-0.6.6/tests/test_xarrayinterface.py`

 * *Files identical despite different names*

