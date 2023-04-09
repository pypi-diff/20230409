# Comparing `tmp/tf-gnns-0.1.4.tar.gz` & `tmp/tf-gnns-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf-gnns-0.1.4.tar", last modified: Mon Nov 15 10:58:13 2021, max compression
+gzip compressed data, was "tf-gnns-0.1.5.tar", last modified: Sun Apr  9 15:20:21 2023, max compression
```

## Comparing `tf-gnns-0.1.4.tar` & `tf-gnns-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2021-11-15 10:58:13.423927 tf-gnns-0.1.4/
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     4073 2021-11-15 10:58:13.423927 tf-gnns-0.1.4/PKG-INFO
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     3141 2021-11-15 10:58:13.000000 tf-gnns-0.1.4/README.md
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)       38 2021-11-15 10:58:13.423927 tf-gnns-0.1.4/setup.cfg
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     1022 2021-11-15 10:58:13.000000 tf-gnns-0.1.4/setup.py
-drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2021-11-15 10:58:13.419927 tf-gnns-0.1.4/tf_gnns/
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      821 2021-11-15 10:58:13.000000 tf-gnns-0.1.4/tf_gnns/__init__.py
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    18671 2021-11-15 10:58:13.000000 tf-gnns-0.1.4/tf_gnns/datastructures.py
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    82644 2021-11-15 10:58:13.000000 tf-gnns-0.1.4/tf_gnns/graphnet_utils.py
-drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2021-11-15 10:58:13.423927 tf-gnns-0.1.4/tf_gnns/lib/
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        0 2021-11-15 10:58:13.000000 tf-gnns-0.1.4/tf_gnns/lib/__init__.py
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     4150 2021-11-15 10:58:13.000000 tf-gnns-0.1.4/tf_gnns/lib/gt_ops.py
-drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2021-11-15 10:58:13.423927 tf-gnns-0.1.4/tf_gnns/models/
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        0 2021-11-15 10:58:13.000000 tf-gnns-0.1.4/tf_gnns/models/__init__.py
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    11175 2021-11-15 10:58:13.000000 tf-gnns-0.1.4/tf_gnns/models/graphnet.py
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     8155 2021-11-15 10:58:13.000000 tf-gnns-0.1.4/tf_gnns/utils.py
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     2259 2021-11-15 10:58:13.000000 tf-gnns-0.1.4/tf_gnns/utils_train.py
-drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2021-11-15 10:58:13.423927 tf-gnns-0.1.4/tf_gnns.egg-info/
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     4073 2021-11-15 10:58:13.000000 tf-gnns-0.1.4/tf_gnns.egg-info/PKG-INFO
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      354 2021-11-15 10:58:13.000000 tf-gnns-0.1.4/tf_gnns.egg-info/SOURCES.txt
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        1 2021-11-15 10:58:13.000000 tf-gnns-0.1.4/tf_gnns.egg-info/dependency_links.txt
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        8 2021-11-15 10:58:13.000000 tf-gnns-0.1.4/tf_gnns.egg-info/top_level.txt
+drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 15:20:21.523487 tf-gnns-0.1.5/
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    11347 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/LICENSE
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     3652 2023-04-09 15:20:21.523487 tf-gnns-0.1.5/PKG-INFO
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     3141 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/README.md
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)       38 2023-04-09 15:20:21.523487 tf-gnns-0.1.5/setup.cfg
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     1022 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/setup.py
+drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 15:20:21.519487 tf-gnns-0.1.5/tf_gnns/
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      821 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/__init__.py
+drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 15:20:21.519487 tf-gnns-0.1.5/tf_gnns/assets/
+drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 15:20:21.523487 tf-gnns-0.1.5/tf_gnns/assets/html_css/
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      557 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/assets/html_css/accordion.js
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      658 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/assets/html_css/pretty_print_accordion.css
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    18665 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/datastructures.py
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    82635 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/graphnet_utils.py
+drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 15:20:21.523487 tf-gnns-0.1.5/tf_gnns/lib/
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/lib/__init__.py
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     4148 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/lib/gt_ops.py
+drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 15:20:21.523487 tf-gnns-0.1.5/tf_gnns/models/
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/models/__init__.py
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    11175 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/models/graphnet.py
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     8155 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/utils.py
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     2259 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/utils_train.py
+drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 15:20:21.523487 tf-gnns-0.1.5/tf_gnns.egg-info/
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     3652 2023-04-09 15:20:21.000000 tf-gnns-0.1.5/tf_gnns.egg-info/PKG-INFO
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      450 2023-04-09 15:20:21.000000 tf-gnns-0.1.5/tf_gnns.egg-info/SOURCES.txt
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        1 2023-04-09 15:20:21.000000 tf-gnns-0.1.5/tf_gnns.egg-info/dependency_links.txt
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        8 2023-04-09 15:20:21.000000 tf-gnns-0.1.5/tf_gnns.egg-info/top_level.txt
```

### Comparing `tf-gnns-0.1.4/PKG-INFO` & `tf-gnns-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,72 @@
 Metadata-Version: 2.1
 Name: tf-gnns
-Version: 0.1.4
+Version: 0.1.5
 Summary: A hackable graphnets library for tensorflow-keras.
 Home-page: https://github.com/mylonasc/tf_gnns.git
 Author: Charilaos Mylonas
 Author-email: mylonas.charilaos@gmail.com
 License: UNKNOWN
-Description: # `tf_gnns` - A Hackable GraphNets library
-        ![alt-img](https://raw.githubusercontent.com/mylonasc/tf_gnns/main/doc/figures/tfgnns_logo2.png)
-        A library for easy construction of message-passing networks in tensorflow keras.
-        It is inspired largely by this [DeepMind paper](https://arxiv.org/abs/1806.01261) and the corresponding open-sourced library ([original graph_nets library](https://github.com/deepmind/graph_nets))
-        
-        The `tf_gnns` library has no external dependencies except tensorflow 2.x (there is no support for tf 1.x graphs/sessions-based computation). 
-        It implements some alternative design constraints from `graph_nets` taking advantage of some facilities keras provides to make complex models easily and without large drops in performance.
-        
-        `tf_gnns` is built to support arbitrary node/edge/global attributes and update functions.
-        A set of convenience functions providing MLP construction with keras are also provided (i.e., handling input/output sizes for valid networks) that replaces sonnet.
-        
-        The main motivation for this library was the absense of a relatively short and efficient implementation of GNNs that was explicitly created to take advantage of keras's functionalities.
-        GNN implementations which take advantage of `tensorflow_probability` functionality are to be released in the future (as the one used in \[2\]).
-        
-        ## Installing `tf_gnns`
-        Install with `pip`:
-        ```
-        pip install tf_gnns
-        ```
-        
-        # Examples
-        
-        ## `tf_gnns` basics
-        You may inspect some basic functionality on the following colab notebook:
-        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mylonasc/tf_gnns/blob/main/notebooks/01_tf_gnn_basics.ipynb)
-        
-        
-        ## list sorting example
-        (Example from the original `deepmind/graph_nets` library)
-        If you are familiar with the original `graph_nets` library, this example will help you understand how you can transition to `tf_gnns`.
-        
-        Sort a list of elements.
-        This notebook and the accompanying code demonstrates how to use the Graph Nets library to learn to sort a list of elements.
-        
-        A list of elements is treated as a fully connected graph between the elements. 
-        The network is trained to label the start node, and which (directed) edges correspond to the links to the next largest element, for each node.
-        
-        After training, the prediction ability is tested by comparing its output to true sorted lists. Then the network's ability to generalise is tested, by using it to sort larger lists.
-        
-        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mylonasc/tf_gnns/blob/main/notebooks/02_list_sorting.ipynb)
-        
-        ## Performance
-        From some initial tests the performance of the `tf_gnns` library seems to be at least as good as `deepmind/graph_nets` when using tensor dictionaries.
-        
-        # Publications using `tf_gnns`
-        The library has been used so far in the following publications:
-        
-        \[1\][Bayesian graph neural networks for strain-based crack localization](https://arxiv.org/abs/2012.06791) 
-        
-        \[2\][Remaining Useful Life Estimation Under Uncertainty with Causal GraphNets](https://arxiv.org/abs/2011.11740)
-        
-        
-        
-        
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# `tf_gnns` - A Hackable GraphNets library
+![alt-img](https://raw.githubusercontent.com/mylonasc/tf_gnns/main/doc/figures/tfgnns_logo2.png)
+A library for easy construction of message-passing networks in tensorflow keras.
+It is inspired largely by this [DeepMind paper](https://arxiv.org/abs/1806.01261) and the corresponding open-sourced library ([original graph_nets library](https://github.com/deepmind/graph_nets))
+
+The `tf_gnns` library has no external dependencies except tensorflow 2.x (there is no support for tf 1.x graphs/sessions-based computation). 
+It implements some alternative design constraints from `graph_nets` taking advantage of some facilities keras provides to make complex models easily and without large drops in performance.
+
+`tf_gnns` is built to support arbitrary node/edge/global attributes and update functions.
+A set of convenience functions providing MLP construction with keras are also provided (i.e., handling input/output sizes for valid networks) that replaces sonnet.
+
+The main motivation for this library was the absense of a relatively short and efficient implementation of GNNs that was explicitly created to take advantage of keras's functionalities.
+GNN implementations which take advantage of `tensorflow_probability` functionality are to be released in the future (as the one used in \[2\]).
+
+## Installing `tf_gnns`
+Install with `pip`:
+```
+pip install tf_gnns
+```
+
+# Examples
+
+## `tf_gnns` basics
+You may inspect some basic functionality on the following colab notebook:
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mylonasc/tf_gnns/blob/main/notebooks/01_tf_gnn_basics.ipynb)
+
+
+## list sorting example
+(Example from the original `deepmind/graph_nets` library)
+If you are familiar with the original `graph_nets` library, this example will help you understand how you can transition to `tf_gnns`.
+
+Sort a list of elements.
+This notebook and the accompanying code demonstrates how to use the Graph Nets library to learn to sort a list of elements.
+
+A list of elements is treated as a fully connected graph between the elements. 
+The network is trained to label the start node, and which (directed) edges correspond to the links to the next largest element, for each node.
+
+After training, the prediction ability is tested by comparing its output to true sorted lists. Then the network's ability to generalise is tested, by using it to sort larger lists.
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mylonasc/tf_gnns/blob/main/notebooks/02_list_sorting.ipynb)
+
+## Performance
+From some initial tests the performance of the `tf_gnns` library seems to be at least as good as `deepmind/graph_nets` when using tensor dictionaries.
+
+# Publications using `tf_gnns`
+The library has been used so far in the following publications:
+
+\[1\][Bayesian graph neural networks for strain-based crack localization](https://arxiv.org/abs/2012.06791) 
+
+\[2\][Remaining Useful Life Estimation Under Uncertainty with Causal GraphNets](https://arxiv.org/abs/2011.11740)
+
+
+
+
+
+
```

### Comparing `tf-gnns-0.1.4/README.md` & `tf-gnns-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.4/setup.py` & `tf-gnns-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     return result.group(1)
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tf-gnns", # Replace with your own username
-    version="0.1.4",
+    version="0.1.5",
     author="Charilaos Mylonas",
     author_email="mylonas.charilaos@gmail.com",
     description="A hackable graphnets library for tensorflow-keras.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mylonasc/tf_gnns.git",
     packages=setuptools.find_packages(),
```

### Comparing `tf-gnns-0.1.4/tf_gnns/__init__.py` & `tf-gnns-0.1.5/tf_gnns/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.4/tf_gnns/datastructures.py` & `tf-gnns-0.1.5/tf_gnns/datastructures.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,29 +233,29 @@
     # is the batched size. It is required that such graphs were provided for the construction (or at least the first dimension is "1").
     edges_attr_stacked = tf.squeeze(tf.stack(edge_attr_tensor,0),1) 
     nodes_attr_stacked = tf.squeeze(tf.stack(nodes_attr_tensor,0),1)
     return GraphTuple(nodes_attr_stacked, edges_attr_stacked,senders, receivers, n_nodes, n_edges)# , graph_id)
 
 
 class GraphTuple:
-    def __init__(self, nodes, edges,senders,receivers, n_nodes, n_edges, global_attr = None,sort_receivers_to_edges  = False , _global_reps_for_nodes = None, _global_reps_for_edges = None, n_graphs = None):
+    def __init__(self, nodes, edges,senders,receivers, n_nodes, n_edges, global_attr = None,sort_receivers_to_edges  = False , global_reps_for_nodes = None, global_reps_for_edges = None, n_graphs = None):
         """
         A graph tuple contains multiple graphs for faster batched computation. 
         
         parameters:
             nodes      : a `tf.Tensor` containing all the node attributes
             edges      : a `tf.Tensor` containing all the edge attributes
             senders    : a list of sender node indices defining the graph connectivity. The indices are unique accross graphs
             receivers  : a list of receiver node indices defining the graph connectivity. The indices are unique accross graphs
             n_nodes    : a list, a numpy array or a tf.Tensor containing how many nodes are in each graph represented by the nodes and edges in the object
             n_edges    : a list,a numpy array or a tf.Tensor containing how many edges are in each graph represented by the nodes and edges in the object
             global_attr: (optional) a `tf.Tensor` or a `np.array` containing global attributes (first size - self.n_graphs)
             sort_receivers :  (optional) whether to sort the edges on construction, allowing for not needing to sort the output of the node receiver aggregators.
-            _global_reps_for_edges : (optional) used for the aggregation of the global var.
-            _global_reps_for_nodes : (optional) used for the aggregation of the global var.
+            global_reps_for_edges : (optional) used for the aggregation of the global var.
+            global_reps_for_nodes : (optional) used for the aggregation of the global var.
             n_graphs   : (optional)
         """
         # Sort edges according to receivers and sort receivers:
         assert(len(n_nodes) == len(n_edges))
         
         self.nodes = nodes # floats tensor
         self.edges = edges # floats tensor
@@ -280,15 +280,15 @@
 
         
         if self.has_global: # <- default global is "None". If it was provided, set the global variable (together with some aggregator indices for convenience and performance).
             self.assign_global(global_attr)
 
         self.graph_indices_nodes , self.graph_indices_edges = graph_indices_nodes, graph_indices_edges
 
-        if (_global_reps_for_edges is None ) and (_global_reps_for_nodes is None):
+        if (global_reps_for_edges is None ) and (global_reps_for_nodes is None):
             self.update_reps_for_globals()
         self.n_graphs = len(self.n_nodes)
 
 
 
 
     def update_reps_for_globals(self):
@@ -406,11 +406,11 @@
             'nodes' : _tf_constant_or_none(gt_.nodes),
             'senders' : _tf_constant_or_none(gt_.senders),
             'receivers' :_tf_constant_or_none(gt_.receivers),
             'n_edges' : _tf_constant_or_none(gt_.n_edges),
             'n_nodes' : _tf_constant_or_none(gt_.n_nodes),
             'n_graphs' : _tf_constant_or_none(gt_.n_graphs),
             'global_attr' : _tf_constant_or_none(gt_.global_attr),
-           '_global_reps_for_edges' : _tf_constant_or_none(gt_._global_reps_for_edges),
-           '_global_reps_for_nodes' : _tf_constant_or_none(gt_._global_reps_for_nodes)}
+            'global_reps_for_edges' : _tf_constant_or_none(gt_._global_reps_for_edges),
+            'global_reps_for_nodes' : _tf_constant_or_none(gt_._global_reps_for_nodes)}
```

### Comparing `tf-gnns-0.1.4/tf_gnns/graphnet_utils.py` & `tf-gnns-0.1.5/tf_gnns/graphnet_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -565,15 +565,15 @@
         
         return tf_graph_tuple
         # no changes in Graph topology - nothing else to do!
 
     @tf.function
     def edge_block(self,edges = None, nodes = None, senders = None, receivers = None,
                    n_edges = None, n_nodes = None,
-                   global_attr= None,_global_reps_for_edges = None, _global_reps_for_nodes = None,n_graphs = None):
+                   global_attr= None, global_reps_for_edges = None, global_reps_for_nodes = None,n_graphs = None):
         
         edge_inputs  = {}
         if EdgeInput.EDGE_STATE.value in self.edge_input_dict.keys():
             v = edges
             edge_inputs.update({EdgeInput.EDGE_STATE.value : v})
 
         if EdgeInput.SENDER_NODE_STATE.value in self.edge_input_dict.keys():
@@ -581,34 +581,34 @@
             edge_inputs.update({EdgeInput.SENDER_NODE_STATE.value : v})
 
         if EdgeInput.RECEIVER_NODE_STATE.value in self.edge_input_dict.keys():
             v = tf.gather(nodes, receivers,axis = 0)
             edge_inputs.update({EdgeInput.RECEIVER_NODE_STATE.value : v })
 
         if EdgeInput.GLOBAL_STATE.value in self.edge_input_dict.keys():
-            edge_reps = _global_reps_for_edges
+            edge_reps = global_reps_for_edges
             edge_inputs.update({
                 EdgeInput.GLOBAL_STATE.value : tf.gather(global_attr,edge_reps, axis = 0)
             })
 
 
         edges = self.edge_function(edge_inputs)
         return edges
 
     @tf.function
     def node_block(self,edges = None, nodes = None, senders = None, receivers = None, 
-                  n_edges = None, n_nodes = None, global_attr = None,_global_reps_for_edges = None, _global_reps_for_nodes = None,n_graphs = None):
+                  n_edges = None, n_nodes = None, global_attr = None, global_reps_for_edges = None, global_reps_for_nodes = None,n_graphs = None):
         # 2) Aggregate the messages (unsorted segment sums etc):
         node_inputs = OrderedDict()
         # 3) Compute node function:
         if NodeInput.NODE_STATE.value in self.node_input_dict.keys():
             node_inputs.update({NodeInput.NODE_STATE.value : nodes})
 
         if NodeInput.GLOBAL_STATE.value in self.node_input_dict.keys():
-            node_inputs.update({NodeInput.GLOBAL_STATE.value : tf.gather(global_attr,_global_reps_for_nodes)})
+            node_inputs.update({NodeInput.GLOBAL_STATE.value : tf.gather(global_attr, global_reps_for_nodes)})
 
         if NodeInput.EDGE_AGG_STATE.value in self.node_input_dict.keys():
             if self.has_seg_aggregator_edge_to_global:
                 max_seq = int(tf.reduce_sum(n_nodes))
                 edge_to_nodes_messages = self.edge_aggregation_function_seg(edges, receivers, max_seq)
             else:
                 raise Exception("Not Implemented!")
@@ -616,32 +616,32 @@
             
         nodes = self.node_function(node_inputs)
             
         return nodes
 
     @tf.function
     def global_block(self, edges = None, nodes = None, senders = None, receivers = None, 
-                    n_edges = None, n_nodes = None , global_attr = None, _global_reps_for_edges = None,
-                     _global_reps_for_nodes = None, n_graphs = None):
+                    n_edges = None, n_nodes = None , global_attr = None, global_reps_for_edges = None,
+                     global_reps_for_nodes = None, n_graphs = None):
         
         global_inputs = {}
         if n_graphs is None:
             n_graphs = len(n_edges)
 
         if (GlobalInput.EDGE_AGG_STATE.value in self.global_input_dict.keys()):
             if self.has_seg_aggregator_edge_to_global: #<- same aggregator for edges-to-nodes and edges-to-global.
                 edges_to_global_messages = self.edge_aggregation_function_seg(
-                        edges, _global_reps_for_edges, n_graphs)
+                        edges, global_reps_for_edges, n_graphs)
                 global_inputs.update({GlobalInput.EDGE_AGG_STATE.value : edges_to_global_messages})
             else:
                 raise Exception("Not Implemented!")
         if (GlobalInput.NODE_AGG_STATE.value in self.global_input_dict.keys()):
             if self.has_seg_aggregator_node_to_global:
                 nodes_to_global_messages = self.node_to_global_aggregation_function[1](
-                    nodes, _global_reps_for_nodes, n_graphs)
+                    nodes, global_reps_for_nodes, n_graphs)
                 global_inputs.update({GlobalInput.NODE_AGG_STATE.value : nodes_to_global_messages})
 
         if GlobalInput.GLOBAL_STATE.value in self.global_input_dict.keys():
             global_inputs.update({GlobalInput.GLOBAL_STATE.value  : global_attr})
             
         if len(global_inputs) > 0:
             global_attr = self.global_function(global_inputs)
@@ -652,15 +652,15 @@
     def eval_tensor_dict(self,d):
         """
         For better performance this uses a dictionary of all the necessary tensors
         rather than a GraphTuple. A graph tuple is easilly transformed to a dictionary 
         of tensors by `_graphtuple_to_tensor_dict` function. 
 
         `d` is an ordered dictionary containing the following:
-          'edges','nodes','senders','receivers','n_edges','n_nodes','global_attr','_global_reps_for_edges','_global_reps_for_nodes'
+          'edges','nodes','senders','receivers','n_edges','n_nodes','global_attr','global_reps_for_edges','global_reps_for_nodes'
 
         """
         d_ = d.copy() # A working on a copy of d (for tf.function compilation requirement).
         if self.edge_function is not None:
             new_edges = self.edge_block(**d_)
             d_['edges'] = new_edges
         if self.node_function is not None:
```

### Comparing `tf-gnns-0.1.4/tf_gnns/lib/gt_ops.py` & `tf-gnns-0.1.5/tf_gnns/lib/gt_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Contains functions for performing some usual operations on tensor dictionaries that correspond
 # to graph tuples. 
 # 
 # 
 
 import tensorflow as tf
 
-GRAPH_TUPLE_STRUCTURE = ['senders', 'receivers', 'n_nodes', 'n_edges', '_global_reps_for_edges', '_global_reps_for_nodes', 'n_graphs']
+GRAPH_TUPLE_STRUCTURE = ['senders', 'receivers', 'n_nodes', 'n_edges', 'global_reps_for_edges', 'global_reps_for_nodes', 'n_graphs']
 
 def _zero_graph(g_,state_size = None):
     """
     Returns a graph full of zeros with all (vector) graph attributes being the same size as g_,
     or all being of size "state_size".
     
     operates on tensor dictionaries which correspond to graph tuples.
```

### Comparing `tf-gnns-0.1.4/tf_gnns/models/graphnet.py` & `tf-gnns-0.1.5/tf_gnns/models/graphnet.py`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.4/tf_gnns/utils.py` & `tf-gnns-0.1.5/tf_gnns/utils.py`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.4/tf_gnns/utils_train.py` & `tf-gnns-0.1.5/tf_gnns/utils_train.py`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.4/tf_gnns.egg-info/PKG-INFO` & `tf-gnns-0.1.5/tf_gnns.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,72 @@
 Metadata-Version: 2.1
 Name: tf-gnns
-Version: 0.1.4
+Version: 0.1.5
 Summary: A hackable graphnets library for tensorflow-keras.
 Home-page: https://github.com/mylonasc/tf_gnns.git
 Author: Charilaos Mylonas
 Author-email: mylonas.charilaos@gmail.com
 License: UNKNOWN
-Description: # `tf_gnns` - A Hackable GraphNets library
-        ![alt-img](https://raw.githubusercontent.com/mylonasc/tf_gnns/main/doc/figures/tfgnns_logo2.png)
-        A library for easy construction of message-passing networks in tensorflow keras.
-        It is inspired largely by this [DeepMind paper](https://arxiv.org/abs/1806.01261) and the corresponding open-sourced library ([original graph_nets library](https://github.com/deepmind/graph_nets))
-        
-        The `tf_gnns` library has no external dependencies except tensorflow 2.x (there is no support for tf 1.x graphs/sessions-based computation). 
-        It implements some alternative design constraints from `graph_nets` taking advantage of some facilities keras provides to make complex models easily and without large drops in performance.
-        
-        `tf_gnns` is built to support arbitrary node/edge/global attributes and update functions.
-        A set of convenience functions providing MLP construction with keras are also provided (i.e., handling input/output sizes for valid networks) that replaces sonnet.
-        
-        The main motivation for this library was the absense of a relatively short and efficient implementation of GNNs that was explicitly created to take advantage of keras's functionalities.
-        GNN implementations which take advantage of `tensorflow_probability` functionality are to be released in the future (as the one used in \[2\]).
-        
-        ## Installing `tf_gnns`
-        Install with `pip`:
-        ```
-        pip install tf_gnns
-        ```
-        
-        # Examples
-        
-        ## `tf_gnns` basics
-        You may inspect some basic functionality on the following colab notebook:
-        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mylonasc/tf_gnns/blob/main/notebooks/01_tf_gnn_basics.ipynb)
-        
-        
-        ## list sorting example
-        (Example from the original `deepmind/graph_nets` library)
-        If you are familiar with the original `graph_nets` library, this example will help you understand how you can transition to `tf_gnns`.
-        
-        Sort a list of elements.
-        This notebook and the accompanying code demonstrates how to use the Graph Nets library to learn to sort a list of elements.
-        
-        A list of elements is treated as a fully connected graph between the elements. 
-        The network is trained to label the start node, and which (directed) edges correspond to the links to the next largest element, for each node.
-        
-        After training, the prediction ability is tested by comparing its output to true sorted lists. Then the network's ability to generalise is tested, by using it to sort larger lists.
-        
-        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mylonasc/tf_gnns/blob/main/notebooks/02_list_sorting.ipynb)
-        
-        ## Performance
-        From some initial tests the performance of the `tf_gnns` library seems to be at least as good as `deepmind/graph_nets` when using tensor dictionaries.
-        
-        # Publications using `tf_gnns`
-        The library has been used so far in the following publications:
-        
-        \[1\][Bayesian graph neural networks for strain-based crack localization](https://arxiv.org/abs/2012.06791) 
-        
-        \[2\][Remaining Useful Life Estimation Under Uncertainty with Causal GraphNets](https://arxiv.org/abs/2011.11740)
-        
-        
-        
-        
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# `tf_gnns` - A Hackable GraphNets library
+![alt-img](https://raw.githubusercontent.com/mylonasc/tf_gnns/main/doc/figures/tfgnns_logo2.png)
+A library for easy construction of message-passing networks in tensorflow keras.
+It is inspired largely by this [DeepMind paper](https://arxiv.org/abs/1806.01261) and the corresponding open-sourced library ([original graph_nets library](https://github.com/deepmind/graph_nets))
+
+The `tf_gnns` library has no external dependencies except tensorflow 2.x (there is no support for tf 1.x graphs/sessions-based computation). 
+It implements some alternative design constraints from `graph_nets` taking advantage of some facilities keras provides to make complex models easily and without large drops in performance.
+
+`tf_gnns` is built to support arbitrary node/edge/global attributes and update functions.
+A set of convenience functions providing MLP construction with keras are also provided (i.e., handling input/output sizes for valid networks) that replaces sonnet.
+
+The main motivation for this library was the absense of a relatively short and efficient implementation of GNNs that was explicitly created to take advantage of keras's functionalities.
+GNN implementations which take advantage of `tensorflow_probability` functionality are to be released in the future (as the one used in \[2\]).
+
+## Installing `tf_gnns`
+Install with `pip`:
+```
+pip install tf_gnns
+```
+
+# Examples
+
+## `tf_gnns` basics
+You may inspect some basic functionality on the following colab notebook:
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mylonasc/tf_gnns/blob/main/notebooks/01_tf_gnn_basics.ipynb)
+
+
+## list sorting example
+(Example from the original `deepmind/graph_nets` library)
+If you are familiar with the original `graph_nets` library, this example will help you understand how you can transition to `tf_gnns`.
+
+Sort a list of elements.
+This notebook and the accompanying code demonstrates how to use the Graph Nets library to learn to sort a list of elements.
+
+A list of elements is treated as a fully connected graph between the elements. 
+The network is trained to label the start node, and which (directed) edges correspond to the links to the next largest element, for each node.
+
+After training, the prediction ability is tested by comparing its output to true sorted lists. Then the network's ability to generalise is tested, by using it to sort larger lists.
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mylonasc/tf_gnns/blob/main/notebooks/02_list_sorting.ipynb)
+
+## Performance
+From some initial tests the performance of the `tf_gnns` library seems to be at least as good as `deepmind/graph_nets` when using tensor dictionaries.
+
+# Publications using `tf_gnns`
+The library has been used so far in the following publications:
+
+\[1\][Bayesian graph neural networks for strain-based crack localization](https://arxiv.org/abs/2012.06791) 
+
+\[2\][Remaining Useful Life Estimation Under Uncertainty with Causal GraphNets](https://arxiv.org/abs/2011.11740)
+
+
+
+
+
+
```

