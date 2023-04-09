# Comparing `tmp/robotathome-1.1.0.tar.gz` & `tmp/robotathome-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotathome-1.1.0.tar", last modified: Sun Apr  9 11:25:36 2023, max compression
+gzip compressed data, was "robotathome-1.1.1.tar", last modified: Sun Apr  9 16:52:09 2023, max compression
```

## Comparing `robotathome-1.1.0.tar` & `robotathome-1.1.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 11:25:36.975787 robotathome-1.1.0/
--rw-r--r--   0 lightman  (1000) lightman  (1000)     1079 2022-03-21 11:50:03.000000 robotathome-1.1.0/LICENSE
--rw-rw-r--   0 lightman  (1000) lightman  (1000)    12821 2023-04-09 11:25:36.975787 robotathome-1.1.0/PKG-INFO
--rw-r--r--   0 lightman  (1000) lightman  (1000)    12097 2022-10-09 16:49:32.000000 robotathome-1.1.0/README.md
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 11:25:36.975787 robotathome-1.1.0/notebooks/
--rw-r--r--   0 lightman  (1000) lightman  (1000)    13106 2022-06-05 03:18:58.000000 robotathome-1.1.0/notebooks/05-Google-colab-drive.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)     7997 2022-06-05 03:26:04.000000 robotathome-1.1.0/notebooks/10-Download-and-install.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)    13634 2022-06-05 03:30:46.000000 robotathome-1.1.0/notebooks/20-Before-starting-the-logging-system.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)    22932 2022-06-04 14:58:34.000000 robotathome-1.1.0/notebooks/30-Getting-started-Framework-data.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)    27537 2022-06-05 03:31:30.000000 robotathome-1.1.0/notebooks/40-Captured-data.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)   937555 2022-06-04 16:10:20.000000 robotathome-1.1.0/notebooks/50-RGBD-observations.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)    42602 2022-06-05 02:05:56.000000 robotathome-1.1.0/notebooks/60-Lsrscan-observations.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)   484536 2022-06-05 02:50:00.000000 robotathome-1.1.0/notebooks/70-Scenes.ipynb
--rw-r--r--   0 lightman  (1000) lightman  (1000)    30269 2022-06-05 03:03:54.000000 robotathome-1.1.0/notebooks/80-Characterized-observations.ipynb
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 11:25:36.975787 robotathome-1.1.0/rh_schema_diagram/
--rw-r--r--   0 lightman  (1000) lightman  (1000)    38841 2022-03-21 11:50:03.000000 robotathome-1.1.0/rh_schema_diagram/rh_schema_brief.pdf
--rw-r--r--   0 lightman  (1000) lightman  (1000)    40694 2022-03-21 11:50:03.000000 robotathome-1.1.0/rh_schema_diagram/rh_schema_full.pdf
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 11:25:36.975787 robotathome-1.1.0/robotathome/
--rw-rw-r--   0 lightman  (1000) lightman  (1000)      473 2023-04-09 10:57:14.000000 robotathome-1.1.0/robotathome/__init__.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)      754 2022-03-21 11:50:03.000000 robotathome-1.1.0/robotathome/_version.py
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 11:25:36.975787 robotathome-1.1.0/robotathome/core/
--rw-rw-r--   0 lightman  (1000) lightman  (1000)      178 2023-04-09 10:57:14.000000 robotathome-1.1.0/robotathome/core/__init__.py
--rw-rw-r--   0 lightman  (1000) lightman  (1000)     4765 2023-04-09 10:57:14.000000 robotathome-1.1.0/robotathome/core/df.py
--rw-rw-r--   0 lightman  (1000) lightman  (1000)    46199 2023-04-09 10:57:14.000000 robotathome-1.1.0/robotathome/core/reader.py
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 11:25:36.975787 robotathome-1.1.0/robotathome/cv/
--rw-r--r--   0 lightman  (1000) lightman  (1000)      194 2022-03-21 11:50:03.000000 robotathome-1.1.0/robotathome/cv/__init__.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)      302 2022-03-21 11:50:03.000000 robotathome-1.1.0/robotathome/cv/_greetings.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)    20144 2022-03-21 11:50:03.000000 robotathome-1.1.0/robotathome/cv/gluoncv.py
--rw-rw-r--   0 lightman  (1000) lightman  (1000)    16622 2023-04-09 10:57:14.000000 robotathome-1.1.0/robotathome/cv/opencv.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)     6705 2022-03-21 11:50:03.000000 robotathome-1.1.0/robotathome/helpers.py
--rw-r--r--   0 lightman  (1000) lightman  (1000)     1464 2022-03-21 11:50:03.000000 robotathome-1.1.0/robotathome/log.py
-drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 11:25:36.975787 robotathome-1.1.0/robotathome.egg-info/
--rw-r--r--   0 lightman  (1000) lightman  (1000)    12821 2023-04-09 11:25:36.000000 robotathome-1.1.0/robotathome.egg-info/PKG-INFO
--rw-r--r--   0 lightman  (1000) lightman  (1000)      915 2023-04-09 11:25:36.000000 robotathome-1.1.0/robotathome.egg-info/SOURCES.txt
--rw-r--r--   0 lightman  (1000) lightman  (1000)        1 2023-04-09 11:25:36.000000 robotathome-1.1.0/robotathome.egg-info/dependency_links.txt
--rw-r--r--   0 lightman  (1000) lightman  (1000)      226 2023-04-09 11:25:36.000000 robotathome-1.1.0/robotathome.egg-info/requires.txt
--rw-r--r--   0 lightman  (1000) lightman  (1000)       12 2023-04-09 11:25:36.000000 robotathome-1.1.0/robotathome.egg-info/top_level.txt
--rw-rw-r--   0 lightman  (1000) lightman  (1000)       38 2023-04-09 11:25:36.975787 robotathome-1.1.0/setup.cfg
--rw-rw-r--   0 lightman  (1000) lightman  (1000)     3306 2023-04-09 11:24:37.000000 robotathome-1.1.0/setup.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 16:52:09.448596 robotathome-1.1.1/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     1079 2022-03-21 11:50:03.000000 robotathome-1.1.1/LICENSE
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)    12802 2023-04-09 16:52:09.448596 robotathome-1.1.1/PKG-INFO
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    12078 2023-04-09 16:48:14.000000 robotathome-1.1.1/README.md
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 16:52:09.444595 robotathome-1.1.1/notebooks/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    13106 2022-06-05 03:18:58.000000 robotathome-1.1.1/notebooks/05-Google-colab-drive.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     7997 2022-06-05 03:26:04.000000 robotathome-1.1.1/notebooks/10-Download-and-install.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    13634 2022-06-05 03:30:46.000000 robotathome-1.1.1/notebooks/20-Before-starting-the-logging-system.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    22932 2022-06-04 14:58:34.000000 robotathome-1.1.1/notebooks/30-Getting-started-Framework-data.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    27537 2022-06-05 03:31:30.000000 robotathome-1.1.1/notebooks/40-Captured-data.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)   937555 2022-06-04 16:10:20.000000 robotathome-1.1.1/notebooks/50-RGBD-observations.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    42602 2022-06-05 02:05:56.000000 robotathome-1.1.1/notebooks/60-Lsrscan-observations.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)   484536 2022-06-05 02:50:00.000000 robotathome-1.1.1/notebooks/70-Scenes.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    30269 2022-06-05 03:03:54.000000 robotathome-1.1.1/notebooks/80-Characterized-observations.ipynb
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 16:52:09.444595 robotathome-1.1.1/rh_schema_diagram/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    38841 2022-03-21 11:50:03.000000 robotathome-1.1.1/rh_schema_diagram/rh_schema_brief.pdf
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    40694 2022-03-21 11:50:03.000000 robotathome-1.1.1/rh_schema_diagram/rh_schema_full.pdf
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 16:52:09.444595 robotathome-1.1.1/robotathome/
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)      473 2023-04-09 16:51:03.000000 robotathome-1.1.1/robotathome/__init__.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      754 2022-03-21 11:50:03.000000 robotathome-1.1.1/robotathome/_version.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 16:52:09.448596 robotathome-1.1.1/robotathome/core/
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)      178 2023-04-09 10:57:14.000000 robotathome-1.1.1/robotathome/core/__init__.py
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)     4765 2023-04-09 10:57:14.000000 robotathome-1.1.1/robotathome/core/df.py
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)    46199 2023-04-09 10:57:14.000000 robotathome-1.1.1/robotathome/core/reader.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 16:52:09.448596 robotathome-1.1.1/robotathome/cv/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      194 2022-03-21 11:50:03.000000 robotathome-1.1.1/robotathome/cv/__init__.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      302 2022-03-21 11:50:03.000000 robotathome-1.1.1/robotathome/cv/_greetings.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    20144 2022-03-21 11:50:03.000000 robotathome-1.1.1/robotathome/cv/gluoncv.py
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)    16622 2023-04-09 10:57:14.000000 robotathome-1.1.1/robotathome/cv/opencv.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     6705 2022-03-21 11:50:03.000000 robotathome-1.1.1/robotathome/helpers.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     1464 2022-03-21 11:50:03.000000 robotathome-1.1.1/robotathome/log.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 16:52:09.448596 robotathome-1.1.1/robotathome.egg-info/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    12802 2023-04-09 16:52:09.000000 robotathome-1.1.1/robotathome.egg-info/PKG-INFO
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      915 2023-04-09 16:52:09.000000 robotathome-1.1.1/robotathome.egg-info/SOURCES.txt
+-rw-r--r--   0 lightman  (1000) lightman  (1000)        1 2023-04-09 16:52:09.000000 robotathome-1.1.1/robotathome.egg-info/dependency_links.txt
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      226 2023-04-09 16:52:09.000000 robotathome-1.1.1/robotathome.egg-info/requires.txt
+-rw-r--r--   0 lightman  (1000) lightman  (1000)       12 2023-04-09 16:52:09.000000 robotathome-1.1.1/robotathome.egg-info/top_level.txt
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)       38 2023-04-09 16:52:09.448596 robotathome-1.1.1/setup.cfg
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)     3306 2023-04-09 11:24:37.000000 robotathome-1.1.1/setup.py
```

### Comparing `robotathome-1.1.0/LICENSE` & `robotathome-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.0/PKG-INFO` & `robotathome-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotathome
-Version: 1.1.0
+Version: 1.1.1
 Summary: This package provides a Python Toolbox with a set of functions to assist in the management of Robot@Home2 Dataset
 Home-page: https://github.com/goyoambrosio/RobotAtHome2
 Author: G. Ambrosio-Cestero
 Author-email: gambrosio@uma.es
 License: MIT
 Keywords: toolbox dataset database relational model mobile robotics computer vision
 Platform: Windows
@@ -18,18 +18,17 @@
 Provides-Extra: interactive
 Provides-Extra: cv
 License-File: LICENSE
 
 # Robot@Home2 Dataset Toolbox #
 
 [![PyPI](https://img.shields.io/pypi/v/robotathome)](https://pypi.org/project/robotathome/ "R@H2 as PyPI package ready to install")
-[![DOI](https://zenodo.org/badge/245370645.svg)](https://zenodo.org/badge/latestdoi/245370645 "This repository released on Zenodo")
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4530453.svg)](https://doi.org/10.5281/zenodo.4530453 "The downloadable R@H2 dataset in Zenodo")
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7811795.svg)](https://doi.org/10.5281/zenodo.7811795 "The downloadable R@H2 dataset in Zenodo")
 [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/drive/folders/1ENnxbKP5MJdlGl2Q93WTbIlofuy6Icxq)
-
+<!-- [![DOI](https://zenodo.org/badge/245370645.svg)](https://zenodo.org/badge/latestdoi/245370645 "This repository released on Zenodo") -->
 The Robot-at-Home dataset (Robot@Home, paper
 [here](http://mapir.uma.es/papersrepo/2017/2017-raul-IJRR-Robot_at_home_dataset.pdf))
 is a collection of raw and processed data from five domestic settings compiled
 by a mobile robot equipped with 4 RGB-D cameras and a 2D laser scanner. Its main
 purpose is to serve as a testbed for semantic mapping algorithms through the
 categorization of objects and/or rooms.
 
@@ -255,73 +254,72 @@
     > `interactive` will include jupyter and needed libraries.
 
 3.  Run `python` and import the `robotathome` library
 
     ```
     $ python
 
-    Python 3.7.11 (default, Jul 27 2021, 14:32:16) 
-    [GCC 7.5.0] :: Anaconda, Inc. on linux
+    Python 3.10.9 (main, Jan 11 2023, 15:21:40) [GCC 11.2.0] on linux
     Type "help", "copyright", "credits" or "license" for more information.
     >>> import robotathome as rh
     >>> print (rh.__version__)
-    0.5.0
+    1.1.0
     ```
 
 4.  Congratulations ! the `robotathome` package has been installed successfully.
 
 
 ### Downloading the dataset
 
 Robot@Home resides in Zenodo site where all data versions can be downloaded.
-Latest version ([v2.0.1](https://zenodo.org/record/4530453)) is composed of two
+Latest version ([v2.0.3](https://zenodo.org/record/7811795)) is composed of two
 files: `Robot@Home2_db.tgz` and `Robot@Home2_files.tgz`. The first one contains the
 database, and the second one contains the bunch of RGBD images and 3D scenes
 
 You can choose to download it on your own or through the new brand toolbox.
 
 In case you are considering Linux
 
 ```shell
-$ wget https://zenodo.org/record/4530453/files/Robot@Home2_db.tgz
-$ wget https://zenodo.org/record/4530453/files/Robot@Home2_files.tgz
+$ wget https://zenodo.org/record/7811795/files/Robot@Home2_db.tgz
+$ wget https://zenodo.org/record/7811795/files/Robot@Home2_files.tgz
 ```
 
 check the files integrity
 
 ```shell
 $ md5sum Robot@Home2_db.tgz 
-c2a3536b6b98b907c56eda3a78300cbe  Robot@Home2_db.tgz
+d34fb44c01f31c87be8ab14e5ecd0767  Robot@Home2_db.tgz
 
 $ md5sum Robot@Home2_files.tgz 
 c55465536738ec3470c75e1671bab5f2  Robot@Home2_files.tgz
 ```
 
 and to finish unzip files
 
 ```shell
-$ pv /home/user/Downloads/Robot@Home2_db.tgz | tar -J -xf - -C /home/user/WORKSPACE/
+$ pv /home/user/Downloads/Robot@Home2_db.tgz | tar -xzf - -C /home/user/WORKSPACE/
 $ pv /home/user/Downloads/Robot@Home2_files.tgz | tar -xzf - -C /home/user/WORKSPACE/files
 ```
 
 or even better, now you can do the same programmatically using the toolbox
 
 ```python
 import robotathome as rh
 
 # Download files
-rh.download('https://zenodo.org/record/4530453/files/Robot@Home2_db.tgz', '~/Downloads')
-rh.download('https://zenodo.org/record/4530453/files/Robot@Home2_files.tgz', '~/Downloads')
+rh.download('https://zenodo.org/record/7811795/files/Robot@Home2_db.tgz', '~/Downloads')
+rh.download('https://zenodo.org/record/7811795/files/Robot@Home2_files.tgz', '~/Downloads')
 
 # Compute md5 checksums
 md5_checksum_db = rh.get_md5('~/Downloads/Robot@Home2_db.tgz')
 md5_checksum_files = rh.get_md5('~/Downloads/Robot@Home2_files.tgz')
 
 # Check the files integrity and download
-if md5_checksum_db == 'c2a3536b6b98b907c56eda3a78300cbe':
+if md5_checksum_db == 'd34fb44c01f31c87be8ab14e5ecd0767':
     rh.uncompress('~/Downloads/Robot@Home2_db.tgz', '~/WORKSPACE')
 else:
     print('Integrity of Robot@Home2_db.tgz is compromised, please download again')
     
 if md5_checksum_files == 'c55465536738ec3470c75e1671bab5f2':
     rh.uncompress('~/Downloads/Robot@Home2_files.tgz', '~/WORKSPACE/files')
 else:
```

### Comparing `robotathome-1.1.0/README.md` & `robotathome-1.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Robot@Home2 Dataset Toolbox #
 
 [![PyPI](https://img.shields.io/pypi/v/robotathome)](https://pypi.org/project/robotathome/ "R@H2 as PyPI package ready to install")
-[![DOI](https://zenodo.org/badge/245370645.svg)](https://zenodo.org/badge/latestdoi/245370645 "This repository released on Zenodo")
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4530453.svg)](https://doi.org/10.5281/zenodo.4530453 "The downloadable R@H2 dataset in Zenodo")
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7811795.svg)](https://doi.org/10.5281/zenodo.7811795 "The downloadable R@H2 dataset in Zenodo")
 [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/drive/folders/1ENnxbKP5MJdlGl2Q93WTbIlofuy6Icxq)
-
+<!-- [![DOI](https://zenodo.org/badge/245370645.svg)](https://zenodo.org/badge/latestdoi/245370645 "This repository released on Zenodo") -->
 The Robot-at-Home dataset (Robot@Home, paper
 [here](http://mapir.uma.es/papersrepo/2017/2017-raul-IJRR-Robot_at_home_dataset.pdf))
 is a collection of raw and processed data from five domestic settings compiled
 by a mobile robot equipped with 4 RGB-D cameras and a 2D laser scanner. Its main
 purpose is to serve as a testbed for semantic mapping algorithms through the
 categorization of objects and/or rooms.
 
@@ -234,73 +233,72 @@
     > `interactive` will include jupyter and needed libraries.
 
 3.  Run `python` and import the `robotathome` library
 
     ```
     $ python
 
-    Python 3.7.11 (default, Jul 27 2021, 14:32:16) 
-    [GCC 7.5.0] :: Anaconda, Inc. on linux
+    Python 3.10.9 (main, Jan 11 2023, 15:21:40) [GCC 11.2.0] on linux
     Type "help", "copyright", "credits" or "license" for more information.
     >>> import robotathome as rh
     >>> print (rh.__version__)
-    0.5.0
+    1.1.0
     ```
 
 4.  Congratulations ! the `robotathome` package has been installed successfully.
 
 
 ### Downloading the dataset
 
 Robot@Home resides in Zenodo site where all data versions can be downloaded.
-Latest version ([v2.0.1](https://zenodo.org/record/4530453)) is composed of two
+Latest version ([v2.0.3](https://zenodo.org/record/7811795)) is composed of two
 files: `Robot@Home2_db.tgz` and `Robot@Home2_files.tgz`. The first one contains the
 database, and the second one contains the bunch of RGBD images and 3D scenes
 
 You can choose to download it on your own or through the new brand toolbox.
 
 In case you are considering Linux
 
 ```shell
-$ wget https://zenodo.org/record/4530453/files/Robot@Home2_db.tgz
-$ wget https://zenodo.org/record/4530453/files/Robot@Home2_files.tgz
+$ wget https://zenodo.org/record/7811795/files/Robot@Home2_db.tgz
+$ wget https://zenodo.org/record/7811795/files/Robot@Home2_files.tgz
 ```
 
 check the files integrity
 
 ```shell
 $ md5sum Robot@Home2_db.tgz 
-c2a3536b6b98b907c56eda3a78300cbe  Robot@Home2_db.tgz
+d34fb44c01f31c87be8ab14e5ecd0767  Robot@Home2_db.tgz
 
 $ md5sum Robot@Home2_files.tgz 
 c55465536738ec3470c75e1671bab5f2  Robot@Home2_files.tgz
 ```
 
 and to finish unzip files
 
 ```shell
-$ pv /home/user/Downloads/Robot@Home2_db.tgz | tar -J -xf - -C /home/user/WORKSPACE/
+$ pv /home/user/Downloads/Robot@Home2_db.tgz | tar -xzf - -C /home/user/WORKSPACE/
 $ pv /home/user/Downloads/Robot@Home2_files.tgz | tar -xzf - -C /home/user/WORKSPACE/files
 ```
 
 or even better, now you can do the same programmatically using the toolbox
 
 ```python
 import robotathome as rh
 
 # Download files
-rh.download('https://zenodo.org/record/4530453/files/Robot@Home2_db.tgz', '~/Downloads')
-rh.download('https://zenodo.org/record/4530453/files/Robot@Home2_files.tgz', '~/Downloads')
+rh.download('https://zenodo.org/record/7811795/files/Robot@Home2_db.tgz', '~/Downloads')
+rh.download('https://zenodo.org/record/7811795/files/Robot@Home2_files.tgz', '~/Downloads')
 
 # Compute md5 checksums
 md5_checksum_db = rh.get_md5('~/Downloads/Robot@Home2_db.tgz')
 md5_checksum_files = rh.get_md5('~/Downloads/Robot@Home2_files.tgz')
 
 # Check the files integrity and download
-if md5_checksum_db == 'c2a3536b6b98b907c56eda3a78300cbe':
+if md5_checksum_db == 'd34fb44c01f31c87be8ab14e5ecd0767':
     rh.uncompress('~/Downloads/Robot@Home2_db.tgz', '~/WORKSPACE')
 else:
     print('Integrity of Robot@Home2_db.tgz is compromised, please download again')
     
 if md5_checksum_files == 'c55465536738ec3470c75e1671bab5f2':
     rh.uncompress('~/Downloads/Robot@Home2_files.tgz', '~/WORKSPACE/files')
 else:
```

### Comparing `robotathome-1.1.0/notebooks/05-Google-colab-drive.ipynb` & `robotathome-1.1.1/notebooks/05-Google-colab-drive.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.0/notebooks/10-Download-and-install.ipynb` & `robotathome-1.1.1/notebooks/10-Download-and-install.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.0/notebooks/20-Before-starting-the-logging-system.ipynb` & `robotathome-1.1.1/notebooks/20-Before-starting-the-logging-system.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.0/notebooks/30-Getting-started-Framework-data.ipynb` & `robotathome-1.1.1/notebooks/30-Getting-started-Framework-data.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.0/notebooks/40-Captured-data.ipynb` & `robotathome-1.1.1/notebooks/40-Captured-data.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.0/notebooks/50-RGBD-observations.ipynb` & `robotathome-1.1.1/notebooks/50-RGBD-observations.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.0/notebooks/60-Lsrscan-observations.ipynb` & `robotathome-1.1.1/notebooks/60-Lsrscan-observations.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.0/notebooks/70-Scenes.ipynb` & `robotathome-1.1.1/notebooks/70-Scenes.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.0/notebooks/80-Characterized-observations.ipynb` & `robotathome-1.1.1/notebooks/80-Characterized-observations.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.0/rh_schema_diagram/rh_schema_brief.pdf` & `robotathome-1.1.1/rh_schema_diagram/rh_schema_brief.pdf`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.0/rh_schema_diagram/rh_schema_full.pdf` & `robotathome-1.1.1/rh_schema_diagram/rh_schema_full.pdf`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.0/robotathome/_version.py` & `robotathome-1.1.1/robotathome/_version.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.0/robotathome/core/df.py` & `robotathome-1.1.1/robotathome/core/df.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.0/robotathome/core/reader.py` & `robotathome-1.1.1/robotathome/core/reader.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.0/robotathome/cv/gluoncv.py` & `robotathome-1.1.1/robotathome/cv/gluoncv.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.0/robotathome/cv/opencv.py` & `robotathome-1.1.1/robotathome/cv/opencv.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.0/robotathome/helpers.py` & `robotathome-1.1.1/robotathome/helpers.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.0/robotathome/log.py` & `robotathome-1.1.1/robotathome/log.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.0/robotathome.egg-info/PKG-INFO` & `robotathome-1.1.1/robotathome.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotathome
-Version: 1.1.0
+Version: 1.1.1
 Summary: This package provides a Python Toolbox with a set of functions to assist in the management of Robot@Home2 Dataset
 Home-page: https://github.com/goyoambrosio/RobotAtHome2
 Author: G. Ambrosio-Cestero
 Author-email: gambrosio@uma.es
 License: MIT
 Keywords: toolbox dataset database relational model mobile robotics computer vision
 Platform: Windows
@@ -18,18 +18,17 @@
 Provides-Extra: interactive
 Provides-Extra: cv
 License-File: LICENSE
 
 # Robot@Home2 Dataset Toolbox #
 
 [![PyPI](https://img.shields.io/pypi/v/robotathome)](https://pypi.org/project/robotathome/ "R@H2 as PyPI package ready to install")
-[![DOI](https://zenodo.org/badge/245370645.svg)](https://zenodo.org/badge/latestdoi/245370645 "This repository released on Zenodo")
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4530453.svg)](https://doi.org/10.5281/zenodo.4530453 "The downloadable R@H2 dataset in Zenodo")
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7811795.svg)](https://doi.org/10.5281/zenodo.7811795 "The downloadable R@H2 dataset in Zenodo")
 [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/drive/folders/1ENnxbKP5MJdlGl2Q93WTbIlofuy6Icxq)
-
+<!-- [![DOI](https://zenodo.org/badge/245370645.svg)](https://zenodo.org/badge/latestdoi/245370645 "This repository released on Zenodo") -->
 The Robot-at-Home dataset (Robot@Home, paper
 [here](http://mapir.uma.es/papersrepo/2017/2017-raul-IJRR-Robot_at_home_dataset.pdf))
 is a collection of raw and processed data from five domestic settings compiled
 by a mobile robot equipped with 4 RGB-D cameras and a 2D laser scanner. Its main
 purpose is to serve as a testbed for semantic mapping algorithms through the
 categorization of objects and/or rooms.
 
@@ -255,73 +254,72 @@
     > `interactive` will include jupyter and needed libraries.
 
 3.  Run `python` and import the `robotathome` library
 
     ```
     $ python
 
-    Python 3.7.11 (default, Jul 27 2021, 14:32:16) 
-    [GCC 7.5.0] :: Anaconda, Inc. on linux
+    Python 3.10.9 (main, Jan 11 2023, 15:21:40) [GCC 11.2.0] on linux
     Type "help", "copyright", "credits" or "license" for more information.
     >>> import robotathome as rh
     >>> print (rh.__version__)
-    0.5.0
+    1.1.0
     ```
 
 4.  Congratulations ! the `robotathome` package has been installed successfully.
 
 
 ### Downloading the dataset
 
 Robot@Home resides in Zenodo site where all data versions can be downloaded.
-Latest version ([v2.0.1](https://zenodo.org/record/4530453)) is composed of two
+Latest version ([v2.0.3](https://zenodo.org/record/7811795)) is composed of two
 files: `Robot@Home2_db.tgz` and `Robot@Home2_files.tgz`. The first one contains the
 database, and the second one contains the bunch of RGBD images and 3D scenes
 
 You can choose to download it on your own or through the new brand toolbox.
 
 In case you are considering Linux
 
 ```shell
-$ wget https://zenodo.org/record/4530453/files/Robot@Home2_db.tgz
-$ wget https://zenodo.org/record/4530453/files/Robot@Home2_files.tgz
+$ wget https://zenodo.org/record/7811795/files/Robot@Home2_db.tgz
+$ wget https://zenodo.org/record/7811795/files/Robot@Home2_files.tgz
 ```
 
 check the files integrity
 
 ```shell
 $ md5sum Robot@Home2_db.tgz 
-c2a3536b6b98b907c56eda3a78300cbe  Robot@Home2_db.tgz
+d34fb44c01f31c87be8ab14e5ecd0767  Robot@Home2_db.tgz
 
 $ md5sum Robot@Home2_files.tgz 
 c55465536738ec3470c75e1671bab5f2  Robot@Home2_files.tgz
 ```
 
 and to finish unzip files
 
 ```shell
-$ pv /home/user/Downloads/Robot@Home2_db.tgz | tar -J -xf - -C /home/user/WORKSPACE/
+$ pv /home/user/Downloads/Robot@Home2_db.tgz | tar -xzf - -C /home/user/WORKSPACE/
 $ pv /home/user/Downloads/Robot@Home2_files.tgz | tar -xzf - -C /home/user/WORKSPACE/files
 ```
 
 or even better, now you can do the same programmatically using the toolbox
 
 ```python
 import robotathome as rh
 
 # Download files
-rh.download('https://zenodo.org/record/4530453/files/Robot@Home2_db.tgz', '~/Downloads')
-rh.download('https://zenodo.org/record/4530453/files/Robot@Home2_files.tgz', '~/Downloads')
+rh.download('https://zenodo.org/record/7811795/files/Robot@Home2_db.tgz', '~/Downloads')
+rh.download('https://zenodo.org/record/7811795/files/Robot@Home2_files.tgz', '~/Downloads')
 
 # Compute md5 checksums
 md5_checksum_db = rh.get_md5('~/Downloads/Robot@Home2_db.tgz')
 md5_checksum_files = rh.get_md5('~/Downloads/Robot@Home2_files.tgz')
 
 # Check the files integrity and download
-if md5_checksum_db == 'c2a3536b6b98b907c56eda3a78300cbe':
+if md5_checksum_db == 'd34fb44c01f31c87be8ab14e5ecd0767':
     rh.uncompress('~/Downloads/Robot@Home2_db.tgz', '~/WORKSPACE')
 else:
     print('Integrity of Robot@Home2_db.tgz is compromised, please download again')
     
 if md5_checksum_files == 'c55465536738ec3470c75e1671bab5f2':
     rh.uncompress('~/Downloads/Robot@Home2_files.tgz', '~/WORKSPACE/files')
 else:
```

### Comparing `robotathome-1.1.0/robotathome.egg-info/SOURCES.txt` & `robotathome-1.1.1/robotathome.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotathome-1.1.0/setup.py` & `robotathome-1.1.1/setup.py`

 * *Files identical despite different names*

