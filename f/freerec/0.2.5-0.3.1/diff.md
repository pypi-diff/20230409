# Comparing `tmp/freerec-0.2.5.tar.gz` & `tmp/freerec-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freerec-0.2.5.tar", last modified: Fri Mar 17 12:53:21 2023, max compression
+gzip compressed data, was "freerec-0.3.1.tar", last modified: Sun Apr  9 03:11:27 2023, max compression
```

## Comparing `freerec-0.2.5.tar` & `freerec-0.3.1.tar`

### file list

```diff
@@ -1,64 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-03-17 12:53:21.790915 freerec-0.2.5/
--rw-rw-rw-   0        0        0     1085 2022-09-12 08:50:27.000000 freerec-0.2.5/LICENSE
--rw-rw-rw-   0        0        0     1615 2023-03-17 12:53:21.790915 freerec-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     1150 2023-03-17 12:23:24.000000 freerec-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-17 12:53:21.657070 freerec-0.2.5/freerec/
--rw-rw-rw-   0        0        0      504 2023-03-17 12:52:21.000000 freerec-0.2.5/freerec/__init__.py
--rw-rw-rw-   0        0        0      282 2023-03-08 10:58:41.000000 freerec-0.2.5/freerec/__main__.py
--rw-rw-rw-   0        0        0     3379 2023-03-16 13:10:00.000000 freerec-0.2.5/freerec/criterions.py
-drwxrwxrwx   0        0        0        0 2023-03-17 12:53:21.693314 freerec-0.2.5/freerec/data/
--rw-rw-rw-   0        0        0       90 2023-02-24 08:54:11.000000 freerec-0.2.5/freerec/data/__init__.py
--rw-rw-rw-   0        0        0      998 2023-02-24 08:54:11.000000 freerec-0.2.5/freerec/data/dataloader.py
-drwxrwxrwx   0        0        0        0 2023-03-17 12:53:21.705714 freerec-0.2.5/freerec/data/datasets/
--rw-rw-rw-   0        0        0      239 2023-03-08 11:54:05.000000 freerec-0.2.5/freerec/data/datasets/__init__.py
--rw-rw-rw-   0        0        0    18023 2023-02-27 06:25:40.000000 freerec-0.2.5/freerec/data/datasets/base.py
-drwxrwxrwx   0        0        0        0 2023-03-17 12:53:21.709713 freerec-0.2.5/freerec/data/datasets/context/
--rw-rw-rw-   0        0        0        0 2023-02-26 02:12:53.000000 freerec-0.2.5/freerec/data/datasets/context/__init__.py
--rw-rw-rw-   0        0        0      209 2023-02-24 08:54:11.000000 freerec-0.2.5/freerec/data/datasets/context/base.py
-drwxrwxrwx   0        0        0        0 2023-03-17 12:53:21.721259 freerec-0.2.5/freerec/data/datasets/general/
--rw-rw-rw-   0        0        0       91 2023-02-24 08:54:11.000000 freerec-0.2.5/freerec/data/datasets/general/__init__.py
--rw-rw-rw-   0        0        0    13760 2023-02-28 12:22:06.000000 freerec-0.2.5/freerec/data/datasets/general/amazon.py
--rw-rw-rw-   0        0        0     3872 2023-03-16 13:18:06.000000 freerec-0.2.5/freerec/data/datasets/general/base.py
--rw-rw-rw-   0        0        0     2861 2023-02-28 12:22:29.000000 freerec-0.2.5/freerec/data/datasets/general/gowalla.py
--rw-rw-rw-   0        0        0     4729 2023-02-28 12:23:17.000000 freerec-0.2.5/freerec/data/datasets/general/movielens.py
--rw-rw-rw-   0        0        0     2845 2023-02-28 12:22:37.000000 freerec-0.2.5/freerec/data/datasets/general/yelp.py
-drwxrwxrwx   0        0        0        0 2023-03-17 12:53:21.725294 freerec-0.2.5/freerec/data/datasets/knowledge/
--rw-rw-rw-   0        0        0        0 2023-02-26 02:12:46.000000 freerec-0.2.5/freerec/data/datasets/knowledge/__init__.py
--rw-rw-rw-   0        0        0      215 2023-02-24 08:54:11.000000 freerec-0.2.5/freerec/data/datasets/knowledge/base.py
-drwxrwxrwx   0        0        0        0 2023-03-17 12:53:21.754098 freerec-0.2.5/freerec/data/datasets/sequential/
--rw-rw-rw-   0        0        0       69 2023-02-28 12:12:56.000000 freerec-0.2.5/freerec/data/datasets/sequential/__init__.py
--rw-rw-rw-   0        0        0     3716 2023-02-28 12:30:03.000000 freerec-0.2.5/freerec/data/datasets/sequential/amazon.py
--rw-rw-rw-   0        0        0     2818 2023-02-28 12:32:59.000000 freerec-0.2.5/freerec/data/datasets/sequential/base.py
--rw-rw-rw-   0        0        0     1792 2023-02-28 12:30:30.000000 freerec-0.2.5/freerec/data/datasets/sequential/movielens.py
--rw-rw-rw-   0        0        0     1794 2023-02-28 12:31:02.000000 freerec-0.2.5/freerec/data/datasets/sequential/steam.py
-drwxrwxrwx   0        0        0        0 2023-03-17 12:53:21.758098 freerec-0.2.5/freerec/data/datasets/session/
--rw-rw-rw-   0        0        0        0 2023-02-26 02:12:38.000000 freerec-0.2.5/freerec/data/datasets/session/__init__.py
--rw-rw-rw-   0        0        0      209 2023-02-24 08:54:11.000000 freerec-0.2.5/freerec/data/datasets/session/base.py
--rw-rw-rw-   0        0        0    29454 2023-03-10 09:09:02.000000 freerec-0.2.5/freerec/data/fields.py
-drwxrwxrwx   0        0        0        0 2023-03-17 12:53:21.785913 freerec-0.2.5/freerec/data/postprocessing/
--rw-rw-rw-   0        0        0      111 2023-02-24 08:54:11.000000 freerec-0.2.5/freerec/data/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     2713 2023-02-24 08:54:11.000000 freerec-0.2.5/freerec/data/postprocessing/base.py
--rw-rw-rw-   0        0        0     2177 2023-02-24 08:54:11.000000 freerec-0.2.5/freerec/data/postprocessing/column.py
--rw-rw-rw-   0        0        0    10232 2023-02-24 08:54:11.000000 freerec-0.2.5/freerec/data/postprocessing/row.py
--rw-rw-rw-   0        0        0    17697 2023-02-24 08:54:11.000000 freerec-0.2.5/freerec/data/postprocessing/sampler.py
--rw-rw-rw-   0        0        0     2737 2023-02-24 08:54:11.000000 freerec-0.2.5/freerec/data/postprocessing/source.py
--rw-rw-rw-   0        0        0     9867 2023-03-17 12:50:13.000000 freerec-0.2.5/freerec/data/preprocessing.py
--rw-rw-rw-   0        0        0      681 2023-02-24 08:54:11.000000 freerec-0.2.5/freerec/data/tags.py
--rw-rw-rw-   0        0        0     4533 2023-02-26 11:58:59.000000 freerec-0.2.5/freerec/data/transformation.py
--rw-rw-rw-   0        0        0     7457 2023-03-17 12:50:23.000000 freerec-0.2.5/freerec/data/utils.py
--rw-rw-rw-   0        0        0     3101 2023-02-24 08:54:11.000000 freerec-0.2.5/freerec/dict2obj.py
--rw-rw-rw-   0        0        0    29222 2023-03-11 10:55:20.000000 freerec-0.2.5/freerec/launcher.py
--rw-rw-rw-   0        0        0    22055 2023-03-15 10:53:59.000000 freerec-0.2.5/freerec/metrics.py
-drwxrwxrwx   0        0        0        0 2023-03-17 12:53:21.789919 freerec-0.2.5/freerec/models/
--rw-rw-rw-   0        0        0       23 2023-02-24 08:54:11.000000 freerec-0.2.5/freerec/models/__init__.py
--rw-rw-rw-   0        0        0     3289 2023-02-24 08:54:11.000000 freerec-0.2.5/freerec/models/base.py
--rw-rw-rw-   0        0        0    17644 2023-03-15 06:46:02.000000 freerec-0.2.5/freerec/parser.py
--rw-rw-rw-   0        0        0    14588 2023-03-16 13:10:40.000000 freerec-0.2.5/freerec/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-17 12:53:21.682144 freerec-0.2.5/freerec.egg-info/
--rw-rw-rw-   0        0        0     1615 2023-03-17 12:53:21.000000 freerec-0.2.5/freerec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1558 2023-03-17 12:53:21.000000 freerec-0.2.5/freerec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-17 12:53:21.000000 freerec-0.2.5/freerec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      111 2023-03-17 12:53:21.000000 freerec-0.2.5/freerec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-17 12:53:21.000000 freerec-0.2.5/freerec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-17 12:53:21.791942 freerec-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1082 2023-02-25 12:08:33.000000 freerec-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.795427 freerec-0.3.1/
+-rw-rw-rw-   0        0        0     1085 2022-09-12 08:50:27.000000 freerec-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     1814 2023-04-09 03:11:27.794838 freerec-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2023-03-24 04:09:10.000000 freerec-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.537852 freerec-0.3.1/freerec/
+-rw-rw-rw-   0        0        0      506 2023-04-09 03:10:25.000000 freerec-0.3.1/freerec/__init__.py
+-rw-rw-rw-   0        0        0     4188 2023-03-27 11:31:30.000000 freerec-0.3.1/freerec/__main__.py
+-rw-rw-rw-   0        0        0     3379 2023-03-16 13:10:00.000000 freerec-0.3.1/freerec/criterions.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.580699 freerec-0.3.1/freerec/data/
+-rw-rw-rw-   0        0        0       90 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/__init__.py
+-rw-rw-rw-   0        0        0      998 2023-03-22 12:08:02.000000 freerec-0.3.1/freerec/data/dataloader.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.598971 freerec-0.3.1/freerec/data/datasets/
+-rw-rw-rw-   0        0        0      239 2023-03-08 11:54:05.000000 freerec-0.3.1/freerec/data/datasets/__init__.py
+-rw-rw-rw-   0        0        0    18023 2023-02-27 06:25:40.000000 freerec-0.3.1/freerec/data/datasets/base.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.606534 freerec-0.3.1/freerec/data/datasets/context/
+-rw-rw-rw-   0        0        0        0 2023-02-26 02:12:53.000000 freerec-0.3.1/freerec/data/datasets/context/__init__.py
+-rw-rw-rw-   0        0        0      209 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/datasets/context/base.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.660108 freerec-0.3.1/freerec/data/datasets/general/
+-rw-rw-rw-   0        0        0       91 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/datasets/general/__init__.py
+-rw-rw-rw-   0        0        0    13760 2023-02-28 12:22:06.000000 freerec-0.3.1/freerec/data/datasets/general/amazon.py
+-rw-rw-rw-   0        0        0     3872 2023-03-16 13:18:06.000000 freerec-0.3.1/freerec/data/datasets/general/base.py
+-rw-rw-rw-   0        0        0     2861 2023-04-08 05:39:36.000000 freerec-0.3.1/freerec/data/datasets/general/gowalla.py
+-rw-rw-rw-   0        0        0     4729 2023-02-28 12:23:17.000000 freerec-0.3.1/freerec/data/datasets/general/movielens.py
+-rw-rw-rw-   0        0        0     2845 2023-02-28 12:22:37.000000 freerec-0.3.1/freerec/data/datasets/general/yelp.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.671157 freerec-0.3.1/freerec/data/datasets/knowledge/
+-rw-rw-rw-   0        0        0        0 2023-02-26 02:12:46.000000 freerec-0.3.1/freerec/data/datasets/knowledge/__init__.py
+-rw-rw-rw-   0        0        0      215 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/datasets/knowledge/base.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.715396 freerec-0.3.1/freerec/data/datasets/sequential/
+-rw-rw-rw-   0        0        0       69 2023-02-28 12:12:56.000000 freerec-0.3.1/freerec/data/datasets/sequential/__init__.py
+-rw-rw-rw-   0        0        0     3716 2023-02-28 12:30:03.000000 freerec-0.3.1/freerec/data/datasets/sequential/amazon.py
+-rw-rw-rw-   0        0        0     2818 2023-02-28 12:32:59.000000 freerec-0.3.1/freerec/data/datasets/sequential/base.py
+-rw-rw-rw-   0        0        0     1792 2023-02-28 12:30:30.000000 freerec-0.3.1/freerec/data/datasets/sequential/movielens.py
+-rw-rw-rw-   0        0        0     1794 2023-02-28 12:31:02.000000 freerec-0.3.1/freerec/data/datasets/sequential/steam.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.726441 freerec-0.3.1/freerec/data/datasets/session/
+-rw-rw-rw-   0        0        0        0 2023-02-26 02:12:38.000000 freerec-0.3.1/freerec/data/datasets/session/__init__.py
+-rw-rw-rw-   0        0        0      209 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/datasets/session/base.py
+-rw-rw-rw-   0        0        0    29454 2023-03-10 09:09:02.000000 freerec-0.3.1/freerec/data/fields.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.779778 freerec-0.3.1/freerec/data/postprocessing/
+-rw-rw-rw-   0        0        0      111 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2713 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/postprocessing/base.py
+-rw-rw-rw-   0        0        0     2177 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/postprocessing/column.py
+-rw-rw-rw-   0        0        0    10232 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/postprocessing/row.py
+-rw-rw-rw-   0        0        0    17697 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/postprocessing/sampler.py
+-rw-rw-rw-   0        0        0     2737 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/data/postprocessing/source.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.792838 freerec-0.3.1/freerec/data/preprocessing/
+-rw-rw-rw-   0        0        0       62 2023-03-24 02:17:25.000000 freerec-0.3.1/freerec/data/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0    18771 2023-03-26 11:55:18.000000 freerec-0.3.1/freerec/data/preprocessing/base.py
+-rw-rw-rw-   0        0        0     7748 2023-04-06 04:06:45.000000 freerec-0.3.1/freerec/data/preprocessing/datasets.py
+-rw-rw-rw-   0        0        0      807 2023-03-23 07:09:59.000000 freerec-0.3.1/freerec/data/tags.py
+-rw-rw-rw-   0        0        0     4533 2023-02-26 11:58:59.000000 freerec-0.3.1/freerec/data/transformation.py
+-rw-rw-rw-   0        0        0     7457 2023-03-17 12:50:23.000000 freerec-0.3.1/freerec/data/utils.py
+-rw-rw-rw-   0        0        0     3101 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/dict2obj.py
+-rw-rw-rw-   0        0        0    31008 2023-04-09 01:47:49.000000 freerec-0.3.1/freerec/launcher.py
+-rw-rw-rw-   0        0        0    22071 2023-03-27 11:15:13.000000 freerec-0.3.1/freerec/metrics.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.793837 freerec-0.3.1/freerec/models/
+-rw-rw-rw-   0        0        0       23 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/models/__init__.py
+-rw-rw-rw-   0        0        0     3289 2023-02-24 08:54:11.000000 freerec-0.3.1/freerec/models/base.py
+-rw-rw-rw-   0        0        0    16542 2023-03-24 05:56:11.000000 freerec-0.3.1/freerec/parser.py
+-rw-rw-rw-   0        0        0    14588 2023-03-16 13:10:40.000000 freerec-0.3.1/freerec/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:11:27.562370 freerec-0.3.1/freerec.egg-info/
+-rw-rw-rw-   0        0        0     1814 2023-04-09 03:11:27.000000 freerec-0.3.1/freerec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1675 2023-04-09 03:11:27.000000 freerec-0.3.1/freerec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 03:11:27.000000 freerec-0.3.1/freerec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-09 03:11:27.000000 freerec-0.3.1/freerec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      111 2023-04-09 03:11:27.000000 freerec-0.3.1/freerec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-09 03:11:27.000000 freerec-0.3.1/freerec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 03:11:27.795427 freerec-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1180 2023-03-24 05:54:08.000000 freerec-0.3.1/setup.py
```

### Comparing `freerec-0.2.5/LICENSE` & `freerec-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/PKG-INFO` & `freerec-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freerec
-Version: 0.2.5
+Version: 0.3.1
 Summary: PyTorch library for recommender systems
 Home-page: https://github.com/MTandHJ/freerec
 Author: MTandHJ
 Author-email: congxueric@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -34,14 +34,17 @@
 
 
 
 ## Data Pipeline
 
 ![](docs/src/pipeline.png)
 
+**Note:** To make dataset, please download corresponding Atomic files from [[RecBole](https://drive.google.com/drive/folders/1so0lckI6N6_niVEYaBu-LIcpOdZf99kj)]. 
+Then, run `make_dataset.ipynb'.
+
 ## Training Flow
 
 
 ![](docs/src/flow.png)
 
 
 ## Reference Code
```

### Comparing `freerec-0.2.5/freerec/criterions.py` & `freerec-0.3.1/freerec/criterions.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/data/dataloader.py` & `freerec-0.3.1/freerec/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/data/datasets/base.py` & `freerec-0.3.1/freerec/data/datasets/base.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/data/datasets/general/amazon.py` & `freerec-0.3.1/freerec/data/datasets/general/amazon.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/data/datasets/general/base.py` & `freerec-0.3.1/freerec/data/datasets/general/base.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/data/datasets/general/gowalla.py` & `freerec-0.3.1/freerec/data/datasets/general/gowalla.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/data/datasets/general/movielens.py` & `freerec-0.3.1/freerec/data/datasets/general/movielens.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/data/datasets/general/yelp.py` & `freerec-0.3.1/freerec/data/datasets/general/yelp.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/data/datasets/sequential/amazon.py` & `freerec-0.3.1/freerec/data/datasets/sequential/amazon.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/data/datasets/sequential/base.py` & `freerec-0.3.1/freerec/data/datasets/sequential/base.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/data/datasets/sequential/movielens.py` & `freerec-0.3.1/freerec/data/datasets/sequential/movielens.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/data/datasets/sequential/steam.py` & `freerec-0.3.1/freerec/data/datasets/sequential/steam.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/data/fields.py` & `freerec-0.3.1/freerec/data/fields.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/data/postprocessing/base.py` & `freerec-0.3.1/freerec/data/postprocessing/base.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/data/postprocessing/column.py` & `freerec-0.3.1/freerec/data/postprocessing/column.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/data/postprocessing/row.py` & `freerec-0.3.1/freerec/data/postprocessing/row.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/data/postprocessing/sampler.py` & `freerec-0.3.1/freerec/data/postprocessing/sampler.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/data/postprocessing/source.py` & `freerec-0.3.1/freerec/data/postprocessing/source.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/data/tags.py` & `freerec-0.3.1/freerec/data/tags.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,29 +4,33 @@
 
 
 class FieldTags(Enum):
     Sparse = 'Sparse'
     Dense = 'Dense'
     User = 'User'
     Item = 'Item'
+    Interaction = 'Interaction'
     Timestamp = 'Timestamp'
+    Rating = 'Rating'
     ID = 'ID'
     Feature = 'Feature'
     Target = 'Target'
     Positive = 'Positive'
     Negative = 'Negative'
     Seen = 'Seen'
     Unseen = 'Unseen'
 
 
 SPARSE = FieldTags('Sparse')
 DENSE = FieldTags('Dense')
 USER = FieldTags('User')
 ITEM = FieldTags('Item')
+INTERACTION = FieldTags('Interaction')
 TIMESTAMP = FieldTags('Timestamp')
+RATING = FieldTags('Rating')
 ID = FieldTags('ID')
 FEATURE = FieldTags('Feature')
 TARGET = FieldTags('Target')
 POSITIVE = FieldTags('Positive')
 NEGATIVE = FieldTags('Negative')
 SEEN = FieldTags('Seen')
 UNSEEN = FieldTags('Unseen')
```

### Comparing `freerec-0.2.5/freerec/data/transformation.py` & `freerec-0.3.1/freerec/data/transformation.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/data/utils.py` & `freerec-0.3.1/freerec/data/utils.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/dict2obj.py` & `freerec-0.3.1/freerec/dict2obj.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/launcher.py` & `freerec-0.3.1/freerec/launcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,1826 +2,1937 @@
 00000010: 696d 706f 7274 2041 6e79 2c20 4361 6c6c  import Any, Call
 00000020: 6162 6c65 2c20 4974 6572 6162 6c65 2c20  able, Iterable, 
 00000030: 4c69 7374 2c20 4469 6374 2c20 4f70 7469  List, Dict, Opti
 00000040: 6f6e 616c 2c20 5475 706c 652c 2055 6e69  onal, Tuple, Uni
 00000050: 6f6e 0d0a 0d0a 696d 706f 7274 2074 6f72  on....import tor
 00000060: 6368 2c20 6162 632c 206f 732c 2073 7562  ch, abc, os, sub
 00000070: 7072 6f63 6573 732c 2073 686c 6578 2c20  process, shlex, 
-00000080: 7469 6d65 2c20 7379 730d 0a69 6d70 6f72  time, sys..impor
-00000090: 7420 7061 6e64 6173 2061 7320 7064 0d0a  t pandas as pd..
-000000a0: 6672 6f6d 2074 6f72 6368 6461 7461 2e64  from torchdata.d
-000000b0: 6174 6170 6970 6573 2e69 7465 7220 696d  atapipes.iter im
-000000c0: 706f 7274 2049 7465 7244 6174 6150 6970  port IterDataPip
-000000d0: 650d 0a66 726f 6d20 746f 7263 682e 7574  e..from torch.ut
-000000e0: 696c 732e 7465 6e73 6f72 626f 6172 6420  ils.tensorboard 
-000000f0: 696d 706f 7274 2053 756d 6d61 7279 5772  import SummaryWr
-00000100: 6974 6572 0d0a 6672 6f6d 2066 756e 6374  iter..from funct
-00000110: 6f6f 6c73 2069 6d70 6f72 7420 7061 7274  ools import part
-00000120: 6961 6c0d 0a66 726f 6d20 6974 6572 746f  ial..from iterto
-00000130: 6f6c 7320 696d 706f 7274 2070 726f 6475  ols import produ
-00000140: 6374 0d0a 6672 6f6d 2063 6f6c 6c65 6374  ct..from collect
-00000150: 696f 6e73 2069 6d70 6f72 7420 6465 6661  ions import defa
-00000160: 756c 7464 6963 740d 0a66 726f 6d20 6672  ultdict..from fr
-00000170: 6565 706c 6f74 2e75 7469 6c73 2069 6d70  eeplot.utils imp
-00000180: 6f72 7420 696d 706f 7274 5f70 6963 6b6c  ort import_pickl
-00000190: 652c 2065 7870 6f72 745f 7069 636b 6c65  e, export_pickle
-000001a0: 0d0a 0d0a 6672 6f6d 202e 6461 7461 2e66  ....from .data.f
-000001b0: 6965 6c64 7320 696d 706f 7274 2046 6965  ields import Fie
-000001c0: 6c64 4d6f 6475 6c65 2c20 4669 656c 6454  ldModule, FieldT
-000001d0: 7570 6c65 0d0a 6672 6f6d 202e 6461 7461  uple..from .data
-000001e0: 2e64 6174 616c 6f61 6465 7220 696d 706f  .dataloader impo
-000001f0: 7274 2044 6174 614c 6f61 6465 720d 0a66  rt DataLoader..f
-00000200: 726f 6d20 2e6d 6f64 656c 7320 696d 706f  rom .models impo
-00000210: 7274 2052 6563 5379 7341 7263 680d 0a66  rt RecSysArch..f
-00000220: 726f 6d20 2e63 7269 7465 7269 6f6e 7320  rom .criterions 
-00000230: 696d 706f 7274 2042 6173 6543 7269 7465  import BaseCrite
-00000240: 7269 6f6e 0d0a 6672 6f6d 202e 6469 6374  rion..from .dict
-00000250: 326f 626a 2069 6d70 6f72 7420 436f 6e66  2obj import Conf
-00000260: 6967 0d0a 6672 6f6d 202e 7574 696c 7320  ig..from .utils 
-00000270: 696d 706f 7274 2041 7665 7261 6765 4d65  import AverageMe
-00000280: 7465 722c 204d 6f6e 6974 6f72 2c20 7469  ter, Monitor, ti
-00000290: 6d65 6d65 7465 722c 2069 6e66 6f4c 6f67  memeter, infoLog
-000002a0: 6765 720d 0a66 726f 6d20 2e6d 6574 7269  ger..from .metri
-000002b0: 6373 2069 6d70 6f72 7420 2a0d 0a66 726f  cs import *..fro
-000002c0: 6d20 2e70 6172 7365 7220 696d 706f 7274  m .parser import
-000002d0: 2054 494d 450d 0a0d 0a0d 0a5f 5f61 6c6c   TIME......__all
-000002e0: 5f5f 203d 205b 2743 6869 6566 436f 6163  __ = ['ChiefCoac
-000002f0: 6827 2c20 2743 6f61 6368 272c 2027 4164  h', 'Coach', 'Ad
-00000300: 6170 7465 7227 5d0d 0a0d 0a0d 0a44 4546  apter']......DEF
-00000310: 4155 4c54 5f4d 4554 5249 4353 203d 207b  AULT_METRICS = {
-00000320: 0d0a 2020 2020 274c 4f53 5327 3a20 6c61  ..    'LOSS': la
-00000330: 6d62 6461 2078 3a20 782c 0d0a 2020 2020  mbda x: x,..    
-00000340: 2323 2323 2323 2323 2323 2323 230d 0a20  #############.. 
-00000350: 2020 2027 4d53 4527 3a20 6d65 616e 5f73     'MSE': mean_s
-00000360: 7175 6172 6564 5f65 7272 6f72 2c0d 0a20  quared_error,.. 
-00000370: 2020 2027 4d41 4527 3a20 6d65 616e 5f61     'MAE': mean_a
-00000380: 6273 5f65 7272 6f72 2c0d 0a20 2020 2027  bs_error,..    '
-00000390: 524d 5345 273a 2072 6f6f 745f 6d73 652c  RMSE': root_mse,
-000003a0: 0d0a 2020 2020 2323 2323 2323 2323 2323  ..    ##########
-000003b0: 2323 230d 0a20 2020 2027 5052 4543 4953  ###..    'PRECIS
-000003c0: 494f 4e27 3a20 7072 6563 6973 696f 6e2c  ION': precision,
-000003d0: 0d0a 2020 2020 2752 4543 414c 4c27 3a20  ..    'RECALL': 
-000003e0: 7265 6361 6c6c 2c0d 0a20 2020 2027 4631  recall,..    'F1
-000003f0: 273a 2066 315f 7363 6f72 652c 0d0a 2020  ': f1_score,..  
-00000400: 2020 2741 5543 273a 2061 7572 6f63 2c0d    'AUC': auroc,.
-00000410: 0a20 2020 2027 4849 5452 4154 4527 3a20  .    'HITRATE': 
-00000420: 6869 745f 7261 7465 2c0d 0a20 2020 2023  hit_rate,..    #
-00000430: 2323 2323 2323 2323 2323 2323 0d0a 2020  ############..  
-00000440: 2020 274e 4443 4727 3a20 6e6f 726d 616c    'NDCG': normal
-00000450: 697a 6564 5f64 6367 2c0d 0a20 2020 2027  ized_dcg,..    '
-00000460: 4d52 5227 3a20 6d65 616e 5f72 6563 6970  MRR': mean_recip
-00000470: 726f 6361 6c5f 7261 6e6b 2c0d 0a20 2020  rocal_rank,..   
-00000480: 2027 4d41 5027 3a20 6d65 616e 5f61 7665   'MAP': mean_ave
-00000490: 7261 6765 5f70 7265 6369 7369 6f6e 0d0a  rage_precision..
-000004a0: 7d0d 0a0d 0a44 4546 4155 4c54 5f46 4d54  }....DEFAULT_FMT
-000004b0: 5320 3d20 7b0d 0a20 2020 2027 4c4f 5353  S = {..    'LOSS
-000004c0: 273a 2022 2e35 6622 2c0d 0a20 2020 2023  ': ".5f",..    #
-000004d0: 2323 2323 2323 2323 2323 2323 0d0a 2020  ############..  
-000004e0: 2020 274d 5345 273a 2022 2e34 6622 2c0d    'MSE': ".4f",.
-000004f0: 0a20 2020 2027 4d41 4527 3a20 222e 3466  .    'MAE': ".4f
-00000500: 222c 0d0a 2020 2020 2752 4d53 4527 3a20  ",..    'RMSE': 
-00000510: 222e 3466 222c 0d0a 2020 2020 2323 2323  ".4f",..    ####
-00000520: 2323 2323 2323 2323 230d 0a20 2020 2027  #########..    '
-00000530: 5052 4543 4953 494f 4e27 3a20 222e 3466  PRECISION': ".4f
-00000540: 222c 0d0a 2020 2020 2752 4543 414c 4c27  ",..    'RECALL'
-00000550: 3a20 222e 3466 222c 0d0a 2020 2020 2746  : ".4f",..    'F
-00000560: 3127 3a20 222e 3466 222c 0d0a 2020 2020  1': ".4f",..    
-00000570: 2741 5543 273a 2022 2e34 6622 2c0d 0a20  'AUC': ".4f",.. 
-00000580: 2020 2027 4849 5452 4154 4527 3a20 222e     'HITRATE': ".
-00000590: 3466 222c 0d0a 2020 2020 2323 2323 2323  4f",..    ######
-000005a0: 2323 2323 2323 230d 0a20 2020 2027 4e44  #######..    'ND
-000005b0: 4347 273a 2022 2e34 6622 2c0d 0a20 2020  CG': ".4f",..   
-000005c0: 2027 4d52 5227 3a20 222e 3466 222c 0d0a   'MRR': ".4f",..
-000005d0: 2020 2020 274d 4150 273a 2022 2e34 6622      'MAP': ".4f"
-000005e0: 2c0d 0a7d 0d0a 0d0a 4445 4641 554c 545f  ,..}....DEFAULT_
-000005f0: 4245 5354 5f43 4153 5445 5220 3d20 7b0d  BEST_CASTER = {.
-00000600: 0a20 2020 2027 4c4f 5353 273a 206d 696e  .    'LOSS': min
-00000610: 2c0d 0a20 2020 2023 2323 2323 2323 2323  ,..    #########
-00000620: 2323 2323 0d0a 2020 2020 274d 5345 273a  ####..    'MSE':
-00000630: 206d 696e 2c0d 0a20 2020 2027 4d41 4527   min,..    'MAE'
-00000640: 3a20 6d69 6e2c 0d0a 2020 2020 2752 4d53  : min,..    'RMS
-00000650: 4527 3a20 6d69 6e2c 0d0a 2020 2020 2323  E': min,..    ##
-00000660: 2323 2323 2323 2323 2323 230d 0a20 2020  ###########..   
-00000670: 2027 5052 4543 4953 494f 4e27 3a20 6d61   'PRECISION': ma
-00000680: 782c 0d0a 2020 2020 2752 4543 414c 4c27  x,..    'RECALL'
-00000690: 3a20 6d61 782c 0d0a 2020 2020 2746 3127  : max,..    'F1'
-000006a0: 3a20 6d61 782c 0d0a 2020 2020 2741 5543  : max,..    'AUC
-000006b0: 273a 206d 6178 2c0d 0a20 2020 2027 4849  ': max,..    'HI
-000006c0: 5452 4154 4527 3a20 6d61 782c 0d0a 2020  TRATE': max,..  
-000006d0: 2020 2323 2323 2323 2323 2323 2323 230d    #############.
-000006e0: 0a20 2020 2027 4e44 4347 273a 206d 6178  .    'NDCG': max
-000006f0: 2c0d 0a20 2020 2027 4d52 5227 3a20 6d61  ,..    'MRR': ma
-00000700: 782c 0d0a 2020 2020 274d 4150 273a 206d  x,..    'MAP': m
-00000710: 6178 2c0d 0a7d 0d0a 0d0a 0d0a 636c 6173  ax,..}......clas
-00000720: 7320 5f44 756d 6d79 4d6f 6475 6c65 2874  s _DummyModule(t
-00000730: 6f72 6368 2e6e 6e2e 4d6f 6475 6c65 293a  orch.nn.Module):
-00000740: 0d0a 2020 2020 2222 2254 6869 7320 6973  ..    """This is
-00000750: 2061 2064 756d 6d79 206d 6f64 756c 6520   a dummy module 
-00000760: 7468 6174 2073 6572 7665 7320 6173 2061  that serves as a
-00000770: 2070 6c61 6365 686f 6c64 6572 2066 6f72   placeholder for
-00000780: 2061 2072 6561 6c20 6d6f 6465 6c2e 2222   a real model.""
-00000790: 220d 0a20 2020 2064 6566 2066 6f72 7761  "..    def forwa
-000007a0: 7264 2873 656c 662c 202a 6172 6773 2c20  rd(self, *args, 
-000007b0: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
-000007c0: 2020 2020 2222 2244 756d 6d79 2066 6f72      """Dummy for
-000007d0: 7761 7264 206d 6574 686f 6420 7468 6174  ward method that
-000007e0: 2072 6169 7365 7320 6120 604e 6f74 496d   raises a `NotIm
-000007f0: 706c 656d 656e 7465 6445 7272 6f72 602e  plementedError`.
-00000800: 2222 220d 0a20 2020 2020 2020 2072 6169  """..        rai
-00000810: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
-00000820: 6445 7272 6f72 2822 4e6f 206d 6f64 656c  dError("No model
-00000830: 2061 7661 696c 6162 6c65 2066 6f72 2043   available for C
-00000840: 6f61 6368 202e 2e2e 2229 0d0a 0d0a 2020  oach ...")....  
-00000850: 2020 6465 6620 7374 6570 2873 656c 662c    def step(self,
-00000860: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
-00000870: 293a 0d0a 2020 2020 2020 2020 2222 2244  ):..        """D
-00000880: 756d 6d79 2073 7465 7020 6d65 7468 6f64  ummy step method
-00000890: 2074 6861 7420 7261 6973 6573 2061 2060   that raises a `
-000008a0: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
-000008b0: 726f 7260 2e22 2222 0d0a 2020 2020 2020  ror`."""..      
-000008c0: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
-000008d0: 6d65 6e74 6564 4572 726f 7228 224e 6f20  mentedError("No 
-000008e0: 6f70 7469 6d69 7a65 7220 6f72 206c 7220  optimizer or lr 
-000008f0: 7363 6865 6475 6c65 7220 6176 6169 6c61  scheduler availa
-00000900: 626c 6520 666f 7220 436f 6163 6820 2e2e  ble for Coach ..
-00000910: 2e22 290d 0a0d 0a20 2020 2064 6566 2062  .")....    def b
-00000920: 6163 6b77 6172 6428 7365 6c66 2c20 2a61  ackward(self, *a
-00000930: 7267 732c 202a 2a6b 7761 7267 7329 3a0d  rgs, **kwargs):.
-00000940: 0a20 2020 2020 2020 2022 2222 4475 6d6d  .        """Dumm
-00000950: 7920 6261 636b 7761 7264 206d 6574 686f  y backward metho
-00000960: 6420 7468 6174 2072 6169 7365 7320 6120  d that raises a 
-00000970: 604e 6f74 496d 706c 656d 656e 7465 6445  `NotImplementedE
-00000980: 7272 6f72 602e 2222 220d 0a20 2020 2020  rror`."""..     
-00000990: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
-000009a0: 656d 656e 7465 6445 7272 6f72 2822 4e6f  ementedError("No
-000009b0: 206f 7074 696d 697a 6572 2061 7661 696c   optimizer avail
-000009c0: 6162 6c65 2066 6f72 2043 6f61 6368 202e  able for Coach .
-000009d0: 2e2e 2229 0d0a 0d0a 0d0a 636c 6173 7320  ..")......class 
-000009e0: 4368 6965 6643 6f61 6368 286d 6574 6163  ChiefCoach(metac
-000009f0: 6c61 7373 3d61 6263 2e41 4243 4d65 7461  lass=abc.ABCMeta
-00000a00: 293a 0d0a 2020 2020 7222 2222 200d 0a20  ):..    r""" .. 
-00000a10: 2020 2054 6865 2060 4368 6965 6643 6f61     The `ChiefCoa
-00000a20: 6368 6020 636c 6173 7320 6973 2074 6865  ch` class is the
-00000a30: 2074 6f70 2d6c 6576 656c 2063 6c61 7373   top-level class
-00000a40: 2066 6f72 2072 756e 6e69 6e67 2074 6865   for running the
-00000a50: 2074 7261 696e 696e 6720 616e 6420 6576   training and ev
-00000a60: 616c 7561 7469 6f6e 206c 6f6f 7073 2e0d  aluation loops..
-00000a70: 0a0d 0a20 2020 2050 6172 616d 6574 6572  ...    Parameter
-00000a80: 733a 0d0a 2020 2020 2d2d 2d2d 2d2d 2d2d  s:..    --------
-00000a90: 2d2d 2d0d 0a20 2020 2074 7261 696e 7069  ---..    trainpi
-00000aa0: 7065 203a 2049 7465 7244 6174 6150 6970  pe : IterDataPip
-00000ab0: 650d 0a20 2020 2020 2020 2049 7465 7261  e..        Itera
-00000ac0: 626c 6520 6461 7461 2070 6970 656c 696e  ble data pipelin
-00000ad0: 6520 666f 7220 7472 6169 6e69 6e67 2064  e for training d
-00000ae0: 6174 612e 0d0a 2020 2020 7661 6c69 6470  ata...    validp
-00000af0: 6970 6520 3a20 4974 6572 4461 7461 5069  ipe : IterDataPi
-00000b00: 7065 2c20 6f70 7469 6f6e 616c 0d0a 2020  pe, optional..  
-00000b10: 2020 2020 2020 4974 6572 6162 6c65 2064        Iterable d
-00000b20: 6174 6120 7069 7065 6c69 6e65 2066 6f72  ata pipeline for
-00000b30: 2076 616c 6964 6174 696f 6e20 6461 7461   validation data
-00000b40: 2e0d 0a20 2020 2020 2020 2049 6620 604e  ...        If `N
-00000b50: 6f6e 6560 2c20 7573 6520 6074 7261 696e  one`, use `train
-00000b60: 7069 7065 6020 696e 7374 6561 642e 0d0a  pipe` instead...
-00000b70: 2020 2020 7465 7374 7069 7065 203a 2049      testpipe : I
-00000b80: 7465 7244 6174 6150 6970 652c 206f 7074  terDataPipe, opt
-00000b90: 696f 6e61 6c0d 0a20 2020 2020 2020 2049  ional..        I
-00000ba0: 7465 7261 626c 6520 6461 7461 2070 6970  terable data pip
-00000bb0: 656c 696e 6520 666f 7220 7465 7374 696e  eline for testin
-00000bc0: 6720 6461 7461 2e0d 0a20 2020 2020 2020  g data...       
-00000bd0: 2049 6620 604e 6f6e 6560 2c20 7573 6520   If `None`, use 
-00000be0: 6076 616c 6964 7069 7065 6020 696e 7374  `validpipe` inst
-00000bf0: 6561 642e 0d0a 2020 2020 6669 656c 6473  ead...    fields
-00000c00: 203a 2049 7465 7261 626c 655b 4669 656c   : Iterable[Fiel
-00000c10: 644d 6f64 756c 655d 0d0a 2020 2020 2020  dModule]..      
-00000c20: 2020 5475 706c 6520 6f66 2060 4669 656c    Tuple of `Fiel
-00000c30: 644d 6f64 756c 6560 7320 666f 7220 6461  dModule`s for da
-00000c40: 7461 7365 7420 6669 656c 6473 2e0d 0a20  taset fields... 
-00000c50: 2020 206d 6f64 656c 203a 2055 6e69 6f6e     model : Union
-00000c60: 5b52 6563 5379 7341 7263 682c 2074 6f72  [RecSysArch, tor
-00000c70: 6368 2e6e 6e2e 4d6f 6475 6c65 2c20 4e6f  ch.nn.Module, No
-00000c80: 6e65 5d0d 0a20 2020 2020 2020 204d 6f64  ne]..        Mod
-00000c90: 656c 2066 6f72 2074 7261 696e 696e 6720  el for training 
-00000ca0: 616e 6420 6576 616c 7561 7469 6e67 2e20  and evaluating. 
-00000cb0: 0d0a 2020 2020 2020 2020 4966 2060 4e6f  ..        If `No
-00000cc0: 6e65 602c 2075 7365 205f 4475 6d6d 794d  ne`, use _DummyM
-00000cd0: 6f64 756c 6520 696e 7374 6561 642c 2077  odule instead, w
-00000ce0: 6869 6368 2073 686f 756c 6420 6e6f 7420  hich should not 
-00000cf0: 6361 6c6c 2060 666f 7277 6172 6460 2e0d  call `forward`..
-00000d00: 0a20 2020 2063 7269 7465 7269 6f6e 203a  .    criterion :
-00000d10: 2055 6e69 6f6e 5b42 6173 6543 7269 7465   Union[BaseCrite
-00000d20: 7269 6f6e 2c20 4361 6c6c 6162 6c65 5d0d  rion, Callable].
-00000d30: 0a20 2020 2020 2020 2043 616c 6c61 626c  .        Callabl
-00000d40: 6520 666f 7220 636f 6d70 7574 696e 6720  e for computing 
-00000d50: 7468 6520 6c6f 7373 2066 756e 6374 696f  the loss functio
-00000d60: 6e2e 0d0a 2020 2020 6f70 7469 6d69 7a65  n...    optimize
-00000d70: 7220 3a20 746f 7263 682e 6f70 7469 6d2e  r : torch.optim.
-00000d80: 4f70 7469 6d69 7a65 722c 206f 7074 696f  Optimizer, optio
-00000d90: 6e61 6c0d 0a20 2020 2020 2020 204f 7074  nal..        Opt
-00000da0: 696d 697a 6572 2066 6f72 2075 7064 6174  imizer for updat
-00000db0: 696e 6720 6d6f 6465 6c20 7061 7261 6d65  ing model parame
-00000dc0: 7465 7273 2e20 0d0a 2020 2020 2020 2020  ters. ..        
-00000dd0: 4966 2060 4e6f 6e65 602c 2075 7365 205f  If `None`, use _
-00000de0: 4475 6d6d 794d 6f64 756c 6520 696e 7374  DummyModule inst
-00000df0: 6561 642c 2077 6869 6368 2073 686f 756c  ead, which shoul
-00000e00: 6420 6e6f 7420 6361 6c6c 2060 7374 6570  d not call `step
-00000e10: 6020 616e 6420 6062 6163 6b77 6172 6460  ` and `backward`
-00000e20: 2e0d 0a20 2020 206c 725f 7363 6865 6475  ...    lr_schedu
-00000e30: 6c65 7220 3a20 746f 7263 682e 6f70 7469  ler : torch.opti
-00000e40: 6d2e 6c72 5f73 6368 6564 756c 6572 2e5f  m.lr_scheduler._
-00000e50: 4c52 5363 6865 6475 6c65 722c 206f 7074  LRScheduler, opt
-00000e60: 696f 6e61 6c0d 0a20 2020 2020 2020 204c  ional..        L
-00000e70: 6561 726e 696e 6720 7261 7465 2073 6368  earning rate sch
-00000e80: 6564 756c 6572 2e20 4966 2060 4e6f 6e65  eduler. If `None
-00000e90: 602c 2075 7365 205f 4475 6d6d 794d 6f64  `, use _DummyMod
-00000ea0: 756c 6520 696e 7374 6561 642c 200d 0a20  ule instead, .. 
-00000eb0: 2020 2020 2020 2077 6869 6368 2073 686f         which sho
-00000ec0: 756c 6420 6e6f 7420 6361 6c6c 2060 7374  uld not call `st
-00000ed0: 6570 602e 0d0a 2020 2020 6465 7669 6365  ep`...    device
-00000ee0: 203a 2055 6e69 6f6e 5b74 6f72 6368 2e64   : Union[torch.d
-00000ef0: 6576 6963 652c 2073 7472 2c20 696e 745d  evice, str, int]
-00000f00: 0d0a 2020 2020 2020 2020 4465 7669 6365  ..        Device
-00000f10: 206f 6e20 7768 6963 6820 746f 2072 756e   on which to run
-00000f20: 2074 6865 2063 6f6d 7075 7461 7469 6f6e   the computation
-00000f30: 2e20 0d0a 2020 2020 2020 2020 2020 2020  . ..            
-00000f40: 2d20 6074 6f72 6368 2e64 6576 6963 6560  - `torch.device`
-00000f50: 0d0a 2020 2020 2020 2020 2020 2020 2d20  ..            - 
-00000f60: 6073 7472 603a 204c 696b 6520 6063 7075  `str`: Like `cpu
-00000f70: 602c 2060 6375 6461 3a30 602e 0d0a 2020  `, `cuda:0`...  
-00000f80: 2020 2020 2020 2020 2020 2d20 6069 6e74            - `int
-00000f90: 603a 2055 7369 6e67 2063 7564 613a 6069  `: Using cuda:`i
-00000fa0: 6e74 602e 0d0a 2020 2020 2222 220d 0a0d  nt`...    """...
-00000fb0: 0a0d 0a20 2020 2064 6566 205f 5f69 6e69  ...    def __ini
-00000fc0: 745f 5f28 0d0a 2020 2020 2020 2020 7365  t__(..        se
-00000fd0: 6c66 2c20 2a2c 0d0a 2020 2020 2020 2020  lf, *,..        
-00000fe0: 7472 6169 6e70 6970 653a 2049 7465 7244  trainpipe: IterD
-00000ff0: 6174 6150 6970 652c 2076 616c 6964 7069  ataPipe, validpi
-00001000: 7065 3a20 4f70 7469 6f6e 616c 5b49 7465  pe: Optional[Ite
-00001010: 7244 6174 6150 6970 655d 2c20 7465 7374  rDataPipe], test
-00001020: 7069 7065 3a20 4f70 7469 6f6e 616c 5b49  pipe: Optional[I
-00001030: 7465 7244 6174 6150 6970 655d 2c20 6669  terDataPipe], fi
-00001040: 656c 6473 3a20 4974 6572 6162 6c65 5b46  elds: Iterable[F
-00001050: 6965 6c64 4d6f 6475 6c65 5d2c 0d0a 2020  ieldModule],..  
-00001060: 2020 2020 2020 6d6f 6465 6c3a 2055 6e69        model: Uni
-00001070: 6f6e 5b52 6563 5379 7341 7263 682c 2074  on[RecSysArch, t
-00001080: 6f72 6368 2e6e 6e2e 4d6f 6475 6c65 2c20  orch.nn.Module, 
-00001090: 4e6f 6e65 5d2c 2063 7269 7465 7269 6f6e  None], criterion
-000010a0: 3a20 556e 696f 6e5b 4261 7365 4372 6974  : Union[BaseCrit
-000010b0: 6572 696f 6e2c 2043 616c 6c61 626c 655d  erion, Callable]
-000010c0: 2c20 0d0a 2020 2020 2020 2020 6f70 7469  , ..        opti
-000010d0: 6d69 7a65 723a 204f 7074 696f 6e61 6c5b  mizer: Optional[
-000010e0: 746f 7263 682e 6f70 7469 6d2e 4f70 7469  torch.optim.Opti
-000010f0: 6d69 7a65 725d 2c20 6c72 5f73 6368 6564  mizer], lr_sched
-00001100: 756c 6572 3a20 4f70 7469 6f6e 616c 5b74  uler: Optional[t
-00001110: 6f72 6368 2e6f 7074 696d 2e6c 725f 7363  orch.optim.lr_sc
-00001120: 6865 6475 6c65 722e 5f4c 5253 6368 6564  heduler._LRSched
-00001130: 756c 6572 5d2c 0d0a 2020 2020 2020 2020  uler],..        
-00001140: 6465 7669 6365 3a20 556e 696f 6e5b 746f  device: Union[to
-00001150: 7263 682e 6465 7669 6365 2c20 7374 722c  rch.device, str,
-00001160: 2069 6e74 5d0d 0a20 2020 2029 3a0d 0a0d   int]..    ):...
-00001170: 0a20 2020 2020 2020 2073 656c 662e 6669  .        self.fi
-00001180: 656c 6473 3a20 4669 656c 6454 7570 6c65  elds: FieldTuple
-00001190: 5b46 6965 6c64 4d6f 6475 6c65 5d20 3d20  [FieldModule] = 
-000011a0: 4669 656c 6454 7570 6c65 2866 6965 6c64  FieldTuple(field
-000011b0: 7329 0d0a 2020 2020 2020 2020 7365 6c66  s)..        self
-000011c0: 2e64 6576 6963 6520 3d20 746f 7263 682e  .device = torch.
-000011d0: 6465 7669 6365 2864 6576 6963 6529 0d0a  device(device)..
-000011e0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
-000011f0: 7365 745f 6461 7461 7069 7065 2874 7261  set_datapipe(tra
-00001200: 696e 7069 7065 2c20 7661 6c69 6470 6970  inpipe, validpip
-00001210: 652c 2074 6573 7470 6970 6529 0d0a 2020  e, testpipe)..  
-00001220: 2020 2020 2020 7365 6c66 2e5f 7365 745f        self._set_
-00001230: 6f74 6865 7228 6d6f 6465 6c2c 2063 7269  other(model, cri
-00001240: 7465 7269 6f6e 2c20 6f70 7469 6d69 7a65  terion, optimize
-00001250: 722c 206c 725f 7363 6865 6475 6c65 7229  r, lr_scheduler)
-00001260: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
-00001270: 2e5f 5f6d 6f64 6520 3d20 2774 7261 696e  .__mode = 'train
-00001280: 270d 0a0d 0a20 2020 2064 6566 205f 7365  '....    def _se
-00001290: 745f 6461 7461 7069 7065 280d 0a20 2020  t_datapipe(..   
-000012a0: 2020 2020 2073 656c 662c 0d0a 2020 2020       self,..    
-000012b0: 2020 2020 7472 6169 6e70 6970 652c 0d0a      trainpipe,..
-000012c0: 2020 2020 2020 2020 7661 6c69 6470 6970          validpip
-000012d0: 653d 4e6f 6e65 2c0d 0a20 2020 2020 2020  e=None,..       
-000012e0: 2074 6573 7470 6970 653d 4e6f 6e65 2c0d   testpipe=None,.
-000012f0: 0a20 2020 2029 3a0d 0a20 2020 2020 2020  .    ):..       
-00001300: 2022 2222 5365 7420 7468 6520 6461 7461   """Set the data
-00001310: 2070 6970 6520 666f 7220 7472 6169 6e69   pipe for traini
-00001320: 6e67 2c20 7661 6c69 6461 7469 6f6e 2061  ng, validation a
-00001330: 6e64 2074 6573 742e 2222 220d 0a20 2020  nd test."""..   
-00001340: 2020 2020 2073 656c 662e 7472 6169 6e70       self.trainp
-00001350: 6970 6520 3d20 7472 6169 6e70 6970 650d  ipe = trainpipe.
-00001360: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
-00001370: 6c69 6470 6970 6520 3d20 7365 6c66 2e74  lidpipe = self.t
-00001380: 7261 696e 7069 7065 2069 6620 7661 6c69  rainpipe if vali
-00001390: 6470 6970 6520 6973 204e 6f6e 6520 656c  dpipe is None el
-000013a0: 7365 2076 616c 6964 7069 7065 0d0a 2020  se validpipe..  
-000013b0: 2020 2020 2020 7365 6c66 2e74 6573 7470        self.testp
-000013c0: 6970 6520 3d20 7365 6c66 2e76 616c 6964  ipe = self.valid
-000013d0: 7069 7065 2069 6620 7465 7374 7069 7065  pipe if testpipe
-000013e0: 2069 7320 4e6f 6e65 2065 6c73 6520 7465   is None else te
-000013f0: 7374 7069 7065 0d0a 0d0a 2020 2020 6465  stpipe....    de
-00001400: 6620 5f73 6574 5f6f 7468 6572 280d 0a20  f _set_other(.. 
-00001410: 2020 2020 2020 2073 656c 662c 0d0a 2020         self,..  
-00001420: 2020 2020 2020 6d6f 6465 6c3d 4e6f 6e65        model=None
-00001430: 2c20 6372 6974 6572 696f 6e3d 4e6f 6e65  , criterion=None
-00001440: 2c20 6f70 7469 6d69 7a65 723d 4e6f 6e65  , optimizer=None
-00001450: 2c20 6c72 5f73 6368 6564 756c 6572 3d4e  , lr_scheduler=N
-00001460: 6f6e 652c 0d0a 2020 2020 293a 0d0a 2020  one,..    ):..  
-00001470: 2020 2020 2020 2222 2253 6574 2074 6865        """Set the
-00001480: 206f 7468 6572 206e 6563 6573 7361 7279   other necessary
-00001490: 2063 6f6d 706f 6e65 6e74 732e 2222 220d   components.""".
-000014a0: 0a20 2020 2020 2020 2073 656c 662e 6372  .        self.cr
-000014b0: 6974 6572 696f 6e20 3d20 6372 6974 6572  iterion = criter
-000014c0: 696f 6e0d 0a20 2020 2020 2020 2073 656c  ion..        sel
-000014d0: 662e 6d6f 6465 6c20 3d20 6d6f 6465 6c2e  f.model = model.
-000014e0: 746f 2873 656c 662e 6465 7669 6365 2920  to(self.device) 
-000014f0: 6966 206d 6f64 656c 2065 6c73 6520 5f44  if model else _D
-00001500: 756d 6d79 4d6f 6475 6c65 2829 0d0a 2020  ummyModule()..  
-00001510: 2020 2020 2020 7365 6c66 2e6f 7074 696d        self.optim
-00001520: 697a 6572 203d 206f 7074 696d 697a 6572  izer = optimizer
-00001530: 2069 6620 6f70 7469 6d69 7a65 7220 656c   if optimizer el
-00001540: 7365 205f 4475 6d6d 794d 6f64 756c 6528  se _DummyModule(
-00001550: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00001560: 6c72 5f73 6368 6564 756c 6572 203d 206c  lr_scheduler = l
-00001570: 725f 7363 6865 6475 6c65 7220 6966 206c  r_scheduler if l
-00001580: 725f 7363 6865 6475 6c65 7220 656c 7365  r_scheduler else
-00001590: 205f 4475 6d6d 794d 6f64 756c 6528 290d   _DummyModule().
-000015a0: 0a0d 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
-000015b0: 0d0a 2020 2020 6465 6620 6d6f 6465 2873  ..    def mode(s
-000015c0: 656c 6629 3a0d 0a20 2020 2020 2020 2022  elf):..        "
-000015d0: 2222 4765 7420 7468 6520 6375 7272 656e  ""Get the curren
-000015e0: 7420 6d6f 6465 206f 6620 7468 6520 6368  t mode of the ch
-000015f0: 6965 6620 636f 6163 682e 2222 220d 0a20  ief coach.""".. 
-00001600: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00001610: 6c66 2e5f 5f6d 6f64 650d 0a0d 0a20 2020  lf.__mode....   
-00001620: 2040 7469 6d65 6d65 7465 7228 2243 6f61   @timemeter("Coa
-00001630: 6368 2f74 7261 696e 2229 0d0a 2020 2020  ch/train")..    
-00001640: 6465 6620 7472 6169 6e28 7365 6c66 293a  def train(self):
-00001650: 0d0a 2020 2020 2020 2020 2222 2253 7461  ..        """Sta
-00001660: 7274 2074 7261 696e 696e 6720 616e 6420  rt training and 
-00001670: 7265 7475 726e 2074 6865 2074 7261 696e  return the train
-00001680: 696e 6720 6c6f 7373 2e22 2222 0d0a 2020  ing loss."""..  
-00001690: 2020 2020 2020 7365 6c66 2e5f 5f6d 6f64        self.__mod
-000016a0: 6520 3d20 2774 7261 696e 270d 0a20 2020  e = 'train'..   
-000016b0: 2020 2020 2073 656c 662e 6d6f 6465 6c2e       self.model.
-000016c0: 7472 6169 6e28 290d 0a20 2020 2020 2020  train()..       
-000016d0: 2072 6574 7572 6e20 7365 6c66 2e74 7261   return self.tra
-000016e0: 696e 5f70 6572 5f65 706f 6368 2829 0d0a  in_per_epoch()..
-000016f0: 0d0a 2020 2020 4074 696d 656d 6574 6572  ..    @timemeter
-00001700: 2822 436f 6163 682f 7661 6c69 6422 290d  ("Coach/valid").
-00001710: 0a20 2020 2040 746f 7263 682e 6e6f 5f67  .    @torch.no_g
-00001720: 7261 6428 290d 0a20 2020 2064 6566 2076  rad()..    def v
-00001730: 616c 6964 2873 656c 6629 3a0d 0a20 2020  alid(self):..   
-00001740: 2020 2020 2022 2222 5374 6172 7420 7661       """Start va
-00001750: 6c69 6461 7469 6f6e 2061 6e64 2072 6574  lidation and ret
-00001760: 7572 6e20 7468 6520 7661 6c69 6461 7469  urn the validati
-00001770: 6f6e 206d 6574 7269 6373 2e22 2222 0d0a  on metrics."""..
-00001780: 2020 2020 2020 2020 7365 6c66 2e5f 5f6d          self.__m
-00001790: 6f64 6520 3d20 2776 616c 6964 270d 0a20  ode = 'valid'.. 
-000017a0: 2020 2020 2020 2073 656c 662e 6d6f 6465         self.mode
-000017b0: 6c2e 6576 616c 2829 0d0a 2020 2020 2020  l.eval()..      
-000017c0: 2020 7265 7475 726e 2073 656c 662e 6576    return self.ev
-000017d0: 616c 7561 7465 2870 7265 6669 783d 2776  aluate(prefix='v
-000017e0: 616c 6964 2729 0d0a 0d0a 2020 2020 4074  alid')....    @t
-000017f0: 696d 656d 6574 6572 2822 436f 6163 682f  imemeter("Coach/
-00001800: 7465 7374 2229 0d0a 2020 2020 4074 6f72  test")..    @tor
-00001810: 6368 2e6e 6f5f 6772 6164 2829 0d0a 2020  ch.no_grad()..  
-00001820: 2020 6465 6620 7465 7374 2873 656c 6629    def test(self)
-00001830: 3a0d 0a20 2020 2020 2020 2022 2222 5374  :..        """St
-00001840: 6172 7420 7465 7374 696e 6720 616e 6420  art testing and 
-00001850: 7265 7475 726e 2074 6865 2074 6573 7420  return the test 
-00001860: 6d65 7472 6963 732e 2222 220d 0a20 2020  metrics."""..   
-00001870: 2020 2020 2073 656c 662e 5f5f 6d6f 6465       self.__mode
-00001880: 203d 2027 7465 7374 270d 0a20 2020 2020   = 'test'..     
-00001890: 2020 2073 656c 662e 6d6f 6465 6c2e 6576     self.model.ev
-000018a0: 616c 2829 0d0a 2020 2020 2020 2020 7265  al()..        re
-000018b0: 7475 726e 2073 656c 662e 6576 616c 7561  turn self.evalua
-000018c0: 7465 2870 7265 6669 783d 2774 6573 7427  te(prefix='test'
-000018d0: 290d 0a0d 0a20 2020 2040 6162 632e 6162  )....    @abc.ab
-000018e0: 7374 7261 6374 6d65 7468 6f64 0d0a 2020  stractmethod..  
-000018f0: 2020 6465 6620 7472 6169 6e5f 7065 725f    def train_per_
-00001900: 6570 6f63 6828 7365 6c66 293a 0d0a 2020  epoch(self):..  
-00001910: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
-00001920: 6d70 6c65 6d65 6e74 6564 4572 726f 7228  mplementedError(
-00001930: 0d0a 2020 2020 2020 2020 2020 2020 6622  ..            f"
-00001940: 7b73 656c 662e 5f5f 636c 6173 735f 5f2e  {self.__class__.
-00001950: 5f5f 6e61 6d65 5f5f 7d2e 7472 6169 6e5f  __name__}.train_
-00001960: 7065 725f 6570 6f63 6828 2920 7368 6f75  per_epoch() shou
-00001970: 6c64 2062 6520 696d 706c 656d 656e 7465  ld be implemente
-00001980: 6420 2e2e 2e22 0d0a 2020 2020 2020 2020  d ..."..        
-00001990: 290d 0a0d 0a20 2020 2040 6162 632e 6162  )....    @abc.ab
-000019a0: 7374 7261 6374 6d65 7468 6f64 0d0a 2020  stractmethod..  
-000019b0: 2020 6465 6620 6576 616c 7561 7465 2873    def evaluate(s
-000019c0: 656c 662c 2070 7265 6669 783a 2073 7472  elf, prefix: str
-000019d0: 203d 2027 7661 6c69 6427 293a 0d0a 2020   = 'valid'):..  
-000019e0: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
-000019f0: 6d70 6c65 6d65 6e74 6564 4572 726f 7228  mplementedError(
-00001a00: 0d0a 2020 2020 2020 2020 2020 2020 6622  ..            f"
-00001a10: 7b73 656c 662e 5f5f 636c 6173 735f 5f2e  {self.__class__.
-00001a20: 5f5f 6e61 6d65 5f5f 7d2e 6576 616c 7561  __name__}.evalua
-00001a30: 7465 2829 2073 686f 756c 6420 6265 2069  te() should be i
-00001a40: 6d70 6c65 6d65 6e74 6564 202e 2e2e 220d  mplemented ...".
-00001a50: 0a20 2020 2020 2020 2029 0d0a 0d0a 2020  .        )....  
-00001a60: 2020 6465 6620 7265 6769 7374 6572 5f6d    def register_m
-00001a70: 6574 7269 6328 0d0a 2020 2020 2020 2020  etric(..        
-00001a80: 7365 6c66 2c20 6e61 6d65 3a20 7374 722c  self, name: str,
-00001a90: 2066 756e 633a 2043 616c 6c61 626c 652c   func: Callable,
-00001aa0: 200d 0a20 2020 2020 2020 2066 6d74 3a20   ..        fmt: 
-00001ab0: 7374 7220 3d20 272e 3466 272c 2062 6573  str = '.4f', bes
-00001ac0: 745f 6361 7374 6572 3a20 4361 6c6c 6162  t_caster: Callab
-00001ad0: 6c65 203d 206d 6178 0d0a 2020 2020 2920  le = max..    ) 
-00001ae0: 2d3e 204e 6f6e 653a 0d0a 2020 2020 2020  -> None:..      
-00001af0: 2020 7222 2222 0d0a 2020 2020 2020 2020    r"""..        
-00001b00: 5265 6769 7374 6572 2061 206d 6574 7269  Register a metri
-00001b10: 632e 0d0a 0d0a 2020 2020 2020 2020 5061  c.....        Pa
-00001b20: 7261 6d65 7465 7273 0d0a 2020 2020 2020  rameters..      
-00001b30: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020    ----------..  
-00001b40: 2020 2020 2020 6e61 6d65 203a 2073 7472        name : str
-00001b50: 0d0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-00001b60: 6520 636f 6d70 6c65 7465 206e 616d 6520  e complete name 
-00001b70: 6f66 2074 6865 206d 6574 7269 632c 2073  of the metric, s
-00001b80: 7563 6820 6173 2060 4c4f 5353 3260 2e0d  uch as `LOSS2`..
-00001b90: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-00001ba0: 206e 6f74 6174 696f 6e20 6040 6020 7368   notation `@` sh
-00001bb0: 6f75 6c64 206e 6f74 2062 6520 696e 636c  ould not be incl
-00001bc0: 7564 6564 2c20 692e 652e 2c20 274c 4f53  uded, i.e., 'LOS
-00001bd0: 5340 3227 2069 7320 696e 7661 6c69 642e  S@2' is invalid.
-00001be0: 0d0a 2020 2020 2020 2020 6675 6e63 203a  ..        func :
-00001bf0: 2043 616c 6c61 626c 650d 0a20 2020 2020   Callable..     
-00001c00: 2020 2020 2020 2054 6865 2066 756e 6374         The funct
-00001c10: 696f 6e20 746f 2070 726f 6365 7373 2074  ion to process t
-00001c20: 6865 2064 6174 6120 666f 7220 7468 6520  he data for the 
-00001c30: 6d65 7472 6963 2e0d 0a20 2020 2020 2020  metric...       
-00001c40: 2066 6d74 203a 2073 7472 2c20 6f70 7469   fmt : str, opti
-00001c50: 6f6e 616c 0d0a 2020 2020 2020 2020 2020  onal..          
-00001c60: 2020 5468 6520 666f 726d 6174 2074 6f20    The format to 
-00001c70: 7573 6520 7768 656e 2070 7269 6e74 696e  use when printin
-00001c80: 6720 7468 6520 6d65 7472 6963 2c20 6465  g the metric, de
-00001c90: 6661 756c 7473 2074 6f20 6027 2e34 6627  faults to `'.4f'
-00001ca0: 602e 0d0a 2020 2020 2020 2020 6265 7374  `...        best
-00001cb0: 5f63 6173 7465 7220 3a20 4361 6c6c 6162  _caster : Callab
-00001cc0: 6c65 2c20 6f70 7469 6f6e 616c 0d0a 2020  le, optional..  
-00001cd0: 2020 2020 2020 2020 2020 4120 6675 6e63            A func
-00001ce0: 7469 6f6e 2075 7365 6420 746f 2063 6173  tion used to cas
-00001cf0: 7420 7468 6520 6265 7374 2076 616c 7565  t the best value
-00001d00: 206f 6620 7468 6520 6d65 7472 6963 2c20   of the metric, 
-00001d10: 6465 6661 756c 7473 2074 6f20 606d 6178  defaults to `max
-00001d20: 602e 0d0a 2020 2020 2020 2020 2020 2020  `...            
-00001d30: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00001d40: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
-00001d50: 2d2d 0d0a 2020 2020 2020 2020 4e6f 6e65  --..        None
-00001d60: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00001d70: 2020 2020 5261 6973 6573 0d0a 2020 2020      Raises..    
-00001d80: 2020 2020 2d2d 2d2d 2d2d 0d0a 2020 2020      ------..    
-00001d90: 2020 2020 4173 7365 7274 696f 6e45 7272      AssertionErr
-00001da0: 6f72 0d0a 2020 2020 2020 2020 2020 2020  or..            
-00001db0: 5768 656e 2060 6e61 6d65 6020 6861 7320  When `name` has 
-00001dc0: 616c 7265 6164 7920 6265 656e 2072 6567  already been reg
-00001dd0: 6973 7465 7265 6420 6f72 2063 6f6e 7461  istered or conta
-00001de0: 696e 7320 7468 6520 6e6f 7461 7469 6f6e  ins the notation
-00001df0: 2060 4060 2e0d 0a20 2020 2020 2020 2022   `@`...        "
-00001e00: 2222 0d0a 0d0a 2020 2020 2020 2020 6e61  ""....        na
-00001e10: 6d65 203d 206e 616d 652e 7570 7065 7228  me = name.upper(
-00001e20: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-00001e30: 7420 4445 4641 554c 545f 4d45 5452 4943  t DEFAULT_METRIC
-00001e40: 532e 6765 7428 6e61 6d65 2c20 4e6f 6e65  S.get(name, None
-00001e50: 2920 6973 204e 6f6e 652c 2066 2254 6865  ) is None, f"The
-00001e60: 206d 6574 7269 6320 7b6e 616d 657d 2061   metric {name} a
-00001e70: 6c72 6561 6479 2065 7869 7374 7320 2e2e  lready exists ..
-00001e80: 2e22 0d0a 2020 2020 2020 2020 6173 7365  ."..        asse
-00001e90: 7274 2027 4027 206e 6f74 2069 6e20 6e61  rt '@' not in na
-00001ea0: 6d65 2c20 6622 5468 6520 6d65 7472 6963  me, f"The metric
-00001eb0: 206e 616d 6520 6861 7320 696e 7661 6c69   name has invali
-00001ec0: 6420 6e6f 7461 7469 6f6e 206f 6620 6040  d notation of `@
-00001ed0: 2720 2e2e 2e22 0d0a 2020 2020 2020 2020  ' ..."..        
-00001ee0: 4445 4641 554c 545f 4d45 5452 4943 535b  DEFAULT_METRICS[
-00001ef0: 6e61 6d65 5d20 3d20 6675 6e63 0d0a 2020  name] = func..  
-00001f00: 2020 2020 2020 4445 4641 554c 545f 464d        DEFAULT_FM
-00001f10: 5453 5b6e 616d 655d 203d 2066 6d74 0d0a  TS[name] = fmt..
-00001f20: 2020 2020 2020 2020 4445 4641 554c 545f          DEFAULT_
-00001f30: 4245 5354 5f43 4153 5445 525b 6e61 6d65  BEST_CASTER[name
-00001f40: 5d20 3d20 6265 7374 5f63 6173 7465 720d  ] = best_caster.
-00001f50: 0a0d 0a0d 0a63 6c61 7373 2043 6f61 6368  .....class Coach
-00001f60: 2843 6869 6566 436f 6163 6829 3a0d 0a20  (ChiefCoach):.. 
-00001f70: 2020 2022 2222 5468 6520 6672 616d 6577     """The framew
-00001f80: 6f72 6b20 666f 7220 7472 6169 6e69 6e67  ork for training
-00001f90: 2e22 2222 0d0a 0d0a 2020 2020 6465 6620  ."""....    def 
-00001fa0: 7072 6570 6172 655f 6461 7461 6c6f 6164  prepare_dataload
-00001fb0: 6572 2873 656c 6629 202d 3e20 4e6f 6e65  er(self) -> None
-00001fc0: 3a0d 0a20 2020 2020 2020 2022 2222 5072  :..        """Pr
-00001fd0: 6570 6172 6520 6461 7461 206c 6f61 6465  epare data loade
-00001fe0: 7273 2066 6f72 2074 7261 696e 696e 672c  rs for training,
-00001ff0: 2076 616c 6964 6174 696f 6e2c 2061 6e64   validation, and
-00002000: 2074 6573 7469 6e67 2064 6174 612e 2222   testing data.""
-00002010: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
-00002020: 7472 6169 6e6c 6f61 6465 7220 3d20 4461  trainloader = Da
-00002030: 7461 4c6f 6164 6572 280d 0a20 2020 2020  taLoader(..     
-00002040: 2020 2020 2020 2064 6174 6170 6970 653d         datapipe=
-00002050: 7365 6c66 2e74 7261 696e 7069 7065 2c20  self.trainpipe, 
-00002060: 0d0a 2020 2020 2020 2020 2020 2020 6e75  ..            nu
-00002070: 6d5f 776f 726b 6572 733d 7365 6c66 2e63  m_workers=self.c
-00002080: 6667 2e6e 756d 5f77 6f72 6b65 7273 2c0d  fg.num_workers,.
-00002090: 0a20 2020 2020 2020 2020 2020 2070 696e  .            pin
-000020a0: 5f6d 656d 6f72 793d 7365 6c66 2e63 6667  _memory=self.cfg
-000020b0: 2e70 696e 5f6d 656d 6f72 790d 0a20 2020  .pin_memory..   
-000020c0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-000020d0: 7365 6c66 2e76 616c 6964 6c6f 6164 6572  self.validloader
-000020e0: 203d 2044 6174 614c 6f61 6465 7228 0d0a   = DataLoader(..
-000020f0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00002100: 7069 7065 3d73 656c 662e 7661 6c69 6470  pipe=self.validp
-00002110: 6970 652c 200d 0a20 2020 2020 2020 2020  ipe, ..         
-00002120: 2020 206e 756d 5f77 6f72 6b65 7273 3d73     num_workers=s
-00002130: 656c 662e 6366 672e 6e75 6d5f 776f 726b  elf.cfg.num_work
-00002140: 6572 732c 0d0a 2020 2020 2020 2020 2020  ers,..          
-00002150: 2020 7069 6e5f 6d65 6d6f 7279 3d73 656c    pin_memory=sel
-00002160: 662e 6366 672e 7069 6e5f 6d65 6d6f 7279  f.cfg.pin_memory
-00002170: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
-00002180: 2020 2020 2073 656c 662e 7465 7374 6c6f       self.testlo
-00002190: 6164 6572 203d 2044 6174 614c 6f61 6465  ader = DataLoade
-000021a0: 7228 0d0a 2020 2020 2020 2020 2020 2020  r(..            
-000021b0: 6461 7461 7069 7065 3d73 656c 662e 7465  datapipe=self.te
-000021c0: 7374 7069 7065 2c20 0d0a 2020 2020 2020  stpipe, ..      
-000021d0: 2020 2020 2020 6e75 6d5f 776f 726b 6572        num_worker
-000021e0: 733d 7365 6c66 2e63 6667 2e6e 756d 5f77  s=self.cfg.num_w
-000021f0: 6f72 6b65 7273 2c0d 0a20 2020 2020 2020  orkers,..       
-00002200: 2020 2020 2070 696e 5f6d 656d 6f72 793d       pin_memory=
-00002210: 7365 6c66 2e63 6667 2e70 696e 5f6d 656d  self.cfg.pin_mem
-00002220: 6f72 790d 0a20 2020 2020 2020 2029 0d0a  ory..        )..
-00002230: 2020 2020 0d0a 2020 2020 4070 726f 7065      ..    @prope
-00002240: 7274 790d 0a20 2020 2064 6566 2064 6174  rty..    def dat
-00002250: 616c 6f61 6465 7228 7365 6c66 293a 0d0a  aloader(self):..
-00002260: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
-00002270: 6e20 7468 6520 636f 7272 6573 706f 6e64  n the correspond
-00002280: 696e 6720 6461 7461 206c 6f61 6465 7220  ing data loader 
-00002290: 6465 7065 6e64 696e 6720 6f6e 2074 6865  depending on the
-000022a0: 2063 7572 7265 6e74 206d 6f64 652e 2222   current mode.""
-000022b0: 220d 0a20 2020 2020 2020 2069 6620 7365  "..        if se
-000022c0: 6c66 2e6d 6f64 6520 3d3d 2027 7472 6169  lf.mode == 'trai
-000022d0: 6e27 3a0d 0a20 2020 2020 2020 2020 2020  n':..           
-000022e0: 2072 6574 7572 6e20 7365 6c66 2e74 7261   return self.tra
-000022f0: 696e 6c6f 6164 6572 0d0a 2020 2020 2020  inloader..      
-00002300: 2020 656c 6966 2073 656c 662e 6d6f 6465    elif self.mode
-00002310: 203d 3d20 2776 616c 6964 273a 0d0a 2020   == 'valid':..  
-00002320: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00002330: 2073 656c 662e 7661 6c69 646c 6f61 6465   self.validloade
-00002340: 720d 0a20 2020 2020 2020 2065 6c73 653a  r..        else:
-00002350: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00002360: 7475 726e 2073 656c 662e 7465 7374 6c6f  turn self.testlo
-00002370: 6164 6572 0d0a 0d0a 2020 2020 4070 726f  ader....    @pro
-00002380: 7065 7274 790d 0a20 2020 2064 6566 206d  perty..    def m
-00002390: 6f6e 6974 6f72 7328 7365 6c66 2920 2d3e  onitors(self) ->
-000023a0: 204d 6f6e 6974 6f72 3a0d 0a20 2020 2020   Monitor:..     
-000023b0: 2020 2022 2222 5265 7475 726e 2074 6865     """Return the
-000023c0: 206d 6f6e 6974 6f72 2064 6963 7469 6f6e   monitor diction
-000023d0: 6172 7920 666f 7220 7468 6520 6469 6666  ary for the diff
-000023e0: 6572 656e 7420 6d6f 6465 7320 2827 7472  erent modes ('tr
-000023f0: 6169 6e27 2c20 2776 616c 6964 272c 2027  ain', 'valid', '
-00002400: 7465 7374 2729 2e22 2222 0d0a 2020 2020  test')."""..    
-00002410: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00002420: 5f5f 6d6f 6e69 746f 7273 0d0a 0d0a 2020  __monitors....  
-00002430: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
-00002440: 2064 6566 206d 6574 6572 3462 6573 7428   def meter4best(
-00002450: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00002460: 7265 7475 726e 2073 656c 662e 5f5f 6265  return self.__be
-00002470: 7374 5f6d 6574 6572 0d0a 0d0a 2020 2020  st_meter....    
-00002480: 406d 6574 6572 3462 6573 742e 7365 7474  @meter4best.sett
-00002490: 6572 0d0a 2020 2020 6465 6620 6d65 7465  er..    def mete
-000024a0: 7234 6265 7374 2873 656c 662c 206d 6574  r4best(self, met
-000024b0: 6572 3a20 4176 6572 6167 654d 6574 6572  er: AverageMeter
-000024c0: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
-000024d0: 2e5f 5f62 6573 745f 6d65 7465 7220 3d20  .__best_meter = 
-000024e0: 6d65 7465 720d 0a20 2020 2020 2020 2069  meter..        i
-000024f0: 6e66 6f4c 6f67 6765 7228 6622 5b43 6f61  nfoLogger(f"[Coa
-00002500: 6368 5d20 3e3e 3e20 5365 7420 6265 7374  ch] >>> Set best
-00002510: 206d 6574 6572 3a20 7b6d 6574 6572 2e6e   meter: {meter.n
-00002520: 616d 657d 2022 290d 0a0d 0a20 2020 2040  ame} ")....    @
-00002530: 7469 6d65 6d65 7465 7228 2243 6f61 6368  timemeter("Coach
-00002540: 2f63 6f6d 7069 6c65 2229 0d0a 2020 2020  /compile")..    
-00002550: 6465 6620 636f 6d70 696c 6528 0d0a 2020  def compile(..  
-00002560: 2020 2020 2020 7365 6c66 2c20 6366 673a        self, cfg:
-00002570: 2043 6f6e 6669 672c 206d 6f6e 6974 6f72   Config, monitor
-00002580: 733a 204c 6973 745b 7374 725d 2c20 0d0a  s: List[str], ..
-00002590: 2020 2020 2020 2020 7768 6963 6834 6265          which4be
-000025a0: 7374 3a20 7374 7220 3d20 274c 4f53 5327  st: str = 'LOSS'
-000025b0: 0d0a 2020 2020 293a 0d0a 2020 2020 2020  ..    ):..      
-000025c0: 2020 7222 2222 0d0a 2020 2020 2020 2020    r"""..        
-000025d0: 4c6f 6164 2074 6865 2063 6f6e 6669 6775  Load the configu
-000025e0: 7261 7469 6f6e 2061 6e64 2073 6574 2075  ration and set u
-000025f0: 7020 6d6f 6e69 746f 7273 2066 6f72 2074  p monitors for t
-00002600: 7261 696e 696e 672e 0d0a 0d0a 2020 2020  raining.....    
-00002610: 2020 2020 5061 7261 6d65 7465 7273 0d0a      Parameters..
-00002620: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00002630: 2d2d 0d0a 2020 2020 2020 2020 6366 6720  --..        cfg 
-00002640: 3a20 436f 6e66 6967 0d0a 2020 2020 2020  : Config..      
-00002650: 2020 2020 2020 4120 636f 6e66 6967 7572        A configur
-00002660: 6174 696f 6e20 6f62 6a65 6374 2077 6974  ation object wit
-00002670: 6820 7468 6520 7472 6169 6e69 6e67 2064  h the training d
-00002680: 6574 6169 6c73 2e0d 0a20 2020 2020 2020  etails...       
-00002690: 206d 6f6e 6974 6f72 7320 3a20 4c69 7374   monitors : List
-000026a0: 5b73 7472 5d0d 0a20 2020 2020 2020 2020  [str]..         
-000026b0: 2020 2041 206c 6973 7420 6f66 206d 6574     A list of met
-000026c0: 7269 6320 6e61 6d65 7320 746f 2062 6520  ric names to be 
-000026d0: 6d6f 6e69 746f 7265 6420 6475 7269 6e67  monitored during
-000026e0: 2074 7261 696e 696e 672e 0d0a 2020 2020   training...    
-000026f0: 2020 2020 7768 6963 6834 6265 7374 203a      which4best :
-00002700: 2073 7472 2c20 6465 6661 756c 7473 2060   str, defaults `
-00002710: 4c4f 5353 270d 0a20 2020 2020 2020 2020  LOSS'..         
-00002720: 2020 2054 6865 206d 6574 7269 6320 7573     The metric us
-00002730: 6564 2066 6f72 2073 656c 6563 7469 6e67  ed for selecting
-00002740: 2074 6865 2062 6573 7420 6368 6563 6b70   the best checkp
-00002750: 6f69 6e74 2e0d 0a0d 0a20 2020 2020 2020  oint.....       
-00002760: 2045 7861 6d70 6c65 730d 0a20 2020 2020   Examples..     
-00002770: 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20 2020     --------..   
-00002780: 2020 2020 203e 3e3e 2063 6f61 6368 3a20       >>> coach: 
-00002790: 436f 6163 680d 0a20 2020 2020 2020 203e  Coach..        >
-000027a0: 3e3e 2063 6f61 6368 2e63 6f6d 7069 6c65  >> coach.compile
-000027b0: 2863 6667 2c20 6d6f 6e69 746f 7273 3d5b  (cfg, monitors=[
-000027c0: 276c 6f73 7327 2c20 2772 6563 616c 6c40  'loss', 'recall@
-000027d0: 3130 272c 2027 7265 6361 6c6c 4032 3027  10', 'recall@20'
-000027e0: 2c20 276e 6463 6740 3130 272c 2027 6e64  , 'ndcg@10', 'nd
-000027f0: 6367 4032 3027 5d29 0d0a 2020 2020 2020  cg@20'])..      
-00002800: 2020 2222 220d 0a20 2020 2020 2020 2073    """..        s
-00002810: 656c 662e 6366 6720 3d20 6366 670d 0a20  elf.cfg = cfg.. 
-00002820: 2020 2020 2020 2023 206d 6574 6572 7320         # meters 
-00002830: 666f 7220 7472 6169 6e7c 7661 6c69 647c  for train|valid|
-00002840: 7465 7374 0d0a 2020 2020 2020 2020 7365  test..        se
-00002850: 6c66 2e5f 5f6d 6f6e 6974 6f72 7320 3d20  lf.__monitors = 
-00002860: 4d6f 6e69 746f 7228 290d 0a20 2020 2020  Monitor()..     
-00002870: 2020 2073 656c 662e 5f5f 6d6f 6e69 746f     self.__monito
-00002880: 7273 5b27 7472 6169 6e27 5d20 3d20 6465  rs['train'] = de
-00002890: 6661 756c 7464 6963 7428 6c69 7374 290d  faultdict(list).
-000028a0: 0a20 2020 2020 2020 2073 656c 662e 5f5f  .        self.__
-000028b0: 6d6f 6e69 746f 7273 5b27 7661 6c69 6427  monitors['valid'
-000028c0: 5d20 3d20 6465 6661 756c 7464 6963 7428  ] = defaultdict(
-000028d0: 6c69 7374 290d 0a20 2020 2020 2020 2073  list)..        s
-000028e0: 656c 662e 5f5f 6d6f 6e69 746f 7273 5b27  elf.__monitors['
-000028f0: 7465 7374 275d 203d 2064 6566 6175 6c74  test'] = default
-00002900: 6469 6374 286c 6973 7429 0d0a 0d0a 2020  dict(list)....  
-00002910: 2020 2020 2020 6465 6620 7365 745f 6d6f        def set_mo
-00002920: 6e69 746f 7228 0d0a 2020 2020 2020 2020  nitor(..        
-00002930: 2020 2020 6e61 6d65 3a20 7374 722c 206c      name: str, l
-00002940: 6173 746e 616d 653a 2073 7472 2c20 7072  astname: str, pr
-00002950: 6566 6978 3a20 7374 7220 3d20 2774 7261  efix: str = 'tra
-00002960: 696e 272c 202a 2a6b 7761 7267 730d 0a20  in', **kwargs.. 
-00002970: 2020 2020 2020 2029 3a0d 0a20 2020 2020         ):..     
-00002980: 2020 2020 2020 2022 2222 4164 6420 6120         """Add a 
-00002990: 6d6f 6e69 746f 7220 666f 7220 7468 6520  monitor for the 
-000029a0: 7370 6563 6966 6965 6420 6d65 7472 6963  specified metric
-000029b0: 2e22 2222 0d0a 2020 2020 2020 2020 2020  ."""..          
-000029c0: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-000029d0: 2020 2020 2020 2020 6d65 7465 7220 3d20          meter = 
-000029e0: 4176 6572 6167 654d 6574 6572 280d 0a20  AverageMeter(.. 
-000029f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a00: 2020 2020 2020 206e 616d 653d 6e61 6d65         name=name
-00002a10: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00002a20: 2020 2020 2020 2020 2020 206d 6574 7269             metri
-00002a30: 633d 7061 7274 6961 6c28 4445 4641 554c  c=partial(DEFAUL
-00002a40: 545f 4d45 5452 4943 535b 6c61 7374 6e61  T_METRICS[lastna
-00002a50: 6d65 5d2c 202a 2a6b 7761 7267 7329 2c0d  me], **kwargs),.
-00002a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a70: 2020 2020 2020 2020 2066 6d74 3d44 4546           fmt=DEF
-00002a80: 4155 4c54 5f46 4d54 535b 6c61 7374 6e61  AULT_FMTS[lastna
-00002a90: 6d65 5d2c 0d0a 2020 2020 2020 2020 2020  me],..          
-00002aa0: 2020 2020 2020 2020 2020 2020 2020 6265                be
-00002ab0: 7374 5f63 6173 7465 723d 4445 4641 554c  st_caster=DEFAUL
-00002ac0: 545f 4245 5354 5f43 4153 5445 525b 6c61  T_BEST_CASTER[la
-00002ad0: 7374 6e61 6d65 5d0d 0a20 2020 2020 2020  stname]..       
-00002ae0: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-00002af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b00: 7365 6c66 2e5f 5f6d 6f6e 6974 6f72 735b  self.__monitors[
-00002b10: 7072 6566 6978 5d5b 6c61 7374 6e61 6d65  prefix][lastname
-00002b20: 5d2e 6170 7065 6e64 286d 6574 6572 290d  ].append(meter).
-00002b30: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-00002b40: 6570 7420 4b65 7945 7272 6f72 3a0d 0a20  ept KeyError:.. 
-00002b50: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00002b60: 6169 7365 204b 6579 4572 726f 7228 0d0a  aise KeyError(..
-00002b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b80: 2020 2020 6622 5468 6520 6d65 7472 6963      f"The metric
-00002b90: 206f 6620 7b6c 6173 746e 616d 657d 2069   of {lastname} i
-00002ba0: 7320 6e6f 7420 696e 636c 7564 6564 2e20  s not included. 
-00002bb0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-00002bc0: 2020 2020 2020 2066 2259 6f75 2063 616e         f"You can
-00002bd0: 2072 6567 6973 7465 7220 6279 2063 616c   register by cal
-00002be0: 6c69 6e67 2060 7265 6769 7374 6572 5f6d  ling `register_m
-00002bf0: 6574 7269 6328 2e2e 2e29 2720 2e2e 2e22  etric(...)' ..."
-00002c00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002c10: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
-00002c20: 2072 6574 7572 6e20 6d65 7465 720d 0a0d   return meter...
-00002c30: 0a20 2020 2020 2020 2023 2055 5050 4552  .        # UPPER
-00002c40: 0d0a 2020 2020 2020 2020 7768 6963 6834  ..        which4
-00002c50: 6265 7374 203d 2077 6869 6368 3462 6573  best = which4bes
-00002c60: 742e 7570 7065 7228 290d 0a20 2020 2020  t.upper()..     
-00002c70: 2020 206d 6f6e 6974 6f72 7320 3d20 5b27     monitors = ['
-00002c80: 4c4f 5353 275d 202b 205b 6e61 6d65 2e75  LOSS'] + [name.u
-00002c90: 7070 6572 2829 2066 6f72 206e 616d 6520  pper() for name 
-00002ca0: 696e 206d 6f6e 6974 6f72 735d 202b 205b  in monitors] + [
-00002cb0: 7768 6963 6834 6265 7374 5d0d 0a20 2020  which4best]..   
-00002cc0: 2020 2020 206d 6f6e 6974 6f72 7320 3d20       monitors = 
-00002cd0: 736f 7274 6564 2873 6574 286d 6f6e 6974  sorted(set(monit
-00002ce0: 6f72 7329 2c20 6b65 793d 6d6f 6e69 746f  ors), key=monito
-00002cf0: 7273 2e69 6e64 6578 290d 0a0d 0a20 2020  rs.index)....   
-00002d00: 2020 2020 2066 6f72 206e 616d 6520 696e       for name in
-00002d10: 206d 6f6e 6974 6f72 733a 0d0a 2020 2020   monitors:..    
-00002d20: 2020 2020 2020 2020 666f 7220 7072 6566          for pref
-00002d30: 6978 2069 6e20 2827 7472 6169 6e27 2c20  ix in ('train', 
-00002d40: 2776 616c 6964 272c 2027 7465 7374 2729  'valid', 'test')
-00002d50: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00002d60: 2020 2069 6620 2740 2720 696e 206e 616d     if '@' in nam
-00002d70: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00002d80: 2020 2020 2020 2020 6c61 7374 6e61 6d65          lastname
-00002d90: 2c20 4b20 3d20 6e61 6d65 2e73 706c 6974  , K = name.split
-00002da0: 2827 4027 290d 0a20 2020 2020 2020 2020  ('@')..         
-00002db0: 2020 2020 2020 2020 2020 206d 6574 6572             meter
-00002dc0: 203d 2073 6574 5f6d 6f6e 6974 6f72 280d   = set_monitor(.
-00002dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002de0: 2020 2020 2020 2020 206e 616d 653d 6e61           name=na
-00002df0: 6d65 2c0d 0a20 2020 2020 2020 2020 2020  me,..           
-00002e00: 2020 2020 2020 2020 2020 2020 206c 6173               las
-00002e10: 746e 616d 653d 6c61 7374 6e61 6d65 2c0d  tname=lastname,.
-00002e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002e30: 2020 2020 2020 2020 2070 7265 6669 783d           prefix=
-00002e40: 7072 6566 6978 2c0d 0a20 2020 2020 2020  prefix,..       
-00002e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e60: 206b 3d69 6e74 284b 290d 0a20 2020 2020   k=int(K)..     
-00002e70: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00002e80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002e90: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00002ea0: 2020 2020 2020 2020 2020 2020 206c 6173               las
-00002eb0: 746e 616d 6520 3d20 6e61 6d65 0d0a 2020  tname = name..  
-00002ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ed0: 2020 6d65 7465 7220 3d20 7365 745f 6d6f    meter = set_mo
-00002ee0: 6e69 746f 7228 0d0a 2020 2020 2020 2020  nitor(..        
-00002ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f00: 6e61 6d65 3d6e 616d 652c 0d0a 2020 2020  name=name,..    
-00002f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f20: 2020 2020 6c61 7374 6e61 6d65 3d6c 6173      lastname=las
-00002f30: 746e 616d 652c 0d0a 2020 2020 2020 2020  tname,..        
-00002f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f50: 7072 6566 6978 3d70 7265 6669 780d 0a20  prefix=prefix.. 
-00002f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f70: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
-00002f80: 2020 2020 2020 6966 2070 7265 6669 7820        if prefix 
-00002f90: 3d3d 2027 7661 6c69 6427 2061 6e64 206e  == 'valid' and n
-00002fa0: 616d 6520 3d3d 2077 6869 6368 3462 6573  ame == which4bes
-00002fb0: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
-00002fc0: 2020 2020 2020 2020 7365 6c66 2e6d 6574          self.met
-00002fd0: 6572 3462 6573 7420 3d20 6d65 7465 720d  er4best = meter.
-00002fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002ff0: 2020 2020 2073 656c 662e 5f62 6573 7420       self._best 
-00003000: 3d20 2d66 6c6f 6174 2827 696e 6627 2920  = -float('inf') 
-00003010: 6966 206d 6574 6572 2e63 6173 7465 7220  if meter.caster 
-00003020: 6973 206d 6178 2065 6c73 6520 666c 6f61  is max else floa
-00003030: 7428 2769 6e66 2729 0d0a 2020 2020 2020  t('inf')..      
-00003040: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00003050: 6c66 2e5f 6265 7374 5f65 706f 6368 203d  lf._best_epoch =
-00003060: 2030 0d0a 0d0a 2020 2020 2020 2020 2320   0....        # 
-00003070: 5072 6570 6172 6520 6461 7461 206c 6f61  Prepare data loa
-00003080: 6465 7273 0d0a 2020 2020 2020 2020 7365  ders..        se
-00003090: 6c66 2e70 7265 7061 7265 5f64 6174 616c  lf.prepare_datal
-000030a0: 6f61 6465 7228 290d 0a0d 0a20 2020 2064  oader()....    d
-000030b0: 6566 2073 6176 6528 7365 6c66 2920 2d3e  ef save(self) ->
-000030c0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-000030d0: 2222 2253 6176 6520 7468 6520 6d6f 6465  """Save the mode
-000030e0: 6c22 2222 0d0a 2020 2020 2020 2020 746f  l"""..        to
-000030f0: 7263 682e 7361 7665 2873 656c 662e 6d6f  rch.save(self.mo
-00003100: 6465 6c2e 7374 6174 655f 6469 6374 2829  del.state_dict()
-00003110: 2c20 6f73 2e70 6174 682e 6a6f 696e 2873  , os.path.join(s
-00003120: 656c 662e 6366 672e 4c4f 475f 5041 5448  elf.cfg.LOG_PATH
-00003130: 2c20 7365 6c66 2e63 6667 2e53 4156 4544  , self.cfg.SAVED
-00003140: 5f46 494c 454e 414d 4529 290d 0a0d 0a20  _FILENAME)).... 
-00003150: 2020 2064 6566 206c 6f61 6428 7365 6c66     def load(self
-00003160: 2c20 7061 7468 3a20 7374 722c 2066 696c  , path: str, fil
-00003170: 656e 616d 653a 204f 7074 696f 6e61 6c5b  ename: Optional[
-00003180: 7374 725d 203d 204e 6f6e 652c 202a 2a6b  str] = None, **k
-00003190: 7761 7267 7329 202d 3e20 4e6f 6e65 3a0d  wargs) -> None:.
-000031a0: 0a20 2020 2020 2020 2066 696c 656e 616d  .        filenam
-000031b0: 6520 3d20 7365 6c66 2e63 6667 2e53 4156  e = self.cfg.SAV
-000031c0: 4544 5f46 494c 454e 414d 4520 6966 2066  ED_FILENAME if f
-000031d0: 696c 656e 616d 6520 6973 204e 6f6e 6520  ilename is None 
-000031e0: 656c 7365 2066 696c 656e 616d 650d 0a20  else filename.. 
-000031f0: 2020 2020 2020 2073 656c 662e 6d6f 6465         self.mode
-00003200: 6c2e 6c6f 6164 5f73 7461 7465 5f64 6963  l.load_state_dic
-00003210: 7428 746f 7263 682e 6c6f 6164 286f 732e  t(torch.load(os.
-00003220: 7061 7468 2e6a 6f69 6e28 7061 7468 2c20  path.join(path, 
-00003230: 6669 6c65 6e61 6d65 292c 202a 2a6b 7761  filename), **kwa
-00003240: 7267 7329 290d 0a0d 0a20 2020 2064 6566  rgs))....    def
-00003250: 2073 6176 655f 6368 6563 6b70 6f69 6e74   save_checkpoint
-00003260: 2873 656c 662c 2065 706f 6368 3a20 696e  (self, epoch: in
-00003270: 7429 202d 3e20 4e6f 6e65 3a0d 0a20 2020  t) -> None:..   
-00003280: 2020 2020 2072 2222 220d 0a20 2020 2020       r"""..     
-00003290: 2020 2053 6176 6520 6375 7272 656e 7420     Save current 
-000032a0: 6368 6563 6b70 6f69 6e74 2061 7420 6570  checkpoint at ep
-000032b0: 6f63 682e 0d0a 0d0a 2020 2020 2020 2020  och.....        
-000032c0: 5061 7261 6d65 7465 7273 3a0d 0a20 2020  Parameters:..   
-000032d0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d       -----------
-000032e0: 0d0a 2020 2020 2020 2020 2020 2020 6570  ..            ep
-000032f0: 6f63 6820 3a69 6e74 2043 7572 7265 6e74  och :int Current
-00003300: 2065 706f 6368 206e 756d 6265 722e 0d0a   epoch number...
-00003310: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00003320: 733a 0d0a 2020 2020 2020 2020 2d2d 2d2d  s:..        ----
-00003330: 2d2d 2d2d 0d0a 2020 2020 2020 2020 2020  ----..          
-00003340: 2020 4e6f 6e65 0d0a 2020 2020 2020 2020    None..        
-00003350: 2222 220d 0a20 2020 2020 2020 2070 6174  """..        pat
-00003360: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
-00003370: 2873 656c 662e 6366 672e 4348 4543 4b50  (self.cfg.CHECKP
-00003380: 4f49 4e54 5f50 4154 482c 2073 656c 662e  OINT_PATH, self.
-00003390: 6366 672e 4348 4543 4b50 4f49 4e54 5f46  cfg.CHECKPOINT_F
-000033a0: 494c 454e 414d 4529 0d0a 2020 2020 2020  ILENAME)..      
-000033b0: 2020 6368 6563 6b70 6f69 6e74 203d 2064    checkpoint = d
-000033c0: 6963 7428 290d 0a20 2020 2020 2020 2063  ict()..        c
-000033d0: 6865 636b 706f 696e 745b 2765 706f 6368  heckpoint['epoch
-000033e0: 275d 203d 2065 706f 6368 0d0a 2020 2020  '] = epoch..    
-000033f0: 2020 2020 666f 7220 6d6f 6475 6c65 2069      for module i
-00003400: 6e20 7365 6c66 2e63 6667 2e43 4845 434b  n self.cfg.CHECK
-00003410: 504f 494e 545f 4d4f 4455 4c45 533a 0d0a  POINT_MODULES:..
-00003420: 2020 2020 2020 2020 2020 2020 6368 6563              chec
-00003430: 6b70 6f69 6e74 5b6d 6f64 756c 655d 203d  kpoint[module] =
-00003440: 2067 6574 6174 7472 2873 656c 662c 206d   getattr(self, m
-00003450: 6f64 756c 6529 2e73 7461 7465 5f64 6963  odule).state_dic
-00003460: 7428 290d 0a20 2020 2020 2020 2063 6865  t()..        che
-00003470: 636b 706f 696e 745b 276d 6f6e 6974 6f72  ckpoint['monitor
-00003480: 7327 5d20 3d20 7365 6c66 2e6d 6f6e 6974  s'] = self.monit
-00003490: 6f72 732e 7374 6174 655f 6469 6374 2829  ors.state_dict()
-000034a0: 0d0a 2020 2020 2020 2020 746f 7263 682e  ..        torch.
-000034b0: 7361 7665 2863 6865 636b 706f 696e 742c  save(checkpoint,
-000034c0: 2070 6174 6829 0d0a 0d0a 2020 2020 6465   path)....    de
-000034d0: 6620 6c6f 6164 5f63 6865 636b 706f 696e  f load_checkpoin
-000034e0: 7428 7365 6c66 2920 2d3e 2069 6e74 3a0d  t(self) -> int:.
-000034f0: 0a20 2020 2020 2020 2072 2222 220d 0a20  .        r""".. 
-00003500: 2020 2020 2020 204c 6f61 6420 6c61 7374         Load last
-00003510: 2073 6176 6564 2063 6865 636b 706f 696e   saved checkpoin
-00003520: 742e 0d0a 0d0a 2020 2020 2020 2020 5265  t.....        Re
-00003530: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
-00003540: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
-00003550: 2020 6570 6f63 683a 2069 6e74 200d 0a20    epoch: int .. 
-00003560: 2020 2020 2020 2020 2020 2054 6865 2065             The e
-00003570: 706f 6368 206e 756d 6265 7220 6c6f 6164  poch number load
-00003580: 6564 2066 726f 6d20 7468 6520 6368 6563  ed from the chec
-00003590: 6b70 6f69 6e74 2e0d 0a20 2020 2020 2020  kpoint...       
-000035a0: 2022 2222 0d0a 2020 2020 2020 2020 7061   """..        pa
-000035b0: 7468 203d 206f 732e 7061 7468 2e6a 6f69  th = os.path.joi
-000035c0: 6e28 7365 6c66 2e63 6667 2e43 4845 434b  n(self.cfg.CHECK
-000035d0: 504f 494e 545f 5041 5448 2c20 7365 6c66  POINT_PATH, self
-000035e0: 2e63 6667 2e43 4845 434b 504f 494e 545f  .cfg.CHECKPOINT_
-000035f0: 4649 4c45 4e41 4d45 290d 0a20 2020 2020  FILENAME)..     
-00003600: 2020 2063 6865 636b 706f 696e 7420 3d20     checkpoint = 
-00003610: 746f 7263 682e 6c6f 6164 2870 6174 6829  torch.load(path)
-00003620: 0d0a 2020 2020 2020 2020 666f 7220 6d6f  ..        for mo
-00003630: 6475 6c65 2069 6e20 7365 6c66 2e63 6667  dule in self.cfg
-00003640: 2e43 4845 434b 504f 494e 545f 4d4f 4455  .CHECKPOINT_MODU
-00003650: 4c45 533a 0d0a 2020 2020 2020 2020 2020  LES:..          
-00003660: 2020 6765 7461 7474 7228 7365 6c66 2c20    getattr(self, 
-00003670: 6d6f 6475 6c65 292e 6c6f 6164 5f73 7461  module).load_sta
-00003680: 7465 5f64 6963 7428 6368 6563 6b70 6f69  te_dict(checkpoi
-00003690: 6e74 5b6d 6f64 756c 655d 290d 0a20 2020  nt[module])..   
-000036a0: 2020 2020 2073 656c 662e 6d6f 6e69 746f       self.monito
-000036b0: 7273 2e6c 6f61 645f 7374 6174 655f 6469  rs.load_state_di
-000036c0: 6374 2863 6865 636b 706f 696e 745b 276d  ct(checkpoint['m
-000036d0: 6f6e 6974 6f72 7327 5d29 0d0a 2020 2020  onitors'])..    
-000036e0: 2020 2020 7265 7475 726e 2063 6865 636b      return check
-000036f0: 706f 696e 745b 2765 706f 6368 275d 0d0a  point['epoch']..
-00003700: 0d0a 2020 2020 6465 6620 7361 7665 5f62  ..    def save_b
-00003710: 6573 7428 7365 6c66 2920 2d3e 204e 6f6e  est(self) -> Non
-00003720: 653a 0d0a 2020 2020 2020 2020 746f 7263  e:..        torc
-00003730: 682e 7361 7665 2873 656c 662e 6d6f 6465  h.save(self.mode
-00003740: 6c2e 7374 6174 655f 6469 6374 2829 2c20  l.state_dict(), 
-00003750: 6f73 2e70 6174 682e 6a6f 696e 2873 656c  os.path.join(sel
-00003760: 662e 6366 672e 4c4f 475f 5041 5448 2c20  f.cfg.LOG_PATH, 
-00003770: 7365 6c66 2e63 6667 2e42 4553 545f 4649  self.cfg.BEST_FI
-00003780: 4c45 4e41 4d45 2929 0d0a 0d0a 2020 2020  LENAME))....    
-00003790: 6465 6620 6c6f 6164 5f62 6573 7428 7365  def load_best(se
-000037a0: 6c66 2920 2d3e 204e 6f6e 653a 0d0a 2020  lf) -> None:..  
-000037b0: 2020 2020 2020 696e 666f 4c6f 6767 6572        infoLogger
-000037c0: 2866 225b 436f 6163 685d 203e 3e3e 204c  (f"[Coach] >>> L
-000037d0: 6f61 6420 6265 7374 206d 6f64 656c 2040  oad best model @
-000037e0: 4570 6f63 6820 7b73 656c 662e 5f62 6573  Epoch {self._bes
-000037f0: 745f 6570 6f63 683a 3c34 647d 2022 290d  t_epoch:<4d} ").
-00003800: 0a20 2020 2020 2020 2073 656c 662e 6d6f  .        self.mo
-00003810: 6465 6c2e 6c6f 6164 5f73 7461 7465 5f64  del.load_state_d
-00003820: 6963 7428 746f 7263 682e 6c6f 6164 286f  ict(torch.load(o
-00003830: 732e 7061 7468 2e6a 6f69 6e28 7365 6c66  s.path.join(self
-00003840: 2e63 6667 2e4c 4f47 5f50 4154 482c 2073  .cfg.LOG_PATH, s
-00003850: 656c 662e 6366 672e 4245 5354 5f46 494c  elf.cfg.BEST_FIL
-00003860: 454e 414d 4529 2929 0d0a 0d0a 2020 2020  ENAME)))....    
-00003870: 6465 6620 6368 6563 6b5f 6265 7374 2873  def check_best(s
-00003880: 656c 662c 2065 706f 6368 3a20 696e 7429  elf, epoch: int)
-00003890: 202d 3e20 4e6f 6e65 3a0d 0a20 2020 2020   -> None:..     
-000038a0: 2020 2022 2222 5570 6461 7465 2062 6573     """Update bes
-000038b0: 7420 7661 6c75 652e 2222 220d 0a20 2020  t value."""..   
-000038c0: 2020 2020 2069 6620 7365 6c66 2e6d 6574       if self.met
-000038d0: 6572 3462 6573 742e 6163 7469 7665 3a0d  er4best.active:.
-000038e0: 0a20 2020 2020 2020 2020 2020 2062 6573  .            bes
-000038f0: 745f 203d 2073 656c 662e 6d65 7465 7234  t_ = self.meter4
-00003900: 6265 7374 2e77 6869 6368 5f69 735f 6265  best.which_is_be
-00003910: 7474 6572 2873 656c 662e 5f62 6573 7429  tter(self._best)
-00003920: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00003930: 2062 6573 745f 2021 3d20 7365 6c66 2e5f   best_ != self._
-00003940: 6265 7374 3a0d 0a20 2020 2020 2020 2020  best:..         
-00003950: 2020 2020 2020 2073 656c 662e 5f62 6573         self._bes
-00003960: 7420 3d20 6265 7374 5f0d 0a20 2020 2020  t = best_..     
-00003970: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003980: 5f62 6573 745f 6570 6f63 6820 3d20 6570  _best_epoch = ep
-00003990: 6f63 680d 0a20 2020 2020 2020 2020 2020  och..           
-000039a0: 2020 2020 2069 6e66 6f4c 6f67 6765 7228       infoLogger(
-000039b0: 6622 5b43 6f61 6368 5d20 3e3e 3e20 4265  f"[Coach] >>> Be
-000039c0: 7474 6572 202a 2a2a 7b73 656c 662e 6d65  tter ***{self.me
-000039d0: 7465 7234 6265 7374 2e6e 616d 657d 2a2a  ter4best.name}**
-000039e0: 2a20 6f66 202a 2a2a 7b73 656c 662e 5f62  * of ***{self._b
-000039f0: 6573 743a 2e34 667d 2a2a 2a20 2229 0d0a  est:.4f}*** ")..
-00003a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a10: 7365 6c66 2e73 6176 655f 6265 7374 2829  self.save_best()
-00003a20: 0d0a 0d0a 2020 2020 6465 6620 6576 616c  ....    def eval
-00003a30: 5f61 745f 6265 7374 2873 656c 6629 3a0d  _at_best(self):.
-00003a40: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
-00003a50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003a60: 6c6f 6164 5f62 6573 7428 290d 0a20 2020  load_best()..   
-00003a70: 2020 2020 2020 2020 2073 656c 662e 7661           self.va
-00003a80: 6c69 6428 290d 0a20 2020 2020 2020 2020  lid()..         
-00003a90: 2020 2073 656c 662e 7465 7374 2829 0d0a     self.test()..
-00003aa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003ab0: 2e73 7465 7028 7365 6c66 2e5f 6265 7374  .step(self._best
-00003ac0: 5f65 706f 6368 290d 0a20 2020 2020 2020  _epoch)..       
-00003ad0: 2020 2020 2073 656c 662e 6c6f 6164 2873       self.load(s
-00003ae0: 656c 662e 6366 672e 4c4f 475f 5041 5448  elf.cfg.LOG_PATH
-00003af0: 2c20 7365 6c66 2e63 6667 2e53 4156 4544  , self.cfg.SAVED
-00003b00: 5f46 494c 454e 414d 4529 0d0a 2020 2020  _FILENAME)..    
-00003b10: 2020 2020 6578 6365 7074 2046 696c 654e      except FileN
-00003b20: 6f74 466f 756e 6445 7272 6f72 3a0d 0a20  otFoundError:.. 
-00003b30: 2020 2020 2020 2020 2020 2069 6e66 6f4c             infoL
-00003b40: 6f67 6765 7228 6622 5b43 6f61 6368 5d20  ogger(f"[Coach] 
-00003b50: 3e3e 3e20 4e6f 2062 6573 7420 6d6f 6465  >>> No best mode
-00003b60: 6c20 7761 7320 7265 636f 7264 6564 2e20  l was recorded. 
-00003b70: 536b 6970 2069 7420 2e2e 2e22 290d 0a0d  Skip it ...")...
-00003b80: 0a20 2020 2064 6566 2072 6573 756d 6528  .    def resume(
-00003b90: 7365 6c66 2920 2d3e 2069 6e74 3a0d 0a20  self) -> int:.. 
-00003ba0: 2020 2020 2020 2072 2222 220d 0a20 2020         r"""..   
-00003bb0: 2020 2020 2052 6573 756d 6520 7472 6169       Resume trai
-00003bc0: 6e69 6e67 2066 726f 6d20 7468 6520 6c61  ning from the la
-00003bd0: 7374 2063 6865 636b 706f 696e 742e 0d0a  st checkpoint...
-00003be0: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00003bf0: 733a 0d0a 2020 2020 2020 2020 2d2d 2d2d  s:..        ----
-00003c00: 2d2d 2d2d 0d0a 2020 2020 2020 2020 7374  ----..        st
-00003c10: 6172 745f 6570 6f63 683a 2069 6e74 0d0a  art_epoch: int..
-00003c20: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00003c30: 6570 6f63 6820 6e75 6d62 6572 2074 6f20  epoch number to 
-00003c40: 7265 7375 6d65 2074 7261 696e 696e 6720  resume training 
-00003c50: 6672 6f6d 2e0d 0a20 2020 2020 2020 2022  from...        "
-00003c60: 2222 0d0a 2020 2020 2020 2020 7374 6172  ""..        star
-00003c70: 745f 6570 6f63 683a 2069 6e74 203d 2030  t_epoch: int = 0
-00003c80: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-00003c90: 662e 6366 672e 7265 7375 6d65 3a0d 0a20  f.cfg.resume:.. 
-00003ca0: 2020 2020 2020 2020 2020 2073 7461 7274             start
-00003cb0: 5f65 706f 6368 203d 2073 656c 662e 6c6f  _epoch = self.lo
-00003cc0: 6164 5f63 6865 636b 706f 696e 7428 290d  ad_checkpoint().
-00003cd0: 0a20 2020 2020 2020 2020 2020 2069 6e66  .            inf
-00003ce0: 6f4c 6f67 6765 7228 6622 5b43 6f61 6368  oLogger(f"[Coach
-00003cf0: 5d20 3e3e 3e20 4c6f 6164 206c 6173 7420  ] >>> Load last 
-00003d00: 6368 6563 6b70 6f69 6e74 2061 6e64 2074  checkpoint and t
-00003d10: 7261 696e 2066 726f 6d20 6570 6f63 683a  rain from epoch:
-00003d20: 207b 7374 6172 745f 6570 6f63 687d 2229   {start_epoch}")
-00003d30: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00003d40: 2073 7461 7274 5f65 706f 6368 0d0a 0d0a   start_epoch....
-00003d50: 2020 2020 4074 6f72 6368 2e6e 6f5f 6772      @torch.no_gr
-00003d60: 6164 2829 0d0a 2020 2020 6465 6620 6d6f  ad()..    def mo
-00003d70: 6e69 746f 7228 0d0a 2020 2020 2020 2020  nitor(..        
-00003d80: 7365 6c66 2c20 2a76 616c 7565 732c 0d0a  self, *values,..
-00003d90: 2020 2020 2020 2020 6e3a 2069 6e74 203d          n: int =
-00003da0: 2031 2c20 6d6f 6465 3a20 7374 7220 3d20   1, mode: str = 
-00003db0: 276d 6561 6e27 2c20 0d0a 2020 2020 2020  'mean', ..      
-00003dc0: 2020 7072 6566 6978 3a20 7374 7220 3d20    prefix: str = 
-00003dd0: 2774 7261 696e 272c 2070 6f6f 6c3a 204f  'train', pool: O
-00003de0: 7074 696f 6e61 6c5b 4974 6572 6162 6c65  ptional[Iterable
-00003df0: 5d20 3d20 4e6f 6e65 0d0a 2020 2020 293a  ] = None..    ):
-00003e00: 0d0a 0d0a 2020 2020 2020 2020 7222 2222  ....        r"""
-00003e10: 0d0a 2020 2020 2020 2020 4c6f 6720 6461  ..        Log da
-00003e20: 7461 2076 616c 7565 7320 746f 2073 7065  ta values to spe
-00003e30: 6369 6669 6320 6d6f 6e69 746f 7273 2e0d  cific monitors..
-00003e40: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-00003e50: 6574 6572 733a 0d0a 2020 2020 2020 2020  eters:..        
-00003e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020  -----------..   
-00003e70: 2020 2020 202a 7661 6c75 6573 203a 2064       *values : d
-00003e80: 6174 610d 0a20 2020 2020 2020 2020 2020  ata..           
-00003e90: 2054 6865 2064 6174 6120 7661 6c75 6573   The data values
-00003ea0: 2074 6f20 6265 206c 6f67 6765 642e 0d0a   to be logged...
-00003eb0: 2020 2020 2020 2020 6e20 3a20 696e 740d          n : int.
-00003ec0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-00003ed0: 2062 6174 6368 2073 697a 6520 696e 2067   batch size in g
-00003ee0: 656e 6572 616c 2e0d 0a20 2020 2020 2020  eneral...       
-00003ef0: 206d 6f64 6520 3a20 7374 722c 206f 7074   mode : str, opt
-00003f00: 696f 6e61 6c0d 0a20 2020 2020 2020 2020  ional..         
-00003f10: 2020 2054 6865 206d 6f64 6520 746f 2063     The mode to c
-00003f20: 6f6d 7075 7465 2074 6865 206d 6574 7269  ompute the metri
-00003f30: 632e 2043 616e 2062 6520 2773 756d 2720  c. Can be 'sum' 
-00003f40: 6f72 2027 6d65 616e 2720 2864 6566 6175  or 'mean' (defau
-00003f50: 6c74 292e 0d0a 2020 2020 2020 2020 7072  lt)...        pr
-00003f60: 6566 6978 203a 2073 7472 2c20 6f70 7469  efix : str, opti
-00003f70: 6f6e 616c 0d0a 2020 2020 2020 2020 2020  onal..          
-00003f80: 2020 5468 6520 7072 6566 6978 2073 7472    The prefix str
-00003f90: 696e 6720 696e 6469 6361 7469 6e67 2077  ing indicating w
-00003fa0: 6869 6368 206d 6f64 6520 7468 6520 7661  hich mode the va
-00003fb0: 6c75 6573 2062 656c 6f6e 6720 746f 2e20  lues belong to. 
-00003fc0: 4361 6e20 6265 2027 7472 6169 6e27 2c20  Can be 'train', 
-00003fd0: 2774 6573 7427 206f 7220 2776 616c 6964  'test' or 'valid
-00003fe0: 272e 0d0a 2020 2020 2020 2020 706f 6f6c  '...        pool
-00003ff0: 203a 204c 6973 745b 7374 725d 2c20 6f70   : List[str], op
-00004000: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-00004010: 2020 2020 4120 6c69 7374 206f 6620 6d65      A list of me
-00004020: 7472 6963 206e 616d 6573 2074 6f20 6c6f  tric names to lo
-00004030: 672e 2049 6620 4e6f 6e65 2c20 616c 6c20  g. If None, all 
-00004040: 6d65 7472 6963 7320 696e 2074 6865 2070  metrics in the p
-00004050: 6f6f 6c20 6f66 2060 7072 6566 6978 6020  ool of `prefix` 
-00004060: 7769 6c6c 2062 6520 6c6f 6767 6564 2e0d  will be logged..
-00004070: 0a20 2020 2020 2020 2022 2222 0d0a 0d0a  .        """....
-00004080: 2020 2020 2020 2020 6d65 7472 6963 733a          metrics:
-00004090: 2044 6963 745b 4c69 7374 5d20 3d20 7365   Dict[List] = se
-000040a0: 6c66 2e6d 6f6e 6974 6f72 735b 7072 6566  lf.monitors[pref
-000040b0: 6978 5d0d 0a20 2020 2020 2020 2070 6f6f  ix]..        poo
-000040c0: 6c20 3d20 6d65 7472 6963 7320 6966 2070  l = metrics if p
-000040d0: 6f6f 6c20 6973 204e 6f6e 6520 656c 7365  ool is None else
-000040e0: 2070 6f6f 6c0d 0a20 2020 2020 2020 2066   pool..        f
-000040f0: 6f72 206c 6173 746e 616d 6520 696e 2070  or lastname in p
-00004100: 6f6f 6c3a 0d0a 2020 2020 2020 2020 2020  ool:..          
-00004110: 2020 666f 7220 6d65 7465 7220 696e 206d    for meter in m
-00004120: 6574 7269 6373 2e67 6574 286c 6173 746e  etrics.get(lastn
-00004130: 616d 652e 7570 7065 7228 292c 205b 5d29  ame.upper(), [])
-00004140: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00004150: 2020 206d 6574 6572 282a 7661 6c75 6573     meter(*values
-00004160: 2c20 6e3d 6e2c 206d 6f64 653d 6d6f 6465  , n=n, mode=mode
-00004170: 290d 0a0d 0a20 2020 2064 6566 2073 7465  )....    def ste
-00004180: 7028 7365 6c66 2c20 6570 6f63 683a 2069  p(self, epoch: i
-00004190: 6e74 293a 0d0a 2020 2020 2020 2020 7222  nt):..        r"
-000041a0: 2222 0d0a 2020 2020 2020 2020 5072 696e  ""..        Prin
-000041b0: 7473 2074 7261 696e 696e 6720 7374 6174  ts training stat
-000041c0: 7573 2061 6e64 2065 7661 6c75 6174 696f  us and evaluatio
-000041d0: 6e20 7265 7375 6c74 7320 666f 7220 6561  n results for ea
-000041e0: 6368 2065 706f 6368 2c20 0d0a 2020 2020  ch epoch, ..    
-000041f0: 2020 2020 616e 6420 7265 7365 7473 2074      and resets t
-00004200: 6865 2063 6f72 7265 7370 6f6e 6469 6e67  he corresponding
-00004210: 2060 4176 6572 6167 654d 6574 6572 6020   `AverageMeter` 
-00004220: 696e 7374 616e 6365 732e 0d0a 0d0a 2020  instances.....  
-00004230: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00004240: 3a0d 0a20 2020 2020 2020 202d 2d2d 2d2d  :..        -----
-00004250: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
-00004260: 6570 6f63 6820 3a20 696e 740d 0a20 2020  epoch : int..   
-00004270: 2020 2020 2020 2020 2054 6865 2065 706f           The epo
-00004280: 6368 206e 756d 6265 722e 0d0a 0d0a 2020  ch number.....  
-00004290: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
-000042a0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-000042b0: 0d0a 2020 2020 2020 2020 4e6f 6e65 0d0a  ..        None..
-000042c0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-000042d0: 2020 2020 206d 6574 7269 6373 3a20 4469       metrics: Di
-000042e0: 6374 5b73 7472 2c20 4c69 7374 5b41 7665  ct[str, List[Ave
-000042f0: 7261 6765 4d65 7465 725d 5d0d 0a20 2020  rageMeter]]..   
-00004300: 2020 2020 2066 6f72 2070 7265 6669 782c       for prefix,
-00004310: 206d 6574 7269 6373 2069 6e20 7365 6c66   metrics in self
-00004320: 2e6d 6f6e 6974 6f72 732e 6974 656d 7328  .monitors.items(
-00004330: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00004340: 696e 666f 7320 3d20 5b66 225b 436f 6163  infos = [f"[Coac
-00004350: 685d 203e 3e3e 207b 7072 6566 6978 2e75  h] >>> {prefix.u
-00004360: 7070 6572 2829 3a35 7d20 4045 706f 6368  pper():5} @Epoch
-00004370: 3a20 7b65 706f 6368 3a3c 3464 7d20 3e3e  : {epoch:<4d} >>
-00004380: 3e20 225d 0d0a 2020 2020 2020 2020 2020  > "]..          
-00004390: 2020 666f 7220 6d65 7465 7273 2069 6e20    for meters in 
-000043a0: 6d65 7472 6963 732e 7661 6c75 6573 2829  metrics.values()
-000043b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000043c0: 2020 2069 6e66 6f73 202b 3d20 5b6d 6574     infos += [met
-000043d0: 6572 2e73 7465 7028 2920 666f 7220 6d65  er.step() for me
-000043e0: 7465 7220 696e 206d 6574 6572 7320 6966  ter in meters if
-000043f0: 206d 6574 6572 2e61 6374 6976 655d 0d0a   meter.active]..
-00004400: 2020 2020 2020 2020 2020 2020 696e 666f              info
-00004410: 4c6f 6767 6572 2827 207c 7c20 272e 6a6f  Logger(' || '.jo
-00004420: 696e 2869 6e66 6f73 2929 0d0a 0d0a 2020  in(infos))....  
-00004430: 2020 4074 696d 656d 6574 6572 2822 436f    @timemeter("Co
-00004440: 6163 682f 7375 6d6d 6172 7922 290d 0a20  ach/summary").. 
-00004450: 2020 2064 6566 2073 756d 6d61 7279 2873     def summary(s
-00004460: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
-00004470: 2222 220d 0a20 2020 2020 2020 2053 756d  """..        Sum
-00004480: 6d61 7279 2074 6865 2077 686f 6c65 2074  mary the whole t
-00004490: 7261 696e 696e 6720 7072 6f63 6573 732e  raining process.
-000044a0: 0d0a 0d0a 2020 2020 2020 2020 4765 6e65  ....        Gene
-000044b0: 7261 7465 2061 2073 756d 6d61 7279 206f  rate a summary o
-000044c0: 6620 7468 6520 656e 7469 7265 2074 7261  f the entire tra
-000044d0: 696e 696e 6720 7072 6f63 6573 732c 2069  ining process, i
-000044e0: 6e63 6c75 6469 6e67 2074 6865 2068 6973  ncluding the his
-000044f0: 746f 7269 6361 6c20 6576 616c 7561 7469  torical evaluati
-00004500: 6f6e 2072 6573 756c 7473 2c20 7468 6520  on results, the 
-00004510: 6265 7374 0d0a 2020 2020 2020 2020 6869  best..        hi
-00004520: 7374 6f72 6963 616c 2072 6573 756c 7473  storical results
-00004530: 2c20 616e 6420 7468 6520 6375 7276 6573  , and the curves
-00004540: 206f 6620 6869 7374 6f72 6963 616c 2072   of historical r
-00004550: 6573 756c 7473 2e20 5468 6520 7265 7375  esults. The resu
-00004560: 6c74 696e 6720 7375 6d6d 6172 7920 6973  lting summary is
-00004570: 2073 6176 6564 2074 6f20 6120 4d61 726b   saved to a Mark
-00004580: 646f 776e 2066 696c 6520 6e61 6d65 640d  down file named.
-00004590: 0a20 2020 2020 2020 2022 5375 6d6d 6172  .        "Summar
-000045a0: 792e 6d64 2220 696e 2074 6865 2060 7365  y.md" in the `se
-000045b0: 6c66 2e63 6667 2e4c 4f47 5f50 4154 4860  lf.cfg.LOG_PATH`
-000045c0: 2064 6972 6563 746f 7279 2e0d 0a0d 0a20   directory..... 
-000045d0: 2020 2020 2020 2041 6464 6974 696f 6e61         Additiona
-000045e0: 6c6c 792c 2074 6865 2062 6573 7420 6869  lly, the best hi
-000045f0: 7374 6f72 6963 616c 2072 6573 756c 7473  storical results
-00004600: 2061 7265 2073 6176 6564 2074 6f20 6120   are saved to a 
-00004610: 6269 6e61 7279 2066 696c 6520 6e61 6d65  binary file name
-00004620: 6420 6073 656c 662e 6366 672e 4d4f 4e49  d `self.cfg.MONI
-00004630: 544f 525f 4245 5354 5f46 494c 454e 414d  TOR_BEST_FILENAM
-00004640: 4560 2e0d 0a20 2020 2020 2020 2022 2222  E`...        """
-00004650: 0d0a 2020 2020 2020 2020 7320 3d20 227c  ..        s = "|
-00004660: 2020 7b70 7265 6669 787d 2020 7c20 2020    {prefix}  |   
-00004670: 7b6e 616d 657d 2020 207c 2020 207b 7661  {name}   |   {va
-00004680: 6c7d 2020 207c 2020 207b 6570 6f63 687d  l}   |   {epoch}
-00004690: 2020 207c 2020 207b 696d 677d 2020 207c     |   {img}   |
-000046a0: 5c6e 220d 0a20 2020 2020 2020 2069 6e66  \n"..        inf
-000046b0: 6f20 3d20 2222 0d0a 2020 2020 2020 2020  o = ""..        
-000046c0: 696e 666f 202b 3d20 227c 2020 5072 6566  info += "|  Pref
-000046d0: 6978 2020 7c20 2020 4d65 7472 6963 2020  ix  |   Metric  
-000046e0: 207c 2020 2042 6573 7420 2020 7c20 2020   |   Best   |   
-000046f0: 4045 706f 6368 2020 207c 2020 2049 6d67  @Epoch   |   Img
-00004700: 2020 207c 5c6e 220d 0a20 2020 2020 2020     |\n"..       
-00004710: 2069 6e66 6f20 2b3d 2022 7c20 3a2d 2d2d   info += "| :---
-00004720: 2d2d 2d2d 3a20 7c20 3a2d 2d2d 2d2d 2d2d  ----: | :-------
-00004730: 3a20 7c20 3a2d 2d2d 2d2d 2d2d 3a20 7c20  : | :-------: | 
-00004740: 3a2d 2d2d 2d2d 2d2d 3a20 7c20 3a2d 2d2d  :-------: | :---
-00004750: 2d2d 2d2d 3a20 7c5c 6e22 0d0a 2020 2020  ----: |\n"..    
-00004760: 2020 2020 6461 7461 203d 205b 5d0d 0a20      data = [].. 
-00004770: 2020 2020 2020 2062 6573 7420 3d20 6465         best = de
-00004780: 6661 756c 7464 6963 7428 6469 6374 290d  faultdict(dict).
-00004790: 0a0d 0a20 2020 2020 2020 2066 6f72 2070  ...        for p
-000047a0: 7265 6669 782c 206d 6574 7269 6373 2069  refix, metrics i
-000047b0: 6e20 7365 6c66 2e6d 6f6e 6974 6f72 732e  n self.monitors.
-000047c0: 6974 656d 7328 293a 0d0a 2020 2020 2020  items():..      
-000047d0: 2020 2020 2020 6d65 7472 6963 733a 2064        metrics: d
-000047e0: 6566 6175 6c74 6469 6374 5b73 7472 2c20  efaultdict[str, 
-000047f0: 4c69 7374 5b41 7665 7261 6765 4d65 7465  List[AverageMete
-00004800: 725d 5d0d 0a20 2020 2020 2020 2020 2020  r]]..           
-00004810: 2066 7265 7120 3d20 3120 6966 2070 7265   freq = 1 if pre
-00004820: 6669 7820 3d3d 2027 7472 6169 6e27 2065  fix == 'train' e
-00004830: 6c73 6520 7365 6c66 2e63 6667 2e45 5641  lse self.cfg.EVA
-00004840: 4c5f 4652 4551 0d0a 2020 2020 2020 2020  L_FREQ..        
-00004850: 2020 2020 666f 7220 6c61 7374 6e61 6d65      for lastname
-00004860: 2c20 6d65 7465 7273 2069 6e20 6d65 7472  , meters in metr
-00004870: 6963 732e 6974 656d 7328 293a 0d0a 2020  ics.items():..  
-00004880: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00004890: 7220 6d65 7465 7220 696e 206d 6574 6572  r meter in meter
-000048a0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000048b0: 2020 2020 2020 2020 2320 536b 6970 2074          # Skip t
-000048c0: 686f 7365 206d 6574 6572 7320 6e65 7665  hose meters neve
-000048d0: 7220 6163 7469 7661 7465 642e 0d0a 2020  r activated...  
-000048e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048f0: 2020 6966 206c 656e 286d 6574 6572 2e68    if len(meter.h
-00004900: 6973 746f 7279 2920 3d3d 2030 3a0d 0a20  istory) == 0:.. 
-00004910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004920: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
-00004930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004940: 2020 2020 206d 6574 6572 2e70 6c6f 7428       meter.plot(
-00004950: 6672 6571 3d66 7265 7129 0d0a 2020 2020  freq=freq)..    
-00004960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004970: 696d 676e 616d 6520 3d20 6d65 7465 722e  imgname = meter.
-00004980: 7361 7665 2870 6174 683d 6f73 2e70 6174  save(path=os.pat
-00004990: 682e 6a6f 696e 2873 656c 662e 6366 672e  h.join(self.cfg.
-000049a0: 4c4f 475f 5041 5448 2c20 7365 6c66 2e63  LOG_PATH, self.c
-000049b0: 6667 2e53 554d 4d41 5259 5f44 4952 292c  fg.SUMMARY_DIR),
-000049c0: 2070 7265 6669 783d 7072 6566 6978 290d   prefix=prefix).
-000049d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000049e0: 2020 2020 2065 706f 6368 2c20 7661 6c20       epoch, val 
-000049f0: 3d20 6d65 7465 722e 6172 6762 6573 7428  = meter.argbest(
-00004a00: 6672 6571 290d 0a20 2020 2020 2020 2020  freq)..         
-00004a10: 2020 2020 2020 2020 2020 2069 6e66 6f20             info 
-00004a20: 2b3d 2073 2e66 6f72 6d61 7428 0d0a 2020  += s.format(..  
-00004a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a40: 2020 2020 2020 7072 6566 6978 3d70 7265        prefix=pre
-00004a50: 6669 782c 206e 616d 653d 6d65 7465 722e  fix, name=meter.
-00004a60: 6e61 6d65 2c0d 0a20 2020 2020 2020 2020  name,..         
-00004a70: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00004a80: 616c 3d76 616c 2c20 6570 6f63 683d 6570  al=val, epoch=ep
-00004a90: 6f63 682c 2069 6d67 3d66 2221 5b5d 287b  och, img=f"![]({
-00004aa0: 696d 676e 616d 657d 2922 0d0a 2020 2020  imgname})"..    
-00004ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ac0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00004ad0: 2020 2020 2020 2064 6174 612e 6170 7065         data.appe
-00004ae0: 6e64 285b 7072 6566 6978 2c20 6d65 7465  nd([prefix, mete
-00004af0: 722e 6e61 6d65 2c20 7661 6c2c 2065 706f  r.name, val, epo
-00004b00: 6368 5d29 0d0a 2020 2020 2020 2020 2020  ch])..          
-00004b10: 2020 2020 2020 2020 2020 6966 2076 616c            if val
-00004b20: 2021 3d20 2d31 3a20 2320 4f6e 6c79 2073   != -1: # Only s
-00004b30: 6176 6520 6176 6169 6c61 626c 6520 6461  ave available da
-00004b40: 7461 2e0d 0a20 2020 2020 2020 2020 2020  ta...           
-00004b50: 2020 2020 2020 2020 2020 2020 2062 6573               bes
-00004b60: 745b 7072 6566 6978 5d5b 6d65 7465 722e  t[prefix][meter.
-00004b70: 6e61 6d65 5d20 3d20 7661 6c0d 0a0d 0a20  name] = val.... 
-00004b80: 2020 2020 2020 2066 696c 655f 203d 206f         file_ = o
-00004b90: 732e 7061 7468 2e6a 6f69 6e28 7365 6c66  s.path.join(self
-00004ba0: 2e63 6667 2e4c 4f47 5f50 4154 482c 2073  .cfg.LOG_PATH, s
-00004bb0: 656c 662e 6366 672e 5355 4d4d 4152 595f  elf.cfg.SUMMARY_
-00004bc0: 4449 522c 2073 656c 662e 6366 672e 5355  DIR, self.cfg.SU
-00004bd0: 4d4d 4152 595f 4649 4c45 4e41 4d45 290d  MMARY_FILENAME).
-00004be0: 0a20 2020 2020 2020 2077 6974 6820 6f70  .        with op
-00004bf0: 656e 2866 696c 655f 2c20 2277 222c 2065  en(file_, "w", e
-00004c00: 6e63 6f64 696e 673d 2275 7466 3822 2920  ncoding="utf8") 
-00004c10: 6173 2066 683a 0d0a 2020 2020 2020 2020  as fh:..        
-00004c20: 2020 2020 6668 2e77 7269 7465 2869 6e66      fh.write(inf
-00004c30: 6f29 0d0a 0d0a 2020 2020 2020 2020 6466  o)....        df
-00004c40: 203d 2070 642e 4461 7461 4672 616d 6528   = pd.DataFrame(
-00004c50: 6461 7461 2c20 636f 6c75 6d6e 733d 5b27  data, columns=['
-00004c60: 5072 6566 6978 272c 2027 4d65 7472 6963  Prefix', 'Metric
-00004c70: 272c 2027 4265 7374 272c 2027 4045 706f  ', 'Best', '@Epo
-00004c80: 6368 275d 290d 0a20 2020 2020 2020 2069  ch'])..        i
-00004c90: 6e66 6f4c 6f67 6765 7228 7374 7228 6466  nfoLogger(str(df
-00004ca0: 2929 0d0a 2020 2020 2020 2020 696e 666f  ))..        info
-00004cb0: 4c6f 6767 6572 2866 225b 4c6f 475f 5061  Logger(f"[LoG_Pa
-00004cc0: 5448 5d20 3e3e 3e20 7b73 656c 662e 6366  TH] >>> {self.cf
-00004cd0: 672e 4c4f 475f 5041 5448 7d22 290d 0a0d  g.LOG_PATH}")...
-00004ce0: 0a20 2020 2020 2020 2073 656c 662e 6d6f  .        self.mo
-00004cf0: 6e69 746f 7273 2e77 7269 7465 286f 732e  nitors.write(os.
-00004d00: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e63  path.join(self.c
-00004d10: 6667 2e4c 4f47 5f50 4154 482c 2073 656c  fg.LOG_PATH, sel
-00004d20: 662e 6366 672e 5355 4d4d 4152 595f 4449  f.cfg.SUMMARY_DI
-00004d30: 5229 2920 2320 7465 6e73 6f72 626f 6172  R)) # tensorboar
-00004d40: 640d 0a0d 0a20 2020 2020 2020 2073 656c  d....        sel
-00004d50: 662e 6d6f 6e69 746f 7273 2e73 6176 6528  f.monitors.save(
-00004d60: 6f73 2e70 6174 682e 6a6f 696e 2873 656c  os.path.join(sel
-00004d70: 662e 6366 672e 4c4f 475f 5041 5448 2c20  f.cfg.LOG_PATH, 
-00004d80: 7365 6c66 2e63 6667 2e44 4154 415f 4449  self.cfg.DATA_DI
-00004d90: 5229 2c20 7365 6c66 2e63 6667 2e4d 4f4e  R), self.cfg.MON
-00004da0: 4954 4f52 5f46 494c 454e 414d 4529 0d0a  ITOR_FILENAME)..
-00004db0: 2020 2020 2020 2020 6578 706f 7274 5f70          export_p
-00004dc0: 6963 6b6c 6528 6265 7374 2c20 6f73 2e70  ickle(best, os.p
-00004dd0: 6174 682e 6a6f 696e 2873 656c 662e 6366  ath.join(self.cf
-00004de0: 672e 4c4f 475f 5041 5448 2c20 7365 6c66  g.LOG_PATH, self
-00004df0: 2e63 6667 2e44 4154 415f 4449 522c 2073  .cfg.DATA_DIR, s
-00004e00: 656c 662e 6366 672e 4d4f 4e49 544f 525f  elf.cfg.MONITOR_
-00004e10: 4245 5354 5f46 494c 454e 414d 4529 290d  BEST_FILENAME)).
-00004e20: 0a20 2020 200d 0a20 2020 2040 7469 6d65  .    ..    @time
-00004e30: 6d65 7465 7228 2243 6f61 6368 2f66 6974  meter("Coach/fit
-00004e40: 2229 0d0a 2020 2020 6465 6620 6669 7428  ")..    def fit(
-00004e50: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00004e60: 7374 6172 745f 6570 6f63 6820 3d20 7365  start_epoch = se
-00004e70: 6c66 2e72 6573 756d 6528 290d 0a20 2020  lf.resume()..   
-00004e80: 2020 2020 2066 6f72 2065 706f 6368 2069       for epoch i
-00004e90: 6e20 7261 6e67 6528 7374 6172 745f 6570  n range(start_ep
-00004ea0: 6f63 682c 2073 656c 662e 6366 672e 6570  och, self.cfg.ep
-00004eb0: 6f63 6873 293a 0d0a 2020 2020 2020 2020  ochs):..        
-00004ec0: 2020 2020 6966 2065 706f 6368 2025 2073      if epoch % s
-00004ed0: 656c 662e 6366 672e 4348 4543 4b50 4f49  elf.cfg.CHECKPOI
-00004ee0: 4e54 5f46 5245 5120 3d3d 2030 3a0d 0a20  NT_FREQ == 0:.. 
-00004ef0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00004f00: 656c 662e 7361 7665 5f63 6865 636b 706f  elf.save_checkpo
-00004f10: 696e 7428 6570 6f63 6829 0d0a 2020 2020  int(epoch)..    
-00004f20: 2020 2020 2020 2020 6966 2065 706f 6368          if epoch
-00004f30: 2025 2073 656c 662e 6366 672e 4556 414c   % self.cfg.EVAL
-00004f40: 5f46 5245 5120 3d3d 2030 3a0d 0a20 2020  _FREQ == 0:..   
-00004f50: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00004f60: 7365 6c66 2e63 6667 2e45 5641 4c5f 5641  self.cfg.EVAL_VA
-00004f70: 4c49 443a 0d0a 2020 2020 2020 2020 2020  LID:..          
-00004f80: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
-00004f90: 616c 6964 2829 0d0a 2020 2020 2020 2020  alid()..        
-00004fa0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00004fb0: 6366 672e 4556 414c 5f54 4553 543a 0d0a  cfg.EVAL_TEST:..
-00004fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fd0: 2020 2020 7365 6c66 2e74 6573 7428 290d      self.test().
-00004fe0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00004ff0: 662e 6368 6563 6b5f 6265 7374 2865 706f  f.check_best(epo
-00005000: 6368 290d 0a20 2020 2020 2020 2020 2020  ch)..           
-00005010: 2073 656c 662e 7374 6570 2865 706f 6368   self.step(epoch
-00005020: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00005030: 656c 662e 7472 6169 6e28 290d 0a0d 0a20  elf.train().... 
-00005040: 2020 2020 2020 2073 656c 662e 7361 7665         self.save
-00005050: 2829 0d0a 0d0a 2020 2020 2020 2020 2320  ()....        # 
-00005060: 6c61 7374 2065 706f 6368 0d0a 2020 2020  last epoch..    
-00005070: 2020 2020 7365 6c66 2e76 616c 6964 2829      self.valid()
-00005080: 0d0a 2020 2020 2020 2020 7365 6c66 2e74  ..        self.t
-00005090: 6573 7428 290d 0a20 2020 2020 2020 2073  est()..        s
-000050a0: 656c 662e 6368 6563 6b5f 6265 7374 2873  elf.check_best(s
-000050b0: 656c 662e 6366 672e 6570 6f63 6873 290d  elf.cfg.epochs).
-000050c0: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-000050d0: 6570 2873 656c 662e 6366 672e 6570 6f63  ep(self.cfg.epoc
-000050e0: 6873 290d 0a0d 0a20 2020 2020 2020 2073  hs)....        s
-000050f0: 656c 662e 7375 6d6d 6172 7928 290d 0a0d  elf.summary()...
-00005100: 0a20 2020 2020 2020 2073 656c 662e 6576  .        self.ev
-00005110: 616c 5f61 745f 6265 7374 2829 0d0a 0d0a  al_at_best()....
-00005120: 0d0a 636c 6173 7320 4164 6170 7465 723a  ..class Adapter:
-00005130: 0d0a 2020 2020 7222 2222 0d0a 2020 2020  ..    r"""..    
-00005140: 5061 7261 6d73 2074 756e 6572 2e0d 0a0d  Params tuner....
-00005150: 0a20 2020 2046 6c6f 7773 3a0d 0a20 2020  .    Flows:..   
-00005160: 202d 2d2d 2d2d 2d0d 0a20 2020 2031 2e20   ------..    1. 
-00005170: 636f 6d70 696c 653a 2063 6f6e 6669 6775  compile: configu
-00005180: 7265 2074 6865 2063 6f6d 6d61 6e64 2c20  re the command, 
-00005190: 656e 7669 726f 6e6d 656e 7473 2c20 616e  environments, an
-000051a0: 6420 7061 7261 6d65 7465 7273 2066 6f72  d parameters for
-000051b0: 2074 7261 696e 696e 672e 0d0a 2020 2020   training...    
-000051c0: 322e 2061 6c6c 6f63 6174 6520 6465 7669  2. allocate devi
-000051d0: 6365 7320 666f 7220 7661 7269 6f75 7320  ces for various 
-000051e0: 7061 7261 6d65 7465 7273 3a0d 0a20 2020  parameters:..   
-000051f0: 2020 2020 202d 2072 6567 6973 7465 7220       - register 
-00005200: 7468 6520 4944 2c20 6c6f 6720 7061 7468  the ID, log path
-00005210: 2c20 616e 6420 6465 7669 6365 2066 6972  , and device fir
-00005220: 7374 0d0a 2020 2020 2020 2020 2d20 6578  st..        - ex
-00005230: 6563 7574 6520 7468 6520 636f 6d6d 616e  ecute the comman
-00005240: 640d 0a20 2020 2020 2020 202d 2063 6f6c  d..        - col
-00005250: 6c65 6374 2069 6e66 6f72 6d61 7469 6f6e  lect information
-00005260: 2066 726f 6d20 7468 6520 6c6f 6720 7061   from the log pa
-00005270: 7468 2061 6e64 206f 7574 7075 7420 746f  th and output to
-00005280: 2054 656e 736f 7242 6f61 7264 0d0a 2020   TensorBoard..  
-00005290: 2020 2020 2020 2d20 7361 7665 2074 6865        - save the
-000052a0: 2063 6865 636b 706f 696e 740d 0a20 2020   checkpoint..   
-000052b0: 2020 2020 202d 2072 656c 6561 7365 2074       - release t
-000052c0: 6865 2063 6f72 7265 7370 6f6e 6469 6e67  he corresponding
-000052d0: 2064 6576 6963 650d 0a0d 0a20 2020 2045   device....    E
-000052e0: 7861 6d70 6c65 733a 0d0a 2020 2020 2d2d  xamples:..    --
-000052f0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 203e 3e3e  -------..    >>>
-00005300: 2063 6667 203d 207b 2763 6f6d 6d61 6e64   cfg = {'command
-00005310: 273a 2027 7079 7468 6f6e 2078 7878 2e70  ': 'python xxx.p
-00005320: 7927 2c20 2770 6172 616d 7327 3a20 7b27  y', 'params': {'
-00005330: 6f70 7469 6d69 7a65 7227 3a20 5b27 7367  optimizer': ['sg
-00005340: 6427 2c20 2761 6461 6d27 5d7d 7d0d 0a20  d', 'adam']}}.. 
-00005350: 2020 203e 3e3e 2074 756e 6572 203d 2041     >>> tuner = A
-00005360: 6461 7074 6572 2829 0d0a 2020 2020 3e3e  dapter()..    >>
-00005370: 3e20 7475 6e65 722e 636f 6d70 696c 6528  > tuner.compile(
-00005380: 6366 6729 0d0a 2020 2020 3e3e 3e20 7475  cfg)..    >>> tu
-00005390: 6e65 722e 6669 7428 290d 0a20 2020 2022  ner.fit()..    "
-000053a0: 2222 0d0a 0d0a 2020 2020 6465 6620 5f5f  ""....    def __
-000053b0: 696e 6974 5f5f 2873 656c 6629 202d 3e20  init__(self) -> 
-000053c0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2073  None:..        s
-000053d0: 656c 662e 7061 7261 6d73 203d 205b 5d0d  elf.params = [].
-000053e0: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
-000053f0: 6c75 6573 203d 205b 5d0d 0a20 2020 2020  lues = []..     
-00005400: 2020 2073 656c 662e 6465 7669 6365 7320     self.devices 
-00005410: 3d20 5b5d 0d0a 0d0a 2020 2020 4070 726f  = []....    @pro
-00005420: 7065 7274 790d 0a20 2020 2064 6566 2043  perty..    def C
-00005430: 4f4d 4d41 4e44 2873 656c 6629 3a0d 0a20  OMMAND(self):.. 
-00005440: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00005450: 6c66 2e63 6667 2e43 4f4d 4d41 4e44 0d0a  lf.cfg.COMMAND..
-00005460: 0d0a 2020 2020 6465 6620 7265 6769 7374  ..    def regist
-00005470: 6572 2873 656c 662c 2064 6576 6963 653a  er(self, device:
-00005480: 2073 7472 2920 2d3e 2054 7570 6c65 5b73   str) -> Tuple[s
-00005490: 7472 2c20 7374 725d 3a0d 0a20 2020 2020  tr, str]:..     
-000054a0: 2020 2073 656c 662e 6366 672e 454e 5653     self.cfg.ENVS
-000054b0: 5b27 6964 275d 203d 2074 696d 652e 7374  ['id'] = time.st
-000054c0: 7266 7469 6d65 2854 494d 4529 0d0a 2020  rftime(TIME)..  
-000054d0: 2020 2020 2020 7365 6c66 2e63 6667 2e45        self.cfg.E
-000054e0: 4e56 535b 2764 6576 6963 6527 5d20 3d20  NVS['device'] = 
-000054f0: 6465 7669 6365 0d0a 2020 2020 2020 2020  device..        
-00005500: 636f 6d6d 616e 6420 3d20 7365 6c66 2e43  command = self.C
-00005510: 4f4d 4d41 4e44 202b 2073 656c 662e 6765  OMMAND + self.ge
-00005520: 745f 6f70 7469 6f6e 2827 6964 272c 2073  t_option('id', s
-00005530: 656c 662e 6366 672e 454e 5653 2e69 6429  elf.cfg.ENVS.id)
-00005540: 0d0a 2020 2020 2020 2020 636f 6d6d 616e  ..        comman
-00005550: 6420 2b3d 2073 656c 662e 6765 745f 6f70  d += self.get_op
-00005560: 7469 6f6e 2827 6465 7669 6365 272c 2073  tion('device', s
-00005570: 656c 662e 6366 672e 454e 5653 2e64 6576  elf.cfg.ENVS.dev
-00005580: 6963 6529 0d0a 2020 2020 2020 2020 7265  ice)..        re
-00005590: 7475 726e 2063 6f6d 6d61 6e64 2c20 7365  turn command, se
-000055a0: 6c66 2e63 6667 2e45 4e56 532e 6964 2c20  lf.cfg.ENVS.id, 
-000055b0: 7365 6c66 2e63 6667 2e4c 4f47 5f50 4154  self.cfg.LOG_PAT
-000055c0: 482e 666f 726d 6174 282a 2a73 656c 662e  H.format(**self.
-000055d0: 6366 672e 454e 5653 290d 0a0d 0a20 2020  cfg.ENVS)....   
-000055e0: 2040 7469 6d65 6d65 7465 7228 2241 6461   @timemeter("Ada
-000055f0: 7074 6572 2f63 6f6d 7069 6c65 2229 0d0a  pter/compile")..
-00005600: 2020 2020 6465 6620 636f 6d70 696c 6528      def compile(
-00005610: 7365 6c66 2c20 6366 673a 2043 6f6e 6669  self, cfg: Confi
-00005620: 6729 202d 3e20 4e6f 6e65 3a0d 0a20 2020  g) -> None:..   
-00005630: 2020 2020 2072 2222 220d 0a20 2020 2020       r"""..     
-00005640: 2020 2043 6f6e 6669 6775 7265 2074 6865     Configure the
-00005650: 2063 6f6d 6d61 6e64 2c20 656e 7669 726f   command, enviro
-00005660: 6e6d 656e 7473 2c20 616e 6420 7061 7261  nments, and para
-00005670: 6d65 7465 7273 2066 6f72 2074 7261 696e  meters for train
-00005680: 696e 672e 0d0a 0d0a 2020 2020 2020 2020  ing.....        
-00005690: 5061 7261 6d65 7465 7273 3a0d 0a20 2020  Parameters:..   
-000056a0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d       -----------
-000056b0: 0d0a 2020 2020 2020 2020 6366 6720 3a20  ..        cfg : 
-000056c0: 436f 6e66 6967 0d0a 2020 2020 2020 2020  Config..        
-000056d0: 2020 2020 416e 206f 626a 6563 7420 7468      An object th
-000056e0: 6174 2063 6f6e 7461 696e 7320 7468 6520  at contains the 
-000056f0: 636f 6d6d 616e 642c 2065 6e76 6972 6f6e  command, environ
-00005700: 6d65 6e74 732c 2070 6172 616d 6574 6572  ments, parameter
-00005710: 732c 2061 6e64 2064 6566 6175 6c74 732e  s, and defaults.
-00005720: 0d0a 0d0a 2020 2020 2020 2020 466c 6f77  ....        Flow
-00005730: 733a 0d0a 2020 2020 2020 2020 2d2d 2d2d  s:..        ----
-00005740: 2d2d 0d0a 2020 2020 2020 2020 312e 2041  --..        1. A
-00005750: 6464 2065 6e76 6972 6f6e 6d65 6e74 616c  dd environmental
-00005760: 2070 6172 616d 6574 6572 7320 746f 2074   parameters to t
-00005770: 6865 2062 6173 6963 2060 636f 6d6d 616e  he basic `comman
-00005780: 6460 2e0d 0a20 2020 2020 2020 2032 2e20  d`...        2. 
-00005790: 5265 6769 7374 6572 2061 6c6c 2061 7661  Register all ava
-000057a0: 696c 6162 6c65 2064 6576 6963 6573 2e0d  ilable devices..
-000057b0: 0a20 2020 2020 2020 2033 2e20 436f 6e76  .        3. Conv
-000057c0: 6572 7420 616c 6c20 7061 7261 6d65 7465  ert all paramete
-000057d0: 7273 2066 726f 6d20 6063 6667 2e50 4152  rs from `cfg.PAR
-000057e0: 414d 5360 2e0d 0a20 2020 2020 2020 2034  AMS`...        4
-000057f0: 2e20 436f 6e76 6572 7420 616c 6c20 6465  . Convert all de
-00005800: 6661 756c 7473 2066 726f 6d20 6063 6667  faults from `cfg
-00005810: 2e44 4546 4155 4c54 5360 2e0d 0a0d 0a20  .DEFAULTS`..... 
-00005820: 2020 2020 2020 2052 6574 7572 6e73 3a0d         Returns:.
-00005830: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00005840: 2d0d 0a20 2020 2020 2020 204e 6f6e 650d  -..        None.
-00005850: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00005860: 2020 2020 2020 7365 6c66 2e63 6667 203d        self.cfg =
-00005870: 2063 6667 0d0a 2020 2020 2020 2020 7069   cfg..        pi
-00005880: 6563 6520 3d20 225c 747b 6b65 797d 3a20  ece = "\t{key}: 
-00005890: 7b76 616c 737d 205c 6e22 0d0a 2020 2020  {vals} \n"..    
-000058a0: 2020 2020 656e 7673 2c20 7061 7261 6d73      envs, params
-000058b0: 2c20 6465 6661 756c 7473 203d 2022 222c  , defaults = "",
-000058c0: 2022 222c 2022 220d 0a20 2020 2020 2020   "", ""..       
-000058d0: 2066 6f72 206b 6579 2c20 7661 6c20 696e   for key, val in
-000058e0: 2073 656c 662e 6366 672e 454e 5653 2e69   self.cfg.ENVS.i
-000058f0: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
-00005900: 2020 2020 2069 6620 6b65 7920 3d3d 2027       if key == '
-00005910: 6465 7669 6365 273a 0d0a 2020 2020 2020  device':..      
-00005920: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00005930: 6576 6963 6573 203d 2076 616c 2e73 706c  evices = val.spl
-00005940: 6974 2827 2c27 290d 0a20 2020 2020 2020  it(',')..       
-00005950: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00005960: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005970: 2e63 6667 2e43 4f4d 4d41 4e44 202b 3d20  .cfg.COMMAND += 
-00005980: 7365 6c66 2e67 6574 5f6f 7074 696f 6e28  self.get_option(
-00005990: 6b65 792c 2076 616c 290d 0a20 2020 2020  key, val)..     
-000059a0: 2020 2020 2020 2065 6e76 7320 2b3d 2070         envs += p
-000059b0: 6965 6365 2e66 6f72 6d61 7428 6b65 793d  iece.format(key=
-000059c0: 6b65 792c 2076 616c 733d 7661 6c29 0d0a  key, vals=val)..
-000059d0: 2020 2020 2020 2020 666f 7220 6b65 792c          for key,
-000059e0: 2076 616c 7320 696e 2073 656c 662e 6366   vals in self.cf
-000059f0: 672e 5041 5241 4d53 2e69 7465 6d73 2829  g.PARAMS.items()
-00005a00: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00005a10: 6620 6973 696e 7374 616e 6365 2876 616c  f isinstance(val
-00005a20: 732c 2028 7374 722c 2069 6e74 2c20 666c  s, (str, int, fl
-00005a30: 6f61 7429 293a 0d0a 2020 2020 2020 2020  oat)):..        
-00005a40: 2020 2020 2020 2020 7661 6c73 203d 205b          vals = [
-00005a50: 7661 6c73 5d0d 0a20 2020 2020 2020 2020  vals]..         
-00005a60: 2020 2073 656c 662e 6465 706c 6f79 5f70     self.deploy_p
-00005a70: 6172 616d 7328 6b65 792c 2076 616c 7329  arams(key, vals)
-00005a80: 0d0a 2020 2020 2020 2020 2020 2020 7061  ..            pa
-00005a90: 7261 6d73 202b 3d20 7069 6563 652e 666f  rams += piece.fo
-00005aa0: 726d 6174 286b 6579 3d6b 6579 2c20 7661  rmat(key=key, va
-00005ab0: 6c73 3d76 616c 7329 0d0a 2020 2020 2020  ls=vals)..      
-00005ac0: 2020 666f 7220 6b65 792c 2076 616c 2069    for key, val i
-00005ad0: 6e20 7365 6c66 2e63 6667 2e44 4546 4155  n self.cfg.DEFAU
-00005ae0: 4c54 532e 6974 656d 7328 293a 0d0a 2020  LTS.items():..  
-00005af0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00005b00: 6667 2e44 4546 4155 4c54 535b 6b65 795d  fg.DEFAULTS[key]
-00005b10: 203d 2076 616c 0d0a 2020 2020 2020 2020   = val..        
-00005b20: 2020 2020 6465 6661 756c 7473 202b 3d20      defaults += 
-00005b30: 7069 6563 652e 666f 726d 6174 286b 6579  piece.format(key
-00005b40: 3d6b 6579 2c20 7661 6c73 3d76 616c 290d  =key, vals=val).
-00005b50: 0a0d 0a20 2020 2020 2020 2063 6667 5f69  ...        cfg_i
-00005b60: 6e66 6f73 203d 2066 2263 6f6d 6d61 6e64  nfos = f"command
-00005b70: 3a20 7b73 656c 662e 6366 672e 434f 4d4d  : {self.cfg.COMM
-00005b80: 414e 447d 205c 6e65 6e76 733a 205c 6e7b  AND} \nenvs: \n{
-00005b90: 656e 7673 7d70 6172 616d 733a 205c 6e7b  envs}params: \n{
-00005ba0: 7061 7261 6d73 7d64 6566 6175 6c74 733a  params}defaults:
-00005bb0: 205c 6e7b 6465 6661 756c 7473 7d22 0d0a   \n{defaults}"..
-00005bc0: 2020 2020 2020 2020 696e 666f 4c6f 6767          infoLogg
-00005bd0: 6572 2866 225c 3033 335b 303b 3331 3b34  er(f"\033[0;31;4
-00005be0: 376d 7b63 6667 5f69 6e66 6f73 7d5c 3033  7m{cfg_infos}\03
-00005bf0: 335b 306d 2229 0d0a 2020 2020 2020 2020  3[0m")..        
-00005c00: 0d0a 0d0a 2020 2020 6465 6620 6465 706c  ....    def depl
-00005c10: 6f79 5f70 6172 616d 7328 7365 6c66 2c20  oy_params(self, 
-00005c20: 6b65 793a 2073 7472 2c20 7661 6c73 3a20  key: str, vals: 
-00005c30: 4974 6572 6162 6c65 293a 0d0a 2020 2020  Iterable):..    
-00005c40: 2020 2020 7365 6c66 2e70 6172 616d 732e      self.params.
-00005c50: 6170 7065 6e64 286b 6579 290d 0a20 2020  append(key)..   
-00005c60: 2020 2020 2073 656c 662e 7661 6c75 6573       self.values
-00005c70: 2e61 7070 656e 6428 7661 6c73 290d 0a0d  .append(vals)...
-00005c80: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-00005c90: 6f64 0d0a 2020 2020 6465 6620 6765 745f  od..    def get_
-00005ca0: 6f70 7469 6f6e 286b 6579 3a20 7374 722c  option(key: str,
-00005cb0: 2076 616c 3a20 416e 7929 3a0d 0a20 2020   val: Any):..   
-00005cc0: 2020 2020 2072 2222 220d 0a20 2020 2020       r"""..     
-00005cd0: 2020 2043 6f6e 7665 7274 2028 6b65 792c     Convert (key,
-00005ce0: 2076 616c 2920 746f 2027 2d2d 6b65 793d   val) to '--key=
-00005cf0: 7661 6c27 2e0d 0a0d 0a20 2020 2020 2020  val'.....       
-00005d00: 2050 6172 616d 6574 6572 733a 0d0a 2020   Parameters:..  
-00005d10: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-00005d20: 2d0d 0a20 2020 2020 2020 206b 6579 203a  -..        key :
-00005d30: 2073 7472 0d0a 2020 2020 2020 2020 2020   str..          
-00005d40: 2020 5468 6520 6b65 7920 6f66 2074 6865    The key of the
-00005d50: 2070 6172 616d 6574 6572 2e0d 0a20 2020   parameter...   
-00005d60: 2020 2020 2076 616c 203a 2041 6e79 0d0a       val : Any..
-00005d70: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00005d80: 7661 6c75 6520 6f66 2074 6865 2070 6172  value of the par
-00005d90: 616d 6574 6572 2e0d 0a0d 0a20 2020 2020  ameter.....     
-00005da0: 2020 204e 6f74 6573 3a0d 0a20 2020 2020     Notes:..     
-00005db0: 2020 202d 2d2d 2d2d 2d0d 0a20 2020 2020     ------..     
-00005dc0: 2020 2041 6c6c 2027 5f27 2069 6e20 606b     All '_' in `k
-00005dd0: 6579 6020 7769 6c6c 2062 6520 7265 706c  ey` will be repl
-00005de0: 6163 6564 2062 7920 272d 272e 0d0a 0d0a  aced by '-'.....
-00005df0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00005e00: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-00005e10: 2d2d 0d0a 2020 2020 2020 2020 7374 720d  --..        str.
-00005e20: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-00005e30: 2070 6172 616d 6574 6572 2077 6974 6820   parameter with 
-00005e40: 666f 726d 6174 2027 2d2d 6b65 793d 7661  format '--key=va
-00005e50: 6c27 2e0d 0a0d 0a20 2020 2020 2020 2045  l'.....        E
-00005e60: 7861 6d70 6c65 733a 0d0a 2020 2020 2020  xamples:..      
-00005e70: 2020 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020    ---------..   
-00005e80: 2020 2020 203e 3e3e 2041 6461 7074 6572       >>> Adapter
-00005e90: 2e67 6574 5f6f 7074 696f 6e28 276c 7227  .get_option('lr'
-00005ea0: 2c20 2731 652d 3327 290d 0a20 2020 2020  , '1e-3')..     
-00005eb0: 2020 2027 2d2d 6c72 3d31 652d 3327 0d0a     '--lr=1e-3'..
-00005ec0: 2020 2020 2020 2020 3e3e 3e20 4164 6170          >>> Adap
-00005ed0: 7465 722e 6765 745f 6f70 7469 6f6e 2827  ter.get_option('
-00005ee0: 6c65 6172 6e69 6e67 5f72 6174 6527 2c20  learning_rate', 
-00005ef0: 2731 652d 3327 290d 0a20 2020 2020 2020  '1e-3')..       
-00005f00: 2027 2d2d 6c65 6172 6e69 6e67 2d72 6174   '--learning-rat
-00005f10: 653d 3165 2d33 270d 0a20 2020 2020 2020  e=1e-3'..       
-00005f20: 2022 2222 0d0a 2020 2020 2020 2020 7265   """..        re
-00005f30: 7475 726e 2066 2220 2d2d 7b6b 6579 2e72  turn f" --{key.r
-00005f40: 6570 6c61 6365 2827 5f27 2c20 272d 2729  eplace('_', '-')
-00005f50: 7d3d 7b76 616c 7d22 0d0a 0d0a 2020 2020  }={val}"....    
-00005f60: 6465 6620 6c6f 6164 5f62 6573 7428 7365  def load_best(se
-00005f70: 6c66 2c20 6c6f 6750 6174 683a 2073 7472  lf, logPath: str
-00005f80: 293a 0d0a 2020 2020 2020 2020 2222 224c  ):..        """L
-00005f90: 6f61 6420 6265 7374 2e70 6963 6b6c 6520  oad best.pickle 
-00005fa0: 6672 6f6d 206c 6f67 5061 7468 206f 6620  from logPath of 
-00005fb0: 636f 7272 6573 706f 6e64 696e 672e 2222  corresponding.""
-00005fc0: 220d 0a20 2020 2020 2020 2066 696c 655f  "..        file_
-00005fd0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-00005fe0: 6c6f 6750 6174 682c 2073 656c 662e 6366  logPath, self.cf
-00005ff0: 672e 4441 5441 5f44 4952 2c20 7365 6c66  g.DATA_DIR, self
-00006000: 2e63 6667 2e4d 4f4e 4954 4f52 5f42 4553  .cfg.MONITOR_BES
-00006010: 545f 4649 4c45 4e41 4d45 290d 0a20 2020  T_FILENAME)..   
-00006020: 2020 2020 2072 6574 7572 6e20 696d 706f       return impo
-00006030: 7274 5f70 6963 6b6c 6528 6669 6c65 5f29  rt_pickle(file_)
-00006040: 0d0a 0d0a 2020 2020 6465 6620 7772 6974  ....    def writ
-00006050: 6528 7365 6c66 2c20 6964 5f3a 2073 7472  e(self, id_: str
-00006060: 2c20 6c6f 6750 6174 683a 2073 7472 2c20  , logPath: str, 
-00006070: 7061 7261 6d73 3a20 4469 6374 293a 0d0a  params: Dict):..
-00006080: 2020 2020 2020 2020 7222 2222 0d0a 2020          r"""..  
-00006090: 2020 2020 2020 5772 6974 6520 6578 7065        Write expe
-000060a0: 7269 6d65 6e74 2072 6573 756c 7473 2074  riment results t
-000060b0: 6f20 7465 6e73 6f72 626f 6172 642e 0d0a  o tensorboard...
-000060c0: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-000060d0: 7465 7273 3a0d 0a20 2020 2020 2020 202d  ters:..        -
-000060e0: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
-000060f0: 2020 2020 6964 5f3a 2073 7472 0d0a 2020      id_: str..  
-00006100: 2020 2020 2020 2020 2020 4578 7065 7269            Experi
-00006110: 6d65 6e74 2049 442e 0d0a 2020 2020 2020  ment ID...      
-00006120: 2020 6c6f 6750 6174 683a 2073 7472 0d0a    logPath: str..
-00006130: 2020 2020 2020 2020 2020 2020 5061 7468              Path
-00006140: 2074 6f20 7468 6520 6578 7065 7269 6d65   to the experime
-00006150: 6e74 206c 6f67 732e 0d0a 2020 2020 2020  nt logs...      
-00006160: 2020 7061 7261 6d73 3a20 4469 6374 0d0a    params: Dict..
-00006170: 2020 2020 2020 2020 2020 2020 436f 6e66              Conf
-00006180: 6967 7572 6174 696f 6e20 7061 7261 6d65  iguration parame
-00006190: 7465 7273 206f 6620 7468 6520 6578 7065  ters of the expe
-000061a0: 7269 6d65 6e74 2e0d 0a0d 0a20 2020 2020  riment.....     
-000061b0: 2020 2046 6c6f 7773 3a0d 0a20 2020 2020     Flows:..     
-000061c0: 2020 202d 2d2d 2d2d 2d0d 0a20 2020 2020     ------..     
-000061d0: 2020 2031 2e20 4c6f 6164 2074 6865 2062     1. Load the b
-000061e0: 6573 7420 6461 7461 2066 726f 6d20 606c  est data from `l
-000061f0: 6f67 5061 7468 602e 0d0a 2020 2020 2020  ogPath`...      
-00006200: 2020 322e 2057 7269 7465 2074 6865 2062    2. Write the b
-00006210: 6573 7420 6461 7461 2074 6f20 7465 6e73  est data to tens
-00006220: 6f72 626f 6172 6420 7769 7468 2060 7061  orboard with `pa
-00006230: 7261 6d73 602e 0d0a 0d0a 2020 2020 2020  rams`.....      
-00006240: 2020 4e6f 7465 733a 0d0a 2020 2020 2020    Notes:..      
-00006250: 2020 2d2d 2d2d 2d2d 0d0a 2020 2020 2020    ------..      
-00006260: 2020 4966 2079 6f75 2066 696e 6420 602d    If you find `-
-00006270: 3160 2061 7070 6561 7269 6e67 2069 6e20  1` appearing in 
-00006280: 7468 6520 7465 6e73 6f72 626f 6172 642c  the tensorboard,
-00006290: 0d0a 2020 2020 2020 2020 6974 2063 6f75  ..        it cou
-000062a0: 6c64 206d 6561 6e20 7468 6174 2074 6865  ld mean that the
-000062b0: 2064 6174 6120 6973 206f 6620 6073 7472   data is of `str
-000062c0: 6020 7479 7065 2c0d 0a20 2020 2020 2020  ` type,..       
-000062d0: 2077 6869 6368 2077 696c 6c20 6361 7573   which will caus
-000062e0: 6520 616e 2065 7272 6f72 2069 6620 6974  e an error if it
-000062f0: 2069 7320 7365 6e74 2074 6f20 7465 6e73   is sent to tens
-00006300: 6f72 626f 6172 6420 6469 7265 6374 6c79  orboard directly
-00006310: 210d 0a20 2020 2020 2020 2022 2222 0d0a  !..        """..
-00006320: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-00006330: 2020 2020 2020 2020 2020 6461 7461 203d            data =
-00006340: 2073 656c 662e 6c6f 6164 5f62 6573 7428   self.load_best(
-00006350: 6c6f 6750 6174 6829 0d0a 2020 2020 2020  logPath)..      
-00006360: 2020 2020 2020 7061 7468 203d 206f 732e        path = os.
-00006370: 7061 7468 2e6a 6f69 6e28 7365 6c66 2e63  path.join(self.c
-00006380: 6667 2e43 4f52 455f 4c4f 475f 5041 5448  fg.CORE_LOG_PATH
-00006390: 2c20 6964 5f29 0d0a 2020 2020 2020 2020  , id_)..        
-000063a0: 2020 2020 7769 7468 2053 756d 6d61 7279      with Summary
-000063b0: 5772 6974 6572 286c 6f67 5f64 6972 3d70  Writer(log_dir=p
-000063c0: 6174 6829 2061 7320 7772 6974 6572 3a0d  ath) as writer:.
-000063d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000063e0: 206d 6574 7269 6373 203d 2064 6963 7428   metrics = dict(
-000063f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00006400: 2020 2066 6f72 2070 7265 6669 782c 2062     for prefix, b
-00006410: 6573 7420 696e 2064 6174 612e 6974 656d  est in data.item
-00006420: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-00006430: 2020 2020 2020 2020 2020 666f 7220 6d65            for me
-00006440: 7472 6963 2c20 7661 6c20 696e 2062 6573  tric, val in bes
-00006450: 742e 6974 656d 7328 293a 0d0a 2020 2020  t.items():..    
-00006460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006470: 2020 2020 7661 6c20 3d20 7661 6c20 6966      val = val if
-00006480: 2069 7369 6e73 7461 6e63 6528 7661 6c2c   isinstance(val,
-00006490: 2028 696e 742c 2066 6c6f 6174 2929 2065   (int, float)) e
-000064a0: 6c73 6520 2d31 0d0a 2020 2020 2020 2020  lse -1..        
-000064b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064c0: 6d65 7472 6963 735b 272f 272e 6a6f 696e  metrics['/'.join
-000064d0: 285b 7072 6566 6978 2c20 6d65 7472 6963  ([prefix, metric
-000064e0: 5d29 5d20 3d20 7661 6c0d 0a20 2020 2020  ])] = val..     
-000064f0: 2020 2020 2020 2020 2020 2077 7269 7465             write
-00006500: 722e 6164 645f 6870 6172 616d 7328 0d0a  r.add_hparams(..
-00006510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006520: 2020 2020 7061 7261 6d73 2c20 6d65 7472      params, metr
-00006530: 6963 732c 0d0a 2020 2020 2020 2020 2020  ics,..          
-00006540: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00006550: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-00006560: 6e3a 0d0a 2020 2020 2020 2020 2020 2020  n:..            
-00006570: 696e 666f 4c6f 6767 6572 280d 0a20 2020  infoLogger(..   
-00006580: 2020 2020 2020 2020 2020 2020 2066 225c               f"\
-00006590: 3033 335b 303b 3331 3b34 376d 5b41 6461  033[0;31;47m[Ada
-000065a0: 7074 6572 5d20 3e3e 3e20 556e 6b6e 6f77  pter] >>> Unknow
-000065b0: 6e20 6572 726f 7273 2068 6170 7065 6e2e  n errors happen.
-000065c0: 2054 6869 7320 6973 206d 6169 6e6c 7920   This is mainly 
-000065d0: 6475 6520 746f 2061 626e 6f72 6d61 6c20  due to abnormal 
-000065e0: 6578 6974 7320 6f66 2063 6869 6c64 2070  exits of child p
-000065f0: 726f 6365 7373 6573 2e5c 3033 335b 306d  rocesses.\033[0m
-00006600: 220d 0a20 2020 2020 2020 2020 2020 2029  "..            )
-00006610: 0d0a 0d0a 0d0a 2020 2020 6465 6620 6561  ......    def ea
-00006620: 6368 5f67 7269 6428 7365 6c66 293a 0d0a  ch_grid(self):..
-00006630: 2020 2020 2020 2020 2222 2247 7269 6420          """Grid 
-00006640: 7365 6172 6368 2066 6f72 2065 6163 6820  search for each 
-00006650: 6b69 6e64 206f 6620 7061 7261 6d2e 2222  kind of param.""
-00006660: 220d 0a20 2020 2020 2020 2066 6f72 206b  "..        for k
-00006670: 6579 2c20 7661 6c73 2069 6e20 7a69 7028  ey, vals in zip(
-00006680: 7365 6c66 2e70 6172 616d 732c 2073 656c  self.params, sel
-00006690: 662e 7661 6c75 6573 293a 0d0a 2020 2020  f.values):..    
-000066a0: 2020 2020 2020 2020 666f 7220 7661 6c20          for val 
-000066b0: 696e 2076 616c 733a 0d0a 2020 2020 2020  in vals:..      
-000066c0: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
-000066d0: 7365 6c66 2e63 6667 2e44 4546 4155 4c54  self.cfg.DEFAULT
-000066e0: 5320 7c20 7b6b 6579 3a20 7661 6c7d 0d0a  S | {key: val}..
-000066f0: 0d0a 2020 2020 6465 6620 7072 6f64 7563  ..    def produc
-00006700: 745f 6772 6964 2873 656c 6629 3a0d 0a20  t_grid(self):.. 
-00006710: 2020 2020 2020 2022 2222 4772 6964 2073         """Grid s
-00006720: 6561 7263 6820 6163 726f 7373 2061 6c6c  earch across all
-00006730: 2063 6f6d 6269 6e61 7469 6f6e 206f 6620   combination of 
-00006740: 7061 7261 6d73 2222 220d 0a20 2020 2020  params"""..     
-00006750: 2020 2066 6f72 2076 616c 7320 696e 2070     for vals in p
-00006760: 726f 6475 6374 282a 7365 6c66 2e76 616c  roduct(*self.val
-00006770: 7565 7329 3a0d 0a20 2020 2020 2020 2020  ues):..         
-00006780: 2020 2079 6965 6c64 2073 656c 662e 6366     yield self.cf
-00006790: 672e 4445 4641 554c 5453 207c 207b 6f70  g.DEFAULTS | {op
-000067a0: 7469 6f6e 3a76 616c 2066 6f72 206f 7074  tion:val for opt
-000067b0: 696f 6e2c 2076 616c 2069 6e20 7a69 7028  ion, val in zip(
-000067c0: 7365 6c66 2e70 6172 616d 732c 2076 616c  self.params, val
-000067d0: 7329 7d0d 0a0d 0a20 2020 2064 6566 2073  s)}....    def s
-000067e0: 6176 655f 6368 6563 6b70 6f69 6e74 2873  ave_checkpoint(s
-000067f0: 656c 662c 2073 6f75 7263 653a 204c 6973  elf, source: Lis
-00006800: 7429 202d 3e20 4e6f 6e65 3a0d 0a20 2020  t) -> None:..   
-00006810: 2020 2020 2022 2222 5361 7665 2074 6865       """Save the
-00006820: 2072 6573 7420 6f66 2070 6172 616d 732e   rest of params.
-00006830: 2222 220d 0a20 2020 2020 2020 2070 6174  """..        pat
-00006840: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
-00006850: 2873 656c 662e 6366 672e 434f 5245 5f43  (self.cfg.CORE_C
-00006860: 4845 434b 504f 494e 545f 5041 5448 2c20  HECKPOINT_PATH, 
-00006870: 7365 6c66 2e63 6667 2e43 4845 434b 504f  self.cfg.CHECKPO
-00006880: 494e 545f 4649 4c45 4e41 4d45 290d 0a20  INT_FILENAME).. 
-00006890: 2020 2020 2020 2063 6865 636b 706f 696e         checkpoin
-000068a0: 7420 3d20 6469 6374 2829 0d0a 2020 2020  t = dict()..    
-000068b0: 2020 2020 6368 6563 6b70 6f69 6e74 5b27      checkpoint['
-000068c0: 736f 7572 6365 275d 203d 2073 6f75 7263  source'] = sourc
-000068d0: 650d 0a20 2020 2020 2020 2074 6f72 6368  e..        torch
-000068e0: 2e73 6176 6528 6368 6563 6b70 6f69 6e74  .save(checkpoint
-000068f0: 2c20 7061 7468 290d 0a0d 0a20 2020 2064  , path)....    d
-00006900: 6566 206c 6f61 645f 6368 6563 6b70 6f69  ef load_checkpoi
-00006910: 6e74 2873 656c 6629 202d 3e20 696e 743a  nt(self) -> int:
-00006920: 0d0a 2020 2020 2020 2020 2222 224c 6f61  ..        """Loa
-00006930: 6420 7468 6520 7265 7374 206f 6620 7061  d the rest of pa
-00006940: 7261 6d73 2e22 2222 0d0a 2020 2020 2020  rams."""..      
-00006950: 2020 7061 7468 203d 206f 732e 7061 7468    path = os.path
-00006960: 2e6a 6f69 6e28 7365 6c66 2e63 6667 2e43  .join(self.cfg.C
-00006970: 4f52 455f 4348 4543 4b50 4f49 4e54 5f50  ORE_CHECKPOINT_P
-00006980: 4154 482c 2073 656c 662e 6366 672e 4348  ATH, self.cfg.CH
-00006990: 4543 4b50 4f49 4e54 5f46 494c 454e 414d  ECKPOINT_FILENAM
-000069a0: 4529 0d0a 2020 2020 2020 2020 6368 6563  E)..        chec
-000069b0: 6b70 6f69 6e74 203d 2074 6f72 6368 2e6c  kpoint = torch.l
-000069c0: 6f61 6428 7061 7468 290d 0a20 2020 2020  oad(path)..     
-000069d0: 2020 2072 6574 7572 6e20 6368 6563 6b70     return checkp
-000069e0: 6f69 6e74 5b27 736f 7572 6365 275d 0d0a  oint['source']..
-000069f0: 0d0a 2020 2020 4074 696d 656d 6574 6572  ..    @timemeter
-00006a00: 2822 436f 6163 682f 7265 7375 6d65 2229  ("Coach/resume")
-00006a10: 0d0a 2020 2020 6465 6620 7265 7375 6d65  ..    def resume
-00006a20: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00006a30: 2022 2222 5265 7375 6d65 2066 726f 6d20   """Resume from 
-00006a40: 7468 6520 7265 6365 6e74 2063 6865 636b  the recent check
-00006a50: 706f 696e 742e 2222 220d 0a20 2020 2020  point."""..     
-00006a60: 2020 2073 6f75 7263 6520 3d20 7365 6c66     source = self
-00006a70: 2e65 6163 685f 6772 6964 2829 2069 6620  .each_grid() if 
-00006a80: 7365 6c66 2e63 6667 2e45 5843 4c55 5349  self.cfg.EXCLUSI
-00006a90: 5645 2065 6c73 6520 7365 6c66 2e70 726f  VE else self.pro
-00006aa0: 6475 6374 5f67 7269 6428 290d 0a20 2020  duct_grid()..   
-00006ab0: 2020 2020 2073 6f75 7263 6520 3d20 6c69       source = li
-00006ac0: 7374 2873 6f75 7263 6529 5b3a 3a2d 315d  st(source)[::-1]
-00006ad0: 0d0a 2020 2020 2020 2020 736f 7572 6365  ..        source
-00006ae0: 203d 2073 656c 662e 6c6f 6164 5f63 6865   = self.load_che
-00006af0: 636b 706f 696e 7428 2920 6966 2073 656c  ckpoint() if sel
-00006b00: 662e 6366 672e 7265 7375 6d65 2065 6c73  f.cfg.resume els
-00006b10: 6520 736f 7572 6365 0d0a 2020 2020 2020  e source..      
-00006b20: 2020 696e 666f 4c6f 6767 6572 2866 225b    infoLogger(f"[
-00006b30: 436f 6163 685d 203e 3e3e 204c 6f61 6420  Coach] >>> Load 
-00006b40: 7468 6520 7265 6365 6e74 2063 6865 636b  the recent check
-00006b50: 706f 696e 7420 2e2e 2e22 290d 0a20 2020  point ...")..   
-00006b60: 2020 2020 2072 6574 7572 6e20 736f 7572       return sour
-00006b70: 6365 0d0a 0d0a 2020 2020 6465 6620 7275  ce....    def ru
-00006b80: 6e28 7365 6c66 2c20 636f 6d6d 616e 643a  n(self, command:
-00006b90: 2073 7472 2c20 7061 7261 6d73 3a20 4469   str, params: Di
-00006ba0: 6374 293a 0d0a 2020 2020 2020 2020 2222  ct):..        ""
-00006bb0: 2253 7461 7274 2061 206e 6577 2073 7562  "Start a new sub
-00006bc0: 7072 6f63 6573 7322 2222 0d0a 2020 2020  process"""..    
-00006bd0: 2020 2020 666f 7220 6f70 7469 6f6e 2c20      for option, 
-00006be0: 7661 6c20 696e 2070 6172 616d 732e 6974  val in params.it
-00006bf0: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
-00006c00: 2020 2020 636f 6d6d 616e 6420 2b3d 2073      command += s
-00006c10: 656c 662e 6765 745f 6f70 7469 6f6e 286f  elf.get_option(o
-00006c20: 7074 696f 6e2c 2076 616c 290d 0a20 2020  ption, val)..   
-00006c30: 2020 2020 2069 6e66 6f4c 6f67 6765 7228       infoLogger(
-00006c40: 6622 5c30 3333 5b30 3b33 313b 3437 6d7b  f"\033[0;31;47m{
-00006c50: 636f 6d6d 616e 647d 5c30 3333 5b30 6d22  command}\033[0m"
-00006c60: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00006c70: 6e20 7375 6270 726f 6365 7373 2e50 6f70  n subprocess.Pop
-00006c80: 656e 2873 686c 6578 2e73 706c 6974 2863  en(shlex.split(c
-00006c90: 6f6d 6d61 6e64 2929 0d0a 0d0a 2020 2020  ommand))....    
-00006ca0: 6465 6620 7761 6974 2873 656c 662c 2074  def wait(self, t
-00006cb0: 6173 6b73 3a20 4469 6374 293a 0d0a 2020  asks: Dict):..  
-00006cc0: 2020 2020 2020 2222 2257 6169 7420 7574        """Wait ut
-00006cd0: 696c 2061 6c6c 2070 726f 6365 7373 6573  il all processes
-00006ce0: 2074 6572 6d69 6e61 7465 2e22 2222 0d0a   terminate."""..
-00006cf0: 2020 2020 2020 2020 666f 7220 7072 6f63          for proc
-00006d00: 6573 735f 2c20 6964 5f2c 206c 6f67 5061  ess_, id_, logPa
-00006d10: 7468 2c20 7061 7261 6d73 2069 6e20 7461  th, params in ta
-00006d20: 736b 732e 7661 6c75 6573 2829 3a0d 0a20  sks.values():.. 
-00006d30: 2020 2020 2020 2020 2020 2070 726f 6365             proce
-00006d40: 7373 5f2e 7761 6974 2829 0d0a 2020 2020  ss_.wait()..    
-00006d50: 2020 2020 2020 2020 7365 6c66 2e77 7269          self.wri
-00006d60: 7465 2869 645f 2c20 6c6f 6750 6174 682c  te(id_, logPath,
-00006d70: 2070 6172 616d 7329 0d0a 0d0a 2020 2020   params)....    
-00006d80: 6465 6620 706f 6c6c 2873 656c 662c 2074  def poll(self, t
-00006d90: 6173 6b73 3a20 4469 6374 293a 0d0a 2020  asks: Dict):..  
-00006da0: 2020 2020 2020 2222 2257 6169 7420 7574        """Wait ut
-00006db0: 696c 2061 6e79 2070 726f 6365 7373 2074  il any process t
-00006dc0: 6572 6d69 6e61 7465 732e 2222 220d 0a20  erminates.""".. 
-00006dd0: 2020 2020 2020 2062 7566 6665 725f 736f         buffer_so
-00006de0: 7572 6365 203d 205b 5d0d 0a20 2020 2020  urce = []..     
-00006df0: 2020 2074 696d 652e 736c 6565 7028 3129     time.sleep(1)
-00006e00: 2023 2066 6f72 2075 6e69 7175 6520 6964   # for unique id
-00006e10: 0d0a 2020 2020 2020 2020 7768 696c 6520  ..        while 
-00006e20: 6c65 6e28 7365 6c66 2e64 6576 6963 6573  len(self.devices
-00006e30: 2920 3d3d 2030 3a0d 0a20 2020 2020 2020  ) == 0:..       
-00006e40: 2020 2020 2074 696d 652e 736c 6565 7028       time.sleep(
-00006e50: 3729 0d0a 2020 2020 2020 2020 2020 2020  7)..            
-00006e60: 666f 7220 6465 7669 6365 2c20 2870 726f  for device, (pro
-00006e70: 6365 7373 5f2c 2069 645f 2c20 6c6f 6750  cess_, id_, logP
-00006e80: 6174 682c 2070 6172 616d 7329 2069 6e20  ath, params) in 
-00006e90: 7461 736b 732e 6974 656d 7328 293a 0d0a  tasks.items():..
-00006ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006eb0: 6966 2070 726f 6365 7373 5f2e 706f 6c6c  if process_.poll
-00006ec0: 2829 2069 7320 6e6f 7420 4e6f 6e65 3a0d  () is not None:.
-00006ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006ee0: 2020 2020 2073 656c 662e 7772 6974 6528       self.write(
-00006ef0: 6964 5f2c 206c 6f67 5061 7468 2c20 7061  id_, logPath, pa
-00006f00: 7261 6d73 290d 0a20 2020 2020 2020 2020  rams)..         
-00006f10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006f20: 6465 7669 6365 732e 6170 7065 6e64 2864  devices.append(d
-00006f30: 6576 6963 6529 0d0a 2020 2020 2020 2020  evice)..        
-00006f40: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00006f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f60: 2020 2062 7566 6665 725f 736f 7572 6365     buffer_source
-00006f70: 2e61 7070 656e 6428 7061 7261 6d73 290d  .append(params).
-00006f80: 0a20 2020 2020 2020 2073 656c 662e 7361  .        self.sa
-00006f90: 7665 5f63 6865 636b 706f 696e 7428 7365  ve_checkpoint(se
-00006fa0: 6c66 2e73 6f75 7263 6520 2b20 6275 6666  lf.source + buff
-00006fb0: 6572 5f73 6f75 7263 6529 0d0a 0d0a 2020  er_source)....  
-00006fc0: 2020 4074 696d 656d 6574 6572 2822 4164    @timemeter("Ad
-00006fd0: 6170 7465 722f 6669 7422 290d 0a20 2020  apter/fit")..   
-00006fe0: 2064 6566 2066 6974 2873 656c 6629 3a0d   def fit(self):.
-00006ff0: 0a20 2020 2020 2020 2022 2222 4772 6964  .        """Grid
-00007000: 2073 6561 7263 682e 2222 220d 0a20 2020   search."""..   
-00007010: 2020 2020 2073 656c 662e 736f 7572 6365       self.source
-00007020: 203d 2073 656c 662e 7265 7375 6d65 2829   = self.resume()
-00007030: 0d0a 2020 2020 2020 2020 7461 736b 7320  ..        tasks 
-00007040: 3d20 6469 6374 2829 0d0a 2020 2020 2020  = dict()..      
-00007050: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-00007060: 2020 2020 7768 696c 6520 7365 6c66 2e73      while self.s
-00007070: 6f75 7263 653a 0d0a 2020 2020 2020 2020  ource:..        
-00007080: 2020 2020 2020 2020 7365 6c66 2e70 6f6c          self.pol
-00007090: 6c28 7461 736b 7329 0d0a 2020 2020 2020  l(tasks)..      
-000070a0: 2020 2020 2020 2020 2020 7061 7261 6d73            params
-000070b0: 203d 2073 656c 662e 736f 7572 6365 2e70   = self.source.p
-000070c0: 6f70 2829 0d0a 2020 2020 2020 2020 2020  op()..          
-000070d0: 2020 2020 2020 6465 7669 6365 203d 2073        device = s
-000070e0: 656c 662e 6465 7669 6365 732e 706f 7028  elf.devices.pop(
-000070f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00007100: 2020 2063 6f6d 6d61 6e64 2c20 6964 5f2c     command, id_,
-00007110: 206c 6f67 5061 7468 203d 2073 656c 662e   logPath = self.
-00007120: 7265 6769 7374 6572 2864 6576 6963 6529  register(device)
-00007130: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007140: 2020 7072 6f63 6573 735f 203d 2073 656c    process_ = sel
-00007150: 662e 7275 6e28 636f 6d6d 616e 642c 2070  f.run(command, p
-00007160: 6172 616d 7329 0d0a 2020 2020 2020 2020  arams)..        
-00007170: 2020 2020 2020 2020 7461 736b 735b 6465          tasks[de
-00007180: 7669 6365 5d20 3d20 2870 726f 6365 7373  vice] = (process
-00007190: 5f2c 2069 645f 2c20 6c6f 6750 6174 682c  _, id_, logPath,
-000071a0: 2070 6172 616d 7329 0d0a 2020 2020 2020   params)..      
-000071b0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-000071c0: 6f6e 2061 7320 653a 0d0a 2020 2020 2020  on as e:..      
-000071d0: 2020 2020 2020 7072 696e 7428 6529 0d0a        print(e)..
-000071e0: 2020 2020 2020 2020 6669 6e61 6c6c 793a          finally:
-000071f0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00007200: 6c66 2e77 6169 7428 7461 736b 7329 0d0a  lf.wait(tasks)..
-00007210: 2020 2020 2020 2020 2020 2020 7379 732e              sys.
-00007220: 6578 6974 2829                           exit()
+00000080: 7469 6d65 2c20 7379 732c 2073 6967 6e61  time, sys, signa
+00000090: 6c2c 2070 7375 7469 6c2c 2061 7465 7869  l, psutil, atexi
+000000a0: 740d 0a69 6d70 6f72 7420 7061 6e64 6173  t..import pandas
+000000b0: 2061 7320 7064 0d0a 6672 6f6d 2074 6f72   as pd..from tor
+000000c0: 6368 6461 7461 2e64 6174 6170 6970 6573  chdata.datapipes
+000000d0: 2e69 7465 7220 696d 706f 7274 2049 7465  .iter import Ite
+000000e0: 7244 6174 6150 6970 650d 0a66 726f 6d20  rDataPipe..from 
+000000f0: 746f 7263 682e 7574 696c 732e 7465 6e73  torch.utils.tens
+00000100: 6f72 626f 6172 6420 696d 706f 7274 2053  orboard import S
+00000110: 756d 6d61 7279 5772 6974 6572 0d0a 6672  ummaryWriter..fr
+00000120: 6f6d 2066 756e 6374 6f6f 6c73 2069 6d70  om functools imp
+00000130: 6f72 7420 7061 7274 6961 6c0d 0a66 726f  ort partial..fro
+00000140: 6d20 6974 6572 746f 6f6c 7320 696d 706f  m itertools impo
+00000150: 7274 2070 726f 6475 6374 0d0a 6672 6f6d  rt product..from
+00000160: 2063 6f6c 6c65 6374 696f 6e73 2069 6d70   collections imp
+00000170: 6f72 7420 6465 6661 756c 7464 6963 740d  ort defaultdict.
+00000180: 0a66 726f 6d20 6672 6565 706c 6f74 2e75  .from freeplot.u
+00000190: 7469 6c73 2069 6d70 6f72 7420 696d 706f  tils import impo
+000001a0: 7274 5f70 6963 6b6c 652c 2065 7870 6f72  rt_pickle, expor
+000001b0: 745f 7069 636b 6c65 0d0a 0d0a 6672 6f6d  t_pickle....from
+000001c0: 202e 6461 7461 2e66 6965 6c64 7320 696d   .data.fields im
+000001d0: 706f 7274 2046 6965 6c64 4d6f 6475 6c65  port FieldModule
+000001e0: 2c20 4669 656c 6454 7570 6c65 0d0a 6672  , FieldTuple..fr
+000001f0: 6f6d 202e 6461 7461 2e64 6174 616c 6f61  om .data.dataloa
+00000200: 6465 7220 696d 706f 7274 2044 6174 614c  der import DataL
+00000210: 6f61 6465 720d 0a66 726f 6d20 2e6d 6f64  oader..from .mod
+00000220: 656c 7320 696d 706f 7274 2052 6563 5379  els import RecSy
+00000230: 7341 7263 680d 0a66 726f 6d20 2e63 7269  sArch..from .cri
+00000240: 7465 7269 6f6e 7320 696d 706f 7274 2042  terions import B
+00000250: 6173 6543 7269 7465 7269 6f6e 0d0a 6672  aseCriterion..fr
+00000260: 6f6d 202e 6469 6374 326f 626a 2069 6d70  om .dict2obj imp
+00000270: 6f72 7420 436f 6e66 6967 0d0a 6672 6f6d  ort Config..from
+00000280: 202e 7574 696c 7320 696d 706f 7274 2041   .utils import A
+00000290: 7665 7261 6765 4d65 7465 722c 204d 6f6e  verageMeter, Mon
+000002a0: 6974 6f72 2c20 7469 6d65 6d65 7465 722c  itor, timemeter,
+000002b0: 2069 6e66 6f4c 6f67 6765 720d 0a66 726f   infoLogger..fro
+000002c0: 6d20 2e6d 6574 7269 6373 2069 6d70 6f72  m .metrics impor
+000002d0: 7420 2a0d 0a66 726f 6d20 2e70 6172 7365  t *..from .parse
+000002e0: 7220 696d 706f 7274 2054 494d 450d 0a0d  r import TIME...
+000002f0: 0a0d 0a5f 5f61 6c6c 5f5f 203d 205b 2743  ...__all__ = ['C
+00000300: 6869 6566 436f 6163 6827 2c20 2743 6f61  hiefCoach', 'Coa
+00000310: 6368 272c 2027 4164 6170 7465 7227 5d0d  ch', 'Adapter'].
+00000320: 0a0d 0a0d 0a44 4546 4155 4c54 5f4d 4554  .....DEFAULT_MET
+00000330: 5249 4353 203d 207b 0d0a 2020 2020 274c  RICS = {..    'L
+00000340: 4f53 5327 3a20 6c61 6d62 6461 2078 3a20  OSS': lambda x: 
+00000350: 782c 0d0a 2020 2020 2323 2323 2323 2323  x,..    ########
+00000360: 2323 2323 230d 0a20 2020 2027 4d53 4527  #####..    'MSE'
+00000370: 3a20 6d65 616e 5f73 7175 6172 6564 5f65  : mean_squared_e
+00000380: 7272 6f72 2c0d 0a20 2020 2027 4d41 4527  rror,..    'MAE'
+00000390: 3a20 6d65 616e 5f61 6273 5f65 7272 6f72  : mean_abs_error
+000003a0: 2c0d 0a20 2020 2027 524d 5345 273a 2072  ,..    'RMSE': r
+000003b0: 6f6f 745f 6d73 652c 0d0a 2020 2020 2323  oot_mse,..    ##
+000003c0: 2323 2323 2323 2323 2323 230d 0a20 2020  ###########..   
+000003d0: 2027 5052 4543 4953 494f 4e27 3a20 7072   'PRECISION': pr
+000003e0: 6563 6973 696f 6e2c 0d0a 2020 2020 2752  ecision,..    'R
+000003f0: 4543 414c 4c27 3a20 7265 6361 6c6c 2c0d  ECALL': recall,.
+00000400: 0a20 2020 2027 4631 273a 2066 315f 7363  .    'F1': f1_sc
+00000410: 6f72 652c 0d0a 2020 2020 2741 5543 273a  ore,..    'AUC':
+00000420: 2061 7572 6f63 2c0d 0a20 2020 2027 4849   auroc,..    'HI
+00000430: 5452 4154 4527 3a20 6869 745f 7261 7465  TRATE': hit_rate
+00000440: 2c0d 0a20 2020 2023 2323 2323 2323 2323  ,..    #########
+00000450: 2323 2323 0d0a 2020 2020 274e 4443 4727  ####..    'NDCG'
+00000460: 3a20 6e6f 726d 616c 697a 6564 5f64 6367  : normalized_dcg
+00000470: 2c0d 0a20 2020 2027 4d52 5227 3a20 6d65  ,..    'MRR': me
+00000480: 616e 5f72 6563 6970 726f 6361 6c5f 7261  an_reciprocal_ra
+00000490: 6e6b 2c0d 0a20 2020 2027 4d41 5027 3a20  nk,..    'MAP': 
+000004a0: 6d65 616e 5f61 7665 7261 6765 5f70 7265  mean_average_pre
+000004b0: 6369 7369 6f6e 0d0a 7d0d 0a0d 0a44 4546  cision..}....DEF
+000004c0: 4155 4c54 5f46 4d54 5320 3d20 7b0d 0a20  AULT_FMTS = {.. 
+000004d0: 2020 2027 4c4f 5353 273a 2022 2e35 6622     'LOSS': ".5f"
+000004e0: 2c0d 0a20 2020 2023 2323 2323 2323 2323  ,..    #########
+000004f0: 2323 2323 0d0a 2020 2020 274d 5345 273a  ####..    'MSE':
+00000500: 2022 2e34 6622 2c0d 0a20 2020 2027 4d41   ".4f",..    'MA
+00000510: 4527 3a20 222e 3466 222c 0d0a 2020 2020  E': ".4f",..    
+00000520: 2752 4d53 4527 3a20 222e 3466 222c 0d0a  'RMSE': ".4f",..
+00000530: 2020 2020 2323 2323 2323 2323 2323 2323      ############
+00000540: 230d 0a20 2020 2027 5052 4543 4953 494f  #..    'PRECISIO
+00000550: 4e27 3a20 222e 3466 222c 0d0a 2020 2020  N': ".4f",..    
+00000560: 2752 4543 414c 4c27 3a20 222e 3466 222c  'RECALL': ".4f",
+00000570: 0d0a 2020 2020 2746 3127 3a20 222e 3466  ..    'F1': ".4f
+00000580: 222c 0d0a 2020 2020 2741 5543 273a 2022  ",..    'AUC': "
+00000590: 2e34 6622 2c0d 0a20 2020 2027 4849 5452  .4f",..    'HITR
+000005a0: 4154 4527 3a20 222e 3466 222c 0d0a 2020  ATE': ".4f",..  
+000005b0: 2020 2323 2323 2323 2323 2323 2323 230d    #############.
+000005c0: 0a20 2020 2027 4e44 4347 273a 2022 2e34  .    'NDCG': ".4
+000005d0: 6622 2c0d 0a20 2020 2027 4d52 5227 3a20  f",..    'MRR': 
+000005e0: 222e 3466 222c 0d0a 2020 2020 274d 4150  ".4f",..    'MAP
+000005f0: 273a 2022 2e34 6622 2c0d 0a7d 0d0a 0d0a  ': ".4f",..}....
+00000600: 4445 4641 554c 545f 4245 5354 5f43 4153  DEFAULT_BEST_CAS
+00000610: 5445 5220 3d20 7b0d 0a20 2020 2027 4c4f  TER = {..    'LO
+00000620: 5353 273a 206d 696e 2c0d 0a20 2020 2023  SS': min,..    #
+00000630: 2323 2323 2323 2323 2323 2323 0d0a 2020  ############..  
+00000640: 2020 274d 5345 273a 206d 696e 2c0d 0a20    'MSE': min,.. 
+00000650: 2020 2027 4d41 4527 3a20 6d69 6e2c 0d0a     'MAE': min,..
+00000660: 2020 2020 2752 4d53 4527 3a20 6d69 6e2c      'RMSE': min,
+00000670: 0d0a 2020 2020 2323 2323 2323 2323 2323  ..    ##########
+00000680: 2323 230d 0a20 2020 2027 5052 4543 4953  ###..    'PRECIS
+00000690: 494f 4e27 3a20 6d61 782c 0d0a 2020 2020  ION': max,..    
+000006a0: 2752 4543 414c 4c27 3a20 6d61 782c 0d0a  'RECALL': max,..
+000006b0: 2020 2020 2746 3127 3a20 6d61 782c 0d0a      'F1': max,..
+000006c0: 2020 2020 2741 5543 273a 206d 6178 2c0d      'AUC': max,.
+000006d0: 0a20 2020 2027 4849 5452 4154 4527 3a20  .    'HITRATE': 
+000006e0: 6d61 782c 0d0a 2020 2020 2323 2323 2323  max,..    ######
+000006f0: 2323 2323 2323 230d 0a20 2020 2027 4e44  #######..    'ND
+00000700: 4347 273a 206d 6178 2c0d 0a20 2020 2027  CG': max,..    '
+00000710: 4d52 5227 3a20 6d61 782c 0d0a 2020 2020  MRR': max,..    
+00000720: 274d 4150 273a 206d 6178 2c0d 0a7d 0d0a  'MAP': max,..}..
+00000730: 0d0a 0d0a 636c 6173 7320 5f44 756d 6d79  ....class _Dummy
+00000740: 4d6f 6475 6c65 2874 6f72 6368 2e6e 6e2e  Module(torch.nn.
+00000750: 4d6f 6475 6c65 293a 0d0a 2020 2020 2222  Module):..    ""
+00000760: 2254 6869 7320 6973 2061 2064 756d 6d79  "This is a dummy
+00000770: 206d 6f64 756c 6520 7468 6174 2073 6572   module that ser
+00000780: 7665 7320 6173 2061 2070 6c61 6365 686f  ves as a placeho
+00000790: 6c64 6572 2066 6f72 2061 2072 6561 6c20  lder for a real 
+000007a0: 6d6f 6465 6c2e 2222 220d 0a20 2020 2064  model."""..    d
+000007b0: 6566 2066 6f72 7761 7264 2873 656c 662c  ef forward(self,
+000007c0: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
+000007d0: 293a 0d0a 2020 2020 2020 2020 2222 2244  ):..        """D
+000007e0: 756d 6d79 2066 6f72 7761 7264 206d 6574  ummy forward met
+000007f0: 686f 6420 7468 6174 2072 6169 7365 7320  hod that raises 
+00000800: 6120 604e 6f74 496d 706c 656d 656e 7465  a `NotImplemente
+00000810: 6445 7272 6f72 602e 2222 220d 0a20 2020  dError`."""..   
+00000820: 2020 2020 2072 6169 7365 204e 6f74 496d       raise NotIm
+00000830: 706c 656d 656e 7465 6445 7272 6f72 2822  plementedError("
+00000840: 4e6f 206d 6f64 656c 2061 7661 696c 6162  No model availab
+00000850: 6c65 2066 6f72 2043 6f61 6368 202e 2e2e  le for Coach ...
+00000860: 2229 0d0a 0d0a 2020 2020 6465 6620 7374  ")....    def st
+00000870: 6570 2873 656c 662c 202a 6172 6773 2c20  ep(self, *args, 
+00000880: 2a2a 6b77 6172 6773 293a 0d0a 2020 2020  **kwargs):..    
+00000890: 2020 2020 2222 2244 756d 6d79 2073 7465      """Dummy ste
+000008a0: 7020 6d65 7468 6f64 2074 6861 7420 7261  p method that ra
+000008b0: 6973 6573 2061 2060 4e6f 7449 6d70 6c65  ises a `NotImple
+000008c0: 6d65 6e74 6564 4572 726f 7260 2e22 2222  mentedError`."""
+000008d0: 0d0a 2020 2020 2020 2020 7261 6973 6520  ..        raise 
+000008e0: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+000008f0: 726f 7228 224e 6f20 6f70 7469 6d69 7a65  ror("No optimize
+00000900: 7220 6f72 206c 7220 7363 6865 6475 6c65  r or lr schedule
+00000910: 7220 6176 6169 6c61 626c 6520 666f 7220  r available for 
+00000920: 436f 6163 6820 2e2e 2e22 290d 0a0d 0a20  Coach ...").... 
+00000930: 2020 2064 6566 2062 6163 6b77 6172 6428     def backward(
+00000940: 7365 6c66 2c20 2a61 7267 732c 202a 2a6b  self, *args, **k
+00000950: 7761 7267 7329 3a0d 0a20 2020 2020 2020  wargs):..       
+00000960: 2022 2222 4475 6d6d 7920 6261 636b 7761   """Dummy backwa
+00000970: 7264 206d 6574 686f 6420 7468 6174 2072  rd method that r
+00000980: 6169 7365 7320 6120 604e 6f74 496d 706c  aises a `NotImpl
+00000990: 656d 656e 7465 6445 7272 6f72 602e 2222  ementedError`.""
+000009a0: 220d 0a20 2020 2020 2020 2072 6169 7365  "..        raise
+000009b0: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
+000009c0: 7272 6f72 2822 4e6f 206f 7074 696d 697a  rror("No optimiz
+000009d0: 6572 2061 7661 696c 6162 6c65 2066 6f72  er available for
+000009e0: 2043 6f61 6368 202e 2e2e 2229 0d0a 0d0a   Coach ...")....
+000009f0: 0d0a 636c 6173 7320 4368 6965 6643 6f61  ..class ChiefCoa
+00000a00: 6368 286d 6574 6163 6c61 7373 3d61 6263  ch(metaclass=abc
+00000a10: 2e41 4243 4d65 7461 293a 0d0a 2020 2020  .ABCMeta):..    
+00000a20: 7222 2222 200d 0a20 2020 2054 6865 2060  r""" ..    The `
+00000a30: 4368 6965 6643 6f61 6368 6020 636c 6173  ChiefCoach` clas
+00000a40: 7320 6973 2074 6865 2074 6f70 2d6c 6576  s is the top-lev
+00000a50: 656c 2063 6c61 7373 2066 6f72 2072 756e  el class for run
+00000a60: 6e69 6e67 2074 6865 2074 7261 696e 696e  ning the trainin
+00000a70: 6720 616e 6420 6576 616c 7561 7469 6f6e  g and evaluation
+00000a80: 206c 6f6f 7073 2e0d 0a0d 0a20 2020 2050   loops.....    P
+00000a90: 6172 616d 6574 6572 733a 0d0a 2020 2020  arameters:..    
+00000aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020  -----------..   
+00000ab0: 2074 7261 696e 7069 7065 203a 2049 7465   trainpipe : Ite
+00000ac0: 7244 6174 6150 6970 650d 0a20 2020 2020  rDataPipe..     
+00000ad0: 2020 2049 7465 7261 626c 6520 6461 7461     Iterable data
+00000ae0: 2070 6970 656c 696e 6520 666f 7220 7472   pipeline for tr
+00000af0: 6169 6e69 6e67 2064 6174 612e 0d0a 2020  aining data...  
+00000b00: 2020 7661 6c69 6470 6970 6520 3a20 4974    validpipe : It
+00000b10: 6572 4461 7461 5069 7065 2c20 6f70 7469  erDataPipe, opti
+00000b20: 6f6e 616c 0d0a 2020 2020 2020 2020 4974  onal..        It
+00000b30: 6572 6162 6c65 2064 6174 6120 7069 7065  erable data pipe
+00000b40: 6c69 6e65 2066 6f72 2076 616c 6964 6174  line for validat
+00000b50: 696f 6e20 6461 7461 2e0d 0a20 2020 2020  ion data...     
+00000b60: 2020 2049 6620 604e 6f6e 6560 2c20 7573     If `None`, us
+00000b70: 6520 6074 7261 696e 7069 7065 6020 696e  e `trainpipe` in
+00000b80: 7374 6561 642e 0d0a 2020 2020 7465 7374  stead...    test
+00000b90: 7069 7065 203a 2049 7465 7244 6174 6150  pipe : IterDataP
+00000ba0: 6970 652c 206f 7074 696f 6e61 6c0d 0a20  ipe, optional.. 
+00000bb0: 2020 2020 2020 2049 7465 7261 626c 6520         Iterable 
+00000bc0: 6461 7461 2070 6970 656c 696e 6520 666f  data pipeline fo
+00000bd0: 7220 7465 7374 696e 6720 6461 7461 2e0d  r testing data..
+00000be0: 0a20 2020 2020 2020 2049 6620 604e 6f6e  .        If `Non
+00000bf0: 6560 2c20 7573 6520 6076 616c 6964 7069  e`, use `validpi
+00000c00: 7065 6020 696e 7374 6561 642e 0d0a 2020  pe` instead...  
+00000c10: 2020 6669 656c 6473 203a 2049 7465 7261    fields : Itera
+00000c20: 626c 655b 4669 656c 644d 6f64 756c 655d  ble[FieldModule]
+00000c30: 0d0a 2020 2020 2020 2020 5475 706c 6520  ..        Tuple 
+00000c40: 6f66 2060 4669 656c 644d 6f64 756c 6560  of `FieldModule`
+00000c50: 7320 666f 7220 6461 7461 7365 7420 6669  s for dataset fi
+00000c60: 656c 6473 2e0d 0a20 2020 206d 6f64 656c  elds...    model
+00000c70: 203a 2055 6e69 6f6e 5b52 6563 5379 7341   : Union[RecSysA
+00000c80: 7263 682c 2074 6f72 6368 2e6e 6e2e 4d6f  rch, torch.nn.Mo
+00000c90: 6475 6c65 2c20 4e6f 6e65 5d0d 0a20 2020  dule, None]..   
+00000ca0: 2020 2020 204d 6f64 656c 2066 6f72 2074       Model for t
+00000cb0: 7261 696e 696e 6720 616e 6420 6576 616c  raining and eval
+00000cc0: 7561 7469 6e67 2e20 0d0a 2020 2020 2020  uating. ..      
+00000cd0: 2020 4966 2060 4e6f 6e65 602c 2075 7365    If `None`, use
+00000ce0: 205f 4475 6d6d 794d 6f64 756c 6520 696e   _DummyModule in
+00000cf0: 7374 6561 642c 2077 6869 6368 2073 686f  stead, which sho
+00000d00: 756c 6420 6e6f 7420 6361 6c6c 2060 666f  uld not call `fo
+00000d10: 7277 6172 6460 2e0d 0a20 2020 2063 7269  rward`...    cri
+00000d20: 7465 7269 6f6e 203a 2055 6e69 6f6e 5b42  terion : Union[B
+00000d30: 6173 6543 7269 7465 7269 6f6e 2c20 4361  aseCriterion, Ca
+00000d40: 6c6c 6162 6c65 5d0d 0a20 2020 2020 2020  llable]..       
+00000d50: 2043 616c 6c61 626c 6520 666f 7220 636f   Callable for co
+00000d60: 6d70 7574 696e 6720 7468 6520 6c6f 7373  mputing the loss
+00000d70: 2066 756e 6374 696f 6e2e 0d0a 2020 2020   function...    
+00000d80: 6f70 7469 6d69 7a65 7220 3a20 746f 7263  optimizer : torc
+00000d90: 682e 6f70 7469 6d2e 4f70 7469 6d69 7a65  h.optim.Optimize
+00000da0: 722c 206f 7074 696f 6e61 6c0d 0a20 2020  r, optional..   
+00000db0: 2020 2020 204f 7074 696d 697a 6572 2066       Optimizer f
+00000dc0: 6f72 2075 7064 6174 696e 6720 6d6f 6465  or updating mode
+00000dd0: 6c20 7061 7261 6d65 7465 7273 2e20 0d0a  l parameters. ..
+00000de0: 2020 2020 2020 2020 4966 2060 4e6f 6e65          If `None
+00000df0: 602c 2075 7365 205f 4475 6d6d 794d 6f64  `, use _DummyMod
+00000e00: 756c 6520 696e 7374 6561 642c 2077 6869  ule instead, whi
+00000e10: 6368 2073 686f 756c 6420 6e6f 7420 6361  ch should not ca
+00000e20: 6c6c 2060 7374 6570 6020 616e 6420 6062  ll `step` and `b
+00000e30: 6163 6b77 6172 6460 2e0d 0a20 2020 206c  ackward`...    l
+00000e40: 725f 7363 6865 6475 6c65 7220 3a20 746f  r_scheduler : to
+00000e50: 7263 682e 6f70 7469 6d2e 6c72 5f73 6368  rch.optim.lr_sch
+00000e60: 6564 756c 6572 2e5f 4c52 5363 6865 6475  eduler._LRSchedu
+00000e70: 6c65 722c 206f 7074 696f 6e61 6c0d 0a20  ler, optional.. 
+00000e80: 2020 2020 2020 204c 6561 726e 696e 6720         Learning 
+00000e90: 7261 7465 2073 6368 6564 756c 6572 2e20  rate scheduler. 
+00000ea0: 4966 2060 4e6f 6e65 602c 2075 7365 205f  If `None`, use _
+00000eb0: 4475 6d6d 794d 6f64 756c 6520 696e 7374  DummyModule inst
+00000ec0: 6561 642c 200d 0a20 2020 2020 2020 2077  ead, ..        w
+00000ed0: 6869 6368 2073 686f 756c 6420 6e6f 7420  hich should not 
+00000ee0: 6361 6c6c 2060 7374 6570 602e 0d0a 2020  call `step`...  
+00000ef0: 2020 6465 7669 6365 203a 2055 6e69 6f6e    device : Union
+00000f00: 5b74 6f72 6368 2e64 6576 6963 652c 2073  [torch.device, s
+00000f10: 7472 2c20 696e 745d 0d0a 2020 2020 2020  tr, int]..      
+00000f20: 2020 4465 7669 6365 206f 6e20 7768 6963    Device on whic
+00000f30: 6820 746f 2072 756e 2074 6865 2063 6f6d  h to run the com
+00000f40: 7075 7461 7469 6f6e 2e20 0d0a 2020 2020  putation. ..    
+00000f50: 2020 2020 2020 2020 2d20 6074 6f72 6368          - `torch
+00000f60: 2e64 6576 6963 6560 0d0a 2020 2020 2020  .device`..      
+00000f70: 2020 2020 2020 2d20 6073 7472 603a 204c        - `str`: L
+00000f80: 696b 6520 6063 7075 602c 2060 6375 6461  ike `cpu`, `cuda
+00000f90: 3a30 602e 0d0a 2020 2020 2020 2020 2020  :0`...          
+00000fa0: 2020 2d20 6069 6e74 603a 2055 7369 6e67    - `int`: Using
+00000fb0: 2063 7564 613a 6069 6e74 602e 0d0a 2020   cuda:`int`...  
+00000fc0: 2020 2222 220d 0a0d 0a0d 0a20 2020 2064    """......    d
+00000fd0: 6566 205f 5f69 6e69 745f 5f28 0d0a 2020  ef __init__(..  
+00000fe0: 2020 2020 2020 7365 6c66 2c20 2a2c 0d0a        self, *,..
+00000ff0: 2020 2020 2020 2020 7472 6169 6e70 6970          trainpip
+00001000: 653a 2049 7465 7244 6174 6150 6970 652c  e: IterDataPipe,
+00001010: 2076 616c 6964 7069 7065 3a20 4f70 7469   validpipe: Opti
+00001020: 6f6e 616c 5b49 7465 7244 6174 6150 6970  onal[IterDataPip
+00001030: 655d 2c20 7465 7374 7069 7065 3a20 4f70  e], testpipe: Op
+00001040: 7469 6f6e 616c 5b49 7465 7244 6174 6150  tional[IterDataP
+00001050: 6970 655d 2c20 6669 656c 6473 3a20 4974  ipe], fields: It
+00001060: 6572 6162 6c65 5b46 6965 6c64 4d6f 6475  erable[FieldModu
+00001070: 6c65 5d2c 0d0a 2020 2020 2020 2020 6d6f  le],..        mo
+00001080: 6465 6c3a 2055 6e69 6f6e 5b52 6563 5379  del: Union[RecSy
+00001090: 7341 7263 682c 2074 6f72 6368 2e6e 6e2e  sArch, torch.nn.
+000010a0: 4d6f 6475 6c65 2c20 4e6f 6e65 5d2c 2063  Module, None], c
+000010b0: 7269 7465 7269 6f6e 3a20 556e 696f 6e5b  riterion: Union[
+000010c0: 4261 7365 4372 6974 6572 696f 6e2c 2043  BaseCriterion, C
+000010d0: 616c 6c61 626c 655d 2c20 0d0a 2020 2020  allable], ..    
+000010e0: 2020 2020 6f70 7469 6d69 7a65 723a 204f      optimizer: O
+000010f0: 7074 696f 6e61 6c5b 746f 7263 682e 6f70  ptional[torch.op
+00001100: 7469 6d2e 4f70 7469 6d69 7a65 725d 2c20  tim.Optimizer], 
+00001110: 6c72 5f73 6368 6564 756c 6572 3a20 4f70  lr_scheduler: Op
+00001120: 7469 6f6e 616c 5b74 6f72 6368 2e6f 7074  tional[torch.opt
+00001130: 696d 2e6c 725f 7363 6865 6475 6c65 722e  im.lr_scheduler.
+00001140: 5f4c 5253 6368 6564 756c 6572 5d2c 0d0a  _LRScheduler],..
+00001150: 2020 2020 2020 2020 6465 7669 6365 3a20          device: 
+00001160: 556e 696f 6e5b 746f 7263 682e 6465 7669  Union[torch.devi
+00001170: 6365 2c20 7374 722c 2069 6e74 5d0d 0a20  ce, str, int].. 
+00001180: 2020 2029 3a0d 0a0d 0a20 2020 2020 2020     ):....       
+00001190: 2073 656c 662e 6669 656c 6473 3a20 4669   self.fields: Fi
+000011a0: 656c 6454 7570 6c65 5b46 6965 6c64 4d6f  eldTuple[FieldMo
+000011b0: 6475 6c65 5d20 3d20 4669 656c 6454 7570  dule] = FieldTup
+000011c0: 6c65 2866 6965 6c64 7329 0d0a 2020 2020  le(fields)..    
+000011d0: 2020 2020 7365 6c66 2e64 6576 6963 6520      self.device 
+000011e0: 3d20 746f 7263 682e 6465 7669 6365 2864  = torch.device(d
+000011f0: 6576 6963 6529 0d0a 2020 2020 2020 2020  evice)..        
+00001200: 746f 7263 682e 6375 6461 2e73 6574 5f64  torch.cuda.set_d
+00001210: 6576 6963 6528 7365 6c66 2e64 6576 6963  evice(self.devic
+00001220: 6529 0d0a 0d0a 2020 2020 2020 2020 7365  e)....        se
+00001230: 6c66 2e5f 7365 745f 6461 7461 7069 7065  lf._set_datapipe
+00001240: 2874 7261 696e 7069 7065 2c20 7661 6c69  (trainpipe, vali
+00001250: 6470 6970 652c 2074 6573 7470 6970 6529  dpipe, testpipe)
+00001260: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+00001270: 7365 745f 6f74 6865 7228 6d6f 6465 6c2c  set_other(model,
+00001280: 2063 7269 7465 7269 6f6e 2c20 6f70 7469   criterion, opti
+00001290: 6d69 7a65 722c 206c 725f 7363 6865 6475  mizer, lr_schedu
+000012a0: 6c65 7229 0d0a 0d0a 2020 2020 2020 2020  ler)....        
+000012b0: 7365 6c66 2e5f 5f6d 6f64 6520 3d20 2774  self.__mode = 't
+000012c0: 7261 696e 270d 0a0d 0a20 2020 2020 2020  rain'....       
+000012d0: 2064 6566 2063 6c65 616e 2829 3a0d 0a20   def clean():.. 
+000012e0: 2020 2020 2020 2020 2020 2070 6172 656e             paren
+000012f0: 7420 3d20 7073 7574 696c 2e50 726f 6365  t = psutil.Proce
+00001300: 7373 286f 732e 6765 7470 6964 2829 290d  ss(os.getpid()).
+00001310: 0a20 2020 2020 2020 2020 2020 2063 6869  .            chi
+00001320: 6c64 7265 6e20 3d20 7061 7265 6e74 2e63  ldren = parent.c
+00001330: 6869 6c64 7265 6e28 7265 6375 7273 6976  hildren(recursiv
+00001340: 653d 5472 7565 290d 0a20 2020 2020 2020  e=True)..       
+00001350: 2020 2020 2066 6f72 2070 726f 6365 7373       for process
+00001360: 2069 6e20 6368 696c 6472 656e 3a0d 0a20   in children:.. 
+00001370: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00001380: 726f 6365 7373 2e73 656e 645f 7369 676e  rocess.send_sign
+00001390: 616c 2873 6967 6e61 6c2e 5349 4754 4552  al(signal.SIGTER
+000013a0: 4d29 0d0a 2020 2020 2020 2020 2020 2020  M)..            
+000013b0: 7073 7574 696c 2e77 6169 745f 7072 6f63  psutil.wait_proc
+000013c0: 7328 6368 696c 6472 656e 2c20 7469 6d65  s(children, time
+000013d0: 6f75 743d 3529 0d0a 0d0a 2020 2020 2020  out=5)....      
+000013e0: 2020 6174 6578 6974 2e72 6567 6973 7465    atexit.registe
+000013f0: 7228 636c 6561 6e29 0d0a 0d0a 2020 2020  r(clean)....    
+00001400: 6465 6620 5f73 6574 5f64 6174 6170 6970  def _set_datapip
+00001410: 6528 0d0a 2020 2020 2020 2020 7365 6c66  e(..        self
+00001420: 2c0d 0a20 2020 2020 2020 2074 7261 696e  ,..        train
+00001430: 7069 7065 2c0d 0a20 2020 2020 2020 2076  pipe,..        v
+00001440: 616c 6964 7069 7065 3d4e 6f6e 652c 0d0a  alidpipe=None,..
+00001450: 2020 2020 2020 2020 7465 7374 7069 7065          testpipe
+00001460: 3d4e 6f6e 652c 0d0a 2020 2020 293a 0d0a  =None,..    ):..
+00001470: 2020 2020 2020 2020 2222 2253 6574 2074          """Set t
+00001480: 6865 2064 6174 6120 7069 7065 2066 6f72  he data pipe for
+00001490: 2074 7261 696e 696e 672c 2076 616c 6964   training, valid
+000014a0: 6174 696f 6e20 616e 6420 7465 7374 2e22  ation and test."
+000014b0: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
+000014c0: 2e74 7261 696e 7069 7065 203d 2074 7261  .trainpipe = tra
+000014d0: 696e 7069 7065 0d0a 2020 2020 2020 2020  inpipe..        
+000014e0: 7365 6c66 2e76 616c 6964 7069 7065 203d  self.validpipe =
+000014f0: 2073 656c 662e 7472 6169 6e70 6970 6520   self.trainpipe 
+00001500: 6966 2076 616c 6964 7069 7065 2069 7320  if validpipe is 
+00001510: 4e6f 6e65 2065 6c73 6520 7661 6c69 6470  None else validp
+00001520: 6970 650d 0a20 2020 2020 2020 2073 656c  ipe..        sel
+00001530: 662e 7465 7374 7069 7065 203d 2073 656c  f.testpipe = sel
+00001540: 662e 7661 6c69 6470 6970 6520 6966 2074  f.validpipe if t
+00001550: 6573 7470 6970 6520 6973 204e 6f6e 6520  estpipe is None 
+00001560: 656c 7365 2074 6573 7470 6970 650d 0a0d  else testpipe...
+00001570: 0a20 2020 2064 6566 205f 7365 745f 6f74  .    def _set_ot
+00001580: 6865 7228 0d0a 2020 2020 2020 2020 7365  her(..        se
+00001590: 6c66 2c0d 0a20 2020 2020 2020 206d 6f64  lf,..        mod
+000015a0: 656c 3d4e 6f6e 652c 2063 7269 7465 7269  el=None, criteri
+000015b0: 6f6e 3d4e 6f6e 652c 206f 7074 696d 697a  on=None, optimiz
+000015c0: 6572 3d4e 6f6e 652c 206c 725f 7363 6865  er=None, lr_sche
+000015d0: 6475 6c65 723d 4e6f 6e65 2c0d 0a20 2020  duler=None,..   
+000015e0: 2029 3a0d 0a20 2020 2020 2020 2022 2222   ):..        """
+000015f0: 5365 7420 7468 6520 6f74 6865 7220 6e65  Set the other ne
+00001600: 6365 7373 6172 7920 636f 6d70 6f6e 656e  cessary componen
+00001610: 7473 2e22 2222 0d0a 2020 2020 2020 2020  ts."""..        
+00001620: 7365 6c66 2e63 7269 7465 7269 6f6e 203d  self.criterion =
+00001630: 2063 7269 7465 7269 6f6e 0d0a 2020 2020   criterion..    
+00001640: 2020 2020 7365 6c66 2e6d 6f64 656c 203d      self.model =
+00001650: 206d 6f64 656c 2e74 6f28 7365 6c66 2e64   model.to(self.d
+00001660: 6576 6963 6529 2069 6620 6d6f 6465 6c20  evice) if model 
+00001670: 656c 7365 205f 4475 6d6d 794d 6f64 756c  else _DummyModul
+00001680: 6528 290d 0a20 2020 2020 2020 2073 656c  e()..        sel
+00001690: 662e 6f70 7469 6d69 7a65 7220 3d20 6f70  f.optimizer = op
+000016a0: 7469 6d69 7a65 7220 6966 206f 7074 696d  timizer if optim
+000016b0: 697a 6572 2065 6c73 6520 5f44 756d 6d79  izer else _Dummy
+000016c0: 4d6f 6475 6c65 2829 0d0a 2020 2020 2020  Module()..      
+000016d0: 2020 7365 6c66 2e6c 725f 7363 6865 6475    self.lr_schedu
+000016e0: 6c65 7220 3d20 6c72 5f73 6368 6564 756c  ler = lr_schedul
+000016f0: 6572 2069 6620 6c72 5f73 6368 6564 756c  er if lr_schedul
+00001700: 6572 2065 6c73 6520 5f44 756d 6d79 4d6f  er else _DummyMo
+00001710: 6475 6c65 2829 0d0a 0d0a 2020 2020 4070  dule()....    @p
+00001720: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
+00001730: 206d 6f64 6528 7365 6c66 293a 0d0a 2020   mode(self):..  
+00001740: 2020 2020 2020 2222 2247 6574 2074 6865        """Get the
+00001750: 2063 7572 7265 6e74 206d 6f64 6520 6f66   current mode of
+00001760: 2074 6865 2063 6869 6566 2063 6f61 6368   the chief coach
+00001770: 2e22 2222 0d0a 2020 2020 2020 2020 7265  ."""..        re
+00001780: 7475 726e 2073 656c 662e 5f5f 6d6f 6465  turn self.__mode
+00001790: 0d0a 0d0a 2020 2020 4074 696d 656d 6574  ....    @timemet
+000017a0: 6572 2822 436f 6163 682f 7472 6169 6e22  er("Coach/train"
+000017b0: 290d 0a20 2020 2064 6566 2074 7261 696e  )..    def train
+000017c0: 2873 656c 662c 2065 706f 6368 3a20 696e  (self, epoch: in
+000017d0: 7429 3a0d 0a20 2020 2020 2020 2022 2222  t):..        """
+000017e0: 5374 6172 7420 7472 6169 6e69 6e67 2061  Start training a
+000017f0: 6e64 2072 6574 7572 6e20 7468 6520 7472  nd return the tr
+00001800: 6169 6e69 6e67 206c 6f73 732e 2222 220d  aining loss.""".
+00001810: 0a20 2020 2020 2020 2073 656c 662e 5f5f  .        self.__
+00001820: 6d6f 6465 203d 2027 7472 6169 6e27 0d0a  mode = 'train'..
+00001830: 2020 2020 2020 2020 7365 6c66 2e6d 6f64          self.mod
+00001840: 656c 2e74 7261 696e 2829 0d0a 2020 2020  el.train()..    
+00001850: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00001860: 7472 6169 6e5f 7065 725f 6570 6f63 6828  train_per_epoch(
+00001870: 6570 6f63 6829 0d0a 0d0a 2020 2020 4074  epoch)....    @t
+00001880: 696d 656d 6574 6572 2822 436f 6163 682f  imemeter("Coach/
+00001890: 7661 6c69 6422 290d 0a20 2020 2040 746f  valid")..    @to
+000018a0: 7263 682e 6e6f 5f67 7261 6428 290d 0a20  rch.no_grad().. 
+000018b0: 2020 2064 6566 2076 616c 6964 2873 656c     def valid(sel
+000018c0: 662c 2065 706f 6368 3a20 696e 7429 3a0d  f, epoch: int):.
+000018d0: 0a20 2020 2020 2020 2022 2222 5374 6172  .        """Star
+000018e0: 7420 7661 6c69 6461 7469 6f6e 2061 6e64  t validation and
+000018f0: 2072 6574 7572 6e20 7468 6520 7661 6c69   return the vali
+00001900: 6461 7469 6f6e 206d 6574 7269 6373 2e22  dation metrics."
+00001910: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
+00001920: 2e5f 5f6d 6f64 6520 3d20 2776 616c 6964  .__mode = 'valid
+00001930: 270d 0a20 2020 2020 2020 2073 656c 662e  '..        self.
+00001940: 6d6f 6465 6c2e 6576 616c 2829 0d0a 2020  model.eval()..  
+00001950: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00001960: 662e 6576 616c 7561 7465 2865 706f 6368  f.evaluate(epoch
+00001970: 3d65 706f 6368 2c20 7072 6566 6978 3d27  =epoch, prefix='
+00001980: 7661 6c69 6427 290d 0a0d 0a20 2020 2040  valid')....    @
+00001990: 7469 6d65 6d65 7465 7228 2243 6f61 6368  timemeter("Coach
+000019a0: 2f74 6573 7422 290d 0a20 2020 2040 746f  /test")..    @to
+000019b0: 7263 682e 6e6f 5f67 7261 6428 290d 0a20  rch.no_grad().. 
+000019c0: 2020 2064 6566 2074 6573 7428 7365 6c66     def test(self
+000019d0: 2c20 6570 6f63 683a 2069 6e74 293a 0d0a  , epoch: int):..
+000019e0: 2020 2020 2020 2020 2222 2253 7461 7274          """Start
+000019f0: 2074 6573 7469 6e67 2061 6e64 2072 6574   testing and ret
+00001a00: 7572 6e20 7468 6520 7465 7374 206d 6574  urn the test met
+00001a10: 7269 6373 2e22 2222 0d0a 2020 2020 2020  rics."""..      
+00001a20: 2020 7365 6c66 2e5f 5f6d 6f64 6520 3d20    self.__mode = 
+00001a30: 2774 6573 7427 0d0a 2020 2020 2020 2020  'test'..        
+00001a40: 7365 6c66 2e6d 6f64 656c 2e65 7661 6c28  self.model.eval(
+00001a50: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00001a60: 6e20 7365 6c66 2e65 7661 6c75 6174 6528  n self.evaluate(
+00001a70: 6570 6f63 683d 6570 6f63 682c 2070 7265  epoch=epoch, pre
+00001a80: 6669 783d 2774 6573 7427 290d 0a0d 0a20  fix='test').... 
+00001a90: 2020 2040 6162 632e 6162 7374 7261 6374     @abc.abstract
+00001aa0: 6d65 7468 6f64 0d0a 2020 2020 6465 6620  method..    def 
+00001ab0: 7472 6169 6e5f 7065 725f 6570 6f63 6828  train_per_epoch(
+00001ac0: 7365 6c66 2c20 6570 6f63 683a 2069 6e74  self, epoch: int
+00001ad0: 293a 0d0a 2020 2020 2020 2020 7261 6973  ):..        rais
+00001ae0: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
+00001af0: 4572 726f 7228 0d0a 2020 2020 2020 2020  Error(..        
+00001b00: 2020 2020 6622 7b73 656c 662e 5f5f 636c      f"{self.__cl
+00001b10: 6173 735f 5f2e 5f5f 6e61 6d65 5f5f 7d2e  ass__.__name__}.
+00001b20: 7472 6169 6e5f 7065 725f 6570 6f63 6828  train_per_epoch(
+00001b30: 2920 7368 6f75 6c64 2062 6520 696d 706c  ) should be impl
+00001b40: 656d 656e 7465 6420 2e2e 2e22 0d0a 2020  emented ..."..  
+00001b50: 2020 2020 2020 290d 0a0d 0a20 2020 2040        )....    @
+00001b60: 6162 632e 6162 7374 7261 6374 6d65 7468  abc.abstractmeth
+00001b70: 6f64 0d0a 2020 2020 6465 6620 6576 616c  od..    def eval
+00001b80: 7561 7465 2873 656c 662c 2065 706f 6368  uate(self, epoch
+00001b90: 3a20 696e 742c 2070 7265 6669 783a 2073  : int, prefix: s
+00001ba0: 7472 203d 2027 7661 6c69 6427 293a 0d0a  tr = 'valid'):..
+00001bb0: 2020 2020 2020 2020 7261 6973 6520 4e6f          raise No
+00001bc0: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
+00001bd0: 7228 0d0a 2020 2020 2020 2020 2020 2020  r(..            
+00001be0: 6622 7b73 656c 662e 5f5f 636c 6173 735f  f"{self.__class_
+00001bf0: 5f2e 5f5f 6e61 6d65 5f5f 7d2e 6576 616c  _.__name__}.eval
+00001c00: 7561 7465 2829 2073 686f 756c 6420 6265  uate() should be
+00001c10: 2069 6d70 6c65 6d65 6e74 6564 202e 2e2e   implemented ...
+00001c20: 220d 0a20 2020 2020 2020 2029 0d0a 0d0a  "..        )....
+00001c30: 2020 2020 6465 6620 7265 6769 7374 6572      def register
+00001c40: 5f6d 6574 7269 6328 0d0a 2020 2020 2020  _metric(..      
+00001c50: 2020 7365 6c66 2c20 6e61 6d65 3a20 7374    self, name: st
+00001c60: 722c 2066 756e 633a 2043 616c 6c61 626c  r, func: Callabl
+00001c70: 652c 200d 0a20 2020 2020 2020 2066 6d74  e, ..        fmt
+00001c80: 3a20 7374 7220 3d20 272e 3466 272c 2062  : str = '.4f', b
+00001c90: 6573 745f 6361 7374 6572 3a20 4361 6c6c  est_caster: Call
+00001ca0: 6162 6c65 203d 206d 6178 0d0a 2020 2020  able = max..    
+00001cb0: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
+00001cc0: 2020 2020 7222 2222 0d0a 2020 2020 2020      r"""..      
+00001cd0: 2020 5265 6769 7374 6572 2061 206d 6574    Register a met
+00001ce0: 7269 632e 0d0a 0d0a 2020 2020 2020 2020  ric.....        
+00001cf0: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
+00001d00: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
+00001d10: 2020 2020 2020 2020 6e61 6d65 203a 2073          name : s
+00001d20: 7472 0d0a 2020 2020 2020 2020 2020 2020  tr..            
+00001d30: 5468 6520 636f 6d70 6c65 7465 206e 616d  The complete nam
+00001d40: 6520 6f66 2074 6865 206d 6574 7269 632c  e of the metric,
+00001d50: 2073 7563 6820 6173 2060 4c4f 5353 3260   such as `LOSS2`
+00001d60: 2e0d 0a20 2020 2020 2020 2020 2020 2054  ...            T
+00001d70: 6865 206e 6f74 6174 696f 6e20 6040 6020  he notation `@` 
+00001d80: 7368 6f75 6c64 206e 6f74 2062 6520 696e  should not be in
+00001d90: 636c 7564 6564 2c20 692e 652e 2c20 274c  cluded, i.e., 'L
+00001da0: 4f53 5340 3227 2069 7320 696e 7661 6c69  OSS@2' is invali
+00001db0: 642e 0d0a 2020 2020 2020 2020 6675 6e63  d...        func
+00001dc0: 203a 2043 616c 6c61 626c 650d 0a20 2020   : Callable..   
+00001dd0: 2020 2020 2020 2020 2054 6865 2066 756e           The fun
+00001de0: 6374 696f 6e20 746f 2070 726f 6365 7373  ction to process
+00001df0: 2074 6865 2064 6174 6120 666f 7220 7468   the data for th
+00001e00: 6520 6d65 7472 6963 2e0d 0a20 2020 2020  e metric...     
+00001e10: 2020 2066 6d74 203a 2073 7472 2c20 6f70     fmt : str, op
+00001e20: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+00001e30: 2020 2020 5468 6520 666f 726d 6174 2074      The format t
+00001e40: 6f20 7573 6520 7768 656e 2070 7269 6e74  o use when print
+00001e50: 696e 6720 7468 6520 6d65 7472 6963 2c20  ing the metric, 
+00001e60: 6465 6661 756c 7473 2074 6f20 6027 2e34  defaults to `'.4
+00001e70: 6627 602e 0d0a 2020 2020 2020 2020 6265  f'`...        be
+00001e80: 7374 5f63 6173 7465 7220 3a20 4361 6c6c  st_caster : Call
+00001e90: 6162 6c65 2c20 6f70 7469 6f6e 616c 0d0a  able, optional..
+00001ea0: 2020 2020 2020 2020 2020 2020 4120 6675              A fu
+00001eb0: 6e63 7469 6f6e 2075 7365 6420 746f 2063  nction used to c
+00001ec0: 6173 7420 7468 6520 6265 7374 2076 616c  ast the best val
+00001ed0: 7565 206f 6620 7468 6520 6d65 7472 6963  ue of the metric
+00001ee0: 2c20 6465 6661 756c 7473 2074 6f20 606d  , defaults to `m
+00001ef0: 6178 602e 0d0a 2020 2020 2020 2020 2020  ax`...          
+00001f00: 2020 0d0a 2020 2020 2020 2020 5265 7475    ..        Retu
+00001f10: 726e 730d 0a20 2020 2020 2020 202d 2d2d  rns..        ---
+00001f20: 2d2d 2d2d 0d0a 2020 2020 2020 2020 4e6f  ----..        No
+00001f30: 6e65 0d0a 2020 2020 2020 2020 0d0a 2020  ne..        ..  
+00001f40: 2020 2020 2020 5261 6973 6573 0d0a 2020        Raises..  
+00001f50: 2020 2020 2020 2d2d 2d2d 2d2d 0d0a 2020        ------..  
+00001f60: 2020 2020 2020 4173 7365 7274 696f 6e45        AssertionE
+00001f70: 7272 6f72 0d0a 2020 2020 2020 2020 2020  rror..          
+00001f80: 2020 5768 656e 2060 6e61 6d65 6020 6861    When `name` ha
+00001f90: 7320 616c 7265 6164 7920 6265 656e 2072  s already been r
+00001fa0: 6567 6973 7465 7265 6420 6f72 2063 6f6e  egistered or con
+00001fb0: 7461 696e 7320 7468 6520 6e6f 7461 7469  tains the notati
+00001fc0: 6f6e 2060 4060 2e0d 0a20 2020 2020 2020  on `@`...       
+00001fd0: 2022 2222 0d0a 0d0a 2020 2020 2020 2020   """....        
+00001fe0: 6e61 6d65 203d 206e 616d 652e 7570 7065  name = name.uppe
+00001ff0: 7228 290d 0a20 2020 2020 2020 2061 7373  r()..        ass
+00002000: 6572 7420 4445 4641 554c 545f 4d45 5452  ert DEFAULT_METR
+00002010: 4943 532e 6765 7428 6e61 6d65 2c20 4e6f  ICS.get(name, No
+00002020: 6e65 2920 6973 204e 6f6e 652c 2066 2254  ne) is None, f"T
+00002030: 6865 206d 6574 7269 6320 7b6e 616d 657d  he metric {name}
+00002040: 2061 6c72 6561 6479 2065 7869 7374 7320   already exists 
+00002050: 2e2e 2e22 0d0a 2020 2020 2020 2020 6173  ..."..        as
+00002060: 7365 7274 2027 4027 206e 6f74 2069 6e20  sert '@' not in 
+00002070: 6e61 6d65 2c20 6622 5468 6520 6d65 7472  name, f"The metr
+00002080: 6963 206e 616d 6520 6861 7320 696e 7661  ic name has inva
+00002090: 6c69 6420 6e6f 7461 7469 6f6e 206f 6620  lid notation of 
+000020a0: 6040 2720 2e2e 2e22 0d0a 2020 2020 2020  `@' ..."..      
+000020b0: 2020 4445 4641 554c 545f 4d45 5452 4943    DEFAULT_METRIC
+000020c0: 535b 6e61 6d65 5d20 3d20 6675 6e63 0d0a  S[name] = func..
+000020d0: 2020 2020 2020 2020 4445 4641 554c 545f          DEFAULT_
+000020e0: 464d 5453 5b6e 616d 655d 203d 2066 6d74  FMTS[name] = fmt
+000020f0: 0d0a 2020 2020 2020 2020 4445 4641 554c  ..        DEFAUL
+00002100: 545f 4245 5354 5f43 4153 5445 525b 6e61  T_BEST_CASTER[na
+00002110: 6d65 5d20 3d20 6265 7374 5f63 6173 7465  me] = best_caste
+00002120: 720d 0a0d 0a0d 0a63 6c61 7373 2043 6f61  r......class Coa
+00002130: 6368 2843 6869 6566 436f 6163 6829 3a0d  ch(ChiefCoach):.
+00002140: 0a20 2020 2022 2222 5468 6520 6672 616d  .    """The fram
+00002150: 6577 6f72 6b20 666f 7220 7472 6169 6e69  ework for traini
+00002160: 6e67 2e22 2222 0d0a 0d0a 2020 2020 6465  ng."""....    de
+00002170: 6620 7072 6570 6172 655f 6461 7461 6c6f  f prepare_datalo
+00002180: 6164 6572 2873 656c 6629 202d 3e20 4e6f  ader(self) -> No
+00002190: 6e65 3a0d 0a20 2020 2020 2020 2022 2222  ne:..        """
+000021a0: 5072 6570 6172 6520 6461 7461 206c 6f61  Prepare data loa
+000021b0: 6465 7273 2066 6f72 2074 7261 696e 696e  ders for trainin
+000021c0: 672c 2076 616c 6964 6174 696f 6e2c 2061  g, validation, a
+000021d0: 6e64 2074 6573 7469 6e67 2064 6174 612e  nd testing data.
+000021e0: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
+000021f0: 662e 7472 6169 6e6c 6f61 6465 7220 3d20  f.trainloader = 
+00002200: 4461 7461 4c6f 6164 6572 280d 0a20 2020  DataLoader(..   
+00002210: 2020 2020 2020 2020 2064 6174 6170 6970           datapip
+00002220: 653d 7365 6c66 2e74 7261 696e 7069 7065  e=self.trainpipe
+00002230: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+00002240: 6e75 6d5f 776f 726b 6572 733d 7365 6c66  num_workers=self
+00002250: 2e63 6667 2e6e 756d 5f77 6f72 6b65 7273  .cfg.num_workers
+00002260: 2c0d 0a20 2020 2020 2020 2020 2020 2070  ,..            p
+00002270: 696e 5f6d 656d 6f72 793d 7365 6c66 2e63  in_memory=self.c
+00002280: 6667 2e70 696e 5f6d 656d 6f72 790d 0a20  fg.pin_memory.. 
+00002290: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+000022a0: 2020 7365 6c66 2e76 616c 6964 6c6f 6164    self.validload
+000022b0: 6572 203d 2044 6174 614c 6f61 6465 7228  er = DataLoader(
+000022c0: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
+000022d0: 7461 7069 7065 3d73 656c 662e 7661 6c69  tapipe=self.vali
+000022e0: 6470 6970 652c 200d 0a20 2020 2020 2020  dpipe, ..       
+000022f0: 2020 2020 206e 756d 5f77 6f72 6b65 7273       num_workers
+00002300: 3d73 656c 662e 6366 672e 6e75 6d5f 776f  =self.cfg.num_wo
+00002310: 726b 6572 732c 0d0a 2020 2020 2020 2020  rkers,..        
+00002320: 2020 2020 7069 6e5f 6d65 6d6f 7279 3d73      pin_memory=s
+00002330: 656c 662e 6366 672e 7069 6e5f 6d65 6d6f  elf.cfg.pin_memo
+00002340: 7279 0d0a 2020 2020 2020 2020 290d 0a20  ry..        ).. 
+00002350: 2020 2020 2020 2073 656c 662e 7465 7374         self.test
+00002360: 6c6f 6164 6572 203d 2044 6174 614c 6f61  loader = DataLoa
+00002370: 6465 7228 0d0a 2020 2020 2020 2020 2020  der(..          
+00002380: 2020 6461 7461 7069 7065 3d73 656c 662e    datapipe=self.
+00002390: 7465 7374 7069 7065 2c20 0d0a 2020 2020  testpipe, ..    
+000023a0: 2020 2020 2020 2020 6e75 6d5f 776f 726b          num_work
+000023b0: 6572 733d 7365 6c66 2e63 6667 2e6e 756d  ers=self.cfg.num
+000023c0: 5f77 6f72 6b65 7273 2c0d 0a20 2020 2020  _workers,..     
+000023d0: 2020 2020 2020 2070 696e 5f6d 656d 6f72         pin_memor
+000023e0: 793d 7365 6c66 2e63 6667 2e70 696e 5f6d  y=self.cfg.pin_m
+000023f0: 656d 6f72 790d 0a20 2020 2020 2020 2029  emory..        )
+00002400: 0d0a 2020 2020 0d0a 2020 2020 4070 726f  ..    ..    @pro
+00002410: 7065 7274 790d 0a20 2020 2064 6566 2064  perty..    def d
+00002420: 6174 616c 6f61 6465 7228 7365 6c66 293a  ataloader(self):
+00002430: 0d0a 2020 2020 2020 2020 2222 2252 6574  ..        """Ret
+00002440: 7572 6e20 7468 6520 636f 7272 6573 706f  urn the correspo
+00002450: 6e64 696e 6720 6461 7461 206c 6f61 6465  nding data loade
+00002460: 7220 6465 7065 6e64 696e 6720 6f6e 2074  r depending on t
+00002470: 6865 2063 7572 7265 6e74 206d 6f64 652e  he current mode.
+00002480: 2222 220d 0a20 2020 2020 2020 2069 6620  """..        if 
+00002490: 7365 6c66 2e6d 6f64 6520 3d3d 2027 7472  self.mode == 'tr
+000024a0: 6169 6e27 3a0d 0a20 2020 2020 2020 2020  ain':..         
+000024b0: 2020 2072 6574 7572 6e20 7365 6c66 2e74     return self.t
+000024c0: 7261 696e 6c6f 6164 6572 0d0a 2020 2020  rainloader..    
+000024d0: 2020 2020 656c 6966 2073 656c 662e 6d6f      elif self.mo
+000024e0: 6465 203d 3d20 2776 616c 6964 273a 0d0a  de == 'valid':..
+000024f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00002500: 726e 2073 656c 662e 7661 6c69 646c 6f61  rn self.validloa
+00002510: 6465 720d 0a20 2020 2020 2020 2065 6c73  der..        els
+00002520: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00002530: 7265 7475 726e 2073 656c 662e 7465 7374  return self.test
+00002540: 6c6f 6164 6572 0d0a 0d0a 2020 2020 4070  loader....    @p
+00002550: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
+00002560: 206d 6f6e 6974 6f72 7328 7365 6c66 2920   monitors(self) 
+00002570: 2d3e 204d 6f6e 6974 6f72 3a0d 0a20 2020  -> Monitor:..   
+00002580: 2020 2020 2022 2222 5265 7475 726e 2074       """Return t
+00002590: 6865 206d 6f6e 6974 6f72 2064 6963 7469  he monitor dicti
+000025a0: 6f6e 6172 7920 666f 7220 7468 6520 6469  onary for the di
+000025b0: 6666 6572 656e 7420 6d6f 6465 7320 2827  fferent modes ('
+000025c0: 7472 6169 6e27 2c20 2776 616c 6964 272c  train', 'valid',
+000025d0: 2027 7465 7374 2729 2e22 2222 0d0a 2020   'test')."""..  
+000025e0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000025f0: 662e 5f5f 6d6f 6e69 746f 7273 0d0a 0d0a  f.__monitors....
+00002600: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
+00002610: 2020 2064 6566 206d 6574 6572 3462 6573     def meter4bes
+00002620: 7428 7365 6c66 293a 0d0a 2020 2020 2020  t(self):..      
+00002630: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
+00002640: 6265 7374 5f6d 6574 6572 0d0a 0d0a 2020  best_meter....  
+00002650: 2020 406d 6574 6572 3462 6573 742e 7365    @meter4best.se
+00002660: 7474 6572 0d0a 2020 2020 6465 6620 6d65  tter..    def me
+00002670: 7465 7234 6265 7374 2873 656c 662c 206d  ter4best(self, m
+00002680: 6574 6572 3a20 4176 6572 6167 654d 6574  eter: AverageMet
+00002690: 6572 293a 0d0a 2020 2020 2020 2020 7365  er):..        se
+000026a0: 6c66 2e5f 5f62 6573 745f 6d65 7465 7220  lf.__best_meter 
+000026b0: 3d20 6d65 7465 720d 0a20 2020 2020 2020  = meter..       
+000026c0: 2069 6e66 6f4c 6f67 6765 7228 6622 5b43   infoLogger(f"[C
+000026d0: 6f61 6368 5d20 3e3e 3e20 5365 7420 6265  oach] >>> Set be
+000026e0: 7374 206d 6574 6572 3a20 7b6d 6574 6572  st meter: {meter
+000026f0: 2e6e 616d 657d 2022 290d 0a0d 0a20 2020  .name} ")....   
+00002700: 2040 7469 6d65 6d65 7465 7228 2243 6f61   @timemeter("Coa
+00002710: 6368 2f63 6f6d 7069 6c65 2229 0d0a 2020  ch/compile")..  
+00002720: 2020 6465 6620 636f 6d70 696c 6528 0d0a    def compile(..
+00002730: 2020 2020 2020 2020 7365 6c66 2c20 6366          self, cf
+00002740: 673a 2043 6f6e 6669 672c 206d 6f6e 6974  g: Config, monit
+00002750: 6f72 733a 204c 6973 745b 7374 725d 2c20  ors: List[str], 
+00002760: 0d0a 2020 2020 2020 2020 7768 6963 6834  ..        which4
+00002770: 6265 7374 3a20 7374 7220 3d20 274c 4f53  best: str = 'LOS
+00002780: 5327 0d0a 2020 2020 293a 0d0a 2020 2020  S'..    ):..    
+00002790: 2020 2020 7222 2222 0d0a 2020 2020 2020      r"""..      
+000027a0: 2020 4c6f 6164 2074 6865 2063 6f6e 6669    Load the confi
+000027b0: 6775 7261 7469 6f6e 2061 6e64 2073 6574  guration and set
+000027c0: 2075 7020 6d6f 6e69 746f 7273 2066 6f72   up monitors for
+000027d0: 2074 7261 696e 696e 672e 0d0a 0d0a 2020   training.....  
+000027e0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+000027f0: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+00002800: 2d2d 2d2d 0d0a 2020 2020 2020 2020 6366  ----..        cf
+00002810: 6720 3a20 436f 6e66 6967 0d0a 2020 2020  g : Config..    
+00002820: 2020 2020 2020 2020 4120 636f 6e66 6967          A config
+00002830: 7572 6174 696f 6e20 6f62 6a65 6374 2077  uration object w
+00002840: 6974 6820 7468 6520 7472 6169 6e69 6e67  ith the training
+00002850: 2064 6574 6169 6c73 2e0d 0a20 2020 2020   details...     
+00002860: 2020 206d 6f6e 6974 6f72 7320 3a20 4c69     monitors : Li
+00002870: 7374 5b73 7472 5d0d 0a20 2020 2020 2020  st[str]..       
+00002880: 2020 2020 2041 206c 6973 7420 6f66 206d       A list of m
+00002890: 6574 7269 6320 6e61 6d65 7320 746f 2062  etric names to b
+000028a0: 6520 6d6f 6e69 746f 7265 6420 6475 7269  e monitored duri
+000028b0: 6e67 2074 7261 696e 696e 672e 0d0a 2020  ng training...  
+000028c0: 2020 2020 2020 7768 6963 6834 6265 7374        which4best
+000028d0: 203a 2073 7472 2c20 6465 6661 756c 7473   : str, defaults
+000028e0: 2060 4c4f 5353 270d 0a20 2020 2020 2020   `LOSS'..       
+000028f0: 2020 2020 2054 6865 206d 6574 7269 6320       The metric 
+00002900: 7573 6564 2066 6f72 2073 656c 6563 7469  used for selecti
+00002910: 6e67 2074 6865 2062 6573 7420 6368 6563  ng the best chec
+00002920: 6b70 6f69 6e74 2e0d 0a0d 0a20 2020 2020  kpoint.....     
+00002930: 2020 2045 7861 6d70 6c65 730d 0a20 2020     Examples..   
+00002940: 2020 2020 202d 2d2d 2d2d 2d2d 2d0d 0a20       --------.. 
+00002950: 2020 2020 2020 203e 3e3e 2063 6f61 6368         >>> coach
+00002960: 3a20 436f 6163 680d 0a20 2020 2020 2020  : Coach..       
+00002970: 203e 3e3e 2063 6f61 6368 2e63 6f6d 7069   >>> coach.compi
+00002980: 6c65 2863 6667 2c20 6d6f 6e69 746f 7273  le(cfg, monitors
+00002990: 3d5b 276c 6f73 7327 2c20 2772 6563 616c  =['loss', 'recal
+000029a0: 6c40 3130 272c 2027 7265 6361 6c6c 4032  l@10', 'recall@2
+000029b0: 3027 2c20 276e 6463 6740 3130 272c 2027  0', 'ndcg@10', '
+000029c0: 6e64 6367 4032 3027 5d29 0d0a 2020 2020  ndcg@20'])..    
+000029d0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+000029e0: 2073 656c 662e 6366 6720 3d20 6366 670d   self.cfg = cfg.
+000029f0: 0a20 2020 2020 2020 2023 206d 6574 6572  .        # meter
+00002a00: 7320 666f 7220 7472 6169 6e7c 7661 6c69  s for train|vali
+00002a10: 647c 7465 7374 0d0a 2020 2020 2020 2020  d|test..        
+00002a20: 7365 6c66 2e5f 5f6d 6f6e 6974 6f72 7320  self.__monitors 
+00002a30: 3d20 4d6f 6e69 746f 7228 290d 0a20 2020  = Monitor()..   
+00002a40: 2020 2020 2073 656c 662e 5f5f 6d6f 6e69       self.__moni
+00002a50: 746f 7273 5b27 7472 6169 6e27 5d20 3d20  tors['train'] = 
+00002a60: 6465 6661 756c 7464 6963 7428 6c69 7374  defaultdict(list
+00002a70: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00002a80: 5f5f 6d6f 6e69 746f 7273 5b27 7661 6c69  __monitors['vali
+00002a90: 6427 5d20 3d20 6465 6661 756c 7464 6963  d'] = defaultdic
+00002aa0: 7428 6c69 7374 290d 0a20 2020 2020 2020  t(list)..       
+00002ab0: 2073 656c 662e 5f5f 6d6f 6e69 746f 7273   self.__monitors
+00002ac0: 5b27 7465 7374 275d 203d 2064 6566 6175  ['test'] = defau
+00002ad0: 6c74 6469 6374 286c 6973 7429 0d0a 0d0a  ltdict(list)....
+00002ae0: 2020 2020 2020 2020 6465 6620 7365 745f          def set_
+00002af0: 6d6f 6e69 746f 7228 0d0a 2020 2020 2020  monitor(..      
+00002b00: 2020 2020 2020 6e61 6d65 3a20 7374 722c        name: str,
+00002b10: 206c 6173 746e 616d 653a 2073 7472 2c20   lastname: str, 
+00002b20: 7072 6566 6978 3a20 7374 7220 3d20 2774  prefix: str = 't
+00002b30: 7261 696e 272c 202a 2a6b 7761 7267 730d  rain', **kwargs.
+00002b40: 0a20 2020 2020 2020 2029 3a0d 0a20 2020  .        ):..   
+00002b50: 2020 2020 2020 2020 2022 2222 4164 6420           """Add 
+00002b60: 6120 6d6f 6e69 746f 7220 666f 7220 7468  a monitor for th
+00002b70: 6520 7370 6563 6966 6965 6420 6d65 7472  e specified metr
+00002b80: 6963 2e22 2222 0d0a 2020 2020 2020 2020  ic."""..        
+00002b90: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00002ba0: 2020 2020 2020 2020 2020 6d65 7465 7220            meter 
+00002bb0: 3d20 4176 6572 6167 654d 6574 6572 280d  = AverageMeter(.
+00002bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002bd0: 2020 2020 2020 2020 206e 616d 653d 6e61           name=na
+00002be0: 6d65 2c0d 0a20 2020 2020 2020 2020 2020  me,..           
+00002bf0: 2020 2020 2020 2020 2020 2020 206d 6574               met
+00002c00: 7269 633d 7061 7274 6961 6c28 4445 4641  ric=partial(DEFA
+00002c10: 554c 545f 4d45 5452 4943 535b 6c61 7374  ULT_METRICS[last
+00002c20: 6e61 6d65 5d2c 202a 2a6b 7761 7267 7329  name], **kwargs)
+00002c30: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00002c40: 2020 2020 2020 2020 2020 2066 6d74 3d44             fmt=D
+00002c50: 4546 4155 4c54 5f46 4d54 535b 6c61 7374  EFAULT_FMTS[last
+00002c60: 6e61 6d65 5d2c 0d0a 2020 2020 2020 2020  name],..        
+00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c80: 6265 7374 5f63 6173 7465 723d 4445 4641  best_caster=DEFA
+00002c90: 554c 545f 4245 5354 5f43 4153 5445 525b  ULT_BEST_CASTER[
+00002ca0: 6c61 7374 6e61 6d65 5d0d 0a20 2020 2020  lastname]..     
+00002cb0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00002cc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002cd0: 2020 7365 6c66 2e5f 5f6d 6f6e 6974 6f72    self.__monitor
+00002ce0: 735b 7072 6566 6978 5d5b 6c61 7374 6e61  s[prefix][lastna
+00002cf0: 6d65 5d2e 6170 7065 6e64 286d 6574 6572  me].append(meter
+00002d00: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+00002d10: 7863 6570 7420 4b65 7945 7272 6f72 3a0d  xcept KeyError:.
+00002d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002d30: 2072 6169 7365 204b 6579 4572 726f 7228   raise KeyError(
+00002d40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002d50: 2020 2020 2020 6622 5468 6520 6d65 7472        f"The metr
+00002d60: 6963 206f 6620 7b6c 6173 746e 616d 657d  ic of {lastname}
+00002d70: 2069 7320 6e6f 7420 696e 636c 7564 6564   is not included
+00002d80: 2e20 220d 0a20 2020 2020 2020 2020 2020  . "..           
+00002d90: 2020 2020 2020 2020 2066 2259 6f75 2063           f"You c
+00002da0: 616e 2072 6567 6973 7465 7220 6279 2063  an register by c
+00002db0: 616c 6c69 6e67 2060 7265 6769 7374 6572  alling `register
+00002dc0: 5f6d 6574 7269 6328 2e2e 2e29 2720 2e2e  _metric(...)' ..
+00002dd0: 2e22 0d0a 2020 2020 2020 2020 2020 2020  ."..            
+00002de0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+00002df0: 2020 2072 6574 7572 6e20 6d65 7465 720d     return meter.
+00002e00: 0a0d 0a20 2020 2020 2020 2023 2055 5050  ...        # UPP
+00002e10: 4552 0d0a 2020 2020 2020 2020 7768 6963  ER..        whic
+00002e20: 6834 6265 7374 203d 2077 6869 6368 3462  h4best = which4b
+00002e30: 6573 742e 7570 7065 7228 290d 0a20 2020  est.upper()..   
+00002e40: 2020 2020 206d 6f6e 6974 6f72 7320 3d20       monitors = 
+00002e50: 5b27 4c4f 5353 275d 202b 205b 6e61 6d65  ['LOSS'] + [name
+00002e60: 2e75 7070 6572 2829 2066 6f72 206e 616d  .upper() for nam
+00002e70: 6520 696e 206d 6f6e 6974 6f72 735d 202b  e in monitors] +
+00002e80: 205b 7768 6963 6834 6265 7374 5d0d 0a20   [which4best].. 
+00002e90: 2020 2020 2020 206d 6f6e 6974 6f72 7320         monitors 
+00002ea0: 3d20 736f 7274 6564 2873 6574 286d 6f6e  = sorted(set(mon
+00002eb0: 6974 6f72 7329 2c20 6b65 793d 6d6f 6e69  itors), key=moni
+00002ec0: 746f 7273 2e69 6e64 6578 290d 0a0d 0a20  tors.index).... 
+00002ed0: 2020 2020 2020 2066 6f72 206e 616d 6520         for name 
+00002ee0: 696e 206d 6f6e 6974 6f72 733a 0d0a 2020  in monitors:..  
+00002ef0: 2020 2020 2020 2020 2020 666f 7220 7072            for pr
+00002f00: 6566 6978 2069 6e20 2827 7472 6169 6e27  efix in ('train'
+00002f10: 2c20 2776 616c 6964 272c 2027 7465 7374  , 'valid', 'test
+00002f20: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
+00002f30: 2020 2020 2069 6620 2740 2720 696e 206e       if '@' in n
+00002f40: 616d 653a 0d0a 2020 2020 2020 2020 2020  ame:..          
+00002f50: 2020 2020 2020 2020 2020 6c61 7374 6e61            lastna
+00002f60: 6d65 2c20 4b20 3d20 6e61 6d65 2e73 706c  me, K = name.spl
+00002f70: 6974 2827 4027 290d 0a20 2020 2020 2020  it('@')..       
+00002f80: 2020 2020 2020 2020 2020 2020 206d 6574               met
+00002f90: 6572 203d 2073 6574 5f6d 6f6e 6974 6f72  er = set_monitor
+00002fa0: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00002fb0: 2020 2020 2020 2020 2020 206e 616d 653d             name=
+00002fc0: 6e61 6d65 2c0d 0a20 2020 2020 2020 2020  name,..         
+00002fd0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00002fe0: 6173 746e 616d 653d 6c61 7374 6e61 6d65  astname=lastname
+00002ff0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003000: 2020 2020 2020 2020 2020 2070 7265 6669             prefi
+00003010: 783d 7072 6566 6978 2c0d 0a20 2020 2020  x=prefix,..     
+00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003030: 2020 206b 3d69 6e74 284b 290d 0a20 2020     k=int(K)..   
+00003040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003050: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+00003060: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00003070: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00003080: 6173 746e 616d 6520 3d20 6e61 6d65 0d0a  astname = name..
+00003090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030a0: 2020 2020 6d65 7465 7220 3d20 7365 745f      meter = set_
+000030b0: 6d6f 6e69 746f 7228 0d0a 2020 2020 2020  monitor(..      
+000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030d0: 2020 6e61 6d65 3d6e 616d 652c 0d0a 2020    name=name,..  
+000030e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030f0: 2020 2020 2020 6c61 7374 6e61 6d65 3d6c        lastname=l
+00003100: 6173 746e 616d 652c 0d0a 2020 2020 2020  astname,..      
+00003110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003120: 2020 7072 6566 6978 3d70 7265 6669 780d    prefix=prefix.
+00003130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003140: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00003150: 2020 2020 2020 2020 6966 2070 7265 6669          if prefi
+00003160: 7820 3d3d 2027 7661 6c69 6427 2061 6e64  x == 'valid' and
+00003170: 206e 616d 6520 3d3d 2077 6869 6368 3462   name == which4b
+00003180: 6573 743a 0d0a 2020 2020 2020 2020 2020  est:..          
+00003190: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+000031a0: 6574 6572 3462 6573 7420 3d20 6d65 7465  eter4best = mete
+000031b0: 720d 0a20 2020 2020 2020 2020 2020 2020  r..             
+000031c0: 2020 2020 2020 2073 656c 662e 5f62 6573         self._bes
+000031d0: 7420 3d20 2d66 6c6f 6174 2827 696e 6627  t = -float('inf'
+000031e0: 2920 6966 206d 6574 6572 2e63 6173 7465  ) if meter.caste
+000031f0: 7220 6973 206d 6178 2065 6c73 6520 666c  r is max else fl
+00003200: 6f61 7428 2769 6e66 2729 0d0a 2020 2020  oat('inf')..    
+00003210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003220: 7365 6c66 2e5f 6265 7374 5f65 706f 6368  self._best_epoch
+00003230: 203d 2030 0d0a 0d0a 2020 2020 2020 2020   = 0....        
+00003240: 2320 5072 6570 6172 6520 6461 7461 206c  # Prepare data l
+00003250: 6f61 6465 7273 0d0a 2020 2020 2020 2020  oaders..        
+00003260: 7365 6c66 2e70 7265 7061 7265 5f64 6174  self.prepare_dat
+00003270: 616c 6f61 6465 7228 290d 0a0d 0a20 2020  aloader()....   
+00003280: 2064 6566 2073 6176 6528 7365 6c66 2920   def save(self) 
+00003290: 2d3e 204e 6f6e 653a 0d0a 2020 2020 2020  -> None:..      
+000032a0: 2020 2222 2253 6176 6520 7468 6520 6d6f    """Save the mo
+000032b0: 6465 6c22 2222 0d0a 2020 2020 2020 2020  del"""..        
+000032c0: 746f 7263 682e 7361 7665 2873 656c 662e  torch.save(self.
+000032d0: 6d6f 6465 6c2e 7374 6174 655f 6469 6374  model.state_dict
+000032e0: 2829 2c20 6f73 2e70 6174 682e 6a6f 696e  (), os.path.join
+000032f0: 2873 656c 662e 6366 672e 4c4f 475f 5041  (self.cfg.LOG_PA
+00003300: 5448 2c20 7365 6c66 2e63 6667 2e53 4156  TH, self.cfg.SAV
+00003310: 4544 5f46 494c 454e 414d 4529 290d 0a0d  ED_FILENAME))...
+00003320: 0a20 2020 2064 6566 206c 6f61 6428 7365  .    def load(se
+00003330: 6c66 2c20 7061 7468 3a20 7374 722c 2066  lf, path: str, f
+00003340: 696c 656e 616d 653a 204f 7074 696f 6e61  ilename: Optiona
+00003350: 6c5b 7374 725d 203d 204e 6f6e 652c 202a  l[str] = None, *
+00003360: 2a6b 7761 7267 7329 202d 3e20 4e6f 6e65  *kwargs) -> None
+00003370: 3a0d 0a20 2020 2020 2020 2066 696c 656e  :..        filen
+00003380: 616d 6520 3d20 7365 6c66 2e63 6667 2e53  ame = self.cfg.S
+00003390: 4156 4544 5f46 494c 454e 414d 4520 6966  AVED_FILENAME if
+000033a0: 2066 696c 656e 616d 6520 6973 204e 6f6e   filename is Non
+000033b0: 6520 656c 7365 2066 696c 656e 616d 650d  e else filename.
+000033c0: 0a20 2020 2020 2020 2073 656c 662e 6d6f  .        self.mo
+000033d0: 6465 6c2e 6c6f 6164 5f73 7461 7465 5f64  del.load_state_d
+000033e0: 6963 7428 746f 7263 682e 6c6f 6164 286f  ict(torch.load(o
+000033f0: 732e 7061 7468 2e6a 6f69 6e28 7061 7468  s.path.join(path
+00003400: 2c20 6669 6c65 6e61 6d65 292c 202a 2a6b  , filename), **k
+00003410: 7761 7267 7329 290d 0a0d 0a20 2020 2064  wargs))....    d
+00003420: 6566 2073 6176 655f 6368 6563 6b70 6f69  ef save_checkpoi
+00003430: 6e74 2873 656c 662c 2065 706f 6368 3a20  nt(self, epoch: 
+00003440: 696e 7429 202d 3e20 4e6f 6e65 3a0d 0a20  int) -> None:.. 
+00003450: 2020 2020 2020 2072 2222 220d 0a20 2020         r"""..   
+00003460: 2020 2020 2053 6176 6520 6375 7272 656e       Save curren
+00003470: 7420 6368 6563 6b70 6f69 6e74 2061 7420  t checkpoint at 
+00003480: 6570 6f63 682e 0d0a 0d0a 2020 2020 2020  epoch.....      
+00003490: 2020 5061 7261 6d65 7465 7273 3a0d 0a20    Parameters:.. 
+000034a0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+000034b0: 2d2d 0d0a 2020 2020 2020 2020 2020 2020  --..            
+000034c0: 6570 6f63 6820 3a69 6e74 2043 7572 7265  epoch :int Curre
+000034d0: 6e74 2065 706f 6368 206e 756d 6265 722e  nt epoch number.
+000034e0: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
+000034f0: 726e 733a 0d0a 2020 2020 2020 2020 2d2d  rns:..        --
+00003500: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+00003510: 2020 2020 4e6f 6e65 0d0a 2020 2020 2020      None..      
+00003520: 2020 2222 220d 0a20 2020 2020 2020 2070    """..        p
+00003530: 6174 6820 3d20 6f73 2e70 6174 682e 6a6f  ath = os.path.jo
+00003540: 696e 2873 656c 662e 6366 672e 4348 4543  in(self.cfg.CHEC
+00003550: 4b50 4f49 4e54 5f50 4154 482c 2073 656c  KPOINT_PATH, sel
+00003560: 662e 6366 672e 4348 4543 4b50 4f49 4e54  f.cfg.CHECKPOINT
+00003570: 5f46 494c 454e 414d 4529 0d0a 2020 2020  _FILENAME)..    
+00003580: 2020 2020 6368 6563 6b70 6f69 6e74 203d      checkpoint =
+00003590: 2064 6963 7428 290d 0a20 2020 2020 2020   dict()..       
+000035a0: 2063 6865 636b 706f 696e 745b 2765 706f   checkpoint['epo
+000035b0: 6368 275d 203d 2065 706f 6368 0d0a 2020  ch'] = epoch..  
+000035c0: 2020 2020 2020 666f 7220 6d6f 6475 6c65        for module
+000035d0: 2069 6e20 7365 6c66 2e63 6667 2e43 4845   in self.cfg.CHE
+000035e0: 434b 504f 494e 545f 4d4f 4455 4c45 533a  CKPOINT_MODULES:
+000035f0: 0d0a 2020 2020 2020 2020 2020 2020 6368  ..            ch
+00003600: 6563 6b70 6f69 6e74 5b6d 6f64 756c 655d  eckpoint[module]
+00003610: 203d 2067 6574 6174 7472 2873 656c 662c   = getattr(self,
+00003620: 206d 6f64 756c 6529 2e73 7461 7465 5f64   module).state_d
+00003630: 6963 7428 290d 0a20 2020 2020 2020 2063  ict()..        c
+00003640: 6865 636b 706f 696e 745b 276d 6f6e 6974  heckpoint['monit
+00003650: 6f72 7327 5d20 3d20 7365 6c66 2e6d 6f6e  ors'] = self.mon
+00003660: 6974 6f72 732e 7374 6174 655f 6469 6374  itors.state_dict
+00003670: 2829 0d0a 2020 2020 2020 2020 746f 7263  ()..        torc
+00003680: 682e 7361 7665 2863 6865 636b 706f 696e  h.save(checkpoin
+00003690: 742c 2070 6174 6829 0d0a 0d0a 2020 2020  t, path)....    
+000036a0: 6465 6620 6c6f 6164 5f63 6865 636b 706f  def load_checkpo
+000036b0: 696e 7428 7365 6c66 2920 2d3e 2069 6e74  int(self) -> int
+000036c0: 3a0d 0a20 2020 2020 2020 2072 2222 220d  :..        r""".
+000036d0: 0a20 2020 2020 2020 204c 6f61 6420 6c61  .        Load la
+000036e0: 7374 2073 6176 6564 2063 6865 636b 706f  st saved checkpo
+000036f0: 696e 742e 0d0a 0d0a 2020 2020 2020 2020  int.....        
+00003700: 5265 7475 726e 733a 0d0a 2020 2020 2020  Returns:..      
+00003710: 2020 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020    --------..    
+00003720: 2020 2020 6570 6f63 683a 2069 6e74 200d      epoch: int .
+00003730: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00003740: 2065 706f 6368 206e 756d 6265 7220 6c6f   epoch number lo
+00003750: 6164 6564 2066 726f 6d20 7468 6520 6368  aded from the ch
+00003760: 6563 6b70 6f69 6e74 2e0d 0a20 2020 2020  eckpoint...     
+00003770: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00003780: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
+00003790: 6f69 6e28 7365 6c66 2e63 6667 2e43 4845  oin(self.cfg.CHE
+000037a0: 434b 504f 494e 545f 5041 5448 2c20 7365  CKPOINT_PATH, se
+000037b0: 6c66 2e63 6667 2e43 4845 434b 504f 494e  lf.cfg.CHECKPOIN
+000037c0: 545f 4649 4c45 4e41 4d45 290d 0a20 2020  T_FILENAME)..   
+000037d0: 2020 2020 2063 6865 636b 706f 696e 7420       checkpoint 
+000037e0: 3d20 746f 7263 682e 6c6f 6164 2870 6174  = torch.load(pat
+000037f0: 6829 0d0a 2020 2020 2020 2020 666f 7220  h)..        for 
+00003800: 6d6f 6475 6c65 2069 6e20 7365 6c66 2e63  module in self.c
+00003810: 6667 2e43 4845 434b 504f 494e 545f 4d4f  fg.CHECKPOINT_MO
+00003820: 4455 4c45 533a 0d0a 2020 2020 2020 2020  DULES:..        
+00003830: 2020 2020 6765 7461 7474 7228 7365 6c66      getattr(self
+00003840: 2c20 6d6f 6475 6c65 292e 6c6f 6164 5f73  , module).load_s
+00003850: 7461 7465 5f64 6963 7428 6368 6563 6b70  tate_dict(checkp
+00003860: 6f69 6e74 5b6d 6f64 756c 655d 290d 0a20  oint[module]).. 
+00003870: 2020 2020 2020 2073 656c 662e 6d6f 6e69         self.moni
+00003880: 746f 7273 2e6c 6f61 645f 7374 6174 655f  tors.load_state_
+00003890: 6469 6374 2863 6865 636b 706f 696e 745b  dict(checkpoint[
+000038a0: 276d 6f6e 6974 6f72 7327 5d29 0d0a 2020  'monitors'])..  
+000038b0: 2020 2020 2020 7265 7475 726e 2063 6865        return che
+000038c0: 636b 706f 696e 745b 2765 706f 6368 275d  ckpoint['epoch']
+000038d0: 0d0a 0d0a 2020 2020 6465 6620 7361 7665  ....    def save
+000038e0: 5f62 6573 7428 7365 6c66 2920 2d3e 204e  _best(self) -> N
+000038f0: 6f6e 653a 0d0a 2020 2020 2020 2020 746f  one:..        to
+00003900: 7263 682e 7361 7665 2873 656c 662e 6d6f  rch.save(self.mo
+00003910: 6465 6c2e 7374 6174 655f 6469 6374 2829  del.state_dict()
+00003920: 2c20 6f73 2e70 6174 682e 6a6f 696e 2873  , os.path.join(s
+00003930: 656c 662e 6366 672e 4c4f 475f 5041 5448  elf.cfg.LOG_PATH
+00003940: 2c20 7365 6c66 2e63 6667 2e42 4553 545f  , self.cfg.BEST_
+00003950: 4649 4c45 4e41 4d45 2929 0d0a 0d0a 2020  FILENAME))....  
+00003960: 2020 6465 6620 6c6f 6164 5f62 6573 7428    def load_best(
+00003970: 7365 6c66 2920 2d3e 204e 6f6e 653a 0d0a  self) -> None:..
+00003980: 2020 2020 2020 2020 696e 666f 4c6f 6767          infoLogg
+00003990: 6572 2866 225b 436f 6163 685d 203e 3e3e  er(f"[Coach] >>>
+000039a0: 204c 6f61 6420 6265 7374 206d 6f64 656c   Load best model
+000039b0: 2040 4570 6f63 6820 7b73 656c 662e 5f62   @Epoch {self._b
+000039c0: 6573 745f 6570 6f63 683a 3c34 647d 2022  est_epoch:<4d} "
+000039d0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000039e0: 6d6f 6465 6c2e 6c6f 6164 5f73 7461 7465  model.load_state
+000039f0: 5f64 6963 7428 746f 7263 682e 6c6f 6164  _dict(torch.load
+00003a00: 286f 732e 7061 7468 2e6a 6f69 6e28 7365  (os.path.join(se
+00003a10: 6c66 2e63 6667 2e4c 4f47 5f50 4154 482c  lf.cfg.LOG_PATH,
+00003a20: 2073 656c 662e 6366 672e 4245 5354 5f46   self.cfg.BEST_F
+00003a30: 494c 454e 414d 4529 2929 0d0a 0d0a 2020  ILENAME)))....  
+00003a40: 2020 6465 6620 6368 6563 6b5f 6265 7374    def check_best
+00003a50: 2873 656c 662c 2065 706f 6368 3a20 696e  (self, epoch: in
+00003a60: 7429 202d 3e20 4e6f 6e65 3a0d 0a20 2020  t) -> None:..   
+00003a70: 2020 2020 2022 2222 5570 6461 7465 2062       """Update b
+00003a80: 6573 7420 7661 6c75 652e 2222 220d 0a20  est value.""".. 
+00003a90: 2020 2020 2020 2069 6620 7365 6c66 2e6d         if self.m
+00003aa0: 6574 6572 3462 6573 742e 6163 7469 7665  eter4best.active
+00003ab0: 3a0d 0a20 2020 2020 2020 2020 2020 2062  :..            b
+00003ac0: 6573 745f 203d 2073 656c 662e 6d65 7465  est_ = self.mete
+00003ad0: 7234 6265 7374 2e77 6869 6368 5f69 735f  r4best.which_is_
+00003ae0: 6265 7474 6572 2873 656c 662e 5f62 6573  better(self._bes
+00003af0: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+00003b00: 6966 2062 6573 745f 2021 3d20 7365 6c66  if best_ != self
+00003b10: 2e5f 6265 7374 3a0d 0a20 2020 2020 2020  ._best:..       
+00003b20: 2020 2020 2020 2020 2073 656c 662e 5f62           self._b
+00003b30: 6573 7420 3d20 6265 7374 5f0d 0a20 2020  est = best_..   
+00003b40: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00003b50: 662e 5f62 6573 745f 6570 6f63 6820 3d20  f._best_epoch = 
+00003b60: 6570 6f63 680d 0a20 2020 2020 2020 2020  epoch..         
+00003b70: 2020 2020 2020 2069 6e66 6f4c 6f67 6765         infoLogge
+00003b80: 7228 6622 5b43 6f61 6368 5d20 3e3e 3e20  r(f"[Coach] >>> 
+00003b90: 4265 7474 6572 202a 2a2a 7b73 656c 662e  Better ***{self.
+00003ba0: 6d65 7465 7234 6265 7374 2e6e 616d 657d  meter4best.name}
+00003bb0: 2a2a 2a20 6f66 202a 2a2a 7b73 656c 662e  *** of ***{self.
+00003bc0: 5f62 6573 743a 2e34 667d 2a2a 2a20 2229  _best:.4f}*** ")
+00003bd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003be0: 2020 7365 6c66 2e73 6176 655f 6265 7374    self.save_best
+00003bf0: 2829 0d0a 0d0a 2020 2020 6465 6620 6576  ()....    def ev
+00003c00: 616c 5f61 745f 6265 7374 2873 656c 6629  al_at_best(self)
+00003c10: 3a0d 0a20 2020 2020 2020 2074 7279 3a0d  :..        try:.
+00003c20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00003c30: 662e 6c6f 6164 5f62 6573 7428 290d 0a20  f.load_best().. 
+00003c40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003c50: 7661 6c69 6428 7365 6c66 2e5f 6265 7374  valid(self._best
+00003c60: 5f65 706f 6368 290d 0a20 2020 2020 2020  _epoch)..       
+00003c70: 2020 2020 2073 656c 662e 7465 7374 2873       self.test(s
+00003c80: 656c 662e 5f62 6573 745f 6570 6f63 6829  elf._best_epoch)
+00003c90: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00003ca0: 6c66 2e73 7465 7028 7365 6c66 2e5f 6265  lf.step(self._be
+00003cb0: 7374 5f65 706f 6368 290d 0a20 2020 2020  st_epoch)..     
+00003cc0: 2020 2020 2020 2073 656c 662e 6c6f 6164         self.load
+00003cd0: 2873 656c 662e 6366 672e 4c4f 475f 5041  (self.cfg.LOG_PA
+00003ce0: 5448 2c20 7365 6c66 2e63 6667 2e53 4156  TH, self.cfg.SAV
+00003cf0: 4544 5f46 494c 454e 414d 4529 0d0a 2020  ED_FILENAME)..  
+00003d00: 2020 2020 2020 6578 6365 7074 2046 696c        except Fil
+00003d10: 654e 6f74 466f 756e 6445 7272 6f72 3a0d  eNotFoundError:.
+00003d20: 0a20 2020 2020 2020 2020 2020 2069 6e66  .            inf
+00003d30: 6f4c 6f67 6765 7228 6622 5b43 6f61 6368  oLogger(f"[Coach
+00003d40: 5d20 3e3e 3e20 4e6f 2062 6573 7420 6d6f  ] >>> No best mo
+00003d50: 6465 6c20 7761 7320 7265 636f 7264 6564  del was recorded
+00003d60: 2e20 536b 6970 2069 7420 2e2e 2e22 290d  . Skip it ...").
+00003d70: 0a0d 0a20 2020 2064 6566 2072 6573 756d  ...    def resum
+00003d80: 6528 7365 6c66 2920 2d3e 2069 6e74 3a0d  e(self) -> int:.
+00003d90: 0a20 2020 2020 2020 2072 2222 220d 0a20  .        r""".. 
+00003da0: 2020 2020 2020 2052 6573 756d 6520 7472         Resume tr
+00003db0: 6169 6e69 6e67 2066 726f 6d20 7468 6520  aining from the 
+00003dc0: 6c61 7374 2063 6865 636b 706f 696e 742e  last checkpoint.
+00003dd0: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
+00003de0: 726e 733a 0d0a 2020 2020 2020 2020 2d2d  rns:..        --
+00003df0: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
+00003e00: 7374 6172 745f 6570 6f63 683a 2069 6e74  start_epoch: int
+00003e10: 0d0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+00003e20: 6520 6570 6f63 6820 6e75 6d62 6572 2074  e epoch number t
+00003e30: 6f20 7265 7375 6d65 2074 7261 696e 696e  o resume trainin
+00003e40: 6720 6672 6f6d 2e0d 0a20 2020 2020 2020  g from...       
+00003e50: 2022 2222 0d0a 2020 2020 2020 2020 7374   """..        st
+00003e60: 6172 745f 6570 6f63 683a 2069 6e74 203d  art_epoch: int =
+00003e70: 2030 0d0a 2020 2020 2020 2020 6966 2073   0..        if s
+00003e80: 656c 662e 6366 672e 7265 7375 6d65 3a0d  elf.cfg.resume:.
+00003e90: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+00003ea0: 7274 5f65 706f 6368 203d 2073 656c 662e  rt_epoch = self.
+00003eb0: 6c6f 6164 5f63 6865 636b 706f 696e 7428  load_checkpoint(
+00003ec0: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00003ed0: 6e66 6f4c 6f67 6765 7228 6622 5b43 6f61  nfoLogger(f"[Coa
+00003ee0: 6368 5d20 3e3e 3e20 4c6f 6164 206c 6173  ch] >>> Load las
+00003ef0: 7420 6368 6563 6b70 6f69 6e74 2061 6e64  t checkpoint and
+00003f00: 2074 7261 696e 2066 726f 6d20 6570 6f63   train from epoc
+00003f10: 683a 207b 7374 6172 745f 6570 6f63 687d  h: {start_epoch}
+00003f20: 2229 0d0a 2020 2020 2020 2020 7265 7475  ")..        retu
+00003f30: 726e 2073 7461 7274 5f65 706f 6368 0d0a  rn start_epoch..
+00003f40: 0d0a 2020 2020 4074 6f72 6368 2e6e 6f5f  ..    @torch.no_
+00003f50: 6772 6164 2829 0d0a 2020 2020 6465 6620  grad()..    def 
+00003f60: 6d6f 6e69 746f 7228 0d0a 2020 2020 2020  monitor(..      
+00003f70: 2020 7365 6c66 2c20 2a76 616c 7565 732c    self, *values,
+00003f80: 0d0a 2020 2020 2020 2020 6e3a 2069 6e74  ..        n: int
+00003f90: 203d 2031 2c20 6d6f 6465 3a20 7374 7220   = 1, mode: str 
+00003fa0: 3d20 276d 6561 6e27 2c20 0d0a 2020 2020  = 'mean', ..    
+00003fb0: 2020 2020 7072 6566 6978 3a20 7374 7220      prefix: str 
+00003fc0: 3d20 2774 7261 696e 272c 2070 6f6f 6c3a  = 'train', pool:
+00003fd0: 204f 7074 696f 6e61 6c5b 4974 6572 6162   Optional[Iterab
+00003fe0: 6c65 5d20 3d20 4e6f 6e65 0d0a 2020 2020  le] = None..    
+00003ff0: 293a 0d0a 0d0a 2020 2020 2020 2020 7222  ):....        r"
+00004000: 2222 0d0a 2020 2020 2020 2020 4c6f 6720  ""..        Log 
+00004010: 6461 7461 2076 616c 7565 7320 746f 2073  data values to s
+00004020: 7065 6369 6669 6320 6d6f 6e69 746f 7273  pecific monitors
+00004030: 2e0d 0a0d 0a20 2020 2020 2020 2050 6172  .....        Par
+00004040: 616d 6574 6572 733a 0d0a 2020 2020 2020  ameters:..      
+00004050: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20    -----------.. 
+00004060: 2020 2020 2020 202a 7661 6c75 6573 203a         *values :
+00004070: 2064 6174 610d 0a20 2020 2020 2020 2020   data..         
+00004080: 2020 2054 6865 2064 6174 6120 7661 6c75     The data valu
+00004090: 6573 2074 6f20 6265 206c 6f67 6765 642e  es to be logged.
+000040a0: 0d0a 2020 2020 2020 2020 6e20 3a20 696e  ..        n : in
+000040b0: 740d 0a20 2020 2020 2020 2020 2020 2054  t..            T
+000040c0: 6865 2062 6174 6368 2073 697a 6520 696e  he batch size in
+000040d0: 2067 656e 6572 616c 2e0d 0a20 2020 2020   general...     
+000040e0: 2020 206d 6f64 6520 3a20 7374 722c 206f     mode : str, o
+000040f0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+00004100: 2020 2020 2054 6865 206d 6f64 6520 746f       The mode to
+00004110: 2063 6f6d 7075 7465 2074 6865 206d 6574   compute the met
+00004120: 7269 632e 2043 616e 2062 6520 2773 756d  ric. Can be 'sum
+00004130: 2720 6f72 2027 6d65 616e 2720 2864 6566  ' or 'mean' (def
+00004140: 6175 6c74 292e 0d0a 2020 2020 2020 2020  ault)...        
+00004150: 7072 6566 6978 203a 2073 7472 2c20 6f70  prefix : str, op
+00004160: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+00004170: 2020 2020 5468 6520 7072 6566 6978 2073      The prefix s
+00004180: 7472 696e 6720 696e 6469 6361 7469 6e67  tring indicating
+00004190: 2077 6869 6368 206d 6f64 6520 7468 6520   which mode the 
+000041a0: 7661 6c75 6573 2062 656c 6f6e 6720 746f  values belong to
+000041b0: 2e20 4361 6e20 6265 2027 7472 6169 6e27  . Can be 'train'
+000041c0: 2c20 2774 6573 7427 206f 7220 2776 616c  , 'test' or 'val
+000041d0: 6964 272e 0d0a 2020 2020 2020 2020 706f  id'...        po
+000041e0: 6f6c 203a 204c 6973 745b 7374 725d 2c20  ol : List[str], 
+000041f0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
+00004200: 2020 2020 2020 4120 6c69 7374 206f 6620        A list of 
+00004210: 6d65 7472 6963 206e 616d 6573 2074 6f20  metric names to 
+00004220: 6c6f 672e 2049 6620 4e6f 6e65 2c20 616c  log. If None, al
+00004230: 6c20 6d65 7472 6963 7320 696e 2074 6865  l metrics in the
+00004240: 2070 6f6f 6c20 6f66 2060 7072 6566 6978   pool of `prefix
+00004250: 6020 7769 6c6c 2062 6520 6c6f 6767 6564  ` will be logged
+00004260: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+00004270: 0d0a 2020 2020 2020 2020 6d65 7472 6963  ..        metric
+00004280: 733a 2044 6963 745b 4c69 7374 5d20 3d20  s: Dict[List] = 
+00004290: 7365 6c66 2e6d 6f6e 6974 6f72 735b 7072  self.monitors[pr
+000042a0: 6566 6978 5d0d 0a20 2020 2020 2020 2070  efix]..        p
+000042b0: 6f6f 6c20 3d20 6d65 7472 6963 7320 6966  ool = metrics if
+000042c0: 2070 6f6f 6c20 6973 204e 6f6e 6520 656c   pool is None el
+000042d0: 7365 2070 6f6f 6c0d 0a20 2020 2020 2020  se pool..       
+000042e0: 2066 6f72 206c 6173 746e 616d 6520 696e   for lastname in
+000042f0: 2070 6f6f 6c3a 0d0a 2020 2020 2020 2020   pool:..        
+00004300: 2020 2020 666f 7220 6d65 7465 7220 696e      for meter in
+00004310: 206d 6574 7269 6373 2e67 6574 286c 6173   metrics.get(las
+00004320: 746e 616d 652e 7570 7065 7228 292c 205b  tname.upper(), [
+00004330: 5d29 3a0d 0a20 2020 2020 2020 2020 2020  ]):..           
+00004340: 2020 2020 206d 6574 6572 282a 7661 6c75       meter(*valu
+00004350: 6573 2c20 6e3d 6e2c 206d 6f64 653d 6d6f  es, n=n, mode=mo
+00004360: 6465 290d 0a0d 0a20 2020 2064 6566 2073  de)....    def s
+00004370: 7465 7028 7365 6c66 2c20 6570 6f63 683a  tep(self, epoch:
+00004380: 2069 6e74 293a 0d0a 2020 2020 2020 2020   int):..        
+00004390: 7222 2222 0d0a 2020 2020 2020 2020 5072  r"""..        Pr
+000043a0: 696e 7473 2074 7261 696e 696e 6720 7374  ints training st
+000043b0: 6174 7573 2061 6e64 2065 7661 6c75 6174  atus and evaluat
+000043c0: 696f 6e20 7265 7375 6c74 7320 666f 7220  ion results for 
+000043d0: 6561 6368 2065 706f 6368 2c20 0d0a 2020  each epoch, ..  
+000043e0: 2020 2020 2020 616e 6420 7265 7365 7473        and resets
+000043f0: 2074 6865 2063 6f72 7265 7370 6f6e 6469   the correspondi
+00004400: 6e67 2060 4176 6572 6167 654d 6574 6572  ng `AverageMeter
+00004410: 6020 696e 7374 616e 6365 732e 0d0a 0d0a  ` instances.....
+00004420: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00004430: 7273 3a0d 0a20 2020 2020 2020 202d 2d2d  rs:..        ---
+00004440: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
+00004450: 2020 6570 6f63 6820 3a20 696e 740d 0a20    epoch : int.. 
+00004460: 2020 2020 2020 2020 2020 2054 6865 2065             The e
+00004470: 706f 6368 206e 756d 6265 722e 0d0a 0d0a  poch number.....
+00004480: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00004490: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+000044a0: 2d2d 0d0a 2020 2020 2020 2020 4e6f 6e65  --..        None
+000044b0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+000044c0: 2020 2020 2020 206d 6574 7269 6373 3a20         metrics: 
+000044d0: 4469 6374 5b73 7472 2c20 4c69 7374 5b41  Dict[str, List[A
+000044e0: 7665 7261 6765 4d65 7465 725d 5d0d 0a20  verageMeter]].. 
+000044f0: 2020 2020 2020 2066 6f72 2070 7265 6669         for prefi
+00004500: 782c 206d 6574 7269 6373 2069 6e20 7365  x, metrics in se
+00004510: 6c66 2e6d 6f6e 6974 6f72 732e 6974 656d  lf.monitors.item
+00004520: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
+00004530: 2020 696e 666f 7320 3d20 5b66 225b 436f    infos = [f"[Co
+00004540: 6163 685d 203e 3e3e 207b 7072 6566 6978  ach] >>> {prefix
+00004550: 2e75 7070 6572 2829 3a35 7d20 4045 706f  .upper():5} @Epo
+00004560: 6368 3a20 7b65 706f 6368 3a3c 3464 7d20  ch: {epoch:<4d} 
+00004570: 3e3e 3e20 225d 0d0a 2020 2020 2020 2020  >>> "]..        
+00004580: 2020 2020 666f 7220 6d65 7465 7273 2069      for meters i
+00004590: 6e20 6d65 7472 6963 732e 7661 6c75 6573  n metrics.values
+000045a0: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+000045b0: 2020 2020 2069 6e66 6f73 202b 3d20 5b6d       infos += [m
+000045c0: 6574 6572 2e73 7465 7028 2920 666f 7220  eter.step() for 
+000045d0: 6d65 7465 7220 696e 206d 6574 6572 7320  meter in meters 
+000045e0: 6966 206d 6574 6572 2e61 6374 6976 655d  if meter.active]
+000045f0: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
+00004600: 666f 4c6f 6767 6572 2827 207c 7c20 272e  foLogger(' || '.
+00004610: 6a6f 696e 2869 6e66 6f73 2929 0d0a 0d0a  join(infos))....
+00004620: 2020 2020 4074 696d 656d 6574 6572 2822      @timemeter("
+00004630: 436f 6163 682f 7375 6d6d 6172 7922 290d  Coach/summary").
+00004640: 0a20 2020 2064 6566 2073 756d 6d61 7279  .    def summary
+00004650: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00004660: 2072 2222 220d 0a20 2020 2020 2020 2053   r"""..        S
+00004670: 756d 6d61 7279 2074 6865 2077 686f 6c65  ummary the whole
+00004680: 2074 7261 696e 696e 6720 7072 6f63 6573   training proces
+00004690: 732e 0d0a 0d0a 2020 2020 2020 2020 4765  s.....        Ge
+000046a0: 6e65 7261 7465 2061 2073 756d 6d61 7279  nerate a summary
+000046b0: 206f 6620 7468 6520 656e 7469 7265 2074   of the entire t
+000046c0: 7261 696e 696e 6720 7072 6f63 6573 732c  raining process,
+000046d0: 2069 6e63 6c75 6469 6e67 2074 6865 2068   including the h
+000046e0: 6973 746f 7269 6361 6c20 6576 616c 7561  istorical evalua
+000046f0: 7469 6f6e 2072 6573 756c 7473 2c20 7468  tion results, th
+00004700: 6520 6265 7374 0d0a 2020 2020 2020 2020  e best..        
+00004710: 6869 7374 6f72 6963 616c 2072 6573 756c  historical resul
+00004720: 7473 2c20 616e 6420 7468 6520 6375 7276  ts, and the curv
+00004730: 6573 206f 6620 6869 7374 6f72 6963 616c  es of historical
+00004740: 2072 6573 756c 7473 2e20 5468 6520 7265   results. The re
+00004750: 7375 6c74 696e 6720 7375 6d6d 6172 7920  sulting summary 
+00004760: 6973 2073 6176 6564 2074 6f20 6120 4d61  is saved to a Ma
+00004770: 726b 646f 776e 2066 696c 6520 6e61 6d65  rkdown file name
+00004780: 640d 0a20 2020 2020 2020 2022 5375 6d6d  d..        "Summ
+00004790: 6172 792e 6d64 2220 696e 2074 6865 2060  ary.md" in the `
+000047a0: 7365 6c66 2e63 6667 2e4c 4f47 5f50 4154  self.cfg.LOG_PAT
+000047b0: 4860 2064 6972 6563 746f 7279 2e0d 0a0d  H` directory....
+000047c0: 0a20 2020 2020 2020 2041 6464 6974 696f  .        Additio
+000047d0: 6e61 6c6c 792c 2074 6865 2062 6573 7420  nally, the best 
+000047e0: 6869 7374 6f72 6963 616c 2072 6573 756c  historical resul
+000047f0: 7473 2061 7265 2073 6176 6564 2074 6f20  ts are saved to 
+00004800: 6120 6269 6e61 7279 2066 696c 6520 6e61  a binary file na
+00004810: 6d65 6420 6073 656c 662e 6366 672e 4d4f  med `self.cfg.MO
+00004820: 4e49 544f 525f 4245 5354 5f46 494c 454e  NITOR_BEST_FILEN
+00004830: 414d 4560 2e0d 0a20 2020 2020 2020 2022  AME`...        "
+00004840: 2222 0d0a 2020 2020 2020 2020 7320 3d20  ""..        s = 
+00004850: 227c 2020 7b70 7265 6669 787d 2020 7c20  "|  {prefix}  | 
+00004860: 2020 7b6e 616d 657d 2020 207c 2020 207b    {name}   |   {
+00004870: 7661 6c7d 2020 207c 2020 207b 6570 6f63  val}   |   {epoc
+00004880: 687d 2020 207c 2020 207b 696d 677d 2020  h}   |   {img}  
+00004890: 207c 5c6e 220d 0a20 2020 2020 2020 2069   |\n"..        i
+000048a0: 6e66 6f20 3d20 2222 0d0a 2020 2020 2020  nfo = ""..      
+000048b0: 2020 696e 666f 202b 3d20 227c 2020 5072    info += "|  Pr
+000048c0: 6566 6978 2020 7c20 2020 4d65 7472 6963  efix  |   Metric
+000048d0: 2020 207c 2020 2042 6573 7420 2020 7c20     |   Best   | 
+000048e0: 2020 4045 706f 6368 2020 207c 2020 2049    @Epoch   |   I
+000048f0: 6d67 2020 207c 5c6e 220d 0a20 2020 2020  mg   |\n"..     
+00004900: 2020 2069 6e66 6f20 2b3d 2022 7c20 3a2d     info += "| :-
+00004910: 2d2d 2d2d 2d2d 3a20 7c20 3a2d 2d2d 2d2d  ------: | :-----
+00004920: 2d2d 3a20 7c20 3a2d 2d2d 2d2d 2d2d 3a20  --: | :-------: 
+00004930: 7c20 3a2d 2d2d 2d2d 2d2d 3a20 7c20 3a2d  | :-------: | :-
+00004940: 2d2d 2d2d 2d2d 3a20 7c5c 6e22 0d0a 2020  ------: |\n"..  
+00004950: 2020 2020 2020 6461 7461 203d 205b 5d0d        data = [].
+00004960: 0a20 2020 2020 2020 2062 6573 7420 3d20  .        best = 
+00004970: 6465 6661 756c 7464 6963 7428 6469 6374  defaultdict(dict
+00004980: 290d 0a0d 0a20 2020 2020 2020 2066 6f72  )....        for
+00004990: 2070 7265 6669 782c 206d 6574 7269 6373   prefix, metrics
+000049a0: 2069 6e20 7365 6c66 2e6d 6f6e 6974 6f72   in self.monitor
+000049b0: 732e 6974 656d 7328 293a 0d0a 2020 2020  s.items():..    
+000049c0: 2020 2020 2020 2020 6d65 7472 6963 733a          metrics:
+000049d0: 2064 6566 6175 6c74 6469 6374 5b73 7472   defaultdict[str
+000049e0: 2c20 4c69 7374 5b41 7665 7261 6765 4d65  , List[AverageMe
+000049f0: 7465 725d 5d0d 0a20 2020 2020 2020 2020  ter]]..         
+00004a00: 2020 2066 7265 7120 3d20 3120 6966 2070     freq = 1 if p
+00004a10: 7265 6669 7820 3d3d 2027 7472 6169 6e27  refix == 'train'
+00004a20: 2065 6c73 6520 7365 6c66 2e63 6667 2e45   else self.cfg.E
+00004a30: 5641 4c5f 4652 4551 0d0a 2020 2020 2020  VAL_FREQ..      
+00004a40: 2020 2020 2020 666f 7220 6c61 7374 6e61        for lastna
+00004a50: 6d65 2c20 6d65 7465 7273 2069 6e20 6d65  me, meters in me
+00004a60: 7472 6963 732e 6974 656d 7328 293a 0d0a  trics.items():..
+00004a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a80: 666f 7220 6d65 7465 7220 696e 206d 6574  for meter in met
+00004a90: 6572 733a 0d0a 2020 2020 2020 2020 2020  ers:..          
+00004aa0: 2020 2020 2020 2020 2020 2320 536b 6970            # Skip
+00004ab0: 2074 686f 7365 206d 6574 6572 7320 6e65   those meters ne
+00004ac0: 7665 7220 6163 7469 7661 7465 642e 0d0a  ver activated...
+00004ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ae0: 2020 2020 6966 206c 656e 286d 6574 6572      if len(meter
+00004af0: 2e68 6973 746f 7279 2920 3d3d 2030 3a0d  .history) == 0:.
+00004b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004b10: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+00004b20: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+00004b30: 2020 2020 2020 206d 6574 6572 2e70 6c6f         meter.plo
+00004b40: 7428 6672 6571 3d66 7265 7129 0d0a 2020  t(freq=freq)..  
+00004b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b60: 2020 696d 676e 616d 6520 3d20 6d65 7465    imgname = mete
+00004b70: 722e 7361 7665 2870 6174 683d 6f73 2e70  r.save(path=os.p
+00004b80: 6174 682e 6a6f 696e 2873 656c 662e 6366  ath.join(self.cf
+00004b90: 672e 4c4f 475f 5041 5448 2c20 7365 6c66  g.LOG_PATH, self
+00004ba0: 2e63 6667 2e53 554d 4d41 5259 5f44 4952  .cfg.SUMMARY_DIR
+00004bb0: 292c 2070 7265 6669 783d 7072 6566 6978  ), prefix=prefix
+00004bc0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00004bd0: 2020 2020 2020 2065 706f 6368 2c20 7661         epoch, va
+00004be0: 6c20 3d20 6d65 7465 722e 6172 6762 6573  l = meter.argbes
+00004bf0: 7428 6672 6571 290d 0a20 2020 2020 2020  t(freq)..       
+00004c00: 2020 2020 2020 2020 2020 2020 2069 6e66               inf
+00004c10: 6f20 2b3d 2073 2e66 6f72 6d61 7428 0d0a  o += s.format(..
+00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c30: 2020 2020 2020 2020 7072 6566 6978 3d70          prefix=p
+00004c40: 7265 6669 782c 206e 616d 653d 6d65 7465  refix, name=mete
+00004c50: 722e 6e61 6d65 2c0d 0a20 2020 2020 2020  r.name,..       
+00004c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c70: 2076 616c 3d76 616c 2c20 6570 6f63 683d   val=val, epoch=
+00004c80: 6570 6f63 682c 2069 6d67 3d66 2221 5b5d  epoch, img=f"![]
+00004c90: 287b 696d 676e 616d 657d 2922 0d0a 2020  ({imgname})"..  
+00004ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cb0: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
+00004cc0: 2020 2020 2020 2020 2064 6174 612e 6170           data.ap
+00004cd0: 7065 6e64 285b 7072 6566 6978 2c20 6d65  pend([prefix, me
+00004ce0: 7465 722e 6e61 6d65 2c20 7661 6c2c 2065  ter.name, val, e
+00004cf0: 706f 6368 5d29 0d0a 2020 2020 2020 2020  poch])..        
+00004d00: 2020 2020 2020 2020 2020 2020 6966 2076              if v
+00004d10: 616c 2021 3d20 2d31 3a20 2320 4f6e 6c79  al != -1: # Only
+00004d20: 2073 6176 6520 6176 6169 6c61 626c 6520   save available 
+00004d30: 6461 7461 2e0d 0a20 2020 2020 2020 2020  data...         
+00004d40: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00004d50: 6573 745b 7072 6566 6978 5d5b 6d65 7465  est[prefix][mete
+00004d60: 722e 6e61 6d65 5d20 3d20 7661 6c0d 0a0d  r.name] = val...
+00004d70: 0a20 2020 2020 2020 2066 696c 655f 203d  .        file_ =
+00004d80: 206f 732e 7061 7468 2e6a 6f69 6e28 7365   os.path.join(se
+00004d90: 6c66 2e63 6667 2e4c 4f47 5f50 4154 482c  lf.cfg.LOG_PATH,
+00004da0: 2073 656c 662e 6366 672e 5355 4d4d 4152   self.cfg.SUMMAR
+00004db0: 595f 4449 522c 2073 656c 662e 6366 672e  Y_DIR, self.cfg.
+00004dc0: 5355 4d4d 4152 595f 4649 4c45 4e41 4d45  SUMMARY_FILENAME
+00004dd0: 290d 0a20 2020 2020 2020 2077 6974 6820  )..        with 
+00004de0: 6f70 656e 2866 696c 655f 2c20 2277 222c  open(file_, "w",
+00004df0: 2065 6e63 6f64 696e 673d 2275 7466 3822   encoding="utf8"
+00004e00: 2920 6173 2066 683a 0d0a 2020 2020 2020  ) as fh:..      
+00004e10: 2020 2020 2020 6668 2e77 7269 7465 2869        fh.write(i
+00004e20: 6e66 6f29 0d0a 0d0a 2020 2020 2020 2020  nfo)....        
+00004e30: 6466 203d 2070 642e 4461 7461 4672 616d  df = pd.DataFram
+00004e40: 6528 6461 7461 2c20 636f 6c75 6d6e 733d  e(data, columns=
+00004e50: 5b27 5072 6566 6978 272c 2027 4d65 7472  ['Prefix', 'Metr
+00004e60: 6963 272c 2027 4265 7374 272c 2027 4045  ic', 'Best', '@E
+00004e70: 706f 6368 275d 290d 0a20 2020 2020 2020  poch'])..       
+00004e80: 2069 6e66 6f4c 6f67 6765 7228 7374 7228   infoLogger(str(
+00004e90: 6466 2929 0d0a 2020 2020 2020 2020 696e  df))..        in
+00004ea0: 666f 4c6f 6767 6572 2866 225b 4c6f 475f  foLogger(f"[LoG_
+00004eb0: 5061 5448 5d20 3e3e 3e20 7b73 656c 662e  PaTH] >>> {self.
+00004ec0: 6366 672e 4c4f 475f 5041 5448 7d22 290d  cfg.LOG_PATH}").
+00004ed0: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
+00004ee0: 6d6f 6e69 746f 7273 2e77 7269 7465 286f  monitors.write(o
+00004ef0: 732e 7061 7468 2e6a 6f69 6e28 7365 6c66  s.path.join(self
+00004f00: 2e63 6667 2e4c 4f47 5f50 4154 482c 2073  .cfg.LOG_PATH, s
+00004f10: 656c 662e 6366 672e 5355 4d4d 4152 595f  elf.cfg.SUMMARY_
+00004f20: 4449 5229 2920 2320 7465 6e73 6f72 626f  DIR)) # tensorbo
+00004f30: 6172 640d 0a0d 0a20 2020 2020 2020 2073  ard....        s
+00004f40: 656c 662e 6d6f 6e69 746f 7273 2e73 6176  elf.monitors.sav
+00004f50: 6528 6f73 2e70 6174 682e 6a6f 696e 2873  e(os.path.join(s
+00004f60: 656c 662e 6366 672e 4c4f 475f 5041 5448  elf.cfg.LOG_PATH
+00004f70: 2c20 7365 6c66 2e63 6667 2e44 4154 415f  , self.cfg.DATA_
+00004f80: 4449 5229 2c20 7365 6c66 2e63 6667 2e4d  DIR), self.cfg.M
+00004f90: 4f4e 4954 4f52 5f46 494c 454e 414d 4529  ONITOR_FILENAME)
+00004fa0: 0d0a 2020 2020 2020 2020 6578 706f 7274  ..        export
+00004fb0: 5f70 6963 6b6c 6528 6265 7374 2c20 6f73  _pickle(best, os
+00004fc0: 2e70 6174 682e 6a6f 696e 2873 656c 662e  .path.join(self.
+00004fd0: 6366 672e 4c4f 475f 5041 5448 2c20 7365  cfg.LOG_PATH, se
+00004fe0: 6c66 2e63 6667 2e44 4154 415f 4449 522c  lf.cfg.DATA_DIR,
+00004ff0: 2073 656c 662e 6366 672e 4d4f 4e49 544f   self.cfg.MONITO
+00005000: 525f 4245 5354 5f46 494c 454e 414d 4529  R_BEST_FILENAME)
+00005010: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00005020: 200d 0a20 2020 2040 7469 6d65 6d65 7465   ..    @timemete
+00005030: 7228 2243 6f61 6368 2f66 6974 2229 0d0a  r("Coach/fit")..
+00005040: 2020 2020 6465 6620 6669 7428 7365 6c66      def fit(self
+00005050: 293a 0d0a 0d0a 2020 2020 2020 2020 6465  ):....        de
+00005060: 6620 7369 676e 616c 5f68 616e 646c 6572  f signal_handler
+00005070: 2873 6967 2c20 6672 616d 6529 3a0d 0a20  (sig, frame):.. 
+00005080: 2020 2020 2020 2020 2020 2069 6e66 6f4c             infoL
+00005090: 6f67 6765 7228 6622 5c30 3333 5b30 3b33  ogger(f"\033[0;3
+000050a0: 313b 3437 6d3d 3d3d 3d3d 3d3d 3d3d 3d3d  1;47m===========
+000050b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000050c0: 3d3d 3d3d 5445 524d 494e 4154 4520 4355  ====TERMINATE CU
+000050d0: 5252 454e 5420 5052 4f43 4553 533d 3d3d  RRENT PROCESS===
+000050e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000050f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 5c30 3333  ============\033
+00005100: 5b30 6d22 290d 0a20 2020 2020 2020 2020  [0m")..         
+00005110: 2020 2073 7973 2e65 7869 7428 290d 0a20     sys.exit().. 
+00005120: 2020 2020 2020 2073 6967 6e61 6c2e 7369         signal.si
+00005130: 676e 616c 2873 6967 6e61 6c2e 5349 4749  gnal(signal.SIGI
+00005140: 4e54 2c20 7369 676e 616c 5f68 616e 646c  NT, signal_handl
+00005150: 6572 290d 0a0d 0a20 2020 2020 2020 2073  er)....        s
+00005160: 7461 7274 5f65 706f 6368 203d 2073 656c  tart_epoch = sel
+00005170: 662e 7265 7375 6d65 2829 0d0a 2020 2020  f.resume()..    
+00005180: 2020 2020 666f 7220 6570 6f63 6820 696e      for epoch in
+00005190: 2072 616e 6765 2873 7461 7274 5f65 706f   range(start_epo
+000051a0: 6368 2c20 7365 6c66 2e63 6667 2e65 706f  ch, self.cfg.epo
+000051b0: 6368 7329 3a0d 0a20 2020 2020 2020 2020  chs):..         
+000051c0: 2020 2069 6620 6570 6f63 6820 2520 7365     if epoch % se
+000051d0: 6c66 2e63 6667 2e43 4845 434b 504f 494e  lf.cfg.CHECKPOIN
+000051e0: 545f 4652 4551 203d 3d20 303a 0d0a 2020  T_FREQ == 0:..  
+000051f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00005200: 6c66 2e73 6176 655f 6368 6563 6b70 6f69  lf.save_checkpoi
+00005210: 6e74 2865 706f 6368 290d 0a20 2020 2020  nt(epoch)..     
+00005220: 2020 2020 2020 2069 6620 6570 6f63 6820         if epoch 
+00005230: 2520 7365 6c66 2e63 6667 2e45 5641 4c5f  % self.cfg.EVAL_
+00005240: 4652 4551 203d 3d20 303a 0d0a 2020 2020  FREQ == 0:..    
+00005250: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00005260: 656c 662e 6366 672e 4556 414c 5f56 414c  elf.cfg.EVAL_VAL
+00005270: 4944 3a0d 0a20 2020 2020 2020 2020 2020  ID:..           
+00005280: 2020 2020 2020 2020 2073 656c 662e 7661           self.va
+00005290: 6c69 6428 6570 6f63 6829 0d0a 2020 2020  lid(epoch)..    
+000052a0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000052b0: 656c 662e 6366 672e 4556 414c 5f54 4553  elf.cfg.EVAL_TES
+000052c0: 543a 0d0a 2020 2020 2020 2020 2020 2020  T:..            
+000052d0: 2020 2020 2020 2020 7365 6c66 2e74 6573          self.tes
+000052e0: 7428 6570 6f63 6829 0d0a 2020 2020 2020  t(epoch)..      
+000052f0: 2020 2020 2020 7365 6c66 2e63 6865 636b        self.check
+00005300: 5f62 6573 7428 6570 6f63 6829 0d0a 2020  _best(epoch)..  
+00005310: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00005320: 7465 7028 6570 6f63 6829 0d0a 2020 2020  tep(epoch)..    
+00005330: 2020 2020 2020 2020 7365 6c66 2e74 7261          self.tra
+00005340: 696e 2865 706f 6368 290d 0a0d 0a20 2020  in(epoch)....   
+00005350: 2020 2020 2073 656c 662e 7361 7665 2829       self.save()
+00005360: 0d0a 0d0a 2020 2020 2020 2020 2320 6c61  ....        # la
+00005370: 7374 2065 706f 6368 0d0a 2020 2020 2020  st epoch..      
+00005380: 2020 7365 6c66 2e76 616c 6964 2873 656c    self.valid(sel
+00005390: 662e 6366 672e 6570 6f63 6873 290d 0a20  f.cfg.epochs).. 
+000053a0: 2020 2020 2020 2073 656c 662e 7465 7374         self.test
+000053b0: 2873 656c 662e 6366 672e 6570 6f63 6873  (self.cfg.epochs
+000053c0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000053d0: 6368 6563 6b5f 6265 7374 2873 656c 662e  check_best(self.
+000053e0: 6366 672e 6570 6f63 6873 290d 0a20 2020  cfg.epochs)..   
+000053f0: 2020 2020 2073 656c 662e 7374 6570 2873       self.step(s
+00005400: 656c 662e 6366 672e 6570 6f63 6873 290d  elf.cfg.epochs).
+00005410: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
+00005420: 7375 6d6d 6172 7928 290d 0a0d 0a20 2020  summary()....   
+00005430: 2020 2020 2073 656c 662e 6576 616c 5f61       self.eval_a
+00005440: 745f 6265 7374 2829 0d0a 0d0a 0d0a 636c  t_best()......cl
+00005450: 6173 7320 4164 6170 7465 723a 0d0a 2020  ass Adapter:..  
+00005460: 2020 7222 2222 0d0a 2020 2020 5061 7261    r"""..    Para
+00005470: 6d73 2074 756e 6572 2e0d 0a0d 0a20 2020  ms tuner.....   
+00005480: 2046 6c6f 7773 3a0d 0a20 2020 202d 2d2d   Flows:..    ---
+00005490: 2d2d 2d0d 0a20 2020 2031 2e20 636f 6d70  ---..    1. comp
+000054a0: 696c 653a 2063 6f6e 6669 6775 7265 2074  ile: configure t
+000054b0: 6865 2063 6f6d 6d61 6e64 2c20 656e 7669  he command, envi
+000054c0: 726f 6e6d 656e 7473 2c20 616e 6420 7061  ronments, and pa
+000054d0: 7261 6d65 7465 7273 2066 6f72 2074 7261  rameters for tra
+000054e0: 696e 696e 672e 0d0a 2020 2020 322e 2061  ining...    2. a
+000054f0: 6c6c 6f63 6174 6520 6465 7669 6365 7320  llocate devices 
+00005500: 666f 7220 7661 7269 6f75 7320 7061 7261  for various para
+00005510: 6d65 7465 7273 3a0d 0a20 2020 2020 2020  meters:..       
+00005520: 202d 2072 6567 6973 7465 7220 7468 6520   - register the 
+00005530: 4944 2c20 6c6f 6720 7061 7468 2c20 616e  ID, log path, an
+00005540: 6420 6465 7669 6365 2066 6972 7374 0d0a  d device first..
+00005550: 2020 2020 2020 2020 2d20 6578 6563 7574          - execut
+00005560: 6520 7468 6520 636f 6d6d 616e 640d 0a20  e the command.. 
+00005570: 2020 2020 2020 202d 2063 6f6c 6c65 6374         - collect
+00005580: 2069 6e66 6f72 6d61 7469 6f6e 2066 726f   information fro
+00005590: 6d20 7468 6520 6c6f 6720 7061 7468 2061  m the log path a
+000055a0: 6e64 206f 7574 7075 7420 746f 2054 656e  nd output to Ten
+000055b0: 736f 7242 6f61 7264 0d0a 2020 2020 2020  sorBoard..      
+000055c0: 2020 2d20 7361 7665 2074 6865 2063 6865    - save the che
+000055d0: 636b 706f 696e 740d 0a20 2020 2020 2020  ckpoint..       
+000055e0: 202d 2072 656c 6561 7365 2074 6865 2063   - release the c
+000055f0: 6f72 7265 7370 6f6e 6469 6e67 2064 6576  orresponding dev
+00005600: 6963 650d 0a0d 0a20 2020 2045 7861 6d70  ice....    Examp
+00005610: 6c65 733a 0d0a 2020 2020 2d2d 2d2d 2d2d  les:..    ------
+00005620: 2d2d 2d0d 0a20 2020 203e 3e3e 2063 6667  ---..    >>> cfg
+00005630: 203d 207b 2763 6f6d 6d61 6e64 273a 2027   = {'command': '
+00005640: 7079 7468 6f6e 2078 7878 2e70 7927 2c20  python xxx.py', 
+00005650: 2770 6172 616d 7327 3a20 7b27 6f70 7469  'params': {'opti
+00005660: 6d69 7a65 7227 3a20 5b27 7367 6427 2c20  mizer': ['sgd', 
+00005670: 2761 6461 6d27 5d7d 7d0d 0a20 2020 203e  'adam']}}..    >
+00005680: 3e3e 2074 756e 6572 203d 2041 6461 7074  >> tuner = Adapt
+00005690: 6572 2829 0d0a 2020 2020 3e3e 3e20 7475  er()..    >>> tu
+000056a0: 6e65 722e 636f 6d70 696c 6528 6366 6729  ner.compile(cfg)
+000056b0: 0d0a 2020 2020 3e3e 3e20 7475 6e65 722e  ..    >>> tuner.
+000056c0: 6669 7428 290d 0a20 2020 2022 2222 0d0a  fit()..    """..
+000056d0: 0d0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+000056e0: 5f5f 2873 656c 6629 202d 3e20 4e6f 6e65  __(self) -> None
+000056f0: 3a0d 0a20 2020 2020 2020 2073 656c 662e  :..        self.
+00005700: 7061 7261 6d73 203d 205b 5d0d 0a20 2020  params = []..   
+00005710: 2020 2020 2073 656c 662e 7661 6c75 6573       self.values
+00005720: 203d 205b 5d0d 0a20 2020 2020 2020 2073   = []..        s
+00005730: 656c 662e 6465 7669 6365 7320 3d20 5b5d  elf.devices = []
+00005740: 0d0a 0d0a 2020 2020 2020 2020 6465 6620  ....        def 
+00005750: 636c 6561 6e28 293a 0d0a 2020 2020 2020  clean():..      
+00005760: 2020 2020 2020 7061 7265 6e74 203d 2070        parent = p
+00005770: 7375 7469 6c2e 5072 6f63 6573 7328 6f73  sutil.Process(os
+00005780: 2e67 6574 7069 6428 2929 0d0a 2020 2020  .getpid())..    
+00005790: 2020 2020 2020 2020 6368 696c 6472 656e          children
+000057a0: 203d 2070 6172 656e 742e 6368 696c 6472   = parent.childr
+000057b0: 656e 2872 6563 7572 7369 7665 3d54 7275  en(recursive=Tru
+000057c0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+000057d0: 666f 7220 7072 6f63 6573 7320 696e 2063  for process in c
+000057e0: 6869 6c64 7265 6e3a 0d0a 2020 2020 2020  hildren:..      
+000057f0: 2020 2020 2020 2020 2020 7072 6f63 6573            proces
+00005800: 732e 7365 6e64 5f73 6967 6e61 6c28 7369  s.send_signal(si
+00005810: 676e 616c 2e53 4947 5445 524d 290d 0a20  gnal.SIGTERM).. 
+00005820: 2020 2020 2020 2020 2020 2070 7375 7469             psuti
+00005830: 6c2e 7761 6974 5f70 726f 6373 2863 6869  l.wait_procs(chi
+00005840: 6c64 7265 6e2c 2074 696d 656f 7574 3d35  ldren, timeout=5
+00005850: 290d 0a0d 0a20 2020 2020 2020 2061 7465  )....        ate
+00005860: 7869 742e 7265 6769 7374 6572 2863 6c65  xit.register(cle
+00005870: 616e 290d 0a0d 0a20 2020 2040 7072 6f70  an)....    @prop
+00005880: 6572 7479 0d0a 2020 2020 6465 6620 434f  erty..    def CO
+00005890: 4d4d 414e 4428 7365 6c66 293a 0d0a 2020  MMAND(self):..  
+000058a0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000058b0: 662e 6366 672e 434f 4d4d 414e 440d 0a0d  f.cfg.COMMAND...
+000058c0: 0a20 2020 2064 6566 2072 6567 6973 7465  .    def registe
+000058d0: 7228 7365 6c66 2c20 6465 7669 6365 3a20  r(self, device: 
+000058e0: 7374 7229 202d 3e20 5475 706c 655b 7374  str) -> Tuple[st
+000058f0: 722c 2073 7472 5d3a 0d0a 2020 2020 2020  r, str]:..      
+00005900: 2020 7365 6c66 2e63 6667 2e45 4e56 535b    self.cfg.ENVS[
+00005910: 2769 6427 5d20 3d20 7469 6d65 2e73 7472  'id'] = time.str
+00005920: 6674 696d 6528 5449 4d45 290d 0a20 2020  ftime(TIME)..   
+00005930: 2020 2020 2073 656c 662e 6366 672e 454e       self.cfg.EN
+00005940: 5653 5b27 6465 7669 6365 275d 203d 2064  VS['device'] = d
+00005950: 6576 6963 650d 0a20 2020 2020 2020 2063  evice..        c
+00005960: 6f6d 6d61 6e64 203d 2073 656c 662e 434f  ommand = self.CO
+00005970: 4d4d 414e 4420 2b20 7365 6c66 2e67 6574  MMAND + self.get
+00005980: 5f6f 7074 696f 6e28 2769 6427 2c20 7365  _option('id', se
+00005990: 6c66 2e63 6667 2e45 4e56 532e 6964 290d  lf.cfg.ENVS.id).
+000059a0: 0a20 2020 2020 2020 2063 6f6d 6d61 6e64  .        command
+000059b0: 202b 3d20 7365 6c66 2e67 6574 5f6f 7074   += self.get_opt
+000059c0: 696f 6e28 2764 6576 6963 6527 2c20 7365  ion('device', se
+000059d0: 6c66 2e63 6667 2e45 4e56 532e 6465 7669  lf.cfg.ENVS.devi
+000059e0: 6365 290d 0a20 2020 2020 2020 2072 6574  ce)..        ret
+000059f0: 7572 6e20 636f 6d6d 616e 642c 2073 656c  urn command, sel
+00005a00: 662e 6366 672e 454e 5653 2e69 642c 2073  f.cfg.ENVS.id, s
+00005a10: 656c 662e 6366 672e 4c4f 475f 5041 5448  elf.cfg.LOG_PATH
+00005a20: 2e66 6f72 6d61 7428 2a2a 7365 6c66 2e63  .format(**self.c
+00005a30: 6667 2e45 4e56 5329 0d0a 0d0a 2020 2020  fg.ENVS)....    
+00005a40: 4074 696d 656d 6574 6572 2822 4164 6170  @timemeter("Adap
+00005a50: 7465 722f 636f 6d70 696c 6522 290d 0a20  ter/compile").. 
+00005a60: 2020 2064 6566 2063 6f6d 7069 6c65 2873     def compile(s
+00005a70: 656c 662c 2063 6667 3a20 436f 6e66 6967  elf, cfg: Config
+00005a80: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
+00005a90: 2020 2020 7222 2222 0d0a 2020 2020 2020      r"""..      
+00005aa0: 2020 436f 6e66 6967 7572 6520 7468 6520    Configure the 
+00005ab0: 636f 6d6d 616e 642c 2065 6e76 6972 6f6e  command, environ
+00005ac0: 6d65 6e74 732c 2061 6e64 2070 6172 616d  ments, and param
+00005ad0: 6574 6572 7320 666f 7220 7472 6169 6e69  eters for traini
+00005ae0: 6e67 2e0d 0a0d 0a20 2020 2020 2020 2050  ng.....        P
+00005af0: 6172 616d 6574 6572 733a 0d0a 2020 2020  arameters:..    
+00005b00: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d      -----------.
+00005b10: 0a20 2020 2020 2020 2063 6667 203a 2043  .        cfg : C
+00005b20: 6f6e 6669 670d 0a20 2020 2020 2020 2020  onfig..         
+00005b30: 2020 2041 6e20 6f62 6a65 6374 2074 6861     An object tha
+00005b40: 7420 636f 6e74 6169 6e73 2074 6865 2063  t contains the c
+00005b50: 6f6d 6d61 6e64 2c20 656e 7669 726f 6e6d  ommand, environm
+00005b60: 656e 7473 2c20 7061 7261 6d65 7465 7273  ents, parameters
+00005b70: 2c20 616e 6420 6465 6661 756c 7473 2e0d  , and defaults..
+00005b80: 0a0d 0a20 2020 2020 2020 2046 6c6f 7773  ...        Flows
+00005b90: 3a0d 0a20 2020 2020 2020 202d 2d2d 2d2d  :..        -----
+00005ba0: 2d0d 0a20 2020 2020 2020 2031 2e20 4164  -..        1. Ad
+00005bb0: 6420 656e 7669 726f 6e6d 656e 7461 6c20  d environmental 
+00005bc0: 7061 7261 6d65 7465 7273 2074 6f20 7468  parameters to th
+00005bd0: 6520 6261 7369 6320 6063 6f6d 6d61 6e64  e basic `command
+00005be0: 602e 0d0a 2020 2020 2020 2020 322e 2052  `...        2. R
+00005bf0: 6567 6973 7465 7220 616c 6c20 6176 6169  egister all avai
+00005c00: 6c61 626c 6520 6465 7669 6365 732e 0d0a  lable devices...
+00005c10: 2020 2020 2020 2020 332e 2043 6f6e 7665          3. Conve
+00005c20: 7274 2061 6c6c 2070 6172 616d 6574 6572  rt all parameter
+00005c30: 7320 6672 6f6d 2060 6366 672e 5041 5241  s from `cfg.PARA
+00005c40: 4d53 602e 0d0a 2020 2020 2020 2020 342e  MS`...        4.
+00005c50: 2043 6f6e 7665 7274 2061 6c6c 2064 6566   Convert all def
+00005c60: 6175 6c74 7320 6672 6f6d 2060 6366 672e  aults from `cfg.
+00005c70: 4445 4641 554c 5453 602e 0d0a 0d0a 2020  DEFAULTS`.....  
+00005c80: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
+00005c90: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00005ca0: 0d0a 2020 2020 2020 2020 4e6f 6e65 0d0a  ..        None..
+00005cb0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00005cc0: 2020 2020 2073 656c 662e 6366 6720 3d20       self.cfg = 
+00005cd0: 6366 670d 0a20 2020 2020 2020 2070 6965  cfg..        pie
+00005ce0: 6365 203d 2022 5c74 7b6b 6579 7d3a 207b  ce = "\t{key}: {
+00005cf0: 7661 6c73 7d20 5c6e 220d 0a20 2020 2020  vals} \n"..     
+00005d00: 2020 2065 6e76 732c 2070 6172 616d 732c     envs, params,
+00005d10: 2064 6566 6175 6c74 7320 3d20 2222 2c20   defaults = "", 
+00005d20: 2222 2c20 2222 0d0a 2020 2020 2020 2020  "", ""..        
+00005d30: 666f 7220 6b65 792c 2076 616c 2069 6e20  for key, val in 
+00005d40: 7365 6c66 2e63 6667 2e45 4e56 532e 6974  self.cfg.ENVS.it
+00005d50: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
+00005d60: 2020 2020 6966 206b 6579 203d 3d20 2764      if key == 'd
+00005d70: 6576 6963 6527 3a0d 0a20 2020 2020 2020  evice':..       
+00005d80: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
+00005d90: 7669 6365 7320 3d20 7661 6c2e 7370 6c69  vices = val.spli
+00005da0: 7428 272c 2729 0d0a 2020 2020 2020 2020  t(',')..        
+00005db0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00005dc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005dd0: 6366 672e 434f 4d4d 414e 4420 2b3d 2073  cfg.COMMAND += s
+00005de0: 656c 662e 6765 745f 6f70 7469 6f6e 286b  elf.get_option(k
+00005df0: 6579 2c20 7661 6c29 0d0a 2020 2020 2020  ey, val)..      
+00005e00: 2020 2020 2020 656e 7673 202b 3d20 7069        envs += pi
+00005e10: 6563 652e 666f 726d 6174 286b 6579 3d6b  ece.format(key=k
+00005e20: 6579 2c20 7661 6c73 3d76 616c 290d 0a20  ey, vals=val).. 
+00005e30: 2020 2020 2020 2066 6f72 206b 6579 2c20         for key, 
+00005e40: 7661 6c73 2069 6e20 7365 6c66 2e63 6667  vals in self.cfg
+00005e50: 2e50 4152 414d 532e 6974 656d 7328 293a  .PARAMS.items():
+00005e60: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00005e70: 2069 7369 6e73 7461 6e63 6528 7661 6c73   isinstance(vals
+00005e80: 2c20 2873 7472 2c20 696e 742c 2066 6c6f  , (str, int, flo
+00005e90: 6174 2929 3a0d 0a20 2020 2020 2020 2020  at)):..         
+00005ea0: 2020 2020 2020 2076 616c 7320 3d20 5b76         vals = [v
+00005eb0: 616c 735d 0d0a 2020 2020 2020 2020 2020  als]..          
+00005ec0: 2020 7365 6c66 2e64 6570 6c6f 795f 7061    self.deploy_pa
+00005ed0: 7261 6d73 286b 6579 2c20 7661 6c73 290d  rams(key, vals).
+00005ee0: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
+00005ef0: 616d 7320 2b3d 2070 6965 6365 2e66 6f72  ams += piece.for
+00005f00: 6d61 7428 6b65 793d 6b65 792c 2076 616c  mat(key=key, val
+00005f10: 733d 7661 6c73 290d 0a20 2020 2020 2020  s=vals)..       
+00005f20: 2066 6f72 206b 6579 2c20 7661 6c20 696e   for key, val in
+00005f30: 2073 656c 662e 6366 672e 4445 4641 554c   self.cfg.DEFAUL
+00005f40: 5453 2e69 7465 6d73 2829 3a0d 0a20 2020  TS.items():..   
+00005f50: 2020 2020 2020 2020 2073 656c 662e 6366           self.cf
+00005f60: 672e 4445 4641 554c 5453 5b6b 6579 5d20  g.DEFAULTS[key] 
+00005f70: 3d20 7661 6c0d 0a20 2020 2020 2020 2020  = val..         
+00005f80: 2020 2064 6566 6175 6c74 7320 2b3d 2070     defaults += p
+00005f90: 6965 6365 2e66 6f72 6d61 7428 6b65 793d  iece.format(key=
+00005fa0: 6b65 792c 2076 616c 733d 7661 6c29 0d0a  key, vals=val)..
+00005fb0: 0d0a 2020 2020 2020 2020 6366 675f 696e  ..        cfg_in
+00005fc0: 666f 7320 3d20 6622 636f 6d6d 616e 643a  fos = f"command:
+00005fd0: 207b 7365 6c66 2e63 6667 2e43 4f4d 4d41   {self.cfg.COMMA
+00005fe0: 4e44 7d20 5c6e 656e 7673 3a20 5c6e 7b65  ND} \nenvs: \n{e
+00005ff0: 6e76 737d 7061 7261 6d73 3a20 5c6e 7b70  nvs}params: \n{p
+00006000: 6172 616d 737d 6465 6661 756c 7473 3a20  arams}defaults: 
+00006010: 5c6e 7b64 6566 6175 6c74 737d 220d 0a20  \n{defaults}".. 
+00006020: 2020 2020 2020 2069 6e66 6f4c 6f67 6765         infoLogge
+00006030: 7228 6622 5c30 3333 5b30 3b33 313b 3437  r(f"\033[0;31;47
+00006040: 6d7b 6366 675f 696e 666f 737d 5c30 3333  m{cfg_infos}\033
+00006050: 5b30 6d22 290d 0a20 2020 2020 2020 200d  [0m")..        .
+00006060: 0a0d 0a20 2020 2064 6566 2064 6570 6c6f  ...    def deplo
+00006070: 795f 7061 7261 6d73 2873 656c 662c 206b  y_params(self, k
+00006080: 6579 3a20 7374 722c 2076 616c 733a 2049  ey: str, vals: I
+00006090: 7465 7261 626c 6529 3a0d 0a20 2020 2020  terable):..     
+000060a0: 2020 2073 656c 662e 7061 7261 6d73 2e61     self.params.a
+000060b0: 7070 656e 6428 6b65 7929 0d0a 2020 2020  ppend(key)..    
+000060c0: 2020 2020 7365 6c66 2e76 616c 7565 732e      self.values.
+000060d0: 6170 7065 6e64 2876 616c 7329 0d0a 0d0a  append(vals)....
+000060e0: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
+000060f0: 640d 0a20 2020 2064 6566 2067 6574 5f6f  d..    def get_o
+00006100: 7074 696f 6e28 6b65 793a 2073 7472 2c20  ption(key: str, 
+00006110: 7661 6c3a 2041 6e79 293a 0d0a 2020 2020  val: Any):..    
+00006120: 2020 2020 7222 2222 0d0a 2020 2020 2020      r"""..      
+00006130: 2020 436f 6e76 6572 7420 286b 6579 2c20    Convert (key, 
+00006140: 7661 6c29 2074 6f20 272d 2d6b 6579 3d76  val) to '--key=v
+00006150: 616c 272e 0d0a 0d0a 2020 2020 2020 2020  al'.....        
+00006160: 5061 7261 6d65 7465 7273 3a0d 0a20 2020  Parameters:..   
+00006170: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d       -----------
+00006180: 0d0a 2020 2020 2020 2020 6b65 7920 3a20  ..        key : 
+00006190: 7374 720d 0a20 2020 2020 2020 2020 2020  str..           
+000061a0: 2054 6865 206b 6579 206f 6620 7468 6520   The key of the 
+000061b0: 7061 7261 6d65 7465 722e 0d0a 2020 2020  parameter...    
+000061c0: 2020 2020 7661 6c20 3a20 416e 790d 0a20      val : Any.. 
+000061d0: 2020 2020 2020 2020 2020 2054 6865 2076             The v
+000061e0: 616c 7565 206f 6620 7468 6520 7061 7261  alue of the para
+000061f0: 6d65 7465 722e 0d0a 0d0a 2020 2020 2020  meter.....      
+00006200: 2020 4e6f 7465 733a 0d0a 2020 2020 2020    Notes:..      
+00006210: 2020 2d2d 2d2d 2d2d 0d0a 2020 2020 2020    ------..      
+00006220: 2020 416c 6c20 275f 2720 696e 2060 6b65    All '_' in `ke
+00006230: 7960 2077 696c 6c20 6265 2072 6570 6c61  y` will be repla
+00006240: 6365 6420 6279 2027 2d27 2e0d 0a0d 0a20  ced by '-'..... 
+00006250: 2020 2020 2020 2052 6574 7572 6e73 3a0d         Returns:.
+00006260: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00006270: 2d0d 0a20 2020 2020 2020 2073 7472 0d0a  -..        str..
+00006280: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+00006290: 7061 7261 6d65 7465 7220 7769 7468 2066  parameter with f
+000062a0: 6f72 6d61 7420 272d 2d6b 6579 3d76 616c  ormat '--key=val
+000062b0: 272e 0d0a 0d0a 2020 2020 2020 2020 4578  '.....        Ex
+000062c0: 616d 706c 6573 3a0d 0a20 2020 2020 2020  amples:..       
+000062d0: 202d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020   ---------..    
+000062e0: 2020 2020 3e3e 3e20 4164 6170 7465 722e      >>> Adapter.
+000062f0: 6765 745f 6f70 7469 6f6e 2827 6c72 272c  get_option('lr',
+00006300: 2027 3165 2d33 2729 0d0a 2020 2020 2020   '1e-3')..      
+00006310: 2020 272d 2d6c 723d 3165 2d33 270d 0a20    '--lr=1e-3'.. 
+00006320: 2020 2020 2020 203e 3e3e 2041 6461 7074         >>> Adapt
+00006330: 6572 2e67 6574 5f6f 7074 696f 6e28 276c  er.get_option('l
+00006340: 6561 726e 696e 675f 7261 7465 272c 2027  earning_rate', '
+00006350: 3165 2d33 2729 0d0a 2020 2020 2020 2020  1e-3')..        
+00006360: 272d 2d6c 6561 726e 696e 672d 7261 7465  '--learning-rate
+00006370: 3d31 652d 3327 0d0a 2020 2020 2020 2020  =1e-3'..        
+00006380: 2222 220d 0a20 2020 2020 2020 2072 6574  """..        ret
+00006390: 7572 6e20 6622 202d 2d7b 6b65 792e 7265  urn f" --{key.re
+000063a0: 706c 6163 6528 275f 272c 2027 2d27 297d  place('_', '-')}
+000063b0: 3d7b 7661 6c7d 220d 0a0d 0a20 2020 2064  ={val}"....    d
+000063c0: 6566 206c 6f61 645f 6265 7374 2873 656c  ef load_best(sel
+000063d0: 662c 206c 6f67 5061 7468 3a20 7374 7229  f, logPath: str)
+000063e0: 3a0d 0a20 2020 2020 2020 2022 2222 4c6f  :..        """Lo
+000063f0: 6164 2062 6573 742e 7069 636b 6c65 2066  ad best.pickle f
+00006400: 726f 6d20 6c6f 6750 6174 6820 6f66 2063  rom logPath of c
+00006410: 6f72 7265 7370 6f6e 6469 6e67 2e22 2222  orresponding."""
+00006420: 0d0a 2020 2020 2020 2020 6669 6c65 5f20  ..        file_ 
+00006430: 3d20 6f73 2e70 6174 682e 6a6f 696e 286c  = os.path.join(l
+00006440: 6f67 5061 7468 2c20 7365 6c66 2e63 6667  ogPath, self.cfg
+00006450: 2e44 4154 415f 4449 522c 2073 656c 662e  .DATA_DIR, self.
+00006460: 6366 672e 4d4f 4e49 544f 525f 4245 5354  cfg.MONITOR_BEST
+00006470: 5f46 494c 454e 414d 4529 0d0a 2020 2020  _FILENAME)..    
+00006480: 2020 2020 7265 7475 726e 2069 6d70 6f72      return impor
+00006490: 745f 7069 636b 6c65 2866 696c 655f 290d  t_pickle(file_).
+000064a0: 0a0d 0a20 2020 2064 6566 2077 7269 7465  ...    def write
+000064b0: 2873 656c 662c 2069 645f 3a20 7374 722c  (self, id_: str,
+000064c0: 206c 6f67 5061 7468 3a20 7374 722c 2070   logPath: str, p
+000064d0: 6172 616d 733a 2044 6963 7429 3a0d 0a20  arams: Dict):.. 
+000064e0: 2020 2020 2020 2072 2222 220d 0a20 2020         r"""..   
+000064f0: 2020 2020 2057 7269 7465 2065 7870 6572       Write exper
+00006500: 696d 656e 7420 7265 7375 6c74 7320 746f  iment results to
+00006510: 2074 656e 736f 7262 6f61 7264 2e0d 0a0d   tensorboard....
+00006520: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00006530: 6572 733a 0d0a 2020 2020 2020 2020 2d2d  ers:..        --
+00006540: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
+00006550: 2020 2069 645f 3a20 7374 720d 0a20 2020     id_: str..   
+00006560: 2020 2020 2020 2020 2045 7870 6572 696d           Experim
+00006570: 656e 7420 4944 2e0d 0a20 2020 2020 2020  ent ID...       
+00006580: 206c 6f67 5061 7468 3a20 7374 720d 0a20   logPath: str.. 
+00006590: 2020 2020 2020 2020 2020 2050 6174 6820             Path 
+000065a0: 746f 2074 6865 2065 7870 6572 696d 656e  to the experimen
+000065b0: 7420 6c6f 6773 2e0d 0a20 2020 2020 2020  t logs...       
+000065c0: 2070 6172 616d 733a 2044 6963 740d 0a20   params: Dict.. 
+000065d0: 2020 2020 2020 2020 2020 2043 6f6e 6669             Confi
+000065e0: 6775 7261 7469 6f6e 2070 6172 616d 6574  guration paramet
+000065f0: 6572 7320 6f66 2074 6865 2065 7870 6572  ers of the exper
+00006600: 696d 656e 742e 0d0a 0d0a 2020 2020 2020  iment.....      
+00006610: 2020 466c 6f77 733a 0d0a 2020 2020 2020    Flows:..      
+00006620: 2020 2d2d 2d2d 2d2d 0d0a 2020 2020 2020    ------..      
+00006630: 2020 312e 204c 6f61 6420 7468 6520 6265    1. Load the be
+00006640: 7374 2064 6174 6120 6672 6f6d 2060 6c6f  st data from `lo
+00006650: 6750 6174 6860 2e0d 0a20 2020 2020 2020  gPath`...       
+00006660: 2032 2e20 5772 6974 6520 7468 6520 6265   2. Write the be
+00006670: 7374 2064 6174 6120 746f 2074 656e 736f  st data to tenso
+00006680: 7262 6f61 7264 2077 6974 6820 6070 6172  rboard with `par
+00006690: 616d 7360 2e0d 0a0d 0a20 2020 2020 2020  ams`.....       
+000066a0: 204e 6f74 6573 3a0d 0a20 2020 2020 2020   Notes:..       
+000066b0: 202d 2d2d 2d2d 2d0d 0a20 2020 2020 2020   ------..       
+000066c0: 2049 6620 796f 7520 6669 6e64 2060 2d31   If you find `-1
+000066d0: 6020 6170 7065 6172 696e 6720 696e 2074  ` appearing in t
+000066e0: 6865 2074 656e 736f 7262 6f61 7264 2c0d  he tensorboard,.
+000066f0: 0a20 2020 2020 2020 2069 7420 636f 756c  .        it coul
+00006700: 6420 6d65 616e 2074 6861 7420 7468 6520  d mean that the 
+00006710: 6461 7461 2069 7320 6f66 2060 7374 7260  data is of `str`
+00006720: 2074 7970 652c 0d0a 2020 2020 2020 2020   type,..        
+00006730: 7768 6963 6820 7769 6c6c 2063 6175 7365  which will cause
+00006740: 2061 6e20 6572 726f 7220 6966 2069 7420   an error if it 
+00006750: 6973 2073 656e 7420 746f 2074 656e 736f  is sent to tenso
+00006760: 7262 6f61 7264 2064 6972 6563 746c 7921  rboard directly!
+00006770: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00006780: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+00006790: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
+000067a0: 7365 6c66 2e6c 6f61 645f 6265 7374 286c  self.load_best(l
+000067b0: 6f67 5061 7468 290d 0a20 2020 2020 2020  ogPath)..       
+000067c0: 2020 2020 2070 6174 6820 3d20 6f73 2e70       path = os.p
+000067d0: 6174 682e 6a6f 696e 2873 656c 662e 6366  ath.join(self.cf
+000067e0: 672e 434f 5245 5f4c 4f47 5f50 4154 482c  g.CORE_LOG_PATH,
+000067f0: 2069 645f 290d 0a20 2020 2020 2020 2020   id_)..         
+00006800: 2020 2077 6974 6820 5375 6d6d 6172 7957     with SummaryW
+00006810: 7269 7465 7228 6c6f 675f 6469 723d 7061  riter(log_dir=pa
+00006820: 7468 2920 6173 2077 7269 7465 723a 0d0a  th) as writer:..
+00006830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006840: 6d65 7472 6963 7320 3d20 6469 6374 2829  metrics = dict()
+00006850: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006860: 2020 666f 7220 7072 6566 6978 2c20 6265    for prefix, be
+00006870: 7374 2069 6e20 6461 7461 2e69 7465 6d73  st in data.items
+00006880: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+00006890: 2020 2020 2020 2020 2066 6f72 206d 6574           for met
+000068a0: 7269 632c 2076 616c 2069 6e20 6265 7374  ric, val in best
+000068b0: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
+000068c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068d0: 2020 2076 616c 203d 2076 616c 2069 6620     val = val if 
+000068e0: 6973 696e 7374 616e 6365 2876 616c 2c20  isinstance(val, 
+000068f0: 2869 6e74 2c20 666c 6f61 7429 2920 656c  (int, float)) el
+00006900: 7365 202d 310d 0a20 2020 2020 2020 2020  se -1..         
+00006910: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00006920: 6574 7269 6373 5b27 2f27 2e6a 6f69 6e28  etrics['/'.join(
+00006930: 5b70 7265 6669 782c 206d 6574 7269 635d  [prefix, metric]
+00006940: 295d 203d 2076 616c 0d0a 2020 2020 2020  )] = val..      
+00006950: 2020 2020 2020 2020 2020 7772 6974 6572            writer
+00006960: 2e61 6464 5f68 7061 7261 6d73 280d 0a20  .add_hparams(.. 
+00006970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006980: 2020 2070 6172 616d 732c 206d 6574 7269     params, metri
+00006990: 6373 2c0d 0a20 2020 2020 2020 2020 2020  cs,..           
+000069a0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+000069b0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+000069c0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+000069d0: 6e66 6f4c 6f67 6765 7228 0d0a 2020 2020  nfoLogger(..    
+000069e0: 2020 2020 2020 2020 2020 2020 6622 5c30              f"\0
+000069f0: 3333 5b30 3b33 313b 3437 6d5b 4164 6170  33[0;31;47m[Adap
+00006a00: 7465 725d 203e 3e3e 2055 6e6b 6e6f 776e  ter] >>> Unknown
+00006a10: 2065 7272 6f72 7320 6861 7070 656e 2e20   errors happen. 
+00006a20: 5468 6973 2069 7320 6d61 696e 6c79 2064  This is mainly d
+00006a30: 7565 2074 6f20 6162 6e6f 726d 616c 2065  ue to abnormal e
+00006a40: 7869 7473 206f 6620 6368 696c 6420 7072  xits of child pr
+00006a50: 6f63 6573 7365 732e 5c30 3333 5b30 6d22  ocesses.\033[0m"
+00006a60: 0d0a 2020 2020 2020 2020 2020 2020 290d  ..            ).
+00006a70: 0a0d 0a0d 0a20 2020 2064 6566 2065 6163  .....    def eac
+00006a80: 685f 6772 6964 2873 656c 6629 3a0d 0a20  h_grid(self):.. 
+00006a90: 2020 2020 2020 2022 2222 4772 6964 2073         """Grid s
+00006aa0: 6561 7263 6820 666f 7220 6561 6368 206b  earch for each k
+00006ab0: 696e 6420 6f66 2070 6172 616d 2e22 2222  ind of param."""
+00006ac0: 0d0a 2020 2020 2020 2020 666f 7220 6b65  ..        for ke
+00006ad0: 792c 2076 616c 7320 696e 207a 6970 2873  y, vals in zip(s
+00006ae0: 656c 662e 7061 7261 6d73 2c20 7365 6c66  elf.params, self
+00006af0: 2e76 616c 7565 7329 3a0d 0a20 2020 2020  .values):..     
+00006b00: 2020 2020 2020 2066 6f72 2076 616c 2069         for val i
+00006b10: 6e20 7661 6c73 3a0d 0a20 2020 2020 2020  n vals:..       
+00006b20: 2020 2020 2020 2020 2079 6965 6c64 2073           yield s
+00006b30: 656c 662e 6366 672e 4445 4641 554c 5453  elf.cfg.DEFAULTS
+00006b40: 207c 207b 6b65 793a 2076 616c 7d0d 0a0d   | {key: val}...
+00006b50: 0a20 2020 2064 6566 2070 726f 6475 6374  .    def product
+00006b60: 5f67 7269 6428 7365 6c66 293a 0d0a 2020  _grid(self):..  
+00006b70: 2020 2020 2020 2222 2247 7269 6420 7365        """Grid se
+00006b80: 6172 6368 2061 6372 6f73 7320 616c 6c20  arch across all 
+00006b90: 636f 6d62 696e 6174 696f 6e20 6f66 2070  combination of p
+00006ba0: 6172 616d 7322 2222 0d0a 2020 2020 2020  arams"""..      
+00006bb0: 2020 666f 7220 7661 6c73 2069 6e20 7072    for vals in pr
+00006bc0: 6f64 7563 7428 2a73 656c 662e 7661 6c75  oduct(*self.valu
+00006bd0: 6573 293a 0d0a 2020 2020 2020 2020 2020  es):..          
+00006be0: 2020 7969 656c 6420 7365 6c66 2e63 6667    yield self.cfg
+00006bf0: 2e44 4546 4155 4c54 5320 7c20 7b6f 7074  .DEFAULTS | {opt
+00006c00: 696f 6e3a 7661 6c20 666f 7220 6f70 7469  ion:val for opti
+00006c10: 6f6e 2c20 7661 6c20 696e 207a 6970 2873  on, val in zip(s
+00006c20: 656c 662e 7061 7261 6d73 2c20 7661 6c73  elf.params, vals
+00006c30: 297d 0d0a 0d0a 2020 2020 6465 6620 7361  )}....    def sa
+00006c40: 7665 5f63 6865 636b 706f 696e 7428 7365  ve_checkpoint(se
+00006c50: 6c66 2c20 736f 7572 6365 3a20 4c69 7374  lf, source: List
+00006c60: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
+00006c70: 2020 2020 2222 2253 6176 6520 7468 6520      """Save the 
+00006c80: 7265 7374 206f 6620 7061 7261 6d73 2e22  rest of params."
+00006c90: 2222 0d0a 2020 2020 2020 2020 7061 7468  ""..        path
+00006ca0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+00006cb0: 7365 6c66 2e63 6667 2e43 4f52 455f 4348  self.cfg.CORE_CH
+00006cc0: 4543 4b50 4f49 4e54 5f50 4154 482c 2073  ECKPOINT_PATH, s
+00006cd0: 656c 662e 6366 672e 4348 4543 4b50 4f49  elf.cfg.CHECKPOI
+00006ce0: 4e54 5f46 494c 454e 414d 4529 0d0a 2020  NT_FILENAME)..  
+00006cf0: 2020 2020 2020 6368 6563 6b70 6f69 6e74        checkpoint
+00006d00: 203d 2064 6963 7428 290d 0a20 2020 2020   = dict()..     
+00006d10: 2020 2063 6865 636b 706f 696e 745b 2773     checkpoint['s
+00006d20: 6f75 7263 6527 5d20 3d20 736f 7572 6365  ource'] = source
+00006d30: 0d0a 2020 2020 2020 2020 746f 7263 682e  ..        torch.
+00006d40: 7361 7665 2863 6865 636b 706f 696e 742c  save(checkpoint,
+00006d50: 2070 6174 6829 0d0a 0d0a 2020 2020 6465   path)....    de
+00006d60: 6620 6c6f 6164 5f63 6865 636b 706f 696e  f load_checkpoin
+00006d70: 7428 7365 6c66 2920 2d3e 2069 6e74 3a0d  t(self) -> int:.
+00006d80: 0a20 2020 2020 2020 2022 2222 4c6f 6164  .        """Load
+00006d90: 2074 6865 2072 6573 7420 6f66 2070 6172   the rest of par
+00006da0: 616d 732e 2222 220d 0a20 2020 2020 2020  ams."""..       
+00006db0: 2070 6174 6820 3d20 6f73 2e70 6174 682e   path = os.path.
+00006dc0: 6a6f 696e 2873 656c 662e 6366 672e 434f  join(self.cfg.CO
+00006dd0: 5245 5f43 4845 434b 504f 494e 545f 5041  RE_CHECKPOINT_PA
+00006de0: 5448 2c20 7365 6c66 2e63 6667 2e43 4845  TH, self.cfg.CHE
+00006df0: 434b 504f 494e 545f 4649 4c45 4e41 4d45  CKPOINT_FILENAME
+00006e00: 290d 0a20 2020 2020 2020 2063 6865 636b  )..        check
+00006e10: 706f 696e 7420 3d20 746f 7263 682e 6c6f  point = torch.lo
+00006e20: 6164 2870 6174 6829 0d0a 2020 2020 2020  ad(path)..      
+00006e30: 2020 7265 7475 726e 2063 6865 636b 706f    return checkpo
+00006e40: 696e 745b 2773 6f75 7263 6527 5d0d 0a0d  int['source']...
+00006e50: 0a20 2020 2040 7469 6d65 6d65 7465 7228  .    @timemeter(
+00006e60: 2243 6f61 6368 2f72 6573 756d 6522 290d  "Coach/resume").
+00006e70: 0a20 2020 2064 6566 2072 6573 756d 6528  .    def resume(
+00006e80: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00006e90: 2222 2252 6573 756d 6520 6672 6f6d 2074  """Resume from t
+00006ea0: 6865 2072 6563 656e 7420 6368 6563 6b70  he recent checkp
+00006eb0: 6f69 6e74 2e22 2222 0d0a 2020 2020 2020  oint."""..      
+00006ec0: 2020 736f 7572 6365 203d 2073 656c 662e    source = self.
+00006ed0: 6561 6368 5f67 7269 6428 2920 6966 2073  each_grid() if s
+00006ee0: 656c 662e 6366 672e 4558 434c 5553 4956  elf.cfg.EXCLUSIV
+00006ef0: 4520 656c 7365 2073 656c 662e 7072 6f64  E else self.prod
+00006f00: 7563 745f 6772 6964 2829 0d0a 2020 2020  uct_grid()..    
+00006f10: 2020 2020 736f 7572 6365 203d 206c 6973      source = lis
+00006f20: 7428 736f 7572 6365 295b 3a3a 2d31 5d0d  t(source)[::-1].
+00006f30: 0a20 2020 2020 2020 2073 6f75 7263 6520  .        source 
+00006f40: 3d20 7365 6c66 2e6c 6f61 645f 6368 6563  = self.load_chec
+00006f50: 6b70 6f69 6e74 2829 2069 6620 7365 6c66  kpoint() if self
+00006f60: 2e63 6667 2e72 6573 756d 6520 656c 7365  .cfg.resume else
+00006f70: 2073 6f75 7263 650d 0a20 2020 2020 2020   source..       
+00006f80: 2069 6e66 6f4c 6f67 6765 7228 6622 5b43   infoLogger(f"[C
+00006f90: 6f61 6368 5d20 3e3e 3e20 4c6f 6164 2074  oach] >>> Load t
+00006fa0: 6865 2072 6563 656e 7420 6368 6563 6b70  he recent checkp
+00006fb0: 6f69 6e74 202e 2e2e 2229 0d0a 2020 2020  oint ...")..    
+00006fc0: 2020 2020 7265 7475 726e 2073 6f75 7263      return sourc
+00006fd0: 650d 0a0d 0a20 2020 2064 6566 2072 756e  e....    def run
+00006fe0: 2873 656c 662c 2063 6f6d 6d61 6e64 3a20  (self, command: 
+00006ff0: 7374 722c 2070 6172 616d 733a 2044 6963  str, params: Dic
+00007000: 7429 3a0d 0a20 2020 2020 2020 2022 2222  t):..        """
+00007010: 5374 6172 7420 6120 6e65 7720 7375 6270  Start a new subp
+00007020: 726f 6365 7373 2222 220d 0a20 2020 2020  rocess"""..     
+00007030: 2020 2066 6f72 206f 7074 696f 6e2c 2076     for option, v
+00007040: 616c 2069 6e20 7061 7261 6d73 2e69 7465  al in params.ite
+00007050: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
+00007060: 2020 2063 6f6d 6d61 6e64 202b 3d20 7365     command += se
+00007070: 6c66 2e67 6574 5f6f 7074 696f 6e28 6f70  lf.get_option(op
+00007080: 7469 6f6e 2c20 7661 6c29 0d0a 2020 2020  tion, val)..    
+00007090: 2020 2020 696e 666f 4c6f 6767 6572 2866      infoLogger(f
+000070a0: 225c 3033 335b 303b 3331 3b34 376d 7b63  "\033[0;31;47m{c
+000070b0: 6f6d 6d61 6e64 7d5c 3033 335b 306d 2229  ommand}\033[0m")
+000070c0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000070d0: 2073 7562 7072 6f63 6573 732e 506f 7065   subprocess.Pope
+000070e0: 6e28 7368 6c65 782e 7370 6c69 7428 636f  n(shlex.split(co
+000070f0: 6d6d 616e 6429 290d 0a0d 0a20 2020 2064  mmand))....    d
+00007100: 6566 2077 6169 7428 7365 6c66 2c20 7461  ef wait(self, ta
+00007110: 736b 733a 2044 6963 7429 3a0d 0a20 2020  sks: Dict):..   
+00007120: 2020 2020 2022 2222 5761 6974 2075 7469       """Wait uti
+00007130: 6c20 616c 6c20 7072 6f63 6573 7365 7320  l all processes 
+00007140: 7465 726d 696e 6174 652e 2222 220d 0a20  terminate.""".. 
+00007150: 2020 2020 2020 2066 6f72 2070 726f 6365         for proce
+00007160: 7373 5f2c 2069 645f 2c20 6c6f 6750 6174  ss_, id_, logPat
+00007170: 682c 2070 6172 616d 7320 696e 2074 6173  h, params in tas
+00007180: 6b73 2e76 616c 7565 7328 293a 0d0a 2020  ks.values():..  
+00007190: 2020 2020 2020 2020 2020 7072 6f63 6573            proces
+000071a0: 735f 2e77 6169 7428 290d 0a20 2020 2020  s_.wait()..     
+000071b0: 2020 2020 2020 2073 656c 662e 7772 6974         self.writ
+000071c0: 6528 6964 5f2c 206c 6f67 5061 7468 2c20  e(id_, logPath, 
+000071d0: 7061 7261 6d73 290d 0a0d 0a20 2020 2064  params)....    d
+000071e0: 6566 2070 6f6c 6c28 7365 6c66 2c20 7461  ef poll(self, ta
+000071f0: 736b 733a 2044 6963 7429 3a0d 0a20 2020  sks: Dict):..   
+00007200: 2020 2020 2022 2222 5761 6974 2075 7469       """Wait uti
+00007210: 6c20 616e 7920 7072 6f63 6573 7320 7465  l any process te
+00007220: 726d 696e 6174 6573 2e22 2222 0d0a 2020  rminates."""..  
+00007230: 2020 2020 2020 6275 6666 6572 5f73 6f75        buffer_sou
+00007240: 7263 6520 3d20 5b5d 0d0a 2020 2020 2020  rce = []..      
+00007250: 2020 7469 6d65 2e73 6c65 6570 2831 2920    time.sleep(1) 
+00007260: 2320 666f 7220 756e 6971 7565 2069 640d  # for unique id.
+00007270: 0a20 2020 2020 2020 2077 6869 6c65 206c  .        while l
+00007280: 656e 2873 656c 662e 6465 7669 6365 7329  en(self.devices)
+00007290: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
+000072a0: 2020 2020 7469 6d65 2e73 6c65 6570 2837      time.sleep(7
+000072b0: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
+000072c0: 6f72 2064 6576 6963 652c 2028 7072 6f63  or device, (proc
+000072d0: 6573 735f 2c20 6964 5f2c 206c 6f67 5061  ess_, id_, logPa
+000072e0: 7468 2c20 7061 7261 6d73 2920 696e 2074  th, params) in t
+000072f0: 6173 6b73 2e69 7465 6d73 2829 3a0d 0a20  asks.items():.. 
+00007300: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00007310: 6620 7072 6f63 6573 735f 2e70 6f6c 6c28  f process_.poll(
+00007320: 2920 6973 206e 6f74 204e 6f6e 653a 0d0a  ) is not None:..
+00007330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007340: 2020 2020 7365 6c66 2e77 7269 7465 2869      self.write(i
+00007350: 645f 2c20 6c6f 6750 6174 682c 2070 6172  d_, logPath, par
+00007360: 616d 7329 0d0a 2020 2020 2020 2020 2020  ams)..          
+00007370: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00007380: 6576 6963 6573 2e61 7070 656e 6428 6465  evices.append(de
+00007390: 7669 6365 290d 0a20 2020 2020 2020 2020  vice)..         
+000073a0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+000073b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073c0: 2020 6275 6666 6572 5f73 6f75 7263 652e    buffer_source.
+000073d0: 6170 7065 6e64 2870 6172 616d 7329 0d0a  append(params)..
+000073e0: 2020 2020 2020 2020 7365 6c66 2e73 6176          self.sav
+000073f0: 655f 6368 6563 6b70 6f69 6e74 2873 656c  e_checkpoint(sel
+00007400: 662e 736f 7572 6365 202b 2062 7566 6665  f.source + buffe
+00007410: 725f 736f 7572 6365 290d 0a0d 0a20 2020  r_source)....   
+00007420: 2064 6566 2074 6572 6d69 6e61 7465 2873   def terminate(s
+00007430: 656c 662c 2074 6173 6b73 293a 0d0a 2020  elf, tasks):..  
+00007440: 2020 2020 2020 666f 7220 6465 7669 6365        for device
+00007450: 2069 6e20 7461 736b 733a 0d0a 2020 2020   in tasks:..    
+00007460: 2020 2020 2020 2020 7072 6f63 6573 735f          process_
+00007470: 2c20 5f2c 205f 2c20 5f20 3d20 7461 736b  , _, _, _ = task
+00007480: 735b 6465 7669 6365 5d0d 0a20 2020 2020  s[device]..     
+00007490: 2020 2020 2020 2069 6620 7072 6f63 6573         if proces
+000074a0: 735f 2e70 6f6c 6c28 2920 6973 204e 6f6e  s_.poll() is Non
+000074b0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000074c0: 2020 2020 7072 6f63 6573 735f 2e74 6572      process_.ter
+000074d0: 6d69 6e61 7465 2829 0d0a 2020 2020 2020  minate()..      
+000074e0: 2020 7469 6d65 2e73 6c65 6570 2833 290d    time.sleep(3).
+000074f0: 0a20 2020 2020 2020 2066 6f72 2064 6576  .        for dev
+00007500: 6963 6520 696e 2074 6173 6b73 3a0d 0a20  ice in tasks:.. 
+00007510: 2020 2020 2020 2020 2020 2070 726f 6365             proce
+00007520: 7373 5f2c 205f 2c20 5f2c 205f 203d 2074  ss_, _, _, _ = t
+00007530: 6173 6b73 5b64 6576 6963 655d 0d0a 2020  asks[device]..  
+00007540: 2020 2020 2020 2020 2020 6966 2070 726f            if pro
+00007550: 6365 7373 5f2e 706f 6c6c 2829 2069 7320  cess_.poll() is 
+00007560: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00007570: 2020 2020 2020 2070 726f 6365 7373 5f2e         process_.
+00007580: 6b69 6c6c 2829 0d0a 2020 2020 2020 2020  kill()..        
+00007590: 7379 732e 6578 6974 2829 0d0a 0d0a 2020  sys.exit()....  
+000075a0: 2020 4074 696d 656d 6574 6572 2822 4164    @timemeter("Ad
+000075b0: 6170 7465 722f 6669 7422 290d 0a20 2020  apter/fit")..   
+000075c0: 2064 6566 2066 6974 2873 656c 6629 3a0d   def fit(self):.
+000075d0: 0a20 2020 2020 2020 2022 2222 4772 6964  .        """Grid
+000075e0: 2073 6561 7263 682e 2222 220d 0a20 2020   search."""..   
+000075f0: 2020 2020 2073 656c 662e 736f 7572 6365       self.source
+00007600: 203d 2073 656c 662e 7265 7375 6d65 2829   = self.resume()
+00007610: 0d0a 2020 2020 2020 2020 7461 736b 7320  ..        tasks 
+00007620: 3d20 6469 6374 2829 0d0a 0d0a 2020 2020  = dict()....    
+00007630: 2020 2020 6465 6620 7369 676e 616c 5f68      def signal_h
+00007640: 616e 646c 6572 2873 6967 2c20 6672 616d  andler(sig, fram
+00007650: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
+00007660: 2069 6e66 6f4c 6f67 6765 7228 6622 5c30   infoLogger(f"\0
+00007670: 3333 5b30 3b33 313b 3437 6d3d 3d3d 3d3d  33[0;31;47m=====
+00007680: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007690: 3d3d 3d3d 3d3d 3d3d 3d3d 5445 524d 494e  ==========TERMIN
+000076a0: 4154 4520 414c 4c20 5355 4250 524f 4345  ATE ALL SUBPROCE
+000076b0: 5353 4553 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  SSES============
+000076c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000076d0: 3d3d 3d5c 3033 335b 306d 2229 0d0a 2020  ===\033[0m")..  
+000076e0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+000076f0: 6572 6d69 6e61 7465 2874 6173 6b73 290d  erminate(tasks).
+00007700: 0a20 2020 2020 2020 2073 6967 6e61 6c2e  .        signal.
+00007710: 7369 676e 616c 2873 6967 6e61 6c2e 5349  signal(signal.SI
+00007720: 4749 4e54 2c20 7369 676e 616c 5f68 616e  GINT, signal_han
+00007730: 646c 6572 290d 0a0d 0a20 2020 2020 2020  dler)....       
+00007740: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
+00007750: 2020 2077 6869 6c65 2073 656c 662e 736f     while self.so
+00007760: 7572 6365 3a0d 0a20 2020 2020 2020 2020  urce:..         
+00007770: 2020 2020 2020 2073 656c 662e 706f 6c6c         self.poll
+00007780: 2874 6173 6b73 290d 0a20 2020 2020 2020  (tasks)..       
+00007790: 2020 2020 2020 2020 2070 6172 616d 7320           params 
+000077a0: 3d20 7365 6c66 2e73 6f75 7263 652e 706f  = self.source.po
+000077b0: 7028 290d 0a20 2020 2020 2020 2020 2020  p()..           
+000077c0: 2020 2020 2064 6576 6963 6520 3d20 7365       device = se
+000077d0: 6c66 2e64 6576 6963 6573 2e70 6f70 2829  lf.devices.pop()
+000077e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000077f0: 2020 636f 6d6d 616e 642c 2069 645f 2c20    command, id_, 
+00007800: 6c6f 6750 6174 6820 3d20 7365 6c66 2e72  logPath = self.r
+00007810: 6567 6973 7465 7228 6465 7669 6365 290d  egister(device).
+00007820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007830: 2070 726f 6365 7373 5f20 3d20 7365 6c66   process_ = self
+00007840: 2e72 756e 2863 6f6d 6d61 6e64 2c20 7061  .run(command, pa
+00007850: 7261 6d73 290d 0a20 2020 2020 2020 2020  rams)..         
+00007860: 2020 2020 2020 2074 6173 6b73 5b64 6576         tasks[dev
+00007870: 6963 655d 203d 2028 7072 6f63 6573 735f  ice] = (process_
+00007880: 2c20 6964 5f2c 206c 6f67 5061 7468 2c20  , id_, logPath, 
+00007890: 7061 7261 6d73 290d 0a20 2020 2020 2020  params)..       
+000078a0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+000078b0: 6e20 6173 2065 3a0d 0a20 2020 2020 2020  n as e:..       
+000078c0: 2020 2020 2070 7269 6e74 2865 290d 0a20       print(e).. 
+000078d0: 2020 2020 2020 2066 696e 616c 6c79 3a0d         finally:.
+000078e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000078f0: 662e 7761 6974 2874 6173 6b73 290d 0a20  f.wait(tasks).. 
+00007900: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00007910: 7465 726d 696e 6174 6528 7461 736b 7329  terminate(tasks)
```

### Comparing `freerec-0.2.5/freerec/metrics.py` & `freerec-0.3.1/freerec/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     The decorator `_reduce` is applied to this function, with `reduction` set to 'mean'. 
     This means that the output of `mean_squared_error` will be the mean of the mean squared error loss values computed for each element in `preds` and `targets`.
     """
     def decorator(func):
         def wrapper(
             preds: Union[List[torch.Tensor], torch.Tensor], 
             targets: Union[List[torch.Tensor], torch.Tensor], 
+            *,
             reduction: str = reduction, **kwargs
         ):
             func_ = partial(func, **kwargs)
             if isinstance(preds, List):
                 results = torch.tensor(list(map(
                     func_, preds, targets
                 )))
```

### Comparing `freerec-0.2.5/freerec/models/base.py` & `freerec-0.3.1/freerec/models/base.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec/parser.py` & `freerec-0.3.1/freerec/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -333,36 +333,14 @@
 
     ALL_ENVS = (
         'description', 'root', 'device', 'eval_freq', 'num_workers'
     )
 
     def __init__(self) -> None:
         super().__init__(**CORE_CONFIG)
-        self.parse()
-
-    @timemeter("CoreParser/parse")
-    def parse(self):
-        """Parse command-line arguments."""
-
-        self.parser = argparse.ArgumentParser()
-
-        self.parser.add_argument("description", type=str, help="...")
-        self.parser.add_argument("config", type=str, help="config.yml")
-        self.parser.add_argument("--exclusive", action="store_true", default=False, help="one by one or one for all")
-
-        self.parser.add_argument("--root", type=str, default=None, help="data")
-        self.parser.add_argument("--dataset", type=str, default=None, help="useless if no need to automatically select a dataset")
-        self.parser.add_argument("--device", type=str, default=None, help="device")
-
-        self.parser.add_argument("--eval-freq", type=int, default=None, help="the evaluation frequency")
-
-        self.parser.add_argument("--num-workers", type=int, default=None)
-
-        self.parser.add_argument("--resume", action="store_true", default=False, help="resume the search from the recent checkpoint")
-
 
     def check(self) -> None:
         """Check the validity of the given config."""
         template = """
         Please make sure the configuration file follows the template below:
 
         command: python xxx.py
@@ -419,15 +397,15 @@
         self.EXCLUSIVE = args.exclusive
         self.resume = args.resume
         for key, val in args._get_kwargs():
             if key in self.ALL_ENVS and val is not None:
                 self.ENVS[key] = val
 
     @timemeter("CoreParser/compile")
-    def compile(self) -> None:
+    def compile(self, args) -> None:
         r"""
         Generate config file according to settings.
 
         Flows:
         ------
         1. Load settings from xxx.yaml which provides parameters for grid searching.
         2. Load settings of the execution environment from parsed args (ArgumentParser).
@@ -435,15 +413,14 @@
             - CHECKPOINT_PATH: subprocess
             - LOG_PATH: subprocess
             - CORE_CHECKPOINT_PATH: saving checkpoints of the rest of params
             - CORE_LOG_PATH: saving best results of each subprocess for comparison
         4. Set Logger, and then you can log information by info|debug|warnLogger ...
         5. Finally, READMD.md will be added under CHECKPOINT_PATH and LOG_PATH both.
         """
-        args = self.parser.parse_args()
         self.load(args)
         self.check()
 
         self['DATA_DIR'] = DATA_DIR
         self['SUMMARY_DIR'] = SUMMARY_DIR
         self['CHECKPOINT_PATH'] = CHECKPOINT_PATH
         self['LOG_PATH'] = LOG_PATH
```

### Comparing `freerec-0.2.5/freerec/utils.py` & `freerec-0.3.1/freerec/utils.py`

 * *Files identical despite different names*

### Comparing `freerec-0.2.5/freerec.egg-info/PKG-INFO` & `freerec-0.3.1/freerec.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freerec
-Version: 0.2.5
+Version: 0.3.1
 Summary: PyTorch library for recommender systems
 Home-page: https://github.com/MTandHJ/freerec
 Author: MTandHJ
 Author-email: congxueric@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -34,14 +34,17 @@
 
 
 
 ## Data Pipeline
 
 ![](docs/src/pipeline.png)
 
+**Note:** To make dataset, please download corresponding Atomic files from [[RecBole](https://drive.google.com/drive/folders/1so0lckI6N6_niVEYaBu-LIcpOdZf99kj)]. 
+Then, run `make_dataset.ipynb'.
+
 ## Training Flow
 
 
 ![](docs/src/flow.png)
 
 
 ## Reference Code
```

### Comparing `freerec-0.2.5/freerec.egg-info/SOURCES.txt` & `freerec-0.3.1/freerec.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 freerec/launcher.py
 freerec/metrics.py
 freerec/parser.py
 freerec/utils.py
 freerec.egg-info/PKG-INFO
 freerec.egg-info/SOURCES.txt
 freerec.egg-info/dependency_links.txt
+freerec.egg-info/entry_points.txt
 freerec.egg-info/requires.txt
 freerec.egg-info/top_level.txt
 freerec/data/__init__.py
 freerec/data/dataloader.py
 freerec/data/fields.py
-freerec/data/preprocessing.py
 freerec/data/tags.py
 freerec/data/transformation.py
 freerec/data/utils.py
 freerec/data/datasets/__init__.py
 freerec/data/datasets/base.py
 freerec/data/datasets/context/__init__.py
 freerec/data/datasets/context/base.py
@@ -42,9 +42,12 @@
 freerec/data/datasets/session/base.py
 freerec/data/postprocessing/__init__.py
 freerec/data/postprocessing/base.py
 freerec/data/postprocessing/column.py
 freerec/data/postprocessing/row.py
 freerec/data/postprocessing/sampler.py
 freerec/data/postprocessing/source.py
+freerec/data/preprocessing/__init__.py
+freerec/data/preprocessing/base.py
+freerec/data/preprocessing/datasets.py
 freerec/models/__init__.py
 freerec/models/base.py
```

### Comparing `freerec-0.2.5/setup.py` & `freerec-0.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 def get_property(prop, project):
     result = re.search(r'{}\s*=\s*[\'"]([^\'"]*)[\'"]'.format(prop), open(project + '/__init__.py').read())
     return result.group(1)
 
 
 setuptools.setup(
   name="freerec",
+  entry_points={
+    'console_scripts': [
+      'freerec=freerec.__main__:main',
+    ],
+  },
   version=get_property('__version__', 'freerec'),
   author="MTandHJ",
   author_email="congxueric@gmail.com",
   description="PyTorch library for recommender systems",
   long_description=long_description,
   long_description_content_type="text/markdown",
   license='MIT License',
```

