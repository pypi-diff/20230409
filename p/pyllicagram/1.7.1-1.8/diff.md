# Comparing `tmp/pyllicagram-1.7.1.tar.gz` & `tmp/pyllicagram-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyllicagram-1.7.1.tar", last modified: Sun Apr  9 16:59:56 2023, max compression
+gzip compressed data, was "dist/pyllicagram-1.8.tar", last modified: Sun Apr  9 17:53:57 2023, max compression
```

## Comparing `pyllicagram-1.7.1.tar` & `pyllicagram-1.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 16:59:56.562337 pyllicagram-1.7.1/
--rw-r--r--   0 benoit2c   (501) staff       (20)      276 2023-04-09 16:59:56.561539 pyllicagram-1.7.1/PKG-INFO
--rw-r--r--   0 benoit2c   (501) staff       (20)     4137 2023-04-09 16:55:14.000000 pyllicagram-1.7.1/README.md
--rw-r--r--   0 benoit2c   (501) staff       (20)       38 2023-04-09 16:59:56.562576 pyllicagram-1.7.1/setup.cfg
--rw-r--r--   0 benoit2c   (501) staff       (20)      406 2023-04-09 16:59:36.000000 pyllicagram-1.7.1/setup.py
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 16:59:56.555961 pyllicagram-1.7.1/src/
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 16:59:56.557539 pyllicagram-1.7.1/src/pyllicagram/
--rw-r--r--   0 benoit2c   (501) staff       (20)     2441 2023-04-09 16:59:17.000000 pyllicagram-1.7.1/src/pyllicagram/__init__.py
-drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 16:59:56.560705 pyllicagram-1.7.1/src/pyllicagram.egg-info/
--rw-r--r--   0 benoit2c   (501) staff       (20)      276 2023-04-09 16:59:56.000000 pyllicagram-1.7.1/src/pyllicagram.egg-info/PKG-INFO
--rw-r--r--   0 benoit2c   (501) staff       (20)      240 2023-04-09 16:59:56.000000 pyllicagram-1.7.1/src/pyllicagram.egg-info/SOURCES.txt
--rw-r--r--   0 benoit2c   (501) staff       (20)        1 2023-04-09 16:59:56.000000 pyllicagram-1.7.1/src/pyllicagram.egg-info/dependency_links.txt
--rw-r--r--   0 benoit2c   (501) staff       (20)        7 2023-04-09 16:59:56.000000 pyllicagram-1.7.1/src/pyllicagram.egg-info/requires.txt
--rw-r--r--   0 benoit2c   (501) staff       (20)       12 2023-04-09 16:59:56.000000 pyllicagram-1.7.1/src/pyllicagram.egg-info/top_level.txt
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 17:53:57.188885 pyllicagram-1.8/
+-rw-r--r--   0 benoit2c   (501) staff       (20)      274 2023-04-09 17:53:57.187823 pyllicagram-1.8/PKG-INFO
+-rw-r--r--   0 benoit2c   (501) staff       (20)     4137 2023-04-09 17:19:41.000000 pyllicagram-1.8/README.md
+-rw-r--r--   0 benoit2c   (501) staff       (20)       38 2023-04-09 17:53:57.189208 pyllicagram-1.8/setup.cfg
+-rw-r--r--   0 benoit2c   (501) staff       (20)      404 2023-04-09 17:53:30.000000 pyllicagram-1.8/setup.py
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 17:53:57.179420 pyllicagram-1.8/src/
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 17:53:57.182776 pyllicagram-1.8/src/pyllicagram/
+-rw-r--r--   0 benoit2c   (501) staff       (20)     3703 2023-04-09 17:53:18.000000 pyllicagram-1.8/src/pyllicagram/__init__.py
+-rw-r--r--   0 benoit2c   (501) staff       (20)      612 2023-04-09 17:37:23.000000 pyllicagram-1.8/src/pyllicagram/joker.py
+drwxr-xr-x   0 benoit2c   (501) staff       (20)        0 2023-04-09 17:53:57.186841 pyllicagram-1.8/src/pyllicagram.egg-info/
+-rw-r--r--   0 benoit2c   (501) staff       (20)      274 2023-04-09 17:53:57.000000 pyllicagram-1.8/src/pyllicagram.egg-info/PKG-INFO
+-rw-r--r--   0 benoit2c   (501) staff       (20)      265 2023-04-09 17:53:57.000000 pyllicagram-1.8/src/pyllicagram.egg-info/SOURCES.txt
+-rw-r--r--   0 benoit2c   (501) staff       (20)        1 2023-04-09 17:53:57.000000 pyllicagram-1.8/src/pyllicagram.egg-info/dependency_links.txt
+-rw-r--r--   0 benoit2c   (501) staff       (20)        7 2023-04-09 17:53:57.000000 pyllicagram-1.8/src/pyllicagram.egg-info/requires.txt
+-rw-r--r--   0 benoit2c   (501) staff       (20)       12 2023-04-09 17:53:57.000000 pyllicagram-1.8/src/pyllicagram.egg-info/top_level.txt
```

### Comparing `pyllicagram-1.7.1/README.md` & `pyllicagram-1.8/README.md`

 * *Files identical despite different names*

### Comparing `pyllicagram-1.7.1/src/pyllicagram/__init__.py` & `pyllicagram-1.8/src/pyllicagram/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -43,7 +43,26 @@
                 else:
                         result = df
         if somme:
                 result = result.groupby(["annee",*(("mois",) if "mois" in result.columns else()),*(("jour",) if 'jour' in result.columns else())]).agg({'n':'sum','total':'mean'}).reset_index()
                 result["gram"] = "+".join(recherche)
         result["ratio"] = result.n.values/result.total.values
         return result
+
+
+def joker(gram,corpus="presse",debut=1789,fin=1950,after=True,n_joker=20):
+    if not isinstance(gram, str) and not isinstance(gram, list):
+            raise ValueError("La recherche doit être une chaîne de caractères ou une liste")
+    assert corpus in ["lemonde","livres","presse"], 'Vous devez choisir le corpus parmi "lemonde","livres" et "presse"'
+    gram = urllib.parse.quote_plus(gram.lower()).replace("-"," ").replace(" ","%20")
+    df = pd.read_csv(f"https://shiny.ens-paris-saclay.fr/guni/joker?corpus={corpus}&mot={gram}&from={debut}&to={fin}&after={after}&n_joker={n_joker}")
+    return df 
+
+
+def contain(mot1,mot2,corpus="presse",debut=1789,fin=1950):
+    if not isinstance(mot1,str) or not isinstance(mot2,str):
+        raise ValueError("La recherche doit être une chaîne de caractères ou une liste")
+    assert corpus in ["lemonde","livres","presse"], 'Vous devez choisir le corpus parmi "lemonde","livres" et "presse"'
+    mot1 = urllib.parse.quote_plus(mot1.lower()).replace("-"," ").replace(" ","%20")
+    mot2 = urllib.parse.quote_plus(mot2.lower()).replace("-"," ").replace(" ","%20")
+    df = pd.read_csv(f"https://shiny.ens-paris-saclay.fr/guni/contain?corpus={corpus}&mot1={mot1}&mot2={mot2}&from={debut}&to={fin}")
+    return df
```

