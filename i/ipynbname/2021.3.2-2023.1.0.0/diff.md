# Comparing `tmp/ipynbname-2021.3.2.tar.gz` & `tmp/ipynbname-2023.1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ipynbname-2021.3.2.tar", last modified: Thu Jan 28 08:07:26 2021, max compression
+gzip compressed data, was "ipynbname-2023.1.0.0.tar", last modified: Sun Apr  9 14:56:24 2023, max compression
```

## Comparing `ipynbname-2021.3.2.tar` & `ipynbname-2023.1.0.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2021-01-28 08:07:26.672904 ipynbname-2021.3.2/
--rw-rw-rw-   0        0        0       19 2020-09-05 11:28:37.000000 ipynbname-2021.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2019 2021-01-28 08:07:26.673894 ipynbname-2021.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1138 2020-09-09 10:52:08.000000 ipynbname-2021.3.2/README.md
-drwxrwxrwx   0        0        0        0 2021-01-28 08:07:26.628895 ipynbname-2021.3.2/ipynbname/
--rw-rw-rw-   0        0        0     3167 2021-01-28 08:02:32.000000 ipynbname-2021.3.2/ipynbname/__init__.py
-drwxrwxrwx   0        0        0        0 2021-01-28 08:07:26.670895 ipynbname-2021.3.2/ipynbname.egg-info/
--rw-rw-rw-   0        0        0     2019 2021-01-28 08:07:26.000000 ipynbname-2021.3.2/ipynbname.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2021-01-28 08:07:26.000000 ipynbname-2021.3.2/ipynbname.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-01-28 08:07:26.000000 ipynbname-2021.3.2/ipynbname.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2021-01-28 08:07:26.000000 ipynbname-2021.3.2/ipynbname.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2021-01-28 08:07:26.000000 ipynbname-2021.3.2/ipynbname.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2021-01-28 08:07:26.676892 ipynbname-2021.3.2/setup.cfg
--rw-rw-rw-   0        0        0      986 2021-01-28 08:05:52.000000 ipynbname-2021.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 14:56:24.551340 ipynbname-2023.1.0.0/
+-rw-rw-rw-   0        0        0     1092 2023-04-09 11:23:56.000000 ipynbname-2023.1.0.0/LICENSE
+-rw-rw-rw-   0        0        0       19 2023-04-09 11:23:56.000000 ipynbname-2023.1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1788 2023-04-09 14:56:24.552340 ipynbname-2023.1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1138 2023-04-09 11:23:56.000000 ipynbname-2023.1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 14:56:24.531798 ipynbname-2023.1.0.0/ipynbname/
+-rw-rw-rw-   0        0        0     3749 2023-04-09 11:23:56.000000 ipynbname-2023.1.0.0/ipynbname/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 14:56:24.550374 ipynbname-2023.1.0.0/ipynbname.egg-info/
+-rw-rw-rw-   0        0        0     1788 2023-04-09 14:56:24.000000 ipynbname-2023.1.0.0/ipynbname.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-04-09 14:56:24.000000 ipynbname-2023.1.0.0/ipynbname.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 14:56:24.000000 ipynbname-2023.1.0.0/ipynbname.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-09 14:56:24.000000 ipynbname-2023.1.0.0/ipynbname.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-09 14:56:24.000000 ipynbname-2023.1.0.0/ipynbname.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-09 14:56:24.558175 ipynbname-2023.1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      988 2023-04-09 14:41:04.000000 ipynbname-2023.1.0.0/setup.py
```

### Comparing `ipynbname-2021.3.2/README.md` & `ipynbname-2023.1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ipynbname-2021.3.2/ipynbname/__init__.py` & `ipynbname-2023.1.0.0/ipynbname/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import os
 import json
+import os
 import urllib.error
 import urllib.request
 from itertools import chain
 from pathlib import Path, PurePath
 from typing import Generator, Tuple, Union
 
 import ipykernel
@@ -19,42 +21,54 @@
     """ Iterate over the server info files of running notebook servers.
     """
     if runtime_dir is None:
         runtime_dir = jupyter_runtime_dir()
     runtime_dir = Path(runtime_dir)
 
     if runtime_dir.is_dir():
-        for file_name in chain(
-            runtime_dir.glob('nbserver-*.json'),  # jupyter notebook (or lab 2)
-            runtime_dir.glob('jpserver-*.json'),  # jupyterlab 3
+        # Get notebook configuration files, sorted to check the more recently modified ones first
+        for file_name in sorted(
+            chain(
+                runtime_dir.glob('nbserver-*.json'),  # jupyter notebook (or lab 2)
+                runtime_dir.glob('jpserver-*.json'),  # jupyterlab 3
+            ),
+            key=os.path.getmtime,
+            reverse=True,
         ):
-            yield json.loads(file_name.read_bytes())
+            try:
+                yield json.loads(file_name.read_bytes())
+            except json.JSONDecodeError as err:
+                # Sometimes we encounter empty JSON files. Ignore them.
+                pass
 
 
 def _get_kernel_id() -> str:
     """ Returns the kernel ID of the ipykernel.
     """
     connection_file = Path(ipykernel.get_connection_file()).stem
     kernel_id = connection_file.split('-', 1)[1]
     return kernel_id
 
 
 def _get_sessions(srv):
     """ Given a server, returns sessions, or HTTPError if access is denied.
         NOTE: Works only when either there is no security or there is token
-        based security. An HTTPError is raised if unable to connect to a 
+        based security. An HTTPError is raised if unable to connect to a
         server.
     """
     try:
         qry_str = ""
         token = srv['token']
         if token:
             qry_str = f"?token={token}"
+        if not token and "JUPYTERHUB_API_TOKEN" in os.environ:
+            token = os.environ["JUPYTERHUB_API_TOKEN"]
         url = f"{srv['url']}api/sessions{qry_str}"
-        with urllib.request.urlopen(url) as req:
+        # Use a timeout in case this is a stale entry.
+        with urllib.request.urlopen(url, timeout=0.5) as req:
             return json.load(req)
     except Exception:
         raise urllib.error.HTTPError(CONN_ERROR)
 
 
 def _find_nb_path() -> Union[Tuple[dict, PurePath], Tuple[None, None]]:
     try:
```

### Comparing `ipynbname-2021.3.2/setup.py` & `ipynbname-2023.1.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 here = Path(__file__).parent
 long_description = (here / 'README.md').read_text()
 
 setuptools.setup(
     name='ipynbname',
-    version='2021.3.2',
+    version='2023.1.0.0',
     author='Mark McPherson',
     author_email='msm1089@yahoo.co.uk',
     description='Simply returns either notebook filename or the full path to the notebook when run from Jupyter notebook in browser.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     keywords='jupyter notebook filename'.split(),
```

