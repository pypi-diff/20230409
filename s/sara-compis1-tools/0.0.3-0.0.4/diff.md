# Comparing `tmp/sara_compis1_tools-0.0.3.tar.gz` & `tmp/sara_compis1_tools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sara_compis1_tools-0.0.3.tar", last modified: Sun Apr  9 02:31:18 2023, max compression
+gzip compressed data, was "sara_compis1_tools-0.0.4.tar", last modified: Sun Apr  9 04:39:15 2023, max compression
```

## Comparing `sara_compis1_tools-0.0.3.tar` & `sara_compis1_tools-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 02:31:18.775308 sara_compis1_tools-0.0.3/
--rw-rw-rw-   0        0        0       92 2023-04-09 02:22:21.000000 sara_compis1_tools-0.0.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1065 2023-04-08 22:44:28.000000 sara_compis1_tools-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2023-04-08 22:41:49.000000 sara_compis1_tools-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      693 2023-04-09 02:31:18.771640 sara_compis1_tools-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      101 2023-04-08 22:40:09.000000 sara_compis1_tools-0.0.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-09 02:31:18.741548 sara_compis1_tools-0.0.3/sara_compis1_tools/
--rw-rw-rw-   0        0        0     5933 2023-04-07 03:05:16.000000 sara_compis1_tools-0.0.3/sara_compis1_tools/Format.py
--rw-rw-rw-   0        0        0      223 2023-03-07 18:50:14.000000 sara_compis1_tools-0.0.3/sara_compis1_tools/StateAFD.py
--rw-rw-rw-   0        0        0     1559 2023-03-06 05:32:15.000000 sara_compis1_tools-0.0.3/sara_compis1_tools/Syntax.py
--rw-rw-rw-   0        0        0        0 2023-04-08 21:45:17.000000 sara_compis1_tools-0.0.3/sara_compis1_tools/__init__.py
--rw-rw-rw-   0        0        0    19116 2023-04-09 00:32:31.000000 sara_compis1_tools-0.0.3/sara_compis1_tools/directAFD.py
--rw-rw-rw-   0        0        0      356 2023-04-09 02:19:40.000000 sara_compis1_tools-0.0.3/sara_compis1_tools/generated.py
--rw-rw-rw-   0        0        0    11751 2023-04-09 02:19:36.000000 sara_compis1_tools-0.0.3/sara_compis1_tools/lexGen.py
-drwxrwxrwx   0        0        0        0 2023-04-09 02:31:18.766783 sara_compis1_tools-0.0.3/sara_compis1_tools.egg-info/
--rw-rw-rw-   0        0        0      693 2023-04-09 02:31:18.000000 sara_compis1_tools-0.0.3/sara_compis1_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      479 2023-04-09 02:31:18.000000 sara_compis1_tools-0.0.3/sara_compis1_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 02:31:18.000000 sara_compis1_tools-0.0.3/sara_compis1_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-09 02:31:18.000000 sara_compis1_tools-0.0.3/sara_compis1_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-09 02:31:18.000000 sara_compis1_tools-0.0.3/sara_compis1_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 02:31:18.775308 sara_compis1_tools-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      790 2023-04-09 02:22:52.000000 sara_compis1_tools-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:39:15.327421 sara_compis1_tools-0.0.4/
+-rw-rw-rw-   0        0        0       80 2023-04-09 04:37:57.000000 sara_compis1_tools-0.0.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1065 2023-04-08 22:44:28.000000 sara_compis1_tools-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-04-08 22:41:49.000000 sara_compis1_tools-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      681 2023-04-09 04:39:15.323040 sara_compis1_tools-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      101 2023-04-08 22:40:09.000000 sara_compis1_tools-0.0.4/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 04:39:15.296522 sara_compis1_tools-0.0.4/sara_compis1_tools/
+-rw-rw-rw-   0        0        0     6258 2023-04-09 04:22:00.000000 sara_compis1_tools-0.0.4/sara_compis1_tools/Format.py
+-rw-rw-rw-   0        0        0      223 2023-03-07 18:50:14.000000 sara_compis1_tools-0.0.4/sara_compis1_tools/StateAFD.py
+-rw-rw-rw-   0        0        0     1559 2023-03-06 05:32:15.000000 sara_compis1_tools-0.0.4/sara_compis1_tools/Syntax.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 21:45:17.000000 sara_compis1_tools-0.0.4/sara_compis1_tools/__init__.py
+-rw-rw-rw-   0        0        0    19116 2023-04-09 00:32:31.000000 sara_compis1_tools-0.0.4/sara_compis1_tools/directAFD.py
+-rw-rw-rw-   0        0        0      381 2023-04-09 03:01:32.000000 sara_compis1_tools-0.0.4/sara_compis1_tools/generated.py
+-rw-rw-rw-   0        0        0    12081 2023-04-09 03:53:00.000000 sara_compis1_tools-0.0.4/sara_compis1_tools/lexGen.py
+drwxrwxrwx   0        0        0        0 2023-04-09 04:39:15.319291 sara_compis1_tools-0.0.4/sara_compis1_tools.egg-info/
+-rw-rw-rw-   0        0        0      681 2023-04-09 04:39:14.000000 sara_compis1_tools-0.0.4/sara_compis1_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      479 2023-04-09 04:39:15.000000 sara_compis1_tools-0.0.4/sara_compis1_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 04:39:14.000000 sara_compis1_tools-0.0.4/sara_compis1_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-09 04:39:14.000000 sara_compis1_tools-0.0.4/sara_compis1_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-09 04:39:14.000000 sara_compis1_tools-0.0.4/sara_compis1_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 04:39:15.328337 sara_compis1_tools-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      790 2023-04-09 04:38:08.000000 sara_compis1_tools-0.0.4/setup.py
```

### Comparing `sara_compis1_tools-0.0.3/LICENSE.txt` & `sara_compis1_tools-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.3/PKG-INFO` & `sara_compis1_tools-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sara_compis1_tools
-Version: 0.0.3
+Version: 0.0.4
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
 
-0.0.3 (08/04/2023)
+0.0.4 (08/04/2023)
 ------------------
-- Considering more cases.
+- More fixes.
```

### Comparing `sara_compis1_tools-0.0.3/sara_compis1_tools/Format.py` & `sara_compis1_tools-0.0.4/sara_compis1_tools/Format.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,16 @@
 
             count_q = expression.count('?')
             count_q_lit = expression.count("'?'")
             count_t = count_q - count_q_lit
 
             for i in range(len(expression)):
 
+                
+
                 if expression[i] == '?':
                     if expression[i-1] == ')':
                         j = i-2
                         continuee = True
                         closeParen = 1
                         while continuee:
                             if expression[j] == ')':
@@ -83,15 +85,23 @@
                                 continuee = False
                         expression = f'{expression[:j+1]}({expression[j+1:i]}|ε){expression[i+1:]}'
 
                     elif expression[i-1].isalnum():
                         before = expression[:i-1]
                         after = expression[i+1:]
                         middle = expression[i-1]
-                        expression = f'{before}({middle}|ε){after}'    
+                        expression = f'{before}({middle}|ε){after}' 
+                    elif i-2 >= 0:
+                        ck = expression[i-3:i]
+                        if ck[0] == "'" and ck[-1] == "'":
+                            expression = f'{expression[:i-3]}({ck}|ε){expression[i+1:]}'
+
+                               
+
+                    
         return expression
 
 
     def concat(self, regexx):
         newRegex, ops = "", list(self.sims.keys())
         ops.remove('(')
 
@@ -103,22 +113,22 @@
                     val = regexx[i + 1]
                     val = str(ord(val))
                     if len(val) == 2:
                         val = '0' + val
                     elif len(val) == 1:
                         val = '00' + val
                     i += 2
-                elif val.isalnum() or val == "#":
+                elif val.isalnum() or val in ["#", '_']:
                     val = str(ord(val))
                     if len(val) == 2:
                         val = '0' + val
                     elif len(val) == 1:
                         val = '00' + val
 
-            elif regexx[i].isalnum() or regexx[i] == "#":
+            elif regexx[i].isalnum() or regexx[i] in ['#', '_']:
                 val = str(ord(val)) 
                 if len(val) == 2:
                     val = '0' + val
                 elif len(val) == 1:
                     val = '00' + val
                     
             if i + 1 < len(regexx):
```

### Comparing `sara_compis1_tools-0.0.3/sara_compis1_tools/Syntax.py` & `sara_compis1_tools-0.0.4/sara_compis1_tools/Syntax.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.3/sara_compis1_tools/directAFD.py` & `sara_compis1_tools-0.0.4/sara_compis1_tools/directAFD.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.3/sara_compis1_tools/lexGen.py` & `sara_compis1_tools-0.0.4/sara_compis1_tools/lexGen.py`

 * *Files 3% similar despite different names*

```diff
@@ -241,18 +241,19 @@
                 node_attrs.update({'color': 'green', 'style': 'filled'})
             if state.accepting:
                 node_attrs.update({'peripheries': '2'})
             G.add_node(str(state.name), **node_attrs)
 
             for transition, final_dest in state.transitions.items():
                 G.add_node(str(final_dest))
-                if int(transition) in [n for n in range(0, 35)]:
-                    G.add_edge(str(state.name), str(final_dest), label=transition, dir='forward')    
-                else:
-                    G.add_edge(str(state.name), str(final_dest), label=str(chr(int(transition))), dir='forward')
+                
+                if int(transition) not in [el for el in range(0, 35)]:
+                    transition = str(chr(int(transition)))
+
+                G.add_edge(str(state.name), str(final_dest), label=transition, dir='forward')    
 
         dot = Digraph()
         for u, v, data in G.edges(data=True):
             dot.edge(u, v, label=data['label'], dir=data['dir'])
         for node in G.nodes:
             attrs = G.nodes[node]
             dot.node(node, **attrs)
@@ -296,27 +297,40 @@
         self.surround_dot()
         self.replace_tokens()
     
 
 
     
 if __name__ == '__main__':
-    
-        script_content = '''
-import sys
-import sara_compis1_tools.lexGen as tool
-
-if len(sys.argv) < 2:
-    print("Por favor ingrese el archivo .yal")
-    sys.exit(1)
-
-yal_file = sys.argv[1]
-lex_var = tool.Lexer(yal_file)
-lex_var.read()
-mega_content = lex_var.generate_automatas()
-mega_automata = lex_var.unify(mega_content)
-lex_var.draw_mega_afd(mega_automata)
-        '''
 
-        with open('generated.py', 'w') as script_file:
-            script_file.write(script_content)
+    # if len(sys.argv) < 2:
+    #     print("Por favor ingrese el archivo .yal")
+    #     sys.exit(1)
+
+    yal_file = 'sara_compis1_tools/lexer.yal'
+    # yal_file = sys.argv[1]
+    lexer = Lexer(yal_file)
+    
+    lexer.read()
+    mega_content = lexer.generate_automatas()
+    mega_automata = lexer.unify(mega_content)
+    lexer.draw_mega_afd(mega_automata)
+
+#     script_content = '''
+# import sys
+# import sara_compis1_tools.readLex as tool
+
+# if len(sys.argv) < 2:
+#     print("Por favor ingrese el archivo .yal")
+#     sys.exit(1)
+
+# yal_file = sys.argv[1]
+# lex_var = tool.Lexer(yal_file)
+# lex_var.read()
+# mega_content = lex_var.generate_automatas()
+# mega_automata = lex_var.unify(mega_content)
+# lex_var.draw_mega_afd(mega_automata)
+#     '''
+
+#     with open('generated.py', 'w') as script_file:
+#         script_file.write(script_content)
```

### Comparing `sara_compis1_tools-0.0.3/sara_compis1_tools.egg-info/PKG-INFO` & `sara_compis1_tools-0.0.4/sara_compis1_tools.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sara-compis1-tools
-Version: 0.0.3
+Version: 0.0.4
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
 
-0.0.3 (08/04/2023)
+0.0.4 (08/04/2023)
 ------------------
-- Considering more cases.
+- More fixes.
```

### Comparing `sara_compis1_tools-0.0.3/setup.py` & `sara_compis1_tools-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sara_compis1_tools',
-    version='0.0.3',
+    version='0.0.4',
     description='A collection of tools for the Language Design course',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='https://github.com/MGonza20/Compis_Lab3',
     author='Sara Paguaga',
     author_email='sara.paguaga@gmail.com',
     license='MIT',
     classifiers=[
```

