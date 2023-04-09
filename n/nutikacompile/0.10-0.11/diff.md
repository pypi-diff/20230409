# Comparing `tmp/nutikacompile-0.10.tar.gz` & `tmp/nutikacompile-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutikacompile-0.10.tar", last modified: Sun Apr  9 08:44:01 2023, max compression
+gzip compressed data, was "nutikacompile-0.11.tar", last modified: Sun Apr  9 13:33:15 2023, max compression
```

## Comparing `nutikacompile-0.10.tar` & `nutikacompile-0.11.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 08:44:01.176717 nutikacompile-0.10/
--rw-rw-rw-   0        0        0     1148 2023-04-09 08:43:55.000000 nutikacompile-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      141 2023-04-09 08:43:55.000000 nutikacompile-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     3963 2023-04-09 08:44:01.177714 nutikacompile-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     3202 2023-04-09 08:41:19.000000 nutikacompile-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 08:44:01.157768 nutikacompile-0.10/nutikacompile/
--rw-rw-rw-   0        0        0     1090 2023-03-31 02:03:52.000000 nutikacompile-0.10/nutikacompile/LICENSE
--rw-rw-rw-   0        0        0     3202 2023-04-09 08:41:19.000000 nutikacompile-0.10/nutikacompile/README.MD
--rw-rw-rw-   0        0        0     6477 2023-04-09 08:36:32.000000 nutikacompile-0.10/nutikacompile/__init__.py
--rw-rw-rw-   0        0        0       32 2023-04-09 08:43:58.000000 nutikacompile-0.10/nutikacompile/requirements.txt
--rw-rw-rw-   0        0        0    58415 2023-04-09 08:43:58.000000 nutikacompile-0.10/nutikacompile/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-09 08:44:01.172729 nutikacompile-0.10/nutikacompile.egg-info/
--rw-rw-rw-   0        0        0     3963 2023-04-09 08:44:00.000000 nutikacompile-0.10/nutikacompile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2023-04-09 08:44:00.000000 nutikacompile-0.10/nutikacompile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 08:44:00.000000 nutikacompile-0.10/nutikacompile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-09 08:44:00.000000 nutikacompile-0.10/nutikacompile.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-09 08:44:00.000000 nutikacompile-0.10/nutikacompile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-04-09 08:44:01.178712 nutikacompile-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1300 2023-04-09 08:43:58.000000 nutikacompile-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 13:33:15.342618 nutikacompile-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-04-09 13:33:10.000000 nutikacompile-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      141 2023-04-09 13:33:10.000000 nutikacompile-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     3963 2023-04-09 13:33:15.342618 nutikacompile-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     3202 2023-04-09 08:41:19.000000 nutikacompile-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 13:33:15.337632 nutikacompile-0.11/nutikacompile/
+-rw-rw-rw-   0        0        0     1090 2023-03-31 02:03:52.000000 nutikacompile-0.11/nutikacompile/LICENSE
+-rw-rw-rw-   0        0        0     3202 2023-04-09 08:41:19.000000 nutikacompile-0.11/nutikacompile/README.MD
+-rw-rw-rw-   0        0        0     6634 2023-04-09 13:32:32.000000 nutikacompile-0.11/nutikacompile/__init__.py
+-rw-rw-rw-   0        0        0       32 2023-04-09 13:33:14.000000 nutikacompile-0.11/nutikacompile/requirements.txt
+-rw-rw-rw-   0        0        0    58415 2023-04-09 13:33:14.000000 nutikacompile-0.11/nutikacompile/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-09 13:33:15.341620 nutikacompile-0.11/nutikacompile.egg-info/
+-rw-rw-rw-   0        0        0     3963 2023-04-09 13:33:15.000000 nutikacompile-0.11/nutikacompile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-04-09 13:33:15.000000 nutikacompile-0.11/nutikacompile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 13:33:15.000000 nutikacompile-0.11/nutikacompile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-09 13:33:15.000000 nutikacompile-0.11/nutikacompile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-09 13:33:15.000000 nutikacompile-0.11/nutikacompile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-04-09 13:33:15.343615 nutikacompile-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1300 2023-04-09 13:33:14.000000 nutikacompile-0.11/setup.py
```

### Comparing `nutikacompile-0.10/LICENSE.rst` & `nutikacompile-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `nutikacompile-0.10/PKG-INFO` & `nutikacompile-0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutikacompile
-Version: 0.10
+Version: 0.11
 Summary: A function that creates the cmd line for nuitka and executes it
 Home-page: https://github.com/hansalemaos/nutikacompile
 Author: Johannes Fischer
 Author-email: <aulasparticularesdealemaosp@gmail.com>
 License: MIT
 Keywords: nuitka,exe,compile
 Classifier: Development Status :: 4 - Beta
```

### Comparing `nutikacompile-0.10/README.md` & `nutikacompile-0.11/README.md`

 * *Files identical despite different names*

### Comparing `nutikacompile-0.10/nutikacompile/LICENSE` & `nutikacompile-0.11/nutikacompile/LICENSE`

 * *Files identical despite different names*

### Comparing `nutikacompile-0.10/nutikacompile/README.MD` & `nutikacompile-0.11/nutikacompile/README.MD`

 * *Files identical despite different names*

### Comparing `nutikacompile-0.10/nutikacompile/__init__.py` & `nutikacompile-0.11/nutikacompile/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,14 +100,15 @@
     disable_console: bool = True,
     onefile: bool = True,
     file_version: str = "1",
     outputdir: Union[str, None] = None,
     addfiles: Union[list, None] = None,
     delete_onefile_temp=False,
     needs_admin=False,
+    relativefolderinapps=None,
 ) -> str:
     r"""
     Compiles a Python file using Nuitka.
 
     Args:
         pyfile (str): The path to the Python file to be compiled.
         icon (Union[str, None], optional): The path to the icon file to be used for the compiled executable, all formats that PIL can read are fine. Defaults to None.
@@ -150,21 +151,23 @@
         addtocmd = addtocmd + foldercommand
     if needs_admin:
         addtocmd = addtocmd + " --windows-uac-admin"
 
     addtocmd = addtocmd + f" --file-version={file_version}"
 
     if not delete_onefile_temp:
-        basename = ".".join(os.path.basename(__file__).split(".")[:-1])
+        if not relativefolderinapps:
+            basename = ".".join(os.path.basename(pyfile).split(".")[:-1])
+        else:
+            basename = relativefolderinapps.strip('\\" ')
         cdi = f"%CACHE_DIR%/{basename}/{file_version}"
         addtocmd = addtocmd + f" --onefile-tempdir-spec={cdi}"
 
     backs = "\\"
     forw = "/"
     wholecommand = (
-        f'start "" "{sys.executable}" -m nuitka {pyfile.replace(backs, forw)} --assume-yes-for-downloads'
+        f'start "" "{sys.executable}" -m nuitka {pyfile.replace(backs, forw)} --standalone --assume-yes-for-downloads'
         + addtocmd
     )
     p = subprocess.Popen(wholecommand, shell=True)
 
     return wholecommand
-
```

### Comparing `nutikacompile-0.10/nutikacompile/thirdparty.json` & `nutikacompile-0.11/nutikacompile/thirdparty.json`

 * *Files identical despite different names*

### Comparing `nutikacompile-0.10/nutikacompile.egg-info/PKG-INFO` & `nutikacompile-0.11/nutikacompile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutikacompile
-Version: 0.10
+Version: 0.11
 Summary: A function that creates the cmd line for nuitka and executes it
 Home-page: https://github.com/hansalemaos/nutikacompile
 Author: Johannes Fischer
 Author-email: <aulasparticularesdealemaosp@gmail.com>
 License: MIT
 Keywords: nuitka,exe,compile
 Classifier: Development Status :: 4 - Beta
```

### Comparing `nutikacompile-0.10/setup.py` & `nutikacompile-0.11/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 #change to dict
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.10'
+VERSION = '0.11'
 DESCRIPTION = "A function that creates the cmd line for nuitka and executes it"
 
 # Setting up
 setup(
     name="nutikacompile",
     version=VERSION,
     license='MIT',
```

