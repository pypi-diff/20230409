# Comparing `tmp/pytest_html-4.0.0rc2.tar.gz` & `tmp/pytest_html-4.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Apr  8 22:35:18 2023, max compression
+gzip compressed data, last modified: Sat Apr  8 23:08:47 2023, max compression
```

## Comparing `pytest_html-4.0.0rc2.tar` & `pytest_html-4.0.0rc4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0      146 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/.coveragerc
--rw-r--r--   0        0        0     1953 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/.eslintrc.json
--rw-r--r--   0        0        0       82 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/.nycrc
--rw-r--r--   0        0        0     1694 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       63 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/.prettierrc
--rw-r--r--   0        0        0      101 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/codecov.yml
--rw-r--r--   0        0        0      215 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docker-compose.tmpl.yml
--rw-r--r--   0        0        0   340564 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/package-lock.json
--rw-r--r--   0        0        0      661 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/package.json
--rwxr-xr-x   0        0        0      391 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/start
--rw-r--r--   0        0        0     1970 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/tox.ini
--rw-r--r--   0        0        0      634 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docs/Makefile
--rw-r--r--   0        0        0      171 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docs/api_reference.rst
--rw-r--r--   0        0        0    13972 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docs/changelog.rst
--rw-r--r--   0        0        0     2208 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docs/conf.py
--rw-r--r--   0        0        0     3460 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docs/deprecations.rst
--rw-r--r--   0        0        0     3991 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docs/development.rst
--rw-r--r--   0        0        0      506 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docs/index.rst
--rw-r--r--   0        0        0      340 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docs/installing.rst
--rw-r--r--   0        0        0      795 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docs/make.bat
--rw-r--r--   0        0        0    10798 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/docs/user_guide.rst
--rw-r--r--   0        0        0      111 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/.gitattributes
--rw-r--r--   0        0        0      125 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/.gitignore
--rw-r--r--   0        0        0     5212 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/layout/css/style.scss
--rw-r--r--   0        0        0      224 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/__init__.py
--rw-r--r--   0        0        0      163 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/__version.py
--rw-r--r--   0        0        0    12854 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/basereport.py
--rw-r--r--   0        0        0     1595 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/extras.py
--rw-r--r--   0        0        0      739 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/hooks.py
--rw-r--r--   0        0        0     4440 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/plugin.py
--rw-r--r--   0        0        0     1372 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/report.py
--rw-r--r--   0        0        0     1178 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/selfcontained_report.py
--rw-r--r--   0        0        0     2429 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/table.py
--rw-r--r--   0        0        0      673 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/util.py
--rw-r--r--   0        0        0    23906 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/resources/app.js
--rw-r--r--   0        0        0     4931 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/resources/index.jinja2
--rw-r--r--   0        0        0     4313 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/resources/style.css
--rw-r--r--   0        0        0     1572 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/scripts/datamanager.js
--rw-r--r--   0        0        0     6131 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/scripts/dom.js
--rw-r--r--   0        0        0      855 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/scripts/filter.js
--rw-r--r--   0        0        0      400 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/scripts/index.js
--rw-r--r--   0        0        0     5059 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/scripts/main.js
--rw-r--r--   0        0        0     2269 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/scripts/mediaviewer.js
--rw-r--r--   0        0        0     1731 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/scripts/sort.js
--rw-r--r--   0        0        0     3696 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/scripts/storage.js
--rw-r--r--   0        0        0     1025 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/src/pytest_html/scripts/utils.js
--rw-r--r--   0        0        0    43300 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/testing/legacy_test_pytest_html.py
--rw-r--r--   0        0        0    30747 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/testing/test_integration.py
--rw-r--r--   0        0        0      728 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/testing/test_unit.py
--rw-r--r--   0        0        0    10475 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/testing/unittest.js
--rw-r--r--   0        0        0      579 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/.gitignore
--rw-r--r--   0        0        0      193 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/LICENSE
--rw-r--r--   0        0        0     1804 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/README.rst
--rw-r--r--   0        0        0     2179 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0     3859 2023-04-08 22:35:18.000000 pytest_html-4.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      146 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/.coveragerc
+-rw-r--r--   0        0        0     1953 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/.eslintrc.json
+-rw-r--r--   0        0        0       82 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/.nycrc
+-rw-r--r--   0        0        0     1694 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       63 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/.prettierrc
+-rw-r--r--   0        0        0      101 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/codecov.yml
+-rw-r--r--   0        0        0      215 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docker-compose.tmpl.yml
+-rw-r--r--   0        0        0   340564 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/package-lock.json
+-rw-r--r--   0        0        0      661 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/package.json
+-rwxr-xr-x   0        0        0      391 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/start
+-rw-r--r--   0        0        0     1970 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/tox.ini
+-rw-r--r--   0        0        0      634 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docs/Makefile
+-rw-r--r--   0        0        0      171 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docs/api_reference.rst
+-rw-r--r--   0        0        0    13972 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docs/changelog.rst
+-rw-r--r--   0        0        0     2208 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docs/conf.py
+-rw-r--r--   0        0        0     3460 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docs/deprecations.rst
+-rw-r--r--   0        0        0     3991 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docs/development.rst
+-rw-r--r--   0        0        0      506 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docs/index.rst
+-rw-r--r--   0        0        0      340 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docs/installing.rst
+-rw-r--r--   0        0        0      795 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docs/make.bat
+-rw-r--r--   0        0        0    10798 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/docs/user_guide.rst
+-rw-r--r--   0        0        0      111 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/.gitattributes
+-rw-r--r--   0        0        0      125 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/.gitignore
+-rw-r--r--   0        0        0     5212 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/layout/css/style.scss
+-rw-r--r--   0        0        0      224 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/__init__.py
+-rw-r--r--   0        0        0      163 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/__version.py
+-rw-r--r--   0        0        0    12862 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/basereport.py
+-rw-r--r--   0        0        0     1595 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/extras.py
+-rw-r--r--   0        0        0      739 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/hooks.py
+-rw-r--r--   0        0        0     4514 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/plugin.py
+-rw-r--r--   0        0        0     1372 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/report.py
+-rw-r--r--   0        0        0     1178 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/selfcontained_report.py
+-rw-r--r--   0        0        0     2429 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/table.py
+-rw-r--r--   0        0        0      673 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/util.py
+-rw-r--r--   0        0        0    23906 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/resources/app.js
+-rw-r--r--   0        0        0     4931 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/resources/index.jinja2
+-rw-r--r--   0        0        0     4313 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/resources/style.css
+-rw-r--r--   0        0        0     1572 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/scripts/datamanager.js
+-rw-r--r--   0        0        0     6131 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/scripts/dom.js
+-rw-r--r--   0        0        0      855 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/scripts/filter.js
+-rw-r--r--   0        0        0      400 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/scripts/index.js
+-rw-r--r--   0        0        0     5059 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/scripts/main.js
+-rw-r--r--   0        0        0     2269 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/scripts/mediaviewer.js
+-rw-r--r--   0        0        0     1731 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/scripts/sort.js
+-rw-r--r--   0        0        0     3696 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/scripts/storage.js
+-rw-r--r--   0        0        0     1025 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/src/pytest_html/scripts/utils.js
+-rw-r--r--   0        0        0    43300 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/testing/legacy_test_pytest_html.py
+-rw-r--r--   0        0        0    30747 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/testing/test_integration.py
+-rw-r--r--   0        0        0      728 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/testing/test_unit.py
+-rw-r--r--   0        0        0    10475 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/testing/unittest.js
+-rw-r--r--   0        0        0      579 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/.gitignore
+-rw-r--r--   0        0        0      193 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/LICENSE
+-rw-r--r--   0        0        0     1804 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/README.rst
+-rw-r--r--   0        0        0     2179 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     3859 2023-04-08 23:08:47.000000 pytest_html-4.0.0rc4/PKG-INFO
```

### Comparing `pytest_html-4.0.0rc2/.eslintrc.json` & `pytest_html-4.0.0rc4/.eslintrc.json`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/.pre-commit-config.yaml` & `pytest_html-4.0.0rc4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/package-lock.json` & `pytest_html-4.0.0rc4/package-lock.json`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/package.json` & `pytest_html-4.0.0rc4/package.json`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/tox.ini` & `pytest_html-4.0.0rc4/tox.ini`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/docs/Makefile` & `pytest_html-4.0.0rc4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/docs/changelog.rst` & `pytest_html-4.0.0rc4/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/docs/conf.py` & `pytest_html-4.0.0rc4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/docs/deprecations.rst` & `pytest_html-4.0.0rc4/docs/deprecations.rst`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/docs/development.rst` & `pytest_html-4.0.0rc4/docs/development.rst`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/docs/make.bat` & `pytest_html-4.0.0rc4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/docs/user_guide.rst` & `pytest_html-4.0.0rc4/docs/user_guide.rst`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/src/layout/css/style.scss` & `pytest_html-4.0.0rc4/src/layout/css/style.scss`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/src/pytest_html/basereport.py` & `pytest_html-4.0.0rc4/src/pytest_html/basereport.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     from _pytest.logging import _remove_ansi_escape_sequences
 
     _handle_ansi = _remove_ansi_escape_sequences
     _ansi_styles = []
 
 
 class BaseReport:
-    class Report:
+    class ReportData:
         def __init__(self, title, config):
             self._config = config
             self._data = {
                 "title": title,
                 "collectedItems": 0,
                 "runningState": "not_started",
                 "environment": {},
@@ -118,15 +118,15 @@
         self._css = _process_css(
             Path(self._resources_path, default_css), self._config.getoption("css")
         )
         self._max_asset_filename_length = int(
             config.getini("max_asset_filename_length")
         )
 
-        self._report = self.Report(self._report_path.name, config)
+        self._report = self.ReportData(self._report_path.name, config)
 
     @property
     def css(self):
         # implement in subclasses
         return
 
     def _asset_filename(self, test_id, extra_index, test_index, file_extension):
```

### Comparing `pytest_html-4.0.0rc2/src/pytest_html/extras.py` & `pytest_html-4.0.0rc4/src/pytest_html/extras.py`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/src/pytest_html/hooks.py` & `pytest_html-4.0.0rc4/src/pytest_html/hooks.py`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/src/pytest_html/plugin.py` & `pytest_html-4.0.0rc4/src/pytest_html/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 import warnings
 from pathlib import Path
 
 import pytest
 
+from pytest_html.basereport import BaseReport as HTMLReport  # noqa: F401
 from pytest_html.report import Report
 from pytest_html.selfcontained_report import SelfContainedReport
 
 
 def pytest_addhooks(pluginmanager):
     from . import hooks
```

### Comparing `pytest_html-4.0.0rc2/src/pytest_html/report.py` & `pytest_html-4.0.0rc4/src/pytest_html/report.py`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/src/pytest_html/selfcontained_report.py` & `pytest_html-4.0.0rc4/src/pytest_html/selfcontained_report.py`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/src/pytest_html/table.py` & `pytest_html-4.0.0rc4/src/pytest_html/table.py`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/src/pytest_html/util.py` & `pytest_html-4.0.0rc4/src/pytest_html/util.py`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/src/pytest_html/resources/app.js` & `pytest_html-4.0.0rc4/src/pytest_html/resources/app.js`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/src/pytest_html/resources/index.jinja2` & `pytest_html-4.0.0rc4/src/pytest_html/resources/index.jinja2`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/src/pytest_html/resources/style.css` & `pytest_html-4.0.0rc4/src/pytest_html/resources/style.css`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/src/pytest_html/scripts/datamanager.js` & `pytest_html-4.0.0rc4/src/pytest_html/scripts/datamanager.js`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/src/pytest_html/scripts/dom.js` & `pytest_html-4.0.0rc4/src/pytest_html/scripts/dom.js`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/src/pytest_html/scripts/filter.js` & `pytest_html-4.0.0rc4/src/pytest_html/scripts/filter.js`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/src/pytest_html/scripts/main.js` & `pytest_html-4.0.0rc4/src/pytest_html/scripts/main.js`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/src/pytest_html/scripts/mediaviewer.js` & `pytest_html-4.0.0rc4/src/pytest_html/scripts/mediaviewer.js`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/src/pytest_html/scripts/sort.js` & `pytest_html-4.0.0rc4/src/pytest_html/scripts/sort.js`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/src/pytest_html/scripts/storage.js` & `pytest_html-4.0.0rc4/src/pytest_html/scripts/storage.js`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/src/pytest_html/scripts/utils.js` & `pytest_html-4.0.0rc4/src/pytest_html/scripts/utils.js`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/testing/legacy_test_pytest_html.py` & `pytest_html-4.0.0rc4/testing/legacy_test_pytest_html.py`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/testing/test_integration.py` & `pytest_html-4.0.0rc4/testing/test_integration.py`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/testing/test_unit.py` & `pytest_html-4.0.0rc4/testing/test_unit.py`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/testing/unittest.js` & `pytest_html-4.0.0rc4/testing/unittest.js`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/.gitignore` & `pytest_html-4.0.0rc4/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/README.rst` & `pytest_html-4.0.0rc4/README.rst`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/pyproject.toml` & `pytest_html-4.0.0rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_html-4.0.0rc2/PKG-INFO` & `pytest_html-4.0.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-html
-Version: 4.0.0rc2
+Version: 4.0.0rc4
 Summary: pytest plugin for generating HTML reports
 Project-URL: Homepage, https://github.com/pytest-dev/pytest-html
 Project-URL: Tracker, https://github.com/pytest-dev/pytest-html/issues
 Project-URL: Source, https://github.com/pytest-dev/pytest-html
 Author-email: Dave Hunt <dhunt@mozilla.com>, Jim Brannlund <jimbrannlund@fastmail.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
```

