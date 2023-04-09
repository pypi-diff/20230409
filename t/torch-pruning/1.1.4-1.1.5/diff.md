# Comparing `tmp/torch-pruning-1.1.4.tar.gz` & `tmp/torch-pruning-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-pruning-1.1.4.tar", last modified: Sat Apr  8 11:37:53 2023, max compression
+gzip compressed data, was "torch-pruning-1.1.5.tar", last modified: Sun Apr  9 09:07:01 2023, max compression
```

## Comparing `torch-pruning-1.1.4.tar` & `torch-pruning-1.1.5.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:37:53.384673 torch-pruning-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-04-08 11:37:53.384673 torch-pruning-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17613 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 11:37:53.384673 torch-pruning-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:37:53.380674 torch-pruning-1.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/tests/test_customized_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/tests/test_dependency_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/tests/test_dependency_lenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/tests/test_fully_connected_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/tests/test_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/tests/test_interactive_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/tests/test_multiple_inputs_and_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/tests/test_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/tests/test_pruning_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/tests/test_reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/tests/test_unwrapped_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:37:53.384673 torch-pruning-1.1.4/torch_pruning/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/torch_pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/torch_pruning/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    35409 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/torch_pruning/dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/torch_pruning/importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/torch_pruning/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:37:53.384673 torch-pruning-1.1.4/torch_pruning/pruner/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/torch_pruning/pruner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:37:53.384673 torch-pruning-1.1.4/torch_pruning/pruner/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/torch_pruning/pruner/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/torch_pruning/pruner/algorithms/batchnorm_scale_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/torch_pruning/pruner/algorithms/group_norm_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/torch_pruning/pruner/algorithms/magnitude_based_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/torch_pruning/pruner/algorithms/metapruner.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/torch_pruning/pruner/algorithms/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20396 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/torch_pruning/pruner/function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:37:53.384673 torch-pruning-1.1.4/torch_pruning/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/torch_pruning/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/torch_pruning/utils/op_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-08 11:37:43.000000 torch-pruning-1.1.4/torch_pruning/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:37:53.384673 torch-pruning-1.1.4/torch_pruning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18057 2023-04-08 11:37:53.000000 torch-pruning-1.1.4/torch_pruning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-08 11:37:53.000000 torch-pruning-1.1.4/torch_pruning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 11:37:53.000000 torch-pruning-1.1.4/torch_pruning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-08 11:37:53.000000 torch-pruning-1.1.4/torch_pruning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-08 11:37:53.000000 torch-pruning-1.1.4/torch_pruning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:07:01.789480 torch-pruning-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-04-09 09:07:01.789480 torch-pruning-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17597 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 09:07:01.789480 torch-pruning-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:07:01.785480 torch-pruning-1.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_backward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_customized_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_dependency_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_dependency_lenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_fully_connected_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_interactive_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_multiple_inputs_and_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_pruning_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/tests/test_unwrapped_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:07:01.785480 torch-pruning-1.1.5/torch_pruning/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36317 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:07:01.785480 torch-pruning-1.1.5/torch_pruning/pruner/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/pruner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:07:01.785480 torch-pruning-1.1.5/torch_pruning/pruner/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/pruner/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/pruner/algorithms/batchnorm_scale_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/pruner/algorithms/group_norm_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/pruner/algorithms/magnitude_based_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/pruner/algorithms/metapruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/pruner/algorithms/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/pruner/function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:07:01.789480 torch-pruning-1.1.5/torch_pruning/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/utils/op_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-09 09:06:46.000000 torch-pruning-1.1.5/torch_pruning/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:07:01.785480 torch-pruning-1.1.5/torch_pruning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-04-09 09:07:01.000000 torch-pruning-1.1.5/torch_pruning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-09 09:07:01.000000 torch-pruning-1.1.5/torch_pruning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 09:07:01.000000 torch-pruning-1.1.5/torch_pruning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-09 09:07:01.000000 torch-pruning-1.1.5/torch_pruning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-09 09:07:01.000000 torch-pruning-1.1.5/torch_pruning.egg-info/top_level.txt
```

### Comparing `torch-pruning-1.1.4/LICENSE` & `torch-pruning-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.4/PKG-INFO` & `torch-pruning-1.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: torch-pruning
-Version: 1.1.4
+Version: 1.1.5
 Summary: Structural Pruning for Model Acceleration.
 Home-page: https://github.com/VainF/Torch-Pruning
 Author: Gongfan Fang
 Author-email: gongfan@u.nus.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center"> <h1>Torch-Pruning <br> <h3>Towards Any Structural Pruning<h3> </h1> </div>
 <div align="center">
-<img src="assets/intro.png" width="45%">
+<img src="assets/intro.png" width="50%">
 </div>
 
 <p align="center">
   <a href="https://github.com/VainF/Torch-Pruning/actions"><img src="https://img.shields.io/badge/tests-passing-9c27b0.svg" alt="Test Status"></a>
   <a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-1.8.1%20%7C%202.0.0-673ab7.svg" alt="Tested PyTorch Versions"></a>
   <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-4caf50.svg" alt="License"></a>
   <a href="https://pepy.tech/project/Torch-Pruning"><img src="https://pepy.tech/badge/Torch-Pruning?color=2196f3" alt="Downloads"></a>
-  <a href="https://github.com/VainF/Torch-Pruning/releases/latest"><img src="https://img.shields.io/badge/Latest%20Version-1.1.3-3f51b5.svg" alt="Latest Version"></a>
+  <a href="https://github.com/VainF/Torch-Pruning/releases/latest"><img src="https://img.shields.io/badge/Latest%20Version-1.1.4-3f51b5.svg" alt="Latest Version"></a>
+  <a href="https://colab.research.google.com/drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
   <a href="https://arxiv.org/abs/2301.12900" target="_blank"><img src="https://img.shields.io/badge/arXiv-2301.12900-009688.svg" alt="arXiv"></a>
 </p>
 
 
 [[中文README | README in Chinese]](README_CN.md)
 
 Torch-Pruning (TP) is a versatile library for Structural Network Pruning with the following features:
 * **General-purpose Pruning Toolkit:** TP enables structural pruning for a wide range of neural networks, including *Vision Transformers, Yolov7, FasterRCNN, SSD, KeypointRCNN, MaskRCNN, ResNe(X)t, ConvNext, DenseNet, ConvNext, RegNet, FCN, DeepLab, etc*. Different from [torch.nn.utils.prune](https://pytorch.org/tutorials/intermediate/pruning_tutorial.html) that zeroizes parameters through masking, Torch-Pruning employs a (non-deep) graph algorithm called DepGraph to physically remove coupled parameters (channels) from models. 
-* **Reproducible [Performance Benchmark](benchmarks) and [Prunability Benchmark](benchmarks/prunability):** Currently, TP is able to prune approximately **77/85=90.6%** of the models from Torchvision 0.13.1. Check out [practical_structural_pruning.md](practical_structural_pruning.md) for an up-to-date list of practical pruning techniques. 
-
+* **Reproducible [Performance Benchmark](benchmarks) and [Prunability Benchmark](benchmarks/prunability):** Currently, TP is able to prune approximately **77/85=90.6%** of the models from Torchvision 0.13.1. Try this [Colab Demo](https://colab.research.google.com/drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing) for quick start.
 
 For more technical details, please refer to our CVPR'23 paper:
 > [**DepGraph: Towards Any Structural Pruning**](https://arxiv.org/abs/2301.12900)   
 > [Gongfan Fang](https://fangggf.github.io/), [Xinyin Ma](https://horseee.github.io/), [Mingli Song](https://person.zju.edu.cn/en/msong), [Michael Bi Mi](https://dblp.org/pid/317/0937.html), [Xinchao Wang](https://sites.google.com/site/sitexinchaowang/)   
 
 Please do not hesitate to open a [discussion](https://github.com/VainF/Torch-Pruning/discussions) or [issue](https://github.com/VainF/Torch-Pruning/issues) if you encounter any problems with the library or the paper. 
 
@@ -59,15 +61,15 @@
 - [ ] More standard layers: GroupNorm, InstanceNorm, Shuffle Layers, etc.
 - [ ] More Transformers like Vision Transformers (:heavy_check_mark:), Swin Transformers, PoolFormers.
 - [ ] Block/Layer/Depth Pruning
 - [ ] Pruning benchmarks for CIFAR, ImageNet and COCO.
 
 ## Installation
 ```bash
-pip install torch-pruning # v1.1.3
+pip install torch-pruning # v1.1.4
 ```
 or
 ```bash
 git clone https://github.com/VainF/Torch-Pruning.git # recommended
 ```
 
 ## Quickstart
@@ -129,28 +131,28 @@
 [14] prune_out_channels on layer1.1.bn2 (BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)) => prune_out_channels on layer1.1.conv2 (Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)), idxs=[2, 6, 9]
 [15] prune_out_channels on layer1.0.bn2 (BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)) => prune_out_channels on layer1.0.conv2 (Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)), idxs=[2, 6, 9]
 --------------------------------
 ```
 For more details about grouping, please refer to [tutorials/2 - Exploring Dependency Groups](https://github.com/VainF/Torch-Pruning/blob/master/tutorials/2%20-%20Exploring%20Dependency%20Groups.ipynb)
 
 #### How to scan all groups:
-Just like what we do in the [MetaPruner](https://github.com/VainF/Torch-Pruning/blob/b607ae3aa61b9dafe19d2c2364f7e4984983afbf/torch_pruning/pruner/algorithms/metapruner.py#L197), one can use ``DG.get_all_groups(ignored_layers, root_module_types)`` to scan all groups sequentially. Each group will begin with a layer that matches a type in the "root_module_types" parameter. Note that DG.get_all_groups is only responsible for grouping and does not have any knowledge or understanding of which parameters should be pruned. Therefore, it is necessary to specify the pruning idxs using  ``group.prune(idxs=idxs)``.
+We can use ``DG.get_all_groups(ignored_layers, root_module_types)`` to scan all groups sequentially. Each group will begin with a layer that matches a type in the "root_module_types" parameter. Note that DG.get_all_groups is only responsible for grouping and does not have any knowledge or understanding of which parameters should be pruned. Therefore, it is necessary to specify the pruning idxs using  ``group.prune(idxs=idxs)``.
 
 ```python
 for group in DG.get_all_groups(ignored_layers=[model.conv1], root_module_types=[nn.Conv2d, nn.Linear]):
     # handle groups in sequential order
     idxs = [2,4,6] # your pruning indices
     group.prune(idxs=idxs)
     print(group)
 ```
 
 
 ### 2. High-level Pruners
 
-Leveraging the DependencyGraph, we developed several high-level pruners in this repository to facilitate effortless pruning. By specifying the desired channel sparsity, you can prune the entire model and fine-tune it using your own training code. For detailed information on this process, we encourage you to consult the [this tutorial](https://github.com/VainF/Torch-Pruning/blob/master/tutorials/1%20-%20Customize%20Your%20Own%20Pruners.ipynb), which demonstrates how to implement a [slimming](https://arxiv.org/abs/1708.06519) pruner from scratch. Additionally, you can find more practical examples in [benchmarks/main.py](benchmarks/main.py).
+Leveraging the DependencyGraph, we developed several high-level pruners in this repository to facilitate effortless pruning. By specifying the desired channel sparsity, you can prune the entire model and fine-tune it using your own training code. For detailed information on this process, please refer to [this tutorial](https://github.com/VainF/Torch-Pruning/blob/master/tutorials/1%20-%20Customize%20Your%20Own%20Pruners.ipynb), which shows how to implement a [slimming](https://arxiv.org/abs/1708.06519) pruner from scratch. Additionally, you can find more practical examples in [benchmarks/main.py](benchmarks/main.py).
 
 ```python
 import torch
 from torchvision.models import resnet18
 import torch_pruning as tp
 
 model = resnet18(pretrained=True)
```

#### html2text {}

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1 Name: torch-pruning Version: 1.1.4 Summary: Structural
+Metadata-Version: 2.1 Name: torch-pruning Version: 1.1.5 Summary: Structural
 Pruning for Model Acceleration. Home-page: https://github.com/VainF/Torch-
 Pruning Author: Gongfan Fang Author-email: gongfan@u.nus.edu Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE
                              ****** Torch-Pruning
                      Towards Any Structural Pruning ******
                               [assets/intro.png]
 [Test_Status] [Tested_PyTorch_Versions] [License] [Downloads] [Latest_Version]
-                                    [arXiv]
+                            [Open_In_Colab] [arXiv]
 [[ä¸­æREADME | README in Chinese]](README_CN.md) Torch-Pruning (TP) is a
 versatile library for Structural Network Pruning with the following features: *
 **General-purpose Pruning Toolkit:** TP enables structural pruning for a wide
 range of neural networks, including *Vision Transformers, Yolov7, FasterRCNN,
 SSD, KeypointRCNN, MaskRCNN, ResNe(X)t, ConvNext, DenseNet, ConvNext, RegNet,
 FCN, DeepLab, etc*. Different from [torch.nn.utils.prune](https://pytorch.org/
 tutorials/intermediate/pruning_tutorial.html) that zeroizes parameters through
 masking, Torch-Pruning employs a (non-deep) graph algorithm called DepGraph to
 physically remove coupled parameters (channels) from models. * **Reproducible
 [Performance Benchmark](benchmarks) and [Prunability Benchmark](benchmarks/
 prunability):** Currently, TP is able to prune approximately **77/85=90.6%** of
-the models from Torchvision 0.13.1. Check out [practical_structural_pruning.md]
-(practical_structural_pruning.md) for an up-to-date list of practical pruning
-techniques. For more technical details, please refer to our CVPR'23 paper: >
-[**DepGraph: Towards Any Structural Pruning**](https://arxiv.org/abs/
+the models from Torchvision 0.13.1. Try this [Colab Demo](https://
+colab.research.google.com/drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing)
+for quick start. For more technical details, please refer to our CVPR'23 paper:
+> [**DepGraph: Towards Any Structural Pruning**](https://arxiv.org/abs/
 2301.12900) > [Gongfan Fang](https://fangggf.github.io/), [Xinyin Ma](https://
 horseee.github.io/), [Mingli Song](https://person.zju.edu.cn/en/msong),
 [Michael Bi Mi](https://dblp.org/pid/317/0937.html), [Xinchao Wang](https://
 sites.google.com/site/sitexinchaowang/) Please do not hesitate to open a
 [discussion](https://github.com/VainF/Torch-Pruning/discussions) or [issue]
 (https://github.com/VainF/Torch-Pruning/issues) if you encounter any problems
 with the library or the paper. ### **Features:** - [x] Structural (Channel)
@@ -54,15 +54,15 @@
 YOLOv8) - [ ] Pruning from Scratch / at Initialization. - [ ] Language, Speech
 and Generative Models. - [ ] More high-level pruners like [FisherPruner](https:
 //arxiv.org/abs/2108.00708), [GrowingReg](https://arxiv.org/abs/2012.09243),
 etc. - [ ] More standard layers: GroupNorm, InstanceNorm, Shuffle Layers, etc.
 - [ ] More Transformers like Vision Transformers (:heavy_check_mark:), Swin
 Transformers, PoolFormers. - [ ] Block/Layer/Depth Pruning - [ ] Pruning
 benchmarks for CIFAR, ImageNet and COCO. ## Installation ```bash pip install
-torch-pruning # v1.1.3 ``` or ```bash git clone https://github.com/VainF/Torch-
+torch-pruning # v1.1.4 ``` or ```bash git clone https://github.com/VainF/Torch-
 Pruning.git # recommended ``` ## Quickstart Here we provide a quick start for
 Torch-Pruning. More explained details can be found in [tutorals](./tutorials/
 ) ### 0. How It Works In structural pruning, **a ``Group`` constitutes the
 minimal prunable unit within deep networks**. Each group typically comprises
 several interdependent parameters that must be removed simultaneously to
 maintain the integrity of the resulting structures. However, deep networks
 often present complex dependencies among parameters, making structural pruning
@@ -127,38 +127,35 @@
 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)), idxs=[2,
 6, 9] [15] prune_out_channels on layer1.0.bn2 (BatchNorm2d(64, eps=1e-05,
 momentum=0.1, affine=True, track_running_stats=True)) => prune_out_channels on
 layer1.0.conv2 (Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1,
 1), bias=False)), idxs=[2, 6, 9] -------------------------------- ``` For more
 details about grouping, please refer to [tutorials/2 - Exploring Dependency
 Groups](https://github.com/VainF/Torch-Pruning/blob/master/tutorials/2%20-
-%20Exploring%20Dependency%20Groups.ipynb) #### How to scan all groups: Just
-like what we do in the [MetaPruner](https://github.com/VainF/Torch-Pruning/
-blob/b607ae3aa61b9dafe19d2c2364f7e4984983afbf/torch_pruning/pruner/algorithms/
-metapruner.py#L197), one can use ``DG.get_all_groups(ignored_layers,
-root_module_types)`` to scan all groups sequentially. Each group will begin
-with a layer that matches a type in the "root_module_types" parameter. Note
-that DG.get_all_groups is only responsible for grouping and does not have any
-knowledge or understanding of which parameters should be pruned. Therefore, it
-is necessary to specify the pruning idxs using ``group.prune(idxs=idxs)``.
-```python for group in DG.get_all_groups(ignored_layers=[model.conv1],
-root_module_types=[nn.Conv2d, nn.Linear]): # handle groups in sequential order
-idxs = [2,4,6] # your pruning indices group.prune(idxs=idxs) print(group) ```
-### 2. High-level Pruners Leveraging the DependencyGraph, we developed several
-high-level pruners in this repository to facilitate effortless pruning. By
-specifying the desired channel sparsity, you can prune the entire model and
-fine-tune it using your own training code. For detailed information on this
-process, we encourage you to consult the [this tutorial](https://github.com/
-VainF/Torch-Pruning/blob/master/tutorials/1%20-
-%20Customize%20Your%20Own%20Pruners.ipynb), which demonstrates how to implement
-a [slimming](https://arxiv.org/abs/1708.06519) pruner from scratch.
-Additionally, you can find more practical examples in [benchmarks/main.py]
-(benchmarks/main.py). ```python import torch from torchvision.models import
-resnet18 import torch_pruning as tp model = resnet18(pretrained=True) #
-Importance criteria example_inputs = torch.randn(1, 3, 224, 224) imp =
+%20Exploring%20Dependency%20Groups.ipynb) #### How to scan all groups: We can
+use ``DG.get_all_groups(ignored_layers, root_module_types)`` to scan all groups
+sequentially. Each group will begin with a layer that matches a type in the
+"root_module_types" parameter. Note that DG.get_all_groups is only responsible
+for grouping and does not have any knowledge or understanding of which
+parameters should be pruned. Therefore, it is necessary to specify the pruning
+idxs using ``group.prune(idxs=idxs)``. ```python for group in DG.get_all_groups
+(ignored_layers=[model.conv1], root_module_types=[nn.Conv2d, nn.Linear]): #
+handle groups in sequential order idxs = [2,4,6] # your pruning indices
+group.prune(idxs=idxs) print(group) ``` ### 2. High-level Pruners Leveraging
+the DependencyGraph, we developed several high-level pruners in this repository
+to facilitate effortless pruning. By specifying the desired channel sparsity,
+you can prune the entire model and fine-tune it using your own training code.
+For detailed information on this process, please refer to [this tutorial]
+(https://github.com/VainF/Torch-Pruning/blob/master/tutorials/1%20-
+%20Customize%20Your%20Own%20Pruners.ipynb), which shows how to implement a
+[slimming](https://arxiv.org/abs/1708.06519) pruner from scratch. Additionally,
+you can find more practical examples in [benchmarks/main.py](benchmarks/
+main.py). ```python import torch from torchvision.models import resnet18 import
+torch_pruning as tp model = resnet18(pretrained=True) # Importance criteria
+example_inputs = torch.randn(1, 3, 224, 224) imp =
 tp.importance.MagnitudeImportance(p=2) ignored_layers = [] for m in
 model.modules(): if isinstance(m, torch.nn.Linear) and m.out_features == 1000:
 ignored_layers.append(m) # DO NOT prune the final classifier! iterative_steps =
 5 # progressive pruning pruner = tp.pruner.MagnitudePruner( model,
 example_inputs, importance=imp, iterative_steps=iterative_steps,
 ch_sparsity=0.5, # remove 50% channels, ResNet18 = {64, 128, 256, 512} =>
 ResNet18_Half = {32, 64, 128, 256} ignored_layers=ignored_layers, ) base_macs,
```

### Comparing `torch-pruning-1.1.4/README.md` & `torch-pruning-1.1.5/torch_pruning.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,44 @@
+Metadata-Version: 2.1
+Name: torch-pruning
+Version: 1.1.5
+Summary: Structural Pruning for Model Acceleration.
+Home-page: https://github.com/VainF/Torch-Pruning
+Author: Gongfan Fang
+Author-email: gongfan@u.nus.edu
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center"> <h1>Torch-Pruning <br> <h3>Towards Any Structural Pruning<h3> </h1> </div>
 <div align="center">
-<img src="assets/intro.png" width="45%">
+<img src="assets/intro.png" width="50%">
 </div>
 
 <p align="center">
   <a href="https://github.com/VainF/Torch-Pruning/actions"><img src="https://img.shields.io/badge/tests-passing-9c27b0.svg" alt="Test Status"></a>
   <a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-1.8.1%20%7C%202.0.0-673ab7.svg" alt="Tested PyTorch Versions"></a>
   <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-4caf50.svg" alt="License"></a>
   <a href="https://pepy.tech/project/Torch-Pruning"><img src="https://pepy.tech/badge/Torch-Pruning?color=2196f3" alt="Downloads"></a>
-  <a href="https://github.com/VainF/Torch-Pruning/releases/latest"><img src="https://img.shields.io/badge/Latest%20Version-1.1.3-3f51b5.svg" alt="Latest Version"></a>
+  <a href="https://github.com/VainF/Torch-Pruning/releases/latest"><img src="https://img.shields.io/badge/Latest%20Version-1.1.4-3f51b5.svg" alt="Latest Version"></a>
+  <a href="https://colab.research.google.com/drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
   <a href="https://arxiv.org/abs/2301.12900" target="_blank"><img src="https://img.shields.io/badge/arXiv-2301.12900-009688.svg" alt="arXiv"></a>
 </p>
 
 
 [[中文README | README in Chinese]](README_CN.md)
 
 Torch-Pruning (TP) is a versatile library for Structural Network Pruning with the following features:
 * **General-purpose Pruning Toolkit:** TP enables structural pruning for a wide range of neural networks, including *Vision Transformers, Yolov7, FasterRCNN, SSD, KeypointRCNN, MaskRCNN, ResNe(X)t, ConvNext, DenseNet, ConvNext, RegNet, FCN, DeepLab, etc*. Different from [torch.nn.utils.prune](https://pytorch.org/tutorials/intermediate/pruning_tutorial.html) that zeroizes parameters through masking, Torch-Pruning employs a (non-deep) graph algorithm called DepGraph to physically remove coupled parameters (channels) from models. 
-* **Reproducible [Performance Benchmark](benchmarks) and [Prunability Benchmark](benchmarks/prunability):** Currently, TP is able to prune approximately **77/85=90.6%** of the models from Torchvision 0.13.1. Check out [practical_structural_pruning.md](practical_structural_pruning.md) for an up-to-date list of practical pruning techniques. 
-
+* **Reproducible [Performance Benchmark](benchmarks) and [Prunability Benchmark](benchmarks/prunability):** Currently, TP is able to prune approximately **77/85=90.6%** of the models from Torchvision 0.13.1. Try this [Colab Demo](https://colab.research.google.com/drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing) for quick start.
 
 For more technical details, please refer to our CVPR'23 paper:
 > [**DepGraph: Towards Any Structural Pruning**](https://arxiv.org/abs/2301.12900)   
 > [Gongfan Fang](https://fangggf.github.io/), [Xinyin Ma](https://horseee.github.io/), [Mingli Song](https://person.zju.edu.cn/en/msong), [Michael Bi Mi](https://dblp.org/pid/317/0937.html), [Xinchao Wang](https://sites.google.com/site/sitexinchaowang/)   
 
 Please do not hesitate to open a [discussion](https://github.com/VainF/Torch-Pruning/discussions) or [issue](https://github.com/VainF/Torch-Pruning/issues) if you encounter any problems with the library or the paper. 
 
@@ -45,15 +61,15 @@
 - [ ] More standard layers: GroupNorm, InstanceNorm, Shuffle Layers, etc.
 - [ ] More Transformers like Vision Transformers (:heavy_check_mark:), Swin Transformers, PoolFormers.
 - [ ] Block/Layer/Depth Pruning
 - [ ] Pruning benchmarks for CIFAR, ImageNet and COCO.
 
 ## Installation
 ```bash
-pip install torch-pruning # v1.1.3
+pip install torch-pruning # v1.1.4
 ```
 or
 ```bash
 git clone https://github.com/VainF/Torch-Pruning.git # recommended
 ```
 
 ## Quickstart
@@ -115,28 +131,28 @@
 [14] prune_out_channels on layer1.1.bn2 (BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)) => prune_out_channels on layer1.1.conv2 (Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)), idxs=[2, 6, 9]
 [15] prune_out_channels on layer1.0.bn2 (BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)) => prune_out_channels on layer1.0.conv2 (Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)), idxs=[2, 6, 9]
 --------------------------------
 ```
 For more details about grouping, please refer to [tutorials/2 - Exploring Dependency Groups](https://github.com/VainF/Torch-Pruning/blob/master/tutorials/2%20-%20Exploring%20Dependency%20Groups.ipynb)
 
 #### How to scan all groups:
-Just like what we do in the [MetaPruner](https://github.com/VainF/Torch-Pruning/blob/b607ae3aa61b9dafe19d2c2364f7e4984983afbf/torch_pruning/pruner/algorithms/metapruner.py#L197), one can use ``DG.get_all_groups(ignored_layers, root_module_types)`` to scan all groups sequentially. Each group will begin with a layer that matches a type in the "root_module_types" parameter. Note that DG.get_all_groups is only responsible for grouping and does not have any knowledge or understanding of which parameters should be pruned. Therefore, it is necessary to specify the pruning idxs using  ``group.prune(idxs=idxs)``.
+We can use ``DG.get_all_groups(ignored_layers, root_module_types)`` to scan all groups sequentially. Each group will begin with a layer that matches a type in the "root_module_types" parameter. Note that DG.get_all_groups is only responsible for grouping and does not have any knowledge or understanding of which parameters should be pruned. Therefore, it is necessary to specify the pruning idxs using  ``group.prune(idxs=idxs)``.
 
 ```python
 for group in DG.get_all_groups(ignored_layers=[model.conv1], root_module_types=[nn.Conv2d, nn.Linear]):
     # handle groups in sequential order
     idxs = [2,4,6] # your pruning indices
     group.prune(idxs=idxs)
     print(group)
 ```
 
 
 ### 2. High-level Pruners
 
-Leveraging the DependencyGraph, we developed several high-level pruners in this repository to facilitate effortless pruning. By specifying the desired channel sparsity, you can prune the entire model and fine-tune it using your own training code. For detailed information on this process, we encourage you to consult the [this tutorial](https://github.com/VainF/Torch-Pruning/blob/master/tutorials/1%20-%20Customize%20Your%20Own%20Pruners.ipynb), which demonstrates how to implement a [slimming](https://arxiv.org/abs/1708.06519) pruner from scratch. Additionally, you can find more practical examples in [benchmarks/main.py](benchmarks/main.py).
+Leveraging the DependencyGraph, we developed several high-level pruners in this repository to facilitate effortless pruning. By specifying the desired channel sparsity, you can prune the entire model and fine-tune it using your own training code. For detailed information on this process, please refer to [this tutorial](https://github.com/VainF/Torch-Pruning/blob/master/tutorials/1%20-%20Customize%20Your%20Own%20Pruners.ipynb), which shows how to implement a [slimming](https://arxiv.org/abs/1708.06519) pruner from scratch. Additionally, you can find more practical examples in [benchmarks/main.py](benchmarks/main.py).
 
 ```python
 import torch
 from torchvision.models import resnet18
 import torch_pruning as tp
 
 model = resnet18(pretrained=True)
```

#### html2text {}

```diff
@@ -1,27 +1,33 @@
+Metadata-Version: 2.1 Name: torch-pruning Version: 1.1.5 Summary: Structural
+Pruning for Model Acceleration. Home-page: https://github.com/VainF/Torch-
+Pruning Author: Gongfan Fang Author-email: gongfan@u.nus.edu Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
+Description-Content-Type: text/markdown License-File: LICENSE
                              ****** Torch-Pruning
                      Towards Any Structural Pruning ******
                               [assets/intro.png]
 [Test_Status] [Tested_PyTorch_Versions] [License] [Downloads] [Latest_Version]
-                                    [arXiv]
+                            [Open_In_Colab] [arXiv]
 [[ä¸­æREADME | README in Chinese]](README_CN.md) Torch-Pruning (TP) is a
 versatile library for Structural Network Pruning with the following features: *
 **General-purpose Pruning Toolkit:** TP enables structural pruning for a wide
 range of neural networks, including *Vision Transformers, Yolov7, FasterRCNN,
 SSD, KeypointRCNN, MaskRCNN, ResNe(X)t, ConvNext, DenseNet, ConvNext, RegNet,
 FCN, DeepLab, etc*. Different from [torch.nn.utils.prune](https://pytorch.org/
 tutorials/intermediate/pruning_tutorial.html) that zeroizes parameters through
 masking, Torch-Pruning employs a (non-deep) graph algorithm called DepGraph to
 physically remove coupled parameters (channels) from models. * **Reproducible
 [Performance Benchmark](benchmarks) and [Prunability Benchmark](benchmarks/
 prunability):** Currently, TP is able to prune approximately **77/85=90.6%** of
-the models from Torchvision 0.13.1. Check out [practical_structural_pruning.md]
-(practical_structural_pruning.md) for an up-to-date list of practical pruning
-techniques. For more technical details, please refer to our CVPR'23 paper: >
-[**DepGraph: Towards Any Structural Pruning**](https://arxiv.org/abs/
+the models from Torchvision 0.13.1. Try this [Colab Demo](https://
+colab.research.google.com/drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing)
+for quick start. For more technical details, please refer to our CVPR'23 paper:
+> [**DepGraph: Towards Any Structural Pruning**](https://arxiv.org/abs/
 2301.12900) > [Gongfan Fang](https://fangggf.github.io/), [Xinyin Ma](https://
 horseee.github.io/), [Mingli Song](https://person.zju.edu.cn/en/msong),
 [Michael Bi Mi](https://dblp.org/pid/317/0937.html), [Xinchao Wang](https://
 sites.google.com/site/sitexinchaowang/) Please do not hesitate to open a
 [discussion](https://github.com/VainF/Torch-Pruning/discussions) or [issue]
 (https://github.com/VainF/Torch-Pruning/issues) if you encounter any problems
 with the library or the paper. ### **Features:** - [x] Structural (Channel)
@@ -48,15 +54,15 @@
 YOLOv8) - [ ] Pruning from Scratch / at Initialization. - [ ] Language, Speech
 and Generative Models. - [ ] More high-level pruners like [FisherPruner](https:
 //arxiv.org/abs/2108.00708), [GrowingReg](https://arxiv.org/abs/2012.09243),
 etc. - [ ] More standard layers: GroupNorm, InstanceNorm, Shuffle Layers, etc.
 - [ ] More Transformers like Vision Transformers (:heavy_check_mark:), Swin
 Transformers, PoolFormers. - [ ] Block/Layer/Depth Pruning - [ ] Pruning
 benchmarks for CIFAR, ImageNet and COCO. ## Installation ```bash pip install
-torch-pruning # v1.1.3 ``` or ```bash git clone https://github.com/VainF/Torch-
+torch-pruning # v1.1.4 ``` or ```bash git clone https://github.com/VainF/Torch-
 Pruning.git # recommended ``` ## Quickstart Here we provide a quick start for
 Torch-Pruning. More explained details can be found in [tutorals](./tutorials/
 ) ### 0. How It Works In structural pruning, **a ``Group`` constitutes the
 minimal prunable unit within deep networks**. Each group typically comprises
 several interdependent parameters that must be removed simultaneously to
 maintain the integrity of the resulting structures. However, deep networks
 often present complex dependencies among parameters, making structural pruning
@@ -121,38 +127,35 @@
 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)), idxs=[2,
 6, 9] [15] prune_out_channels on layer1.0.bn2 (BatchNorm2d(64, eps=1e-05,
 momentum=0.1, affine=True, track_running_stats=True)) => prune_out_channels on
 layer1.0.conv2 (Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1,
 1), bias=False)), idxs=[2, 6, 9] -------------------------------- ``` For more
 details about grouping, please refer to [tutorials/2 - Exploring Dependency
 Groups](https://github.com/VainF/Torch-Pruning/blob/master/tutorials/2%20-
-%20Exploring%20Dependency%20Groups.ipynb) #### How to scan all groups: Just
-like what we do in the [MetaPruner](https://github.com/VainF/Torch-Pruning/
-blob/b607ae3aa61b9dafe19d2c2364f7e4984983afbf/torch_pruning/pruner/algorithms/
-metapruner.py#L197), one can use ``DG.get_all_groups(ignored_layers,
-root_module_types)`` to scan all groups sequentially. Each group will begin
-with a layer that matches a type in the "root_module_types" parameter. Note
-that DG.get_all_groups is only responsible for grouping and does not have any
-knowledge or understanding of which parameters should be pruned. Therefore, it
-is necessary to specify the pruning idxs using ``group.prune(idxs=idxs)``.
-```python for group in DG.get_all_groups(ignored_layers=[model.conv1],
-root_module_types=[nn.Conv2d, nn.Linear]): # handle groups in sequential order
-idxs = [2,4,6] # your pruning indices group.prune(idxs=idxs) print(group) ```
-### 2. High-level Pruners Leveraging the DependencyGraph, we developed several
-high-level pruners in this repository to facilitate effortless pruning. By
-specifying the desired channel sparsity, you can prune the entire model and
-fine-tune it using your own training code. For detailed information on this
-process, we encourage you to consult the [this tutorial](https://github.com/
-VainF/Torch-Pruning/blob/master/tutorials/1%20-
-%20Customize%20Your%20Own%20Pruners.ipynb), which demonstrates how to implement
-a [slimming](https://arxiv.org/abs/1708.06519) pruner from scratch.
-Additionally, you can find more practical examples in [benchmarks/main.py]
-(benchmarks/main.py). ```python import torch from torchvision.models import
-resnet18 import torch_pruning as tp model = resnet18(pretrained=True) #
-Importance criteria example_inputs = torch.randn(1, 3, 224, 224) imp =
+%20Exploring%20Dependency%20Groups.ipynb) #### How to scan all groups: We can
+use ``DG.get_all_groups(ignored_layers, root_module_types)`` to scan all groups
+sequentially. Each group will begin with a layer that matches a type in the
+"root_module_types" parameter. Note that DG.get_all_groups is only responsible
+for grouping and does not have any knowledge or understanding of which
+parameters should be pruned. Therefore, it is necessary to specify the pruning
+idxs using ``group.prune(idxs=idxs)``. ```python for group in DG.get_all_groups
+(ignored_layers=[model.conv1], root_module_types=[nn.Conv2d, nn.Linear]): #
+handle groups in sequential order idxs = [2,4,6] # your pruning indices
+group.prune(idxs=idxs) print(group) ``` ### 2. High-level Pruners Leveraging
+the DependencyGraph, we developed several high-level pruners in this repository
+to facilitate effortless pruning. By specifying the desired channel sparsity,
+you can prune the entire model and fine-tune it using your own training code.
+For detailed information on this process, please refer to [this tutorial]
+(https://github.com/VainF/Torch-Pruning/blob/master/tutorials/1%20-
+%20Customize%20Your%20Own%20Pruners.ipynb), which shows how to implement a
+[slimming](https://arxiv.org/abs/1708.06519) pruner from scratch. Additionally,
+you can find more practical examples in [benchmarks/main.py](benchmarks/
+main.py). ```python import torch from torchvision.models import resnet18 import
+torch_pruning as tp model = resnet18(pretrained=True) # Importance criteria
+example_inputs = torch.randn(1, 3, 224, 224) imp =
 tp.importance.MagnitudeImportance(p=2) ignored_layers = [] for m in
 model.modules(): if isinstance(m, torch.nn.Linear) and m.out_features == 1000:
 ignored_layers.append(m) # DO NOT prune the final classifier! iterative_steps =
 5 # progressive pruning pruner = tp.pruner.MagnitudePruner( model,
 example_inputs, importance=imp, iterative_steps=iterative_steps,
 ch_sparsity=0.5, # remove 50% channels, ResNet18 = {64, 128, 256, 512} =>
 ResNet18_Half = {32, 64, 128, 256} ignored_layers=ignored_layers, ) base_macs,
```

### Comparing `torch-pruning-1.1.4/setup.py` & `torch-pruning-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="torch-pruning",
-    version="v1.1.4",
+    version="v1.1.5",
     author="Gongfan Fang",
     author_email="gongfan@u.nus.edu",
     description="Structural Pruning for Model Acceleration.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/VainF/Torch-Pruning",
     packages=setuptools.find_packages(),
```

### Comparing `torch-pruning-1.1.4/tests/test_customized_layer.py` & `torch-pruning-1.1.5/tests/test_customized_layer.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.4/tests/test_dependency_graph.py` & `torch-pruning-1.1.5/tests/test_dependency_graph.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.4/tests/test_dependency_lenet.py` & `torch-pruning-1.1.5/tests/test_dependency_lenet.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.4/tests/test_fully_connected_layers.py` & `torch-pruning-1.1.5/tests/test_fully_connected_layers.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.4/tests/test_importance.py` & `torch-pruning-1.1.5/tests/test_importance.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.4/tests/test_interactive_pruner.py` & `torch-pruning-1.1.5/tests/test_interactive_pruner.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.4/tests/test_multiple_inputs_and_outputs.py` & `torch-pruning-1.1.5/tests/test_multiple_inputs_and_outputs.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.4/tests/test_pruner.py` & `torch-pruning-1.1.5/tests/test_pruner.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.4/tests/test_pruning_fn.py` & `torch-pruning-1.1.5/tests/test_pruning_fn.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.4/tests/test_reshape.py` & `torch-pruning-1.1.5/tests/test_reshape.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.4/tests/test_unwrapped_parameters.py` & `torch-pruning-1.1.5/tests/test_unwrapped_parameters.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.4/torch_pruning/_helpers.py` & `torch-pruning-1.1.5/torch_pruning/_helpers.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.4/torch_pruning/dependency.py` & `torch-pruning-1.1.5/torch_pruning/dependency.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,27 +142,42 @@
     Each element is defined as a namedtuple('GroupItem', ['dep', 'idxs']).
     A group is a iterable list 
     [ [Dep1, Indices1], [Dep2, Indices2], ..., [DepK, IndicesK] ]
     """
 
     def __init__(self):
         self._group = list()
-        self._DG = None
+
+        self._DG = None # for group.prune(idxs=NEW_IDXS)
 
     def prune(self, idxs=None):
         """Prune all coupled layers in the group
         """
         if idxs is not None:
             module = self._group[0].dep.target.module
             pruning_fn = self._group[0].dep.handler
             new_group = self._DG.get_pruning_group(module, pruning_fn, idxs)
             new_group.prune()
         else:
             for dep, idxs in self._group:
-                dep(idxs)
+                if dep.target.type == ops.OPTYPE.PARAMETER:
+                    old_parameter = dep.target.module
+                    name = self._DG._param_to_name[old_parameter]
+                    self._DG._param_to_name.pop(old_parameter)
+                    pruned_parameter = dep(idxs)
+                    path = name.split('.')
+                    module = self._DG.model
+                    for p in path[:-1]:
+                        module = getattr(module, p)
+                    setattr(module, path[-1], pruned_parameter)
+                    self._DG._param_to_name[pruned_parameter] = name
+                    self._DG.module2node[pruned_parameter] = self._DG.module2node.pop(old_parameter)
+                    self._DG.module2node[pruned_parameter].module = pruned_parameter           
+                else:
+                    dep(idxs)
 
     def add_dep(self, dep, idxs):
         self._group.append(GroupItem(dep=dep, idxs=idxs))
 
     def __getitem__(self, k):
         return self._group[k]
 
@@ -293,30 +308,30 @@
         wrapped_parameters = []
         prunable_module_types = self.REGISTERED_PRUNERS.keys()
         for m in self.model.modules():
             op_type = ops.module2type(m)
             if ( op_type in prunable_module_types and op_type!=ops.OPTYPE.ELEMENTWISE ) or m.__class__ in self.CUSTOMIZED_PRUNERS.keys():
                 wrapped_parameters.extend(list(m.parameters()))
         unwrapped_detected = []
-        param_to_name = {}
+        _param_to_name = {}
         for name, p in self.model.named_parameters():
             is_wrapped = False
             for p_wrapped in wrapped_parameters:
                 if p is p_wrapped:
                     is_wrapped = True
                     break
             if not is_wrapped:
                 unwrapped_detected.append(p)
-                param_to_name[p] = name
+                _param_to_name[p] = name
         if unwrapped_parameters is None:
             unwrapped_parameters = []
-
+        self._param_to_name = _param_to_name
         unwrapped_detected = list( set(unwrapped_detected) - set([p for (p, _) in unwrapped_parameters]) )
         if len(unwrapped_detected)>0 and self.verbose:
-            warnings.warn("Unwrapped parameters detected: {}.\n Torch-Pruning will prune the last non-singleton dimension of a parameter. If you wish to customize this behavior, please provide an unwrapped_parameters argument.".format([param_to_name[p] for p in unwrapped_detected]))
+            warnings.warn("Unwrapped parameters detected: {}.\n Torch-Pruning will prune the last non-singleton dimension of a parameter. If you wish to customize this behavior, please provide an unwrapped_parameters argument.".format([_param_to_name[p] for p in unwrapped_detected]))
         for p in unwrapped_detected:
             # get the last dimension that >1
             def last_non_singleton_dim(tensor):
                 non_singleton_dims = [i for i, s in enumerate(tensor.shape) if s > 1]
                 return non_singleton_dims[-1] if non_singleton_dims else None
             pruning_dim = last_non_singleton_dim(p)
             if pruning_dim is not None:
```

### Comparing `torch-pruning-1.1.4/torch_pruning/importance.py` & `torch-pruning-1.1.5/torch_pruning/importance.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.4/torch_pruning/ops.py` & `torch-pruning-1.1.5/torch_pruning/ops.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.4/torch_pruning/pruner/algorithms/batchnorm_scale_pruner.py` & `torch-pruning-1.1.5/torch_pruning/pruner/algorithms/batchnorm_scale_pruner.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.4/torch_pruning/pruner/algorithms/group_norm_pruner.py` & `torch-pruning-1.1.5/torch_pruning/pruner/algorithms/group_norm_pruner.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.4/torch_pruning/pruner/algorithms/metapruner.py` & `torch-pruning-1.1.5/torch_pruning/pruner/algorithms/metapruner.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,16 @@
     def estimate_importance(self, group, ch_groups=1):
         return self.importance(group, ch_groups=ch_groups)
 
     def _check_sparsity(self, group):
         for dep, _ in group:
             module = dep.target.module
             pruning_fn = dep.handler
+            if dep.target.type == ops.OPTYPE.PARAMETER:
+                continue
             if self.DG.is_out_channel_pruning_fn(pruning_fn):
                 target_sparsity = self.get_target_sparsity(module)
                 layer_out_ch = self.DG.get_out_channels(module)
                 if layer_out_ch is None: continue
                 if layer_out_ch < self.layer_init_out_ch[module] * (
                     1 - self.max_ch_sparsity
                 ) or layer_out_ch == 1:
```

### Comparing `torch-pruning-1.1.4/torch_pruning/pruner/function.py` & `torch-pruning-1.1.5/torch_pruning/pruner/function.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,34 +87,34 @@
 
     def prune_out_channels(self, layer: nn.Module, idxs: Sequence[int]) -> nn.Module:
         keep_idxs = list(set(range(layer.out_channels)) - set(idxs))
         keep_idxs.sort()
         layer.out_channels = layer.out_channels-len(idxs)
         if not layer.transposed:
             layer.weight = torch.nn.Parameter(
-                layer.weight.data.clone()[keep_idxs])
+                layer.weight.data[keep_idxs])
         else:
             layer.weight = torch.nn.Parameter(
-                layer.weight.data.clone()[:, keep_idxs])
+                layer.weight.data[:, keep_idxs])
         if layer.bias is not None:
-            layer.bias = torch.nn.Parameter(layer.bias.data.clone()[keep_idxs])
+            layer.bias = torch.nn.Parameter(layer.bias.data[keep_idxs])
         return layer
 
     def prune_in_channels(self, layer: nn.Module, idxs: Sequence[int]) -> nn.Module:
         keep_idxs = list(set(range(layer.in_channels)) - set(idxs))
         keep_idxs.sort()
         layer.in_channels = layer.in_channels - len(idxs)
         if layer.groups>1:
             keep_idxs = keep_idxs[:len(keep_idxs)//layer.groups]
         if not layer.transposed:
             layer.weight = torch.nn.Parameter(
-                layer.weight.data.clone()[:, keep_idxs])
+                layer.weight.data[:, keep_idxs])
         else:
             layer.weight = torch.nn.Parameter(
-                layer.weight.data.clone()[keep_idxs])
+                layer.weight.data[keep_idxs])
         # no bias pruning because it does not change the output channels
         return layer
 
     def get_out_channels(self, layer):
         return layer.out_channels
 
     def get_in_channels(self, layer):
@@ -126,42 +126,42 @@
 
     def prune_out_channels(self, layer: nn.Module, idxs: Sequence[int]) -> nn.Module:
         keep_idxs = list(set(range(layer.out_channels)) - set(idxs))
         keep_idxs.sort()
         layer.out_channels = layer.out_channels-len(idxs)
         layer.in_channels = layer.in_channels-len(idxs)
         layer.groups = layer.groups-len(idxs)
-        layer.weight = torch.nn.Parameter(layer.weight.data.clone()[keep_idxs])
+        layer.weight = torch.nn.Parameter(layer.weight.data[keep_idxs])
         if layer.bias is not None:
-            layer.bias = torch.nn.Parameter(layer.bias.data.clone()[keep_idxs])
+            layer.bias = torch.nn.Parameter(layer.bias.data[keep_idxs])
         return layer
 
     prune_in_channels = prune_out_channels
     # def prune_input(self, layer: nn.Module, idxs: Sequence[int]) -> nn.Module:
     #    return self.prune_output(layer, idxs)
 
 
 class LinearPruner(BasePruningFunc):
     TARGET_MODULES = ops.TORCH_LINEAR
 
     def prune_out_channels(self, layer: nn.Module, idxs: Sequence[int]) -> nn.Module:
         keep_idxs = list(set(range(layer.out_features)) - set(idxs))
         keep_idxs.sort()
         layer.out_features = layer.out_features-len(idxs)
-        layer.weight = torch.nn.Parameter(layer.weight.data.clone()[keep_idxs])
+        layer.weight = torch.nn.Parameter(layer.weight.data[keep_idxs])
         if layer.bias is not None:
-            layer.bias = torch.nn.Parameter(layer.bias.data.clone()[keep_idxs])
+            layer.bias = torch.nn.Parameter(layer.bias.data[keep_idxs])
         return layer
 
     def prune_in_channels(self, layer: nn.Module, idxs: Sequence[int]) -> nn.Module:
         keep_idxs = list(set(range(layer.in_features)) - set(idxs))
         keep_idxs.sort()
         layer.in_features = layer.in_features-len(idxs)
         layer.weight = torch.nn.Parameter(
-            layer.weight.data.clone()[:, keep_idxs])
+            layer.weight.data[:, keep_idxs])
         return layer
 
     def get_out_channels(self, layer):
         return layer.out_features
 
     def get_in_channels(self, layer):
         return layer.in_features
@@ -170,20 +170,20 @@
 class BatchnormPruner(BasePruningFunc):
     TARGET_MODULES = ops.TORCH_BATCHNORM
 
     def prune_out_channels(self, layer: nn.Module, idxs: Sequence[int]) -> nn.Module:
         keep_idxs = list(set(range(layer.num_features)) - set(idxs))
         keep_idxs.sort()
         layer.num_features = layer.num_features-len(idxs)
-        layer.running_mean = layer.running_mean.data.clone()[keep_idxs]
-        layer.running_var = layer.running_var.data.clone()[keep_idxs]
+        layer.running_mean = layer.running_mean.data[keep_idxs]
+        layer.running_var = layer.running_var.data[keep_idxs]
         if layer.affine:
             layer.weight = torch.nn.Parameter(
-                layer.weight.data.clone()[keep_idxs])
-            layer.bias = torch.nn.Parameter(layer.bias.data.clone()[keep_idxs])
+                layer.weight.data[keep_idxs])
+            layer.bias = torch.nn.Parameter(layer.bias.data[keep_idxs])
         return layer
 
     prune_in_channels = prune_out_channels
     # def prune_in_channels(self, layer: nn.Module, idxs: Sequence[int]) -> nn.Module:
     #    return self.prune_out_channels(layer=layer, idxs=idxs)
 
     def get_out_channels(self, layer):
@@ -208,17 +208,17 @@
         if len(layer.normalized_shape) < -pruning_dim:
             return layer
         num_features = layer.normalized_shape[pruning_dim]
         keep_idxs = torch.tensor(list(set(range(num_features)) - set(idxs)))
         keep_idxs.sort()
         if layer.elementwise_affine:
             layer.weight = torch.nn.Parameter(
-                layer.weight.data.clone().index_select(pruning_dim, keep_idxs))
+                layer.weight.data.index_select(pruning_dim, keep_idxs))
             layer.bias = torch.nn.Parameter(
-                layer.bias.data.clone().index_select(pruning_dim, keep_idxs))
+                layer.bias.data.index_select(pruning_dim, keep_idxs))
         if pruning_dim != -1:
             layer.normalized_shape = layer.normalized_shape[:pruning_dim] + (
                 keep_idxs.size(0), ) + layer.normalized_shape[pruning_dim+1:]
         else:
             layer.normalized_shape = layer.normalized_shape[:pruning_dim] + (
                 keep_idxs.size(0), )
         return layer
@@ -234,16 +234,16 @@
 class GroupNormPruner(BasePruningFunc):
     def prune_out_channels(self, layer: nn.PReLU, idxs: list) -> nn.Module:
         keep_idxs = list(set(range(layer.num_channels)) - set(idxs))
         keep_idxs.sort()
         layer.num_channels = layer.num_channels-len(idxs)
         if layer.affine:
             layer.weight = torch.nn.Parameter(
-                layer.weight.data.clone()[keep_idxs])
-            layer.bias = torch.nn.Parameter(layer.bias.data.clone()[keep_idxs])
+                layer.weight.data[keep_idxs])
+            layer.bias = torch.nn.Parameter(layer.bias.data[keep_idxs])
         return layer
     
     prune_in_channels = prune_out_channels
 
     def get_out_channels(self, layer):
         return layer.num_channels
 
@@ -253,16 +253,16 @@
 class InstanceNormPruner(BasePruningFunc):
     def prune_out_channels(self, layer: nn.Module, idxs: Sequence[int]) -> nn.Module:
         keep_idxs = list(set(range(layer.num_features)) - set(idxs))
         keep_idxs.sort()
         layer.num_features = layer.num_features-len(idxs)
         if layer.affine:
             layer.weight = torch.nn.Parameter(
-                layer.weight.data.clone()[keep_idxs])
-            layer.bias = torch.nn.Parameter(layer.bias.data.clone()[keep_idxs])
+                layer.weight.data[keep_idxs])
+            layer.bias = torch.nn.Parameter(layer.bias.data[keep_idxs])
         return layer
 
     prune_in_channels = prune_out_channels
 
     def get_out_channels(self, layer):
         return layer.num_features
 
@@ -275,15 +275,15 @@
 
     def prune_out_channels(self, layer: nn.PReLU, idxs: list) -> nn.Module:
         if layer.num_parameters == 1:
             return layer
         keep_idxs = list(set(range(layer.num_parameters)) - set(idxs))
         keep_idxs.sort()
         layer.num_parameters = layer.num_parameters-len(idxs)
-        layer.weight = torch.nn.Parameter(layer.weight.data.clone()[keep_idxs])
+        layer.weight = torch.nn.Parameter(layer.weight.data[keep_idxs])
         return layer
 
     prune_in_channels = prune_out_channels
 
     # def prune_in_channels(self, layer:nn.Module, idxs: Sequence[int]) -> nn.Module:
     #    return self.prune_out_channels(layer=layer, idxs=idxs)
 
@@ -300,15 +300,15 @@
     TARGET_MODULES = ops.TORCH_EMBED
 
     def prune_out_channels(self, layer: nn.Embedding, idxs: list) -> nn.Module:
         num_features = layer.embedding_dim
         keep_idxs = list(set(range(num_features)) - set(idxs))
         keep_idxs.sort()
         layer.weight = torch.nn.Parameter(
-            layer.weight.data.clone()[:, keep_idxs])
+            layer.weight.data[:, keep_idxs])
         layer.embedding_dim = len(keep_idxs)
         return layer
 
     prune_in_channels = prune_out_channels
 
     # def prune_in_channels(self, layer: nn.Embedding, idxs: list)-> nn.Module:
     #    return self.prune_out_channels(layer=layer, idxs=idxs)
@@ -333,37 +333,37 @@
         if layer.bidirectional:
             postfix = ['', '_reverse']
         else:
             postfix = ['']
         #for l in range(num_layers):
         for pf in postfix:
             setattr(layer, 'weight_hh_l0'+pf, torch.nn.Parameter(
-                getattr(layer, 'weight_hh_l0'+pf).data.clone()[expanded_keep_idxs]))
+                getattr(layer, 'weight_hh_l0'+pf).data[expanded_keep_idxs]))
             if layer.bias:
                 setattr(layer, 'bias_hh_l0'+pf, torch.nn.Parameter(
-                    getattr(layer, 'bias_hh_l0'+pf).data.clone()[expanded_keep_idxs]))
+                    getattr(layer, 'bias_hh_l0'+pf).data[expanded_keep_idxs]))
             setattr(layer, 'weight_hh_l0'+pf, torch.nn.Parameter(
-                getattr(layer, 'weight_hh_l0'+pf).data.clone()[:, keep_idxs]))
+                getattr(layer, 'weight_hh_l0'+pf).data[:, keep_idxs]))
 
             setattr(layer, 'weight_ih_l0'+pf, torch.nn.Parameter(
-                getattr(layer, 'weight_ih_l0'+pf).data.clone()[expanded_keep_idxs]))
+                getattr(layer, 'weight_ih_l0'+pf).data[expanded_keep_idxs]))
             if layer.bias:
                 setattr(layer, 'bias_ih_l0'+pf, torch.nn.Parameter(
-                    getattr(layer, 'bias_ih_l0'+pf).data.clone()[expanded_keep_idxs]))
+                    getattr(layer, 'bias_ih_l0'+pf).data[expanded_keep_idxs]))
         layer.hidden_size = len(keep_idxs)
 
     def prune_in_channels(self, layer: nn.LSTM, idxs: list):
         num_features = layer.input_size
         keep_idxs = list(set(range(num_features)) - set(idxs))
         keep_idxs.sort()
         setattr(layer, 'weight_ih_l0', torch.nn.Parameter(
-                    getattr(layer, 'weight_ih_l0').data.clone()[:, keep_idxs]))
+                    getattr(layer, 'weight_ih_l0').data[:, keep_idxs]))
         if layer.bidirectional:
             setattr(layer, 'weight_ih_l0_reverse', torch.nn.Parameter(
-                    getattr(layer, 'weight_ih_l0_reverse').data.clone()[:, keep_idxs]))
+                    getattr(layer, 'weight_ih_l0_reverse').data[:, keep_idxs]))
         layer.input_size = len(keep_idxs)
 
     def get_out_channels(self, layer):
         return layer.hidden_size
         
     def get_in_channels(self, layer):
         return layer.input_size
@@ -373,17 +373,17 @@
     TARGET_MODULES = ops.TORCH_PARAMETER
     def __init__(self, pruning_dim=-1):
         super().__init__(pruning_dim=pruning_dim)
         
     def prune_out_channels(self, tensor, idxs: list) -> nn.Module:
         keep_idxs = list(set(range(tensor.data.shape[self.pruning_dim])) - set(idxs))
         keep_idxs.sort()
-        tensor.data = torch.index_select(
-            tensor.data, self.pruning_dim, torch.LongTensor(keep_idxs).to(tensor.device))
-        return tensor
+        pruned_parameter = nn.Parameter(torch.index_select(
+            tensor.data, self.pruning_dim, torch.LongTensor(keep_idxs).to(tensor.device)))
+        return pruned_parameter
 
     prune_in_channels = prune_out_channels
 
     def get_out_channels(self, parameter):
         return parameter.shape[self.pruning_dim]
 
     def get_in_channels(self, parameter):
@@ -396,69 +396,73 @@
     def check(self, layer, idxs, to_output):
         super().check(layer, idxs, to_output)
         assert (layer.embed_dim - len(idxs)) % layer.num_heads == 0, "embed_dim (%d) of MultiheadAttention after pruning must divide evenly by `num_heads` (%d)" % (layer.embed_dim, layer.num_heads)
 
     def prune_out_channels(self, layer, idxs: list) -> nn.Module:
         keep_idxs = list(set(range(layer.embed_dim)) - set(idxs))
         keep_idxs.sort()
+
+
         if layer.q_proj_weight is not None:
-            layer.q_proj_weight.data = torch.index_select(
-                layer.q_proj_weight.data, 0, torch.LongTensor(keep_idxs))
+            layer.q_proj_weight = nn.Parameter(torch.index_select(
+                layer.q_proj_weight.data, 0, torch.LongTensor(keep_idxs)))
         if layer.k_proj_weight is not None:
-            layer.q_proj_weight.data = torch.index_select(
-                layer.q_proj_weight.data, 0, torch.LongTensor(keep_idxs))
+            layer.q_proj_weight = nn.Parameter(torch.index_select(
+                layer.q_proj_weight.data, 0, torch.LongTensor(keep_idxs)))
         if layer.v_proj_weight is not None:
-            layer.v_proj_weight.data = torch.index_select(
-                layer.v_proj_weight.data, 0, torch.LongTensor(keep_idxs))
+            layer.v_proj_weight = nn.Parameter(torch.index_select(
+                layer.v_proj_weight.data, 0, torch.LongTensor(keep_idxs)))
+
 
         pruning_idxs_repeated = idxs + \
             [i+layer.embed_dim for i in idxs] + \
             [i+2*layer.embed_dim for i in idxs]
         keep_idxs_3x_repeated = list(
             set(range(3*layer.embed_dim)) - set(pruning_idxs_repeated))
         keep_idxs_3x_repeated.sort()
         if layer.in_proj_weight is not None:
-            layer.in_proj_weight.data = torch.index_select(
-                layer.in_proj_weight.data, 0, torch.LongTensor(keep_idxs_3x_repeated))
-            layer.in_proj_weight.data = torch.index_select(
-                layer.in_proj_weight.data, 1, torch.LongTensor(keep_idxs))
-
+            layer.in_proj_weight = nn.Parameter(torch.index_select(
+                layer.in_proj_weight.data, 0, torch.LongTensor(keep_idxs_3x_repeated)))
+            layer.in_proj_weight = nn.Parameter(torch.index_select(
+                layer.in_proj_weight.data, 1, torch.LongTensor(keep_idxs)))
         if layer.in_proj_bias is not None:
-            layer.in_proj_bias.data = torch.index_select(
-                layer.in_proj_bias.data, 0, torch.LongTensor(keep_idxs_3x_repeated))
+            layer.in_proj_bias = nn.Parameter(torch.index_select(
+                layer.in_proj_bias.data, 0, torch.LongTensor(keep_idxs_3x_repeated)))
+
 
         if layer.bias_k is not None:
-            layer.bias_k.data = torch.index_select(
-                layer.bias_k.data, 2, torch.LongTensor(keep_idxs))
+            layer.bias_k = nn.Parameter(torch.index_select(
+                layer.bias_k.data, 2, torch.LongTensor(keep_idxs)))
         if layer.bias_v is not None:
-            layer.bias_v.data = torch.index_select(
-                layer.bias_v.data, 2, torch.LongTensor(keep_idxs))
+            layer.bias_v = nn.Parameter(torch.index_select(
+                layer.bias_v.data, 2, torch.LongTensor(keep_idxs)))
 
         linear = layer.out_proj
         keep_idxs = list(set(range(linear.out_features)) - set(idxs))
         keep_idxs.sort()
         linear.out_features = linear.out_features-len(idxs)
         linear.weight = torch.nn.Parameter(
-            linear.weight.data.clone()[keep_idxs])
+            linear.weight.data[keep_idxs])
         if linear.bias is not None:
             linear.bias = torch.nn.Parameter(
-                linear.bias.data.clone()[keep_idxs])
+                linear.bias.data[keep_idxs])
         keep_idxs = list(set(range(linear.in_features)) - set(idxs))
         keep_idxs.sort()
         linear.in_features = linear.in_features-len(idxs)
         linear.weight = torch.nn.Parameter(
-            linear.weight.data.clone()[:, keep_idxs])
+            linear.weight.data[:, keep_idxs])
+
         layer.embed_dim = layer.embed_dim - len(idxs)
+        layer.head_dim = layer.embed_dim // layer.num_heads
+        layer.kdim = layer.embed_dim
+        layer.vdim = layer.embed_dim
         return layer
 
     prune_in_channels = prune_out_channels
 
-    # def prune_in_channels(self, layer, idxs: list)-> nn.Module:
-    #    return self.prune_out_channels(layer=layer, idxs=idxs)
-
     def get_out_channels(self, layer):
         return layer.embed_dim
 
     def get_in_channels(self, layer):
         return self.get_out_channels(layer)
 
 PrunerBox = {
```

### Comparing `torch-pruning-1.1.4/torch_pruning/utils/op_counter.py` & `torch-pruning-1.1.5/torch_pruning/utils/op_counter.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.4/torch_pruning/utils/utils.py` & `torch-pruning-1.1.5/torch_pruning/utils/utils.py`

 * *Files identical despite different names*

### Comparing `torch-pruning-1.1.4/torch_pruning.egg-info/PKG-INFO` & `torch-pruning-1.1.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,30 @@
-Metadata-Version: 2.1
-Name: torch-pruning
-Version: 1.1.4
-Summary: Structural Pruning for Model Acceleration.
-Home-page: https://github.com/VainF/Torch-Pruning
-Author: Gongfan Fang
-Author-email: gongfan@u.nus.edu
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center"> <h1>Torch-Pruning <br> <h3>Towards Any Structural Pruning<h3> </h1> </div>
 <div align="center">
-<img src="assets/intro.png" width="45%">
+<img src="assets/intro.png" width="50%">
 </div>
 
 <p align="center">
   <a href="https://github.com/VainF/Torch-Pruning/actions"><img src="https://img.shields.io/badge/tests-passing-9c27b0.svg" alt="Test Status"></a>
   <a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-1.8.1%20%7C%202.0.0-673ab7.svg" alt="Tested PyTorch Versions"></a>
   <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-4caf50.svg" alt="License"></a>
   <a href="https://pepy.tech/project/Torch-Pruning"><img src="https://pepy.tech/badge/Torch-Pruning?color=2196f3" alt="Downloads"></a>
-  <a href="https://github.com/VainF/Torch-Pruning/releases/latest"><img src="https://img.shields.io/badge/Latest%20Version-1.1.3-3f51b5.svg" alt="Latest Version"></a>
+  <a href="https://github.com/VainF/Torch-Pruning/releases/latest"><img src="https://img.shields.io/badge/Latest%20Version-1.1.4-3f51b5.svg" alt="Latest Version"></a>
+  <a href="https://colab.research.google.com/drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing">
+  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
+</a>
   <a href="https://arxiv.org/abs/2301.12900" target="_blank"><img src="https://img.shields.io/badge/arXiv-2301.12900-009688.svg" alt="arXiv"></a>
 </p>
 
 
 [[中文README | README in Chinese]](README_CN.md)
 
 Torch-Pruning (TP) is a versatile library for Structural Network Pruning with the following features:
 * **General-purpose Pruning Toolkit:** TP enables structural pruning for a wide range of neural networks, including *Vision Transformers, Yolov7, FasterRCNN, SSD, KeypointRCNN, MaskRCNN, ResNe(X)t, ConvNext, DenseNet, ConvNext, RegNet, FCN, DeepLab, etc*. Different from [torch.nn.utils.prune](https://pytorch.org/tutorials/intermediate/pruning_tutorial.html) that zeroizes parameters through masking, Torch-Pruning employs a (non-deep) graph algorithm called DepGraph to physically remove coupled parameters (channels) from models. 
-* **Reproducible [Performance Benchmark](benchmarks) and [Prunability Benchmark](benchmarks/prunability):** Currently, TP is able to prune approximately **77/85=90.6%** of the models from Torchvision 0.13.1. Check out [practical_structural_pruning.md](practical_structural_pruning.md) for an up-to-date list of practical pruning techniques. 
-
+* **Reproducible [Performance Benchmark](benchmarks) and [Prunability Benchmark](benchmarks/prunability):** Currently, TP is able to prune approximately **77/85=90.6%** of the models from Torchvision 0.13.1. Try this [Colab Demo](https://colab.research.google.com/drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing) for quick start.
 
 For more technical details, please refer to our CVPR'23 paper:
 > [**DepGraph: Towards Any Structural Pruning**](https://arxiv.org/abs/2301.12900)   
 > [Gongfan Fang](https://fangggf.github.io/), [Xinyin Ma](https://horseee.github.io/), [Mingli Song](https://person.zju.edu.cn/en/msong), [Michael Bi Mi](https://dblp.org/pid/317/0937.html), [Xinchao Wang](https://sites.google.com/site/sitexinchaowang/)   
 
 Please do not hesitate to open a [discussion](https://github.com/VainF/Torch-Pruning/discussions) or [issue](https://github.com/VainF/Torch-Pruning/issues) if you encounter any problems with the library or the paper. 
 
@@ -59,15 +47,15 @@
 - [ ] More standard layers: GroupNorm, InstanceNorm, Shuffle Layers, etc.
 - [ ] More Transformers like Vision Transformers (:heavy_check_mark:), Swin Transformers, PoolFormers.
 - [ ] Block/Layer/Depth Pruning
 - [ ] Pruning benchmarks for CIFAR, ImageNet and COCO.
 
 ## Installation
 ```bash
-pip install torch-pruning # v1.1.3
+pip install torch-pruning # v1.1.4
 ```
 or
 ```bash
 git clone https://github.com/VainF/Torch-Pruning.git # recommended
 ```
 
 ## Quickstart
@@ -129,28 +117,28 @@
 [14] prune_out_channels on layer1.1.bn2 (BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)) => prune_out_channels on layer1.1.conv2 (Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)), idxs=[2, 6, 9]
 [15] prune_out_channels on layer1.0.bn2 (BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)) => prune_out_channels on layer1.0.conv2 (Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)), idxs=[2, 6, 9]
 --------------------------------
 ```
 For more details about grouping, please refer to [tutorials/2 - Exploring Dependency Groups](https://github.com/VainF/Torch-Pruning/blob/master/tutorials/2%20-%20Exploring%20Dependency%20Groups.ipynb)
 
 #### How to scan all groups:
-Just like what we do in the [MetaPruner](https://github.com/VainF/Torch-Pruning/blob/b607ae3aa61b9dafe19d2c2364f7e4984983afbf/torch_pruning/pruner/algorithms/metapruner.py#L197), one can use ``DG.get_all_groups(ignored_layers, root_module_types)`` to scan all groups sequentially. Each group will begin with a layer that matches a type in the "root_module_types" parameter. Note that DG.get_all_groups is only responsible for grouping and does not have any knowledge or understanding of which parameters should be pruned. Therefore, it is necessary to specify the pruning idxs using  ``group.prune(idxs=idxs)``.
+We can use ``DG.get_all_groups(ignored_layers, root_module_types)`` to scan all groups sequentially. Each group will begin with a layer that matches a type in the "root_module_types" parameter. Note that DG.get_all_groups is only responsible for grouping and does not have any knowledge or understanding of which parameters should be pruned. Therefore, it is necessary to specify the pruning idxs using  ``group.prune(idxs=idxs)``.
 
 ```python
 for group in DG.get_all_groups(ignored_layers=[model.conv1], root_module_types=[nn.Conv2d, nn.Linear]):
     # handle groups in sequential order
     idxs = [2,4,6] # your pruning indices
     group.prune(idxs=idxs)
     print(group)
 ```
 
 
 ### 2. High-level Pruners
 
-Leveraging the DependencyGraph, we developed several high-level pruners in this repository to facilitate effortless pruning. By specifying the desired channel sparsity, you can prune the entire model and fine-tune it using your own training code. For detailed information on this process, we encourage you to consult the [this tutorial](https://github.com/VainF/Torch-Pruning/blob/master/tutorials/1%20-%20Customize%20Your%20Own%20Pruners.ipynb), which demonstrates how to implement a [slimming](https://arxiv.org/abs/1708.06519) pruner from scratch. Additionally, you can find more practical examples in [benchmarks/main.py](benchmarks/main.py).
+Leveraging the DependencyGraph, we developed several high-level pruners in this repository to facilitate effortless pruning. By specifying the desired channel sparsity, you can prune the entire model and fine-tune it using your own training code. For detailed information on this process, please refer to [this tutorial](https://github.com/VainF/Torch-Pruning/blob/master/tutorials/1%20-%20Customize%20Your%20Own%20Pruners.ipynb), which shows how to implement a [slimming](https://arxiv.org/abs/1708.06519) pruner from scratch. Additionally, you can find more practical examples in [benchmarks/main.py](benchmarks/main.py).
 
 ```python
 import torch
 from torchvision.models import resnet18
 import torch_pruning as tp
 
 model = resnet18(pretrained=True)
```

#### html2text {}

```diff
@@ -1,33 +1,27 @@
-Metadata-Version: 2.1 Name: torch-pruning Version: 1.1.4 Summary: Structural
-Pruning for Model Acceleration. Home-page: https://github.com/VainF/Torch-
-Pruning Author: Gongfan Fang Author-email: gongfan@u.nus.edu Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE
                              ****** Torch-Pruning
                      Towards Any Structural Pruning ******
                               [assets/intro.png]
 [Test_Status] [Tested_PyTorch_Versions] [License] [Downloads] [Latest_Version]
-                                    [arXiv]
+                            [Open_In_Colab] [arXiv]
 [[ä¸­æREADME | README in Chinese]](README_CN.md) Torch-Pruning (TP) is a
 versatile library for Structural Network Pruning with the following features: *
 **General-purpose Pruning Toolkit:** TP enables structural pruning for a wide
 range of neural networks, including *Vision Transformers, Yolov7, FasterRCNN,
 SSD, KeypointRCNN, MaskRCNN, ResNe(X)t, ConvNext, DenseNet, ConvNext, RegNet,
 FCN, DeepLab, etc*. Different from [torch.nn.utils.prune](https://pytorch.org/
 tutorials/intermediate/pruning_tutorial.html) that zeroizes parameters through
 masking, Torch-Pruning employs a (non-deep) graph algorithm called DepGraph to
 physically remove coupled parameters (channels) from models. * **Reproducible
 [Performance Benchmark](benchmarks) and [Prunability Benchmark](benchmarks/
 prunability):** Currently, TP is able to prune approximately **77/85=90.6%** of
-the models from Torchvision 0.13.1. Check out [practical_structural_pruning.md]
-(practical_structural_pruning.md) for an up-to-date list of practical pruning
-techniques. For more technical details, please refer to our CVPR'23 paper: >
-[**DepGraph: Towards Any Structural Pruning**](https://arxiv.org/abs/
+the models from Torchvision 0.13.1. Try this [Colab Demo](https://
+colab.research.google.com/drive/1TRvELQDNj9PwM-EERWbF3IQOyxZeDepp?usp=sharing)
+for quick start. For more technical details, please refer to our CVPR'23 paper:
+> [**DepGraph: Towards Any Structural Pruning**](https://arxiv.org/abs/
 2301.12900) > [Gongfan Fang](https://fangggf.github.io/), [Xinyin Ma](https://
 horseee.github.io/), [Mingli Song](https://person.zju.edu.cn/en/msong),
 [Michael Bi Mi](https://dblp.org/pid/317/0937.html), [Xinchao Wang](https://
 sites.google.com/site/sitexinchaowang/) Please do not hesitate to open a
 [discussion](https://github.com/VainF/Torch-Pruning/discussions) or [issue]
 (https://github.com/VainF/Torch-Pruning/issues) if you encounter any problems
 with the library or the paper. ### **Features:** - [x] Structural (Channel)
@@ -54,15 +48,15 @@
 YOLOv8) - [ ] Pruning from Scratch / at Initialization. - [ ] Language, Speech
 and Generative Models. - [ ] More high-level pruners like [FisherPruner](https:
 //arxiv.org/abs/2108.00708), [GrowingReg](https://arxiv.org/abs/2012.09243),
 etc. - [ ] More standard layers: GroupNorm, InstanceNorm, Shuffle Layers, etc.
 - [ ] More Transformers like Vision Transformers (:heavy_check_mark:), Swin
 Transformers, PoolFormers. - [ ] Block/Layer/Depth Pruning - [ ] Pruning
 benchmarks for CIFAR, ImageNet and COCO. ## Installation ```bash pip install
-torch-pruning # v1.1.3 ``` or ```bash git clone https://github.com/VainF/Torch-
+torch-pruning # v1.1.4 ``` or ```bash git clone https://github.com/VainF/Torch-
 Pruning.git # recommended ``` ## Quickstart Here we provide a quick start for
 Torch-Pruning. More explained details can be found in [tutorals](./tutorials/
 ) ### 0. How It Works In structural pruning, **a ``Group`` constitutes the
 minimal prunable unit within deep networks**. Each group typically comprises
 several interdependent parameters that must be removed simultaneously to
 maintain the integrity of the resulting structures. However, deep networks
 often present complex dependencies among parameters, making structural pruning
@@ -127,38 +121,35 @@
 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)), idxs=[2,
 6, 9] [15] prune_out_channels on layer1.0.bn2 (BatchNorm2d(64, eps=1e-05,
 momentum=0.1, affine=True, track_running_stats=True)) => prune_out_channels on
 layer1.0.conv2 (Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1,
 1), bias=False)), idxs=[2, 6, 9] -------------------------------- ``` For more
 details about grouping, please refer to [tutorials/2 - Exploring Dependency
 Groups](https://github.com/VainF/Torch-Pruning/blob/master/tutorials/2%20-
-%20Exploring%20Dependency%20Groups.ipynb) #### How to scan all groups: Just
-like what we do in the [MetaPruner](https://github.com/VainF/Torch-Pruning/
-blob/b607ae3aa61b9dafe19d2c2364f7e4984983afbf/torch_pruning/pruner/algorithms/
-metapruner.py#L197), one can use ``DG.get_all_groups(ignored_layers,
-root_module_types)`` to scan all groups sequentially. Each group will begin
-with a layer that matches a type in the "root_module_types" parameter. Note
-that DG.get_all_groups is only responsible for grouping and does not have any
-knowledge or understanding of which parameters should be pruned. Therefore, it
-is necessary to specify the pruning idxs using ``group.prune(idxs=idxs)``.
-```python for group in DG.get_all_groups(ignored_layers=[model.conv1],
-root_module_types=[nn.Conv2d, nn.Linear]): # handle groups in sequential order
-idxs = [2,4,6] # your pruning indices group.prune(idxs=idxs) print(group) ```
-### 2. High-level Pruners Leveraging the DependencyGraph, we developed several
-high-level pruners in this repository to facilitate effortless pruning. By
-specifying the desired channel sparsity, you can prune the entire model and
-fine-tune it using your own training code. For detailed information on this
-process, we encourage you to consult the [this tutorial](https://github.com/
-VainF/Torch-Pruning/blob/master/tutorials/1%20-
-%20Customize%20Your%20Own%20Pruners.ipynb), which demonstrates how to implement
-a [slimming](https://arxiv.org/abs/1708.06519) pruner from scratch.
-Additionally, you can find more practical examples in [benchmarks/main.py]
-(benchmarks/main.py). ```python import torch from torchvision.models import
-resnet18 import torch_pruning as tp model = resnet18(pretrained=True) #
-Importance criteria example_inputs = torch.randn(1, 3, 224, 224) imp =
+%20Exploring%20Dependency%20Groups.ipynb) #### How to scan all groups: We can
+use ``DG.get_all_groups(ignored_layers, root_module_types)`` to scan all groups
+sequentially. Each group will begin with a layer that matches a type in the
+"root_module_types" parameter. Note that DG.get_all_groups is only responsible
+for grouping and does not have any knowledge or understanding of which
+parameters should be pruned. Therefore, it is necessary to specify the pruning
+idxs using ``group.prune(idxs=idxs)``. ```python for group in DG.get_all_groups
+(ignored_layers=[model.conv1], root_module_types=[nn.Conv2d, nn.Linear]): #
+handle groups in sequential order idxs = [2,4,6] # your pruning indices
+group.prune(idxs=idxs) print(group) ``` ### 2. High-level Pruners Leveraging
+the DependencyGraph, we developed several high-level pruners in this repository
+to facilitate effortless pruning. By specifying the desired channel sparsity,
+you can prune the entire model and fine-tune it using your own training code.
+For detailed information on this process, please refer to [this tutorial]
+(https://github.com/VainF/Torch-Pruning/blob/master/tutorials/1%20-
+%20Customize%20Your%20Own%20Pruners.ipynb), which shows how to implement a
+[slimming](https://arxiv.org/abs/1708.06519) pruner from scratch. Additionally,
+you can find more practical examples in [benchmarks/main.py](benchmarks/
+main.py). ```python import torch from torchvision.models import resnet18 import
+torch_pruning as tp model = resnet18(pretrained=True) # Importance criteria
+example_inputs = torch.randn(1, 3, 224, 224) imp =
 tp.importance.MagnitudeImportance(p=2) ignored_layers = [] for m in
 model.modules(): if isinstance(m, torch.nn.Linear) and m.out_features == 1000:
 ignored_layers.append(m) # DO NOT prune the final classifier! iterative_steps =
 5 # progressive pruning pruner = tp.pruner.MagnitudePruner( model,
 example_inputs, importance=imp, iterative_steps=iterative_steps,
 ch_sparsity=0.5, # remove 50% channels, ResNet18 = {64, 128, 256, 512} =>
 ResNet18_Half = {32, 64, 128, 256} ignored_layers=ignored_layers, ) base_macs,
```

### Comparing `torch-pruning-1.1.4/torch_pruning.egg-info/SOURCES.txt` & `torch-pruning-1.1.5/torch_pruning.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 setup.py
+tests/test_backward.py
 tests/test_customized_layer.py
 tests/test_dependency_graph.py
 tests/test_dependency_lenet.py
 tests/test_fully_connected_layers.py
 tests/test_importance.py
 tests/test_interactive_pruner.py
 tests/test_multiple_inputs_and_outputs.py
```

