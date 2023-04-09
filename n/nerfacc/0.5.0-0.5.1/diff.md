# Comparing `tmp/nerfacc-0.5.0.tar.gz` & `tmp/nerfacc-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/nerfacc/nerfacc/dist/.tmp-neajoesk/nerfacc-0.5.0.tar", last modified: Tue Apr  4 18:11:15 2023, max compression
+gzip compressed data, was "/home/runner/work/nerfacc/nerfacc/dist/.tmp-xeko1dq4/nerfacc-0.5.1.tar", last modified: Sun Apr  9 10:22:38 2023, max compression
```

## Comparing `nerfacc-0.5.0.tar` & `nerfacc-0.5.1.tar`

### file list

```diff
@@ -1,49 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:11:15.000000 nerfacc-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-04 18:10:53.000000 nerfacc-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-04 18:10:53.000000 nerfacc-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-04 18:11:15.000000 nerfacc-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-04-04 18:11:05.000000 nerfacc-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:11:15.000000 nerfacc-0.5.0/nerfacc/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:11:15.000000 nerfacc-0.5.0/nerfacc/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/cuda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/cuda/_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:11:15.000000 nerfacc-0.5.0/nerfacc/cuda/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)    16208 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/cuda/csrc/grid.cu
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:11:15.000000 nerfacc-0.5.0/nerfacc/cuda/csrc/include/
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/cuda/csrc/include/data_spec.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/cuda/csrc/include/data_spec_packed.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/cuda/csrc/include/utils_contraction.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/cuda/csrc/include/utils_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/cuda/csrc/include/utils_grid.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    38908 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/cuda/csrc/include/utils_math.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/cuda/csrc/include/utils_scan.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/cuda/csrc/nerfacc.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/cuda/csrc/pdf.cu
--rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/cuda/csrc/scan.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/data_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:11:15.000000 nerfacc-0.5.0/nerfacc/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/estimators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/estimators/occ_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/estimators/prop_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21810 2023-04-04 18:10:53.000000 nerfacc-0.5.0/nerfacc/volrend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:11:15.000000 nerfacc-0.5.0/nerfacc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-04 18:11:15.000000 nerfacc-0.5.0/nerfacc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-04 18:11:15.000000 nerfacc-0.5.0/nerfacc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 18:11:15.000000 nerfacc-0.5.0/nerfacc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-04 18:11:15.000000 nerfacc-0.5.0/nerfacc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-04 18:11:15.000000 nerfacc-0.5.0/nerfacc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-04 18:11:15.000000 nerfacc-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-04-04 18:10:53.000000 nerfacc-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:11:15.000000 nerfacc-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-04 18:10:53.000000 nerfacc-0.5.0/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-04 18:10:53.000000 nerfacc-0.5.0/tests/test_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-04 18:10:53.000000 nerfacc-0.5.0/tests/test_pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-04-04 18:10:53.000000 nerfacc-0.5.0/tests/test_rendering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-04 18:10:53.000000 nerfacc-0.5.0/tests/test_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:22:38.000000 nerfacc-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-09 10:22:20.000000 nerfacc-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-09 10:22:20.000000 nerfacc-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-09 10:22:38.000000 nerfacc-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-04-09 10:22:31.000000 nerfacc-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cameras2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc/cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/camera.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    16208 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/grid.cu
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/include/data_spec.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/include/data_spec_packed.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_camera.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_contraction.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_cuda.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_grid.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)    38908 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_math.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_scan.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/nerfacc.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/pdf.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/cuda/csrc/scan.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/data_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/estimators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/estimators/occ_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/estimators/prop_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21810 2023-04-09 10:22:20.000000 nerfacc-0.5.1/nerfacc/volrend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-09 10:22:38.000000 nerfacc-0.5.1/nerfacc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-09 10:22:38.000000 nerfacc-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-09 10:22:20.000000 nerfacc-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:22:38.000000 nerfacc-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-09 10:22:20.000000 nerfacc-0.5.1/tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-09 10:22:20.000000 nerfacc-0.5.1/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-09 10:22:20.000000 nerfacc-0.5.1/tests/test_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-09 10:22:20.000000 nerfacc-0.5.1/tests/test_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-04-09 10:22:20.000000 nerfacc-0.5.1/tests/test_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-09 10:22:20.000000 nerfacc-0.5.1/tests/test_scan.py
```

### Comparing `nerfacc-0.5.0/LICENSE` & `nerfacc-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/README.md` & `nerfacc-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 [![Core Tests.](https://github.com/KAIR-BAIR/nerfacc/actions/workflows/code_checks.yml/badge.svg)](https://github.com/KAIR-BAIR/nerfacc/actions/workflows/code_checks.yml)
 [![Documentation Status](https://readthedocs.com/projects/plenoptix-nerfacc/badge/?version=latest)](https://www.nerfacc.com/en/latest/?badge=latest)
 [![Downloads](https://pepy.tech/badge/nerfacc)](https://pepy.tech/project/nerfacc)
 
 https://www.nerfacc.com/
 
+[News] 2023/04/04. If you were using `nerfacc <= 0.3.5` and would like to migrate to our latest version (`nerfacc >= 0.5.0`), Please check the [CHANGELOG](CHANGELOG.md) on how to migrate.
+
 NerfAcc is a PyTorch Nerf acceleration toolbox for both training and inference. It focus on
 efficient sampling in the volumetric rendering pipeline of radiance fields, which is 
 universal and plug-and-play for most of the NeRFs.
 With minimal modifications to the existing codebases, Nerfacc provides significant speedups 
 in training various recent NeRF papers.
 **And it is pure Python interface with flexible APIs!**
 
@@ -110,25 +112,25 @@
 loss = F.mse_loss(color, color_gt)
 loss.backward()
 optimizer.step()
 ```
 
 ## Examples: 
 
-See full benchmarking here: https://www.nerfacc.com/en/latest/examples/
-
 Before running those example scripts, please check the script about which dataset is needed, and download the dataset first. You could use `--data_root` to specify the path.
 
 ```bash
 # clone the repo with submodules.
 git clone --recursive git://github.com/KAIR-BAIR/nerfacc/
 ```
 
 ### Static NeRFs
 
+See full benchmarking here: https://www.nerfacc.com/en/stable/examples/static.html
+
 Instant-NGP on NeRF-Synthetic dataset with better performance in 4.5 minutes.
 ``` bash
 # Occupancy Grid Estimator
 python examples/train_ngp_nerf_occ.py --scene lego --data_root data/nerf_synthetic
 # Proposal Net Estimator
 python examples/train_ngp_nerf_prop.py --scene lego --data_root data/nerf_synthetic
 ```
@@ -152,14 +154,17 @@
 cd benchmarks/tensorf/
 # (set up the environment for that repo)
 bash script.sh nerfsyn-nerfacc-occgrid 0
 bash script.sh tt-nerfacc-occgrid 0
 ```
 
 ### Dynamic NeRFs
+
+See full benchmarking here: https://www.nerfacc.com/en/stable/examples/dynamic.html
+
 T-NeRF on D-NeRF dataset in an hour.
 ``` bash
 # Occupancy Grid Estimator
 python examples/train_mlp_tnerf.py --scene lego --data_root data/dnerf
 ```
 
 K-Planes on D-NeRF dataset (plugin in the official codebase).
@@ -176,14 +181,16 @@
 bash script.sh dnerf-nerfacc-occgrid 0
 bash script.sh hypernerf-nerfacc-occgrid 0
 bash script.sh hypernerf-nerfacc-propnet 0
 ```
 
 ### Camera Optimization NeRFs
 
+See full benchmarking here: https://www.nerfacc.com/en/stable/examples/camera.html
+
 BARF on the NeRF-Synthetic dataset (plugin in the official codebase).
 ```bash
 cd benchmarks/barf/
 # (set up the environment for that repo)
 bash script.sh nerfsyn-nerfacc-occgrid 0
 ```
 
@@ -203,12 +210,12 @@
 </details>
 
 ## Citation
 
 ```bibtex
 @article{li2023nerfacc,
   title={NerfAcc: Efficient Sampling Accelerates NeRFs.},
-  author={Li, Ruilong and Hang Gao and Tancik, Matthew and Kanazawa, Angjoo},
-  journal={TBD},
+  author={Li, Ruilong and Gao, Hang and Tancik, Matthew and Kanazawa, Angjoo},
+  journal={To Be Updated},
   year={2023}
 }
 ```
```

### Comparing `nerfacc-0.5.0/nerfacc/__init__.py` & `nerfacc-0.5.1/nerfacc/__init__.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/nerfacc/cuda/__init__.py` & `nerfacc-0.5.1/nerfacc/cuda/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,7 +34,13 @@
 inclusive_prod_backward = _make_lazy_cuda_func("inclusive_prod_backward")
 exclusive_prod_forward = _make_lazy_cuda_func("exclusive_prod_forward")
 exclusive_prod_backward = _make_lazy_cuda_func("exclusive_prod_backward")
 
 # pdf
 importance_sampling = _make_lazy_cuda_func("importance_sampling")
 searchsorted = _make_lazy_cuda_func("searchsorted")
+
+# camera
+opencv_lens_undistortion = _make_lazy_cuda_func("opencv_lens_undistortion")
+opencv_lens_undistortion_fisheye = _make_lazy_cuda_func(
+    "opencv_lens_undistortion_fisheye"
+)
```

### Comparing `nerfacc-0.5.0/nerfacc/cuda/_backend.py` & `nerfacc-0.5.1/nerfacc/cuda/_backend.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/nerfacc/cuda/csrc/grid.cu` & `nerfacc-0.5.1/nerfacc/cuda/csrc/grid.cu`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/nerfacc/cuda/csrc/include/data_spec.hpp` & `nerfacc-0.5.1/nerfacc/cuda/csrc/include/data_spec.hpp`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/nerfacc/cuda/csrc/include/data_spec_packed.cuh` & `nerfacc-0.5.1/nerfacc/cuda/csrc/include/data_spec_packed.cuh`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/nerfacc/cuda/csrc/include/utils_contraction.cuh` & `nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_contraction.cuh`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/nerfacc/cuda/csrc/include/utils_cuda.cuh` & `nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_cuda.cuh`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/nerfacc/cuda/csrc/include/utils_grid.cuh` & `nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_grid.cuh`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/nerfacc/cuda/csrc/include/utils_math.cuh` & `nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_math.cuh`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/nerfacc/cuda/csrc/include/utils_scan.cuh` & `nerfacc-0.5.1/nerfacc/cuda/csrc/include/utils_scan.cuh`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/nerfacc/cuda/csrc/nerfacc.cpp` & `nerfacc-0.5.1/nerfacc/cuda/csrc/nerfacc.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -84,47 +84,63 @@
     torch::Tensor cdfs,                  
     int64_t n_intervels_per_ray,
     bool stratified);
 std::vector<torch::Tensor> searchsorted(
     RaySegmentsSpec query,
     RaySegmentsSpec key);
 
+// cameras
+torch::Tensor opencv_lens_undistortion(
+    const torch::Tensor& uv,      // [..., 2]
+    const torch::Tensor& params,  // [..., 6]
+    const float eps,
+    const int max_iterations);
+torch::Tensor opencv_lens_undistortion_fisheye(
+    const torch::Tensor& uv,      // [..., 2]
+    const torch::Tensor& params,  // [..., 4]
+    const float criteria_eps,
+    const int criteria_iters);
+
+
 PYBIND11_MODULE(TORCH_EXTENSION_NAME, m) {
 #define _REG_FUNC(funname) m.def(#funname, &funname)
-  _REG_FUNC(is_cub_available);  // TODO: check this function
-  
-  _REG_FUNC(exclusive_sum_by_key);
-  _REG_FUNC(inclusive_sum);
-  _REG_FUNC(exclusive_sum);
-  _REG_FUNC(inclusive_prod_forward);
-  _REG_FUNC(inclusive_prod_backward);
-  _REG_FUNC(exclusive_prod_forward);
-  _REG_FUNC(exclusive_prod_backward);
-
-  _REG_FUNC(ray_aabb_intersect);
-  _REG_FUNC(traverse_grids);
-  _REG_FUNC(searchsorted);
+    _REG_FUNC(is_cub_available);  // TODO: check this function
+
+    _REG_FUNC(exclusive_sum_by_key);
+    _REG_FUNC(inclusive_sum);
+    _REG_FUNC(exclusive_sum);
+    _REG_FUNC(inclusive_prod_forward);
+    _REG_FUNC(inclusive_prod_backward);
+    _REG_FUNC(exclusive_prod_forward);
+    _REG_FUNC(exclusive_prod_backward);
+
+    _REG_FUNC(ray_aabb_intersect);
+    _REG_FUNC(traverse_grids);
+    _REG_FUNC(searchsorted);
+
+    _REG_FUNC(opencv_lens_undistortion);
+    _REG_FUNC(opencv_lens_undistortion_fisheye);
 #undef _REG_FUNC
 
-  m.def("importance_sampling", py::overload_cast<RaySegmentsSpec, torch::Tensor, torch::Tensor, bool>(&importance_sampling));
-  m.def("importance_sampling", py::overload_cast<RaySegmentsSpec, torch::Tensor, int64_t, bool>(&importance_sampling));
+    m.def("importance_sampling", py::overload_cast<RaySegmentsSpec, torch::Tensor, torch::Tensor, bool>(&importance_sampling));
+    m.def("importance_sampling", py::overload_cast<RaySegmentsSpec, torch::Tensor, int64_t, bool>(&importance_sampling));
 
-  py::class_<MultiScaleGridSpec>(m, "MultiScaleGridSpec")
-      .def(py::init<>())
-      .def_readwrite("data", &MultiScaleGridSpec::data)
-      .def_readwrite("occupied", &MultiScaleGridSpec::occupied)
-      .def_readwrite("base_aabb", &MultiScaleGridSpec::base_aabb);
-
-  py::class_<RaysSpec>(m, "RaysSpec")
-      .def(py::init<>())
-      .def_readwrite("origins", &RaysSpec::origins)
-      .def_readwrite("dirs", &RaysSpec::dirs);
-
-  py::class_<RaySegmentsSpec>(m, "RaySegmentsSpec")
-      .def(py::init<>())
-      .def_readwrite("vals", &RaySegmentsSpec::vals)
-      .def_readwrite("is_left", &RaySegmentsSpec::is_left)
-      .def_readwrite("is_right", &RaySegmentsSpec::is_right)
-      .def_readwrite("chunk_starts", &RaySegmentsSpec::chunk_starts)
-      .def_readwrite("chunk_cnts", &RaySegmentsSpec::chunk_cnts)
-      .def_readwrite("ray_indices", &RaySegmentsSpec::ray_indices);
+    py::class_<MultiScaleGridSpec>(m, "MultiScaleGridSpec")
+        .def(py::init<>())
+        .def_readwrite("data", &MultiScaleGridSpec::data)
+        .def_readwrite("occupied", &MultiScaleGridSpec::occupied)
+        .def_readwrite("base_aabb", &MultiScaleGridSpec::base_aabb);
+
+    py::class_<RaysSpec>(m, "RaysSpec")
+        .def(py::init<>())
+        .def_readwrite("origins", &RaysSpec::origins)
+        .def_readwrite("dirs", &RaysSpec::dirs);
+
+    py::class_<RaySegmentsSpec>(m, "RaySegmentsSpec")
+        .def(py::init<>())
+        .def_readwrite("vals", &RaySegmentsSpec::vals)
+        .def_readwrite("is_left", &RaySegmentsSpec::is_left)
+        .def_readwrite("is_right", &RaySegmentsSpec::is_right)
+        .def_readwrite("chunk_starts", &RaySegmentsSpec::chunk_starts)
+        .def_readwrite("chunk_cnts", &RaySegmentsSpec::chunk_cnts)
+        .def_readwrite("ray_indices", &RaySegmentsSpec::ray_indices);
 }
```

### Comparing `nerfacc-0.5.0/nerfacc/cuda/csrc/pdf.cu` & `nerfacc-0.5.1/nerfacc/cuda/csrc/pdf.cu`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/nerfacc/cuda/csrc/scan.cu` & `nerfacc-0.5.1/nerfacc/cuda/csrc/scan.cu`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/nerfacc/data_specs.py` & `nerfacc-0.5.1/nerfacc/data_specs.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/nerfacc/estimators/base.py` & `nerfacc-0.5.1/nerfacc/estimators/base.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/nerfacc/estimators/occ_grid.py` & `nerfacc-0.5.1/nerfacc/estimators/occ_grid.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/nerfacc/estimators/prop_net.py` & `nerfacc-0.5.1/nerfacc/estimators/prop_net.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from typing import Callable, List, Literal, Optional, Tuple
+from typing import Callable, List, Optional, Tuple
+
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal
 
 import torch
 from torch import Tensor
 
 from ..data_specs import RayIntervals
 from ..pdf import importance_sampling, searchsorted
 from ..volrend import render_transmittance_from_density
```

### Comparing `nerfacc-0.5.0/nerfacc/grid.py` & `nerfacc-0.5.1/nerfacc/grid.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,17 +27,19 @@
         aabbs: (m, 6) Axis-aligned bounding boxes {xmin, ymin, zmin, xmax, ymax, zmax}.
         near_plane: Optional. Near plane. Default to -infinity.
         far_plane: Optional. Far plane. Default to infinity.
         miss_value: Optional. Value to use for tmin and tmax when there is no intersection.
             Default to infinity.
 
     Returns:
-        t_mins: (n_rays, m) tmin for each ray-AABB pair.
-        t_maxs: (n_rays, m) tmax for each ray-AABB pair.
-        hits: (n_rays, m) whether each ray-AABB pair intersects.
+        A tuple of {Tensor, Tensor, BoolTensor}:
+
+        - **t_mins**: (n_rays, m) tmin for each ray-AABB pair.
+        - **t_maxs**: (n_rays, m) tmax for each ray-AABB pair.
+        - **hits**: (n_rays, m) whether each ray-AABB pair intersects.
     """
     assert rays_o.ndim == 2 and rays_o.shape[-1] == 3
     assert rays_d.ndim == 2 and rays_d.shape[-1] == 3
     assert aabbs.ndim == 2 and aabbs.shape[-1] == 6
     t_mins, t_maxs, hits = _C.ray_aabb_intersect(
         rays_o.contiguous(),
         rays_d.contiguous(),
```

### Comparing `nerfacc-0.5.0/nerfacc/pack.py` & `nerfacc-0.5.1/nerfacc/pack.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/nerfacc/pdf.py` & `nerfacc-0.5.1/nerfacc/pdf.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/nerfacc/scan.py` & `nerfacc-0.5.1/nerfacc/scan.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/nerfacc/volrend.py` & `nerfacc-0.5.1/nerfacc/volrend.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/nerfacc.egg-info/SOURCES.txt` & `nerfacc-0.5.1/nerfacc.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 nerfacc/__init__.py
+nerfacc/cameras.py
+nerfacc/cameras2.py
 nerfacc/data_specs.py
 nerfacc/grid.py
 nerfacc/pack.py
 nerfacc/pdf.py
 nerfacc/scan.py
 nerfacc/version.py
 nerfacc/volrend.py
 nerfacc.egg-info/PKG-INFO
 nerfacc.egg-info/SOURCES.txt
 nerfacc.egg-info/dependency_links.txt
 nerfacc.egg-info/requires.txt
 nerfacc.egg-info/top_level.txt
 nerfacc/cuda/__init__.py
 nerfacc/cuda/_backend.py
+nerfacc/cuda/csrc/camera.cu
 nerfacc/cuda/csrc/grid.cu
 nerfacc/cuda/csrc/nerfacc.cpp
 nerfacc/cuda/csrc/pdf.cu
 nerfacc/cuda/csrc/scan.cu
 nerfacc/cuda/csrc/include/data_spec.hpp
 nerfacc/cuda/csrc/include/data_spec_packed.cuh
+nerfacc/cuda/csrc/include/utils_camera.cuh
 nerfacc/cuda/csrc/include/utils_contraction.cuh
 nerfacc/cuda/csrc/include/utils_cuda.cuh
 nerfacc/cuda/csrc/include/utils_grid.cuh
 nerfacc/cuda/csrc/include/utils_math.cuh
 nerfacc/cuda/csrc/include/utils_scan.cuh
 nerfacc/estimators/__init__.py
 nerfacc/estimators/base.py
 nerfacc/estimators/occ_grid.py
 nerfacc/estimators/prop_net.py
+tests/test_camera.py
 tests/test_grid.py
 tests/test_pack.py
 tests/test_pdf.py
 tests/test_rendering.py
 tests/test_scan.py
```

### Comparing `nerfacc-0.5.0/setup.py` & `nerfacc-0.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     description="A General NeRF Acceleration Toolbox",
     author="Ruilong",
     author_email="ruilongli94@gmail.com",
     url=URL,
     download_url=f"{URL}/archive/{__version__}.tar.gz",
     keywords=[],
     python_requires=">=3.7",
-    install_requires=["rich>=12", "torch"],
+    install_requires=["rich>=12", "torch", "typing_extensions; python_version<'3.8'"],
     extras_require={
         # dev dependencies. Install them by `pip install nerfacc[dev]`
         "dev": [
             "black[jupyter]==22.3.0",
             "isort==5.10.1",
             "pylint==2.13.4",
             "pytest==7.1.2",
```

### Comparing `nerfacc-0.5.0/tests/test_grid.py` & `nerfacc-0.5.1/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/tests/test_pack.py` & `nerfacc-0.5.1/tests/test_pack.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/tests/test_pdf.py` & `nerfacc-0.5.1/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/tests/test_rendering.py` & `nerfacc-0.5.1/tests/test_rendering.py`

 * *Files identical despite different names*

### Comparing `nerfacc-0.5.0/tests/test_scan.py` & `nerfacc-0.5.1/tests/test_scan.py`

 * *Files identical despite different names*

