# Comparing `tmp/sara_compis1_tools-0.0.2.tar.gz` & `tmp/sara_compis1_tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sara_compis1_tools-0.0.2.tar", last modified: Sun Apr  9 00:57:06 2023, max compression
+gzip compressed data, was "sara_compis1_tools-0.0.3.tar", last modified: Sun Apr  9 02:31:18 2023, max compression
```

## Comparing `sara_compis1_tools-0.0.2.tar` & `sara_compis1_tools-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 00:57:06.239431 sara_compis1_tools-0.0.2/
--rw-rw-rw-   0        0        0       80 2023-04-09 00:51:27.000000 sara_compis1_tools-0.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1065 2023-04-08 22:44:28.000000 sara_compis1_tools-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2023-04-08 22:41:49.000000 sara_compis1_tools-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      681 2023-04-09 00:57:06.236370 sara_compis1_tools-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      101 2023-04-08 22:40:09.000000 sara_compis1_tools-0.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-09 00:57:06.209797 sara_compis1_tools-0.0.2/sara_compis1_tools/
--rw-rw-rw-   0        0        0     5933 2023-04-07 03:05:16.000000 sara_compis1_tools-0.0.2/sara_compis1_tools/Format.py
--rw-rw-rw-   0        0        0      437 2023-04-09 00:48:21.000000 sara_compis1_tools-0.0.2/sara_compis1_tools/Lex_gen.py
--rw-rw-rw-   0        0        0      223 2023-03-07 18:50:14.000000 sara_compis1_tools-0.0.2/sara_compis1_tools/StateAFD.py
--rw-rw-rw-   0        0        0     1559 2023-03-06 05:32:15.000000 sara_compis1_tools-0.0.2/sara_compis1_tools/Syntax.py
--rw-rw-rw-   0        0        0        0 2023-04-08 21:45:17.000000 sara_compis1_tools-0.0.2/sara_compis1_tools/__init__.py
--rw-rw-rw-   0        0        0    19116 2023-04-09 00:32:31.000000 sara_compis1_tools-0.0.2/sara_compis1_tools/directAFD.py
--rw-rw-rw-   0        0        0    11129 2023-04-09 00:50:00.000000 sara_compis1_tools-0.0.2/sara_compis1_tools/readLex.py
-drwxrwxrwx   0        0        0        0 2023-04-09 00:57:06.231778 sara_compis1_tools-0.0.2/sara_compis1_tools.egg-info/
--rw-rw-rw-   0        0        0      681 2023-04-09 00:57:05.000000 sara_compis1_tools-0.0.2/sara_compis1_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      478 2023-04-09 00:57:06.000000 sara_compis1_tools-0.0.2/sara_compis1_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 00:57:05.000000 sara_compis1_tools-0.0.2/sara_compis1_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-09 00:57:05.000000 sara_compis1_tools-0.0.2/sara_compis1_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-09 00:57:05.000000 sara_compis1_tools-0.0.2/sara_compis1_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 00:57:06.239431 sara_compis1_tools-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      790 2023-04-09 00:51:52.000000 sara_compis1_tools-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 02:31:18.775308 sara_compis1_tools-0.0.3/
+-rw-rw-rw-   0        0        0       92 2023-04-09 02:22:21.000000 sara_compis1_tools-0.0.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1065 2023-04-08 22:44:28.000000 sara_compis1_tools-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-04-08 22:41:49.000000 sara_compis1_tools-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      693 2023-04-09 02:31:18.771640 sara_compis1_tools-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      101 2023-04-08 22:40:09.000000 sara_compis1_tools-0.0.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 02:31:18.741548 sara_compis1_tools-0.0.3/sara_compis1_tools/
+-rw-rw-rw-   0        0        0     5933 2023-04-07 03:05:16.000000 sara_compis1_tools-0.0.3/sara_compis1_tools/Format.py
+-rw-rw-rw-   0        0        0      223 2023-03-07 18:50:14.000000 sara_compis1_tools-0.0.3/sara_compis1_tools/StateAFD.py
+-rw-rw-rw-   0        0        0     1559 2023-03-06 05:32:15.000000 sara_compis1_tools-0.0.3/sara_compis1_tools/Syntax.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 21:45:17.000000 sara_compis1_tools-0.0.3/sara_compis1_tools/__init__.py
+-rw-rw-rw-   0        0        0    19116 2023-04-09 00:32:31.000000 sara_compis1_tools-0.0.3/sara_compis1_tools/directAFD.py
+-rw-rw-rw-   0        0        0      356 2023-04-09 02:19:40.000000 sara_compis1_tools-0.0.3/sara_compis1_tools/generated.py
+-rw-rw-rw-   0        0        0    11751 2023-04-09 02:19:36.000000 sara_compis1_tools-0.0.3/sara_compis1_tools/lexGen.py
+drwxrwxrwx   0        0        0        0 2023-04-09 02:31:18.766783 sara_compis1_tools-0.0.3/sara_compis1_tools.egg-info/
+-rw-rw-rw-   0        0        0      693 2023-04-09 02:31:18.000000 sara_compis1_tools-0.0.3/sara_compis1_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      479 2023-04-09 02:31:18.000000 sara_compis1_tools-0.0.3/sara_compis1_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 02:31:18.000000 sara_compis1_tools-0.0.3/sara_compis1_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-09 02:31:18.000000 sara_compis1_tools-0.0.3/sara_compis1_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-09 02:31:18.000000 sara_compis1_tools-0.0.3/sara_compis1_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 02:31:18.775308 sara_compis1_tools-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      790 2023-04-09 02:22:52.000000 sara_compis1_tools-0.0.3/setup.py
```

### Comparing `sara_compis1_tools-0.0.2/LICENSE.txt` & `sara_compis1_tools-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.2/PKG-INFO` & `sara_compis1_tools-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sara_compis1_tools
-Version: 0.0.2
+Version: 0.0.3
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
 
-0.0.2 (08/04/2023)
+0.0.3 (08/04/2023)
 ------------------
-- Minor Fixes
+- Considering more cases.
```

### Comparing `sara_compis1_tools-0.0.2/sara_compis1_tools/Format.py` & `sara_compis1_tools-0.0.3/sara_compis1_tools/Format.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.2/sara_compis1_tools/Syntax.py` & `sara_compis1_tools-0.0.3/sara_compis1_tools/Syntax.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.2/sara_compis1_tools/directAFD.py` & `sara_compis1_tools-0.0.3/sara_compis1_tools/directAFD.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.2/sara_compis1_tools/readLex.py` & `sara_compis1_tools-0.0.3/sara_compis1_tools/lexGen.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,14 +151,18 @@
                     else:
                         if '-' in content:
                             if content.count('-') > 1:
                                 raise Exception("Formato de regex incorrecto,"+ "linea " + str(token.line_no))
                             start, end = content.split('-')
                             elements = self.range_maker(start, end, token.line_no)
                             content = '|'.join(elements)
+                        elif '-' not in content:
+                            content = content[1:-1]
+                            elements = [content[i] for i in range(len(content))]
+                            content = '|'.join(elements)
                     new_regex += '(' + content + ')'
                     i = j
                 else:
                     check = ""
                     j = i
                     while token.regex[j] not in ['+', '*', '?']:
                         check += token.regex[j]
@@ -237,15 +241,18 @@
                 node_attrs.update({'color': 'green', 'style': 'filled'})
             if state.accepting:
                 node_attrs.update({'peripheries': '2'})
             G.add_node(str(state.name), **node_attrs)
 
             for transition, final_dest in state.transitions.items():
                 G.add_node(str(final_dest))
-                G.add_edge(str(state.name), str(final_dest), label=str(chr(int(transition))), dir='forward')
+                if int(transition) in [n for n in range(0, 35)]:
+                    G.add_edge(str(state.name), str(final_dest), label=transition, dir='forward')    
+                else:
+                    G.add_edge(str(state.name), str(final_dest), label=str(chr(int(transition))), dir='forward')
 
         dot = Digraph()
         for u, v, data in G.edges(data=True):
             dot.edge(u, v, label=data['label'], dir=data['dir'])
         for node in G.nodes:
             attrs = G.nodes[node]
             dot.node(node, **attrs)
@@ -289,19 +296,27 @@
         self.surround_dot()
         self.replace_tokens()
     
 
 
     
 if __name__ == '__main__':
+    
+        script_content = '''
+import sys
+import sara_compis1_tools.lexGen as tool
+
+if len(sys.argv) < 2:
+    print("Por favor ingrese el archivo .yal")
+    sys.exit(1)
+
+yal_file = sys.argv[1]
+lex_var = tool.Lexer(yal_file)
+lex_var.read()
+mega_content = lex_var.generate_automatas()
+mega_automata = lex_var.unify(mega_content)
+lex_var.draw_mega_afd(mega_automata)
+        '''
+
+        with open('generated.py', 'w') as script_file:
+            script_file.write(script_content)
 
-    if len(sys.argv) < 2:
-        print("Por favor ingrese el archivo .yal")
-        sys.exit(1)
-
-    yal_file = sys.argv[1]
-    lexer = Lexer(yal_file)
-    
-    lexer.read()
-    mega_content = lexer.generate_automatas()
-    mega_automata = lexer.unify(mega_content)
-    lexer.draw_mega_afd(mega_automata)
```

### Comparing `sara_compis1_tools-0.0.2/sara_compis1_tools.egg-info/PKG-INFO` & `sara_compis1_tools-0.0.3/sara_compis1_tools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sara-compis1-tools
-Version: 0.0.2
+Version: 0.0.3
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
 
-0.0.2 (08/04/2023)
+0.0.3 (08/04/2023)
 ------------------
-- Minor Fixes
+- Considering more cases.
```

### Comparing `sara_compis1_tools-0.0.2/setup.py` & `sara_compis1_tools-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sara_compis1_tools',
-    version='0.0.2',
+    version='0.0.3',
     description='A collection of tools for the Language Design course',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='https://github.com/MGonza20/Compis_Lab3',
     author='Sara Paguaga',
     author_email='sara.paguaga@gmail.com',
     license='MIT',
     classifiers=[
```

