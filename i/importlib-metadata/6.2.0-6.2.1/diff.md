# Comparing `tmp/importlib_metadata-6.2.0.tar.gz` & `tmp/importlib_metadata-6.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "importlib_metadata-6.2.0.tar", last modified: Fri Apr  7 17:13:17 2023, max compression
+gzip compressed data, was "importlib_metadata-6.2.1.tar", last modified: Sun Apr  9 15:29:34 2023, max compression
```

## Comparing `importlib_metadata-6.2.0.tar` & `importlib_metadata-6.2.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.038359 importlib_metadata-6.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.038359 importlib_metadata-6.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.038359 importlib_metadata-6.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/docs/migration.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13802 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/docs/using.rst
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/exercises.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    26518 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/importlib_metadata/_py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/importlib_metadata/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/importlib_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/importlib_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-07 17:13:17.000000 importlib_metadata-6.2.0/importlib_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-07 17:13:17.000000 importlib_metadata-6.2.0/importlib_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 17:13:17.000000 importlib_metadata-6.2.0/importlib_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-07 17:13:17.000000 importlib_metadata-6.2.0/importlib_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-07 17:13:17.000000 importlib_metadata-6.2.0/importlib_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.038359 importlib_metadata-6.2.0/prepare/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/prepare/example/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/prepare/example/example/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/prepare/example/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/prepare/example/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/prepare/example2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/prepare/example2/example2/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/prepare/example2/example2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/prepare/example2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 17:13:17.042359 importlib_metadata-6.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/data/example-21.12-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/data/example-21.12-py3.6.egg
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/data/example2-1.0.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/test_py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tests/test_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-07 17:12:56.000000 importlib_metadata-6.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.870788 importlib_metadata-6.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.862788 importlib_metadata-6.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.862788 importlib_metadata-6.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20500 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-09 15:29:34.870788 importlib_metadata-6.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.862788 importlib_metadata-6.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/docs/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13802 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/docs/using.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/exercises.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.866788 importlib_metadata-6.2.1/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    26608 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/importlib_metadata/_py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/importlib_metadata/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/importlib_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.866788 importlib_metadata-6.2.1/importlib_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-09 15:29:34.000000 importlib_metadata-6.2.1/importlib_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-09 15:29:34.000000 importlib_metadata-6.2.1/importlib_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 15:29:34.000000 importlib_metadata-6.2.1/importlib_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-09 15:29:34.000000 importlib_metadata-6.2.1/importlib_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-09 15:29:34.000000 importlib_metadata-6.2.1/importlib_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.858788 importlib_metadata-6.2.1/prepare/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.866788 importlib_metadata-6.2.1/prepare/example/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.866788 importlib_metadata-6.2.1/prepare/example/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/prepare/example/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/prepare/example/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.870788 importlib_metadata-6.2.1/prepare/example2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.870788 importlib_metadata-6.2.1/prepare/example2/example2/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/prepare/example2/example2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/prepare/example2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-09 15:29:34.870788 importlib_metadata-6.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.870788 importlib_metadata-6.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:34.870788 importlib_metadata-6.2.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/data/example-21.12-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/data/example-21.12-py3.6.egg
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/data/example2-1.0.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/test_py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tests/test_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-09 15:29:12.000000 importlib_metadata-6.2.1/tox.ini
```

### Comparing `importlib_metadata-6.2.0/.github/workflows/main.yml` & `importlib_metadata-6.2.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/CHANGES.rst` & `importlib_metadata-6.2.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+v6.2.1
+======
+
+* #442: Fixed issue introduced in v6.1.0 where non-importable
+  names (metadata dirs) began appearing in
+  ``packages_distributions``.
+
 v6.2.0
 ======
 
 * #384: ``PackageMetadata`` now stipulates an additional ``get``
   method allowing for easy querying of metadata keys that may not
   be present.
```

### Comparing `importlib_metadata-6.2.0/LICENSE` & `importlib_metadata-6.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/PKG-INFO` & `importlib_metadata-6.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importlib_metadata
-Version: 6.2.0
+Version: 6.2.1
 Summary: Read metadata from Python packages
 Home-page: https://github.com/python/importlib_metadata
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `importlib_metadata-6.2.0/README.rst` & `importlib_metadata-6.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/conftest.py` & `importlib_metadata-6.2.1/conftest.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/docs/conf.py` & `importlib_metadata-6.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/docs/index.rst` & `importlib_metadata-6.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/docs/migration.rst` & `importlib_metadata-6.2.1/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/docs/using.rst` & `importlib_metadata-6.2.1/docs/using.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/exercises.py` & `importlib_metadata-6.2.1/exercises.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/importlib_metadata/__init__.py` & `importlib_metadata-6.2.1/importlib_metadata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -898,8 +898,13 @@
 
 
 def _top_level_inferred(dist):
     opt_names = {
         f.parts[0] if len(f.parts) > 1 else inspect.getmodulename(f)
         for f in always_iterable(dist.files)
     }
-    return filter(None, opt_names)
+
+    @pass_none
+    def importable_name(name):
+        return '.' not in name
+
+    return filter(importable_name, opt_names)
```

### Comparing `importlib_metadata-6.2.0/importlib_metadata/_adapters.py` & `importlib_metadata-6.2.1/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/importlib_metadata/_collections.py` & `importlib_metadata-6.2.1/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/importlib_metadata/_compat.py` & `importlib_metadata-6.2.1/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/importlib_metadata/_functools.py` & `importlib_metadata-6.2.1/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/importlib_metadata/_itertools.py` & `importlib_metadata-6.2.1/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/importlib_metadata/_meta.py` & `importlib_metadata-6.2.1/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/importlib_metadata/_py39compat.py` & `importlib_metadata-6.2.1/importlib_metadata/_py39compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/importlib_metadata/_text.py` & `importlib_metadata-6.2.1/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/importlib_metadata.egg-info/PKG-INFO` & `importlib_metadata-6.2.1/importlib_metadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importlib-metadata
-Version: 6.2.0
+Version: 6.2.1
 Summary: Read metadata from Python packages
 Home-page: https://github.com/python/importlib_metadata
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `importlib_metadata-6.2.0/importlib_metadata.egg-info/SOURCES.txt` & `importlib_metadata-6.2.1/importlib_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/pytest.ini` & `importlib_metadata-6.2.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/setup.cfg` & `importlib_metadata-6.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/tests/data/example-21.12-py3-none-any.whl` & `importlib_metadata-6.2.1/tests/data/example-21.12-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/tests/data/example-21.12-py3.6.egg` & `importlib_metadata-6.2.1/tests/data/example-21.12-py3.6.egg`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/tests/data/example2-1.0.0-py3-none-any.whl` & `importlib_metadata-6.2.1/tests/data/example2-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/tests/fixtures.py` & `importlib_metadata-6.2.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/tests/test_api.py` & `importlib_metadata-6.2.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/tests/test_integration.py` & `importlib_metadata-6.2.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/tests/test_main.py` & `importlib_metadata-6.2.1/tests/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,25 +331,28 @@
         fixtures.build_files(
             {
                 'all_distributions-1.0.0.dist-info': {
                     'METADATA': """
                         Name: all_distributions
                         Version: 1.0.0
                     """,
-                    'RECORD': ''.join(
-                        f'{i}-top-level{suffix},,\n'
-                        f'{i}-in-namespace/mod{suffix},,\n'
-                        f'{i}-in-package/__init__.py,,\n'
-                        f'{i}-in-package/mod{suffix},,\n'
+                    'RECORD': 'all_distributions-1.0.0.dist-info/METADATA\n'
+                    + ''.join(
+                        f'importable-name {i}{suffix},,\n'
+                        f'in_namespace_{i}/mod{suffix},,\n'
+                        f'in_package_{i}/__init__.py,,\n'
+                        f'in_package_{i}/mod{suffix},,\n'
                         for i, suffix in enumerate(suffixes)
                     ),
                 },
             },
             prefix=self.site_dir,
         )
 
         distributions = packages_distributions()
 
         for i in range(len(suffixes)):
-            assert distributions[f'{i}-top-level'] == ['all_distributions']
-            assert distributions[f'{i}-in-namespace'] == ['all_distributions']
-            assert distributions[f'{i}-in-package'] == ['all_distributions']
+            assert distributions[f'importable-name {i}'] == ['all_distributions']
+            assert distributions[f'in_namespace_{i}'] == ['all_distributions']
+            assert distributions[f'in_package_{i}'] == ['all_distributions']
+
+        assert not any(name.endswith('.dist-info') for name in distributions)
```

### Comparing `importlib_metadata-6.2.0/tests/test_py39compat.py` & `importlib_metadata-6.2.1/tests/test_py39compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/tests/test_zip.py` & `importlib_metadata-6.2.1/tests/test_zip.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.2.0/tox.ini` & `importlib_metadata-6.2.1/tox.ini`

 * *Files identical despite different names*

