# Comparing `tmp/orchestra-logger-0.0.4.tar.gz` & `tmp/orchestra-logger-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchestra-logger-0.0.4.tar", last modified: Sat Apr  8 22:23:35 2023, max compression
+gzip compressed data, was "orchestra-logger-0.0.5.tar", last modified: Sat Apr  8 22:27:51 2023, max compression
```

## Comparing `orchestra-logger-0.0.4.tar` & `orchestra-logger-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 22:23:35.033430 orchestra-logger-0.0.4/
--rw-rw-rw-   0        0        0     1098 2023-04-08 22:02:33.000000 orchestra-logger-0.0.4/LICENSE.gitignore
--rw-rw-rw-   0        0        0      711 2023-04-08 22:23:35.033430 orchestra-logger-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-04-08 11:40:32.000000 orchestra-logger-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 22:23:35.025455 orchestra-logger-0.0.4/orchestra_logger.egg-info/
--rw-rw-rw-   0        0        0      711 2023-04-08 22:23:34.000000 orchestra-logger-0.0.4/orchestra_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-04-08 22:23:34.000000 orchestra-logger-0.0.4/orchestra_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 22:23:34.000000 orchestra-logger-0.0.4/orchestra_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-04-08 22:23:34.000000 orchestra-logger-0.0.4/orchestra_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-08 22:23:35.035468 orchestra-logger-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1396 2023-04-08 22:23:21.000000 orchestra-logger-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 22:23:35.028384 orchestra-logger-0.0.4/src/
--rw-rw-rw-   0        0        0       53 2023-04-08 22:23:21.000000 orchestra-logger-0.0.4/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 22:23:35.031423 orchestra-logger-0.0.4/src/orclogger/
--rw-rw-rw-   0        0        0        0 2023-04-08 11:57:19.000000 orchestra-logger-0.0.4/src/orclogger/__init__.py
--rw-rw-rw-   0        0        0     1582 2023-04-08 21:40:40.000000 orchestra-logger-0.0.4/src/orclogger/orclogger.py
+drwxrwxrwx   0        0        0        0 2023-04-08 22:27:51.990539 orchestra-logger-0.0.5/
+-rw-rw-rw-   0        0        0     1098 2023-04-08 22:02:33.000000 orchestra-logger-0.0.5/LICENSE.gitignore
+-rw-rw-rw-   0        0        0      711 2023-04-08 22:27:51.990539 orchestra-logger-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-04-08 11:40:32.000000 orchestra-logger-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-08 22:27:51.983535 orchestra-logger-0.0.5/orchestra_logger.egg-info/
+-rw-rw-rw-   0        0        0      711 2023-04-08 22:27:51.000000 orchestra-logger-0.0.5/orchestra_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-04-08 22:27:51.000000 orchestra-logger-0.0.5/orchestra_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 22:27:51.000000 orchestra-logger-0.0.5/orchestra_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-04-08 22:27:51.000000 orchestra-logger-0.0.5/orchestra_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-08 22:27:51.992619 orchestra-logger-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1396 2023-04-08 22:27:33.000000 orchestra-logger-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 22:27:51.985622 orchestra-logger-0.0.5/src/
+-rw-rw-rw-   0        0        0       57 2023-04-08 22:26:31.000000 orchestra-logger-0.0.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-08 22:27:51.988540 orchestra-logger-0.0.5/src/orclogger/
+-rw-rw-rw-   0        0        0        0 2023-04-08 11:57:19.000000 orchestra-logger-0.0.5/src/orclogger/__init__.py
+-rw-rw-rw-   0        0        0     1582 2023-04-08 21:40:40.000000 orchestra-logger-0.0.5/src/orclogger/orclogger.py
```

### Comparing `orchestra-logger-0.0.4/LICENSE.gitignore` & `orchestra-logger-0.0.5/LICENSE.gitignore`

 * *Files identical despite different names*

### Comparing `orchestra-logger-0.0.4/PKG-INFO` & `orchestra-logger-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestra-logger
-Version: 0.0.4
+Version: 0.0.5
 Summary: Logging module to enable orchestration on self-hosted applications
 Home-page: UNKNOWN
 Author: Orchestra (Hugo Lu)
 Author-email: <hugo@getorchestra.io>
 License: UNKNOWN
 Keywords: python,logging,data,orchestration
 Platform: UNKNOWN
```

### Comparing `orchestra-logger-0.0.4/orchestra_logger.egg-info/PKG-INFO` & `orchestra-logger-0.0.5/orchestra_logger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestra-logger
-Version: 0.0.4
+Version: 0.0.5
 Summary: Logging module to enable orchestration on self-hosted applications
 Home-page: UNKNOWN
 Author: Orchestra (Hugo Lu)
 Author-email: <hugo@getorchestra.io>
 License: UNKNOWN
 Keywords: python,logging,data,orchestration
 Platform: UNKNOWN
```

### Comparing `orchestra-logger-0.0.4/setup.py` & `orchestra-logger-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Logging module to enable orchestration on self-hosted applications'
 LONG_DESCRIPTION = 'A logging-like module to be implemented on self-hosted applications that allows Orchestra to coordinate tasks and gather metadata'
 
 # Setting up
 setup(
     name="orchestra-logger",
     version=VERSION,
```

### Comparing `orchestra-logger-0.0.4/src/orclogger/orclogger.py` & `orchestra-logger-0.0.5/src/orclogger/orclogger.py`

 * *Files identical despite different names*

