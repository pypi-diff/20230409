# Comparing `tmp/tf-gnns-0.1.5a1.tar.gz` & `tmp/tf-gnns-0.1.5a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf-gnns-0.1.5a1.tar", last modified: Sun Apr  9 18:24:59 2023, max compression
+gzip compressed data, was "tf-gnns-0.1.5a2.tar", last modified: Sun Apr  9 18:59:57 2023, max compression
```

## Comparing `tf-gnns-0.1.5a1.tar` & `tf-gnns-0.1.5a2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:24:59.171147 tf-gnns-0.1.5a1/
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    11347 2023-04-09 18:24:58.000000 tf-gnns-0.1.5a1/LICENSE
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     3654 2023-04-09 18:24:59.171147 tf-gnns-0.1.5a1/PKG-INFO
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     3141 2023-04-09 18:24:58.000000 tf-gnns-0.1.5a1/README.md
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)       38 2023-04-09 18:24:59.171147 tf-gnns-0.1.5a1/setup.cfg
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     1024 2023-04-09 18:24:58.000000 tf-gnns-0.1.5a1/setup.py
-drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:24:59.171147 tf-gnns-0.1.5a1/tf_gnns/
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      839 2023-04-09 18:24:58.000000 tf-gnns-0.1.5a1/tf_gnns/__init__.py
-drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:24:59.171147 tf-gnns-0.1.5a1/tf_gnns/assets/
-drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:24:59.171147 tf-gnns-0.1.5a1/tf_gnns/assets/html_css/
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      557 2023-04-09 18:24:58.000000 tf-gnns-0.1.5a1/tf_gnns/assets/html_css/accordion.js
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      658 2023-04-09 18:24:58.000000 tf-gnns-0.1.5a1/tf_gnns/assets/html_css/pretty_print_accordion.css
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    18665 2023-04-09 18:24:58.000000 tf-gnns-0.1.5a1/tf_gnns/datastructures.py
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    82736 2023-04-09 18:24:58.000000 tf-gnns-0.1.5a1/tf_gnns/graphnet_utils.py
-drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:24:59.171147 tf-gnns-0.1.5a1/tf_gnns/lib/
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:24:58.000000 tf-gnns-0.1.5a1/tf_gnns/lib/__init__.py
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     4148 2023-04-09 18:24:58.000000 tf-gnns-0.1.5a1/tf_gnns/lib/gt_ops.py
-drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:24:59.171147 tf-gnns-0.1.5a1/tf_gnns/models/
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:24:58.000000 tf-gnns-0.1.5a1/tf_gnns/models/__init__.py
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    16947 2023-04-09 18:24:58.000000 tf-gnns-0.1.5a1/tf_gnns/models/graphnet.py
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     8155 2023-04-09 18:24:58.000000 tf-gnns-0.1.5a1/tf_gnns/utils.py
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     2259 2023-04-09 18:24:58.000000 tf-gnns-0.1.5a1/tf_gnns/utils_train.py
-drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:24:59.171147 tf-gnns-0.1.5a1/tf_gnns.egg-info/
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     3654 2023-04-09 18:24:59.000000 tf-gnns-0.1.5a1/tf_gnns.egg-info/PKG-INFO
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      450 2023-04-09 18:24:59.000000 tf-gnns-0.1.5a1/tf_gnns.egg-info/SOURCES.txt
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        1 2023-04-09 18:24:59.000000 tf-gnns-0.1.5a1/tf_gnns.egg-info/dependency_links.txt
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        8 2023-04-09 18:24:59.000000 tf-gnns-0.1.5a1/tf_gnns.egg-info/top_level.txt
+drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:59:57.953835 tf-gnns-0.1.5a2/
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    11347 2023-04-09 18:59:57.000000 tf-gnns-0.1.5a2/LICENSE
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     3654 2023-04-09 18:59:57.953835 tf-gnns-0.1.5a2/PKG-INFO
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     3141 2023-04-09 18:59:57.000000 tf-gnns-0.1.5a2/README.md
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)       38 2023-04-09 18:59:57.953835 tf-gnns-0.1.5a2/setup.cfg
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     1024 2023-04-09 18:59:57.000000 tf-gnns-0.1.5a2/setup.py
+drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:59:57.949835 tf-gnns-0.1.5a2/tf_gnns/
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      839 2023-04-09 18:59:57.000000 tf-gnns-0.1.5a2/tf_gnns/__init__.py
+drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:59:57.949835 tf-gnns-0.1.5a2/tf_gnns/assets/
+drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:59:57.953835 tf-gnns-0.1.5a2/tf_gnns/assets/html_css/
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      557 2023-04-09 18:59:57.000000 tf-gnns-0.1.5a2/tf_gnns/assets/html_css/accordion.js
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      658 2023-04-09 18:59:57.000000 tf-gnns-0.1.5a2/tf_gnns/assets/html_css/pretty_print_accordion.css
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    18665 2023-04-09 18:59:57.000000 tf-gnns-0.1.5a2/tf_gnns/datastructures.py
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    82736 2023-04-09 18:59:57.000000 tf-gnns-0.1.5a2/tf_gnns/graphnet_utils.py
+drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:59:57.953835 tf-gnns-0.1.5a2/tf_gnns/lib/
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:59:57.000000 tf-gnns-0.1.5a2/tf_gnns/lib/__init__.py
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     4148 2023-04-09 18:59:57.000000 tf-gnns-0.1.5a2/tf_gnns/lib/gt_ops.py
+drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:59:57.953835 tf-gnns-0.1.5a2/tf_gnns/models/
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:59:57.000000 tf-gnns-0.1.5a2/tf_gnns/models/__init__.py
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    17010 2023-04-09 18:59:57.000000 tf-gnns-0.1.5a2/tf_gnns/models/graphnet.py
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     8155 2023-04-09 18:59:57.000000 tf-gnns-0.1.5a2/tf_gnns/utils.py
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     2259 2023-04-09 18:59:57.000000 tf-gnns-0.1.5a2/tf_gnns/utils_train.py
+drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:59:57.953835 tf-gnns-0.1.5a2/tf_gnns.egg-info/
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     3654 2023-04-09 18:59:57.000000 tf-gnns-0.1.5a2/tf_gnns.egg-info/PKG-INFO
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      450 2023-04-09 18:59:57.000000 tf-gnns-0.1.5a2/tf_gnns.egg-info/SOURCES.txt
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        1 2023-04-09 18:59:57.000000 tf-gnns-0.1.5a2/tf_gnns.egg-info/dependency_links.txt
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        8 2023-04-09 18:59:57.000000 tf-gnns-0.1.5a2/tf_gnns.egg-info/top_level.txt
```

### Comparing `tf-gnns-0.1.5a1/LICENSE` & `tf-gnns-0.1.5a2/LICENSE`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.5a1/PKG-INFO` & `tf-gnns-0.1.5a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-gnns
-Version: 0.1.5a1
+Version: 0.1.5a2
 Summary: A hackable graphnets library for tensorflow-keras.
 Home-page: https://github.com/mylonasc/tf_gnns.git
 Author: Charilaos Mylonas
 Author-email: mylonas.charilaos@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tf-gnns-0.1.5a1/README.md` & `tf-gnns-0.1.5a2/README.md`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.5a1/setup.py` & `tf-gnns-0.1.5a2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     return result.group(1)
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tf-gnns", # Replace with your own username
-    version="0.1.5a1",
+    version="0.1.5a2",
     author="Charilaos Mylonas",
     author_email="mylonas.charilaos@gmail.com",
     description="A hackable graphnets library for tensorflow-keras.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mylonasc/tf_gnns.git",
     packages=setuptools.find_packages(),
```

### Comparing `tf-gnns-0.1.5a1/tf_gnns/__init__.py` & `tf-gnns-0.1.5a2/tf_gnns/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.5a1/tf_gnns/assets/html_css/accordion.js` & `tf-gnns-0.1.5a2/tf_gnns/assets/html_css/accordion.js`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.5a1/tf_gnns/assets/html_css/pretty_print_accordion.css` & `tf-gnns-0.1.5a2/tf_gnns/assets/html_css/pretty_print_accordion.css`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.5a1/tf_gnns/datastructures.py` & `tf-gnns-0.1.5a2/tf_gnns/datastructures.py`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.5a1/tf_gnns/graphnet_utils.py` & `tf-gnns-0.1.5a2/tf_gnns/graphnet_utils.py`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.5a1/tf_gnns/lib/gt_ops.py` & `tf-gnns-0.1.5a2/tf_gnns/lib/gt_ops.py`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.5a1/tf_gnns/models/graphnet.py` & `tf-gnns-0.1.5a2/tf_gnns/models/graphnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from tf_gnns.graphnet_utils import make_full_graphnet_functions, make_graph_indep_graphnet_functions, make_graph_to_graph_and_global_functions, _aggregation_function_factory
+from tf_gnns.graphnet_utils import make_full_graphnet_functions, make_mlp_graphnet_functions
+from tf_gnns.graphnet_utils import make_graph_indep_graphnet_functions, make_graph_to_graph_and_global_functions, _aggregation_function_factory
 from tf_gnns.graphnet_utils import GraphNet 
 
 from tf_gnns.lib.gt_ops import _assign_add_tensor_dict
 
 import tensorflow as tf
 import IPython
```

### Comparing `tf-gnns-0.1.5a1/tf_gnns/utils.py` & `tf-gnns-0.1.5a2/tf_gnns/utils.py`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.5a1/tf_gnns/utils_train.py` & `tf-gnns-0.1.5a2/tf_gnns/utils_train.py`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.5a1/tf_gnns.egg-info/PKG-INFO` & `tf-gnns-0.1.5a2/tf_gnns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-gnns
-Version: 0.1.5a1
+Version: 0.1.5a2
 Summary: A hackable graphnets library for tensorflow-keras.
 Home-page: https://github.com/mylonasc/tf_gnns.git
 Author: Charilaos Mylonas
 Author-email: mylonas.charilaos@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

