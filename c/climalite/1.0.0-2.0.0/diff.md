# Comparing `tmp/climalite-1.0.0.tar.gz` & `tmp/climalite-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climalite-1.0.0.tar", last modified: Sat Apr  8 23:00:43 2023, max compression
+gzip compressed data, was "climalite-2.0.0.tar", last modified: Sat Apr  8 23:17:21 2023, max compression
```

## Comparing `climalite-1.0.0.tar` & `climalite-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 michaelbitz   (501) staff       (20)        0 2023-04-08 23:00:43.522703 climalite-1.0.0/
--rw-r--r--   0 michaelbitz   (501) staff       (20)      623 2023-04-08 23:00:43.522268 climalite-1.0.0/PKG-INFO
-drwxr-xr-x   0 michaelbitz   (501) staff       (20)        0 2023-04-08 23:00:43.518192 climalite-1.0.0/climalite/
--rw-r--r--   0 michaelbitz   (501) staff       (20)       39 2023-04-08 22:47:03.000000 climalite-1.0.0/climalite/__init__.py
--rw-r--r--   0 michaelbitz   (501) staff       (20)     1666 2023-04-08 22:41:54.000000 climalite-1.0.0/climalite/climalite.py
-drwxr-xr-x   0 michaelbitz   (501) staff       (20)        0 2023-04-08 23:00:43.521500 climalite-1.0.0/climalite.egg-info/
--rw-r--r--   0 michaelbitz   (501) staff       (20)      623 2023-04-08 23:00:43.000000 climalite-1.0.0/climalite.egg-info/PKG-INFO
--rw-r--r--   0 michaelbitz   (501) staff       (20)      217 2023-04-08 23:00:43.000000 climalite-1.0.0/climalite.egg-info/SOURCES.txt
--rw-r--r--   0 michaelbitz   (501) staff       (20)        1 2023-04-08 23:00:43.000000 climalite-1.0.0/climalite.egg-info/dependency_links.txt
--rw-r--r--   0 michaelbitz   (501) staff       (20)        9 2023-04-08 23:00:43.000000 climalite-1.0.0/climalite.egg-info/requires.txt
--rw-r--r--   0 michaelbitz   (501) staff       (20)       10 2023-04-08 23:00:43.000000 climalite-1.0.0/climalite.egg-info/top_level.txt
--rw-r--r--   0 michaelbitz   (501) staff       (20)       38 2023-04-08 23:00:43.522863 climalite-1.0.0/setup.cfg
--rw-r--r--   0 michaelbitz   (501) staff       (20)      782 2023-04-08 22:56:27.000000 climalite-1.0.0/setup.py
+drwxr-xr-x   0 michaelbitz   (501) staff       (20)        0 2023-04-08 23:17:21.622331 climalite-2.0.0/
+-rw-r--r--   0 michaelbitz   (501) staff       (20)      623 2023-04-08 23:17:21.621827 climalite-2.0.0/PKG-INFO
+drwxr-xr-x   0 michaelbitz   (501) staff       (20)        0 2023-04-08 23:17:21.618239 climalite-2.0.0/climalite/
+-rw-r--r--   0 michaelbitz   (501) staff       (20)       39 2023-04-08 22:47:03.000000 climalite-2.0.0/climalite/__init__.py
+-rw-r--r--   0 michaelbitz   (501) staff       (20)     1781 2023-04-08 23:09:51.000000 climalite-2.0.0/climalite/climalite.py
+drwxr-xr-x   0 michaelbitz   (501) staff       (20)        0 2023-04-08 23:17:21.621103 climalite-2.0.0/climalite.egg-info/
+-rw-r--r--   0 michaelbitz   (501) staff       (20)      623 2023-04-08 23:17:21.000000 climalite-2.0.0/climalite.egg-info/PKG-INFO
+-rw-r--r--   0 michaelbitz   (501) staff       (20)      217 2023-04-08 23:17:21.000000 climalite-2.0.0/climalite.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelbitz   (501) staff       (20)        1 2023-04-08 23:17:21.000000 climalite-2.0.0/climalite.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelbitz   (501) staff       (20)        9 2023-04-08 23:17:21.000000 climalite-2.0.0/climalite.egg-info/requires.txt
+-rw-r--r--   0 michaelbitz   (501) staff       (20)       10 2023-04-08 23:17:21.000000 climalite-2.0.0/climalite.egg-info/top_level.txt
+-rw-r--r--   0 michaelbitz   (501) staff       (20)       38 2023-04-08 23:17:21.622511 climalite-2.0.0/setup.cfg
+-rw-r--r--   0 michaelbitz   (501) staff       (20)      782 2023-04-08 23:16:13.000000 climalite-2.0.0/setup.py
```

### Comparing `climalite-1.0.0/PKG-INFO` & `climalite-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climalite
-Version: 1.0.0
+Version: 2.0.0
 Summary: weather forcast data
 Home-page: https://github.com/Michael-Bitz/climalite
 Author-email: MichaelBitzDev@gmail.com
 License: MIT
 Keywords: weather,forecast,openweather
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `climalite-1.0.0/climalite/climalite.py` & `climalite-2.0.0/climalite/climalite.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,9 +37,12 @@
         """
         return self.data['list'][:4]
 
     def next_12h_simplified(self):
         data = self.next_12h()
         results = []
         for i in range(4):
-            results.append((data[i]['dt_txt'], data[i]['main']['temp'], data[i]['weather'][0]['description']))
+            results.append((data[i]['dt_txt'],
+                            data[i]['main']['temp'],
+                            data[i]['weather'][0]['description'],
+                            data[i]['weather'][0]['icon']))
         return results
```

### Comparing `climalite-1.0.0/climalite.egg-info/PKG-INFO` & `climalite-2.0.0/climalite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climalite
-Version: 1.0.0
+Version: 2.0.0
 Summary: weather forcast data
 Home-page: https://github.com/Michael-Bitz/climalite
 Author-email: MichaelBitzDev@gmail.com
 License: MIT
 Keywords: weather,forecast,openweather
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `climalite-1.0.0/setup.py` & `climalite-2.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='climalite',
     packages=['climalite'],
-    version='1.0.0',
+    version='2.0.0',
     license='MIT',
     description='weather forcast data',
     author_email='MichaelBitzDev@gmail.com',
     url='https://github.com/Michael-Bitz/climalite',
     keywords=['weather', 'forecast', 'openweather'],
     install_requires=[
         'requests',
```

