# Comparing `tmp/chromat-0.0.2.tar.gz` & `tmp/chromat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromat-0.0.2.tar", max compression
+gzip compressed data, was "chromat-0.0.3.tar", max compression
```

## Comparing `chromat-0.0.2.tar` & `chromat-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0       61 2023-04-08 22:20:34.106730 chromat-0.0.2/chromat/__init__.py
--rw-r--r--   0        0        0     1273 2023-04-08 22:21:02.542212 chromat-0.0.2/chromat/printing.py
--rw-r--r--   0        0        0      818 2023-04-08 22:19:46.760887 chromat-0.0.2/chromat/swatches.py
--rw-r--r--   0        0        0     3958 2023-04-08 22:19:40.309035 chromat-0.0.2/chromat/utils.py
--rw-r--r--   0        0        0      701 2023-04-09 00:35:25.668676 chromat-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       93 2023-04-03 02:42:30.536779 chromat-0.0.2/README.md
--rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 chromat-0.0.2/setup.py
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 chromat-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-04-08 22:20:34.106730 chromat-0.0.3/chromat/__init__.py
+-rw-r--r--   0        0        0      244 2023-04-07 19:33:13.563276 chromat-0.0.3/chromat/app.py
+-rw-r--r--   0        0        0     1273 2023-04-08 22:21:02.542212 chromat-0.0.3/chromat/printing.py
+-rw-r--r--   0        0        0      818 2023-04-08 22:19:46.760887 chromat-0.0.3/chromat/swatches.py
+-rw-r--r--   0        0        0     3958 2023-04-08 22:19:40.309035 chromat-0.0.3/chromat/utils.py
+-rw-r--r--   0        0        0     1312 2023-04-09 00:46:50.451732 chromat-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-04-03 02:42:30.536779 chromat-0.0.3/README.md
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 chromat-0.0.3/setup.py
+-rw-r--r--   0        0        0     1158 1970-01-01 00:00:00.000000 chromat-0.0.3/PKG-INFO
```

### Comparing `chromat-0.0.2/chromat/printing.py` & `chromat-0.0.3/chromat/printing.py`

 * *Files identical despite different names*

### Comparing `chromat-0.0.2/chromat/swatches.py` & `chromat-0.0.3/chromat/swatches.py`

 * *Files identical despite different names*

### Comparing `chromat-0.0.2/chromat/utils.py` & `chromat-0.0.3/chromat/utils.py`

 * *Files identical despite different names*

### Comparing `chromat-0.0.2/pyproject.toml` & `chromat-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,51 @@
 [tool.poetry]
 name = "chromat"
-version = "0.0.2"
+version = "0.0.3"
 description = "color palettes! under heavy construction!"
+license = "GPL-3.0-or-later"
 authors = ["hex benjamin <hex@hexbenjam.in>"]
 readme = "README.md"
+repository = "https://github.com/hexbenjamin/chromat"
+keywords = ["color", "palette"]
+classifiers = [
+    "Development Status :: 1 - Planning",
+    "Environment :: Console",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+    "Natural Language :: English",
+    "Operating System :: Microsoft :: Windows :: Windows 10",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.10",
+    "Topic :: Artistic Software",
+    "Topic :: Utilities",
+]
+packages = [
+    { include = "chromat" },
+]
 exclude = [
     "backup/*",
     "img/*",
     "tests/*",
     "__pycache__/*",
     "*.dist-info/*",
     "*.egg-info/*",
     "*.pyc",
     ".flake8",
+    ".gitignore",
     "testing.py",
-    "chromat/app.py",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-textual = {extras = ["dev"], version = "^0.18.0"}
+textual = "^0.18.0"
 colour = "^0.1.5"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.2"
 black = "^23.3.0"
-mypy = "^1.1.1"
 flake8 = "^6.0.0"
+mypy = "^1.1.1"
+pytest = "^7.2.2"
+textual = {extras = ["dev"], version = "^0.18.0"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `chromat-0.0.2/setup.py` & `chromat-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 packages = \
 ['chromat']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['colour>=0.1.5,<0.2.0', 'textual[dev]>=0.18.0,<0.19.0']
+['colour>=0.1.5,<0.2.0', 'textual>=0.18.0,<0.19.0']
 
 setup_kwargs = {
     'name': 'chromat',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'color palettes! under heavy construction!',
     'long_description': '\ufeff# chromat: algorithmic color palettes\ncoming soon!\n\nhttps://github.com/hexbenjamin/chromat',
     'author': 'hex benjamin',
     'author_email': 'hex@hexbenjam.in',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/hexbenjamin/chromat',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.10,<4.0',
 }
```

