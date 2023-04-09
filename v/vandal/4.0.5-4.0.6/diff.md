# Comparing `tmp/vandal-4.0.5.tar.gz` & `tmp/vandal-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vandal-4.0.5.tar", last modified: Sun Apr  9 07:51:00 2023, max compression
+gzip compressed data, was "vandal-4.0.6.tar", last modified: Sun Apr  9 07:53:58 2023, max compression
```

## Comparing `vandal-4.0.5.tar` & `vandal-4.0.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 07:51:00.499905 vandal-4.0.5/
--rw-rw-rw-   0        0        0    14378 2023-04-09 07:47:16.000000 vandal-4.0.5/CHANGELOG.md
--rw-rw-rw-   0        0        0       30 2021-12-27 12:01:11.000000 vandal-4.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0    28951 2023-04-09 07:51:00.497903 vandal-4.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     6704 2023-04-09 07:50:35.000000 vandal-4.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 07:50:59.883906 vandal-4.0.5/_deprecated/
-drwxrwxrwx   0        0        0        0 2023-04-09 07:50:59.943905 vandal-4.0.5/_deprecated/app/
--rw-rw-rw-   0        0        0      286 2022-01-04 13:44:00.000000 vandal-4.0.5/_deprecated/app/__init__.py
--rw-rw-rw-   0        0        0     7353 2022-01-26 00:01:34.000000 vandal-4.0.5/_deprecated/app/particles.py
-drwxrwxrwx   0        0        0        0 2023-04-09 07:50:59.951906 vandal-4.0.5/_manifesto/
--rw-rw-rw-   0        0        0      527 2022-06-13 10:00:51.000000 vandal-4.0.5/_manifesto/Manifesto.md
-drwxrwxrwx   0        0        0        0 2023-04-09 07:50:59.889906 vandal-4.0.5/_testenv/
-drwxrwxrwx   0        0        0        0 2023-04-09 07:50:59.953906 vandal-4.0.5/_testenv/GUI/
--rw-rw-rw-   0        0        0      672 2022-06-07 08:33:58.000000 vandal-4.0.5/_testenv/GUI/GUIapp.py
-drwxrwxrwx   0        0        0        0 2023-04-09 07:50:59.956905 vandal-4.0.5/_testenv/pyscript/
--rw-rw-rw-   0        0        0       37 2022-06-05 23:46:06.000000 vandal-4.0.5/_testenv/pyscript/data.py
--rw-rw-rw-   0        0        0       75 2021-12-30 09:21:24.000000 vandal-4.0.5/_upload.txt
--rw-rw-rw-   0        0        0       94 2022-11-10 00:42:11.000000 vandal-4.0.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 07:51:00.500905 vandal-4.0.5/setup.cfg
--rw-rw-rw-   0        0        0     2651 2022-11-10 00:42:30.000000 vandal-4.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 07:50:59.962906 vandal-4.0.5/vandal/
--rw-rw-rw-   0        0        0     5976 2023-04-09 07:26:45.000000 vandal-4.0.5/vandal/__init__.py
--rw-rw-rw-   0        0        0     1238 2023-04-09 07:44:05.000000 vandal-4.0.5/vandal/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 07:51:00.282907 vandal-4.0.5/vandal/apps/
--rw-rw-rw-   0        0        0      307 2023-04-09 07:23:51.000000 vandal-4.0.5/vandal/apps/__init__.py
--rw-rw-rw-   0        0        0     5555 2023-04-09 07:47:09.000000 vandal-4.0.5/vandal/apps/montecarlo_gui.py
-drwxrwxrwx   0        0        0        0 2023-04-09 07:51:00.290904 vandal-4.0.5/vandal/hub/
--rw-rw-rw-   0        0        0      870 2022-08-07 13:51:39.000000 vandal-4.0.5/vandal/hub/__init__.py
--rw-rw-rw-   0        0        0     1006 2022-07-28 00:47:42.000000 vandal-4.0.5/vandal/hub/example.py
--rw-rw-rw-   0        0        0     8951 2022-08-22 21:06:18.000000 vandal-4.0.5/vandal/hub/toolkit.py
-drwxrwxrwx   0        0        0        0 2023-04-09 07:51:00.367904 vandal-4.0.5/vandal/misc/
--rw-rw-rw-   0        0        0      482 2022-02-09 00:26:37.000000 vandal-4.0.5/vandal/misc/__init__.py
--rw-rw-rw-   0        0        0      812 2023-04-09 07:50:53.000000 vandal-4.0.5/vandal/misc/_meta.py
-drwxrwxrwx   0        0        0        0 2023-04-09 07:51:00.495904 vandal-4.0.5/vandal/objects/
--rw-rw-rw-   0        0        0      506 2022-06-11 11:46:21.000000 vandal-4.0.5/vandal/objects/__init__.py
--rw-rw-rw-   0        0        0     4803 2022-06-11 11:46:31.000000 vandal-4.0.5/vandal/objects/dijkstra.py
--rw-rw-rw-   0        0        0     4851 2022-08-07 13:51:43.000000 vandal-4.0.5/vandal/objects/eoq.py
--rw-rw-rw-   0        0        0    21002 2022-08-07 13:51:48.000000 vandal-4.0.5/vandal/objects/montecarlo.py
-drwxrwxrwx   0        0        0        0 2023-04-09 07:51:00.180907 vandal-4.0.5/vandal.egg-info/
--rw-rw-rw-   0        0        0    28951 2023-04-09 07:50:59.000000 vandal-4.0.5/vandal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      660 2023-04-09 07:50:59.000000 vandal-4.0.5/vandal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 07:50:59.000000 vandal-4.0.5/vandal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2023-04-09 07:50:59.000000 vandal-4.0.5/vandal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-09 07:50:59.000000 vandal-4.0.5/vandal.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 07:53:58.702039 vandal-4.0.6/
+-rw-rw-rw-   0        0        0    14378 2023-04-09 07:53:41.000000 vandal-4.0.6/CHANGELOG.md
+-rw-rw-rw-   0        0        0       30 2021-12-27 12:01:11.000000 vandal-4.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    28951 2023-04-09 07:53:58.700039 vandal-4.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6704 2023-04-09 07:50:35.000000 vandal-4.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 07:53:58.278721 vandal-4.0.6/_deprecated/
+drwxrwxrwx   0        0        0        0 2023-04-09 07:53:58.365038 vandal-4.0.6/_deprecated/app/
+-rw-rw-rw-   0        0        0      286 2022-01-04 13:44:00.000000 vandal-4.0.6/_deprecated/app/__init__.py
+-rw-rw-rw-   0        0        0     7353 2022-01-26 00:01:34.000000 vandal-4.0.6/_deprecated/app/particles.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:53:58.367040 vandal-4.0.6/_manifesto/
+-rw-rw-rw-   0        0        0      527 2022-06-13 10:00:51.000000 vandal-4.0.6/_manifesto/Manifesto.md
+drwxrwxrwx   0        0        0        0 2023-04-09 07:53:58.290300 vandal-4.0.6/_testenv/
+drwxrwxrwx   0        0        0        0 2023-04-09 07:53:58.370108 vandal-4.0.6/_testenv/GUI/
+-rw-rw-rw-   0        0        0      672 2022-06-07 08:33:58.000000 vandal-4.0.6/_testenv/GUI/GUIapp.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:53:58.375039 vandal-4.0.6/_testenv/pyscript/
+-rw-rw-rw-   0        0        0       37 2022-06-05 23:46:06.000000 vandal-4.0.6/_testenv/pyscript/data.py
+-rw-rw-rw-   0        0        0       75 2021-12-30 09:21:24.000000 vandal-4.0.6/_upload.txt
+-rw-rw-rw-   0        0        0       94 2022-11-10 00:42:11.000000 vandal-4.0.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 07:53:58.703039 vandal-4.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2651 2022-11-10 00:42:30.000000 vandal-4.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:53:58.429037 vandal-4.0.6/vandal/
+-rw-rw-rw-   0        0        0     5976 2023-04-09 07:26:45.000000 vandal-4.0.6/vandal/__init__.py
+-rw-rw-rw-   0        0        0     1238 2023-04-09 07:53:44.000000 vandal-4.0.6/vandal/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:53:58.559039 vandal-4.0.6/vandal/apps/
+-rw-rw-rw-   0        0        0      307 2023-04-09 07:23:51.000000 vandal-4.0.6/vandal/apps/__init__.py
+-rw-rw-rw-   0        0        0     5537 2023-04-09 07:53:32.000000 vandal-4.0.6/vandal/apps/montecarlo_gui.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:53:58.600039 vandal-4.0.6/vandal/hub/
+-rw-rw-rw-   0        0        0      870 2022-08-07 13:51:39.000000 vandal-4.0.6/vandal/hub/__init__.py
+-rw-rw-rw-   0        0        0     1006 2022-07-28 00:47:42.000000 vandal-4.0.6/vandal/hub/example.py
+-rw-rw-rw-   0        0        0     8951 2022-08-22 21:06:18.000000 vandal-4.0.6/vandal/hub/toolkit.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:53:58.654036 vandal-4.0.6/vandal/misc/
+-rw-rw-rw-   0        0        0      482 2022-02-09 00:26:37.000000 vandal-4.0.6/vandal/misc/__init__.py
+-rw-rw-rw-   0        0        0      812 2023-04-09 07:53:51.000000 vandal-4.0.6/vandal/misc/_meta.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:53:58.695037 vandal-4.0.6/vandal/objects/
+-rw-rw-rw-   0        0        0      506 2022-06-11 11:46:21.000000 vandal-4.0.6/vandal/objects/__init__.py
+-rw-rw-rw-   0        0        0     4803 2022-06-11 11:46:31.000000 vandal-4.0.6/vandal/objects/dijkstra.py
+-rw-rw-rw-   0        0        0     4851 2022-08-07 13:51:43.000000 vandal-4.0.6/vandal/objects/eoq.py
+-rw-rw-rw-   0        0        0    21002 2022-08-07 13:51:48.000000 vandal-4.0.6/vandal/objects/montecarlo.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:53:58.555038 vandal-4.0.6/vandal.egg-info/
+-rw-rw-rw-   0        0        0    28951 2023-04-09 07:53:57.000000 vandal-4.0.6/vandal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      660 2023-04-09 07:53:58.000000 vandal-4.0.6/vandal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 07:53:57.000000 vandal-4.0.6/vandal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-04-09 07:53:57.000000 vandal-4.0.6/vandal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-09 07:53:57.000000 vandal-4.0.6/vandal.egg-info/top_level.txt
```

### Comparing `vandal-4.0.5/CHANGELOG.md` & `vandal-4.0.6/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -521,9 +521,9 @@
 3.8.11 (13/08/2022)
 - aligned to recent logistics and duality changes.
 
 4.0.0 (09/04/2023)
 Hello everyone, I am back with great news after a few months:
 - MonteCarlo now has a GUI. Call it as python -m vandal -e montecarlogui. It is in testing phase so stay patient.
 
-4.0.5 (09/04/2023)
+4.0.6 (09/04/2023)
 - Attempt on fixing GUI issues.
```

### Comparing `vandal-4.0.5/PKG-INFO` & `vandal-4.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: vandal
-Version: 4.0.5
+Version: 4.0.6
 Summary: Data science, Data manipulation and Machine learning library.
 Home-page: http://github.com/dkundih/vandal
 Author: David Kundih
 Author-email: kundihdavid@gmail.com
 Maintainer: David Kundih
 Maintainer-email: kundihdavid@gmail.com
 License: Apache Software License
-Download-URL: https://github.com/dkundih/vandal/archive/refs/tags/v4.0.5.tar.gz
+Download-URL: https://github.com/dkundih/vandal/archive/refs/tags/v4.0.6.tar.gz
 Project-URL: Documentation, https://github.com/dkundih/vandal/blob/master/README.md
 Project-URL: Source Code, https://github.com/dkundih/vandal/tree/master/vandal
 Description: ![vandal-header](https://raw.githubusercontent.com/dkundih/vandal/master/_logistics/vandal.jpg)
         
         [![Downloads](https://img.shields.io/pypi/dm/vandal?color=F43&label=Downloads&style=flat-square)](https://pypi.org/project/vandal)
         [![License](https://img.shields.io/pypi/l/vandal?color=178&label=License&style=flat-square)](https://github.com/dkundih/vandal/blob/main/LICENSE)
         [![PyPi version](https://img.shields.io/pypi/v/vandal?color=178&&label=PyPi%20version&style=flat-square)](https://pypi.org/project/vandal)
@@ -705,15 +705,15 @@
         3.8.11 (13/08/2022)
         - aligned to recent logistics and duality changes.
         
         4.0.0 (09/04/2023)
         Hello everyone, I am back with great news after a few months:
         - MonteCarlo now has a GUI. Call it as python -m vandal -e montecarlogui. It is in testing phase so stay patient.
         
-        4.0.5 (09/04/2023)
+        4.0.6 (09/04/2023)
         - Attempt on fixing GUI issues.
 Keywords: data science,machine learning,data manipulation,artificial intelligence,AI,unin,duality,duality-py,duality.py,vandal,vandal-py,vandal.py
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Customer Service
```

### Comparing `vandal-4.0.5/README.md` & `vandal-4.0.6/README.md`

 * *Files identical despite different names*

### Comparing `vandal-4.0.5/_deprecated/app/particles.py` & `vandal-4.0.6/_deprecated/app/particles.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.5/_manifesto/Manifesto.md` & `vandal-4.0.6/_manifesto/Manifesto.md`

 * *Files identical despite different names*

### Comparing `vandal-4.0.5/_testenv/GUI/GUIapp.py` & `vandal-4.0.6/_testenv/GUI/GUIapp.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.5/setup.py` & `vandal-4.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.5/vandal/__init__.py` & `vandal-4.0.6/vandal/__init__.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.5/vandal/__main__.py` & `vandal-4.0.6/vandal/__main__.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.5/vandal/apps/montecarlo_gui.py` & `vandal-4.0.6/vandal/apps/montecarlo_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,12 +120,10 @@
         except:
             tk.messagebox.showwarning(title="Warning", message="The input data must be in the first column of a document, each field containing one value. Column index can be of the type string, but it is advised that all values are of the type integer or float. Only .csv files are supported in the current version.")
             return
         plt.title('vandal (c) David Kundih, 2021-', fontsize=12, weight='regular', loc='right')
         plt.plot(MC)
         self.plot_canvas.draw()
 
-
-if __name__ == '__main__':
-    master = tk.Tk()
-    MonteCarloGUI(master)
-    master.mainloop()
+        master = tk.Tk()
+        MonteCarloGUI(master)
+        master.mainloop()
```

### Comparing `vandal-4.0.5/vandal/hub/__init__.py` & `vandal-4.0.6/vandal/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.5/vandal/hub/example.py` & `vandal-4.0.6/vandal/hub/example.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.5/vandal/hub/toolkit.py` & `vandal-4.0.6/vandal/hub/toolkit.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.5/vandal/misc/_meta.py` & `vandal-4.0.6/vandal/misc/_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 __author__ = 'David Kundih'
 __copyright__ = 'Copyright © 2021-2022 David Kundih'
 __credits__ = [
 	'dkundih <https://github.com/dkundih>',
 
 ]
 __license__ = 'Copyright © 2021-2023 David Kundih. All rights reserved. Licensed under the Apache License, Version 2.0 | For more details about the license and terms of use visit the official vandal documentation linked at https://github.com/dkundih/vandal and https://pypi.org/project/vandal'
-__version__ = '4.0.5'
+__version__ = '4.0.6'
 __documentation__ = 'https://github.com/dkundih/vandal | https://pypi.org/project/vandal'
 __contact__ = 'dakundih@unin.hr | kundihdavid@gmail.com'
 __donate__ = 'https://patreon.com/dkundih | https://buymeacoffee.com/dkundih'
 __APPversion__ = 'v 1.4.4'
```

### Comparing `vandal-4.0.5/vandal/objects/dijkstra.py` & `vandal-4.0.6/vandal/objects/dijkstra.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.5/vandal/objects/eoq.py` & `vandal-4.0.6/vandal/objects/eoq.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.5/vandal/objects/montecarlo.py` & `vandal-4.0.6/vandal/objects/montecarlo.py`

 * *Files identical despite different names*

### Comparing `vandal-4.0.5/vandal.egg-info/PKG-INFO` & `vandal-4.0.6/vandal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: vandal
-Version: 4.0.5
+Version: 4.0.6
 Summary: Data science, Data manipulation and Machine learning library.
 Home-page: http://github.com/dkundih/vandal
 Author: David Kundih
 Author-email: kundihdavid@gmail.com
 Maintainer: David Kundih
 Maintainer-email: kundihdavid@gmail.com
 License: Apache Software License
-Download-URL: https://github.com/dkundih/vandal/archive/refs/tags/v4.0.5.tar.gz
+Download-URL: https://github.com/dkundih/vandal/archive/refs/tags/v4.0.6.tar.gz
 Project-URL: Documentation, https://github.com/dkundih/vandal/blob/master/README.md
 Project-URL: Source Code, https://github.com/dkundih/vandal/tree/master/vandal
 Description: ![vandal-header](https://raw.githubusercontent.com/dkundih/vandal/master/_logistics/vandal.jpg)
         
         [![Downloads](https://img.shields.io/pypi/dm/vandal?color=F43&label=Downloads&style=flat-square)](https://pypi.org/project/vandal)
         [![License](https://img.shields.io/pypi/l/vandal?color=178&label=License&style=flat-square)](https://github.com/dkundih/vandal/blob/main/LICENSE)
         [![PyPi version](https://img.shields.io/pypi/v/vandal?color=178&&label=PyPi%20version&style=flat-square)](https://pypi.org/project/vandal)
@@ -705,15 +705,15 @@
         3.8.11 (13/08/2022)
         - aligned to recent logistics and duality changes.
         
         4.0.0 (09/04/2023)
         Hello everyone, I am back with great news after a few months:
         - MonteCarlo now has a GUI. Call it as python -m vandal -e montecarlogui. It is in testing phase so stay patient.
         
-        4.0.5 (09/04/2023)
+        4.0.6 (09/04/2023)
         - Attempt on fixing GUI issues.
 Keywords: data science,machine learning,data manipulation,artificial intelligence,AI,unin,duality,duality-py,duality.py,vandal,vandal-py,vandal.py
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Customer Service
```

### Comparing `vandal-4.0.5/vandal.egg-info/SOURCES.txt` & `vandal-4.0.6/vandal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

