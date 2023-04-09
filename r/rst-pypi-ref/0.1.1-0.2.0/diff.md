# Comparing `tmp/rst-pypi-ref-0.1.1.tar.gz` & `tmp/rst-pypi-ref-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rst-pypi-ref-0.1.1.tar", last modified: Thu Dec 22 15:28:08 2022, max compression
+gzip compressed data, was "rst-pypi-ref-0.2.0.tar", last modified: Sun Apr  9 02:38:32 2023, max compression
```

## Comparing `rst-pypi-ref-0.1.1.tar` & `rst-pypi-ref-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      560 2022-12-22 15:28:04.831586 rst-pypi-ref-0.1.1/.editorconfig
--rw-r--r--   0        0        0      788 2022-12-22 15:28:04.831586 rst-pypi-ref-0.1.1/.github/workflows/main.yml
--rw-r--r--   0        0        0     1863 2022-12-22 15:28:04.831586 rst-pypi-ref-0.1.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     3278 2022-12-22 15:28:04.831586 rst-pypi-ref-0.1.1/.gitignore
--rw-r--r--   0        0        0      492 2022-12-22 15:28:04.831586 rst-pypi-ref-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      268 2022-12-22 15:28:04.831586 rst-pypi-ref-0.1.1/CHANGES.rst
--rw-r--r--   0        0        0     9161 2022-12-22 15:28:04.831586 rst-pypi-ref-0.1.1/LICENSE
--rw-r--r--   0        0        0     1061 2022-12-22 15:28:04.831586 rst-pypi-ref-0.1.1/README.rst
--rw-r--r--   0        0        0     1386 2022-12-22 15:28:04.831586 rst-pypi-ref-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       78 2022-12-22 15:28:04.831586 rst-pypi-ref-0.1.1/rst_pypi_ref/__init__.py
--rwxr-xr-x   0        0        0      204 2022-12-22 15:28:04.831586 rst-pypi-ref-0.1.1/rst_pypi_ref/cli.py
--rw-r--r--   0        0        0      636 2022-12-22 15:28:04.831586 rst-pypi-ref-0.1.1/rst_pypi_ref/core.py
--rw-r--r--   0        0        0      384 2022-12-22 15:28:04.831586 rst-pypi-ref-0.1.1/rst_pypi_ref/sphinx.py
--rw-r--r--   0        0        0      741 2022-12-22 15:28:04.831586 rst-pypi-ref-0.1.1/setup.cfg
--rw-r--r--   0        0        0      317 2022-12-22 15:28:04.831586 rst-pypi-ref-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0       65 2022-12-22 15:28:04.831586 rst-pypi-ref-0.1.1/tests/roots/test-default/conf.py
--rw-r--r--   0        0        0      100 2022-12-22 15:28:04.831586 rst-pypi-ref-0.1.1/tests/roots/test-default/index.rst
--rw-r--r--   0        0        0      287 2022-12-22 15:28:04.831586 rst-pypi-ref-0.1.1/tests/test_it.py
--rw-r--r--   0        0        0      355 2022-12-22 15:28:04.831586 rst-pypi-ref-0.1.1/tests/test_sphinx.py
--rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 rst-pypi-ref-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      560 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/.editorconfig
+-rw-r--r--   0        0        0      792 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1863 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     3278 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/.gitignore
+-rw-r--r--   0        0        0      492 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      382 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/CHANGES.rst
+-rw-r--r--   0        0        0     9161 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1061 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/README.rst
+-rw-r--r--   0        0        0     1386 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/rst_pypi_ref/__init__.py
+-rwxr-xr-x   0        0        0      204 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/rst_pypi_ref/cli.py
+-rw-r--r--   0        0        0      926 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/rst_pypi_ref/core.py
+-rw-r--r--   0        0        0      384 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/rst_pypi_ref/sphinx.py
+-rw-r--r--   0        0        0      741 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/setup.cfg
+-rw-r--r--   0        0        0      317 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0       65 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/tests/roots/test-default/conf.py
+-rw-r--r--   0        0        0      100 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/tests/roots/test-default/index.rst
+-rw-r--r--   0        0        0      612 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/tests/test_it.py
+-rw-r--r--   0        0        0      355 2023-04-09 02:38:28.755431 rst-pypi-ref-0.2.0/tests/test_sphinx.py
+-rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 rst-pypi-ref-0.2.0/PKG-INFO
```

### Comparing `rst-pypi-ref-0.1.1/.editorconfig` & `rst-pypi-ref-0.2.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `rst-pypi-ref-0.1.1/.github/workflows/main.yml` & `rst-pypi-ref-0.2.0/.github/workflows/main.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: CI
+name: Run CI
 
 on:
   push:
   pull_request:
   workflow_dispatch:
 
 jobs:
```

### Comparing `rst-pypi-ref-0.1.1/.github/workflows/release.yml` & `rst-pypi-ref-0.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `rst-pypi-ref-0.1.1/.gitignore` & `rst-pypi-ref-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rst-pypi-ref-0.1.1/LICENSE` & `rst-pypi-ref-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rst-pypi-ref-0.1.1/README.rst` & `rst-pypi-ref-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `rst-pypi-ref-0.1.1/pyproject.toml` & `rst-pypi-ref-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rst-pypi-ref-0.1.1/setup.cfg` & `rst-pypi-ref-0.2.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.1
+current_version = 0.2.0
 commit = True
 tag = False
 message = release: Bump version {current_version} -> {new_version}
 
 [bumpversion:file:rst_pypi_ref/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
```

### Comparing `rst-pypi-ref-0.1.1/PKG-INFO` & `rst-pypi-ref-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rst-pypi-ref
-Version: 0.1.1
+Version: 0.2.0
 Summary: reStructuredText custom role to add ref to PyPI.
 Author-email: Kazuya Takei <myself@attakei.net>
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Sphinx
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

