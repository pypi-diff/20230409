# Comparing `tmp/MetrPlot-0.0.3.tar.gz` & `tmp/MetrPlot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MetrPlot-0.0.3.tar", last modified: Sun Apr  9 01:13:59 2023, max compression
+gzip compressed data, was "MetrPlot-0.0.4.tar", last modified: Sun Apr  9 01:52:46 2023, max compression
```

## Comparing `MetrPlot-0.0.3.tar` & `MetrPlot-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-09 01:13:59.790294 MetrPlot-0.0.3/
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)    35149 2023-04-08 23:44:21.000000 MetrPlot-0.0.3/LICENSE
-drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-09 01:13:59.766294 MetrPlot-0.0.3/MetrPlot/
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     3334 2023-04-09 01:12:52.000000 MetrPlot-0.0.3/MetrPlot/MetrPlot.py
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      119 2023-04-09 01:13:37.000000 MetrPlot-0.0.3/MetrPlot/__init__.py
-drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-09 01:13:59.790294 MetrPlot-0.0.3/MetrPlot.egg-info/
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1187 2023-04-09 01:13:59.000000 MetrPlot-0.0.3/MetrPlot.egg-info/PKG-INFO
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      237 2023-04-09 01:13:59.000000 MetrPlot-0.0.3/MetrPlot.egg-info/SOURCES.txt
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        1 2023-04-09 01:13:59.000000 MetrPlot-0.0.3/MetrPlot.egg-info/dependency_links.txt
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        6 2023-04-09 01:13:59.000000 MetrPlot-0.0.3/MetrPlot.egg-info/requires.txt
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        9 2023-04-09 01:13:59.000000 MetrPlot-0.0.3/MetrPlot.egg-info/top_level.txt
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1187 2023-04-09 01:13:59.790294 MetrPlot-0.0.3/PKG-INFO
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       10 2023-04-08 23:44:21.000000 MetrPlot-0.0.3/README.md
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       38 2023-04-09 01:13:59.798294 MetrPlot-0.0.3/setup.cfg
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1564 2023-04-09 01:13:29.000000 MetrPlot-0.0.3/setup.py
+drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-09 01:52:46.027458 MetrPlot-0.0.4/
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)    35149 2023-04-08 23:44:21.000000 MetrPlot-0.0.4/LICENSE
+drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-09 01:52:46.003458 MetrPlot-0.0.4/MetrPlot/
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     3399 2023-04-09 01:51:37.000000 MetrPlot-0.0.4/MetrPlot/MetrPlot.py
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      119 2023-04-09 01:51:49.000000 MetrPlot-0.0.4/MetrPlot/__init__.py
+drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-09 01:52:46.027458 MetrPlot-0.0.4/MetrPlot.egg-info/
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1187 2023-04-09 01:52:45.000000 MetrPlot-0.0.4/MetrPlot.egg-info/PKG-INFO
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      237 2023-04-09 01:52:45.000000 MetrPlot-0.0.4/MetrPlot.egg-info/SOURCES.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        1 2023-04-09 01:52:45.000000 MetrPlot-0.0.4/MetrPlot.egg-info/dependency_links.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        6 2023-04-09 01:52:45.000000 MetrPlot-0.0.4/MetrPlot.egg-info/requires.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        9 2023-04-09 01:52:45.000000 MetrPlot-0.0.4/MetrPlot.egg-info/top_level.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1187 2023-04-09 01:52:46.027458 MetrPlot-0.0.4/PKG-INFO
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       10 2023-04-08 23:44:21.000000 MetrPlot-0.0.4/README.md
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       38 2023-04-09 01:52:46.039458 MetrPlot-0.0.4/setup.cfg
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1564 2023-04-09 01:51:57.000000 MetrPlot-0.0.4/setup.py
```

### Comparing `MetrPlot-0.0.3/LICENSE` & `MetrPlot-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `MetrPlot-0.0.3/MetrPlot/MetrPlot.py` & `MetrPlot-0.0.4/MetrPlot/MetrPlot.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import matplotlib as mpl
 import math
 from decimal import Decimal
 import numpy as np
 
 class MetrPlot:
     def __init__(self, ms=30, sc_x="log",sc_y="log", name_plot=None, x_name="X", y_name="Y",save_name="Plot",x_s=12,y_s=7,
-                    y_l_s=30,x_l_s=30):
+                    y_l_s=20,x_l_s=20):
         self.ms = ms
         self.sc_x = sc_x
         self.sc_y = sc_y
         self.name_plot = name_plot
         self.x_name = x_name
         self.y_name = y_name
         self.save_name = save_name
@@ -37,25 +37,28 @@
         mi=min(array)
         delta=(ma-mi)
         step=delta/6
         if delta<=0.5:
             return self.my_round(step,ma,mi,2,"1.01")
         if delta >0.5 and delta < 5:
             return self.my_round(step, ma, mi, 1, "1.1")
-        if delta >=5 and delta <= 15:
+        if delta >=5:
             return self.my_round(step, ma, mi, 0, "1")
 
     def logger(self, arr, sc):
         if sc=="log":
             return np.log10(arr)
         return arr
     
-    def pr_axes(self,arr):
+    def pr_axes(self,arr,sc):
         d=0.25*(arr[1]-arr[0])
-        return [arr[0]-d,arr[-1]+d]
+        li=[arr[0]-d,arr[-1]+d]
+        if sc=="log":
+            return np.power(10,li)
+        return  li
     
     def format_lab_ax(self, arr,arr_num, sc):
         if sc=="log":
             arr=['10$^{'+str(i)+'}$' for i in arr]
             arr_num=np.power(10,arr_num)
         return arr,arr_num
     
@@ -68,18 +71,19 @@
 
         x_copy=self.logger(x, self.sc_x)
         y_copy=self.logger(y, self.sc_y)
 
         lis_x, lis_x_num = self.ax(x_copy)
         lis_y, lis_y_num = self.ax(y_copy)
 
-        y_pr=self.pr_axes(lis_y_num)
-        x_pr=self.pr_axes(lis_x_num)
-        axs.set_ylim(ymin=10**y_pr[0],ymax=10**y_pr[1])
-        axs.set_xlim(xmin=10**x_pr[0],xmax=10**x_pr[1])
+        y_pr=self.pr_axes(lis_y_num,self.sc_y)
+        x_pr=self.pr_axes(lis_x_num,self.sc_x)
+
+        axs.set_ylim(ymin=y_pr[0],ymax=y_pr[1])
+        axs.set_xlim(xmin=x_pr[0],xmax=x_pr[1])
 
         lis_x, lis_x_num =self.format_lab_ax(lis_x, lis_x_num, self.sc_x)
         lis_y, lis_y_num =self.format_lab_ax(lis_y, lis_y_num, self.sc_y)
 
         axs.set_xticks(lis_x_num)
         axs.set_yticks(lis_y_num)
 
@@ -101,12 +105,13 @@
         plt.show()
         return 0
 
 
 
 
 
+
```

### Comparing `MetrPlot-0.0.3/MetrPlot.egg-info/PKG-INFO` & `MetrPlot-0.0.4/MetrPlot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: MetrPlot
-Version: 0.0.3
+Version: 0.0.4
 Summary: It is a Python library for build a very nice scatter plots. It is an extension of the matplotlib library
 Home-page: https://github.com/89605502155/MetrPlot
 Author: Andrey Ferubko
 Author-email: ferubko1999@yandex.ru
 License: GNU General Public License v3.0
-Download-URL: https://github.com/89605502155/MetrPlot/archive/v0.0.3.zip
+Download-URL: https://github.com/89605502155/MetrPlot/archive/v0.0.4.zip
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MetrPlot-0.0.3/PKG-INFO` & `MetrPlot-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: MetrPlot
-Version: 0.0.3
+Version: 0.0.4
 Summary: It is a Python library for build a very nice scatter plots. It is an extension of the matplotlib library
 Home-page: https://github.com/89605502155/MetrPlot
 Author: Andrey Ferubko
 Author-email: ferubko1999@yandex.ru
 License: GNU General Public License v3.0
-Download-URL: https://github.com/89605502155/MetrPlot/archive/v0.0.3.zip
+Download-URL: https://github.com/89605502155/MetrPlot/archive/v0.0.4.zip
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MetrPlot-0.0.3/setup.py` & `MetrPlot-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from io import open
 from setuptools import setup
 
 
-version = '0.0.3'
+version = '0.0.4'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='MetrPlot',
     version=version,
```

