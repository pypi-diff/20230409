# Comparing `tmp/HELML-0.1.7.tar.gz` & `tmp/HELML-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HELML-0.1.7.tar", last modified: Tue Apr  4 14:26:36 2023, max compression
+gzip compressed data, was "HELML-0.1.8.tar", last modified: Sun Apr  9 11:39:30 2023, max compression
```

## Comparing `HELML-0.1.7.tar` & `HELML-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 14:26:36.490637 HELML-0.1.7/
-drwxrwxrwx   0        0        0        0 2023-04-04 14:26:36.485636 HELML-0.1.7/HELML/
--rw-rw-rw-   0        0        0      274 2023-03-15 13:42:07.000000 HELML-0.1.7/HELML/__init__.py
--rw-rw-rw-   0        0        0    16014 2023-04-04 11:57:46.000000 HELML-0.1.7/HELML/_helml.py
--rw-rw-rw-   0        0        0      122 2023-04-04 14:05:34.000000 HELML-0.1.7/HELML/_version.py
-drwxrwxrwx   0        0        0        0 2023-04-04 14:26:36.488637 HELML-0.1.7/HELML.egg-info/
--rw-rw-rw-   0        0        0     2449 2023-04-04 14:26:36.000000 HELML-0.1.7/HELML.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-04-04 14:26:36.000000 HELML-0.1.7/HELML.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 14:26:36.000000 HELML-0.1.7/HELML.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-04 14:26:36.000000 HELML-0.1.7/HELML.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-03-15 16:11:37.000000 HELML-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     2449 2023-04-04 14:26:36.489637 HELML-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1724 2023-04-04 14:04:54.000000 HELML-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-04-04 14:26:36.490637 HELML-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      884 2023-04-04 14:05:43.000000 HELML-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 11:39:30.855459 HELML-0.1.8/
+drwxrwxrwx   0        0        0        0 2023-04-09 11:39:30.850459 HELML-0.1.8/HELML/
+-rw-rw-rw-   0        0        0      274 2023-03-15 13:42:07.000000 HELML-0.1.8/HELML/__init__.py
+-rw-rw-rw-   0        0        0    16401 2023-04-09 11:29:37.000000 HELML-0.1.8/HELML/_helml.py
+-rw-rw-rw-   0        0        0      122 2023-04-09 11:38:27.000000 HELML-0.1.8/HELML/_version.py
+drwxrwxrwx   0        0        0        0 2023-04-09 11:39:30.853459 HELML-0.1.8/HELML.egg-info/
+-rw-rw-rw-   0        0        0     2472 2023-04-09 11:39:30.000000 HELML-0.1.8/HELML.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-04-09 11:39:30.000000 HELML-0.1.8/HELML.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 11:39:30.000000 HELML-0.1.8/HELML.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-09 11:39:30.000000 HELML-0.1.8/HELML.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-03-15 16:11:37.000000 HELML-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     2472 2023-04-09 11:39:30.854459 HELML-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1747 2023-04-04 15:46:14.000000 HELML-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-09 11:39:30.855459 HELML-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      884 2023-04-09 11:39:04.000000 HELML-0.1.8/setup.py
```

### Comparing `HELML-0.1.7/HELML/_helml.py` & `HELML-0.1.8/HELML/_helml.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,43 +14,49 @@
         'NIF': float('-inf')
     }
 
     CUSTOM_FORMAT_DECODER = None
     CUSTOM_VALUE_ENCODER = None
     CUSTOM_VALUE_DECODER = None
     
-    ENABLE_SPC_IDENT = True # For encode: add space-indentation at begin of string
+    ENABLE_SPC_IDENT = 1 # For encode: add space-indentation at begin of string
     ENABLE_BONES = True # For encode: enable use "next"-keys like :--:
     ENABLE_KEY_UPLINES = True # For encode: add empty line before create-array-keys
     ENABLE_HASHSYMBOLS = True # For encode: adding # after nested-blocks
 
     @staticmethod
     def encode(
         arr: Union[dict, list, tuple, set],
-        url_mode: bool = False
+        one_line_mode: int = 0
     ) -> str:
         """
         Encode array to HELML string.
-        
+
         :param arr: Input data structure (list, dict, or tuple) to be encoded.
-        :param url_mode: A boolean indicating if the URL mode should be used.
+        :param one_line_mode: The encoding mode to use (0-multi-line, 1-URL-mode, 2-LINE-mode)
         :return: Encoded HELML string.
         """
         results_arr = []
 
-        str_imp = "~" if url_mode else "\n"
+        str_imp = "~" if one_line_mode else "\n"
+        url_mode = one_line_mode == 1
         lvl_ch = "." if url_mode else ":"
         spc_ch = "_" if url_mode else " "
 
         is_list = HELML.num_keys_cnt(arr)
         
         HELML._encode(arr, results_arr, 0, lvl_ch, spc_ch, is_list)
 
-        if url_mode and len(results_arr) == 1:
+        if url_mode:
             results_arr.append('')
+        elif one_line_mode:
+            # Remove whitespace from beginning and end of each string
+            results_arr = [s.strip() for s in results_arr]
+            # Remove empty strings and comments that start with '#'
+            results_arr = [s for s in results_arr if s and not s.startswith('#')]
 
         return str_imp.join(results_arr)
     
     @staticmethod
     def _encode(
         arr: Union[dict, list, tuple, set],
         results_arr: list,
@@ -87,15 +93,15 @@
                     key = '-' + HELML.base64Uencode(key)
 
             # add the appropriate number of colons to the left of the key, based on the current level
             ident = lvl_ch * level
 
              # add space-ident to the left of the key (if need)
             if HELML.ENABLE_SPC_IDENT and spc_ch == ' ':
-                ident = spc_ch * level + ident
+                ident = spc_ch * (level * HELML.ENABLE_SPC_IDENT) + ident
 
             is_arr = isinstance(value, (list, tuple, set))
 
             if is_arr or isinstance(value, dict):
                 # Add empty line before create-key
                 if HELML.ENABLE_KEY_UPLINES and spc_ch == ' ':
                     results_arr.append('')
@@ -143,15 +149,15 @@
                 i = str(i)
             layers_set.add(i)
 
 
         # Explode src_rows to lines
         for exploder_ch in ["\n", "\r", "~"]:
             if exploder_ch in src_rows:
-                if "~" == exploder_ch:
+                if "~" == exploder_ch and src_rows[-1] == "~":
                     lvl_ch = "."
                     spc_ch = "_"
                 break
 
         str_arr = src_rows.split(exploder_ch)
 
         # Initialize result array and stack for keeping track of current array nesting
```

### Comparing `HELML-0.1.7/HELML.egg-info/PKG-INFO` & `HELML-0.1.8/HELML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HELML
-Version: 0.1.7
+Version: 0.1.8
 Summary: Encoding-decoding HELML format
 Home-page: https://github.com/dynoser/HELML/tree/master/Python
 Author: AlexanderJer
 Author-email: alexierusalim@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -17,17 +17,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HELML
 
 ![helml-logo](https://github.com/dynoser/HELML/raw/master/logo/icon.png)
 
+## Python package
+
 * [HELML format definition (en)](https://github.com/dynoser/HELML/blob/master/docs/README-HELML_en.md)
 * [РћРїРёСЃР°РЅРёРµ С„РѕСЂРјР°С‚Р° HELML (ru)](https://github.com/dynoser/HELML/blob/master/docs/README-HELML_ru.md)
 
+
 ## Install
 To install HELML, simply use pip:
 
 ```bash
 pip install helml
 ```
```

### Comparing `HELML-0.1.7/LICENSE` & `HELML-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `HELML-0.1.7/PKG-INFO` & `HELML-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HELML
-Version: 0.1.7
+Version: 0.1.8
 Summary: Encoding-decoding HELML format
 Home-page: https://github.com/dynoser/HELML/tree/master/Python
 Author: AlexanderJer
 Author-email: alexierusalim@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -17,17 +17,20 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HELML
 
 ![helml-logo](https://github.com/dynoser/HELML/raw/master/logo/icon.png)
 
+## Python package
+
 * [HELML format definition (en)](https://github.com/dynoser/HELML/blob/master/docs/README-HELML_en.md)
 * [РћРїРёСЃР°РЅРёРµ С„РѕСЂРјР°С‚Р° HELML (ru)](https://github.com/dynoser/HELML/blob/master/docs/README-HELML_ru.md)
 
+
 ## Install
 To install HELML, simply use pip:
 
 ```bash
 pip install helml
 ```
```

### Comparing `HELML-0.1.7/README.md` & `HELML-0.1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # HELML
 
 ![helml-logo](https://github.com/dynoser/HELML/raw/master/logo/icon.png)
 
+## Python package
+
 * [HELML format definition (en)](https://github.com/dynoser/HELML/blob/master/docs/README-HELML_en.md)
 * [Описание формата HELML (ru)](https://github.com/dynoser/HELML/blob/master/docs/README-HELML_ru.md)
 
+
 ## Install
 To install HELML, simply use pip:
 
 ```bash
 pip install helml
 ```
```

### Comparing `HELML-0.1.7/setup.py` & `HELML-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='HELML',
-    version='0.1.7',
+    version='0.1.8',
     packages=find_packages(),
     install_requires=[
     ],
     author='AlexanderJer',
     author_email='alexierusalim@gmail.com',
     description='Encoding-decoding HELML format',
     long_description=open('README.md').read(),
```

