# Comparing `tmp/MetrPlot-0.0.2.tar.gz` & `tmp/MetrPlot-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MetrPlot-0.0.2.tar", last modified: Sun Apr  9 01:01:41 2023, max compression
+gzip compressed data, was "MetrPlot-0.0.3.tar", last modified: Sun Apr  9 01:13:59 2023, max compression
```

## Comparing `MetrPlot-0.0.2.tar` & `MetrPlot-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-09 01:01:41.817992 MetrPlot-0.0.2/
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)    35149 2023-04-08 23:44:21.000000 MetrPlot-0.0.2/LICENSE
-drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-09 01:01:41.801992 MetrPlot-0.0.2/MetrPlot/
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     3225 2023-04-09 01:00:35.000000 MetrPlot-0.0.2/MetrPlot/MetrPlot.py
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      119 2023-04-09 01:00:45.000000 MetrPlot-0.0.2/MetrPlot/__init__.py
-drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-09 01:01:41.817992 MetrPlot-0.0.2/MetrPlot.egg-info/
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1187 2023-04-09 01:01:41.000000 MetrPlot-0.0.2/MetrPlot.egg-info/PKG-INFO
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      237 2023-04-09 01:01:41.000000 MetrPlot-0.0.2/MetrPlot.egg-info/SOURCES.txt
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        1 2023-04-09 01:01:41.000000 MetrPlot-0.0.2/MetrPlot.egg-info/dependency_links.txt
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        6 2023-04-09 01:01:41.000000 MetrPlot-0.0.2/MetrPlot.egg-info/requires.txt
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        9 2023-04-09 01:01:41.000000 MetrPlot-0.0.2/MetrPlot.egg-info/top_level.txt
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1187 2023-04-09 01:01:41.817992 MetrPlot-0.0.2/PKG-INFO
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       10 2023-04-08 23:44:21.000000 MetrPlot-0.0.2/README.md
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       38 2023-04-09 01:01:41.829992 MetrPlot-0.0.2/setup.cfg
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1564 2023-04-09 01:01:17.000000 MetrPlot-0.0.2/setup.py
+drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-09 01:13:59.790294 MetrPlot-0.0.3/
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)    35149 2023-04-08 23:44:21.000000 MetrPlot-0.0.3/LICENSE
+drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-09 01:13:59.766294 MetrPlot-0.0.3/MetrPlot/
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     3334 2023-04-09 01:12:52.000000 MetrPlot-0.0.3/MetrPlot/MetrPlot.py
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      119 2023-04-09 01:13:37.000000 MetrPlot-0.0.3/MetrPlot/__init__.py
+drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-09 01:13:59.790294 MetrPlot-0.0.3/MetrPlot.egg-info/
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1187 2023-04-09 01:13:59.000000 MetrPlot-0.0.3/MetrPlot.egg-info/PKG-INFO
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      237 2023-04-09 01:13:59.000000 MetrPlot-0.0.3/MetrPlot.egg-info/SOURCES.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        1 2023-04-09 01:13:59.000000 MetrPlot-0.0.3/MetrPlot.egg-info/dependency_links.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        6 2023-04-09 01:13:59.000000 MetrPlot-0.0.3/MetrPlot.egg-info/requires.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        9 2023-04-09 01:13:59.000000 MetrPlot-0.0.3/MetrPlot.egg-info/top_level.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1187 2023-04-09 01:13:59.790294 MetrPlot-0.0.3/PKG-INFO
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       10 2023-04-08 23:44:21.000000 MetrPlot-0.0.3/README.md
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       38 2023-04-09 01:13:59.798294 MetrPlot-0.0.3/setup.cfg
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1564 2023-04-09 01:13:29.000000 MetrPlot-0.0.3/setup.py
```

### Comparing `MetrPlot-0.0.2/LICENSE` & `MetrPlot-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MetrPlot-0.0.2/MetrPlot/MetrPlot.py` & `MetrPlot-0.0.3/MetrPlot/MetrPlot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 import math
 from decimal import Decimal
 import numpy as np
 
 class MetrPlot:
-    def __init__(self, ms=30, sc_x="log",sc_y="log", name_plot=None, x_name="X", y_name="Y",save_name="Plot",x_s=12,y_s=7):
+    def __init__(self, ms=30, sc_x="log",sc_y="log", name_plot=None, x_name="X", y_name="Y",save_name="Plot",x_s=12,y_s=7,
+                    y_l_s=30,x_l_s=30):
         self.ms = ms
         self.sc_x = sc_x
         self.sc_y = sc_y
         self.name_plot = name_plot
         self.x_name = x_name
         self.y_name = y_name
         self.save_name = save_name
         self.x_s = x_s
         self.y_s = y_s
+        self.y_l_s = y_l_s
+        self.x_l_s = x_l_s
 
     def my_round(self,step,ma,mi,num,str):
         lis = list()
         lis_n=list()
         step = round(step, num)
         start = math.floor(mi / step)
         for i in range(start, start + 18):
@@ -82,16 +85,16 @@
 
         axs.set_ylabel(self.y_name, fontsize=25, labelpad=8)
         axs.grid(color="black", linewidth=0.7)
         axs.set_xlabel(self.x_name, fontsize=25, labelpad=15)
         axs.set_title(self.name_plot, fontsize=28, loc="center", pad=15)
         axs.tick_params(which='major', length=10, width=2)
 
-        axs.set_xticklabels(lis_x, fontsize=20)
-        axs.set_yticklabels(lis_y, fontsize=20)
+        axs.set_xticklabels(lis_x, fontsize=self.x_l_s)
+        axs.set_yticklabels(lis_y, fontsize=self.y_l_s)
 
         axs.get_xaxis().set_tick_params(direction='in')
         axs.get_yaxis().set_tick_params(direction='in')
 
         if save:
             plt.savefig(self.save_name+'.png', format='png', dpi=300)
             plt.savefig(self.save_name+".svg", format="svg")
```

### Comparing `MetrPlot-0.0.2/MetrPlot.egg-info/PKG-INFO` & `MetrPlot-0.0.3/MetrPlot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: MetrPlot
-Version: 0.0.2
+Version: 0.0.3
 Summary: It is a Python library for build a very nice scatter plots. It is an extension of the matplotlib library
 Home-page: https://github.com/89605502155/MetrPlot
 Author: Andrey Ferubko
 Author-email: ferubko1999@yandex.ru
 License: GNU General Public License v3.0
-Download-URL: https://github.com/89605502155/MetrPlot/archive/v0.0.2.zip
+Download-URL: https://github.com/89605502155/MetrPlot/archive/v0.0.3.zip
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MetrPlot-0.0.2/PKG-INFO` & `MetrPlot-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: MetrPlot
-Version: 0.0.2
+Version: 0.0.3
 Summary: It is a Python library for build a very nice scatter plots. It is an extension of the matplotlib library
 Home-page: https://github.com/89605502155/MetrPlot
 Author: Andrey Ferubko
 Author-email: ferubko1999@yandex.ru
 License: GNU General Public License v3.0
-Download-URL: https://github.com/89605502155/MetrPlot/archive/v0.0.2.zip
+Download-URL: https://github.com/89605502155/MetrPlot/archive/v0.0.3.zip
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MetrPlot-0.0.2/setup.py` & `MetrPlot-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from io import open
 from setuptools import setup
 
 
-version = '0.0.2'
+version = '0.0.3'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='MetrPlot',
     version=version,
```

