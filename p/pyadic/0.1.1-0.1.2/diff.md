# Comparing `tmp/pyadic-0.1.1.tar.gz` & `tmp/pyadic-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyadic-0.1.1.tar", last modified: Tue Apr  4 10:23:24 2023, max compression
+gzip compressed data, was "pyadic-0.1.2.tar", last modified: Sun Apr  9 16:18:32 2023, max compression
```

## Comparing `pyadic-0.1.1.tar` & `pyadic-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2023-04-04 10:23:24.801108 pyadic-0.1.1/
-drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2023-04-04 10:23:24.797108 pyadic-0.1.1/.github/
-drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2023-04-04 10:23:24.797108 pyadic-0.1.1/.github/workflows/
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     1175 2022-07-29 17:12:44.000000 pyadic-0.1.1/.github/workflows/continuous_integration.yml
--rw-rw-r--   0 gdl       (1000) gdl       (1000)       67 2021-07-14 17:26:37.000000 pyadic-0.1.1/.gitignore
--rw-rw-r--   0 gdl       (1000) gdl       (1000)       15 2022-07-25 22:46:02.000000 pyadic-0.1.1/.hidden
--rw-rw-r--   0 gdl       (1000) gdl       (1000)    35149 2022-03-24 18:46:40.000000 pyadic-0.1.1/LICENSE.txt
--rw-rw-r--   0 gdl       (1000) gdl       (1000)      237 2023-04-04 10:23:24.801108 pyadic-0.1.1/PKG-INFO
--rw-rw-r--   0 gdl       (1000) gdl       (1000)      872 2022-10-21 11:10:53.000000 pyadic-0.1.1/README.md
-drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2023-04-04 10:23:24.801108 pyadic-0.1.1/pyadic/
--rw-rw-r--   0 gdl       (1000) gdl       (1000)       11 2022-07-25 22:51:57.000000 pyadic-0.1.1/pyadic/.hidden
--rw-rw-r--   0 gdl       (1000) gdl       (1000)      108 2022-07-25 22:49:35.000000 pyadic-0.1.1/pyadic/__init__.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     3949 2022-07-31 00:56:53.000000 pyadic-0.1.1/pyadic/field_extension.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)    12138 2023-04-03 14:45:25.000000 pyadic-0.1.1/pyadic/finite_field.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)    13212 2023-03-22 15:28:46.000000 pyadic-0.1.1/pyadic/padic.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     1380 2023-04-03 14:45:28.000000 pyadic-0.1.1/pyadic/primes.py
-drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2023-04-04 10:23:24.801108 pyadic-0.1.1/pyadic.egg-info/
--rw-rw-r--   0 gdl       (1000) gdl       (1000)      237 2023-04-04 10:23:24.000000 pyadic-0.1.1/pyadic.egg-info/PKG-INFO
--rw-rw-r--   0 gdl       (1000) gdl       (1000)      489 2023-04-04 10:23:24.000000 pyadic-0.1.1/pyadic.egg-info/SOURCES.txt
--rw-rw-r--   0 gdl       (1000) gdl       (1000)        1 2023-04-04 10:23:24.000000 pyadic-0.1.1/pyadic.egg-info/dependency_links.txt
--rw-rw-r--   0 gdl       (1000) gdl       (1000)       12 2023-04-04 10:23:24.000000 pyadic-0.1.1/pyadic.egg-info/requires.txt
--rw-rw-r--   0 gdl       (1000) gdl       (1000)        7 2023-04-04 10:23:24.000000 pyadic-0.1.1/pyadic.egg-info/top_level.txt
--rw-rw-r--   0 gdl       (1000) gdl       (1000)       14 2022-10-21 11:06:30.000000 pyadic-0.1.1/runtime.txt
--rw-rw-r--   0 gdl       (1000) gdl       (1000)      201 2023-04-04 10:23:24.801108 pyadic-0.1.1/setup.cfg
--rw-rw-r--   0 gdl       (1000) gdl       (1000)      331 2023-04-04 10:22:38.000000 pyadic-0.1.1/setup.py
-drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2023-04-04 10:23:24.801108 pyadic-0.1.1/tests/
--rw-rw-r--   0 gdl       (1000) gdl       (1000)       11 2022-07-25 22:51:57.000000 pyadic-0.1.1/tests/.hidden
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     1716 2022-07-29 22:37:00.000000 pyadic-0.1.1/tests/test_field_extension.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     5176 2023-04-03 14:47:29.000000 pyadic-0.1.1/tests/test_finite_field.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     4320 2023-01-11 15:39:03.000000 pyadic-0.1.1/tests/test_padic.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     1253 2022-07-25 22:36:25.000000 pyadic-0.1.1/update-badges.py
+drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2023-04-09 16:18:32.394642 pyadic-0.1.2/
+drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2023-04-09 16:18:32.394642 pyadic-0.1.2/.github/
+drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2023-04-09 16:18:32.394642 pyadic-0.1.2/.github/workflows/
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)     1175 2022-07-29 17:12:44.000000 pyadic-0.1.2/.github/workflows/continuous_integration.yml
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)       67 2021-07-14 17:26:37.000000 pyadic-0.1.2/.gitignore
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)       15 2022-07-25 22:46:02.000000 pyadic-0.1.2/.hidden
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)    35149 2022-03-24 18:46:40.000000 pyadic-0.1.2/LICENSE.txt
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)     3745 2023-04-09 16:18:32.394642 pyadic-0.1.2/PKG-INFO
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)     2908 2023-04-09 16:16:15.000000 pyadic-0.1.2/README.md
+drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2023-04-09 16:18:32.394642 pyadic-0.1.2/pyadic/
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)       11 2022-07-25 22:51:57.000000 pyadic-0.1.2/pyadic/.hidden
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)      108 2022-07-25 22:49:35.000000 pyadic-0.1.2/pyadic/__init__.py
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)     3949 2022-07-31 00:56:53.000000 pyadic-0.1.2/pyadic/field_extension.py
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)    12138 2023-04-03 14:45:25.000000 pyadic-0.1.2/pyadic/finite_field.py
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)    13212 2023-03-22 15:28:46.000000 pyadic-0.1.2/pyadic/padic.py
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)     1380 2023-04-03 14:45:28.000000 pyadic-0.1.2/pyadic/primes.py
+drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2023-04-09 16:18:32.394642 pyadic-0.1.2/pyadic.egg-info/
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)     3745 2023-04-09 16:18:32.000000 pyadic-0.1.2/pyadic.egg-info/PKG-INFO
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)      489 2023-04-09 16:18:32.000000 pyadic-0.1.2/pyadic.egg-info/SOURCES.txt
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)        1 2023-04-09 16:18:32.000000 pyadic-0.1.2/pyadic.egg-info/dependency_links.txt
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)       12 2023-04-09 16:18:32.000000 pyadic-0.1.2/pyadic.egg-info/requires.txt
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)        7 2023-04-09 16:18:32.000000 pyadic-0.1.2/pyadic.egg-info/top_level.txt
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)       14 2022-10-21 11:06:30.000000 pyadic-0.1.2/runtime.txt
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)      201 2023-04-09 16:18:32.394642 pyadic-0.1.2/setup.cfg
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)      684 2023-04-09 16:14:06.000000 pyadic-0.1.2/setup.py
+drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2023-04-09 16:18:32.394642 pyadic-0.1.2/tests/
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)       11 2022-07-25 22:51:57.000000 pyadic-0.1.2/tests/.hidden
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)     1716 2022-07-29 22:37:00.000000 pyadic-0.1.2/tests/test_field_extension.py
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)     5176 2023-04-03 14:47:29.000000 pyadic-0.1.2/tests/test_finite_field.py
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)     4320 2023-01-11 15:39:03.000000 pyadic-0.1.2/tests/test_padic.py
+-rw-rw-r--   0 gdl       (1000) gdl       (1000)     1253 2022-07-25 22:36:25.000000 pyadic-0.1.2/update-badges.py
```

### Comparing `pyadic-0.1.1/.github/workflows/continuous_integration.yml` & `pyadic-0.1.2/.github/workflows/continuous_integration.yml`

 * *Files identical despite different names*

### Comparing `pyadic-0.1.1/LICENSE.txt` & `pyadic-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyadic-0.1.1/pyadic/field_extension.py` & `pyadic-0.1.2/pyadic/field_extension.py`

 * *Files identical despite different names*

### Comparing `pyadic-0.1.1/pyadic/finite_field.py` & `pyadic-0.1.2/pyadic/finite_field.py`

 * *Files identical despite different names*

### Comparing `pyadic-0.1.1/pyadic/padic.py` & `pyadic-0.1.2/pyadic/padic.py`

 * *Files identical despite different names*

### Comparing `pyadic-0.1.1/pyadic/primes.py` & `pyadic-0.1.2/pyadic/primes.py`

 * *Files identical despite different names*

### Comparing `pyadic-0.1.1/tests/test_field_extension.py` & `pyadic-0.1.2/tests/test_field_extension.py`

 * *Files identical despite different names*

### Comparing `pyadic-0.1.1/tests/test_finite_field.py` & `pyadic-0.1.2/tests/test_finite_field.py`

 * *Files identical despite different names*

### Comparing `pyadic-0.1.1/tests/test_padic.py` & `pyadic-0.1.2/tests/test_padic.py`

 * *Files identical despite different names*

### Comparing `pyadic-0.1.1/update-badges.py` & `pyadic-0.1.2/update-badges.py`

 * *Files identical despite different names*

