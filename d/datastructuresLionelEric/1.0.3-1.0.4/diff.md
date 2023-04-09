# Comparing `tmp/datastructuresLionelEric-1.0.3.tar.gz` & `tmp/datastructuresLionelEric-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datastructuresLionelEric-1.0.3.tar", last modified: Sun Apr  9 21:34:38 2023, max compression
+gzip compressed data, was "datastructuresLionelEric-1.0.4.tar", last modified: Sun Apr  9 21:43:57 2023, max compression
```

## Comparing `datastructuresLionelEric-1.0.3.tar` & `datastructuresLionelEric-1.0.4.tar`

### file list

```diff
@@ -1,58 +1,29 @@
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:34:38.361388 datastructuresLionelEric-1.0.3/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-03-29 13:29:16.000000 datastructuresLionelEric-1.0.3/.DS_Store
--rw-r--r--   0 lionelhasan   (501) staff       (20)      215 2023-04-09 21:34:38.361088 datastructuresLionelEric-1.0.3/PKG-INFO
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:34:38.350320 datastructuresLionelEric-1.0.3/datastructures/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/.DS_Store
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:34:38.353096 datastructuresLionelEric-1.0.3/datastructures/Linear/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6914 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/Linear/CDLL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     8735 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/Linear/CSLL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6857 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/Linear/DLL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     1065 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/Linear/LLQueue.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     1259 2023-04-08 22:50:35.000000 datastructuresLionelEric-1.0.3/datastructures/Linear/LLStack.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     7718 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/Linear/SLL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/Linear/__init__.py
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:34:38.356270 datastructuresLionelEric-1.0.3/datastructures/Linear/__pycache__/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     8979 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/Linear/__pycache__/CDLL.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     4716 2023-04-08 22:47:46.000000 datastructuresLionelEric-1.0.3/datastructures/Linear/__pycache__/CDLL.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     9916 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/Linear/__pycache__/CSLL.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     5162 2023-04-08 22:47:46.000000 datastructuresLionelEric-1.0.3/datastructures/Linear/__pycache__/CSLL.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     8342 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/Linear/__pycache__/DLL.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     4620 2023-04-08 22:47:46.000000 datastructuresLionelEric-1.0.3/datastructures/Linear/__pycache__/DLL.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     2516 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/Linear/__pycache__/LLQueue.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     1780 2023-04-08 22:47:46.000000 datastructuresLionelEric-1.0.3/datastructures/Linear/__pycache__/LLQueue.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     3403 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/Linear/__pycache__/LLStack.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     2365 2023-04-08 22:50:36.000000 datastructuresLionelEric-1.0.3/datastructures/Linear/__pycache__/LLStack.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     8307 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/Linear/__pycache__/SLL.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     4657 2023-04-08 22:47:46.000000 datastructuresLionelEric-1.0.3/datastructures/Linear/__pycache__/SLL.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)      199 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/Linear/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)      177 2023-04-08 22:47:46.000000 datastructuresLionelEric-1.0.3/datastructures/Linear/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:34:38.357024 datastructuresLionelEric-1.0.3/datastructures/nodes/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/nodes/.DS_Store
--rw-r--r--   0 lionelhasan   (501) staff       (20)      116 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/nodes/Dnode.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     1080 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/nodes/TNode.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/nodes/__init__.py
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:34:38.358106 datastructuresLionelEric-1.0.3/datastructures/nodes/__pycache__/
--rw-r--r--   0 lionelhasan   (501) staff       (20)      629 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/nodes/__pycache__/Dnode.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)      476 2023-04-08 22:47:46.000000 datastructuresLionelEric-1.0.3/datastructures/nodes/__pycache__/Dnode.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     2706 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/nodes/__pycache__/TNode.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     2118 2023-04-08 22:48:38.000000 datastructuresLionelEric-1.0.3/datastructures/nodes/__pycache__/TNode.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)      198 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/nodes/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)      176 2023-04-08 22:47:46.000000 datastructuresLionelEric-1.0.3/datastructures/nodes/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:34:38.358684 datastructuresLionelEric-1.0.3/datastructures/trees/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6667 2023-04-09 21:33:54.000000 datastructuresLionelEric-1.0.3/datastructures/trees/AVL.py
--rw-r--r--   0 lionelhasan   (501) staff       (20)     5584 2023-04-09 21:33:39.000000 datastructuresLionelEric-1.0.3/datastructures/trees/BST.py
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:34:38.359831 datastructuresLionelEric-1.0.3/datastructures/trees/__pycache__/
--rw-r--r--   0 lionelhasan   (501) staff       (20)     5386 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/trees/__pycache__/AVL.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     3696 2023-04-09 21:33:54.000000 datastructuresLionelEric-1.0.3/datastructures/trees/__pycache__/AVL.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     6289 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/trees/__pycache__/BST.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     3364 2023-04-09 21:33:54.000000 datastructuresLionelEric-1.0.3/datastructures/trees/__pycache__/BST.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)      198 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.3/datastructures/trees/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)      176 2023-04-09 21:33:54.000000 datastructuresLionelEric-1.0.3/datastructures/trees/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 lionelhasan   (501) staff       (20)     2809 2023-04-09 21:33:37.000000 datastructuresLionelEric-1.0.3/datastructures/trees/main.py
-drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:34:38.360549 datastructuresLionelEric-1.0.3/datastructuresLionelEric.egg-info/
--rw-r--r--   0 lionelhasan   (501) staff       (20)      215 2023-04-09 21:34:38.000000 datastructuresLionelEric-1.0.3/datastructuresLionelEric.egg-info/PKG-INFO
--rw-r--r--   0 lionelhasan   (501) staff       (20)     2099 2023-04-09 21:34:38.000000 datastructuresLionelEric-1.0.3/datastructuresLionelEric.egg-info/SOURCES.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 21:34:38.000000 datastructuresLionelEric-1.0.3/datastructuresLionelEric.egg-info/dependency_links.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 21:34:38.000000 datastructuresLionelEric-1.0.3/datastructuresLionelEric.egg-info/top_level.txt
--rw-r--r--   0 lionelhasan   (501) staff       (20)       38 2023-04-09 21:34:38.361446 datastructuresLionelEric-1.0.3/setup.cfg
--rw-r--r--   0 lionelhasan   (501) staff       (20)      314 2023-04-09 21:32:06.000000 datastructuresLionelEric-1.0.3/setup.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:43:57.454330 datastructuresLionelEric-1.0.4/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-03-29 13:29:16.000000 datastructuresLionelEric-1.0.4/.DS_Store
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      215 2023-04-09 21:43:57.454151 datastructuresLionelEric-1.0.4/PKG-INFO
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:43:57.451410 datastructuresLionelEric-1.0.4/datastructures/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.4/datastructures/.DS_Store
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:43:57.452365 datastructuresLionelEric-1.0.4/datastructures/Linear/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6914 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.4/datastructures/Linear/CDLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     8735 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.4/datastructures/Linear/CSLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6857 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.4/datastructures/Linear/DLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1065 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.4/datastructures/Linear/LLQueue.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1259 2023-04-08 22:50:35.000000 datastructuresLionelEric-1.0.4/datastructures/Linear/LLStack.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     7718 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.4/datastructures/Linear/SLL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.4/datastructures/Linear/__init__.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:43:57.452915 datastructuresLionelEric-1.0.4/datastructures/nodes/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6148 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.4/datastructures/nodes/.DS_Store
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      116 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.4/datastructures/nodes/Dnode.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     1080 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.4/datastructures/nodes/TNode.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        0 2023-04-08 22:45:52.000000 datastructuresLionelEric-1.0.4/datastructures/nodes/__init__.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:43:57.453392 datastructuresLionelEric-1.0.4/datastructures/trees/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     6667 2023-04-09 21:33:54.000000 datastructuresLionelEric-1.0.4/datastructures/trees/AVL.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     5584 2023-04-09 21:33:39.000000 datastructuresLionelEric-1.0.4/datastructures/trees/BST.py
+-rw-r--r--   0 lionelhasan   (501) staff       (20)     2809 2023-04-09 21:33:37.000000 datastructuresLionelEric-1.0.4/datastructures/trees/main.py
+drwxr-xr-x   0 lionelhasan   (501) staff       (20)        0 2023-04-09 21:43:57.453924 datastructuresLionelEric-1.0.4/datastructuresLionelEric.egg-info/
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      215 2023-04-09 21:43:57.000000 datastructuresLionelEric-1.0.4/datastructuresLionelEric.egg-info/PKG-INFO
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      662 2023-04-09 21:43:57.000000 datastructuresLionelEric-1.0.4/datastructuresLionelEric.egg-info/SOURCES.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 21:43:57.000000 datastructuresLionelEric-1.0.4/datastructuresLionelEric.egg-info/dependency_links.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)        1 2023-04-09 21:43:57.000000 datastructuresLionelEric-1.0.4/datastructuresLionelEric.egg-info/top_level.txt
+-rw-r--r--   0 lionelhasan   (501) staff       (20)       38 2023-04-09 21:43:57.454494 datastructuresLionelEric-1.0.4/setup.cfg
+-rw-r--r--   0 lionelhasan   (501) staff       (20)      314 2023-04-09 21:41:46.000000 datastructuresLionelEric-1.0.4/setup.py
```

### Comparing `datastructuresLionelEric-1.0.3/.DS_Store` & `datastructuresLionelEric-1.0.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.3/datastructures/.DS_Store` & `datastructuresLionelEric-1.0.4/datastructures/.DS_Store`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.3/datastructures/Linear/CDLL.py` & `datastructuresLionelEric-1.0.4/datastructures/Linear/CDLL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.3/datastructures/Linear/CSLL.py` & `datastructuresLionelEric-1.0.4/datastructures/Linear/CSLL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.3/datastructures/Linear/DLL.py` & `datastructuresLionelEric-1.0.4/datastructures/Linear/DLL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.3/datastructures/Linear/LLQueue.py` & `datastructuresLionelEric-1.0.4/datastructures/Linear/LLQueue.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.3/datastructures/Linear/LLStack.py` & `datastructuresLionelEric-1.0.4/datastructures/Linear/LLStack.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.3/datastructures/Linear/SLL.py` & `datastructuresLionelEric-1.0.4/datastructures/Linear/SLL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.3/datastructures/nodes/.DS_Store` & `datastructuresLionelEric-1.0.4/datastructures/nodes/.DS_Store`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.3/datastructures/nodes/TNode.py` & `datastructuresLionelEric-1.0.4/datastructures/nodes/TNode.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.3/datastructures/trees/AVL.py` & `datastructuresLionelEric-1.0.4/datastructures/trees/AVL.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.3/datastructures/trees/BST.py` & `datastructuresLionelEric-1.0.4/datastructures/trees/BST.py`

 * *Files identical despite different names*

### Comparing `datastructuresLionelEric-1.0.3/datastructures/trees/main.py` & `datastructuresLionelEric-1.0.4/datastructures/trees/main.py`

 * *Files identical despite different names*

