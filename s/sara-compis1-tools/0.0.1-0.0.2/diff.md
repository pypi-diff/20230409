# Comparing `tmp/sara_compis1_tools-0.0.1.tar.gz` & `tmp/sara_compis1_tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sara_compis1_tools-0.0.1.tar", last modified: Sat Apr  8 23:01:35 2023, max compression
+gzip compressed data, was "sara_compis1_tools-0.0.2.tar", last modified: Sun Apr  9 00:57:06 2023, max compression
```

## Comparing `sara_compis1_tools-0.0.1.tar` & `sara_compis1_tools-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 23:01:35.973477 sara_compis1_tools-0.0.1/
--rw-rw-rw-   0        0        0       82 2023-04-08 22:38:05.000000 sara_compis1_tools-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1065 2023-04-08 22:44:28.000000 sara_compis1_tools-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2023-04-08 22:41:49.000000 sara_compis1_tools-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      683 2023-04-08 23:01:35.969953 sara_compis1_tools-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      101 2023-04-08 22:40:09.000000 sara_compis1_tools-0.0.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-08 23:01:35.936728 sara_compis1_tools-0.0.1/sara_compis1_tools/
--rw-rw-rw-   0        0        0     5933 2023-04-07 03:05:16.000000 sara_compis1_tools-0.0.1/sara_compis1_tools/Format.py
--rw-rw-rw-   0        0        0      223 2023-03-07 18:50:14.000000 sara_compis1_tools-0.0.1/sara_compis1_tools/StateAFD.py
--rw-rw-rw-   0        0        0     1559 2023-03-06 05:32:15.000000 sara_compis1_tools-0.0.1/sara_compis1_tools/Syntax.py
--rw-rw-rw-   0        0        0        0 2023-04-08 21:45:17.000000 sara_compis1_tools-0.0.1/sara_compis1_tools/__init__.py
--rw-rw-rw-   0        0        0    19120 2023-04-08 21:53:35.000000 sara_compis1_tools-0.0.1/sara_compis1_tools/directAFD.py
--rw-rw-rw-   0        0        0    11131 2023-04-08 21:16:18.000000 sara_compis1_tools-0.0.1/sara_compis1_tools/readLex.py
-drwxrwxrwx   0        0        0        0 2023-04-08 23:01:35.965068 sara_compis1_tools-0.0.1/sara_compis1_tools.egg-info/
--rw-rw-rw-   0        0        0      683 2023-04-08 23:01:35.000000 sara_compis1_tools-0.0.1/sara_compis1_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-04-08 23:01:35.000000 sara_compis1_tools-0.0.1/sara_compis1_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 23:01:35.000000 sara_compis1_tools-0.0.1/sara_compis1_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-08 23:01:35.000000 sara_compis1_tools-0.0.1/sara_compis1_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-08 23:01:35.000000 sara_compis1_tools-0.0.1/sara_compis1_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 23:01:35.974241 sara_compis1_tools-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      790 2023-04-08 23:01:28.000000 sara_compis1_tools-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 00:57:06.239431 sara_compis1_tools-0.0.2/
+-rw-rw-rw-   0        0        0       80 2023-04-09 00:51:27.000000 sara_compis1_tools-0.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1065 2023-04-08 22:44:28.000000 sara_compis1_tools-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-04-08 22:41:49.000000 sara_compis1_tools-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      681 2023-04-09 00:57:06.236370 sara_compis1_tools-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      101 2023-04-08 22:40:09.000000 sara_compis1_tools-0.0.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 00:57:06.209797 sara_compis1_tools-0.0.2/sara_compis1_tools/
+-rw-rw-rw-   0        0        0     5933 2023-04-07 03:05:16.000000 sara_compis1_tools-0.0.2/sara_compis1_tools/Format.py
+-rw-rw-rw-   0        0        0      437 2023-04-09 00:48:21.000000 sara_compis1_tools-0.0.2/sara_compis1_tools/Lex_gen.py
+-rw-rw-rw-   0        0        0      223 2023-03-07 18:50:14.000000 sara_compis1_tools-0.0.2/sara_compis1_tools/StateAFD.py
+-rw-rw-rw-   0        0        0     1559 2023-03-06 05:32:15.000000 sara_compis1_tools-0.0.2/sara_compis1_tools/Syntax.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 21:45:17.000000 sara_compis1_tools-0.0.2/sara_compis1_tools/__init__.py
+-rw-rw-rw-   0        0        0    19116 2023-04-09 00:32:31.000000 sara_compis1_tools-0.0.2/sara_compis1_tools/directAFD.py
+-rw-rw-rw-   0        0        0    11129 2023-04-09 00:50:00.000000 sara_compis1_tools-0.0.2/sara_compis1_tools/readLex.py
+drwxrwxrwx   0        0        0        0 2023-04-09 00:57:06.231778 sara_compis1_tools-0.0.2/sara_compis1_tools.egg-info/
+-rw-rw-rw-   0        0        0      681 2023-04-09 00:57:05.000000 sara_compis1_tools-0.0.2/sara_compis1_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2023-04-09 00:57:06.000000 sara_compis1_tools-0.0.2/sara_compis1_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 00:57:05.000000 sara_compis1_tools-0.0.2/sara_compis1_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-09 00:57:05.000000 sara_compis1_tools-0.0.2/sara_compis1_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-09 00:57:05.000000 sara_compis1_tools-0.0.2/sara_compis1_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 00:57:06.239431 sara_compis1_tools-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      790 2023-04-09 00:51:52.000000 sara_compis1_tools-0.0.2/setup.py
```

### Comparing `sara_compis1_tools-0.0.1/LICENSE.txt` & `sara_compis1_tools-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.1/PKG-INFO` & `sara_compis1_tools-0.0.2/sara_compis1_tools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sara_compis1_tools
-Version: 0.0.1
+Name: sara-compis1-tools
+Version: 0.0.2
 Summary: A collection of tools for the Language Design course
 Home-page: https://github.com/MGonza20/Compis_Lab3
 Author: Sara Paguaga
 Author-email: sara.paguaga@gmail.com
 License: MIT
 Keywords: Compiler
 Classifier: Development Status :: 3 - Alpha
@@ -14,10 +14,10 @@
 License-File: LICENSE.txt
 
 This is collection of tools for the Language Design course to be able to generate a lexical analyzer.
 
 Change Log
 ===========
 
-0.0.1 (08/04/2023)
+0.0.2 (08/04/2023)
 ------------------
-- First Release
+- Minor Fixes
```

### Comparing `sara_compis1_tools-0.0.1/sara_compis1_tools/Format.py` & `sara_compis1_tools-0.0.2/sara_compis1_tools/Format.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.1/sara_compis1_tools/Syntax.py` & `sara_compis1_tools-0.0.2/sara_compis1_tools/Syntax.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.1/sara_compis1_tools/directAFD.py` & `sara_compis1_tools-0.0.2/sara_compis1_tools/directAFD.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-
 import os
 import networkx as nx
 from graphviz import Digraph
 
-
 from Format import Format
 os.environ["PATH"] += os.pathsep + 'C:/Program Files (x86)/Graphviz/bin'    
 from StateAFD import StateAFD
 
 
 class Node:
     def __init__(self, symbol, parent = None, left = None, right = None, no = None, anulable = False, firstpos = [], lastpos = []):
```

### Comparing `sara_compis1_tools-0.0.1/sara_compis1_tools/readLex.py` & `sara_compis1_tools-0.0.2/sara_compis1_tools/readLex.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,19 +252,19 @@
 
         dot.render('mega/megaautomata', format='png')
 
     
     def generate_automatas(self):
         mega_content = []
         count = 0
-        for token in lexer.tokens:
+        for token in self.tokens:
             ff = Format(token.regex)
             token.regex = ff.positiveId(token.regex + '#')
             token.regex = ff.zeroOrOneId(token.regex)
-            token.regex = lexer.remove_double_parentheses(token.regex)
+            token.regex = self.remove_double_parentheses(token.regex)
             token.regex = ff.concat(token.regex)
             
             afdd = AFD(token)
             new_afd = afdd.generateAFD(count)
             mega_content.append(new_afd)
             count += len(new_afd)
         return mega_content
```

### Comparing `sara_compis1_tools-0.0.1/setup.py` & `sara_compis1_tools-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sara_compis1_tools',
-    version='0.0.1',
+    version='0.0.2',
     description='A collection of tools for the Language Design course',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='https://github.com/MGonza20/Compis_Lab3',
     author='Sara Paguaga',
     author_email='sara.paguaga@gmail.com',
     license='MIT',
     classifiers=[
```

