# Comparing `tmp/PRPlot-0.0.7.tar.gz` & `tmp/PRPlot-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PRPlot-0.0.7.tar", last modified: Fri Apr  7 02:17:14 2023, max compression
+gzip compressed data, was "PRPlot-0.0.8.tar", last modified: Sat Apr  8 23:13:27 2023, max compression
```

## Comparing `PRPlot-0.0.7.tar` & `PRPlot-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-07 02:17:14.629146 PRPlot-0.0.7/
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)    35149 2023-04-06 20:40:07.000000 PRPlot-0.0.7/LICENSE
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1188 2023-04-07 02:17:14.629146 PRPlot-0.0.7/PKG-INFO
-drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-07 02:17:14.529144 PRPlot-0.0.7/PRPlot/
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     2464 2023-04-07 02:16:21.000000 PRPlot-0.0.7/PRPlot/PRPlot.py
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      115 2023-04-07 02:16:31.000000 PRPlot-0.0.7/PRPlot/__init__.py
-drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-07 02:17:14.629146 PRPlot-0.0.7/PRPlot.egg-info/
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1188 2023-04-07 02:17:14.000000 PRPlot-0.0.7/PRPlot.egg-info/PKG-INFO
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      192 2023-04-07 02:17:14.000000 PRPlot-0.0.7/PRPlot.egg-info/SOURCES.txt
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        1 2023-04-07 02:17:14.000000 PRPlot-0.0.7/PRPlot.egg-info/dependency_links.txt
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        7 2023-04-07 02:17:14.000000 PRPlot-0.0.7/PRPlot.egg-info/top_level.txt
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        8 2023-04-06 20:40:07.000000 PRPlot-0.0.7/README.md
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       38 2023-04-07 02:17:14.641146 PRPlot-0.0.7/setup.cfg
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1557 2023-04-07 02:16:39.000000 PRPlot-0.0.7/setup.py
+drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-08 23:13:27.508092 PRPlot-0.0.8/
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)    35149 2023-04-06 20:40:07.000000 PRPlot-0.0.8/LICENSE
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1294 2023-04-08 23:13:27.508092 PRPlot-0.0.8/PKG-INFO
+drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-08 23:13:27.488092 PRPlot-0.0.8/PRPlot/
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     2745 2023-04-08 23:10:38.000000 PRPlot-0.0.8/PRPlot/PRPlot.py
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      115 2023-04-08 23:12:58.000000 PRPlot-0.0.8/PRPlot/__init__.py
+drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-08 23:13:27.508092 PRPlot-0.0.8/PRPlot.egg-info/
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1294 2023-04-08 23:13:27.000000 PRPlot-0.0.8/PRPlot.egg-info/PKG-INFO
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      192 2023-04-08 23:13:27.000000 PRPlot-0.0.8/PRPlot.egg-info/SOURCES.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        1 2023-04-08 23:13:27.000000 PRPlot-0.0.8/PRPlot.egg-info/dependency_links.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        7 2023-04-08 23:13:27.000000 PRPlot-0.0.8/PRPlot.egg-info/top_level.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      114 2023-04-08 23:12:36.000000 PRPlot-0.0.8/README.md
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       38 2023-04-08 23:13:27.596093 PRPlot-0.0.8/setup.cfg
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1557 2023-04-08 23:12:50.000000 PRPlot-0.0.8/setup.py
```

### Comparing `PRPlot-0.0.7/LICENSE` & `PRPlot-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PRPlot-0.0.7/PRPlot/PRPlot.py` & `PRPlot-0.0.8/PRPlot/PRPlot.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,23 +41,31 @@
     def n_dat(self,arr1,arr2):
         lis=list()
         for i in arr1:
             lis.append(i)
         for i in arr2:
             lis.append(i)
         return lis
+    
+    def pr_axes(self,arr:list)-> list:
+        d=0.25*(arr[1]-arr[0])
+        return [arr[0]-d,arr[-1]+d]
 
     def main(self, ref, predict, save,ms=30, lw=3, name_plot=None, x_name="X", y_name="Y",save_name="Plot"):
         mpl.rc('font', family='Times New Roman')
         fig, axs = plt.subplots(figsize=(12, 7))
         axs.plot(ref, predict, ".", color="red", ms=ms)
         axs.plot(ref, ref, color="blue", lw=lw)
 
         lis_x, lis_x_num = self.ax(ref)
         lis_y, lis_y_num = self.ax(self.n_dat(ref,predict))
+        y_pr=self.pr_axes(lis_y_num)
+        x_pr=self.pr_axes(lis_x_num)
+        axs.set_ylim(ymin=y_pr[0],ymax=y_pr[1])
+        axs.set_xlim(xmin=x_pr[0],xmax=x_pr[1])
 
         axs.set_xticks(lis_x_num)
         axs.set_yticks(lis_y_num)
 
         axs.set_ylabel(y_name, fontsize=25, labelpad=8)
         axs.grid(color="black", linewidth=0.7)
         axs.set_xlabel(x_name, fontsize=25, labelpad=15)
```

### Comparing `PRPlot-0.0.7/setup.py` & `PRPlot-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from io import open
 from setuptools import setup
 
 
-version = '0.0.7'
+version = '0.0.8'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='PRPlot',
     version=version,
```

