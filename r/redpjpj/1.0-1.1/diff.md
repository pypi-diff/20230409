# Comparing `tmp/redpjpj-1.0.tar.gz` & `tmp/redpjpj-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redpjpj-1.0.tar", last modified: Sun Apr  9 19:31:43 2023, max compression
+gzip compressed data, was "redpjpj-1.1.tar", last modified: Sun Apr  9 19:48:17 2023, max compression
```

## Comparing `redpjpj-1.0.tar` & `redpjpj-1.1.tar`

### file list

```diff
@@ -1,38 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 19:31:43.674551 redpjpj-1.0/
--rw-rw-rw-   0        0        0      112 2023-04-09 19:31:43.674551 redpjpj-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-09 19:31:43.583904 redpjpj-1.0/myPackage/
-drwxrwxrwx   0        0        0        0 2023-04-09 19:31:43.612042 redpjpj-1.0/myPackage/Linear/
--rw-rw-rw-   0        0        0     4154 2023-04-09 06:11:13.000000 redpjpj-1.0/myPackage/Linear/DoublyCLL.py
--rw-rw-rw-   0        0        0     8673 2023-04-09 06:11:13.000000 redpjpj-1.0/myPackage/Linear/DoublyLL.py
--rw-rw-rw-   0        0        0     2272 2023-04-09 06:11:13.000000 redpjpj-1.0/myPackage/Linear/LLQueue.py
--rw-rw-rw-   0        0        0     1981 2023-04-08 00:28:46.000000 redpjpj-1.0/myPackage/Linear/LLStack.py
--rw-rw-rw-   0        0        0     4109 2023-04-09 06:11:13.000000 redpjpj-1.0/myPackage/Linear/SinglyCLL.py
--rw-rw-rw-   0        0        0     7497 2023-04-08 00:28:46.000000 redpjpj-1.0/myPackage/Linear/SinglyLL.py
--rw-rw-rw-   0        0        0        0 2023-04-09 17:18:02.000000 redpjpj-1.0/myPackage/Linear/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 19:31:43.612042 redpjpj-1.0/myPackage/Nodes/
--rw-rw-rw-   0        0        0      122 2023-04-07 16:51:25.000000 redpjpj-1.0/myPackage/Nodes/DoublyNode.py
--rw-rw-rw-   0        0        0      105 2023-04-07 16:51:25.000000 redpjpj-1.0/myPackage/Nodes/SinglyNode.py
--rw-rw-rw-   0        0        0     1813 2023-04-09 06:11:17.000000 redpjpj-1.0/myPackage/Nodes/TNode.py
--rw-rw-rw-   0        0        0        0 2023-04-09 17:18:02.000000 redpjpj-1.0/myPackage/Nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 19:31:43.627672 redpjpj-1.0/myPackage/Trees/
--rw-rw-rw-   0        0        0     8802 2023-04-09 06:11:17.000000 redpjpj-1.0/myPackage/Trees/AVL.py
--rw-rw-rw-   0        0        0     4950 2023-04-09 06:11:17.000000 redpjpj-1.0/myPackage/Trees/BST.py
--rw-rw-rw-   0        0        0        0 2023-04-09 17:18:02.000000 redpjpj-1.0/myPackage/Trees/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-09 17:18:02.000000 redpjpj-1.0/myPackage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 19:31:43.643300 redpjpj-1.0/myPackage/test/
--rw-rw-rw-   0        0        0    10058 2023-04-09 17:14:55.000000 redpjpj-1.0/myPackage/test/AVL_test.py
--rw-rw-rw-   0        0        0     4790 2023-04-09 06:11:13.000000 redpjpj-1.0/myPackage/test/BST_test.py
--rw-rw-rw-   0        0        0     5959 2023-04-09 06:11:13.000000 redpjpj-1.0/myPackage/test/DoublyCLL_test.py
--rw-rw-rw-   0        0        0     4900 2023-04-09 06:11:13.000000 redpjpj-1.0/myPackage/test/DoublyLL_test.py
--rw-rw-rw-   0        0        0     3937 2023-04-09 06:11:13.000000 redpjpj-1.0/myPackage/test/LLQueue_test.py
--rw-rw-rw-   0        0        0     4010 2023-04-09 06:11:13.000000 redpjpj-1.0/myPackage/test/LLStack_test.py
--rw-rw-rw-   0        0        0     5679 2023-04-09 06:11:13.000000 redpjpj-1.0/myPackage/test/SinglyCLL_test.py
--rw-rw-rw-   0        0        0     5820 2023-04-09 06:11:13.000000 redpjpj-1.0/myPackage/test/SinglyLL_test.py
--rw-rw-rw-   0        0        0        0 2023-04-09 17:18:02.000000 redpjpj-1.0/myPackage/test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 19:31:43.674551 redpjpj-1.0/redpjpj.egg-info/
--rw-rw-rw-   0        0        0      112 2023-04-09 19:31:43.000000 redpjpj-1.0/redpjpj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      817 2023-04-09 19:31:43.000000 redpjpj-1.0/redpjpj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 19:31:43.000000 redpjpj-1.0/redpjpj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-09 19:31:43.000000 redpjpj-1.0/redpjpj.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 19:31:43.690176 redpjpj-1.0/setup.cfg
--rw-rw-rw-   0        0        0      261 2023-04-09 19:31:32.000000 redpjpj-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 19:48:17.978603 redpjpj-1.1/
+drwxrwxrwx   0        0        0        0 2023-04-09 19:48:17.916100 redpjpj-1.1/Linear/
+-rw-rw-rw-   0        0        0     4154 2023-04-09 06:11:13.000000 redpjpj-1.1/Linear/DoublyCLL.py
+-rw-rw-rw-   0        0        0     8673 2023-04-09 06:11:13.000000 redpjpj-1.1/Linear/DoublyLL.py
+-rw-rw-rw-   0        0        0     2272 2023-04-09 06:11:13.000000 redpjpj-1.1/Linear/LLQueue.py
+-rw-rw-rw-   0        0        0     1981 2023-04-08 00:28:46.000000 redpjpj-1.1/Linear/LLStack.py
+-rw-rw-rw-   0        0        0     4109 2023-04-09 06:11:13.000000 redpjpj-1.1/Linear/SinglyCLL.py
+-rw-rw-rw-   0        0        0     7497 2023-04-08 00:28:46.000000 redpjpj-1.1/Linear/SinglyLL.py
+-rw-rw-rw-   0        0        0        0 2023-04-09 17:18:02.000000 redpjpj-1.1/Linear/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 19:48:17.931737 redpjpj-1.1/Nodes/
+-rw-rw-rw-   0        0        0      122 2023-04-07 16:51:25.000000 redpjpj-1.1/Nodes/DoublyNode.py
+-rw-rw-rw-   0        0        0      105 2023-04-07 16:51:25.000000 redpjpj-1.1/Nodes/SinglyNode.py
+-rw-rw-rw-   0        0        0     1813 2023-04-09 06:11:17.000000 redpjpj-1.1/Nodes/TNode.py
+-rw-rw-rw-   0        0        0        0 2023-04-09 17:18:02.000000 redpjpj-1.1/Nodes/__init__.py
+-rw-rw-rw-   0        0        0      112 2023-04-09 19:48:17.978603 redpjpj-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-09 19:48:17.931737 redpjpj-1.1/Trees/
+-rw-rw-rw-   0        0        0     8802 2023-04-09 06:11:17.000000 redpjpj-1.1/Trees/AVL.py
+-rw-rw-rw-   0        0        0     4950 2023-04-09 06:11:17.000000 redpjpj-1.1/Trees/BST.py
+-rw-rw-rw-   0        0        0        0 2023-04-09 17:18:02.000000 redpjpj-1.1/Trees/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 19:48:17.947367 redpjpj-1.1/redpjpj.egg-info/
+-rw-rw-rw-   0        0        0      112 2023-04-09 19:48:17.000000 redpjpj-1.1/redpjpj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      565 2023-04-09 19:48:17.000000 redpjpj-1.1/redpjpj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 19:48:17.000000 redpjpj-1.1/redpjpj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-09 19:48:17.000000 redpjpj-1.1/redpjpj.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 19:48:17.978603 redpjpj-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      261 2023-04-09 19:45:41.000000 redpjpj-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 19:48:17.978603 redpjpj-1.1/test/
+-rw-rw-rw-   0        0        0    10058 2023-04-09 17:14:55.000000 redpjpj-1.1/test/AVL_test.py
+-rw-rw-rw-   0        0        0     4790 2023-04-09 06:11:13.000000 redpjpj-1.1/test/BST_test.py
+-rw-rw-rw-   0        0        0     5959 2023-04-09 06:11:13.000000 redpjpj-1.1/test/DoublyCLL_test.py
+-rw-rw-rw-   0        0        0     4900 2023-04-09 06:11:13.000000 redpjpj-1.1/test/DoublyLL_test.py
+-rw-rw-rw-   0        0        0     3937 2023-04-09 06:11:13.000000 redpjpj-1.1/test/LLQueue_test.py
+-rw-rw-rw-   0        0        0     4010 2023-04-09 06:11:13.000000 redpjpj-1.1/test/LLStack_test.py
+-rw-rw-rw-   0        0        0     5679 2023-04-09 06:11:13.000000 redpjpj-1.1/test/SinglyCLL_test.py
+-rw-rw-rw-   0        0        0     5820 2023-04-09 06:11:13.000000 redpjpj-1.1/test/SinglyLL_test.py
+-rw-rw-rw-   0        0        0        0 2023-04-09 17:18:02.000000 redpjpj-1.1/test/__init__.py
```

### Comparing `redpjpj-1.0/myPackage/Linear/DoublyCLL.py` & `redpjpj-1.1/Linear/DoublyCLL.py`

 * *Files identical despite different names*

### Comparing `redpjpj-1.0/myPackage/Linear/DoublyLL.py` & `redpjpj-1.1/Linear/DoublyLL.py`

 * *Files identical despite different names*

### Comparing `redpjpj-1.0/myPackage/Linear/LLQueue.py` & `redpjpj-1.1/Linear/LLQueue.py`

 * *Files identical despite different names*

### Comparing `redpjpj-1.0/myPackage/Linear/LLStack.py` & `redpjpj-1.1/Linear/LLStack.py`

 * *Files identical despite different names*

### Comparing `redpjpj-1.0/myPackage/Linear/SinglyCLL.py` & `redpjpj-1.1/Linear/SinglyCLL.py`

 * *Files identical despite different names*

### Comparing `redpjpj-1.0/myPackage/Linear/SinglyLL.py` & `redpjpj-1.1/Linear/SinglyLL.py`

 * *Files identical despite different names*

### Comparing `redpjpj-1.0/myPackage/Nodes/TNode.py` & `redpjpj-1.1/Nodes/TNode.py`

 * *Files identical despite different names*

### Comparing `redpjpj-1.0/myPackage/Trees/AVL.py` & `redpjpj-1.1/Trees/AVL.py`

 * *Files identical despite different names*

### Comparing `redpjpj-1.0/myPackage/Trees/BST.py` & `redpjpj-1.1/Trees/BST.py`

 * *Files identical despite different names*

### Comparing `redpjpj-1.0/myPackage/test/AVL_test.py` & `redpjpj-1.1/test/AVL_test.py`

 * *Files identical despite different names*

### Comparing `redpjpj-1.0/myPackage/test/BST_test.py` & `redpjpj-1.1/test/BST_test.py`

 * *Files identical despite different names*

### Comparing `redpjpj-1.0/myPackage/test/DoublyCLL_test.py` & `redpjpj-1.1/test/DoublyCLL_test.py`

 * *Files identical despite different names*

### Comparing `redpjpj-1.0/myPackage/test/DoublyLL_test.py` & `redpjpj-1.1/test/DoublyLL_test.py`

 * *Files identical despite different names*

### Comparing `redpjpj-1.0/myPackage/test/LLQueue_test.py` & `redpjpj-1.1/test/LLQueue_test.py`

 * *Files identical despite different names*

### Comparing `redpjpj-1.0/myPackage/test/LLStack_test.py` & `redpjpj-1.1/test/LLStack_test.py`

 * *Files identical despite different names*

### Comparing `redpjpj-1.0/myPackage/test/SinglyCLL_test.py` & `redpjpj-1.1/test/SinglyCLL_test.py`

 * *Files identical despite different names*

### Comparing `redpjpj-1.0/myPackage/test/SinglyLL_test.py` & `redpjpj-1.1/test/SinglyLL_test.py`

 * *Files identical despite different names*

