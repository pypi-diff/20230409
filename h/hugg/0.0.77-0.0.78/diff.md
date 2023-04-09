# Comparing `tmp/hugg-0.0.77.tar.gz` & `tmp/hugg-0.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugg-0.0.77.tar", last modified: Sun Apr  9 07:03:30 2023, max compression
+gzip compressed data, was "hugg-0.0.78.tar", last modified: Sun Apr  9 07:05:41 2023, max compression
```

## Comparing `hugg-0.0.77.tar` & `hugg-0.0.78.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:03:30.717244 hugg-0.0.77/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-09 07:03:15.000000 hugg-0.0.77/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-09 07:03:30.717244 hugg-0.0.77/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-09 07:03:15.000000 hugg-0.0.77/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:03:30.717244 hugg-0.0.77/hugg/
--rw-r--r--   0 runner    (1001) docker     (123)    35856 2023-04-09 07:03:15.000000 hugg-0.0.77/hugg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:03:30.717244 hugg-0.0.77/hugg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-09 07:03:30.000000 hugg-0.0.77/hugg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-09 07:03:30.000000 hugg-0.0.77/hugg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 07:03:30.000000 hugg-0.0.77/hugg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-09 07:03:30.000000 hugg-0.0.77/hugg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 07:03:30.000000 hugg-0.0.77/hugg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 07:03:30.717244 hugg-0.0.77/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3533 2023-04-09 07:03:15.000000 hugg-0.0.77/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:41.747801 hugg-0.0.78/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-09 07:05:29.000000 hugg-0.0.78/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-09 07:05:41.747801 hugg-0.0.78/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-09 07:05:29.000000 hugg-0.0.78/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:41.747801 hugg-0.0.78/hugg/
+-rw-r--r--   0 runner    (1001) docker     (123)    35895 2023-04-09 07:05:29.000000 hugg-0.0.78/hugg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:05:41.747801 hugg-0.0.78/hugg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-09 07:05:41.000000 hugg-0.0.78/hugg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-09 07:05:41.000000 hugg-0.0.78/hugg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 07:05:41.000000 hugg-0.0.78/hugg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-09 07:05:41.000000 hugg-0.0.78/hugg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 07:05:41.000000 hugg-0.0.78/hugg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 07:05:41.747801 hugg-0.0.78/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3533 2023-04-09 07:05:29.000000 hugg-0.0.78/setup.py
```

### Comparing `hugg-0.0.77/LICENSE` & `hugg-0.0.78/LICENSE`

 * *Files identical despite different names*

### Comparing `hugg-0.0.77/hugg/__init__.py` & `hugg-0.0.78/hugg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -790,15 +790,15 @@
     
     def download(self, file_path=None,download_to=None, encoding="utf-8"):
         download_to = download_to or os.path.basename(file_path)
         if download_to is None:
             download_to = os.path.join(os.curdir,file_path.split("/")[-1])
         if file_path and isinstance(file_path,str):
             current_contents = self.repo.get_contents(file_path, ref=self.branch).decoded_content
-            if encoding:
+            if encoding is not None and encoding.strip() != '':
                 current_contents = current_contents.decode(encoding)
             with open(download_to,"w+" if encoding else "wb+") as writer:
                 writer.write(current_contents)
         return download_to
     
     def upload(self, file_path=None,path_in_repo=None):
         from pathlib import Path
```

### Comparing `hugg-0.0.77/setup.py` & `hugg-0.0.78/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.77"
+VERSION = "0.0.78"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

