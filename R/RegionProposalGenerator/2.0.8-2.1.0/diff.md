# Comparing `tmp/RegionProposalGenerator-2.0.8.tar.gz` & `tmp/RegionProposalGenerator-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RegionProposalGenerator-2.0.8.tar", last modified: Sun Apr 17 01:01:48 2022, max compression
+gzip compressed data, was "RegionProposalGenerator-2.1.0.tar", last modified: Sun Apr  9 20:27:56 2023, max compression
```

## Comparing `RegionProposalGenerator-2.0.8.tar` & `RegionProposalGenerator-2.1.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2022-04-17 01:01:48.513008 RegionProposalGenerator-2.0.8/
-drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2022-04-17 01:01:48.509008 RegionProposalGenerator-2.0.8/ExamplesObjectDetection/
--rw-r--r--   0 kak       (1000) avi       (1000)      998 2022-04-17 00:25:57.000000 RegionProposalGenerator-2.0.8/ExamplesObjectDetection/README
--rwxr-xr-x   0 kak       (1000) avi       (1000)     2517 2022-04-17 00:16:45.000000 RegionProposalGenerator-2.0.8/ExamplesObjectDetection/multi_instance_object_detection.py
--rwxr-xr-x   0 kak       (1000) avi       (1000)     3152 2022-04-17 00:20:52.000000 RegionProposalGenerator-2.0.8/ExamplesObjectDetection/single_instance_object_detection.py
-drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2022-04-17 01:01:48.509008 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/
--rw-rw-r--   0 kak       (1000) avi       (1000)      546 2022-04-06 21:31:11.000000 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/README
-drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2022-04-17 01:01:48.509008 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/color_blobs/
--rwxr-x---   0 kak       (1000) avi       (1000)     7981 2019-12-28 00:05:11.000000 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/color_blobs/color_blobs.jpg
--rwxr-xr-x   0 kak       (1000) avi       (1000)     1418 2020-01-02 01:06:32.000000 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/color_blobs/selective_search.py
-drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2022-04-17 01:01:48.513008 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/images/
--rw-rw-r--   0 kak       (1000) avi       (1000)     1101 2019-12-23 11:04:18.000000 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/images/disk.jpg
--rw-r-----   0 kak       (1000) avi       (1000)    99726 2016-06-21 02:56:03.000000 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/images/london6.jpg
--rw-rw-r--   0 kak       (1000) avi       (1000)     4319 2019-12-28 09:05:55.000000 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/images/mondrian.jpg
--rw-rw-r--   0 kak       (1000) avi       (1000)    36621 2019-12-21 14:29:38.000000 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/images/polkadots.jpg
--rw-r-----   0 kak       (1000) avi       (1000)      362 2016-06-04 22:38:36.000000 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/images/rect_with_4_colors.jpg
--rw-r--r--   0 kak       (1000) avi       (1000)    17102 2014-10-21 03:43:39.000000 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/images/tulip0036.jpg
--rw-rw-r--   0 kak       (1000) avi       (1000)    57150 2019-12-20 05:11:12.000000 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/images/wallpic2.jpg
--rwxrwxr-x   0 kak       (1000) avi       (1000)     1557 2020-01-02 03:40:36.000000 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/interactive_graph_based_segmentation.py
-drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2022-04-17 01:01:48.513008 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/mondrian/
--rw-r--r--   0 kak       (1000) avi       (1000)     1240 2020-01-01 19:26:22.000000 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/mondrian/README
--rw-r--r--   0 kak       (1000) avi       (1000)     4319 2019-12-28 16:40:19.000000 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/mondrian/mondrian.jpg
--rwxr-xr-x   0 kak       (1000) avi       (1000)     1407 2020-01-02 00:33:54.000000 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/mondrian/selective_search.py
--rwxr-xr-x   0 kak       (1000) avi       (1000)     1416 2020-01-02 00:54:17.000000 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/selective_search.py
--rwxr-xr-x   0 kak       (1000) avi       (1000)      657 2019-12-30 10:21:36.000000 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/torchvision_based_image_processing.py
--rwxr-xr-x   0 kak       (1000) avi       (1000)      368 2020-01-27 23:44:30.000000 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/torchvision_some_basic_transformations.py
-drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2022-04-17 01:01:48.513008 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/wallpic2/
--rwxr-xr-x   0 kak       (1000) avi       (1000)     1412 2020-01-02 00:53:43.000000 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/wallpic2/selective_search.py
--rw-r--r--   0 kak       (1000) avi       (1000)    16188 2020-01-01 20:20:23.000000 RegionProposalGenerator-2.0.8/ExamplesRegionProposals/wallpic2/wallpic2.jpg
--rw-r--r--   0 kak       (1000) avi       (1000)     1763 2022-04-17 00:27:33.000000 RegionProposalGenerator-2.0.8/MANIFEST.in
--rw-r--r--   0 kak       (1000) avi       (1000)     1236 2021-05-17 18:59:52.000000 RegionProposalGenerator-2.0.8/Makefile
--rw-r--r--   0 kak       (1000) avi       (1000)     4602 2022-04-17 01:01:48.513008 RegionProposalGenerator-2.0.8/PKG-INFO
--rw-r--r--   0 kak       (1000) avi       (1000)     1158 2021-03-31 18:49:34.000000 RegionProposalGenerator-2.0.8/README
-drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2022-04-17 01:01:48.513008 RegionProposalGenerator-2.0.8/RegionProposalGenerator/
--rwxr-xr-x   0 kak       (1000) avi       (1000)   302090 2022-04-17 00:35:50.000000 RegionProposalGenerator-2.0.8/RegionProposalGenerator/RegionProposalGenerator.py
--rw-rw-r--   0 kak       (1000) avi       (1000)      855 2022-03-21 16:17:38.000000 RegionProposalGenerator-2.0.8/RegionProposalGenerator/__init__.py
--rw-r--r--   0 kak       (1000) avi       (1000)   129011 2022-04-17 00:58:21.000000 RegionProposalGenerator-2.0.8/RegionProposalGenerator-2.0.8.html
-drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2022-04-17 01:01:48.513008 RegionProposalGenerator-2.0.8/RegionProposalGenerator.egg-info/
--rw-r--r--   0 kak       (1000) avi       (1000)     4602 2022-04-17 01:01:48.000000 RegionProposalGenerator-2.0.8/RegionProposalGenerator.egg-info/PKG-INFO
--rw-r--r--   0 kak       (1000) avi       (1000)     1671 2022-04-17 01:01:48.000000 RegionProposalGenerator-2.0.8/RegionProposalGenerator.egg-info/SOURCES.txt
--rw-r--r--   0 kak       (1000) avi       (1000)        1 2022-04-17 01:01:48.000000 RegionProposalGenerator-2.0.8/RegionProposalGenerator.egg-info/dependency_links.txt
--rw-r--r--   0 kak       (1000) avi       (1000)       24 2022-04-17 01:01:48.000000 RegionProposalGenerator-2.0.8/RegionProposalGenerator.egg-info/top_level.txt
-drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2022-04-17 01:01:48.513008 RegionProposalGenerator-2.0.8/TestRegionProposalGenerator/
--rwxr-xr-x   0 kak       (1000) avi       (1000)   302090 2022-04-17 00:40:57.000000 RegionProposalGenerator-2.0.8/TestRegionProposalGenerator/RegionProposalGenerator.py
--rwxr-xr-x   0 kak       (1000) avi       (1000)      717 2020-01-02 01:42:01.000000 RegionProposalGenerator-2.0.8/TestRegionProposalGenerator/Test.py
--rw-r--r--   0 kak       (1000) avi       (1000)      819 2020-01-02 03:03:37.000000 RegionProposalGenerator-2.0.8/TestRegionProposalGenerator/TestImageConversion.py
--rw-r--r--   0 kak       (1000) avi       (1000)     1015 2020-11-30 19:29:54.000000 RegionProposalGenerator-2.0.8/TestRegionProposalGenerator/TestImageLoadingAndDataExtraction.py
--rw-r--r--   0 kak       (1000) avi       (1000)     1408 2020-01-02 01:50:03.000000 RegionProposalGenerator-2.0.8/TestRegionProposalGenerator/halfsun.jpg
--rw-r--r--   0 kak       (1000) avi       (1000)       38 2022-04-17 01:01:48.513008 RegionProposalGenerator-2.0.8/setup.cfg
--rwxr-xr-x   0 kak       (1000) avi       (1000)     4303 2022-04-10 15:05:07.000000 RegionProposalGenerator-2.0.8/setup.py
+drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2023-04-09 20:27:56.439665 RegionProposalGenerator-2.1.0/
+drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2023-04-09 20:27:56.439665 RegionProposalGenerator-2.1.0/ExamplesObjectDetection/
+-rw-r--r--   0 kak       (1000) avi       (1000)      998 2022-04-17 00:25:57.000000 RegionProposalGenerator-2.1.0/ExamplesObjectDetection/README
+-rwxr-xr-x   0 kak       (1000) avi       (1000)     2425 2023-04-09 20:04:03.000000 RegionProposalGenerator-2.1.0/ExamplesObjectDetection/multi_instance_object_detection.py
+-rwxr-xr-x   0 kak       (1000) avi       (1000)     3152 2022-04-17 00:20:52.000000 RegionProposalGenerator-2.1.0/ExamplesObjectDetection/single_instance_object_detection.py
+drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2023-04-09 20:27:56.439665 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/
+-rw-rw-r--   0 kak       (1000) avi       (1000)      546 2022-04-06 21:31:11.000000 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/README
+drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2023-04-09 20:27:56.439665 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/color_blobs/
+-rwxr-x---   0 kak       (1000) avi       (1000)     7981 2019-12-28 00:05:11.000000 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/color_blobs/color_blobs.jpg
+-rwxr-xr-x   0 kak       (1000) avi       (1000)     1418 2020-01-02 01:06:32.000000 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/color_blobs/selective_search.py
+drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2023-04-09 20:27:56.439665 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/images/
+-rw-rw-r--   0 kak       (1000) avi       (1000)     1101 2019-12-23 11:04:18.000000 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/images/disk.jpg
+-rw-r-----   0 kak       (1000) avi       (1000)    99726 2016-06-21 02:56:03.000000 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/images/london6.jpg
+-rw-rw-r--   0 kak       (1000) avi       (1000)     4319 2019-12-28 09:05:55.000000 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/images/mondrian.jpg
+-rw-rw-r--   0 kak       (1000) avi       (1000)    36621 2019-12-21 14:29:38.000000 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/images/polkadots.jpg
+-rw-r-----   0 kak       (1000) avi       (1000)      362 2016-06-04 22:38:36.000000 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/images/rect_with_4_colors.jpg
+-rw-r--r--   0 kak       (1000) avi       (1000)    17102 2014-10-21 03:43:39.000000 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/images/tulip0036.jpg
+-rw-rw-r--   0 kak       (1000) avi       (1000)    57150 2019-12-20 05:11:12.000000 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/images/wallpic2.jpg
+-rwxrwxr-x   0 kak       (1000) avi       (1000)     1557 2020-01-02 03:40:36.000000 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/interactive_graph_based_segmentation.py
+drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2023-04-09 20:27:56.439665 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/mondrian/
+-rw-r--r--   0 kak       (1000) avi       (1000)     1240 2020-01-01 19:26:22.000000 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/mondrian/README
+-rw-r--r--   0 kak       (1000) avi       (1000)     4319 2019-12-28 16:40:19.000000 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/mondrian/mondrian.jpg
+-rwxr-xr-x   0 kak       (1000) avi       (1000)     1407 2020-01-02 00:33:54.000000 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/mondrian/selective_search.py
+-rwxr-xr-x   0 kak       (1000) avi       (1000)     1416 2020-01-02 00:54:17.000000 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/selective_search.py
+-rwxr-xr-x   0 kak       (1000) avi       (1000)      657 2019-12-30 10:21:36.000000 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/torchvision_based_image_processing.py
+-rwxr-xr-x   0 kak       (1000) avi       (1000)      368 2020-01-27 23:44:30.000000 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/torchvision_some_basic_transformations.py
+drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2023-04-09 20:27:56.439665 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/wallpic2/
+-rwxr-xr-x   0 kak       (1000) avi       (1000)     1412 2020-01-02 00:53:43.000000 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/wallpic2/selective_search.py
+-rw-r--r--   0 kak       (1000) avi       (1000)    16188 2020-01-01 20:20:23.000000 RegionProposalGenerator-2.1.0/ExamplesRegionProposals/wallpic2/wallpic2.jpg
+-rw-r--r--   0 kak       (1000) avi       (1000)     1763 2023-04-07 14:28:24.000000 RegionProposalGenerator-2.1.0/MANIFEST.in
+-rw-r--r--   0 kak       (1000) avi       (1000)     1236 2021-05-17 18:59:52.000000 RegionProposalGenerator-2.1.0/Makefile
+-rw-r--r--   0 kak       (1000) avi       (1000)     4601 2023-04-09 20:27:56.439665 RegionProposalGenerator-2.1.0/PKG-INFO
+-rw-r--r--   0 kak       (1000) avi       (1000)     1158 2021-03-31 18:49:34.000000 RegionProposalGenerator-2.1.0/README
+drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2023-04-09 20:27:56.439665 RegionProposalGenerator-2.1.0/RegionProposalGenerator/
+-rwxr-xr-x   0 kak       (1000) avi       (1000)   305505 2023-04-09 19:58:08.000000 RegionProposalGenerator-2.1.0/RegionProposalGenerator/RegionProposalGenerator.py
+-rw-rw-r--   0 kak       (1000) avi       (1000)      855 2022-03-21 16:17:38.000000 RegionProposalGenerator-2.1.0/RegionProposalGenerator/__init__.py
+-rw-r--r--   0 kak       (1000) avi       (1000)   129316 2023-04-09 20:23:01.000000 RegionProposalGenerator-2.1.0/RegionProposalGenerator-2.1.0.html
+drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2023-04-09 20:27:56.439665 RegionProposalGenerator-2.1.0/RegionProposalGenerator.egg-info/
+-rw-r--r--   0 kak       (1000) avi       (1000)     4601 2023-04-09 20:27:56.000000 RegionProposalGenerator-2.1.0/RegionProposalGenerator.egg-info/PKG-INFO
+-rw-r--r--   0 kak       (1000) avi       (1000)     1671 2023-04-09 20:27:56.000000 RegionProposalGenerator-2.1.0/RegionProposalGenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 kak       (1000) avi       (1000)        1 2023-04-09 20:27:56.000000 RegionProposalGenerator-2.1.0/RegionProposalGenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 kak       (1000) avi       (1000)       24 2023-04-09 20:27:56.000000 RegionProposalGenerator-2.1.0/RegionProposalGenerator.egg-info/top_level.txt
+drwxr-xr-x   0 kak       (1000) avi       (1000)        0 2023-04-09 20:27:56.439665 RegionProposalGenerator-2.1.0/TestRegionProposalGenerator/
+-rwxr-xr-x   0 kak       (1000) avi       (1000)   305505 2023-04-09 20:06:52.000000 RegionProposalGenerator-2.1.0/TestRegionProposalGenerator/RegionProposalGenerator.py
+-rwxr-xr-x   0 kak       (1000) avi       (1000)      717 2020-01-02 01:42:01.000000 RegionProposalGenerator-2.1.0/TestRegionProposalGenerator/Test.py
+-rw-r--r--   0 kak       (1000) avi       (1000)      819 2020-01-02 03:03:37.000000 RegionProposalGenerator-2.1.0/TestRegionProposalGenerator/TestImageConversion.py
+-rw-r--r--   0 kak       (1000) avi       (1000)     1015 2020-11-30 19:29:54.000000 RegionProposalGenerator-2.1.0/TestRegionProposalGenerator/TestImageLoadingAndDataExtraction.py
+-rw-r--r--   0 kak       (1000) avi       (1000)     1408 2020-01-02 01:50:03.000000 RegionProposalGenerator-2.1.0/TestRegionProposalGenerator/halfsun.jpg
+-rw-r--r--   0 kak       (1000) avi       (1000)       38 2023-04-09 20:27:56.439665 RegionProposalGenerator-2.1.0/setup.cfg
+-rwxr-xr-x   0 kak       (1000) avi       (1000)     4302 2023-04-07 14:27:55.000000 RegionProposalGenerator-2.1.0/setup.py
```

### Comparing `RegionProposalGenerator-2.0.8/ExamplesObjectDetection/README` & `RegionProposalGenerator-2.1.0/ExamplesObjectDetection/README`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/ExamplesObjectDetection/multi_instance_object_detection.py` & `RegionProposalGenerator-2.1.0/ExamplesObjectDetection/multi_instance_object_detection.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 #                  dataroot_test = "/home/kak/ImageDatasets/Purdue_Dr_Eval_multi_dataset_test_1000/",
                   image_size = [128,128],
                   yolo_interval = 20,
                   path_saved_yolo_model = "./saved_yolo_model",
                   momentum = 0.9,
                   learning_rate = 1e-5,
                   epochs = 20,
-                  batch_size = 1,
+                  batch_size = 4,
                   classes = ('Dr_Eval','house','watertower'),
                   use_gpu = True,
               )
 
 
 yolo = RegionProposalGenerator.YoloLikeDetector( rpg = rpg )
 
@@ -57,13 +57,12 @@
 model = yolo.NetForYolo(skip_connections=True, depth=8) 
 
 number_of_learnable_params = sum(p.numel() for p in model.parameters() if p.requires_grad)
 print("\n\nThe number of learnable parameters in the model: %d" % number_of_learnable_params)
 num_layers = len(list(model.parameters()))
 print("\n\nThe number of layers in the model: %d\n\n" % num_layers)
 
-#model = yolo.run_code_for_training_multi_instance_detection(model, display_labels=True, display_images=True)
 model = yolo.run_code_for_training_multi_instance_detection(model, display_labels=True, display_images=False)
 
-yolo.run_code_for_testing_multi_instance_detection(model, display_images = True)
+yolo.run_code_for_testing_multi_instance_detection(model, "figs_for_movie", display_images = True)
```

### Comparing `RegionProposalGenerator-2.0.8/ExamplesObjectDetection/single_instance_object_detection.py` & `RegionProposalGenerator-2.1.0/ExamplesObjectDetection/single_instance_object_detection.py`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/ExamplesRegionProposals/README` & `RegionProposalGenerator-2.1.0/ExamplesRegionProposals/README`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/ExamplesRegionProposals/color_blobs/color_blobs.jpg` & `RegionProposalGenerator-2.1.0/ExamplesRegionProposals/color_blobs/color_blobs.jpg`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/ExamplesRegionProposals/color_blobs/selective_search.py` & `RegionProposalGenerator-2.1.0/ExamplesRegionProposals/color_blobs/selective_search.py`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/ExamplesRegionProposals/images/disk.jpg` & `RegionProposalGenerator-2.1.0/ExamplesRegionProposals/images/disk.jpg`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/ExamplesRegionProposals/images/london6.jpg` & `RegionProposalGenerator-2.1.0/ExamplesRegionProposals/images/london6.jpg`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/ExamplesRegionProposals/images/mondrian.jpg` & `RegionProposalGenerator-2.1.0/ExamplesRegionProposals/images/mondrian.jpg`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/ExamplesRegionProposals/images/polkadots.jpg` & `RegionProposalGenerator-2.1.0/ExamplesRegionProposals/images/polkadots.jpg`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/ExamplesRegionProposals/images/tulip0036.jpg` & `RegionProposalGenerator-2.1.0/ExamplesRegionProposals/images/tulip0036.jpg`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/ExamplesRegionProposals/images/wallpic2.jpg` & `RegionProposalGenerator-2.1.0/ExamplesRegionProposals/images/wallpic2.jpg`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/ExamplesRegionProposals/interactive_graph_based_segmentation.py` & `RegionProposalGenerator-2.1.0/ExamplesRegionProposals/interactive_graph_based_segmentation.py`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/ExamplesRegionProposals/mondrian/README` & `RegionProposalGenerator-2.1.0/ExamplesRegionProposals/mondrian/README`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/ExamplesRegionProposals/mondrian/mondrian.jpg` & `RegionProposalGenerator-2.1.0/ExamplesRegionProposals/mondrian/mondrian.jpg`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/ExamplesRegionProposals/mondrian/selective_search.py` & `RegionProposalGenerator-2.1.0/ExamplesRegionProposals/mondrian/selective_search.py`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/ExamplesRegionProposals/selective_search.py` & `RegionProposalGenerator-2.1.0/ExamplesRegionProposals/selective_search.py`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/ExamplesRegionProposals/torchvision_based_image_processing.py` & `RegionProposalGenerator-2.1.0/ExamplesRegionProposals/torchvision_based_image_processing.py`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/ExamplesRegionProposals/wallpic2/selective_search.py` & `RegionProposalGenerator-2.1.0/ExamplesRegionProposals/wallpic2/selective_search.py`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/ExamplesRegionProposals/wallpic2/wallpic2.jpg` & `RegionProposalGenerator-2.1.0/ExamplesRegionProposals/wallpic2/wallpic2.jpg`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/MANIFEST.in` & `RegionProposalGenerator-2.1.0/MANIFEST.in`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 include MANIFEST.in
 include RegionProposalGenerator/RegionProposalGenerator.py
 include RegionProposalGenerator/__init__.py
 include setup.py
 include Makefile
 include README
-include RegionProposalGenerator-2.0.8.html
+include RegionProposalGenerator-2.1.0.html
 include TestRegionProposalGenerator/RegionProposalGenerator.py
 include TestRegionProposalGenerator/TestImageLoadingAndDataExtraction.py
 include TestRegionProposalGenerator/TestImageConversion.py
 include TestRegionProposalGenerator/Test.py
 include TestRegionProposalGenerator/halfsun.jpg
 include ExamplesObjectDetection/README
 include ExamplesObjectDetection/single_instance_object_detection.py
```

### Comparing `RegionProposalGenerator-2.0.8/Makefile` & `RegionProposalGenerator-2.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/PKG-INFO` & `RegionProposalGenerator-2.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,83 +1,91 @@
-Metadata-Version: 1.2
-Name: RegionProposalGenerator
-Version: 2.0.8
-Summary: An educational module for experimenting with single-instance and multi-instance object detection and for generating region proposals with graph-based algorithms
-Home-page: https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.0.8.html
-Author: Avinash Kak
-Author-email: kak@purdue.edu
-Maintainer: Avinash Kak
-Maintainer-email: kak@purdue.edu
-License: Python Software Foundation License
-Download-URL: https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.0.8.tar.gz
-Description: 
-        
-        Consult the module API page at
-        
-              https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.0.8.html
-        
-        for all information related to this module, including information related
-        to the latest changes to the code.  The page at the URL shown above lists
-        all of the module functionality you can invoke in your own code.
-        
-        ::
-        
-                Single-Instance and Multi-Instance Object Detection:
-            
-                    Say you wish to experiment with YOLO-like logic for multi-instance
-                    object detection, you would need to construct an instance of the
-                    RegionProposalGenerator class and invoke the methods shown below on
-                    this instance:
-                
-                    rpg = RegionProposalGenerator(
-                                      dataroot = "./data/",
-                                      image_size = [128,128],
-                                      yolo_interval = 20,
-                                      path_saved_yolo_model = "./saved_yolo_model",
-                                      momentum = 0.9,
-                                      learning_rate = 1e-6,
-                                      epochs = 40,
-                                      batch_size = 4,
-                                      classes = ('Dr_Eval','house','watertower'),
-                                      use_gpu = True,
-                                  )
-                    yolo = RegionProposalGenerator.YoloLikeDetector( rpg = rpg )
-                    yolo.set_dataloaders(train=True)
-                    yolo.set_dataloaders(test=True)
-                    model = yolo.NetForYolo(skip_connections=True, depth=8) 
-                    model = yolo.run_code_for_training_multi_instance_detection(model, display_images=False)
-                    yolo.run_code_for_training_multi_instance_detection(model, display_images = True)
-                    
-            
-                Graph-Based Algorithms for Region Proposals:
-            
-                    To generate region proposals, you would need to construct an instance
-                    of the RegionProposalGenerator class and invoke the methods shown below
-                    on this instance:
-                
-                    rpg = RegionProposalGenerator(
-                                   ###  The first 6 options affect only the graph-based part of the algo
-                                   sigma = 1.0,
-                                   max_iterations = 40,
-                                   kay = 0.05,
-                                   image_normalization_required = True,
-                                   image_size_reduction_factor = 4,
-                                   min_size_for_graph_based_blobs = 4,
-                                   ###  The next 4 options affect only the Selective Search part of the algo
-                                   color_homogeneity_thresh = [20,20,20],
-                                   gray_var_thresh = 16000,           
-                                   texture_homogeneity_thresh = 120,
-                                   max_num_blobs_expected = 8,
+#!/usr/bin/env python
+
+### setup.py
+
+from setuptools import setup, find_packages
+import sys, os
+
+setup(name='RegionProposalGenerator',
+      version='2.1.0',
+      author='Avinash Kak',
+      author_email='kak@purdue.edu',
+      maintainer='Avinash Kak',
+      maintainer_email='kak@purdue.edu',
+      url='https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.1.0.html',
+      download_url='https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.1.0.tar.gz',
+      description='An educational module for experimenting with the YOLO logic for multi-instance object detection and for generating region proposals with graph-based algorithms',
+      long_description='''
+
+Consult the module API page at
+
+      https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.1.0.html
+
+for all information related to this module, including information related
+to the latest changes to the code.  The page at the URL shown above lists
+all of the module functionality you can invoke in your own code.
+
+::
+
+        Single-Instance and Multi-Instance Object Detection:
+    
+            Say you wish to experiment with YOLO-like logic for multi-instance
+            object detection, you would need to construct an instance of the
+            RegionProposalGenerator class and invoke the methods shown below on
+            this instance:
+        
+            rpg = RegionProposalGenerator(
+                              dataroot = "./data/",
+                              image_size = [128,128],
+                              yolo_interval = 20,
+                              path_saved_yolo_model = "./saved_yolo_model",
+                              momentum = 0.9,
+                              learning_rate = 1e-6,
+                              epochs = 40,
+                              batch_size = 4,
+                              classes = ('Dr_Eval','house','watertower'),
+                              use_gpu = True,
                           )
-                    
-                    image_name = "images/mondrian.jpg"
-                    segmented_graph,color_map = rpg.graph_based_segmentation(image_name)
-                    rpg.visualize_segmentation_in_pseudocolor(segmented_graph[0], color_map, "graph_based" )
-                    merged_blobs, color_map = rpg.selective_search_for_region_proposals( segmented_graph, image_name )
-                    rpg.visualize_segmentation_with_mean_gray(merged_blobs, "ss_based_segmentation_in_bw" )
-        
+            yolo = RegionProposalGenerator.YoloLikeDetector( rpg = rpg )
+            yolo.set_dataloaders(train=True)
+            yolo.set_dataloaders(test=True)
+            model = yolo.NetForYolo(skip_connections=True, depth=8) 
+            model = yolo.run_code_for_training_multi_instance_detection(model, display_images=False)
+            yolo.run_code_for_training_multi_instance_detection(model, display_images = True)
+            
+    
+        Graph-Based Algorithms for Region Proposals:
+    
+            To generate region proposals, you would need to construct an instance
+            of the RegionProposalGenerator class and invoke the methods shown below
+            on this instance:
+        
+            rpg = RegionProposalGenerator(
+                           ###  The first 6 options affect only the graph-based part of the algo
+                           sigma = 1.0,
+                           max_iterations = 40,
+                           kay = 0.05,
+                           image_normalization_required = True,
+                           image_size_reduction_factor = 4,
+                           min_size_for_graph_based_blobs = 4,
+                           ###  The next 4 options affect only the Selective Search part of the algo
+                           color_homogeneity_thresh = [20,20,20],
+                           gray_var_thresh = 16000,           
+                           texture_homogeneity_thresh = 120,
+                           max_num_blobs_expected = 8,
+                  )
             
-                  
-Keywords: object detection,image segmentation,computer vision
-Platform: All platforms
-Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Classifier: Programming Language :: Python :: 3.8
+            image_name = "images/mondrian.jpg"
+            segmented_graph,color_map = rpg.graph_based_segmentation(image_name)
+            rpg.visualize_segmentation_in_pseudocolor(segmented_graph[0], color_map, "graph_based" )
+            merged_blobs, color_map = rpg.selective_search_for_region_proposals( segmented_graph, image_name )
+            rpg.visualize_segmentation_with_mean_gray(merged_blobs, "ss_based_segmentation_in_bw" )
+
+    
+          ''',
+
+      license='Python Software Foundation License',
+      keywords='object detection, image segmentation, computer vision',
+      platforms='All platforms',
+      classifiers=['Topic :: Scientific/Engineering :: Image Recognition', 'Programming Language :: Python :: 3.8'],
+      packages=['RegionProposalGenerator']
+)
```

### Comparing `RegionProposalGenerator-2.0.8/README` & `RegionProposalGenerator-2.1.0/README`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/RegionProposalGenerator/RegionProposalGenerator.py` & `RegionProposalGenerator-2.1.0/RegionProposalGenerator/RegionProposalGenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-__version__   = '2.0.8'
+# -*- coding: utf-8 -*-
+
+__version__   = '2.1.0'
 __author__    = "Avinash Kak (kak@purdue.edu)"
-__date__      = '2022-April-16'   
-__url__       = 'https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.0.8.html'
-__copyright__ = "(C) 2022 Avinash Kak. Python Software Foundation."
+__date__      = '2023-April-9'   
+__url__       = 'https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.1.0.html'
+__copyright__ = "(C) 2023 Avinash Kak. Python Software Foundation."
 
 
 __doc__ = '''
 
 RegionProposalGenerator.py
 
 Version: ''' + __version__ + '''
@@ -15,228 +17,227 @@
 
 Date: ''' + __date__ + '''
 
 
 @title
 CHANGE LOG:
 
+  Version 2.1.0:
+
+    With this version, you can now use batches of any size for YOLO learning.
+    Previously, the batch size was limited to 1 for the YOLO part of the module.
+    Allowing for batches required changes in the handling of problem images, such
+    as the images with no meaningful objects, or the images with object bounding
+    boxes with unrealistic aspect ratios.
+
   Version 2.0.8:
 
-    This version constitutes a complete implementation of a YOLO
-    multi-instance object detector.  In addition to the new multi-loss
-    function that I introduced in the previous public release of this module,
-    the new version includes a full-blown implementation of what you need for
-    validation testing.  I should also mention that I have split what used to
-    be the Examples directory in the distribution into two directories:
-    ExamplesObjectDetection and ExamplesRegionProposals.  Your entry point for
-    learning the YOLO implementation would be the script
-    multi_instance_object_detection.py in the directory
-    ExamplesObjectDetection.
+    This version constitutes a complete implementation of a YOLO multi-instance
+    object detector.  In addition to the new multi-loss function that I introduced
+    in the previous public release of this module, the new version includes a
+    full-blown implementation of what you need for validation testing.  I should
+    also mention that I have split what used to be the Examples directory in the
+    distribution into two directories: ExamplesObjectDetection and
+    ExamplesRegionProposals.  Your entry point for learning the YOLO
+    implementation would be the script multi_instance_object_detection.py in the
+    directory ExamplesObjectDetection.
     
   Version 2.0.6:
 
-    This version incorporates a more sophisticated loss function for
-    YOLO-based multi-instance object detection in images.  In the new loss
-    function, I use different criteria for the different segments of the YOLO
-    vector.  [Assigning an object instance in a training image to an anchor
-    box for a cell in the image involves creating a "5+C"-element YOLO vector,
-    where C is the number of object classes.] I now use the Binary
-    Cross-Entropy Loss (nn.BCELoss) for the first element of the YOLO vector
-    that stands for the presence or the absence of an object instance in a
-    specific anchor box in a specific cell.  I use mean-squared-error loss
-    (nn.MSELoss) for the next four numerical elements that express the precise
-    location of the object bounding-box vis-a-vis the center of the cell to
-    which the object is assigned and also for the dimensions of the bounding
-    box.  Finally, I use the regular Cross-Entropy loss (nn.CrossEntropyLoss)
-    for the last C elements of the YOLO vector.  Using the cross-entropy loss
-    for the labeling errors required augmenting the YOLO vector with one
-    additional element to express the absence of an object.
+    This version incorporates a more sophisticated loss function for YOLO-based
+    multi-instance object detection in images.  In the new loss function, I use
+    different criteria for the different segments of the YOLO vector.  [Assigning
+    an object instance in a training image to an anchor box for a cell in the
+    image involves creating a "5+C"-element YOLO vector, where C is the number of
+    object classes.] I now use the Binary Cross-Entropy Loss (nn.BCELoss) for the
+    first element of the YOLO vector that stands for the presence or the absence
+    of an object instance in a specific anchor box in a specific cell.  I use
+    mean-squared-error loss (nn.MSELoss) for the next four numerical elements that
+    express the precise location of the object bounding-box vis-a-vis the center
+    of the cell to which the object is assigned and also for the dimensions of the
+    bounding box.  Finally, I use the regular Cross-Entropy loss
+    (nn.CrossEntropyLoss) for the last C elements of the YOLO vector.  Using the
+    cross-entropy loss for the labeling errors required augmenting the YOLO vector
+    with one additional element to express the absence of an object.
 
   Version 2.0.2:
 
-    This version fixes a couple of bugs in the YOLO-based logic for
-    multi-instance object detection.
+    This version fixes a couple of bugs in the YOLO-based logic for multi-instance
+    object detection.
 
   Version 2.0.1:
 
     This module has gone through several changes since its last public-release
     version as I was experimenting with different ways of imparting to the
     students the sudden increase in model complexity as one goes from
-    single-instance object detection to multi-instance object detection.
-    These experiments led to the creation of two new datasets,
-    PurdueDrEvalDataset and PurdueDrEvalMultiDataset, the former for playing
-    with single-instance object detection and the latter for doing the same
-    with multi-instance object detection.  The module also includes two inner
-    classes, SingleInstanceDetector and YoloLikeDetector, the former a
-    reference implementation for single instance object detection and the
-    latter a YOLO-like reference implementation for multi-instance object
-    detection. [By the way, "DrEval" in the names of the two datasets
-    mentioned here has a connection with "Dr Evil" in the Austin Powers
-    movies.]
+    single-instance object detection to multi-instance object detection.  These
+    experiments led to the creation of two new datasets, PurdueDrEvalDataset and
+    PurdueDrEvalMultiDataset, the former for playing with single-instance object
+    detection and the latter for doing the same with multi-instance object
+    detection.  The module also includes two inner classes, SingleInstanceDetector
+    and YoloLikeDetector, the former a reference implementation for single
+    instance object detection and the latter a YOLO-like reference implementation
+    for multi-instance object detection. [By the way, "DrEval" in the names of the
+    two datasets mentioned here has a connection with "Dr Evil" in the Austin
+    Powers movies.]
 
   Version 1.0.5:
 
     In keeping with the tutorial nature of this module, this version includes
-    methods that come in handy for batch-based processing of images. These
-    methods carry names like "displaying_and_histogramming_
-    images_in_batchX()" where X is 1, 2, and 3.  The rest of the module,
-    especially the part that deals with constructing region proposals remains
-    unchanged.
+    methods that come in handy for batch-based processing of images. These methods
+    carry names like "displaying_and_histogramming_ images_in_batchX()" where X is
+    1, 2, and 3.  The rest of the module, especially the part that deals with
+    constructing region proposals remains unchanged.
 
   Version 1.0.4:
 
     This is the first public release version of the module.
 
 
 @title
 INTRODUCTION:
 
     Single-Instance vs. Multi-Instance Detection:
 
-    This module was created for experimenting with the logic of object
-    detection with neural networks.  On the face of it, object detection in
-    images sounds like a well-defined problem that should lend itself to
-    well-defined solutions.  Unfortunately, the reality is otherwise.  Yes,
-    simple examples of the problem -- such as when the images contain
-    single object instances and with no competing clutter in the background
-    -- the problem can be solved straightforwardly with a neural network.
-    However, the object detection problems that are encountered in real
-    life are rarely that simple.  A practically useful framework for object
-    detection must be able to recognize and localize all possible instances
-    of the objects of interest in a given image.
+    This module was created for experimenting with the logic of object detection
+    with neural networks.  On the face of it, object detection in images sounds
+    like a well-defined problem that should lend itself to well-defined solutions.
+    Unfortunately, the reality is otherwise.  Yes, simple examples of the problem
+    -- such as when the images contain single object instances and with no
+    competing clutter in the background -- the problem can be solved
+    straightforwardly with a neural network.  However, the object detection
+    problems that are encountered in real life are rarely that simple.  A
+    practically useful framework for object detection must be able to recognize
+    and localize all possible instances of the objects of interest in a given
+    image.
 
     So how does one solve the problem of multi-instance object detection and
     localization with a neural network?
 
     The last half-dozen years have seen the emergence of the following three
-    competition-grade neural-network based approaches for multi-instance
-    object detection: R-CNN, YOLO, and SSD.  The Preamble section of my Week 8
-    lecture for Purdue's Deep Learning class provides a brief overview of
-    these approaches.  YOLO stands for "You Only Look Once" --- in contrast
-    with R-CNN based approaches in which you may have to subject the images to
-    a couple of neural networks, one for generating region proposals and the
-    other for actual object detection.
-
-    The main goal of the present module is to provide an educational example
-    of a complete implementation of the YOLO logic for multi-instance object
-    detection in images.
+    competition-grade neural-network based approaches for multi-instance object
+    detection: R-CNN, YOLO, and SSD.  The Preamble section of my Week 8 lecture
+    for Purdue's Deep Learning class provides a brief overview of these
+    approaches.  YOLO stands for "You Only Look Once" --- in contrast with R-CNN
+    based approaches in which you may have to subject the images to a couple of
+    neural networks, one for generating region proposals and the other for actual
+    object detection.
+
+    The main goal of the present module is to provide an educational example of a
+    complete implementation of the YOLO logic for multi-instance object detection
+    in images.
 
     Graph-Based Algorithms for Region Proposals:
 
-    A second goal of this module is to provide implementations for a couple
-    of the more modern graph-based approaches for generating region
-    proposals.  At this point, the reader might ask: What is a region
-    proposal?  A region proposal is a blob of pixels that is highly likely
-    to contain an object instance.  Another way of saying same thing is
-    that region proposals are pixel blobs that look different from the
-    general background in the images.  While it is possible to use a neural
-    network for generating region proposals, as demonstrated by the success
-    of RPN (Region Proposal Network) in the R-CNN based multi-instance
+    A second goal of this module is to provide implementations for a couple of the
+    more modern graph-based approaches for generating region proposals.  At this
+    point, the reader might ask: What is a region proposal?  A region proposal is
+    a blob of pixels that is highly likely to contain an object instance.  Another
+    way of saying same thing is that region proposals are pixel blobs that look
+    different from the general background in the images.  While it is possible to
+    use a neural network for generating region proposals, as demonstrated by the
+    success of RPN (Region Proposal Network) in the R-CNN based multi-instance
     object detection, the RPG module is concerned primarily with the
-    non-neural-network based methods -- the graph-based methods -- for
-    generating region proposals.  I believe that becoming familiar with the
-    non-learning based methods for constructing region proposals still has
-    considerable value.  Consider, for example, the problem of detecting
-    objects in satellite images where you simply do not have access to the
-    amount of training data you would need for a neural-network based
-    approach to work.
-
-    With regard to the graph-based method for generating region proposals,
-    RPG (RegionProposalGenerator) implements elements of the Selective
-    Search (SS) algorithm for object detection as proposed by Uijlings, van
-    de Sande, Gevers, and Smeulders.  The Selective Search algorithm sits
-    on top of the graph-based image segmentation algorithm of Felzenszwalb
-    and Huttenlocher (FH) whose implementation is also included in the RPG
-    module.  The RPG module first processes an image with the FH
-    graph-based algorithm for image segmentation to divide an image into
-    pixel blobs.  The module subsequently invokes elements of the SS
-    algorithm to selectively merge the blobs on the basis of three
+    non-neural-network based methods -- the graph-based methods -- for generating
+    region proposals.  I believe that becoming familiar with the non-learning
+    based methods for constructing region proposals still has considerable value.
+    Consider, for example, the problem of detecting objects in satellite images
+    where you simply do not have access to the amount of training data you would
+    need for a neural-network based approach to work.
+
+    With regard to the graph-based method for generating region proposals, RPG
+    (RegionProposalGenerator) implements elements of the Selective Search (SS)
+    algorithm for object detection as proposed by Uijlings, van de Sande, Gevers,
+    and Smeulders.  The Selective Search algorithm sits on top of the graph-based
+    image segmentation algorithm of Felzenszwalb and Huttenlocher (FH) whose
+    implementation is also included in the RPG module.  The RPG module first
+    processes an image with the FH graph-based algorithm for image segmentation to
+    divide an image into pixel blobs.  The module subsequently invokes elements of
+    the SS algorithm to selectively merge the blobs on the basis of three
     properties: homogeneity of the color, grayscale variance, and texture
     homogeneity.
 
-    The FH algorithm is based on creating a graph-based representation of
-    an image in which, at the beginning, each pixel is a single vertex and
-    the edge between two vertices that stand for two adjacent pixels
-    represents the difference between some pixel property (such as the
-    color difference) at the two pixels.  Subsequently, for the vertex
-    merging logic, each vertex u, that after the first iteration stands for
-    a grouping of pixels, is characterized by a property called Int(u),
-    which is the largest value of the inter-pixel color difference between
-    the adjacent pixels.  In order to account for the fact that, at the
-    beginning, each vertex consists of only one pixel [which would not
-    allow for the calculation of Int(u)], the unary property of the pixels
-    at a vertex is extended from Int(u) to MInt(u) with the addition of a
-    vertex-size dependent number equal to k/|C| where "k" is a
-    user-specified parameter and |C| the cardinality of the set of pixels
-    represented by the vertex u in the graph.
-
-    As mentioned above, initially the edges in the graph representation of
-    an image are set to the color difference between the two 8-adjacent
-    pixels that correspond to two different vertices.  Subsequently, as the
-    vertices are merged, an edge, E(u,v), between two vertices u and v is
-    set to the smallest value of the inter-pixel color difference for two
-    adjacent pixels that belong to the two vertices. At each iteration of
-    the algorithm, two vertices u and v are merged provided E(u,v) is less
-    than the smaller of the MInt(u) or MInt(v) attributes at the two
-    vertices.  My experience is that for most images the algorithm
-    terminates of its own accord after a small number of iterations while
-    the vertex merging condition can be satisfied.
-
-    Since the algorithm is driven by the color differences between
-    8-adjacent pixels, the FH algorithm is likely to create too fine a
-    segmentation of an image.  The segments produced by FH can be made
-    larger by using the logic of SS that allows blobs of pixels to merge
-    into larger blobs provided doing so makes sense based on the inter-blob
-    values for mean color levels, color variances, texture values, etc.
+    The FH algorithm is based on creating a graph-based representation of an image
+    in which, at the beginning, each pixel is a single vertex and the edge between
+    two vertices that stand for two adjacent pixels represents the difference
+    between some pixel property (such as the color difference) at the two pixels.
+    Subsequently, for the vertex merging logic, each vertex u, that after the
+    first iteration stands for a grouping of pixels, is characterized by a
+    property called Int(u), which is the largest value of the inter-pixel color
+    difference between the adjacent pixels.  In order to account for the fact
+    that, at the beginning, each vertex consists of only one pixel [which would
+    not allow for the calculation of Int(u)], the unary property of the pixels at
+    a vertex is extended from Int(u) to MInt(u) with the addition of a vertex-size
+    dependent number equal to k/|C| where "k" is a user-specified parameter and
+    |C| the cardinality of the set of pixels represented by the vertex u in the
+    graph.
+
+    As mentioned above, initially the edges in the graph representation of an
+    image are set to the color difference between the two 8-adjacent pixels that
+    correspond to two different vertices.  Subsequently, as the vertices are
+    merged, an edge, E(u,v), between two vertices u and v is set to the smallest
+    value of the inter-pixel color difference for two adjacent pixels that belong
+    to the two vertices. At each iteration of the algorithm, two vertices u and v
+    are merged provided E(u,v) is less than the smaller of the MInt(u) or MInt(v)
+    attributes at the two vertices.  My experience is that for most images the
+    algorithm terminates of its own accord after a small number of iterations
+    while the vertex merging condition can be satisfied.
+
+    Since the algorithm is driven by the color differences between 8-adjacent
+    pixels, the FH algorithm is likely to create too fine a segmentation of an
+    image.  The segments produced by FH can be made larger by using the logic of
+    SS that allows blobs of pixels to merge into larger blobs provided doing so
+    makes sense based on the inter-blob values for mean color levels, color
+    variances, texture values, etc.
 
 
 @title
 INSTALLATION:
 
     The RegionProposalGenerator class was packaged using setuptools.  For
-    installation, execute the following command in the source directory
-    (this is the directory that contains the setup.py file after you have
-    downloaded and uncompressed the package):
+    installation, execute the following command in the source directory (this is
+    the directory that contains the setup.py file after you have downloaded and
+    uncompressed the package):
  
             sudo python3 setup.py install
 
-    On Linux distributions, this will install the module file at a location
-    that looks like
+    On Linux distributions, this will install the module file at a location that
+    looks like
 
              /usr/local/lib/python3.8/dist-packages/
 
-    If you do not have root access, you have the option of working directly
-    off the directory in which you downloaded the software by simply
-    placing the following statements at the top of your scripts that use
-    the RegionProposalGenerator class:
+    If you do not have root access, you have the option of working directly off
+    the directory in which you downloaded the software by simply placing the
+    following statements at the top of your scripts that use the
+    RegionProposalGenerator class:
 
             import sys
             sys.path.append( "pathname_to_RegionProposalGenerator_directory" )
 
-    To uninstall the module, simply delete the source directory, locate
-    where the RegionProposalGenerator module was installed with "locate
-    RegionProposalGenerator" and delete those files.  As mentioned above,
-    the full pathname to the installed version is likely to look like
+    To uninstall the module, simply delete the source directory, locate where the
+    RegionProposalGenerator module was installed with "locate
+    RegionProposalGenerator" and delete those files.  As mentioned above, the full
+    pathname to the installed version is likely to look like
     /usr/local/lib/python2.7/dist-packages/RegionProposalGenerator*
 
-    If you want to carry out a non-standard install of the
-    RegionProposalGenerator module, look up the on-line information on
-    Disutils by pointing your browser to
+    If you want to carry out a non-standard install of the RegionProposalGenerator
+    module, look up the on-line information on Disutils by pointing your browser
+    to
 
               http://docs.python.org/dist/dist.html
 
 @title
 USAGE:
 
     Single-Instance and Multi-Instance Detection:
 
-    If you wish to experiment with YOLO-like logic for multi-instance
-    object detection, you would need to construct an instance of the
-    RegionProposalGenerator class and invoke the methods shown below on
-    this instance:
+    If you wish to experiment with YOLO-like logic for multi-instance object
+    detection, you would need to construct an instance of the
+    RegionProposalGenerator class and invoke the methods shown below on this
+    instance:
 
     rpg = RegionProposalGenerator(
                       dataroot = "./data/",
                       image_size = [128,128],
                       yolo_interval = 20,
                       path_saved_yolo_model = "./saved_yolo_model",
                       momentum = 0.9,
@@ -252,17 +253,17 @@
     model = yolo.NetForYolo(skip_connections=True, depth=8) 
     model = yolo.run_code_for_training_multi_instance_detection(model, display_images=False)
     yolo.run_code_for_training_multi_instance_detection(model, display_images = True)
     
 
     Graph-Based Algorithms for Region Proposals:
 
-    To generate region proposals, you would need to construct an instance
-    of the RegionProposalGenerator class and invoke the methods shown below
-    on this instance:
+    To generate region proposals, you would need to construct an instance of the
+    RegionProposalGenerator class and invoke the methods shown below on this
+    instance:
 
         rpg = RegionProposalGenerator(
                        ###  The first 6 options affect only the Graph-Based part of the algo
                        sigma = 1.0,
                        max_iterations = 40,
                        kay = 0.05,
                        image_normalization_required = True,
@@ -280,352 +281,344 @@
         merged_blobs, color_map = rpg.selective_search_for_region_proposals( segmented_graph, image_name )
         rpg.visualize_segmentation_with_mean_gray(merged_blobs, "ss_based_segmentation_in_bw" )
 
 
 @title
 CONSTRUCTOR PARAMETERS: 
 
-    Of the 10 constructor parameters listed below, the first six are meant for
-    the FH algorithm and the last four for the SS algorithm.
+    Of the 10 constructor parameters listed below, the first six are meant for the
+    FH algorithm and the last four for the SS algorithm.
 
-    sigma: Controls the size of the Gaussian kernel used for smoothing the
-                    image before its gradient is calculated.  Assuming the
-                    pixel sampling interval to be unity, a sigma of 1 gives
-                    you a 7x7 smoothing operator with Gaussian weighting.
-                    The default for this parameter is 1.
+    sigma: Controls the size of the Gaussian kernel used for smoothing the image
+                    before its gradient is calculated.  Assuming the pixel
+                    sampling interval to be unity, a sigma of 1 gives you a 7x7
+                    smoothing operator with Gaussian weighting.  The default for
+                    this parameter is 1.
 
     max_iterations: Sets an upper limit on the number of iterations of the
                     graph-based FH algorithm for image segmentation.
 
-    kay: This is the same as the "k" parameter in the FH algorithm.  As
-                    mentioned in the Introduction above, the Int(u)
-                    property of the pixels represented by each vertex in
-                    the graph representation of the image is extended to
-                    MInt(u) by the addition of a number k/|C| where |C| is
-                    the cardinality of the set of pixels at that vertex.
-
-    image_normalization_required: This applies Torchvision's image
-                    normalization to the pixel values in the image.
-
-    image_size_reduction_factor: As mentioned at the beginning of this
-                    document, RegionProposalGenerator is really not meant
-                    for production work.  The code is pure Python and, even
-                    with that, not at all optimized.  The focus of the
-                    module is primarily on easy understandability of what
-                    the code is doing so that you can experiment with the
-                    algorithm itself.  For the module to produce results
-                    within a reasonable length of time, you can use this
-                    constructor parameter to downsize the array of pixels
-                    that the module must work with.  Set this parameter to
-                    a value so that the initial graph constructed from the
-                    image has no more than around 3500 vertices if you
-                    don't want to wait too long for the results.
-
-    min_size_for_graph_based_blobs: This declares a threshold on the
-                   smallest size you'd like to see (in terms of the number
-                   of pixels) in a segmented blob in the output of the
-                   graph-based segmenter.  (I typically use values from 1
-                   to 4 for this parameter.)
+    kay: This is the same as the "k" parameter in the FH algorithm.  As mentioned
+                    in the Introduction above, the Int(u) property of the pixels
+                    represented by each vertex in the graph representation of the
+                    image is extended to MInt(u) by the addition of a number k/|C|
+                    where |C| is the cardinality of the set of pixels at that
+                    vertex.
+
+    image_normalization_required: This applies Torchvision's image normalization
+                    to the pixel values in the image.
+
+    image_size_reduction_factor: As mentioned at the beginning of this document,
+                    RegionProposalGenerator is really not meant for production
+                    work.  The code is pure Python and, even with that, not at all
+                    optimized.  The focus of the module is primarily on easy
+                    understandability of what the code is doing so that you can
+                    experiment with the algorithm itself.  For the module to
+                    produce results within a reasonable length of time, you can
+                    use this constructor parameter to downsize the array of pixels
+                    that the module must work with.  Set this parameter to a value
+                    so that the initial graph constructed from the image has no
+                    more than around 3500 vertices if you don't want to wait too
+                    long for the results.
+
+    min_size_for_graph_based_blobs: This declares a threshold on the smallest size
+                   you'd like to see (in terms of the number of pixels) in a
+                   segmented blob in the output of the graph-based segmenter.  (I
+                   typically use values from 1 to 4 for this parameter.)
 
-    color_homogeneity_thresh:  
+    color_homogeneity_thresh:
 
                     This and the next three constructor options are meant
-                    specifically for the SS algorithm that sits on top of
-                    the FH algorithm for further merging of the pixel blobs
-                    produced by FH.  This constructor option specifies the
-                    maximum allowable difference between the mean color
-                    values in two pixel blobs for them to be merged.
+                    specifically for the SS algorithm that sits on top of the FH
+                    algorithm for further merging of the pixel blobs produced by
+                    FH.  This constructor option specifies the maximum allowable
+                    difference between the mean color values in two pixel blobs
+                    for them to be merged.
 
     gray_var_thresh:
 
-                   This option declares the maximum allowable difference in 
-                   the variances in the grayscale in two blobs if they are
-                   to be merged. 
+                   This option declares the maximum allowable difference in the
+                   variances in the grayscale in two blobs if they are to be
+                   merged.
 
     texture_homogeneity_thresh:
 
-                   The RegionProposalGenerator module characterizes the
-                   texture of the pixels in each segmented blob by its LBP
-                   (Local Binary Patterns) texture.  We want the LBP
-                   texture values for two different blobs to be within the
-                   value specified by this constructor option if those
-                   blobs are to be merged.
+                   The RegionProposalGenerator module characterizes the texture of
+                   the pixels in each segmented blob by its LBP (Local Binary
+                   Patterns) texture.  We want the LBP texture values for two
+                   different blobs to be within the value specified by this
+                   constructor option if those blobs are to be merged.
 
     max_num_blobs_expected:
 
-                   If you only want to extract a certain number of the
-                   largest possible blobs, you can do that by giving a
-                   value to this constructor option.
+                   If you only want to extract a certain number of the largest
+                   possible blobs, you can do that by giving a value to this
+                   constructor option.
 
 
 @title
 Inner Classes:
 
     (1)  PurdueDrEvalDataset
 
-         This is the dataset to use if you are experimenting with
-         single-instance object detection.  The dataset contains three
-         kinds of objects in its images: Dr. Eval, and two "objects" in his
-         neighborhood: a house and a watertower.  Each 128x128 image in the
-         dataset contains one of these objects after it is randomly scaled
-         and colored. Each image also contains substantial structured noise
-         in addition to 20% Gaussian noise.  Examples of these images are
-         shown in the Week 8 lecture material in Purdue's Deep Learning
-         class.
+         This is the dataset to use if you are experimenting with single-instance
+         object detection.  The dataset contains three kinds of objects in its
+         images: Dr. Eval, and two "objects" in his neighborhood: a house and a
+         watertower.  Each 128x128 image in the dataset contains one of these
+         objects after it is randomly scaled and colored. Each image also contains
+         substantial structured noise in addition to 20% Gaussian noise.  Examples
+         of these images are shown in the Week 8 lecture material in Purdue's Deep
+         Learning class.
 
     (2)  PurdueDrEvalMultiDataset
 
-         This is the dataset to use if you are experimenting with
-         multi-instance object detection.  Each image in the dataset
-         contains randomly chosen multiple instances of the same three
-         kinds of objects as mentioned above: Dr. Eval, house, and
-         watertower.  The number of object instances in each image is
-         limited to a maximum of five.  The images contain substantial
+         This is the dataset to use if you are experimenting with multi-instance
+         object detection.  Each image in the dataset contains randomly chosen
+         multiple instances of the same three kinds of objects as mentioned above:
+         Dr. Eval, house, and watertower.  The number of object instances in each
+         image is limited to a maximum of five.  The images contain substantial
          amount of structured noise in addition to 20% random noise.
          
-         The reason for why the above two datasets have "DrEval" in their
-         names: After having watched every contemporary movie at Netflix
-         that was worth watching, my wife and I decided to revisit some of
-         old movies that we had enjoyed a long time back.  That led us to
-         watching again a couple of Austin Powers movies.  If you are too
-         young to know what I am talking about, these movies are spoofs on
-         the James Bond movies in which the great comedian Mike Myers plays
-         both Austin Powers and his nemesis Dr. Evil.  Around the same
-         time, I was writing code for the two datasets mentioned above.
-         One of the three objects types in these images is a human-like
-         cartoon figure that I needed a name for.  So, after Dr. Evil in
-         the movies, I decided to call this cartoon figure Dr Eval and to
-         refer to the datasets as Dr Eval datasets. As you all know, "Eval"
-         is an important word for people like us.  All programming
-         languages provide a function with a name like "eval()".
+         The reason for why the above two datasets have "DrEval" in their names:
+         After having watched every contemporary movie at Netflix that was worth
+         watching, my wife and I decided to revisit some of old movies that we had
+         enjoyed a long time back.  That led us to watching again a couple of
+         Austin Powers movies.  If you are too young to know what I am talking
+         about, these movies are spoofs on the James Bond movies in which the
+         great comedian Mike Myers plays both Austin Powers and his nemesis
+         Dr. Evil.  Around the same time, I was writing code for the two datasets
+         mentioned above.  One of the three objects types in these images is a
+         human-like cartoon figure that I needed a name for.  So, after Dr. Evil
+         in the movies, I decided to call this cartoon figure Dr Eval and to refer
+         to the datasets as Dr Eval datasets. As you all know, "Eval" is an
+         important word for people like us.  All programming languages provide a
+         function with a name like "eval()".
 
     (3)  SingleInstanceDetector
 
          This provides a reference implementation for constructing a
-         single-instance object detector to be used for the
-         PurdueDrEvalDataset dataset. For the detection and regression
-         network, it uses the LOADnet2 network from DLStudio with small
-         modifications to account for the larger 128x128 images in the
-         dataset.
+         single-instance object detector to be used for the PurdueDrEvalDataset
+         dataset. For the detection and regression network, it uses the LOADnet2
+         network from DLStudio with small modifications to account for the larger
+         128x128 images in the dataset.
 
     (4)  YoloLikeDetector   [For multi-instance detection]
 
          The code in this inner class provides an implementation for the key
          elements of the YOLO logic for multi-instance object detection.  Each
          training image is divided into a grid of cells and it is the
          responsibility of the cell that contains the center of an object
-         bounding-box to provide at the output of the neural network an
-         estimate for the exact location of the center of the object bounding
-         box vis-a-vis the center of the cell.  That cell must also lead to an
-         estimate for the height and the width of the bounding-box for the
-         object instance.
+         bounding-box to provide at the output of the neural network an estimate
+         for the exact location of the center of the object bounding box vis-a-vis
+         the center of the cell.  That cell must also lead to an estimate for the
+         height and the width of the bounding-box for the object instance.
 
 
 @title
 PUBLIC METHODS:
 
-    Many of these method are related to using this module for experimenting
-    with the traditional graph-based algorithms for constructing region
-    proposals in images:
+    Many of these method are related to using this module for experimenting with
+    the traditional graph-based algorithms for constructing region proposals in
+    images:
 
     (1)  selective_search_for_region_proposals()
 
-         This method implements elements of the Selective Search (SS)
-         algorithm proposed by Uijlings, van de Sande, Gevers, and Smeulders
-         for creating region proposals for object detection.  As mentioned
-         elsewhere here, this algorithm sits on top of the graph based image
-         segmentation algorithm that was proposed by Felzenszwalb and
-         Huttenlocher.
+         This method implements elements of the Selective Search (SS) algorithm
+         proposed by Uijlings, van de Sande, Gevers, and Smeulders for creating
+         region proposals for object detection.  As mentioned elsewhere here, this
+         algorithm sits on top of the graph based image segmentation algorithm
+         that was proposed by Felzenszwalb and Huttenlocher.
 
     (2)  graph_based_segmentation()
 
          This is an implementation of the Felzenszwalb and Huttenlocher (FH)
-         algorithm for graph-based segmentation of images.  At the moment, it
-         is limited to working on grayscale images.
+         algorithm for graph-based segmentation of images.  At the moment, it is
+         limited to working on grayscale images.
 
     (3)  display_tensor_as_image()
 
-         This method converts the argument tensor into a photo image that you
-         can display in your terminal screen. It can convert tensors of three
-         different shapes into images: (3,H,W), (1,H,W), and (H,W), where H,
-         for height, stands for the number of pixel in the vertical direction
-         and W, for width, the same along the horizontal direction. When the
-         first element of the shape is 3, that means that the tensor
-         represents a color image in which each pixel in the (H,W) plane has
-         three values for the three color channels.  On the other hand, when
-         the first element is 1, that stands for a tensor that will be shown
-         as a grayscale image.  And when the shape is just (H,W), that is
-         automatically taken to be for a grayscale image.
+         This method converts the argument tensor into a photo image that you can
+         display in your terminal screen. It can convert tensors of three
+         different shapes into images: (3,H,W), (1,H,W), and (H,W), where H, for
+         height, stands for the number of pixel in the vertical direction and W,
+         for width, the same along the horizontal direction. When the first
+         element of the shape is 3, that means that the tensor represents a color
+         image in which each pixel in the (H,W) plane has three values for the
+         three color channels.  On the other hand, when the first element is 1,
+         that stands for a tensor that will be shown as a grayscale image.  And
+         when the shape is just (H,W), that is automatically taken to be for a
+         grayscale image.
 
     (4)  graying_resizing_binarizing()
 
-         This is a demonstration of some of the more basic and commonly used
-         image transformations from the torchvision.transformations module.
-         The large comment blocks are meant to serve as tutorial introduction
-         to the syntax used for invoking these transformations.  The
-         transformations shown can be used for converting a color image into a
-         grayscale image, for resizing an image, for converting a PIL.Image
-         into a tensor and a tensor back into an PIL.Image object, and so on.
+         This is a demonstration of some of the more basic and commonly used image
+         transformations from the torchvision.transformations module.  The large
+         comment blocks are meant to serve as tutorial introduction to the syntax
+         used for invoking these transformations.  The transformations shown can
+         be used for converting a color image into a grayscale image, for resizing
+         an image, for converting a PIL.Image into a tensor and a tensor back into
+         an PIL.Image object, and so on.
 
     (5)  accessing_one_color_plane()
 
          This method shows how can access the n-th color plane of the argument
          color image.
 
     (6)  working_with_hsv_color_space()
 
-         Illustrates converting an RGB color image into its HSV
-         representation.
+         Illustrates converting an RGB color image into its HSV representation.
 
     (7)  histogramming_the_image()
 
-         PyTorch based experiments with histogramming the grayscale and the
-         color values in an image
+         PyTorch based experiments with histogramming the grayscale and the color
+         values in an image
 
     (8)  histogramming_and_thresholding():
 
-         This method illustrates using the PyTorch functionality for
-         histogramming and thresholding individual images.
+         This method illustrates using the PyTorch functionality for histogramming
+         and thresholding individual images.
 
     (9)  convolutions_with_pytorch()
 
          This method calls on torch.nn.functional.conv2d() for demonstrating a
          single image convolution with a specified kernel.
 
     (10) gaussian_smooth()
 
-         This method smooths an image with a Gaussian of specified sigma.  You
-         can do the same much faster by using the functionality programmed
-         into torch.nn.functional.
+         This method smooths an image with a Gaussian of specified sigma.  You can
+         do the same much faster by using the functionality programmed into
+         torch.nn.functional.
 
     (11) visualize_segmentation_in_pseudocolor()
 
-         After an image has been segmented, this method can be used to assign
-         a random color to each blob in the segmented output for a better
+         After an image has been segmented, this method can be used to assign a
+         random color to each blob in the segmented output for a better
          visualization of the segmentation.
 
     (12) visualize_segmentation_with_mean_gray()
 
-         If the visualization produced by the previous method appears too
-         chaotic, you can use this method to assign the mean color to each
-         each blob in the output of an image segmentation algorithm.  The mean
-         color is derived from the pixel values in the blob.
+         If the visualization produced by the previous method appears too chaotic,
+         you can use this method to assign the mean color to each each blob in the
+         output of an image segmentation algorithm.  The mean color is derived
+         from the pixel values in the blob.
 
     (13) extract_image_region_interactively_by_dragging_mouse()
 
          You can use this method to apply the graph-based segmentation and the
-         selective search algorithms to just a portion of your image.  This
-         method extract the portion you want.  You click at the upper left
-         corner of the rectangular portion of the image you are interested in
-         and you then drag the mouse pointer to the lower right corner.  Make
-         sure that you click on "save" and "exit" after you have delineated
-         the area.
+         selective search algorithms to just a portion of your image.  This method
+         extract the portion you want.  You click at the upper left corner of the
+         rectangular portion of the image you are interested in and you then drag
+         the mouse pointer to the lower right corner.  Make sure that you click on
+         "save" and "exit" after you have delineated the area.
 
     (14) extract_image_region_interactively_through_mouse_clicks()
 
-         This method allows a user to use a sequence of mouse clicks in order
-         to specify a region of the input image that should be subject to
-         further processing.  The mouse clicks taken together define a
-         polygon. The method encloses the polygonal region by a minimum
-         bounding rectangle, which then becomes the new input image for the
-         rest of processing.
+         This method allows a user to use a sequence of mouse clicks in order to
+         specify a region of the input image that should be subject to further
+         processing.  The mouse clicks taken together define a polygon. The method
+         encloses the polygonal region by a minimum bounding rectangle, which then
+         becomes the new input image for the rest of processing.
 
     (15) displaying_and_histogramming_images_in_batch1(image_dir, batch_size)
 
          This method is the first of three such methods in this module for
          illustrating the functionality of matplotlib for simultaneously
          displaying multiple images and the results obtained from them in a
          gridded arrangement.  The core idea in this method is to call
          "plt.subplots(2,batch_size)" to create 'batch_size' number of subplot
-         objects, called "axes", in the form of a '2xbatch_size' array. We use
-         the first row of this grid to display each image in its own subplot
-         object.  And we use the second row of the grid to display the
-         histograms of the corresponding images in the first row.
+         objects, called "axes", in the form of a '2xbatch_size' array. We use the
+         first row of this grid to display each image in its own subplot object.
+         And we use the second row of the grid to display the histograms of the
+         corresponding images in the first row.
 
     (16) displaying_and_histogramming_images_in_batch2(image_dir, batch_size)
 
          I now show a second approach to displaying multiple images and their
-         corresponding histograms in a gridded display.  In this method we
-         call on "torchvision.utils.make_grid()" to construct a grid for us.
-         The grid is created by giving an argument like "nrow=4" to it.  The
-         grid object returned by the call to make_grid() is a tensor unto
-         itself. Such a tensor object is converted into a numpy array so that
-         it can be displayed by matplotlib's "imshow()" function.
+         corresponding histograms in a gridded display.  In this method we call on
+         "torchvision.utils.make_grid()" to construct a grid for us.  The grid is
+         created by giving an argument like "nrow=4" to it.  The grid object
+         returned by the call to make_grid() is a tensor unto itself. Such a
+         tensor object is converted into a numpy array so that it can be displayed
+         by matplotlib's "imshow()" function.
 
     (17) displaying_and_histogramming_images_in_batch3(image_dir, batch_size)
 
          This method illustrates two things: (1) The syntax used for the
-         'singular' version of the subplot function "plt.subplot()" ---
-         although I'll be doing so by actually calling "fig.add_subplot()".
-         And (2) How you can put together multiple multi-image plots by
-         creating multiple Figure objects.  'Figure' is the top-level
-         container of plots in matplotlib.  This method creates two separate
-         Figure objects, one as a container for all the images in a batch and
-         the other as a container for all the histograms for the images.  The
-         two Figure containers are displayed in two separate windows on your
-         computer screen.
+         'singular' version of the subplot function "plt.subplot()" --- although
+         I'll be doing so by actually calling "fig.add_subplot()".  And (2) How
+         you can put together multiple multi-image plots by creating multiple
+         Figure objects.  'Figure' is the top-level container of plots in
+         matplotlib.  This method creates two separate Figure objects, one as a
+         container for all the images in a batch and the other as a container for
+         all the histograms for the images.  The two Figure containers are
+         displayed in two separate windows on your computer screen.
+
 
 @title
 THE DATASETS INCLUDED:
 
     Download the archive
 
         datasets_for_RPG.tar.gz
 
-    through the link "Download the image datasets for RPG" at the main
-    webpage for this module and store the archive in the Examples directory
-    of your install of the module. Subsequently, execute the following
-    command in the Examples directory:
+    through the link "Download the image datasets for RPG" at the main webpage for
+    this module and store the archive in the ExamplesObjectDetection directory of
+    your install of the module. Subsequently, execute the following command in the
+    ExamplesObjectDetection directory:
 
         tar zxvf datasets_for_RPG.tar.gz
 
-    This command will create a 'data' subdirectory in the Examples directory
-    and deposit the following datasets in it:
+    This command will create a 'data' subdirectory in the ExamplesObjectDetection
+    directory and deposit the following datasets in it:
 
         Purdue_Dr_Eval_Dataset-clutter-10-noise-20-size-10000-train.gz
         Purdue_Dr_Eval_Dataset-clutter-10-noise-20-size-1000-test.gz
 
         Purdue_Dr_Eval_Multi_Dataset-clutter-10-noise-20-size-10000-train.gz
         Purdue_Dr_Eval_Multi_Dataset-clutter-10-noise-20-size-1000-test.gz
 
-    In the naming convention used for the archives, the string 'clutter-10'
-    means that each image will have a maximum of 10 clutter objects in it,
-    and the string 'noise-20' means that I have added 20% Gaussian noise to
-    each image. The string 'size-10000' means that the dataset consists of
-    '10,000' images.
+    In the naming convention used for the archives, the string 'clutter-10' means
+    that each image will have a maximum of 10 clutter objects in it, and the
+    string 'noise-20' means that I have added 20% Gaussian noise to each
+    image. The string 'size-10000' means that the dataset consists of '10,000'
+    images.
 
     The two "Multi" datasets named above are for experimenting with the YOLO
-    implementation in the module for multi-instance object detection in
-    images.  The datasets without the word "Multi" in their names are for
-    experimenting with single-instance detection --- but under circumstances
-    that are more difficult than discussed in my Week 7 Deep Learning Lecture
-    at Purdue.
-
-    You will also find two smaller datasets in the overall archive that 
-    contain just 30 images each.  Those are for debugging your code.
-
+    implementation in the module for multi-instance object detection in images.
+    The datasets without the word "Multi" in their names are for experimenting
+    with single-instance detection --- but under circumstances that are more
+    difficult than discussed in my Week 7 Deep Learning Lecture at Purdue.
+
+    You will also find two smaller datasets in the overall archive that contain
+    just 30 images each.  Those are for debugging your code.
+
+    ABOUT THE ANNOTATIONS IN THE DATASETS:
+
+    See the Slides 43 and 44 of the "Week 8: Multi-Instance Object Detection"
+    slides at the course website for a description of how the annotations are
+    organized for the dataset mentioned above.
 
 
 @title 
 THE ExamplesObjectDetection DIRECTORY:
 
-    This directory contains the following two scripts related to object
-    detection in images:
+    This directory contains the following two scripts related to object detection
+    in images:
 
         single_instance_object_detection.py
 
         multi_instance_object_detection.py
 
-    The first script carries out single-instance detections in the images in
-    the PurdueDrEvalDataset dataset and the second script carries out
-    multi-instance detections in the PurdueDrEvalMultiDataset.  In the former
-    dataset, each 128x128 image has only one instance of a meaningful object
-    along with structured artifacts and 20% random noise.  And, in the latter
-    dataset, each image has up to five instances of meaningful objects along
-    with the structured artifacts and 20% random noise.
+    The first script carries out single-instance detections in the images in the
+    PurdueDrEvalDataset dataset and the second script carries out multi-instance
+    detections in the PurdueDrEvalMultiDataset.  In the former dataset, each
+    128x128 image has only one instance of a meaningful object along with
+    structured artifacts and 20% random noise.  And, in the latter dataset, each
+    image has up to five instances of meaningful objects along with the structured
+    artifacts and 20% random noise.
 
 
 
 @title 
 THE ExamplesRegionProposals DIRECTORY:
 
     This directory contains the following scripts for showcasing graph-based
@@ -637,59 +630,59 @@
 
         torchvision_some_basic_transformations.py    
 
         torchvision_based_image_processing.py
 
         multi_image_histogramming_and_display.py  
 
-    The Examples directory also illustrates the sort of region proposal
-    results you can obtain with the graph-based algorithms in this module.
-    The specific illustrations are in the following subdirectories of the
-    Examples directory:
+    The ExamplesRegionProposals directory also illustrates the sort of region
+    proposal results you can obtain with the graph-based algorithms in this
+    module.  The specific illustrations are in the following subdirectories of the
+    ExamplesRegionProposals directory:
 
-        Examples/color_blobs/
+        ExamplesRegionProposals/color_blobs/
 
-        Examples/mondrian/
+        ExamplesRegionProposals/mondrian/
 
-        Examples/wallpic2/
+        ExamplesRegionProposals/wallpic2/
 
     Each subdirectory contains at least the following two files:
 
         selective_search.py
 
         the image file specific for that subdirectory.
 
-    All you have to do is to execute selective_search.py in that directory to
-    see the results on the image in that directory.
+    All you have to do is to execute selective_search.py in that directory to see
+    the results on the image in that directory.
 
 
 
 @title
 BUGS:
 
-    Please notify the author if you encounter any bugs.  When sending
-    email, please place the string 'RegionProposalGenerator' in the
-    subject line to get past the author's spam filter.
+    Please notify the author if you encounter any bugs.  When sending email,
+    please place the string 'RegionProposalGenerator' in the subject line to get
+    past the author's spam filter.
 
 
 @title
 ABOUT THE AUTHOR:
 
-    The author, Avinash Kak, is a professor of Electrical and Computer
-    Engineering at Purdue University.  For all issues related to this
-    module, contact the author at kak@purdue.edu If you send email,
-    please place the string "RegionProposalGenerator" in your subject
-    line to get past the author's spam filter.
+    The author, Avinash Kak, is a professor of Electrical and Computer Engineering
+    at Purdue University.  For all issues related to this module, contact the
+    author at kak@purdue.edu If you send email, please place the string
+    "RegionProposalGenerator" in your subject line to get past the author's spam
+    filter.
 
 @title
 COPYRIGHT:
 
     Python Software Foundation License
 
-    Copyright 2022 Avinash Kak
+    Copyright 2023 Avinash Kak
 
 @endofdocs
 '''
 
 import torch
 import torch.nn as nn
 import torchvision
@@ -706,15 +699,14 @@
 from PIL import ImageFont
 import sys,os,os.path,glob,signal
 import re
 import functools
 import math
 import random
 import copy
-import gzip
 import pickle
 if sys.version_info[0] == 3:
     import tkinter as Tkinter
     from tkinter.constants import *
 else:
     import Tkinter    
     from Tkconstants import *
@@ -879,15 +871,14 @@
         if 'max_iterations' in kwargs                :   max_iterations=kwargs.pop('max_iterations')
         if 'color_homogeneity_thresh' in kwargs      :   color_homogeneity_thresh = kwargs.pop('color_homogeneity_thresh')
         if 'gray_var_thresh' in kwargs               :    gray_var_thresh = kwargs.pop('gray_var_thresh')
         if 'texture_homogeneity_thresh' in kwargs    :   texture_homogeneity_thresh = kwargs.pop('texture_homogeneity_thresh')
         if 'min_size_for_graph_based_blobs' in kwargs :  min_size_for_graph_based_blobs = kwargs.pop('min_size_for_graph_based_blobs')
         if 'max_num_blobs_expected' in kwargs        :  max_num_blobs_expected = kwargs.pop('max_num_blobs_expected')
         if 'debug' in kwargs                         :   debug = kwargs.pop('debug') 
-#        if len(kwargs) != 0: raise ValueError('''You have provided unrecognizable keyword args''')
         if dataroot_train:
             self.dataroot_train = dataroot_train
         if dataroot_test:
             self.dataroot_test = dataroot_test
         if image_size:   
             self.image_size = image_size      
         if  path_saved_RPN_model:
@@ -896,15 +887,14 @@
             self.path_saved_single_instance_detector_model = path_saved_single_instance_detector_model
         if  path_saved_yolo_model:
             self.path_saved_yolo_model = path_saved_yolo_model
         if yolo_interval:
             self.yolo_interval = yolo_interval
         if classes:
             self.class_labels = classes
-#            self.class_labels_to_index = {label : classes.index(label) for label in classes}
         if learning_rate:
             self.learning_rate = learning_rate
         else:
             self.learning_rate = 1e-6
         if momentum:
             self.momentum = momentum
         if epochs:
@@ -914,16 +904,16 @@
         if use_gpu is not None:
             self.use_gpu = use_gpu
             if use_gpu is True:
                 if torch.cuda.is_available():
                     self.device = torch.device("cuda:0")
                 else:
                     raise Exception("You requested GPU support, but there's no GPU on this machine")
-            else:
-                self.device = torch.device("cpu")
+        else:
+            self.device = torch.device("cpu")
         if debug_train:                             
             self.debug_train = debug_train
         else:
             self.debug_train = 0
         if debug_test:                             
             self.debug_test = debug_test
         else:
@@ -1034,15 +1024,15 @@
             self.dataroot_train = dataroot_train
             self.dataroot_test  = dataroot_test
             self.database_train = {}
             self.database_test = {}
             self.dataset_size_train = None
             self.dataset_size_test = None
             if train_or_test == 'train':
-                self.training_dataset = self.index_dataset()
+                self.training_dataset = self.index_dataset()                  ### index_dataset() does NOT NOT NOT NOT return anything.  Only side effect used
             if train_or_test == 'test':
                 self.testing_dataset = self.index_dataset()
             self.class_labels = None
 
         def index_dataset(self):
             if self.train_or_test == 'train':
                 dataroot = self.dataroot_train
@@ -1524,17 +1514,17 @@
                     bbox_tensor = bbox_tensor.to(self.rpg.device)
                     optimizer.zero_grad()
                     outputs = net(im_tensor)
                     outputs_label = outputs[0]
                     bbox_pred = outputs[1]
                     bbox_gt = bbox_tensor
                     if i % 500 == 499:
-                        inputs_copy = im_tensor.detach().clone()
+                        inputs_copy = im_tensor.detach()
                         inputs_copy = inputs_copy.cpu()
-                        bbox_pc = bbox_pred.detach().clone()
+                        bbox_pc = bbox_pred.detach()
                         bbox_pc[bbox_pc<0] = 0
                         bbox_pc[bbox_pc>127] = 127
                         bbox_pc[torch.isnan(bbox_pc)] = 0
                         _, predicted = torch.max(outputs_label.data, 1)
                         print("[epoch:%d/%d  iter=%4d  elapsed_time=%5d secs]   Predicted Labels: " % 
                          (epoch+1, self.rpg.epochs, i+1, elapsed_time) + 
                          ' '.join('%15s' % self.rpg.class_labels[predicted[j].item()] for j in range(self.rpg.batch_size)))
@@ -1545,22 +1535,22 @@
                             j2 = int(bbox_gt[idx][2])
                             k1 = int(bbox_pc[idx][1])
                             k2 = int(bbox_pc[idx][3])
                             l1 = int(bbox_pc[idx][0])
                             l2 = int(bbox_pc[idx][2])
                             print("                    gt_bb:  [%d,%d,%d,%d]"%(j1,i1,j2,i2))
                             print("                  pred_bb:  [%d,%d,%d,%d]"%(l1,k1,l2,k2))
-                            inputs_copy[idx,0,i1:i2,j1] = 255
-                            inputs_copy[idx,0,i1:i2,j2] = 255
-                            inputs_copy[idx,0,i1,j1:j2] = 255
-                            inputs_copy[idx,0,i2,j1:j2] = 255
-                            inputs_copy[idx,2,k1:k2,l1] = 255                      
-                            inputs_copy[idx,2,k1:k2,l2] = 255
-                            inputs_copy[idx,2,k1,l1:l2] = 255
-                            inputs_copy[idx,2,k2,l1:l2] = 255
+                            inputs_copy[idx,1,i1:i2,j1] = 255
+                            inputs_copy[idx,1,i1:i2,j2] = 255
+                            inputs_copy[idx,1,i1,j1:j2] = 255
+                            inputs_copy[idx,1,i2,j1:j2] = 255
+                            inputs_copy[idx,0,k1:k2,l1] = 255                      
+                            inputs_copy[idx,0,k1:k2,l2] = 255
+                            inputs_copy[idx,0,k1,l1:l2] = 255
+                            inputs_copy[idx,0,k2,l1:l2] = 255
                     loss_labeling = criterion1(outputs_label, image_label)
                     loss_labeling.backward(retain_graph=True)        
                     loss_regression = criterion2(bbox_pred, bbox_tensor)
                     loss_regression.backward()
                     optimizer.step()
                     running_loss_labeling += loss_labeling.item()    
                     running_loss_regression += loss_regression.item()                
@@ -1758,16 +1748,16 @@
                 dataserver_train = RegionProposalGenerator.PurdueDrEvalMultiDataset(self.rpg, 
                                                        "train", dataroot_train=self.rpg.dataroot_train)
                 self.train_dataloader = torch.utils.data.DataLoader(dataserver_train, 
                                                       self.rpg.batch_size, shuffle=True, num_workers=4)
             if test:
                 dataserver_test = RegionProposalGenerator.PurdueDrEvalMultiDataset(self.rpg, 
                                                           "test", dataroot_test=self.rpg.dataroot_test)
-                self.test_dataloader = torch.utils.data.DataLoader(dataserver_test, 
-                                                     self.rpg.batch_size, shuffle=False, num_workers=4)
+                ## In the statement below, 1 is for the batch_size for testing
+                self.test_dataloader = torch.utils.data.DataLoader(dataserver_test, 1, shuffle=False)
 
         def check_dataloader(self, how_many_batches_to_show, train=False, test=False):
             if train:      
                 dataloader = self.train_dataloader
             if test:
                 dataloader = self.test_dataloader
             for idx, data in enumerate(dataloader): 
@@ -1948,15 +1938,14 @@
                 self.skip256ds = RegionProposalGenerator.YoloLikeDetector.SkipBlock(256,256,
                                                                     downsample=True, skip_connections=skip_connections)
                 self.fc_seqn = nn.Sequential(
                     nn.Linear(8192, 4096),
                     nn.ReLU(inplace=True),
                     nn.Linear(4096, 2048),
                     nn.ReLU(inplace=True),
-#                    nn.Linear(2048, 1440)
                     nn.Linear(2048, 1620)
                 )
 
             def forward(self, x):
                 x = self.pool(torch.nn.functional.relu(self.conv1(x)))          
                 x = nn.MaxPool2d(2,2)(torch.nn.functional.relu(self.conv2(x)))       
                 for i,skip64 in enumerate(self.skip64_arr[:self.depth//4]):
@@ -1997,268 +1986,269 @@
                 self.adx = adx
             def __str__(self):
                 return "AnchorBox type (h/w): %s    tlc for yolo cell: %s    anchor-box height: %d     \
                    anchor-box width: %d   adx: %d" % (self.AR, str(self.tlc), self.ab_height, self.ab_width, self.adx)
 
     
         def run_code_for_training_multi_instance_detection(self, net, display_labels=False, display_images=False):        
+
             """
             Version 2.0.6 introduced a loss function that respects the semantics of the different elements 
             of the YOLO vector.  Recall that when you assign an object bounding box to an anchor-box in a 
             specific cell of the grid over the images, you create a 5+C element YOLO vector where C is 
             the number of object classes in your dataset.  Since C=3 in our case, the YOLO vectors in our 
             case are 8-element vectors. See Slide 36 of the Week 8 slides for the meaning to be associated 
             with the different elements of a YOLO vector.
 
-            Lines 64 through 83 in the code shown below are the implementation of the new loss function.
+            Lines (68) through (79) in the code shown below are the implementation of the new loss function.
 
             Since the first element of the YOLO vector is to indicate the presence or the absence of object 
-            in a specific anchor-box in a specific cell, I use nn.BCELoss for that purpose.  The next four 
+            in a specific anchor-box of a specific cell, I use nn.BCELoss for that purpose.  The next four 
             elements carry purely numerical values that indicate the precise location of the object 
             vis-a-vis the center of the cell to which the object is assigned and also the precise height 
             and the width of the object bounding-box, I use nn.MSELoss for these four elements. The last 
             three elements are a one-hot representation of the object class label, so I use the regular 
             nn.CrossEntropyLoss for these elements.
 
             As I started writing code for incorporating the nn.CrossEntropyLoss mentioned above, I realized
             that (for purpose of loss calculation) I needed to append one more element to the last three 
             class-label elements of the YOLO vector to take care of the case when there is no object 
-            instance present in an anchor box.  You see, the dataset assumes that an image can have a 
-            maximum of 5 objects. If an image has fewer than 5 objects, that fact is expressed in the 
-            annotations by using the label value of 13 for the 'missing' objects.  To illustrate, say a
-            training image has just two objects in it, one being Dr. Eval and the other a house. In this
-            case, the annotation for the class labels would be the list [0,1,13,13,13].  If I had not 
-            augmented the YOLO vector for loss calculation, the network would be forced to choose
-            one of the actual class labels --- 0, 1, or 2 --- in the prediction for a YOLO vector even 
-            when there was no object present in the training image for that cell and that anchor box. So 
-            when the object label is 13, I throw all the probability mass related to class labels into the 
-            additional element (the 9th element) for a YOLO vector.
-
-            See Lines 57 through 60 for the above-mentioned augmentation of the YOLO vectors for all the
-            anchor boxes in all of the cells of the grid.
+            instance present in the anchor box corresponding to that yolo vector.  You see, the dataset 
+            assumes that an image can have a maximum of 5 objects. If an image has fewer than 5 objects, 
+            that fact is expressed in the annotations by using the label value of 13 for the 'missing' 
+            objects.  To illustrate, say a training image has just two objects in it, one being Dr. Eval 
+            and the other a house. In this case, the annotation for the class labels would be the list 
+            [0,1,13,13,13].  If I did not augment the YOLO vector for loss calculation, the network would 
+            be forced to choose one of the actual class labels --- 0, 1, or 2 --- in the object-label 
+            prediction for a YOLO vector even when there was no object present in the training image for 
+            that cell and that anchor box. So when the object label is 13, I throw all the probability mass 
+            related to class labels into the additional element (the 9th element) for a YOLO vector.
+
+            Line (13) initializes an augmented yolo_tensor for the augmented yolo_vectors mentioned above. 
+            Subsequently, Line (59) inserts in the augmented yolo_tensor an augmented yolo_vector for each
+            cell in the image and every anchor-box in that cell.  The loop in Lines (60) through (64) makes
+            sure of the fact that when the first element of an augmented yolo_vector is 0, meaning that there
+            is no object in the corresponding cell/anchor_box, the last element of the augmented yolo_vector
+            is set to 1. 
 
             An important consequence of augmenting the YOLO vectors in the manner explained above is that 
-            you must factor the augmentations in the processing of the predictions made by the network.
-            An example of that is shown in Line 91 where we supply 9 as the size of the vectors that
+            you must factor in the augmentations in the processing of the predictions made by the network.
+            An example of that is shown in Line (67) where we supply 9 as the size of the vectors that
             need to be recovered from the predictions.
             """
-            if self.rpg.batch_size > 1:                                                                                    ## (1)
-                sys.exit("YOLO-like multi-instance object detection has only been tested for batch_size of 1")             ## (2)
             yolo_debug = False
             filename_for_out1 = "performance_numbers_" + str(self.rpg.epochs) + "label.txt"                                
             filename_for_out2 = "performance_numbers_" + str(self.rpg.epochs) + "regres.txt"                               
             FILE1 = open(filename_for_out1, 'w')                                                                           
             FILE2 = open(filename_for_out2, 'w')                                                                           
             net = net.to(self.rpg.device)                                                                                  
-            criterion1 = nn.BCELoss()                    # For the first element of the 8 element yolo vector              ## (3)
-            criterion2 = nn.MSELoss()                    # For the regression elements (indexed 2,3,4,5) of yolo vector   ## (4)
-            criterion3 = nn.CrossEntropyLoss()           # For the last three elements of the 8 element yolo vector        ## (5)
+            criterion1 = nn.BCELoss(reduction='sum')          # For the first element of the 8 element yolo vector                ## (1)
+            criterion2 = nn.MSELoss(reduction='sum')          # For the regression elements (indexed 2,3,4,5) of yolo vector      ## (2)
+            criterion3 = nn.CrossEntropyLoss(reduction='sum') # For the last three elements of the 8 element yolo vector          ## (3)
+                                                              # Actually, the CrossEntropyLoss works on last four elements of
+                                                              #   the augmented yolo vectors.  We add one more element to the 
+                                                              #   8-element yolo vectors to allow for nilmapping.
             print("\n\nLearning Rate: ", self.rpg.learning_rate)
-            optimizer = optim.SGD(net.parameters(), lr=self.rpg.learning_rate, momentum=self.rpg.momentum)                 ## (6)
+            optimizer = optim.SGD(net.parameters(), lr=self.rpg.learning_rate, momentum=self.rpg.momentum)                        ## (4)
             print("\n\nStarting training loop...\n\n")
             start_time = time.perf_counter()
             Loss_tally = []
             elapsed_time = 0.0
-            yolo_interval = self.rpg.yolo_interval                                                                         ## (7)
-            num_yolo_cells = (self.rpg.image_size[0] // yolo_interval) * (self.rpg.image_size[1] // yolo_interval)         ## (8)
-            num_anchor_boxes =  5    # (height/width)   1/5  1/3  1/1  3/1  5/1                                            ## (9)
-            max_obj_num  = 5                                                                                               ## (10)
-            ## The 8 in the following is the size of the yolo_vector for each anchor-box in a given cell.  The 8 elements 
-            ## are: [obj_present, bx, by, bh, bw, c1, c2, c3] where bx and by are the delta diffs between the centers
-            ## of the yolo cell and the center of the object bounding box in terms of a unit for the cell width and cell 
-            ## height.  bh and bw are the height and the width of object bounding box in terms of the cell height and width.
-            for epoch in range(self.rpg.epochs):                                                                           ## (11)
+            yolo_interval = self.rpg.yolo_interval                                                                                ## (5)
+            num_yolo_cells = (self.rpg.image_size[0] // yolo_interval) * (self.rpg.image_size[1] // yolo_interval)                ## (6)
+            num_anchor_boxes =  5    # (height/width)   1/5  1/3  1/1  3/1  5/1                                                   ## (7)
+            max_obj_num  = 5                                                                                                      ## (8)
+            for epoch in range(self.rpg.epochs):                                                                                  ## (9)
                 print("")
-                running_loss = 0.0                                                                                         ## (12)
+                running_loss = 0.0                                                                                                ## (10)
                 for iter, data in enumerate(self.train_dataloader):   
                     if yolo_debug:
                         print("\n\n\n======================================= iteration: %d ========================================\n" % iter)
-                    yolo_tensor = torch.zeros( self.rpg.batch_size, num_yolo_cells, num_anchor_boxes, 8 )                  ## (13)
-                    im_tensor, seg_mask_tensor, bbox_tensor, bbox_label_tensor, num_objects_in_image = data                ## (14)
-                    im_tensor   = im_tensor.to(self.rpg.device)                                                            ## (15)
+                    im_tensor, seg_mask_tensor, bbox_tensor, bbox_label_tensor, num_objects_in_image = data                       ## (11)
+                    im_tensor   = im_tensor.to(self.rpg.device)                                 
                     seg_mask_tensor = seg_mask_tensor.to(self.rpg.device)                 
                     bbox_tensor = bbox_tensor.to(self.rpg.device)
                     bbox_label_tensor = bbox_label_tensor.to(self.rpg.device)
-                    yolo_tensor = yolo_tensor.to(self.rpg.device)
+                    ## The 8 in the following is the size of the yolo_vector for each anchor-box in a given cell.  The 8 elements 
+                    ## are: [obj_present, bx, by, bh, bw, c1, c2, c3] where bx and by are the delta diffs between the centers
+                    ## of the yolo cell and the center of the object bounding box in terms of a unit for the cell width and cell 
+                    ## height.  bh and bw are the height and the width of object bounding box in terms of the cell height and 
+                    ## width.
+                    yolo_tensor = torch.zeros( im_tensor.shape[0], num_yolo_cells, num_anchor_boxes, 8 ).to(self.rpg.device)      ## (12)
+                    ## We also define an augmented version of the above in which each yolo vector is augmented with one 
+                    ## additional element so that its length is now equal to 9 elements.  The additional element is for what's
+                    ## known as nil-mapping in computer vision.  What that means is that if we know there is no object present in
+                    ## a given cell/anchor_box combo, then we need a place to park the probability mass for the class labels
+                    ## for that combo. Speaking a bit more precisely, using CrossEntropy loss for the class labels means that
+                    ## a Softmax activation (involving a probability based normalization of the computed values) would ordinarily 
+                    ## be applied to the last 3 elements of the 8-element yolo vector.  However, that would make no sense for
+                    ## the case when a given cell/anchor_box combo contains no objects.  Extending the yolo vector by one 
+                    ## additional element allows for the probability mass to shift to that element when there is nothing in
+                    ## combo. From the standpoint of learning, a value of 1 stored in that extra element becomes the target
+                    ## for the CrossEntropy loss calculation applied to the bast FOUR elements of the yolo vectors in the 
+                    ## following tensor:
+                    yolo_tensor_aug = torch.zeros(im_tensor.shape[0], num_yolo_cells,num_anchor_boxes,9).to(self.rpg.device)      ## (13)
                     if yolo_debug:
                         logger = logging.getLogger()
                         old_level = logger.level
                         logger.setLevel(100)
                         plt.figure(figsize=[15,4])
                         plt.imshow(np.transpose(torchvision.utils.make_grid(im_tensor,normalize=True,padding=3,pad_value=255).cpu(), (1,2,0)))
                         plt.show()
                         logger.setLevel(old_level)
-                    cell_height = yolo_interval                                                                            ## (16)
-                    cell_width = yolo_interval                                                                             ## (17)
+                    cell_height = yolo_interval                                                                                   ## (14)
+                    cell_width = yolo_interval                                                                                    ## (15)
                     if yolo_debug:
                         print("\n\nnum_objects_in_image: ")
                         print(num_objects_in_image)
-                    num_cells_image_width = self.rpg.image_size[0] // yolo_interval                                        ## (18)
-                    num_cells_image_height = self.rpg.image_size[1] // yolo_interval                                       ## (19)
-                    height_center_bb = torch.zeros(im_tensor.shape[0], 1).float().to(self.rpg.device)                      ## (20)
-                    width_center_bb = torch.zeros(im_tensor.shape[0], 1).float().to(self.rpg.device)                       ## (21)
-                    obj_bb_height = torch.zeros(im_tensor.shape[0], 1).float().to(self.rpg.device)                         ## (22)
-                    obj_bb_width =  torch.zeros(im_tensor.shape[0], 1).float().to(self.rpg.device)                         ## (23)
-
-                    ## idx is for object index
-                    for idx in range(max_obj_num):                                                                         ## (24)
-                        ## In the mask, 1 means good image instance in batch, 0 means bad image instance in batch
-#                        batch_mask = torch.ones( self.rpg.batch_size, dtype=torch.int8).to(self.rpg.device)
-                        if yolo_debug:
-                            print("\n\n               ================  object indexed %d ===============              \n\n" % idx)
-                        ## Note that the bounding-box coordinates are in the (x,y) format, with x-positive going to
-                        ## right and the y-positive going down. A bbox is specified by (x_min,y_min,x_max,y_max):
-                        if yolo_debug:
-                            print("\n\nshape of bbox_tensor: ", bbox_tensor.shape)
-                            print("\n\nbbox_tensor:")
-                            print(bbox_tensor)
-                        ## in what follows, the first index (set to 0) is for the batch axis
-                        height_center_bb =  (bbox_tensor[0,idx,1] + bbox_tensor[0,idx,3]) // 2                             ## (25)
-                        width_center_bb =  (bbox_tensor[0,idx,0] + bbox_tensor[0,idx,2]) // 2                              ## (26)
-                        obj_bb_height = bbox_tensor[0,idx,3] -  bbox_tensor[0,idx,1]                                       ## (27)
-                        obj_bb_width = bbox_tensor[0,idx,2] - bbox_tensor[0,idx,0]                                         ## (28)
-                        if (obj_bb_height < 4.0) or (obj_bb_width < 4.0): continue                                         ## (29)
-
-                        cell_row_indx =  (height_center_bb / yolo_interval).int()          ## for the i coordinate         ## (30)
-                        cell_col_indx =  (width_center_bb / yolo_interval).int()           ## for the j coordinates        ## (31)
-                        cell_row_indx = torch.clamp(cell_row_indx, max=num_cells_image_height - 1)                         ## (32)
-                        cell_col_indx = torch.clamp(cell_col_indx, max=num_cells_image_width - 1)                          ## (33)
-
-                        ## The bh and bw elements in the yolo vector for this object:  bh and bw are measured relative 
-                        ## to the size of the grid cell to which the object is assigned.  For example, bh is the 
-                        ## height of the bounding-box divided by the actual height of the grid cell.
-                        bh  =  obj_bb_height.float() / yolo_interval                                                       ## (34)
-                        bw  =  obj_bb_width.float()  / yolo_interval                                                       ## (35)
-
-                        ## You have to be CAREFUL about object center calculation since bounding-box coordinates
-                        ## are in (x,y) format --- with x-positive going to the right and y-positive going down.
-                        obj_center_x =  (bbox_tensor[0,idx][2].float() +  bbox_tensor[0,idx][0].float()) / 2.0             ## (36)
-                        obj_center_y =  (bbox_tensor[0,idx][3].float() +  bbox_tensor[0,idx][1].float()) / 2.0             ## (37)
-                        ## Now you need to switch back from (x,y) format to (i,j) format:
-                        yolocell_center_i =  cell_row_indx*yolo_interval + float(yolo_interval) / 2.0                      ## (38)
-                        yolocell_center_j =  cell_col_indx*yolo_interval + float(yolo_interval) / 2.0                      ## (39)
-                        del_x  =  (obj_center_x.float() - yolocell_center_j.float()) / yolo_interval                       ## (40)
-                        del_y  =  (obj_center_y.float() - yolocell_center_i.float()) / yolo_interval                       ## (41)
-                        class_label_of_object = bbox_label_tensor[0,idx].item()                                            ## (42)
-                        ## When batch_size is only 1, it is easy to discard an image that has no known objects in it.
-                        ## To generalize this notion to arbitrary batch sizes, you will need a batch mask to indicate
-                        ## the images in a batch that should not be considered in the rest of this code.
-                        if class_label_of_object == 13: continue                                                           ## (43)
-                        AR = obj_bb_height.float() / obj_bb_width.float()                                                  ## (44)
-                        if AR <= 0.2:               anch_box_index = 0                                                     ## (45)
-                        if 0.2 < AR <= 0.5:         anch_box_index = 1                                                     ## (46)
-                        if 0.5 < AR <= 1.5:         anch_box_index = 2                                                     ## (47)
-                        if 1.5 < AR <= 4.0:         anch_box_index = 3                                                     ## (48)
-                        if AR > 4.0:                anch_box_index = 4                                                     ## (49)
-                        yolo_vector = torch.FloatTensor([0,del_x.item(), del_y.item(), bh.item(), bw.item(), 0, 0, 0] )    ## (50)
-                        yolo_vector[0] = 1                                                                                 ## (51)
-                        yolo_vector[5 + class_label_of_object] = 1                                                         ## (52)
-                        yolo_cell_index =  cell_row_indx.item() * num_cells_image_width  +  cell_col_indx.item()           ## (53)
-                        yolo_tensor[0,yolo_cell_index, anch_box_index] = yolo_vector                                       ## (54)
-                        yolo_tensor_aug = torch.zeros(self.rpg.batch_size, num_yolo_cells, \
-                                                                   num_anchor_boxes,9).float().to(self.rpg.device)         ## (55) 
-                        yolo_tensor_aug[:,:,:,:-1] =  yolo_tensor                                                          ## (56)
-                        if yolo_debug: 
-                            print("\n\nyolo_tensor specific: ")
-                            print(yolo_tensor[0,18,2])
-                            print("\nyolo_tensor_aug_aug: ") 
-                            print(yolo_tensor_aug[0,18,2])
-                    ## If no object is present, throw all the prob mass into the extra 9th ele of yolo_vector
-                    for icx in range(num_yolo_cells):                                                                      ## (57)
-                        for iax in range(num_anchor_boxes):                                                                ## (58)
-                            if yolo_tensor_aug[0,icx,iax,0] == 0:                                                          ## (59)
-                                yolo_tensor_aug[0,icx,iax,-1] = 1                                                          ## (60)
-                    if yolo_debug:
-                        logger = logging.getLogger()
-                        old_level = logger.level
-                        logger.setLevel(100)
-                        plt.figure(figsize=[15,4])
-                        plt.imshow(np.transpose(torchvision.utils.make_grid(im_tensor, normalize=True,
-                                                                         padding=3, pad_value=255).cpu(), (1,2,0)))
-                        plt.show()
-
-                    optimizer.zero_grad()                                                                                  ## (61)
-                    output = net(im_tensor)                                                                                ## (62)
-                    predictions_aug = output.view(self.rpg.batch_size,num_yolo_cells,num_anchor_boxes,9)                   ## (63)
-                    loss = torch.tensor(0.0, requires_grad=True).float().to(self.rpg.device)                               ## (64)
-                    for icx in range(num_yolo_cells):                                                                      ## (65)
-                        for iax in range(num_anchor_boxes):                                                                ## (66)
-                            pred_yolo_vector = predictions_aug[0,icx,iax]                                                  ## (67)
-                            target_yolo_vector = yolo_tensor_aug[0,icx,iax]                                                ## (68)
-                            ##  Estimating presence/absence of object and the Binary Cross Entropy section:
-                            object_presence = nn.Sigmoid()(torch.unsqueeze(pred_yolo_vector[0], dim=0))                    ## (69)
-                            target_for_prediction = torch.unsqueeze(target_yolo_vector[0], dim=0)                          ## (70)
-                            bceloss = criterion1(object_presence, target_for_prediction)                                   ## (71)
-                            loss += bceloss                                                                                ## (72)
-                            ## MSE section for regression params:
-                            pred_regression_vec = pred_yolo_vector[1:5]                                                    ## (73)
-                            pred_regression_vec = torch.unsqueeze(pred_regression_vec, dim=0)                              ## (74)
-                            target_regression_vec = torch.unsqueeze(target_yolo_vector[1:5], dim=0)                        ## (75)
-                            regression_loss = criterion2(pred_regression_vec, target_regression_vec)                       ## (76)
-                            loss += regression_loss                                                                        ## (77)
-                            ##  CrossEntropy section for object class label:
-                            probs_vector = pred_yolo_vector[5:]                                                            ## (78)
-                            probs_vector = torch.unsqueeze( probs_vector, dim=0 )                                          ## (79)
-                            target = torch.argmax(target_yolo_vector[5:])                                                  ## (80)
-                            target = torch.unsqueeze( target, dim=0 )                                                      ## (81)
-                            class_labeling_loss = criterion3(probs_vector, target)                                         ## (82)
-                            loss += class_labeling_loss                                                                    ## (83)
+                    num_cells_image_width = self.rpg.image_size[0] // yolo_interval                                               ## (16)
+                    num_cells_image_height = self.rpg.image_size[1] // yolo_interval                                              ## (17)
+                    ## ibx is batch instance index
+                    for ibx in range(im_tensor.shape[0]):                                                                         ## (18)
+                        ## idx is for object index
+                        num_of_objects =   (torch.sum(bbox_label_tensor[ibx] != 13).type(torch.uint8)).item()                     ## (19)
+                        for idx in range(num_of_objects):                                                                         ## (20)
+                            if yolo_debug:
+                                print("\n\n               ================  object indexed %d ===============              \n\n" % idx)
+                                ## Note that the bounding-box coordinates are in the (x,y) format, with x-positive going to
+                                ## right and the y-positive going down. A bbox is specified by (x_min,y_min,x_max,y_max):
+                                print("\n\nshape of bbox_tensor: ", bbox_tensor[ibx].shape)
+                                print("\n\nbbox_tensor:")
+                                print(bbox_tensor[ibx])
+                            ##  Since we are at pixel resolution at this point, there's not a whole lot of
+                            ##  between floating point division and integer division:
+                            height_center_bb =  (bbox_tensor[ibx,idx,1] + bbox_tensor[ibx,idx,3]) / 2.0                           ## (21)
+                            width_center_bb =  (bbox_tensor[ibx,idx,0] + bbox_tensor[ibx,idx,2]) / 2.0                            ## (22)
+                            obj_bb_height = bbox_tensor[ibx,idx,3] -  bbox_tensor[ibx,idx,1]                                      ## (23)
+                            obj_bb_width = bbox_tensor[ibx,idx,2] - bbox_tensor[ibx,idx,0]                                        ## (24)
+                            cell_row_indx =  (height_center_bb / yolo_interval).int()          ## for the i coordinate            ## (25)
+                            cell_col_indx =  (width_center_bb / yolo_interval).int()           ## for the j coordinates           ## (26)
+                            cell_row_indx = torch.clamp(cell_row_indx, max=num_cells_image_height - 1)                            ## (27)
+                            cell_col_indx = torch.clamp(cell_col_indx, max=num_cells_image_width - 1)                             ## (28)
+                            ## The bh and bw elements in the yolo vector for this object:  bh and bw are measured relative 
+                            ## to the size of the grid cell to which the object is assigned.  For example, bh is the 
+                            ## height of the bounding-box divided by the actual height of the grid cell.
+                            bh  =  obj_bb_height.float() / yolo_interval                                                          ## (29)
+                            bw  =  obj_bb_width.float()  / yolo_interval                                                          ## (30)
+                            ## You have to be CAREFUL about object center calculation since bounding-box coordinates
+                            ## are in (x,y) format --- with x-positive going to the right and y-positive going down.
+                            obj_center_x =  (bbox_tensor[ibx,idx][2].float() +  bbox_tensor[ibx,idx][0].float()) / 2.0            ## (31)
+                            obj_center_y =  (bbox_tensor[ibx,idx][3].float() +  bbox_tensor[ibx,idx][1].float()) / 2.0            ## (32)
+                            ## Now you need to switch back from (x,y) format to (i,j) format:
+                            yolocell_center_i =  cell_row_indx*yolo_interval + float(yolo_interval) / 2.0                         ## (33)
+                            yolocell_center_j =  cell_col_indx*yolo_interval + float(yolo_interval) / 2.0                         ## (34)
+                            del_x  =  (obj_center_x.float() - yolocell_center_j.float()) / yolo_interval                          ## (35)
+                            del_y  =  (obj_center_y.float() - yolocell_center_i.float()) / yolo_interval                          ## (36)
+                            class_label_of_object = bbox_label_tensor[ibx,idx].item()                                             ## (37)
+                            AR = obj_bb_height.float() / obj_bb_width.float()                                                     ## (38)
+                            if torch.isnan(AR):                                                                                   ## (39)
+                                AR = 100.0                                                                                        ## (40)
+                            else:
+                                AR = AR.item()                                                                                    ## (41)
+                            if AR <= 0.2:                                                                                         ## (42)
+                                anch_box_index = 0                                                                                ## (43)
+                            elif 0.2 < AR <= 0.5:                                                                                 ## (44)
+                                anch_box_index = 1                                                                                ## (45)
+                            elif 0.5 < AR <= 1.5:                                                                                 ## (46)
+                                anch_box_index = 2                                                                                ## (47)
+                            elif 1.5 < AR <= 4.0:                                                                                 ## (48)
+                                anch_box_index = 3                                                                                ## (49)
+                            elif AR > 4.0:                                                                                        ## (50)
+                                anch_box_index = 4                                                                                ## (51)
+                            yolo_vector = torch.FloatTensor([0,del_x, del_y, bh, bw, 0, 0, 0] ).to(self.rpg.device)               ## (52)
+                            if class_label_of_object != 13:                                                                       ## (53)
+                                yolo_vector[0] = 1.0                                                                              ## (54)
+                                yolo_vector[5 + class_label_of_object] = 1                                                        ## (55)
+                            yolo_cell_index =  (cell_row_indx * num_cells_image_width  +  cell_col_indx).type(torch.uint8)        ## (56)
+                            yolo_cell_index = yolo_cell_index.item()                                                              ## (57)
+                            yolo_tensor[ibx, yolo_cell_index, anch_box_index] = yolo_vector                                       ## (58)
+                            yolo_tensor_aug[ibx, yolo_cell_index, anch_box_index,:-1] = yolo_vector                               ## (59)
+                    ##  The following loop plays a critical role in the overall logic of learning. The network needs
+                    ##  to know that if the first element of a yolo vector is 0, meaning that there is no object present
+                    ##  in that cell/anchor_box combo, then all the probability weight in the last four elements of the
+                    ##  augmented yolo vector shifts to the last of the four elements:
+                    for ibx in range(im_tensor.shape[0]):                                                                         ## (60)
+                        for icx in range(num_yolo_cells):                                                                         ## (61)
+                            for iax in range(num_anchor_boxes):                                                                   ## (62)
+                                if yolo_tensor_aug[ibx, icx, iax, 0] == 0:                                                        ## (63)
+                                    yolo_tensor_aug[ibx, icx, iax,-1] = 1                                                         ## (64)
+                    optimizer.zero_grad()                                                                                         ## (65)
+                    output = net(im_tensor)                                                                                       ## (66)
+                    predictions_aug = output.view(-1,num_yolo_cells,num_anchor_boxes,9)                                           ## (67)
+
+                    ##  Now that we have the output of the network, must calculate the loss.  We initialize the loss tensors
+                    ##  for this iteration of training:
+                    loss = torch.tensor(0.0, requires_grad=True).float().to(self.rpg.device)                                      ## (68)
+                    ##  Estimating presence/absence of object with the Binary Cross Entropy loss:
+                    bceloss = criterion1( nn.Sigmoid()(predictions_aug[:,:,:,0]), yolo_tensor_aug[:,:,:,0] )                      ## (69)
+                    loss += bceloss                                                                                               ## (70)
+                    ## MSE loss for the regression params for the object bounding boxes:
+                    regression_loss = criterion2(predictions_aug[:,:,:,1:5], yolo_tensor_aug[:,:,:,1:5])                          ## (71)
+                    loss += regression_loss                                                                                       ## (72)
+                    ##  CrossEntropy loss for object class labels:
+                    targets = yolo_tensor_aug[:,:,:,5:]                                                                           ## (73)
+                    targets = targets.view(-1,4)                                                                                  ## (74)
+                    targets = torch.argmax(targets, dim=1)                                                                        ## (75)
+                    probs = predictions_aug[:,:,:,5:]                                                                             ## (76)
+                    probs = probs.view(-1,4)                                                                                      ## (77)
+                    class_labeling_loss = criterion3( probs, targets)                                                             ## (78)
+                    loss +=  class_labeling_loss                                                                                  ## (79)
                     if yolo_debug:
                         print("\n\nshape of loss: ", loss.shape)
                         print("\n\nloss: ", loss)
-                    loss.backward()                                                                                        ## (84)
-                    optimizer.step()                                                                                       ## (85)
-                    running_loss += loss.item()                                                                            ## (86)
-                    if iter%500==499:                                                                                      ## (87)
-                        current_time = time.perf_counter()
+                    loss.backward()                                                                                               ## (80)
+                    optimizer.step()                                                                                              ## (81)
+                    running_loss += loss.item()                                                                                   ## (82)
+                    if iter%500==499:                                                                                             ## (83)
+                        current_time = time.perf_counter()                                                                    
                         elapsed_time = current_time - start_time 
-                        avg_loss = running_loss / float(1000)                                                              ## (88)
+                        avg_loss = running_loss / float(500)                                                                      ## (84)
                         print("\n[epoch:%d/%d, iter=%4d  elapsed_time=%5d secs]      mean value for loss: %7.4f" % 
-                                                            (epoch+1,self.rpg.epochs, iter+1, elapsed_time, avg_loss))     ## (89)
+                                                            (epoch+1,self.rpg.epochs, iter+1, elapsed_time, avg_loss))            ## (85)
                         Loss_tally.append(running_loss)
                         FILE1.write("%.3f\n" % avg_loss)
                         FILE1.flush()
-                        running_loss = 0.0                                                                                 ## (90)
+                        running_loss = 0.0                                                                                        ## (86)
+                        running_bceloss = 0.0
+                        running_regressionloss = 0.0
+                        running_labelingloss = 0.0
                         if display_labels:
-                            predictions = output.view(self.rpg.batch_size,num_yolo_cells,num_anchor_boxes,9)               ## (91)
-                            if yolo_debug:
-                                print("\n\nyolo_vector for first image in batch, cell indexed 18, and AB indexed 2: ")
-                                print(predictions[0, 18, 2])
-                            for ibx in range(predictions.shape[0]):                             # for each batch image     ## (92)
-                                icx_2_best_anchor_box = {ic : None for ic in range(36)}                                    ## (93)
-                                for icx in range(predictions.shape[1]):                         # for each yolo cell       ## (94)
-                                    cell_predi = predictions[ibx,icx]                                                      ## (95)
-                                    prev_best = 0                                                                          ## (96)
-                                    for anchor_bdx in range(cell_predi.shape[0]):                                          ## (97)
-                                        if cell_predi[anchor_bdx][0] > cell_predi[prev_best][0]:                           ## (98)
-                                            prev_best = anchor_bdx                                                         ## (99)
-                                    best_anchor_box_icx = prev_best                                                        ## (100)
-                                    icx_2_best_anchor_box[icx] = best_anchor_box_icx                                       ## (101)
-                                sorted_icx_to_box = sorted(icx_2_best_anchor_box,                                   
-                                      key=lambda x: predictions[ibx,x,icx_2_best_anchor_box[x]][0].item(), reverse=True)   ## (102)
-                                retained_cells = sorted_icx_to_box[:5]                                                     ## (103)
-                                objects_detected = []                                                                      ## (104)
-                                for icx in retained_cells:                                                                 ## (105)
-                                    pred_vec = predictions[ibx,icx, icx_2_best_anchor_box[icx]]                            ## (106)
-                                    class_labels_predi  = pred_vec[-4:]                                                    ## (107)
-                                    class_labels_probs = torch.nn.Softmax(dim=0)(class_labels_predi)                       ## (108)
-                                    class_labels_probs = class_labels_probs[:-1]                                           ## (109)
+                            for ibx in range(predictions_aug.shape[0]):                             # for each batch image        ## (87)
+                                icx_2_best_anchor_box = {ic : None for ic in range(36)}                                           ## (88)
+                                for icx in range(predictions_aug.shape[1]):                         # for each yolo cell          ## (89)
+                                    cell_predi = predictions_aug[ibx,icx]                                                         ## (90)
+                                    prev_best = 0                                                                                 ## (91)
+                                    for anchor_bdx in range(cell_predi.shape[0]):                                                 ## (92)
+                                        if cell_predi[anchor_bdx][0] > cell_predi[prev_best][0]:                                  ## (93)
+                                            prev_best = anchor_bdx                                                                ## (94)
+                                    best_anchor_box_icx = prev_best                                                               ## (95)
+                                    icx_2_best_anchor_box[icx] = best_anchor_box_icx                                              ## (96)
+                                sorted_icx_to_box = sorted(icx_2_best_anchor_box,                                                 ## (97)
+                                      key=lambda x: predictions_aug[ibx,x,icx_2_best_anchor_box[x]][0].item(), reverse=True)      ## (98)
+                                retained_cells = sorted_icx_to_box[:5]                                                            ## (99)
+                                objects_detected = []                                                                             ## (100)
+                                for icx in retained_cells:                                                                        ## (101)
+                                    pred_vec = predictions_aug[ibx,icx, icx_2_best_anchor_box[icx]]                               ## (102)
+                                    class_labels_predi  = pred_vec[-4:]                                                           ## (103)
+                                    class_labels_probs = torch.nn.Softmax(dim=0)(class_labels_predi)                              ## (104)
+                                    class_labels_probs = class_labels_probs[:-1]                                                  ## (105)
                                     ##  The threshold of 0.25 applies only to the case of there being 3 classes of objects 
                                     ##  in the dataset.  In the absence of an object, the values in the first three nodes
                                     ##  that represent the classes should all be less than 0.25. In general, for N classes
                                     ##  you would want to set this threshold to 1.0/N
-                                    if torch.all(class_labels_probs < 0.25):                                               ## (110)
-                                        predicted_class_label = None                                                       ## (111)
+                                    if torch.all(class_labels_probs < 0.25):                                                      ## (115)
+                                        predicted_class_label = None                                                              ## (116)
                                     else:                                                                                
-                                        best_predicted_class_index = (class_labels_probs == class_labels_probs.max())      ## (112)
-                                        best_predicted_class_index =torch.nonzero(best_predicted_class_index,as_tuple=True)## (113)
-                                        predicted_class_label =self.rpg.class_labels[best_predicted_class_index[0].item()] ## (114)
-                                        objects_detected.append(predicted_class_label)                                     ## (115)
+                                        best_predicted_class_index = (class_labels_probs == class_labels_probs.max())             ## (117)
+                                        best_predicted_class_index =torch.nonzero(best_predicted_class_index,as_tuple=True)       ## (118)
+                                        predicted_class_label =self.rpg.class_labels[best_predicted_class_index[0].item()]        ## (119)
+                                        objects_detected.append(predicted_class_label)                                            ## (120)
+
                                 print("[batch image=%d]  objects found in descending probability order: " % ibx, 
-                                                                                                     objects_detected)     ## (116)
+                                                                                                     objects_detected)            ## (121)
                         if display_images:
                             logger = logging.getLogger()
                             old_level = logger.level
                             logger.setLevel(100)
                             plt.figure(figsize=[15,4])
                             plt.imshow(np.transpose(torchvision.utils.make_grid(im_tensor, normalize=True,
                                                                              padding=3, pad_value=255).cpu(), (1,2,0)))
@@ -2280,16 +2270,26 @@
         def save_yolo_model(self, model):
             '''
             Save the trained yolo model to a disk file
             '''
             torch.save(model.state_dict(), self.rpg.path_saved_yolo_model)
 
 
-        def run_code_for_testing_multi_instance_detection(self, net, display_images=False):        
+        def run_code_for_testing_multi_instance_detection(self, net, dir_name_for_results, display_images=False):        
             yolo_debug = False
+            if os.path.exists(dir_name_for_results):
+                files = glob.glob(dir_name_for_results + "/*")
+                for file in files:
+                    if os.path.isfile(file):
+                        os.remove(file)
+                    else:
+                        files = glob.glob(file + "/*")
+                        list(map(lambda x: os.remove(x), files))
+            else:
+                os.mkdir(dir_name_for_results)
             net.load_state_dict(torch.load(self.rpg.path_saved_yolo_model))
             net = net.to(self.rpg.device)
             yolo_interval = self.rpg.yolo_interval
             num_yolo_cells = (self.rpg.image_size[0] // yolo_interval) * (self.rpg.image_size[1] // yolo_interval)
             num_anchor_boxes =  5    # (height/width)   1/5  1/3  1/1  3/1  5/1
             ##  The next 5 assignment are for the calculations of the confusion matrix:
             confusion_matrix = torch.zeros(3,3)   #  We have only 3 classes:  Dr. Eval, house, and watertower
@@ -2311,15 +2311,15 @@
                     if iter % 50 == 49:
                         if display_images:
                             print("\n\n\n\nShowing output for test image %d: " % (iter+1))
                         im_tensor   = im_tensor.to(self.rpg.device)
                         seg_mask_tensor = seg_mask_tensor.to(self.rpg.device)                 
                         bbox_tensor = bbox_tensor.to(self.rpg.device)
                         output = net(im_tensor)
-                        predictions = output.view(self.rpg.batch_size,num_yolo_cells,num_anchor_boxes,9)
+                        predictions = output.view(-1, num_yolo_cells, num_anchor_boxes,9)
                         for ibx in range(predictions.shape[0]):                             # for each batch image
                             ## Our goal is to look through all the cells and identify at most five of the cells/anchor_boxes for 
                             ## the value in the first element of the predicted yolo_vectors is the highest:
                             icx_2_best_anchor_box = {ic : None for ic in range(36)}
                             for icx in range(predictions.shape[1]):                         # for each yolo cell
                                 cell_predi = predictions[ibx,icx]               
                                 prev_best = 0
@@ -2383,14 +2383,15 @@
                             print(gt_bboxes)
                         ## These are the mappings from indexes for the predicted bboxes to the indexes for the gt bboxes:
                         mapping_from_pred_to_gt = { i : None for i in range(len(predicted_bboxes))}
                         for i in range(len(predicted_bboxes)):
                             gt_possibles = {k : 0.0 for k in range(5)}      ## 0.0 for IoU 
                             for j in range(len(gt_bboxes)):
                                 if all(gt_bboxes[j][x] == 0 for x in range(4)): continue       ## 4 is for the four coords of a bbox
+                                if (gt_bboxes[j].all() == 0): continue       ## 4 is for the four coords of a bbox
                                 gt_possibles[j] = self.IoU_calculator(predicted_bboxes[i], gt_bboxes[j])
                             sorted_gt_possibles =  sorted(gt_possibles, key=lambda x: gt_possibles[x], reverse=True)
                             if display_images:
                                 print("For predicted bbox %d: the best gt bbox is: %d" % (i, sorted_gt_possibles[0]))
                             mapping_from_pred_to_gt[i] = (sorted_gt_possibles[0], gt_possibles[sorted_gt_possibles[0]])
                         ##  If you want to see the IoU scores for the overlap between each predicted bbox and all of the individual gt bboxes:
                         if display_images:
@@ -2428,17 +2429,23 @@
                             ax.imshow(np.transpose(torchvision.utils.make_grid(new_im_tensor, normalize=True, padding=3, pad_value=255).cpu(), (1,2,0)))
                             for i,bbox_pred in enumerate(predicted_bboxes):
                                 x,y,w,h = np.array(bbox_pred)                                                                     
                                 x,y,w,h = [item * display_scale for item in (x,y,w,h)]
                                 rect = Rectangle((x,y),w,h,angle=0.0,edgecolor='r',fill = False,lw=2) 
                                 ax.add_patch(rect)                                                                      
                                 ax.annotate(predicted_labels_for_bboxes[i], (x,y-1), color='red', weight='bold', fontsize=10*display_scale)
+                                gt_box_index = mapping_from_pred_to_gt[i][0]              ## '[0]' becaause mapping returns (index,prob) pair
+                                x1,y1,x2,y2 = np.array(gt_bboxes[gt_box_index])                                                                     
+                                x,y,w,h = x1,y1,x2-x1,y2-y1
+                                x,y,w,h = [item * display_scale for item in (x,y,w,h)]
+                                rect = Rectangle((x,y),w,h,angle=0.0,edgecolor='g',fill = False,lw=2) 
+                                ax.add_patch(rect)                                                                      
+                            plt.savefig(dir_name_for_results + "/" +  str(iter) + ".png")
                             plt.show()
                             logger.setLevel(old_level)
-                                                                                            
             ##  Our next job is to present to the user the information collected for the confusion matrix for the validation dataset:
             if yolo_debug:
                 print("\nConfusion Matrix: ", confusion_matrix)
                 print("\nclass_correct: ", class_correct)
                 print("\nclass_total: ", class_total)
                 print("\ntotals_for_conf_mat: ", totals_for_conf_mat)
                 print("\ntotals_correct: ", totals_correct)
```

### Comparing `RegionProposalGenerator-2.0.8/RegionProposalGenerator/__init__.py` & `RegionProposalGenerator-2.1.0/RegionProposalGenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/RegionProposalGenerator-2.0.8.html` & `RegionProposalGenerator-2.1.0/RegionProposalGenerator-2.1.0.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
  <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd"> 
 <html lang="en">
 <head>
 <title>
-RegionProposalGenerator-2.0.8.html
+RegionProposalGenerator-2.1.0.html
 </title>
 <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
 </head>
 <body bgcolor="#f0f0f8">
 <table width="100%" cellspacing="0" cellpadding="2" border="0" summary="heading">
 <tr bgcolor="#7799ee">
 <td valign=bottom>&nbsp;<br>
-<font color="#ffffff" face="helvetica, arial">&nbsp;<br><big><big><strong>RegionProposalGenerator</strong></big></big> (version 2.0.8, 2022-April-16)</font></td
+<font color="#ffffff" face="helvetica, arial">&nbsp;<br><big><big><strong>RegionProposalGenerator</strong></big></big> (version 2.1.0, 2023-April-9)</font></td
 ><td align=right valign=bottom
 ><font color="#ffffff" face="helvetica, arial">
 </font></td></tr></table>
 <p><a href="#RegionProposalGenerator"><tt>RegionProposalGenerator</tt></a>.py<br>
 <tt>
 &nbsp;<br>
-Version:&nbsp;2.0.8<br>
+Version:&nbsp;2.1.0<br>
 &nbsp;&nbsp;&nbsp;<br>
 Author:&nbsp;Avinash&nbsp;Kak&nbsp;(kak@purdue.edu)<br>
 &nbsp;<br>
-Date:&nbsp;2022-April-16<br>
+Date:&nbsp;2023-April-9<br>
 &nbsp;<br>
 &nbsp;<br>
 </tt>
 <TABLE BORDER="0" CELLPADDING="0" CELLSPACING="2"> 
 <TR>
 <TH ALIGN=left>
 <tt>
-<b>Download Version 2.0.8:</b>&nbsp;  
-<a HREF="https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.0.8.tar.gz?download">gztar</a> 
+<b>Download Version 2.1.0:</b>&nbsp;  
+<a HREF="https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.1.0.tar.gz?download">gztar</a> 
 &nbsp;             
 <br>
 <br>
 &nbsp;
 </tt>
 </TH>
 <TD>
@@ -68,237 +68,237 @@
 </tt>
 </center>
 </TD>
 </TR>
 </TABLE>
 <br>
 <tt>
-<a HREF="RegionProposalGenerator-2.0.8_CodeOnly.html">View the main module code file in your browser</a> 
+<a HREF="RegionProposalGenerator-2.1.0_CodeOnly.html">View the main module code file in your browser</a> 
 &nbsp;<br>
 &nbsp;<br>
 <a HREF="datasets_for_RPG.tar.gz">Download the image datasets for RPG</a>
 &nbsp;<br>
 &nbsp;<br>
 &nbsp;<br>   
 &nbsp;<br>
 <font size="+2" color="red">CHANGES:<br>
 </font>
 <br>
 
+
+&nbsp;&nbsp;Version&nbsp;2.1.0:<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;With&nbsp;this&nbsp;version,&nbsp;you&nbsp;can&nbsp;now&nbsp;use&nbsp;batches&nbsp;of&nbsp;any&nbsp;size&nbsp;for&nbsp;YOLO&nbsp;learning.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Previously,&nbsp;the&nbsp;batch&nbsp;size&nbsp;was&nbsp;limited&nbsp;to&nbsp;1&nbsp;for&nbsp;the&nbsp;YOLO&nbsp;part&nbsp;of&nbsp;the&nbsp;module.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Allowing&nbsp;for&nbsp;batches&nbsp;required&nbsp;changes&nbsp;in&nbsp;the&nbsp;handling&nbsp;of&nbsp;problem&nbsp;images,&nbsp;such<br>
+&nbsp;&nbsp;&nbsp;&nbsp;as&nbsp;the&nbsp;images&nbsp;with&nbsp;no&nbsp;meaningful&nbsp;objects,&nbsp;or&nbsp;the&nbsp;images&nbsp;with&nbsp;object&nbsp;bounding<br>
+&nbsp;&nbsp;&nbsp;&nbsp;boxes&nbsp;with&nbsp;unrealistic&nbsp;aspect&nbsp;ratios.<br>
+&nbsp;<br>
 &nbsp;&nbsp;Version&nbsp;2.0.8:<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;version&nbsp;constitutes&nbsp;a&nbsp;complete&nbsp;implementation&nbsp;of&nbsp;a&nbsp;YOLO<br>
-&nbsp;&nbsp;&nbsp;&nbsp;multi-instance&nbsp;object&nbsp;detector.&nbsp;&nbsp;In&nbsp;addition&nbsp;to&nbsp;the&nbsp;new&nbsp;multi-loss<br>
-&nbsp;&nbsp;&nbsp;&nbsp;function&nbsp;that&nbsp;I&nbsp;introduced&nbsp;in&nbsp;the&nbsp;previous&nbsp;public&nbsp;release&nbsp;of&nbsp;this&nbsp;module,<br>
-&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;new&nbsp;version&nbsp;includes&nbsp;a&nbsp;full-blown&nbsp;implementation&nbsp;of&nbsp;what&nbsp;you&nbsp;need&nbsp;for<br>
-&nbsp;&nbsp;&nbsp;&nbsp;validation&nbsp;testing.&nbsp;&nbsp;I&nbsp;should&nbsp;also&nbsp;mention&nbsp;that&nbsp;I&nbsp;have&nbsp;split&nbsp;what&nbsp;used&nbsp;to<br>
-&nbsp;&nbsp;&nbsp;&nbsp;be&nbsp;the&nbsp;Examples&nbsp;directory&nbsp;in&nbsp;the&nbsp;distribution&nbsp;into&nbsp;two&nbsp;directories:<br>
-&nbsp;&nbsp;&nbsp;&nbsp;ExamplesObjectDetection&nbsp;and&nbsp;ExamplesRegionProposals.&nbsp;&nbsp;Your&nbsp;entry&nbsp;point&nbsp;for<br>
-&nbsp;&nbsp;&nbsp;&nbsp;learning&nbsp;the&nbsp;YOLO&nbsp;implementation&nbsp;would&nbsp;be&nbsp;the&nbsp;script<br>
-&nbsp;&nbsp;&nbsp;&nbsp;multi_instance_object_detection.py&nbsp;in&nbsp;the&nbsp;directory<br>
-&nbsp;&nbsp;&nbsp;&nbsp;ExamplesObjectDetection.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;version&nbsp;constitutes&nbsp;a&nbsp;complete&nbsp;implementation&nbsp;of&nbsp;a&nbsp;YOLO&nbsp;multi-instance<br>
+&nbsp;&nbsp;&nbsp;&nbsp;object&nbsp;detector.&nbsp;&nbsp;In&nbsp;addition&nbsp;to&nbsp;the&nbsp;new&nbsp;multi-loss&nbsp;function&nbsp;that&nbsp;I&nbsp;introduced<br>
+&nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;the&nbsp;previous&nbsp;public&nbsp;release&nbsp;of&nbsp;this&nbsp;module,&nbsp;the&nbsp;new&nbsp;version&nbsp;includes&nbsp;a<br>
+&nbsp;&nbsp;&nbsp;&nbsp;full-blown&nbsp;implementation&nbsp;of&nbsp;what&nbsp;you&nbsp;need&nbsp;for&nbsp;validation&nbsp;testing.&nbsp;&nbsp;I&nbsp;should<br>
+&nbsp;&nbsp;&nbsp;&nbsp;also&nbsp;mention&nbsp;that&nbsp;I&nbsp;have&nbsp;split&nbsp;what&nbsp;used&nbsp;to&nbsp;be&nbsp;the&nbsp;Examples&nbsp;directory&nbsp;in&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;distribution&nbsp;into&nbsp;two&nbsp;directories:&nbsp;ExamplesObjectDetection&nbsp;and<br>
+&nbsp;&nbsp;&nbsp;&nbsp;ExamplesRegionProposals.&nbsp;&nbsp;Your&nbsp;entry&nbsp;point&nbsp;for&nbsp;learning&nbsp;the&nbsp;YOLO<br>
+&nbsp;&nbsp;&nbsp;&nbsp;implementation&nbsp;would&nbsp;be&nbsp;the&nbsp;script&nbsp;multi_instance_object_detection.py&nbsp;in&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;directory&nbsp;ExamplesObjectDetection.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;<br>
 &nbsp;&nbsp;Version&nbsp;2.0.6:<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;version&nbsp;incorporates&nbsp;a&nbsp;more&nbsp;sophisticated&nbsp;loss&nbsp;function&nbsp;for<br>
-&nbsp;&nbsp;&nbsp;&nbsp;YOLO-based&nbsp;multi-instance&nbsp;object&nbsp;detection&nbsp;in&nbsp;images.&nbsp;&nbsp;In&nbsp;the&nbsp;new&nbsp;loss<br>
-&nbsp;&nbsp;&nbsp;&nbsp;function,&nbsp;I&nbsp;use&nbsp;different&nbsp;criteria&nbsp;for&nbsp;the&nbsp;different&nbsp;segments&nbsp;of&nbsp;the&nbsp;YOLO<br>
-&nbsp;&nbsp;&nbsp;&nbsp;vector.&nbsp;&nbsp;[Assigning&nbsp;an&nbsp;object&nbsp;instance&nbsp;in&nbsp;a&nbsp;training&nbsp;image&nbsp;to&nbsp;an&nbsp;anchor<br>
-&nbsp;&nbsp;&nbsp;&nbsp;box&nbsp;for&nbsp;a&nbsp;cell&nbsp;in&nbsp;the&nbsp;image&nbsp;involves&nbsp;creating&nbsp;a&nbsp;"5+C"-element&nbsp;YOLO&nbsp;vector,<br>
-&nbsp;&nbsp;&nbsp;&nbsp;where&nbsp;C&nbsp;is&nbsp;the&nbsp;number&nbsp;of&nbsp;object&nbsp;classes.]&nbsp;I&nbsp;now&nbsp;use&nbsp;the&nbsp;Binary<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Cross-Entropy&nbsp;Loss&nbsp;(nn.BCELoss)&nbsp;for&nbsp;the&nbsp;first&nbsp;element&nbsp;of&nbsp;the&nbsp;YOLO&nbsp;vector<br>
-&nbsp;&nbsp;&nbsp;&nbsp;that&nbsp;stands&nbsp;for&nbsp;the&nbsp;presence&nbsp;or&nbsp;the&nbsp;absence&nbsp;of&nbsp;an&nbsp;object&nbsp;instance&nbsp;in&nbsp;a<br>
-&nbsp;&nbsp;&nbsp;&nbsp;specific&nbsp;anchor&nbsp;box&nbsp;in&nbsp;a&nbsp;specific&nbsp;cell.&nbsp;&nbsp;I&nbsp;use&nbsp;mean-squared-error&nbsp;loss<br>
-&nbsp;&nbsp;&nbsp;&nbsp;(nn.MSELoss)&nbsp;for&nbsp;the&nbsp;next&nbsp;four&nbsp;numerical&nbsp;elements&nbsp;that&nbsp;express&nbsp;the&nbsp;precise<br>
-&nbsp;&nbsp;&nbsp;&nbsp;location&nbsp;of&nbsp;the&nbsp;object&nbsp;bounding-box&nbsp;vis-a-vis&nbsp;the&nbsp;center&nbsp;of&nbsp;the&nbsp;cell&nbsp;to<br>
-&nbsp;&nbsp;&nbsp;&nbsp;which&nbsp;the&nbsp;object&nbsp;is&nbsp;assigned&nbsp;and&nbsp;also&nbsp;for&nbsp;the&nbsp;dimensions&nbsp;of&nbsp;the&nbsp;bounding<br>
-&nbsp;&nbsp;&nbsp;&nbsp;box.&nbsp;&nbsp;Finally,&nbsp;I&nbsp;use&nbsp;the&nbsp;regular&nbsp;Cross-Entropy&nbsp;loss&nbsp;(nn.CrossEntropyLoss)<br>
-&nbsp;&nbsp;&nbsp;&nbsp;for&nbsp;the&nbsp;last&nbsp;C&nbsp;elements&nbsp;of&nbsp;the&nbsp;YOLO&nbsp;vector.&nbsp;&nbsp;Using&nbsp;the&nbsp;cross-entropy&nbsp;loss<br>
-&nbsp;&nbsp;&nbsp;&nbsp;for&nbsp;the&nbsp;labeling&nbsp;errors&nbsp;required&nbsp;augmenting&nbsp;the&nbsp;YOLO&nbsp;vector&nbsp;with&nbsp;one<br>
-&nbsp;&nbsp;&nbsp;&nbsp;additional&nbsp;element&nbsp;to&nbsp;express&nbsp;the&nbsp;absence&nbsp;of&nbsp;an&nbsp;object.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;version&nbsp;incorporates&nbsp;a&nbsp;more&nbsp;sophisticated&nbsp;loss&nbsp;function&nbsp;for&nbsp;YOLO-based<br>
+&nbsp;&nbsp;&nbsp;&nbsp;multi-instance&nbsp;object&nbsp;detection&nbsp;in&nbsp;images.&nbsp;&nbsp;In&nbsp;the&nbsp;new&nbsp;loss&nbsp;function,&nbsp;I&nbsp;use<br>
+&nbsp;&nbsp;&nbsp;&nbsp;different&nbsp;criteria&nbsp;for&nbsp;the&nbsp;different&nbsp;segments&nbsp;of&nbsp;the&nbsp;YOLO&nbsp;vector.&nbsp;&nbsp;[Assigning<br>
+&nbsp;&nbsp;&nbsp;&nbsp;an&nbsp;object&nbsp;instance&nbsp;in&nbsp;a&nbsp;training&nbsp;image&nbsp;to&nbsp;an&nbsp;anchor&nbsp;box&nbsp;for&nbsp;a&nbsp;cell&nbsp;in&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;image&nbsp;involves&nbsp;creating&nbsp;a&nbsp;"5+C"-element&nbsp;YOLO&nbsp;vector,&nbsp;where&nbsp;C&nbsp;is&nbsp;the&nbsp;number&nbsp;of<br>
+&nbsp;&nbsp;&nbsp;&nbsp;object&nbsp;classes.]&nbsp;I&nbsp;now&nbsp;use&nbsp;the&nbsp;Binary&nbsp;Cross-Entropy&nbsp;Loss&nbsp;(nn.BCELoss)&nbsp;for&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;first&nbsp;element&nbsp;of&nbsp;the&nbsp;YOLO&nbsp;vector&nbsp;that&nbsp;stands&nbsp;for&nbsp;the&nbsp;presence&nbsp;or&nbsp;the&nbsp;absence<br>
+&nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;an&nbsp;object&nbsp;instance&nbsp;in&nbsp;a&nbsp;specific&nbsp;anchor&nbsp;box&nbsp;in&nbsp;a&nbsp;specific&nbsp;cell.&nbsp;&nbsp;I&nbsp;use<br>
+&nbsp;&nbsp;&nbsp;&nbsp;mean-squared-error&nbsp;loss&nbsp;(nn.MSELoss)&nbsp;for&nbsp;the&nbsp;next&nbsp;four&nbsp;numerical&nbsp;elements&nbsp;that<br>
+&nbsp;&nbsp;&nbsp;&nbsp;express&nbsp;the&nbsp;precise&nbsp;location&nbsp;of&nbsp;the&nbsp;object&nbsp;bounding-box&nbsp;vis-a-vis&nbsp;the&nbsp;center<br>
+&nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;the&nbsp;cell&nbsp;to&nbsp;which&nbsp;the&nbsp;object&nbsp;is&nbsp;assigned&nbsp;and&nbsp;also&nbsp;for&nbsp;the&nbsp;dimensions&nbsp;of&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;bounding&nbsp;box.&nbsp;&nbsp;Finally,&nbsp;I&nbsp;use&nbsp;the&nbsp;regular&nbsp;Cross-Entropy&nbsp;loss<br>
+&nbsp;&nbsp;&nbsp;&nbsp;(nn.CrossEntropyLoss)&nbsp;for&nbsp;the&nbsp;last&nbsp;C&nbsp;elements&nbsp;of&nbsp;the&nbsp;YOLO&nbsp;vector.&nbsp;&nbsp;Using&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;cross-entropy&nbsp;loss&nbsp;for&nbsp;the&nbsp;labeling&nbsp;errors&nbsp;required&nbsp;augmenting&nbsp;the&nbsp;YOLO&nbsp;vector<br>
+&nbsp;&nbsp;&nbsp;&nbsp;with&nbsp;one&nbsp;additional&nbsp;element&nbsp;to&nbsp;express&nbsp;the&nbsp;absence&nbsp;of&nbsp;an&nbsp;object.<br>
 &nbsp;<br>
 &nbsp;&nbsp;Version&nbsp;2.0.2:<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;version&nbsp;fixes&nbsp;a&nbsp;couple&nbsp;of&nbsp;bugs&nbsp;in&nbsp;the&nbsp;YOLO-based&nbsp;logic&nbsp;for<br>
-&nbsp;&nbsp;&nbsp;&nbsp;multi-instance&nbsp;object&nbsp;detection.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;version&nbsp;fixes&nbsp;a&nbsp;couple&nbsp;of&nbsp;bugs&nbsp;in&nbsp;the&nbsp;YOLO-based&nbsp;logic&nbsp;for&nbsp;multi-instance<br>
+&nbsp;&nbsp;&nbsp;&nbsp;object&nbsp;detection.<br>
 &nbsp;<br>
 &nbsp;&nbsp;Version&nbsp;2.0.1:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;module&nbsp;has&nbsp;gone&nbsp;through&nbsp;several&nbsp;changes&nbsp;since&nbsp;its&nbsp;last&nbsp;public-release<br>
 &nbsp;&nbsp;&nbsp;&nbsp;version&nbsp;as&nbsp;I&nbsp;was&nbsp;experimenting&nbsp;with&nbsp;different&nbsp;ways&nbsp;of&nbsp;imparting&nbsp;to&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;students&nbsp;the&nbsp;sudden&nbsp;increase&nbsp;in&nbsp;model&nbsp;complexity&nbsp;as&nbsp;one&nbsp;goes&nbsp;from<br>
-&nbsp;&nbsp;&nbsp;&nbsp;single-instance&nbsp;object&nbsp;detection&nbsp;to&nbsp;multi-instance&nbsp;object&nbsp;detection.<br>
-&nbsp;&nbsp;&nbsp;&nbsp;These&nbsp;experiments&nbsp;led&nbsp;to&nbsp;the&nbsp;creation&nbsp;of&nbsp;two&nbsp;new&nbsp;datasets,<br>
-&nbsp;&nbsp;&nbsp;&nbsp;PurdueDrEvalDataset&nbsp;and&nbsp;PurdueDrEvalMultiDataset,&nbsp;the&nbsp;former&nbsp;for&nbsp;playing<br>
-&nbsp;&nbsp;&nbsp;&nbsp;with&nbsp;single-instance&nbsp;object&nbsp;detection&nbsp;and&nbsp;the&nbsp;latter&nbsp;for&nbsp;doing&nbsp;the&nbsp;same<br>
-&nbsp;&nbsp;&nbsp;&nbsp;with&nbsp;multi-instance&nbsp;object&nbsp;detection.&nbsp;&nbsp;The&nbsp;module&nbsp;also&nbsp;includes&nbsp;two&nbsp;inner<br>
-&nbsp;&nbsp;&nbsp;&nbsp;classes,&nbsp;SingleInstanceDetector&nbsp;and&nbsp;YoloLikeDetector,&nbsp;the&nbsp;former&nbsp;a<br>
-&nbsp;&nbsp;&nbsp;&nbsp;reference&nbsp;implementation&nbsp;for&nbsp;single&nbsp;instance&nbsp;object&nbsp;detection&nbsp;and&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;latter&nbsp;a&nbsp;YOLO-like&nbsp;reference&nbsp;implementation&nbsp;for&nbsp;multi-instance&nbsp;object<br>
-&nbsp;&nbsp;&nbsp;&nbsp;detection.&nbsp;[By&nbsp;the&nbsp;way,&nbsp;"DrEval"&nbsp;in&nbsp;the&nbsp;names&nbsp;of&nbsp;the&nbsp;two&nbsp;datasets<br>
-&nbsp;&nbsp;&nbsp;&nbsp;mentioned&nbsp;here&nbsp;has&nbsp;a&nbsp;connection&nbsp;with&nbsp;"Dr&nbsp;Evil"&nbsp;in&nbsp;the&nbsp;Austin&nbsp;Powers<br>
-&nbsp;&nbsp;&nbsp;&nbsp;movies.]<br>
+&nbsp;&nbsp;&nbsp;&nbsp;single-instance&nbsp;object&nbsp;detection&nbsp;to&nbsp;multi-instance&nbsp;object&nbsp;detection.&nbsp;&nbsp;These<br>
+&nbsp;&nbsp;&nbsp;&nbsp;experiments&nbsp;led&nbsp;to&nbsp;the&nbsp;creation&nbsp;of&nbsp;two&nbsp;new&nbsp;datasets,&nbsp;PurdueDrEvalDataset&nbsp;and<br>
+&nbsp;&nbsp;&nbsp;&nbsp;PurdueDrEvalMultiDataset,&nbsp;the&nbsp;former&nbsp;for&nbsp;playing&nbsp;with&nbsp;single-instance&nbsp;object<br>
+&nbsp;&nbsp;&nbsp;&nbsp;detection&nbsp;and&nbsp;the&nbsp;latter&nbsp;for&nbsp;doing&nbsp;the&nbsp;same&nbsp;with&nbsp;multi-instance&nbsp;object<br>
+&nbsp;&nbsp;&nbsp;&nbsp;detection.&nbsp;&nbsp;The&nbsp;module&nbsp;also&nbsp;includes&nbsp;two&nbsp;inner&nbsp;classes,&nbsp;SingleInstanceDetector<br>
+&nbsp;&nbsp;&nbsp;&nbsp;and&nbsp;YoloLikeDetector,&nbsp;the&nbsp;former&nbsp;a&nbsp;reference&nbsp;implementation&nbsp;for&nbsp;single<br>
+&nbsp;&nbsp;&nbsp;&nbsp;instance&nbsp;object&nbsp;detection&nbsp;and&nbsp;the&nbsp;latter&nbsp;a&nbsp;YOLO-like&nbsp;reference&nbsp;implementation<br>
+&nbsp;&nbsp;&nbsp;&nbsp;for&nbsp;multi-instance&nbsp;object&nbsp;detection.&nbsp;[By&nbsp;the&nbsp;way,&nbsp;"DrEval"&nbsp;in&nbsp;the&nbsp;names&nbsp;of&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;two&nbsp;datasets&nbsp;mentioned&nbsp;here&nbsp;has&nbsp;a&nbsp;connection&nbsp;with&nbsp;"Dr&nbsp;Evil"&nbsp;in&nbsp;the&nbsp;Austin<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Powers&nbsp;movies.]<br>
 &nbsp;<br>
 &nbsp;&nbsp;Version&nbsp;1.0.5:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;In&nbsp;keeping&nbsp;with&nbsp;the&nbsp;tutorial&nbsp;nature&nbsp;of&nbsp;this&nbsp;module,&nbsp;this&nbsp;version&nbsp;includes<br>
-&nbsp;&nbsp;&nbsp;&nbsp;methods&nbsp;that&nbsp;come&nbsp;in&nbsp;handy&nbsp;for&nbsp;batch-based&nbsp;processing&nbsp;of&nbsp;images.&nbsp;These<br>
-&nbsp;&nbsp;&nbsp;&nbsp;methods&nbsp;carry&nbsp;names&nbsp;like&nbsp;"displaying_and_histogramming_<br>
-&nbsp;&nbsp;&nbsp;&nbsp;images_in_batchX()"&nbsp;where&nbsp;X&nbsp;is&nbsp;1,&nbsp;2,&nbsp;and&nbsp;3.&nbsp;&nbsp;The&nbsp;rest&nbsp;of&nbsp;the&nbsp;module,<br>
-&nbsp;&nbsp;&nbsp;&nbsp;especially&nbsp;the&nbsp;part&nbsp;that&nbsp;deals&nbsp;with&nbsp;constructing&nbsp;region&nbsp;proposals&nbsp;remains<br>
-&nbsp;&nbsp;&nbsp;&nbsp;unchanged.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;methods&nbsp;that&nbsp;come&nbsp;in&nbsp;handy&nbsp;for&nbsp;batch-based&nbsp;processing&nbsp;of&nbsp;images.&nbsp;These&nbsp;methods<br>
+&nbsp;&nbsp;&nbsp;&nbsp;carry&nbsp;names&nbsp;like&nbsp;"displaying_and_histogramming_&nbsp;images_in_batchX()"&nbsp;where&nbsp;X&nbsp;is<br>
+&nbsp;&nbsp;&nbsp;&nbsp;1,&nbsp;2,&nbsp;and&nbsp;3.&nbsp;&nbsp;The&nbsp;rest&nbsp;of&nbsp;the&nbsp;module,&nbsp;especially&nbsp;the&nbsp;part&nbsp;that&nbsp;deals&nbsp;with<br>
+&nbsp;&nbsp;&nbsp;&nbsp;constructing&nbsp;region&nbsp;proposals&nbsp;remains&nbsp;unchanged.<br>
 &nbsp;<br>
 &nbsp;&nbsp;Version&nbsp;1.0.4:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;is&nbsp;the&nbsp;first&nbsp;public&nbsp;release&nbsp;version&nbsp;of&nbsp;the&nbsp;module.<br>
 &nbsp;<br>
 &nbsp;<br>
 <font size="+2" color="red">INTRODUCTION:<br>
 </font>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Single-Instance&nbsp;vs.&nbsp;Multi-Instance&nbsp;Detection:<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;module&nbsp;was&nbsp;created&nbsp;for&nbsp;experimenting&nbsp;with&nbsp;the&nbsp;logic&nbsp;of&nbsp;object<br>
-&nbsp;&nbsp;&nbsp;&nbsp;detection&nbsp;with&nbsp;neural&nbsp;networks.&nbsp;&nbsp;On&nbsp;the&nbsp;face&nbsp;of&nbsp;it,&nbsp;object&nbsp;detection&nbsp;in<br>
-&nbsp;&nbsp;&nbsp;&nbsp;images&nbsp;sounds&nbsp;like&nbsp;a&nbsp;well-defined&nbsp;problem&nbsp;that&nbsp;should&nbsp;lend&nbsp;itself&nbsp;to<br>
-&nbsp;&nbsp;&nbsp;&nbsp;well-defined&nbsp;solutions.&nbsp;&nbsp;Unfortunately,&nbsp;the&nbsp;reality&nbsp;is&nbsp;otherwise.&nbsp;&nbsp;Yes,<br>
-&nbsp;&nbsp;&nbsp;&nbsp;simple&nbsp;examples&nbsp;of&nbsp;the&nbsp;problem&nbsp;--&nbsp;such&nbsp;as&nbsp;when&nbsp;the&nbsp;images&nbsp;contain<br>
-&nbsp;&nbsp;&nbsp;&nbsp;single&nbsp;object&nbsp;instances&nbsp;and&nbsp;with&nbsp;no&nbsp;competing&nbsp;clutter&nbsp;in&nbsp;the&nbsp;background<br>
-&nbsp;&nbsp;&nbsp;&nbsp;--&nbsp;the&nbsp;problem&nbsp;can&nbsp;be&nbsp;solved&nbsp;straightforwardly&nbsp;with&nbsp;a&nbsp;neural&nbsp;network.<br>
-&nbsp;&nbsp;&nbsp;&nbsp;However,&nbsp;the&nbsp;object&nbsp;detection&nbsp;problems&nbsp;that&nbsp;are&nbsp;encountered&nbsp;in&nbsp;real<br>
-&nbsp;&nbsp;&nbsp;&nbsp;life&nbsp;are&nbsp;rarely&nbsp;that&nbsp;simple.&nbsp;&nbsp;A&nbsp;practically&nbsp;useful&nbsp;framework&nbsp;for&nbsp;object<br>
-&nbsp;&nbsp;&nbsp;&nbsp;detection&nbsp;must&nbsp;be&nbsp;able&nbsp;to&nbsp;recognize&nbsp;and&nbsp;localize&nbsp;all&nbsp;possible&nbsp;instances<br>
-&nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;the&nbsp;objects&nbsp;of&nbsp;interest&nbsp;in&nbsp;a&nbsp;given&nbsp;image.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;module&nbsp;was&nbsp;created&nbsp;for&nbsp;experimenting&nbsp;with&nbsp;the&nbsp;logic&nbsp;of&nbsp;object&nbsp;detection<br>
+&nbsp;&nbsp;&nbsp;&nbsp;with&nbsp;neural&nbsp;networks.&nbsp;&nbsp;On&nbsp;the&nbsp;face&nbsp;of&nbsp;it,&nbsp;object&nbsp;detection&nbsp;in&nbsp;images&nbsp;sounds<br>
+&nbsp;&nbsp;&nbsp;&nbsp;like&nbsp;a&nbsp;well-defined&nbsp;problem&nbsp;that&nbsp;should&nbsp;lend&nbsp;itself&nbsp;to&nbsp;well-defined&nbsp;solutions.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Unfortunately,&nbsp;the&nbsp;reality&nbsp;is&nbsp;otherwise.&nbsp;&nbsp;Yes,&nbsp;simple&nbsp;examples&nbsp;of&nbsp;the&nbsp;problem<br>
+&nbsp;&nbsp;&nbsp;&nbsp;--&nbsp;such&nbsp;as&nbsp;when&nbsp;the&nbsp;images&nbsp;contain&nbsp;single&nbsp;object&nbsp;instances&nbsp;and&nbsp;with&nbsp;no<br>
+&nbsp;&nbsp;&nbsp;&nbsp;competing&nbsp;clutter&nbsp;in&nbsp;the&nbsp;background&nbsp;--&nbsp;the&nbsp;problem&nbsp;can&nbsp;be&nbsp;solved<br>
+&nbsp;&nbsp;&nbsp;&nbsp;straightforwardly&nbsp;with&nbsp;a&nbsp;neural&nbsp;network.&nbsp;&nbsp;However,&nbsp;the&nbsp;object&nbsp;detection<br>
+&nbsp;&nbsp;&nbsp;&nbsp;problems&nbsp;that&nbsp;are&nbsp;encountered&nbsp;in&nbsp;real&nbsp;life&nbsp;are&nbsp;rarely&nbsp;that&nbsp;simple.&nbsp;&nbsp;A<br>
+&nbsp;&nbsp;&nbsp;&nbsp;practically&nbsp;useful&nbsp;framework&nbsp;for&nbsp;object&nbsp;detection&nbsp;must&nbsp;be&nbsp;able&nbsp;to&nbsp;recognize<br>
+&nbsp;&nbsp;&nbsp;&nbsp;and&nbsp;localize&nbsp;all&nbsp;possible&nbsp;instances&nbsp;of&nbsp;the&nbsp;objects&nbsp;of&nbsp;interest&nbsp;in&nbsp;a&nbsp;given<br>
+&nbsp;&nbsp;&nbsp;&nbsp;image.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;So&nbsp;how&nbsp;does&nbsp;one&nbsp;solve&nbsp;the&nbsp;problem&nbsp;of&nbsp;multi-instance&nbsp;object&nbsp;detection&nbsp;and<br>
 &nbsp;&nbsp;&nbsp;&nbsp;localization&nbsp;with&nbsp;a&nbsp;neural&nbsp;network?<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;last&nbsp;half-dozen&nbsp;years&nbsp;have&nbsp;seen&nbsp;the&nbsp;emergence&nbsp;of&nbsp;the&nbsp;following&nbsp;three<br>
-&nbsp;&nbsp;&nbsp;&nbsp;competition-grade&nbsp;neural-network&nbsp;based&nbsp;approaches&nbsp;for&nbsp;multi-instance<br>
-&nbsp;&nbsp;&nbsp;&nbsp;object&nbsp;detection:&nbsp;R-CNN,&nbsp;YOLO,&nbsp;and&nbsp;SSD.&nbsp;&nbsp;The&nbsp;Preamble&nbsp;section&nbsp;of&nbsp;my&nbsp;Week&nbsp;8<br>
-&nbsp;&nbsp;&nbsp;&nbsp;lecture&nbsp;for&nbsp;Purdue's&nbsp;Deep&nbsp;Learning&nbsp;class&nbsp;provides&nbsp;a&nbsp;brief&nbsp;overview&nbsp;of<br>
-&nbsp;&nbsp;&nbsp;&nbsp;these&nbsp;approaches.&nbsp;&nbsp;YOLO&nbsp;stands&nbsp;for&nbsp;"You&nbsp;Only&nbsp;Look&nbsp;Once"&nbsp;---&nbsp;in&nbsp;contrast<br>
-&nbsp;&nbsp;&nbsp;&nbsp;with&nbsp;R-CNN&nbsp;based&nbsp;approaches&nbsp;in&nbsp;which&nbsp;you&nbsp;may&nbsp;have&nbsp;to&nbsp;subject&nbsp;the&nbsp;images&nbsp;to<br>
-&nbsp;&nbsp;&nbsp;&nbsp;a&nbsp;couple&nbsp;of&nbsp;neural&nbsp;networks,&nbsp;one&nbsp;for&nbsp;generating&nbsp;region&nbsp;proposals&nbsp;and&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;other&nbsp;for&nbsp;actual&nbsp;object&nbsp;detection.<br>
-&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;main&nbsp;goal&nbsp;of&nbsp;the&nbsp;present&nbsp;module&nbsp;is&nbsp;to&nbsp;provide&nbsp;an&nbsp;educational&nbsp;example<br>
-&nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;a&nbsp;complete&nbsp;implementation&nbsp;of&nbsp;the&nbsp;YOLO&nbsp;logic&nbsp;for&nbsp;multi-instance&nbsp;object<br>
-&nbsp;&nbsp;&nbsp;&nbsp;detection&nbsp;in&nbsp;images.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;competition-grade&nbsp;neural-network&nbsp;based&nbsp;approaches&nbsp;for&nbsp;multi-instance&nbsp;object<br>
+&nbsp;&nbsp;&nbsp;&nbsp;detection:&nbsp;R-CNN,&nbsp;YOLO,&nbsp;and&nbsp;SSD.&nbsp;&nbsp;The&nbsp;Preamble&nbsp;section&nbsp;of&nbsp;my&nbsp;Week&nbsp;8&nbsp;lecture<br>
+&nbsp;&nbsp;&nbsp;&nbsp;for&nbsp;Purdue's&nbsp;Deep&nbsp;Learning&nbsp;class&nbsp;provides&nbsp;a&nbsp;brief&nbsp;overview&nbsp;of&nbsp;these<br>
+&nbsp;&nbsp;&nbsp;&nbsp;approaches.&nbsp;&nbsp;YOLO&nbsp;stands&nbsp;for&nbsp;"You&nbsp;Only&nbsp;Look&nbsp;Once"&nbsp;---&nbsp;in&nbsp;contrast&nbsp;with&nbsp;R-CNN<br>
+&nbsp;&nbsp;&nbsp;&nbsp;based&nbsp;approaches&nbsp;in&nbsp;which&nbsp;you&nbsp;may&nbsp;have&nbsp;to&nbsp;subject&nbsp;the&nbsp;images&nbsp;to&nbsp;a&nbsp;couple&nbsp;of<br>
+&nbsp;&nbsp;&nbsp;&nbsp;neural&nbsp;networks,&nbsp;one&nbsp;for&nbsp;generating&nbsp;region&nbsp;proposals&nbsp;and&nbsp;the&nbsp;other&nbsp;for&nbsp;actual<br>
+&nbsp;&nbsp;&nbsp;&nbsp;object&nbsp;detection.<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;main&nbsp;goal&nbsp;of&nbsp;the&nbsp;present&nbsp;module&nbsp;is&nbsp;to&nbsp;provide&nbsp;an&nbsp;educational&nbsp;example&nbsp;of&nbsp;a<br>
+&nbsp;&nbsp;&nbsp;&nbsp;complete&nbsp;implementation&nbsp;of&nbsp;the&nbsp;YOLO&nbsp;logic&nbsp;for&nbsp;multi-instance&nbsp;object&nbsp;detection<br>
+&nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;images.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Graph-Based&nbsp;Algorithms&nbsp;for&nbsp;Region&nbsp;Proposals:<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;A&nbsp;second&nbsp;goal&nbsp;of&nbsp;this&nbsp;module&nbsp;is&nbsp;to&nbsp;provide&nbsp;implementations&nbsp;for&nbsp;a&nbsp;couple<br>
-&nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;the&nbsp;more&nbsp;modern&nbsp;graph-based&nbsp;approaches&nbsp;for&nbsp;generating&nbsp;region<br>
-&nbsp;&nbsp;&nbsp;&nbsp;proposals.&nbsp;&nbsp;At&nbsp;this&nbsp;point,&nbsp;the&nbsp;reader&nbsp;might&nbsp;ask:&nbsp;What&nbsp;is&nbsp;a&nbsp;region<br>
-&nbsp;&nbsp;&nbsp;&nbsp;proposal?&nbsp;&nbsp;A&nbsp;region&nbsp;proposal&nbsp;is&nbsp;a&nbsp;blob&nbsp;of&nbsp;pixels&nbsp;that&nbsp;is&nbsp;highly&nbsp;likely<br>
-&nbsp;&nbsp;&nbsp;&nbsp;to&nbsp;contain&nbsp;an&nbsp;object&nbsp;instance.&nbsp;&nbsp;Another&nbsp;way&nbsp;of&nbsp;saying&nbsp;same&nbsp;thing&nbsp;is<br>
-&nbsp;&nbsp;&nbsp;&nbsp;that&nbsp;region&nbsp;proposals&nbsp;are&nbsp;pixel&nbsp;blobs&nbsp;that&nbsp;look&nbsp;different&nbsp;from&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;general&nbsp;background&nbsp;in&nbsp;the&nbsp;images.&nbsp;&nbsp;While&nbsp;it&nbsp;is&nbsp;possible&nbsp;to&nbsp;use&nbsp;a&nbsp;neural<br>
-&nbsp;&nbsp;&nbsp;&nbsp;network&nbsp;for&nbsp;generating&nbsp;region&nbsp;proposals,&nbsp;as&nbsp;demonstrated&nbsp;by&nbsp;the&nbsp;success<br>
-&nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;RPN&nbsp;(Region&nbsp;Proposal&nbsp;Network)&nbsp;in&nbsp;the&nbsp;R-CNN&nbsp;based&nbsp;multi-instance<br>
+&nbsp;&nbsp;&nbsp;&nbsp;A&nbsp;second&nbsp;goal&nbsp;of&nbsp;this&nbsp;module&nbsp;is&nbsp;to&nbsp;provide&nbsp;implementations&nbsp;for&nbsp;a&nbsp;couple&nbsp;of&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;more&nbsp;modern&nbsp;graph-based&nbsp;approaches&nbsp;for&nbsp;generating&nbsp;region&nbsp;proposals.&nbsp;&nbsp;At&nbsp;this<br>
+&nbsp;&nbsp;&nbsp;&nbsp;point,&nbsp;the&nbsp;reader&nbsp;might&nbsp;ask:&nbsp;What&nbsp;is&nbsp;a&nbsp;region&nbsp;proposal?&nbsp;&nbsp;A&nbsp;region&nbsp;proposal&nbsp;is<br>
+&nbsp;&nbsp;&nbsp;&nbsp;a&nbsp;blob&nbsp;of&nbsp;pixels&nbsp;that&nbsp;is&nbsp;highly&nbsp;likely&nbsp;to&nbsp;contain&nbsp;an&nbsp;object&nbsp;instance.&nbsp;&nbsp;Another<br>
+&nbsp;&nbsp;&nbsp;&nbsp;way&nbsp;of&nbsp;saying&nbsp;same&nbsp;thing&nbsp;is&nbsp;that&nbsp;region&nbsp;proposals&nbsp;are&nbsp;pixel&nbsp;blobs&nbsp;that&nbsp;look<br>
+&nbsp;&nbsp;&nbsp;&nbsp;different&nbsp;from&nbsp;the&nbsp;general&nbsp;background&nbsp;in&nbsp;the&nbsp;images.&nbsp;&nbsp;While&nbsp;it&nbsp;is&nbsp;possible&nbsp;to<br>
+&nbsp;&nbsp;&nbsp;&nbsp;use&nbsp;a&nbsp;neural&nbsp;network&nbsp;for&nbsp;generating&nbsp;region&nbsp;proposals,&nbsp;as&nbsp;demonstrated&nbsp;by&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;success&nbsp;of&nbsp;RPN&nbsp;(Region&nbsp;Proposal&nbsp;Network)&nbsp;in&nbsp;the&nbsp;R-CNN&nbsp;based&nbsp;multi-instance<br>
 &nbsp;&nbsp;&nbsp;&nbsp;object&nbsp;detection,&nbsp;the&nbsp;RPG&nbsp;module&nbsp;is&nbsp;concerned&nbsp;primarily&nbsp;with&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;non-neural-network&nbsp;based&nbsp;methods&nbsp;--&nbsp;the&nbsp;graph-based&nbsp;methods&nbsp;--&nbsp;for<br>
-&nbsp;&nbsp;&nbsp;&nbsp;generating&nbsp;region&nbsp;proposals.&nbsp;&nbsp;I&nbsp;believe&nbsp;that&nbsp;becoming&nbsp;familiar&nbsp;with&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;non-learning&nbsp;based&nbsp;methods&nbsp;for&nbsp;constructing&nbsp;region&nbsp;proposals&nbsp;still&nbsp;has<br>
-&nbsp;&nbsp;&nbsp;&nbsp;considerable&nbsp;value.&nbsp;&nbsp;Consider,&nbsp;for&nbsp;example,&nbsp;the&nbsp;problem&nbsp;of&nbsp;detecting<br>
-&nbsp;&nbsp;&nbsp;&nbsp;objects&nbsp;in&nbsp;satellite&nbsp;images&nbsp;where&nbsp;you&nbsp;simply&nbsp;do&nbsp;not&nbsp;have&nbsp;access&nbsp;to&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;amount&nbsp;of&nbsp;training&nbsp;data&nbsp;you&nbsp;would&nbsp;need&nbsp;for&nbsp;a&nbsp;neural-network&nbsp;based<br>
-&nbsp;&nbsp;&nbsp;&nbsp;approach&nbsp;to&nbsp;work.<br>
-&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;With&nbsp;regard&nbsp;to&nbsp;the&nbsp;graph-based&nbsp;method&nbsp;for&nbsp;generating&nbsp;region&nbsp;proposals,<br>
-&nbsp;&nbsp;&nbsp;&nbsp;RPG&nbsp;(RegionProposalGenerator)&nbsp;implements&nbsp;elements&nbsp;of&nbsp;the&nbsp;Selective<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Search&nbsp;(SS)&nbsp;algorithm&nbsp;for&nbsp;object&nbsp;detection&nbsp;as&nbsp;proposed&nbsp;by&nbsp;Uijlings,&nbsp;van<br>
-&nbsp;&nbsp;&nbsp;&nbsp;de&nbsp;Sande,&nbsp;Gevers,&nbsp;and&nbsp;Smeulders.&nbsp;&nbsp;The&nbsp;Selective&nbsp;Search&nbsp;algorithm&nbsp;sits<br>
-&nbsp;&nbsp;&nbsp;&nbsp;on&nbsp;top&nbsp;of&nbsp;the&nbsp;graph-based&nbsp;image&nbsp;segmentation&nbsp;algorithm&nbsp;of&nbsp;Felzenszwalb<br>
-&nbsp;&nbsp;&nbsp;&nbsp;and&nbsp;Huttenlocher&nbsp;(FH)&nbsp;whose&nbsp;implementation&nbsp;is&nbsp;also&nbsp;included&nbsp;in&nbsp;the&nbsp;RPG<br>
-&nbsp;&nbsp;&nbsp;&nbsp;module.&nbsp;&nbsp;The&nbsp;RPG&nbsp;module&nbsp;first&nbsp;processes&nbsp;an&nbsp;image&nbsp;with&nbsp;the&nbsp;FH<br>
-&nbsp;&nbsp;&nbsp;&nbsp;graph-based&nbsp;algorithm&nbsp;for&nbsp;image&nbsp;segmentation&nbsp;to&nbsp;divide&nbsp;an&nbsp;image&nbsp;into<br>
-&nbsp;&nbsp;&nbsp;&nbsp;pixel&nbsp;blobs.&nbsp;&nbsp;The&nbsp;module&nbsp;subsequently&nbsp;invokes&nbsp;elements&nbsp;of&nbsp;the&nbsp;SS<br>
-&nbsp;&nbsp;&nbsp;&nbsp;algorithm&nbsp;to&nbsp;selectively&nbsp;merge&nbsp;the&nbsp;blobs&nbsp;on&nbsp;the&nbsp;basis&nbsp;of&nbsp;three<br>
+&nbsp;&nbsp;&nbsp;&nbsp;non-neural-network&nbsp;based&nbsp;methods&nbsp;--&nbsp;the&nbsp;graph-based&nbsp;methods&nbsp;--&nbsp;for&nbsp;generating<br>
+&nbsp;&nbsp;&nbsp;&nbsp;region&nbsp;proposals.&nbsp;&nbsp;I&nbsp;believe&nbsp;that&nbsp;becoming&nbsp;familiar&nbsp;with&nbsp;the&nbsp;non-learning<br>
+&nbsp;&nbsp;&nbsp;&nbsp;based&nbsp;methods&nbsp;for&nbsp;constructing&nbsp;region&nbsp;proposals&nbsp;still&nbsp;has&nbsp;considerable&nbsp;value.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Consider,&nbsp;for&nbsp;example,&nbsp;the&nbsp;problem&nbsp;of&nbsp;detecting&nbsp;objects&nbsp;in&nbsp;satellite&nbsp;images<br>
+&nbsp;&nbsp;&nbsp;&nbsp;where&nbsp;you&nbsp;simply&nbsp;do&nbsp;not&nbsp;have&nbsp;access&nbsp;to&nbsp;the&nbsp;amount&nbsp;of&nbsp;training&nbsp;data&nbsp;you&nbsp;would<br>
+&nbsp;&nbsp;&nbsp;&nbsp;need&nbsp;for&nbsp;a&nbsp;neural-network&nbsp;based&nbsp;approach&nbsp;to&nbsp;work.<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;With&nbsp;regard&nbsp;to&nbsp;the&nbsp;graph-based&nbsp;method&nbsp;for&nbsp;generating&nbsp;region&nbsp;proposals,&nbsp;RPG<br>
+&nbsp;&nbsp;&nbsp;&nbsp;(RegionProposalGenerator)&nbsp;implements&nbsp;elements&nbsp;of&nbsp;the&nbsp;Selective&nbsp;Search&nbsp;(SS)<br>
+&nbsp;&nbsp;&nbsp;&nbsp;algorithm&nbsp;for&nbsp;object&nbsp;detection&nbsp;as&nbsp;proposed&nbsp;by&nbsp;Uijlings,&nbsp;van&nbsp;de&nbsp;Sande,&nbsp;Gevers,<br>
+&nbsp;&nbsp;&nbsp;&nbsp;and&nbsp;Smeulders.&nbsp;&nbsp;The&nbsp;Selective&nbsp;Search&nbsp;algorithm&nbsp;sits&nbsp;on&nbsp;top&nbsp;of&nbsp;the&nbsp;graph-based<br>
+&nbsp;&nbsp;&nbsp;&nbsp;image&nbsp;segmentation&nbsp;algorithm&nbsp;of&nbsp;Felzenszwalb&nbsp;and&nbsp;Huttenlocher&nbsp;(FH)&nbsp;whose<br>
+&nbsp;&nbsp;&nbsp;&nbsp;implementation&nbsp;is&nbsp;also&nbsp;included&nbsp;in&nbsp;the&nbsp;RPG&nbsp;module.&nbsp;&nbsp;The&nbsp;RPG&nbsp;module&nbsp;first<br>
+&nbsp;&nbsp;&nbsp;&nbsp;processes&nbsp;an&nbsp;image&nbsp;with&nbsp;the&nbsp;FH&nbsp;graph-based&nbsp;algorithm&nbsp;for&nbsp;image&nbsp;segmentation&nbsp;to<br>
+&nbsp;&nbsp;&nbsp;&nbsp;divide&nbsp;an&nbsp;image&nbsp;into&nbsp;pixel&nbsp;blobs.&nbsp;&nbsp;The&nbsp;module&nbsp;subsequently&nbsp;invokes&nbsp;elements&nbsp;of<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;SS&nbsp;algorithm&nbsp;to&nbsp;selectively&nbsp;merge&nbsp;the&nbsp;blobs&nbsp;on&nbsp;the&nbsp;basis&nbsp;of&nbsp;three<br>
 &nbsp;&nbsp;&nbsp;&nbsp;properties:&nbsp;homogeneity&nbsp;of&nbsp;the&nbsp;color,&nbsp;grayscale&nbsp;variance,&nbsp;and&nbsp;texture<br>
 &nbsp;&nbsp;&nbsp;&nbsp;homogeneity.<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;FH&nbsp;algorithm&nbsp;is&nbsp;based&nbsp;on&nbsp;creating&nbsp;a&nbsp;graph-based&nbsp;representation&nbsp;of<br>
-&nbsp;&nbsp;&nbsp;&nbsp;an&nbsp;image&nbsp;in&nbsp;which,&nbsp;at&nbsp;the&nbsp;beginning,&nbsp;each&nbsp;pixel&nbsp;is&nbsp;a&nbsp;single&nbsp;vertex&nbsp;and<br>
-&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;edge&nbsp;between&nbsp;two&nbsp;vertices&nbsp;that&nbsp;stand&nbsp;for&nbsp;two&nbsp;adjacent&nbsp;pixels<br>
-&nbsp;&nbsp;&nbsp;&nbsp;represents&nbsp;the&nbsp;difference&nbsp;between&nbsp;some&nbsp;pixel&nbsp;property&nbsp;(such&nbsp;as&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;color&nbsp;difference)&nbsp;at&nbsp;the&nbsp;two&nbsp;pixels.&nbsp;&nbsp;Subsequently,&nbsp;for&nbsp;the&nbsp;vertex<br>
-&nbsp;&nbsp;&nbsp;&nbsp;merging&nbsp;logic,&nbsp;each&nbsp;vertex&nbsp;u,&nbsp;that&nbsp;after&nbsp;the&nbsp;first&nbsp;iteration&nbsp;stands&nbsp;for<br>
-&nbsp;&nbsp;&nbsp;&nbsp;a&nbsp;grouping&nbsp;of&nbsp;pixels,&nbsp;is&nbsp;characterized&nbsp;by&nbsp;a&nbsp;property&nbsp;called&nbsp;Int(u),<br>
-&nbsp;&nbsp;&nbsp;&nbsp;which&nbsp;is&nbsp;the&nbsp;largest&nbsp;value&nbsp;of&nbsp;the&nbsp;inter-pixel&nbsp;color&nbsp;difference&nbsp;between<br>
-&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;adjacent&nbsp;pixels.&nbsp;&nbsp;In&nbsp;order&nbsp;to&nbsp;account&nbsp;for&nbsp;the&nbsp;fact&nbsp;that,&nbsp;at&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;beginning,&nbsp;each&nbsp;vertex&nbsp;consists&nbsp;of&nbsp;only&nbsp;one&nbsp;pixel&nbsp;[which&nbsp;would&nbsp;not<br>
-&nbsp;&nbsp;&nbsp;&nbsp;allow&nbsp;for&nbsp;the&nbsp;calculation&nbsp;of&nbsp;Int(u)],&nbsp;the&nbsp;unary&nbsp;property&nbsp;of&nbsp;the&nbsp;pixels<br>
-&nbsp;&nbsp;&nbsp;&nbsp;at&nbsp;a&nbsp;vertex&nbsp;is&nbsp;extended&nbsp;from&nbsp;Int(u)&nbsp;to&nbsp;MInt(u)&nbsp;with&nbsp;the&nbsp;addition&nbsp;of&nbsp;a<br>
-&nbsp;&nbsp;&nbsp;&nbsp;vertex-size&nbsp;dependent&nbsp;number&nbsp;equal&nbsp;to&nbsp;k/|C|&nbsp;where&nbsp;"k"&nbsp;is&nbsp;a<br>
-&nbsp;&nbsp;&nbsp;&nbsp;user-specified&nbsp;parameter&nbsp;and&nbsp;|C|&nbsp;the&nbsp;cardinality&nbsp;of&nbsp;the&nbsp;set&nbsp;of&nbsp;pixels<br>
-&nbsp;&nbsp;&nbsp;&nbsp;represented&nbsp;by&nbsp;the&nbsp;vertex&nbsp;u&nbsp;in&nbsp;the&nbsp;graph.<br>
-&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;As&nbsp;mentioned&nbsp;above,&nbsp;initially&nbsp;the&nbsp;edges&nbsp;in&nbsp;the&nbsp;graph&nbsp;representation&nbsp;of<br>
-&nbsp;&nbsp;&nbsp;&nbsp;an&nbsp;image&nbsp;are&nbsp;set&nbsp;to&nbsp;the&nbsp;color&nbsp;difference&nbsp;between&nbsp;the&nbsp;two&nbsp;8-adjacent<br>
-&nbsp;&nbsp;&nbsp;&nbsp;pixels&nbsp;that&nbsp;correspond&nbsp;to&nbsp;two&nbsp;different&nbsp;vertices.&nbsp;&nbsp;Subsequently,&nbsp;as&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;vertices&nbsp;are&nbsp;merged,&nbsp;an&nbsp;edge,&nbsp;E(u,v),&nbsp;between&nbsp;two&nbsp;vertices&nbsp;u&nbsp;and&nbsp;v&nbsp;is<br>
-&nbsp;&nbsp;&nbsp;&nbsp;set&nbsp;to&nbsp;the&nbsp;smallest&nbsp;value&nbsp;of&nbsp;the&nbsp;inter-pixel&nbsp;color&nbsp;difference&nbsp;for&nbsp;two<br>
-&nbsp;&nbsp;&nbsp;&nbsp;adjacent&nbsp;pixels&nbsp;that&nbsp;belong&nbsp;to&nbsp;the&nbsp;two&nbsp;vertices.&nbsp;At&nbsp;each&nbsp;iteration&nbsp;of<br>
-&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;algorithm,&nbsp;two&nbsp;vertices&nbsp;u&nbsp;and&nbsp;v&nbsp;are&nbsp;merged&nbsp;provided&nbsp;E(u,v)&nbsp;is&nbsp;less<br>
-&nbsp;&nbsp;&nbsp;&nbsp;than&nbsp;the&nbsp;smaller&nbsp;of&nbsp;the&nbsp;MInt(u)&nbsp;or&nbsp;MInt(v)&nbsp;attributes&nbsp;at&nbsp;the&nbsp;two<br>
-&nbsp;&nbsp;&nbsp;&nbsp;vertices.&nbsp;&nbsp;My&nbsp;experience&nbsp;is&nbsp;that&nbsp;for&nbsp;most&nbsp;images&nbsp;the&nbsp;algorithm<br>
-&nbsp;&nbsp;&nbsp;&nbsp;terminates&nbsp;of&nbsp;its&nbsp;own&nbsp;accord&nbsp;after&nbsp;a&nbsp;small&nbsp;number&nbsp;of&nbsp;iterations&nbsp;while<br>
-&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;vertex&nbsp;merging&nbsp;condition&nbsp;can&nbsp;be&nbsp;satisfied.<br>
-&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Since&nbsp;the&nbsp;algorithm&nbsp;is&nbsp;driven&nbsp;by&nbsp;the&nbsp;color&nbsp;differences&nbsp;between<br>
-&nbsp;&nbsp;&nbsp;&nbsp;8-adjacent&nbsp;pixels,&nbsp;the&nbsp;FH&nbsp;algorithm&nbsp;is&nbsp;likely&nbsp;to&nbsp;create&nbsp;too&nbsp;fine&nbsp;a<br>
-&nbsp;&nbsp;&nbsp;&nbsp;segmentation&nbsp;of&nbsp;an&nbsp;image.&nbsp;&nbsp;The&nbsp;segments&nbsp;produced&nbsp;by&nbsp;FH&nbsp;can&nbsp;be&nbsp;made<br>
-&nbsp;&nbsp;&nbsp;&nbsp;larger&nbsp;by&nbsp;using&nbsp;the&nbsp;logic&nbsp;of&nbsp;SS&nbsp;that&nbsp;allows&nbsp;blobs&nbsp;of&nbsp;pixels&nbsp;to&nbsp;merge<br>
-&nbsp;&nbsp;&nbsp;&nbsp;into&nbsp;larger&nbsp;blobs&nbsp;provided&nbsp;doing&nbsp;so&nbsp;makes&nbsp;sense&nbsp;based&nbsp;on&nbsp;the&nbsp;inter-blob<br>
-&nbsp;&nbsp;&nbsp;&nbsp;values&nbsp;for&nbsp;mean&nbsp;color&nbsp;levels,&nbsp;color&nbsp;variances,&nbsp;texture&nbsp;values,&nbsp;etc.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;FH&nbsp;algorithm&nbsp;is&nbsp;based&nbsp;on&nbsp;creating&nbsp;a&nbsp;graph-based&nbsp;representation&nbsp;of&nbsp;an&nbsp;image<br>
+&nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;which,&nbsp;at&nbsp;the&nbsp;beginning,&nbsp;each&nbsp;pixel&nbsp;is&nbsp;a&nbsp;single&nbsp;vertex&nbsp;and&nbsp;the&nbsp;edge&nbsp;between<br>
+&nbsp;&nbsp;&nbsp;&nbsp;two&nbsp;vertices&nbsp;that&nbsp;stand&nbsp;for&nbsp;two&nbsp;adjacent&nbsp;pixels&nbsp;represents&nbsp;the&nbsp;difference<br>
+&nbsp;&nbsp;&nbsp;&nbsp;between&nbsp;some&nbsp;pixel&nbsp;property&nbsp;(such&nbsp;as&nbsp;the&nbsp;color&nbsp;difference)&nbsp;at&nbsp;the&nbsp;two&nbsp;pixels.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Subsequently,&nbsp;for&nbsp;the&nbsp;vertex&nbsp;merging&nbsp;logic,&nbsp;each&nbsp;vertex&nbsp;u,&nbsp;that&nbsp;after&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;first&nbsp;iteration&nbsp;stands&nbsp;for&nbsp;a&nbsp;grouping&nbsp;of&nbsp;pixels,&nbsp;is&nbsp;characterized&nbsp;by&nbsp;a<br>
+&nbsp;&nbsp;&nbsp;&nbsp;property&nbsp;called&nbsp;Int(u),&nbsp;which&nbsp;is&nbsp;the&nbsp;largest&nbsp;value&nbsp;of&nbsp;the&nbsp;inter-pixel&nbsp;color<br>
+&nbsp;&nbsp;&nbsp;&nbsp;difference&nbsp;between&nbsp;the&nbsp;adjacent&nbsp;pixels.&nbsp;&nbsp;In&nbsp;order&nbsp;to&nbsp;account&nbsp;for&nbsp;the&nbsp;fact<br>
+&nbsp;&nbsp;&nbsp;&nbsp;that,&nbsp;at&nbsp;the&nbsp;beginning,&nbsp;each&nbsp;vertex&nbsp;consists&nbsp;of&nbsp;only&nbsp;one&nbsp;pixel&nbsp;[which&nbsp;would<br>
+&nbsp;&nbsp;&nbsp;&nbsp;not&nbsp;allow&nbsp;for&nbsp;the&nbsp;calculation&nbsp;of&nbsp;Int(u)],&nbsp;the&nbsp;unary&nbsp;property&nbsp;of&nbsp;the&nbsp;pixels&nbsp;at<br>
+&nbsp;&nbsp;&nbsp;&nbsp;a&nbsp;vertex&nbsp;is&nbsp;extended&nbsp;from&nbsp;Int(u)&nbsp;to&nbsp;MInt(u)&nbsp;with&nbsp;the&nbsp;addition&nbsp;of&nbsp;a&nbsp;vertex-size<br>
+&nbsp;&nbsp;&nbsp;&nbsp;dependent&nbsp;number&nbsp;equal&nbsp;to&nbsp;k/|C|&nbsp;where&nbsp;"k"&nbsp;is&nbsp;a&nbsp;user-specified&nbsp;parameter&nbsp;and<br>
+&nbsp;&nbsp;&nbsp;&nbsp;|C|&nbsp;the&nbsp;cardinality&nbsp;of&nbsp;the&nbsp;set&nbsp;of&nbsp;pixels&nbsp;represented&nbsp;by&nbsp;the&nbsp;vertex&nbsp;u&nbsp;in&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;graph.<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;As&nbsp;mentioned&nbsp;above,&nbsp;initially&nbsp;the&nbsp;edges&nbsp;in&nbsp;the&nbsp;graph&nbsp;representation&nbsp;of&nbsp;an<br>
+&nbsp;&nbsp;&nbsp;&nbsp;image&nbsp;are&nbsp;set&nbsp;to&nbsp;the&nbsp;color&nbsp;difference&nbsp;between&nbsp;the&nbsp;two&nbsp;8-adjacent&nbsp;pixels&nbsp;that<br>
+&nbsp;&nbsp;&nbsp;&nbsp;correspond&nbsp;to&nbsp;two&nbsp;different&nbsp;vertices.&nbsp;&nbsp;Subsequently,&nbsp;as&nbsp;the&nbsp;vertices&nbsp;are<br>
+&nbsp;&nbsp;&nbsp;&nbsp;merged,&nbsp;an&nbsp;edge,&nbsp;E(u,v),&nbsp;between&nbsp;two&nbsp;vertices&nbsp;u&nbsp;and&nbsp;v&nbsp;is&nbsp;set&nbsp;to&nbsp;the&nbsp;smallest<br>
+&nbsp;&nbsp;&nbsp;&nbsp;value&nbsp;of&nbsp;the&nbsp;inter-pixel&nbsp;color&nbsp;difference&nbsp;for&nbsp;two&nbsp;adjacent&nbsp;pixels&nbsp;that&nbsp;belong<br>
+&nbsp;&nbsp;&nbsp;&nbsp;to&nbsp;the&nbsp;two&nbsp;vertices.&nbsp;At&nbsp;each&nbsp;iteration&nbsp;of&nbsp;the&nbsp;algorithm,&nbsp;two&nbsp;vertices&nbsp;u&nbsp;and&nbsp;v<br>
+&nbsp;&nbsp;&nbsp;&nbsp;are&nbsp;merged&nbsp;provided&nbsp;E(u,v)&nbsp;is&nbsp;less&nbsp;than&nbsp;the&nbsp;smaller&nbsp;of&nbsp;the&nbsp;MInt(u)&nbsp;or&nbsp;MInt(v)<br>
+&nbsp;&nbsp;&nbsp;&nbsp;attributes&nbsp;at&nbsp;the&nbsp;two&nbsp;vertices.&nbsp;&nbsp;My&nbsp;experience&nbsp;is&nbsp;that&nbsp;for&nbsp;most&nbsp;images&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;algorithm&nbsp;terminates&nbsp;of&nbsp;its&nbsp;own&nbsp;accord&nbsp;after&nbsp;a&nbsp;small&nbsp;number&nbsp;of&nbsp;iterations<br>
+&nbsp;&nbsp;&nbsp;&nbsp;while&nbsp;the&nbsp;vertex&nbsp;merging&nbsp;condition&nbsp;can&nbsp;be&nbsp;satisfied.<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Since&nbsp;the&nbsp;algorithm&nbsp;is&nbsp;driven&nbsp;by&nbsp;the&nbsp;color&nbsp;differences&nbsp;between&nbsp;8-adjacent<br>
+&nbsp;&nbsp;&nbsp;&nbsp;pixels,&nbsp;the&nbsp;FH&nbsp;algorithm&nbsp;is&nbsp;likely&nbsp;to&nbsp;create&nbsp;too&nbsp;fine&nbsp;a&nbsp;segmentation&nbsp;of&nbsp;an<br>
+&nbsp;&nbsp;&nbsp;&nbsp;image.&nbsp;&nbsp;The&nbsp;segments&nbsp;produced&nbsp;by&nbsp;FH&nbsp;can&nbsp;be&nbsp;made&nbsp;larger&nbsp;by&nbsp;using&nbsp;the&nbsp;logic&nbsp;of<br>
+&nbsp;&nbsp;&nbsp;&nbsp;SS&nbsp;that&nbsp;allows&nbsp;blobs&nbsp;of&nbsp;pixels&nbsp;to&nbsp;merge&nbsp;into&nbsp;larger&nbsp;blobs&nbsp;provided&nbsp;doing&nbsp;so<br>
+&nbsp;&nbsp;&nbsp;&nbsp;makes&nbsp;sense&nbsp;based&nbsp;on&nbsp;the&nbsp;inter-blob&nbsp;values&nbsp;for&nbsp;mean&nbsp;color&nbsp;levels,&nbsp;color<br>
+&nbsp;&nbsp;&nbsp;&nbsp;variances,&nbsp;texture&nbsp;values,&nbsp;etc.<br>
 &nbsp;<br>
 &nbsp;<br>
 <font size="+2" color="red">INSTALLATION:<br>
 </font>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;RegionProposalGenerator&nbsp;class&nbsp;was&nbsp;packaged&nbsp;using&nbsp;setuptools.&nbsp;&nbsp;For<br>
-&nbsp;&nbsp;&nbsp;&nbsp;installation,&nbsp;execute&nbsp;the&nbsp;following&nbsp;command&nbsp;in&nbsp;the&nbsp;source&nbsp;directory<br>
-&nbsp;&nbsp;&nbsp;&nbsp;(this&nbsp;is&nbsp;the&nbsp;directory&nbsp;that&nbsp;contains&nbsp;the&nbsp;setup.py&nbsp;file&nbsp;after&nbsp;you&nbsp;have<br>
-&nbsp;&nbsp;&nbsp;&nbsp;downloaded&nbsp;and&nbsp;uncompressed&nbsp;the&nbsp;package):<br>
+&nbsp;&nbsp;&nbsp;&nbsp;installation,&nbsp;execute&nbsp;the&nbsp;following&nbsp;command&nbsp;in&nbsp;the&nbsp;source&nbsp;directory&nbsp;(this&nbsp;is<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;directory&nbsp;that&nbsp;contains&nbsp;the&nbsp;setup.py&nbsp;file&nbsp;after&nbsp;you&nbsp;have&nbsp;downloaded&nbsp;and<br>
+&nbsp;&nbsp;&nbsp;&nbsp;uncompressed&nbsp;the&nbsp;package):<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;sudo&nbsp;python3&nbsp;setup.py&nbsp;install<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;On&nbsp;Linux&nbsp;distributions,&nbsp;this&nbsp;will&nbsp;install&nbsp;the&nbsp;module&nbsp;file&nbsp;at&nbsp;a&nbsp;location<br>
-&nbsp;&nbsp;&nbsp;&nbsp;that&nbsp;looks&nbsp;like<br>
+&nbsp;&nbsp;&nbsp;&nbsp;On&nbsp;Linux&nbsp;distributions,&nbsp;this&nbsp;will&nbsp;install&nbsp;the&nbsp;module&nbsp;file&nbsp;at&nbsp;a&nbsp;location&nbsp;that<br>
+&nbsp;&nbsp;&nbsp;&nbsp;looks&nbsp;like<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;/usr/local/lib/python3.8/dist-packages/<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;If&nbsp;you&nbsp;do&nbsp;not&nbsp;have&nbsp;root&nbsp;access,&nbsp;you&nbsp;have&nbsp;the&nbsp;option&nbsp;of&nbsp;working&nbsp;directly<br>
-&nbsp;&nbsp;&nbsp;&nbsp;off&nbsp;the&nbsp;directory&nbsp;in&nbsp;which&nbsp;you&nbsp;downloaded&nbsp;the&nbsp;software&nbsp;by&nbsp;simply<br>
-&nbsp;&nbsp;&nbsp;&nbsp;placing&nbsp;the&nbsp;following&nbsp;statements&nbsp;at&nbsp;the&nbsp;top&nbsp;of&nbsp;your&nbsp;scripts&nbsp;that&nbsp;use<br>
-&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;RegionProposalGenerator&nbsp;class:<br>
+&nbsp;&nbsp;&nbsp;&nbsp;If&nbsp;you&nbsp;do&nbsp;not&nbsp;have&nbsp;root&nbsp;access,&nbsp;you&nbsp;have&nbsp;the&nbsp;option&nbsp;of&nbsp;working&nbsp;directly&nbsp;off<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;directory&nbsp;in&nbsp;which&nbsp;you&nbsp;downloaded&nbsp;the&nbsp;software&nbsp;by&nbsp;simply&nbsp;placing&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;following&nbsp;statements&nbsp;at&nbsp;the&nbsp;top&nbsp;of&nbsp;your&nbsp;scripts&nbsp;that&nbsp;use&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;RegionProposalGenerator&nbsp;class:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;import&nbsp;sys<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;sys.path.append(&nbsp;"pathname_to_RegionProposalGenerator_directory"&nbsp;)<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;To&nbsp;uninstall&nbsp;the&nbsp;module,&nbsp;simply&nbsp;delete&nbsp;the&nbsp;source&nbsp;directory,&nbsp;locate<br>
-&nbsp;&nbsp;&nbsp;&nbsp;where&nbsp;the&nbsp;RegionProposalGenerator&nbsp;module&nbsp;was&nbsp;installed&nbsp;with&nbsp;"locate<br>
-&nbsp;&nbsp;&nbsp;&nbsp;RegionProposalGenerator"&nbsp;and&nbsp;delete&nbsp;those&nbsp;files.&nbsp;&nbsp;As&nbsp;mentioned&nbsp;above,<br>
-&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;full&nbsp;pathname&nbsp;to&nbsp;the&nbsp;installed&nbsp;version&nbsp;is&nbsp;likely&nbsp;to&nbsp;look&nbsp;like<br>
+&nbsp;&nbsp;&nbsp;&nbsp;To&nbsp;uninstall&nbsp;the&nbsp;module,&nbsp;simply&nbsp;delete&nbsp;the&nbsp;source&nbsp;directory,&nbsp;locate&nbsp;where&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;RegionProposalGenerator&nbsp;module&nbsp;was&nbsp;installed&nbsp;with&nbsp;"locate<br>
+&nbsp;&nbsp;&nbsp;&nbsp;RegionProposalGenerator"&nbsp;and&nbsp;delete&nbsp;those&nbsp;files.&nbsp;&nbsp;As&nbsp;mentioned&nbsp;above,&nbsp;the&nbsp;full<br>
+&nbsp;&nbsp;&nbsp;&nbsp;pathname&nbsp;to&nbsp;the&nbsp;installed&nbsp;version&nbsp;is&nbsp;likely&nbsp;to&nbsp;look&nbsp;like<br>
 &nbsp;&nbsp;&nbsp;&nbsp;/usr/local/lib/python2.7/dist-packages/RegionProposalGenerator*<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;If&nbsp;you&nbsp;want&nbsp;to&nbsp;carry&nbsp;out&nbsp;a&nbsp;non-standard&nbsp;install&nbsp;of&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;RegionProposalGenerator&nbsp;module,&nbsp;look&nbsp;up&nbsp;the&nbsp;on-line&nbsp;information&nbsp;on<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Disutils&nbsp;by&nbsp;pointing&nbsp;your&nbsp;browser&nbsp;to<br>
+&nbsp;&nbsp;&nbsp;&nbsp;If&nbsp;you&nbsp;want&nbsp;to&nbsp;carry&nbsp;out&nbsp;a&nbsp;non-standard&nbsp;install&nbsp;of&nbsp;the&nbsp;RegionProposalGenerator<br>
+&nbsp;&nbsp;&nbsp;&nbsp;module,&nbsp;look&nbsp;up&nbsp;the&nbsp;on-line&nbsp;information&nbsp;on&nbsp;Disutils&nbsp;by&nbsp;pointing&nbsp;your&nbsp;browser<br>
+&nbsp;&nbsp;&nbsp;&nbsp;to<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<a href="http://docs.python.org/dist/dist.html">http://docs.python.org/dist/dist.html</a><br>
 &nbsp;<br>
 <font size="+2" color="red">USAGE:<br>
 </font>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Single-Instance&nbsp;and&nbsp;Multi-Instance&nbsp;Detection:<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;If&nbsp;you&nbsp;wish&nbsp;to&nbsp;experiment&nbsp;with&nbsp;YOLO-like&nbsp;logic&nbsp;for&nbsp;multi-instance<br>
-&nbsp;&nbsp;&nbsp;&nbsp;object&nbsp;detection,&nbsp;you&nbsp;would&nbsp;need&nbsp;to&nbsp;construct&nbsp;an&nbsp;instance&nbsp;of&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;RegionProposalGenerator&nbsp;class&nbsp;and&nbsp;invoke&nbsp;the&nbsp;methods&nbsp;shown&nbsp;below&nbsp;on<br>
-&nbsp;&nbsp;&nbsp;&nbsp;this&nbsp;instance:<br>
+&nbsp;&nbsp;&nbsp;&nbsp;If&nbsp;you&nbsp;wish&nbsp;to&nbsp;experiment&nbsp;with&nbsp;YOLO-like&nbsp;logic&nbsp;for&nbsp;multi-instance&nbsp;object<br>
+&nbsp;&nbsp;&nbsp;&nbsp;detection,&nbsp;you&nbsp;would&nbsp;need&nbsp;to&nbsp;construct&nbsp;an&nbsp;instance&nbsp;of&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;RegionProposalGenerator&nbsp;class&nbsp;and&nbsp;invoke&nbsp;the&nbsp;methods&nbsp;shown&nbsp;below&nbsp;on&nbsp;this<br>
+&nbsp;&nbsp;&nbsp;&nbsp;instance:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;rpg&nbsp;=&nbsp;RegionProposalGenerator(<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;dataroot&nbsp;=&nbsp;"./data/",<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;image_size&nbsp;=&nbsp;[128,128],<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;yolo_interval&nbsp;=&nbsp;20,<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;path_saved_yolo_model&nbsp;=&nbsp;"./saved_yolo_model",<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;momentum&nbsp;=&nbsp;0.9,<br>
@@ -314,17 +314,17 @@
 &nbsp;&nbsp;&nbsp;&nbsp;model&nbsp;=&nbsp;yolo.NetForYolo(skip_connections=True,&nbsp;depth=8)&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;model&nbsp;=&nbsp;yolo.run_code_for_training_multi_instance_detection(model,&nbsp;display_images=False)<br>
 &nbsp;&nbsp;&nbsp;&nbsp;yolo.run_code_for_training_multi_instance_detection(model,&nbsp;display_images&nbsp;=&nbsp;True)<br>
 &nbsp;&nbsp;&nbsp;&nbsp;<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Graph-Based&nbsp;Algorithms&nbsp;for&nbsp;Region&nbsp;Proposals:<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;To&nbsp;generate&nbsp;region&nbsp;proposals,&nbsp;you&nbsp;would&nbsp;need&nbsp;to&nbsp;construct&nbsp;an&nbsp;instance<br>
-&nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;the&nbsp;RegionProposalGenerator&nbsp;class&nbsp;and&nbsp;invoke&nbsp;the&nbsp;methods&nbsp;shown&nbsp;below<br>
-&nbsp;&nbsp;&nbsp;&nbsp;on&nbsp;this&nbsp;instance:<br>
+&nbsp;&nbsp;&nbsp;&nbsp;To&nbsp;generate&nbsp;region&nbsp;proposals,&nbsp;you&nbsp;would&nbsp;need&nbsp;to&nbsp;construct&nbsp;an&nbsp;instance&nbsp;of&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;RegionProposalGenerator&nbsp;class&nbsp;and&nbsp;invoke&nbsp;the&nbsp;methods&nbsp;shown&nbsp;below&nbsp;on&nbsp;this<br>
+&nbsp;&nbsp;&nbsp;&nbsp;instance:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;rpg&nbsp;=&nbsp;RegionProposalGenerator(<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;###&nbsp;&nbsp;The&nbsp;first&nbsp;6&nbsp;options&nbsp;affect&nbsp;only&nbsp;the&nbsp;Graph-Based&nbsp;part&nbsp;of&nbsp;the&nbsp;algo<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;sigma&nbsp;=&nbsp;1.0,<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;max_iterations&nbsp;=&nbsp;40,<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;kay&nbsp;=&nbsp;0.05,<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;image_normalization_required&nbsp;=&nbsp;True,<br>
@@ -341,348 +341,340 @@
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;rpg.visualize_segmentation_in_pseudocolor(segmented_graph[0],&nbsp;color_map,&nbsp;"graph_based"&nbsp;)<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;merged_blobs,&nbsp;color_map&nbsp;=&nbsp;rpg.selective_search_for_region_proposals(&nbsp;segmented_graph,&nbsp;image_name&nbsp;)<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;rpg.visualize_segmentation_with_mean_gray(merged_blobs,&nbsp;"ss_based_segmentation_in_bw"&nbsp;)<br>
 &nbsp;<br>
 &nbsp;<br>
 <font size="+2" color="red">CONSTRUCTOR&nbsp;PARAMETERS:&nbsp;<br>
 </font>&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Of&nbsp;the&nbsp;10&nbsp;constructor&nbsp;parameters&nbsp;listed&nbsp;below,&nbsp;the&nbsp;first&nbsp;six&nbsp;are&nbsp;meant&nbsp;for<br>
-&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;FH&nbsp;algorithm&nbsp;and&nbsp;the&nbsp;last&nbsp;four&nbsp;for&nbsp;the&nbsp;SS&nbsp;algorithm.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Of&nbsp;the&nbsp;10&nbsp;constructor&nbsp;parameters&nbsp;listed&nbsp;below,&nbsp;the&nbsp;first&nbsp;six&nbsp;are&nbsp;meant&nbsp;for&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;FH&nbsp;algorithm&nbsp;and&nbsp;the&nbsp;last&nbsp;four&nbsp;for&nbsp;the&nbsp;SS&nbsp;algorithm.<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;sigma:&nbsp;Controls&nbsp;the&nbsp;size&nbsp;of&nbsp;the&nbsp;Gaussian&nbsp;kernel&nbsp;used&nbsp;for&nbsp;smoothing&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;image&nbsp;before&nbsp;its&nbsp;gradient&nbsp;is&nbsp;calculated.&nbsp;&nbsp;Assuming&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;pixel&nbsp;sampling&nbsp;interval&nbsp;to&nbsp;be&nbsp;unity,&nbsp;a&nbsp;sigma&nbsp;of&nbsp;1&nbsp;gives<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;you&nbsp;a&nbsp;7x7&nbsp;smoothing&nbsp;operator&nbsp;with&nbsp;Gaussian&nbsp;weighting.<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;default&nbsp;for&nbsp;this&nbsp;parameter&nbsp;is&nbsp;1.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;sigma:&nbsp;Controls&nbsp;the&nbsp;size&nbsp;of&nbsp;the&nbsp;Gaussian&nbsp;kernel&nbsp;used&nbsp;for&nbsp;smoothing&nbsp;the&nbsp;image<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;before&nbsp;its&nbsp;gradient&nbsp;is&nbsp;calculated.&nbsp;&nbsp;Assuming&nbsp;the&nbsp;pixel<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;sampling&nbsp;interval&nbsp;to&nbsp;be&nbsp;unity,&nbsp;a&nbsp;sigma&nbsp;of&nbsp;1&nbsp;gives&nbsp;you&nbsp;a&nbsp;7x7<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;smoothing&nbsp;operator&nbsp;with&nbsp;Gaussian&nbsp;weighting.&nbsp;&nbsp;The&nbsp;default&nbsp;for<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;this&nbsp;parameter&nbsp;is&nbsp;1.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;max_iterations:&nbsp;Sets&nbsp;an&nbsp;upper&nbsp;limit&nbsp;on&nbsp;the&nbsp;number&nbsp;of&nbsp;iterations&nbsp;of&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;graph-based&nbsp;FH&nbsp;algorithm&nbsp;for&nbsp;image&nbsp;segmentation.<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;kay:&nbsp;This&nbsp;is&nbsp;the&nbsp;same&nbsp;as&nbsp;the&nbsp;"k"&nbsp;parameter&nbsp;in&nbsp;the&nbsp;FH&nbsp;algorithm.&nbsp;&nbsp;As<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;mentioned&nbsp;in&nbsp;the&nbsp;Introduction&nbsp;above,&nbsp;the&nbsp;Int(u)<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;property&nbsp;of&nbsp;the&nbsp;pixels&nbsp;represented&nbsp;by&nbsp;each&nbsp;vertex&nbsp;in<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;graph&nbsp;representation&nbsp;of&nbsp;the&nbsp;image&nbsp;is&nbsp;extended&nbsp;to<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MInt(u)&nbsp;by&nbsp;the&nbsp;addition&nbsp;of&nbsp;a&nbsp;number&nbsp;k/|C|&nbsp;where&nbsp;|C|&nbsp;is<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;cardinality&nbsp;of&nbsp;the&nbsp;set&nbsp;of&nbsp;pixels&nbsp;at&nbsp;that&nbsp;vertex.<br>
-&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;image_normalization_required:&nbsp;This&nbsp;applies&nbsp;Torchvision's&nbsp;image<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;normalization&nbsp;to&nbsp;the&nbsp;pixel&nbsp;values&nbsp;in&nbsp;the&nbsp;image.<br>
-&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;image_size_reduction_factor:&nbsp;As&nbsp;mentioned&nbsp;at&nbsp;the&nbsp;beginning&nbsp;of&nbsp;this<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;document,&nbsp;RegionProposalGenerator&nbsp;is&nbsp;really&nbsp;not&nbsp;meant<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;for&nbsp;production&nbsp;work.&nbsp;&nbsp;The&nbsp;code&nbsp;is&nbsp;pure&nbsp;Python&nbsp;and,&nbsp;even<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;with&nbsp;that,&nbsp;not&nbsp;at&nbsp;all&nbsp;optimized.&nbsp;&nbsp;The&nbsp;focus&nbsp;of&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;module&nbsp;is&nbsp;primarily&nbsp;on&nbsp;easy&nbsp;understandability&nbsp;of&nbsp;what<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;code&nbsp;is&nbsp;doing&nbsp;so&nbsp;that&nbsp;you&nbsp;can&nbsp;experiment&nbsp;with&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;algorithm&nbsp;itself.&nbsp;&nbsp;For&nbsp;the&nbsp;module&nbsp;to&nbsp;produce&nbsp;results<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;within&nbsp;a&nbsp;reasonable&nbsp;length&nbsp;of&nbsp;time,&nbsp;you&nbsp;can&nbsp;use&nbsp;this<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;constructor&nbsp;parameter&nbsp;to&nbsp;downsize&nbsp;the&nbsp;array&nbsp;of&nbsp;pixels<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;that&nbsp;the&nbsp;module&nbsp;must&nbsp;work&nbsp;with.&nbsp;&nbsp;Set&nbsp;this&nbsp;parameter&nbsp;to<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;a&nbsp;value&nbsp;so&nbsp;that&nbsp;the&nbsp;initial&nbsp;graph&nbsp;constructed&nbsp;from&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;image&nbsp;has&nbsp;no&nbsp;more&nbsp;than&nbsp;around&nbsp;3500&nbsp;vertices&nbsp;if&nbsp;you<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;don't&nbsp;want&nbsp;to&nbsp;wait&nbsp;too&nbsp;long&nbsp;for&nbsp;the&nbsp;results.<br>
-&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;min_size_for_graph_based_blobs:&nbsp;This&nbsp;declares&nbsp;a&nbsp;threshold&nbsp;on&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;smallest&nbsp;size&nbsp;you'd&nbsp;like&nbsp;to&nbsp;see&nbsp;(in&nbsp;terms&nbsp;of&nbsp;the&nbsp;number<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;pixels)&nbsp;in&nbsp;a&nbsp;segmented&nbsp;blob&nbsp;in&nbsp;the&nbsp;output&nbsp;of&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;graph-based&nbsp;segmenter.&nbsp;&nbsp;(I&nbsp;typically&nbsp;use&nbsp;values&nbsp;from&nbsp;1<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;to&nbsp;4&nbsp;for&nbsp;this&nbsp;parameter.)<br>
+&nbsp;&nbsp;&nbsp;&nbsp;kay:&nbsp;This&nbsp;is&nbsp;the&nbsp;same&nbsp;as&nbsp;the&nbsp;"k"&nbsp;parameter&nbsp;in&nbsp;the&nbsp;FH&nbsp;algorithm.&nbsp;&nbsp;As&nbsp;mentioned<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;the&nbsp;Introduction&nbsp;above,&nbsp;the&nbsp;Int(u)&nbsp;property&nbsp;of&nbsp;the&nbsp;pixels<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;represented&nbsp;by&nbsp;each&nbsp;vertex&nbsp;in&nbsp;the&nbsp;graph&nbsp;representation&nbsp;of&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;image&nbsp;is&nbsp;extended&nbsp;to&nbsp;MInt(u)&nbsp;by&nbsp;the&nbsp;addition&nbsp;of&nbsp;a&nbsp;number&nbsp;k/|C|<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;where&nbsp;|C|&nbsp;is&nbsp;the&nbsp;cardinality&nbsp;of&nbsp;the&nbsp;set&nbsp;of&nbsp;pixels&nbsp;at&nbsp;that<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;vertex.<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;image_normalization_required:&nbsp;This&nbsp;applies&nbsp;Torchvision's&nbsp;image&nbsp;normalization<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;to&nbsp;the&nbsp;pixel&nbsp;values&nbsp;in&nbsp;the&nbsp;image.<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;image_size_reduction_factor:&nbsp;As&nbsp;mentioned&nbsp;at&nbsp;the&nbsp;beginning&nbsp;of&nbsp;this&nbsp;document,<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;RegionProposalGenerator&nbsp;is&nbsp;really&nbsp;not&nbsp;meant&nbsp;for&nbsp;production<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;work.&nbsp;&nbsp;The&nbsp;code&nbsp;is&nbsp;pure&nbsp;Python&nbsp;and,&nbsp;even&nbsp;with&nbsp;that,&nbsp;not&nbsp;at&nbsp;all<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;optimized.&nbsp;&nbsp;The&nbsp;focus&nbsp;of&nbsp;the&nbsp;module&nbsp;is&nbsp;primarily&nbsp;on&nbsp;easy<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;understandability&nbsp;of&nbsp;what&nbsp;the&nbsp;code&nbsp;is&nbsp;doing&nbsp;so&nbsp;that&nbsp;you&nbsp;can<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;experiment&nbsp;with&nbsp;the&nbsp;algorithm&nbsp;itself.&nbsp;&nbsp;For&nbsp;the&nbsp;module&nbsp;to<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;produce&nbsp;results&nbsp;within&nbsp;a&nbsp;reasonable&nbsp;length&nbsp;of&nbsp;time,&nbsp;you&nbsp;can<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;use&nbsp;this&nbsp;constructor&nbsp;parameter&nbsp;to&nbsp;downsize&nbsp;the&nbsp;array&nbsp;of&nbsp;pixels<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;that&nbsp;the&nbsp;module&nbsp;must&nbsp;work&nbsp;with.&nbsp;&nbsp;Set&nbsp;this&nbsp;parameter&nbsp;to&nbsp;a&nbsp;value<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;so&nbsp;that&nbsp;the&nbsp;initial&nbsp;graph&nbsp;constructed&nbsp;from&nbsp;the&nbsp;image&nbsp;has&nbsp;no<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;more&nbsp;than&nbsp;around&nbsp;3500&nbsp;vertices&nbsp;if&nbsp;you&nbsp;don't&nbsp;want&nbsp;to&nbsp;wait&nbsp;too<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;long&nbsp;for&nbsp;the&nbsp;results.<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;min_size_for_graph_based_blobs:&nbsp;This&nbsp;declares&nbsp;a&nbsp;threshold&nbsp;on&nbsp;the&nbsp;smallest&nbsp;size<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;you'd&nbsp;like&nbsp;to&nbsp;see&nbsp;(in&nbsp;terms&nbsp;of&nbsp;the&nbsp;number&nbsp;of&nbsp;pixels)&nbsp;in&nbsp;a<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;segmented&nbsp;blob&nbsp;in&nbsp;the&nbsp;output&nbsp;of&nbsp;the&nbsp;graph-based&nbsp;segmenter.&nbsp;&nbsp;(I<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;typically&nbsp;use&nbsp;values&nbsp;from&nbsp;1&nbsp;to&nbsp;4&nbsp;for&nbsp;this&nbsp;parameter.)<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;color_homogeneity_thresh:&nbsp;&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;color_homogeneity_thresh:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;and&nbsp;the&nbsp;next&nbsp;three&nbsp;constructor&nbsp;options&nbsp;are&nbsp;meant<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;specifically&nbsp;for&nbsp;the&nbsp;SS&nbsp;algorithm&nbsp;that&nbsp;sits&nbsp;on&nbsp;top&nbsp;of<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;FH&nbsp;algorithm&nbsp;for&nbsp;further&nbsp;merging&nbsp;of&nbsp;the&nbsp;pixel&nbsp;blobs<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;produced&nbsp;by&nbsp;FH.&nbsp;&nbsp;This&nbsp;constructor&nbsp;option&nbsp;specifies&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;maximum&nbsp;allowable&nbsp;difference&nbsp;between&nbsp;the&nbsp;mean&nbsp;color<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;values&nbsp;in&nbsp;two&nbsp;pixel&nbsp;blobs&nbsp;for&nbsp;them&nbsp;to&nbsp;be&nbsp;merged.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;specifically&nbsp;for&nbsp;the&nbsp;SS&nbsp;algorithm&nbsp;that&nbsp;sits&nbsp;on&nbsp;top&nbsp;of&nbsp;the&nbsp;FH<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;algorithm&nbsp;for&nbsp;further&nbsp;merging&nbsp;of&nbsp;the&nbsp;pixel&nbsp;blobs&nbsp;produced&nbsp;by<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;FH.&nbsp;&nbsp;This&nbsp;constructor&nbsp;option&nbsp;specifies&nbsp;the&nbsp;maximum&nbsp;allowable<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;difference&nbsp;between&nbsp;the&nbsp;mean&nbsp;color&nbsp;values&nbsp;in&nbsp;two&nbsp;pixel&nbsp;blobs<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;for&nbsp;them&nbsp;to&nbsp;be&nbsp;merged.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;gray_var_thresh:<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;option&nbsp;declares&nbsp;the&nbsp;maximum&nbsp;allowable&nbsp;difference&nbsp;in&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;variances&nbsp;in&nbsp;the&nbsp;grayscale&nbsp;in&nbsp;two&nbsp;blobs&nbsp;if&nbsp;they&nbsp;are<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;to&nbsp;be&nbsp;merged.&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;option&nbsp;declares&nbsp;the&nbsp;maximum&nbsp;allowable&nbsp;difference&nbsp;in&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;variances&nbsp;in&nbsp;the&nbsp;grayscale&nbsp;in&nbsp;two&nbsp;blobs&nbsp;if&nbsp;they&nbsp;are&nbsp;to&nbsp;be<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;merged.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;texture_homogeneity_thresh:<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;RegionProposalGenerator&nbsp;module&nbsp;characterizes&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;texture&nbsp;of&nbsp;the&nbsp;pixels&nbsp;in&nbsp;each&nbsp;segmented&nbsp;blob&nbsp;by&nbsp;its&nbsp;LBP<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(Local&nbsp;Binary&nbsp;Patterns)&nbsp;texture.&nbsp;&nbsp;We&nbsp;want&nbsp;the&nbsp;LBP<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;texture&nbsp;values&nbsp;for&nbsp;two&nbsp;different&nbsp;blobs&nbsp;to&nbsp;be&nbsp;within&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;value&nbsp;specified&nbsp;by&nbsp;this&nbsp;constructor&nbsp;option&nbsp;if&nbsp;those<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;blobs&nbsp;are&nbsp;to&nbsp;be&nbsp;merged.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;RegionProposalGenerator&nbsp;module&nbsp;characterizes&nbsp;the&nbsp;texture&nbsp;of<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;pixels&nbsp;in&nbsp;each&nbsp;segmented&nbsp;blob&nbsp;by&nbsp;its&nbsp;LBP&nbsp;(Local&nbsp;Binary<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Patterns)&nbsp;texture.&nbsp;&nbsp;We&nbsp;want&nbsp;the&nbsp;LBP&nbsp;texture&nbsp;values&nbsp;for&nbsp;two<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;different&nbsp;blobs&nbsp;to&nbsp;be&nbsp;within&nbsp;the&nbsp;value&nbsp;specified&nbsp;by&nbsp;this<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;constructor&nbsp;option&nbsp;if&nbsp;those&nbsp;blobs&nbsp;are&nbsp;to&nbsp;be&nbsp;merged.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;max_num_blobs_expected:<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;If&nbsp;you&nbsp;only&nbsp;want&nbsp;to&nbsp;extract&nbsp;a&nbsp;certain&nbsp;number&nbsp;of&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;largest&nbsp;possible&nbsp;blobs,&nbsp;you&nbsp;can&nbsp;do&nbsp;that&nbsp;by&nbsp;giving&nbsp;a<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;value&nbsp;to&nbsp;this&nbsp;constructor&nbsp;option.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;If&nbsp;you&nbsp;only&nbsp;want&nbsp;to&nbsp;extract&nbsp;a&nbsp;certain&nbsp;number&nbsp;of&nbsp;the&nbsp;largest<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;possible&nbsp;blobs,&nbsp;you&nbsp;can&nbsp;do&nbsp;that&nbsp;by&nbsp;giving&nbsp;a&nbsp;value&nbsp;to&nbsp;this<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;constructor&nbsp;option.<br>
 &nbsp;<br>
 &nbsp;<br>
 <font size="+2" color="red">Inner&nbsp;Classes:<br>
 </font>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(1)&nbsp;&nbsp;PurdueDrEvalDataset<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;is&nbsp;the&nbsp;dataset&nbsp;to&nbsp;use&nbsp;if&nbsp;you&nbsp;are&nbsp;experimenting&nbsp;with<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;single-instance&nbsp;object&nbsp;detection.&nbsp;&nbsp;The&nbsp;dataset&nbsp;contains&nbsp;three<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;kinds&nbsp;of&nbsp;objects&nbsp;in&nbsp;its&nbsp;images:&nbsp;Dr.&nbsp;Eval,&nbsp;and&nbsp;two&nbsp;"objects"&nbsp;in&nbsp;his<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;neighborhood:&nbsp;a&nbsp;house&nbsp;and&nbsp;a&nbsp;watertower.&nbsp;&nbsp;Each&nbsp;128x128&nbsp;image&nbsp;in&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;dataset&nbsp;contains&nbsp;one&nbsp;of&nbsp;these&nbsp;objects&nbsp;after&nbsp;it&nbsp;is&nbsp;randomly&nbsp;scaled<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;and&nbsp;colored.&nbsp;Each&nbsp;image&nbsp;also&nbsp;contains&nbsp;substantial&nbsp;structured&nbsp;noise<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;addition&nbsp;to&nbsp;20%&nbsp;Gaussian&nbsp;noise.&nbsp;&nbsp;Examples&nbsp;of&nbsp;these&nbsp;images&nbsp;are<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;shown&nbsp;in&nbsp;the&nbsp;Week&nbsp;8&nbsp;lecture&nbsp;material&nbsp;in&nbsp;Purdue's&nbsp;Deep&nbsp;Learning<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;class.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;is&nbsp;the&nbsp;dataset&nbsp;to&nbsp;use&nbsp;if&nbsp;you&nbsp;are&nbsp;experimenting&nbsp;with&nbsp;single-instance<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;object&nbsp;detection.&nbsp;&nbsp;The&nbsp;dataset&nbsp;contains&nbsp;three&nbsp;kinds&nbsp;of&nbsp;objects&nbsp;in&nbsp;its<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;images:&nbsp;Dr.&nbsp;Eval,&nbsp;and&nbsp;two&nbsp;"objects"&nbsp;in&nbsp;his&nbsp;neighborhood:&nbsp;a&nbsp;house&nbsp;and&nbsp;a<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;watertower.&nbsp;&nbsp;Each&nbsp;128x128&nbsp;image&nbsp;in&nbsp;the&nbsp;dataset&nbsp;contains&nbsp;one&nbsp;of&nbsp;these<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;objects&nbsp;after&nbsp;it&nbsp;is&nbsp;randomly&nbsp;scaled&nbsp;and&nbsp;colored.&nbsp;Each&nbsp;image&nbsp;also&nbsp;contains<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;substantial&nbsp;structured&nbsp;noise&nbsp;in&nbsp;addition&nbsp;to&nbsp;20%&nbsp;Gaussian&nbsp;noise.&nbsp;&nbsp;Examples<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;these&nbsp;images&nbsp;are&nbsp;shown&nbsp;in&nbsp;the&nbsp;Week&nbsp;8&nbsp;lecture&nbsp;material&nbsp;in&nbsp;Purdue's&nbsp;Deep<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Learning&nbsp;class.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(2)&nbsp;&nbsp;PurdueDrEvalMultiDataset<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;is&nbsp;the&nbsp;dataset&nbsp;to&nbsp;use&nbsp;if&nbsp;you&nbsp;are&nbsp;experimenting&nbsp;with<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;multi-instance&nbsp;object&nbsp;detection.&nbsp;&nbsp;Each&nbsp;image&nbsp;in&nbsp;the&nbsp;dataset<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;contains&nbsp;randomly&nbsp;chosen&nbsp;multiple&nbsp;instances&nbsp;of&nbsp;the&nbsp;same&nbsp;three<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;kinds&nbsp;of&nbsp;objects&nbsp;as&nbsp;mentioned&nbsp;above:&nbsp;Dr.&nbsp;Eval,&nbsp;house,&nbsp;and<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;watertower.&nbsp;&nbsp;The&nbsp;number&nbsp;of&nbsp;object&nbsp;instances&nbsp;in&nbsp;each&nbsp;image&nbsp;is<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;limited&nbsp;to&nbsp;a&nbsp;maximum&nbsp;of&nbsp;five.&nbsp;&nbsp;The&nbsp;images&nbsp;contain&nbsp;substantial<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;is&nbsp;the&nbsp;dataset&nbsp;to&nbsp;use&nbsp;if&nbsp;you&nbsp;are&nbsp;experimenting&nbsp;with&nbsp;multi-instance<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;object&nbsp;detection.&nbsp;&nbsp;Each&nbsp;image&nbsp;in&nbsp;the&nbsp;dataset&nbsp;contains&nbsp;randomly&nbsp;chosen<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;multiple&nbsp;instances&nbsp;of&nbsp;the&nbsp;same&nbsp;three&nbsp;kinds&nbsp;of&nbsp;objects&nbsp;as&nbsp;mentioned&nbsp;above:<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Dr.&nbsp;Eval,&nbsp;house,&nbsp;and&nbsp;watertower.&nbsp;&nbsp;The&nbsp;number&nbsp;of&nbsp;object&nbsp;instances&nbsp;in&nbsp;each<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;image&nbsp;is&nbsp;limited&nbsp;to&nbsp;a&nbsp;maximum&nbsp;of&nbsp;five.&nbsp;&nbsp;The&nbsp;images&nbsp;contain&nbsp;substantial<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;amount&nbsp;of&nbsp;structured&nbsp;noise&nbsp;in&nbsp;addition&nbsp;to&nbsp;20%&nbsp;random&nbsp;noise.<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;reason&nbsp;for&nbsp;why&nbsp;the&nbsp;above&nbsp;two&nbsp;datasets&nbsp;have&nbsp;"DrEval"&nbsp;in&nbsp;their<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;names:&nbsp;After&nbsp;having&nbsp;watched&nbsp;every&nbsp;contemporary&nbsp;movie&nbsp;at&nbsp;Netflix<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;that&nbsp;was&nbsp;worth&nbsp;watching,&nbsp;my&nbsp;wife&nbsp;and&nbsp;I&nbsp;decided&nbsp;to&nbsp;revisit&nbsp;some&nbsp;of<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;old&nbsp;movies&nbsp;that&nbsp;we&nbsp;had&nbsp;enjoyed&nbsp;a&nbsp;long&nbsp;time&nbsp;back.&nbsp;&nbsp;That&nbsp;led&nbsp;us&nbsp;to<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;watching&nbsp;again&nbsp;a&nbsp;couple&nbsp;of&nbsp;Austin&nbsp;Powers&nbsp;movies.&nbsp;&nbsp;If&nbsp;you&nbsp;are&nbsp;too<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;young&nbsp;to&nbsp;know&nbsp;what&nbsp;I&nbsp;am&nbsp;talking&nbsp;about,&nbsp;these&nbsp;movies&nbsp;are&nbsp;spoofs&nbsp;on<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;James&nbsp;Bond&nbsp;movies&nbsp;in&nbsp;which&nbsp;the&nbsp;great&nbsp;comedian&nbsp;Mike&nbsp;Myers&nbsp;plays<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;both&nbsp;Austin&nbsp;Powers&nbsp;and&nbsp;his&nbsp;nemesis&nbsp;Dr.&nbsp;Evil.&nbsp;&nbsp;Around&nbsp;the&nbsp;same<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;time,&nbsp;I&nbsp;was&nbsp;writing&nbsp;code&nbsp;for&nbsp;the&nbsp;two&nbsp;datasets&nbsp;mentioned&nbsp;above.<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;One&nbsp;of&nbsp;the&nbsp;three&nbsp;objects&nbsp;types&nbsp;in&nbsp;these&nbsp;images&nbsp;is&nbsp;a&nbsp;human-like<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;cartoon&nbsp;figure&nbsp;that&nbsp;I&nbsp;needed&nbsp;a&nbsp;name&nbsp;for.&nbsp;&nbsp;So,&nbsp;after&nbsp;Dr.&nbsp;Evil&nbsp;in<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;movies,&nbsp;I&nbsp;decided&nbsp;to&nbsp;call&nbsp;this&nbsp;cartoon&nbsp;figure&nbsp;Dr&nbsp;Eval&nbsp;and&nbsp;to<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;refer&nbsp;to&nbsp;the&nbsp;datasets&nbsp;as&nbsp;Dr&nbsp;Eval&nbsp;datasets.&nbsp;As&nbsp;you&nbsp;all&nbsp;know,&nbsp;"Eval"<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;is&nbsp;an&nbsp;important&nbsp;word&nbsp;for&nbsp;people&nbsp;like&nbsp;us.&nbsp;&nbsp;All&nbsp;programming<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;languages&nbsp;provide&nbsp;a&nbsp;function&nbsp;with&nbsp;a&nbsp;name&nbsp;like&nbsp;"eval()".<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;reason&nbsp;for&nbsp;why&nbsp;the&nbsp;above&nbsp;two&nbsp;datasets&nbsp;have&nbsp;"DrEval"&nbsp;in&nbsp;their&nbsp;names:<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;After&nbsp;having&nbsp;watched&nbsp;every&nbsp;contemporary&nbsp;movie&nbsp;at&nbsp;Netflix&nbsp;that&nbsp;was&nbsp;worth<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;watching,&nbsp;my&nbsp;wife&nbsp;and&nbsp;I&nbsp;decided&nbsp;to&nbsp;revisit&nbsp;some&nbsp;of&nbsp;old&nbsp;movies&nbsp;that&nbsp;we&nbsp;had<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;enjoyed&nbsp;a&nbsp;long&nbsp;time&nbsp;back.&nbsp;&nbsp;That&nbsp;led&nbsp;us&nbsp;to&nbsp;watching&nbsp;again&nbsp;a&nbsp;couple&nbsp;of<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Austin&nbsp;Powers&nbsp;movies.&nbsp;&nbsp;If&nbsp;you&nbsp;are&nbsp;too&nbsp;young&nbsp;to&nbsp;know&nbsp;what&nbsp;I&nbsp;am&nbsp;talking<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;about,&nbsp;these&nbsp;movies&nbsp;are&nbsp;spoofs&nbsp;on&nbsp;the&nbsp;James&nbsp;Bond&nbsp;movies&nbsp;in&nbsp;which&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;great&nbsp;comedian&nbsp;Mike&nbsp;Myers&nbsp;plays&nbsp;both&nbsp;Austin&nbsp;Powers&nbsp;and&nbsp;his&nbsp;nemesis<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Dr.&nbsp;Evil.&nbsp;&nbsp;Around&nbsp;the&nbsp;same&nbsp;time,&nbsp;I&nbsp;was&nbsp;writing&nbsp;code&nbsp;for&nbsp;the&nbsp;two&nbsp;datasets<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;mentioned&nbsp;above.&nbsp;&nbsp;One&nbsp;of&nbsp;the&nbsp;three&nbsp;objects&nbsp;types&nbsp;in&nbsp;these&nbsp;images&nbsp;is&nbsp;a<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;human-like&nbsp;cartoon&nbsp;figure&nbsp;that&nbsp;I&nbsp;needed&nbsp;a&nbsp;name&nbsp;for.&nbsp;&nbsp;So,&nbsp;after&nbsp;Dr.&nbsp;Evil<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;the&nbsp;movies,&nbsp;I&nbsp;decided&nbsp;to&nbsp;call&nbsp;this&nbsp;cartoon&nbsp;figure&nbsp;Dr&nbsp;Eval&nbsp;and&nbsp;to&nbsp;refer<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;to&nbsp;the&nbsp;datasets&nbsp;as&nbsp;Dr&nbsp;Eval&nbsp;datasets.&nbsp;As&nbsp;you&nbsp;all&nbsp;know,&nbsp;"Eval"&nbsp;is&nbsp;an<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;important&nbsp;word&nbsp;for&nbsp;people&nbsp;like&nbsp;us.&nbsp;&nbsp;All&nbsp;programming&nbsp;languages&nbsp;provide&nbsp;a<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;function&nbsp;with&nbsp;a&nbsp;name&nbsp;like&nbsp;"eval()".<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(3)&nbsp;&nbsp;SingleInstanceDetector<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;provides&nbsp;a&nbsp;reference&nbsp;implementation&nbsp;for&nbsp;constructing&nbsp;a<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;single-instance&nbsp;object&nbsp;detector&nbsp;to&nbsp;be&nbsp;used&nbsp;for&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PurdueDrEvalDataset&nbsp;dataset.&nbsp;For&nbsp;the&nbsp;detection&nbsp;and&nbsp;regression<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;network,&nbsp;it&nbsp;uses&nbsp;the&nbsp;LOADnet2&nbsp;network&nbsp;from&nbsp;DLStudio&nbsp;with&nbsp;small<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;modifications&nbsp;to&nbsp;account&nbsp;for&nbsp;the&nbsp;larger&nbsp;128x128&nbsp;images&nbsp;in&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;dataset.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;single-instance&nbsp;object&nbsp;detector&nbsp;to&nbsp;be&nbsp;used&nbsp;for&nbsp;the&nbsp;PurdueDrEvalDataset<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;dataset.&nbsp;For&nbsp;the&nbsp;detection&nbsp;and&nbsp;regression&nbsp;network,&nbsp;it&nbsp;uses&nbsp;the&nbsp;LOADnet2<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;network&nbsp;from&nbsp;DLStudio&nbsp;with&nbsp;small&nbsp;modifications&nbsp;to&nbsp;account&nbsp;for&nbsp;the&nbsp;larger<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;128x128&nbsp;images&nbsp;in&nbsp;the&nbsp;dataset.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(4)&nbsp;&nbsp;YoloLikeDetector&nbsp;&nbsp;&nbsp;[For&nbsp;multi-instance&nbsp;detection]<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;code&nbsp;in&nbsp;this&nbsp;inner&nbsp;class&nbsp;provides&nbsp;an&nbsp;implementation&nbsp;for&nbsp;the&nbsp;key<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;elements&nbsp;of&nbsp;the&nbsp;YOLO&nbsp;logic&nbsp;for&nbsp;multi-instance&nbsp;object&nbsp;detection.&nbsp;&nbsp;Each<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;training&nbsp;image&nbsp;is&nbsp;divided&nbsp;into&nbsp;a&nbsp;grid&nbsp;of&nbsp;cells&nbsp;and&nbsp;it&nbsp;is&nbsp;the<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;responsibility&nbsp;of&nbsp;the&nbsp;cell&nbsp;that&nbsp;contains&nbsp;the&nbsp;center&nbsp;of&nbsp;an&nbsp;object<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;bounding-box&nbsp;to&nbsp;provide&nbsp;at&nbsp;the&nbsp;output&nbsp;of&nbsp;the&nbsp;neural&nbsp;network&nbsp;an<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;estimate&nbsp;for&nbsp;the&nbsp;exact&nbsp;location&nbsp;of&nbsp;the&nbsp;center&nbsp;of&nbsp;the&nbsp;object&nbsp;bounding<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;box&nbsp;vis-a-vis&nbsp;the&nbsp;center&nbsp;of&nbsp;the&nbsp;cell.&nbsp;&nbsp;That&nbsp;cell&nbsp;must&nbsp;also&nbsp;lead&nbsp;to&nbsp;an<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;estimate&nbsp;for&nbsp;the&nbsp;height&nbsp;and&nbsp;the&nbsp;width&nbsp;of&nbsp;the&nbsp;bounding-box&nbsp;for&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;object&nbsp;instance.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;bounding-box&nbsp;to&nbsp;provide&nbsp;at&nbsp;the&nbsp;output&nbsp;of&nbsp;the&nbsp;neural&nbsp;network&nbsp;an&nbsp;estimate<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;for&nbsp;the&nbsp;exact&nbsp;location&nbsp;of&nbsp;the&nbsp;center&nbsp;of&nbsp;the&nbsp;object&nbsp;bounding&nbsp;box&nbsp;vis-a-vis<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;center&nbsp;of&nbsp;the&nbsp;cell.&nbsp;&nbsp;That&nbsp;cell&nbsp;must&nbsp;also&nbsp;lead&nbsp;to&nbsp;an&nbsp;estimate&nbsp;for&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;height&nbsp;and&nbsp;the&nbsp;width&nbsp;of&nbsp;the&nbsp;bounding-box&nbsp;for&nbsp;the&nbsp;object&nbsp;instance.<br>
 &nbsp;<br>
 &nbsp;<br>
 <font size="+2" color="red">PUBLIC&nbsp;METHODS:<br>
 </font>&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Many&nbsp;of&nbsp;these&nbsp;method&nbsp;are&nbsp;related&nbsp;to&nbsp;using&nbsp;this&nbsp;module&nbsp;for&nbsp;experimenting<br>
-&nbsp;&nbsp;&nbsp;&nbsp;with&nbsp;the&nbsp;traditional&nbsp;graph-based&nbsp;algorithms&nbsp;for&nbsp;constructing&nbsp;region<br>
-&nbsp;&nbsp;&nbsp;&nbsp;proposals&nbsp;in&nbsp;images:<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Many&nbsp;of&nbsp;these&nbsp;method&nbsp;are&nbsp;related&nbsp;to&nbsp;using&nbsp;this&nbsp;module&nbsp;for&nbsp;experimenting&nbsp;with<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;traditional&nbsp;graph-based&nbsp;algorithms&nbsp;for&nbsp;constructing&nbsp;region&nbsp;proposals&nbsp;in<br>
+&nbsp;&nbsp;&nbsp;&nbsp;images:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(1)&nbsp;&nbsp;selective_search_for_region_proposals()<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;method&nbsp;implements&nbsp;elements&nbsp;of&nbsp;the&nbsp;Selective&nbsp;Search&nbsp;(SS)<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;algorithm&nbsp;proposed&nbsp;by&nbsp;Uijlings,&nbsp;van&nbsp;de&nbsp;Sande,&nbsp;Gevers,&nbsp;and&nbsp;Smeulders<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;for&nbsp;creating&nbsp;region&nbsp;proposals&nbsp;for&nbsp;object&nbsp;detection.&nbsp;&nbsp;As&nbsp;mentioned<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;elsewhere&nbsp;here,&nbsp;this&nbsp;algorithm&nbsp;sits&nbsp;on&nbsp;top&nbsp;of&nbsp;the&nbsp;graph&nbsp;based&nbsp;image<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;segmentation&nbsp;algorithm&nbsp;that&nbsp;was&nbsp;proposed&nbsp;by&nbsp;Felzenszwalb&nbsp;and<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Huttenlocher.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;method&nbsp;implements&nbsp;elements&nbsp;of&nbsp;the&nbsp;Selective&nbsp;Search&nbsp;(SS)&nbsp;algorithm<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;proposed&nbsp;by&nbsp;Uijlings,&nbsp;van&nbsp;de&nbsp;Sande,&nbsp;Gevers,&nbsp;and&nbsp;Smeulders&nbsp;for&nbsp;creating<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;region&nbsp;proposals&nbsp;for&nbsp;object&nbsp;detection.&nbsp;&nbsp;As&nbsp;mentioned&nbsp;elsewhere&nbsp;here,&nbsp;this<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;algorithm&nbsp;sits&nbsp;on&nbsp;top&nbsp;of&nbsp;the&nbsp;graph&nbsp;based&nbsp;image&nbsp;segmentation&nbsp;algorithm<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;that&nbsp;was&nbsp;proposed&nbsp;by&nbsp;Felzenszwalb&nbsp;and&nbsp;Huttenlocher.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(2)&nbsp;&nbsp;graph_based_segmentation()<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;is&nbsp;an&nbsp;implementation&nbsp;of&nbsp;the&nbsp;Felzenszwalb&nbsp;and&nbsp;Huttenlocher&nbsp;(FH)<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;algorithm&nbsp;for&nbsp;graph-based&nbsp;segmentation&nbsp;of&nbsp;images.&nbsp;&nbsp;At&nbsp;the&nbsp;moment,&nbsp;it<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;is&nbsp;limited&nbsp;to&nbsp;working&nbsp;on&nbsp;grayscale&nbsp;images.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;algorithm&nbsp;for&nbsp;graph-based&nbsp;segmentation&nbsp;of&nbsp;images.&nbsp;&nbsp;At&nbsp;the&nbsp;moment,&nbsp;it&nbsp;is<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;limited&nbsp;to&nbsp;working&nbsp;on&nbsp;grayscale&nbsp;images.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(3)&nbsp;&nbsp;display_tensor_as_image()<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;method&nbsp;converts&nbsp;the&nbsp;argument&nbsp;tensor&nbsp;into&nbsp;a&nbsp;photo&nbsp;image&nbsp;that&nbsp;you<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;can&nbsp;display&nbsp;in&nbsp;your&nbsp;terminal&nbsp;screen.&nbsp;It&nbsp;can&nbsp;convert&nbsp;tensors&nbsp;of&nbsp;three<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;different&nbsp;shapes&nbsp;into&nbsp;images:&nbsp;(3,H,W),&nbsp;(1,H,W),&nbsp;and&nbsp;(H,W),&nbsp;where&nbsp;H,<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;for&nbsp;height,&nbsp;stands&nbsp;for&nbsp;the&nbsp;number&nbsp;of&nbsp;pixel&nbsp;in&nbsp;the&nbsp;vertical&nbsp;direction<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;and&nbsp;W,&nbsp;for&nbsp;width,&nbsp;the&nbsp;same&nbsp;along&nbsp;the&nbsp;horizontal&nbsp;direction.&nbsp;When&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;first&nbsp;element&nbsp;of&nbsp;the&nbsp;shape&nbsp;is&nbsp;3,&nbsp;that&nbsp;means&nbsp;that&nbsp;the&nbsp;tensor<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;represents&nbsp;a&nbsp;color&nbsp;image&nbsp;in&nbsp;which&nbsp;each&nbsp;pixel&nbsp;in&nbsp;the&nbsp;(H,W)&nbsp;plane&nbsp;has<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;three&nbsp;values&nbsp;for&nbsp;the&nbsp;three&nbsp;color&nbsp;channels.&nbsp;&nbsp;On&nbsp;the&nbsp;other&nbsp;hand,&nbsp;when<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;first&nbsp;element&nbsp;is&nbsp;1,&nbsp;that&nbsp;stands&nbsp;for&nbsp;a&nbsp;tensor&nbsp;that&nbsp;will&nbsp;be&nbsp;shown<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;as&nbsp;a&nbsp;grayscale&nbsp;image.&nbsp;&nbsp;And&nbsp;when&nbsp;the&nbsp;shape&nbsp;is&nbsp;just&nbsp;(H,W),&nbsp;that&nbsp;is<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;automatically&nbsp;taken&nbsp;to&nbsp;be&nbsp;for&nbsp;a&nbsp;grayscale&nbsp;image.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;method&nbsp;converts&nbsp;the&nbsp;argument&nbsp;tensor&nbsp;into&nbsp;a&nbsp;photo&nbsp;image&nbsp;that&nbsp;you&nbsp;can<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;display&nbsp;in&nbsp;your&nbsp;terminal&nbsp;screen.&nbsp;It&nbsp;can&nbsp;convert&nbsp;tensors&nbsp;of&nbsp;three<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;different&nbsp;shapes&nbsp;into&nbsp;images:&nbsp;(3,H,W),&nbsp;(1,H,W),&nbsp;and&nbsp;(H,W),&nbsp;where&nbsp;H,&nbsp;for<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;height,&nbsp;stands&nbsp;for&nbsp;the&nbsp;number&nbsp;of&nbsp;pixel&nbsp;in&nbsp;the&nbsp;vertical&nbsp;direction&nbsp;and&nbsp;W,<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;for&nbsp;width,&nbsp;the&nbsp;same&nbsp;along&nbsp;the&nbsp;horizontal&nbsp;direction.&nbsp;When&nbsp;the&nbsp;first<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;element&nbsp;of&nbsp;the&nbsp;shape&nbsp;is&nbsp;3,&nbsp;that&nbsp;means&nbsp;that&nbsp;the&nbsp;tensor&nbsp;represents&nbsp;a&nbsp;color<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;image&nbsp;in&nbsp;which&nbsp;each&nbsp;pixel&nbsp;in&nbsp;the&nbsp;(H,W)&nbsp;plane&nbsp;has&nbsp;three&nbsp;values&nbsp;for&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;three&nbsp;color&nbsp;channels.&nbsp;&nbsp;On&nbsp;the&nbsp;other&nbsp;hand,&nbsp;when&nbsp;the&nbsp;first&nbsp;element&nbsp;is&nbsp;1,<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;that&nbsp;stands&nbsp;for&nbsp;a&nbsp;tensor&nbsp;that&nbsp;will&nbsp;be&nbsp;shown&nbsp;as&nbsp;a&nbsp;grayscale&nbsp;image.&nbsp;&nbsp;And<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;when&nbsp;the&nbsp;shape&nbsp;is&nbsp;just&nbsp;(H,W),&nbsp;that&nbsp;is&nbsp;automatically&nbsp;taken&nbsp;to&nbsp;be&nbsp;for&nbsp;a<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;grayscale&nbsp;image.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(4)&nbsp;&nbsp;graying_resizing_binarizing()<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;is&nbsp;a&nbsp;demonstration&nbsp;of&nbsp;some&nbsp;of&nbsp;the&nbsp;more&nbsp;basic&nbsp;and&nbsp;commonly&nbsp;used<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;image&nbsp;transformations&nbsp;from&nbsp;the&nbsp;torchvision.transformations&nbsp;module.<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;large&nbsp;comment&nbsp;blocks&nbsp;are&nbsp;meant&nbsp;to&nbsp;serve&nbsp;as&nbsp;tutorial&nbsp;introduction<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;to&nbsp;the&nbsp;syntax&nbsp;used&nbsp;for&nbsp;invoking&nbsp;these&nbsp;transformations.&nbsp;&nbsp;The<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;transformations&nbsp;shown&nbsp;can&nbsp;be&nbsp;used&nbsp;for&nbsp;converting&nbsp;a&nbsp;color&nbsp;image&nbsp;into&nbsp;a<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;grayscale&nbsp;image,&nbsp;for&nbsp;resizing&nbsp;an&nbsp;image,&nbsp;for&nbsp;converting&nbsp;a&nbsp;PIL.Image<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;into&nbsp;a&nbsp;tensor&nbsp;and&nbsp;a&nbsp;tensor&nbsp;back&nbsp;into&nbsp;an&nbsp;PIL.Image&nbsp;object,&nbsp;and&nbsp;so&nbsp;on.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;is&nbsp;a&nbsp;demonstration&nbsp;of&nbsp;some&nbsp;of&nbsp;the&nbsp;more&nbsp;basic&nbsp;and&nbsp;commonly&nbsp;used&nbsp;image<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;transformations&nbsp;from&nbsp;the&nbsp;torchvision.transformations&nbsp;module.&nbsp;&nbsp;The&nbsp;large<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;comment&nbsp;blocks&nbsp;are&nbsp;meant&nbsp;to&nbsp;serve&nbsp;as&nbsp;tutorial&nbsp;introduction&nbsp;to&nbsp;the&nbsp;syntax<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;used&nbsp;for&nbsp;invoking&nbsp;these&nbsp;transformations.&nbsp;&nbsp;The&nbsp;transformations&nbsp;shown&nbsp;can<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;be&nbsp;used&nbsp;for&nbsp;converting&nbsp;a&nbsp;color&nbsp;image&nbsp;into&nbsp;a&nbsp;grayscale&nbsp;image,&nbsp;for&nbsp;resizing<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;an&nbsp;image,&nbsp;for&nbsp;converting&nbsp;a&nbsp;PIL.Image&nbsp;into&nbsp;a&nbsp;tensor&nbsp;and&nbsp;a&nbsp;tensor&nbsp;back&nbsp;into<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;an&nbsp;PIL.Image&nbsp;object,&nbsp;and&nbsp;so&nbsp;on.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(5)&nbsp;&nbsp;accessing_one_color_plane()<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;method&nbsp;shows&nbsp;how&nbsp;can&nbsp;access&nbsp;the&nbsp;n-th&nbsp;color&nbsp;plane&nbsp;of&nbsp;the&nbsp;argument<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;color&nbsp;image.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(6)&nbsp;&nbsp;working_with_hsv_color_space()<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Illustrates&nbsp;converting&nbsp;an&nbsp;RGB&nbsp;color&nbsp;image&nbsp;into&nbsp;its&nbsp;HSV<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;representation.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Illustrates&nbsp;converting&nbsp;an&nbsp;RGB&nbsp;color&nbsp;image&nbsp;into&nbsp;its&nbsp;HSV&nbsp;representation.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(7)&nbsp;&nbsp;histogramming_the_image()<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PyTorch&nbsp;based&nbsp;experiments&nbsp;with&nbsp;histogramming&nbsp;the&nbsp;grayscale&nbsp;and&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;color&nbsp;values&nbsp;in&nbsp;an&nbsp;image<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;PyTorch&nbsp;based&nbsp;experiments&nbsp;with&nbsp;histogramming&nbsp;the&nbsp;grayscale&nbsp;and&nbsp;the&nbsp;color<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;values&nbsp;in&nbsp;an&nbsp;image<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(8)&nbsp;&nbsp;histogramming_and_thresholding():<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;method&nbsp;illustrates&nbsp;using&nbsp;the&nbsp;PyTorch&nbsp;functionality&nbsp;for<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;histogramming&nbsp;and&nbsp;thresholding&nbsp;individual&nbsp;images.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;method&nbsp;illustrates&nbsp;using&nbsp;the&nbsp;PyTorch&nbsp;functionality&nbsp;for&nbsp;histogramming<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;and&nbsp;thresholding&nbsp;individual&nbsp;images.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(9)&nbsp;&nbsp;convolutions_with_pytorch()<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;method&nbsp;calls&nbsp;on&nbsp;torch.nn.functional.conv2d()&nbsp;for&nbsp;demonstrating&nbsp;a<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;single&nbsp;image&nbsp;convolution&nbsp;with&nbsp;a&nbsp;specified&nbsp;kernel.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(10)&nbsp;gaussian_smooth()<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;method&nbsp;smooths&nbsp;an&nbsp;image&nbsp;with&nbsp;a&nbsp;Gaussian&nbsp;of&nbsp;specified&nbsp;sigma.&nbsp;&nbsp;You<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;can&nbsp;do&nbsp;the&nbsp;same&nbsp;much&nbsp;faster&nbsp;by&nbsp;using&nbsp;the&nbsp;functionality&nbsp;programmed<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;into&nbsp;torch.nn.functional.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;method&nbsp;smooths&nbsp;an&nbsp;image&nbsp;with&nbsp;a&nbsp;Gaussian&nbsp;of&nbsp;specified&nbsp;sigma.&nbsp;&nbsp;You&nbsp;can<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;do&nbsp;the&nbsp;same&nbsp;much&nbsp;faster&nbsp;by&nbsp;using&nbsp;the&nbsp;functionality&nbsp;programmed&nbsp;into<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;torch.nn.functional.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(11)&nbsp;visualize_segmentation_in_pseudocolor()<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;After&nbsp;an&nbsp;image&nbsp;has&nbsp;been&nbsp;segmented,&nbsp;this&nbsp;method&nbsp;can&nbsp;be&nbsp;used&nbsp;to&nbsp;assign<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;a&nbsp;random&nbsp;color&nbsp;to&nbsp;each&nbsp;blob&nbsp;in&nbsp;the&nbsp;segmented&nbsp;output&nbsp;for&nbsp;a&nbsp;better<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;After&nbsp;an&nbsp;image&nbsp;has&nbsp;been&nbsp;segmented,&nbsp;this&nbsp;method&nbsp;can&nbsp;be&nbsp;used&nbsp;to&nbsp;assign&nbsp;a<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;random&nbsp;color&nbsp;to&nbsp;each&nbsp;blob&nbsp;in&nbsp;the&nbsp;segmented&nbsp;output&nbsp;for&nbsp;a&nbsp;better<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;visualization&nbsp;of&nbsp;the&nbsp;segmentation.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(12)&nbsp;visualize_segmentation_with_mean_gray()<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;If&nbsp;the&nbsp;visualization&nbsp;produced&nbsp;by&nbsp;the&nbsp;previous&nbsp;method&nbsp;appears&nbsp;too<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;chaotic,&nbsp;you&nbsp;can&nbsp;use&nbsp;this&nbsp;method&nbsp;to&nbsp;assign&nbsp;the&nbsp;mean&nbsp;color&nbsp;to&nbsp;each<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;each&nbsp;blob&nbsp;in&nbsp;the&nbsp;output&nbsp;of&nbsp;an&nbsp;image&nbsp;segmentation&nbsp;algorithm.&nbsp;&nbsp;The&nbsp;mean<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;color&nbsp;is&nbsp;derived&nbsp;from&nbsp;the&nbsp;pixel&nbsp;values&nbsp;in&nbsp;the&nbsp;blob.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;If&nbsp;the&nbsp;visualization&nbsp;produced&nbsp;by&nbsp;the&nbsp;previous&nbsp;method&nbsp;appears&nbsp;too&nbsp;chaotic,<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;you&nbsp;can&nbsp;use&nbsp;this&nbsp;method&nbsp;to&nbsp;assign&nbsp;the&nbsp;mean&nbsp;color&nbsp;to&nbsp;each&nbsp;each&nbsp;blob&nbsp;in&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;output&nbsp;of&nbsp;an&nbsp;image&nbsp;segmentation&nbsp;algorithm.&nbsp;&nbsp;The&nbsp;mean&nbsp;color&nbsp;is&nbsp;derived<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;from&nbsp;the&nbsp;pixel&nbsp;values&nbsp;in&nbsp;the&nbsp;blob.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(13)&nbsp;extract_image_region_interactively_by_dragging_mouse()<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;You&nbsp;can&nbsp;use&nbsp;this&nbsp;method&nbsp;to&nbsp;apply&nbsp;the&nbsp;graph-based&nbsp;segmentation&nbsp;and&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;selective&nbsp;search&nbsp;algorithms&nbsp;to&nbsp;just&nbsp;a&nbsp;portion&nbsp;of&nbsp;your&nbsp;image.&nbsp;&nbsp;This<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;method&nbsp;extract&nbsp;the&nbsp;portion&nbsp;you&nbsp;want.&nbsp;&nbsp;You&nbsp;click&nbsp;at&nbsp;the&nbsp;upper&nbsp;left<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;corner&nbsp;of&nbsp;the&nbsp;rectangular&nbsp;portion&nbsp;of&nbsp;the&nbsp;image&nbsp;you&nbsp;are&nbsp;interested&nbsp;in<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;and&nbsp;you&nbsp;then&nbsp;drag&nbsp;the&nbsp;mouse&nbsp;pointer&nbsp;to&nbsp;the&nbsp;lower&nbsp;right&nbsp;corner.&nbsp;&nbsp;Make<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;sure&nbsp;that&nbsp;you&nbsp;click&nbsp;on&nbsp;"save"&nbsp;and&nbsp;"exit"&nbsp;after&nbsp;you&nbsp;have&nbsp;delineated<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;area.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;selective&nbsp;search&nbsp;algorithms&nbsp;to&nbsp;just&nbsp;a&nbsp;portion&nbsp;of&nbsp;your&nbsp;image.&nbsp;&nbsp;This&nbsp;method<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;extract&nbsp;the&nbsp;portion&nbsp;you&nbsp;want.&nbsp;&nbsp;You&nbsp;click&nbsp;at&nbsp;the&nbsp;upper&nbsp;left&nbsp;corner&nbsp;of&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;rectangular&nbsp;portion&nbsp;of&nbsp;the&nbsp;image&nbsp;you&nbsp;are&nbsp;interested&nbsp;in&nbsp;and&nbsp;you&nbsp;then&nbsp;drag<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;mouse&nbsp;pointer&nbsp;to&nbsp;the&nbsp;lower&nbsp;right&nbsp;corner.&nbsp;&nbsp;Make&nbsp;sure&nbsp;that&nbsp;you&nbsp;click&nbsp;on<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"save"&nbsp;and&nbsp;"exit"&nbsp;after&nbsp;you&nbsp;have&nbsp;delineated&nbsp;the&nbsp;area.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(14)&nbsp;extract_image_region_interactively_through_mouse_clicks()<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;method&nbsp;allows&nbsp;a&nbsp;user&nbsp;to&nbsp;use&nbsp;a&nbsp;sequence&nbsp;of&nbsp;mouse&nbsp;clicks&nbsp;in&nbsp;order<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;to&nbsp;specify&nbsp;a&nbsp;region&nbsp;of&nbsp;the&nbsp;input&nbsp;image&nbsp;that&nbsp;should&nbsp;be&nbsp;subject&nbsp;to<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;further&nbsp;processing.&nbsp;&nbsp;The&nbsp;mouse&nbsp;clicks&nbsp;taken&nbsp;together&nbsp;define&nbsp;a<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;polygon.&nbsp;The&nbsp;method&nbsp;encloses&nbsp;the&nbsp;polygonal&nbsp;region&nbsp;by&nbsp;a&nbsp;minimum<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;bounding&nbsp;rectangle,&nbsp;which&nbsp;then&nbsp;becomes&nbsp;the&nbsp;new&nbsp;input&nbsp;image&nbsp;for&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;rest&nbsp;of&nbsp;processing.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;method&nbsp;allows&nbsp;a&nbsp;user&nbsp;to&nbsp;use&nbsp;a&nbsp;sequence&nbsp;of&nbsp;mouse&nbsp;clicks&nbsp;in&nbsp;order&nbsp;to<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;specify&nbsp;a&nbsp;region&nbsp;of&nbsp;the&nbsp;input&nbsp;image&nbsp;that&nbsp;should&nbsp;be&nbsp;subject&nbsp;to&nbsp;further<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;processing.&nbsp;&nbsp;The&nbsp;mouse&nbsp;clicks&nbsp;taken&nbsp;together&nbsp;define&nbsp;a&nbsp;polygon.&nbsp;The&nbsp;method<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;encloses&nbsp;the&nbsp;polygonal&nbsp;region&nbsp;by&nbsp;a&nbsp;minimum&nbsp;bounding&nbsp;rectangle,&nbsp;which&nbsp;then<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;becomes&nbsp;the&nbsp;new&nbsp;input&nbsp;image&nbsp;for&nbsp;the&nbsp;rest&nbsp;of&nbsp;processing.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(15)&nbsp;displaying_and_histogramming_images_in_batch1(image_dir,&nbsp;batch_size)<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;method&nbsp;is&nbsp;the&nbsp;first&nbsp;of&nbsp;three&nbsp;such&nbsp;methods&nbsp;in&nbsp;this&nbsp;module&nbsp;for<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;illustrating&nbsp;the&nbsp;functionality&nbsp;of&nbsp;matplotlib&nbsp;for&nbsp;simultaneously<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;displaying&nbsp;multiple&nbsp;images&nbsp;and&nbsp;the&nbsp;results&nbsp;obtained&nbsp;from&nbsp;them&nbsp;in&nbsp;a<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;gridded&nbsp;arrangement.&nbsp;&nbsp;The&nbsp;core&nbsp;idea&nbsp;in&nbsp;this&nbsp;method&nbsp;is&nbsp;to&nbsp;call<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"plt.subplots(2,batch_size)"&nbsp;to&nbsp;create&nbsp;'batch_size'&nbsp;number&nbsp;of&nbsp;subplot<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;objects,&nbsp;called&nbsp;"axes",&nbsp;in&nbsp;the&nbsp;form&nbsp;of&nbsp;a&nbsp;'2xbatch_size'&nbsp;array.&nbsp;We&nbsp;use<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;first&nbsp;row&nbsp;of&nbsp;this&nbsp;grid&nbsp;to&nbsp;display&nbsp;each&nbsp;image&nbsp;in&nbsp;its&nbsp;own&nbsp;subplot<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;object.&nbsp;&nbsp;And&nbsp;we&nbsp;use&nbsp;the&nbsp;second&nbsp;row&nbsp;of&nbsp;the&nbsp;grid&nbsp;to&nbsp;display&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;histograms&nbsp;of&nbsp;the&nbsp;corresponding&nbsp;images&nbsp;in&nbsp;the&nbsp;first&nbsp;row.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;objects,&nbsp;called&nbsp;"axes",&nbsp;in&nbsp;the&nbsp;form&nbsp;of&nbsp;a&nbsp;'2xbatch_size'&nbsp;array.&nbsp;We&nbsp;use&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;first&nbsp;row&nbsp;of&nbsp;this&nbsp;grid&nbsp;to&nbsp;display&nbsp;each&nbsp;image&nbsp;in&nbsp;its&nbsp;own&nbsp;subplot&nbsp;object.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;And&nbsp;we&nbsp;use&nbsp;the&nbsp;second&nbsp;row&nbsp;of&nbsp;the&nbsp;grid&nbsp;to&nbsp;display&nbsp;the&nbsp;histograms&nbsp;of&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;corresponding&nbsp;images&nbsp;in&nbsp;the&nbsp;first&nbsp;row.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(16)&nbsp;displaying_and_histogramming_images_in_batch2(image_dir,&nbsp;batch_size)<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;I&nbsp;now&nbsp;show&nbsp;a&nbsp;second&nbsp;approach&nbsp;to&nbsp;displaying&nbsp;multiple&nbsp;images&nbsp;and&nbsp;their<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;corresponding&nbsp;histograms&nbsp;in&nbsp;a&nbsp;gridded&nbsp;display.&nbsp;&nbsp;In&nbsp;this&nbsp;method&nbsp;we<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;call&nbsp;on&nbsp;"torchvision.utils.make_grid()"&nbsp;to&nbsp;construct&nbsp;a&nbsp;grid&nbsp;for&nbsp;us.<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;grid&nbsp;is&nbsp;created&nbsp;by&nbsp;giving&nbsp;an&nbsp;argument&nbsp;like&nbsp;"nrow=4"&nbsp;to&nbsp;it.&nbsp;&nbsp;The<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;grid&nbsp;object&nbsp;returned&nbsp;by&nbsp;the&nbsp;call&nbsp;to&nbsp;make_grid()&nbsp;is&nbsp;a&nbsp;tensor&nbsp;unto<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;itself.&nbsp;Such&nbsp;a&nbsp;tensor&nbsp;object&nbsp;is&nbsp;converted&nbsp;into&nbsp;a&nbsp;numpy&nbsp;array&nbsp;so&nbsp;that<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;it&nbsp;can&nbsp;be&nbsp;displayed&nbsp;by&nbsp;matplotlib's&nbsp;"imshow()"&nbsp;function.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;corresponding&nbsp;histograms&nbsp;in&nbsp;a&nbsp;gridded&nbsp;display.&nbsp;&nbsp;In&nbsp;this&nbsp;method&nbsp;we&nbsp;call&nbsp;on<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"torchvision.utils.make_grid()"&nbsp;to&nbsp;construct&nbsp;a&nbsp;grid&nbsp;for&nbsp;us.&nbsp;&nbsp;The&nbsp;grid&nbsp;is<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;created&nbsp;by&nbsp;giving&nbsp;an&nbsp;argument&nbsp;like&nbsp;"nrow=4"&nbsp;to&nbsp;it.&nbsp;&nbsp;The&nbsp;grid&nbsp;object<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;returned&nbsp;by&nbsp;the&nbsp;call&nbsp;to&nbsp;make_grid()&nbsp;is&nbsp;a&nbsp;tensor&nbsp;unto&nbsp;itself.&nbsp;Such&nbsp;a<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;tensor&nbsp;object&nbsp;is&nbsp;converted&nbsp;into&nbsp;a&nbsp;numpy&nbsp;array&nbsp;so&nbsp;that&nbsp;it&nbsp;can&nbsp;be&nbsp;displayed<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;by&nbsp;matplotlib's&nbsp;"imshow()"&nbsp;function.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;(17)&nbsp;displaying_and_histogramming_images_in_batch3(image_dir,&nbsp;batch_size)<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;method&nbsp;illustrates&nbsp;two&nbsp;things:&nbsp;(1)&nbsp;The&nbsp;syntax&nbsp;used&nbsp;for&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;'singular'&nbsp;version&nbsp;of&nbsp;the&nbsp;subplot&nbsp;function&nbsp;"plt.subplot()"&nbsp;---<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;although&nbsp;I'll&nbsp;be&nbsp;doing&nbsp;so&nbsp;by&nbsp;actually&nbsp;calling&nbsp;"fig.add_subplot()".<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;And&nbsp;(2)&nbsp;How&nbsp;you&nbsp;can&nbsp;put&nbsp;together&nbsp;multiple&nbsp;multi-image&nbsp;plots&nbsp;by<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;creating&nbsp;multiple&nbsp;Figure&nbsp;objects.&nbsp;&nbsp;'Figure'&nbsp;is&nbsp;the&nbsp;top-level<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;container&nbsp;of&nbsp;plots&nbsp;in&nbsp;matplotlib.&nbsp;&nbsp;This&nbsp;method&nbsp;creates&nbsp;two&nbsp;separate<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Figure&nbsp;objects,&nbsp;one&nbsp;as&nbsp;a&nbsp;container&nbsp;for&nbsp;all&nbsp;the&nbsp;images&nbsp;in&nbsp;a&nbsp;batch&nbsp;and<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;other&nbsp;as&nbsp;a&nbsp;container&nbsp;for&nbsp;all&nbsp;the&nbsp;histograms&nbsp;for&nbsp;the&nbsp;images.&nbsp;&nbsp;The<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;two&nbsp;Figure&nbsp;containers&nbsp;are&nbsp;displayed&nbsp;in&nbsp;two&nbsp;separate&nbsp;windows&nbsp;on&nbsp;your<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;computer&nbsp;screen.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;'singular'&nbsp;version&nbsp;of&nbsp;the&nbsp;subplot&nbsp;function&nbsp;"plt.subplot()"&nbsp;---&nbsp;although<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;I'll&nbsp;be&nbsp;doing&nbsp;so&nbsp;by&nbsp;actually&nbsp;calling&nbsp;"fig.add_subplot()".&nbsp;&nbsp;And&nbsp;(2)&nbsp;How<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;you&nbsp;can&nbsp;put&nbsp;together&nbsp;multiple&nbsp;multi-image&nbsp;plots&nbsp;by&nbsp;creating&nbsp;multiple<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Figure&nbsp;objects.&nbsp;&nbsp;'Figure'&nbsp;is&nbsp;the&nbsp;top-level&nbsp;container&nbsp;of&nbsp;plots&nbsp;in<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;matplotlib.&nbsp;&nbsp;This&nbsp;method&nbsp;creates&nbsp;two&nbsp;separate&nbsp;Figure&nbsp;objects,&nbsp;one&nbsp;as&nbsp;a<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;container&nbsp;for&nbsp;all&nbsp;the&nbsp;images&nbsp;in&nbsp;a&nbsp;batch&nbsp;and&nbsp;the&nbsp;other&nbsp;as&nbsp;a&nbsp;container&nbsp;for<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;all&nbsp;the&nbsp;histograms&nbsp;for&nbsp;the&nbsp;images.&nbsp;&nbsp;The&nbsp;two&nbsp;Figure&nbsp;containers&nbsp;are<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;displayed&nbsp;in&nbsp;two&nbsp;separate&nbsp;windows&nbsp;on&nbsp;your&nbsp;computer&nbsp;screen.<br>
+&nbsp;<br>
 &nbsp;<br>
 <font size="+2" color="red">THE&nbsp;DATASETS&nbsp;INCLUDED:<br>
 </font>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Download&nbsp;the&nbsp;archive<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;datasets_for_RPG.tar.gz<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;through&nbsp;the&nbsp;link&nbsp;"Download&nbsp;the&nbsp;image&nbsp;datasets&nbsp;for&nbsp;RPG"&nbsp;at&nbsp;the&nbsp;main<br>
-&nbsp;&nbsp;&nbsp;&nbsp;webpage&nbsp;for&nbsp;this&nbsp;module&nbsp;and&nbsp;store&nbsp;the&nbsp;archive&nbsp;in&nbsp;the&nbsp;Examples&nbsp;directory<br>
-&nbsp;&nbsp;&nbsp;&nbsp;of&nbsp;your&nbsp;install&nbsp;of&nbsp;the&nbsp;module.&nbsp;Subsequently,&nbsp;execute&nbsp;the&nbsp;following<br>
-&nbsp;&nbsp;&nbsp;&nbsp;command&nbsp;in&nbsp;the&nbsp;Examples&nbsp;directory:<br>
+&nbsp;&nbsp;&nbsp;&nbsp;through&nbsp;the&nbsp;link&nbsp;"Download&nbsp;the&nbsp;image&nbsp;datasets&nbsp;for&nbsp;RPG"&nbsp;at&nbsp;the&nbsp;main&nbsp;webpage&nbsp;for<br>
+&nbsp;&nbsp;&nbsp;&nbsp;this&nbsp;module&nbsp;and&nbsp;store&nbsp;the&nbsp;archive&nbsp;in&nbsp;the&nbsp;ExamplesObjectDetection&nbsp;directory&nbsp;of<br>
+&nbsp;&nbsp;&nbsp;&nbsp;your&nbsp;install&nbsp;of&nbsp;the&nbsp;module.&nbsp;Subsequently,&nbsp;execute&nbsp;the&nbsp;following&nbsp;command&nbsp;in&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;ExamplesObjectDetection&nbsp;directory:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;tar&nbsp;zxvf&nbsp;datasets_for_RPG.tar.gz<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;command&nbsp;will&nbsp;create&nbsp;a&nbsp;'data'&nbsp;subdirectory&nbsp;in&nbsp;the&nbsp;Examples&nbsp;directory<br>
-&nbsp;&nbsp;&nbsp;&nbsp;and&nbsp;deposit&nbsp;the&nbsp;following&nbsp;datasets&nbsp;in&nbsp;it:<br>
+&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;command&nbsp;will&nbsp;create&nbsp;a&nbsp;'data'&nbsp;subdirectory&nbsp;in&nbsp;the&nbsp;ExamplesObjectDetection<br>
+&nbsp;&nbsp;&nbsp;&nbsp;directory&nbsp;and&nbsp;deposit&nbsp;the&nbsp;following&nbsp;datasets&nbsp;in&nbsp;it:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Purdue_Dr_Eval_Dataset-clutter-10-noise-20-size-10000-train.gz<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Purdue_Dr_Eval_Dataset-clutter-10-noise-20-size-1000-test.gz<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Purdue_Dr_Eval_Multi_Dataset-clutter-10-noise-20-size-10000-train.gz<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Purdue_Dr_Eval_Multi_Dataset-clutter-10-noise-20-size-1000-test.gz<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;In&nbsp;the&nbsp;naming&nbsp;convention&nbsp;used&nbsp;for&nbsp;the&nbsp;archives,&nbsp;the&nbsp;string&nbsp;'clutter-10'<br>
-&nbsp;&nbsp;&nbsp;&nbsp;means&nbsp;that&nbsp;each&nbsp;image&nbsp;will&nbsp;have&nbsp;a&nbsp;maximum&nbsp;of&nbsp;10&nbsp;clutter&nbsp;objects&nbsp;in&nbsp;it,<br>
-&nbsp;&nbsp;&nbsp;&nbsp;and&nbsp;the&nbsp;string&nbsp;'noise-20'&nbsp;means&nbsp;that&nbsp;I&nbsp;have&nbsp;added&nbsp;20%&nbsp;Gaussian&nbsp;noise&nbsp;to<br>
-&nbsp;&nbsp;&nbsp;&nbsp;each&nbsp;image.&nbsp;The&nbsp;string&nbsp;'size-10000'&nbsp;means&nbsp;that&nbsp;the&nbsp;dataset&nbsp;consists&nbsp;of<br>
-&nbsp;&nbsp;&nbsp;&nbsp;'10,000'&nbsp;images.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;In&nbsp;the&nbsp;naming&nbsp;convention&nbsp;used&nbsp;for&nbsp;the&nbsp;archives,&nbsp;the&nbsp;string&nbsp;'clutter-10'&nbsp;means<br>
+&nbsp;&nbsp;&nbsp;&nbsp;that&nbsp;each&nbsp;image&nbsp;will&nbsp;have&nbsp;a&nbsp;maximum&nbsp;of&nbsp;10&nbsp;clutter&nbsp;objects&nbsp;in&nbsp;it,&nbsp;and&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;string&nbsp;'noise-20'&nbsp;means&nbsp;that&nbsp;I&nbsp;have&nbsp;added&nbsp;20%&nbsp;Gaussian&nbsp;noise&nbsp;to&nbsp;each<br>
+&nbsp;&nbsp;&nbsp;&nbsp;image.&nbsp;The&nbsp;string&nbsp;'size-10000'&nbsp;means&nbsp;that&nbsp;the&nbsp;dataset&nbsp;consists&nbsp;of&nbsp;'10,000'<br>
+&nbsp;&nbsp;&nbsp;&nbsp;images.<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;two&nbsp;"Multi"&nbsp;datasets&nbsp;named&nbsp;above&nbsp;are&nbsp;for&nbsp;experimenting&nbsp;with&nbsp;the&nbsp;YOLO<br>
-&nbsp;&nbsp;&nbsp;&nbsp;implementation&nbsp;in&nbsp;the&nbsp;module&nbsp;for&nbsp;multi-instance&nbsp;object&nbsp;detection&nbsp;in<br>
-&nbsp;&nbsp;&nbsp;&nbsp;images.&nbsp;&nbsp;The&nbsp;datasets&nbsp;without&nbsp;the&nbsp;word&nbsp;"Multi"&nbsp;in&nbsp;their&nbsp;names&nbsp;are&nbsp;for<br>
-&nbsp;&nbsp;&nbsp;&nbsp;experimenting&nbsp;with&nbsp;single-instance&nbsp;detection&nbsp;---&nbsp;but&nbsp;under&nbsp;circumstances<br>
-&nbsp;&nbsp;&nbsp;&nbsp;that&nbsp;are&nbsp;more&nbsp;difficult&nbsp;than&nbsp;discussed&nbsp;in&nbsp;my&nbsp;Week&nbsp;7&nbsp;Deep&nbsp;Learning&nbsp;Lecture<br>
-&nbsp;&nbsp;&nbsp;&nbsp;at&nbsp;Purdue.<br>
-&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;You&nbsp;will&nbsp;also&nbsp;find&nbsp;two&nbsp;smaller&nbsp;datasets&nbsp;in&nbsp;the&nbsp;overall&nbsp;archive&nbsp;that&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;contain&nbsp;just&nbsp;30&nbsp;images&nbsp;each.&nbsp;&nbsp;Those&nbsp;are&nbsp;for&nbsp;debugging&nbsp;your&nbsp;code.<br>
-&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;implementation&nbsp;in&nbsp;the&nbsp;module&nbsp;for&nbsp;multi-instance&nbsp;object&nbsp;detection&nbsp;in&nbsp;images.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;datasets&nbsp;without&nbsp;the&nbsp;word&nbsp;"Multi"&nbsp;in&nbsp;their&nbsp;names&nbsp;are&nbsp;for&nbsp;experimenting<br>
+&nbsp;&nbsp;&nbsp;&nbsp;with&nbsp;single-instance&nbsp;detection&nbsp;---&nbsp;but&nbsp;under&nbsp;circumstances&nbsp;that&nbsp;are&nbsp;more<br>
+&nbsp;&nbsp;&nbsp;&nbsp;difficult&nbsp;than&nbsp;discussed&nbsp;in&nbsp;my&nbsp;Week&nbsp;7&nbsp;Deep&nbsp;Learning&nbsp;Lecture&nbsp;at&nbsp;Purdue.<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;You&nbsp;will&nbsp;also&nbsp;find&nbsp;two&nbsp;smaller&nbsp;datasets&nbsp;in&nbsp;the&nbsp;overall&nbsp;archive&nbsp;that&nbsp;contain<br>
+&nbsp;&nbsp;&nbsp;&nbsp;just&nbsp;30&nbsp;images&nbsp;each.&nbsp;&nbsp;Those&nbsp;are&nbsp;for&nbsp;debugging&nbsp;your&nbsp;code.<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;ABOUT&nbsp;THE&nbsp;ANNOTATIONS&nbsp;IN&nbsp;THE&nbsp;DATASETS:<br>
+&nbsp;<br>
+&nbsp;&nbsp;&nbsp;&nbsp;See&nbsp;the&nbsp;Slides&nbsp;43&nbsp;and&nbsp;44&nbsp;of&nbsp;the&nbsp;"Week&nbsp;8:&nbsp;Multi-Instance&nbsp;Object&nbsp;Detection"<br>
+&nbsp;&nbsp;&nbsp;&nbsp;slides&nbsp;at&nbsp;the&nbsp;course&nbsp;website&nbsp;for&nbsp;a&nbsp;description&nbsp;of&nbsp;how&nbsp;the&nbsp;annotations&nbsp;are<br>
+&nbsp;&nbsp;&nbsp;&nbsp;organized&nbsp;for&nbsp;the&nbsp;dataset&nbsp;mentioned&nbsp;above.<br>
 &nbsp;<br>
 &nbsp;<br>
 <font size="+2" color="red">THE&nbsp;ExamplesObjectDetection&nbsp;DIRECTORY:<br>
 </font>&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;directory&nbsp;contains&nbsp;the&nbsp;following&nbsp;two&nbsp;scripts&nbsp;related&nbsp;to&nbsp;object<br>
-&nbsp;&nbsp;&nbsp;&nbsp;detection&nbsp;in&nbsp;images:<br>
+&nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;directory&nbsp;contains&nbsp;the&nbsp;following&nbsp;two&nbsp;scripts&nbsp;related&nbsp;to&nbsp;object&nbsp;detection<br>
+&nbsp;&nbsp;&nbsp;&nbsp;in&nbsp;images:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;single_instance_object_detection.py<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;multi_instance_object_detection.py<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;first&nbsp;script&nbsp;carries&nbsp;out&nbsp;single-instance&nbsp;detections&nbsp;in&nbsp;the&nbsp;images&nbsp;in<br>
-&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;PurdueDrEvalDataset&nbsp;dataset&nbsp;and&nbsp;the&nbsp;second&nbsp;script&nbsp;carries&nbsp;out<br>
-&nbsp;&nbsp;&nbsp;&nbsp;multi-instance&nbsp;detections&nbsp;in&nbsp;the&nbsp;PurdueDrEvalMultiDataset.&nbsp;&nbsp;In&nbsp;the&nbsp;former<br>
-&nbsp;&nbsp;&nbsp;&nbsp;dataset,&nbsp;each&nbsp;128x128&nbsp;image&nbsp;has&nbsp;only&nbsp;one&nbsp;instance&nbsp;of&nbsp;a&nbsp;meaningful&nbsp;object<br>
-&nbsp;&nbsp;&nbsp;&nbsp;along&nbsp;with&nbsp;structured&nbsp;artifacts&nbsp;and&nbsp;20%&nbsp;random&nbsp;noise.&nbsp;&nbsp;And,&nbsp;in&nbsp;the&nbsp;latter<br>
-&nbsp;&nbsp;&nbsp;&nbsp;dataset,&nbsp;each&nbsp;image&nbsp;has&nbsp;up&nbsp;to&nbsp;five&nbsp;instances&nbsp;of&nbsp;meaningful&nbsp;objects&nbsp;along<br>
-&nbsp;&nbsp;&nbsp;&nbsp;with&nbsp;the&nbsp;structured&nbsp;artifacts&nbsp;and&nbsp;20%&nbsp;random&nbsp;noise.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;first&nbsp;script&nbsp;carries&nbsp;out&nbsp;single-instance&nbsp;detections&nbsp;in&nbsp;the&nbsp;images&nbsp;in&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;PurdueDrEvalDataset&nbsp;dataset&nbsp;and&nbsp;the&nbsp;second&nbsp;script&nbsp;carries&nbsp;out&nbsp;multi-instance<br>
+&nbsp;&nbsp;&nbsp;&nbsp;detections&nbsp;in&nbsp;the&nbsp;PurdueDrEvalMultiDataset.&nbsp;&nbsp;In&nbsp;the&nbsp;former&nbsp;dataset,&nbsp;each<br>
+&nbsp;&nbsp;&nbsp;&nbsp;128x128&nbsp;image&nbsp;has&nbsp;only&nbsp;one&nbsp;instance&nbsp;of&nbsp;a&nbsp;meaningful&nbsp;object&nbsp;along&nbsp;with<br>
+&nbsp;&nbsp;&nbsp;&nbsp;structured&nbsp;artifacts&nbsp;and&nbsp;20%&nbsp;random&nbsp;noise.&nbsp;&nbsp;And,&nbsp;in&nbsp;the&nbsp;latter&nbsp;dataset,&nbsp;each<br>
+&nbsp;&nbsp;&nbsp;&nbsp;image&nbsp;has&nbsp;up&nbsp;to&nbsp;five&nbsp;instances&nbsp;of&nbsp;meaningful&nbsp;objects&nbsp;along&nbsp;with&nbsp;the&nbsp;structured<br>
+&nbsp;&nbsp;&nbsp;&nbsp;artifacts&nbsp;and&nbsp;20%&nbsp;random&nbsp;noise.<br>
 &nbsp;<br>
 &nbsp;<br>
 &nbsp;<br>
 <font size="+2" color="red">THE&nbsp;ExamplesRegionProposals&nbsp;DIRECTORY:<br>
 </font>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;This&nbsp;directory&nbsp;contains&nbsp;the&nbsp;following&nbsp;scripts&nbsp;for&nbsp;showcasing&nbsp;graph-based<br>
 &nbsp;&nbsp;&nbsp;&nbsp;algorithms&nbsp;for&nbsp;constructing&nbsp;region&nbsp;proposals:<br>
@@ -693,88 +685,87 @@
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;torchvision_some_basic_transformations.py&nbsp;&nbsp;&nbsp;&nbsp;<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;torchvision_based_image_processing.py<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;multi_image_histogramming_and_display.py&nbsp;&nbsp;<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;Examples&nbsp;directory&nbsp;also&nbsp;illustrates&nbsp;the&nbsp;sort&nbsp;of&nbsp;region&nbsp;proposal<br>
-&nbsp;&nbsp;&nbsp;&nbsp;results&nbsp;you&nbsp;can&nbsp;obtain&nbsp;with&nbsp;the&nbsp;graph-based&nbsp;algorithms&nbsp;in&nbsp;this&nbsp;module.<br>
-&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;specific&nbsp;illustrations&nbsp;are&nbsp;in&nbsp;the&nbsp;following&nbsp;subdirectories&nbsp;of&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Examples&nbsp;directory:<br>
+&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;ExamplesRegionProposals&nbsp;directory&nbsp;also&nbsp;illustrates&nbsp;the&nbsp;sort&nbsp;of&nbsp;region<br>
+&nbsp;&nbsp;&nbsp;&nbsp;proposal&nbsp;results&nbsp;you&nbsp;can&nbsp;obtain&nbsp;with&nbsp;the&nbsp;graph-based&nbsp;algorithms&nbsp;in&nbsp;this<br>
+&nbsp;&nbsp;&nbsp;&nbsp;module.&nbsp;&nbsp;The&nbsp;specific&nbsp;illustrations&nbsp;are&nbsp;in&nbsp;the&nbsp;following&nbsp;subdirectories&nbsp;of&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;ExamplesRegionProposals&nbsp;directory:<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Examples/color_blobs/<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ExamplesRegionProposals/color_blobs/<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Examples/mondrian/<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ExamplesRegionProposals/mondrian/<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Examples/wallpic2/<br>
+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ExamplesRegionProposals/wallpic2/<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Each&nbsp;subdirectory&nbsp;contains&nbsp;at&nbsp;least&nbsp;the&nbsp;following&nbsp;two&nbsp;files:<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;selective_search.py<br>
 &nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;image&nbsp;file&nbsp;specific&nbsp;for&nbsp;that&nbsp;subdirectory.<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;All&nbsp;you&nbsp;have&nbsp;to&nbsp;do&nbsp;is&nbsp;to&nbsp;execute&nbsp;selective_search.py&nbsp;in&nbsp;that&nbsp;directory&nbsp;to<br>
-&nbsp;&nbsp;&nbsp;&nbsp;see&nbsp;the&nbsp;results&nbsp;on&nbsp;the&nbsp;image&nbsp;in&nbsp;that&nbsp;directory.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;All&nbsp;you&nbsp;have&nbsp;to&nbsp;do&nbsp;is&nbsp;to&nbsp;execute&nbsp;selective_search.py&nbsp;in&nbsp;that&nbsp;directory&nbsp;to&nbsp;see<br>
+&nbsp;&nbsp;&nbsp;&nbsp;the&nbsp;results&nbsp;on&nbsp;the&nbsp;image&nbsp;in&nbsp;that&nbsp;directory.<br>
 &nbsp;<br>
 &nbsp;<br>
 &nbsp;<br>
 <font size="+2" color="red">BUGS:<br>
 </font>&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Please&nbsp;notify&nbsp;the&nbsp;author&nbsp;if&nbsp;you&nbsp;encounter&nbsp;any&nbsp;bugs.&nbsp;&nbsp;When&nbsp;sending<br>
-&nbsp;&nbsp;&nbsp;&nbsp;email,&nbsp;please&nbsp;place&nbsp;the&nbsp;string&nbsp;'RegionProposalGenerator'&nbsp;in&nbsp;the<br>
-&nbsp;&nbsp;&nbsp;&nbsp;subject&nbsp;line&nbsp;to&nbsp;get&nbsp;past&nbsp;the&nbsp;author's&nbsp;spam&nbsp;filter.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Please&nbsp;notify&nbsp;the&nbsp;author&nbsp;if&nbsp;you&nbsp;encounter&nbsp;any&nbsp;bugs.&nbsp;&nbsp;When&nbsp;sending&nbsp;email,<br>
+&nbsp;&nbsp;&nbsp;&nbsp;please&nbsp;place&nbsp;the&nbsp;string&nbsp;'RegionProposalGenerator'&nbsp;in&nbsp;the&nbsp;subject&nbsp;line&nbsp;to&nbsp;get<br>
+&nbsp;&nbsp;&nbsp;&nbsp;past&nbsp;the&nbsp;author's&nbsp;spam&nbsp;filter.<br>
 &nbsp;<br>
 &nbsp;<br>
 <font size="+2" color="red">ABOUT&nbsp;THE&nbsp;AUTHOR:<br>
 </font>&nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;author,&nbsp;Avinash&nbsp;Kak,&nbsp;is&nbsp;a&nbsp;professor&nbsp;of&nbsp;Electrical&nbsp;and&nbsp;Computer<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Engineering&nbsp;at&nbsp;Purdue&nbsp;University.&nbsp;&nbsp;For&nbsp;all&nbsp;issues&nbsp;related&nbsp;to&nbsp;this<br>
-&nbsp;&nbsp;&nbsp;&nbsp;module,&nbsp;contact&nbsp;the&nbsp;author&nbsp;at&nbsp;kak@purdue.edu&nbsp;If&nbsp;you&nbsp;send&nbsp;email,<br>
-&nbsp;&nbsp;&nbsp;&nbsp;please&nbsp;place&nbsp;the&nbsp;string&nbsp;"RegionProposalGenerator"&nbsp;in&nbsp;your&nbsp;subject<br>
-&nbsp;&nbsp;&nbsp;&nbsp;line&nbsp;to&nbsp;get&nbsp;past&nbsp;the&nbsp;author's&nbsp;spam&nbsp;filter.<br>
+&nbsp;&nbsp;&nbsp;&nbsp;The&nbsp;author,&nbsp;Avinash&nbsp;Kak,&nbsp;is&nbsp;a&nbsp;professor&nbsp;of&nbsp;Electrical&nbsp;and&nbsp;Computer&nbsp;Engineering<br>
+&nbsp;&nbsp;&nbsp;&nbsp;at&nbsp;Purdue&nbsp;University.&nbsp;&nbsp;For&nbsp;all&nbsp;issues&nbsp;related&nbsp;to&nbsp;this&nbsp;module,&nbsp;contact&nbsp;the<br>
+&nbsp;&nbsp;&nbsp;&nbsp;author&nbsp;at&nbsp;kak@purdue.edu&nbsp;If&nbsp;you&nbsp;send&nbsp;email,&nbsp;please&nbsp;place&nbsp;the&nbsp;string<br>
+&nbsp;&nbsp;&nbsp;&nbsp;"RegionProposalGenerator"&nbsp;in&nbsp;your&nbsp;subject&nbsp;line&nbsp;to&nbsp;get&nbsp;past&nbsp;the&nbsp;author's&nbsp;spam<br>
+&nbsp;&nbsp;&nbsp;&nbsp;filter.<br>
 &nbsp;<br>
 <font size="+2" color="red">COPYRIGHT:<br>
 </font>&nbsp;<br>
 &nbsp;&nbsp;&nbsp;&nbsp;Python&nbsp;Software&nbsp;Foundation&nbsp;License<br>
 &nbsp;<br>
-&nbsp;&nbsp;&nbsp;&nbsp;Copyright&nbsp;2022&nbsp;Avinash&nbsp;Kak<br>
+&nbsp;&nbsp;&nbsp;&nbsp;Copyright&nbsp;2023&nbsp;Avinash&nbsp;Kak<br>
 &nbsp;<br>
 @endofdocs</tt></p>
 <p>
 <table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
 <tr bgcolor="#aa55cc">
 <td colspan=3 valign=bottom>&nbsp;<br>
-<font color="#ffffff" face="helvetica, arial"><big><strong>Imported Modules</strong></big></font></td></tr>
+<font color="#ffffff" face="helvetica, arial"><big><strong>Modules</strong></big></font></td></tr>
     
 <tr><td bgcolor="#aa55cc"><tt>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</tt></td><td>&nbsp;</td>
 <td width="100%"><table width="100%" summary="list"><tr><td width="25%" valign=top><a href="torchvision.transforms.functional.html">torchvision.transforms.functional</a><br>
 <a href="PIL.Image.html">PIL.Image</a><br>
 <a href="PIL.ImageDraw.html">PIL.ImageDraw</a><br>
 <a href="PIL.ImageFont.html">PIL.ImageFont</a><br>
 <a href="PIL.ImageTk.html">PIL.ImageTk</a><br>
 <a href="tkinter.html">tkinter</a><br>
 <a href="copy.html">copy</a><br>
 </td><td width="25%" valign=top><a href="functools.html">functools</a><br>
 <a href="glob.html">glob</a><br>
-<a href="gzip.html">gzip</a><br>
 <a href="logging.html">logging</a><br>
 <a href="math.html">math</a><br>
 <a href="torch.nn.html">torch.nn</a><br>
 <a href="numpy.html">numpy</a><br>
-</td><td width="25%" valign=top><a href="torch.optim.html">torch.optim</a><br>
-<a href="os.html">os</a><br>
+<a href="torch.optim.html">torch.optim</a><br>
+</td><td width="25%" valign=top><a href="os.html">os</a><br>
 <a href="pickle.html">pickle</a><br>
 <a href="matplotlib.pyplot.html">matplotlib.pyplot</a><br>
 <a href="random.html">random</a><br>
 <a href="re.html">re</a><br>
 <a href="signal.html">signal</a><br>
-</td><td width="25%" valign=top><a href="sys.html">sys</a><br>
-<a href="time.html">time</a><br>
+<a href="sys.html">sys</a><br>
+</td><td width="25%" valign=top><a href="time.html">time</a><br>
 <a href="torch.html">torch</a><br>
 <a href="torchvision.html">torchvision</a><br>
 <a href="torchvision.utils.html">torchvision.utils</a><br>
 <a href="torchvision.transforms.html">torchvision.transforms</a><br>
 </td></tr></table></td></tr></table><p>
 <table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
 <tr bgcolor="#ee77aa">
@@ -1172,18 +1163,18 @@
 </td></tr></table><p>
 <table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
 <tr bgcolor="#55aa55">
 <td colspan=3 valign=bottom>&nbsp;<br>
 
 p<tr><td bgcolor="#55aa55"><tt>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</tt></td><td>&nbsp;</td>
 <td width="100%"><strong>__author__</strong> = 'Avinash Kak (kak@purdue.edu)'<br>
-<strong>__copyright__</strong> = '(C) 2022 Avinash Kak. Python Software Foundation.'<br>
-<strong>__date__</strong> = '2022-April-16'<br>
-<strong>__url__</strong> = 'https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.0.8.html'<br>
-<strong>__version__</strong> = '2.0.8'</td></tr></table>
+<strong>__copyright__</strong> = '(C) 2023 Avinash Kak. Python Software Foundation.'<br>
+<strong>__date__</strong> = '2023-April-9'<br>
+<strong>__url__</strong> = 'https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.1.0.html'<br>
+<strong>__version__</strong> = '2.1.0'</td></tr></table>
 <table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
 <tr bgcolor="#7799ee">
 <td colspan=3 valign=bottom>&nbsp;<br>
 <font color="#ffffff" face="helvetica, arial"><big><strong>Author</strong></big></font></td></tr>
 <tr><td bgcolor="#7799ee"><tt>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</tt></td><td>&nbsp;</td>
 <td width="100%">Avinash&nbsp;Kak&nbsp;(kak@purdue.edu)</td></tr></table>
 </body></html>
```

#### html2text {}

```diff
@@ -1,247 +1,280 @@
 
  
  
-RegionProposalGenerator (version 2.0.8, 2022-April-16)
+RegionProposalGenerator (version 2.1.0, 2023-April-9)
 RegionProposalGenerator.py
  
-Version: 2.0.8
+Version: 2.1.0
    
 Author: Avinash Kak (kak@purdue.edu)
  
-Date: 2022-April-16
+Date: 2023-April-9
  
  
                                          Total number of downloads (all versions): <?php $file = fopen
                                     ("HowManyCounts.txt", "r") or exit("Unable to open file!"); echo fgets($file);
-Download Version 2.0.8:  gztar    fclose($file); ?>
+Download Version 2.1.0:  gztar    fclose($file); ?>
                                                    This count is automatically updated at every rotation of
                                                      the weblogs (normally once every two to four days)
                                          Last updated: <?php $file = fopen("LastUpdated.txt", "r") or exit("Unable to
                                                     open file!"); echo fgets($file); fclose($file); ?>
 
 View_the_main_module_code_file_in_your_browser  
  
 Download_the_image_datasets_for_RPG  
  
  
  
 CHANGES:
 
+  Version 2.1.0:
+ 
+    With this version, you can now use batches of any size for YOLO learning.
+    Previously, the batch size was limited to 1 for the YOLO part of the module.
+    Allowing for batches required changes in the handling of problem images, such
+    as the images with no meaningful objects, or the images with object bounding
+    boxes with unrealistic aspect ratios.
+ 
   Version 2.0.8:
  
-    This version constitutes a complete implementation of a YOLO
-    multi-instance object detector.  In addition to the new multi-loss
-    function that I introduced in the previous public release of this module,
-    the new version includes a full-blown implementation of what you need for
-    validation testing.  I should also mention that I have split what used to
-    be the Examples directory in the distribution into two directories:
-    ExamplesObjectDetection and ExamplesRegionProposals.  Your entry point for
-    learning the YOLO implementation would be the script
-    multi_instance_object_detection.py in the directory
-    ExamplesObjectDetection.
+    This version constitutes a complete implementation of a YOLO multi-instance
+    object detector.  In addition to the new multi-
+loss function that I introduced
+    in the previous public release of this module, the new version includes a
+    full-
+blown implementation of what you need for validation testing.  I should
+    also mention that I have split what used to be the Examples directory in the
+    distribution into two directories: ExamplesObjectDetection and
+    ExamplesRegionProposals.  Your entry point for learning the YOLO
+    implementation would be the script multi_instance_object_detection.py in the
+    directory ExamplesObjectDetection.
     
   Version 2.0.6:
  
-    This version incorporates a more sophisticated loss function for
-    YOLO-based multi-instance object detection in images.  In the new loss
-    function, I use different criteria for the different segments of the YOLO
-    vector.  [Assigning an object instance in a training image to an anchor
-    box for a cell in the image involves creating a "5+C"-element YOLO vector,
-    where C is the number of object classes.] I now use the Binary
-    Cross-Entropy Loss (nn.BCELoss) for the first element of the YOLO vector
-    that stands for the presence or the absence of an object instance in a
-    specific anchor box in a specific cell.  I use mean-squared-error loss
-    (nn.MSELoss) for the next four numerical elements that express the precise
-    location of the object bounding-box vis-a-vis the center of the cell to
-    which the object is assigned and also for the dimensions of the bounding
-    box.  Finally, I use the regular Cross-Entropy loss (nn.CrossEntropyLoss)
-    for the last C elements of the YOLO vector.  Using the cross-entropy loss
-    for the labeling errors required augmenting the YOLO vector with one
-    additional element to express the absence of an object.
+    This version incorporates a more sophisticated loss function for YOLO-based
+    multi-instance object detection in images.  In the new loss function, I use
+    different criteria for the different segments of the YOLO vector.  
+[Assigning
+    an object instance in a training image to an anchor box for a cell in the
+    image involves creating a "5+C"-
+element YOLO vector, where C is the number of
+    object classes.] I now use the Binary Cross-Entropy Loss 
+(nn.BCELoss) for the
+    first element of the YOLO vector that stands for the presence or the absence
+    of an object instance in a specific anchor box in a specific cell.  I use
+    mean-squared-error loss 
+(nn.MSELoss) for the next four numerical elements that
+    express the precise location of the object bounding-box vis-a-
+vis the center
+    of the cell to which the object is assigned and also for the dimensions of the
+    bounding box.  Finally, I use the regular Cross-Entropy loss
+    
+(nn.CrossEntropyLoss) for the last C elements of the YOLO vector.  Using the
+    cross-
+entropy loss for the labeling errors required augmenting the YOLO vector
+    with one additional element to express the absence of an object.
  
   Version 2.0.2:
  
-    This version fixes a couple of bugs in the YOLO-based logic for
-    multi-instance object detection.
+    This version fixes a couple of bugs in the YOLO-based logic for multi-
+instance
+    object detection.
  
   Version 2.0.1:
  
     This module has gone through several changes since its last public-release
     version as I was experimenting with different ways of imparting to the
     students the sudden increase in model complexity as one goes from
-    single-instance object detection to multi-instance object detection.
-    These experiments led to the creation of two new datasets,
-    PurdueDrEvalDataset and PurdueDrEvalMultiDataset, the former for playing
-    with single-instance object detection and the latter for doing the same
-    with multi-instance object detection.  The module also includes two inner
-    classes, SingleInstanceDetector and YoloLikeDetector, the former a
-    reference implementation for single instance object detection and the
-    latter a YOLO-like reference implementation for multi-instance object
-    detection. [By the way, "DrEval" in the names of the two datasets
-    mentioned here has a connection with "Dr Evil" in the Austin Powers
-    movies.]
+    single-instance object detection to multi-instance object detection.  These
+    experiments led to the creation of two new datasets, PurdueDrEvalDataset and
+    PurdueDrEvalMultiDataset, the former for playing with single-
+instance object
+    detection and the latter for doing the same with multi-instance object
+    detection.  The module also includes two inner classes, SingleInstanceDetector
+    and YoloLikeDetector, the former a reference implementation for single
+    instance object detection and the latter a YOLO-
+like reference implementation
+    for multi-instance object detection. 
+[By the way, "DrEval" in the names of the
+    two datasets mentioned here has a connection with "Dr Evil" in the Austin
+    Powers movies.]
  
   Version 1.0.5:
  
     In keeping with the tutorial nature of this module, this version includes
-    methods that come in handy for batch-based processing of images. These
-    methods carry names like "displaying_and_histogramming_
-    images_in_batchX()" where X is 1, 2, and 3.  The rest of the module,
-    especially the part that deals with constructing region proposals remains
-    unchanged.
+    methods that come in handy for batch-
+based processing of images. These methods
+    carry names like "displaying_and_histogramming_ images_in_batchX
+()" where X is
+    1, 2, and 3.  The rest of the module, especially the part that deals with
+    constructing region proposals remains unchanged.
  
   Version 1.0.4:
  
     This is the first public release version of the module.
  
  
 INTRODUCTION:
  
     Single-Instance vs. Multi-Instance Detection:
  
-    This module was created for experimenting with the logic of object
-    detection with neural networks.  On the face of it, object detection in
-    images sounds like a well-defined problem that should lend itself to
-    well-defined solutions.  Unfortunately, the reality is otherwise.  Yes,
-    simple examples of the problem -- such as when the images contain
-    single object instances and with no competing clutter in the background
-    -- the problem can be solved straightforwardly with a neural network.
-    However, the object detection problems that are encountered in real
-    life are rarely that simple.  A practically useful framework for object
-    detection must be able to recognize and localize all possible instances
-    of the objects of interest in a given image.
+    This module was created for experimenting with the logic of object detection
+    with neural networks.  On the face of it, object detection in images sounds
+    like a well-defined problem that should lend itself to well-
+defined solutions.
+    Unfortunately, the reality is otherwise.  Yes, simple examples of the problem
+    -- such as when the images contain single object instances and with no
+    competing clutter in the background -- the problem can be solved
+    straightforwardly with a neural network.  However, the object detection
+    problems that are encountered in real life are rarely that simple.  A
+    practically useful framework for object detection must be able to recognize
+    and localize all possible instances of the objects of interest in a given
+    image.
  
     So how does one solve the problem of multi-instance object detection and
     localization with a neural network?
  
     The last half-dozen years have seen the emergence of the following three
-    competition-grade neural-network based approaches for multi-instance
-    object detection: R-CNN, YOLO, and SSD.  The Preamble section of my Week 8
-    lecture for Purdue's Deep Learning class provides a brief overview of
-    these approaches.  YOLO stands for "You Only Look Once" --- in contrast
-    with R-CNN based approaches in which you may have to subject the images to
-    a couple of neural networks, one for generating region proposals and the
-    other for actual object detection.
- 
-    The main goal of the present module is to provide an educational example
-    of a complete implementation of the YOLO logic for multi-instance object
-    detection in images.
+    competition-grade neural-network based approaches for multi-instance object
+    detection: R-CNN, YOLO, and SSD.  The Preamble section of my Week 8 lecture
+    for Purdue's Deep Learning class provides a brief overview of these
+    approaches.  YOLO stands for "You Only Look Once" --- in contrast with R-
+CNN
+    based approaches in which you may have to subject the images to a couple of
+    neural networks, one for generating region proposals and the other for actual
+    object detection.
+ 
+    The main goal of the present module is to provide an educational example of a
+    complete implementation of the YOLO logic for multi-
+instance object detection
+    in images.
  
     Graph-Based Algorithms for Region Proposals:
  
-    A second goal of this module is to provide implementations for a couple
-    of the more modern graph-based approaches for generating region
-    proposals.  At this point, the reader might ask: What is a region
-    proposal?  A region proposal is a blob of pixels that is highly likely
-    to contain an object instance.  Another way of saying same thing is
-    that region proposals are pixel blobs that look different from the
-    general background in the images.  While it is possible to use a neural
-    network for generating region proposals, as demonstrated by the success
-    of RPN (Region Proposal Network) in the R-CNN based multi-instance
+    A second goal of this module is to provide implementations for a couple of the
+    more modern graph-
+based approaches for generating region proposals.  At this
+    point, the reader might ask:
+ What is a region proposal?  A region proposal is
+    a blob of pixels that is highly likely to contain an object instance.  Another
+    way of saying same thing is that region proposals are pixel blobs that look
+    different from the general background in the images.  While it is possible to
+    use a neural network for generating region proposals, as demonstrated by the
+    success of RPN (Region Proposal Network) in the R-CNN based multi-instance
     object detection, the RPG module is concerned primarily with the
-    non-neural-network based methods -- the graph-based methods -- for
-    generating region proposals.  I believe that becoming familiar with the
-    non-learning based methods for constructing region proposals still has
-    considerable value.  Consider, for example, the problem of detecting
-    objects in satellite images where you simply do not have access to the
-    amount of training data you would need for a neural-network based
-    approach to work.
- 
-    With regard to the graph-based method for generating region proposals,
-    RPG (RegionProposalGenerator) implements elements of the Selective
-    Search (SS) algorithm for object detection as proposed by Uijlings, van
-    de Sande, Gevers, and Smeulders.  The Selective Search algorithm sits
-    on top of the graph-based image segmentation algorithm of Felzenszwalb
-    and Huttenlocher (FH) whose implementation is also included in the RPG
-    module.  The RPG module first processes an image with the FH
-    graph-based algorithm for image segmentation to divide an image into
-    pixel blobs.  The module subsequently invokes elements of the SS
-    algorithm to selectively merge the blobs on the basis of three
+    non-neural-network based methods -- the graph-based methods --
+ for generating
+    region proposals.  I believe that becoming familiar with the non-learning
+    based methods for constructing region proposals still has considerable value.
+    Consider, for example, the problem of detecting objects in satellite images
+    where you simply do not have access to the amount of training data you would
+    need for a neural-network based approach to work.
+ 
+    With regard to the graph-based method for generating region proposals, RPG
+    (RegionProposalGenerator) implements elements of the Selective Search (SS)
+    algorithm for object detection as proposed by Uijlings, van de Sande, Gevers,
+    and Smeulders.  The Selective Search algorithm sits on top of the graph-
+based
+    image segmentation algorithm of Felzenszwalb and Huttenlocher (FH) whose
+    implementation is also included in the RPG module.  The RPG module first
+    processes an image with the FH graph-
+based algorithm for image segmentation to
+    divide an image into pixel blobs.  The module subsequently invokes elements of
+    the SS algorithm to selectively merge the blobs on the basis of three
     properties: homogeneity of the color, grayscale variance, and texture
     homogeneity.
  
-    The FH algorithm is based on creating a graph-based representation of
-    an image in which, at the beginning, each pixel is a single vertex and
-    the edge between two vertices that stand for two adjacent pixels
-    represents the difference between some pixel property (such as the
-    color difference) at the two pixels.  Subsequently, for the vertex
-    merging logic, each vertex u, that after the first iteration stands for
-    a grouping of pixels, is characterized by a property called Int(u),
-    which is the largest value of the inter-pixel color difference between
-    the adjacent pixels.  In order to account for the fact that, at the
-    beginning, each vertex consists of only one pixel [which would not
-    allow for the calculation of Int(u)], the unary property of the pixels
-    at a vertex is extended from Int(u) to MInt(u) with the addition of a
-    vertex-size dependent number equal to k/|C| where "k" is a
-    user-specified parameter and |C| the cardinality of the set of pixels
-    represented by the vertex u in the graph.
- 
-    As mentioned above, initially the edges in the graph representation of
-    an image are set to the color difference between the two 8-adjacent
-    pixels that correspond to two different vertices.  Subsequently, as the
-    vertices are merged, an edge, E(u,v), between two vertices u and v is
-    set to the smallest value of the inter-pixel color difference for two
-    adjacent pixels that belong to the two vertices. At each iteration of
-    the algorithm, two vertices u and v are merged provided E(u,v) is less
-    than the smaller of the MInt(u) or MInt(v) attributes at the two
-    vertices.  My experience is that for most images the algorithm
-    terminates of its own accord after a small number of iterations while
-    the vertex merging condition can be satisfied.
- 
-    Since the algorithm is driven by the color differences between
-    8-adjacent pixels, the FH algorithm is likely to create too fine a
-    segmentation of an image.  The segments produced by FH can be made
-    larger by using the logic of SS that allows blobs of pixels to merge
-    into larger blobs provided doing so makes sense based on the inter-blob
-    values for mean color levels, color variances, texture values, etc.
+    The FH algorithm is based on creating a graph-
+based representation of an image
+    in which, at the beginning, each pixel is a single vertex and the edge between
+    two vertices that stand for two adjacent pixels represents the difference
+    between some pixel property 
+(such as the color difference) at the two pixels.
+    Subsequently, for the vertex merging logic, each vertex u, that after the
+    first iteration stands for a grouping of pixels, is characterized by a
+    property called Int(u), which is the largest value of the inter-pixel color
+    difference between the adjacent pixels.  In order to account for the fact
+    that, at the beginning, each vertex consists of only one pixel [which would
+    not allow for the calculation of Int
+(u)], the unary property of the pixels at
+    a vertex is extended from Int(u) to MInt(u) with the addition of a vertex-
+size
+    dependent number equal to k/|C| where "k" is a user-specified parameter and
+    |C| the cardinality of the set of pixels represented by the vertex u in the
+    graph.
+ 
+    As mentioned above, initially the edges in the graph representation of an
+    image are set to the color difference between the two 8-
+adjacent pixels that
+    correspond to two different vertices.  Subsequently, as the vertices are
+    merged, an edge, E
+(u,v), between two vertices u and v is set to the smallest
+    value of the inter-
+pixel color difference for two adjacent pixels that belong
+    to the two vertices. At each iteration of the algorithm, two vertices u and v
+    are merged provided E(u,v) is less than the smaller of the MInt(u) or MInt
+(v)
+    attributes at the two vertices.  My experience is that for most images the
+    algorithm terminates of its own accord after a small number of iterations
+    while the vertex merging condition can be satisfied.
+ 
+    Since the algorithm is driven by the color differences between 8-adjacent
+    pixels, the FH algorithm is likely to create too fine a segmentation of an
+    image.  The segments produced by FH can be made larger by using the logic of
+    SS that allows blobs of pixels to merge into larger blobs provided doing so
+    makes sense based on the inter-blob values for mean color levels, color
+    variances, texture values, etc.
  
  
 INSTALLATION:
  
     The RegionProposalGenerator class was packaged using setuptools.  For
-    installation, execute the following command in the source directory
-    (this is the directory that contains the setup.py file after you have
-    downloaded and uncompressed the package):
+    installation, execute the following command in the source directory 
+(this is
+    the directory that contains the setup.py file after you have downloaded and
+    uncompressed the package):
  
             sudo python3 setup.py install
  
-    On Linux distributions, this will install the module file at a location
-    that looks like
+    On Linux distributions, this will install the module file at a location that
+    looks like
  
              /usr/local/lib/python3.8/dist-packages/
  
-    If you do not have root access, you have the option of working directly
-    off the directory in which you downloaded the software by simply
-    placing the following statements at the top of your scripts that use
-    the RegionProposalGenerator class:
+    If you do not have root access, you have the option of working directly off
+    the directory in which you downloaded the software by simply placing the
+    following statements at the top of your scripts that use the
+    RegionProposalGenerator class:
  
             import sys
             sys.path.append( "pathname_to_RegionProposalGenerator_directory" )
  
-    To uninstall the module, simply delete the source directory, locate
-    where the RegionProposalGenerator module was installed with "locate
-    RegionProposalGenerator" and delete those files.  As mentioned above,
-    the full pathname to the installed version is likely to look like
+    To uninstall the module, simply delete the source directory, locate where the
+    RegionProposalGenerator module was installed with "locate
+    RegionProposalGenerator" and delete those files.  As mentioned above, the full
+    pathname to the installed version is likely to look like
     /usr/local/lib/python2.7/dist-packages/RegionProposalGenerator*
  
-    If you want to carry out a non-standard install of the
-    RegionProposalGenerator module, look up the on-line information on
-    Disutils by pointing your browser to
+    If you want to carry out a non-
+standard install of the RegionProposalGenerator
+    module, look up the on-
+line information on Disutils by pointing your browser
+    to
  
               http://docs.python.org/dist/dist.html
  
 USAGE:
  
     Single-Instance and Multi-Instance Detection:
  
-    If you wish to experiment with YOLO-like logic for multi-instance
-    object detection, you would need to construct an instance of the
-    RegionProposalGenerator class and invoke the methods shown below on
-    this instance:
+    If you wish to experiment with YOLO-like logic for multi-instance object
+    detection, you would need to construct an instance of the
+    RegionProposalGenerator class and invoke the methods shown below on this
+    instance:
  
     rpg = RegionProposalGenerator(
                       dataroot = "./data/",
                       image_size = [128,128],
                       yolo_interval = 20,
                       path_saved_yolo_model = "./saved_yolo_model",
                       momentum = 0.9,
@@ -259,17 +292,17 @@
 (model, display_images=False)
     yolo.run_code_for_training_multi_instance_detection
 (model, display_images = True)
     
  
     Graph-Based Algorithms for Region Proposals:
  
-    To generate region proposals, you would need to construct an instance
-    of the RegionProposalGenerator class and invoke the methods shown below
-    on this instance:
+    To generate region proposals, you would need to construct an instance of the
+    RegionProposalGenerator class and invoke the methods shown below on this
+    instance:
  
         rpg = RegionProposalGenerator(
                        ###  The first 6 options affect only the Graph-
 Based part of the algo
                        sigma = 1.0,
                        max_iterations = 40,
                        kay = 0.05,
@@ -290,348 +323,360 @@
 ( segmented_graph, image_name )
         rpg.visualize_segmentation_with_mean_gray
 (merged_blobs, "ss_based_segmentation_in_bw" )
  
  
 CONSTRUCTOR PARAMETERS: 
  
-    Of the 10 constructor parameters listed below, the first six are meant for
-    the FH algorithm and the last four for the SS algorithm.
+    Of the 10 constructor parameters listed below, the first six are meant for the
+    FH algorithm and the last four for the SS algorithm.
  
-    sigma: Controls the size of the Gaussian kernel used for smoothing the
-                    image before its gradient is calculated.  Assuming the
-                    pixel sampling interval to be unity, a sigma of 1 gives
-                    you a 7x7 smoothing operator with Gaussian weighting.
-                    The default for this parameter is 1.
+    sigma:
+ Controls the size of the Gaussian kernel used for smoothing the image
+                    before its gradient is calculated.  Assuming the pixel
+                    sampling interval to be unity, a sigma of 1 gives you a 7x7
+                    smoothing operator with Gaussian weighting.  The default for
+                    this parameter is 1.
  
     max_iterations: Sets an upper limit on the number of iterations of the
                     graph-based FH algorithm for image segmentation.
  
-    kay: This is the same as the "k" parameter in the FH algorithm.  As
-                    mentioned in the Introduction above, the Int(u)
-                    property of the pixels represented by each vertex in
-                    the graph representation of the image is extended to
-                    MInt(u) by the addition of a number k/|C| where |C| is
-                    the cardinality of the set of pixels at that vertex.
- 
-    image_normalization_required: This applies Torchvision's image
-                    normalization to the pixel values in the image.
- 
-    image_size_reduction_factor: As mentioned at the beginning of this
-                    document, RegionProposalGenerator is really not meant
-                    for production work.  The code is pure Python and, even
-                    with that, not at all optimized.  The focus of the
-                    module is primarily on easy understandability of what
-                    the code is doing so that you can experiment with the
-                    algorithm itself.  For the module to produce results
-                    within a reasonable length of time, you can use this
-                    constructor parameter to downsize the array of pixels
-                    that the module must work with.  Set this parameter to
-                    a value so that the initial graph constructed from the
-                    image has no more than around 3500 vertices if you
-                    don't want to wait too long for the results.
- 
-    min_size_for_graph_based_blobs: This declares a threshold on the
-                   smallest size you'd like to see (in terms of the number
-                   of pixels) in a segmented blob in the output of the
-                   graph-based segmenter.  (I typically use values from 1
-                   to 4 for this parameter.)
+    kay:
+ This is the same as the "k" parameter in the FH algorithm.  As mentioned
+                    in the Introduction above, the Int
+(u) property of the pixels
+                    represented by each vertex in the graph representation of the
+                    image is extended to MInt(u) by the addition of a number k/
+|C|
+                    where |C| is the cardinality of the set of pixels at that
+                    vertex.
+ 
+    image_normalization_required:
+ This applies Torchvision's image normalization
+                    to the pixel values in the image.
+ 
+    image_size_reduction_factor:
+ As mentioned at the beginning of this document,
+                    RegionProposalGenerator is really not meant for production
+                    work.  The code is pure Python and, even with that, not at all
+                    optimized.  The focus of the module is primarily on easy
+                    understandability of what the code is doing so that you can
+                    experiment with the algorithm itself.  For the module to
+                    produce results within a reasonable length of time, you can
+                    use this constructor parameter to downsize the array of pixels
+                    that the module must work with.  Set this parameter to a value
+                    so that the initial graph constructed from the image has no
+                    more than around 3500 vertices if you don't want to wait too
+                    long for the results.
+ 
+    min_size_for_graph_based_blobs:
+ This declares a threshold on the smallest size
+                   you'd like to see (in terms of the number of pixels) in a
+                   segmented blob in the output of the graph-based segmenter.  
+(I
+                   typically use values from 1 to 4 for this parameter.)
  
-    color_homogeneity_thresh:  
+    color_homogeneity_thresh:
  
                     This and the next three constructor options are meant
-                    specifically for the SS algorithm that sits on top of
-                    the FH algorithm for further merging of the pixel blobs
-                    produced by FH.  This constructor option specifies the
-                    maximum allowable difference between the mean color
-                    values in two pixel blobs for them to be merged.
+                    specifically for the SS algorithm that sits on top of the FH
+                    algorithm for further merging of the pixel blobs produced by
+                    FH.  This constructor option specifies the maximum allowable
+                    difference between the mean color values in two pixel blobs
+                    for them to be merged.
  
     gray_var_thresh:
  
-                   This option declares the maximum allowable difference in 
-                   the variances in the grayscale in two blobs if they are
-                   to be merged. 
+                   This option declares the maximum allowable difference in the
+                   variances in the grayscale in two blobs if they are to be
+                   merged.
  
     texture_homogeneity_thresh:
  
-                   The RegionProposalGenerator module characterizes the
-                   texture of the pixels in each segmented blob by its LBP
-                   (Local Binary Patterns) texture.  We want the LBP
-                   texture values for two different blobs to be within the
-                   value specified by this constructor option if those
-                   blobs are to be merged.
+                   The RegionProposalGenerator module characterizes the texture of
+                   the pixels in each segmented blob by its LBP (Local Binary
+                   Patterns) texture.  We want the LBP texture values for two
+                   different blobs to be within the value specified by this
+                   constructor option if those blobs are to be merged.
  
     max_num_blobs_expected:
  
-                   If you only want to extract a certain number of the
-                   largest possible blobs, you can do that by giving a
-                   value to this constructor option.
+                   If you only want to extract a certain number of the largest
+                   possible blobs, you can do that by giving a value to this
+                   constructor option.
  
  
 Inner Classes:
  
     (1)  PurdueDrEvalDataset
  
-         This is the dataset to use if you are experimenting with
-         single-instance object detection.  The dataset contains three
-         kinds of objects in its images: Dr. Eval, and two "objects" in his
-         neighborhood: a house and a watertower.  Each 128x128 image in the
-         dataset contains one of these objects after it is randomly scaled
-         and colored. Each image also contains substantial structured noise
-         in addition to 20% Gaussian noise.  Examples of these images are
-         shown in the Week 8 lecture material in Purdue's Deep Learning
-         class.
+         This is the dataset to use if you are experimenting with single-
+instance
+         object detection.  The dataset contains three kinds of objects in its
+         images: Dr. Eval, and two "objects" in his neighborhood: a house and a
+         watertower.  Each 128x128 image in the dataset contains one of these
+         objects after it is randomly scaled and colored. Each image also contains
+         substantial structured noise in addition to 20% Gaussian noise.  Examples
+         of these images are shown in the Week 8 lecture material in Purdue's Deep
+         Learning class.
  
     (2)  PurdueDrEvalMultiDataset
  
-         This is the dataset to use if you are experimenting with
-         multi-instance object detection.  Each image in the dataset
-         contains randomly chosen multiple instances of the same three
-         kinds of objects as mentioned above: Dr. Eval, house, and
-         watertower.  The number of object instances in each image is
-         limited to a maximum of five.  The images contain substantial
+         This is the dataset to use if you are experimenting with multi-
+instance
+         object detection.  Each image in the dataset contains randomly chosen
+         multiple instances of the same three kinds of objects as mentioned above:
+         Dr. Eval, house, and watertower.  The number of object instances in each
+         image is limited to a maximum of five.  The images contain substantial
          amount of structured noise in addition to 20% random noise.
          
-         The reason for why the above two datasets have "DrEval" in their
-         names: After having watched every contemporary movie at Netflix
-         that was worth watching, my wife and I decided to revisit some of
-         old movies that we had enjoyed a long time back.  That led us to
-         watching again a couple of Austin Powers movies.  If you are too
-         young to know what I am talking about, these movies are spoofs on
-         the James Bond movies in which the great comedian Mike Myers plays
-         both Austin Powers and his nemesis Dr. Evil.  Around the same
-         time, I was writing code for the two datasets mentioned above.
-         One of the three objects types in these images is a human-like
-         cartoon figure that I needed a name for.  So, after Dr. Evil in
-         the movies, I decided to call this cartoon figure Dr Eval and to
-         refer to the datasets as Dr Eval datasets. As you all know, "Eval"
-         is an important word for people like us.  All programming
-         languages provide a function with a name like "eval()".
+         The reason for why the above two datasets have "DrEval" in their names:
+         After having watched every contemporary movie at Netflix that was worth
+         watching, my wife and I decided to revisit some of old movies that we had
+         enjoyed a long time back.  That led us to watching again a couple of
+         Austin Powers movies.  If you are too young to know what I am talking
+         about, these movies are spoofs on the James Bond movies in which the
+         great comedian Mike Myers plays both Austin Powers and his nemesis
+         Dr. Evil.  Around the same time, I was writing code for the two datasets
+         mentioned above.  One of the three objects types in these images is a
+         human-
+like cartoon figure that I needed a name for.  So, after Dr. Evil
+         in the movies, I decided to call this cartoon figure Dr Eval and to refer
+         to the datasets as Dr Eval datasets. As you all know, "Eval" is an
+         important word for people like us.  All programming languages provide a
+         function with a name like "eval()".
  
     (3)  SingleInstanceDetector
  
          This provides a reference implementation for constructing a
-         single-instance object detector to be used for the
-         PurdueDrEvalDataset dataset. For the detection and regression
-         network, it uses the LOADnet2 network from DLStudio with small
-         modifications to account for the larger 128x128 images in the
-         dataset.
+         single-instance object detector to be used for the PurdueDrEvalDataset
+         dataset. For the detection and regression network, it uses the LOADnet2
+         network from DLStudio with small modifications to account for the larger
+         128x128 images in the dataset.
  
     (4)  YoloLikeDetector   [For multi-instance detection]
  
          The code in this inner class provides an implementation for the key
          elements of the YOLO logic for multi-instance object detection.  Each
          training image is divided into a grid of cells and it is the
          responsibility of the cell that contains the center of an object
-         bounding-box to provide at the output of the neural network an
-         estimate for the exact location of the center of the object bounding
-         box vis-a-vis the center of the cell.  That cell must also lead to an
-         estimate for the height and the width of the bounding-box for the
-         object instance.
+         bounding-
+box to provide at the output of the neural network an estimate
+         for the exact location of the center of the object bounding box vis-a-
+vis
+         the center of the cell.  That cell must also lead to an estimate for the
+         height and the width of the bounding-box for the object instance.
  
  
 PUBLIC METHODS:
  
-    Many of these method are related to using this module for experimenting
-    with the traditional graph-based algorithms for constructing region
-    proposals in images:
+    Many of these method are related to using this module for experimenting with
+    the traditional graph-based algorithms for constructing region proposals in
+    images:
  
     (1)  selective_search_for_region_proposals()
  
-         This method implements elements of the Selective Search (SS)
-         algorithm proposed by Uijlings, van de Sande, Gevers, and Smeulders
-         for creating region proposals for object detection.  As mentioned
-         elsewhere here, this algorithm sits on top of the graph based image
-         segmentation algorithm that was proposed by Felzenszwalb and
-         Huttenlocher.
+         This method implements elements of the Selective Search (SS) algorithm
+         proposed by Uijlings, van de Sande, Gevers, and Smeulders for creating
+         region proposals for object detection.  As mentioned elsewhere here, this
+         algorithm sits on top of the graph based image segmentation algorithm
+         that was proposed by Felzenszwalb and Huttenlocher.
  
     (2)  graph_based_segmentation()
  
          This is an implementation of the Felzenszwalb and Huttenlocher (FH)
-         algorithm for graph-based segmentation of images.  At the moment, it
-         is limited to working on grayscale images.
+         algorithm for graph-
+based segmentation of images.  At the moment, it is
+         limited to working on grayscale images.
  
     (3)  display_tensor_as_image()
  
-         This method converts the argument tensor into a photo image that you
-         can display in your terminal screen. It can convert tensors of three
-         different shapes into images: (3,H,W), (1,H,W), and (H,W), where H,
-         for height, stands for the number of pixel in the vertical direction
-         and W, for width, the same along the horizontal direction. When the
-         first element of the shape is 3, that means that the tensor
-         represents a color image in which each pixel in the (H,W) plane has
-         three values for the three color channels.  On the other hand, when
-         the first element is 1, that stands for a tensor that will be shown
-         as a grayscale image.  And when the shape is just (H,W), that is
-         automatically taken to be for a grayscale image.
+         This method converts the argument tensor into a photo image that you can
+         display in your terminal screen. It can convert tensors of three
+         different shapes into images: (3,H,W), (1,H,W), and 
+(H,W), where H, for
+         height, stands for the number of pixel in the vertical direction and W,
+         for width, the same along the horizontal direction. When the first
+         element of the shape is 3, that means that the tensor represents a color
+         image in which each pixel in the (H,W) plane has three values for the
+         three color channels.  On the other hand, when the first element is 1,
+         that stands for a tensor that will be shown as a grayscale image.  And
+         when the shape is just (H,W), that is automatically taken to be for a
+         grayscale image.
  
     (4)  graying_resizing_binarizing()
  
-         This is a demonstration of some of the more basic and commonly used
-         image transformations from the torchvision.transformations module.
-         The large comment blocks are meant to serve as tutorial introduction
-         to the syntax used for invoking these transformations.  The
-         transformations shown can be used for converting a color image into a
-         grayscale image, for resizing an image, for converting a PIL.Image
-         into a tensor and a tensor back into an PIL.Image object, and so on.
+         This is a demonstration of some of the more basic and commonly used image
+         transformations from the torchvision.transformations module.  The large
+         comment blocks are meant to serve as tutorial introduction to the syntax
+         used for invoking these transformations.  The transformations shown can
+         be used for converting a color image into a grayscale image, for resizing
+         an image, for converting a PIL.Image into a tensor and a tensor back into
+         an PIL.Image object, and so on.
  
     (5)  accessing_one_color_plane()
  
          This method shows how can access the n-th color plane of the argument
          color image.
  
     (6)  working_with_hsv_color_space()
  
-         Illustrates converting an RGB color image into its HSV
-         representation.
+         Illustrates converting an RGB color image into its HSV representation.
  
     (7)  histogramming_the_image()
  
-         PyTorch based experiments with histogramming the grayscale and the
-         color values in an image
+         PyTorch based experiments with histogramming the grayscale and the color
+         values in an image
  
     (8)  histogramming_and_thresholding():
  
-         This method illustrates using the PyTorch functionality for
-         histogramming and thresholding individual images.
+         This method illustrates using the PyTorch functionality for histogramming
+         and thresholding individual images.
  
     (9)  convolutions_with_pytorch()
  
          This method calls on torch.nn.functional.conv2d() for demonstrating a
          single image convolution with a specified kernel.
  
     (10) gaussian_smooth()
  
-         This method smooths an image with a Gaussian of specified sigma.  You
-         can do the same much faster by using the functionality programmed
-         into torch.nn.functional.
+         This method smooths an image with a Gaussian of specified sigma.  You can
+         do the same much faster by using the functionality programmed into
+         torch.nn.functional.
  
     (11) visualize_segmentation_in_pseudocolor()
  
-         After an image has been segmented, this method can be used to assign
-         a random color to each blob in the segmented output for a better
+         After an image has been segmented, this method can be used to assign a
+         random color to each blob in the segmented output for a better
          visualization of the segmentation.
  
     (12) visualize_segmentation_with_mean_gray()
  
-         If the visualization produced by the previous method appears too
-         chaotic, you can use this method to assign the mean color to each
-         each blob in the output of an image segmentation algorithm.  The mean
-         color is derived from the pixel values in the blob.
+         If the visualization produced by the previous method appears too chaotic,
+         you can use this method to assign the mean color to each each blob in the
+         output of an image segmentation algorithm.  The mean color is derived
+         from the pixel values in the blob.
  
     (13) extract_image_region_interactively_by_dragging_mouse()
  
          You can use this method to apply the graph-based segmentation and the
-         selective search algorithms to just a portion of your image.  This
-         method extract the portion you want.  You click at the upper left
-         corner of the rectangular portion of the image you are interested in
-         and you then drag the mouse pointer to the lower right corner.  Make
-         sure that you click on "save" and "exit" after you have delineated
-         the area.
+         selective search algorithms to just a portion of your image.  This method
+         extract the portion you want.  You click at the upper left corner of the
+         rectangular portion of the image you are interested in and you then drag
+         the mouse pointer to the lower right corner.  Make sure that you click on
+         "save" and "exit" after you have delineated the area.
  
     (14) extract_image_region_interactively_through_mouse_clicks()
  
-         This method allows a user to use a sequence of mouse clicks in order
-         to specify a region of the input image that should be subject to
-         further processing.  The mouse clicks taken together define a
-         polygon. The method encloses the polygonal region by a minimum
-         bounding rectangle, which then becomes the new input image for the
-         rest of processing.
+         This method allows a user to use a sequence of mouse clicks in order to
+         specify a region of the input image that should be subject to further
+         processing.  The mouse clicks taken together define a polygon. The method
+         encloses the polygonal region by a minimum bounding rectangle, which then
+         becomes the new input image for the rest of processing.
  
     (15) displaying_and_histogramming_images_in_batch1(image_dir, batch_size)
  
          This method is the first of three such methods in this module for
          illustrating the functionality of matplotlib for simultaneously
          displaying multiple images and the results obtained from them in a
          gridded arrangement.  The core idea in this method is to call
          "plt.subplots(2,batch_size)" to create 'batch_size' number of subplot
-         objects, called "axes", in the form of a '2xbatch_size' array. We use
-         the first row of this grid to display each image in its own subplot
-         object.  And we use the second row of the grid to display the
-         histograms of the corresponding images in the first row.
+         objects, called "axes", in the form of a '2xbatch_size' array. We use the
+         first row of this grid to display each image in its own subplot object.
+         And we use the second row of the grid to display the histograms of the
+         corresponding images in the first row.
  
     (16) displaying_and_histogramming_images_in_batch2(image_dir, batch_size)
  
          I now show a second approach to displaying multiple images and their
-         corresponding histograms in a gridded display.  In this method we
-         call on "torchvision.utils.make_grid()" to construct a grid for us.
-         The grid is created by giving an argument like "nrow=4" to it.  The
-         grid object returned by the call to make_grid() is a tensor unto
-         itself. Such a tensor object is converted into a numpy array so that
-         it can be displayed by matplotlib's "imshow()" function.
+         corresponding histograms in a gridded display.  In this method we call on
+         "torchvision.utils.make_grid
+()" to construct a grid for us.  The grid is
+         created by giving an argument like "nrow=4" to it.  The grid object
+         returned by the call to make_grid() is a tensor unto itself. Such a
+         tensor object is converted into a numpy array so that it can be displayed
+         by matplotlib's "imshow()" function.
  
     (17) displaying_and_histogramming_images_in_batch3(image_dir, batch_size)
  
          This method illustrates two things: (1) The syntax used for the
          'singular' version of the subplot function "plt.subplot()" ---
-         although I'll be doing so by actually calling "fig.add_subplot()".
-         And (2) How you can put together multiple multi-image plots by
-         creating multiple Figure objects.  'Figure' is the top-level
-         container of plots in matplotlib.  This method creates two separate
-         Figure objects, one as a container for all the images in a batch and
-         the other as a container for all the histograms for the images.  The
-         two Figure containers are displayed in two separate windows on your
-         computer screen.
+ although
+         I'll be doing so by actually calling "fig.add_subplot()".  And (2) How
+         you can put together multiple multi-image plots by creating multiple
+         Figure objects.  'Figure' is the top-level container of plots in
+         matplotlib.  This method creates two separate Figure objects, one as a
+         container for all the images in a batch and the other as a container for
+         all the histograms for the images.  The two Figure containers are
+         displayed in two separate windows on your computer screen.
+ 
  
 THE DATASETS INCLUDED:
  
     Download the archive
  
         datasets_for_RPG.tar.gz
  
-    through the link "Download the image datasets for RPG" at the main
-    webpage for this module and store the archive in the Examples directory
-    of your install of the module. Subsequently, execute the following
-    command in the Examples directory:
+    through the link "Download the image datasets for RPG" at the main webpage for
+    this module and store the archive in the ExamplesObjectDetection directory of
+    your install of the module. Subsequently, execute the following command in the
+    ExamplesObjectDetection directory:
  
         tar zxvf datasets_for_RPG.tar.gz
  
-    This command will create a 'data' subdirectory in the Examples directory
-    and deposit the following datasets in it:
+    This command will create a 'data' subdirectory in the ExamplesObjectDetection
+    directory and deposit the following datasets in it:
  
         Purdue_Dr_Eval_Dataset-clutter-10-noise-20-size-10000-train.gz
         Purdue_Dr_Eval_Dataset-clutter-10-noise-20-size-1000-test.gz
  
         Purdue_Dr_Eval_Multi_Dataset-clutter-10-noise-20-size-10000-train.gz
         Purdue_Dr_Eval_Multi_Dataset-clutter-10-noise-20-size-1000-test.gz
  
-    In the naming convention used for the archives, the string 'clutter-10'
-    means that each image will have a maximum of 10 clutter objects in it,
-    and the string 'noise-20' means that I have added 20% Gaussian noise to
-    each image. The string 'size-10000' means that the dataset consists of
-    '10,000' images.
+    In the naming convention used for the archives, the string 'clutter-
+10' means
+    that each image will have a maximum of 10 clutter objects in it, and the
+    string 'noise-20' means that I have added 20% Gaussian noise to each
+    image. The string 'size-10000' means that the dataset consists of '10,000'
+    images.
  
     The two "Multi" datasets named above are for experimenting with the YOLO
-    implementation in the module for multi-instance object detection in
-    images.  The datasets without the word "Multi" in their names are for
-    experimenting with single-instance detection --- but under circumstances
-    that are more difficult than discussed in my Week 7 Deep Learning Lecture
-    at Purdue.
- 
-    You will also find two smaller datasets in the overall archive that 
-    contain just 30 images each.  Those are for debugging your code.
- 
+    implementation in the module for multi-instance object detection in images.
+    The datasets without the word "Multi" in their names are for experimenting
+    with single-instance detection --- but under circumstances that are more
+    difficult than discussed in my Week 7 Deep Learning Lecture at Purdue.
+ 
+    You will also find two smaller datasets in the overall archive that contain
+    just 30 images each.  Those are for debugging your code.
+ 
+    ABOUT THE ANNOTATIONS IN THE DATASETS:
+ 
+    See the Slides 43 and 44 of the "Week 8: Multi-Instance Object Detection"
+    slides at the course website for a description of how the annotations are
+    organized for the dataset mentioned above.
  
  
 THE ExamplesObjectDetection DIRECTORY:
  
-    This directory contains the following two scripts related to object
-    detection in images:
+    This directory contains the following two scripts related to object detection
+    in images:
  
         single_instance_object_detection.py
  
         multi_instance_object_detection.py
  
-    The first script carries out single-instance detections in the images in
-    the PurdueDrEvalDataset dataset and the second script carries out
-    multi-instance detections in the PurdueDrEvalMultiDataset.  In the former
-    dataset, each 128x128 image has only one instance of a meaningful object
-    along with structured artifacts and 20% random noise.  And, in the latter
-    dataset, each image has up to five instances of meaningful objects along
-    with the structured artifacts and 20% random noise.
+    The first script carries out single-
+instance detections in the images in the
+    PurdueDrEvalDataset dataset and the second script carries out multi-
+instance
+    detections in the PurdueDrEvalMultiDataset.  In the former dataset, each
+    128x128 image has only one instance of a meaningful object along with
+    structured artifacts and 20% random noise.  And, in the latter dataset, each
+    image has up to five instances of meaningful objects along with the structured
+    artifacts and 20% random noise.
  
  
  
 THE ExamplesRegionProposals DIRECTORY:
  
     This directory contains the following scripts for showcasing graph-based
     algorithms for constructing region proposals:
@@ -642,67 +687,67 @@
  
         torchvision_some_basic_transformations.py    
  
         torchvision_based_image_processing.py
  
         multi_image_histogramming_and_display.py  
  
-    The Examples directory also illustrates the sort of region proposal
-    results you can obtain with the graph-based algorithms in this module.
-    The specific illustrations are in the following subdirectories of the
-    Examples directory:
+    The ExamplesRegionProposals directory also illustrates the sort of region
+    proposal results you can obtain with the graph-based algorithms in this
+    module.  The specific illustrations are in the following subdirectories of the
+    ExamplesRegionProposals directory:
  
-        Examples/color_blobs/
+        ExamplesRegionProposals/color_blobs/
  
-        Examples/mondrian/
+        ExamplesRegionProposals/mondrian/
  
-        Examples/wallpic2/
+        ExamplesRegionProposals/wallpic2/
  
     Each subdirectory contains at least the following two files:
  
         selective_search.py
  
         the image file specific for that subdirectory.
  
-    All you have to do is to execute selective_search.py in that directory to
-    see the results on the image in that directory.
+    All you have to do is to execute selective_search.py in that directory to see
+    the results on the image in that directory.
  
  
  
 BUGS:
  
-    Please notify the author if you encounter any bugs.  When sending
-    email, please place the string 'RegionProposalGenerator' in the
-    subject line to get past the author's spam filter.
+    Please notify the author if you encounter any bugs.  When sending email,
+    please place the string 'RegionProposalGenerator' in the subject line to get
+    past the author's spam filter.
  
  
 ABOUT THE AUTHOR:
  
-    The author, Avinash Kak, is a professor of Electrical and Computer
-    Engineering at Purdue University.  For all issues related to this
-    module, contact the author at kak@purdue.edu If you send email,
-    please place the string "RegionProposalGenerator" in your subject
-    line to get past the author's spam filter.
+    The author, Avinash Kak, is a professor of Electrical and Computer Engineering
+    at Purdue University.  For all issues related to this module, contact the
+    author at kak@purdue.edu If you send email, please place the string
+    "RegionProposalGenerator" in your subject line to get past the author's spam
+    filter.
  
 COPYRIGHT:
  
     Python Software Foundation License
  
-    Copyright 2022 Avinash Kak
+    Copyright 2023 Avinash Kak
  
 @endofdocs
  
-Imported Modules
-         torchvision.transforms.functional functools torch.optim       sys
-         PIL.Image                         glob      os                time
-         PIL.ImageDraw                     gzip      pickle            torch
-   � PIL.ImageFont                     logging   matplotlib.pyplot torchvision
-         PIL.ImageTk                       math      random            torchvision.utils
-         tkinter                           torch.nn  re                torchvision.transforms
-         copy                              numpy     signal
+Modules
+         torchvision.transforms.functional functools   os                time
+         PIL.Image                         glob        pickle            torch
+         PIL.ImageDraw                     logging     matplotlib.pyplot torchvision
+   � PIL.ImageFont                     math        random            torchvision.utils
+         PIL.ImageTk                       torch.nn    re                torchvision.transforms
+         tkinter                           numpy       signal
+         copy                              torch.optim sys
  
 Classes
            builtins.object
                  RegionProposalGenerator
           
          class RegionProposalGenerator(builtins.object)
              RegionProposalGenerator(*args, **kwargs)
@@ -1064,15 +1109,15 @@
                  startY = 0
  
 Functions
    �   ctrl_c_handler(signum, frame)
  
 p
          __author__ = 'Avinash Kak (kak@purdue.edu)'
-         __copyright__ = '(C) 2022 Avinash Kak. Python Software Foundation.'
-   � __date__ = '2022-April-16'
+         __copyright__ = '(C) 2023 Avinash Kak. Python Software Foundation.'
+   � __date__ = '2023-April-9'
          __url__ = 'https://engineering.purdue.edu/kak/distRPG/
-         RegionProposalGenerator-2.0.8.html'
-         __version__ = '2.0.8'
+         RegionProposalGenerator-2.1.0.html'
+         __version__ = '2.1.0'
  
 Author
    � Avinash Kak (kak@purdue.edu)
```

### Comparing `RegionProposalGenerator-2.0.8/RegionProposalGenerator.egg-info/PKG-INFO` & `RegionProposalGenerator-2.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 1.2
 Name: RegionProposalGenerator
-Version: 2.0.8
-Summary: An educational module for experimenting with single-instance and multi-instance object detection and for generating region proposals with graph-based algorithms
-Home-page: https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.0.8.html
+Version: 2.1.0
+Summary: An educational module for experimenting with the YOLO logic for multi-instance object detection and for generating region proposals with graph-based algorithms
+Home-page: https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.1.0.html
 Author: Avinash Kak
 Author-email: kak@purdue.edu
 Maintainer: Avinash Kak
 Maintainer-email: kak@purdue.edu
 License: Python Software Foundation License
-Download-URL: https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.0.8.tar.gz
+Download-URL: https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.1.0.tar.gz
 Description: 
         
         Consult the module API page at
         
-              https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.0.8.html
+              https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.1.0.html
         
         for all information related to this module, including information related
         to the latest changes to the code.  The page at the URL shown above lists
         all of the module functionality you can invoke in your own code.
         
         ::
```

### Comparing `RegionProposalGenerator-2.0.8/RegionProposalGenerator.egg-info/SOURCES.txt` & `RegionProposalGenerator-2.1.0/RegionProposalGenerator.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MANIFEST.in
 Makefile
 README
-RegionProposalGenerator-2.0.8.html
+RegionProposalGenerator-2.1.0.html
 setup.py
 ExamplesObjectDetection/README
 ExamplesObjectDetection/multi_instance_object_detection.py
 ExamplesObjectDetection/single_instance_object_detection.py
 ExamplesRegionProposals/README
 ExamplesRegionProposals/interactive_graph_based_segmentation.py
 ExamplesRegionProposals/selective_search.py
```

### Comparing `RegionProposalGenerator-2.0.8/TestRegionProposalGenerator/RegionProposalGenerator.py` & `RegionProposalGenerator-2.1.0/TestRegionProposalGenerator/RegionProposalGenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-__version__   = '2.0.8'
+# -*- coding: utf-8 -*-
+
+__version__   = '2.1.0'
 __author__    = "Avinash Kak (kak@purdue.edu)"
-__date__      = '2022-April-16'   
-__url__       = 'https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.0.8.html'
-__copyright__ = "(C) 2022 Avinash Kak. Python Software Foundation."
+__date__      = '2023-April-9'   
+__url__       = 'https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.1.0.html'
+__copyright__ = "(C) 2023 Avinash Kak. Python Software Foundation."
 
 
 __doc__ = '''
 
 RegionProposalGenerator.py
 
 Version: ''' + __version__ + '''
@@ -15,228 +17,227 @@
 
 Date: ''' + __date__ + '''
 
 
 @title
 CHANGE LOG:
 
+  Version 2.1.0:
+
+    With this version, you can now use batches of any size for YOLO learning.
+    Previously, the batch size was limited to 1 for the YOLO part of the module.
+    Allowing for batches required changes in the handling of problem images, such
+    as the images with no meaningful objects, or the images with object bounding
+    boxes with unrealistic aspect ratios.
+
   Version 2.0.8:
 
-    This version constitutes a complete implementation of a YOLO
-    multi-instance object detector.  In addition to the new multi-loss
-    function that I introduced in the previous public release of this module,
-    the new version includes a full-blown implementation of what you need for
-    validation testing.  I should also mention that I have split what used to
-    be the Examples directory in the distribution into two directories:
-    ExamplesObjectDetection and ExamplesRegionProposals.  Your entry point for
-    learning the YOLO implementation would be the script
-    multi_instance_object_detection.py in the directory
-    ExamplesObjectDetection.
+    This version constitutes a complete implementation of a YOLO multi-instance
+    object detector.  In addition to the new multi-loss function that I introduced
+    in the previous public release of this module, the new version includes a
+    full-blown implementation of what you need for validation testing.  I should
+    also mention that I have split what used to be the Examples directory in the
+    distribution into two directories: ExamplesObjectDetection and
+    ExamplesRegionProposals.  Your entry point for learning the YOLO
+    implementation would be the script multi_instance_object_detection.py in the
+    directory ExamplesObjectDetection.
     
   Version 2.0.6:
 
-    This version incorporates a more sophisticated loss function for
-    YOLO-based multi-instance object detection in images.  In the new loss
-    function, I use different criteria for the different segments of the YOLO
-    vector.  [Assigning an object instance in a training image to an anchor
-    box for a cell in the image involves creating a "5+C"-element YOLO vector,
-    where C is the number of object classes.] I now use the Binary
-    Cross-Entropy Loss (nn.BCELoss) for the first element of the YOLO vector
-    that stands for the presence or the absence of an object instance in a
-    specific anchor box in a specific cell.  I use mean-squared-error loss
-    (nn.MSELoss) for the next four numerical elements that express the precise
-    location of the object bounding-box vis-a-vis the center of the cell to
-    which the object is assigned and also for the dimensions of the bounding
-    box.  Finally, I use the regular Cross-Entropy loss (nn.CrossEntropyLoss)
-    for the last C elements of the YOLO vector.  Using the cross-entropy loss
-    for the labeling errors required augmenting the YOLO vector with one
-    additional element to express the absence of an object.
+    This version incorporates a more sophisticated loss function for YOLO-based
+    multi-instance object detection in images.  In the new loss function, I use
+    different criteria for the different segments of the YOLO vector.  [Assigning
+    an object instance in a training image to an anchor box for a cell in the
+    image involves creating a "5+C"-element YOLO vector, where C is the number of
+    object classes.] I now use the Binary Cross-Entropy Loss (nn.BCELoss) for the
+    first element of the YOLO vector that stands for the presence or the absence
+    of an object instance in a specific anchor box in a specific cell.  I use
+    mean-squared-error loss (nn.MSELoss) for the next four numerical elements that
+    express the precise location of the object bounding-box vis-a-vis the center
+    of the cell to which the object is assigned and also for the dimensions of the
+    bounding box.  Finally, I use the regular Cross-Entropy loss
+    (nn.CrossEntropyLoss) for the last C elements of the YOLO vector.  Using the
+    cross-entropy loss for the labeling errors required augmenting the YOLO vector
+    with one additional element to express the absence of an object.
 
   Version 2.0.2:
 
-    This version fixes a couple of bugs in the YOLO-based logic for
-    multi-instance object detection.
+    This version fixes a couple of bugs in the YOLO-based logic for multi-instance
+    object detection.
 
   Version 2.0.1:
 
     This module has gone through several changes since its last public-release
     version as I was experimenting with different ways of imparting to the
     students the sudden increase in model complexity as one goes from
-    single-instance object detection to multi-instance object detection.
-    These experiments led to the creation of two new datasets,
-    PurdueDrEvalDataset and PurdueDrEvalMultiDataset, the former for playing
-    with single-instance object detection and the latter for doing the same
-    with multi-instance object detection.  The module also includes two inner
-    classes, SingleInstanceDetector and YoloLikeDetector, the former a
-    reference implementation for single instance object detection and the
-    latter a YOLO-like reference implementation for multi-instance object
-    detection. [By the way, "DrEval" in the names of the two datasets
-    mentioned here has a connection with "Dr Evil" in the Austin Powers
-    movies.]
+    single-instance object detection to multi-instance object detection.  These
+    experiments led to the creation of two new datasets, PurdueDrEvalDataset and
+    PurdueDrEvalMultiDataset, the former for playing with single-instance object
+    detection and the latter for doing the same with multi-instance object
+    detection.  The module also includes two inner classes, SingleInstanceDetector
+    and YoloLikeDetector, the former a reference implementation for single
+    instance object detection and the latter a YOLO-like reference implementation
+    for multi-instance object detection. [By the way, "DrEval" in the names of the
+    two datasets mentioned here has a connection with "Dr Evil" in the Austin
+    Powers movies.]
 
   Version 1.0.5:
 
     In keeping with the tutorial nature of this module, this version includes
-    methods that come in handy for batch-based processing of images. These
-    methods carry names like "displaying_and_histogramming_
-    images_in_batchX()" where X is 1, 2, and 3.  The rest of the module,
-    especially the part that deals with constructing region proposals remains
-    unchanged.
+    methods that come in handy for batch-based processing of images. These methods
+    carry names like "displaying_and_histogramming_ images_in_batchX()" where X is
+    1, 2, and 3.  The rest of the module, especially the part that deals with
+    constructing region proposals remains unchanged.
 
   Version 1.0.4:
 
     This is the first public release version of the module.
 
 
 @title
 INTRODUCTION:
 
     Single-Instance vs. Multi-Instance Detection:
 
-    This module was created for experimenting with the logic of object
-    detection with neural networks.  On the face of it, object detection in
-    images sounds like a well-defined problem that should lend itself to
-    well-defined solutions.  Unfortunately, the reality is otherwise.  Yes,
-    simple examples of the problem -- such as when the images contain
-    single object instances and with no competing clutter in the background
-    -- the problem can be solved straightforwardly with a neural network.
-    However, the object detection problems that are encountered in real
-    life are rarely that simple.  A practically useful framework for object
-    detection must be able to recognize and localize all possible instances
-    of the objects of interest in a given image.
+    This module was created for experimenting with the logic of object detection
+    with neural networks.  On the face of it, object detection in images sounds
+    like a well-defined problem that should lend itself to well-defined solutions.
+    Unfortunately, the reality is otherwise.  Yes, simple examples of the problem
+    -- such as when the images contain single object instances and with no
+    competing clutter in the background -- the problem can be solved
+    straightforwardly with a neural network.  However, the object detection
+    problems that are encountered in real life are rarely that simple.  A
+    practically useful framework for object detection must be able to recognize
+    and localize all possible instances of the objects of interest in a given
+    image.
 
     So how does one solve the problem of multi-instance object detection and
     localization with a neural network?
 
     The last half-dozen years have seen the emergence of the following three
-    competition-grade neural-network based approaches for multi-instance
-    object detection: R-CNN, YOLO, and SSD.  The Preamble section of my Week 8
-    lecture for Purdue's Deep Learning class provides a brief overview of
-    these approaches.  YOLO stands for "You Only Look Once" --- in contrast
-    with R-CNN based approaches in which you may have to subject the images to
-    a couple of neural networks, one for generating region proposals and the
-    other for actual object detection.
-
-    The main goal of the present module is to provide an educational example
-    of a complete implementation of the YOLO logic for multi-instance object
-    detection in images.
+    competition-grade neural-network based approaches for multi-instance object
+    detection: R-CNN, YOLO, and SSD.  The Preamble section of my Week 8 lecture
+    for Purdue's Deep Learning class provides a brief overview of these
+    approaches.  YOLO stands for "You Only Look Once" --- in contrast with R-CNN
+    based approaches in which you may have to subject the images to a couple of
+    neural networks, one for generating region proposals and the other for actual
+    object detection.
+
+    The main goal of the present module is to provide an educational example of a
+    complete implementation of the YOLO logic for multi-instance object detection
+    in images.
 
     Graph-Based Algorithms for Region Proposals:
 
-    A second goal of this module is to provide implementations for a couple
-    of the more modern graph-based approaches for generating region
-    proposals.  At this point, the reader might ask: What is a region
-    proposal?  A region proposal is a blob of pixels that is highly likely
-    to contain an object instance.  Another way of saying same thing is
-    that region proposals are pixel blobs that look different from the
-    general background in the images.  While it is possible to use a neural
-    network for generating region proposals, as demonstrated by the success
-    of RPN (Region Proposal Network) in the R-CNN based multi-instance
+    A second goal of this module is to provide implementations for a couple of the
+    more modern graph-based approaches for generating region proposals.  At this
+    point, the reader might ask: What is a region proposal?  A region proposal is
+    a blob of pixels that is highly likely to contain an object instance.  Another
+    way of saying same thing is that region proposals are pixel blobs that look
+    different from the general background in the images.  While it is possible to
+    use a neural network for generating region proposals, as demonstrated by the
+    success of RPN (Region Proposal Network) in the R-CNN based multi-instance
     object detection, the RPG module is concerned primarily with the
-    non-neural-network based methods -- the graph-based methods -- for
-    generating region proposals.  I believe that becoming familiar with the
-    non-learning based methods for constructing region proposals still has
-    considerable value.  Consider, for example, the problem of detecting
-    objects in satellite images where you simply do not have access to the
-    amount of training data you would need for a neural-network based
-    approach to work.
-
-    With regard to the graph-based method for generating region proposals,
-    RPG (RegionProposalGenerator) implements elements of the Selective
-    Search (SS) algorithm for object detection as proposed by Uijlings, van
-    de Sande, Gevers, and Smeulders.  The Selective Search algorithm sits
-    on top of the graph-based image segmentation algorithm of Felzenszwalb
-    and Huttenlocher (FH) whose implementation is also included in the RPG
-    module.  The RPG module first processes an image with the FH
-    graph-based algorithm for image segmentation to divide an image into
-    pixel blobs.  The module subsequently invokes elements of the SS
-    algorithm to selectively merge the blobs on the basis of three
+    non-neural-network based methods -- the graph-based methods -- for generating
+    region proposals.  I believe that becoming familiar with the non-learning
+    based methods for constructing region proposals still has considerable value.
+    Consider, for example, the problem of detecting objects in satellite images
+    where you simply do not have access to the amount of training data you would
+    need for a neural-network based approach to work.
+
+    With regard to the graph-based method for generating region proposals, RPG
+    (RegionProposalGenerator) implements elements of the Selective Search (SS)
+    algorithm for object detection as proposed by Uijlings, van de Sande, Gevers,
+    and Smeulders.  The Selective Search algorithm sits on top of the graph-based
+    image segmentation algorithm of Felzenszwalb and Huttenlocher (FH) whose
+    implementation is also included in the RPG module.  The RPG module first
+    processes an image with the FH graph-based algorithm for image segmentation to
+    divide an image into pixel blobs.  The module subsequently invokes elements of
+    the SS algorithm to selectively merge the blobs on the basis of three
     properties: homogeneity of the color, grayscale variance, and texture
     homogeneity.
 
-    The FH algorithm is based on creating a graph-based representation of
-    an image in which, at the beginning, each pixel is a single vertex and
-    the edge between two vertices that stand for two adjacent pixels
-    represents the difference between some pixel property (such as the
-    color difference) at the two pixels.  Subsequently, for the vertex
-    merging logic, each vertex u, that after the first iteration stands for
-    a grouping of pixels, is characterized by a property called Int(u),
-    which is the largest value of the inter-pixel color difference between
-    the adjacent pixels.  In order to account for the fact that, at the
-    beginning, each vertex consists of only one pixel [which would not
-    allow for the calculation of Int(u)], the unary property of the pixels
-    at a vertex is extended from Int(u) to MInt(u) with the addition of a
-    vertex-size dependent number equal to k/|C| where "k" is a
-    user-specified parameter and |C| the cardinality of the set of pixels
-    represented by the vertex u in the graph.
-
-    As mentioned above, initially the edges in the graph representation of
-    an image are set to the color difference between the two 8-adjacent
-    pixels that correspond to two different vertices.  Subsequently, as the
-    vertices are merged, an edge, E(u,v), between two vertices u and v is
-    set to the smallest value of the inter-pixel color difference for two
-    adjacent pixels that belong to the two vertices. At each iteration of
-    the algorithm, two vertices u and v are merged provided E(u,v) is less
-    than the smaller of the MInt(u) or MInt(v) attributes at the two
-    vertices.  My experience is that for most images the algorithm
-    terminates of its own accord after a small number of iterations while
-    the vertex merging condition can be satisfied.
-
-    Since the algorithm is driven by the color differences between
-    8-adjacent pixels, the FH algorithm is likely to create too fine a
-    segmentation of an image.  The segments produced by FH can be made
-    larger by using the logic of SS that allows blobs of pixels to merge
-    into larger blobs provided doing so makes sense based on the inter-blob
-    values for mean color levels, color variances, texture values, etc.
+    The FH algorithm is based on creating a graph-based representation of an image
+    in which, at the beginning, each pixel is a single vertex and the edge between
+    two vertices that stand for two adjacent pixels represents the difference
+    between some pixel property (such as the color difference) at the two pixels.
+    Subsequently, for the vertex merging logic, each vertex u, that after the
+    first iteration stands for a grouping of pixels, is characterized by a
+    property called Int(u), which is the largest value of the inter-pixel color
+    difference between the adjacent pixels.  In order to account for the fact
+    that, at the beginning, each vertex consists of only one pixel [which would
+    not allow for the calculation of Int(u)], the unary property of the pixels at
+    a vertex is extended from Int(u) to MInt(u) with the addition of a vertex-size
+    dependent number equal to k/|C| where "k" is a user-specified parameter and
+    |C| the cardinality of the set of pixels represented by the vertex u in the
+    graph.
+
+    As mentioned above, initially the edges in the graph representation of an
+    image are set to the color difference between the two 8-adjacent pixels that
+    correspond to two different vertices.  Subsequently, as the vertices are
+    merged, an edge, E(u,v), between two vertices u and v is set to the smallest
+    value of the inter-pixel color difference for two adjacent pixels that belong
+    to the two vertices. At each iteration of the algorithm, two vertices u and v
+    are merged provided E(u,v) is less than the smaller of the MInt(u) or MInt(v)
+    attributes at the two vertices.  My experience is that for most images the
+    algorithm terminates of its own accord after a small number of iterations
+    while the vertex merging condition can be satisfied.
+
+    Since the algorithm is driven by the color differences between 8-adjacent
+    pixels, the FH algorithm is likely to create too fine a segmentation of an
+    image.  The segments produced by FH can be made larger by using the logic of
+    SS that allows blobs of pixels to merge into larger blobs provided doing so
+    makes sense based on the inter-blob values for mean color levels, color
+    variances, texture values, etc.
 
 
 @title
 INSTALLATION:
 
     The RegionProposalGenerator class was packaged using setuptools.  For
-    installation, execute the following command in the source directory
-    (this is the directory that contains the setup.py file after you have
-    downloaded and uncompressed the package):
+    installation, execute the following command in the source directory (this is
+    the directory that contains the setup.py file after you have downloaded and
+    uncompressed the package):
  
             sudo python3 setup.py install
 
-    On Linux distributions, this will install the module file at a location
-    that looks like
+    On Linux distributions, this will install the module file at a location that
+    looks like
 
              /usr/local/lib/python3.8/dist-packages/
 
-    If you do not have root access, you have the option of working directly
-    off the directory in which you downloaded the software by simply
-    placing the following statements at the top of your scripts that use
-    the RegionProposalGenerator class:
+    If you do not have root access, you have the option of working directly off
+    the directory in which you downloaded the software by simply placing the
+    following statements at the top of your scripts that use the
+    RegionProposalGenerator class:
 
             import sys
             sys.path.append( "pathname_to_RegionProposalGenerator_directory" )
 
-    To uninstall the module, simply delete the source directory, locate
-    where the RegionProposalGenerator module was installed with "locate
-    RegionProposalGenerator" and delete those files.  As mentioned above,
-    the full pathname to the installed version is likely to look like
+    To uninstall the module, simply delete the source directory, locate where the
+    RegionProposalGenerator module was installed with "locate
+    RegionProposalGenerator" and delete those files.  As mentioned above, the full
+    pathname to the installed version is likely to look like
     /usr/local/lib/python2.7/dist-packages/RegionProposalGenerator*
 
-    If you want to carry out a non-standard install of the
-    RegionProposalGenerator module, look up the on-line information on
-    Disutils by pointing your browser to
+    If you want to carry out a non-standard install of the RegionProposalGenerator
+    module, look up the on-line information on Disutils by pointing your browser
+    to
 
               http://docs.python.org/dist/dist.html
 
 @title
 USAGE:
 
     Single-Instance and Multi-Instance Detection:
 
-    If you wish to experiment with YOLO-like logic for multi-instance
-    object detection, you would need to construct an instance of the
-    RegionProposalGenerator class and invoke the methods shown below on
-    this instance:
+    If you wish to experiment with YOLO-like logic for multi-instance object
+    detection, you would need to construct an instance of the
+    RegionProposalGenerator class and invoke the methods shown below on this
+    instance:
 
     rpg = RegionProposalGenerator(
                       dataroot = "./data/",
                       image_size = [128,128],
                       yolo_interval = 20,
                       path_saved_yolo_model = "./saved_yolo_model",
                       momentum = 0.9,
@@ -252,17 +253,17 @@
     model = yolo.NetForYolo(skip_connections=True, depth=8) 
     model = yolo.run_code_for_training_multi_instance_detection(model, display_images=False)
     yolo.run_code_for_training_multi_instance_detection(model, display_images = True)
     
 
     Graph-Based Algorithms for Region Proposals:
 
-    To generate region proposals, you would need to construct an instance
-    of the RegionProposalGenerator class and invoke the methods shown below
-    on this instance:
+    To generate region proposals, you would need to construct an instance of the
+    RegionProposalGenerator class and invoke the methods shown below on this
+    instance:
 
         rpg = RegionProposalGenerator(
                        ###  The first 6 options affect only the Graph-Based part of the algo
                        sigma = 1.0,
                        max_iterations = 40,
                        kay = 0.05,
                        image_normalization_required = True,
@@ -280,352 +281,344 @@
         merged_blobs, color_map = rpg.selective_search_for_region_proposals( segmented_graph, image_name )
         rpg.visualize_segmentation_with_mean_gray(merged_blobs, "ss_based_segmentation_in_bw" )
 
 
 @title
 CONSTRUCTOR PARAMETERS: 
 
-    Of the 10 constructor parameters listed below, the first six are meant for
-    the FH algorithm and the last four for the SS algorithm.
+    Of the 10 constructor parameters listed below, the first six are meant for the
+    FH algorithm and the last four for the SS algorithm.
 
-    sigma: Controls the size of the Gaussian kernel used for smoothing the
-                    image before its gradient is calculated.  Assuming the
-                    pixel sampling interval to be unity, a sigma of 1 gives
-                    you a 7x7 smoothing operator with Gaussian weighting.
-                    The default for this parameter is 1.
+    sigma: Controls the size of the Gaussian kernel used for smoothing the image
+                    before its gradient is calculated.  Assuming the pixel
+                    sampling interval to be unity, a sigma of 1 gives you a 7x7
+                    smoothing operator with Gaussian weighting.  The default for
+                    this parameter is 1.
 
     max_iterations: Sets an upper limit on the number of iterations of the
                     graph-based FH algorithm for image segmentation.
 
-    kay: This is the same as the "k" parameter in the FH algorithm.  As
-                    mentioned in the Introduction above, the Int(u)
-                    property of the pixels represented by each vertex in
-                    the graph representation of the image is extended to
-                    MInt(u) by the addition of a number k/|C| where |C| is
-                    the cardinality of the set of pixels at that vertex.
-
-    image_normalization_required: This applies Torchvision's image
-                    normalization to the pixel values in the image.
-
-    image_size_reduction_factor: As mentioned at the beginning of this
-                    document, RegionProposalGenerator is really not meant
-                    for production work.  The code is pure Python and, even
-                    with that, not at all optimized.  The focus of the
-                    module is primarily on easy understandability of what
-                    the code is doing so that you can experiment with the
-                    algorithm itself.  For the module to produce results
-                    within a reasonable length of time, you can use this
-                    constructor parameter to downsize the array of pixels
-                    that the module must work with.  Set this parameter to
-                    a value so that the initial graph constructed from the
-                    image has no more than around 3500 vertices if you
-                    don't want to wait too long for the results.
-
-    min_size_for_graph_based_blobs: This declares a threshold on the
-                   smallest size you'd like to see (in terms of the number
-                   of pixels) in a segmented blob in the output of the
-                   graph-based segmenter.  (I typically use values from 1
-                   to 4 for this parameter.)
+    kay: This is the same as the "k" parameter in the FH algorithm.  As mentioned
+                    in the Introduction above, the Int(u) property of the pixels
+                    represented by each vertex in the graph representation of the
+                    image is extended to MInt(u) by the addition of a number k/|C|
+                    where |C| is the cardinality of the set of pixels at that
+                    vertex.
+
+    image_normalization_required: This applies Torchvision's image normalization
+                    to the pixel values in the image.
+
+    image_size_reduction_factor: As mentioned at the beginning of this document,
+                    RegionProposalGenerator is really not meant for production
+                    work.  The code is pure Python and, even with that, not at all
+                    optimized.  The focus of the module is primarily on easy
+                    understandability of what the code is doing so that you can
+                    experiment with the algorithm itself.  For the module to
+                    produce results within a reasonable length of time, you can
+                    use this constructor parameter to downsize the array of pixels
+                    that the module must work with.  Set this parameter to a value
+                    so that the initial graph constructed from the image has no
+                    more than around 3500 vertices if you don't want to wait too
+                    long for the results.
+
+    min_size_for_graph_based_blobs: This declares a threshold on the smallest size
+                   you'd like to see (in terms of the number of pixels) in a
+                   segmented blob in the output of the graph-based segmenter.  (I
+                   typically use values from 1 to 4 for this parameter.)
 
-    color_homogeneity_thresh:  
+    color_homogeneity_thresh:
 
                     This and the next three constructor options are meant
-                    specifically for the SS algorithm that sits on top of
-                    the FH algorithm for further merging of the pixel blobs
-                    produced by FH.  This constructor option specifies the
-                    maximum allowable difference between the mean color
-                    values in two pixel blobs for them to be merged.
+                    specifically for the SS algorithm that sits on top of the FH
+                    algorithm for further merging of the pixel blobs produced by
+                    FH.  This constructor option specifies the maximum allowable
+                    difference between the mean color values in two pixel blobs
+                    for them to be merged.
 
     gray_var_thresh:
 
-                   This option declares the maximum allowable difference in 
-                   the variances in the grayscale in two blobs if they are
-                   to be merged. 
+                   This option declares the maximum allowable difference in the
+                   variances in the grayscale in two blobs if they are to be
+                   merged.
 
     texture_homogeneity_thresh:
 
-                   The RegionProposalGenerator module characterizes the
-                   texture of the pixels in each segmented blob by its LBP
-                   (Local Binary Patterns) texture.  We want the LBP
-                   texture values for two different blobs to be within the
-                   value specified by this constructor option if those
-                   blobs are to be merged.
+                   The RegionProposalGenerator module characterizes the texture of
+                   the pixels in each segmented blob by its LBP (Local Binary
+                   Patterns) texture.  We want the LBP texture values for two
+                   different blobs to be within the value specified by this
+                   constructor option if those blobs are to be merged.
 
     max_num_blobs_expected:
 
-                   If you only want to extract a certain number of the
-                   largest possible blobs, you can do that by giving a
-                   value to this constructor option.
+                   If you only want to extract a certain number of the largest
+                   possible blobs, you can do that by giving a value to this
+                   constructor option.
 
 
 @title
 Inner Classes:
 
     (1)  PurdueDrEvalDataset
 
-         This is the dataset to use if you are experimenting with
-         single-instance object detection.  The dataset contains three
-         kinds of objects in its images: Dr. Eval, and two "objects" in his
-         neighborhood: a house and a watertower.  Each 128x128 image in the
-         dataset contains one of these objects after it is randomly scaled
-         and colored. Each image also contains substantial structured noise
-         in addition to 20% Gaussian noise.  Examples of these images are
-         shown in the Week 8 lecture material in Purdue's Deep Learning
-         class.
+         This is the dataset to use if you are experimenting with single-instance
+         object detection.  The dataset contains three kinds of objects in its
+         images: Dr. Eval, and two "objects" in his neighborhood: a house and a
+         watertower.  Each 128x128 image in the dataset contains one of these
+         objects after it is randomly scaled and colored. Each image also contains
+         substantial structured noise in addition to 20% Gaussian noise.  Examples
+         of these images are shown in the Week 8 lecture material in Purdue's Deep
+         Learning class.
 
     (2)  PurdueDrEvalMultiDataset
 
-         This is the dataset to use if you are experimenting with
-         multi-instance object detection.  Each image in the dataset
-         contains randomly chosen multiple instances of the same three
-         kinds of objects as mentioned above: Dr. Eval, house, and
-         watertower.  The number of object instances in each image is
-         limited to a maximum of five.  The images contain substantial
+         This is the dataset to use if you are experimenting with multi-instance
+         object detection.  Each image in the dataset contains randomly chosen
+         multiple instances of the same three kinds of objects as mentioned above:
+         Dr. Eval, house, and watertower.  The number of object instances in each
+         image is limited to a maximum of five.  The images contain substantial
          amount of structured noise in addition to 20% random noise.
          
-         The reason for why the above two datasets have "DrEval" in their
-         names: After having watched every contemporary movie at Netflix
-         that was worth watching, my wife and I decided to revisit some of
-         old movies that we had enjoyed a long time back.  That led us to
-         watching again a couple of Austin Powers movies.  If you are too
-         young to know what I am talking about, these movies are spoofs on
-         the James Bond movies in which the great comedian Mike Myers plays
-         both Austin Powers and his nemesis Dr. Evil.  Around the same
-         time, I was writing code for the two datasets mentioned above.
-         One of the three objects types in these images is a human-like
-         cartoon figure that I needed a name for.  So, after Dr. Evil in
-         the movies, I decided to call this cartoon figure Dr Eval and to
-         refer to the datasets as Dr Eval datasets. As you all know, "Eval"
-         is an important word for people like us.  All programming
-         languages provide a function with a name like "eval()".
+         The reason for why the above two datasets have "DrEval" in their names:
+         After having watched every contemporary movie at Netflix that was worth
+         watching, my wife and I decided to revisit some of old movies that we had
+         enjoyed a long time back.  That led us to watching again a couple of
+         Austin Powers movies.  If you are too young to know what I am talking
+         about, these movies are spoofs on the James Bond movies in which the
+         great comedian Mike Myers plays both Austin Powers and his nemesis
+         Dr. Evil.  Around the same time, I was writing code for the two datasets
+         mentioned above.  One of the three objects types in these images is a
+         human-like cartoon figure that I needed a name for.  So, after Dr. Evil
+         in the movies, I decided to call this cartoon figure Dr Eval and to refer
+         to the datasets as Dr Eval datasets. As you all know, "Eval" is an
+         important word for people like us.  All programming languages provide a
+         function with a name like "eval()".
 
     (3)  SingleInstanceDetector
 
          This provides a reference implementation for constructing a
-         single-instance object detector to be used for the
-         PurdueDrEvalDataset dataset. For the detection and regression
-         network, it uses the LOADnet2 network from DLStudio with small
-         modifications to account for the larger 128x128 images in the
-         dataset.
+         single-instance object detector to be used for the PurdueDrEvalDataset
+         dataset. For the detection and regression network, it uses the LOADnet2
+         network from DLStudio with small modifications to account for the larger
+         128x128 images in the dataset.
 
     (4)  YoloLikeDetector   [For multi-instance detection]
 
          The code in this inner class provides an implementation for the key
          elements of the YOLO logic for multi-instance object detection.  Each
          training image is divided into a grid of cells and it is the
          responsibility of the cell that contains the center of an object
-         bounding-box to provide at the output of the neural network an
-         estimate for the exact location of the center of the object bounding
-         box vis-a-vis the center of the cell.  That cell must also lead to an
-         estimate for the height and the width of the bounding-box for the
-         object instance.
+         bounding-box to provide at the output of the neural network an estimate
+         for the exact location of the center of the object bounding box vis-a-vis
+         the center of the cell.  That cell must also lead to an estimate for the
+         height and the width of the bounding-box for the object instance.
 
 
 @title
 PUBLIC METHODS:
 
-    Many of these method are related to using this module for experimenting
-    with the traditional graph-based algorithms for constructing region
-    proposals in images:
+    Many of these method are related to using this module for experimenting with
+    the traditional graph-based algorithms for constructing region proposals in
+    images:
 
     (1)  selective_search_for_region_proposals()
 
-         This method implements elements of the Selective Search (SS)
-         algorithm proposed by Uijlings, van de Sande, Gevers, and Smeulders
-         for creating region proposals for object detection.  As mentioned
-         elsewhere here, this algorithm sits on top of the graph based image
-         segmentation algorithm that was proposed by Felzenszwalb and
-         Huttenlocher.
+         This method implements elements of the Selective Search (SS) algorithm
+         proposed by Uijlings, van de Sande, Gevers, and Smeulders for creating
+         region proposals for object detection.  As mentioned elsewhere here, this
+         algorithm sits on top of the graph based image segmentation algorithm
+         that was proposed by Felzenszwalb and Huttenlocher.
 
     (2)  graph_based_segmentation()
 
          This is an implementation of the Felzenszwalb and Huttenlocher (FH)
-         algorithm for graph-based segmentation of images.  At the moment, it
-         is limited to working on grayscale images.
+         algorithm for graph-based segmentation of images.  At the moment, it is
+         limited to working on grayscale images.
 
     (3)  display_tensor_as_image()
 
-         This method converts the argument tensor into a photo image that you
-         can display in your terminal screen. It can convert tensors of three
-         different shapes into images: (3,H,W), (1,H,W), and (H,W), where H,
-         for height, stands for the number of pixel in the vertical direction
-         and W, for width, the same along the horizontal direction. When the
-         first element of the shape is 3, that means that the tensor
-         represents a color image in which each pixel in the (H,W) plane has
-         three values for the three color channels.  On the other hand, when
-         the first element is 1, that stands for a tensor that will be shown
-         as a grayscale image.  And when the shape is just (H,W), that is
-         automatically taken to be for a grayscale image.
+         This method converts the argument tensor into a photo image that you can
+         display in your terminal screen. It can convert tensors of three
+         different shapes into images: (3,H,W), (1,H,W), and (H,W), where H, for
+         height, stands for the number of pixel in the vertical direction and W,
+         for width, the same along the horizontal direction. When the first
+         element of the shape is 3, that means that the tensor represents a color
+         image in which each pixel in the (H,W) plane has three values for the
+         three color channels.  On the other hand, when the first element is 1,
+         that stands for a tensor that will be shown as a grayscale image.  And
+         when the shape is just (H,W), that is automatically taken to be for a
+         grayscale image.
 
     (4)  graying_resizing_binarizing()
 
-         This is a demonstration of some of the more basic and commonly used
-         image transformations from the torchvision.transformations module.
-         The large comment blocks are meant to serve as tutorial introduction
-         to the syntax used for invoking these transformations.  The
-         transformations shown can be used for converting a color image into a
-         grayscale image, for resizing an image, for converting a PIL.Image
-         into a tensor and a tensor back into an PIL.Image object, and so on.
+         This is a demonstration of some of the more basic and commonly used image
+         transformations from the torchvision.transformations module.  The large
+         comment blocks are meant to serve as tutorial introduction to the syntax
+         used for invoking these transformations.  The transformations shown can
+         be used for converting a color image into a grayscale image, for resizing
+         an image, for converting a PIL.Image into a tensor and a tensor back into
+         an PIL.Image object, and so on.
 
     (5)  accessing_one_color_plane()
 
          This method shows how can access the n-th color plane of the argument
          color image.
 
     (6)  working_with_hsv_color_space()
 
-         Illustrates converting an RGB color image into its HSV
-         representation.
+         Illustrates converting an RGB color image into its HSV representation.
 
     (7)  histogramming_the_image()
 
-         PyTorch based experiments with histogramming the grayscale and the
-         color values in an image
+         PyTorch based experiments with histogramming the grayscale and the color
+         values in an image
 
     (8)  histogramming_and_thresholding():
 
-         This method illustrates using the PyTorch functionality for
-         histogramming and thresholding individual images.
+         This method illustrates using the PyTorch functionality for histogramming
+         and thresholding individual images.
 
     (9)  convolutions_with_pytorch()
 
          This method calls on torch.nn.functional.conv2d() for demonstrating a
          single image convolution with a specified kernel.
 
     (10) gaussian_smooth()
 
-         This method smooths an image with a Gaussian of specified sigma.  You
-         can do the same much faster by using the functionality programmed
-         into torch.nn.functional.
+         This method smooths an image with a Gaussian of specified sigma.  You can
+         do the same much faster by using the functionality programmed into
+         torch.nn.functional.
 
     (11) visualize_segmentation_in_pseudocolor()
 
-         After an image has been segmented, this method can be used to assign
-         a random color to each blob in the segmented output for a better
+         After an image has been segmented, this method can be used to assign a
+         random color to each blob in the segmented output for a better
          visualization of the segmentation.
 
     (12) visualize_segmentation_with_mean_gray()
 
-         If the visualization produced by the previous method appears too
-         chaotic, you can use this method to assign the mean color to each
-         each blob in the output of an image segmentation algorithm.  The mean
-         color is derived from the pixel values in the blob.
+         If the visualization produced by the previous method appears too chaotic,
+         you can use this method to assign the mean color to each each blob in the
+         output of an image segmentation algorithm.  The mean color is derived
+         from the pixel values in the blob.
 
     (13) extract_image_region_interactively_by_dragging_mouse()
 
          You can use this method to apply the graph-based segmentation and the
-         selective search algorithms to just a portion of your image.  This
-         method extract the portion you want.  You click at the upper left
-         corner of the rectangular portion of the image you are interested in
-         and you then drag the mouse pointer to the lower right corner.  Make
-         sure that you click on "save" and "exit" after you have delineated
-         the area.
+         selective search algorithms to just a portion of your image.  This method
+         extract the portion you want.  You click at the upper left corner of the
+         rectangular portion of the image you are interested in and you then drag
+         the mouse pointer to the lower right corner.  Make sure that you click on
+         "save" and "exit" after you have delineated the area.
 
     (14) extract_image_region_interactively_through_mouse_clicks()
 
-         This method allows a user to use a sequence of mouse clicks in order
-         to specify a region of the input image that should be subject to
-         further processing.  The mouse clicks taken together define a
-         polygon. The method encloses the polygonal region by a minimum
-         bounding rectangle, which then becomes the new input image for the
-         rest of processing.
+         This method allows a user to use a sequence of mouse clicks in order to
+         specify a region of the input image that should be subject to further
+         processing.  The mouse clicks taken together define a polygon. The method
+         encloses the polygonal region by a minimum bounding rectangle, which then
+         becomes the new input image for the rest of processing.
 
     (15) displaying_and_histogramming_images_in_batch1(image_dir, batch_size)
 
          This method is the first of three such methods in this module for
          illustrating the functionality of matplotlib for simultaneously
          displaying multiple images and the results obtained from them in a
          gridded arrangement.  The core idea in this method is to call
          "plt.subplots(2,batch_size)" to create 'batch_size' number of subplot
-         objects, called "axes", in the form of a '2xbatch_size' array. We use
-         the first row of this grid to display each image in its own subplot
-         object.  And we use the second row of the grid to display the
-         histograms of the corresponding images in the first row.
+         objects, called "axes", in the form of a '2xbatch_size' array. We use the
+         first row of this grid to display each image in its own subplot object.
+         And we use the second row of the grid to display the histograms of the
+         corresponding images in the first row.
 
     (16) displaying_and_histogramming_images_in_batch2(image_dir, batch_size)
 
          I now show a second approach to displaying multiple images and their
-         corresponding histograms in a gridded display.  In this method we
-         call on "torchvision.utils.make_grid()" to construct a grid for us.
-         The grid is created by giving an argument like "nrow=4" to it.  The
-         grid object returned by the call to make_grid() is a tensor unto
-         itself. Such a tensor object is converted into a numpy array so that
-         it can be displayed by matplotlib's "imshow()" function.
+         corresponding histograms in a gridded display.  In this method we call on
+         "torchvision.utils.make_grid()" to construct a grid for us.  The grid is
+         created by giving an argument like "nrow=4" to it.  The grid object
+         returned by the call to make_grid() is a tensor unto itself. Such a
+         tensor object is converted into a numpy array so that it can be displayed
+         by matplotlib's "imshow()" function.
 
     (17) displaying_and_histogramming_images_in_batch3(image_dir, batch_size)
 
          This method illustrates two things: (1) The syntax used for the
-         'singular' version of the subplot function "plt.subplot()" ---
-         although I'll be doing so by actually calling "fig.add_subplot()".
-         And (2) How you can put together multiple multi-image plots by
-         creating multiple Figure objects.  'Figure' is the top-level
-         container of plots in matplotlib.  This method creates two separate
-         Figure objects, one as a container for all the images in a batch and
-         the other as a container for all the histograms for the images.  The
-         two Figure containers are displayed in two separate windows on your
-         computer screen.
+         'singular' version of the subplot function "plt.subplot()" --- although
+         I'll be doing so by actually calling "fig.add_subplot()".  And (2) How
+         you can put together multiple multi-image plots by creating multiple
+         Figure objects.  'Figure' is the top-level container of plots in
+         matplotlib.  This method creates two separate Figure objects, one as a
+         container for all the images in a batch and the other as a container for
+         all the histograms for the images.  The two Figure containers are
+         displayed in two separate windows on your computer screen.
+
 
 @title
 THE DATASETS INCLUDED:
 
     Download the archive
 
         datasets_for_RPG.tar.gz
 
-    through the link "Download the image datasets for RPG" at the main
-    webpage for this module and store the archive in the Examples directory
-    of your install of the module. Subsequently, execute the following
-    command in the Examples directory:
+    through the link "Download the image datasets for RPG" at the main webpage for
+    this module and store the archive in the ExamplesObjectDetection directory of
+    your install of the module. Subsequently, execute the following command in the
+    ExamplesObjectDetection directory:
 
         tar zxvf datasets_for_RPG.tar.gz
 
-    This command will create a 'data' subdirectory in the Examples directory
-    and deposit the following datasets in it:
+    This command will create a 'data' subdirectory in the ExamplesObjectDetection
+    directory and deposit the following datasets in it:
 
         Purdue_Dr_Eval_Dataset-clutter-10-noise-20-size-10000-train.gz
         Purdue_Dr_Eval_Dataset-clutter-10-noise-20-size-1000-test.gz
 
         Purdue_Dr_Eval_Multi_Dataset-clutter-10-noise-20-size-10000-train.gz
         Purdue_Dr_Eval_Multi_Dataset-clutter-10-noise-20-size-1000-test.gz
 
-    In the naming convention used for the archives, the string 'clutter-10'
-    means that each image will have a maximum of 10 clutter objects in it,
-    and the string 'noise-20' means that I have added 20% Gaussian noise to
-    each image. The string 'size-10000' means that the dataset consists of
-    '10,000' images.
+    In the naming convention used for the archives, the string 'clutter-10' means
+    that each image will have a maximum of 10 clutter objects in it, and the
+    string 'noise-20' means that I have added 20% Gaussian noise to each
+    image. The string 'size-10000' means that the dataset consists of '10,000'
+    images.
 
     The two "Multi" datasets named above are for experimenting with the YOLO
-    implementation in the module for multi-instance object detection in
-    images.  The datasets without the word "Multi" in their names are for
-    experimenting with single-instance detection --- but under circumstances
-    that are more difficult than discussed in my Week 7 Deep Learning Lecture
-    at Purdue.
-
-    You will also find two smaller datasets in the overall archive that 
-    contain just 30 images each.  Those are for debugging your code.
-
+    implementation in the module for multi-instance object detection in images.
+    The datasets without the word "Multi" in their names are for experimenting
+    with single-instance detection --- but under circumstances that are more
+    difficult than discussed in my Week 7 Deep Learning Lecture at Purdue.
+
+    You will also find two smaller datasets in the overall archive that contain
+    just 30 images each.  Those are for debugging your code.
+
+    ABOUT THE ANNOTATIONS IN THE DATASETS:
+
+    See the Slides 43 and 44 of the "Week 8: Multi-Instance Object Detection"
+    slides at the course website for a description of how the annotations are
+    organized for the dataset mentioned above.
 
 
 @title 
 THE ExamplesObjectDetection DIRECTORY:
 
-    This directory contains the following two scripts related to object
-    detection in images:
+    This directory contains the following two scripts related to object detection
+    in images:
 
         single_instance_object_detection.py
 
         multi_instance_object_detection.py
 
-    The first script carries out single-instance detections in the images in
-    the PurdueDrEvalDataset dataset and the second script carries out
-    multi-instance detections in the PurdueDrEvalMultiDataset.  In the former
-    dataset, each 128x128 image has only one instance of a meaningful object
-    along with structured artifacts and 20% random noise.  And, in the latter
-    dataset, each image has up to five instances of meaningful objects along
-    with the structured artifacts and 20% random noise.
+    The first script carries out single-instance detections in the images in the
+    PurdueDrEvalDataset dataset and the second script carries out multi-instance
+    detections in the PurdueDrEvalMultiDataset.  In the former dataset, each
+    128x128 image has only one instance of a meaningful object along with
+    structured artifacts and 20% random noise.  And, in the latter dataset, each
+    image has up to five instances of meaningful objects along with the structured
+    artifacts and 20% random noise.
 
 
 
 @title 
 THE ExamplesRegionProposals DIRECTORY:
 
     This directory contains the following scripts for showcasing graph-based
@@ -637,59 +630,59 @@
 
         torchvision_some_basic_transformations.py    
 
         torchvision_based_image_processing.py
 
         multi_image_histogramming_and_display.py  
 
-    The Examples directory also illustrates the sort of region proposal
-    results you can obtain with the graph-based algorithms in this module.
-    The specific illustrations are in the following subdirectories of the
-    Examples directory:
+    The ExamplesRegionProposals directory also illustrates the sort of region
+    proposal results you can obtain with the graph-based algorithms in this
+    module.  The specific illustrations are in the following subdirectories of the
+    ExamplesRegionProposals directory:
 
-        Examples/color_blobs/
+        ExamplesRegionProposals/color_blobs/
 
-        Examples/mondrian/
+        ExamplesRegionProposals/mondrian/
 
-        Examples/wallpic2/
+        ExamplesRegionProposals/wallpic2/
 
     Each subdirectory contains at least the following two files:
 
         selective_search.py
 
         the image file specific for that subdirectory.
 
-    All you have to do is to execute selective_search.py in that directory to
-    see the results on the image in that directory.
+    All you have to do is to execute selective_search.py in that directory to see
+    the results on the image in that directory.
 
 
 
 @title
 BUGS:
 
-    Please notify the author if you encounter any bugs.  When sending
-    email, please place the string 'RegionProposalGenerator' in the
-    subject line to get past the author's spam filter.
+    Please notify the author if you encounter any bugs.  When sending email,
+    please place the string 'RegionProposalGenerator' in the subject line to get
+    past the author's spam filter.
 
 
 @title
 ABOUT THE AUTHOR:
 
-    The author, Avinash Kak, is a professor of Electrical and Computer
-    Engineering at Purdue University.  For all issues related to this
-    module, contact the author at kak@purdue.edu If you send email,
-    please place the string "RegionProposalGenerator" in your subject
-    line to get past the author's spam filter.
+    The author, Avinash Kak, is a professor of Electrical and Computer Engineering
+    at Purdue University.  For all issues related to this module, contact the
+    author at kak@purdue.edu If you send email, please place the string
+    "RegionProposalGenerator" in your subject line to get past the author's spam
+    filter.
 
 @title
 COPYRIGHT:
 
     Python Software Foundation License
 
-    Copyright 2022 Avinash Kak
+    Copyright 2023 Avinash Kak
 
 @endofdocs
 '''
 
 import torch
 import torch.nn as nn
 import torchvision
@@ -706,15 +699,14 @@
 from PIL import ImageFont
 import sys,os,os.path,glob,signal
 import re
 import functools
 import math
 import random
 import copy
-import gzip
 import pickle
 if sys.version_info[0] == 3:
     import tkinter as Tkinter
     from tkinter.constants import *
 else:
     import Tkinter    
     from Tkconstants import *
@@ -879,15 +871,14 @@
         if 'max_iterations' in kwargs                :   max_iterations=kwargs.pop('max_iterations')
         if 'color_homogeneity_thresh' in kwargs      :   color_homogeneity_thresh = kwargs.pop('color_homogeneity_thresh')
         if 'gray_var_thresh' in kwargs               :    gray_var_thresh = kwargs.pop('gray_var_thresh')
         if 'texture_homogeneity_thresh' in kwargs    :   texture_homogeneity_thresh = kwargs.pop('texture_homogeneity_thresh')
         if 'min_size_for_graph_based_blobs' in kwargs :  min_size_for_graph_based_blobs = kwargs.pop('min_size_for_graph_based_blobs')
         if 'max_num_blobs_expected' in kwargs        :  max_num_blobs_expected = kwargs.pop('max_num_blobs_expected')
         if 'debug' in kwargs                         :   debug = kwargs.pop('debug') 
-#        if len(kwargs) != 0: raise ValueError('''You have provided unrecognizable keyword args''')
         if dataroot_train:
             self.dataroot_train = dataroot_train
         if dataroot_test:
             self.dataroot_test = dataroot_test
         if image_size:   
             self.image_size = image_size      
         if  path_saved_RPN_model:
@@ -896,15 +887,14 @@
             self.path_saved_single_instance_detector_model = path_saved_single_instance_detector_model
         if  path_saved_yolo_model:
             self.path_saved_yolo_model = path_saved_yolo_model
         if yolo_interval:
             self.yolo_interval = yolo_interval
         if classes:
             self.class_labels = classes
-#            self.class_labels_to_index = {label : classes.index(label) for label in classes}
         if learning_rate:
             self.learning_rate = learning_rate
         else:
             self.learning_rate = 1e-6
         if momentum:
             self.momentum = momentum
         if epochs:
@@ -914,16 +904,16 @@
         if use_gpu is not None:
             self.use_gpu = use_gpu
             if use_gpu is True:
                 if torch.cuda.is_available():
                     self.device = torch.device("cuda:0")
                 else:
                     raise Exception("You requested GPU support, but there's no GPU on this machine")
-            else:
-                self.device = torch.device("cpu")
+        else:
+            self.device = torch.device("cpu")
         if debug_train:                             
             self.debug_train = debug_train
         else:
             self.debug_train = 0
         if debug_test:                             
             self.debug_test = debug_test
         else:
@@ -1034,15 +1024,15 @@
             self.dataroot_train = dataroot_train
             self.dataroot_test  = dataroot_test
             self.database_train = {}
             self.database_test = {}
             self.dataset_size_train = None
             self.dataset_size_test = None
             if train_or_test == 'train':
-                self.training_dataset = self.index_dataset()
+                self.training_dataset = self.index_dataset()                  ### index_dataset() does NOT NOT NOT NOT return anything.  Only side effect used
             if train_or_test == 'test':
                 self.testing_dataset = self.index_dataset()
             self.class_labels = None
 
         def index_dataset(self):
             if self.train_or_test == 'train':
                 dataroot = self.dataroot_train
@@ -1524,17 +1514,17 @@
                     bbox_tensor = bbox_tensor.to(self.rpg.device)
                     optimizer.zero_grad()
                     outputs = net(im_tensor)
                     outputs_label = outputs[0]
                     bbox_pred = outputs[1]
                     bbox_gt = bbox_tensor
                     if i % 500 == 499:
-                        inputs_copy = im_tensor.detach().clone()
+                        inputs_copy = im_tensor.detach()
                         inputs_copy = inputs_copy.cpu()
-                        bbox_pc = bbox_pred.detach().clone()
+                        bbox_pc = bbox_pred.detach()
                         bbox_pc[bbox_pc<0] = 0
                         bbox_pc[bbox_pc>127] = 127
                         bbox_pc[torch.isnan(bbox_pc)] = 0
                         _, predicted = torch.max(outputs_label.data, 1)
                         print("[epoch:%d/%d  iter=%4d  elapsed_time=%5d secs]   Predicted Labels: " % 
                          (epoch+1, self.rpg.epochs, i+1, elapsed_time) + 
                          ' '.join('%15s' % self.rpg.class_labels[predicted[j].item()] for j in range(self.rpg.batch_size)))
@@ -1545,22 +1535,22 @@
                             j2 = int(bbox_gt[idx][2])
                             k1 = int(bbox_pc[idx][1])
                             k2 = int(bbox_pc[idx][3])
                             l1 = int(bbox_pc[idx][0])
                             l2 = int(bbox_pc[idx][2])
                             print("                    gt_bb:  [%d,%d,%d,%d]"%(j1,i1,j2,i2))
                             print("                  pred_bb:  [%d,%d,%d,%d]"%(l1,k1,l2,k2))
-                            inputs_copy[idx,0,i1:i2,j1] = 255
-                            inputs_copy[idx,0,i1:i2,j2] = 255
-                            inputs_copy[idx,0,i1,j1:j2] = 255
-                            inputs_copy[idx,0,i2,j1:j2] = 255
-                            inputs_copy[idx,2,k1:k2,l1] = 255                      
-                            inputs_copy[idx,2,k1:k2,l2] = 255
-                            inputs_copy[idx,2,k1,l1:l2] = 255
-                            inputs_copy[idx,2,k2,l1:l2] = 255
+                            inputs_copy[idx,1,i1:i2,j1] = 255
+                            inputs_copy[idx,1,i1:i2,j2] = 255
+                            inputs_copy[idx,1,i1,j1:j2] = 255
+                            inputs_copy[idx,1,i2,j1:j2] = 255
+                            inputs_copy[idx,0,k1:k2,l1] = 255                      
+                            inputs_copy[idx,0,k1:k2,l2] = 255
+                            inputs_copy[idx,0,k1,l1:l2] = 255
+                            inputs_copy[idx,0,k2,l1:l2] = 255
                     loss_labeling = criterion1(outputs_label, image_label)
                     loss_labeling.backward(retain_graph=True)        
                     loss_regression = criterion2(bbox_pred, bbox_tensor)
                     loss_regression.backward()
                     optimizer.step()
                     running_loss_labeling += loss_labeling.item()    
                     running_loss_regression += loss_regression.item()                
@@ -1758,16 +1748,16 @@
                 dataserver_train = RegionProposalGenerator.PurdueDrEvalMultiDataset(self.rpg, 
                                                        "train", dataroot_train=self.rpg.dataroot_train)
                 self.train_dataloader = torch.utils.data.DataLoader(dataserver_train, 
                                                       self.rpg.batch_size, shuffle=True, num_workers=4)
             if test:
                 dataserver_test = RegionProposalGenerator.PurdueDrEvalMultiDataset(self.rpg, 
                                                           "test", dataroot_test=self.rpg.dataroot_test)
-                self.test_dataloader = torch.utils.data.DataLoader(dataserver_test, 
-                                                     self.rpg.batch_size, shuffle=False, num_workers=4)
+                ## In the statement below, 1 is for the batch_size for testing
+                self.test_dataloader = torch.utils.data.DataLoader(dataserver_test, 1, shuffle=False)
 
         def check_dataloader(self, how_many_batches_to_show, train=False, test=False):
             if train:      
                 dataloader = self.train_dataloader
             if test:
                 dataloader = self.test_dataloader
             for idx, data in enumerate(dataloader): 
@@ -1948,15 +1938,14 @@
                 self.skip256ds = RegionProposalGenerator.YoloLikeDetector.SkipBlock(256,256,
                                                                     downsample=True, skip_connections=skip_connections)
                 self.fc_seqn = nn.Sequential(
                     nn.Linear(8192, 4096),
                     nn.ReLU(inplace=True),
                     nn.Linear(4096, 2048),
                     nn.ReLU(inplace=True),
-#                    nn.Linear(2048, 1440)
                     nn.Linear(2048, 1620)
                 )
 
             def forward(self, x):
                 x = self.pool(torch.nn.functional.relu(self.conv1(x)))          
                 x = nn.MaxPool2d(2,2)(torch.nn.functional.relu(self.conv2(x)))       
                 for i,skip64 in enumerate(self.skip64_arr[:self.depth//4]):
@@ -1997,268 +1986,269 @@
                 self.adx = adx
             def __str__(self):
                 return "AnchorBox type (h/w): %s    tlc for yolo cell: %s    anchor-box height: %d     \
                    anchor-box width: %d   adx: %d" % (self.AR, str(self.tlc), self.ab_height, self.ab_width, self.adx)
 
     
         def run_code_for_training_multi_instance_detection(self, net, display_labels=False, display_images=False):        
+
             """
             Version 2.0.6 introduced a loss function that respects the semantics of the different elements 
             of the YOLO vector.  Recall that when you assign an object bounding box to an anchor-box in a 
             specific cell of the grid over the images, you create a 5+C element YOLO vector where C is 
             the number of object classes in your dataset.  Since C=3 in our case, the YOLO vectors in our 
             case are 8-element vectors. See Slide 36 of the Week 8 slides for the meaning to be associated 
             with the different elements of a YOLO vector.
 
-            Lines 64 through 83 in the code shown below are the implementation of the new loss function.
+            Lines (68) through (79) in the code shown below are the implementation of the new loss function.
 
             Since the first element of the YOLO vector is to indicate the presence or the absence of object 
-            in a specific anchor-box in a specific cell, I use nn.BCELoss for that purpose.  The next four 
+            in a specific anchor-box of a specific cell, I use nn.BCELoss for that purpose.  The next four 
             elements carry purely numerical values that indicate the precise location of the object 
             vis-a-vis the center of the cell to which the object is assigned and also the precise height 
             and the width of the object bounding-box, I use nn.MSELoss for these four elements. The last 
             three elements are a one-hot representation of the object class label, so I use the regular 
             nn.CrossEntropyLoss for these elements.
 
             As I started writing code for incorporating the nn.CrossEntropyLoss mentioned above, I realized
             that (for purpose of loss calculation) I needed to append one more element to the last three 
             class-label elements of the YOLO vector to take care of the case when there is no object 
-            instance present in an anchor box.  You see, the dataset assumes that an image can have a 
-            maximum of 5 objects. If an image has fewer than 5 objects, that fact is expressed in the 
-            annotations by using the label value of 13 for the 'missing' objects.  To illustrate, say a
-            training image has just two objects in it, one being Dr. Eval and the other a house. In this
-            case, the annotation for the class labels would be the list [0,1,13,13,13].  If I had not 
-            augmented the YOLO vector for loss calculation, the network would be forced to choose
-            one of the actual class labels --- 0, 1, or 2 --- in the prediction for a YOLO vector even 
-            when there was no object present in the training image for that cell and that anchor box. So 
-            when the object label is 13, I throw all the probability mass related to class labels into the 
-            additional element (the 9th element) for a YOLO vector.
-
-            See Lines 57 through 60 for the above-mentioned augmentation of the YOLO vectors for all the
-            anchor boxes in all of the cells of the grid.
+            instance present in the anchor box corresponding to that yolo vector.  You see, the dataset 
+            assumes that an image can have a maximum of 5 objects. If an image has fewer than 5 objects, 
+            that fact is expressed in the annotations by using the label value of 13 for the 'missing' 
+            objects.  To illustrate, say a training image has just two objects in it, one being Dr. Eval 
+            and the other a house. In this case, the annotation for the class labels would be the list 
+            [0,1,13,13,13].  If I did not augment the YOLO vector for loss calculation, the network would 
+            be forced to choose one of the actual class labels --- 0, 1, or 2 --- in the object-label 
+            prediction for a YOLO vector even when there was no object present in the training image for 
+            that cell and that anchor box. So when the object label is 13, I throw all the probability mass 
+            related to class labels into the additional element (the 9th element) for a YOLO vector.
+
+            Line (13) initializes an augmented yolo_tensor for the augmented yolo_vectors mentioned above. 
+            Subsequently, Line (59) inserts in the augmented yolo_tensor an augmented yolo_vector for each
+            cell in the image and every anchor-box in that cell.  The loop in Lines (60) through (64) makes
+            sure of the fact that when the first element of an augmented yolo_vector is 0, meaning that there
+            is no object in the corresponding cell/anchor_box, the last element of the augmented yolo_vector
+            is set to 1. 
 
             An important consequence of augmenting the YOLO vectors in the manner explained above is that 
-            you must factor the augmentations in the processing of the predictions made by the network.
-            An example of that is shown in Line 91 where we supply 9 as the size of the vectors that
+            you must factor in the augmentations in the processing of the predictions made by the network.
+            An example of that is shown in Line (67) where we supply 9 as the size of the vectors that
             need to be recovered from the predictions.
             """
-            if self.rpg.batch_size > 1:                                                                                    ## (1)
-                sys.exit("YOLO-like multi-instance object detection has only been tested for batch_size of 1")             ## (2)
             yolo_debug = False
             filename_for_out1 = "performance_numbers_" + str(self.rpg.epochs) + "label.txt"                                
             filename_for_out2 = "performance_numbers_" + str(self.rpg.epochs) + "regres.txt"                               
             FILE1 = open(filename_for_out1, 'w')                                                                           
             FILE2 = open(filename_for_out2, 'w')                                                                           
             net = net.to(self.rpg.device)                                                                                  
-            criterion1 = nn.BCELoss()                    # For the first element of the 8 element yolo vector              ## (3)
-            criterion2 = nn.MSELoss()                    # For the regression elements (indexed 2,3,4,5) of yolo vector   ## (4)
-            criterion3 = nn.CrossEntropyLoss()           # For the last three elements of the 8 element yolo vector        ## (5)
+            criterion1 = nn.BCELoss(reduction='sum')          # For the first element of the 8 element yolo vector                ## (1)
+            criterion2 = nn.MSELoss(reduction='sum')          # For the regression elements (indexed 2,3,4,5) of yolo vector      ## (2)
+            criterion3 = nn.CrossEntropyLoss(reduction='sum') # For the last three elements of the 8 element yolo vector          ## (3)
+                                                              # Actually, the CrossEntropyLoss works on last four elements of
+                                                              #   the augmented yolo vectors.  We add one more element to the 
+                                                              #   8-element yolo vectors to allow for nilmapping.
             print("\n\nLearning Rate: ", self.rpg.learning_rate)
-            optimizer = optim.SGD(net.parameters(), lr=self.rpg.learning_rate, momentum=self.rpg.momentum)                 ## (6)
+            optimizer = optim.SGD(net.parameters(), lr=self.rpg.learning_rate, momentum=self.rpg.momentum)                        ## (4)
             print("\n\nStarting training loop...\n\n")
             start_time = time.perf_counter()
             Loss_tally = []
             elapsed_time = 0.0
-            yolo_interval = self.rpg.yolo_interval                                                                         ## (7)
-            num_yolo_cells = (self.rpg.image_size[0] // yolo_interval) * (self.rpg.image_size[1] // yolo_interval)         ## (8)
-            num_anchor_boxes =  5    # (height/width)   1/5  1/3  1/1  3/1  5/1                                            ## (9)
-            max_obj_num  = 5                                                                                               ## (10)
-            ## The 8 in the following is the size of the yolo_vector for each anchor-box in a given cell.  The 8 elements 
-            ## are: [obj_present, bx, by, bh, bw, c1, c2, c3] where bx and by are the delta diffs between the centers
-            ## of the yolo cell and the center of the object bounding box in terms of a unit for the cell width and cell 
-            ## height.  bh and bw are the height and the width of object bounding box in terms of the cell height and width.
-            for epoch in range(self.rpg.epochs):                                                                           ## (11)
+            yolo_interval = self.rpg.yolo_interval                                                                                ## (5)
+            num_yolo_cells = (self.rpg.image_size[0] // yolo_interval) * (self.rpg.image_size[1] // yolo_interval)                ## (6)
+            num_anchor_boxes =  5    # (height/width)   1/5  1/3  1/1  3/1  5/1                                                   ## (7)
+            max_obj_num  = 5                                                                                                      ## (8)
+            for epoch in range(self.rpg.epochs):                                                                                  ## (9)
                 print("")
-                running_loss = 0.0                                                                                         ## (12)
+                running_loss = 0.0                                                                                                ## (10)
                 for iter, data in enumerate(self.train_dataloader):   
                     if yolo_debug:
                         print("\n\n\n======================================= iteration: %d ========================================\n" % iter)
-                    yolo_tensor = torch.zeros( self.rpg.batch_size, num_yolo_cells, num_anchor_boxes, 8 )                  ## (13)
-                    im_tensor, seg_mask_tensor, bbox_tensor, bbox_label_tensor, num_objects_in_image = data                ## (14)
-                    im_tensor   = im_tensor.to(self.rpg.device)                                                            ## (15)
+                    im_tensor, seg_mask_tensor, bbox_tensor, bbox_label_tensor, num_objects_in_image = data                       ## (11)
+                    im_tensor   = im_tensor.to(self.rpg.device)                                 
                     seg_mask_tensor = seg_mask_tensor.to(self.rpg.device)                 
                     bbox_tensor = bbox_tensor.to(self.rpg.device)
                     bbox_label_tensor = bbox_label_tensor.to(self.rpg.device)
-                    yolo_tensor = yolo_tensor.to(self.rpg.device)
+                    ## The 8 in the following is the size of the yolo_vector for each anchor-box in a given cell.  The 8 elements 
+                    ## are: [obj_present, bx, by, bh, bw, c1, c2, c3] where bx and by are the delta diffs between the centers
+                    ## of the yolo cell and the center of the object bounding box in terms of a unit for the cell width and cell 
+                    ## height.  bh and bw are the height and the width of object bounding box in terms of the cell height and 
+                    ## width.
+                    yolo_tensor = torch.zeros( im_tensor.shape[0], num_yolo_cells, num_anchor_boxes, 8 ).to(self.rpg.device)      ## (12)
+                    ## We also define an augmented version of the above in which each yolo vector is augmented with one 
+                    ## additional element so that its length is now equal to 9 elements.  The additional element is for what's
+                    ## known as nil-mapping in computer vision.  What that means is that if we know there is no object present in
+                    ## a given cell/anchor_box combo, then we need a place to park the probability mass for the class labels
+                    ## for that combo. Speaking a bit more precisely, using CrossEntropy loss for the class labels means that
+                    ## a Softmax activation (involving a probability based normalization of the computed values) would ordinarily 
+                    ## be applied to the last 3 elements of the 8-element yolo vector.  However, that would make no sense for
+                    ## the case when a given cell/anchor_box combo contains no objects.  Extending the yolo vector by one 
+                    ## additional element allows for the probability mass to shift to that element when there is nothing in
+                    ## combo. From the standpoint of learning, a value of 1 stored in that extra element becomes the target
+                    ## for the CrossEntropy loss calculation applied to the bast FOUR elements of the yolo vectors in the 
+                    ## following tensor:
+                    yolo_tensor_aug = torch.zeros(im_tensor.shape[0], num_yolo_cells,num_anchor_boxes,9).to(self.rpg.device)      ## (13)
                     if yolo_debug:
                         logger = logging.getLogger()
                         old_level = logger.level
                         logger.setLevel(100)
                         plt.figure(figsize=[15,4])
                         plt.imshow(np.transpose(torchvision.utils.make_grid(im_tensor,normalize=True,padding=3,pad_value=255).cpu(), (1,2,0)))
                         plt.show()
                         logger.setLevel(old_level)
-                    cell_height = yolo_interval                                                                            ## (16)
-                    cell_width = yolo_interval                                                                             ## (17)
+                    cell_height = yolo_interval                                                                                   ## (14)
+                    cell_width = yolo_interval                                                                                    ## (15)
                     if yolo_debug:
                         print("\n\nnum_objects_in_image: ")
                         print(num_objects_in_image)
-                    num_cells_image_width = self.rpg.image_size[0] // yolo_interval                                        ## (18)
-                    num_cells_image_height = self.rpg.image_size[1] // yolo_interval                                       ## (19)
-                    height_center_bb = torch.zeros(im_tensor.shape[0], 1).float().to(self.rpg.device)                      ## (20)
-                    width_center_bb = torch.zeros(im_tensor.shape[0], 1).float().to(self.rpg.device)                       ## (21)
-                    obj_bb_height = torch.zeros(im_tensor.shape[0], 1).float().to(self.rpg.device)                         ## (22)
-                    obj_bb_width =  torch.zeros(im_tensor.shape[0], 1).float().to(self.rpg.device)                         ## (23)
-
-                    ## idx is for object index
-                    for idx in range(max_obj_num):                                                                         ## (24)
-                        ## In the mask, 1 means good image instance in batch, 0 means bad image instance in batch
-#                        batch_mask = torch.ones( self.rpg.batch_size, dtype=torch.int8).to(self.rpg.device)
-                        if yolo_debug:
-                            print("\n\n               ================  object indexed %d ===============              \n\n" % idx)
-                        ## Note that the bounding-box coordinates are in the (x,y) format, with x-positive going to
-                        ## right and the y-positive going down. A bbox is specified by (x_min,y_min,x_max,y_max):
-                        if yolo_debug:
-                            print("\n\nshape of bbox_tensor: ", bbox_tensor.shape)
-                            print("\n\nbbox_tensor:")
-                            print(bbox_tensor)
-                        ## in what follows, the first index (set to 0) is for the batch axis
-                        height_center_bb =  (bbox_tensor[0,idx,1] + bbox_tensor[0,idx,3]) // 2                             ## (25)
-                        width_center_bb =  (bbox_tensor[0,idx,0] + bbox_tensor[0,idx,2]) // 2                              ## (26)
-                        obj_bb_height = bbox_tensor[0,idx,3] -  bbox_tensor[0,idx,1]                                       ## (27)
-                        obj_bb_width = bbox_tensor[0,idx,2] - bbox_tensor[0,idx,0]                                         ## (28)
-                        if (obj_bb_height < 4.0) or (obj_bb_width < 4.0): continue                                         ## (29)
-
-                        cell_row_indx =  (height_center_bb / yolo_interval).int()          ## for the i coordinate         ## (30)
-                        cell_col_indx =  (width_center_bb / yolo_interval).int()           ## for the j coordinates        ## (31)
-                        cell_row_indx = torch.clamp(cell_row_indx, max=num_cells_image_height - 1)                         ## (32)
-                        cell_col_indx = torch.clamp(cell_col_indx, max=num_cells_image_width - 1)                          ## (33)
-
-                        ## The bh and bw elements in the yolo vector for this object:  bh and bw are measured relative 
-                        ## to the size of the grid cell to which the object is assigned.  For example, bh is the 
-                        ## height of the bounding-box divided by the actual height of the grid cell.
-                        bh  =  obj_bb_height.float() / yolo_interval                                                       ## (34)
-                        bw  =  obj_bb_width.float()  / yolo_interval                                                       ## (35)
-
-                        ## You have to be CAREFUL about object center calculation since bounding-box coordinates
-                        ## are in (x,y) format --- with x-positive going to the right and y-positive going down.
-                        obj_center_x =  (bbox_tensor[0,idx][2].float() +  bbox_tensor[0,idx][0].float()) / 2.0             ## (36)
-                        obj_center_y =  (bbox_tensor[0,idx][3].float() +  bbox_tensor[0,idx][1].float()) / 2.0             ## (37)
-                        ## Now you need to switch back from (x,y) format to (i,j) format:
-                        yolocell_center_i =  cell_row_indx*yolo_interval + float(yolo_interval) / 2.0                      ## (38)
-                        yolocell_center_j =  cell_col_indx*yolo_interval + float(yolo_interval) / 2.0                      ## (39)
-                        del_x  =  (obj_center_x.float() - yolocell_center_j.float()) / yolo_interval                       ## (40)
-                        del_y  =  (obj_center_y.float() - yolocell_center_i.float()) / yolo_interval                       ## (41)
-                        class_label_of_object = bbox_label_tensor[0,idx].item()                                            ## (42)
-                        ## When batch_size is only 1, it is easy to discard an image that has no known objects in it.
-                        ## To generalize this notion to arbitrary batch sizes, you will need a batch mask to indicate
-                        ## the images in a batch that should not be considered in the rest of this code.
-                        if class_label_of_object == 13: continue                                                           ## (43)
-                        AR = obj_bb_height.float() / obj_bb_width.float()                                                  ## (44)
-                        if AR <= 0.2:               anch_box_index = 0                                                     ## (45)
-                        if 0.2 < AR <= 0.5:         anch_box_index = 1                                                     ## (46)
-                        if 0.5 < AR <= 1.5:         anch_box_index = 2                                                     ## (47)
-                        if 1.5 < AR <= 4.0:         anch_box_index = 3                                                     ## (48)
-                        if AR > 4.0:                anch_box_index = 4                                                     ## (49)
-                        yolo_vector = torch.FloatTensor([0,del_x.item(), del_y.item(), bh.item(), bw.item(), 0, 0, 0] )    ## (50)
-                        yolo_vector[0] = 1                                                                                 ## (51)
-                        yolo_vector[5 + class_label_of_object] = 1                                                         ## (52)
-                        yolo_cell_index =  cell_row_indx.item() * num_cells_image_width  +  cell_col_indx.item()           ## (53)
-                        yolo_tensor[0,yolo_cell_index, anch_box_index] = yolo_vector                                       ## (54)
-                        yolo_tensor_aug = torch.zeros(self.rpg.batch_size, num_yolo_cells, \
-                                                                   num_anchor_boxes,9).float().to(self.rpg.device)         ## (55) 
-                        yolo_tensor_aug[:,:,:,:-1] =  yolo_tensor                                                          ## (56)
-                        if yolo_debug: 
-                            print("\n\nyolo_tensor specific: ")
-                            print(yolo_tensor[0,18,2])
-                            print("\nyolo_tensor_aug_aug: ") 
-                            print(yolo_tensor_aug[0,18,2])
-                    ## If no object is present, throw all the prob mass into the extra 9th ele of yolo_vector
-                    for icx in range(num_yolo_cells):                                                                      ## (57)
-                        for iax in range(num_anchor_boxes):                                                                ## (58)
-                            if yolo_tensor_aug[0,icx,iax,0] == 0:                                                          ## (59)
-                                yolo_tensor_aug[0,icx,iax,-1] = 1                                                          ## (60)
-                    if yolo_debug:
-                        logger = logging.getLogger()
-                        old_level = logger.level
-                        logger.setLevel(100)
-                        plt.figure(figsize=[15,4])
-                        plt.imshow(np.transpose(torchvision.utils.make_grid(im_tensor, normalize=True,
-                                                                         padding=3, pad_value=255).cpu(), (1,2,0)))
-                        plt.show()
-
-                    optimizer.zero_grad()                                                                                  ## (61)
-                    output = net(im_tensor)                                                                                ## (62)
-                    predictions_aug = output.view(self.rpg.batch_size,num_yolo_cells,num_anchor_boxes,9)                   ## (63)
-                    loss = torch.tensor(0.0, requires_grad=True).float().to(self.rpg.device)                               ## (64)
-                    for icx in range(num_yolo_cells):                                                                      ## (65)
-                        for iax in range(num_anchor_boxes):                                                                ## (66)
-                            pred_yolo_vector = predictions_aug[0,icx,iax]                                                  ## (67)
-                            target_yolo_vector = yolo_tensor_aug[0,icx,iax]                                                ## (68)
-                            ##  Estimating presence/absence of object and the Binary Cross Entropy section:
-                            object_presence = nn.Sigmoid()(torch.unsqueeze(pred_yolo_vector[0], dim=0))                    ## (69)
-                            target_for_prediction = torch.unsqueeze(target_yolo_vector[0], dim=0)                          ## (70)
-                            bceloss = criterion1(object_presence, target_for_prediction)                                   ## (71)
-                            loss += bceloss                                                                                ## (72)
-                            ## MSE section for regression params:
-                            pred_regression_vec = pred_yolo_vector[1:5]                                                    ## (73)
-                            pred_regression_vec = torch.unsqueeze(pred_regression_vec, dim=0)                              ## (74)
-                            target_regression_vec = torch.unsqueeze(target_yolo_vector[1:5], dim=0)                        ## (75)
-                            regression_loss = criterion2(pred_regression_vec, target_regression_vec)                       ## (76)
-                            loss += regression_loss                                                                        ## (77)
-                            ##  CrossEntropy section for object class label:
-                            probs_vector = pred_yolo_vector[5:]                                                            ## (78)
-                            probs_vector = torch.unsqueeze( probs_vector, dim=0 )                                          ## (79)
-                            target = torch.argmax(target_yolo_vector[5:])                                                  ## (80)
-                            target = torch.unsqueeze( target, dim=0 )                                                      ## (81)
-                            class_labeling_loss = criterion3(probs_vector, target)                                         ## (82)
-                            loss += class_labeling_loss                                                                    ## (83)
+                    num_cells_image_width = self.rpg.image_size[0] // yolo_interval                                               ## (16)
+                    num_cells_image_height = self.rpg.image_size[1] // yolo_interval                                              ## (17)
+                    ## ibx is batch instance index
+                    for ibx in range(im_tensor.shape[0]):                                                                         ## (18)
+                        ## idx is for object index
+                        num_of_objects =   (torch.sum(bbox_label_tensor[ibx] != 13).type(torch.uint8)).item()                     ## (19)
+                        for idx in range(num_of_objects):                                                                         ## (20)
+                            if yolo_debug:
+                                print("\n\n               ================  object indexed %d ===============              \n\n" % idx)
+                                ## Note that the bounding-box coordinates are in the (x,y) format, with x-positive going to
+                                ## right and the y-positive going down. A bbox is specified by (x_min,y_min,x_max,y_max):
+                                print("\n\nshape of bbox_tensor: ", bbox_tensor[ibx].shape)
+                                print("\n\nbbox_tensor:")
+                                print(bbox_tensor[ibx])
+                            ##  Since we are at pixel resolution at this point, there's not a whole lot of
+                            ##  between floating point division and integer division:
+                            height_center_bb =  (bbox_tensor[ibx,idx,1] + bbox_tensor[ibx,idx,3]) / 2.0                           ## (21)
+                            width_center_bb =  (bbox_tensor[ibx,idx,0] + bbox_tensor[ibx,idx,2]) / 2.0                            ## (22)
+                            obj_bb_height = bbox_tensor[ibx,idx,3] -  bbox_tensor[ibx,idx,1]                                      ## (23)
+                            obj_bb_width = bbox_tensor[ibx,idx,2] - bbox_tensor[ibx,idx,0]                                        ## (24)
+                            cell_row_indx =  (height_center_bb / yolo_interval).int()          ## for the i coordinate            ## (25)
+                            cell_col_indx =  (width_center_bb / yolo_interval).int()           ## for the j coordinates           ## (26)
+                            cell_row_indx = torch.clamp(cell_row_indx, max=num_cells_image_height - 1)                            ## (27)
+                            cell_col_indx = torch.clamp(cell_col_indx, max=num_cells_image_width - 1)                             ## (28)
+                            ## The bh and bw elements in the yolo vector for this object:  bh and bw are measured relative 
+                            ## to the size of the grid cell to which the object is assigned.  For example, bh is the 
+                            ## height of the bounding-box divided by the actual height of the grid cell.
+                            bh  =  obj_bb_height.float() / yolo_interval                                                          ## (29)
+                            bw  =  obj_bb_width.float()  / yolo_interval                                                          ## (30)
+                            ## You have to be CAREFUL about object center calculation since bounding-box coordinates
+                            ## are in (x,y) format --- with x-positive going to the right and y-positive going down.
+                            obj_center_x =  (bbox_tensor[ibx,idx][2].float() +  bbox_tensor[ibx,idx][0].float()) / 2.0            ## (31)
+                            obj_center_y =  (bbox_tensor[ibx,idx][3].float() +  bbox_tensor[ibx,idx][1].float()) / 2.0            ## (32)
+                            ## Now you need to switch back from (x,y) format to (i,j) format:
+                            yolocell_center_i =  cell_row_indx*yolo_interval + float(yolo_interval) / 2.0                         ## (33)
+                            yolocell_center_j =  cell_col_indx*yolo_interval + float(yolo_interval) / 2.0                         ## (34)
+                            del_x  =  (obj_center_x.float() - yolocell_center_j.float()) / yolo_interval                          ## (35)
+                            del_y  =  (obj_center_y.float() - yolocell_center_i.float()) / yolo_interval                          ## (36)
+                            class_label_of_object = bbox_label_tensor[ibx,idx].item()                                             ## (37)
+                            AR = obj_bb_height.float() / obj_bb_width.float()                                                     ## (38)
+                            if torch.isnan(AR):                                                                                   ## (39)
+                                AR = 100.0                                                                                        ## (40)
+                            else:
+                                AR = AR.item()                                                                                    ## (41)
+                            if AR <= 0.2:                                                                                         ## (42)
+                                anch_box_index = 0                                                                                ## (43)
+                            elif 0.2 < AR <= 0.5:                                                                                 ## (44)
+                                anch_box_index = 1                                                                                ## (45)
+                            elif 0.5 < AR <= 1.5:                                                                                 ## (46)
+                                anch_box_index = 2                                                                                ## (47)
+                            elif 1.5 < AR <= 4.0:                                                                                 ## (48)
+                                anch_box_index = 3                                                                                ## (49)
+                            elif AR > 4.0:                                                                                        ## (50)
+                                anch_box_index = 4                                                                                ## (51)
+                            yolo_vector = torch.FloatTensor([0,del_x, del_y, bh, bw, 0, 0, 0] ).to(self.rpg.device)               ## (52)
+                            if class_label_of_object != 13:                                                                       ## (53)
+                                yolo_vector[0] = 1.0                                                                              ## (54)
+                                yolo_vector[5 + class_label_of_object] = 1                                                        ## (55)
+                            yolo_cell_index =  (cell_row_indx * num_cells_image_width  +  cell_col_indx).type(torch.uint8)        ## (56)
+                            yolo_cell_index = yolo_cell_index.item()                                                              ## (57)
+                            yolo_tensor[ibx, yolo_cell_index, anch_box_index] = yolo_vector                                       ## (58)
+                            yolo_tensor_aug[ibx, yolo_cell_index, anch_box_index,:-1] = yolo_vector                               ## (59)
+                    ##  The following loop plays a critical role in the overall logic of learning. The network needs
+                    ##  to know that if the first element of a yolo vector is 0, meaning that there is no object present
+                    ##  in that cell/anchor_box combo, then all the probability weight in the last four elements of the
+                    ##  augmented yolo vector shifts to the last of the four elements:
+                    for ibx in range(im_tensor.shape[0]):                                                                         ## (60)
+                        for icx in range(num_yolo_cells):                                                                         ## (61)
+                            for iax in range(num_anchor_boxes):                                                                   ## (62)
+                                if yolo_tensor_aug[ibx, icx, iax, 0] == 0:                                                        ## (63)
+                                    yolo_tensor_aug[ibx, icx, iax,-1] = 1                                                         ## (64)
+                    optimizer.zero_grad()                                                                                         ## (65)
+                    output = net(im_tensor)                                                                                       ## (66)
+                    predictions_aug = output.view(-1,num_yolo_cells,num_anchor_boxes,9)                                           ## (67)
+
+                    ##  Now that we have the output of the network, must calculate the loss.  We initialize the loss tensors
+                    ##  for this iteration of training:
+                    loss = torch.tensor(0.0, requires_grad=True).float().to(self.rpg.device)                                      ## (68)
+                    ##  Estimating presence/absence of object with the Binary Cross Entropy loss:
+                    bceloss = criterion1( nn.Sigmoid()(predictions_aug[:,:,:,0]), yolo_tensor_aug[:,:,:,0] )                      ## (69)
+                    loss += bceloss                                                                                               ## (70)
+                    ## MSE loss for the regression params for the object bounding boxes:
+                    regression_loss = criterion2(predictions_aug[:,:,:,1:5], yolo_tensor_aug[:,:,:,1:5])                          ## (71)
+                    loss += regression_loss                                                                                       ## (72)
+                    ##  CrossEntropy loss for object class labels:
+                    targets = yolo_tensor_aug[:,:,:,5:]                                                                           ## (73)
+                    targets = targets.view(-1,4)                                                                                  ## (74)
+                    targets = torch.argmax(targets, dim=1)                                                                        ## (75)
+                    probs = predictions_aug[:,:,:,5:]                                                                             ## (76)
+                    probs = probs.view(-1,4)                                                                                      ## (77)
+                    class_labeling_loss = criterion3( probs, targets)                                                             ## (78)
+                    loss +=  class_labeling_loss                                                                                  ## (79)
                     if yolo_debug:
                         print("\n\nshape of loss: ", loss.shape)
                         print("\n\nloss: ", loss)
-                    loss.backward()                                                                                        ## (84)
-                    optimizer.step()                                                                                       ## (85)
-                    running_loss += loss.item()                                                                            ## (86)
-                    if iter%500==499:                                                                                      ## (87)
-                        current_time = time.perf_counter()
+                    loss.backward()                                                                                               ## (80)
+                    optimizer.step()                                                                                              ## (81)
+                    running_loss += loss.item()                                                                                   ## (82)
+                    if iter%500==499:                                                                                             ## (83)
+                        current_time = time.perf_counter()                                                                    
                         elapsed_time = current_time - start_time 
-                        avg_loss = running_loss / float(1000)                                                              ## (88)
+                        avg_loss = running_loss / float(500)                                                                      ## (84)
                         print("\n[epoch:%d/%d, iter=%4d  elapsed_time=%5d secs]      mean value for loss: %7.4f" % 
-                                                            (epoch+1,self.rpg.epochs, iter+1, elapsed_time, avg_loss))     ## (89)
+                                                            (epoch+1,self.rpg.epochs, iter+1, elapsed_time, avg_loss))            ## (85)
                         Loss_tally.append(running_loss)
                         FILE1.write("%.3f\n" % avg_loss)
                         FILE1.flush()
-                        running_loss = 0.0                                                                                 ## (90)
+                        running_loss = 0.0                                                                                        ## (86)
+                        running_bceloss = 0.0
+                        running_regressionloss = 0.0
+                        running_labelingloss = 0.0
                         if display_labels:
-                            predictions = output.view(self.rpg.batch_size,num_yolo_cells,num_anchor_boxes,9)               ## (91)
-                            if yolo_debug:
-                                print("\n\nyolo_vector for first image in batch, cell indexed 18, and AB indexed 2: ")
-                                print(predictions[0, 18, 2])
-                            for ibx in range(predictions.shape[0]):                             # for each batch image     ## (92)
-                                icx_2_best_anchor_box = {ic : None for ic in range(36)}                                    ## (93)
-                                for icx in range(predictions.shape[1]):                         # for each yolo cell       ## (94)
-                                    cell_predi = predictions[ibx,icx]                                                      ## (95)
-                                    prev_best = 0                                                                          ## (96)
-                                    for anchor_bdx in range(cell_predi.shape[0]):                                          ## (97)
-                                        if cell_predi[anchor_bdx][0] > cell_predi[prev_best][0]:                           ## (98)
-                                            prev_best = anchor_bdx                                                         ## (99)
-                                    best_anchor_box_icx = prev_best                                                        ## (100)
-                                    icx_2_best_anchor_box[icx] = best_anchor_box_icx                                       ## (101)
-                                sorted_icx_to_box = sorted(icx_2_best_anchor_box,                                   
-                                      key=lambda x: predictions[ibx,x,icx_2_best_anchor_box[x]][0].item(), reverse=True)   ## (102)
-                                retained_cells = sorted_icx_to_box[:5]                                                     ## (103)
-                                objects_detected = []                                                                      ## (104)
-                                for icx in retained_cells:                                                                 ## (105)
-                                    pred_vec = predictions[ibx,icx, icx_2_best_anchor_box[icx]]                            ## (106)
-                                    class_labels_predi  = pred_vec[-4:]                                                    ## (107)
-                                    class_labels_probs = torch.nn.Softmax(dim=0)(class_labels_predi)                       ## (108)
-                                    class_labels_probs = class_labels_probs[:-1]                                           ## (109)
+                            for ibx in range(predictions_aug.shape[0]):                             # for each batch image        ## (87)
+                                icx_2_best_anchor_box = {ic : None for ic in range(36)}                                           ## (88)
+                                for icx in range(predictions_aug.shape[1]):                         # for each yolo cell          ## (89)
+                                    cell_predi = predictions_aug[ibx,icx]                                                         ## (90)
+                                    prev_best = 0                                                                                 ## (91)
+                                    for anchor_bdx in range(cell_predi.shape[0]):                                                 ## (92)
+                                        if cell_predi[anchor_bdx][0] > cell_predi[prev_best][0]:                                  ## (93)
+                                            prev_best = anchor_bdx                                                                ## (94)
+                                    best_anchor_box_icx = prev_best                                                               ## (95)
+                                    icx_2_best_anchor_box[icx] = best_anchor_box_icx                                              ## (96)
+                                sorted_icx_to_box = sorted(icx_2_best_anchor_box,                                                 ## (97)
+                                      key=lambda x: predictions_aug[ibx,x,icx_2_best_anchor_box[x]][0].item(), reverse=True)      ## (98)
+                                retained_cells = sorted_icx_to_box[:5]                                                            ## (99)
+                                objects_detected = []                                                                             ## (100)
+                                for icx in retained_cells:                                                                        ## (101)
+                                    pred_vec = predictions_aug[ibx,icx, icx_2_best_anchor_box[icx]]                               ## (102)
+                                    class_labels_predi  = pred_vec[-4:]                                                           ## (103)
+                                    class_labels_probs = torch.nn.Softmax(dim=0)(class_labels_predi)                              ## (104)
+                                    class_labels_probs = class_labels_probs[:-1]                                                  ## (105)
                                     ##  The threshold of 0.25 applies only to the case of there being 3 classes of objects 
                                     ##  in the dataset.  In the absence of an object, the values in the first three nodes
                                     ##  that represent the classes should all be less than 0.25. In general, for N classes
                                     ##  you would want to set this threshold to 1.0/N
-                                    if torch.all(class_labels_probs < 0.25):                                               ## (110)
-                                        predicted_class_label = None                                                       ## (111)
+                                    if torch.all(class_labels_probs < 0.25):                                                      ## (115)
+                                        predicted_class_label = None                                                              ## (116)
                                     else:                                                                                
-                                        best_predicted_class_index = (class_labels_probs == class_labels_probs.max())      ## (112)
-                                        best_predicted_class_index =torch.nonzero(best_predicted_class_index,as_tuple=True)## (113)
-                                        predicted_class_label =self.rpg.class_labels[best_predicted_class_index[0].item()] ## (114)
-                                        objects_detected.append(predicted_class_label)                                     ## (115)
+                                        best_predicted_class_index = (class_labels_probs == class_labels_probs.max())             ## (117)
+                                        best_predicted_class_index =torch.nonzero(best_predicted_class_index,as_tuple=True)       ## (118)
+                                        predicted_class_label =self.rpg.class_labels[best_predicted_class_index[0].item()]        ## (119)
+                                        objects_detected.append(predicted_class_label)                                            ## (120)
+
                                 print("[batch image=%d]  objects found in descending probability order: " % ibx, 
-                                                                                                     objects_detected)     ## (116)
+                                                                                                     objects_detected)            ## (121)
                         if display_images:
                             logger = logging.getLogger()
                             old_level = logger.level
                             logger.setLevel(100)
                             plt.figure(figsize=[15,4])
                             plt.imshow(np.transpose(torchvision.utils.make_grid(im_tensor, normalize=True,
                                                                              padding=3, pad_value=255).cpu(), (1,2,0)))
@@ -2280,16 +2270,26 @@
         def save_yolo_model(self, model):
             '''
             Save the trained yolo model to a disk file
             '''
             torch.save(model.state_dict(), self.rpg.path_saved_yolo_model)
 
 
-        def run_code_for_testing_multi_instance_detection(self, net, display_images=False):        
+        def run_code_for_testing_multi_instance_detection(self, net, dir_name_for_results, display_images=False):        
             yolo_debug = False
+            if os.path.exists(dir_name_for_results):
+                files = glob.glob(dir_name_for_results + "/*")
+                for file in files:
+                    if os.path.isfile(file):
+                        os.remove(file)
+                    else:
+                        files = glob.glob(file + "/*")
+                        list(map(lambda x: os.remove(x), files))
+            else:
+                os.mkdir(dir_name_for_results)
             net.load_state_dict(torch.load(self.rpg.path_saved_yolo_model))
             net = net.to(self.rpg.device)
             yolo_interval = self.rpg.yolo_interval
             num_yolo_cells = (self.rpg.image_size[0] // yolo_interval) * (self.rpg.image_size[1] // yolo_interval)
             num_anchor_boxes =  5    # (height/width)   1/5  1/3  1/1  3/1  5/1
             ##  The next 5 assignment are for the calculations of the confusion matrix:
             confusion_matrix = torch.zeros(3,3)   #  We have only 3 classes:  Dr. Eval, house, and watertower
@@ -2311,15 +2311,15 @@
                     if iter % 50 == 49:
                         if display_images:
                             print("\n\n\n\nShowing output for test image %d: " % (iter+1))
                         im_tensor   = im_tensor.to(self.rpg.device)
                         seg_mask_tensor = seg_mask_tensor.to(self.rpg.device)                 
                         bbox_tensor = bbox_tensor.to(self.rpg.device)
                         output = net(im_tensor)
-                        predictions = output.view(self.rpg.batch_size,num_yolo_cells,num_anchor_boxes,9)
+                        predictions = output.view(-1, num_yolo_cells, num_anchor_boxes,9)
                         for ibx in range(predictions.shape[0]):                             # for each batch image
                             ## Our goal is to look through all the cells and identify at most five of the cells/anchor_boxes for 
                             ## the value in the first element of the predicted yolo_vectors is the highest:
                             icx_2_best_anchor_box = {ic : None for ic in range(36)}
                             for icx in range(predictions.shape[1]):                         # for each yolo cell
                                 cell_predi = predictions[ibx,icx]               
                                 prev_best = 0
@@ -2383,14 +2383,15 @@
                             print(gt_bboxes)
                         ## These are the mappings from indexes for the predicted bboxes to the indexes for the gt bboxes:
                         mapping_from_pred_to_gt = { i : None for i in range(len(predicted_bboxes))}
                         for i in range(len(predicted_bboxes)):
                             gt_possibles = {k : 0.0 for k in range(5)}      ## 0.0 for IoU 
                             for j in range(len(gt_bboxes)):
                                 if all(gt_bboxes[j][x] == 0 for x in range(4)): continue       ## 4 is for the four coords of a bbox
+                                if (gt_bboxes[j].all() == 0): continue       ## 4 is for the four coords of a bbox
                                 gt_possibles[j] = self.IoU_calculator(predicted_bboxes[i], gt_bboxes[j])
                             sorted_gt_possibles =  sorted(gt_possibles, key=lambda x: gt_possibles[x], reverse=True)
                             if display_images:
                                 print("For predicted bbox %d: the best gt bbox is: %d" % (i, sorted_gt_possibles[0]))
                             mapping_from_pred_to_gt[i] = (sorted_gt_possibles[0], gt_possibles[sorted_gt_possibles[0]])
                         ##  If you want to see the IoU scores for the overlap between each predicted bbox and all of the individual gt bboxes:
                         if display_images:
@@ -2428,17 +2429,23 @@
                             ax.imshow(np.transpose(torchvision.utils.make_grid(new_im_tensor, normalize=True, padding=3, pad_value=255).cpu(), (1,2,0)))
                             for i,bbox_pred in enumerate(predicted_bboxes):
                                 x,y,w,h = np.array(bbox_pred)                                                                     
                                 x,y,w,h = [item * display_scale for item in (x,y,w,h)]
                                 rect = Rectangle((x,y),w,h,angle=0.0,edgecolor='r',fill = False,lw=2) 
                                 ax.add_patch(rect)                                                                      
                                 ax.annotate(predicted_labels_for_bboxes[i], (x,y-1), color='red', weight='bold', fontsize=10*display_scale)
+                                gt_box_index = mapping_from_pred_to_gt[i][0]              ## '[0]' becaause mapping returns (index,prob) pair
+                                x1,y1,x2,y2 = np.array(gt_bboxes[gt_box_index])                                                                     
+                                x,y,w,h = x1,y1,x2-x1,y2-y1
+                                x,y,w,h = [item * display_scale for item in (x,y,w,h)]
+                                rect = Rectangle((x,y),w,h,angle=0.0,edgecolor='g',fill = False,lw=2) 
+                                ax.add_patch(rect)                                                                      
+                            plt.savefig(dir_name_for_results + "/" +  str(iter) + ".png")
                             plt.show()
                             logger.setLevel(old_level)
-                                                                                            
             ##  Our next job is to present to the user the information collected for the confusion matrix for the validation dataset:
             if yolo_debug:
                 print("\nConfusion Matrix: ", confusion_matrix)
                 print("\nclass_correct: ", class_correct)
                 print("\nclass_total: ", class_total)
                 print("\ntotals_for_conf_mat: ", totals_for_conf_mat)
                 print("\ntotals_correct: ", totals_correct)
```

### Comparing `RegionProposalGenerator-2.0.8/TestRegionProposalGenerator/Test.py` & `RegionProposalGenerator-2.1.0/TestRegionProposalGenerator/Test.py`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/TestRegionProposalGenerator/TestImageConversion.py` & `RegionProposalGenerator-2.1.0/TestRegionProposalGenerator/TestImageConversion.py`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/TestRegionProposalGenerator/TestImageLoadingAndDataExtraction.py` & `RegionProposalGenerator-2.1.0/TestRegionProposalGenerator/TestImageLoadingAndDataExtraction.py`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/TestRegionProposalGenerator/halfsun.jpg` & `RegionProposalGenerator-2.1.0/TestRegionProposalGenerator/halfsun.jpg`

 * *Files identical despite different names*

### Comparing `RegionProposalGenerator-2.0.8/setup.py` & `RegionProposalGenerator-2.1.0/RegionProposalGenerator.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,91 +1,83 @@
-#!/usr/bin/env python
-
-### setup.py
-
-from setuptools import setup, find_packages
-import sys, os
-
-setup(name='RegionProposalGenerator',
-      version='2.0.8',
-      author='Avinash Kak',
-      author_email='kak@purdue.edu',
-      maintainer='Avinash Kak',
-      maintainer_email='kak@purdue.edu',
-      url='https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.0.8.html',
-      download_url='https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.0.8.tar.gz',
-      description='An educational module for experimenting with single-instance and multi-instance object detection and for generating region proposals with graph-based algorithms',
-      long_description='''
-
-Consult the module API page at
-
-      https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.0.8.html
-
-for all information related to this module, including information related
-to the latest changes to the code.  The page at the URL shown above lists
-all of the module functionality you can invoke in your own code.
-
-::
-
-        Single-Instance and Multi-Instance Object Detection:
-    
-            Say you wish to experiment with YOLO-like logic for multi-instance
-            object detection, you would need to construct an instance of the
-            RegionProposalGenerator class and invoke the methods shown below on
-            this instance:
-        
-            rpg = RegionProposalGenerator(
-                              dataroot = "./data/",
-                              image_size = [128,128],
-                              yolo_interval = 20,
-                              path_saved_yolo_model = "./saved_yolo_model",
-                              momentum = 0.9,
-                              learning_rate = 1e-6,
-                              epochs = 40,
-                              batch_size = 4,
-                              classes = ('Dr_Eval','house','watertower'),
-                              use_gpu = True,
-                          )
-            yolo = RegionProposalGenerator.YoloLikeDetector( rpg = rpg )
-            yolo.set_dataloaders(train=True)
-            yolo.set_dataloaders(test=True)
-            model = yolo.NetForYolo(skip_connections=True, depth=8) 
-            model = yolo.run_code_for_training_multi_instance_detection(model, display_images=False)
-            yolo.run_code_for_training_multi_instance_detection(model, display_images = True)
+Metadata-Version: 1.2
+Name: RegionProposalGenerator
+Version: 2.1.0
+Summary: An educational module for experimenting with the YOLO logic for multi-instance object detection and for generating region proposals with graph-based algorithms
+Home-page: https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.1.0.html
+Author: Avinash Kak
+Author-email: kak@purdue.edu
+Maintainer: Avinash Kak
+Maintainer-email: kak@purdue.edu
+License: Python Software Foundation License
+Download-URL: https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.1.0.tar.gz
+Description: 
+        
+        Consult the module API page at
+        
+              https://engineering.purdue.edu/kak/distRPG/RegionProposalGenerator-2.1.0.html
+        
+        for all information related to this module, including information related
+        to the latest changes to the code.  The page at the URL shown above lists
+        all of the module functionality you can invoke in your own code.
+        
+        ::
+        
+                Single-Instance and Multi-Instance Object Detection:
+            
+                    Say you wish to experiment with YOLO-like logic for multi-instance
+                    object detection, you would need to construct an instance of the
+                    RegionProposalGenerator class and invoke the methods shown below on
+                    this instance:
+                
+                    rpg = RegionProposalGenerator(
+                                      dataroot = "./data/",
+                                      image_size = [128,128],
+                                      yolo_interval = 20,
+                                      path_saved_yolo_model = "./saved_yolo_model",
+                                      momentum = 0.9,
+                                      learning_rate = 1e-6,
+                                      epochs = 40,
+                                      batch_size = 4,
+                                      classes = ('Dr_Eval','house','watertower'),
+                                      use_gpu = True,
+                                  )
+                    yolo = RegionProposalGenerator.YoloLikeDetector( rpg = rpg )
+                    yolo.set_dataloaders(train=True)
+                    yolo.set_dataloaders(test=True)
+                    model = yolo.NetForYolo(skip_connections=True, depth=8) 
+                    model = yolo.run_code_for_training_multi_instance_detection(model, display_images=False)
+                    yolo.run_code_for_training_multi_instance_detection(model, display_images = True)
+                    
+            
+                Graph-Based Algorithms for Region Proposals:
             
-    
-        Graph-Based Algorithms for Region Proposals:
-    
-            To generate region proposals, you would need to construct an instance
-            of the RegionProposalGenerator class and invoke the methods shown below
-            on this instance:
-        
-            rpg = RegionProposalGenerator(
-                           ###  The first 6 options affect only the graph-based part of the algo
-                           sigma = 1.0,
-                           max_iterations = 40,
-                           kay = 0.05,
-                           image_normalization_required = True,
-                           image_size_reduction_factor = 4,
-                           min_size_for_graph_based_blobs = 4,
-                           ###  The next 4 options affect only the Selective Search part of the algo
-                           color_homogeneity_thresh = [20,20,20],
-                           gray_var_thresh = 16000,           
-                           texture_homogeneity_thresh = 120,
-                           max_num_blobs_expected = 8,
-                  )
+                    To generate region proposals, you would need to construct an instance
+                    of the RegionProposalGenerator class and invoke the methods shown below
+                    on this instance:
+                
+                    rpg = RegionProposalGenerator(
+                                   ###  The first 6 options affect only the graph-based part of the algo
+                                   sigma = 1.0,
+                                   max_iterations = 40,
+                                   kay = 0.05,
+                                   image_normalization_required = True,
+                                   image_size_reduction_factor = 4,
+                                   min_size_for_graph_based_blobs = 4,
+                                   ###  The next 4 options affect only the Selective Search part of the algo
+                                   color_homogeneity_thresh = [20,20,20],
+                                   gray_var_thresh = 16000,           
+                                   texture_homogeneity_thresh = 120,
+                                   max_num_blobs_expected = 8,
+                          )
+                    
+                    image_name = "images/mondrian.jpg"
+                    segmented_graph,color_map = rpg.graph_based_segmentation(image_name)
+                    rpg.visualize_segmentation_in_pseudocolor(segmented_graph[0], color_map, "graph_based" )
+                    merged_blobs, color_map = rpg.selective_search_for_region_proposals( segmented_graph, image_name )
+                    rpg.visualize_segmentation_with_mean_gray(merged_blobs, "ss_based_segmentation_in_bw" )
+        
             
-            image_name = "images/mondrian.jpg"
-            segmented_graph,color_map = rpg.graph_based_segmentation(image_name)
-            rpg.visualize_segmentation_in_pseudocolor(segmented_graph[0], color_map, "graph_based" )
-            merged_blobs, color_map = rpg.selective_search_for_region_proposals( segmented_graph, image_name )
-            rpg.visualize_segmentation_with_mean_gray(merged_blobs, "ss_based_segmentation_in_bw" )
-
-    
-          ''',
-
-      license='Python Software Foundation License',
-      keywords='object detection, image segmentation, computer vision',
-      platforms='All platforms',
-      classifiers=['Topic :: Scientific/Engineering :: Image Recognition', 'Programming Language :: Python :: 3.8'],
-      packages=['RegionProposalGenerator']
-)
+                  
+Keywords: object detection,image segmentation,computer vision
+Platform: All platforms
+Classifier: Topic :: Scientific/Engineering :: Image Recognition
+Classifier: Programming Language :: Python :: 3.8
```

