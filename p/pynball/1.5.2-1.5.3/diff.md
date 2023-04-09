# Comparing `tmp/pynball-1.5.2.tar.gz` & `tmp/pynball-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynball-1.5.2.tar", last modified: Sat Apr  8 12:51:09 2023, max compression
+gzip compressed data, was "pynball-1.5.3.tar", last modified: Sun Apr  9 07:36:17 2023, max compression
```

## Comparing `pynball-1.5.2.tar` & `pynball-1.5.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 12:51:09.717115 pynball-1.5.2/
--rw-rw-rw-   0        0        0      155 2022-07-17 14:14:50.000000 pynball-1.5.2/AUTHORS.md
--rw-rw-rw-   0        0        0     6242 2023-04-08 12:50:59.000000 pynball-1.5.2/CHANGELOG.md
--rw-rw-rw-   0        0        0     1074 2022-05-31 13:06:01.000000 pynball-1.5.2/LICENSE
--rw-rw-rw-   0        0        0      203 2022-07-17 14:14:50.000000 pynball-1.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0    11835 2023-04-08 12:51:09.718115 pynball-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0    10522 2023-04-05 15:25:24.000000 pynball-1.5.2/README.md
--rw-rw-rw-   0        0        0     2212 2022-10-08 17:05:50.000000 pynball-1.5.2/pyproject.toml
--rw-rw-rw-   0        0        0     1550 2023-04-08 12:51:09.719115 pynball-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0      108 2022-05-31 13:06:01.000000 pynball-1.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 12:51:09.497115 pynball-1.5.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-08 12:51:09.549118 pynball-1.5.2/src/pynball/
--rw-rw-rw-   0        0        0      269 2023-04-08 12:50:59.000000 pynball-1.5.2/src/pynball/__init__.py
--rw-rw-rw-   0        0        0    30835 2023-04-06 18:58:07.000000 pynball-1.5.2/src/pynball/pynball.py
-drwxrwxrwx   0        0        0        0 2023-04-08 12:51:09.560116 pynball-1.5.2/src/pynball.egg-info/
--rw-rw-rw-   0        0        0    11835 2023-04-08 12:51:09.000000 pynball-1.5.2/src/pynball.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      693 2023-04-08 12:51:09.000000 pynball-1.5.2/src/pynball.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 12:51:09.000000 pynball-1.5.2/src/pynball.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-08 12:51:09.000000 pynball-1.5.2/src/pynball.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-04-08 12:51:09.000000 pynball-1.5.2/src/pynball.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-08 12:51:09.000000 pynball-1.5.2/src/pynball.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-08 12:51:09.716114 pynball-1.5.2/tests/
--rw-rw-rw-   0        0        0      574 2022-03-26 17:49:23.000000 pynball-1.5.2/tests/test__check_pyenv.py
--rw-rw-rw-   0        0        0     1159 2022-03-26 17:49:24.000000 pynball-1.5.2/tests/test__check_virtual_env.py
--rw-rw-rw-   0        0        0      374 2022-03-26 17:46:41.000000 pynball-1.5.2/tests/test__execute.py
--rw-rw-rw-   0        0        0     3502 2023-04-05 14:01:44.000000 pynball-1.5.2/tests/test__get_pynball.py
--rw-rw-rw-   0        0        0      759 2022-03-26 13:16:29.000000 pynball-1.5.2/tests/test__message.py
--rw-rw-rw-   0        0        0     1802 2022-04-04 12:59:03.000000 pynball-1.5.2/tests/test__set_get_del_env.py
--rw-rw-rw-   0        0        0      437 2022-04-03 21:08:13.000000 pynball-1.5.2/tests/test__set_pynball.py
--rw-rw-rw-   0        0        0     1183 2022-03-26 22:14:26.000000 pynball-1.5.2/tests/test_add.py
--rw-rw-rw-   0        0        0      630 2022-04-03 21:08:13.000000 pynball-1.5.2/tests/test_delete.py
--rw-rw-rw-   0        0        0      869 2022-04-06 20:25:30.000000 pynball-1.5.2/tests/test_lsproject.py
--rw-rw-rw-   0        0        0     1714 2022-03-27 15:36:00.000000 pynball-1.5.2/tests/test_mkproject.py
--rw-rw-rw-   0        0        0     1442 2022-03-27 15:34:50.000000 pynball-1.5.2/tests/test_rmproject.py
--rw-rw-rw-   0        0        0      418 2023-04-05 14:49:56.000000 pynball-1.5.2/tests/test_version.py
--rw-rw-rw-   0        0        0     1014 2023-04-05 14:01:44.000000 pynball-1.5.2/tests/test_versions.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:36:17.140355 pynball-1.5.3/
+-rw-rw-rw-   0        0        0      155 2022-07-17 14:14:50.000000 pynball-1.5.3/AUTHORS.md
+-rw-rw-rw-   0        0        0     6404 2023-04-09 07:36:04.000000 pynball-1.5.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1074 2022-05-31 13:06:01.000000 pynball-1.5.3/LICENSE
+-rw-rw-rw-   0        0        0      203 2022-07-17 14:14:50.000000 pynball-1.5.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    12054 2023-04-09 07:36:17.140355 pynball-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10737 2023-04-09 07:31:38.000000 pynball-1.5.3/README.md
+-rw-rw-rw-   0        0        0     2212 2022-10-08 17:05:50.000000 pynball-1.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1550 2023-04-09 07:36:17.155982 pynball-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      108 2022-05-31 13:06:01.000000 pynball-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:36:16.959407 pynball-1.5.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-09 07:36:16.993249 pynball-1.5.3/src/pynball/
+-rw-rw-rw-   0        0        0      269 2023-04-09 07:36:04.000000 pynball-1.5.3/src/pynball/__init__.py
+-rw-rw-rw-   0        0        0    30835 2023-04-06 18:58:07.000000 pynball-1.5.3/src/pynball/pynball.py
+drwxrwxrwx   0        0        0        0 2023-04-09 07:36:17.008911 pynball-1.5.3/src/pynball.egg-info/
+-rw-rw-rw-   0        0        0    12054 2023-04-09 07:36:16.000000 pynball-1.5.3/src/pynball.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      693 2023-04-09 07:36:16.000000 pynball-1.5.3/src/pynball.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 07:36:16.000000 pynball-1.5.3/src/pynball.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-09 07:36:16.000000 pynball-1.5.3/src/pynball.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-04-09 07:36:16.000000 pynball-1.5.3/src/pynball.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-09 07:36:16.000000 pynball-1.5.3/src/pynball.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 07:36:17.140355 pynball-1.5.3/tests/
+-rw-rw-rw-   0        0        0      574 2022-03-26 17:49:23.000000 pynball-1.5.3/tests/test__check_pyenv.py
+-rw-rw-rw-   0        0        0     1159 2022-03-26 17:49:24.000000 pynball-1.5.3/tests/test__check_virtual_env.py
+-rw-rw-rw-   0        0        0      374 2022-03-26 17:46:41.000000 pynball-1.5.3/tests/test__execute.py
+-rw-rw-rw-   0        0        0     3502 2023-04-05 14:01:44.000000 pynball-1.5.3/tests/test__get_pynball.py
+-rw-rw-rw-   0        0        0      759 2022-03-26 13:16:29.000000 pynball-1.5.3/tests/test__message.py
+-rw-rw-rw-   0        0        0     1802 2022-04-04 12:59:03.000000 pynball-1.5.3/tests/test__set_get_del_env.py
+-rw-rw-rw-   0        0        0      437 2022-04-03 21:08:13.000000 pynball-1.5.3/tests/test__set_pynball.py
+-rw-rw-rw-   0        0        0     1183 2022-03-26 22:14:26.000000 pynball-1.5.3/tests/test_add.py
+-rw-rw-rw-   0        0        0      630 2022-04-03 21:08:13.000000 pynball-1.5.3/tests/test_delete.py
+-rw-rw-rw-   0        0        0      869 2022-04-06 20:25:30.000000 pynball-1.5.3/tests/test_lsproject.py
+-rw-rw-rw-   0        0        0     1714 2022-03-27 15:36:00.000000 pynball-1.5.3/tests/test_mkproject.py
+-rw-rw-rw-   0        0        0     1442 2022-03-27 15:34:50.000000 pynball-1.5.3/tests/test_rmproject.py
+-rw-rw-rw-   0        0        0      418 2023-04-05 14:49:56.000000 pynball-1.5.3/tests/test_version.py
+-rw-rw-rw-   0        0        0     1014 2023-04-05 14:01:44.000000 pynball-1.5.3/tests/test_versions.py
```

### Comparing `pynball-1.5.2/CHANGELOG.md` & `pynball-1.5.3/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.5.3 (2023-04-09)
+### Fix
+* Missing url links ([`c7209ee`](https://github.com/Stephen-RA-King/pynball/commit/c7209eeeb1e09ea8cc35049d5d7deabd94104cc1))
+
 ## v1.5.2 (2023-04-08)
 ### Documentation
 * Add mnissing docstrings to functions ([`d19176f`](https://github.com/Stephen-RA-King/pynball/commit/d19176f36d3abe491f006757600bc87a885bbb20))
 * Update readme with test results & coverage ([`cad0b5e`](https://github.com/Stephen-RA-King/pynball/commit/cad0b5e8724936f652f3fe2a83c6f80173a129be))
 
 ## v1.5.1 (2023-03-14)
 ### Fix
```

### Comparing `pynball-1.5.2/LICENSE` & `pynball-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pynball-1.5.2/PKG-INFO` & `pynball-1.5.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynball
-Version: 1.5.2
+Version: 1.5.3
 Summary: Utility command line tool to manage python versions
 Home-page: https://github.com/stephen-ra-king/pynball
 Download-URL: 
 Author: Stephen R A King
 Author-email: stephen.ra.king@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: stephen.ra.king@gmail.com
@@ -76,19 +76,19 @@
 
 #### For Maximum Benefits additionally install the following:
 
 1. [**pyenv**][pyenv-url]
 
 ## Installation
 
-OS X & Linux:
+**OS X & Linux:**
 
 Will be supported in version 2
 
-Windows:
+**Windows:**
 
 ```sh
 pipx install pynball
 ```
 
 ## Usage example
 
@@ -282,20 +282,24 @@
 [lgtm-quality-image]: https://img.shields.io/lgtm/grade/python/g/Stephen-RA-King/pynball.svg?logo=lgtm&logoWidth=18
 [lgtm-quality-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynball/context:python
 [license-image]: https://img.shields.io/pypi/l/pynball
 [license-url]: https://github.com/Stephen-RA-King/pynball/blob/main/LICENSE
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
 [pip-tools-url]: https://github.com/jazzband/pip-tools/
+[pipx-url]: https://pypa.github.io/pipx/
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
 [pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/pynball/main.svg
 [pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/pynball/main
+[pyenv-url]: https://github.com/pyenv/pyenv
 [pypi-url]: https://pypi.org/project/pynball/
 [pypi-image]: https://img.shields.io/pypi/v/pynball.svg
 [python-version-image]: https://img.shields.io/pypi/pyversions/pynball
 [readthedocs-image]: https://readthedocs.org/projects/pynball/badge/?version=latest
 [readthedocs-url]: https://pynball.readthedocs.io/en/latest/?badge=latest
 [status-image]: https://img.shields.io/pypi/status/pynball.svg
 [tests-image]: https://github.com/Stephen-RA-King/pynball/actions/workflows/tests.yml/badge.svg
 [tests-url]: https://github.com/Stephen-RA-King/pynball/actions/workflows/tests.yml
+[virtualenv-url]: https://github.com/pypa/virtualenv
+[virtualenvwrapper-url]: https://pypi.org/project/virtualenvwrapper/
 [wiki]: https://github.com/Stephen-RA-King/pynball/wiki
```

### Comparing `pynball-1.5.2/README.md` & `pynball-1.5.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -47,19 +47,19 @@
 
 #### For Maximum Benefits additionally install the following:
 
 1. [**pyenv**][pyenv-url]
 
 ## Installation
 
-OS X & Linux:
+**OS X & Linux:**
 
 Will be supported in version 2
 
-Windows:
+**Windows:**
 
 ```sh
 pipx install pynball
 ```
 
 ## Usage example
 
@@ -253,20 +253,24 @@
 [lgtm-quality-image]: https://img.shields.io/lgtm/grade/python/g/Stephen-RA-King/pynball.svg?logo=lgtm&logoWidth=18
 [lgtm-quality-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynball/context:python
 [license-image]: https://img.shields.io/pypi/l/pynball
 [license-url]: https://github.com/Stephen-RA-King/pynball/blob/main/LICENSE
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
 [pip-tools-url]: https://github.com/jazzband/pip-tools/
+[pipx-url]: https://pypa.github.io/pipx/
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
 [pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/pynball/main.svg
 [pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/pynball/main
+[pyenv-url]: https://github.com/pyenv/pyenv
 [pypi-url]: https://pypi.org/project/pynball/
 [pypi-image]: https://img.shields.io/pypi/v/pynball.svg
 [python-version-image]: https://img.shields.io/pypi/pyversions/pynball
 [readthedocs-image]: https://readthedocs.org/projects/pynball/badge/?version=latest
 [readthedocs-url]: https://pynball.readthedocs.io/en/latest/?badge=latest
 [status-image]: https://img.shields.io/pypi/status/pynball.svg
 [tests-image]: https://github.com/Stephen-RA-King/pynball/actions/workflows/tests.yml/badge.svg
 [tests-url]: https://github.com/Stephen-RA-King/pynball/actions/workflows/tests.yml
+[virtualenv-url]: https://github.com/pypa/virtualenv
+[virtualenvwrapper-url]: https://pypi.org/project/virtualenvwrapper/
 [wiki]: https://github.com/Stephen-RA-King/pynball/wiki
```

### Comparing `pynball-1.5.2/pyproject.toml` & `pynball-1.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynball-1.5.2/setup.cfg` & `pynball-1.5.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pynball-1.5.2/src/pynball/pynball.py` & `pynball-1.5.3/src/pynball/pynball.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.2/src/pynball.egg-info/PKG-INFO` & `pynball-1.5.3/src/pynball.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynball
-Version: 1.5.2
+Version: 1.5.3
 Summary: Utility command line tool to manage python versions
 Home-page: https://github.com/stephen-ra-king/pynball
 Download-URL: 
 Author: Stephen R A King
 Author-email: stephen.ra.king@gmail.com
 Maintainer: Stephen R A King
 Maintainer-email: stephen.ra.king@gmail.com
@@ -76,19 +76,19 @@
 
 #### For Maximum Benefits additionally install the following:
 
 1. [**pyenv**][pyenv-url]
 
 ## Installation
 
-OS X & Linux:
+**OS X & Linux:**
 
 Will be supported in version 2
 
-Windows:
+**Windows:**
 
 ```sh
 pipx install pynball
 ```
 
 ## Usage example
 
@@ -282,20 +282,24 @@
 [lgtm-quality-image]: https://img.shields.io/lgtm/grade/python/g/Stephen-RA-King/pynball.svg?logo=lgtm&logoWidth=18
 [lgtm-quality-url]: https://lgtm.com/projects/g/Stephen-RA-King/pynball/context:python
 [license-image]: https://img.shields.io/pypi/l/pynball
 [license-url]: https://github.com/Stephen-RA-King/pynball/blob/main/LICENSE
 [mypy-image]: http://www.mypy-lang.org/static/mypy_badge.svg
 [mypy-url]: http://mypy-lang.org/
 [pip-tools-url]: https://github.com/jazzband/pip-tools/
+[pipx-url]: https://pypa.github.io/pipx/
 [pre-commit-image]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
 [pre-commit-url]: https://github.com/pre-commit/pre-commit
 [pre-commit.ci-image]: https://results.pre-commit.ci/badge/github/Stephen-RA-King/pynball/main.svg
 [pre-commit.ci-url]: https://results.pre-commit.ci/latest/github/Stephen-RA-King/pynball/main
+[pyenv-url]: https://github.com/pyenv/pyenv
 [pypi-url]: https://pypi.org/project/pynball/
 [pypi-image]: https://img.shields.io/pypi/v/pynball.svg
 [python-version-image]: https://img.shields.io/pypi/pyversions/pynball
 [readthedocs-image]: https://readthedocs.org/projects/pynball/badge/?version=latest
 [readthedocs-url]: https://pynball.readthedocs.io/en/latest/?badge=latest
 [status-image]: https://img.shields.io/pypi/status/pynball.svg
 [tests-image]: https://github.com/Stephen-RA-King/pynball/actions/workflows/tests.yml/badge.svg
 [tests-url]: https://github.com/Stephen-RA-King/pynball/actions/workflows/tests.yml
+[virtualenv-url]: https://github.com/pypa/virtualenv
+[virtualenvwrapper-url]: https://pypi.org/project/virtualenvwrapper/
 [wiki]: https://github.com/Stephen-RA-King/pynball/wiki
```

### Comparing `pynball-1.5.2/src/pynball.egg-info/SOURCES.txt` & `pynball-1.5.3/src/pynball.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynball-1.5.2/tests/test__check_pyenv.py` & `pynball-1.5.3/tests/test__check_pyenv.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.2/tests/test__check_virtual_env.py` & `pynball-1.5.3/tests/test__check_virtual_env.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.2/tests/test__get_pynball.py` & `pynball-1.5.3/tests/test__get_pynball.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.2/tests/test__message.py` & `pynball-1.5.3/tests/test__message.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.2/tests/test__set_get_del_env.py` & `pynball-1.5.3/tests/test__set_get_del_env.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.2/tests/test_add.py` & `pynball-1.5.3/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.2/tests/test_delete.py` & `pynball-1.5.3/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.2/tests/test_lsproject.py` & `pynball-1.5.3/tests/test_lsproject.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.2/tests/test_mkproject.py` & `pynball-1.5.3/tests/test_mkproject.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.2/tests/test_rmproject.py` & `pynball-1.5.3/tests/test_rmproject.py`

 * *Files identical despite different names*

### Comparing `pynball-1.5.2/tests/test_versions.py` & `pynball-1.5.3/tests/test_versions.py`

 * *Files identical despite different names*

