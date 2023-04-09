# Comparing `tmp/fastencode-1.0.tar.gz` & `tmp/fastencode-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastencode-1.0.tar", last modified: Sun Apr  9 08:24:47 2023, max compression
+gzip compressed data, was "fastencode-1.1.tar", last modified: Sun Apr  9 14:12:57 2023, max compression
```

## Comparing `fastencode-1.0.tar` & `fastencode-1.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 08:24:47.476704 fastencode-1.0/
--rw-rw-rw-   0        0        0     1119 2023-04-09 08:24:47.477702 fastencode-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-09 08:24:47.476704 fastencode-1.0/fastencode/
--rw-rw-rw-   0        0        0       26 2023-04-09 07:52:39.340390 fastencode-1.0/fastencode/__init__.py
--rw-rw-rw-   0        0        0     4320 2023-04-09 08:24:43.116360 fastencode-1.0/fastencode/utils.py
--rw-rw-rw-   0        0        0       40 2023-04-09 08:15:21.759616 fastencode-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1924 2023-04-09 08:24:25.439859 fastencode-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 14:12:57.974356 fastencode-1.1/
+-rw-rw-rw-   0        0        0     1077 2023-04-09 08:15:47.000000 fastencode-1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3772 2023-04-09 14:12:57.974356 fastencode-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2601 2023-04-09 14:10:43.000000 fastencode-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 14:12:57.966729 fastencode-1.1/fastencode/
+-rw-rw-rw-   0        0        0       36 2023-04-09 09:11:20.000000 fastencode-1.1/fastencode/__init__.py
+-rw-rw-rw-   0        0        0     3058 2023-04-09 09:23:06.000000 fastencode-1.1/fastencode/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-09 14:12:57.973355 fastencode-1.1/fastencode.egg-info/
+-rw-rw-rw-   0        0        0     3772 2023-04-09 14:12:57.000000 fastencode-1.1/fastencode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-04-09 14:12:57.000000 fastencode-1.1/fastencode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 14:12:57.000000 fastencode-1.1/fastencode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-09 14:12:57.000000 fastencode-1.1/fastencode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-09 14:12:57.000000 fastencode-1.1/fastencode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-09 14:12:57.975757 fastencode-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     2147 2023-04-09 14:12:34.000000 fastencode-1.1/setup.py
```

### Comparing `fastencode-1.0/setup.py` & `fastencode-1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,23 @@
-from distutils.core import setup
+from setuptools import setup
+
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
+
+
 setup(
   name = 'fastencode',         # How you named your package folder (MyLib)
   packages = ['fastencode'],   # Chose the same as "name"
-  version = '1.0',      # Start with a small number and increase it with every change you make
+  version = '1.1',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'An easy way to use different encoding: bytes, hex, ascii array, binary, long',   # Give a short description about your library
+  long_description = long_description,
+  long_description_content_type='text/markdown',
   author = 'ES3',                   # Type in your name
   author_email = 'ourteamscare@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/user/reponame',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/elyassaf/Easy-Encoding/archive/refs/tags/v_1.0.tar.gz',    # I explain this later on
   keywords = ['encoding', 'hex', 'bytes', 'binary representation', 'decoding', 'ascii'],   # Keywords that define your package best
   install_requires=['typing'],
   classifiers=[
```

