# Comparing `tmp/smartapp_sdk-0.5.4.tar.gz` & `tmp/smartapp_sdk-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartapp_sdk-0.5.4.tar", max compression
+gzip compressed data, was "smartapp_sdk-0.6.0.tar", max compression
```

## Comparing `smartapp_sdk-0.5.4.tar` & `smartapp_sdk-0.6.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1609 2023-02-26 08:40:15.902906 smartapp_sdk-0.5.4/Changelog
--rw-r--r--   0        0        0    11324 2023-02-26 08:40:15.902906 smartapp_sdk-0.5.4/LICENSE
--rw-r--r--   0        0        0      761 2023-02-26 08:40:15.902906 smartapp_sdk-0.5.4/NOTICE
--rw-r--r--   0        0        0     2167 2023-02-26 08:40:15.902906 smartapp_sdk-0.5.4/PyPI.md
--rw-r--r--   0        0        0     2366 2023-02-26 08:40:15.902906 smartapp_sdk-0.5.4/README.md
--rw-r--r--   0        0        0       22 2023-02-26 08:40:15.902906 smartapp_sdk-0.5.4/docs/.gitignore
--rw-r--r--   0        0        0      142 2023-02-26 08:40:15.902906 smartapp_sdk-0.5.4/docs/.sphinxignore
--rw-r--r--   0        0        0     6814 2023-02-26 08:40:15.902906 smartapp_sdk-0.5.4/docs/Makefile
--rw-r--r--   0        0        0      120 2023-02-26 08:40:15.902906 smartapp_sdk-0.5.4/docs/README.md
--rw-r--r--   0        0        0      130 2023-02-26 08:40:15.902906 smartapp_sdk-0.5.4/docs/_static/custom.css
--rw-r--r--   0        0        0     1861 2023-02-26 08:40:15.902906 smartapp_sdk-0.5.4/docs/_themes/LICENSE
--rw-r--r--   0        0        0     3905 2023-02-26 08:40:15.902906 smartapp_sdk-0.5.4/docs/_themes/flask_theme_support.py
--rw-r--r--   0        0        0    13018 2023-02-26 08:40:15.902906 smartapp_sdk-0.5.4/docs/conf.py
--rw-r--r--   0        0        0     9479 2023-02-26 08:40:15.902906 smartapp_sdk-0.5.4/docs/index.rst
--rw-r--r--   0        0        0     6709 2023-02-26 08:40:15.902906 smartapp_sdk-0.5.4/docs/make.bat
--rw-r--r--   0        0        0     2756 2023-02-26 08:40:44.934832 smartapp_sdk-0.5.4/pyproject.toml
--rw-r--r--   0        0        0       29 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/src/smartapp/__init__.py
--rw-r--r--   0        0        0     6888 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/src/smartapp/converter.py
--rw-r--r--   0        0        0     7781 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/src/smartapp/dispatcher.py
--rw-r--r--   0        0        0    34669 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/src/smartapp/interface.py
--rw-r--r--   0        0        0       60 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/src/smartapp/py.typed
--rw-r--r--   0        0        0     9893 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/src/smartapp/signature.py
--rw-r--r--   0        0        0       29 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/__init__.py
--rw-r--r--   0        0        0      213 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/live/README.md
--rw-r--r--   0        0        0     2885 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/live/request/INSTALL.1.json
--rw-r--r--   0        0        0     1011 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/README.md
--rw-r--r--   0        0        0      813 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/request/CONFIGURATION-INITIALIZE.json
--rw-r--r--   0        0        0      457 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/request/CONFIGURATION-PAGE.json
--rw-r--r--   0        0        0      381 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/request/CONFIRMATION.json
--rw-r--r--   0        0        0     1793 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/request/EVENT-DEVICE.json
--rw-r--r--   0        0        0     1567 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/request/EVENT-TIMER.json
--rw-r--r--   0        0        0     1327 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/request/INSTALL.json
--rw-r--r--   0        0        0      218 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/request/OAUTH_CALLBACK.json
--rw-r--r--   0        0        0     1255 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/request/UNINSTALL.json
--rw-r--r--   0        0        0     2152 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/request/UPDATE.json
--rw-r--r--   0        0        0      249 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/response/CONFIGURATION-INITIALIZE.json
--rw-r--r--   0        0        0      742 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/response/CONFIGURATION-PAGE-1of2.json
--rw-r--r--   0        0        0     1251 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/response/CONFIGURATION-PAGE-only.json
--rw-r--r--   0        0        0       33 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/response/CONFIRMATION.json
--rw-r--r--   0        0        0       21 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/response/EVENT.json
--rw-r--r--   0        0        0       23 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/response/INSTALL.json
--rw-r--r--   0        0        0       29 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/response/OAUTH_CALLBACK.json
--rw-r--r--   0        0        0       25 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/response/UNINSTALL.json
--rw-r--r--   0        0        0       22 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/response/UPDATE.json
--rw-r--r--   0        0        0      156 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/settings/BOOLEAN.json
--rw-r--r--   0        0        0      117 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/settings/DECIMAL.json
--rw-r--r--   0        0        0      231 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/settings/DEVICE.json
--rw-r--r--   0        0        0      114 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/settings/EMAIL.json
--rw-r--r--   0        0        0      700 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/settings/ENUM-GROUP.json
--rw-r--r--   0        0        0      292 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/settings/ENUM.json
--rw-r--r--   0        0        0      152 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/settings/ICON.json
--rw-r--r--   0        0        0      146 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/settings/IMAGE.json
--rw-r--r--   0        0        0      187 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/settings/LINK.json
--rw-r--r--   0        0        0      108 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/settings/NUMBER.json
--rw-r--r--   0        0        0      291 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/settings/OAUTH.json
--rw-r--r--   0        0        0      167 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/settings/PAGE.json
--rw-r--r--   0        0        0      185 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/settings/PARAGRAPH.json
--rw-r--r--   0        0        0      112 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/settings/PHONE.json
--rw-r--r--   0        0        0      165 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/settings/TEXT.json
--rw-r--r--   0        0        0      101 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/fixtures/samples/settings/TIME.json
--rw-r--r--   0        0        0    38670 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/test_converter.py
--rw-r--r--   0        0        0    14130 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/test_dispatcher.py
--rw-r--r--   0        0        0     7893 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/test_interface.py
--rw-r--r--   0        0        0    24779 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/test_signature.py
--rw-r--r--   0        0        0      549 2023-02-26 08:40:15.906906 smartapp_sdk-0.5.4/tests/testutil.py
--rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 smartapp_sdk-0.5.4/setup.py
--rw-r--r--   0        0        0     3660 1970-01-01 00:00:00.000000 smartapp_sdk-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1747 2023-04-09 19:22:50.420316 smartapp_sdk-0.6.0/Changelog
+-rw-r--r--   0        0        0    11324 2023-04-09 19:22:50.420316 smartapp_sdk-0.6.0/LICENSE
+-rw-r--r--   0        0        0      761 2023-04-09 19:22:50.420316 smartapp_sdk-0.6.0/NOTICE
+-rw-r--r--   0        0        0     2167 2023-04-09 19:22:50.420316 smartapp_sdk-0.6.0/PyPI.md
+-rw-r--r--   0        0        0     2366 2023-04-09 19:22:50.420316 smartapp_sdk-0.6.0/README.md
+-rw-r--r--   0        0        0       22 2023-04-09 19:22:50.420316 smartapp_sdk-0.6.0/docs/.gitignore
+-rw-r--r--   0        0        0      142 2023-04-09 19:22:50.420316 smartapp_sdk-0.6.0/docs/.sphinxignore
+-rw-r--r--   0        0        0     6814 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/docs/Makefile
+-rw-r--r--   0        0        0      120 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/docs/README.md
+-rw-r--r--   0        0        0      130 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/docs/_static/custom.css
+-rw-r--r--   0        0        0     1861 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/docs/_themes/LICENSE
+-rw-r--r--   0        0        0     3905 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/docs/_themes/flask_theme_support.py
+-rw-r--r--   0        0        0    13018 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/docs/conf.py
+-rw-r--r--   0        0        0     9479 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/docs/index.rst
+-rw-r--r--   0        0        0     6709 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/docs/make.bat
+-rw-r--r--   0        0        0     2783 2023-04-09 19:23:11.772697 smartapp_sdk-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/src/smartapp/__init__.py
+-rw-r--r--   0        0        0     6888 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/src/smartapp/converter.py
+-rw-r--r--   0        0        0     7781 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/src/smartapp/dispatcher.py
+-rw-r--r--   0        0        0    35006 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/src/smartapp/interface.py
+-rw-r--r--   0        0        0       60 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/src/smartapp/py.typed
+-rw-r--r--   0        0        0     9893 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/src/smartapp/signature.py
+-rw-r--r--   0        0        0       29 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      213 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/live/README.md
+-rw-r--r--   0        0        0     2885 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/live/request/INSTALL.1.json
+-rw-r--r--   0        0        0     1011 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/README.md
+-rw-r--r--   0        0        0      813 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/request/CONFIGURATION-INITIALIZE.json
+-rw-r--r--   0        0        0      457 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/request/CONFIGURATION-PAGE.json
+-rw-r--r--   0        0        0      381 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/request/CONFIRMATION.json
+-rw-r--r--   0        0        0     1793 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/request/EVENT-DEVICE.json
+-rw-r--r--   0        0        0     1567 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/request/EVENT-TIMER.json
+-rw-r--r--   0        0        0     1327 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/request/INSTALL.json
+-rw-r--r--   0        0        0      218 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/request/OAUTH_CALLBACK.json
+-rw-r--r--   0        0        0     1255 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/request/UNINSTALL.json
+-rw-r--r--   0        0        0     2152 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/request/UPDATE.json
+-rw-r--r--   0        0        0      249 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/response/CONFIGURATION-INITIALIZE.json
+-rw-r--r--   0        0        0      742 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/response/CONFIGURATION-PAGE-1of2.json
+-rw-r--r--   0        0        0     1251 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/response/CONFIGURATION-PAGE-only.json
+-rw-r--r--   0        0        0       33 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/response/CONFIRMATION.json
+-rw-r--r--   0        0        0       21 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/response/EVENT.json
+-rw-r--r--   0        0        0       23 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/response/INSTALL.json
+-rw-r--r--   0        0        0       29 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/response/OAUTH_CALLBACK.json
+-rw-r--r--   0        0        0       25 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/response/UNINSTALL.json
+-rw-r--r--   0        0        0       22 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/response/UPDATE.json
+-rw-r--r--   0        0        0      156 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/BOOLEAN.json
+-rw-r--r--   0        0        0      117 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/DECIMAL.json
+-rw-r--r--   0        0        0      231 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/DEVICE.json
+-rw-r--r--   0        0        0      114 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/EMAIL.json
+-rw-r--r--   0        0        0      700 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/ENUM-GROUP.json
+-rw-r--r--   0        0        0      292 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/ENUM.json
+-rw-r--r--   0        0        0      152 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/ICON.json
+-rw-r--r--   0        0        0      146 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/IMAGE.json
+-rw-r--r--   0        0        0      187 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/LINK.json
+-rw-r--r--   0        0        0      108 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/NUMBER.json
+-rw-r--r--   0        0        0      291 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/OAUTH.json
+-rw-r--r--   0        0        0      167 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/PAGE.json
+-rw-r--r--   0        0        0      185 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/PARAGRAPH.json
+-rw-r--r--   0        0        0      112 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/PHONE.json
+-rw-r--r--   0        0        0      165 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/TEXT.json
+-rw-r--r--   0        0        0      101 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/fixtures/samples/settings/TIME.json
+-rw-r--r--   0        0        0    38670 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/test_converter.py
+-rw-r--r--   0        0        0    14130 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/test_dispatcher.py
+-rw-r--r--   0        0        0     7893 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/test_interface.py
+-rw-r--r--   0        0        0    25529 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/test_signature.py
+-rw-r--r--   0        0        0      549 2023-04-09 19:22:50.424316 smartapp_sdk-0.6.0/tests/testutil.py
+-rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 smartapp_sdk-0.6.0/setup.py
+-rw-r--r--   0        0        0     3660 1970-01-01 00:00:00.000000 smartapp_sdk-0.6.0/PKG-INFO
```

### Comparing `smartapp_sdk-0.5.4/Changelog` & `smartapp_sdk-0.6.0/Changelog`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Version 0.6.0     09 Apr 2023
+
+	* Add new SubscriptionType enumeration.
+	* Rewrite request-related tests to use the responses framework.
+
 Version 0.5.4     26 Feb 2023
 
 	* Upgrade all dependencies to the latest major version.
 	* Pull Sphinx fields from metadata rather than parsing pyproject.toml.
 
 Version 0.5.3     30 Dec 2022
```

### Comparing `smartapp_sdk-0.5.4/LICENSE` & `smartapp_sdk-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/NOTICE` & `smartapp_sdk-0.6.0/NOTICE`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/PyPI.md` & `smartapp_sdk-0.6.0/PyPI.md`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/README.md` & `smartapp_sdk-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/docs/Makefile` & `smartapp_sdk-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/docs/_themes/LICENSE` & `smartapp_sdk-0.6.0/docs/_themes/LICENSE`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/docs/_themes/flask_theme_support.py` & `smartapp_sdk-0.6.0/docs/_themes/flask_theme_support.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/docs/conf.py` & `smartapp_sdk-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/docs/index.rst` & `smartapp_sdk-0.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/docs/make.bat` & `smartapp_sdk-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/pyproject.toml` & `smartapp_sdk-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smartapp-sdk"
-version = "0.5.4" # published version is managed using Git tags (see below)
+version = "0.6.0" # published version is managed using Git tags (see below)
 description = "Framework to build a webhook-based SmartThings SmartApp"
 authors = ["Kenneth J. Pronovici <pronovic@ieee.org>"]
 license = "Apache-2.0"
 readme = "PyPI.md"
 homepage = "https://pypi.org/project/smartapp-sdk/"
 repository = "https://github.com/pronovic/smartapp-sdk"
 include = [
@@ -63,14 +63,15 @@
 black = "^23.1.0"
 mypy = "^1.0.1"
 isort = "^5.12.0"
 coveralls = "^3.3.1"
 types-PyYAML = "^6.0.12.8"
 types-requests = "^2.28.11.15"
 colorama = "~0, >=0.4.6"
+responses = "~0, >=0.22.0"
 
 [tool.black]
 line-length = 132
 target-version = ['py39', 'py310', 'py311' ]
 include = '(src\/scripts\/.*$|\.pyi?$)'
 exclude = '''
 /(
```

### Comparing `smartapp_sdk-0.5.4/src/smartapp/converter.py` & `smartapp_sdk-0.6.0/src/smartapp/converter.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/src/smartapp/dispatcher.py` & `smartapp_sdk-0.6.0/src/smartapp/dispatcher.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/src/smartapp/interface.py` & `smartapp_sdk-0.6.0/src/smartapp/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,27 @@
     MODE_EVENT = "MODE_EVENT"
     SCENE_LIFECYCLE_EVENT = "SCENE_LIFECYCLE_EVENT"
     SECURITY_ARM_STATE_EVENT = "SECURITY_ARM_STATE_EVENT"
     TIMER_EVENT = "TIMER_EVENT"
     WEATHER_EVENT = "WEATHER_EVENT"
 
 
+class SubscriptionType(Enum):
+    """Supported subscription types."""
+
+    DEVICE = "DEVICE"
+    CAPABILITY = "CAPABILITY"
+    MODE = "MODE"
+    DEVICE_LIFECYCLE = "DEVICE_LIFECYCLE"
+    DEVICE_HEALTH = "DEVICE_HEALTH"
+    SECURITY_ARM_STATE = "SECURITY_ARM_STATE"
+    HUB_HEALTH = "HUB_HEALTH"
+    SCENE_LIFECYCLE = "SCENE_LIFECYCLE"
+
+
 class BooleanValue(str, Enum):
     """String boolean values."""
 
     TRUE = "true"
     FALSE = "false"
```

### Comparing `smartapp_sdk-0.5.4/src/smartapp/signature.py` & `smartapp_sdk-0.6.0/src/smartapp/signature.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/tests/fixtures/live/request/INSTALL.1.json` & `smartapp_sdk-0.6.0/tests/fixtures/live/request/INSTALL.1.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/tests/fixtures/samples/README.md` & `smartapp_sdk-0.6.0/tests/fixtures/samples/README.md`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/tests/fixtures/samples/request/CONFIGURATION-INITIALIZE.json` & `smartapp_sdk-0.6.0/tests/fixtures/samples/request/CONFIGURATION-INITIALIZE.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/tests/fixtures/samples/request/EVENT-DEVICE.json` & `smartapp_sdk-0.6.0/tests/fixtures/samples/request/EVENT-DEVICE.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/tests/fixtures/samples/request/EVENT-TIMER.json` & `smartapp_sdk-0.6.0/tests/fixtures/samples/request/EVENT-TIMER.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/tests/fixtures/samples/request/INSTALL.json` & `smartapp_sdk-0.6.0/tests/fixtures/samples/request/INSTALL.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/tests/fixtures/samples/request/UNINSTALL.json` & `smartapp_sdk-0.6.0/tests/fixtures/samples/request/UNINSTALL.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/tests/fixtures/samples/request/UPDATE.json` & `smartapp_sdk-0.6.0/tests/fixtures/samples/request/UPDATE.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/tests/fixtures/samples/response/CONFIGURATION-PAGE-1of2.json` & `smartapp_sdk-0.6.0/tests/fixtures/samples/response/CONFIGURATION-PAGE-1of2.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/tests/fixtures/samples/response/CONFIGURATION-PAGE-only.json` & `smartapp_sdk-0.6.0/tests/fixtures/samples/response/CONFIGURATION-PAGE-only.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/tests/fixtures/samples/settings/ENUM-GROUP.json` & `smartapp_sdk-0.6.0/tests/fixtures/samples/settings/ENUM-GROUP.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/tests/test_converter.py` & `smartapp_sdk-0.6.0/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/tests/test_dispatcher.py` & `smartapp_sdk-0.6.0/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/tests/test_interface.py` & `smartapp_sdk-0.6.0/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/tests/test_signature.py` & `smartapp_sdk-0.6.0/tests/test_signature.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # -*- coding: utf-8 -*-
 # vim: set ft=python ts=4 sw=4 expandtab:
 # pylint: disable=redefined-outer-name,line-too-long:
 from typing import Dict, Optional
-from unittest.mock import MagicMock, call, patch
+from unittest.mock import patch
 
 import pendulum
 import pytest
+import responses
 from requests import HTTPError
+from responses import matchers
+from responses.registries import OrderedRegistry
+from tenacity import RetryError
 
 from smartapp.interface import SignatureError, SmartAppDefinition, SmartAppDispatcherConfig, SmartAppRequestContext
 from smartapp.signature import SignatureVerifier, retrieve_public_key
 
 # These tests are built on sample data found in the Joyent specification.
 # See: https://github.com/TritonDataCenter/node-http-signature/blob/master/http_signing.md#appendix-a---test-values
 #
@@ -168,14 +172,16 @@
 host: example.com
 date: Thu, 05 Jan 2014 21:31:40 GMT
 content-type: application/json
 digest: SHA-256=X48E9qOokqqrvdts8nOJRJN3OWDUoyWxBf7kbu9DBPE=
 content-length: 18
 """.strip()
 
+TIMEOUT_MATCHER = matchers.request_kwargs_matcher({"timeout": 5.0})
+
 
 def build_config(clock_skew_sec: Optional[int] = CLOCK_SKEW) -> SmartAppDispatcherConfig:
     """Build configuration to test with."""
     return SmartAppDispatcherConfig(
         check_signatures=True,
         clock_skew_sec=clock_skew_sec,
         keyserver_url=KEYSERVER_URL,
@@ -502,37 +508,53 @@
         config = build_config()
         definition = build_definition()
         with pytest.raises(SignatureError, match="Algorithm not supported: bogus") as e:
             SignatureVerifier(context=context, config=config, definition=definition)
         assert e.value.correlation_id == context.correlation_id
 
 
-@patch("smartapp.signature.requests.get")
 class TestRetrievePublicKey:
     # This checks both the retry logic and the LRU cache.
     # Note that the LRU cache does not cache exceptions, only returned values.
 
-    def test_retrieve_public_key_succeeds(self, get):
-        response = MagicMock(text="public-key")
-        response.raise_for_status = MagicMock()
-        get.return_value = response
-        key1 = retrieve_public_key("https://whatever.com", "key-succeeds")  # note: no leading slash
-        assert key1 == "public-key"
-        key2 = retrieve_public_key("https://whatever.com", "key-succeeds")  # this call is cached
-        assert key2 == "public-key"
-        get.assert_called_once_with("https://whatever.com/key-succeeds", timeout=5.0)
-        response.raise_for_status.assert_called_once()
-
-    def test_retrieve_public_key_retry(self, get):
-        response1 = MagicMock()
-        response1.raise_for_status = MagicMock()
-        response1.raise_for_status.side_effect = HTTPError("hello")
-        response2 = MagicMock(text="public-key")
-        response2.raise_for_status = MagicMock()
-        get.side_effect = [response1, response2]
-        key1 = retrieve_public_key("https://whatever.com", "/key-retry")  # note: leading slash
-        assert key1 == "public-key"
-        key2 = retrieve_public_key("https://whatever.com", "/key-retry")  # this call is cached
-        assert key2 == "public-key"
-        get.assert_has_calls([call("https://whatever.com/key-retry", timeout=5.0)] * 2)
-        response1.raise_for_status.assert_called_once()
-        response2.raise_for_status.assert_called_once()
+    def test_retrieve_public_key_succeeds(self):
+        # Note that this test does not use a leading slash for the key id
+        with responses.RequestsMock() as r:
+            r.get(
+                url="https://whatever.com/key-succeeds",
+                status=200,
+                body="public-key",
+                match=[TIMEOUT_MATCHER],
+            )
+            assert retrieve_public_key("https://whatever.com", "key-succeeds") == "public-key"
+            assert retrieve_public_key("https://whatever.com", "key-succeeds") == "public-key"
+            assert len(r.calls) == 1  # only one call is made, because the first response is cached
+
+    def test_retrieve_public_key_fails(self):
+        # Note that this test does not use a leading slash for the key id
+        with responses.RequestsMock() as r:
+            r.get(
+                url="https://whatever.com/key-fails",
+                status=500,
+                match=[TIMEOUT_MATCHER],
+            )
+            with pytest.raises(RetryError):
+                retrieve_public_key("https://whatever.com", "key-fails")
+                assert len(r.calls) == 5  # five calls are made because failures are not cached
+
+    def test_retrieve_public_key_retry(self):
+        # Note that this test does use a leading slash for the key id
+        with responses.RequestsMock(registry=OrderedRegistry) as r:
+            r.get(
+                url="https://whatever.com/key-retry",
+                status=500,
+                match=[TIMEOUT_MATCHER],
+            )
+            r.get(
+                url="https://whatever.com/key-retry",
+                status=200,
+                body="public-key",
+                match=[TIMEOUT_MATCHER],
+            )
+            assert retrieve_public_key("https://whatever.com", "/key-retry") == "public-key"
+            assert retrieve_public_key("https://whatever.com", "/key-retry") == "public-key"
+            assert len(r.calls) == 2  # two calls are made because of the initial retry; the second attempt is cached
```

### Comparing `smartapp_sdk-0.5.4/tests/testutil.py` & `smartapp_sdk-0.6.0/tests/testutil.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.5.4/setup.py` & `smartapp_sdk-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 extras_require = \
 {'docs': ['importlib-metadata>=6.0.0,<7.0.0',
           'sphinx>=6.1.3,<7.0.0',
           'sphinx-autoapi>=2.0.1,<3.0.0']}
 
 setup_kwargs = {
     'name': 'smartapp-sdk',
-    'version': '0.5.4',
+    'version': '0.6.0',
     'description': 'Framework to build a webhook-based SmartThings SmartApp',
     'long_description': "# SmartApp SDK\n\n[![pypi](https://img.shields.io/pypi/v/smartapp-sdk.svg)](https://pypi.org/project/smartapp-sdk/)\n[![license](https://img.shields.io/pypi/l/smartapp-sdk.svg)](https://github.com/pronovic/smartapp-sdk/blob/master/LICENSE)\n[![wheel](https://img.shields.io/pypi/wheel/smartapp-sdk.svg)](https://pypi.org/project/smartapp-sdk/)\n[![python](https://img.shields.io/pypi/pyversions/smartapp-sdk.svg)](https://pypi.org/project/smartapp-sdk/)\n[![Test Suite](https://github.com/pronovic/smartapp-sdk/workflows/Test%20Suite/badge.svg)](https://github.com/pronovic/smartapp-sdk/actions?query=workflow%3A%22Test+Suite%22)\n[![docs](https://readthedocs.org/projects/smartapp-sdk/badge/?version=stable&style=flat)](https://smartapp-sdk.readthedocs.io/en/stable/)\n[![coverage](https://coveralls.io/repos/github/pronovic/smartapp-sdk/badge.svg?branch=master)](https://coveralls.io/github/pronovic/smartapp-sdk?branch=master)\n\nsmartapp-sdk is a Python library to build a [webhook-based SmartApp](https://developer-preview.smartthings.com/docs/connected-services/smartapp-basics/) for the [SmartThings platform](https://www.smartthings.com/).\n\nThe SDK is intended to be easy to use no matter how you choose to structure your code, whether that's a traditional Python webapp (such as FastAPI on Uvicorn) or a serverless application (such as AWS Lambda).\n\nThe SDK handles all the mechanics of the [webhook lifecycle interface](https://developer-preview.smartthings.com/docs/connected-services/lifecycles/) on your behalf.  You just implement a single endpoint to accept the SmartApp webhook requests, and a single callback class where you define specialized behavior for the webhook events.  A clean [attrs](https://www.attrs.org/en/stable/) object interface is exposed for use by your callback.\n\nSDK documentation is found at [smartapp-sdk.readthedocs.io](https://smartapp-sdk.readthedocs.io/en/stable/).  Look there for installation instructions, the class model documentation, and example code. The [smartapp-sensortrack](https://github.com/pronovic/smartapp-sensortrack) repo on GitHub is also a good example of how to use this SDK to build a traditional Python webapp.\n",
     'author': 'Kenneth J. Pronovici',
     'author_email': 'pronovic@ieee.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pypi.org/project/smartapp-sdk/',
```

### Comparing `smartapp_sdk-0.5.4/PKG-INFO` & `smartapp_sdk-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartapp-sdk
-Version: 0.5.4
+Version: 0.6.0
 Summary: Framework to build a webhook-based SmartThings SmartApp
 Home-page: https://pypi.org/project/smartapp-sdk/
 License: Apache-2.0
 Author: Kenneth J. Pronovici
 Author-email: pronovic@ieee.org
 Requires-Python: >=3.9,<4
 Classifier: Development Status :: 4 - Beta
```

