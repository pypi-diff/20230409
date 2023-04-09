# Comparing `tmp/cryptographyComplements-0.2.4.tar.gz` & `tmp/cryptographyComplements-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptographyComplements-0.2.4.tar", last modified: Sat Apr  8 13:00:16 2023, max compression
+gzip compressed data, was "cryptographyComplements-0.2.5.tar", last modified: Sun Apr  9 19:59:25 2023, max compression
```

## Comparing `cryptographyComplements-0.2.4.tar` & `cryptographyComplements-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 13:00:16.266295 cryptographyComplements-0.2.4/
--rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.2.4/LICENSE
--rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0      579 2023-04-08 13:00:16.265210 cryptographyComplements-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-03-18 18:48:58.000000 cryptographyComplements-0.2.4/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 13:00:16.262229 cryptographyComplements-0.2.4/cryptographyComplements/
--rw-rw-rw-   0        0        0      197 2023-03-18 18:48:58.000000 cryptographyComplements-0.2.4/cryptographyComplements/__init__.py
--rw-rw-rw-   0        0        0     1629 2023-03-18 19:21:02.000000 cryptographyComplements-0.2.4/cryptographyComplements/ciphers.py
--rw-rw-rw-   0        0        0     9607 2023-04-08 12:58:40.000000 cryptographyComplements-0.2.4/cryptographyComplements/mathFunctions.py
--rw-rw-rw-   0        0        0     2510 2023-04-07 19:28:48.000000 cryptographyComplements-0.2.4/cryptographyComplements/primalityTests.py
--rw-rw-rw-   0        0        0     2252 2023-03-31 15:53:30.000000 cryptographyComplements-0.2.4/cryptographyComplements/tools.py
-drwxrwxrwx   0        0        0        0 2023-04-08 13:00:16.264227 cryptographyComplements-0.2.4/cryptographyComplements.egg-info/
--rw-rw-rw-   0        0        0      279 2023-04-08 13:00:16.000000 cryptographyComplements-0.2.4/cryptographyComplements.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 13:00:16.266295 cryptographyComplements-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      742 2023-04-08 13:00:10.000000 cryptographyComplements-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 19:59:25.202017 cryptographyComplements-0.2.5/
+-rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      579 2023-04-09 19:59:25.200645 cryptographyComplements-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-03-18 18:48:58.000000 cryptographyComplements-0.2.5/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 19:59:25.197551 cryptographyComplements-0.2.5/cryptographyComplements/
+-rw-rw-rw-   0        0        0      197 2023-03-18 18:48:58.000000 cryptographyComplements-0.2.5/cryptographyComplements/__init__.py
+-rw-rw-rw-   0        0        0     1631 2023-04-09 18:34:14.000000 cryptographyComplements-0.2.5/cryptographyComplements/ciphers.py
+-rw-rw-rw-   0        0        0    10180 2023-04-09 19:58:33.000000 cryptographyComplements-0.2.5/cryptographyComplements/mathFunctions.py
+-rw-rw-rw-   0        0        0     2510 2023-04-07 19:28:48.000000 cryptographyComplements-0.2.5/cryptographyComplements/primalityTests.py
+-rw-rw-rw-   0        0        0     2252 2023-03-31 15:53:30.000000 cryptographyComplements-0.2.5/cryptographyComplements/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-09 19:59:25.199643 cryptographyComplements-0.2.5/cryptographyComplements.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-04-09 19:59:25.000000 cryptographyComplements-0.2.5/cryptographyComplements.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 19:59:25.202017 cryptographyComplements-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      742 2023-04-09 19:59:13.000000 cryptographyComplements-0.2.5/setup.py
```

### Comparing `cryptographyComplements-0.2.4/LICENSE` & `cryptographyComplements-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.2.4/PKG-INFO` & `cryptographyComplements-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptographyComplements
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python library, in development, that allows the user to use cryptography, and related, functions.
 Author: Forzo
 License: GPL-3.0
 Project-URL: Source, https://github.com/Forzooo/cryptographyComplements
 Project-URL: Documentation, https://cryptographycomplements.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `cryptographyComplements-0.2.4/cryptographyComplements/ciphers.py` & `cryptographyComplements-0.2.5/cryptographyComplements/ciphers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 def MonoalphabeticCipher():
     "This function generates a cipher using the monoalphabetic encryption"
     import string, random
-    elements = string.ascii_letters + string.digits + string.punctuation + "àèéìòù" + " "
+    elements = string.ascii_letters + string.digits + string.punctuation + "àèéìòù"# + " "
     cipher = {elements[i]: None for i in range(len(elements))}
 
     already_sorted = []
     element_sorted = None
 
     for i in cipher.keys():
         while True:
@@ -23,15 +23,15 @@
     writeCipher(cipher)
     return cipher
 
 
 def CaesarCipher():
     "This functions generate the Caesar Cipher with a random sequence, or if enabled by the user in the script, the original one."
     import string, random
-    elements = string.ascii_letters + string.digits + string.punctuation + "àèéìòù" + " "
+    elements = string.ascii_letters + string.digits + string.punctuation + "àèéìòù"# + " "
     cipher = {elements[i]: None for i in range(len(elements))}
 
     # sequence = 3 # use this for the original Caesar cipher
     sequence = random.randint(0, len(cipher)) # use this for a random Caesar cipher
 
     modulo = int(len(cipher))
     for i in cipher.keys():
```

### Comparing `cryptographyComplements-0.2.4/cryptographyComplements/mathFunctions.py` & `cryptographyComplements-0.2.5/cryptographyComplements/mathFunctions.py`

 * *Files 4% similar despite different names*

```diff
@@ -292,8 +292,27 @@
         steps += 1
 
     return steps
 
 
 def FermatEulerTheorem(a:int, n:int) -> int:
     "From a given two given integers calculate Fermat-Euler Theorem. \n\nNote: a is the number and n is the modulo"
-    return (a**(EulerTotientFunction(n))) % n
+    return (a**(EulerTotientFunction(n))) % n
+
+
+def EulerFormula(p: int, q: int) -> bool:
+    "The Euler Formula from two given integers p and q returns True if the congruence a^((p-1)(q-1)/g) mod pq is congruent to 1 and False if it's not."
+
+    if p == 2 or q == 2:
+        return FermatEulerTheorem(p, q)
+
+    g = EuclideanAlgorithm(p-1, q-1)
+
+    a = pow(2, (p-1)*(q-1)//g, p*q) # 2 can be set, to the base, because is coprime with p*q if p or q isn't 2
+
+    if EuclideanAlgorithm(a, p*q) != 1:
+        return False
+
+    if pow(a, (p-1)*(q-1)//g, p*q) != 1:
+        return False
+
+    return True
```

### Comparing `cryptographyComplements-0.2.4/cryptographyComplements/primalityTests.py` & `cryptographyComplements-0.2.5/cryptographyComplements/primalityTests.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.2.4/cryptographyComplements/tools.py` & `cryptographyComplements-0.2.5/cryptographyComplements/tools.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.2.4/setup.py` & `cryptographyComplements-0.2.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cryptographyComplements',
-    version='0.2.4',
+    version='0.2.5',
     description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description_content_type='text/markdown',
     author='Forzo',
     packages=find_packages(),
     license="GPL-3.0",
     project_urls={
```

