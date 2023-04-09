# Comparing `tmp/hugg-0.0.84.tar.gz` & `tmp/hugg-0.0.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugg-0.0.84.tar", last modified: Sun Apr  9 16:22:08 2023, max compression
+gzip compressed data, was "hugg-0.0.85.tar", last modified: Sun Apr  9 16:40:40 2023, max compression
```

## Comparing `hugg-0.0.84.tar` & `hugg-0.0.85.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:22:08.799039 hugg-0.0.84/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-09 16:21:54.000000 hugg-0.0.84/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-09 16:22:08.799039 hugg-0.0.84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-09 16:21:54.000000 hugg-0.0.84/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:22:08.799039 hugg-0.0.84/hugg/
--rw-r--r--   0 runner    (1001) docker     (123)    36142 2023-04-09 16:21:54.000000 hugg-0.0.84/hugg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:22:08.799039 hugg-0.0.84/hugg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-09 16:22:08.000000 hugg-0.0.84/hugg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-09 16:22:08.000000 hugg-0.0.84/hugg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 16:22:08.000000 hugg-0.0.84/hugg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-09 16:22:08.000000 hugg-0.0.84/hugg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 16:22:08.000000 hugg-0.0.84/hugg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 16:22:08.799039 hugg-0.0.84/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3533 2023-04-09 16:21:54.000000 hugg-0.0.84/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:40:40.034904 hugg-0.0.85/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-09 16:40:29.000000 hugg-0.0.85/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-09 16:40:40.034904 hugg-0.0.85/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-09 16:40:29.000000 hugg-0.0.85/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:40:40.034904 hugg-0.0.85/hugg/
+-rw-r--r--   0 runner    (1001) docker     (123)    36150 2023-04-09 16:40:29.000000 hugg-0.0.85/hugg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:40:40.034904 hugg-0.0.85/hugg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-09 16:40:40.000000 hugg-0.0.85/hugg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-09 16:40:40.000000 hugg-0.0.85/hugg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 16:40:40.000000 hugg-0.0.85/hugg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-09 16:40:40.000000 hugg-0.0.85/hugg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 16:40:40.000000 hugg-0.0.85/hugg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 16:40:40.034904 hugg-0.0.85/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3533 2023-04-09 16:40:29.000000 hugg-0.0.85/setup.py
```

### Comparing `hugg-0.0.84/LICENSE` & `hugg-0.0.85/LICENSE`

 * *Files identical despite different names*

### Comparing `hugg-0.0.84/hugg/__init__.py` & `hugg-0.0.85/hugg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -798,15 +798,15 @@
             print(":> "+str(encoding))
             if encoding is not None and encoding.strip() != '':
                 print("none")
                 current_contents = current_contents.decoded_content.decode(encoding)
                 encode_writing = "w+"
             else:
                 print("bin")
-                current_contents = current_contents.content
+                current_contents = current_contents.decoded_content
                 encode_writing = "w+"#"wb+"
 
             with open(download_to,encode_writing) as writer:
                 writer.write(current_contents)
         return download_to
     
     def upload(self, file_path=None,path_in_repo=None):
```

### Comparing `hugg-0.0.84/setup.py` & `hugg-0.0.85/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.84"
+VERSION = "0.0.85"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

