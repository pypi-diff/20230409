# Comparing `tmp/pun_cli-0.1.1.tar.gz` & `tmp/pun_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pun_cli-0.1.1.tar", max compression
+gzip compressed data, was "pun_cli-0.1.2.tar", max compression
```

## Comparing `pun_cli-0.1.1.tar` & `pun_cli-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2023-04-09 20:56:41.961148 pun_cli-0.1.1/LICENSE
--rw-r--r--   0        0        0     1208 2023-04-09 21:16:56.021875 pun_cli-0.1.1/README.md
--rw-r--r--   0        0        0       23 2023-04-09 21:31:55.530381 pun_cli-0.1.1/pun_cli/__init__.py
--rw-r--r--   0        0        0     1658 2023-04-09 21:43:11.827713 pun_cli-0.1.1/pun_cli/main.py
--rw-r--r--   0        0        0      977 2023-04-09 21:43:06.087693 pun_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2288 1970-01-01 00:00:00.000000 pun_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-09 20:56:41.961148 pun_cli-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1208 2023-04-09 21:16:56.021875 pun_cli-0.1.2/README.md
+-rw-r--r--   0        0        0       23 2023-04-09 21:31:55.530381 pun_cli-0.1.2/pun_cli/__init__.py
+-rw-r--r--   0        0        0     1925 2023-04-09 21:53:24.841205 pun_cli-0.1.2/pun_cli/main.py
+-rw-r--r--   0        0        0      977 2023-04-09 21:53:29.317261 pun_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2288 1970-01-01 00:00:00.000000 pun_cli-0.1.2/PKG-INFO
```

### Comparing `pun_cli-0.1.1/LICENSE` & `pun_cli-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pun_cli-0.1.1/README.md` & `pun_cli-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pun_cli-0.1.1/pun_cli/main.py` & `pun_cli-0.1.2/pun_cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import random
 import argparse
 import requests
 import cowsay
 
 PUN_REPOSITORY = 'https://raw.githubusercontent.com/thevahidal/pun-cli/main/pun_repository.txt'
-VERSION = 'v' + '0.1.1'
+VERSION = 'v' + '0.1.2'
 
 def get_puns():
     try:
         response = requests.get(PUN_REPOSITORY)
         puns = response.text.split('\n')
         puns = [pun.strip() for pun in puns if pun.strip() != '']
         return puns
@@ -27,27 +27,32 @@
         if len(puns) == 0:
             print('No puns found for keyword:', keyword)
             return ''
 
     return random.choice(puns)
 
 def main():
-    parser = argparse.ArgumentParser(description='Generate a random pun.')
+    parser = argparse.ArgumentParser(description='Unleash hilarious wordplay with a single command.')
     parser.add_argument('--keyword', '-k', help='Keyword to search for puns.')
-    parser.add_argument('--version', '-v', action='version', version='%(prog)s ' + VERSION, help='Print version and exit.')
+    parser.add_argument('--character', '-c', help='Character to use for the pun. One of: ' + ', '.join(cowsay.char_names))
     parser.add_argument('--add', '-a', help='Add a pun to the repository.', action='store_true')
+    parser.add_argument('--version', '-v', action='version', version='%(prog)s ' + VERSION, help='Print version and exit.')
 
     args = parser.parse_args()
 
     if args.add:
         print("Thanks for your contribution!")
         print("Please create a pull request to add your pun to the repository.")
         print("https://github.com/thevahidal/pun-cli")
 
     else:
       pun = generate_pun(args.keyword)
-      character = random.choice(cowsay.char_names)
+      if args.character and args.character in cowsay.char_names:
+          character = args.character
+      else:
+        character = random.choice(cowsay.char_names)
+
       print(cowsay.get_output_string(character, pun))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pun_cli-0.1.1/pyproject.toml` & `pun_cli-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pun-cli"
-version = "0.1.1"
+version = "0.1.2"
 description = "Pun-CLI: Because you can't resist a good pun. Generate hilarious puns from our pun repository or contribute your own puns to the list. Pun-CLI, the command-line tool you never knew you needed."
 authors = ["Vahid Al <thevahidal@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pun_cli"}]
 license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `pun_cli-0.1.1/PKG-INFO` & `pun_cli-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pun-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pun-CLI: Because you can't resist a good pun. Generate hilarious puns from our pun repository or contribute your own puns to the list. Pun-CLI, the command-line tool you never knew you needed.
 License: MIT
 Author: Vahid Al
 Author-email: thevahidal@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

