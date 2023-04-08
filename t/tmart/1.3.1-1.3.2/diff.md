# Comparing `tmp/tmart-1.3.1.tar.gz` & `tmp/tmart-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmart-1.3.1.tar", last modified: Mon Apr  3 05:41:21 2023, max compression
+gzip compressed data, was "tmart-1.3.2.tar", last modified: Sat Apr  8 22:51:28 2023, max compression
```

## Comparing `tmart-1.3.1.tar` & `tmart-1.3.2.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-03 05:41:21.038704 tmart-1.3.1/
--rw-r--r--   0 yw         (501) staff       (20)       45 2022-09-20 16:15:46.000000 tmart-1.3.1/MANIFEST.in
--rw-r--r--   0 yw         (501) staff       (20)     3803 2023-04-03 05:41:21.038489 tmart-1.3.1/PKG-INFO
--rw-r--r--   0 yw         (501) staff       (20)     3181 2023-04-03 04:04:03.000000 tmart-1.3.1/README.md
--rw-r--r--   0 yw         (501) staff       (20)       38 2023-04-03 05:41:21.038766 tmart-1.3.1/setup.cfg
--rw-r--r--   0 yw         (501) staff       (20)     1956 2023-04-03 05:39:18.000000 tmart-1.3.1/setup.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-03 05:41:21.021914 tmart-1.3.1/tests/
--rw-r--r--   0 yw         (501) staff       (20)      246 2023-03-29 21:18:48.000000 tmart-1.3.1/tests/test_AEC.py
--rw-r--r--   0 yw         (501) staff       (20)     3048 2023-01-03 02:43:30.000000 tmart-1.3.1/tests/test_E_diffuse.py
--rw-r--r--   0 yw         (501) staff       (20)     2310 2023-01-03 03:48:03.000000 tmart-1.3.1/tests/test_L_sky.py
--rw-r--r--   0 yw         (501) staff       (20)     1827 2023-03-25 22:34:08.000000 tmart-1.3.1/tests/test_basic.py
--rw-r--r--   0 yw         (501) staff       (20)     1327 2022-09-21 16:59:26.000000 tmart-1.3.1/tests/test_basic_import.py
--rw-r--r--   0 yw         (501) staff       (20)     3197 2022-09-17 14:43:02.000000 tmart-1.3.1/tests/test_calcref.py
--rw-r--r--   0 yw         (501) staff       (20)     2993 2023-03-25 22:34:08.000000 tmart-1.3.1/tests/test_quickstart.py
--rw-r--r--   0 yw         (501) staff       (20)     3113 2022-09-26 04:25:24.000000 tmart-1.3.1/tests/test_specular_contribution.py
--rw-r--r--   0 yw         (501) staff       (20)     3228 2022-09-27 15:07:16.000000 tmart-1.3.1/tests/test_typical_ocean.py
--rw-r--r--   0 yw         (501) staff       (20)     3021 2022-10-03 05:42:50.000000 tmart-1.3.1/tests/test_whales_SR.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-03 05:41:21.026012 tmart-1.3.1/tmart/
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-03 05:41:21.027320 tmart-1.3.1/tmart/AEC/
--rw-r--r--   0 yw         (501) staff       (20)      345 2023-03-29 21:15:27.000000 tmart-1.3.1/tmart/AEC/__init__.py
--rw-r--r--   0 yw         (501) staff       (20)     5528 2023-04-03 00:52:28.000000 tmart-1.3.1/tmart/AEC/get_parameters.py
--rw-r--r--   0 yw         (501) staff       (20)     2319 2022-09-17 14:42:06.000000 tmart-1.3.1/tmart/Aerosol.py
--rw-r--r--   0 yw         (501) staff       (20)    10525 2023-03-24 23:31:27.000000 tmart-1.3.1/tmart/Atmosphere.py
--rw-r--r--   0 yw         (501) staff       (20)    10103 2022-12-20 19:47:51.000000 tmart-1.3.1/tmart/Surface.py
--rw-r--r--   0 yw         (501) staff       (20)    13618 2023-04-03 00:51:14.000000 tmart-1.3.1/tmart/Tmart.py
--rw-r--r--   0 yw         (501) staff       (20)    41659 2023-03-24 23:59:45.000000 tmart-1.3.1/tmart/Tmart2.py
--rw-r--r--   0 yw         (501) staff       (20)      521 2023-03-29 21:15:26.000000 tmart-1.3.1/tmart/__init__.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-03 05:41:21.030627 tmart-1.3.1/tmart/ancillary/
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-03 05:41:21.037175 tmart-1.3.1/tmart/ancillary/aerosolSPF/
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:20:25.000000 tmart-1.3.1/tmart/ancillary/aerosolSPF/BiomassBurning.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:49:56.000000 tmart-1.3.1/tmart/ancillary/aerosolSPF/Continental.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:55:10.000000 tmart-1.3.1/tmart/ancillary/aerosolSPF/Desert.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 16:59:28.000000 tmart-1.3.1/tmart/ancillary/aerosolSPF/Maritime.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:21:44.000000 tmart-1.3.1/tmart/ancillary/aerosolSPF/Stratospheric.csv
--rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:53:59.000000 tmart-1.3.1/tmart/ancillary/aerosolSPF/Urban.csv
--rw-r--r--   0 yw         (501) staff       (20)     1763 2022-12-14 22:44:42.000000 tmart-1.3.1/tmart/ancillary/conifer_forest.csv
--rw-r--r--   0 yw         (501) staff       (20)      838 2022-12-14 22:45:12.000000 tmart-1.3.1/tmart/ancillary/dry_beach_sand.csv
--rw-r--r--   0 yw         (501) staff       (20)     1618 2022-12-14 22:45:48.000000 tmart-1.3.1/tmart/ancillary/lawn_grass.csv
--rw-r--r--   0 yw         (501) staff       (20)      794 2021-08-03 20:21:41.000000 tmart-1.3.1/tmart/ancillary/soil.csv
--rw-r--r--   0 yw         (501) staff       (20)     1190 2021-08-03 20:22:22.000000 tmart-1.3.1/tmart/ancillary/vegetation.csv
--rw-r--r--   0 yw         (501) staff       (20)      284 2021-08-03 20:21:58.000000 tmart-1.3.1/tmart/ancillary/water.csv
--rw-r--r--   0 yw         (501) staff       (20)      707 2022-02-08 17:04:47.000000 tmart-1.3.1/tmart/ancillary/water_chl1.csv
--rw-r--r--   0 yw         (501) staff       (20)     1015 2022-12-14 22:46:19.000000 tmart-1.3.1/tmart/ancillary/wet_beach_sand.csv
--rw-r--r--   0 yw         (501) staff       (20)      181 2023-03-31 22:46:09.000000 tmart-1.3.1/tmart/ancillary/whitecap_factor.csv
--rw-r--r--   0 yw         (501) staff       (20)     2683 2022-09-17 14:41:21.000000 tmart-1.3.1/tmart/tm_OT.py
--rw-r--r--   0 yw         (501) staff       (20)    11781 2022-10-20 22:04:09.000000 tmart-1.3.1/tmart/tm_calcref.py
--rw-r--r--   0 yw         (501) staff       (20)     4093 2022-09-17 14:42:43.000000 tmart-1.3.1/tmart/tm_geometry.py
--rw-r--r--   0 yw         (501) staff       (20)    19398 2022-10-28 20:06:07.000000 tmart-1.3.1/tmart/tm_intersect.py
--rw-r--r--   0 yw         (501) staff       (20)    11288 2022-09-17 14:42:43.000000 tmart-1.3.1/tmart/tm_move.py
--rw-r--r--   0 yw         (501) staff       (20)     8648 2022-09-17 14:41:21.000000 tmart-1.3.1/tmart/tm_sampling.py
--rw-r--r--   0 yw         (501) staff       (20)    20017 2022-11-21 03:09:44.000000 tmart-1.3.1/tmart/tm_water.py
-drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-03 05:41:21.026919 tmart-1.3.1/tmart.egg-info/
--rw-r--r--   0 yw         (501) staff       (20)     3803 2023-04-03 05:41:20.000000 tmart-1.3.1/tmart.egg-info/PKG-INFO
--rw-r--r--   0 yw         (501) staff       (20)     1239 2023-04-03 05:41:20.000000 tmart-1.3.1/tmart.egg-info/SOURCES.txt
--rw-r--r--   0 yw         (501) staff       (20)        1 2023-04-03 05:41:20.000000 tmart-1.3.1/tmart.egg-info/dependency_links.txt
--rw-r--r--   0 yw         (501) staff       (20)       42 2023-04-03 05:41:20.000000 tmart-1.3.1/tmart.egg-info/requires.txt
--rw-r--r--   0 yw         (501) staff       (20)        6 2023-04-03 05:41:20.000000 tmart-1.3.1/tmart.egg-info/top_level.txt
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-08 22:51:28.385299 tmart-1.3.2/
+-rw-r--r--   0 yw         (501) staff       (20)       45 2022-09-20 16:15:46.000000 tmart-1.3.2/MANIFEST.in
+-rw-r--r--   0 yw         (501) staff       (20)     3803 2023-04-08 22:51:28.385064 tmart-1.3.2/PKG-INFO
+-rw-r--r--   0 yw         (501) staff       (20)     3181 2023-04-03 04:04:03.000000 tmart-1.3.2/README.md
+-rw-r--r--   0 yw         (501) staff       (20)       38 2023-04-08 22:51:28.385380 tmart-1.3.2/setup.cfg
+-rw-r--r--   0 yw         (501) staff       (20)     1966 2023-04-08 22:46:54.000000 tmart-1.3.2/setup.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-08 22:51:28.370787 tmart-1.3.2/tests/
+-rw-r--r--   0 yw         (501) staff       (20)      246 2023-03-29 21:18:48.000000 tmart-1.3.2/tests/test_AEC.py
+-rw-r--r--   0 yw         (501) staff       (20)     3048 2023-01-03 02:43:30.000000 tmart-1.3.2/tests/test_E_diffuse.py
+-rw-r--r--   0 yw         (501) staff       (20)     2310 2023-01-03 03:48:03.000000 tmart-1.3.2/tests/test_L_sky.py
+-rw-r--r--   0 yw         (501) staff       (20)     1827 2023-03-25 22:34:08.000000 tmart-1.3.2/tests/test_basic.py
+-rw-r--r--   0 yw         (501) staff       (20)     1327 2022-09-21 16:59:26.000000 tmart-1.3.2/tests/test_basic_import.py
+-rw-r--r--   0 yw         (501) staff       (20)     3197 2022-09-17 14:43:02.000000 tmart-1.3.2/tests/test_calcref.py
+-rw-r--r--   0 yw         (501) staff       (20)     2993 2023-03-25 22:34:08.000000 tmart-1.3.2/tests/test_quickstart.py
+-rw-r--r--   0 yw         (501) staff       (20)     3113 2022-09-26 04:25:24.000000 tmart-1.3.2/tests/test_specular_contribution.py
+-rw-r--r--   0 yw         (501) staff       (20)     3228 2022-09-27 15:07:16.000000 tmart-1.3.2/tests/test_typical_ocean.py
+-rw-r--r--   0 yw         (501) staff       (20)     3021 2022-10-03 05:42:50.000000 tmart-1.3.2/tests/test_whales_SR.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-08 22:51:28.372704 tmart-1.3.2/tmart/
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-08 22:51:28.373771 tmart-1.3.2/tmart/AEC/
+-rw-r--r--   0 yw         (501) staff       (20)      382 2023-04-08 19:19:35.000000 tmart-1.3.2/tmart/AEC/__init__.py
+-rw-r--r--   0 yw         (501) staff       (20)     5531 2023-04-08 22:45:49.000000 tmart-1.3.2/tmart/AEC/get_parameters.py
+-rw-r--r--   0 yw         (501) staff       (20)     2753 2023-04-08 21:44:12.000000 tmart-1.3.2/tmart/AEC/reflectance_correction.py
+-rw-r--r--   0 yw         (501) staff       (20)     2320 2023-04-08 22:49:14.000000 tmart-1.3.2/tmart/Aerosol.py
+-rw-r--r--   0 yw         (501) staff       (20)    10526 2023-04-08 22:49:20.000000 tmart-1.3.2/tmart/Atmosphere.py
+-rw-r--r--   0 yw         (501) staff       (20)    10104 2023-04-08 22:49:24.000000 tmart-1.3.2/tmart/Surface.py
+-rw-r--r--   0 yw         (501) staff       (20)    13619 2023-04-08 22:50:39.000000 tmart-1.3.2/tmart/Tmart.py
+-rw-r--r--   0 yw         (501) staff       (20)    41660 2023-04-08 22:50:38.000000 tmart-1.3.2/tmart/Tmart2.py
+-rw-r--r--   0 yw         (501) staff       (20)      522 2023-04-08 22:49:15.000000 tmart-1.3.2/tmart/__init__.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-08 22:51:28.376500 tmart-1.3.2/tmart/ancillary/
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-08 22:51:28.383610 tmart-1.3.2/tmart/ancillary/aerosolSPF/
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:20:25.000000 tmart-1.3.2/tmart/ancillary/aerosolSPF/BiomassBurning.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:49:56.000000 tmart-1.3.2/tmart/ancillary/aerosolSPF/Continental.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:55:10.000000 tmart-1.3.2/tmart/ancillary/aerosolSPF/Desert.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 16:59:28.000000 tmart-1.3.2/tmart/ancillary/aerosolSPF/Maritime.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 20:21:44.000000 tmart-1.3.2/tmart/ancillary/aerosolSPF/Stratospheric.csv
+-rw-r--r--   0 yw         (501) staff       (20)   399399 2022-06-05 19:53:59.000000 tmart-1.3.2/tmart/ancillary/aerosolSPF/Urban.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1763 2022-12-14 22:44:42.000000 tmart-1.3.2/tmart/ancillary/conifer_forest.csv
+-rw-r--r--   0 yw         (501) staff       (20)      838 2022-12-14 22:45:12.000000 tmart-1.3.2/tmart/ancillary/dry_beach_sand.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1618 2022-12-14 22:45:48.000000 tmart-1.3.2/tmart/ancillary/lawn_grass.csv
+-rw-r--r--   0 yw         (501) staff       (20)      794 2021-08-03 20:21:41.000000 tmart-1.3.2/tmart/ancillary/soil.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1190 2021-08-03 20:22:22.000000 tmart-1.3.2/tmart/ancillary/vegetation.csv
+-rw-r--r--   0 yw         (501) staff       (20)      284 2021-08-03 20:21:58.000000 tmart-1.3.2/tmart/ancillary/water.csv
+-rw-r--r--   0 yw         (501) staff       (20)      707 2022-02-08 17:04:47.000000 tmart-1.3.2/tmart/ancillary/water_chl1.csv
+-rw-r--r--   0 yw         (501) staff       (20)     1015 2022-12-14 22:46:19.000000 tmart-1.3.2/tmart/ancillary/wet_beach_sand.csv
+-rw-r--r--   0 yw         (501) staff       (20)      181 2023-03-31 22:46:09.000000 tmart-1.3.2/tmart/ancillary/whitecap_factor.csv
+-rw-r--r--   0 yw         (501) staff       (20)     2684 2023-04-08 22:50:41.000000 tmart-1.3.2/tmart/tm_OT.py
+-rw-r--r--   0 yw         (501) staff       (20)    11784 2023-04-08 22:49:35.000000 tmart-1.3.2/tmart/tm_calcref.py
+-rw-r--r--   0 yw         (501) staff       (20)     4094 2023-04-08 22:49:45.000000 tmart-1.3.2/tmart/tm_geometry.py
+-rw-r--r--   0 yw         (501) staff       (20)    19399 2023-04-08 22:49:52.000000 tmart-1.3.2/tmart/tm_intersect.py
+-rw-r--r--   0 yw         (501) staff       (20)    11289 2023-04-08 22:50:00.000000 tmart-1.3.2/tmart/tm_move.py
+-rw-r--r--   0 yw         (501) staff       (20)     8649 2023-04-08 22:50:40.000000 tmart-1.3.2/tmart/tm_sampling.py
+-rw-r--r--   0 yw         (501) staff       (20)    20018 2023-04-08 22:50:39.000000 tmart-1.3.2/tmart/tm_water.py
+drwxr-xr-x   0 yw         (501) staff       (20)        0 2023-04-08 22:51:28.373372 tmart-1.3.2/tmart.egg-info/
+-rw-r--r--   0 yw         (501) staff       (20)     3803 2023-04-08 22:51:28.000000 tmart-1.3.2/tmart.egg-info/PKG-INFO
+-rw-r--r--   0 yw         (501) staff       (20)     1275 2023-04-08 22:51:28.000000 tmart-1.3.2/tmart.egg-info/SOURCES.txt
+-rw-r--r--   0 yw         (501) staff       (20)        1 2023-04-08 22:51:28.000000 tmart-1.3.2/tmart.egg-info/dependency_links.txt
+-rw-r--r--   0 yw         (501) staff       (20)       50 2023-04-08 22:51:28.000000 tmart-1.3.2/tmart.egg-info/requires.txt
+-rw-r--r--   0 yw         (501) staff       (20)        6 2023-04-08 22:51:28.000000 tmart-1.3.2/tmart.egg-info/top_level.txt
```

### Comparing `tmart-1.3.1/PKG-INFO` & `tmart-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmart
-Version: 1.3.1
+Version: 1.3.2
 Summary: Radiative transfer modelling for aquatic remote sensing
 Author: Yulun Wu
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tmart Version: 1.3.1 Summary: Radiative transfer
+Metadata-Version: 2.1 Name: tmart Version: 1.3.2 Summary: Radiative transfer
 modelling for aquatic remote sensing Author: Yulun Wu Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering ::
 Atmospheric Science Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
```

### Comparing `tmart-1.3.1/README.md` & `tmart-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/setup.py` & `tmart-1.3.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tmart",                     # This is the name of the package
-    version="1.3.1",                       
+    version="1.3.2",                       
     author="Yulun Wu",                     # Full name of the author
     description="Radiative transfer modelling for aquatic remote sensing",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     # packages=setuptools.find_packages(),    # List of all python modules to be installed
     packages = ['tmart','tmart.AEC','tmart.ancillary','tmart.ancillary.aerosolSPF'],
     include_package_data=True,
@@ -35,9 +35,9 @@
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.6',                # Minimum version requirement of the package
     # py_modules=["tmart"],             # Name of the python package
     # package_dir={'':'tmart/'},     # Directory of the source code of the package
     license_files=('license.txt'),
-    install_requires=['Py6S','numpy','pandas','scipy','pathos','matplotlib']  # Install other dependencies if any
+    install_requires=['Py6S','numpy','pandas','scipy','pathos','matplotlib','netCDF4']  # Install other dependencies if any
 )
```

### Comparing `tmart-1.3.1/tests/test_E_diffuse.py` & `tmart-1.3.2/tests/test_E_diffuse.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tests/test_L_sky.py` & `tmart-1.3.2/tests/test_L_sky.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tests/test_basic.py` & `tmart-1.3.2/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tests/test_basic_import.py` & `tmart-1.3.2/tests/test_basic_import.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tests/test_calcref.py` & `tmart-1.3.2/tests/test_calcref.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tests/test_quickstart.py` & `tmart-1.3.2/tests/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tests/test_specular_contribution.py` & `tmart-1.3.2/tests/test_specular_contribution.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tests/test_typical_ocean.py` & `tmart-1.3.2/tests/test_typical_ocean.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tests/test_whales_SR.py` & `tmart-1.3.2/tests/test_whales_SR.py`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tmart/AEC/get_parameters.py` & `tmart-1.3.2/tmart/AEC/get_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # This file is part of TMart.
 #
 # Copyright 2023 Yulun Wu.
 #
-# TMart is free software: you can redistribute it and/or modify
+# T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 
 ### Derive AE correction parameters 
 
-def get_parameters(n_photon = 10_000, SR_avg = 1, wl = 833, band = None, 
+def get_parameters(n_photon = 10_000, SR_avg = 0.5, wl = 833, band = None, 
         target_pt_direction=[180,0], sun_dir=[0,0], 
         atm_profile = None, 
         aerosol_type = 'Maritime', aot550 = 0.2, 
         cell_size = 100,window_size = None,
         window_size_x = None, window_size_y = None):
```

### Comparing `tmart-1.3.1/tmart/Aerosol.py` & `tmart-1.3.2/tmart/Aerosol.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file is part of TMart.
 #
 # Copyright 2022 Yulun Wu.
 #
-# TMart is free software: you can redistribute it and/or modify
+# T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `tmart-1.3.1/tmart/Atmosphere.py` & `tmart-1.3.2/tmart/Atmosphere.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file is part of TMart.
 #
 # Copyright 2022 Yulun Wu.
 #
-# TMart is free software: you can redistribute it and/or modify
+# T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `tmart-1.3.1/tmart/Surface.py` & `tmart-1.3.2/tmart/Surface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file is part of TMart.
 #
 # Copyright 2022 Yulun Wu.
 #
-# TMart is free software: you can redistribute it and/or modify
+# T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 
 # Surface object
```

### Comparing `tmart-1.3.1/tmart/Tmart.py` & `tmart-1.3.2/tmart/Tmart.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file is part of TMart.
 #
 # Copyright 2022 Yulun Wu.
 #
-# TMart is free software: you can redistribute it and/or modify
+# T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `tmart-1.3.1/tmart/Tmart2.py` & `tmart-1.3.2/tmart/Tmart2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file is part of TMart.
 #
 # Copyright 2022 Yulun Wu.
 #
-# TMart is free software: you can redistribute it and/or modify
+# T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `tmart-1.3.1/tmart/__init__.py` & `tmart-1.3.2/tmart/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file is part of TMart.
 #
 # Copyright 2022 Yulun Wu.
 #
-# TMart is free software: you can redistribute it and/or modify
+# T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `tmart-1.3.1/tmart/ancillary/aerosolSPF/BiomassBurning.csv` & `tmart-1.3.2/tmart/ancillary/aerosolSPF/BiomassBurning.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tmart/ancillary/aerosolSPF/Continental.csv` & `tmart-1.3.2/tmart/ancillary/aerosolSPF/Continental.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tmart/ancillary/aerosolSPF/Desert.csv` & `tmart-1.3.2/tmart/ancillary/aerosolSPF/Desert.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tmart/ancillary/aerosolSPF/Maritime.csv` & `tmart-1.3.2/tmart/ancillary/aerosolSPF/Maritime.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tmart/ancillary/aerosolSPF/Stratospheric.csv` & `tmart-1.3.2/tmart/ancillary/aerosolSPF/Stratospheric.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tmart/ancillary/aerosolSPF/Urban.csv` & `tmart-1.3.2/tmart/ancillary/aerosolSPF/Urban.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tmart/ancillary/conifer_forest.csv` & `tmart-1.3.2/tmart/ancillary/conifer_forest.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tmart/ancillary/dry_beach_sand.csv` & `tmart-1.3.2/tmart/ancillary/dry_beach_sand.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tmart/ancillary/lawn_grass.csv` & `tmart-1.3.2/tmart/ancillary/lawn_grass.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tmart/ancillary/soil.csv` & `tmart-1.3.2/tmart/ancillary/soil.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tmart/ancillary/vegetation.csv` & `tmart-1.3.2/tmart/ancillary/vegetation.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tmart/ancillary/water_chl1.csv` & `tmart-1.3.2/tmart/ancillary/water_chl1.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tmart/ancillary/wet_beach_sand.csv` & `tmart-1.3.2/tmart/ancillary/wet_beach_sand.csv`

 * *Files identical despite different names*

### Comparing `tmart-1.3.1/tmart/tm_OT.py` & `tmart-1.3.2/tmart/tm_OT.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file is part of TMart.
 #
 # Copyright 2022 Yulun Wu.
 #
-# TMart is free software: you can redistribute it and/or modify
+# T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `tmart-1.3.1/tmart/tm_calcref.py` & `tmart-1.3.2/tmart/tm_calcref.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file is part of TMart.
 #
 # Copyright 2022 Yulun Wu.
 #
-# TMart is free software: you can redistribute it and/or modify
+# T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 
 
 
@@ -41,15 +41,15 @@
       R = tmart.calc_ref(results)
       for k, v in R.items():
           print(k, '\t ' , v)
 
     '''
     
     print('=====================================')
-    print('Calculating radiative properties...')
+    print('Calculating radiometric quantities...')
     
     # Columes: 0 pt_id, 1 movement, 2 L_cox-munk, 3 L_whitecap, 4 L_water, 5 L_land, 
     # 6 L_rayleigh, 7 L_mie, 8 9 10 surface xyz, 11 shadowed, 12 if_env
```

### Comparing `tmart-1.3.1/tmart/tm_geometry.py` & `tmart-1.3.2/tmart/tm_geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file is part of TMart.
 #
 # Copyright 2022 Yulun Wu.
 #
-# TMart is free software: you can redistribute it and/or modify
+# T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 
 # Geometry
```

### Comparing `tmart-1.3.1/tmart/tm_intersect.py` & `tmart-1.3.2/tmart/tm_intersect.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file is part of TMart.
 #
 # Copyright 2022 Yulun Wu.
 #
-# TMart is free software: you can redistribute it and/or modify
+# T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 
 
 # intersect
```

### Comparing `tmart-1.3.1/tmart/tm_move.py` & `tmart-1.3.2/tmart/tm_move.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file is part of TMart.
 #
 # Copyright 2022 Yulun Wu.
 #
-# TMart is free software: you can redistribute it and/or modify
+# T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `tmart-1.3.1/tmart/tm_sampling.py` & `tmart-1.3.2/tmart/tm_sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file is part of TMart.
 #
 # Copyright 2022 Yulun Wu.
 #
-# TMart is free software: you can redistribute it and/or modify
+# T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `tmart-1.3.1/tmart/tm_water.py` & `tmart-1.3.2/tmart/tm_water.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file is part of TMart.
 #
 # Copyright 2022 Yulun Wu.
 #
-# TMart is free software: you can redistribute it and/or modify
+# T-Mart is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `tmart-1.3.1/tmart.egg-info/PKG-INFO` & `tmart-1.3.2/tmart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmart
-Version: 1.3.1
+Version: 1.3.2
 Summary: Radiative transfer modelling for aquatic remote sensing
 Author: Yulun Wu
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tmart Version: 1.3.1 Summary: Radiative transfer
+Metadata-Version: 2.1 Name: tmart Version: 1.3.2 Summary: Radiative transfer
 modelling for aquatic remote sensing Author: Yulun Wu Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering ::
 Atmospheric Science Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
```

### Comparing `tmart-1.3.1/tmart.egg-info/SOURCES.txt` & `tmart-1.3.2/tmart.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 tmart.egg-info/PKG-INFO
 tmart.egg-info/SOURCES.txt
 tmart.egg-info/dependency_links.txt
 tmart.egg-info/requires.txt
 tmart.egg-info/top_level.txt
 tmart/AEC/__init__.py
 tmart/AEC/get_parameters.py
+tmart/AEC/reflectance_correction.py
 tmart/ancillary/conifer_forest.csv
 tmart/ancillary/dry_beach_sand.csv
 tmart/ancillary/lawn_grass.csv
 tmart/ancillary/soil.csv
 tmart/ancillary/vegetation.csv
 tmart/ancillary/water.csv
 tmart/ancillary/water_chl1.csv
```

