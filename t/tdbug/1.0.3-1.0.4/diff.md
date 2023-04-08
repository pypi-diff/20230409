# Comparing `tmp/tdbug-1.0.3.tar.gz` & `tmp/tdbug-1.0.4.tar.gz`

## Comparing `tdbug-1.0.3.tar` & `tdbug-1.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tdbug-1.0.3/MANIFEST.in
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 tdbug-1.0.3/setup.cfg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tdbug-1.0.3/src/tdbug/__init__.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 tdbug-1.0.3/src/tdbug/main.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tdbug-1.0.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tdbug-1.0.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tdbug-1.0.3/README.md
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 tdbug-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 tdbug-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tdbug-1.0.4/MANIFEST.in
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 tdbug-1.0.4/setup.cfg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tdbug-1.0.4/src/tdbug/__init__.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 tdbug-1.0.4/src/tdbug/main.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tdbug-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tdbug-1.0.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tdbug-1.0.4/README.md
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 tdbug-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 tdbug-1.0.4/PKG-INFO
```

### Comparing `tdbug-1.0.3/setup.cfg` & `tdbug-1.0.4/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tdbug
-version = 1.0.3
+version = 1.0.4
 author = Damon Pickett
 author_email = damon.pickett@gmail.com
 description = tdbug is a command-line application that uses the OpenAI API to diagnose bugs when programming.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/damonpickett/tdbug
 classifiers =
@@ -13,14 +13,17 @@
     Programming Language :: Python :: 3.8
     Programming Language :: Python :: 3.9
     License :: OSI Approved :: MIT License
     Operating System :: OS Independent
 
 [options]
 packages = find:
+setup_requires =
+    setuptools
+    wheel
 install_requires =
     openai
     python-dotenv
     rich
 python_requires = >=3.7
 
 [options.entry_points]
```

### Comparing `tdbug-1.0.3/src/tdbug/main.py` & `tdbug-1.0.4/src/tdbug/main.py`

 * *Files identical despite different names*

### Comparing `tdbug-1.0.3/LICENSE` & `tdbug-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tdbug-1.0.3/pyproject.toml` & `tdbug-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tdbug"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Damon Pickett", email="damon.pickett@gmail.com" },
 ]
 description = "tdbug is a command-line application that uses the OpenAI API to diagnose bugs when programming."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tdbug-1.0.3/PKG-INFO` & `tdbug-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdbug
-Version: 1.0.3
+Version: 1.0.4
 Summary: tdbug is a command-line application that uses the OpenAI API to diagnose bugs when programming.
 Project-URL: Homepage, https://github.com/damonpickett/tdbug
 Project-URL: Bug Tracker, https://github.com/damonpickett/tdbug/issues
 Author-email: Damon Pickett <damon.pickett@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

