# Comparing `tmp/bellek-0.7.6.tar.gz` & `tmp/bellek-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bellek-0.7.6.tar", last modified: Sun Apr  9 15:18:08 2023, max compression
+gzip compressed data, was "bellek-0.7.7.tar", last modified: Sun Apr  9 15:21:30 2023, max compression
```

## Comparing `bellek-0.7.6.tar` & `bellek-0.7.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2023-04-09 15:18:08.647697 bellek-0.7.6/
--rw-rw-r--   0 bdsaglam   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 bellek-0.7.6/LICENSE
--rw-rw-r--   0 bdsaglam   (501) staff       (20)      111 2022-09-05 16:31:43.000000 bellek-0.7.6/MANIFEST.in
--rw-r--r--   0 bdsaglam   (501) staff       (20)      887 2023-04-09 15:18:08.647154 bellek-0.7.6/PKG-INFO
--rw-r--r--   0 bdsaglam   (501) staff       (20)      128 2023-02-25 13:23:11.000000 bellek-0.7.6/README.md
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2023-04-09 15:18:08.632452 bellek-0.7.6/bellek/
--rw-r--r--   0 bdsaglam   (501) staff       (20)       22 2023-04-09 15:15:58.000000 bellek-0.7.6/bellek/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    17642 2023-04-09 15:16:03.000000 bellek-0.7.6/bellek/_modidx.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2023-04-09 15:18:08.646209 bellek-0.7.6/bellek/ml/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2023-04-09 15:15:58.000000 bellek-0.7.6/bellek/ml/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2225 2023-04-09 15:15:58.000000 bellek-0.7.6/bellek/ml/clip.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     8525 2023-04-09 15:15:58.000000 bellek-0.7.6/bellek/ml/cocoop.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    28983 2023-04-09 15:15:58.000000 bellek-0.7.6/bellek/ml/data.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3293 2023-04-09 15:15:58.000000 bellek-0.7.6/bellek/ml/evaluation.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2199 2023-04-09 15:15:58.000000 bellek-0.7.6/bellek/ml/experiment.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      711 2023-04-09 15:15:58.000000 bellek-0.7.6/bellek/ml/layer.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1718 2023-04-09 15:15:58.000000 bellek-0.7.6/bellek/ml/loss.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     9174 2023-04-09 15:15:58.000000 bellek-0.7.6/bellek/ml/mcd.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      939 2023-04-09 15:15:58.000000 bellek-0.7.6/bellek/ml/vision.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      539 2023-04-09 15:15:58.000000 bellek-0.7.6/bellek/testing.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2838 2023-04-09 15:15:58.000000 bellek-0.7.6/bellek/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2023-04-09 15:18:08.638113 bellek-0.7.6/bellek.egg-info/
--rw-r--r--   0 bdsaglam   (501) staff       (20)      887 2023-04-09 15:18:08.000000 bellek-0.7.6/bellek.egg-info/PKG-INFO
--rw-r--r--   0 bdsaglam   (501) staff       (20)      533 2023-04-09 15:18:08.000000 bellek-0.7.6/bellek.egg-info/SOURCES.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2023-04-09 15:18:08.000000 bellek-0.7.6/bellek.egg-info/dependency_links.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)       55 2023-04-09 15:18:08.000000 bellek-0.7.6/bellek.egg-info/entry_points.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2023-01-13 22:27:25.000000 bellek-0.7.6/bellek.egg-info/not-zip-safe
--rw-r--r--   0 bdsaglam   (501) staff       (20)      144 2023-04-09 15:18:08.000000 bellek-0.7.6/bellek.egg-info/requires.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        7 2023-04-09 15:18:08.000000 bellek-0.7.6/bellek.egg-info/top_level.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)      928 2023-04-09 15:15:28.000000 bellek-0.7.6/settings.ini
--rw-r--r--   0 bdsaglam   (501) staff       (20)       38 2023-04-09 15:18:08.647883 bellek-0.7.6/setup.cfg
--rw-rw-r--   0 bdsaglam   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 bellek-0.7.6/setup.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2023-04-09 15:21:30.910493 bellek-0.7.7/
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 bellek-0.7.7/LICENSE
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)      111 2022-09-05 16:31:43.000000 bellek-0.7.7/MANIFEST.in
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      887 2023-04-09 15:21:30.909985 bellek-0.7.7/PKG-INFO
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      128 2023-02-25 13:23:11.000000 bellek-0.7.7/README.md
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2023-04-09 15:21:30.898536 bellek-0.7.7/bellek/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       22 2023-04-09 15:21:18.000000 bellek-0.7.7/bellek/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    17642 2023-04-09 15:21:18.000000 bellek-0.7.7/bellek/_modidx.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2023-04-09 15:21:30.909105 bellek-0.7.7/bellek/ml/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2023-04-09 15:21:18.000000 bellek-0.7.7/bellek/ml/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2225 2023-04-09 15:21:18.000000 bellek-0.7.7/bellek/ml/clip.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     8525 2023-04-09 15:21:18.000000 bellek-0.7.7/bellek/ml/cocoop.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    28983 2023-04-09 15:21:18.000000 bellek-0.7.7/bellek/ml/data.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3293 2023-04-09 15:21:18.000000 bellek-0.7.7/bellek/ml/evaluation.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2199 2023-04-09 15:21:18.000000 bellek-0.7.7/bellek/ml/experiment.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      711 2023-04-09 15:21:18.000000 bellek-0.7.7/bellek/ml/layer.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1718 2023-04-09 15:21:18.000000 bellek-0.7.7/bellek/ml/loss.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     9174 2023-04-09 15:21:18.000000 bellek-0.7.7/bellek/ml/mcd.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      939 2023-04-09 15:21:18.000000 bellek-0.7.7/bellek/ml/vision.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      539 2023-04-09 15:21:18.000000 bellek-0.7.7/bellek/testing.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2838 2023-04-09 15:21:18.000000 bellek-0.7.7/bellek/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2023-04-09 15:21:30.903548 bellek-0.7.7/bellek.egg-info/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      887 2023-04-09 15:21:30.000000 bellek-0.7.7/bellek.egg-info/PKG-INFO
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      533 2023-04-09 15:21:30.000000 bellek-0.7.7/bellek.egg-info/SOURCES.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2023-04-09 15:21:30.000000 bellek-0.7.7/bellek.egg-info/dependency_links.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       55 2023-04-09 15:21:30.000000 bellek-0.7.7/bellek.egg-info/entry_points.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2023-01-13 22:27:25.000000 bellek-0.7.7/bellek.egg-info/not-zip-safe
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       99 2023-04-09 15:21:30.000000 bellek-0.7.7/bellek.egg-info/requires.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        7 2023-04-09 15:21:30.000000 bellek-0.7.7/bellek.egg-info/top_level.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      884 2023-04-09 15:21:05.000000 bellek-0.7.7/settings.ini
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       38 2023-04-09 15:21:30.910660 bellek-0.7.7/setup.cfg
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 bellek-0.7.7/setup.py
```

### Comparing `bellek-0.7.6/LICENSE` & `bellek-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bellek-0.7.6/PKG-INFO` & `bellek-0.7.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bellek
-Version: 0.7.6
+Version: 0.7.7
 Summary: My digital memory
 Home-page: https://github.com/bdsaglam/bellek
 Author: Barış Deniz Sağlam
 Author-email: bdsaglam@gmail.com
 License: Apache Software License 2.0
 Keywords: notebook
 Platform: UNKNOWN
```

### Comparing `bellek-0.7.6/bellek/_modidx.py` & `bellek-0.7.7/bellek/_modidx.py`

 * *Files identical despite different names*

### Comparing `bellek-0.7.6/bellek/ml/clip.py` & `bellek-0.7.7/bellek/ml/clip.py`

 * *Files identical despite different names*

### Comparing `bellek-0.7.6/bellek/ml/cocoop.py` & `bellek-0.7.7/bellek/ml/cocoop.py`

 * *Files identical despite different names*

### Comparing `bellek-0.7.6/bellek/ml/data.py` & `bellek-0.7.7/bellek/ml/data.py`

 * *Files identical despite different names*

### Comparing `bellek-0.7.6/bellek/ml/evaluation.py` & `bellek-0.7.7/bellek/ml/evaluation.py`

 * *Files identical despite different names*

### Comparing `bellek-0.7.6/bellek/ml/experiment.py` & `bellek-0.7.7/bellek/ml/experiment.py`

 * *Files identical despite different names*

### Comparing `bellek-0.7.6/bellek/ml/layer.py` & `bellek-0.7.7/bellek/ml/layer.py`

 * *Files identical despite different names*

### Comparing `bellek-0.7.6/bellek/ml/loss.py` & `bellek-0.7.7/bellek/ml/loss.py`

 * *Files identical despite different names*

### Comparing `bellek-0.7.6/bellek/ml/mcd.py` & `bellek-0.7.7/bellek/ml/mcd.py`

 * *Files identical despite different names*

### Comparing `bellek-0.7.6/bellek/ml/vision.py` & `bellek-0.7.7/bellek/ml/vision.py`

 * *Files identical despite different names*

### Comparing `bellek-0.7.6/bellek/testing.py` & `bellek-0.7.7/bellek/testing.py`

 * *Files identical despite different names*

### Comparing `bellek-0.7.6/bellek/utils.py` & `bellek-0.7.7/bellek/utils.py`

 * *Files identical despite different names*

### Comparing `bellek-0.7.6/bellek.egg-info/PKG-INFO` & `bellek-0.7.7/bellek.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bellek
-Version: 0.7.6
+Version: 0.7.7
 Summary: My digital memory
 Home-page: https://github.com/bdsaglam/bellek
 Author: Barış Deniz Sağlam
 Author-email: bdsaglam@gmail.com
 License: Apache Software License 2.0
 Keywords: notebook
 Platform: UNKNOWN
```

### Comparing `bellek-0.7.6/bellek.egg-info/SOURCES.txt` & `bellek-0.7.7/bellek.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bellek-0.7.6/settings.ini` & `bellek-0.7.7/settings.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = bellek
 lib_name = bellek
-version = 0.7.6
+version = 0.7.7
 min_python = 3.7
 license = apache2
 doc_path = _docs
 lib_path = bellek
 nbs_path = nbs
 recursive = True
 tst_flags = notest
@@ -21,15 +21,15 @@
 author_email = bdsaglam@gmail.com
 copyright = 2022 onwards, Barış Deniz Sağlam
 description = My digital memory
 keywords = notebook
 language = English
 status = 3
 user = bdsaglam
-requirements = numpy pandas fastai>=2.7.11 fastmtl>=1.2.0 clip@git+https://github.com/openai/CLIP.git
+requirements = numpy pandas fastai>=2.7.11 fastmtl>=1.2.0
 dev_requirements = nbdev jupyter twine pre-commit isort black wandb
 black_formatting = False
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
```

### Comparing `bellek-0.7.6/setup.py` & `bellek-0.7.7/setup.py`

 * *Files identical despite different names*

