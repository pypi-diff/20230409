# Comparing `tmp/apache-age-community-detection-0.1.0.tar.gz` & `tmp/apache-age-community-detection-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-age-community-detection-0.1.0.tar", last modified: Sat Apr  8 16:45:45 2023, max compression
+gzip compressed data, was "apache-age-community-detection-0.1.1.tar", last modified: Sun Apr  9 13:22:41 2023, max compression
```

## Comparing `apache-age-community-detection-0.1.0.tar` & `apache-age-community-detection-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:45:45.233186 apache-age-community-detection-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-08 16:45:36.000000 apache-age-community-detection-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-08 16:45:45.233186 apache-age-community-detection-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-08 16:45:36.000000 apache-age-community-detection-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:45:45.233186 apache-age-community-detection-0.1.0/age_community_detection/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-08 16:45:36.000000 apache-age-community-detection-0.1.0/age_community_detection/Check.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-08 16:45:36.000000 apache-age-community-detection-0.1.0/age_community_detection/Exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-08 16:45:36.000000 apache-age-community-detection-0.1.0/age_community_detection/Graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-08 16:45:36.000000 apache-age-community-detection-0.1.0/age_community_detection/Lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-08 16:45:36.000000 apache-age-community-detection-0.1.0/age_community_detection/VERSION.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-08 16:45:36.000000 apache-age-community-detection-0.1.0/age_community_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:45:45.233186 apache-age-community-detection-0.1.0/age_community_detection/lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)    17112 2023-04-08 16:45:36.000000 apache-age-community-detection-0.1.0/age_community_detection/lib/library.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:45:45.233186 apache-age-community-detection-0.1.0/apache_age_community_detection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-08 16:45:45.000000 apache-age-community-detection-0.1.0/apache_age_community_detection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-08 16:45:45.000000 apache-age-community-detection-0.1.0/apache_age_community_detection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 16:45:45.000000 apache-age-community-detection-0.1.0/apache_age_community_detection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 16:45:45.000000 apache-age-community-detection-0.1.0/apache_age_community_detection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-08 16:45:45.000000 apache-age-community-detection-0.1.0/apache_age_community_detection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 16:45:45.233186 apache-age-community-detection-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-08 16:45:36.000000 apache-age-community-detection-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:22:41.136507 apache-age-community-detection-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-09 13:22:31.000000 apache-age-community-detection-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-09 13:22:41.136507 apache-age-community-detection-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-09 13:22:31.000000 apache-age-community-detection-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:22:41.136507 apache-age-community-detection-0.1.1/age_community_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-09 13:22:31.000000 apache-age-community-detection-0.1.1/age_community_detection/Check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-09 13:22:31.000000 apache-age-community-detection-0.1.1/age_community_detection/Exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 13:22:31.000000 apache-age-community-detection-0.1.1/age_community_detection/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-09 13:22:31.000000 apache-age-community-detection-0.1.1/age_community_detection/Lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-09 13:22:31.000000 apache-age-community-detection-0.1.1/age_community_detection/VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-09 13:22:31.000000 apache-age-community-detection-0.1.1/age_community_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:22:41.136507 apache-age-community-detection-0.1.1/age_community_detection/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17112 2023-04-09 13:22:31.000000 apache-age-community-detection-0.1.1/age_community_detection/lib/library.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:22:41.136507 apache-age-community-detection-0.1.1/apache_age_community_detection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-09 13:22:41.000000 apache-age-community-detection-0.1.1/apache_age_community_detection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-09 13:22:41.000000 apache-age-community-detection-0.1.1/apache_age_community_detection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 13:22:41.000000 apache-age-community-detection-0.1.1/apache_age_community_detection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 13:22:41.000000 apache-age-community-detection-0.1.1/apache_age_community_detection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-09 13:22:41.000000 apache-age-community-detection-0.1.1/apache_age_community_detection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 13:22:41.136507 apache-age-community-detection-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-09 13:22:31.000000 apache-age-community-detection-0.1.1/setup.py
```

### Comparing `apache-age-community-detection-0.1.0/LICENSE` & `apache-age-community-detection-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.0/PKG-INFO` & `apache-age-community-detection-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-age-community-detection
-Version: 0.1.0
+Version: 0.1.1
 Summary: Detection of Community by maximizing modularity
 Home-page: https://github.com/Munmud/Community-Detection-Modularity
 Author: Moontasir Mahmood
 Author-email: moontasir042@gmail.com
 License: Apache2.0
 Keywords: Community-Detection,Modularity,Reichardt and Bornholdt,Newman,partition network,k means cluster
 Classifier: Programming Language :: Python :: 3.9
@@ -36,14 +36,19 @@
 sudo apt-get update
 sudo apt-get install libeigen3-dev
 git clone https://github.com/Munmud/Community-Detection-Modularity
 cd Community-Detection-Modularity
 python setup.py install
 ```
 
+### Unit Test
+```cmd
+python -m unittest test_community.py
+```
+
 ## Instruction
 
 ### import
 ```py
 from age_community_detection import Graph
 ```
```

### Comparing `apache-age-community-detection-0.1.0/README.md` & `apache-age-community-detection-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,19 @@
 sudo apt-get update
 sudo apt-get install libeigen3-dev
 git clone https://github.com/Munmud/Community-Detection-Modularity
 cd Community-Detection-Modularity
 python setup.py install
 ```
 
+### Unit Test
+```cmd
+python -m unittest test_community.py
+```
+
 ## Instruction
 
 ### import
 ```py
 from age_community_detection import Graph
 ```
```

### Comparing `apache-age-community-detection-0.1.0/age_community_detection/Check.py` & `apache-age-community-detection-0.1.1/age_community_detection/Check.py`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.0/age_community_detection/Exception.py` & `apache-age-community-detection-0.1.1/age_community_detection/Exception.py`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.0/age_community_detection/Graph.py` & `apache-age-community-detection-0.1.1/age_community_detection/Graph.py`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.0/age_community_detection/lib/library.so` & `apache-age-community-detection-0.1.1/age_community_detection/lib/library.so`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.0/apache_age_community_detection.egg-info/PKG-INFO` & `apache-age-community-detection-0.1.1/apache_age_community_detection.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-age-community-detection
-Version: 0.1.0
+Version: 0.1.1
 Summary: Detection of Community by maximizing modularity
 Home-page: https://github.com/Munmud/Community-Detection-Modularity
 Author: Moontasir Mahmood
 Author-email: moontasir042@gmail.com
 License: Apache2.0
 Keywords: Community-Detection,Modularity,Reichardt and Bornholdt,Newman,partition network,k means cluster
 Classifier: Programming Language :: Python :: 3.9
@@ -36,14 +36,19 @@
 sudo apt-get update
 sudo apt-get install libeigen3-dev
 git clone https://github.com/Munmud/Community-Detection-Modularity
 cd Community-Detection-Modularity
 python setup.py install
 ```
 
+### Unit Test
+```cmd
+python -m unittest test_community.py
+```
+
 ## Instruction
 
 ### import
 ```py
 from age_community_detection import Graph
 ```
```

### Comparing `apache-age-community-detection-0.1.0/apache_age_community_detection.egg-info/SOURCES.txt` & `apache-age-community-detection-0.1.1/apache_age_community_detection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.0/setup.py` & `apache-age-community-detection-0.1.1/setup.py`

 * *Files identical despite different names*

