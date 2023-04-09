# Comparing `tmp/pytest-describe-2.0.1.tar.gz` & `tmp/pytest-describe-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-describe-2.0.1.tar", last modified: Sat Nov 13 20:10:06 2021, max compression
+gzip compressed data, was "pytest-describe-2.0.2.tar", last modified: Sun Apr  9 14:53:32 2023, max compression
```

## Comparing `pytest-describe-2.0.1.tar` & `pytest-describe-2.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 20:10:06.757585 pytest-describe-2.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 20:10:06.753585 pytest-describe-2.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 20:10:06.753585 pytest-describe-2.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2225 2021-11-13 20:10:01.000000 pytest-describe-2.0.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)      569 2021-11-13 20:10:01.000000 pytest-describe-2.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1055 2021-11-13 20:10:01.000000 pytest-describe-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       86 2021-11-13 20:10:01.000000 pytest-describe-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5595 2021-11-13 20:10:06.757585 pytest-describe-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4389 2021-11-13 20:10:01.000000 pytest-describe-2.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 20:10:06.753585 pytest-describe-2.0.1/pytest_describe/
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-11-13 20:10:01.000000 pytest-describe-2.0.1/pytest_describe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4104 2021-11-13 20:10:01.000000 pytest-describe-2.0.1/pytest_describe/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      229 2021-11-13 20:10:01.000000 pytest-describe-2.0.1/pytest_describe/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 20:10:06.757585 pytest-describe-2.0.1/pytest_describe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5595 2021-11-13 20:10:06.000000 pytest-describe-2.0.1/pytest_describe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      573 2021-11-13 20:10:06.000000 pytest-describe-2.0.1/pytest_describe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-13 20:10:06.000000 pytest-describe-2.0.1/pytest_describe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-11-13 20:10:06.000000 pytest-describe-2.0.1/pytest_describe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-11-13 20:10:06.000000 pytest-describe-2.0.1/pytest_describe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-11-13 20:10:06.000000 pytest-describe-2.0.1/pytest_describe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-13 20:10:06.757585 pytest-describe-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1587 2021-11-13 20:10:01.000000 pytest-describe-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-13 20:10:06.757585 pytest-describe-2.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1732 2021-11-13 20:10:01.000000 pytest-describe-2.0.1/test/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (121)      790 2021-11-13 20:10:01.000000 pytest-describe-2.0.1/test/test_custom_prefix.py
--rw-r--r--   0 runner    (1001) docker     (121)     1615 2021-11-13 20:10:01.000000 pytest-describe-2.0.1/test/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)     8438 2021-11-13 20:10:01.000000 pytest-describe-2.0.1/test/test_marks.py
--rw-r--r--   0 runner    (1001) docker     (121)      758 2021-11-13 20:10:01.000000 pytest-describe-2.0.1/test/test_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     4984 2021-11-13 20:10:01.000000 pytest-describe-2.0.1/test/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2021-11-13 20:10:01.000000 pytest-describe-2.0.1/test/test_simple_execution.py
--rw-r--r--   0 runner    (1001) docker     (121)      220 2021-11-13 20:10:01.000000 pytest-describe-2.0.1/test/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2021-11-13 20:10:01.000000 pytest-describe-2.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:53:32.356340 pytest-describe-2.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:53:32.356340 pytest-describe-2.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:53:32.356340 pytest-describe-2.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-04-09 14:53:32.356340 pytest-describe-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:53:32.356340 pytest-describe-2.0.2/pytest_describe/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/pytest_describe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/pytest_describe/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/pytest_describe/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:53:32.356340 pytest-describe-2.0.2/pytest_describe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-04-09 14:53:32.000000 pytest-describe-2.0.2/pytest_describe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 14:53:32.000000 pytest-describe-2.0.2/pytest_describe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:53:32.000000 pytest-describe-2.0.2/pytest_describe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-09 14:53:32.000000 pytest-describe-2.0.2/pytest_describe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-09 14:53:32.000000 pytest-describe-2.0.2/pytest_describe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-09 14:53:32.000000 pytest-describe-2.0.2/pytest_describe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 14:53:32.356340 pytest-describe-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:53:32.356340 pytest-describe-2.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/test/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/test/test_custom_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/test/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/test/test_marks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/test/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/test/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/test/test_simple_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/test/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-09 14:53:26.000000 pytest-describe-2.0.2/tox.ini
```

### Comparing `pytest-describe-2.0.1/.github/workflows/main.yml` & `pytest-describe-2.0.2/.github/workflows/main.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,93 +1,93 @@
 name: main
 
 on:
   push:
     branches:
       - main
     tags:
-      - "*"
+      - '*'
 
   pull_request:
     branches:
       - main
 
 jobs:
   build:
-    runs-on: ubuntu-latest
+    runs-on: ubuntu-20.04
 
     strategy:
       matrix:
-        python: [3.6, 3.7, 3.8, 3.9, pypy3]
+        python: ['3.6', '3.7', '3.8', '3.9', '3.10', 'pypy3.9']
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
       with:
         fetch-depth: 0
 
     - name: Set up Python ${{ matrix.python }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python }}
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip setuptools
-        python -m pip install tox
+        python -m pip install 'tox>=3.28,<4.0'
 
     - name: Test with Python 3.6
       if: matrix.python == '3.6'
-      run: tox -e "py36-pytest_{4,50,51,52,53,54,60,61,62,latest}"
+      run: tox -e 'py36-pytest{4,50,51,52,53,54,60,61,62,70}'
 
     - name: Test with Python 3.7
       if: matrix.python == '3.7'
-      run: tox -e "py37-pytest_{4,50,51,52,53,54,60,61,62,latest}"
+      run: tox -e 'py37-pytest{4,50,51,52,53,54,60,61,62,70}'
 
     - name: Test with Python 3.8
       if: matrix.python == '3.8'
-      run: tox -e "py38-pytest_{4,50,51,52,53,54,60,61,62,latest}"
+      run: tox -e 'py38-pytest{4,50,51,52,53,54,60,61,62,70}'
 
     - name: Test with Python 3.9
       if: matrix.python == '3.9'
-      run: tox -e "py39-pytest_{4,50,51,52,53,54,60,61,62,latest}"
+      run: tox -e 'py39-pytest{4,50,51,52,53,54,60,61,62,70}'
 
     - name: Test with Python 3.10
       if: matrix.python == '3.10'
-      run: tox -e "py310-pytest_{62,latest}"
+      run: tox -e 'py310-pytest{62,70}'
 
-    - name: Test with PyPy
-      if: matrix.python == 'pypy3'
-      run: tox -e "pypy-pytest_{4,50,51,52,53,54,60,61,62,latest}"
+    - name: Test with PyPy 3.9
+      if: matrix.python == 'pypy3.9'
+      run: tox -e 'pypy39-pytest{4,50,51,52,53,54,60,61,62,70}'
 
     - name: Linting with Flake8
       if: matrix.python == '3.9'
       run: tox -e flake8
 
   deploy:
     if: |
       github.event_name == 'push' &&
       startsWith(github.event.ref, 'refs/tags') &&
       github.repository == 'pytest-dev/pytest-describe'
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
         with:
-          python-version: "3.9"
+          python-version: '3.9'
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install --upgrade wheel setuptools setuptools_scm
 
       - name: Build package
         run: python setup.py sdist bdist_wheel
 
       - name: Publish package
-        uses: pypa/gh-action-pypi-publish@v1.4.2
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.pypi_token }}
```

### Comparing `pytest-describe-2.0.1/.gitignore` & `pytest-describe-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-describe-2.0.1/LICENSE` & `pytest-describe-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-describe-2.0.1/PKG-INFO` & `pytest-describe-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-describe
-Version: 2.0.1
+Version: 2.0.2
 Summary: Describe-style plugin for pytest
 Home-page: https://github.com/pytest-dev/pytest-describe
 Author: Robin Pedersen
 Author-email: robinpeder@gmail.com
 Maintainer: Christoph Zwerschke
 Maintainer-email: cito@online.de
 License: MIT
@@ -169,9 +169,7 @@
 
         # the it_quacks test in this describe will fail (as expected)
 
 Fixtures defined in the block that includes the shared behavior take precedence
 over fixtures defined in the shared behavior. This rule only applies to
 fixtures, not to other functions (nested describe blocks and tests). Instead,
 they are all collected as separate tests.
-
-
```

### Comparing `pytest-describe-2.0.1/README.rst` & `pytest-describe-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-describe-2.0.1/pytest_describe/plugin.py` & `pytest-describe-2.0.2/pytest_describe/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-describe-2.0.1/pytest_describe.egg-info/PKG-INFO` & `pytest-describe-2.0.2/pytest_describe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-describe
-Version: 2.0.1
+Version: 2.0.2
 Summary: Describe-style plugin for pytest
 Home-page: https://github.com/pytest-dev/pytest-describe
 Author: Robin Pedersen
 Author-email: robinpeder@gmail.com
 Maintainer: Christoph Zwerschke
 Maintainer-email: cito@online.de
 License: MIT
@@ -169,9 +169,7 @@
 
         # the it_quacks test in this describe will fail (as expected)
 
 Fixtures defined in the block that includes the shared behavior take precedence
 over fixtures defined in the shared behavior. This rule only applies to
 fixtures, not to other functions (nested describe blocks and tests). Instead,
 they are all collected as separate tests.
-
-
```

### Comparing `pytest-describe-2.0.1/pytest_describe.egg-info/SOURCES.txt` & `pytest-describe-2.0.2/pytest_describe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-describe-2.0.1/setup.py` & `pytest-describe-2.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 
 with open("README.rst") as readme_file:
     readme = readme_file.read()
 
 
 setup(
     name='pytest-describe',
-    version='2.0.1',
+    version='2.0.2',
     description='Describe-style plugin for pytest',
     long_description=readme,
     long_description_content_type='text/x-rst',
     url='https://github.com/pytest-dev/pytest-describe',
     author='Robin Pedersen',
     author_email='robinpeder@gmail.com',
     maintainer='Christoph Zwerschke',
     maintainer_email='cito@online.de',
     license='MIT',
     license_file='LICENSE',
     platforms=['unix', 'linux', 'osx', 'cygwin', 'win32'],
     install_requires=[
-        'pytest>=4.0.0',
+        'pytest>=4.0,<7.1',
     ],
     entry_points={
         'pytest11': [
             'pytest-describe = pytest_describe.plugin',
         ],
     },
     packages=['pytest_describe'],
```

### Comparing `pytest-describe-2.0.1/test/test_collect.py` & `pytest-describe-2.0.2/test/test_collect.py`

 * *Files identical despite different names*

### Comparing `pytest-describe-2.0.1/test/test_custom_prefix.py` & `pytest-describe-2.0.2/test/test_custom_prefix.py`

 * *Files identical despite different names*

### Comparing `pytest-describe-2.0.1/test/test_fixtures.py` & `pytest-describe-2.0.2/test/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-describe-2.0.1/test/test_marks.py` & `pytest-describe-2.0.2/test/test_marks.py`

 * *Files identical despite different names*

### Comparing `pytest-describe-2.0.1/test/test_output.py` & `pytest-describe-2.0.2/test/test_output.py`

 * *Files identical despite different names*

### Comparing `pytest-describe-2.0.1/test/test_shared.py` & `pytest-describe-2.0.2/test/test_shared.py`

 * *Files identical despite different names*

### Comparing `pytest-describe-2.0.1/test/test_simple_execution.py` & `pytest-describe-2.0.2/test/test_simple_execution.py`

 * *Files identical despite different names*

### Comparing `pytest-describe-2.0.1/tox.ini` & `pytest-describe-2.0.2/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 [tox]
-envlist = py{36,37,38,39,py}-pytest_{4,50,51,52,53,54,60,61,62,latest,main},py{310}-pytest_{62,latest,main},flake8
+envlist = py{36,37,38,39,py39}-pytest{4,50,51,52,53,54,60,61,62,70},py{310}-pytest{62,70},flake8
 
 [testenv]
 basepython =
     py36: python3.6
     py37: python3.7
     py38: python3.8
     py39: python3.9
     py310: python3.10
-    pypy: pypy3
+    pypy39: pypy3.9
 deps =
-    pytest_4: pytest>=4.6,<5.0
-    pytest_50: pytest>=5.0,<5.2
-    pytest_51: pytest>=5.1,<5.2
-    pytest_52: pytest>=5.2,<5.3
-    pytest_53: pytest>=5.3,<5.4
-    pytest_54: pytest>=5.4,<5.5
-    pytest_60: pytest>=6.0,<6.1
-    pytest_61: pytest>=6.1,<6.2
-    pytest_62: pytest>=6.2,<6.3
-    pytest_latest: pytest
-    pytest_main: git+https://github.com/pytest-dev/pytest.git@main
+    pytest4: pytest>=4.6,<5.0
+    pytest50: pytest>=5.0,<5.2
+    pytest51: pytest>=5.1,<5.2
+    pytest52: pytest>=5.2,<5.3
+    pytest53: pytest>=5.3,<5.4
+    pytest54: pytest>=5.4,<5.5
+    pytest60: pytest>=6.0,<6.1
+    pytest61: pytest>=6.1,<6.2
+    pytest62: pytest>=6.2,<6.3
+    pytest70: pytest>=7.0,<7.1
+    pytest-latest: pytest
+    pytest-main: git+https://github.com/pytest-dev/pytest.git@main
 commands = pytest -rw {posargs}
 
 [testenv:flake8]
 basepython = python3.9
-deps = flake8>=4,<5
+deps = flake8>=6,<7
 commands =
     flake8 pytest_describe test setup.py
 
 [testenv:coverage]
 basepython = python3.9
 deps =
     coverage
```

