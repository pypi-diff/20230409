# Comparing `tmp/kpLib-1.1.0.tar.gz` & `tmp/kpLib-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kpLib-1.1.0.tar", last modified: Sun Apr  9 03:28:31 2023, max compression
+gzip compressed data, was "kpLib-1.1.1.tar", last modified: Sun Apr  9 05:10:51 2023, max compression
```

## Comparing `kpLib-1.1.0.tar` & `kpLib-1.1.1.tar`

### file list

```diff
@@ -1,25 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 03:28:31.806728 kpLib-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)    10767 2023-04-09 03:27:56.000000 kpLib-1.1.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-04-09 03:27:56.000000 kpLib-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    25972 2023-04-09 03:28:31.805728 kpLib-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    24795 2023-04-09 03:27:56.000000 kpLib-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 03:28:31.798728 kpLib-1.1.0/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 03:28:31.802728 kpLib-1.1.0/python/kpLib/
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-04-09 03:27:56.000000 kpLib-1.1.0/python/kpLib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3301 2023-04-09 03:27:56.000000 kpLib-1.1.0/python/kpLib/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     4245 2023-04-09 03:27:56.000000 kpLib-1.1.0/python/kpLib/interface.cpp
--rw-rw-rw-   0 root         (0) root         (0)     6839 2023-04-09 03:27:56.000000 kpLib-1.1.0/python/kpLib/interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 03:28:31.805728 kpLib-1.1.0/python/kpLib.egg-info/
--rw-r--r--   0 root         (0) root         (0)    25972 2023-04-09 03:28:31.000000 kpLib-1.1.0/python/kpLib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      463 2023-04-09 03:28:31.000000 kpLib-1.1.0/python/kpLib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 03:28:31.000000 kpLib-1.1.0/python/kpLib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-04-09 03:28:31.000000 kpLib-1.1.0/python/kpLib.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 03:28:28.000000 kpLib-1.1.0/python/kpLib.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-09 03:28:31.000000 kpLib-1.1.0/python/kpLib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-09 03:28:31.000000 kpLib-1.1.0/python/kpLib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 03:28:31.806728 kpLib-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2938 2023-04-09 03:27:56.000000 kpLib-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 03:28:31.801728 kpLib-1.1.0/src/
--rw-rw-rw-   0 root         (0) root         (0)     5150 2023-04-09 03:27:56.000000 kpLib-1.1.0/src/kPointLattice.cpp
--rw-rw-rw-   0 root         (0) root         (0)    33024 2023-04-09 03:27:56.000000 kpLib-1.1.0/src/kPointLatticeGenerator.cpp
--rw-rw-rw-   0 root         (0) root         (0)     6788 2023-04-09 03:27:56.000000 kpLib-1.1.0/src/msmath.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 05:10:51.990481 kpLib-1.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)    10767 2023-04-09 05:10:17.000000 kpLib-1.1.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-04-09 05:10:17.000000 kpLib-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    26168 2023-04-09 05:10:51.990481 kpLib-1.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    24991 2023-04-09 05:10:17.000000 kpLib-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 05:10:51.980480 kpLib-1.1.1/demo_kplib/
+-rw-rw-rw-   0 root         (0) root         (0)     1159 2023-04-09 05:10:17.000000 kpLib-1.1.1/demo_kplib/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 05:10:51.980480 kpLib-1.1.1/demo_kplib/include/
+-rw-rw-rw-   0 root         (0) root         (0)    24229 2023-04-09 05:10:17.000000 kpLib-1.1.1/demo_kplib/include/spglib.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 05:10:51.981480 kpLib-1.1.1/demo_kplib/lib/
+-rw-rw-rw-   0 root         (0) root         (0)   387268 2023-04-09 05:10:17.000000 kpLib-1.1.1/demo_kplib/lib/libsymspg.a
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 05:10:51.984480 kpLib-1.1.1/demo_kplib/src/
+-rw-rw-rw-   0 root         (0) root         (0)     1913 2023-04-09 05:10:17.000000 kpLib-1.1.1/demo_kplib/src/main.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     2487 2023-04-09 05:10:17.000000 kpLib-1.1.1/demo_kplib/src/poscar.cpp
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-04-09 05:10:17.000000 kpLib-1.1.1/demo_kplib/src/poscar.h
+-rw-rw-rw-   0 root         (0) root         (0)      914 2023-04-09 05:10:17.000000 kpLib-1.1.1/demo_kplib/src/precalc.cpp
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-09 05:10:17.000000 kpLib-1.1.1/demo_kplib/src/precalc.h
+-rw-rw-rw-   0 root         (0) root         (0)    12086 2023-04-09 05:10:17.000000 kpLib-1.1.1/demo_kplib/src/utils.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1402 2023-04-09 05:10:17.000000 kpLib-1.1.1/demo_kplib/src/utils.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 05:10:51.976480 kpLib-1.1.1/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 05:10:51.985481 kpLib-1.1.1/python/kpLib/
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-04-09 05:10:17.000000 kpLib-1.1.1/python/kpLib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3301 2023-04-09 05:10:17.000000 kpLib-1.1.1/python/kpLib/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     4245 2023-04-09 05:10:17.000000 kpLib-1.1.1/python/kpLib/interface.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     6839 2023-04-09 05:10:17.000000 kpLib-1.1.1/python/kpLib/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 05:10:51.988481 kpLib-1.1.1/python/kpLib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    26168 2023-04-09 05:10:51.000000 kpLib-1.1.1/python/kpLib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      863 2023-04-09 05:10:51.000000 kpLib-1.1.1/python/kpLib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 05:10:51.000000 kpLib-1.1.1/python/kpLib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-04-09 05:10:51.000000 kpLib-1.1.1/python/kpLib.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 05:10:48.000000 kpLib-1.1.1/python/kpLib.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-09 05:10:51.000000 kpLib-1.1.1/python/kpLib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-09 05:10:51.000000 kpLib-1.1.1/python/kpLib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 05:10:51.990481 kpLib-1.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2938 2023-04-09 05:10:17.000000 kpLib-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 05:10:51.989481 kpLib-1.1.1/src/
+-rw-rw-rw-   0 root         (0) root         (0)     5150 2023-04-09 05:10:17.000000 kpLib-1.1.1/src/kPointLattice.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     2984 2023-04-09 05:10:17.000000 kpLib-1.1.1/src/kPointLattice.h
+-rw-rw-rw-   0 root         (0) root         (0)    33024 2023-04-09 05:10:17.000000 kpLib-1.1.1/src/kPointLatticeGenerator.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    10816 2023-04-09 05:10:17.000000 kpLib-1.1.1/src/kPointLatticeGenerator.h
+-rw-rw-rw-   0 root         (0) root         (0)     6788 2023-04-09 05:10:17.000000 kpLib-1.1.1/src/msmath.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     2717 2023-04-09 05:10:17.000000 kpLib-1.1.1/src/msmath.h
+-rw-rw-rw-   0 root         (0) root         (0)     5993 2023-04-09 05:10:17.000000 kpLib-1.1.1/src/msmath.ipp
```

### Comparing `kpLib-1.1.0/LICENSE` & `kpLib-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kpLib-1.1.0/PKG-INFO` & `kpLib-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kpLib
-Version: 1.1.0
+Version: 1.1.1
 Summary: Library for generating highly-efficient generalized Monkhorst-Pack K-point grids to accelerate electronic structure calculations, like DFT.
 Home-page: https://gitlab.com/muellergroup/kplib
 Author: Yunzhe Wang
 Author-email: ywang393@jhu.edu
 License: Apache-2.0
 Keywords: Computational Materials Science,Materials Simulation,Electronic Structure,K-points,kpoint,Density Functional Theory,DFT,VASP,Crystal
 Classifier: Programming Language :: Python :: 3
@@ -83,15 +83,17 @@
 ## Installation
 
 ### **Install from PyPI using `pip`**
 This will install the core KpLib module with minimal third-party dependencies. User will need to parse input structures and write out generated *K*-point grid using their favorite matsci packages (e.g. `ase` and `pymatgen`). 
 
 ```
 $ pip install --user pybind11 build wheel
-$ pip install --user kplib
+$ pip install --user kplib       # Install only the core kplib package. 
+$ pip install --user kplib[cli]  # To install the CLI tool `kpgen`. 
+                                 # This will also install `pymatgen` and `click`
 ```
 
 ### **Install from source using `pip`**
 The Python interface is a thin wrapper of the C++ library. Building from source should be straight forward. It also provides a way to install a CLI command to be called in terminal (requiring `pymatgen` for IO).
 
 
 Step 1. Download source code from https://gitlab.com/muellergroup/kplib.
```

### Comparing `kpLib-1.1.0/README.md` & `kpLib-1.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,17 @@
 ## Installation
 
 ### **Install from PyPI using `pip`**
 This will install the core KpLib module with minimal third-party dependencies. User will need to parse input structures and write out generated *K*-point grid using their favorite matsci packages (e.g. `ase` and `pymatgen`). 
 
 ```
 $ pip install --user pybind11 build wheel
-$ pip install --user kplib
+$ pip install --user kplib       # Install only the core kplib package. 
+$ pip install --user kplib[cli]  # To install the CLI tool `kpgen`. 
+                                 # This will also install `pymatgen` and `click`
 ```
 
 ### **Install from source using `pip`**
 The Python interface is a thin wrapper of the C++ library. Building from source should be straight forward. It also provides a way to install a CLI command to be called in terminal (requiring `pymatgen` for IO).
 
 
 Step 1. Download source code from https://gitlab.com/muellergroup/kplib.
```

### Comparing `kpLib-1.1.0/python/kpLib/cli.py` & `kpLib-1.1.1/python/kpLib/cli.py`

 * *Files identical despite different names*

### Comparing `kpLib-1.1.0/python/kpLib/interface.cpp` & `kpLib-1.1.1/python/kpLib/interface.cpp`

 * *Files identical despite different names*

### Comparing `kpLib-1.1.0/python/kpLib/interface.py` & `kpLib-1.1.1/python/kpLib/interface.py`

 * *Files identical despite different names*

### Comparing `kpLib-1.1.0/python/kpLib.egg-info/PKG-INFO` & `kpLib-1.1.1/python/kpLib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kpLib
-Version: 1.1.0
+Version: 1.1.1
 Summary: Library for generating highly-efficient generalized Monkhorst-Pack K-point grids to accelerate electronic structure calculations, like DFT.
 Home-page: https://gitlab.com/muellergroup/kplib
 Author: Yunzhe Wang
 Author-email: ywang393@jhu.edu
 License: Apache-2.0
 Keywords: Computational Materials Science,Materials Simulation,Electronic Structure,K-points,kpoint,Density Functional Theory,DFT,VASP,Crystal
 Classifier: Programming Language :: Python :: 3
@@ -83,15 +83,17 @@
 ## Installation
 
 ### **Install from PyPI using `pip`**
 This will install the core KpLib module with minimal third-party dependencies. User will need to parse input structures and write out generated *K*-point grid using their favorite matsci packages (e.g. `ase` and `pymatgen`). 
 
 ```
 $ pip install --user pybind11 build wheel
-$ pip install --user kplib
+$ pip install --user kplib       # Install only the core kplib package. 
+$ pip install --user kplib[cli]  # To install the CLI tool `kpgen`. 
+                                 # This will also install `pymatgen` and `click`
 ```
 
 ### **Install from source using `pip`**
 The Python interface is a thin wrapper of the C++ library. Building from source should be straight forward. It also provides a way to install a CLI command to be called in terminal (requiring `pymatgen` for IO).
 
 
 Step 1. Download source code from https://gitlab.com/muellergroup/kplib.
```

### Comparing `kpLib-1.1.0/setup.py` & `kpLib-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 cli_requires = ["pymatgen", "click"]
 
 with open(Path(__file__).parent.joinpath("README.md").resolve()) as f:
     long_description = f.read()
 
 setup(
     name="kpLib", # The name appear in PyPI. Not necessarily the one used in import statement.
-    version="1.1.0",
+    version="1.1.1",
     #use_scm_version={
     #   'version_scheme': 'post-release'
     #},
     author="Yunzhe Wang",
     author_email="ywang393@jhu.edu",
     url="https://gitlab.com/muellergroup/kplib",
     description="Library for generating highly-efficient generalized Monkhorst-Pack K-point grids" \
```

### Comparing `kpLib-1.1.0/src/kPointLattice.cpp` & `kpLib-1.1.1/src/kPointLattice.cpp`

 * *Files identical despite different names*

### Comparing `kpLib-1.1.0/src/kPointLatticeGenerator.cpp` & `kpLib-1.1.1/src/kPointLatticeGenerator.cpp`

 * *Files identical despite different names*

### Comparing `kpLib-1.1.0/src/msmath.cpp` & `kpLib-1.1.1/src/msmath.cpp`

 * *Files identical despite different names*

