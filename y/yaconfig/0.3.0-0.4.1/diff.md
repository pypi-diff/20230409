# Comparing `tmp/yaconfig-0.3.0.tar.gz` & `tmp/yaconfig-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaconfig-0.3.0.tar", last modified: Wed Feb 10 17:12:16 2021, max compression
+gzip compressed data, was "yaconfig-0.4.1.tar", last modified: Sun Apr  9 00:06:01 2023, max compression
```

## Comparing `yaconfig-0.3.0.tar` & `yaconfig-0.4.1.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-10 17:12:16.878046 yaconfig-0.3.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4000 2021-02-10 17:12:16.878046 yaconfig-0.3.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2686 2021-02-10 17:11:39.000000 yaconfig-0.3.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      483 2021-02-10 17:12:16.878046 yaconfig-0.3.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1390 2021-02-10 17:11:39.000000 yaconfig-0.3.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-10 17:12:16.878046 yaconfig-0.3.0/yaconfig/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7057 2021-02-10 17:11:39.000000 yaconfig-0.3.0/yaconfig/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-10 17:12:16.878046 yaconfig-0.3.0/yaconfig.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4000 2021-02-10 17:12:16.000000 yaconfig-0.3.0/yaconfig.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      208 2021-02-10 17:12:16.000000 yaconfig-0.3.0/yaconfig.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-10 17:12:16.000000 yaconfig-0.3.0/yaconfig.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       57 2021-02-10 17:12:16.000000 yaconfig-0.3.0/yaconfig.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2021-02-10 17:12:16.000000 yaconfig-0.3.0/yaconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:06:01.950345 yaconfig-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-09 00:05:48.000000 yaconfig-0.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-09 00:06:01.950345 yaconfig-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-09 00:05:48.000000 yaconfig-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-09 00:06:01.950345 yaconfig-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-09 00:05:48.000000 yaconfig-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:06:01.946345 yaconfig-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-09 00:05:48.000000 yaconfig-0.4.1/tests/test_yaconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:06:01.946345 yaconfig-0.4.1/yaconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-04-09 00:05:48.000000 yaconfig-0.4.1/yaconfig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:06:01.950345 yaconfig-0.4.1/yaconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-09 00:06:01.000000 yaconfig-0.4.1/yaconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-09 00:06:01.000000 yaconfig-0.4.1/yaconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 00:06:01.000000 yaconfig-0.4.1/yaconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-09 00:06:01.000000 yaconfig-0.4.1/yaconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 00:06:01.000000 yaconfig-0.4.1/yaconfig.egg-info/top_level.txt
```

### Comparing `yaconfig-0.3.0/README.md` & `yaconfig-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `yaconfig-0.3.0/setup.py` & `yaconfig-0.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,33 +9,34 @@
 # Get the long description from the README file
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)), 'README.md')) as f:
     long_description = f.read()
 
 setup(author="Dih5",
       author_email='dihedralfive@gmail.com',
       classifiers=[
-          'Development Status :: 3 - Alpha',
+          'Development Status :: 4 - Beta',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: MIT License',
           'Natural Language :: English',
           'Programming Language :: Python :: 3',
           'Programming Language :: Python :: 3.5',
           'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3.10',
       ],
       description='Python package to assist configuration',
       extras_require={
           "docs": ["nbsphinx", "sphinx-rtd-theme", "IPython"],
           "test": ["pytest"],
       },
       keywords=[],
       long_description=long_description,
       long_description_content_type='text/markdown',
       name='yaconfig',
       packages=find_packages(include=['yaconfig'], exclude=["demos", "tests", "docs"]),
       install_requires=[],
       url='https://github.com/dih5/yaconfig',
-      version='0.3.0',
+      version='0.4.1',
 
       )
```

### Comparing `yaconfig-0.3.0/yaconfig/__init__.py` & `yaconfig-0.4.1/yaconfig/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """yaconfig - Python package to assist configuration"""
 
-__version__ = '0.3.0'
+__version__ = '0.4.1'
 __author__ = 'Dih5 <dihedralfive@gmail.com>'
 
 import json
 import os
 from collections import OrderedDict
 from shlex import quote
 
@@ -123,14 +123,30 @@
         text += "\n"
         if path is None:
             return text
         else:
             with open(path, "w") as f:
                 f.write(text)
 
+    def generate_environment_md(self, prefix=""):
+        """Generate a description Markdown table for a environment-based configuration"""
+
+        names = [prefix + name.upper() for name, variable in self.items()]
+        descriptions = [variable.help for name, variable in self.items()]
+
+        # Max widths for more aesthetic code
+        name_width = max([len(name) for name in names])
+        desc_width = max([len(desc) for desc in descriptions])
+
+        header = f"| {'Name':<{name_width}} | {'Description':<{desc_width}} |\n| {'-' * name_width} | {'-' * desc_width} |\n"
+        rows = "\n".join(
+            [f"| {name:<{name_width}} | {desc:<{desc_width}} |" for name, desc in zip(names, descriptions)])
+
+        return header + rows
+
     def interactive_environment(self, path="environment.sh", prefix=""):
         values = self.prompt()
         text = "#!/bin/bash\n"
         text += "\n\n".join(variable._get_bash(prefix=prefix, value=values[var_name]) for var_name, variable in self.items())
         text += "\n"
         if path is None:
             return text
```

