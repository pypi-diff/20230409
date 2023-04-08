# Comparing `tmp/python-codicefiscale-0.7.1.tar.gz` & `tmp/python-codicefiscale-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-codicefiscale-0.7.1.tar", last modified: Thu Mar 30 11:27:52 2023, max compression
+gzip compressed data, was "python-codicefiscale-0.8.0.tar", last modified: Sat Apr  8 22:08:14 2023, max compression
```

## Comparing `python-codicefiscale-0.7.1.tar` & `python-codicefiscale-0.8.0.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:27:52.478323 python-codicefiscale-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-30 11:27:36.000000 python-codicefiscale-0.7.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-30 11:27:36.000000 python-codicefiscale-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-03-30 11:27:52.478323 python-codicefiscale-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-03-30 11:27:36.000000 python-codicefiscale-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:27:52.470322 python-codicefiscale-0.7.1/codicefiscale/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-30 11:27:36.000000 python-codicefiscale-0.7.1/codicefiscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-30 11:27:36.000000 python-codicefiscale-0.7.1/codicefiscale/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-03-30 11:27:36.000000 python-codicefiscale-0.7.1/codicefiscale/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15127 2023-03-30 11:27:36.000000 python-codicefiscale-0.7.1/codicefiscale/codicefiscale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:27:52.470322 python-codicefiscale-0.7.1/codicefiscale/data/
--rw-r--r--   0 runner    (1001) docker     (123)    70304 2023-03-30 11:27:36.000000 python-codicefiscale-0.7.1/codicefiscale/data/countries.json
--rw-r--r--   0 runner    (1001) docker     (123)  6904593 2023-03-30 11:27:36.000000 python-codicefiscale-0.7.1/codicefiscale/data/municipalities.json
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-03-30 11:27:36.000000 python-codicefiscale-0.7.1/codicefiscale/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 11:27:36.000000 python-codicefiscale-0.7.1/codicefiscale/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:27:52.478323 python-codicefiscale-0.7.1/python_codicefiscale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-03-30 11:27:52.000000 python-codicefiscale-0.7.1/python_codicefiscale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-30 11:27:52.000000 python-codicefiscale-0.7.1/python_codicefiscale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 11:27:52.000000 python-codicefiscale-0.7.1/python_codicefiscale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-30 11:27:52.000000 python-codicefiscale-0.7.1/python_codicefiscale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-30 11:27:52.000000 python-codicefiscale-0.7.1/python_codicefiscale.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-03-30 11:27:52.478323 python-codicefiscale-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-30 11:27:36.000000 python-codicefiscale-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 11:27:52.478323 python-codicefiscale-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    20109 2023-03-30 11:27:36.000000 python-codicefiscale-0.7.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    23931 2023-03-30 11:27:36.000000 python-codicefiscale-0.7.1/tests/test_codicefiscale.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-30 11:27:36.000000 python-codicefiscale-0.7.1/tests/test_issue_0016.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-03-30 11:27:36.000000 python-codicefiscale-0.7.1/tests/test_issue_0037.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-03-30 11:27:36.000000 python-codicefiscale-0.7.1/tests/test_issue_0079.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:08:14.123621 python-codicefiscale-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-08 22:08:02.000000 python-codicefiscale-0.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-08 22:08:02.000000 python-codicefiscale-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-04-08 22:08:14.123621 python-codicefiscale-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-04-08 22:08:02.000000 python-codicefiscale-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:08:14.115621 python-codicefiscale-0.8.0/codicefiscale/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-08 22:08:02.000000 python-codicefiscale-0.8.0/codicefiscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-08 22:08:02.000000 python-codicefiscale-0.8.0/codicefiscale/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-08 22:08:02.000000 python-codicefiscale-0.8.0/codicefiscale/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-04-08 22:08:02.000000 python-codicefiscale-0.8.0/codicefiscale/codicefiscale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:08:14.115621 python-codicefiscale-0.8.0/codicefiscale/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    70304 2023-04-08 22:08:02.000000 python-codicefiscale-0.8.0/codicefiscale/data/countries.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-08 22:08:02.000000 python-codicefiscale-0.8.0/codicefiscale/data/deleted-countries.json
+-rw-r--r--   0 runner    (1001) docker     (123)  6904593 2023-04-08 22:08:02.000000 python-codicefiscale-0.8.0/codicefiscale/data/municipalities.json
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-08 22:08:02.000000 python-codicefiscale-0.8.0/codicefiscale/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 22:08:02.000000 python-codicefiscale-0.8.0/codicefiscale/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-08 22:08:02.000000 python-codicefiscale-0.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:08:14.123621 python-codicefiscale-0.8.0/python_codicefiscale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-04-08 22:08:14.000000 python-codicefiscale-0.8.0/python_codicefiscale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-08 22:08:14.000000 python-codicefiscale-0.8.0/python_codicefiscale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 22:08:14.000000 python-codicefiscale-0.8.0/python_codicefiscale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-08 22:08:14.000000 python-codicefiscale-0.8.0/python_codicefiscale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-08 22:08:14.000000 python-codicefiscale-0.8.0/python_codicefiscale.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 22:08:14.123621 python-codicefiscale-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-08 22:08:02.000000 python-codicefiscale-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:08:14.123621 python-codicefiscale-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20109 2023-04-08 22:08:02.000000 python-codicefiscale-0.8.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23931 2023-04-08 22:08:02.000000 python-codicefiscale-0.8.0/tests/test_codicefiscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-08 22:08:02.000000 python-codicefiscale-0.8.0/tests/test_issue_0016.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-08 22:08:02.000000 python-codicefiscale-0.8.0/tests/test_issue_0036.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-08 22:08:02.000000 python-codicefiscale-0.8.0/tests/test_issue_0037.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-08 22:08:02.000000 python-codicefiscale-0.8.0/tests/test_issue_0079.py
```

### Comparing `python-codicefiscale-0.7.1/LICENSE.txt` & `python-codicefiscale-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-codicefiscale-0.7.1/PKG-INFO` & `python-codicefiscale-0.8.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,37 @@
 Metadata-Version: 2.1
 Name: python-codicefiscale
-Version: 0.7.1
+Version: 0.8.0
 Summary: encode / decode italian fiscal codes - codifica / decodifica del Codice Fiscale italiano.
-Home-page: https://github.com/fabiocaccamo/python-codicefiscale
-Download-URL: https://github.com/fabiocaccamo/python-codicefiscale/releases
-Author: Fabio Caccamo
-Author-email: fabio.caccamo@gmail.com
-Maintainer: Fabio Caccamo
-Maintainer-email: fabio.caccamo@gmail.com
-License: MIT
+Author-email: Fabio Caccamo <fabio.caccamo@gmail.com>
+Maintainer-email: Fabio Caccamo <fabio.caccamo@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2017-present Fabio Caccamo
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/fabiocaccamo/python-codicefiscale
+Project-URL: Download, https://github.com/fabiocaccamo/python-codicefiscale/releases
 Project-URL: Documentation, https://github.com/fabiocaccamo/python-codicefiscale#readme
 Project-URL: Issues, https://github.com/fabiocaccamo/python-codicefiscale/issues
 Project-URL: Funding, https://github.com/sponsors/fabiocaccamo/
 Project-URL: Twitter, https://twitter.com/fabiocaccamo
 Keywords: codicefiscale,codice,fiscale,cf,fiscal code,italia,italy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `python-codicefiscale-0.7.1/README.md` & `python-codicefiscale-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `python-codicefiscale-0.7.1/codicefiscale/cli.py` & `python-codicefiscale-0.8.0/codicefiscale/cli.py`

 * *Files identical despite different names*

### Comparing `python-codicefiscale-0.7.1/codicefiscale/codicefiscale.py` & `python-codicefiscale-0.8.0/codicefiscale/codicefiscale.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     "4": "Q",
     "5": "R",
     "6": "S",
     "7": "T",
     "8": "U",
     "9": "V",
 }
-_OMOCODIA_DIGITS: str = "".join([digit for digit in _OMOCODIA])
+_OMOCODIA_DIGITS: str = "".join(list(_OMOCODIA))
 _OMOCODIA_LETTERS: str = "".join([_OMOCODIA[digit] for digit in _OMOCODIA])
 _OMOCODIA_ENCODE_TRANS: dict[int, int] = "".maketrans(
     _OMOCODIA_DIGITS, _OMOCODIA_LETTERS
 )
 _OMOCODIA_DECODE_TRANS: dict[int, int] = "".maketrans(
     _OMOCODIA_LETTERS, _OMOCODIA_DIGITS
 )
@@ -84,15 +84,15 @@
     return fsutil.read_file_json(fsutil.join_path(__file__, f"data/{filename}"))
 
 
 def _get_indexed_data() -> (
     dict[str, dict[str, list[dict[str, bool | datetime | str | list[str]]]]]
 ):
     municipalities = _get_data("municipalities.json")
-    countries = _get_data("countries.json")
+    countries = _get_data("deleted-countries.json") + _get_data("countries.json")
     data: dict[str, dict[str, list[dict[str, bool | datetime | str | list[str]]]]] = {
         "municipalities": {},
         "countries": {},
         "codes": {},
     }
 
     for municipality in municipalities:
```

### Comparing `python-codicefiscale-0.7.1/codicefiscale/data/countries.json` & `python-codicefiscale-0.8.0/codicefiscale/data/countries.json`

 * *Files identical despite different names*

### Comparing `python-codicefiscale-0.7.1/codicefiscale/data/municipalities.json` & `python-codicefiscale-0.8.0/codicefiscale/data/municipalities.json`

 * *Files identical despite different names*

### Comparing `python-codicefiscale-0.7.1/python_codicefiscale.egg-info/PKG-INFO` & `python-codicefiscale-0.8.0/python_codicefiscale.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,37 @@
 Metadata-Version: 2.1
 Name: python-codicefiscale
-Version: 0.7.1
+Version: 0.8.0
 Summary: encode / decode italian fiscal codes - codifica / decodifica del Codice Fiscale italiano.
-Home-page: https://github.com/fabiocaccamo/python-codicefiscale
-Download-URL: https://github.com/fabiocaccamo/python-codicefiscale/releases
-Author: Fabio Caccamo
-Author-email: fabio.caccamo@gmail.com
-Maintainer: Fabio Caccamo
-Maintainer-email: fabio.caccamo@gmail.com
-License: MIT
+Author-email: Fabio Caccamo <fabio.caccamo@gmail.com>
+Maintainer-email: Fabio Caccamo <fabio.caccamo@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2017-present Fabio Caccamo
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/fabiocaccamo/python-codicefiscale
+Project-URL: Download, https://github.com/fabiocaccamo/python-codicefiscale/releases
 Project-URL: Documentation, https://github.com/fabiocaccamo/python-codicefiscale#readme
 Project-URL: Issues, https://github.com/fabiocaccamo/python-codicefiscale/issues
 Project-URL: Funding, https://github.com/sponsors/fabiocaccamo/
 Project-URL: Twitter, https://twitter.com/fabiocaccamo
 Keywords: codicefiscale,codice,fiscale,cf,fiscal code,italia,italy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `python-codicefiscale-0.7.1/python_codicefiscale.egg-info/SOURCES.txt` & `python-codicefiscale-0.8.0/python_codicefiscale.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 LICENSE.txt
 MANIFEST.in
 README.md
-setup.cfg
+pyproject.toml
 setup.py
 codicefiscale/__init__.py
 codicefiscale/__main__.py
 codicefiscale/cli.py
 codicefiscale/codicefiscale.py
 codicefiscale/metadata.py
 codicefiscale/py.typed
 codicefiscale/data/countries.json
+codicefiscale/data/deleted-countries.json
 codicefiscale/data/municipalities.json
 python_codicefiscale.egg-info/PKG-INFO
 python_codicefiscale.egg-info/SOURCES.txt
 python_codicefiscale.egg-info/dependency_links.txt
 python_codicefiscale.egg-info/requires.txt
 python_codicefiscale.egg-info/top_level.txt
 tests/test_cli.py
 tests/test_codicefiscale.py
 tests/test_issue_0016.py
+tests/test_issue_0036.py
 tests/test_issue_0037.py
 tests/test_issue_0079.py
```

### Comparing `python-codicefiscale-0.7.1/setup.cfg` & `python-codicefiscale-0.8.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,96 @@
-[metadata]
-name = python-codicefiscale
-version = attr: codicefiscale.metadata.__version__
-author = Fabio Caccamo
-author_email = fabio.caccamo@gmail.com
-maintainer = Fabio Caccamo
-maintainer_email = fabio.caccamo@gmail.com
-description = encode / decode italian fiscal codes - codifica / decodifica del Codice Fiscale italiano.
-keywords = 
-	codicefiscale
-	codice
-	fiscale
-	cf
-	fiscal code
-	italia
-	italy
-url = https://github.com/fabiocaccamo/%(name)s
-download_url = https://github.com/fabiocaccamo/%(name)s/releases
-license = MIT
-long_description = file: README.md
-long_description_content_type = text/markdown
-classifiers = 
-	Development Status :: 5 - Production/Stable
-	Environment :: Web Environment
-	Intended Audience :: Developers
-	License :: OSI Approved :: MIT License
-	Natural Language :: English
-	Operating System :: OS Independent
-	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
-	Programming Language :: Python :: 3.11
-	Programming Language :: Python :: Implementation :: PyPy
-	Topic :: Software Development :: Build Tools
-project_urls = 
-	Documentation = https://github.com/fabiocaccamo/%(name)s#readme
-	Issues = https://github.com/fabiocaccamo/%(name)s/issues
-	Funding = https://github.com/sponsors/fabiocaccamo/
-	Twitter = https://twitter.com/fabiocaccamo
-
-[options]
-packages = find:
-install_requires = 
-	python-dateutil ~= 2.8.0, < 3.0.0
-	python-fsutil >= 0.10.0, < 1.0.0
-	python-slugify >= 7.0.0, < 9.0.0
-include_package_data = True
-
-[options.packages.find]
-exclude = 
-	docs*
-	images*
-	scripts*
-	tests*
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "python-codicefiscale"
+description = "encode / decode italian fiscal codes - codifica / decodifica del Codice Fiscale italiano."
+authors = [
+    { name = "Fabio Caccamo", email = "fabio.caccamo@gmail.com" },
+]
+keywords = [
+    "codicefiscale",
+    "codice",
+    "fiscale",
+    "cf",
+    "fiscal code",
+    "italia",
+    "italy",
+]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Environment :: Web Environment",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Natural Language :: English",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: Implementation :: PyPy",
+    "Topic :: Software Development :: Build Tools",
+]
+dependencies = [
+    "python-dateutil ~= 2.8.0, < 3.0.0",
+    "python-fsutil >= 0.10.0, < 1.0.0",
+    "python-slugify >= 7.0.0, < 9.0.0",
+]
+dynamic = ["version"]
+maintainers = [
+    { name = "Fabio Caccamo", email = "fabio.caccamo@gmail.com" },
+]
+
+[project.readme]
+file = "README.md"
+content-type = "text/markdown"
+
+[project.license]
+file = "LICENSE.txt"
+content-type = "text/plain"
+
+[project.urls]
+Homepage = "https://github.com/fabiocaccamo/python-codicefiscale"
+Download = "https://github.com/fabiocaccamo/python-codicefiscale/releases"
+Documentation = "https://github.com/fabiocaccamo/python-codicefiscale#readme"
+Issues = "https://github.com/fabiocaccamo/python-codicefiscale/issues"
+Funding = "https://github.com/sponsors/fabiocaccamo/"
+Twitter = "https://twitter.com/fabiocaccamo"
+
+[tool.black]
+line-length = 88
+include = '\.pyi?$'
+exclude = '''
+/(
+    \.git
+  | \.hg
+  | \.mypy_cache
+  | \.tox
+  | \.venv
+  | _build
+  | buck-out
+  | build
+  | dist
+  | venv
+)/
+'''
+
+[tool.mypy]
+files = ["codicefiscale"]
+ignore_missing_imports = true
+strict = true
+
+[tool.ruff]
+ignore = []
+line-length = 88
+select = ["B", "B9", "C", "E", "F", "W"]
 
-[flake8]
-max-line-length = 88
+[tool.ruff.mccabe]
 max-complexity = 10
-select = B,C,E,F,W,T4,B9
 
-[mypy]
-files = codicefiscale
-ignore_missing_imports = True
-strict = True
-
-[egg_info]
-tag_build = 
-tag_date = 0
+[tool.setuptools.packages.find]
+include = ["codicefiscale*"]
 
+[tool.setuptools.dynamic.version]
+attr = "codicefiscale.metadata.__version__"
```

### Comparing `python-codicefiscale-0.7.1/tests/test_cli.py` & `python-codicefiscale-0.8.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `python-codicefiscale-0.7.1/tests/test_codicefiscale.py` & `python-codicefiscale-0.8.0/tests/test_codicefiscale.py`

 * *Files identical despite different names*

### Comparing `python-codicefiscale-0.7.1/tests/test_issue_0016.py` & `python-codicefiscale-0.8.0/tests/test_issue_0016.py`

 * *Files identical despite different names*

### Comparing `python-codicefiscale-0.7.1/tests/test_issue_0037.py` & `python-codicefiscale-0.8.0/tests/test_issue_0037.py`

 * *Files identical despite different names*

### Comparing `python-codicefiscale-0.7.1/tests/test_issue_0079.py` & `python-codicefiscale-0.8.0/tests/test_issue_0079.py`

 * *Files identical despite different names*

