# Comparing `tmp/hugg-0.0.86.tar.gz` & `tmp/hugg-0.0.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugg-0.0.86.tar", last modified: Sun Apr  9 16:57:31 2023, max compression
+gzip compressed data, was "hugg-0.0.87.tar", last modified: Sun Apr  9 17:03:48 2023, max compression
```

## Comparing `hugg-0.0.86.tar` & `hugg-0.0.87.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:57:31.716549 hugg-0.0.86/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-09 16:57:21.000000 hugg-0.0.86/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-09 16:57:31.716549 hugg-0.0.86/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-09 16:57:21.000000 hugg-0.0.86/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:57:31.712548 hugg-0.0.86/hugg/
--rw-r--r--   0 runner    (1001) docker     (123)    36198 2023-04-09 16:57:21.000000 hugg-0.0.86/hugg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:57:31.716549 hugg-0.0.86/hugg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-09 16:57:31.000000 hugg-0.0.86/hugg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-09 16:57:31.000000 hugg-0.0.86/hugg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 16:57:31.000000 hugg-0.0.86/hugg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-09 16:57:31.000000 hugg-0.0.86/hugg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 16:57:31.000000 hugg-0.0.86/hugg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 16:57:31.716549 hugg-0.0.86/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3533 2023-04-09 16:57:21.000000 hugg-0.0.86/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:48.368757 hugg-0.0.87/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-09 17:03:36.000000 hugg-0.0.87/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-09 17:03:48.368757 hugg-0.0.87/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-09 17:03:36.000000 hugg-0.0.87/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:48.368757 hugg-0.0.87/hugg/
+-rw-r--r--   0 runner    (1001) docker     (123)    36255 2023-04-09 17:03:36.000000 hugg-0.0.87/hugg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:03:48.368757 hugg-0.0.87/hugg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-09 17:03:48.000000 hugg-0.0.87/hugg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-09 17:03:48.000000 hugg-0.0.87/hugg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:03:48.000000 hugg-0.0.87/hugg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-09 17:03:48.000000 hugg-0.0.87/hugg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 17:03:48.000000 hugg-0.0.87/hugg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 17:03:48.368757 hugg-0.0.87/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3533 2023-04-09 17:03:36.000000 hugg-0.0.87/setup.py
```

### Comparing `hugg-0.0.86/LICENSE` & `hugg-0.0.87/LICENSE`

 * *Files identical despite different names*

### Comparing `hugg-0.0.86/hugg/__init__.py` & `hugg-0.0.87/hugg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -798,16 +798,17 @@
             print(":> "+str(encoding))
             if encoding is not None and encoding.strip() != '':
                 print("none")
                 current_contents = current_contents.decoded_content.decode(encoding)
                 encode_writing = "w+"
             else:
                 print("bin")
-                current_contents.encoding = "base64"
-                current_contents = current_contents.decoded_content
+                import base64
+                #base64.b64decode(bytearray(self.content, "utf-8"))
+                current_contents = bytearray(current_contents.content, "utf-8")
                 encode_writing = "wb+"
 
             with open(download_to,encode_writing) as writer:
                 writer.write(current_contents)
         return download_to
     
     def upload(self, file_path=None,path_in_repo=None):
```

### Comparing `hugg-0.0.86/setup.py` & `hugg-0.0.87/setup.py`

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
-VERSION = "0.0.86"
+VERSION = "0.0.87"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

