# Comparing `tmp/pikvm-cli-1.0.1.tar.gz` & `tmp/pikvm-cli-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikvm-cli-1.0.1.tar", last modified: Sun Apr  9 09:37:26 2023, max compression
+gzip compressed data, was "pikvm-cli-1.0.2.tar", last modified: Sun Apr  9 10:42:57 2023, max compression
```

## Comparing `pikvm-cli-1.0.1.tar` & `pikvm-cli-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:37:26.987110 pikvm-cli-1.0.1/
--rw-r--r--   0 root         (0) root         (0)     1422 2023-04-09 09:37:26.987110 pikvm-cli-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1060 2023-04-08 10:33:30.000000 pikvm-cli-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:37:26.987110 pikvm-cli-1.0.1/pikvm_cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-08 12:48:40.000000 pikvm-cli-1.0.1/pikvm_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4301 2023-04-09 09:30:44.000000 pikvm-cli-1.0.1/pikvm_cli/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 09:37:26.987110 pikvm-cli-1.0.1/pikvm_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1422 2023-04-09 09:37:26.000000 pikvm-cli-1.0.1/pikvm_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      262 2023-04-09 09:37:26.000000 pikvm-cli-1.0.1/pikvm_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 09:37:26.000000 pikvm-cli-1.0.1/pikvm_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-04-09 09:37:26.000000 pikvm-cli-1.0.1/pikvm_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-09 09:37:26.000000 pikvm-cli-1.0.1/pikvm_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-09 09:37:26.000000 pikvm-cli-1.0.1/pikvm_cli.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 09:37:26.987110 pikvm-cli-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      963 2023-04-09 09:35:41.000000 pikvm-cli-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 10:42:57.304038 pikvm-cli-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1422 2023-04-09 10:42:57.304038 pikvm-cli-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-04-08 10:33:30.000000 pikvm-cli-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 10:42:57.304038 pikvm-cli-1.0.2/pikvm_cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-08 12:48:40.000000 pikvm-cli-1.0.2/pikvm_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4301 2023-04-09 10:41:39.000000 pikvm-cli-1.0.2/pikvm_cli/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 10:42:57.304038 pikvm-cli-1.0.2/pikvm_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1422 2023-04-09 10:42:57.000000 pikvm-cli-1.0.2/pikvm_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      262 2023-04-09 10:42:57.000000 pikvm-cli-1.0.2/pikvm_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 10:42:57.000000 pikvm-cli-1.0.2/pikvm_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-04-09 10:42:57.000000 pikvm-cli-1.0.2/pikvm_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-09 10:42:57.000000 pikvm-cli-1.0.2/pikvm_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-09 10:42:57.000000 pikvm-cli-1.0.2/pikvm_cli.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 10:42:57.304038 pikvm-cli-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      772 2023-04-09 10:41:40.000000 pikvm-cli-1.0.2/setup.py
```

### Comparing `pikvm-cli-1.0.1/PKG-INFO` & `pikvm-cli-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pikvm-cli
-Version: 1.0.1
+Version: 1.0.2
 Summary: CLI tool for managing PIKVM device
 Home-page: https://github.com/lysyi3m/pikvm-cli
 Author: Emil Kashkevich
 Author-email: emil.kashkevich@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pikvm-cli-1.0.1/README.md` & `pikvm-cli-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pikvm-cli-1.0.1/pikvm_cli/__main__.py` & `pikvm-cli-1.0.2/pikvm_cli/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     return
 
   data = response.json()
 
   click.echo(json.dumps(data, indent=2))
 
 @click.group()
-@click.version_option("1.0.1")
+@click.version_option("1.0.2")
 def main():
   """
   CLI tool to control and manage PIKVM devices
   """
   pass
 
 @main.command()
```

### Comparing `pikvm-cli-1.0.1/pikvm_cli.egg-info/PKG-INFO` & `pikvm-cli-1.0.2/pikvm_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pikvm-cli
-Version: 1.0.1
+Version: 1.0.2
 Summary: CLI tool for managing PIKVM device
 Home-page: https://github.com/lysyi3m/pikvm-cli
 Author: Emil Kashkevich
 Author-email: emil.kashkevich@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pikvm-cli-1.0.1/setup.py` & `pikvm-cli-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 from setuptools import setup, find_packages
 from io import open
-from os import path
 
-import pathlib
-
-with open(path.join(pathlib.Path(__file__).parent, 'README.md'), 'r', encoding='utf-8') as f:
+with open('README.md', 'r', encoding='utf-8') as f:
   long_description = f.read()
 
-with open(path.join(pathlib.Path(__file__).parent, 'requirements.txt'), 'r', encoding='utf-8') as f:
-  install_requires = f.read().splitlines()
-
 setup(
   name='pikvm-cli',
-  version='1.0.1',
+  version='1.0.2',
   author='Emil Kashkevich',
   author_email='emil.kashkevich@gmail.com',
   description='CLI tool for managing PIKVM device',
   long_description=long_description,
   long_description_content_type='text/markdown',
   license='MIT',
   url='https://github.com/lysyi3m/pikvm-cli',
   packages=find_packages(),
   classifiers=[
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3',
   ],
-  install_requires=install_requires,
+  install_requires=[
+    'click==8.1.3',
+    'requests==2.28.2'
+  ],
   entry_points={
     'console_scripts': [
       'pikvm-cli=pikvm_cli.__main__:main',
     ]
   },
 )
```

