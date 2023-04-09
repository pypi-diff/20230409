# Comparing `tmp/pun_cli-0.1.0.tar.gz` & `tmp/pun_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pun_cli-0.1.0.tar", max compression
+gzip compressed data, was "pun_cli-0.1.1.tar", max compression
```

## Comparing `pun_cli-0.1.0.tar` & `pun_cli-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2023-04-09 20:56:41.961148 pun_cli-0.1.0/LICENSE
--rw-r--r--   0        0        0     1208 2023-04-09 21:16:56.021875 pun_cli-0.1.0/README.md
--rw-r--r--   0        0        0       23 2023-04-09 21:31:55.530381 pun_cli-0.1.0/pun_cli/__init__.py
--rw-r--r--   0        0        0     1556 2023-04-09 21:32:25.629870 pun_cli-0.1.0/pun_cli/main.py
--rw-r--r--   0        0        0      961 2023-04-09 21:18:15.332400 pun_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 pun_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-09 20:56:41.961148 pun_cli-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1208 2023-04-09 21:16:56.021875 pun_cli-0.1.1/README.md
+-rw-r--r--   0        0        0       23 2023-04-09 21:31:55.530381 pun_cli-0.1.1/pun_cli/__init__.py
+-rw-r--r--   0        0        0     1658 2023-04-09 21:43:11.827713 pun_cli-0.1.1/pun_cli/main.py
+-rw-r--r--   0        0        0      977 2023-04-09 21:43:06.087693 pun_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2288 1970-01-01 00:00:00.000000 pun_cli-0.1.1/PKG-INFO
```

### Comparing `pun_cli-0.1.0/LICENSE` & `pun_cli-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pun_cli-0.1.0/README.md` & `pun_cli-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pun_cli-0.1.0/pun_cli/main.py` & `pun_cli-0.1.1/pun_cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import random
 import argparse
 import requests
+import cowsay
 
 PUN_REPOSITORY = 'https://raw.githubusercontent.com/thevahidal/pun-cli/main/pun_repository.txt'
-VERSION = 'v' + '0.1.0'
+VERSION = 'v' + '0.1.1'
 
 def get_puns():
     try:
         response = requests.get(PUN_REPOSITORY)
         puns = response.text.split('\n')
         puns = [pun.strip() for pun in puns if pun.strip() != '']
         return puns
@@ -40,12 +41,13 @@
     if args.add:
         print("Thanks for your contribution!")
         print("Please create a pull request to add your pun to the repository.")
         print("https://github.com/thevahidal/pun-cli")
 
     else:
       pun = generate_pun(args.keyword)
+      character = random.choice(cowsay.char_names)
+      print(cowsay.get_output_string(character, pun))
 
-      print(pun)
 
 if __name__ == '__main__':
     main()
```

### Comparing `pun_cli-0.1.0/pyproject.toml` & `pun_cli-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pun-cli"
-version = "0.1.0"
+version = "0.1.1"
 description = "Pun-CLI: Because you can't resist a good pun. Generate hilarious puns from our pun repository or contribute your own puns to the list. Pun-CLI, the command-line tool you never knew you needed."
 authors = ["Vahid Al <thevahidal@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pun_cli"}]
 license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -19,12 +19,13 @@
     "Topic :: Utilities",
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.28.2"
+cowsay = "^5.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pun_cli-0.1.0/PKG-INFO` & `pun_cli-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pun-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pun-CLI: Because you can't resist a good pun. Generate hilarious puns from our pun repository or contribute your own puns to the list. Pun-CLI, the command-line tool you never knew you needed.
 License: MIT
 Author: Vahid Al
 Author-email: thevahidal@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
+Requires-Dist: cowsay (>=5.0,<6.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Pun CLI
 
 `pun-cli` is a Python-based command-line tool that generates a random pun based on a given keyword.
```

