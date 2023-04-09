# Comparing `tmp/PRPlot-0.0.8.tar.gz` & `tmp/PRPlot-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PRPlot-0.0.8.tar", last modified: Sat Apr  8 23:13:27 2023, max compression
+gzip compressed data, was "PRPlot-0.0.9.tar", last modified: Sun Apr  9 02:06:36 2023, max compression
```

## Comparing `PRPlot-0.0.8.tar` & `PRPlot-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-08 23:13:27.508092 PRPlot-0.0.8/
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)    35149 2023-04-06 20:40:07.000000 PRPlot-0.0.8/LICENSE
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1294 2023-04-08 23:13:27.508092 PRPlot-0.0.8/PKG-INFO
-drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-08 23:13:27.488092 PRPlot-0.0.8/PRPlot/
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     2745 2023-04-08 23:10:38.000000 PRPlot-0.0.8/PRPlot/PRPlot.py
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      115 2023-04-08 23:12:58.000000 PRPlot-0.0.8/PRPlot/__init__.py
-drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-08 23:13:27.508092 PRPlot-0.0.8/PRPlot.egg-info/
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1294 2023-04-08 23:13:27.000000 PRPlot-0.0.8/PRPlot.egg-info/PKG-INFO
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      192 2023-04-08 23:13:27.000000 PRPlot-0.0.8/PRPlot.egg-info/SOURCES.txt
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        1 2023-04-08 23:13:27.000000 PRPlot-0.0.8/PRPlot.egg-info/dependency_links.txt
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        7 2023-04-08 23:13:27.000000 PRPlot-0.0.8/PRPlot.egg-info/top_level.txt
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      114 2023-04-08 23:12:36.000000 PRPlot-0.0.8/README.md
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       38 2023-04-08 23:13:27.596093 PRPlot-0.0.8/setup.cfg
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1557 2023-04-08 23:12:50.000000 PRPlot-0.0.8/setup.py
+drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-09 02:06:36.223437 PRPlot-0.0.9/
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)    35149 2023-04-06 20:40:07.000000 PRPlot-0.0.9/LICENSE
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1295 2023-04-09 02:06:36.223437 PRPlot-0.0.9/PKG-INFO
+drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-09 02:06:36.199437 PRPlot-0.0.9/PRPlot/
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     2943 2023-04-09 02:05:22.000000 PRPlot-0.0.9/PRPlot/PRPlot.py
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      115 2023-04-09 01:58:10.000000 PRPlot-0.0.9/PRPlot/__init__.py
+drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-09 02:06:36.215437 PRPlot-0.0.9/PRPlot.egg-info/
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1295 2023-04-09 02:06:35.000000 PRPlot-0.0.9/PRPlot.egg-info/PKG-INFO
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      192 2023-04-09 02:06:35.000000 PRPlot-0.0.9/PRPlot.egg-info/SOURCES.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        1 2023-04-09 02:06:35.000000 PRPlot-0.0.9/PRPlot.egg-info/dependency_links.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        7 2023-04-09 02:06:35.000000 PRPlot-0.0.9/PRPlot.egg-info/top_level.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      114 2023-04-08 23:12:36.000000 PRPlot-0.0.9/README.md
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       38 2023-04-09 02:06:36.251438 PRPlot-0.0.9/setup.cfg
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1558 2023-04-09 02:06:17.000000 PRPlot-0.0.9/setup.py
```

### Comparing `PRPlot-0.0.8/LICENSE` & `PRPlot-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PRPlot-0.0.8/PKG-INFO` & `PRPlot-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PRPlot
-Version: 0.0.8
+Version: 0.0.9
 Summary: It is a Python library for build a very nice predict-reference plots. It is an extension of the matplotlib library
 Home-page: https://github.com/89605502155/PRPlot
 Author: Andrey Ferubko
 Author-email: ferubko1999@yandex.ru
 License: GNU General Public License v3.0
-Download-URL: https://github.com/89605502155/N-PLS/archive/v0.0.8.zip
+Download-URL: https://github.com/89605502155/PRPlot/archive/v0.0.9.zip
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PRPlot-0.0.8/PRPlot/PRPlot.py` & `PRPlot-0.0.9/PRPlot/PRPlot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 import math
 from decimal import Decimal
 
 
-class PRPlot():
-    def __int__(self, ms=30, lw=3, name_plot=None, x_name="X", y_name="Y",save_name="Plot"):
+class PRPlot:
+    def __int__(self, ms=30, lw=3, name_plot=None, x_name="X", y_name="Y",
+                save_name="Plot",size_x=12,size_y=7,lab_size_x=20,
+                lab_size_y=20):
         self.ms = ms
         self.lw = lw
         self.name_plot = name_plot
         self.x_name = x_name
         self.y_name = y_name
         self.save_name = save_name
+        self.size_x=size_x
+        self.size_y=size_y
+        self.lab_size_x=lab_size_x
+        self.lab_size_y=lab_size_y
 
     def my_round(self,step,ma,mi,num,str):
         lis = list()
         lis_n=list()
         step = round(step, num)
         start = math.floor(mi / step)
         for i in range(start, start + 18):
@@ -31,56 +37,56 @@
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
 
     def n_dat(self,arr1,arr2):
         lis=list()
         for i in arr1:
             lis.append(i)
         for i in arr2:
             lis.append(i)
         return lis
     
     def pr_axes(self,arr:list)-> list:
         d=0.25*(arr[1]-arr[0])
         return [arr[0]-d,arr[-1]+d]
 
-    def main(self, ref, predict, save,ms=30, lw=3, name_plot=None, x_name="X", y_name="Y",save_name="Plot"):
+    def main(self, ref, predict, save):
         mpl.rc('font', family='Times New Roman')
-        fig, axs = plt.subplots(figsize=(12, 7))
-        axs.plot(ref, predict, ".", color="red", ms=ms)
-        axs.plot(ref, ref, color="blue", lw=lw)
+        fig, axs = plt.subplots(figsize=(self.size_x, self.size_y))
+        axs.plot(ref, predict, ".", color="red", ms=self.ms)
+        axs.plot(ref, ref, color="blue", lw=self.lw)
 
         lis_x, lis_x_num = self.ax(ref)
         lis_y, lis_y_num = self.ax(self.n_dat(ref,predict))
         y_pr=self.pr_axes(lis_y_num)
         x_pr=self.pr_axes(lis_x_num)
         axs.set_ylim(ymin=y_pr[0],ymax=y_pr[1])
         axs.set_xlim(xmin=x_pr[0],xmax=x_pr[1])
 
         axs.set_xticks(lis_x_num)
         axs.set_yticks(lis_y_num)
 
-        axs.set_ylabel(y_name, fontsize=25, labelpad=8)
+        axs.set_ylabel(self.y_name, fontsize=25, labelpad=8)
         axs.grid(color="black", linewidth=0.7)
-        axs.set_xlabel(x_name, fontsize=25, labelpad=15)
-        axs.set_title(name_plot, fontsize=28, loc="center", pad=15)
+        axs.set_xlabel(self.x_name, fontsize=25, labelpad=15)
+        axs.set_title(self.name_plot, fontsize=28, loc="center", pad=15)
         axs.tick_params(which='major', length=10, width=2)
 
-        axs.set_xticklabels(lis_x, fontsize=20)
-        axs.set_yticklabels(lis_y, fontsize=20)
+        axs.set_xticklabels(lis_x, fontsize=self.lab_size_x)
+        axs.set_yticklabels(lis_y, fontsize=self.lab_size_y)
 
         axs.get_xaxis().set_tick_params(direction='in')
         axs.get_yaxis().set_tick_params(direction='in')
 
         if save:
-            plt.savefig(save_name+'.png', format='png', dpi=300)
-            plt.savefig(save_name+".svg", format="svg")
+            plt.savefig(self.save_name+'.png', format='png', dpi=300)
+            plt.savefig(self.save_name+".svg", format="svg")
         plt.show()
         return 0
```

### Comparing `PRPlot-0.0.8/PRPlot.egg-info/PKG-INFO` & `PRPlot-0.0.9/PRPlot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PRPlot
-Version: 0.0.8
+Version: 0.0.9
 Summary: It is a Python library for build a very nice predict-reference plots. It is an extension of the matplotlib library
 Home-page: https://github.com/89605502155/PRPlot
 Author: Andrey Ferubko
 Author-email: ferubko1999@yandex.ru
 License: GNU General Public License v3.0
-Download-URL: https://github.com/89605502155/N-PLS/archive/v0.0.8.zip
+Download-URL: https://github.com/89605502155/PRPlot/archive/v0.0.9.zip
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PRPlot-0.0.8/setup.py` & `PRPlot-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from io import open
 from setuptools import setup
 
 
-version = '0.0.8'
+version = '0.0.9'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='PRPlot',
     version=version,
@@ -17,15 +17,15 @@
     description=(
         'It is a Python library for build a very nice predict-reference plots. It is an extension of the matplotlib library'
     ),
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     url='https://github.com/89605502155/PRPlot',
-    download_url='https://github.com/89605502155/N-PLS/archive/v{}.zip'.format(
+    download_url='https://github.com/89605502155/PRPlot/archive/v{}.zip'.format(
         version
     ),
     # download_url='https://github.com/89605502155/PRPlot/archive/main.zip',
 
     license='GNU General Public License v3.0',
 
     packages=['PRPlot'],
```

