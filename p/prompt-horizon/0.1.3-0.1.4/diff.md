# Comparing `tmp/prompt-horizon-0.1.3.tar.gz` & `tmp/prompt-horizon-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt-horizon-0.1.3.tar", last modified: Sun Apr  9 05:32:17 2023, max compression
+gzip compressed data, was "prompt-horizon-0.1.4.tar", last modified: Sun Apr  9 14:16:08 2023, max compression
```

## Comparing `prompt-horizon-0.1.3.tar` & `prompt-horizon-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 05:32:17.879716 prompt-horizon-0.1.3/
--rw-rw-rw-   0        0        0     1098 2023-04-06 09:13:09.000000 prompt-horizon-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     3644 2023-04-09 05:32:17.878716 prompt-horizon-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2837 2023-04-09 05:30:48.000000 prompt-horizon-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 05:32:17.854716 prompt-horizon-0.1.3/prompt_horizon/
--rw-rw-rw-   0        0        0       74 2023-04-07 11:09:20.000000 prompt-horizon-0.1.3/prompt_horizon/__init__.py
--rw-rw-rw-   0        0        0     1917 2023-04-09 05:15:59.000000 prompt-horizon-0.1.3/prompt_horizon/anonymizer.py
--rw-rw-rw-   0        0        0     1727 2023-04-09 05:22:51.000000 prompt-horizon-0.1.3/prompt_horizon/de_anonymizer.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:32:17.865716 prompt-horizon-0.1.3/prompt_horizon.egg-info/
--rw-rw-rw-   0        0        0     3644 2023-04-09 05:32:17.000000 prompt-horizon-0.1.3/prompt_horizon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2023-04-09 05:32:17.000000 prompt-horizon-0.1.3/prompt_horizon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 05:32:17.000000 prompt-horizon-0.1.3/prompt_horizon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-09 05:32:17.000000 prompt-horizon-0.1.3/prompt_horizon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 05:32:17.879716 prompt-horizon-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1200 2023-04-09 05:31:04.000000 prompt-horizon-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 05:32:17.876715 prompt-horizon-0.1.3/tests/
--rw-rw-rw-   0        0        0        0 2023-04-06 09:32:02.000000 prompt-horizon-0.1.3/tests/__init__.py
--rw-rw-rw-   0        0        0     3923 2023-04-09 05:19:36.000000 prompt-horizon-0.1.3/tests/test_anonymizer.py
--rw-rw-rw-   0        0        0     1349 2023-04-06 21:06:53.000000 prompt-horizon-0.1.3/tests/test_anonymizer_complex.py
--rw-rw-rw-   0        0        0     3663 2023-04-09 05:28:59.000000 prompt-horizon-0.1.3/tests/test_de_anonymizer.py
+drwxrwxrwx   0        0        0        0 2023-04-09 14:16:08.446746 prompt-horizon-0.1.4/
+-rw-rw-rw-   0        0        0     1098 2023-04-06 09:13:09.000000 prompt-horizon-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     3590 2023-04-09 14:16:08.445747 prompt-horizon-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2783 2023-04-09 14:15:08.000000 prompt-horizon-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 14:16:08.418748 prompt-horizon-0.1.4/prompt_horizon/
+-rw-rw-rw-   0        0        0       74 2023-04-07 11:09:20.000000 prompt-horizon-0.1.4/prompt_horizon/__init__.py
+-rw-rw-rw-   0        0        0     1917 2023-04-09 05:15:59.000000 prompt-horizon-0.1.4/prompt_horizon/anonymizer.py
+-rw-rw-rw-   0        0        0     1727 2023-04-09 05:22:51.000000 prompt-horizon-0.1.4/prompt_horizon/de_anonymizer.py
+drwxrwxrwx   0        0        0        0 2023-04-09 14:16:08.432747 prompt-horizon-0.1.4/prompt_horizon.egg-info/
+-rw-rw-rw-   0        0        0     3590 2023-04-09 14:16:08.000000 prompt-horizon-0.1.4/prompt_horizon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2023-04-09 14:16:08.000000 prompt-horizon-0.1.4/prompt_horizon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 14:16:08.000000 prompt-horizon-0.1.4/prompt_horizon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-09 14:16:08.000000 prompt-horizon-0.1.4/prompt_horizon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 14:16:08.446746 prompt-horizon-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1200 2023-04-09 14:15:34.000000 prompt-horizon-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 14:16:08.442747 prompt-horizon-0.1.4/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-06 09:32:02.000000 prompt-horizon-0.1.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     3923 2023-04-09 05:19:36.000000 prompt-horizon-0.1.4/tests/test_anonymizer.py
+-rw-rw-rw-   0        0        0     1349 2023-04-06 21:06:53.000000 prompt-horizon-0.1.4/tests/test_anonymizer_complex.py
+-rw-rw-rw-   0        0        0     3663 2023-04-09 05:28:59.000000 prompt-horizon-0.1.4/tests/test_de_anonymizer.py
```

### Comparing `prompt-horizon-0.1.3/LICENSE` & `prompt-horizon-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prompt-horizon-0.1.3/PKG-INFO` & `prompt-horizon-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-horizon
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library to anonymize JSON objects by creating placeholders for keys and values, while generating a reversible mapping to restore afterwards
 Home-page: https://github.com/gkanellopoulos/prompthorizon.git
 Author: George Kanellopoulos
 Author-email: george@gkanellopoulos.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -113,18 +113,10 @@
 ```python
 from prompt_horizon import de_anonymize
 
 #This will read the anonymized JSON data from "anonymized.json", the mapping object from "map_file.json", de-anonymize the JSON data, and save the de-anonymized JSON to "deanonymized.json".
 deanonymized_json = de_anonymize("anonymized.json", map_file_path="map_file.json", output_file_path="deanonymized.json")
 ```
 
-
-
-<br>
-
-### Saving and loading the map
-
-<br>
-
 ## License
 
 This project is licensed under the [MIT License](LICENSE).
```

### Comparing `prompt-horizon-0.1.3/README.md` & `prompt-horizon-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -95,18 +95,10 @@
 ```python
 from prompt_horizon import de_anonymize
 
 #This will read the anonymized JSON data from "anonymized.json", the mapping object from "map_file.json", de-anonymize the JSON data, and save the de-anonymized JSON to "deanonymized.json".
 deanonymized_json = de_anonymize("anonymized.json", map_file_path="map_file.json", output_file_path="deanonymized.json")
 ```
 
-
-
-<br>
-
-### Saving and loading the map
-
-<br>
-
 ## License
 
 This project is licensed under the [MIT License](LICENSE).
```

### Comparing `prompt-horizon-0.1.3/prompt_horizon/anonymizer.py` & `prompt-horizon-0.1.4/prompt_horizon/anonymizer.py`

 * *Files identical despite different names*

### Comparing `prompt-horizon-0.1.3/prompt_horizon/de_anonymizer.py` & `prompt-horizon-0.1.4/prompt_horizon/de_anonymizer.py`

 * *Files identical despite different names*

### Comparing `prompt-horizon-0.1.3/prompt_horizon.egg-info/PKG-INFO` & `prompt-horizon-0.1.4/prompt_horizon.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-horizon
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library to anonymize JSON objects by creating placeholders for keys and values, while generating a reversible mapping to restore afterwards
 Home-page: https://github.com/gkanellopoulos/prompthorizon.git
 Author: George Kanellopoulos
 Author-email: george@gkanellopoulos.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -113,18 +113,10 @@
 ```python
 from prompt_horizon import de_anonymize
 
 #This will read the anonymized JSON data from "anonymized.json", the mapping object from "map_file.json", de-anonymize the JSON data, and save the de-anonymized JSON to "deanonymized.json".
 deanonymized_json = de_anonymize("anonymized.json", map_file_path="map_file.json", output_file_path="deanonymized.json")
 ```
 
-
-
-<br>
-
-### Saving and loading the map
-
-<br>
-
 ## License
 
 This project is licensed under the [MIT License](LICENSE).
```

### Comparing `prompt-horizon-0.1.3/setup.py` & `prompt-horizon-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def read_file(filename):
     with open(os.path.join(os.path.dirname(__file__), filename), encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='prompt-horizon',
-    version='0.1.3',
+    version='0.1.4',
     description='Library to anonymize JSON objects by creating placeholders for keys and values, while generating a reversible mapping to restore afterwards',
     long_description=read_file('README.md'),
     long_description_content_type='text/markdown',
     author='George Kanellopoulos',
     author_email='george@gkanellopoulos.com',
     url='https://github.com/gkanellopoulos/prompthorizon.git',
     packages=find_packages(),
```

### Comparing `prompt-horizon-0.1.3/tests/test_anonymizer.py` & `prompt-horizon-0.1.4/tests/test_anonymizer.py`

 * *Files identical despite different names*

### Comparing `prompt-horizon-0.1.3/tests/test_anonymizer_complex.py` & `prompt-horizon-0.1.4/tests/test_anonymizer_complex.py`

 * *Files identical despite different names*

### Comparing `prompt-horizon-0.1.3/tests/test_de_anonymizer.py` & `prompt-horizon-0.1.4/tests/test_de_anonymizer.py`

 * *Files identical despite different names*

