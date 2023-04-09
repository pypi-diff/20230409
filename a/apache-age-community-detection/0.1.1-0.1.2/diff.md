# Comparing `tmp/apache-age-community-detection-0.1.1.tar.gz` & `tmp/apache-age-community-detection-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-age-community-detection-0.1.1.tar", last modified: Sun Apr  9 13:22:41 2023, max compression
+gzip compressed data, was "apache-age-community-detection-0.1.2.tar", last modified: Sun Apr  9 13:37:51 2023, max compression
```

## Comparing `apache-age-community-detection-0.1.1.tar` & `apache-age-community-detection-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:22:41.136507 apache-age-community-detection-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-09 13:22:31.000000 apache-age-community-detection-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-09 13:22:41.136507 apache-age-community-detection-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-09 13:22:31.000000 apache-age-community-detection-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:22:41.136507 apache-age-community-detection-0.1.1/age_community_detection/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-09 13:22:31.000000 apache-age-community-detection-0.1.1/age_community_detection/Check.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-09 13:22:31.000000 apache-age-community-detection-0.1.1/age_community_detection/Exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 13:22:31.000000 apache-age-community-detection-0.1.1/age_community_detection/Graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-09 13:22:31.000000 apache-age-community-detection-0.1.1/age_community_detection/Lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-09 13:22:31.000000 apache-age-community-detection-0.1.1/age_community_detection/VERSION.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-09 13:22:31.000000 apache-age-community-detection-0.1.1/age_community_detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:22:41.136507 apache-age-community-detection-0.1.1/age_community_detection/lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)    17112 2023-04-09 13:22:31.000000 apache-age-community-detection-0.1.1/age_community_detection/lib/library.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:22:41.136507 apache-age-community-detection-0.1.1/apache_age_community_detection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-09 13:22:41.000000 apache-age-community-detection-0.1.1/apache_age_community_detection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-09 13:22:41.000000 apache-age-community-detection-0.1.1/apache_age_community_detection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 13:22:41.000000 apache-age-community-detection-0.1.1/apache_age_community_detection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 13:22:41.000000 apache-age-community-detection-0.1.1/apache_age_community_detection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-09 13:22:41.000000 apache-age-community-detection-0.1.1/apache_age_community_detection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 13:22:41.136507 apache-age-community-detection-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-09 13:22:31.000000 apache-age-community-detection-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:37:51.193340 apache-age-community-detection-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-09 13:37:42.000000 apache-age-community-detection-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-09 13:37:51.193340 apache-age-community-detection-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-09 13:37:42.000000 apache-age-community-detection-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:37:51.189339 apache-age-community-detection-0.1.2/age_community_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-09 13:37:42.000000 apache-age-community-detection-0.1.2/age_community_detection/Check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-09 13:37:42.000000 apache-age-community-detection-0.1.2/age_community_detection/Exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 13:37:42.000000 apache-age-community-detection-0.1.2/age_community_detection/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-09 13:37:42.000000 apache-age-community-detection-0.1.2/age_community_detection/Lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-09 13:37:42.000000 apache-age-community-detection-0.1.2/age_community_detection/VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-09 13:37:42.000000 apache-age-community-detection-0.1.2/age_community_detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:37:51.189339 apache-age-community-detection-0.1.2/age_community_detection/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17112 2023-04-09 13:37:42.000000 apache-age-community-detection-0.1.2/age_community_detection/lib/library.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 13:37:51.193340 apache-age-community-detection-0.1.2/apache_age_community_detection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-09 13:37:51.000000 apache-age-community-detection-0.1.2/apache_age_community_detection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-09 13:37:51.000000 apache-age-community-detection-0.1.2/apache_age_community_detection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 13:37:51.000000 apache-age-community-detection-0.1.2/apache_age_community_detection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 13:37:51.000000 apache-age-community-detection-0.1.2/apache_age_community_detection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-09 13:37:51.000000 apache-age-community-detection-0.1.2/apache_age_community_detection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 13:37:51.193340 apache-age-community-detection-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-09 13:37:42.000000 apache-age-community-detection-0.1.2/setup.py
```

### Comparing `apache-age-community-detection-0.1.1/LICENSE` & `apache-age-community-detection-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.1/PKG-INFO` & `apache-age-community-detection-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-age-community-detection
-Version: 0.1.1
+Version: 0.1.2
 Summary: Detection of Community by maximizing modularity
 Home-page: https://github.com/Munmud/Community-Detection-Modularity
 Author: Moontasir Mahmood
 Author-email: moontasir042@gmail.com
 License: Apache2.0
 Keywords: Community-Detection,Modularity,Reichardt and Bornholdt,Newman,partition network,k means cluster
 Classifier: Programming Language :: Python :: 3.9
@@ -53,14 +53,15 @@
 ```
 
 ### Create Graph
 ```py
 nodes = [0, 1, 2, 3, 4, 5]
 edges = [[0, 1], [0, 2], [1, 2], [2, 3], [3, 4], [3, 5], [4, 5]]
 g = Graph.Graph()
+g.createGraph(nodes, edges)
 ```
 - Nodes : `0 to N-1`
 - Edges : 
     - `2d array : adjacency list`
     - `Each element between 0 to N-1`
 
 ### Generate Community Assignment
@@ -70,11 +71,14 @@
 
 ### Output Format
 ```
 [1, 1, 1, 0, 0, 0, 2, 2, 0, 3, 3, 1, 3]
 ```
 - Here each number represents the community number of corresponding node
 
+### Samples
+- [Creating Graph](https://github.com/Munmud/Community-Detection-Modularity/blob/main/Samples/sample1.py)
+
 ### Reference
 - [Finding community structure in networks using the eigenvectors of matrices](https://arxiv.org/pdf/physics/0605087.pdf)
 - [Modularity and community structure in networks](https://www.pnas.org/doi/10.1073/pnas.0601602103)
 - [Statistical Mechanics of Community Detection](https://ia903002.us.archive.org/33/items/arxiv-cond-mat0603718/cond-mat0603718.pdf)
```

### Comparing `apache-age-community-detection-0.1.1/README.md` & `apache-age-community-detection-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 ```
 
 ### Create Graph
 ```py
 nodes = [0, 1, 2, 3, 4, 5]
 edges = [[0, 1], [0, 2], [1, 2], [2, 3], [3, 4], [3, 5], [4, 5]]
 g = Graph.Graph()
+g.createGraph(nodes, edges)
 ```
 - Nodes : `0 to N-1`
 - Edges : 
     - `2d array : adjacency list`
     - `Each element between 0 to N-1`
 
 ### Generate Community Assignment
@@ -56,11 +57,14 @@
 
 ### Output Format
 ```
 [1, 1, 1, 0, 0, 0, 2, 2, 0, 3, 3, 1, 3]
 ```
 - Here each number represents the community number of corresponding node
 
+### Samples
+- [Creating Graph](https://github.com/Munmud/Community-Detection-Modularity/blob/main/Samples/sample1.py)
+
 ### Reference
 - [Finding community structure in networks using the eigenvectors of matrices](https://arxiv.org/pdf/physics/0605087.pdf)
 - [Modularity and community structure in networks](https://www.pnas.org/doi/10.1073/pnas.0601602103)
 - [Statistical Mechanics of Community Detection](https://ia903002.us.archive.org/33/items/arxiv-cond-mat0603718/cond-mat0603718.pdf)
```

### Comparing `apache-age-community-detection-0.1.1/age_community_detection/Check.py` & `apache-age-community-detection-0.1.2/age_community_detection/Check.py`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.1/age_community_detection/Exception.py` & `apache-age-community-detection-0.1.2/age_community_detection/Exception.py`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.1/age_community_detection/Graph.py` & `apache-age-community-detection-0.1.2/age_community_detection/Graph.py`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.1/age_community_detection/Lib.py` & `apache-age-community-detection-0.1.2/age_community_detection/Lib.py`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.1/age_community_detection/lib/library.so` & `apache-age-community-detection-0.1.2/age_community_detection/lib/library.so`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.1/apache_age_community_detection.egg-info/PKG-INFO` & `apache-age-community-detection-0.1.2/apache_age_community_detection.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-age-community-detection
-Version: 0.1.1
+Version: 0.1.2
 Summary: Detection of Community by maximizing modularity
 Home-page: https://github.com/Munmud/Community-Detection-Modularity
 Author: Moontasir Mahmood
 Author-email: moontasir042@gmail.com
 License: Apache2.0
 Keywords: Community-Detection,Modularity,Reichardt and Bornholdt,Newman,partition network,k means cluster
 Classifier: Programming Language :: Python :: 3.9
@@ -53,14 +53,15 @@
 ```
 
 ### Create Graph
 ```py
 nodes = [0, 1, 2, 3, 4, 5]
 edges = [[0, 1], [0, 2], [1, 2], [2, 3], [3, 4], [3, 5], [4, 5]]
 g = Graph.Graph()
+g.createGraph(nodes, edges)
 ```
 - Nodes : `0 to N-1`
 - Edges : 
     - `2d array : adjacency list`
     - `Each element between 0 to N-1`
 
 ### Generate Community Assignment
@@ -70,11 +71,14 @@
 
 ### Output Format
 ```
 [1, 1, 1, 0, 0, 0, 2, 2, 0, 3, 3, 1, 3]
 ```
 - Here each number represents the community number of corresponding node
 
+### Samples
+- [Creating Graph](https://github.com/Munmud/Community-Detection-Modularity/blob/main/Samples/sample1.py)
+
 ### Reference
 - [Finding community structure in networks using the eigenvectors of matrices](https://arxiv.org/pdf/physics/0605087.pdf)
 - [Modularity and community structure in networks](https://www.pnas.org/doi/10.1073/pnas.0601602103)
 - [Statistical Mechanics of Community Detection](https://ia903002.us.archive.org/33/items/arxiv-cond-mat0603718/cond-mat0603718.pdf)
```

### Comparing `apache-age-community-detection-0.1.1/apache_age_community_detection.egg-info/SOURCES.txt` & `apache-age-community-detection-0.1.2/apache_age_community_detection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-age-community-detection-0.1.1/setup.py` & `apache-age-community-detection-0.1.2/setup.py`

 * *Files identical despite different names*

