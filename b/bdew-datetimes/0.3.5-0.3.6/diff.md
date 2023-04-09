# Comparing `tmp/bdew_datetimes-0.3.5.tar.gz` & `tmp/bdew_datetimes-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdew_datetimes-0.3.5.tar", last modified: Sun Mar 12 22:46:39 2023, max compression
+gzip compressed data, was "bdew_datetimes-0.3.6.tar", last modified: Sun Apr  9 13:46:47 2023, max compression
```

## Comparing `bdew_datetimes-0.3.5.tar` & `bdew_datetimes-0.3.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 22:46:39.547523 bdew_datetimes-0.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 22:46:39.547523 bdew_datetimes-0.3.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 22:46:39.547523 bdew_datetimes-0.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/.github/workflows/linters.yml
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/.github/workflows/packaging_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-03-12 22:46:39.547523 bdew_datetimes-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-03-12 22:46:39.551523 bdew_datetimes-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 22:46:39.547523 bdew_datetimes-0.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 22:46:39.547523 bdew_datetimes-0.3.5/src/bdew_datetimes/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/src/bdew_datetimes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/src/bdew_datetimes/calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/src/bdew_datetimes/german_strom_and_gas_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/src/bdew_datetimes/periods.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/src/bdew_datetimes/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 22:46:39.547523 bdew_datetimes-0.3.5/src/bdew_datetimes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-03-12 22:46:39.000000 bdew_datetimes-0.3.5/src/bdew_datetimes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-12 22:46:39.000000 bdew_datetimes-0.3.5/src/bdew_datetimes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 22:46:39.000000 bdew_datetimes-0.3.5/src/bdew_datetimes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-12 22:46:39.000000 bdew_datetimes-0.3.5/src/bdew_datetimes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-12 22:46:39.000000 bdew_datetimes-0.3.5/src/bdew_datetimes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 22:46:39.547523 bdew_datetimes-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/tests/test_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/tests/test_german_strom_and_gas_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/tests/test_period.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-12 22:46:32.000000 bdew_datetimes-0.3.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:46:47.492800 bdew_datetimes-0.3.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:46:47.488800 bdew_datetimes-0.3.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:46:47.488800 bdew_datetimes-0.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/.github/workflows/linters.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/.github/workflows/packaging_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/.github/workflows/unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-09 13:46:47.492800 bdew_datetimes-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-09 13:46:47.492800 bdew_datetimes-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:46:47.488800 bdew_datetimes-0.3.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:46:47.488800 bdew_datetimes-0.3.6/src/bdew_datetimes/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/src/bdew_datetimes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/src/bdew_datetimes/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/src/bdew_datetimes/german_strom_and_gas_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/src/bdew_datetimes/periods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/src/bdew_datetimes/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:46:47.492800 bdew_datetimes-0.3.6/src/bdew_datetimes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-04-09 13:46:47.000000 bdew_datetimes-0.3.6/src/bdew_datetimes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-09 13:46:47.000000 bdew_datetimes-0.3.6/src/bdew_datetimes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 13:46:47.000000 bdew_datetimes-0.3.6/src/bdew_datetimes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-09 13:46:47.000000 bdew_datetimes-0.3.6/src/bdew_datetimes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-09 13:46:47.000000 bdew_datetimes-0.3.6/src/bdew_datetimes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:46:47.492800 bdew_datetimes-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/tests/test_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/tests/test_german_strom_and_gas_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/tests/test_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-09 13:46:40.000000 bdew_datetimes-0.3.6/tox.ini
```

### Comparing `bdew_datetimes-0.3.5/.github/dependabot.yml` & `bdew_datetimes-0.3.6/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.5/.github/workflows/linters.yml` & `bdew_datetimes-0.3.6/.github/workflows/linters.yml`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.5/.github/workflows/packaging_test.yml` & `bdew_datetimes-0.3.6/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.5/.github/workflows/release.yml` & `bdew_datetimes-0.3.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.5/.github/workflows/unittests.yml` & `bdew_datetimes-0.3.6/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.5/.gitignore` & `bdew_datetimes-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.5/LICENSE` & `bdew_datetimes-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.5/PKG-INFO` & `bdew_datetimes-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdew_datetimes
-Version: 0.3.5
+Version: 0.3.6
 Summary: Generate and work with holidays of the BDEW-Calendar for power and gas in Germany.
 Home-page: UNKNOWN
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bdew_datetimes-0.3.5/README.md` & `bdew_datetimes-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.5/requirements.txt` & `bdew_datetimes-0.3.6/requirements.txt`

 * *Files 26% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 #
 #    pip-compile requirements.in
 #
 convertdate==2.4.0
     # via holidays
 hijri-converter==2.2.4
     # via holidays
-holidays==0.21
+holidays==0.22
     # via -r requirements.in
 korean-lunar-calendar==0.3.1
     # via holidays
 pymeeus==0.5.12
     # via
     #   convertdate
     #   holidays
 python-dateutil==2.8.2
     # via
     #   -r requirements.in
     #   holidays
-pytz==2022.7.1
+pytz==2023.3
     # via -r requirements.in
 six==1.16.0
     # via python-dateutil
+tzdata==2023.3
+    # via holidays
```

### Comparing `bdew_datetimes-0.3.5/setup.cfg` & `bdew_datetimes-0.3.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.5/src/bdew_datetimes/calendar.py` & `bdew_datetimes-0.3.6/src/bdew_datetimes/calendar.py`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.5/src/bdew_datetimes/german_strom_and_gas_tag.py` & `bdew_datetimes-0.3.6/src/bdew_datetimes/german_strom_and_gas_tag.py`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.5/src/bdew_datetimes/periods.py` & `bdew_datetimes-0.3.6/src/bdew_datetimes/periods.py`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.5/src/bdew_datetimes.egg-info/PKG-INFO` & `bdew_datetimes-0.3.6/src/bdew_datetimes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdew-datetimes
-Version: 0.3.5
+Version: 0.3.6
 Summary: Generate and work with holidays of the BDEW-Calendar for power and gas in Germany.
 Home-page: UNKNOWN
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bdew_datetimes-0.3.5/src/bdew_datetimes.egg-info/SOURCES.txt` & `bdew_datetimes-0.3.6/src/bdew_datetimes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.5/tests/test_calendar.py` & `bdew_datetimes-0.3.6/tests/test_calendar.py`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.5/tests/test_german_strom_and_gas_tag.py` & `bdew_datetimes-0.3.6/tests/test_german_strom_and_gas_tag.py`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.5/tests/test_period.py` & `bdew_datetimes-0.3.6/tests/test_period.py`

 * *Files identical despite different names*

### Comparing `bdew_datetimes-0.3.5/tox.ini` & `bdew_datetimes-0.3.6/tox.ini`

 * *Files identical despite different names*

