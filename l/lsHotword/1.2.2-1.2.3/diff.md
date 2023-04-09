# Comparing `tmp/lsHotword-1.2.2.tar.gz` & `tmp/lsHotword-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\lsHotword-1.2.2.tar", last modified: Wed Apr  5 18:01:19 2023, max compression
+gzip compressed data, was "dist\lsHotword-1.2.3.tar", last modified: Sun Apr  9 05:51:34 2023, max compression
```

## Comparing `lsHotword-1.2.2.tar` & `lsHotword-1.2.3.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 18:01:19.000000 lsHotword-1.2.2/
--rw-rw-rw-   0        0        0     1090 2023-04-02 19:52:59.000000 lsHotword-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     6517 2023-04-05 18:01:19.000000 lsHotword-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     6074 2023-04-05 17:59:50.000000 lsHotword-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 18:01:19.000000 lsHotword-1.2.2/lsHotword/
--rw-rw-rw-   0        0        0        0 2020-08-20 03:34:58.000000 lsHotword-1.2.2/lsHotword/__init__.py
--rw-rw-rw-   0        0        0   165476 2020-05-06 13:48:08.000000 lsHotword-1.2.2/lsHotword/chime.wav
--rw-rw-rw-   0        0        0    10018 2023-04-02 17:46:55.000000 lsHotword-1.2.2/lsHotword/funcHDatagen.py
--rw-rw-rw-   0        0        0     2154 2023-04-05 17:22:55.000000 lsHotword-1.2.2/lsHotword/funcHTrainer.py
--rw-rw-rw-   0        0        0    11194 2023-04-05 17:22:55.000000 lsHotword-1.2.2/lsHotword/funcHfTrainModel.py
--rw-rw-rw-   0        0        0    12616 2023-04-05 17:22:55.000000 lsHotword-1.2.2/lsHotword/hotword.py
--rw-rw-rw-   0        0        0     6013 2023-04-05 17:22:55.000000 lsHotword-1.2.2/lsHotword/ls.py
--rw-rw-rw-   0        0        0  1392640 2023-04-05 18:00:59.000000 lsHotword-1.2.2/lsHotword/lsrc.py
--rw-rw-rw-   0        0        0    33666 2023-04-05 17:22:55.000000 lsHotword-1.2.2/lsHotword/uitrainer.py
-drwxrwxrwx   0        0        0        0 2023-04-05 18:01:19.000000 lsHotword-1.2.2/lsHotword.egg-info/
--rw-rw-rw-   0        0        0     6517 2023-04-05 18:01:19.000000 lsHotword-1.2.2/lsHotword.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      438 2023-04-05 18:01:19.000000 lsHotword-1.2.2/lsHotword.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 18:01:19.000000 lsHotword-1.2.2/lsHotword.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      224 2023-04-05 18:01:19.000000 lsHotword-1.2.2/lsHotword.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       54 2023-04-05 18:01:19.000000 lsHotword-1.2.2/lsHotword.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-05 18:01:19.000000 lsHotword-1.2.2/lsHotword.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-05 18:01:19.000000 lsHotword-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1442 2023-04-05 18:00:52.000000 lsHotword-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:51:34.000000 lsHotword-1.2.3/
+-rw-rw-rw-   0        0        0     1090 2023-04-02 19:52:59.000000 lsHotword-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0     6517 2023-04-09 05:51:34.000000 lsHotword-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6074 2023-04-05 17:59:50.000000 lsHotword-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 05:51:34.000000 lsHotword-1.2.3/lsHotword/
+-rw-rw-rw-   0        0        0     9648 2023-04-06 09:21:35.000000 lsHotword-1.2.3/lsHotword/HDatagen.py
+-rw-rw-rw-   0        0        0     4248 2023-04-09 05:48:25.000000 lsHotword-1.2.3/lsHotword/HTrainer.py
+-rw-rw-rw-   0        0        0        0 2020-08-20 03:34:58.000000 lsHotword-1.2.3/lsHotword/__init__.py
+-rw-rw-rw-   0        0        0   165476 2020-05-06 13:48:08.000000 lsHotword-1.2.3/lsHotword/chime.wav
+-rw-rw-rw-   0        0        0    10018 2023-04-02 17:46:55.000000 lsHotword-1.2.3/lsHotword/funcHDatagen.py
+-rw-rw-rw-   0        0        0     2230 2023-04-09 05:45:59.000000 lsHotword-1.2.3/lsHotword/funcHTrainer.py
+-rw-rw-rw-   0        0        0    11270 2023-04-09 05:45:48.000000 lsHotword-1.2.3/lsHotword/funcHfTrainModel.py
+-rw-rw-rw-   0        0        0    12616 2023-04-05 17:22:55.000000 lsHotword-1.2.3/lsHotword/hotword.py
+-rw-rw-rw-   0        0        0     6013 2023-04-05 17:22:55.000000 lsHotword-1.2.3/lsHotword/ls.py
+-rw-rw-rw-   0        0        0  7579064 2023-04-05 17:22:55.000000 lsHotword-1.2.3/lsHotword/lsrc.py
+-rw-rw-rw-   0        0        0    33742 2023-04-09 05:48:16.000000 lsHotword-1.2.3/lsHotword/uitrainer.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:51:34.000000 lsHotword-1.2.3/lsHotword.egg-info/
+-rw-rw-rw-   0        0        0     6517 2023-04-09 05:51:34.000000 lsHotword-1.2.3/lsHotword.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-04-09 05:51:34.000000 lsHotword-1.2.3/lsHotword.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 05:51:34.000000 lsHotword-1.2.3/lsHotword.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      224 2023-04-09 05:51:34.000000 lsHotword-1.2.3/lsHotword.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       54 2023-04-09 05:51:34.000000 lsHotword-1.2.3/lsHotword.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-09 05:51:34.000000 lsHotword-1.2.3/lsHotword.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-09 05:51:34.000000 lsHotword-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1442 2023-04-09 05:50:08.000000 lsHotword-1.2.3/setup.py
```

### Comparing `lsHotword-1.2.2/LICENSE` & `lsHotword-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lsHotword-1.2.2/PKG-INFO` & `lsHotword-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsHotword
-Version: 1.2.2
+Version: 1.2.3
 Summary: Hotword/Wake Word detection in python for all platforms(Windows/Linux/Mac).
 Home-page: https://github.com/HemantKArya/lsHotword
 Download-URL: 
 Author: Hemant Kumar
 Author-email: iamhemantindia@protonmail.com
 License: MIT
 Keywords: hotword,detector,lshotword,windows,python,wake word,wake-word,detection
```

### Comparing `lsHotword-1.2.2/README.md` & `lsHotword-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `lsHotword-1.2.2/lsHotword/chime.wav` & `lsHotword-1.2.3/lsHotword/chime.wav`

 * *Files identical despite different names*

### Comparing `lsHotword-1.2.2/lsHotword/funcHDatagen.py` & `lsHotword-1.2.3/lsHotword/funcHDatagen.py`

 * *Files identical despite different names*

### Comparing `lsHotword-1.2.2/lsHotword/funcHTrainer.py` & `lsHotword-1.2.3/lsHotword/funcHTrainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 
 from numpy import load as npload
 from os import path
 print("lsHotwordTrainer")
 import argparse
 from sklearn.model_selection import train_test_split
-from tensorflow.keras.optimizers import Adam
+try:
+    from tensorflow.keras.optimizers.legacy import Adam
+except:
+    from tensorflow.keras.optimizers import Adam
 from . import hotword as ht
 
 
 
 
 def main():
     parser = argparse.ArgumentParser(description='Dir For Dataset e.g. neg an pos')
```

### Comparing `lsHotword-1.2.2/lsHotword/funcHfTrainModel.py` & `lsHotword-1.2.3/lsHotword/funcHfTrainModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from numpy.random import randint
 from numpy import zeros,array
 from numpy import save as npsave
 from pydub import AudioSegment
 import os
 from scipy.io import wavfile
-from tensorflow.keras.optimizers import Adam
+try:
+    from tensorflow.keras.optimizers.legacy import Adam
+except:
+    from tensorflow.keras.optimizers import Adam
 print("Full Hotword Data Generator and Trainer")
 import argparse
 from matplotlib.pyplot import specgram
 from sklearn.model_selection import train_test_split
 from . import hotword as ht
```

### Comparing `lsHotword-1.2.2/lsHotword/hotword.py` & `lsHotword-1.2.3/lsHotword/hotword.py`

 * *Files identical despite different names*

### Comparing `lsHotword-1.2.2/lsHotword/ls.py` & `lsHotword-1.2.3/lsHotword/ls.py`

 * *Files identical despite different names*

### Comparing `lsHotword-1.2.2/lsHotword/uitrainer.py` & `lsHotword-1.2.3/lsHotword/uitrainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 from numpy import zeros,array
 from numpy import save as npsave
 from pydub import AudioSegment
 import sys
 import os
 from scipy.io import wavfile
 from tensorflow.keras.callbacks import Callback
-from tensorflow.keras.optimizers import Adam
+try:
+    from tensorflow.keras.optimizers.legacy import Adam
+except:
+    from tensorflow.keras.optimizers import Adam
 print("Full Hotword Data Generator and Trainer")
 # import argparse
 from matplotlib.pyplot import specgram
 from sklearn.model_selection import train_test_split
 from . import hotword as ht
```

### Comparing `lsHotword-1.2.2/lsHotword.egg-info/PKG-INFO` & `lsHotword-1.2.3/lsHotword.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsHotword
-Version: 1.2.2
+Version: 1.2.3
 Summary: Hotword/Wake Word detection in python for all platforms(Windows/Linux/Mac).
 Home-page: https://github.com/HemantKArya/lsHotword
 Download-URL: 
 Author: Hemant Kumar
 Author-email: iamhemantindia@protonmail.com
 License: MIT
 Keywords: hotword,detector,lshotword,windows,python,wake word,wake-word,detection
```

### Comparing `lsHotword-1.2.2/setup.py` & `lsHotword-1.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 HERE = path.abspath(path.dirname(__file__))
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'lsHotword',
   packages = ['lsHotword'],
-  version = '1.2.2',
+  version = '1.2.3',
   license='MIT',
   include_package_data=True,
   long_description=long_description,
   long_description_content_type='text/markdown',
   description = 'Hotword/Wake Word detection in python for all platforms(Windows/Linux/Mac).',
   author = 'Hemant Kumar',
   author_email = 'iamhemantindia@protonmail.com',
```

