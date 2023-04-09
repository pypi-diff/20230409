# Comparing `tmp/pyllicagram-1.7.tar.gz` & `tmp/pyllicagram-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyllicagram-1.7.tar", last modified: Sun Apr  9 16:49:29 2023, max compression
+gzip compressed data, was "dist/pyllicagram-1.7.1.tar", last modified: Sun Apr  9 16:59:56 2023, max compression
```

## Comparing `pyllicagram-1.7.tar` & `pyllicagram-1.7.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 16:49:29.373391 pyllicagram-1.7/
--rw-r--r--   0 benoit2c   (501) staff       (20)      274 2023-04-09 16:49:29.372666 pyllicagram-1.7/PKG-INFO
--rw-r--r--   0 benoit2c   (501) staff       (20)     4137 2023-04-09 16:45:51.000000 pyllicagram-1.7/README.md
--rw-r--r--   0 benoit2c   (501) staff       (20)       38 2023-04-09 16:49:29.373631 pyllicagram-1.7/setup.cfg
--rw-r--r--   0 benoit2c   (501) staff       (20)      404 2023-04-09 16:48:38.000000 pyllicagram-1.7/setup.py
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 16:49:29.368091 pyllicagram-1.7/src/
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 16:49:29.369439 pyllicagram-1.7/src/pyllicagram/
--rw-r--r--   0 benoit2c   (501) staff       (20)     2421 2023-04-09 16:45:51.000000 pyllicagram-1.7/src/pyllicagram/__init__.py
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 16:49:29.371902 pyllicagram-1.7/src/pyllicagram.egg-info/
--rw-r--r--   0 benoit2c   (501) staff       (20)      274 2023-04-09 16:49:29.000000 pyllicagram-1.7/src/pyllicagram.egg-info/PKG-INFO
--rw-r--r--   0 benoit2c   (501) staff       (20)      240 2023-04-09 16:49:29.000000 pyllicagram-1.7/src/pyllicagram.egg-info/SOURCES.txt
--rw-r--r--   0 benoit2c   (501) staff       (20)        1 2023-04-09 16:49:29.000000 pyllicagram-1.7/src/pyllicagram.egg-info/dependency_links.txt
--rw-r--r--   0 benoit2c   (501) staff       (20)        7 2023-04-09 16:49:29.000000 pyllicagram-1.7/src/pyllicagram.egg-info/requires.txt
--rw-r--r--   0 benoit2c   (501) staff       (20)       12 2023-04-09 16:49:29.000000 pyllicagram-1.7/src/pyllicagram.egg-info/top_level.txt
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 16:59:56.562337 pyllicagram-1.7.1/
+-rw-r--r--   0 benoit2c   (501) staff       (20)      276 2023-04-09 16:59:56.561539 pyllicagram-1.7.1/PKG-INFO
+-rw-r--r--   0 benoit2c   (501) staff       (20)     4137 2023-04-09 16:55:14.000000 pyllicagram-1.7.1/README.md
+-rw-r--r--   0 benoit2c   (501) staff       (20)       38 2023-04-09 16:59:56.562576 pyllicagram-1.7.1/setup.cfg
+-rw-r--r--   0 benoit2c   (501) staff       (20)      406 2023-04-09 16:59:36.000000 pyllicagram-1.7.1/setup.py
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 16:59:56.555961 pyllicagram-1.7.1/src/
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 16:59:56.557539 pyllicagram-1.7.1/src/pyllicagram/
+-rw-r--r--   0 benoit2c   (501) staff       (20)     2441 2023-04-09 16:59:17.000000 pyllicagram-1.7.1/src/pyllicagram/__init__.py
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 16:59:56.560705 pyllicagram-1.7.1/src/pyllicagram.egg-info/
+-rw-r--r--   0 benoit2c   (501) staff       (20)      276 2023-04-09 16:59:56.000000 pyllicagram-1.7.1/src/pyllicagram.egg-info/PKG-INFO
+-rw-r--r--   0 benoit2c   (501) staff       (20)      240 2023-04-09 16:59:56.000000 pyllicagram-1.7.1/src/pyllicagram.egg-info/SOURCES.txt
+-rw-r--r--   0 benoit2c   (501) staff       (20)        1 2023-04-09 16:59:56.000000 pyllicagram-1.7.1/src/pyllicagram.egg-info/dependency_links.txt
+-rw-r--r--   0 benoit2c   (501) staff       (20)        7 2023-04-09 16:59:56.000000 pyllicagram-1.7.1/src/pyllicagram.egg-info/requires.txt
+-rw-r--r--   0 benoit2c   (501) staff       (20)       12 2023-04-09 16:59:56.000000 pyllicagram-1.7.1/src/pyllicagram.egg-info/top_level.txt
```

### Comparing `pyllicagram-1.7/README.md` & `pyllicagram-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pyllicagram-1.7/src/pyllicagram/__init__.py` & `pyllicagram-1.7.1/src/pyllicagram/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import os
 import collections
 import ssl
 ssl._create_default_https_context = ssl._create_unverified_context
 # import pandas
 try:
         import pandas as pd
-        pd.read_csv(f"https://shiny.ens-paris-saclay.fr/guni/corpus=presse_test_from=1789_to=1950")
+        pd.read_csv(f"https://shiny.ens-paris-saclay.fr/guni/query?corpus=presse&mot=test&from=1789&to=1950")
         print(sys.executable)
 except:
         print("install pandas...")
         # install pandas as a subprocess if needed
         os.system(sys.executable + " -m pip install pandas")
         os.system(sys.executable + " " + " ".join(sys.argv))
         exit()
@@ -29,15 +29,15 @@
             raise ValueError("La recherche doit être une chaîne de caractères ou une liste")
         if not isinstance(recherche, list): recherche = [recherche]
         assert corpus in ["lemonde","livres","presse"], 'Vous devez choisir le corpus parmi "lemonde","livres" et "presse"'
         assert resolution in ["default","annee","mois"], 'Vous devez choisir la résolution parmi "default", "annee" ou "mois"'
         for gram in recherche:
                 gram = urllib.parse.quote_plus(gram.lower()).replace("-"," ").replace("+"," ")
                 gram = gram.replace(" ","%20")
-                df = pd.read_csv(f"https://shiny.ens-paris-saclay.fr/guni/corpus={corpus}_{gram}_from={debut}_to={fin}")
+                df = pd.read_csv(f"https://shiny.ens-paris-saclay.fr/guni/query?corpus={corpus}&mot={gram}&from={debut}&to={fin}")
                 if resolution=="mois" and corpus != "livres":
                         df = df.groupby(["annee","mois", "gram"]).agg({'n':'sum','total':'sum'}).reset_index()
                 if resolution=="annee":
                         df = df.groupby(["annee","gram"]).agg({'n':'sum','total':'sum'}).reset_index()
                 if 'result' in locals():
                         result = pd.concat([result, df])
                 else:
```

