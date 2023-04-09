# Comparing `tmp/robotathome-1.0.6.tar.gz` & `tmp/robotathome-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotathome-1.0.6.tar", last modified: Sun Jun  5 12:47:40 2022, max compression
+gzip compressed data, was "robotathome-1.1.0.tar", last modified: Sun Apr  9 11:25:36 2023, max compression
```

## Comparing `robotathome-1.0.6.tar` & `robotathome-1.1.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 goyo      (1000) goyo      (1000)        0 2022-06-05 12:47:40.000000 robotathome-1.0.6/
--rw-r--r--   0 goyo      (1000) goyo      (1000)     1079 2022-03-21 11:50:03.000000 robotathome-1.0.6/LICENSE
--rw-r--r--   0 goyo      (1000) goyo      (1000)    12578 2022-06-05 12:47:40.000000 robotathome-1.0.6/PKG-INFO
--rw-r--r--   0 goyo      (1000) goyo      (1000)    11731 2022-03-21 11:50:03.000000 robotathome-1.0.6/README.md
-drwxr-xr-x   0 goyo      (1000) goyo      (1000)        0 2022-06-05 12:47:40.000000 robotathome-1.0.6/notebooks/
--rw-r--r--   0 goyo      (1000) goyo      (1000)    13106 2022-06-05 03:18:58.000000 robotathome-1.0.6/notebooks/05-Google-colab-drive.ipynb
--rw-r--r--   0 goyo      (1000) goyo      (1000)     7997 2022-06-05 03:26:04.000000 robotathome-1.0.6/notebooks/10-Download-and-install.ipynb
--rw-r--r--   0 goyo      (1000) goyo      (1000)    13634 2022-06-05 03:30:46.000000 robotathome-1.0.6/notebooks/20-Before-starting-the-logging-system.ipynb
--rw-r--r--   0 goyo      (1000) goyo      (1000)    22932 2022-06-04 14:58:34.000000 robotathome-1.0.6/notebooks/30-Getting-started-Framework-data.ipynb
--rw-r--r--   0 goyo      (1000) goyo      (1000)    27537 2022-06-05 03:31:30.000000 robotathome-1.0.6/notebooks/40-Captured-data.ipynb
--rw-r--r--   0 goyo      (1000) goyo      (1000)   937555 2022-06-04 16:10:20.000000 robotathome-1.0.6/notebooks/50-RGBD-observations.ipynb
--rw-r--r--   0 goyo      (1000) goyo      (1000)    42602 2022-06-05 02:05:56.000000 robotathome-1.0.6/notebooks/60-Lsrscan-observations.ipynb
--rw-r--r--   0 goyo      (1000) goyo      (1000)   484536 2022-06-05 02:50:00.000000 robotathome-1.0.6/notebooks/70-Scenes.ipynb
--rw-r--r--   0 goyo      (1000) goyo      (1000)    30269 2022-06-05 03:03:54.000000 robotathome-1.0.6/notebooks/80-Characterized-observations.ipynb
-drwxr-xr-x   0 goyo      (1000) goyo      (1000)        0 2022-06-05 12:47:40.000000 robotathome-1.0.6/rh_schema_diagram/
--rw-r--r--   0 goyo      (1000) goyo      (1000)    38841 2022-03-21 11:50:03.000000 robotathome-1.0.6/rh_schema_diagram/rh_schema_brief.pdf
--rw-r--r--   0 goyo      (1000) goyo      (1000)    40694 2022-03-21 11:50:03.000000 robotathome-1.0.6/rh_schema_diagram/rh_schema_full.pdf
-drwxr-xr-x   0 goyo      (1000) goyo      (1000)        0 2022-06-05 12:47:40.000000 robotathome-1.0.6/robotathome/
--rw-r--r--   0 goyo      (1000) goyo      (1000)      481 2022-06-04 16:11:42.000000 robotathome-1.0.6/robotathome/__init__.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)      754 2022-03-21 11:50:03.000000 robotathome-1.0.6/robotathome/_version.py
-drwxr-xr-x   0 goyo      (1000) goyo      (1000)        0 2022-06-05 12:47:40.000000 robotathome-1.0.6/robotathome/core/
--rw-r--r--   0 goyo      (1000) goyo      (1000)      135 2022-03-21 11:50:03.000000 robotathome-1.0.6/robotathome/core/__init__.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)    31893 2022-03-21 11:50:03.000000 robotathome-1.0.6/robotathome/core/reader.py
-drwxr-xr-x   0 goyo      (1000) goyo      (1000)        0 2022-06-05 12:47:40.000000 robotathome-1.0.6/robotathome/cv/
--rw-r--r--   0 goyo      (1000) goyo      (1000)      194 2022-03-21 11:50:03.000000 robotathome-1.0.6/robotathome/cv/__init__.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)      302 2022-03-21 11:50:03.000000 robotathome-1.0.6/robotathome/cv/_greetings.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)    20144 2022-03-21 11:50:03.000000 robotathome-1.0.6/robotathome/cv/gluoncv.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)    15552 2022-03-21 11:50:03.000000 robotathome-1.0.6/robotathome/cv/opencv.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)     6705 2022-03-21 11:50:03.000000 robotathome-1.0.6/robotathome/helpers.py
--rw-r--r--   0 goyo      (1000) goyo      (1000)     1464 2022-03-21 11:50:03.000000 robotathome-1.0.6/robotathome/log.py
-drwxr-xr-x   0 goyo      (1000) goyo      (1000)        0 2022-06-05 12:47:40.000000 robotathome-1.0.6/robotathome.egg-info/
--rw-r--r--   0 goyo      (1000) goyo      (1000)    12578 2022-06-05 12:47:40.000000 robotathome-1.0.6/robotathome.egg-info/PKG-INFO
--rw-r--r--   0 goyo      (1000) goyo      (1000)      892 2022-06-05 12:47:40.000000 robotathome-1.0.6/robotathome.egg-info/SOURCES.txt
--rw-r--r--   0 goyo      (1000) goyo      (1000)        1 2022-06-05 12:47:40.000000 robotathome-1.0.6/robotathome.egg-info/dependency_links.txt
--rw-r--r--   0 goyo      (1000) goyo      (1000)      226 2022-06-05 12:47:40.000000 robotathome-1.0.6/robotathome.egg-info/requires.txt
--rw-r--r--   0 goyo      (1000) goyo      (1000)       12 2022-06-05 12:47:40.000000 robotathome-1.0.6/robotathome.egg-info/top_level.txt
--rw-r--r--   0 goyo      (1000) goyo      (1000)       38 2022-06-05 12:47:40.000000 robotathome-1.0.6/setup.cfg
--rw-r--r--   0 goyo      (1000) goyo      (1000)     3498 2022-06-04 16:11:11.000000 robotathome-1.0.6/setup.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 11:25:36.975787 robotathome-1.1.0/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     1079 2022-03-21 11:50:03.000000 robotathome-1.1.0/LICENSE
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)    12821 2023-04-09 11:25:36.975787 robotathome-1.1.0/PKG-INFO
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    12097 2022-10-09 16:49:32.000000 robotathome-1.1.0/README.md
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 11:25:36.975787 robotathome-1.1.0/notebooks/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    13106 2022-06-05 03:18:58.000000 robotathome-1.1.0/notebooks/05-Google-colab-drive.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     7997 2022-06-05 03:26:04.000000 robotathome-1.1.0/notebooks/10-Download-and-install.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    13634 2022-06-05 03:30:46.000000 robotathome-1.1.0/notebooks/20-Before-starting-the-logging-system.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    22932 2022-06-04 14:58:34.000000 robotathome-1.1.0/notebooks/30-Getting-started-Framework-data.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    27537 2022-06-05 03:31:30.000000 robotathome-1.1.0/notebooks/40-Captured-data.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)   937555 2022-06-04 16:10:20.000000 robotathome-1.1.0/notebooks/50-RGBD-observations.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    42602 2022-06-05 02:05:56.000000 robotathome-1.1.0/notebooks/60-Lsrscan-observations.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)   484536 2022-06-05 02:50:00.000000 robotathome-1.1.0/notebooks/70-Scenes.ipynb
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    30269 2022-06-05 03:03:54.000000 robotathome-1.1.0/notebooks/80-Characterized-observations.ipynb
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 11:25:36.975787 robotathome-1.1.0/rh_schema_diagram/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    38841 2022-03-21 11:50:03.000000 robotathome-1.1.0/rh_schema_diagram/rh_schema_brief.pdf
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    40694 2022-03-21 11:50:03.000000 robotathome-1.1.0/rh_schema_diagram/rh_schema_full.pdf
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 11:25:36.975787 robotathome-1.1.0/robotathome/
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)      473 2023-04-09 10:57:14.000000 robotathome-1.1.0/robotathome/__init__.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      754 2022-03-21 11:50:03.000000 robotathome-1.1.0/robotathome/_version.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 11:25:36.975787 robotathome-1.1.0/robotathome/core/
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)      178 2023-04-09 10:57:14.000000 robotathome-1.1.0/robotathome/core/__init__.py
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)     4765 2023-04-09 10:57:14.000000 robotathome-1.1.0/robotathome/core/df.py
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)    46199 2023-04-09 10:57:14.000000 robotathome-1.1.0/robotathome/core/reader.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 11:25:36.975787 robotathome-1.1.0/robotathome/cv/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      194 2022-03-21 11:50:03.000000 robotathome-1.1.0/robotathome/cv/__init__.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      302 2022-03-21 11:50:03.000000 robotathome-1.1.0/robotathome/cv/_greetings.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    20144 2022-03-21 11:50:03.000000 robotathome-1.1.0/robotathome/cv/gluoncv.py
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)    16622 2023-04-09 10:57:14.000000 robotathome-1.1.0/robotathome/cv/opencv.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     6705 2022-03-21 11:50:03.000000 robotathome-1.1.0/robotathome/helpers.py
+-rw-r--r--   0 lightman  (1000) lightman  (1000)     1464 2022-03-21 11:50:03.000000 robotathome-1.1.0/robotathome/log.py
+drwxrwxr-x   0 lightman  (1000) lightman  (1000)        0 2023-04-09 11:25:36.975787 robotathome-1.1.0/robotathome.egg-info/
+-rw-r--r--   0 lightman  (1000) lightman  (1000)    12821 2023-04-09 11:25:36.000000 robotathome-1.1.0/robotathome.egg-info/PKG-INFO
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      915 2023-04-09 11:25:36.000000 robotathome-1.1.0/robotathome.egg-info/SOURCES.txt
+-rw-r--r--   0 lightman  (1000) lightman  (1000)        1 2023-04-09 11:25:36.000000 robotathome-1.1.0/robotathome.egg-info/dependency_links.txt
+-rw-r--r--   0 lightman  (1000) lightman  (1000)      226 2023-04-09 11:25:36.000000 robotathome-1.1.0/robotathome.egg-info/requires.txt
+-rw-r--r--   0 lightman  (1000) lightman  (1000)       12 2023-04-09 11:25:36.000000 robotathome-1.1.0/robotathome.egg-info/top_level.txt
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)       38 2023-04-09 11:25:36.975787 robotathome-1.1.0/setup.cfg
+-rw-rw-r--   0 lightman  (1000) lightman  (1000)     3306 2023-04-09 11:24:37.000000 robotathome-1.1.0/setup.py
```

### Comparing `robotathome-1.0.6/LICENSE` & `robotathome-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotathome-1.0.6/PKG-INFO` & `robotathome-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: robotathome
-Version: 1.0.6
-Summary: This package provides a Python Toolbox with a set of functions to assist in the management of Robot@Home 2 Dataset
-Home-page: https://github.com/goyoambrosio/RobotAtHome_API
+Version: 1.1.0
+Summary: This package provides a Python Toolbox with a set of functions to assist in the management of Robot@Home2 Dataset
+Home-page: https://github.com/goyoambrosio/RobotAtHome2
 Author: G. Ambrosio-Cestero
 Author-email: gambrosio@uma.es
 License: MIT
-Keywords: semantic mapping object categorization object recognition room categorization room recognition contextual information mobile robots domestic robots home environment robotic dataset benchmark
+Keywords: toolbox dataset database relational model mobile robotics computer vision
 Platform: Windows
 Platform: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: full
 Provides-Extra: interactive
 Provides-Extra: cv
 License-File: LICENSE
 
 # Robot@Home2 Dataset Toolbox #
 
-[![PyPI](https://img.shields.io/pypi/v/robotathome)](https://pypi.org/project/robotathome/)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4530453.svg)](https://doi.org/10.5281/zenodo.4530453)
+[![PyPI](https://img.shields.io/pypi/v/robotathome)](https://pypi.org/project/robotathome/ "R@H2 as PyPI package ready to install")
+[![DOI](https://zenodo.org/badge/245370645.svg)](https://zenodo.org/badge/latestdoi/245370645 "This repository released on Zenodo")
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4530453.svg)](https://doi.org/10.5281/zenodo.4530453 "The downloadable R@H2 dataset in Zenodo")
+[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/drive/folders/1ENnxbKP5MJdlGl2Q93WTbIlofuy6Icxq)
 
 The Robot-at-Home dataset (Robot@Home, paper
 [here](http://mapir.uma.es/papersrepo/2017/2017-raul-IJRR-Robot_at_home_dataset.pdf))
 is a collection of raw and processed data from five domestic settings compiled
 by a mobile robot equipped with 4 RGB-D cameras and a 2D laser scanner. Its main
 purpose is to serve as a testbed for semantic mapping algorithms through the
 categorization of objects and/or rooms.
@@ -324,9 +326,7 @@
     rh.uncompress('~/Downloads/Robot@Home2_files.tgz', '~/WORKSPACE/files')
 else:
     print('Integrity of Robot@Home2_files.tgz is compromised, please download again')
 ```
 
 
 
-
-
```

### Comparing `robotathome-1.0.6/README.md` & `robotathome-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Robot@Home2 Dataset Toolbox #
 
-[![PyPI](https://img.shields.io/pypi/v/robotathome)](https://pypi.org/project/robotathome/)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4530453.svg)](https://doi.org/10.5281/zenodo.4530453)
+[![PyPI](https://img.shields.io/pypi/v/robotathome)](https://pypi.org/project/robotathome/ "R@H2 as PyPI package ready to install")
+[![DOI](https://zenodo.org/badge/245370645.svg)](https://zenodo.org/badge/latestdoi/245370645 "This repository released on Zenodo")
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4530453.svg)](https://doi.org/10.5281/zenodo.4530453 "The downloadable R@H2 dataset in Zenodo")
+[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/drive/folders/1ENnxbKP5MJdlGl2Q93WTbIlofuy6Icxq)
 
 The Robot-at-Home dataset (Robot@Home, paper
 [here](http://mapir.uma.es/papersrepo/2017/2017-raul-IJRR-Robot_at_home_dataset.pdf))
 is a collection of raw and processed data from five domestic settings compiled
 by a mobile robot equipped with 4 RGB-D cameras and a 2D laser scanner. Its main
 purpose is to serve as a testbed for semantic mapping algorithms through the
 categorization of objects and/or rooms.
```

### Comparing `robotathome-1.0.6/notebooks/05-Google-colab-drive.ipynb` & `robotathome-1.1.0/notebooks/05-Google-colab-drive.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.0.6/notebooks/10-Download-and-install.ipynb` & `robotathome-1.1.0/notebooks/10-Download-and-install.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.0.6/notebooks/20-Before-starting-the-logging-system.ipynb` & `robotathome-1.1.0/notebooks/20-Before-starting-the-logging-system.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.0.6/notebooks/30-Getting-started-Framework-data.ipynb` & `robotathome-1.1.0/notebooks/30-Getting-started-Framework-data.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.0.6/notebooks/40-Captured-data.ipynb` & `robotathome-1.1.0/notebooks/40-Captured-data.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.0.6/notebooks/50-RGBD-observations.ipynb` & `robotathome-1.1.0/notebooks/50-RGBD-observations.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.0.6/notebooks/60-Lsrscan-observations.ipynb` & `robotathome-1.1.0/notebooks/60-Lsrscan-observations.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.0.6/notebooks/70-Scenes.ipynb` & `robotathome-1.1.0/notebooks/70-Scenes.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.0.6/notebooks/80-Characterized-observations.ipynb` & `robotathome-1.1.0/notebooks/80-Characterized-observations.ipynb`

 * *Files identical despite different names*

### Comparing `robotathome-1.0.6/rh_schema_diagram/rh_schema_brief.pdf` & `robotathome-1.1.0/rh_schema_diagram/rh_schema_brief.pdf`

 * *Files identical despite different names*

### Comparing `robotathome-1.0.6/rh_schema_diagram/rh_schema_full.pdf` & `robotathome-1.1.0/rh_schema_diagram/rh_schema_full.pdf`

 * *Files identical despite different names*

### Comparing `robotathome-1.0.6/robotathome/_version.py` & `robotathome-1.1.0/robotathome/_version.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.0.6/robotathome/core/reader.py` & `robotathome-1.1.0/robotathome/core/reader.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,31 @@
 __contact__ = "gambrosio[at]uma.es"
 __copyright__ = "Copyright 2021, Gregorio Ambrosio"
 __date__ = "2021/07/27"
 __license__ = "MIT"
 
 import sqlite3
 import os
+import configparser
 import numpy as np
 import pandas as pd
+
 from robotathome.log import logger
 
 __all__ = ['RobotAtHome']
 
+
 # @logger.catch
 class RobotAtHome():
-    """RobotAtHome class with methods for Robot@Home2 dataset
+    """RobotAtHome class with methods for Robot@Home2 dataset.
 
     The RobotAtHome class encapsulates methods to access the RobotAtHome
     database. <https://doi.org/10.5281/zenodo.4530453>
 
-    Attributes:
+    Main attributes:
         rh_path (str, optional):
             root path for robotathome database, usually rh.db
         wspc_path (str, optional):
             workspace path where temporary files are stored
         db_filename (str, optional):
             default database name
         rgbd_path (str, optional):
@@ -36,146 +39,199 @@
     """
 
     def __init__(self,
                  rh_path='.',
                  rgbd_path='./files/rgbd',
                  scene_path='./files/scene',
                  wspc_path='.',
-                 db_filename='rh.db'
+                 db_filename='rh.db',
+                 config_filename='.rh'
                  ):
-        """ RobotAtHome constructor method """
-        self.__rh_path = os.path.expanduser(rh_path)
-        self.__rgbd_path = os.path.expanduser(rgbd_path)
-        self.__scene_path = os.path.expanduser(scene_path)
-        self.__wspc_path = os.path.expanduser(wspc_path)
-        self.__db_filename = db_filename
+        """Initialize instance variables.
+
+        There are two ways to get initial values for main attributes:
+        with arguments values or by reading a configuration file. This function
+        first tries to read a file called .rh . If the file does not exist,
+        the attributes get values from the arguments. Additionally, arguments
+        can be provided or default values can be obtained.
+
+        Attributes:
+            rh_path: path where the database resides.
+            rgbd_path: path where rgbd files are located.
+            scene_path: path where scene files are located.
+            wspc_path: workspace path where the toolbox stores results or
+                intermediate data.
+            db_filename: file name of the database.
+
+        Raises:
+            Exception: If the object cannot be instantiated (usually because
+                a database connection could not be done).
+
+        Note 1: The default folder structure is:
+            R@H2-2.0.1
+                 │    └── files
+                 │        ├── rgbd
+                 │        └── scene
+                 └─────── rh.db
+
+        Note 2: Example of .rh file
+            # This is a default configuration file
+            [PATHS]
+            rh_path     = $HOME/R@H2-2.0.1
+            rgbd_path   = ~/R@H2-2.0.1/files/rgbd
+            scene_path  = ~/R@H2-2.0.1/files/scene
+            wspc_path   = ~/R@H2-2.0.1
+            db_filename = rh.db
+
+            Paths strings can content environmental variables such as $HOME or
+            a tilde prefix.
+        """
         self.__con = None
         self.__aliases = {}
 
+        # configparser related code
+        config = configparser.ConfigParser()
+        config.read(os.path.expanduser(os.path.expandvars(config_filename)))
+        self.__rh_path = os.path.expanduser(os.path.expandvars(config.get(
+            'PATHS',
+            'rh_path',
+            fallback=rh_path)))
+        self.__rgbd_path = os.path.expanduser(os.path.expandvars(config.get(
+            'PATHS',
+            'rgbd_path',
+            fallback=rgbd_path)))
+        self.__scene_path = os.path.expanduser(os.path.expandvars(config.get(
+            'PATHS',
+            'scene_path',
+            fallback=scene_path)))
+        self.__wspc_path = os.path.expanduser(os.path.expandvars(config.get(
+            'PATHS',
+            'wspc_path',
+            fallback=wspc_path)))
+        self.__db_filename = os.path.expanduser(os.path.expandvars(config.get(
+            'PATHS',
+            'db_filename',
+            fallback=db_filename)))
+
         logger.debug('rh_path     : {}', self.__rh_path)
         logger.debug('rgbd_path   : {}', self.__rgbd_path)
         logger.debug('scene_path  : {}', self.__scene_path)
         logger.debug('wspc_path   : {}', self.__wspc_path)
         logger.debug('db_filename : {}', self.__db_filename)
 
         # Initialization functions
         try:
             self.__open_dataset()
-        except Exception as e:
+        except Exception as generic_error:
             logger.error("object cannot be instantiated")
             # return None
-            raise e
+            raise generic_error
 
     def __del__(self):
-        """ Robot@Home destructor method"""
+        """Delete instance variables."""
 
     def __open_dataset(self):
-
-        """
-        This function makes the connection with the database and calls the
-        initialization functions, e.g. create temporal views
-        """
-
+        """Make the connection with the database."""
         db_full_path = os.path.join(self.__rh_path, self.__db_filename)
         logger.debug("db_full_path: {}", db_full_path)
 
         try:
             db_full_filename = 'file:'+db_full_path+'?mode=rw'
             logger.debug("db_full_filename: {}", db_full_filename)
             self.__con = sqlite3.connect(db_full_filename, uri=True)
             logger.success("Connection is established: {}", self.__db_filename)
-        except sqlite3.Error as e:
-            logger.error("Error while trying to open database: {}", e.args[0])
+        except sqlite3.Error as sqlite_error:
+            logger.error("Error while trying to open database: {}",
+                         sqlite_error.args[0])
             # sys.exit() , quit() , exit() ,raise SystemExit
             # os._exit(1)
             raise
 
     def __close_dataset(self):
-        """
-        This function closes the connection with the database
-        """
+        """Close the connection with the database."""
         self.__con.close()
-        logger.info("The connection with the database has been successfully closed")
+        logger.info("The connection with the database has been successfully \
+                     closed")
 
     def __get_temp_sql_object_names(self):
-        ''' Return a list with temporary/internal created views'''
+        """Return a list with temporary/internal created views."""
         return self.select_column('tbl_name', 'sqlite_temp_master')
 
     def get_con(self):
-        """
-        This function returns the sql connection variable
-        """
+        """Return the sql connection variable."""
         return self.__con
 
+    def get_path_vars(self):
+        """Return path variables.
 
+        Returns:
+            array: [rh_path, rgbd_path, scene_path, wspc_path, db_filename]
+        """
+        return [self.__rh_path,
+                self.__rgbd_path,
+                self.__scene_path,
+                self.__wspc_path,
+                self.__db_filename]
     """
     Framework
     """
     def get_homes(self):
-        """
-        Return a dataframe with home names
-        """
-        sql_str = ('select * from rh_homes;')
+        """Return a dataframe with home names."""
+        sql_str = 'select * from rh_homes;'
         return self.query(sql_str)
 
     def get_home_sessions(self):
-        """
-        Return a dataframe with home session names
-        """
-        sql_str = ('select * from rh_home_sessions;')
+        """Return a dataframe with home session names."""
+        sql_str = 'select * from rh_home_sessions;'
         return self.query(sql_str)
+
     def get_rooms(self):
-        """
-        Return a dataframe with room names
-        """
-        sql_str = ('select * from rh_rooms;')
+        """Return a dataframe with room names."""
+        sql_str = 'select * from rh_rooms;'
         return self.query(sql_str)
+
     def get_room_types(self):
-        """
-        Return a dataframe with room type names
-        """
-        sql_str = ('select * from rh_room_types;')
+        """Return a dataframe with room type names."""
+        sql_str = 'select * from rh_room_types;'
         return self.query(sql_str)
+
     def get_sensors(self):
-        """
-        Return a dataframe with sensor names
-        """
-        sql_str = ('select * from rh_sensors;')
+        """Return a dataframe with sensor names."""
+        sql_str = 'select * from rh_sensors;'
         return self.query(sql_str)
+
     def get_sensor_types(self):
-        """
-        Return a dataframe with sensor type names
-        """
-        sql_str = ('select * from rh_sensor_types;')
+        """Return a dataframe with sensor type names."""
+        sql_str = 'select * from rh_sensor_types;'
         return self.query(sql_str)
+
     def get_hometopo(self):
-        """
-        Return a dataframe with home topo relationships
-        """
+        """Return a dataframe with home topo relationships."""
         sql_str = ('''
         select
             rh_homes.id as home_id,
             rh_homes.name as home_name,
-	        rh_rooms1.id as room1_id,
-	        rh_rooms1.name as room1_name,
-	        rh_rooms2.id as room2_id,
-	        rh_rooms2.name as room2_name
+            rh_rooms1.id as room1_id,
+            rh_rooms1.name as room1_name,
+            rh_rooms2.id as room2_id,
+            rh_rooms2.name as room2_name
         from rh_hometopo
         inner join rh_homes on rh_hometopo.home_id = rh_homes.id
         inner join rh_rooms as rh_rooms1 on rh_rooms1.id = rh_hometopo.room1_id
         inner join rh_rooms as rh_rooms2 on rh_rooms2.id = rh_hometopo.room2_id
         '''
-        )
+                   )
         return self.query(sql_str)
 
     def get_locators(self):
-        """ Return a dataframe with main indexes values (id and name),
-        i.e., home_session, home, room and home_subsession
         """
+        Return a dataframe with main indexes values (id and name).
 
+        i.e., home_session, home, room and home_subsession
+        """
         sql_str = """
         select
             home_session_id, rh_home_sessions.name as home_session_name,
             rh_raw.home_id, rh_homes.name as home_name,
             rh_raw.room_id, rh_rooms.name as room_name,
             rh_raw.home_subsession_id
         from rh_raw
@@ -192,43 +248,86 @@
             rh_raw.home_session_id
         """
 
         df_rows = pd.read_sql_query(sql_str, self.__con)
 
         return df_rows
 
-
-
     """
     Captured data
     """
     def get_sensor_observations(self, arg='full'):
-        """ Docstring """
+        """Return RGB-D and Laser observations as a pandas dataframe.
+
+        The data provided by R@H2 have been collected within rooms of five
+        dwellings (homes) Raw data were collected in different sessions and
+        sub-sessions, each one containing a number of sequences of RGB-D
+        observations and laser scans. These sequences were gathered by
+        teleoperating the robot to fully inspect each individual room.
+
+        Sensor data comprises ~75 minutes of recorded data collected in
+        different sessions.
+
+        These data include:
+
+        RGB-D observations from the four RGB-D cameras, including intensity
+        images, depth images, and 3D point clouds.
+
+        Laser scanner data: 2D observations from the laser scanner captured in
+        the inspected rooms.
+
+        The R@H2 dataset contains those RGBD and Laser observations
+
+        Args:
+            arg:
+                Can get five values:
+                "full": indicates that the full set of observations will be
+                    returned. This is the default value.
+                "discarded": discarded observations are those that have not
+                    been labeled (annotated).
+                "lblrgbd": only labeled (annotated) RGB-D observations will
+                    be returned.
+                "lsrscan": laser scans will be returned.
+                "rgbdlsr": both labeled RGB-D and laser scans will be returned.
+        Returns:
+            df: a Pandas dataframe with selected observations ordered by
+                timestamp.
+        """
 
         def get_full_data():
-            """ Docstring """
+            """Return a dataframe containing the full set of observations.
+
+            Returns:
+                df: a Pandas dataframe with the data resulting from the
+                    execution of the query according the SQL string.
+            """
             sql_str = (
-                f'''
+                '''
                 select
                     id, time_stamp as timestamp,
                     home_session_id, home_subsession_id, home_id, room_id,
                     sensor_id, name as sensor_name,
                     sensor_pose_x, sensor_pose_y, sensor_pose_z,
                     sensor_pose_yaw, sensor_pose_pitch, sensor_pose_roll
                 from rh2_sensor_observations
                 order by time_stamp
                 '''
             )
             logger.debug(sql_str)
             return self.query(sql_str)
 
         def get_discarded_data():
-            """ Docstring """
+            """Return a dataframe containing the not processed observs.
+
+            Returns:
+                df: a Pandas dataframe with the data resulting from the
+                    execution of the query according the SQL string.
+            """
             sql_str = (
-                f'''
+                '''
                 select
                     id, time_stamp as timestamp,
                     home_session_id, home_subsession_id, home_id, room_id,
                     sensor_id, name as sensor_name,
                     sensor_pose_x, sensor_pose_y, sensor_pose_z,
                     sensor_pose_yaw, sensor_pose_pitch, sensor_pose_roll
                 from rh2_sensor_observations
@@ -236,35 +335,45 @@
                 order by time_stamp
                 '''
             )
             logger.debug(sql_str)
             return self.query(sql_str)
 
         def get_lblrgbd_data():
-            """ Docstring """
+            """Return a dataframe containing labeled RGB-D observations.
+
+            Returns:
+                df: a Pandas dataframe with the data resulting from the
+                    execution of the query according the SQL string.
+            """
             sql_str = (
-                f'''
+                '''
                 select
                     id, time_stamp as timestamp,
                     home_session_id, home_subsession_id, home_id, room_id,
                     sensor_id, name as sensor_name,
                     sensor_pose_x, sensor_pose_y, sensor_pose_z,
                     sensor_pose_yaw, sensor_pose_pitch, sensor_pose_roll
                 from rh2_sensor_observations
-                where id >= 100000 and id < 200000 
+                where id >= 100000 and id < 200000
                 order by time_stamp
                 '''
             )
             logger.debug(sql_str)
             return self.query(sql_str)
 
         def get_lsrscan_data():
-            """ Docstring """
+            """Return a dataframe containing laser scans observations.
+
+            Returns:
+                df: a Pandas dataframe with the data resulting from the
+                    execution of the query according the SQL string.
+            """
             sql_str = (
-                f'''
+                '''
                 select
                     id, time_stamp as timestamp,
                     home_session_id, home_subsession_id, home_id, room_id,
                     sensor_id, name as sensor_name,
                     sensor_pose_x, sensor_pose_y, sensor_pose_z,
                     sensor_pose_yaw, sensor_pose_pitch, sensor_pose_roll
                 from rh2_sensor_observations
@@ -272,320 +381,501 @@
                 order by time_stamp
                 '''
             )
             logger.debug(sql_str)
             return self.query(sql_str)
 
         def get_rgbd_lsr_data():
-            """ Docstring """
+            """Return a dataframe containing labeled RGB-D and laser scans.
+
+            Returns:
+                df: a Pandas dataframe with the data resulting from the
+                    execution of the query according the SQL string.
+            """
             sql_str = (
-                f'''
+                '''
                 select
                     id, time_stamp as timestamp,
                     home_session_id, home_subsession_id, home_id, room_id,
                     sensor_id, name as sensor_name,
                     sensor_pose_x, sensor_pose_y, sensor_pose_z,
                     sensor_pose_yaw, sensor_pose_pitch, sensor_pose_roll
                 from rh2_sensor_observations
                 where id >= 100000 and id < 300000
                 order by time_stamp
                 '''
             )
             logger.debug(sql_str)
             return self.query(sql_str)
 
-
         switcher = {
-            "full"      : get_full_data,
-            "discarded" : get_discarded_data,
-            "lblrgbd"   : get_lblrgbd_data,
-            "lsrscan"   : get_lsrscan_data,
-            "rgbdlsr"   : get_rgbd_lsr_data,
+            "full":      get_full_data,
+            "discarded": get_discarded_data,
+            "lblrgbd":   get_lblrgbd_data,
+            "lsrscan":   get_lsrscan_data,
+            "rgbdlsr":   get_rgbd_lsr_data,
         }
         func = switcher.get(arg, lambda: "Invalid argument")
 
         df = func()
 
         return df
 
     def id2name(self, id, arg='r'):
-        """Doc string"""
+        """Return the name corresponding to an id.
+
+        The R@H2 database contains observations gathered from sensors of a
+        mobile robot. Furthermore, it contains data about the framework where
+        the data were gathered. That framework data is composed of some tables:
+
+        - rh_homes
+        - rh_home_sessions
+        - rh_rooms
+        - rh_sensors
+        - rh_room_types
+        - rh_sensor_types
+        - rh_objects
+        - rh_object_types
+
+        All those tables have registries that associates ids (integer numbers)
+        with names (descriptor strings).
+
+        This functions takes an argument depicting the framework table to be
+        searched and returns the name for the provided id.
+
+        Args:
+            id: the id number to be searched ('r' is the default value)
+            arg: a string indicating the framework table to be searched:
+            "h"            : rh_homes
+            "hs"           : rh_home_sessions
+            "r"            : rh_rooms
+            "rt"           : rh_room_types
+            "s"            : rh_sensors
+            "st"           : rh_sensor_types
+            "o"            : rh_objects
+            "ot"           : rh_object_types
+            "home"         : rh_homes
+            "home_session" : rh_home_sessions
+            "room"         : rh_rooms
+            "room_type"    : rh_room_types
+            "sensor"       : rh_sensors
+            "sensor_type"  : rh_sensor_types
+            "object"       : rh_objects
+            "object_type"  : rh_object_types
+
+        Returns:
+            name: a string name associated with the id.
+        """
 
         def get_home_name():
-            """ Docstring """
+            """Return a dataframe containing the name corresponding to the id.
+
+            Returns:
+                df: a Pandas dataframe with the data resulting from the
+                    execution of the query according the SQL string.
+            """
             sql_str = (
                 f'''
                 select name
                 from rh_homes
                 where id = {id}
                 '''
             )
             logger.debug(sql_str)
             return self.query(sql_str)
 
         def get_home_session_name():
-            """ Docstring """
+            """Return a dataframe containing the name corresponding to the id.
+
+            Returns:
+                df: a Pandas dataframe with the data resulting from the
+                    execution of the query according the SQL string.
+            """
             sql_str = (
                 f'''
                 select name
                 from rh_home_sessions
                 where id = {id}
                 '''
             )
             logger.debug(sql_str)
             return self.query(sql_str)
 
         def get_room_name():
-            """ Docstring """
+            """Return a dataframe containing the name corresponding to the id.
+
+            Returns:
+                df: a Pandas dataframe with the data resulting from the
+                    execution of the query according the SQL string.
+            """
             sql_str = (
                 f'''
                 select name
                 from rh_rooms
                 where id = {id}
                 '''
             )
             logger.debug(sql_str)
             return self.query(sql_str)
 
         def get_sensor_name():
-            """ Docstring """
+            """Return a dataframe containing the name corresponding to the id.
+
+            Returns:
+                df: a Pandas dataframe with the data resulting from the
+                    execution of the query according the SQL string.
+            """
             sql_str = (
                 f'''
                 select name
                 from rh_sensors
                 where id = {id}
                 '''
             )
             logger.debug(sql_str)
             return self.query(sql_str)
 
         def get_room_type_name():
-            """ Docstring """
+            """Return a dataframe containing the name corresponding to the id.
+
+            Returns:
+                df: a Pandas dataframe with the data resulting from the
+                    execution of the query according the SQL string.
+            """
             sql_str = (
                 f'''
                 select name
                 from rh_room_types
                 where id = {id}
                 '''
             )
             logger.debug(sql_str)
             return self.query(sql_str)
 
         def get_sensor_type_name():
-            """ Docstring """
+            """Return a dataframe containing the name corresponding to the id.
+
+            Returns:
+                df: a Pandas dataframe with the data resulting from the
+                    execution of the query according the SQL string.
+            """
             sql_str = (
                 f'''
                 select name
                 from rh_sensor_types
                 where id = {id}
                 '''
             )
             logger.debug(sql_str)
             return self.query(sql_str)
 
         def get_object_name():
-            """ Docstring """
+            """Return a dataframe containing the name corresponding to the id.
+
+            Returns:
+                df: a Pandas dataframe with the data resulting from the
+                    execution of the query according the SQL string.
+            """
             sql_str = (
                 f'''
                 select name
                 from rh_objects
                 where id = {id}
                 '''
             )
             logger.debug(sql_str)
             return self.query(sql_str)
 
         def get_object_type_name():
-            """ Docstring """
+            """Return a dataframe containing the name corresponding to the id.
+
+            Returns:
+                df: a Pandas dataframe with the data resulting from the
+                    execution of the query according the SQL string.
+            """
             sql_str = (
                 f'''
                 select name
                 from rh_object_types
                 where id = {id}
                 '''
             )
             logger.debug(sql_str)
             return self.query(sql_str)
 
-
         switcher = {
-            "h"            : get_home_name,
-            "hs"           : get_home_session_name,
-            "r"            : get_room_name,
-            "rt"           : get_room_type_name,
-            "s"            : get_sensor_name,
-            "st"           : get_sensor_type_name,
-            "o"            : get_object_name,
-            "ot"           : get_object_type_name,
-            "home"         : get_home_name,
-            "home_session" : get_home_session_name,
-            "room"         : get_room_name,
-            "room_type"    : get_room_type_name,
-            "sensor"       : get_sensor_name,
-            "sensor_type"  : get_sensor_type_name,
-            "object"       : get_object_name,
-            "object_type"  : get_object_type_name,
-
+            "h":            get_home_name,
+            "hs":           get_home_session_name,
+            "r":            get_room_name,
+            "rt":           get_room_type_name,
+            "s":            get_sensor_name,
+            "st":           get_sensor_type_name,
+            "o":            get_object_name,
+            "ot":           get_object_type_name,
+            "home":         get_home_name,
+            "home_session": get_home_session_name,
+            "room":         get_room_name,
+            "room_type":    get_room_type_name,
+            "sensor":       get_sensor_name,
+            "sensor_type":  get_sensor_type_name,
+            "object":       get_object_name,
+            "object_type":  get_object_type_name,
         }
         func = switcher.get(arg, lambda: "Invalid argument")
 
-        return func().iat[0,0]
+        return func().iat[0, 0]
 
     def name2id(self, name, arg='r'):
-        """Doc string"""
+        """Return the id corresponding to a name.
+
+        The R@H2 database contains observations gathered from sensors of a
+        mobile robot. Furthermore, it contains data about the framework where
+        the data were gathered. That framework data is composed of some tables:
+
+        - rh_homes
+        - rh_home_sessions
+        - rh_rooms
+        - rh_sensors
+        - rh_room_types
+        - rh_sensor_types
+        - rh_objects
+        - rh_object_types
+
+        All those tables have registries that associates ids (integer numbers)
+        with names (descriptor strings).
+
+        This functions takes an argument depicting the framework table to be
+        searched and returns the name for the provided id.
+
+        Args:
+            id: the id number to be searched ('r' is the default value)
+            arg: a string indicating the framework table to be searched:
+            "h"            : rh_homes
+            "hs"           : rh_home_sessions
+            "r"            : rh_rooms
+            "rt"           : rh_room_types
+            "s"            : rh_sensors
+            "st"           : rh_sensor_types
+            "o"            : rh_objects
+            "ot"           : rh_object_types
+            "home"         : rh_homes
+            "home_session" : rh_home_sessions
+            "room"         : rh_rooms
+            "room_type"    : rh_room_types
+            "sensor"       : rh_sensors
+            "sensor_type"  : rh_sensor_types
+            "object"       : rh_objects
+            "object_type"  : rh_object_types
+
+        Returns:
+            id: an identification number associated with the name.
+        """
 
         def get_home_id():
-            """ Docstring """
+            """Return a dataframe containing the id corresponding to the name.
+
+            Returns:
+                df: a Pandas dataframe with the data resulting from the
+                    execution of the query according the SQL string.
+            """
             sql_str = (
                 f'''
                 select id
                 from rh_homes
                 where name like '%{name}%'
                 '''
             )
             logger.debug(sql_str)
             return self.query(sql_str)
 
         def get_home_session_id():
-            """ Docstring """
+            """Return a dataframe containing the id corresponding to the name.
+
+            Returns:
+                df: a Pandas dataframe with the data resulting from the
+                    execution of the query according the SQL string.
+            """
             sql_str = (
                 f'''
                 select id
                 from rh_home_sessions
                 where name like '%{name}%'
                 '''
             )
             logger.debug(sql_str)
             return self.query(sql_str)
 
         def get_room_id():
-            """ Docstring """
+            """Return a dataframe containing the id corresponding to the name.
+
+            Returns:
+                df: a Pandas dataframe with the data resulting from the
+                    execution of the query according the SQL string.
+            """
             sql_str = (
                 f'''
                 select id
                 from rh_rooms
                 where name like '%{name}%'
                 '''
             )
             logger.debug(sql_str)
             return self.query(sql_str)
 
         def get_sensor_id():
-            """ Docstring """
+            """Return a dataframe containing the id corresponding to the name.
+
+            Returns:
+                df: a Pandas dataframe with the data resulting from the
+                    execution of the query according the SQL string.
+            """
             sql_str = (
                 f'''
                 select id
                 from rh_sensors
                 where name like '%{name}%'
                 '''
             )
             logger.debug(sql_str)
             return self.query(sql_str)
 
         def get_room_type_id():
-            """ Docstring """
+            """Return a dataframe containing the id corresponding to the name.
+
+            Returns:
+                df: a Pandas dataframe with the data resulting from the
+                    execution of the query according the SQL string.
+            """
             sql_str = (
                 f'''
                 select id
                 from rh_room_types
                 where name like '%{name}%'
                 '''
             )
             logger.debug(sql_str)
             return self.query(sql_str)
 
         def get_sensor_type_id():
-            """ Docstring """
+            """Return a dataframe containing the id corresponding to the name.
+
+            Returns:
+                df: a Pandas dataframe with the data resulting from the
+                    execution of the query according the SQL string.
+            """
             sql_str = (
                 f'''
                 select id
                 from rh_sensor_types
                 where name like '%{name}%'
                 '''
             )
             logger.debug(sql_str)
             return self.query(sql_str)
 
         def get_object_id():
-            """ Docstring """
+            """Return a dataframe containing the id corresponding to the name.
+
+            Returns:
+                df: a Pandas dataframe with the data resulting from the
+                    execution of the query according the SQL string.
+            """
             sql_str = (
                 f'''
                 select id
                 from rh_objects
                 where name like '%{name}%'
                 '''
             )
             logger.debug(sql_str)
             return self.query(sql_str)
 
         def get_object_type_id():
-            """ Docstring """
+            """Return a dataframe containing the id corresponding to the name.
+
+            Returns:
+                df: a Pandas dataframe with the data resulting from the
+                    execution of the query according the SQL string.
+            """
             sql_str = (
                 f'''
                 select id
                 from rh_object_types
                 where name like '%{name}%'
                 '''
             )
             logger.debug(sql_str)
             return self.query(sql_str)
 
-
         switcher = {
-            "h"            : get_home_id,
-            "hs"           : get_home_session_id,
-            "r"            : get_room_id,
-            "rt"           : get_room_type_id,
-            "s"            : get_sensor_id,
-            "st"           : get_sensor_type_id,
-            "o"            : get_object_id,
-            "ot"           : get_object_type_id,
-            "home"         : get_home_id,
-            "home_session" : get_home_session_id,
-            "room"         : get_room_id,
-            "room_type"    : get_room_type_id,
-            "sensor"       : get_sensor_id,
-            "sensor_type"  : get_sensor_type_id,
-            "object"       : get_object_id,
-            "object_type"  : get_object_type_id,
+            "h": get_home_id,
+            "hs": get_home_session_id,
+            "r": get_room_id,
+            "rt": get_room_type_id,
+            "s": get_sensor_id,
+            "st": get_sensor_type_id,
+            "o": get_object_id,
+            "ot": get_object_type_id,
+            "home": get_home_id,
+            "home_session": get_home_session_id,
+            "room": get_room_id,
+            "room_type": get_room_type_id,
+            "sensor": get_sensor_id,
+            "sensor_type": get_sensor_type_id,
+            "object": get_object_id,
+            "object_type": get_object_type_id,
 
         }
         func = switcher.get(arg, lambda: "Invalid argument")
 
-        return func().iat[0,0]
-
+        return func().iat[0, 0]
 
     """
     RGBD data
     """
     def get_RGBD_files(self, id):
-        """ Docstring """
+        """
+        Return the full path of RGB and D files for an observation.
+
+        Args:
+            id: the observation identification number to search for.
+
+        Returns:
+            An array with two strings:
+                rgb_file: a string containing the full path of the RGB image
+                    file corresponding to the observation.
+                depth_file: a string containing the full path of the D(epth)
+                    image file corresponding to the observation.
+        """
         sql_str = (
             f'''
             select
               new_path as local_path,
               new_file_2 as rgb_file,
               new_file_1 as depth_file
             from rh2_old2new_rgbd_files
             where id = {id}
             '''
         )
         logger.debug(sql_str)
         # self.query(sql_str).values.flatten().tolist()
         # self.query(sql_str).loc[0,:].tolist()
         logger.debug('rh_rgbd_path: {}', self.__rgbd_path)
-        files_path = self.query(sql_str).loc[0,:].tolist()
-        depth_file = os.path.join(self.__rgbd_path, files_path[0], files_path[2])
-        rgb_file = os.path.join(self.__rgbd_path, files_path[0], files_path[1])
+        files_path = self.query(sql_str).loc[0, :].tolist()
+        depth_file = os.path.join(self.__rgbd_path,
+                                  files_path[0],
+                                  files_path[2])
+        rgb_file = os.path.join(self.__rgbd_path,
+                                files_path[0],
+                                files_path[1])
         return [rgb_file, depth_file]
 
     def __get_RGBD_labels(self, id):
         """
-        This function return a dataframe with labels for the observations
-        referenced by id
+        Return a dataframe with labels for the observation referenced by id.
 
         SQL query
 
         select * from rh_lblrgbd_labels
             where sensor_observation_id = id
 
         Parameters
@@ -595,58 +885,60 @@
             rh_lbl_rgbd_labels.
 
         Returns
         -------
         A dataframe with the query result. An empty dataframe is returned when
         no rows are available, i.e., when the sensor observation does not
         belong to rh_lblrgbd (labelled rgbd)
+
+        Note
+        ----
+        This is a local function
         """
         sql_str = (
             f'''
             select *
             from rh_lblrgbd_labels
              where sensor_observation_id = {id}
             '''
         )
         logger.debug(sql_str)
         return self.query(sql_str)
 
     def __get_Labels_file(self, id):
-        """
-        Returns the <id>_labels.txt full path filename
-        """
+        """Return the <id>_labels.txt full path filename."""
         sql_str = (
             f'''
             select
               new_path as local_path,
               new_file_3 as labels_file
             from rh2_old2new_rgbd_files
             where id = {id}
             '''
         )
         logger.debug(sql_str)
-        files_path = self.query(sql_str).loc[0,:].tolist()
-        labels_file = os.path.join(self.__rgbd_path, files_path[0], files_path[1])
+        files_path = self.query(sql_str).loc[0, :].tolist()
+        labels_file = os.path.join(self.__rgbd_path,
+                                   files_path[0],
+                                   files_path[1])
         return labels_file
 
     def __get_label_mask_array(self, l_f):
-        """
-        Returns a numpy array from the <id>_labels.txt
-        """
+        """Return a numpy array from the <id>_labels.txt."""
         mask = []
         with open(l_f, "r") as file_handler:
             line = file_handler.readline()
             while line:
                 words = line.strip().split()
                 if words[0][0] != '#':
                     num_of_labels = int(words[0])
                     break
                 line = file_handler.readline()
 
-            for i in range(num_of_labels):
+            for _ in range(num_of_labels):
                 line = file_handler.readline()
                 words = line.strip().split()
 
             num_of_rows = 0
             line = file_handler.readline()
             while line:
                 num_of_rows += 1
@@ -663,15 +955,16 @@
         logger.debug("\nmask array size: {} (# rows, # cols)", mask_array.shape)
         logger.debug("\nmask array max value: {}", np.amax(mask_array))
 
         return mask_array
 
     def __decompose_label_mask_array(self, label_mask_array, labels):
         """
-        Returns a list of binary 2D numpy.ndarray arrays (pixels being 1s and 0s)
+        Return a list of binary 2D numpy.ndarray arrays (pixels being 1 and 0).
+
         A 2D numpy.ndarray array per label
 
         Input
         =====
         label_mask_array: a numpy.ndarray of numpy.int64 values
                     Each value of the matrix must represents a pixel by means
                     of an int64. This number must be interpreted as a binary
@@ -689,33 +982,33 @@
         Output
         ======
         masks: a 1-column dataframe of 2D binary arrays. Each item is a 2D binary
                numpy.nparray (pixels being 1s and 0s) corresponding to a label,
                where each matrix value <numpy.int8> corresponds to a pixel,
                being 1 if belongs to the label and 0 otherwise.
         """
-
         masks = []
         for label in labels:
             arr = label_mask_array & (2**(label))
             np.clip(arr, 0, 1, out=arr)
-            arr = np.uint8(arr[:,2:-2])
+            arr = np.uint8(arr[:, 2:-2])
             masks.append(arr)
         logger.debug("\nmask list with {} items of {} binary arrays", len(masks), masks[0].shape)
 
         # Transform masks list to a one-column pandas dataframe
         mask_df = pd.DataFrame(columns=['mask'])
         mask_df['mask'] = mask_df['mask'].astype(object)
         mask_df.loc[:, 'mask'] = masks
         return mask_df
 
-    def get_RGBD_labels(self, id, masks = True):
+    def get_RGBD_labels(self, id, masks=True):
         """
-        Returns a list of one binary array per label of the RGBD image
-        referenced by its id
+        Return a list of one binary array per label of the RGBD image.
+
+        The image is referenced by its id
         """
         # Get a dataframe from rh_lblrgbd_labels with labels of the id
         labels = self.__get_RGBD_labels(id)
 
         # By default 2D binary masks column is added to the labels dataframe
         if masks:
             # Get the <id>_labels.txt full path filename
@@ -727,22 +1020,44 @@
             label_masks = self.__decompose_label_mask_array(label_mask_array, labels['local_id'])
             # Return the labels dataframe concatenated with the new label_masks
             # 1-column dataframe
             labels = pd.concat([labels, label_masks], axis=1)
 
         return labels
 
+    def get_RGBD_sensor_size(self):
+        """Return RGB sensor pixel dimension."""
+        RGBD_sensor_size = {
+            'w': 240,
+            'h': 320
+        }
+        return RGBD_sensor_size
+
+
+    def get_RGBD_fps(self):
+        """Return RGBD cameras frame rate.
+        
+        The returned value is a fixed quantity resulting from
+        previous average computations.
+        A more precise value can be calculated by dividing the
+        time between the first frame and the last frame by the
+        number of frames.
+        """
+
+        return 10.72
+
 
     """
     Laser Scanner data
     """
-    def get_laser_scan(self,id):
+    def get_laser_scan(self, id):
         """
-        This function return a dataframe with a laser scan for
-        the observation referenced by id
+        Return a dataframe with a laser scan for the observation.
+
+        The observation is referenced by id
 
         SQL query
 
         select * from rh_lsrscan_scans
             where sensor_observation_id = id
 
         Parameters
@@ -753,15 +1068,14 @@
 
         Returns
         -------
         A dataframe with the query result. An empty dataframe is returned when
         no rows are available, i.e., when the sensor observation does not
         belong to rh_lblrgbd (labelled rgbd)
         """
-
         # if id < 200000:
         #     scan_table_name = 'rh_scans'
         # else:
         #     scan_table_name = 'rh_lsrscan_scans'
 
         scan_table = lambda id: 'rh_raw_scans' if id < 200000 else 'rh_lsrscan_scans'
 
@@ -781,22 +1095,19 @@
         # rh2_sensor_observations
         df.aperture = 4.1847
         df.max_range = 5.6
         df.no_of_shots = 682
 
         return df
 
-
     """
     Scenes
     """
     def get_scenes(self):
-        """
-        Return a dataframe with scenes
-        """
+        """Return a dataframe with scenes."""
         sql_str = (
             f'''
             select
               rh_lblscene.id,
               home_session_id, home_subsession_id, home_id, room_id,
               '{self.__scene_path}' || '/' || new_path || '/' || new_file as scene_file
             from rh_lblscene
@@ -805,16 +1116,17 @@
         )
         logger.debug(sql_str)
         scenes = self.query(sql_str)
         return scenes
 
     def get_scene_labels(self, id, obj=False):
         """
-        This function return a dataframe with a laser scan for
-        the observation referenced by id
+        Return a dataframe with a scene labels for the observation.
+
+        The observation is referenced by id
 
         SQL query
 
         select * from rh_lsrscan_scans
             where sensor_observation_id = id
 
         Parameters
@@ -825,15 +1137,14 @@
 
         Returns
         -------
         A dataframe with the query result. An empty dataframe is returned when
         no rows are available, i.e., when the sensor observation does not
         belong to rh_lblrgbd (labelled rgbd)
         """
-
         # if id < 200000:
         #     scan_table_name = 'rh_scans'
         # else:
         #     scan_table_name = 'rh_lsrscan_scans'
 
         labels_table = lambda obj: 'rh2_scene_bb_objects' if obj else 'rh_lblscene_bboxes'
 
@@ -904,70 +1215,74 @@
                 '''
             )
 
         logger.debug(sql_str)
         df = self.query(sql_str)
         return df
 
-
     """
     Observations
     """
-
     def get_observations(self):
-        """
-        Return a dataframe with observations
+        """Return a dataframe with observations.
+
+        For rooms there is a set of RGBD observations that has been
+        characterized considering averaged features from past observations, as
+        well as features of the closest laser scan in time. The number of room
+        features is 48 and the number of scan features is 9.
+
+        Unfortunately, this set of observations should be considered
+        experimental in the sense that the timestamp data has been lost,
+        preventing the identification of the sensor observations from which
+        they where extracted. Nevertheless, RGBD observations are sequentially
+        ordered.
         """
         sql_str = (
-            f'''
+            '''
             select *
             from rh_observations
             '''
         )
         logger.debug(sql_str)
         observations = self.query(sql_str)
         return observations
 
-    def get_objects_in_observation(self, id):
-        """
-        Return a dataframe with objects in observation
-        """
-        sql_str = (
-            f'''
-            select rh_objects.*
-            from rh_objects_in_observation
-            inner join rh_objects on rh_objects_in_observation.object_id == rh_objects.id
-            where  rh_objects_in_observation.observation_id == {id}
-            '''
-        )
-        logger.debug(sql_str)
-        objects = self.query(sql_str)
-        return objects
-
     def get_objects(self):
-        """
-        Return a dataframe with objects
+        """Return a dataframe with all objects.
+
+        The objects extracted from the observations have also been
+        characterized. For each object the number of features is 32.
         """
         sql_str = (
-            f'''
+            '''
             select *
             from rh_objects
             '''
         )
         logger.debug(sql_str)
         objects = self.query(sql_str)
         return objects
 
     def get_object_relations(self, id=None):
-        """
-        Return a dataframe with object relationships
-        """
+        """Return a dataframe with object relationships.
+
+        The relation between objects has also been calculated and characterized
+        with 11 features.
 
+        The returned dataframe contains the relationships an object is implicit
+        in.
+
+        Args:
+            id: integer number with the identification of an object. If this
+                value is empty this functions returns a dataframe with all
+                relations in the database.
+
+        """
         sql_str = (
-            f'''
+            '''
             select *
             from rh_relations
             '''
         )
 
         where_str = (
             f'''
@@ -978,48 +1293,62 @@
         if (id is not None):
             sql_str = sql_str + where_str
 
         logger.debug(sql_str)
         object_relations = self.query(sql_str)
         return object_relations
 
+    def get_objects_in_observation(self, id):
+        """Return a dataframe with objects in observation.
+
+        The returned objects are contained in a characterized RGBD observation.
+        """
+        sql_str = (
+            f'''
+            select rh_objects.*
+            from rh_objects_in_observation
+            inner join rh_objects on rh_objects_in_observation.object_id == rh_objects.id
+            where  rh_objects_in_observation.observation_id == {id}
+            '''
+        )
+        logger.debug(sql_str)
+        objects = self.query(sql_str)
+        return objects
 
     """
     Stuff
     """
     def select_column(self, column_name, table_name):
-        '''
-        Returns a dataframe with grouped column values
-        (without repetition)
-        '''
+        """
+        Return a dataframe with grouped column values.
 
+        (without repetition)
+        """
         # Get a cursor to execute SQLite statements
-        cur = self.__con.cursor()
         sql_str = (f"select {column_name}  from {table_name} group by {column_name};")
         df_rows = pd.read_sql_query(sql_str, self.__con)
         return df_rows
 
     def query(self, sql, df=True):
-        """Execute a sqlquery over robotathome database
+        """
+        Execute a sqlquery over robotathome database.
 
         Parameters
         ----------
         sql: can be a string with a sql query or a file name that contains the
-             sql query
+             sql query.
         df:  boolean indicating if result is returned as a DataFrame (True) or
              as a sqlite row list (False).  This option (False) is mandatory if
-             the query string has more than one sql command, i.e., it's a script
+             the query string has more than one sql command, i.e., it's a
+             script.
 
         Returns
         -------
-        ans: a DataFrame or a sqlite row list
-
+        ans: a DataFrame or a sqlite row list.
         """
-
-
         if os.path.isfile(sql):
             script = open(sql, 'r')
             query = script.read()
         else:
             query = sql
 
         if df:
@@ -1030,11 +1359,10 @@
             ans = cur.fetchall()
 
         if os.path.isfile(sql):
             script.close()
 
         return ans
 
-
     """
     Lab
     """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `robotathome-1.0.6/robotathome/cv/gluoncv.py` & `robotathome-1.1.0/robotathome/cv/gluoncv.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.0.6/robotathome/cv/opencv.py` & `robotathome-1.1.0/robotathome/cv/opencv.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,33 +4,37 @@
 __author__ = "Gregorio Ambrosio"
 __contact__ = "gambrosio[at]uma.es"
 __copyright__ = "Copyright 2021, Gregorio Ambrosio"
 __date__ = "2021/07/27"
 __license__ = "MIT"
 
 import numpy as np
+import cv2  # note: pip install opencv-python opencv-contrib-python
 import pandas as pd
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 
-# note: conda install -c conda-forge opencv
-import cv2
-# from .log import logger
+from robotathome import logger
 
 
-__all__ = ['get_labeled_img', 'plot_labeled_img', 'get_scan_xy', 'plot_scan', 'plot_scene']
+__all__ = ['get_labeled_img',
+           'plot_labeled_img',
+           'get_scan_xy',
+           'plot_scan',
+           'plot_scene',
+           'process_image',
+           'concat_images']
 
 
-"""
-opencv related functions
-"""
+# computer vision related functions
+
 
 def get_labeled_img(labels, img_file):
     """
-    Returns an image patched with labels
+    Return an image patched with labels.
 
     Input
     =====
     labels:
         Label dataframe with masks (label df + mask col <- get_label_masks(id))
 
     img-file:
@@ -44,34 +48,36 @@
     colors:
         A list with the RGB + Alpha components (4 x 0<= n <=1) of randomly
         chosen colors
     """
     alpha = 0.7
     bgr_img = cv2.imread(img_file, cv2.IMREAD_COLOR)
     labeled_img, colors = overlay_mask(cv2.cvtColor(bgr_img, cv2.COLOR_BGR2RGB),
-                                   labels['mask'],
-                                   alpha)
+                                       labels['mask'],
+                                       alpha)
     return [labeled_img, colors]
 
+
 def plot_labeled_img(labels, img_file):
     """
-    Plot a RGB image patched with colored labels with legend
+    Plot a RGB image patched with colored labels with legend.
 
     Input
     =====
     labels:
         Label dataframe with masks (label df + mask col <- get_label_masks(id))
 
     img-file:
         Full path filename of the RGB image
 
     """
     [labeled_img, colors] = get_labeled_img(labels, img_file)
     plot_mask(labeled_img, labels['name'], colors)
 
+
 def get_scan_xy(laser_scan):
 
     # Computing the smallest angle change
     da = laser_scan.aperture / laser_scan.no_of_shots
     # epsilon = np.finfo(np.float64).eps
 
     # Computing x, y coodinates
@@ -85,15 +91,16 @@
     x.name = 'x'
     y.name = 'y'
     xy = pd.concat([x, y], axis=1)
     # xy(columns = ['x', 'y'])
     xy.index.name = 'shot_id'
     return xy
 
-def plot_scan(laser_scan, cmap = 'gist_heat'):
+
+def plot_scan(laser_scan, cmap='gist_heat'):
 
     # Getting a laser scan dataframe with only valid values
     valid_laser_scan = laser_scan.loc[laser_scan['valid_scan'] == 1]
 
     # Computing the smallest angle change
     da = laser_scan.aperture / laser_scan.no_of_shots
     # epsilon = np.finfo(np.float64).eps
@@ -104,20 +111,27 @@
 
     x = dist * np.cos(angle)
     y = dist * np.sin(angle)
 
     # Plotting points
     # plt.plot(x, y, marker=".", markersize=2)
     sc = plt.scatter(x, y, vmin=0, vmax=laser_scan.max_range, c=dist, s=1, cmap = cmap) # or 'gist_heat'
-    plt.scatter(0,0,s=50)
+    plt.scatter(0, 0, s=50)
     plt.colorbar(sc, label='Distance (m)')
     plt.show()
 
+
 def plot_scene(scene_file):
-    """Docstring
+    """
+    Plot a scene using open3d package.
+
+    Input
+    =====
+    scene_file:
+        File containing the point cloud
     """
     # https://towardsdatascience.com/guide-to-real-time-visualisation-of-massive-3d-point-clouds-in-python-ea6f00241ee0
     # https://towardsdatascience.com/discover-3d-point-cloud-processing-with-python-6112d9ee38e7
 
     # from mpl_toolkits import mplot3d
     # point_cloud = np.loadtxt(scene_file, skiprows=6)
     # xyz = point_cloud[:,:3]
@@ -136,76 +150,103 @@
 
     import open3d as o3d
     pcd = o3d.io.read_point_cloud(scene_file, format='xyzrgb')
     # downpcd = pcd.voxel_down_sample(voxel_size=0.01)
     o3d.visualization.draw_geometries([pcd])
 
 
-"""
-Helpers
-"""
+# Related to RGBD generic function.
+
+
+def process_image(f, img):
+    """ Apply generic function f over img."""
+    return f(img)
+
+
+def concat_images(img_dict):  # (img, par1, ... parn)
+    """ Process the image. """
+    # do something with the img
+    img_list = list(img_dict.values())
+    composed_img = cv2.hconcat(img_list)
+    return composed_img
+
+
+def RGBD_stiching(img_dict):  # (img, par1, ... parn)
+    """ Process the image. """
+    # do something with the img
+    img_list = list(img_dict.values())
+    stitcher = cv2.Stitcher.create(cv2.Stitcher_PANORAMA)
+    status, pano = stitcher.stitch(img_list)
+    if status != cv2.Stitcher_OK:
+        # error code = 1 means that there are no enough features between the 
+        # image intersections.
+        logger.error("Can't stitch images, error code = %d" % status)
+        sys.exit(-1)
+    return pano
+
+
+# Helpers
+
 
 def bin2rgba(img):
     """
     TODO
     """
 
     img = cv2.cvtColor(img*255, cv2.COLOR_GRAY2RGB)
     color_mask = np.random.random((1, 3)).tolist()[0]
 
-    my_mask = cv2.compare(img,245,cv2.CMP_GT)
+    my_mask = cv2.compare(img, 245, cv2.CMP_GT)
     img[my_mask > 0] = 255
 
     for i in range(3):
-        img[:,:,i] = color_mask[i]*255
+        img[:, :, i] = color_mask[i]*255
     plt.imshow(img, interpolation='nearest')
     plt.show()
 
+
 def overlay_mask(img, masks, alpha=0.5):
     # cv2.addWeighted(ovl_img, alpha, base_img, 1 - alpha, 0, base_img)
     # return base_img
     colors = []
     for mask in masks:
         color = np.random.random(3)
-        colors.append(np.append(color,[alpha]))
+        colors.append(np.append(color, [alpha]))
         mask = np.repeat((mask > 0)[:, :, np.newaxis], repeats=3, axis=2)
         img = np.where(mask, img * (1 - alpha) + color*255 * alpha, img)
     return img.astype('uint8'), colors
 
+
 def plot_mask(patched_img, names, colors):
     plt.imshow(patched_img)
     plt.xticks([]), plt.yticks([])  # to hide tick values on X and Y axis
     mpatches_ = []
     for i, color_ in enumerate(colors):
         mpatches_.append(mpatches.Patch(color=color_, label=names[i]))
     plt.legend(handles=mpatches_)
-    # plt.savefig('~/temp/foo.png')
     plt.show()
 
 
-"""
-Lab
-"""
-
-"""
-Stuff
-"""
+# Lab
+
+
+# Old stuff
+
+
 def get_video_from_rgbd(self,
                         source='lblrgbd',
                         home_session_name='alma-s1',
                         home_subsession=0,
                         room_name='alma_masterroom1',
                         sensor_name='RGBD_1',
                         video_file_name=None
                         ):
-
     """
     This functions ...
     """
-
     rows = self.get_sensor_observation_files(source,
                                              home_session_name,
                                              home_subsession,
                                              room_name,
                                              sensor_name)
 
     # Computing frames per second
@@ -264,14 +305,15 @@
     out.release()
 
     if rh.is_being_logged():
         cv2.destroyAllWindows()
 
     return video_file_name
 
+
 def get_composed_video_from_lblrgbd(self,
                                     home_session_name='alma-s1',
                                     home_subsession=0,
                                     room_name='alma_masterroom1',
                                     video_file_name=None
                                     ):
 
@@ -384,14 +426,15 @@
     out.release()
 
     if rh.is_being_logged():
         cv2.destroyAllWindows()
 
     return video_file_name
 
+
 def get_rgb_image_from_lblrgbd(self, so_id):
     """
     This function 
 
     Parameters
     ----------
 
@@ -416,14 +459,15 @@
 
     # rh.logger.debug("rgb_image_path_file_name: {}",
     #                 rgb_image_path_file_name)
     bgr_img = cv2.imread(rgb_image_path_file_name, cv2.IMREAD_COLOR)
 
     return bgr_img
 
+
 def get_depth_image_from_lblrgbd(self, so_id):
     """
     This function
 
     Parameters
     ----------
 
@@ -448,14 +492,15 @@
 
     rh.logger.debug("rgb_image_path_file_name: {}",
                     rgb_image_path_file_name)
     img = cv2.imread(rgb_image_path_file_name, cv2.IMREAD_COLOR)
 
     return cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
 
+
 def lblrgbd_plot_labels(self, so_id):
     img = self.get_rgb_image_from_lblrgbd(so_id)
     labels = self.get_labels_from_lblrgbd(so_id)
     rh.logger.debug("labels: {}", labels)
     mask = self.get_mask_from_lblrgbd(so_id)
     label_mask = self.get_label_mask(mask, labels['local_id'])
     alpha = 0.7
```

### Comparing `robotathome-1.0.6/robotathome/helpers.py` & `robotathome-1.1.0/robotathome/helpers.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.0.6/robotathome/log.py` & `robotathome-1.1.0/robotathome/log.py`

 * *Files identical despite different names*

### Comparing `robotathome-1.0.6/robotathome.egg-info/PKG-INFO` & `robotathome-1.1.0/robotathome.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: robotathome
-Version: 1.0.6
-Summary: This package provides a Python Toolbox with a set of functions to assist in the management of Robot@Home 2 Dataset
-Home-page: https://github.com/goyoambrosio/RobotAtHome_API
+Version: 1.1.0
+Summary: This package provides a Python Toolbox with a set of functions to assist in the management of Robot@Home2 Dataset
+Home-page: https://github.com/goyoambrosio/RobotAtHome2
 Author: G. Ambrosio-Cestero
 Author-email: gambrosio@uma.es
 License: MIT
-Keywords: semantic mapping object categorization object recognition room categorization room recognition contextual information mobile robots domestic robots home environment robotic dataset benchmark
+Keywords: toolbox dataset database relational model mobile robotics computer vision
 Platform: Windows
 Platform: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: full
 Provides-Extra: interactive
 Provides-Extra: cv
 License-File: LICENSE
 
 # Robot@Home2 Dataset Toolbox #
 
-[![PyPI](https://img.shields.io/pypi/v/robotathome)](https://pypi.org/project/robotathome/)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4530453.svg)](https://doi.org/10.5281/zenodo.4530453)
+[![PyPI](https://img.shields.io/pypi/v/robotathome)](https://pypi.org/project/robotathome/ "R@H2 as PyPI package ready to install")
+[![DOI](https://zenodo.org/badge/245370645.svg)](https://zenodo.org/badge/latestdoi/245370645 "This repository released on Zenodo")
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4530453.svg)](https://doi.org/10.5281/zenodo.4530453 "The downloadable R@H2 dataset in Zenodo")
+[![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/drive/folders/1ENnxbKP5MJdlGl2Q93WTbIlofuy6Icxq)
 
 The Robot-at-Home dataset (Robot@Home, paper
 [here](http://mapir.uma.es/papersrepo/2017/2017-raul-IJRR-Robot_at_home_dataset.pdf))
 is a collection of raw and processed data from five domestic settings compiled
 by a mobile robot equipped with 4 RGB-D cameras and a 2D laser scanner. Its main
 purpose is to serve as a testbed for semantic mapping algorithms through the
 categorization of objects and/or rooms.
@@ -324,9 +326,7 @@
     rh.uncompress('~/Downloads/Robot@Home2_files.tgz', '~/WORKSPACE/files')
 else:
     print('Integrity of Robot@Home2_files.tgz is compromised, please download again')
 ```
 
 
 
-
-
```

### Comparing `robotathome-1.0.6/robotathome.egg-info/SOURCES.txt` & `robotathome-1.1.0/robotathome.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -18,12 +18,13 @@
 robotathome/log.py
 robotathome.egg-info/PKG-INFO
 robotathome.egg-info/SOURCES.txt
 robotathome.egg-info/dependency_links.txt
 robotathome.egg-info/requires.txt
 robotathome.egg-info/top_level.txt
 robotathome/core/__init__.py
+robotathome/core/df.py
 robotathome/core/reader.py
 robotathome/cv/__init__.py
 robotathome/cv/_greetings.py
 robotathome/cv/gluoncv.py
 robotathome/cv/opencv.py
```

### Comparing `robotathome-1.0.6/setup.py` & `robotathome-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """
-Setup for RobotAtHome API
+Setup for RobotAtHome2
 """
 
 import os
 import sys
 
 from setuptools import find_packages, setup
 
@@ -35,35 +35,31 @@
     PYTHON_REQUIRES = '<3.7'
 elif sys.platform.startswith('linux'):
     PYTHON_REQUIRES = '>=3.7'
 
 setup(
     name="robotathome",
     version=get_version("robotathome/__init__.py"),
-    description="This package provides a Python Toolbox with a set of functions to assist in the management of Robot@Home 2 Dataset",
+    description="This package provides a Python Toolbox with a set of functions to assist in the management of Robot@Home2 Dataset",
     long_description = LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
 
     license='MIT',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    url="https://github.com/goyoambrosio/RobotAtHome_API",
-    keywords=('semantic mapping '
-              'object categorization '
-              'object recognition '
-              'room categorization '
-              'room recognition '
-              'contextual information '
-              'mobile robots '
-              'domestic robots '
-              'home environment '
-              'robotic dataset benchmark '
+    url="https://github.com/goyoambrosio/RobotAtHome2",
+    keywords=('toolbox '
+              'dataset '
+              'database '
+              'relational model '
+              'mobile robotics '
+              'computer vision '
               ),
 
     author="G. Ambrosio-Cestero",
     author_email="gambrosio@uma.es",
     platforms=['Windows', 'Linux'],
 
     packages=find_packages(),
```

