# Comparing `tmp/hds-stats-0.1.3.tar.gz` & `tmp/hds-stats-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hds-stats-0.1.3.tar", last modified: Sun Apr  9 20:18:43 2023, max compression
+gzip compressed data, was "hds-stats-0.1.4.tar", last modified: Sun Apr  9 20:38:41 2023, max compression
```

## Comparing `hds-stats-0.1.3.tar` & `hds-stats-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-09 20:18:43.809574 hds-stats-0.1.3/
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.1.3/LICENSE
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-04-09 20:18:43.809323 hds-stats-0.1.3/PKG-INFO
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.1.3/README.md
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-09 20:18:43.806917 hds-stats-0.1.3/hds_stats/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       26 2023-04-09 20:04:38.000000 hds-stats-0.1.3/hds_stats/__init__.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     7055 2023-04-09 07:18:03.000000 hds-stats-0.1.3/hds_stats/plot.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    17278 2023-04-09 07:52:15.000000 hds-stats-0.1.3/hds_stats/stat.py
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-09 20:18:43.808950 hds-stats-0.1.3/hds_stats.egg-info/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-04-09 20:18:43.000000 hds-stats-0.1.3/hds_stats.egg-info/PKG-INFO
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      263 2023-04-09 20:18:43.000000 hds-stats-0.1.3/hds_stats.egg-info/SOURCES.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-04-09 20:18:43.000000 hds-stats-0.1.3/hds_stats.egg-info/dependency_links.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       63 2023-04-09 20:18:43.000000 hds-stats-0.1.3/hds_stats.egg-info/requires.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-04-09 20:18:43.000000 hds-stats-0.1.3/hds_stats.egg-info/top_level.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.1.3/pyproject.toml
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-04-09 20:18:43.809668 hds-stats-0.1.3/setup.cfg
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     1177 2023-04-09 20:18:06.000000 hds-stats-0.1.3/setup.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-09 20:38:41.878010 hds-stats-0.1.4/
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.1.4/LICENSE
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-04-09 20:38:41.877781 hds-stats-0.1.4/PKG-INFO
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.1.4/README.md
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-09 20:38:41.875586 hds-stats-0.1.4/hds_stats/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       82 2023-04-09 20:34:59.000000 hds-stats-0.1.4/hds_stats/__init__.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     7055 2023-04-09 07:18:03.000000 hds-stats-0.1.4/hds_stats/plot.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    17281 2023-04-09 20:36:40.000000 hds-stats-0.1.4/hds_stats/stat.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-09 20:38:41.877429 hds-stats-0.1.4/hds_stats.egg-info/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-04-09 20:38:41.000000 hds-stats-0.1.4/hds_stats.egg-info/PKG-INFO
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      263 2023-04-09 20:38:41.000000 hds-stats-0.1.4/hds_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-04-09 20:38:41.000000 hds-stats-0.1.4/hds_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       63 2023-04-09 20:38:41.000000 hds-stats-0.1.4/hds_stats.egg-info/requires.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-04-09 20:38:41.000000 hds-stats-0.1.4/hds_stats.egg-info/top_level.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.1.4/pyproject.toml
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-04-09 20:38:41.878096 hds-stats-0.1.4/setup.cfg
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     1177 2023-04-09 20:38:02.000000 hds-stats-0.1.4/setup.py
```

### Comparing `hds-stats-0.1.3/LICENSE` & `hds-stats-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hds-stats-0.1.3/PKG-INFO` & `hds-stats-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.1.3
+Version: 0.1.4
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.1.3/hds_stats/plot.py` & `hds-stats-0.1.4/hds_stats/plot.py`

 * *Files identical despite different names*

### Comparing `hds-stats-0.1.3/hds_stats/stat.py` & `hds-stats-0.1.4/hds_stats/stat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Linear Regression Variable Selection
+
 def forward_selection(y, X):
     import numpy as np
     import pandas as pd
     import statsmodels.formula.api as smf
     
     if 'const' in X.columns:
         X = X.drop(labels = ['const'], axis = 1)
@@ -380,15 +381,15 @@
     ).T
     
     # result = result.round(3)
     return result
 
 
 # Metrics for Classification: ROC, AUC
-def plot_roc(
+def roc_curve(
     y_true, 
     y_prob, 
     pos = None, 
     color = None
 ):
     import numpy as np
     import pandas as pd
@@ -432,15 +433,15 @@
     plt.title(label = 'ROC Curve')
     plt.xlabel(xlabel = 'FPR')
     plt.ylabel(ylabel = 'TPR')
     plt.legend(loc = 'lower right');
 
 
 # Metrics for Classification: PR, AP
-def plot_pr(
+def pr_curve(
     y_true, 
     y_prob, 
     pos = None, 
     name = None, 
     color = None
 ):
     import numpy as np
```

### Comparing `hds-stats-0.1.3/hds_stats.egg-info/PKG-INFO` & `hds-stats-0.1.4/hds_stats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.1.3
+Version: 0.1.4
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.1.3/setup.py` & `hds-stats-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open(file = 'README.md', mode = 'r', encoding = 'utf-8') as file:
     long_description = file.read()
 
 setup(
     name = 'hds-stats',
-    version = '0.1.3',
+    version = '0.1.4',
     author = 'HelloDataScience',
     author_email = 'hellodatasciencekorea@gmail.com',
     
     description = 'Useful functions for Statistics and Machine Learning',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
```

