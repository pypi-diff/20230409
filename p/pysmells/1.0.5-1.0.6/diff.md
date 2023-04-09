# Comparing `tmp/pysmells-1.0.5.tar.gz` & `tmp/pysmells-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmells-1.0.5.tar", last modified: Sat Apr  8 17:12:16 2023, max compression
+gzip compressed data, was "pysmells-1.0.6.tar", last modified: Sun Apr  9 11:56:50 2023, max compression
```

## Comparing `pysmells-1.0.5.tar` & `pysmells-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-08 17:12:16.945591 pysmells-1.0.5/
--rw-r--r--   0 marcossousa   (501) staff       (20)     1115 2023-04-07 23:01:55.000000 pysmells-1.0.5/LICENSE
--rw-r--r--   0 marcossousa   (501) staff       (20)     2143 2023-04-08 17:12:16.944827 pysmells-1.0.5/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)     1131 2023-04-07 23:28:38.000000 pysmells-1.0.5/README.md
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-08 17:12:16.929927 pysmells-1.0.5/pysmells/
--rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-04-07 22:10:03.000000 pysmells-1.0.5/pysmells/__init__.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     3459 2023-04-08 00:31:24.000000 pysmells-1.0.5/pysmells/analyze.py
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-08 17:12:16.942210 pysmells-1.0.5/pysmells.egg-info/
--rw-r--r--   0 marcossousa   (501) staff       (20)     2143 2023-04-08 17:12:16.000000 pysmells-1.0.5/pysmells.egg-info/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)      261 2023-04-08 17:12:16.000000 pysmells-1.0.5/pysmells.egg-info/SOURCES.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-04-08 17:12:16.000000 pysmells-1.0.5/pysmells.egg-info/dependency_links.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       44 2023-04-08 17:12:16.000000 pysmells-1.0.5/pysmells.egg-info/entry_points.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       21 2023-04-08 17:12:16.000000 pysmells-1.0.5/pysmells.egg-info/requires.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)        9 2023-04-08 17:12:16.000000 pysmells-1.0.5/pysmells.egg-info/top_level.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-04-08 17:12:16.945993 pysmells-1.0.5/setup.cfg
--rw-r--r--   0 marcossousa   (501) staff       (20)     1398 2023-04-08 17:12:01.000000 pysmells-1.0.5/setup.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-09 11:56:50.729267 pysmells-1.0.6/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1115 2023-04-07 23:01:55.000000 pysmells-1.0.6/LICENSE
+-rw-r--r--   0 marcossousa   (501) staff       (20)     2169 2023-04-09 11:56:50.728026 pysmells-1.0.6/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1131 2023-04-07 23:28:38.000000 pysmells-1.0.6/README.md
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-09 11:56:50.719250 pysmells-1.0.6/pysmells/
+-rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-04-07 22:10:03.000000 pysmells-1.0.6/pysmells/__init__.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     3852 2023-04-09 11:51:48.000000 pysmells-1.0.6/pysmells/pysmells.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-09 11:56:50.726858 pysmells-1.0.6/pysmells.egg-info/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     2169 2023-04-09 11:56:50.000000 pysmells-1.0.6/pysmells.egg-info/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)      262 2023-04-09 11:56:50.000000 pysmells-1.0.6/pysmells.egg-info/SOURCES.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-04-09 11:56:50.000000 pysmells-1.0.6/pysmells.egg-info/dependency_links.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       44 2023-04-09 11:56:50.000000 pysmells-1.0.6/pysmells.egg-info/entry_points.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       21 2023-04-09 11:56:50.000000 pysmells-1.0.6/pysmells.egg-info/requires.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)        9 2023-04-09 11:56:50.000000 pysmells-1.0.6/pysmells.egg-info/top_level.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-04-09 11:56:50.730623 pysmells-1.0.6/setup.cfg
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1424 2023-04-08 18:38:59.000000 pysmells-1.0.6/setup.py
```

### Comparing `pysmells-1.0.5/LICENSE` & `pysmells-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmells-1.0.5/PKG-INFO` & `pysmells-1.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pysmells
-Version: 1.0.5
-Summary: A Python code analysis tool that checks for programming errors, inconsistencies, and programming style violations, as well as the correctness of type annotations in programs. The pysmells tool is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 20, PEP 257, PEP 484, PEP 526, PEP 544, PEP 561, PEP 563, and PEP 589.
+Version: 1.0.6
+Summary: Pysmells is a tool that identifies when something doesn't 'smell right' in a python code, checking for programming errors, inconsistencies, programming style violations and the correctness of type annotations. Pysmells is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 20, PEP 257, PEP 484, PEP 526, PEP 544, PEP 561, PEP 563, and PEP 589.
 Home-page: https://github.com/pysmells/pysmells
 Author: Marcos Paulo Alves de Sousa and Marco Aurélio Proença Neto
 Author-email: msousa@museu-goeldi.br
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pysmells-1.0.5/README.md` & `pysmells-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pysmells-1.0.5/pysmells/analyze.py` & `pysmells-1.0.6/pysmells/pysmells.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
 import re
+import argparse
 import subprocess
+import csv
 from collections import Counter, defaultdict
 from tabulate import tabulate
 
 
 def check_type_annotations(file_path):
     with open(file_path, "r") as file:
         content = file.read()
@@ -44,53 +46,64 @@
             alert_code = match.group(0)
             alert_type = alert_code[0]
             alert_count[alert_type] += 1
             alert_details[alert_type].append(alert_code)
 
     total_alerts = sum(alert_count.values())
     # Update the table data structure
-    table_row = [directory, file_path, total_alerts]
+    table_row = [file_path, total_alerts]
     for alert_type in alert_type_names.keys():
         table_row.append(alert_count[alert_type])
 
     table_row.append(", ".join(sorted(set(alert_code for alert_codes in alert_details.values() for alert_code in alert_codes))))
     table_row.append("Yes" if type_annotations_present else "No")  # Adds the "Adopt Type Annotations?" field
 
     # Run Mypy
     mypy_process = subprocess.run(["mypy", file_path], stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
                                   universal_newlines=True, check=False)
     mypy_output = mypy_process.stdout
 
-    table_row.append(mypy_output if type_annotations_present else "None")  # Adds the "Type Annotations Description" field
+    mypy_output_no_newline = mypy_output.replace('\n', ' | ')
+    table_row.append(mypy_output_no_newline if type_annotations_present else "None")  # Adds the "Type Annotations Description" field
     table_data.append(table_row)
 
-    print(f"\nFile '{file_path}' {'adopts' if type_annotations_present else 'does not adopt'} Type Annotations.\n")
-    print("========================================\n")
-
-    print("\nMypy analysis result:")
-    print(mypy_output)
-
     return total_alerts
 
+def export_to_csv(table_data, headers, csv_output):
+    with open(csv_output, 'w', newline='') as csvfile:
+        csv_writer = csv.writer(csvfile)
+        csv_writer.writerow(headers)
+        for row in table_data:
+            csv_writer.writerow(row)
 
 def main():
-    root_directory = input("Enter the directory path containing the Python files to analyze: ")
+    parser = argparse.ArgumentParser(description="Analyze Python files in the specified directory.")
+    parser.add_argument("directory", help="The directory path containing the Python files to analyze.")
+    parser.add_argument("-o", "--output", help="The path and file name for the CSV output.", type=str)
+
+    args = parser.parse_args()
+    root_directory = args.directory
+    csv_output = args.output
 
     table_data = []
     total_alerts_directory = 0
 
     for root, dirs, files in os.walk(root_directory):
         for file_name in files:
             if file_name.endswith(".py"):
                 file_path = os.path.join(root, file_name)
                 total_alerts_directory += analyze_file(root, file_path, table_data)
 
     print(f"\nTotal alerts found in the directory: {total_alerts_directory}\n")
-    print(tabulate(table_data, headers=["Directory", "File",
-                                        "Total Alerts", "Convention", "Refactor",
-                                        "Warning", "Error", "Fatal", "Alert Codes",
-                                        "Adopt Type Annotations?",
-                                        "Type Annotations Description"],
-                   tablefmt="grid"))
+    headers = ["File", "Total Alerts", "Convention", "Refactor", "Warning", "Error", "Fatal", "Alert Codes",
+               "Adopt Type Annotations?", "Type Annotations Description"]
+    print(tabulate(table_data, headers=headers, tablefmt="grid"))
+
+    if csv_output:
+        export_to_csv(table_data, headers, csv_output)
+        print(f"CSV file exported to: {csv_output}")
 
 if __name__ == "__main__":
     main()
+
+
+
```

### Comparing `pysmells-1.0.5/pysmells.egg-info/PKG-INFO` & `pysmells-1.0.6/pysmells.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pysmells
-Version: 1.0.5
-Summary: A Python code analysis tool that checks for programming errors, inconsistencies, and programming style violations, as well as the correctness of type annotations in programs. The pysmells tool is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 20, PEP 257, PEP 484, PEP 526, PEP 544, PEP 561, PEP 563, and PEP 589.
+Version: 1.0.6
+Summary: Pysmells is a tool that identifies when something doesn't 'smell right' in a python code, checking for programming errors, inconsistencies, programming style violations and the correctness of type annotations. Pysmells is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 20, PEP 257, PEP 484, PEP 526, PEP 544, PEP 561, PEP 563, and PEP 589.
 Home-page: https://github.com/pysmells/pysmells
 Author: Marcos Paulo Alves de Sousa and Marco Aurélio Proença Neto
 Author-email: msousa@museu-goeldi.br
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pysmells-1.0.5/setup.py` & `pysmells-1.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pysmells",
-    version="1.0.5",
+    version="1.0.6",
     author="Marcos Paulo Alves de Sousa and Marco Aurélio Proença Neto",
     author_email="msousa@museu-goeldi.br",
-    description="A Python code analysis tool that checks for programming errors, inconsistencies, and programming style violations, as well as the correctness of type annotations in programs. The pysmells tool is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 20, PEP 257, PEP 484, PEP 526, PEP 544, PEP 561, PEP 563, and PEP 589.",
+    description="Pysmells is a tool that identifies when something doesn't 'smell right' in a python code, checking for programming errors, inconsistencies, programming style violations and the correctness of type annotations. Pysmells is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 20, PEP 257, PEP 484, PEP 526, PEP 544, PEP 561, PEP 563, and PEP 589.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pysmells/pysmells",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

