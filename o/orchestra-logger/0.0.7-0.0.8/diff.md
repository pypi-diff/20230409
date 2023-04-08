# Comparing `tmp/orchestra-logger-0.0.7.tar.gz` & `tmp/orchestra-logger-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchestra-logger-0.0.7.tar", last modified: Sat Apr  8 22:40:06 2023, max compression
+gzip compressed data, was "orchestra-logger-0.0.8.tar", last modified: Sat Apr  8 22:42:47 2023, max compression
```

## Comparing `orchestra-logger-0.0.7.tar` & `orchestra-logger-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 22:40:06.007160 orchestra-logger-0.0.7/
--rw-rw-rw-   0        0        0     1098 2023-04-08 22:02:33.000000 orchestra-logger-0.0.7/LICENSE.gitignore
--rw-rw-rw-   0        0        0      711 2023-04-08 22:40:06.007160 orchestra-logger-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-04-08 11:40:32.000000 orchestra-logger-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 22:40:05.990161 orchestra-logger-0.0.7/orchestra_logger/
--rw-rw-rw-   0        0        0       70 2023-04-08 22:38:50.000000 orchestra-logger-0.0.7/orchestra_logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 22:40:06.006161 orchestra-logger-0.0.7/orchestra_logger/orclogger/
--rw-rw-rw-   0        0        0        0 2023-04-08 11:57:19.000000 orchestra-logger-0.0.7/orchestra_logger/orclogger/__init__.py
--rw-rw-rw-   0        0        0     1582 2023-04-08 21:40:40.000000 orchestra-logger-0.0.7/orchestra_logger/orclogger/orclogger.py
-drwxrwxrwx   0        0        0        0 2023-04-08 22:40:06.004163 orchestra-logger-0.0.7/orchestra_logger.egg-info/
--rw-rw-rw-   0        0        0      711 2023-04-08 22:40:05.000000 orchestra-logger-0.0.7/orchestra_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-04-08 22:40:05.000000 orchestra-logger-0.0.7/orchestra_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 22:40:05.000000 orchestra-logger-0.0.7/orchestra_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-08 22:40:05.000000 orchestra-logger-0.0.7/orchestra_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-08 22:40:06.008912 orchestra-logger-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1396 2023-04-08 22:39:51.000000 orchestra-logger-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 22:42:47.952741 orchestra-logger-0.0.8/
+-rw-rw-rw-   0        0        0     1098 2023-04-08 22:02:33.000000 orchestra-logger-0.0.8/LICENSE.gitignore
+-rw-rw-rw-   0        0        0      711 2023-04-08 22:42:47.952741 orchestra-logger-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-04-08 11:40:32.000000 orchestra-logger-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-08 22:42:47.921756 orchestra-logger-0.0.8/orchestra_logger/
+-rw-rw-rw-   0        0        0       70 2023-04-08 22:38:50.000000 orchestra-logger-0.0.8/orchestra_logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-08 22:42:47.951748 orchestra-logger-0.0.8/orchestra_logger/orclogger/
+-rw-rw-rw-   0        0        0        0 2023-04-08 11:57:19.000000 orchestra-logger-0.0.8/orchestra_logger/orclogger/__init__.py
+-rw-rw-rw-   0        0        0     1582 2023-04-08 21:40:40.000000 orchestra-logger-0.0.8/orchestra_logger/orclogger/orclogger.py
+drwxrwxrwx   0        0        0        0 2023-04-08 22:42:47.946487 orchestra-logger-0.0.8/orchestra_logger.egg-info/
+-rw-rw-rw-   0        0        0      711 2023-04-08 22:42:47.000000 orchestra-logger-0.0.8/orchestra_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-04-08 22:42:47.000000 orchestra-logger-0.0.8/orchestra_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 22:42:47.000000 orchestra-logger-0.0.8/orchestra_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-08 22:42:47.000000 orchestra-logger-0.0.8/orchestra_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-08 22:42:47.956569 orchestra-logger-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1396 2023-04-08 22:42:22.000000 orchestra-logger-0.0.8/setup.py
```

### Comparing `orchestra-logger-0.0.7/LICENSE.gitignore` & `orchestra-logger-0.0.8/LICENSE.gitignore`

 * *Files identical despite different names*

### Comparing `orchestra-logger-0.0.7/PKG-INFO` & `orchestra-logger-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestra-logger
-Version: 0.0.7
+Version: 0.0.8
 Summary: Logging module to enable orchestration on self-hosted applications
 Home-page: UNKNOWN
 Author: Orchestra (Hugo Lu)
 Author-email: <hugo@getorchestra.io>
 License: UNKNOWN
 Keywords: python,logging,data,orchestration
 Platform: UNKNOWN
```

### Comparing `orchestra-logger-0.0.7/orchestra_logger/orclogger/orclogger.py` & `orchestra-logger-0.0.8/orchestra_logger/orclogger/orclogger.py`

 * *Files identical despite different names*

### Comparing `orchestra-logger-0.0.7/orchestra_logger.egg-info/PKG-INFO` & `orchestra-logger-0.0.8/orchestra_logger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchestra-logger
-Version: 0.0.7
+Version: 0.0.8
 Summary: Logging module to enable orchestration on self-hosted applications
 Home-page: UNKNOWN
 Author: Orchestra (Hugo Lu)
 Author-email: <hugo@getorchestra.io>
 License: UNKNOWN
 Keywords: python,logging,data,orchestration
 Platform: UNKNOWN
```

### Comparing `orchestra-logger-0.0.7/setup.py` & `orchestra-logger-0.0.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'Logging module to enable orchestration on self-hosted applications'
 LONG_DESCRIPTION = 'A logging-like module to be implemented on self-hosted applications that allows Orchestra to coordinate tasks and gather metadata'
 
 # Setting up
 setup(
     name="orchestra-logger",
     version=VERSION,
```

