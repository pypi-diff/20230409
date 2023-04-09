# Comparing `tmp/MetrPlot-0.0.1.tar.gz` & `tmp/MetrPlot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MetrPlot-0.0.1.tar", last modified: Sun Apr  9 00:47:52 2023, max compression
+gzip compressed data, was "MetrPlot-0.0.2.tar", last modified: Sun Apr  9 01:01:41 2023, max compression
```

## Comparing `MetrPlot-0.0.1.tar` & `MetrPlot-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-09 00:47:52.497030 MetrPlot-0.0.1/
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)    35149 2023-04-08 23:44:21.000000 MetrPlot-0.0.1/LICENSE
-drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-09 00:47:52.473029 MetrPlot-0.0.1/MetrPlot/
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     3220 2023-04-09 00:44:17.000000 MetrPlot-0.0.1/MetrPlot/MetrPlot.py
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      119 2023-04-09 00:45:39.000000 MetrPlot-0.0.1/MetrPlot/__init__.py
-drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-09 00:47:52.493030 MetrPlot-0.0.1/MetrPlot.egg-info/
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1187 2023-04-09 00:47:52.000000 MetrPlot-0.0.1/MetrPlot.egg-info/PKG-INFO
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      206 2023-04-09 00:47:52.000000 MetrPlot-0.0.1/MetrPlot.egg-info/SOURCES.txt
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        1 2023-04-09 00:47:52.000000 MetrPlot-0.0.1/MetrPlot.egg-info/dependency_links.txt
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        9 2023-04-09 00:47:52.000000 MetrPlot-0.0.1/MetrPlot.egg-info/top_level.txt
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1187 2023-04-09 00:47:52.497030 MetrPlot-0.0.1/PKG-INFO
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       10 2023-04-08 23:44:21.000000 MetrPlot-0.0.1/README.md
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       38 2023-04-09 00:47:52.509030 MetrPlot-0.0.1/setup.cfg
--rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1558 2023-04-08 23:49:31.000000 MetrPlot-0.0.1/setup.py
+drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-09 01:01:41.817992 MetrPlot-0.0.2/
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)    35149 2023-04-08 23:44:21.000000 MetrPlot-0.0.2/LICENSE
+drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-09 01:01:41.801992 MetrPlot-0.0.2/MetrPlot/
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     3225 2023-04-09 01:00:35.000000 MetrPlot-0.0.2/MetrPlot/MetrPlot.py
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      119 2023-04-09 01:00:45.000000 MetrPlot-0.0.2/MetrPlot/__init__.py
+drwxrwxr-x   0 ferubko   (1000) ferubko   (1000)        0 2023-04-09 01:01:41.817992 MetrPlot-0.0.2/MetrPlot.egg-info/
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1187 2023-04-09 01:01:41.000000 MetrPlot-0.0.2/MetrPlot.egg-info/PKG-INFO
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)      237 2023-04-09 01:01:41.000000 MetrPlot-0.0.2/MetrPlot.egg-info/SOURCES.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        1 2023-04-09 01:01:41.000000 MetrPlot-0.0.2/MetrPlot.egg-info/dependency_links.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        6 2023-04-09 01:01:41.000000 MetrPlot-0.0.2/MetrPlot.egg-info/requires.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)        9 2023-04-09 01:01:41.000000 MetrPlot-0.0.2/MetrPlot.egg-info/top_level.txt
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1187 2023-04-09 01:01:41.817992 MetrPlot-0.0.2/PKG-INFO
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       10 2023-04-08 23:44:21.000000 MetrPlot-0.0.2/README.md
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)       38 2023-04-09 01:01:41.829992 MetrPlot-0.0.2/setup.cfg
+-rw-rw-r--   0 ferubko   (1000) ferubko   (1000)     1564 2023-04-09 01:01:17.000000 MetrPlot-0.0.2/setup.py
```

### Comparing `MetrPlot-0.0.1/LICENSE` & `MetrPlot-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MetrPlot-0.0.1/MetrPlot/MetrPlot.py` & `MetrPlot-0.0.2/MetrPlot/MetrPlot.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     
     def pr_axes(self,arr):
         d=0.25*(arr[1]-arr[0])
         return [arr[0]-d,arr[-1]+d]
     
     def format_lab_ax(self, arr,arr_num, sc):
         if sc=="log":
-            arr=['10$^{'+i+'}$' for i in arr]
+            arr=['10$^{'+str(i)+'}$' for i in arr]
             arr_num=np.power(10,arr_num)
         return arr,arr_num
     
     def main(self, x, y,save=False):
         mpl.rc('font',family='Times New Roman')
         fig, axs = plt.subplots(figsize=(self.x_s, self.y_s))
         plt.xscale(self.sc_x)
```

### Comparing `MetrPlot-0.0.1/MetrPlot.egg-info/PKG-INFO` & `MetrPlot-0.0.2/MetrPlot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: MetrPlot
-Version: 0.0.1
+Version: 0.0.2
 Summary: It is a Python library for build a very nice scatter plots. It is an extension of the matplotlib library
 Home-page: https://github.com/89605502155/MetrPlot
 Author: Andrey Ferubko
 Author-email: ferubko1999@yandex.ru
 License: GNU General Public License v3.0
-Download-URL: https://github.com/89605502155/MetrPlot/archive/v0.0.1.zip
+Download-URL: https://github.com/89605502155/MetrPlot/archive/v0.0.2.zip
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MetrPlot-0.0.1/PKG-INFO` & `MetrPlot-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: MetrPlot
-Version: 0.0.1
+Version: 0.0.2
 Summary: It is a Python library for build a very nice scatter plots. It is an extension of the matplotlib library
 Home-page: https://github.com/89605502155/MetrPlot
 Author: Andrey Ferubko
 Author-email: ferubko1999@yandex.ru
 License: GNU General Public License v3.0
-Download-URL: https://github.com/89605502155/MetrPlot/archive/v0.0.1.zip
+Download-URL: https://github.com/89605502155/MetrPlot/archive/v0.0.2.zip
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MetrPlot-0.0.1/setup.py` & `MetrPlot-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from io import open
 from setuptools import setup
 
 
-version = '0.0.1'
+version = '0.0.2'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='MetrPlot',
     version=version,
@@ -25,15 +25,15 @@
         version
     ),
     # download_url='https://github.com/89605502155/MetrPlot/archive/main.zip',
 
     license='GNU General Public License v3.0',
 
     packages=['MetrPlot'],
-    #install_requires=[],
+    install_requires=['numpy'],
 
     classifiers=[
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
         'Intended Audience :: End Users/Desktop',
         'Intended Audience :: Developers',
         'Programming Language :: Python',
```

