# Comparing `tmp/datastructuresLionelEric-1.0.7.tar.gz` & `tmp/datastructuresLionelEric-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datastructuresLionelEric-1.0.7.tar", last modified: Sun Apr  9 21:58:25 2023, max compression
+gzip compressed data, was "datastructuresLionelEric-1.0.8.tar", last modified: Sun Apr  9 22:00:26 2023, max compression
```

## Comparing `datastructuresLionelEric-1.0.7.tar` & `datastructuresLionelEric-1.0.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:58:25.700428 datastructuresLionelEric-1.0.7/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-03-29 13:29:16.000000 datastructuresLionelEric-1.0.7/.DS_Store
--rw-r--r--   0 lionelhasan   (501) staff       (20)      215 2023-04-09 21:58:25.700167 datastructuresLionelEric-1.0.7/PKG-INFO
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:58:25.693703 datastructuresLionelEric-1.0.7/datastructures/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.7/datastructures/.DS_Store
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:58:25.696479 datastructuresLionelEric-1.0.7/datastructures/Linear/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6914 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.7/datastructures/Linear/CDLL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     8735 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.7/datastructures/Linear/CSLL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6857 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.7/datastructures/Linear/DLL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     1065 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.7/datastructures/Linear/LLQueue.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     1259 2023-04-08 22:50:35.000000 datastructuresLionelEric-1.0.7/datastructures/Linear/LLStack.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     7718 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.7/datastructures/Linear/SLL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.7/datastructures/Linear/__init__.py
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:58:25.697486 datastructuresLionelEric-1.0.7/datastructures/Linear/__pycache__/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     4716 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.7/datastructures/Linear/__pycache__/CDLL.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     5162 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.7/datastructures/Linear/__pycache__/CSLL.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     4620 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.7/datastructures/Linear/__pycache__/DLL.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     1780 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.7/datastructures/Linear/__pycache__/LLQueue.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     2365 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.7/datastructures/Linear/__pycache__/LLStack.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     4657 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.7/datastructures/Linear/__pycache__/SLL.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)      177 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.7/datastructures/Linear/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:58:25.698145 datastructuresLionelEric-1.0.7/datastructures/nodes/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.7/datastructures/nodes/.DS_Store
--rw-r--r--   0 lionelhasan   (501) staff       (20)      116 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.7/datastructures/nodes/Dnode.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     1080 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.7/datastructures/nodes/TNode.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.7/datastructures/nodes/__init__.py
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:58:25.698509 datastructuresLionelEric-1.0.7/datastructures/nodes/__pycache__/
--rw-r--r--   0 lionelhasan   (501) staff       (20)      476 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.7/datastructures/nodes/__pycache__/Dnode.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     2118 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.7/datastructures/nodes/__pycache__/TNode.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)      176 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.7/datastructures/nodes/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:58:25.698767 datastructuresLionelEric-1.0.7/datastructures/trees/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6667 2023-04-09 21:33:54.000000 datastructuresLionelEric-1.0.7/datastructures/trees/AVL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     5584 2023-04-09 21:50:16.000000 datastructuresLionelEric-1.0.7/datastructures/trees/BST.py
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:58:25.699457 datastructuresLionelEric-1.0.7/datastructures/trees/__pycache__/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     3696 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.7/datastructures/trees/__pycache__/AVL.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     3364 2023-04-09 21:50:17.000000 datastructuresLionelEric-1.0.7/datastructures/trees/__pycache__/BST.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)      176 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.7/datastructures/trees/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:58:25.699955 datastructuresLionelEric-1.0.7/datastructuresLionelEric.egg-info/
--rw-r--r--   0 lionelhasan   (501) staff       (20)      215 2023-04-09 21:58:25.000000 datastructuresLionelEric-1.0.7/datastructuresLionelEric.egg-info/PKG-INFO
--rw-r--r--   0 lionelhasan   (501) staff       (20)     1345 2023-04-09 21:58:25.000000 datastructuresLionelEric-1.0.7/datastructuresLionelEric.egg-info/SOURCES.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 21:58:25.000000 datastructuresLionelEric-1.0.7/datastructuresLionelEric.egg-info/dependency_links.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 21:58:25.000000 datastructuresLionelEric-1.0.7/datastructuresLionelEric.egg-info/top_level.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)       38 2023-04-09 21:58:25.700481 datastructuresLionelEric-1.0.7/setup.cfg
--rw-r--r--   0 lionelhasan   (501) staff       (20)      202 2023-04-09 21:58:24.000000 datastructuresLionelEric-1.0.7/setup.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:00:26.143598 datastructuresLionelEric-1.0.8/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-03-29 13:29:16.000000 datastructuresLionelEric-1.0.8/.DS_Store
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      215 2023-04-09 22:00:26.143412 datastructuresLionelEric-1.0.8/PKG-INFO
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:00:26.135681 datastructuresLionelEric-1.0.8/datastructures/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/.DS_Store
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:00:26.138342 datastructuresLionelEric-1.0.8/datastructures/Linear/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6914 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/CDLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     8735 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/CSLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6857 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/DLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1065 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/LLQueue.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1259 2023-04-08 22:50:35.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/LLStack.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     7718 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/SLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/__init__.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:00:26.139950 datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     4716 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/CDLL.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     5162 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/CSLL.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     4620 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/DLL.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1780 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/LLQueue.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     2365 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/LLStack.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     4657 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/SLL.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      177 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:00:26.140553 datastructuresLionelEric-1.0.8/datastructures/nodes/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/nodes/.DS_Store
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      116 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/nodes/Dnode.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1080 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/nodes/TNode.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.8/datastructures/nodes/__init__.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:00:26.141017 datastructuresLionelEric-1.0.8/datastructures/nodes/__pycache__/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      476 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/nodes/__pycache__/Dnode.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     2118 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/nodes/__pycache__/TNode.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      176 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/nodes/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:00:26.141467 datastructuresLionelEric-1.0.8/datastructures/trees/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6667 2023-04-09 21:33:54.000000 datastructuresLionelEric-1.0.8/datastructures/trees/AVL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     5584 2023-04-09 21:50:16.000000 datastructuresLionelEric-1.0.8/datastructures/trees/BST.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:00:26.142273 datastructuresLionelEric-1.0.8/datastructures/trees/__pycache__/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     3696 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/trees/__pycache__/AVL.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     3364 2023-04-09 21:50:17.000000 datastructuresLionelEric-1.0.8/datastructures/trees/__pycache__/BST.cpython-39.pyc
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      176 2023-04-09 21:43:58.000000 datastructuresLionelEric-1.0.8/datastructures/trees/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 22:00:26.143132 datastructuresLionelEric-1.0.8/datastructuresLionelEric.egg-info/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      215 2023-04-09 22:00:26.000000 datastructuresLionelEric-1.0.8/datastructuresLionelEric.egg-info/PKG-INFO
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1345 2023-04-09 22:00:26.000000 datastructuresLionelEric-1.0.8/datastructuresLionelEric.egg-info/SOURCES.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 22:00:26.000000 datastructuresLionelEric-1.0.8/datastructuresLionelEric.egg-info/dependency_links.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 22:00:26.000000 datastructuresLionelEric-1.0.8/datastructuresLionelEric.egg-info/top_level.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)       38 2023-04-09 22:00:26.143671 datastructuresLionelEric-1.0.8/setup.cfg
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      314 2023-04-09 21:59:45.000000 datastructuresLionelEric-1.0.8/setup.py
```

### Comparing `datastructuresLionelEric-1.0.7/.DS_Store` & `datastructuresLionelEric-1.0.8/.DS_Store`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.7/datastructures/.DS_Store` & `datastructuresLionelEric-1.0.8/datastructures/.DS_Store`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.7/datastructures/Linear/CDLL.py` & `datastructuresLionelEric-1.0.8/datastructures/Linear/CDLL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.7/datastructures/Linear/CSLL.py` & `datastructuresLionelEric-1.0.8/datastructures/Linear/CSLL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.7/datastructures/Linear/DLL.py` & `datastructuresLionelEric-1.0.8/datastructures/Linear/DLL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.7/datastructures/Linear/LLQueue.py` & `datastructuresLionelEric-1.0.8/datastructures/Linear/LLQueue.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.7/datastructures/Linear/LLStack.py` & `datastructuresLionelEric-1.0.8/datastructures/Linear/LLStack.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.7/datastructures/Linear/SLL.py` & `datastructuresLionelEric-1.0.8/datastructures/Linear/SLL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.7/datastructures/Linear/__pycache__/CDLL.cpython-39.pyc` & `datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/CDLL.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.7/datastructures/Linear/__pycache__/CSLL.cpython-39.pyc` & `datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/CSLL.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.7/datastructures/Linear/__pycache__/DLL.cpython-39.pyc` & `datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/DLL.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.7/datastructures/Linear/__pycache__/LLQueue.cpython-39.pyc` & `datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/LLQueue.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.7/datastructures/Linear/__pycache__/LLStack.cpython-39.pyc` & `datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/LLStack.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.7/datastructures/Linear/__pycache__/SLL.cpython-39.pyc` & `datastructuresLionelEric-1.0.8/datastructures/Linear/__pycache__/SLL.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.7/datastructures/nodes/.DS_Store` & `datastructuresLionelEric-1.0.8/datastructures/nodes/.DS_Store`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.7/datastructures/nodes/TNode.py` & `datastructuresLionelEric-1.0.8/datastructures/nodes/TNode.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.7/datastructures/nodes/__pycache__/TNode.cpython-39.pyc` & `datastructuresLionelEric-1.0.8/datastructures/nodes/__pycache__/TNode.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.7/datastructures/trees/AVL.py` & `datastructuresLionelEric-1.0.8/datastructures/trees/AVL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.7/datastructures/trees/BST.py` & `datastructuresLionelEric-1.0.8/datastructures/trees/BST.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.7/datastructures/trees/__pycache__/AVL.cpython-39.pyc` & `datastructuresLionelEric-1.0.8/datastructures/trees/__pycache__/AVL.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.7/datastructures/trees/__pycache__/BST.cpython-39.pyc` & `datastructuresLionelEric-1.0.8/datastructures/trees/__pycache__/BST.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.7/datastructuresLionelEric.egg-info/SOURCES.txt` & `datastructuresLionelEric-1.0.8/datastructuresLionelEric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

