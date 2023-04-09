# Comparing `tmp/prompt-horizon-0.1.2.tar.gz` & `tmp/prompt-horizon-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt-horizon-0.1.2.tar", last modified: Fri Apr  7 11:13:45 2023, max compression
+gzip compressed data, was "prompt-horizon-0.1.3.tar", last modified: Sun Apr  9 05:32:17 2023, max compression
```

## Comparing `prompt-horizon-0.1.2.tar` & `prompt-horizon-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 11:13:45.470378 prompt-horizon-0.1.2/
--rw-rw-rw-   0        0        0     1098 2023-04-06 09:13:09.000000 prompt-horizon-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     3382 2023-04-07 11:13:45.470378 prompt-horizon-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2575 2023-04-07 11:08:50.000000 prompt-horizon-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 11:13:45.444210 prompt-horizon-0.1.2/prompt_horizon/
--rw-rw-rw-   0        0        0       74 2023-04-07 11:09:20.000000 prompt-horizon-0.1.2/prompt_horizon/__init__.py
--rw-rw-rw-   0        0        0     1841 2023-04-06 13:26:55.000000 prompt-horizon-0.1.2/prompt_horizon/anonymizer.py
--rw-rw-rw-   0        0        0     1549 2023-04-06 17:37:27.000000 prompt-horizon-0.1.2/prompt_horizon/de_anonymizer.py
-drwxrwxrwx   0        0        0        0 2023-04-07 11:13:45.455392 prompt-horizon-0.1.2/prompt_horizon.egg-info/
--rw-rw-rw-   0        0        0     3382 2023-04-07 11:13:45.000000 prompt-horizon-0.1.2/prompt_horizon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2023-04-07 11:13:45.000000 prompt-horizon-0.1.2/prompt_horizon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 11:13:45.000000 prompt-horizon-0.1.2/prompt_horizon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-07 11:13:45.000000 prompt-horizon-0.1.2/prompt_horizon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 11:13:45.471380 prompt-horizon-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1200 2023-04-07 11:11:21.000000 prompt-horizon-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 11:13:45.467379 prompt-horizon-0.1.2/tests/
--rw-rw-rw-   0        0        0        0 2023-04-06 09:32:02.000000 prompt-horizon-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0     3369 2023-04-06 21:06:53.000000 prompt-horizon-0.1.2/tests/test_anonymizer.py
--rw-rw-rw-   0        0        0     1349 2023-04-06 21:06:53.000000 prompt-horizon-0.1.2/tests/test_anonymizer_complex.py
--rw-rw-rw-   0        0        0     3160 2023-04-06 21:06:53.000000 prompt-horizon-0.1.2/tests/test_de_anonymizer.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:32:17.879716 prompt-horizon-0.1.3/
+-rw-rw-rw-   0        0        0     1098 2023-04-06 09:13:09.000000 prompt-horizon-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3644 2023-04-09 05:32:17.878716 prompt-horizon-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2837 2023-04-09 05:30:48.000000 prompt-horizon-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 05:32:17.854716 prompt-horizon-0.1.3/prompt_horizon/
+-rw-rw-rw-   0        0        0       74 2023-04-07 11:09:20.000000 prompt-horizon-0.1.3/prompt_horizon/__init__.py
+-rw-rw-rw-   0        0        0     1917 2023-04-09 05:15:59.000000 prompt-horizon-0.1.3/prompt_horizon/anonymizer.py
+-rw-rw-rw-   0        0        0     1727 2023-04-09 05:22:51.000000 prompt-horizon-0.1.3/prompt_horizon/de_anonymizer.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:32:17.865716 prompt-horizon-0.1.3/prompt_horizon.egg-info/
+-rw-rw-rw-   0        0        0     3644 2023-04-09 05:32:17.000000 prompt-horizon-0.1.3/prompt_horizon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2023-04-09 05:32:17.000000 prompt-horizon-0.1.3/prompt_horizon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 05:32:17.000000 prompt-horizon-0.1.3/prompt_horizon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-09 05:32:17.000000 prompt-horizon-0.1.3/prompt_horizon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 05:32:17.879716 prompt-horizon-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1200 2023-04-09 05:31:04.000000 prompt-horizon-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:32:17.876715 prompt-horizon-0.1.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-06 09:32:02.000000 prompt-horizon-0.1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     3923 2023-04-09 05:19:36.000000 prompt-horizon-0.1.3/tests/test_anonymizer.py
+-rw-rw-rw-   0        0        0     1349 2023-04-06 21:06:53.000000 prompt-horizon-0.1.3/tests/test_anonymizer_complex.py
+-rw-rw-rw-   0        0        0     3663 2023-04-09 05:28:59.000000 prompt-horizon-0.1.3/tests/test_de_anonymizer.py
```

### Comparing `prompt-horizon-0.1.2/LICENSE` & `prompt-horizon-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prompt-horizon-0.1.2/PKG-INFO` & `prompt-horizon-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-horizon
-Version: 0.1.2
+Version: 0.1.3
 Summary: Library to anonymize JSON objects by creating placeholders for keys and values, while generating a reversible mapping to restore afterwards
 Home-page: https://github.com/gkanellopoulos/prompthorizon.git
 Author: George Kanellopoulos
 Author-email: george@gkanellopoulos.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -82,14 +82,25 @@
 
 #This line will read the JSON data from "input.json", anonymize it, and save the anonymized JSON to "anonymized.json".
 anonymized_json, map_object = anonymize("input.json", output_file_path="anonymized.json")
 ```
 
 <br>
 
+#### anonymize only the values
+
+```python
+from prompt_horizon import anonymize
+
+#This line will read the JSON data from "input.json" and anonymize only the values.
+anonymized_json, map_object = anonymize("input.json", anonymize_keys=False)
+```
+
+<br>
+
 ### De-anonymize JSON
 
 <br>
 
 ```python
 from prompt_horizon import de_anonymize
```

### Comparing `prompt-horizon-0.1.2/README.md` & `prompt-horizon-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -64,14 +64,25 @@
 
 #This line will read the JSON data from "input.json", anonymize it, and save the anonymized JSON to "anonymized.json".
 anonymized_json, map_object = anonymize("input.json", output_file_path="anonymized.json")
 ```
 
 <br>
 
+#### anonymize only the values
+
+```python
+from prompt_horizon import anonymize
+
+#This line will read the JSON data from "input.json" and anonymize only the values.
+anonymized_json, map_object = anonymize("input.json", anonymize_keys=False)
+```
+
+<br>
+
 ### De-anonymize JSON
 
 <br>
 
 ```python
 from prompt_horizon import de_anonymize
```

### Comparing `prompt-horizon-0.1.2/prompt_horizon/anonymizer.py` & `prompt-horizon-0.1.3/prompt_horizon/anonymizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from collections.abc import MutableMapping
 
-def anonymize(json_input, map_file_path=None, anonymized_file_path=None):
+def anonymize(json_input, map_file_path=None, anonymized_file_path=None, anonymize_keys=True):
     key_counter = 1
     value_counter = 1
     keys_map = {}
     values_map = {}
 
     if isinstance(json_input, str):
         with open(json_input, 'r') as f:
@@ -15,19 +15,19 @@
 
     def anonymize_recursive(obj):
         nonlocal key_counter, value_counter
 
         if isinstance(obj, dict):
             anonymized_dict = {}
             for key, value in obj.items():
-                if key not in keys_map:
+                if anonymize_keys and key not in keys_map:
                     keys_map[key] = f"k{key_counter}"
                     key_counter += 1
 
-                anon_key = keys_map[key]
+                anon_key = keys_map.get(key, key) if anonymize_keys else key
                 anon_value = anonymize_recursive(value)
 
                 anonymized_dict[anon_key] = anon_value
 
             return anonymized_dict
 
         elif isinstance(obj, list):
```

### Comparing `prompt-horizon-0.1.2/prompt_horizon/de_anonymizer.py` & `prompt-horizon-0.1.3/prompt_horizon/de_anonymizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,21 @@
     keys_map = map_object["keys"]
     values_map = map_object["values"]
 
     def de_anonymize_recursive(obj):
         if isinstance(obj, dict):
             de_anonymized_dict = {}
             for key, value in obj.items():
-                orig_key = [k for k, v in keys_map.items() if v == key][0]
+                orig_key = None
+                
+                if keys_map:  # Check if keys_map is populated
+                    orig_key = [k for k, v in keys_map.items() if v == key][0]
+                else:
+                    orig_key = key
+
                 orig_value = de_anonymize_recursive(value)
 
                 de_anonymized_dict[orig_key] = orig_value
 
             return de_anonymized_dict
 
         elif isinstance(obj, list):
@@ -39,8 +45,8 @@
 
     de_anonymized_object = de_anonymize_recursive(anonymized_object)
 
     if output_file_path:
         with open(output_file_path, 'w') as f:
             json.dump(de_anonymized_object, f, indent=2)
     else:
-        return de_anonymized_object
+        return de_anonymized_object
```

### Comparing `prompt-horizon-0.1.2/prompt_horizon.egg-info/PKG-INFO` & `prompt-horizon-0.1.3/prompt_horizon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-horizon
-Version: 0.1.2
+Version: 0.1.3
 Summary: Library to anonymize JSON objects by creating placeholders for keys and values, while generating a reversible mapping to restore afterwards
 Home-page: https://github.com/gkanellopoulos/prompthorizon.git
 Author: George Kanellopoulos
 Author-email: george@gkanellopoulos.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -82,14 +82,25 @@
 
 #This line will read the JSON data from "input.json", anonymize it, and save the anonymized JSON to "anonymized.json".
 anonymized_json, map_object = anonymize("input.json", output_file_path="anonymized.json")
 ```
 
 <br>
 
+#### anonymize only the values
+
+```python
+from prompt_horizon import anonymize
+
+#This line will read the JSON data from "input.json" and anonymize only the values.
+anonymized_json, map_object = anonymize("input.json", anonymize_keys=False)
+```
+
+<br>
+
 ### De-anonymize JSON
 
 <br>
 
 ```python
 from prompt_horizon import de_anonymize
```

### Comparing `prompt-horizon-0.1.2/setup.py` & `prompt-horizon-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def read_file(filename):
     with open(os.path.join(os.path.dirname(__file__), filename), encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='prompt-horizon',
-    version='0.1.2',
+    version='0.1.3',
     description='Library to anonymize JSON objects by creating placeholders for keys and values, while generating a reversible mapping to restore afterwards',
     long_description=read_file('README.md'),
     long_description_content_type='text/markdown',
     author='George Kanellopoulos',
     author_email='george@gkanellopoulos.com',
     url='https://github.com/gkanellopoulos/prompthorizon.git',
     packages=find_packages(),
```

### Comparing `prompt-horizon-0.1.2/tests/test_anonymizer.py` & `prompt-horizon-0.1.3/tests/test_anonymizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -74,11 +74,24 @@
 
             # Load the anonymized JSON file and compare it with the anonymized_json
             with open(anonymized_file_path, 'r') as f:
                 loaded_anonymized_json = json.load(f)
 
             self.assertEqual(anonymized_json, loaded_anonymized_json)
 
+    def test_anonymize_no_key_anonymization(self):
+        input_json = {"name": "John", "age": 30, "city": "New York"}
+        expected_anonymized_json = {"name": "v1", "age": "v2", "city": "v3"}
+        expected_map_object = {
+            "keys": {},
+            "values": {"John": "v1", "30": "v2", "New York": "v3"}
+        }
+
+        anonymized_json, map_object = anonymize(input_json, anonymize_keys=False)
+
+        self.assertEqual(anonymized_json, expected_anonymized_json)
+        self.assertEqual(map_object, expected_map_object)
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `prompt-horizon-0.1.2/tests/test_anonymizer_complex.py` & `prompt-horizon-0.1.3/tests/test_anonymizer_complex.py`

 * *Files identical despite different names*

### Comparing `prompt-horizon-0.1.2/tests/test_de_anonymizer.py` & `prompt-horizon-0.1.3/tests/test_de_anonymizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,9 +68,21 @@
         deanonymized_json = de_anonymize(temp_anonymized_file_path, map_object=map_object)
 
         self.assertEqual(deanonymized_json, expected_deanonymized_json)
 
         # Clean up the temporary file
         os.remove(temp_anonymized_file_path)
 
+    def test_de_anonymize_values_only(self):
+        input_json = {"name": "John", "age": 30, "city": "New York"}
+        expected_deanonymized_json = {"name": "John", "age": 30, "city": "New York"}
+
+        # Anonymize the input JSON with only values
+        anonymized_json, map_object = anonymize(input_json, anonymize_keys=False)
+
+        deanonymized_json = de_anonymize(anonymized_json, map_object=map_object)
+
+        self.assertEqual(deanonymized_json, expected_deanonymized_json)
+
+
 if __name__ == '__main__':
     unittest.main()
```

