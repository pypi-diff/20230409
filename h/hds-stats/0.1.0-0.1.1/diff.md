# Comparing `tmp/hds-stats-0.1.0.tar.gz` & `tmp/hds-stats-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hds-stats-0.1.0.tar", last modified: Sun Apr  9 07:39:45 2023, max compression
+gzip compressed data, was "hds-stats-0.1.1.tar", last modified: Sun Apr  9 07:59:40 2023, max compression
```

## Comparing `hds-stats-0.1.0.tar` & `hds-stats-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-09 07:39:45.366311 hds-stats-0.1.0/
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.1.0/LICENSE
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-04-09 07:39:45.366079 hds-stats-0.1.0/PKG-INFO
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.1.0/README.md
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     7055 2023-04-09 07:18:03.000000 hds-stats-0.1.0/hds_plot.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    17245 2023-04-09 07:28:29.000000 hds-stats-0.1.0/hds_stat.py
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-09 07:39:45.365708 hds-stats-0.1.0/hds_stats.egg-info/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-04-09 07:39:45.000000 hds-stats-0.1.0/hds_stats.egg-info/PKG-INFO
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      229 2023-04-09 07:39:45.000000 hds-stats-0.1.0/hds_stats.egg-info/SOURCES.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-04-09 07:39:45.000000 hds-stats-0.1.0/hds_stats.egg-info/dependency_links.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       63 2023-04-09 07:39:45.000000 hds-stats-0.1.0/hds_stats.egg-info/requires.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       18 2023-04-09 07:39:45.000000 hds-stats-0.1.0/hds_stats.egg-info/top_level.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.1.0/pyproject.toml
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-04-09 07:39:45.366397 hds-stats-0.1.0/setup.cfg
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     1164 2023-04-09 07:34:20.000000 hds-stats-0.1.0/setup.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-09 07:59:40.276522 hds-stats-0.1.1/
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.1.1/LICENSE
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-04-09 07:59:40.276242 hds-stats-0.1.1/PKG-INFO
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.1.1/README.md
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     7055 2023-04-09 07:18:03.000000 hds-stats-0.1.1/hds_plot.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    17278 2023-04-09 07:52:15.000000 hds-stats-0.1.1/hds_stat.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-09 07:59:40.275800 hds-stats-0.1.1/hds_stats.egg-info/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-04-09 07:59:40.000000 hds-stats-0.1.1/hds_stats.egg-info/PKG-INFO
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      229 2023-04-09 07:59:40.000000 hds-stats-0.1.1/hds_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-04-09 07:59:40.000000 hds-stats-0.1.1/hds_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       63 2023-04-09 07:59:40.000000 hds-stats-0.1.1/hds_stats.egg-info/requires.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       18 2023-04-09 07:59:40.000000 hds-stats-0.1.1/hds_stats.egg-info/top_level.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.1.1/pyproject.toml
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-04-09 07:59:40.276619 hds-stats-0.1.1/setup.cfg
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     1164 2023-04-09 07:59:04.000000 hds-stats-0.1.1/setup.py
```

### Comparing `hds-stats-0.1.0/LICENSE` & `hds-stats-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hds-stats-0.1.0/PKG-INFO` & `hds-stats-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.1.0
+Version: 0.1.1
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.1.0/hds_plot.py` & `hds-stats-0.1.1/hds_plot.py`

 * *Files identical despite different names*

### Comparing `hds-stats-0.1.0/hds_stat.py` & `hds-stats-0.1.1/hds_stat.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,14 +141,15 @@
 # Linear Regression Diagnosis
 def regressionDiagnosis(model):
     import numpy as np
     import pandas as pd
     import seaborn as sns
     import matplotlib.pyplot as plt
     from scipy import stats
+    import statsmodels.api as sm
     
     plt.figure(figsize = (10, 10), dpi = 100)
     
     # Linearity
     # lowess: locally weighted linear regression
     ax1 = plt.subplot(2, 2, 1)
     sns.regplot(
```

### Comparing `hds-stats-0.1.0/hds_stats.egg-info/PKG-INFO` & `hds-stats-0.1.1/hds_stats.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.1.0
+Version: 0.1.1
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.1.0/setup.py` & `hds-stats-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open(file = "README.md", mode = "r", encoding = "utf-8") as file:
     long_description = file.read()
 
 setup(
     name = "hds-stats",
     
-    version = "0.1.0",
+    version = "0.1.1",
     
     author = "HelloDataScience",
     
     author_email = "hellodatasciencekorea@gmail.com",
     
     description = "Useful functions for Statistics and Machine Learning",
```

