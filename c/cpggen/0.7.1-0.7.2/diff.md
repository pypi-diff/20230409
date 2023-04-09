# Comparing `tmp/cpggen-0.7.1.tar.gz` & `tmp/cpggen-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-0.7.1.tar", max compression
+gzip compressed data, was "cpggen-0.7.2.tar", max compression
```

## Comparing `cpggen-0.7.1.tar` & `cpggen-0.7.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-04-06 12:19:09.022715 cpggen-0.7.1/LICENSE
--rw-r--r--   0        0        0     4409 2023-04-06 12:19:09.022715 cpggen-0.7.1/README.md
--rw-r--r--   0        0        0        0 2023-04-06 12:19:09.022715 cpggen-0.7.1/cpggen/__init__.py
--rw-r--r--   0        0        0     8264 2023-04-06 12:19:09.022715 cpggen-0.7.1/cpggen/cli.py
--rw-r--r--   0        0        0    16565 2023-04-06 12:19:09.022715 cpggen-0.7.1/cpggen/executor.py
--rw-r--r--   0        0        0      731 2023-04-06 12:19:09.022715 cpggen-0.7.1/cpggen/logger.py
--rw-r--r--   0        0        0     9581 2023-04-06 12:19:09.022715 cpggen-0.7.1/cpggen/utils.py
--rw-r--r--   0        0        0     1245 2023-04-06 12:19:09.022715 cpggen-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     5737 1970-01-01 00:00:00.000000 cpggen-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-09 18:02:12.315227 cpggen-0.7.2/LICENSE
+-rw-r--r--   0        0        0     5622 2023-04-09 18:02:12.315227 cpggen-0.7.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-09 18:02:12.315227 cpggen-0.7.2/cpggen/__init__.py
+-rw-r--r--   0        0        0     8290 2023-04-09 18:02:12.315227 cpggen-0.7.2/cpggen/cli.py
+-rw-r--r--   0        0        0    16565 2023-04-09 18:02:12.319227 cpggen-0.7.2/cpggen/executor.py
+-rw-r--r--   0        0        0      731 2023-04-09 18:02:12.319227 cpggen-0.7.2/cpggen/logger.py
+-rw-r--r--   0        0        0     9682 2023-04-09 18:02:12.319227 cpggen-0.7.2/cpggen/utils.py
+-rw-r--r--   0        0        0     1245 2023-04-09 18:02:12.319227 cpggen-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     6950 1970-01-01 00:00:00.000000 cpggen-0.7.2/PKG-INFO
```

### Comparing `cpggen-0.7.1/LICENSE` & `cpggen-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-0.7.1/README.md` & `cpggen-0.7.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -29,14 +29,45 @@
 Or use the nightly to always get the latest joern and tools.
 
 ```
 docker pull ghcr.io/appthreat/cpggen:nightly
 # podman pull ghcr.io/appthreat/cpggen:nightly
 ```
 
+### Single executable binaries
+
+Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
+
+- cpggen with Python 3.10
+- cdxgen with Node.js 18
+- cdxgen binary plugins
+
+```bash
+curl -LO https://github.com/appthreat/cpggen/releases/download/latest/cpggen-linux-amd64
+chmod +x cpggen-linux-amd64
+./cpggen-linux-amd64 --help
+```
+
+On Windows,
+
+```powershell
+curl -LO https://github.com/appthreat/cpggen/releases/download/latest/cpggen.exe
+.\cpggen.exe --help
+```
+
+### OCI Artifacts via ORAS cli
+
+Use [ORAS cli](https://oras.land/cli/) to download the cpggen binary with Python and Node.js preinstalled.
+
+```bash
+oras pull ghcr.io/appthreat/cpggen-bin:v1
+chmod +x cpggen-linux-amd64
+./cpggen-linux-amd64 --help
+```
+
 ## Usage
 
 To auto detect the language from the current directory and generate CPG.
 
 ```
 cpggen
 ```
@@ -53,14 +84,17 @@
 cpggen -i https://github.com/HooliCorp/vulnerable-aws-koa-app -o /tmp/cpg
 ```
 
 To specify language type.
 
 ```
 cpggen -i <src directory> -o <CPG directory or file name> -l java
+
+# Comma separated values are accepted for multiple languages
+cpggen -i <src directory> -o <CPG directory or file name> -l java,js,python
 ```
 
 Container based invocation
 
 ```
 docker run --rm -it -v /tmp:/tmp -v $(pwd):/app:rw --cpus=4 --memory=16g -t ghcr.io/appthreat/cpggen cpggen -i <src directory> -o <CPG directory or file name>
 ```
@@ -135,7 +169,21 @@
     name: cpg
     path: cpg_out
 ```
 
 ## License
 
 Apache-2.0
+
+## Developing / Contributing
+
+```
+git clone git@github.com:AppThreat/cpggen.git
+cd cpggen
+
+python -m pip install --upgrade pip
+python -m pip install poetry
+# Add poetry to the PATH environment variable
+poetry install
+
+poetry run cpggen -i <src directory>
+```
```

### Comparing `cpggen-0.7.1/cpggen/cli.py` & `cpggen-0.7.2/cpggen/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
 import argparse
 import os
 import signal
 import tempfile
 from multiprocessing import Pool
 from pathlib import Path
 
@@ -224,15 +227,15 @@
                 pool.close()
             except KeyboardInterrupt:
                 pool.terminate()
             pool.join()
 
 
 def main():
-    console.print(product_logo, style="info")
+    print(product_logo)
     args = build_args()
     if args.server_mode:
         return run_server(args)
     src = args.src
     cpg_out_dir = args.cpg_out_dir
     languages = args.language
     joern_home = args.joern_home
```

### Comparing `cpggen-0.7.1/cpggen/executor.py` & `cpggen-0.7.2/cpggen/executor.py`

 * *Files identical despite different names*

### Comparing `cpggen-0.7.1/cpggen/logger.py` & `cpggen-0.7.2/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-0.7.1/cpggen/utils.py` & `cpggen-0.7.2/cpggen/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,20 +119,24 @@
     :param dir_name: Directory to compare
     :return: Boolean True if directory can be ignored. False otherwise
     """
     base_dir = base_dir.lower()
     dir_name = dir_name.lower()
     if dir_name.startswith("."):
         return True
-    elif dir_name.startswith("/" + base_dir):
-        dir_name = re.sub(r"^/" + base_dir + "/", "", dir_name)
+    elif dir_name.startswith(os.path.sep + base_dir):
+        dir_name = re.sub(r"^" + os.path.sep + base_dir + os.path.sep, "", dir_name)
     elif dir_name.startswith(base_dir):
-        dir_name = re.sub(r"^" + base_dir + "/", "", dir_name)
+        dir_name = re.sub(r"^" + base_dir + os.path.sep, "", dir_name)
     for d in ignore_directories:
-        if dir_name == d or dir_name.startswith(d) or ("/" + d + "/") in dir_name:
+        if (
+            dir_name == d
+            or dir_name.startswith(d)
+            or (os.path.sep + d + os.path.sep) in dir_name
+        ):
             return True
     return False
 
 
 def find_files(src, src_ext_name, use_start=False, quick=False):
     """
     Method to find files with given extension
```

### Comparing `cpggen-0.7.1/pyproject.toml` & `cpggen-0.7.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "0.7.1"
+version = "0.7.2"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-0.7.1/PKG-INFO` & `cpggen-0.7.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 0.7.1
+Version: 0.7.2
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8,<3.12
@@ -61,14 +61,45 @@
 Or use the nightly to always get the latest joern and tools.
 
 ```
 docker pull ghcr.io/appthreat/cpggen:nightly
 # podman pull ghcr.io/appthreat/cpggen:nightly
 ```
 
+### Single executable binaries
+
+Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
+
+- cpggen with Python 3.10
+- cdxgen with Node.js 18
+- cdxgen binary plugins
+
+```bash
+curl -LO https://github.com/appthreat/cpggen/releases/download/latest/cpggen-linux-amd64
+chmod +x cpggen-linux-amd64
+./cpggen-linux-amd64 --help
+```
+
+On Windows,
+
+```powershell
+curl -LO https://github.com/appthreat/cpggen/releases/download/latest/cpggen.exe
+.\cpggen.exe --help
+```
+
+### OCI Artifacts via ORAS cli
+
+Use [ORAS cli](https://oras.land/cli/) to download the cpggen binary with Python and Node.js preinstalled.
+
+```bash
+oras pull ghcr.io/appthreat/cpggen-bin:v1
+chmod +x cpggen-linux-amd64
+./cpggen-linux-amd64 --help
+```
+
 ## Usage
 
 To auto detect the language from the current directory and generate CPG.
 
 ```
 cpggen
 ```
@@ -85,14 +116,17 @@
 cpggen -i https://github.com/HooliCorp/vulnerable-aws-koa-app -o /tmp/cpg
 ```
 
 To specify language type.
 
 ```
 cpggen -i <src directory> -o <CPG directory or file name> -l java
+
+# Comma separated values are accepted for multiple languages
+cpggen -i <src directory> -o <CPG directory or file name> -l java,js,python
 ```
 
 Container based invocation
 
 ```
 docker run --rm -it -v /tmp:/tmp -v $(pwd):/app:rw --cpus=4 --memory=16g -t ghcr.io/appthreat/cpggen cpggen -i <src directory> -o <CPG directory or file name>
 ```
@@ -168,7 +202,21 @@
     path: cpg_out
 ```
 
 ## License
 
 Apache-2.0
 
+## Developing / Contributing
+
+```
+git clone git@github.com:AppThreat/cpggen.git
+cd cpggen
+
+python -m pip install --upgrade pip
+python -m pip install poetry
+# Add poetry to the PATH environment variable
+poetry install
+
+poetry run cpggen -i <src directory>
+```
+
```

