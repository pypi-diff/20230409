# Comparing `tmp/vandal-3.8.9.tar.gz` & `tmp/vandal-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vandal-3.8.9.tar", last modified: Sat Aug  6 23:50:22 2022, max compression
+gzip compressed data, was "vandal-4.0.0.tar", last modified: Sun Apr  9 07:30:54 2023, max compression
```

## Comparing `vandal-3.8.9.tar` & `vandal-4.0.0.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxrwxrwx   0        0        0        0 2022-08-06 23:50:22.561632 vandal-3.8.9/
--rw-rw-rw-   0        0        0    13938 2022-08-06 23:47:26.000000 vandal-3.8.9/CHANGELOG.md
--rw-rw-rw-   0        0        0       30 2021-12-27 12:01:11.000000 vandal-3.8.9/MANIFEST.in
--rw-rw-rw-   0        0        0    27768 2022-08-06 23:50:22.558631 vandal-3.8.9/PKG-INFO
--rw-rw-rw-   0        0        0     6185 2022-07-19 13:16:35.000000 vandal-3.8.9/README.md
-drwxrwxrwx   0        0        0        0 2022-08-06 23:50:22.352631 vandal-3.8.9/_deprecated/
-drwxrwxrwx   0        0        0        0 2022-08-06 23:50:22.405631 vandal-3.8.9/_deprecated/app/
--rw-rw-rw-   0        0        0      286 2022-01-04 13:44:00.000000 vandal-3.8.9/_deprecated/app/__init__.py
--rw-rw-rw-   0        0        0     7353 2022-01-26 00:01:34.000000 vandal-3.8.9/_deprecated/app/particles.py
-drwxrwxrwx   0        0        0        0 2022-08-06 23:50:22.432679 vandal-3.8.9/_manifesto/
--rw-rw-rw-   0        0        0      527 2022-06-13 10:00:51.000000 vandal-3.8.9/_manifesto/Manifesto.md
-drwxrwxrwx   0        0        0        0 2022-08-06 23:50:22.465629 vandal-3.8.9/_testenv/
--rw-rw-rw-   0        0        0    32870 2022-07-20 12:09:22.000000 vandal-3.8.9/_testenv/F_montecarlo.py
-drwxrwxrwx   0        0        0        0 2022-08-06 23:50:22.467631 vandal-3.8.9/_testenv/GUI/
--rw-rw-rw-   0        0        0      672 2022-06-07 08:33:58.000000 vandal-3.8.9/_testenv/GUI/GUIapp.py
-drwxrwxrwx   0        0        0        0 2022-08-06 23:50:22.469629 vandal-3.8.9/_testenv/pyscript/
--rw-rw-rw-   0        0        0       37 2022-06-05 23:46:06.000000 vandal-3.8.9/_testenv/pyscript/data.py
--rw-rw-rw-   0        0        0       75 2021-12-30 09:21:24.000000 vandal-3.8.9/_upload.txt
--rw-rw-rw-   0        0        0      112 2022-08-06 23:50:03.000000 vandal-3.8.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-08-06 23:50:22.561632 vandal-3.8.9/setup.cfg
--rw-rw-rw-   0        0        0     2677 2022-08-06 23:49:55.000000 vandal-3.8.9/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-06 23:50:22.476632 vandal-3.8.9/vandal/
--rw-rw-rw-   0        0        0     5836 2022-08-06 23:44:35.000000 vandal-3.8.9/vandal/__init__.py
--rw-rw-rw-   0        0        0      964 2022-08-06 23:44:13.000000 vandal-3.8.9/vandal/__main__.py
-drwxrwxrwx   0        0        0        0 2022-08-06 23:50:22.536630 vandal-3.8.9/vandal/hub/
--rw-rw-rw-   0        0        0      773 2022-08-06 23:40:19.000000 vandal-3.8.9/vandal/hub/__init__.py
--rw-rw-rw-   0        0        0     1006 2022-07-28 00:47:42.000000 vandal-3.8.9/vandal/hub/example.py
--rw-rw-rw-   0        0        0     7975 2022-08-06 23:49:34.000000 vandal-3.8.9/vandal/hub/toolkit.py
-drwxrwxrwx   0        0        0        0 2022-08-06 23:50:22.541636 vandal-3.8.9/vandal/misc/
--rw-rw-rw-   0        0        0      482 2022-02-09 00:26:37.000000 vandal-3.8.9/vandal/misc/__init__.py
--rw-rw-rw-   0        0        0      812 2022-08-06 23:47:50.000000 vandal-3.8.9/vandal/misc/_meta.py
-drwxrwxrwx   0        0        0        0 2022-08-06 23:50:22.553631 vandal-3.8.9/vandal/objects/
--rw-rw-rw-   0        0        0      506 2022-06-11 11:46:21.000000 vandal-3.8.9/vandal/objects/__init__.py
--rw-rw-rw-   0        0        0     4803 2022-06-11 11:46:31.000000 vandal-3.8.9/vandal/objects/dijkstra.py
--rw-rw-rw-   0        0        0     4829 2022-08-06 23:48:43.000000 vandal-3.8.9/vandal/objects/eoq.py
--rw-rw-rw-   0        0        0    20980 2022-08-06 23:48:13.000000 vandal-3.8.9/vandal/objects/montecarlo.py
-drwxrwxrwx   0        0        0        0 2022-08-06 23:50:22.529632 vandal-3.8.9/vandal.egg-info/
--rw-rw-rw-   0        0        0    27768 2022-08-06 23:50:16.000000 vandal-3.8.9/vandal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2022-08-06 23:50:22.000000 vandal-3.8.9/vandal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-06 23:50:16.000000 vandal-3.8.9/vandal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2022-08-06 23:50:16.000000 vandal-3.8.9/vandal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-08-06 23:50:16.000000 vandal-3.8.9/vandal.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 07:30:54.673886 vandal-4.0.0/
+-rw-rw-rw-   0        0        0    14325 2023-04-09 07:29:42.000000 vandal-4.0.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0       30 2021-12-27 12:01:11.000000 vandal-4.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    28349 2023-04-09 07:30:54.672884 vandal-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6267 2022-10-11 15:31:44.000000 vandal-4.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 07:30:54.234881 vandal-4.0.0/_deprecated/
+drwxrwxrwx   0        0        0        0 2023-04-09 07:30:54.341885 vandal-4.0.0/_deprecated/app/
+-rw-rw-rw-   0        0        0      286 2022-01-04 13:44:00.000000 vandal-4.0.0/_deprecated/app/__init__.py
+-rw-rw-rw-   0        0        0     7353 2022-01-26 00:01:34.000000 vandal-4.0.0/_deprecated/app/particles.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:30:54.367884 vandal-4.0.0/_manifesto/
+-rw-rw-rw-   0        0        0      527 2022-06-13 10:00:51.000000 vandal-4.0.0/_manifesto/Manifesto.md
+drwxrwxrwx   0        0        0        0 2023-04-09 07:30:54.246885 vandal-4.0.0/_testenv/
+drwxrwxrwx   0        0        0        0 2023-04-09 07:30:54.379885 vandal-4.0.0/_testenv/GUI/
+-rw-rw-rw-   0        0        0      672 2022-06-07 08:33:58.000000 vandal-4.0.0/_testenv/GUI/GUIapp.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:30:54.382883 vandal-4.0.0/_testenv/pyscript/
+-rw-rw-rw-   0        0        0       37 2022-06-05 23:46:06.000000 vandal-4.0.0/_testenv/pyscript/data.py
+-rw-rw-rw-   0        0        0       75 2021-12-30 09:21:24.000000 vandal-4.0.0/_upload.txt
+-rw-rw-rw-   0        0        0       94 2022-11-10 00:42:11.000000 vandal-4.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 07:30:54.674885 vandal-4.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     2651 2022-11-10 00:42:30.000000 vandal-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:30:54.389886 vandal-4.0.0/vandal/
+-rw-rw-rw-   0        0        0     5976 2023-04-09 07:26:45.000000 vandal-4.0.0/vandal/__init__.py
+-rw-rw-rw-   0        0        0     1238 2023-04-09 07:26:22.000000 vandal-4.0.0/vandal/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:30:54.585884 vandal-4.0.0/vandal/apps/
+-rw-rw-rw-   0        0        0      307 2023-04-09 07:23:51.000000 vandal-4.0.0/vandal/apps/__init__.py
+-rw-rw-rw-   0        0        0     5545 2023-04-09 07:24:24.000000 vandal-4.0.0/vandal/apps/montecarlo_gui.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:30:54.592884 vandal-4.0.0/vandal/hub/
+-rw-rw-rw-   0        0        0      870 2022-08-07 13:51:39.000000 vandal-4.0.0/vandal/hub/__init__.py
+-rw-rw-rw-   0        0        0     1006 2022-07-28 00:47:42.000000 vandal-4.0.0/vandal/hub/example.py
+-rw-rw-rw-   0        0        0     8951 2022-08-22 21:06:18.000000 vandal-4.0.0/vandal/hub/toolkit.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:30:54.601883 vandal-4.0.0/vandal/misc/
+-rw-rw-rw-   0        0        0      482 2022-02-09 00:26:37.000000 vandal-4.0.0/vandal/misc/__init__.py
+-rw-rw-rw-   0        0        0      812 2023-04-09 07:30:24.000000 vandal-4.0.0/vandal/misc/_meta.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:30:54.669883 vandal-4.0.0/vandal/objects/
+-rw-rw-rw-   0        0        0      506 2022-06-11 11:46:21.000000 vandal-4.0.0/vandal/objects/__init__.py
+-rw-rw-rw-   0        0        0     4803 2022-06-11 11:46:31.000000 vandal-4.0.0/vandal/objects/dijkstra.py
+-rw-rw-rw-   0        0        0     4851 2022-08-07 13:51:43.000000 vandal-4.0.0/vandal/objects/eoq.py
+-rw-rw-rw-   0        0        0    21002 2022-08-07 13:51:48.000000 vandal-4.0.0/vandal/objects/montecarlo.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:30:54.489886 vandal-4.0.0/vandal.egg-info/
+-rw-rw-rw-   0        0        0    28349 2023-04-09 07:30:47.000000 vandal-4.0.0/vandal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      660 2023-04-09 07:30:52.000000 vandal-4.0.0/vandal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 07:30:47.000000 vandal-4.0.0/vandal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-04-09 07:30:47.000000 vandal-4.0.0/vandal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-09 07:30:47.000000 vandal-4.0.0/vandal.egg-info/top_level.txt
```

### Comparing `vandal-3.8.9/CHANGELOG.md` & `vandal-4.0.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -508,8 +508,19 @@
 - aligned to logistics changes.
 
 3.8.8 (28/07/2022)
 - aligned to logistics changes.
 
 3.8.9 (07/08/2022)
 - paint_text added to toolkit.
-- now also inits colorama colors before other packages to avoid conflicts.
+- now also inits colorama colors before other packages to avoid conflicts.
+
+3.8.10 (07/08/2022)
+- changes to coloring policies.
+- aligned paint_text to duality._paint_text changes.
+
+3.8.11 (13/08/2022)
+- aligned to recent logistics and duality changes.
+
+4.0.0 (09/04/2023)
+Hello everyone, I am back with great news after a few months:
+- MonteCarlo now has a GUI. Call it as python -m vandal -e montecarlogui. It is in testing phase so stay patient.
```

### Comparing `vandal-3.8.9/PKG-INFO` & `vandal-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: vandal
-Version: 3.8.9
+Version: 4.0.0
 Summary: Data science, Data manipulation and Machine learning library.
 Home-page: http://github.com/dkundih/vandal
 Author: David Kundih
 Author-email: kundihdavid@gmail.com
 Maintainer: David Kundih
 Maintainer-email: kundihdavid@gmail.com
 License: Apache Software License
-Download-URL: https://github.com/dkundih/vandal/archive/refs/tags/v3.8.9.tar.gz
+Download-URL: https://github.com/dkundih/vandal/archive/refs/tags/v4.0.0.tar.gz
 Project-URL: Documentation, https://github.com/dkundih/vandal/blob/master/README.md
 Project-URL: Source Code, https://github.com/dkundih/vandal/tree/master/vandal
 Description: ![vandal-header](https://raw.githubusercontent.com/dkundih/vandal/master/_logistics/vandal.jpg)
         
         [![Downloads](https://img.shields.io/pypi/dm/vandal?color=F43&label=Downloads&style=flat-square)](https://pypi.org/project/vandal)
         [![License](https://img.shields.io/pypi/l/vandal?color=178&label=License&style=flat-square)](https://github.com/dkundih/vandal/blob/main/LICENSE)
         [![PyPi version](https://img.shields.io/pypi/v/vandal?color=178&&label=PyPi%20version&style=flat-square)](https://pypi.org/project/vandal)
@@ -137,19 +137,21 @@
         The library itself, it's maintenance, updates and stability, logo, videos, promotional materials and everything associated with duality are done by **David Kundih** from **Croatia**.
         
         <h1 align='center'> Hi! :wave:</h1>
          
         <img src='https://raw.githubusercontent.com/dkundih/dkundih/main/.logistics/BLUERED_GHiLI.jpg'/>
         
         <p align='center'>
-        My name is <b>David Kundih</b> and I am a Master's student of <b>Sustainable mobility and logistics</b> at the <b>University North</b>, currently specializing in <b>Digital transformation of traffic and logistics using Python.</b>
+        My name is <b>David Kundih</b> and I am a <b>Master of Engineering in Sustainable Mobility and Logistics</b>, currently specializing in <b>Digital Transformation of Traffic and Logistics using Python, JavaScript, HTML and CSS.</b>
         </p>
          
         <h4 align='center'>My latest projects:</h4>
         <p align='center'>
+        <a href="https://github.com/dkundih/promet-kc">promet-kc</p>
+        <p align='center'>
         <a href="https://github.com/dkundih/vandal">vandal</p>  
         <p align='center'>
         <a href="https://github.com/dkundih/duality">duality</p>  
         <p align='center'>
         <a href="https://github.com/dkundih/logistics">logistics</p>  
         <p align='center'>
         <a href="https://github.com/dkundih/unin">unin</a></p>
@@ -679,14 +681,26 @@
         
         3.8.8 (28/07/2022)
         - aligned to logistics changes.
         
         3.8.9 (07/08/2022)
         - paint_text added to toolkit.
         - now also inits colorama colors before other packages to avoid conflicts.
+        
+        3.8.10 (07/08/2022)
+        - changes to coloring policies.
+        - aligned paint_text to duality._paint_text changes.
+        
+        3.8.11 (13/08/2022)
+        - aligned to recent logistics and duality changes.
+        
+        4.0.0 (09/04/2023)
+        Hello everyone, I am back with great news after a few months:
+        - MonteCarlo now has a GUI. Call it as python -m vandal -e montecarlogui. It is in testing phase so stay patient.
+        
 Keywords: data science,machine learning,data manipulation,artificial intelligence,AI,unin,duality,duality-py,duality.py,vandal,vandal-py,vandal.py
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `vandal-3.8.9/README.md` & `vandal-4.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -124,19 +124,21 @@
 The library itself, it's maintenance, updates and stability, logo, videos, promotional materials and everything associated with duality are done by **David Kundih** from **Croatia**.
 
 <h1 align='center'> Hi! :wave:</h1>
  
 <img src='https://raw.githubusercontent.com/dkundih/dkundih/main/.logistics/BLUERED_GHiLI.jpg'/>
 
 <p align='center'>
-My name is <b>David Kundih</b> and I am a Master's student of <b>Sustainable mobility and logistics</b> at the <b>University North</b>, currently specializing in <b>Digital transformation of traffic and logistics using Python.</b>
+My name is <b>David Kundih</b> and I am a <b>Master of Engineering in Sustainable Mobility and Logistics</b>, currently specializing in <b>Digital Transformation of Traffic and Logistics using Python, JavaScript, HTML and CSS.</b>
 </p>
  
 <h4 align='center'>My latest projects:</h4>
 <p align='center'>
+<a href="https://github.com/dkundih/promet-kc">promet-kc</p>
+<p align='center'>
 <a href="https://github.com/dkundih/vandal">vandal</p>  
 <p align='center'>
 <a href="https://github.com/dkundih/duality">duality</p>  
 <p align='center'>
 <a href="https://github.com/dkundih/logistics">logistics</p>  
 <p align='center'>
 <a href="https://github.com/dkundih/unin">unin</a></p>
```

### Comparing `vandal-3.8.9/_deprecated/app/particles.py` & `vandal-4.0.0/_deprecated/app/particles.py`

 * *Files identical despite different names*

### Comparing `vandal-3.8.9/_manifesto/Manifesto.md` & `vandal-4.0.0/_manifesto/Manifesto.md`

 * *Files identical despite different names*

### Comparing `vandal-3.8.9/_testenv/GUI/GUIapp.py` & `vandal-4.0.0/_testenv/GUI/GUIapp.py`

 * *Files identical despite different names*

### Comparing `vandal-3.8.9/setup.py` & `vandal-4.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,16 +49,15 @@
     'Documentation': 'https://github.com/dkundih/vandal/blob/master/README.md',
     'Source Code': 'https://github.com/dkundih/vandal/tree/master/vandal'
   }, 
   classifiers = classifiers,
   keywords = 'data science, machine learning, data manipulation, artificial intelligence, AI, unin, duality, duality-py, duality.py, vandal, vandal-py, vandal.py',
   packages = find_packages(),
   install_requires = [
-    'duality >= 4.8.2',
-    'logistics >= 0.0.11', 
     'colorama',
+    'logistics >= 0.0.15',
     'pandas >= 1.2.3',
     'numpy >= 1.19.5',
     'matplotlib >= 3.4.3',
     'openpyxl',
 ]
   )
```

### Comparing `vandal-3.8.9/vandal/__init__.py` & `vandal-4.0.0/vandal/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
             create_password(length) - creates a random password with adjustable lenght (default: length = 8).
 
             save_to(file, prefix, func_name, choice) - file saver for code clarity.
 
             file_handler(file) - handles the file extension upon import.
             
-            paint_text(text, color, print_trigger = True) - paints the text with a desired color ('r', 'g', 'b', 'k', 'c', 'm', 'y').
+            paint_text(text, color, print_trigger) - paints the text with a desired color ('Fr', 'Fg', 'Fb', 'Fk', 'Fc', 'Fm', 'Fy', 'Fw', 'Br', 'Bg', 'Bb', 'Bk', 'Bc', 'Bm', 'By', 'Bw').
 
     EXAMPLE (MODULE FUNCTIONS)
         --------------------------
 
         set of example functions to perform machine learning and data science operations over.
             print(help(any_function_listed_below)) in order to see the function details or print(help(vandal.example)) for all functions at once.
 
@@ -87,14 +87,16 @@
 # ignore __pycache__ from forming inside the library directory.
 import sys
 sys.dont_write_bytecode = True
 
 # colorama imports.
 from colorama import (
     Fore,
+    Back,
+    Style,
     init,
 )
 
 init()
 
 # meta data imports from the vandal library.
 from vandal.misc._meta import (
@@ -129,14 +131,16 @@
 )
 from vandal.objects.montecarlo import (
     MonteCarlo,
     MCapp,
 )
 from vandal.objects.dijkstra import Dijkstra
 
+from vandal.apps import montecarlo_gui
+
 # hub toolkit imports.
 from vandal.hub.toolkit import (
     random_value,
     random_pool,
     split_values,
     join_values,
     replace_values,
@@ -167,13 +171,14 @@
     'save_to',
     'paint_text',
     'toolkit',
     'example',
     'linear_regression',
     'MonteCarlo',
     'MCapp',
+    'MonteCarloGUI'
     'EOQ',
     'EOQapp',
     'Dijkstra',
     'VandalTypes',
     'Meta',
 ]
```

### Comparing `vandal-3.8.9/vandal/hub/example.py` & `vandal-4.0.0/vandal/hub/example.py`

 * *Files identical despite different names*

### Comparing `vandal-3.8.9/vandal/hub/toolkit.py` & `vandal-4.0.0/vandal/hub/toolkit.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # coloring.
 from colorama import (
-        Fore,
-        init,
+    Fore,
+    Back,
+    Style,
+    init,
 )
 
 init()
 
 # dependencies.
 import pandas as pd
 import os
@@ -37,15 +39,15 @@
 
 	create_password(length) - creates a random password with adjustable lenght (default: length = 8).
 
         save_to(file, prefix, func_name, choice) - file saver for code clarity.
 
         file_handler(file) - handles the file extenstion upon import.
         
-        paint_text(text, color, print_trigger = True) - paints the text with a desired color ('r', 'g', 'b', 'k', 'c', 'm', 'y').
+        paint_text(text, color, print_trigger) - paints the text with a desired color ('fr', 'fg', 'fb', 'fk', 'fc', 'fm', 'fy', 'br', 'bg', 'bb', 'bk', 'bc', 'bm', 'by').
 	
 '''
 
 # metadata of the used library.
 from vandal.misc._meta import (
 	__author__,
 	__copyright__,
@@ -184,23 +186,50 @@
         elif choice == '2' or choice == 'json':
                 extension = '.json'
                 file.to_json(prefix + func_name + extension)
                 print(Fore.YELLOW + os.path.join(os.getcwd() + '\\' + prefix + func_name + extension) + Fore.RESET)
         else:
                 print('=== NO OPTION CHOSEN, EXITING THE MENU... ===\n')
 
-#p aints the text with a desired color ('r', 'g', 'b', 'k', 'c', 'm', 'y').
-def paint_text(text, color, print_trigger = True):
-    colors = {'r': Fore.RED,
-              'g' : Fore.GREEN,
-              'b' : Fore.BLUE,
-              'k' : Fore.BLACK,
-              'm' : Fore.MAGENTA,
-              'y' : Fore.YELLOW,
-              'c' : Fore.CYAN,
-              }
-    
-    if print_trigger == True:
-        return print(colors[color] + text + Fore.RESET)
-    
-    elif print_trigger == False:
-        return colors[color] + text + Fore.RESET
+# >>> DEPRECATED AND MIGHT BE REMOVED IN THE FUTURE. THIS FUNCTION HAS BEEN MIGRATED TO THE LOGISTICS LIBRARY INSTEAD. <<<
+# paints the text with a desired color ('Fr', 'Fg', 'Fb', 'Fk', 'Fc', 'Fm', 'Fy', 'Fw', 'Br', 'Bg', 'Bb', 'Bk', 'Bc', 'Bm', 'By', 'Bw').
+def paint_text(
+        text : StringType,
+        color : StringType,
+        print_trigger : BooleanType = True
+        ) -> StringType:
+        
+        '''
+        * coloring of CLI.
+        
+        - text - desired text to print.
+        - color - desired color to print in.
+        - print_trigger (True/False) - modify return type.
+        '''
+        
+        # Fore coloring.
+        colors = {
+            'Fr' : Fore.RED,
+            'Fg' : Fore.GREEN,
+            'Fb' : Fore.BLUE,
+            'Fk' : Fore.BLACK,
+            'Fm' : Fore.MAGENTA,
+            'Fy' : Fore.YELLOW,
+            'Fc' : Fore.CYAN,
+            'Fw' : Fore.WHITE,
+            
+        # Back coloring.
+            'Br' : Back.RED,
+            'Bg' : Back.GREEN,
+            'Bb' : Back.BLUE,
+            'Bk' : Back.BLACK,
+            'Bm' : Back.MAGENTA,
+            'By' : Back.YELLOW,
+            'Bc' : Back.CYAN,
+            'Bw' : Back.WHITE,
+            }
+        
+        if print_trigger == True:
+            return print(colors[color] + str(text) + Style.RESET_ALL)
+        
+        elif print_trigger == False:
+            return colors[color] + str(text) + Style.RESET_ALL
```

### Comparing `vandal-3.8.9/vandal/misc/_meta.py` & `vandal-4.0.0/vandal/misc/_meta.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 
 __author__ = 'David Kundih'
 __copyright__ = 'Copyright © 2021-2022 David Kundih'
 __credits__ = [
 	'dkundih <https://github.com/dkundih>',
 
 ]
-__license__ = 'Copyright © 2021-2022 David Kundih. All rights reserved. Licensed under the Apache License, Version 2.0 | For more details about the license and terms of use visit the official vandal documentation linked at https://github.com/dkundih/vandal and https://pypi.org/project/vandal'
-__version__ = '3.8.9'
+__license__ = 'Copyright © 2021-2023 David Kundih. All rights reserved. Licensed under the Apache License, Version 2.0 | For more details about the license and terms of use visit the official vandal documentation linked at https://github.com/dkundih/vandal and https://pypi.org/project/vandal'
+__version__ = '4.0.0'
 __documentation__ = 'https://github.com/dkundih/vandal | https://pypi.org/project/vandal'
 __contact__ = 'dakundih@unin.hr | kundihdavid@gmail.com'
 __donate__ = 'https://patreon.com/dkundih | https://buymeacoffee.com/dkundih'
 __APPversion__ = 'v 1.4.4'
```

### Comparing `vandal-3.8.9/vandal/objects/dijkstra.py` & `vandal-4.0.0/vandal/objects/dijkstra.py`

 * *Files identical despite different names*

### Comparing `vandal-3.8.9/vandal/objects/eoq.py` & `vandal-4.0.0/vandal/objects/eoq.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # coloring.
 from colorama import (
     Fore,
+    Back,
+    Style,
     init,
-) 
+)
 
 init()
 
 # type hints and annotations.
 from logistics.plugins.metaclass import Meta
 
 # imports all data types.
```

### Comparing `vandal-3.8.9/vandal/objects/montecarlo.py` & `vandal-4.0.0/vandal/objects/montecarlo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # coloring.
 from colorama import (
     Fore,
+    Back,
+    Style,
     init,
-) 
+)
 
 init()
 
 # type hints and annotations.
 from logistics.plugins.metaclass import Meta
 
 # imports all data types.
```

### Comparing `vandal-3.8.9/vandal.egg-info/PKG-INFO` & `vandal-4.0.0/vandal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: vandal
-Version: 3.8.9
+Version: 4.0.0
 Summary: Data science, Data manipulation and Machine learning library.
 Home-page: http://github.com/dkundih/vandal
 Author: David Kundih
 Author-email: kundihdavid@gmail.com
 Maintainer: David Kundih
 Maintainer-email: kundihdavid@gmail.com
 License: Apache Software License
-Download-URL: https://github.com/dkundih/vandal/archive/refs/tags/v3.8.9.tar.gz
+Download-URL: https://github.com/dkundih/vandal/archive/refs/tags/v4.0.0.tar.gz
 Project-URL: Documentation, https://github.com/dkundih/vandal/blob/master/README.md
 Project-URL: Source Code, https://github.com/dkundih/vandal/tree/master/vandal
 Description: ![vandal-header](https://raw.githubusercontent.com/dkundih/vandal/master/_logistics/vandal.jpg)
         
         [![Downloads](https://img.shields.io/pypi/dm/vandal?color=F43&label=Downloads&style=flat-square)](https://pypi.org/project/vandal)
         [![License](https://img.shields.io/pypi/l/vandal?color=178&label=License&style=flat-square)](https://github.com/dkundih/vandal/blob/main/LICENSE)
         [![PyPi version](https://img.shields.io/pypi/v/vandal?color=178&&label=PyPi%20version&style=flat-square)](https://pypi.org/project/vandal)
@@ -137,19 +137,21 @@
         The library itself, it's maintenance, updates and stability, logo, videos, promotional materials and everything associated with duality are done by **David Kundih** from **Croatia**.
         
         <h1 align='center'> Hi! :wave:</h1>
          
         <img src='https://raw.githubusercontent.com/dkundih/dkundih/main/.logistics/BLUERED_GHiLI.jpg'/>
         
         <p align='center'>
-        My name is <b>David Kundih</b> and I am a Master's student of <b>Sustainable mobility and logistics</b> at the <b>University North</b>, currently specializing in <b>Digital transformation of traffic and logistics using Python.</b>
+        My name is <b>David Kundih</b> and I am a <b>Master of Engineering in Sustainable Mobility and Logistics</b>, currently specializing in <b>Digital Transformation of Traffic and Logistics using Python, JavaScript, HTML and CSS.</b>
         </p>
          
         <h4 align='center'>My latest projects:</h4>
         <p align='center'>
+        <a href="https://github.com/dkundih/promet-kc">promet-kc</p>
+        <p align='center'>
         <a href="https://github.com/dkundih/vandal">vandal</p>  
         <p align='center'>
         <a href="https://github.com/dkundih/duality">duality</p>  
         <p align='center'>
         <a href="https://github.com/dkundih/logistics">logistics</p>  
         <p align='center'>
         <a href="https://github.com/dkundih/unin">unin</a></p>
@@ -679,14 +681,26 @@
         
         3.8.8 (28/07/2022)
         - aligned to logistics changes.
         
         3.8.9 (07/08/2022)
         - paint_text added to toolkit.
         - now also inits colorama colors before other packages to avoid conflicts.
+        
+        3.8.10 (07/08/2022)
+        - changes to coloring policies.
+        - aligned paint_text to duality._paint_text changes.
+        
+        3.8.11 (13/08/2022)
+        - aligned to recent logistics and duality changes.
+        
+        4.0.0 (09/04/2023)
+        Hello everyone, I am back with great news after a few months:
+        - MonteCarlo now has a GUI. Call it as python -m vandal -e montecarlogui. It is in testing phase so stay patient.
+        
 Keywords: data science,machine learning,data manipulation,artificial intelligence,AI,unin,duality,duality-py,duality.py,vandal,vandal-py,vandal.py
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `vandal-3.8.9/vandal.egg-info/SOURCES.txt` & `vandal-4.0.0/vandal.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 README.md
 _upload.txt
 requirements.txt
 setup.py
 _deprecated/app/__init__.py
 _deprecated/app/particles.py
 _manifesto/Manifesto.md
-_testenv/F_montecarlo.py
 _testenv/GUI/GUIapp.py
 _testenv/pyscript/data.py
 vandal/__init__.py
 vandal/__main__.py
 vandal.egg-info/PKG-INFO
 vandal.egg-info/SOURCES.txt
 vandal.egg-info/dependency_links.txt
 vandal.egg-info/requires.txt
 vandal.egg-info/top_level.txt
+vandal/apps/__init__.py
+vandal/apps/montecarlo_gui.py
 vandal/hub/__init__.py
 vandal/hub/example.py
 vandal/hub/toolkit.py
 vandal/misc/__init__.py
 vandal/misc/_meta.py
 vandal/objects/__init__.py
 vandal/objects/dijkstra.py
```

