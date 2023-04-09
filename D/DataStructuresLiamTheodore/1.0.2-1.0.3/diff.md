# Comparing `tmp/DataStructuresLiamTheodore-1.0.2.tar.gz` & `tmp/DataStructuresLiamTheodore-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DataStructuresLiamTheodore-1.0.2.tar", last modified: Sun Apr  9 19:55:47 2023, max compression
+gzip compressed data, was "DataStructuresLiamTheodore-1.0.3.tar", last modified: Sun Apr  9 20:00:17 2023, max compression
```

## Comparing `DataStructuresLiamTheodore-1.0.2.tar` & `DataStructuresLiamTheodore-1.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-09 19:55:47.520237 DataStructuresLiamTheodore-1.0.2/
-drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-09 19:55:47.513888 DataStructuresLiamTheodore-1.0.2/DataStructuresLiamTheodore.egg-info/
--rw-r--r--   0 liammah    (501) staff       (20)      219 2023-04-09 19:55:47.000000 DataStructuresLiamTheodore-1.0.2/DataStructuresLiamTheodore.egg-info/PKG-INFO
--rw-r--r--   0 liammah    (501) staff       (20)      695 2023-04-09 19:55:47.000000 DataStructuresLiamTheodore-1.0.2/DataStructuresLiamTheodore.egg-info/SOURCES.txt
--rw-r--r--   0 liammah    (501) staff       (20)        1 2023-04-09 19:55:47.000000 DataStructuresLiamTheodore-1.0.2/DataStructuresLiamTheodore.egg-info/dependency_links.txt
--rw-r--r--   0 liammah    (501) staff       (20)       15 2023-04-09 19:55:47.000000 DataStructuresLiamTheodore-1.0.2/DataStructuresLiamTheodore.egg-info/top_level.txt
--rw-r--r--   0 liammah    (501) staff       (20)      219 2023-04-09 19:55:47.520006 DataStructuresLiamTheodore-1.0.2/PKG-INFO
-drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-09 19:55:47.514091 DataStructuresLiamTheodore-1.0.2/datastructures/
-drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-09 19:55:47.516930 DataStructuresLiamTheodore-1.0.2/datastructures/Linear/
--rw-r--r--   0 liammah    (501) staff       (20)     4017 2023-04-09 02:22:21.000000 DataStructuresLiamTheodore-1.0.2/datastructures/Linear/DoublyCLL.py
--rw-r--r--   0 liammah    (501) staff       (20)     8425 2023-04-09 01:57:51.000000 DataStructuresLiamTheodore-1.0.2/datastructures/Linear/DoublyLL.py
--rw-r--r--   0 liammah    (501) staff       (20)     2172 2023-04-09 03:32:44.000000 DataStructuresLiamTheodore-1.0.2/datastructures/Linear/LLQueue.py
--rw-r--r--   0 liammah    (501) staff       (20)     1904 2023-04-07 16:54:07.000000 DataStructuresLiamTheodore-1.0.2/datastructures/Linear/LLStack.py
--rw-r--r--   0 liammah    (501) staff       (20)     3977 2023-04-09 03:41:36.000000 DataStructuresLiamTheodore-1.0.2/datastructures/Linear/SinglyCLL.py
--rw-r--r--   0 liammah    (501) staff       (20)     7251 2023-04-07 23:11:54.000000 DataStructuresLiamTheodore-1.0.2/datastructures/Linear/SinglyLL.py
--rw-r--r--   0 liammah    (501) staff       (20)      227 2023-04-09 19:27:46.000000 DataStructuresLiamTheodore-1.0.2/datastructures/Linear/__init__.py
-drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-09 19:55:47.518432 DataStructuresLiamTheodore-1.0.2/datastructures/Nodes/
--rw-r--r--   0 liammah    (501) staff       (20)      117 2023-04-07 16:52:52.000000 DataStructuresLiamTheodore-1.0.2/datastructures/Nodes/DoublyNode.py
--rw-r--r--   0 liammah    (501) staff       (20)      100 2023-04-07 16:52:52.000000 DataStructuresLiamTheodore-1.0.2/datastructures/Nodes/SinglyNode.py
--rw-r--r--   0 liammah    (501) staff       (20)     1754 2023-04-09 06:13:40.000000 DataStructuresLiamTheodore-1.0.2/datastructures/Nodes/TNode.py
--rw-r--r--   0 liammah    (501) staff       (20)      227 2023-04-09 19:27:42.000000 DataStructuresLiamTheodore-1.0.2/datastructures/Nodes/__init__.py
-drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-09 19:55:47.519545 DataStructuresLiamTheodore-1.0.2/datastructures/Trees/
--rw-r--r--   0 liammah    (501) staff       (20)     8558 2023-04-09 06:13:40.000000 DataStructuresLiamTheodore-1.0.2/datastructures/Trees/AVL.py
--rw-r--r--   0 liammah    (501) staff       (20)     4797 2023-04-09 06:13:40.000000 DataStructuresLiamTheodore-1.0.2/datastructures/Trees/BST.py
--rw-r--r--   0 liammah    (501) staff       (20)      227 2023-04-09 19:27:51.000000 DataStructuresLiamTheodore-1.0.2/datastructures/Trees/__init__.py
--rw-r--r--   0 liammah    (501) staff       (20)        0 2023-04-09 19:39:37.000000 DataStructuresLiamTheodore-1.0.2/datastructures/__init__.py
--rw-r--r--   0 liammah    (501) staff       (20)       38 2023-04-09 19:55:47.520315 DataStructuresLiamTheodore-1.0.2/setup.cfg
--rw-r--r--   0 liammah    (501) staff       (20)      333 2023-04-09 19:55:43.000000 DataStructuresLiamTheodore-1.0.2/setup.py
+drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-09 20:00:17.529102 DataStructuresLiamTheodore-1.0.3/
+drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-09 20:00:17.523437 DataStructuresLiamTheodore-1.0.3/DataStructuresLiamTheodore.egg-info/
+-rw-r--r--   0 liammah    (501) staff       (20)      219 2023-04-09 20:00:17.000000 DataStructuresLiamTheodore-1.0.3/DataStructuresLiamTheodore.egg-info/PKG-INFO
+-rw-r--r--   0 liammah    (501) staff       (20)      695 2023-04-09 20:00:17.000000 DataStructuresLiamTheodore-1.0.3/DataStructuresLiamTheodore.egg-info/SOURCES.txt
+-rw-r--r--   0 liammah    (501) staff       (20)        1 2023-04-09 20:00:17.000000 DataStructuresLiamTheodore-1.0.3/DataStructuresLiamTheodore.egg-info/dependency_links.txt
+-rw-r--r--   0 liammah    (501) staff       (20)       15 2023-04-09 20:00:17.000000 DataStructuresLiamTheodore-1.0.3/DataStructuresLiamTheodore.egg-info/top_level.txt
+-rw-r--r--   0 liammah    (501) staff       (20)      219 2023-04-09 20:00:17.528876 DataStructuresLiamTheodore-1.0.3/PKG-INFO
+drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-09 20:00:17.523695 DataStructuresLiamTheodore-1.0.3/datastructures/
+drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-09 20:00:17.526359 DataStructuresLiamTheodore-1.0.3/datastructures/Linear/
+-rw-r--r--   0 liammah    (501) staff       (20)     4017 2023-04-09 02:22:21.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Linear/DoublyCLL.py
+-rw-r--r--   0 liammah    (501) staff       (20)     8425 2023-04-09 01:57:51.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Linear/DoublyLL.py
+-rw-r--r--   0 liammah    (501) staff       (20)     2172 2023-04-09 03:32:44.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Linear/LLQueue.py
+-rw-r--r--   0 liammah    (501) staff       (20)     1904 2023-04-07 16:54:07.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Linear/LLStack.py
+-rw-r--r--   0 liammah    (501) staff       (20)     3977 2023-04-09 03:41:36.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Linear/SinglyCLL.py
+-rw-r--r--   0 liammah    (501) staff       (20)     7251 2023-04-07 23:11:54.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Linear/SinglyLL.py
+-rw-r--r--   0 liammah    (501) staff       (20)        0 2023-04-09 19:59:08.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Linear/__init__.py
+drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-09 20:00:17.527712 DataStructuresLiamTheodore-1.0.3/datastructures/Nodes/
+-rw-r--r--   0 liammah    (501) staff       (20)      117 2023-04-07 16:52:52.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Nodes/DoublyNode.py
+-rw-r--r--   0 liammah    (501) staff       (20)      100 2023-04-07 16:52:52.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Nodes/SinglyNode.py
+-rw-r--r--   0 liammah    (501) staff       (20)     1754 2023-04-09 06:13:40.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Nodes/TNode.py
+-rw-r--r--   0 liammah    (501) staff       (20)        0 2023-04-09 19:58:49.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Nodes/__init__.py
+drwxr-xr-x   0 liammah    (501) staff       (20)        0 2023-04-09 20:00:17.528574 DataStructuresLiamTheodore-1.0.3/datastructures/Trees/
+-rw-r--r--   0 liammah    (501) staff       (20)     8558 2023-04-09 06:13:40.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Trees/AVL.py
+-rw-r--r--   0 liammah    (501) staff       (20)     4797 2023-04-09 06:13:40.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Trees/BST.py
+-rw-r--r--   0 liammah    (501) staff       (20)        0 2023-04-09 19:59:44.000000 DataStructuresLiamTheodore-1.0.3/datastructures/Trees/__init__.py
+-rw-r--r--   0 liammah    (501) staff       (20)        0 2023-04-09 19:39:37.000000 DataStructuresLiamTheodore-1.0.3/datastructures/__init__.py
+-rw-r--r--   0 liammah    (501) staff       (20)       38 2023-04-09 20:00:17.529183 DataStructuresLiamTheodore-1.0.3/setup.cfg
+-rw-r--r--   0 liammah    (501) staff       (20)      333 2023-04-09 20:00:07.000000 DataStructuresLiamTheodore-1.0.3/setup.py
```

### Comparing `DataStructuresLiamTheodore-1.0.2/DataStructuresLiamTheodore.egg-info/SOURCES.txt` & `DataStructuresLiamTheodore-1.0.3/DataStructuresLiamTheodore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DataStructuresLiamTheodore-1.0.2/datastructures/Linear/DoublyCLL.py` & `DataStructuresLiamTheodore-1.0.3/datastructures/Linear/DoublyCLL.py`

 * *Files identical despite different names*

### Comparing `DataStructuresLiamTheodore-1.0.2/datastructures/Linear/DoublyLL.py` & `DataStructuresLiamTheodore-1.0.3/datastructures/Linear/DoublyLL.py`

 * *Files identical despite different names*

### Comparing `DataStructuresLiamTheodore-1.0.2/datastructures/Linear/LLQueue.py` & `DataStructuresLiamTheodore-1.0.3/datastructures/Linear/LLQueue.py`

 * *Files identical despite different names*

### Comparing `DataStructuresLiamTheodore-1.0.2/datastructures/Linear/LLStack.py` & `DataStructuresLiamTheodore-1.0.3/datastructures/Linear/LLStack.py`

 * *Files identical despite different names*

### Comparing `DataStructuresLiamTheodore-1.0.2/datastructures/Linear/SinglyCLL.py` & `DataStructuresLiamTheodore-1.0.3/datastructures/Linear/SinglyCLL.py`

 * *Files identical despite different names*

### Comparing `DataStructuresLiamTheodore-1.0.2/datastructures/Linear/SinglyLL.py` & `DataStructuresLiamTheodore-1.0.3/datastructures/Linear/SinglyLL.py`

 * *Files identical despite different names*

### Comparing `DataStructuresLiamTheodore-1.0.2/datastructures/Nodes/TNode.py` & `DataStructuresLiamTheodore-1.0.3/datastructures/Nodes/TNode.py`

 * *Files identical despite different names*

### Comparing `DataStructuresLiamTheodore-1.0.2/datastructures/Trees/AVL.py` & `DataStructuresLiamTheodore-1.0.3/datastructures/Trees/AVL.py`

 * *Files identical despite different names*

### Comparing `DataStructuresLiamTheodore-1.0.2/datastructures/Trees/BST.py` & `DataStructuresLiamTheodore-1.0.3/datastructures/Trees/BST.py`

 * *Files identical despite different names*

