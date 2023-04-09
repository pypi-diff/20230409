# Comparing `tmp/vandal-4.0.3.tar.gz` & `tmp/vandal-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vandal-4.0.3.tar", last modified: Sun Apr  9 07:40:27 2023, max compression
+gzip compressed data, was "vandal-4.0.4.tar", last modified: Sun Apr  9 07:42:49 2023, max compression
```

## Comparing `vandal-4.0.3.tar` & `vandal-4.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 07:40:27.561448 vandal-4.0.3/
--rw-rw-rw-   0        0        0    14378 2023-04-09 07:40:22.000000 vandal-4.0.3/CHANGELOG.md
--rw-rw-rw-   0        0        0       30 2021-12-27 12:01:11.000000 vandal-4.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0    28418 2023-04-09 07:40:27.559445 vandal-4.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6267 2022-10-11 15:31:44.000000 vandal-4.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 07:40:27.231302 vandal-4.0.3/_deprecated/
-drwxrwxrwx   0        0        0        0 2023-04-09 07:40:27.331303 vandal-4.0.3/_deprecated/app/
--rw-rw-rw-   0        0        0      286 2022-01-04 13:44:00.000000 vandal-4.0.3/_deprecated/app/__init__.py
--rw-rw-rw-   0        0        0     7353 2022-01-26 00:01:34.000000 vandal-4.0.3/_deprecated/app/particles.py
-drwxrwxrwx   0        0        0        0 2023-04-09 07:40:27.333305 vandal-4.0.3/_manifesto/
--rw-rw-rw-   0        0        0      527 2022-06-13 10:00:51.000000 vandal-4.0.3/_manifesto/Manifesto.md
-drwxrwxrwx   0        0        0        0 2023-04-09 07:40:27.255301 vandal-4.0.3/_testenv/
-drwxrwxrwx   0        0        0        0 2023-04-09 07:40:27.335303 vandal-4.0.3/_testenv/GUI/
--rw-rw-rw-   0        0        0      672 2022-06-07 08:33:58.000000 vandal-4.0.3/_testenv/GUI/GUIapp.py
-drwxrwxrwx   0        0        0        0 2023-04-09 07:40:27.337302 vandal-4.0.3/_testenv/pyscript/
--rw-rw-rw-   0        0        0       37 2022-06-05 23:46:06.000000 vandal-4.0.3/_testenv/pyscript/data.py
--rw-rw-rw-   0        0        0       75 2021-12-30 09:21:24.000000 vandal-4.0.3/_upload.txt
--rw-rw-rw-   0        0        0       94 2022-11-10 00:42:11.000000 vandal-4.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 07:40:27.561448 vandal-4.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2651 2022-11-10 00:42:30.000000 vandal-4.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 07:40:27.361301 vandal-4.0.3/vandal/
--rw-rw-rw-   0        0        0     5976 2023-04-09 07:26:45.000000 vandal-4.0.3/vandal/__init__.py
--rw-rw-rw-   0        0        0     1238 2023-04-09 07:26:22.000000 vandal-4.0.3/vandal/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 07:40:27.461446 vandal-4.0.3/vandal/apps/
--rw-rw-rw-   0        0        0      307 2023-04-09 07:23:51.000000 vandal-4.0.3/vandal/apps/__init__.py
--rw-rw-rw-   0        0        0     5941 2023-04-09 07:39:59.000000 vandal-4.0.3/vandal/apps/montecarlo_gui.py
-drwxrwxrwx   0        0        0        0 2023-04-09 07:40:27.468450 vandal-4.0.3/vandal/hub/
--rw-rw-rw-   0        0        0      870 2022-08-07 13:51:39.000000 vandal-4.0.3/vandal/hub/__init__.py
--rw-rw-rw-   0        0        0     1006 2022-07-28 00:47:42.000000 vandal-4.0.3/vandal/hub/example.py
--rw-rw-rw-   0        0        0     8951 2022-08-22 21:06:18.000000 vandal-4.0.3/vandal/hub/toolkit.py
-drwxrwxrwx   0        0        0        0 2023-04-09 07:40:27.474449 vandal-4.0.3/vandal/misc/
--rw-rw-rw-   0        0        0      482 2022-02-09 00:26:37.000000 vandal-4.0.3/vandal/misc/__init__.py
--rw-rw-rw-   0        0        0      812 2023-04-09 07:40:17.000000 vandal-4.0.3/vandal/misc/_meta.py
-drwxrwxrwx   0        0        0        0 2023-04-09 07:40:27.557448 vandal-4.0.3/vandal/objects/
--rw-rw-rw-   0        0        0      506 2022-06-11 11:46:21.000000 vandal-4.0.3/vandal/objects/__init__.py
--rw-rw-rw-   0        0        0     4803 2022-06-11 11:46:31.000000 vandal-4.0.3/vandal/objects/dijkstra.py
--rw-rw-rw-   0        0        0     4851 2022-08-07 13:51:43.000000 vandal-4.0.3/vandal/objects/eoq.py
--rw-rw-rw-   0        0        0    21002 2022-08-07 13:51:48.000000 vandal-4.0.3/vandal/objects/montecarlo.py
-drwxrwxrwx   0        0        0        0 2023-04-09 07:40:27.434449 vandal-4.0.3/vandal.egg-info/
--rw-rw-rw-   0        0        0    28418 2023-04-09 07:40:26.000000 vandal-4.0.3/vandal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      660 2023-04-09 07:40:27.000000 vandal-4.0.3/vandal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 07:40:26.000000 vandal-4.0.3/vandal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-04-09 07:40:26.000000 vandal-4.0.3/vandal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-09 07:40:26.000000 vandal-4.0.3/vandal.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 07:42:49.967396 vandal-4.0.4/
+-rw-rw-rw-   0        0        0    14378 2023-04-09 07:42:16.000000 vandal-4.0.4/CHANGELOG.md
+-rw-rw-rw-   0        0        0       30 2021-12-27 12:01:11.000000 vandal-4.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    28418 2023-04-09 07:42:49.955392 vandal-4.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6267 2022-10-11 15:31:44.000000 vandal-4.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 07:42:49.729339 vandal-4.0.4/_deprecated/
+drwxrwxrwx   0        0        0        0 2023-04-09 07:42:49.792336 vandal-4.0.4/_deprecated/app/
+-rw-rw-rw-   0        0        0      286 2022-01-04 13:44:00.000000 vandal-4.0.4/_deprecated/app/__init__.py
+-rw-rw-rw-   0        0        0     7353 2022-01-26 00:01:34.000000 vandal-4.0.4/_deprecated/app/particles.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:42:49.795336 vandal-4.0.4/_manifesto/
+-rw-rw-rw-   0        0        0      527 2022-06-13 10:00:51.000000 vandal-4.0.4/_manifesto/Manifesto.md
+drwxrwxrwx   0        0        0        0 2023-04-09 07:42:49.735340 vandal-4.0.4/_testenv/
+drwxrwxrwx   0        0        0        0 2023-04-09 07:42:49.806338 vandal-4.0.4/_testenv/GUI/
+-rw-rw-rw-   0        0        0      672 2022-06-07 08:33:58.000000 vandal-4.0.4/_testenv/GUI/GUIapp.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:42:49.837396 vandal-4.0.4/_testenv/pyscript/
+-rw-rw-rw-   0        0        0       37 2022-06-05 23:46:06.000000 vandal-4.0.4/_testenv/pyscript/data.py
+-rw-rw-rw-   0        0        0       75 2021-12-30 09:21:24.000000 vandal-4.0.4/_upload.txt
+-rw-rw-rw-   0        0        0       94 2022-11-10 00:42:11.000000 vandal-4.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 07:42:49.968395 vandal-4.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2651 2022-11-10 00:42:30.000000 vandal-4.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:42:49.855395 vandal-4.0.4/vandal/
+-rw-rw-rw-   0        0        0     5976 2023-04-09 07:26:45.000000 vandal-4.0.4/vandal/__init__.py
+-rw-rw-rw-   0        0        0     1224 2023-04-09 07:42:07.000000 vandal-4.0.4/vandal/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:42:49.905393 vandal-4.0.4/vandal/apps/
+-rw-rw-rw-   0        0        0      307 2023-04-09 07:23:51.000000 vandal-4.0.4/vandal/apps/__init__.py
+-rw-rw-rw-   0        0        0     5941 2023-04-09 07:39:59.000000 vandal-4.0.4/vandal/apps/montecarlo_gui.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:42:49.914395 vandal-4.0.4/vandal/hub/
+-rw-rw-rw-   0        0        0      870 2022-08-07 13:51:39.000000 vandal-4.0.4/vandal/hub/__init__.py
+-rw-rw-rw-   0        0        0     1006 2022-07-28 00:47:42.000000 vandal-4.0.4/vandal/hub/example.py
+-rw-rw-rw-   0        0        0     8951 2022-08-22 21:06:18.000000 vandal-4.0.4/vandal/hub/toolkit.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:42:49.919448 vandal-4.0.4/vandal/misc/
+-rw-rw-rw-   0        0        0      482 2022-02-09 00:26:37.000000 vandal-4.0.4/vandal/misc/__init__.py
+-rw-rw-rw-   0        0        0      812 2023-04-09 07:42:34.000000 vandal-4.0.4/vandal/misc/_meta.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:42:49.951393 vandal-4.0.4/vandal/objects/
+-rw-rw-rw-   0        0        0      506 2022-06-11 11:46:21.000000 vandal-4.0.4/vandal/objects/__init__.py
+-rw-rw-rw-   0        0        0     4803 2022-06-11 11:46:31.000000 vandal-4.0.4/vandal/objects/dijkstra.py
+-rw-rw-rw-   0        0        0     4851 2022-08-07 13:51:43.000000 vandal-4.0.4/vandal/objects/eoq.py
+-rw-rw-rw-   0        0        0    21002 2022-08-07 13:51:48.000000 vandal-4.0.4/vandal/objects/montecarlo.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:42:49.899393 vandal-4.0.4/vandal.egg-info/
+-rw-rw-rw-   0        0        0    28418 2023-04-09 07:42:49.000000 vandal-4.0.4/vandal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      660 2023-04-09 07:42:49.000000 vandal-4.0.4/vandal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 07:42:49.000000 vandal-4.0.4/vandal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-04-09 07:42:49.000000 vandal-4.0.4/vandal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-09 07:42:49.000000 vandal-4.0.4/vandal.egg-info/top_level.txt
```

### Comparing `vandal-4.0.3/CHANGELOG.md` & `vandal-4.0.4/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -521,9 +521,9 @@
 3.8.11 (13/08/2022)
 - aligned to recent logistics and duality changes.
 
 4.0.0 (09/04/2023)
 Hello everyone, I am back with great news after a few months:
 - MonteCarlo now has a GUI. Call it as python -m vandal -e montecarlogui. It is in testing phase so stay patient.
 
-4.0.3 (09/04/2023)
+4.0.4 (09/04/2023)
 - Attempt on fixing GUI issues.
```

### Comparing `vandal-4.0.3/PKG-INFO` & `vandal-4.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: vandal
-Version: 4.0.3
+Version: 4.0.4
 Summary: Data science, Data manipulation and Machine learning library.
 Home-page: http://github.com/dkundih/vandal
 Author: David Kundih
 Author-email: kundihdavid@gmail.com
 Maintainer: David Kundih
 Maintainer-email: kundihdavid@gmail.com
 License: Apache Software License
-Download-URL: https://github.com/dkundih/vandal/archive/refs/tags/v4.0.3.tar.gz
+Download-URL: https://github.com/dkundih/vandal/archive/refs/tags/v4.0.4.tar.gz
 Project-URL: Documentation, https://github.com/dkundih/vandal/blob/master/README.md
 Project-URL: Source Code, https://github.com/dkundih/vandal/tree/master/vandal
 Description: ![vandal-header](https://raw.githubusercontent.com/dkundih/vandal/master/_logistics/vandal.jpg)
         
         [![Downloads](https://img.shields.io/pypi/dm/vandal?color=F43&label=Downloads&style=flat-square)](https://pypi.org/project/vandal)
         [![License](https://img.shields.io/pypi/l/vandal?color=178&label=License&style=flat-square)](https://github.com/dkundih/vandal/blob/main/LICENSE)
         [![PyPi version](https://img.shields.io/pypi/v/vandal?color=178&&label=PyPi%20version&style=flat-square)](https://pypi.org/project/vandal)
@@ -693,15 +693,15 @@
         3.8.11 (13/08/2022)
         - aligned to recent logistics and duality changes.
         
         4.0.0 (09/04/2023)
         Hello everyone, I am back with great news after a few months:
         - MonteCarlo now has a GUI. Call it as python -m vandal -e montecarlogui. It is in testing phase so stay patient.
         
-        4.0.3 (09/04/2023)
+        4.0.4 (09/04/2023)
         - Attempt on fixing GUI issues.
 Keywords: data science,machine learning,data manipulation,artificial intelligence,AI,unin,duality,duality-py,duality.py,vandal,vandal-py,vandal.py
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Customer Service
```

### Comparing `vandal-4.0.3/README.md` & `vandal-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `vandal-4.0.3/_deprecated/app/particles.py` & `vandal-4.0.4/_deprecated/app/particles.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.3/_manifesto/Manifesto.md` & `vandal-4.0.4/_manifesto/Manifesto.md`

 * *Files identical despite different names*

### Comparing `vandal-4.0.3/_testenv/GUI/GUIapp.py` & `vandal-4.0.4/_testenv/GUI/GUIapp.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.3/setup.py` & `vandal-4.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.3/vandal/__init__.py` & `vandal-4.0.4/vandal/__init__.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.3/vandal/__main__.py` & `vandal-4.0.4/vandal/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,8 +36,8 @@
         print(Fore.YELLOW + '=== ENTERING MONTECARLO CLIENT... ===\n', Fore.RESET)
         vandal.objects.montecarlo.MCapp()
     elif args.entry == 'eoq':
         print(Fore.YELLOW + '=== ENTERING ECONOMIC ORDER QUANTITY CLIENT... ===\n', Fore.RESET)
         vandal.objects.eoq.EOQapp()
     elif args.entry == 'montecarlogui':
         print(Fore.YELLOW + '=== ENTERING MONTECARLO GUI... ===\n', Fore.RESET)
-        vandal.apps.montecarlo_gui.MonteCarloGUI()
+        vandal.apps.montecarlo_gui()
```

### Comparing `vandal-4.0.3/vandal/apps/montecarlo_gui.py` & `vandal-4.0.4/vandal/apps/montecarlo_gui.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.3/vandal/hub/__init__.py` & `vandal-4.0.4/vandal/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.3/vandal/hub/example.py` & `vandal-4.0.4/vandal/hub/example.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.3/vandal/hub/toolkit.py` & `vandal-4.0.4/vandal/hub/toolkit.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.3/vandal/misc/_meta.py` & `vandal-4.0.4/vandal/misc/_meta.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 __author__ = 'David Kundih'
 __copyright__ = 'Copyright © 2021-2022 David Kundih'
 __credits__ = [
 	'dkundih <https://github.com/dkundih>',
 
 ]
 __license__ = 'Copyright © 2021-2023 David Kundih. All rights reserved. Licensed under the Apache License, Version 2.0 | For more details about the license and terms of use visit the official vandal documentation linked at https://github.com/dkundih/vandal and https://pypi.org/project/vandal'
-__version__ = '4.0.3'
+__version__ = '4.0.4'
 __documentation__ = 'https://github.com/dkundih/vandal | https://pypi.org/project/vandal'
 __contact__ = 'dakundih@unin.hr | kundihdavid@gmail.com'
 __donate__ = 'https://patreon.com/dkundih | https://buymeacoffee.com/dkundih'
 __APPversion__ = 'v 1.4.4'
```

### Comparing `vandal-4.0.3/vandal/objects/dijkstra.py` & `vandal-4.0.4/vandal/objects/dijkstra.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.3/vandal/objects/eoq.py` & `vandal-4.0.4/vandal/objects/eoq.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.3/vandal/objects/montecarlo.py` & `vandal-4.0.4/vandal/objects/montecarlo.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.3/vandal.egg-info/PKG-INFO` & `vandal-4.0.4/vandal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: vandal
-Version: 4.0.3
+Version: 4.0.4
 Summary: Data science, Data manipulation and Machine learning library.
 Home-page: http://github.com/dkundih/vandal
 Author: David Kundih
 Author-email: kundihdavid@gmail.com
 Maintainer: David Kundih
 Maintainer-email: kundihdavid@gmail.com
 License: Apache Software License
-Download-URL: https://github.com/dkundih/vandal/archive/refs/tags/v4.0.3.tar.gz
+Download-URL: https://github.com/dkundih/vandal/archive/refs/tags/v4.0.4.tar.gz
 Project-URL: Documentation, https://github.com/dkundih/vandal/blob/master/README.md
 Project-URL: Source Code, https://github.com/dkundih/vandal/tree/master/vandal
 Description: ![vandal-header](https://raw.githubusercontent.com/dkundih/vandal/master/_logistics/vandal.jpg)
         
         [![Downloads](https://img.shields.io/pypi/dm/vandal?color=F43&label=Downloads&style=flat-square)](https://pypi.org/project/vandal)
         [![License](https://img.shields.io/pypi/l/vandal?color=178&label=License&style=flat-square)](https://github.com/dkundih/vandal/blob/main/LICENSE)
         [![PyPi version](https://img.shields.io/pypi/v/vandal?color=178&&label=PyPi%20version&style=flat-square)](https://pypi.org/project/vandal)
@@ -693,15 +693,15 @@
         3.8.11 (13/08/2022)
         - aligned to recent logistics and duality changes.
         
         4.0.0 (09/04/2023)
         Hello everyone, I am back with great news after a few months:
         - MonteCarlo now has a GUI. Call it as python -m vandal -e montecarlogui. It is in testing phase so stay patient.
         
-        4.0.3 (09/04/2023)
+        4.0.4 (09/04/2023)
         - Attempt on fixing GUI issues.
 Keywords: data science,machine learning,data manipulation,artificial intelligence,AI,unin,duality,duality-py,duality.py,vandal,vandal-py,vandal.py
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Customer Service
```

### Comparing `vandal-4.0.3/vandal.egg-info/SOURCES.txt` & `vandal-4.0.4/vandal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

