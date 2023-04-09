# Comparing `tmp/indian_cities-1.0.0.tar.gz` & `tmp/indian_cities-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indian_cities-1.0.0.tar", last modified: Mon May 31 15:30:30 2021, max compression
+gzip compressed data, was "indian_cities-1.0.1.tar", last modified: Sun Apr  9 08:22:08 2023, max compression
```

## Comparing `indian_cities-1.0.0.tar` & `indian_cities-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 chayan    (1000) chayan    (1000)        0 2021-05-31 15:30:30.143543 indian_cities-1.0.0/
--rw-r--r--   0 chayan    (1000) chayan    (1000)     1069 2021-05-31 11:49:18.000000 indian_cities-1.0.0/LICENSE
--rw-r--r--   0 chayan    (1000) chayan    (1000)     2040 2021-05-31 15:30:30.143543 indian_cities-1.0.0/PKG-INFO
--rw-r--r--   0 chayan    (1000) chayan    (1000)     1126 2021-05-31 15:26:05.000000 indian_cities-1.0.0/README.md
-drwxr-xr-x   0 chayan    (1000) chayan    (1000)        0 2021-05-31 15:30:30.143543 indian_cities-1.0.0/indian_cities/
--rw-r--r--   0 chayan    (1000) chayan    (1000)        0 2021-05-31 11:59:09.000000 indian_cities-1.0.0/indian_cities/__init__.py
--rw-r--r--   0 chayan    (1000) chayan    (1000)    20789 2021-05-31 11:50:11.000000 indian_cities-1.0.0/indian_cities/dj_city.py
-drwxr-xr-x   0 chayan    (1000) chayan    (1000)        0 2021-05-31 15:30:30.143543 indian_cities-1.0.0/indian_cities.egg-info/
--rw-r--r--   0 chayan    (1000) chayan    (1000)     2040 2021-05-31 15:30:29.000000 indian_cities-1.0.0/indian_cities.egg-info/PKG-INFO
--rw-r--r--   0 chayan    (1000) chayan    (1000)      225 2021-05-31 15:30:30.000000 indian_cities-1.0.0/indian_cities.egg-info/SOURCES.txt
--rw-r--r--   0 chayan    (1000) chayan    (1000)        1 2021-05-31 15:30:29.000000 indian_cities-1.0.0/indian_cities.egg-info/dependency_links.txt
--rw-r--r--   0 chayan    (1000) chayan    (1000)       14 2021-05-31 15:30:29.000000 indian_cities-1.0.0/indian_cities.egg-info/top_level.txt
--rw-r--r--   0 chayan    (1000) chayan    (1000)       38 2021-05-31 15:30:30.143543 indian_cities-1.0.0/setup.cfg
--rw-r--r--   0 chayan    (1000) chayan    (1000)      681 2021-05-31 15:29:05.000000 indian_cities-1.0.0/setup.py
+drwxr-xr-x   0 chayan     (501) staff       (20)        0 2023-04-09 08:22:08.607217 indian_cities-1.0.1/
+-rw-r--r--   0 chayan     (501) staff       (20)     1069 2023-04-09 08:20:13.000000 indian_cities-1.0.1/LICENSE
+-rw-r--r--   0 chayan     (501) staff       (20)     1762 2023-04-09 08:22:08.606922 indian_cities-1.0.1/PKG-INFO
+-rw-r--r--   0 chayan     (501) staff       (20)     1305 2023-04-09 08:20:13.000000 indian_cities-1.0.1/README.md
+drwxr-xr-x   0 chayan     (501) staff       (20)        0 2023-04-09 08:22:08.605225 indian_cities-1.0.1/indian_cities/
+-rw-r--r--   0 chayan     (501) staff       (20)        0 2023-04-09 08:20:13.000000 indian_cities-1.0.1/indian_cities/__init__.py
+-rw-r--r--   0 chayan     (501) staff       (20)    21260 2023-04-09 08:20:13.000000 indian_cities-1.0.1/indian_cities/dj_city.py
+drwxr-xr-x   0 chayan     (501) staff       (20)        0 2023-04-09 08:22:08.606597 indian_cities-1.0.1/indian_cities.egg-info/
+-rw-r--r--   0 chayan     (501) staff       (20)     1762 2023-04-09 08:22:08.000000 indian_cities-1.0.1/indian_cities.egg-info/PKG-INFO
+-rw-r--r--   0 chayan     (501) staff       (20)      225 2023-04-09 08:22:08.000000 indian_cities-1.0.1/indian_cities.egg-info/SOURCES.txt
+-rw-r--r--   0 chayan     (501) staff       (20)        1 2023-04-09 08:22:08.000000 indian_cities-1.0.1/indian_cities.egg-info/dependency_links.txt
+-rw-r--r--   0 chayan     (501) staff       (20)       14 2023-04-09 08:22:08.000000 indian_cities-1.0.1/indian_cities.egg-info/top_level.txt
+-rw-r--r--   0 chayan     (501) staff       (20)       38 2023-04-09 08:22:08.607290 indian_cities-1.0.1/setup.cfg
+-rw-r--r--   0 chayan     (501) staff       (20)      681 2023-04-09 08:21:54.000000 indian_cities-1.0.1/setup.py
```

### Comparing `indian_cities-1.0.0/LICENSE` & `indian_cities-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `indian_cities-1.0.0/PKG-INFO` & `indian_cities-1.0.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,71 +1,73 @@
 Metadata-Version: 2.1
 Name: indian_cities
-Version: 1.0.0
+Version: 1.0.1
 Summary: Django Indian Cities
 Home-page: https://github.com/chayandatta/django_indian_cities
 Author: Chayan Datta
 Author-email: chayan.datta1996@gmail.com
 License: MIT
-Description: [![PyPI version](https://badge.fury.io/py/indian-cities.svg)](https://badge.fury.io/py/indian-cities)
-        ![PyPI - License](https://img.shields.io/pypi/l/indian-cities)
-        [![Downloads](https://pepy.tech/badge/indian-cities)](https://pepy.tech/project/indian-cities)
-        
-        # indian-cities  -- states & cities for india 🇮🇳
-        
-        ## Why?
-        
-        If there was something plug 🔌 and play
-        which can be just imported and it'll fill the choices fields with Indian cities or states.
-        How good it'll be.
-        
-        
-        ## How to use this
-        
-        > To import just add this line
-        
-        ```
-        from indian_cities.dj_city import cities
-        ```
-        > Test it
-        
-        ```
-        print(cities[0])
-        ```
-        Now if the output looks like this
-        ```
-        ('Andaman and Nicobar Islands', (('Port Blair', 'Port Blair'),))
-        ```
-        Then awesome, it did work 👍
-        ```
-        class myModel(models.Model):
-        
-            city = models.CharField(choices=cities, null=False, max_length=20)
-        
-        ```
-        
-        ### Requirements:
-        
-        Any version of Python, Django
-        
-        ## Installation
-        
-        To install this
-        
-        > pip install indian-cities
-        
-        ---
-        ## Connect with me:
-        
-        LinkedIn: https://www.linkedin.com/in/chayandatta/
-        
-        github: https://github.com/chayandatta
-        
-        ---
-        
-        made with ❤️ and 🐍
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI version](https://badge.fury.io/py/indian-cities.svg)](https://badge.fury.io/py/indian-cities)
+![PyPI - License](https://img.shields.io/pypi/l/indian-cities)
+[![Downloads](https://pepy.tech/badge/indian-cities)](https://pepy.tech/project/indian-cities)
+[![CodeFactor](https://www.codefactor.io/repository/github/chayandatta/django_indian_cities/badge)](https://www.codefactor.io/repository/github/chayandatta/django_indian_cities)
+
+# indian-cities  -- states & cities for india 🇮🇳
+
+## Why?
+
+If there was something plug 🔌 and play
+which can be just imported and it'll fill the choices fields with Indian cities or states.
+How good it'll be.
+
+
+## How to use this
+
+> To import just add this line
+
+```
+from indian_cities.dj_city import cities
+```
+> Test it
+
+```
+print(cities[0])
+```
+Now if the output looks like this
+```
+('Andaman and Nicobar Islands', (('Port Blair', 'Port Blair'),))
+```
+Then awesome, it did work 👍
+```
+class myModel(models.Model):
+
+    city = models.CharField(choices=cities, null=False, max_length=20)
+
+```
+
+### Requirements:
+
+Any version of Python, Django
+
+## Installation
+
+To install this
+
+> pip install indian-cities
+
+---
+## Connect with me:
+
+LinkedIn: https://www.linkedin.com/in/chayandatta/
+
+github: https://github.com/chayandatta
+
+---
+
+made with ❤️ and 🐍
```

### Comparing `indian_cities-1.0.0/README.md` & `indian_cities-1.0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [![PyPI version](https://badge.fury.io/py/indian-cities.svg)](https://badge.fury.io/py/indian-cities)
 ![PyPI - License](https://img.shields.io/pypi/l/indian-cities)
 [![Downloads](https://pepy.tech/badge/indian-cities)](https://pepy.tech/project/indian-cities)
+[![CodeFactor](https://www.codefactor.io/repository/github/chayandatta/django_indian_cities/badge)](https://www.codefactor.io/repository/github/chayandatta/django_indian_cities)
 
 # indian-cities  -- states & cities for india 🇮🇳
 
 ## Why?
 
 If there was something plug 🔌 and play
 which can be just imported and it'll fill the choices fields with Indian cities or states.
@@ -50,8 +51,8 @@
 
 LinkedIn: https://www.linkedin.com/in/chayandatta/
 
 github: https://github.com/chayandatta
 
 ---
 
-made with ❤️ and 🐍
+made with ❤️ and 🐍
```

### Comparing `indian_cities-1.0.0/indian_cities/dj_city.py` & `indian_cities-1.0.1/indian_cities/dj_city.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,30 @@
             ("Narasaraopet", "Narasaraopet"),
             ("Tadipatri", "Tadipatri"),
             ("Tadepalligudem", "Tadepalligudem"),
             ("Amaravati", "Amaravati"),
             ("Chilakaluripet", "Chilakaluripet"),
         ),
     ),
+    ("Arunachal Pradesh", (("Itanagar", "Itanagar"),)),
+    (
+        "Assam", 
+        (
+            ("Dhuburi", "Dhuburi"),
+            ("Dibrugarh", "Dibrugarh"),
+            ("Dispur", "Dispur"),
+            ("Guwahati", "Guwahati"),
+            ("Jorhat", "Jorhat"),
+            ("Nagaon", "Nagaon"),
+            ("Sivasagar", "Sivasagar"),
+            ("Silchar", "Silchar"),
+            ("Tezpur", "Tezpur"),
+            ("Tinsukia", "Tinsukia"),
+        )
+    ),
     (
         "Bihar",
         (
             ("Patna", "Patna"),
             ("Gaya", "Gaya"),
             ("Bhagalpur", "Bhagalpur"),
             ("Muzaffarpur", "Muzaffarpur"),
```

### Comparing `indian_cities-1.0.0/indian_cities.egg-info/PKG-INFO` & `indian_cities-1.0.1/indian_cities.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,73 @@
 Metadata-Version: 2.1
 Name: indian-cities
-Version: 1.0.0
+Version: 1.0.1
 Summary: Django Indian Cities
 Home-page: https://github.com/chayandatta/django_indian_cities
 Author: Chayan Datta
 Author-email: chayan.datta1996@gmail.com
 License: MIT
-Description: [![PyPI version](https://badge.fury.io/py/indian-cities.svg)](https://badge.fury.io/py/indian-cities)
-        ![PyPI - License](https://img.shields.io/pypi/l/indian-cities)
-        [![Downloads](https://pepy.tech/badge/indian-cities)](https://pepy.tech/project/indian-cities)
-        
-        # indian-cities  -- states & cities for india 🇮🇳
-        
-        ## Why?
-        
-        If there was something plug 🔌 and play
-        which can be just imported and it'll fill the choices fields with Indian cities or states.
-        How good it'll be.
-        
-        
-        ## How to use this
-        
-        > To import just add this line
-        
-        ```
-        from indian_cities.dj_city import cities
-        ```
-        > Test it
-        
-        ```
-        print(cities[0])
-        ```
-        Now if the output looks like this
-        ```
-        ('Andaman and Nicobar Islands', (('Port Blair', 'Port Blair'),))
-        ```
-        Then awesome, it did work 👍
-        ```
-        class myModel(models.Model):
-        
-            city = models.CharField(choices=cities, null=False, max_length=20)
-        
-        ```
-        
-        ### Requirements:
-        
-        Any version of Python, Django
-        
-        ## Installation
-        
-        To install this
-        
-        > pip install indian-cities
-        
-        ---
-        ## Connect with me:
-        
-        LinkedIn: https://www.linkedin.com/in/chayandatta/
-        
-        github: https://github.com/chayandatta
-        
-        ---
-        
-        made with ❤️ and 🐍
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI version](https://badge.fury.io/py/indian-cities.svg)](https://badge.fury.io/py/indian-cities)
+![PyPI - License](https://img.shields.io/pypi/l/indian-cities)
+[![Downloads](https://pepy.tech/badge/indian-cities)](https://pepy.tech/project/indian-cities)
+[![CodeFactor](https://www.codefactor.io/repository/github/chayandatta/django_indian_cities/badge)](https://www.codefactor.io/repository/github/chayandatta/django_indian_cities)
+
+# indian-cities  -- states & cities for india 🇮🇳
+
+## Why?
+
+If there was something plug 🔌 and play
+which can be just imported and it'll fill the choices fields with Indian cities or states.
+How good it'll be.
+
+
+## How to use this
+
+> To import just add this line
+
+```
+from indian_cities.dj_city import cities
+```
+> Test it
+
+```
+print(cities[0])
+```
+Now if the output looks like this
+```
+('Andaman and Nicobar Islands', (('Port Blair', 'Port Blair'),))
+```
+Then awesome, it did work 👍
+```
+class myModel(models.Model):
+
+    city = models.CharField(choices=cities, null=False, max_length=20)
+
+```
+
+### Requirements:
+
+Any version of Python, Django
+
+## Installation
+
+To install this
+
+> pip install indian-cities
+
+---
+## Connect with me:
+
+LinkedIn: https://www.linkedin.com/in/chayandatta/
+
+github: https://github.com/chayandatta
+
+---
+
+made with ❤️ and 🐍
```

### Comparing `indian_cities-1.0.0/setup.py` & `indian_cities-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="indian_cities",
-    version="1.0.0",
+    version="1.0.1",
     description="Django Indian Cities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     url="https://github.com/chayandatta/django_indian_cities",
     author="Chayan Datta",
     author_email="chayan.datta1996@gmail.com",
```

