# Comparing `tmp/famouscipheralgorithms-0.1.3.tar.gz` & `tmp/famouscipheralgorithms-0.1.4.tar.gz`

## Comparing `famouscipheralgorithms-0.1.3.tar` & `famouscipheralgorithms-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,18 @@
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/setup.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/FamousCipherAlgorithms/Affine.py
--rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/FamousCipherAlgorithms/Hill.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/FamousCipherAlgorithms/Permutation.py
--rw-r--r--   0        0        0     6292 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/FamousCipherAlgorithms/Playfair.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/FamousCipherAlgorithms/RailFence.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/FamousCipherAlgorithms/Shift.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/FamousCipherAlgorithms/Vigenere.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/FamousCipherAlgorithms/__init__.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/FamousCipherAlgorithms.egg-info/PKG-INFO
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/FamousCipherAlgorithms.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/FamousCipherAlgorithms.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/FamousCipherAlgorithms.egg-info/top_level.txt
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/build/lib/FamousCipherAlgorithms/Affine.py
--rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/build/lib/FamousCipherAlgorithms/Hill.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/build/lib/FamousCipherAlgorithms/Permutation.py
--rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/build/lib/FamousCipherAlgorithms/Playfair.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/build/lib/FamousCipherAlgorithms/Shift.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/build/lib/FamousCipherAlgorithms/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/LICENSE
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/README.md
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.4/setup.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.4/FamousCipherAlgorithms/ADFGVX.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.4/FamousCipherAlgorithms/Affine.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.4/FamousCipherAlgorithms/Columnar.py
+-rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.4/FamousCipherAlgorithms/Hill.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.4/FamousCipherAlgorithms/OneTimePad.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.4/FamousCipherAlgorithms/Permutation.py
+-rw-r--r--   0        0        0     6292 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.4/FamousCipherAlgorithms/Playfair.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.4/FamousCipherAlgorithms/Polybius.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.4/FamousCipherAlgorithms/RailFence.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.4/FamousCipherAlgorithms/Shift.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.4/FamousCipherAlgorithms/Vigenere.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.4/FamousCipherAlgorithms/__init__.py
+-rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.4/README.md
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 famouscipheralgorithms-0.1.4/PKG-INFO
```

### Comparing `famouscipheralgorithms-0.1.3/setup.py` & `famouscipheralgorithms-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `famouscipheralgorithms-0.1.3/FamousCipherAlgorithms/Affine.py` & `famouscipheralgorithms-0.1.4/FamousCipherAlgorithms/Affine.py`

 * *Files identical despite different names*

### Comparing `famouscipheralgorithms-0.1.3/FamousCipherAlgorithms/Hill.py` & `famouscipheralgorithms-0.1.4/FamousCipherAlgorithms/Hill.py`

 * *Files identical despite different names*

### Comparing `famouscipheralgorithms-0.1.3/FamousCipherAlgorithms/Permutation.py` & `famouscipheralgorithms-0.1.4/FamousCipherAlgorithms/Permutation.py`

 * *Files identical despite different names*

### Comparing `famouscipheralgorithms-0.1.3/FamousCipherAlgorithms/Playfair.py` & `famouscipheralgorithms-0.1.4/FamousCipherAlgorithms/Playfair.py`

 * *Files identical despite different names*

### Comparing `famouscipheralgorithms-0.1.3/FamousCipherAlgorithms/RailFence.py` & `famouscipheralgorithms-0.1.4/FamousCipherAlgorithms/RailFence.py`

 * *Files identical despite different names*

### Comparing `famouscipheralgorithms-0.1.3/FamousCipherAlgorithms/Shift.py` & `famouscipheralgorithms-0.1.4/FamousCipherAlgorithms/Shift.py`

 * *Files identical despite different names*

### Comparing `famouscipheralgorithms-0.1.3/FamousCipherAlgorithms/Vigenere.py` & `famouscipheralgorithms-0.1.4/FamousCipherAlgorithms/Vigenere.py`

 * *Files identical despite different names*

### Comparing `famouscipheralgorithms-0.1.3/LICENSE` & `famouscipheralgorithms-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `famouscipheralgorithms-0.1.3/pyproject.toml` & `famouscipheralgorithms-0.1.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "FamousCipherAlgorithms"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Mobin Nesari", email="mobinnesari81@gmail.com" },
   { name="Mohammad Mehdi Begmaz", email="mohammadmehdi.begmaz@gmail.com"}
 ]
 maintainers =[
     { name="Mobin Nesari", email="mobinnesari@gmail.com"},
     { name="Mohammad Mehdi Begmaz", email="mohammadmehdi.begmaz@gmail.com"},
```

