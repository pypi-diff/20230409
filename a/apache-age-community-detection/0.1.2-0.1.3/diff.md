# Comparing `tmp/apache-age-community-detection-0.1.2.tar.gz` & `tmp/apache-age-community-detection-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-age-community-detection-0.1.2.tar", last modified: Sun Apr  9 13:37:51 2023, max compression
+gzip compressed data, was "apache-age-community-detection-0.1.3.tar", last modified: Sun Apr  9 13:41:59 2023, max compression
```

## Comparing `apache-age-community-detection-0.1.2.tar` & `apache-age-community-detection-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:37:51.193340 apache-age-community-detection-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-09 13:37:42.000000 apache-age-community-detection-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-09 13:37:51.193340 apache-age-community-detection-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-09 13:37:42.000000 apache-age-community-detection-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:37:51.189339 apache-age-community-detection-0.1.2/age_community_detection/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-09 13:37:42.000000 apache-age-community-detection-0.1.2/age_community_detection/Check.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-09 13:37:42.000000 apache-age-community-detection-0.1.2/age_community_detection/Exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 13:37:42.000000 apache-age-community-detection-0.1.2/age_community_detection/Graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-09 13:37:42.000000 apache-age-community-detection-0.1.2/age_community_detection/Lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-09 13:37:42.000000 apache-age-community-detection-0.1.2/age_community_detection/VERSION.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-09 13:37:42.000000 apache-age-community-detection-0.1.2/age_community_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:37:51.189339 apache-age-community-detection-0.1.2/age_community_detection/lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)    17112 2023-04-09 13:37:42.000000 apache-age-community-detection-0.1.2/age_community_detection/lib/library.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:37:51.193340 apache-age-community-detection-0.1.2/apache_age_community_detection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-09 13:37:51.000000 apache-age-community-detection-0.1.2/apache_age_community_detection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-09 13:37:51.000000 apache-age-community-detection-0.1.2/apache_age_community_detection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 13:37:51.000000 apache-age-community-detection-0.1.2/apache_age_community_detection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 13:37:51.000000 apache-age-community-detection-0.1.2/apache_age_community_detection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-09 13:37:51.000000 apache-age-community-detection-0.1.2/apache_age_community_detection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 13:37:51.193340 apache-age-community-detection-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-09 13:37:42.000000 apache-age-community-detection-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:41:59.131273 apache-age-community-detection-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-09 13:41:59.131273 apache-age-community-detection-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:41:59.131273 apache-age-community-detection-0.1.3/age_community_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/age_community_detection/Check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/age_community_detection/Exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/age_community_detection/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/age_community_detection/Lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/age_community_detection/VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/age_community_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:41:59.131273 apache-age-community-detection-0.1.3/age_community_detection/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17112 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/age_community_detection/lib/library.dll
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17112 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/age_community_detection/lib/library.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:41:59.131273 apache-age-community-detection-0.1.3/apache_age_community_detection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-09 13:41:59.000000 apache-age-community-detection-0.1.3/apache_age_community_detection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-09 13:41:59.000000 apache-age-community-detection-0.1.3/apache_age_community_detection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 13:41:59.000000 apache-age-community-detection-0.1.3/apache_age_community_detection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 13:41:59.000000 apache-age-community-detection-0.1.3/apache_age_community_detection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-09 13:41:59.000000 apache-age-community-detection-0.1.3/apache_age_community_detection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 13:41:59.131273 apache-age-community-detection-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-09 13:41:50.000000 apache-age-community-detection-0.1.3/setup.py
```

### Comparing `apache-age-community-detection-0.1.2/LICENSE` & `apache-age-community-detection-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.2/PKG-INFO` & `apache-age-community-detection-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-age-community-detection
-Version: 0.1.2
+Version: 0.1.3
 Summary: Detection of Community by maximizing modularity
 Home-page: https://github.com/Munmud/Community-Detection-Modularity
 Author: Moontasir Mahmood
 Author-email: moontasir042@gmail.com
 License: Apache2.0
 Keywords: Community-Detection,Modularity,Reichardt and Bornholdt,Newman,partition network,k means cluster
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `apache-age-community-detection-0.1.2/README.md` & `apache-age-community-detection-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.2/age_community_detection/Check.py` & `apache-age-community-detection-0.1.3/age_community_detection/Check.py`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.2/age_community_detection/Exception.py` & `apache-age-community-detection-0.1.3/age_community_detection/Exception.py`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.2/age_community_detection/Graph.py` & `apache-age-community-detection-0.1.3/age_community_detection/Graph.py`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.2/age_community_detection/Lib.py` & `apache-age-community-detection-0.1.3/age_community_detection/Lib.py`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.2/age_community_detection/lib/library.so` & `apache-age-community-detection-0.1.3/age_community_detection/lib/library.dll`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.2/apache_age_community_detection.egg-info/PKG-INFO` & `apache-age-community-detection-0.1.3/apache_age_community_detection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-age-community-detection
-Version: 0.1.2
+Version: 0.1.3
 Summary: Detection of Community by maximizing modularity
 Home-page: https://github.com/Munmud/Community-Detection-Modularity
 Author: Moontasir Mahmood
 Author-email: moontasir042@gmail.com
 License: Apache2.0
 Keywords: Community-Detection,Modularity,Reichardt and Bornholdt,Newman,partition network,k means cluster
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `apache-age-community-detection-0.1.2/apache_age_community_detection.egg-info/SOURCES.txt` & `apache-age-community-detection-0.1.3/apache_age_community_detection.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -3,13 +3,14 @@
 setup.py
 age_community_detection/Check.py
 age_community_detection/Exception.py
 age_community_detection/Graph.py
 age_community_detection/Lib.py
 age_community_detection/VERSION.py
 age_community_detection/__init__.py
+age_community_detection/lib/library.dll
 age_community_detection/lib/library.so
 apache_age_community_detection.egg-info/PKG-INFO
 apache_age_community_detection.egg-info/SOURCES.txt
 apache_age_community_detection.egg-info/dependency_links.txt
 apache_age_community_detection.egg-info/requires.txt
 apache_age_community_detection.egg-info/top_level.txt
```

### Comparing `apache-age-community-detection-0.1.2/setup.py` & `apache-age-community-detection-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,14 @@
     long_description_content_type="text/markdown",
     author           = 'Moontasir Mahmood',
     author_email     = 'moontasir042@gmail.com',
     url              = 'https://github.com/Munmud/Community-Detection-Modularity',
     license          = 'Apache2.0',
     install_requires = ['numpy'],
     packages         = ['age_community_detection'],
-    package_data={'age_community_detection': ['lib/*.so']},
+    package_data={'age_community_detection': ['lib/*.so', 'lib/*.dll']},
     keywords         = ['Community-Detection', 'Modularity', 'Reichardt and Bornholdt','Newman', 'partition network', 'k means cluster'],
     python_requires  = '>=3.9',
     classifiers      = [
         'Programming Language :: Python :: 3.9'
     ]
 )
```

