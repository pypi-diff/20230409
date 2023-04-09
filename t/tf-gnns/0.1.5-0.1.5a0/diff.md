# Comparing `tmp/tf-gnns-0.1.5.tar.gz` & `tmp/tf-gnns-0.1.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf-gnns-0.1.5.tar", last modified: Sun Apr  9 15:20:21 2023, max compression
+gzip compressed data, was "tf-gnns-0.1.5a0.tar", last modified: Sun Apr  9 18:12:30 2023, max compression
```

## Comparing `tf-gnns-0.1.5.tar` & `tf-gnns-0.1.5a0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 15:20:21.523487 tf-gnns-0.1.5/
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    11347 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/LICENSE
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     3652 2023-04-09 15:20:21.523487 tf-gnns-0.1.5/PKG-INFO
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     3141 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/README.md
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)       38 2023-04-09 15:20:21.523487 tf-gnns-0.1.5/setup.cfg
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     1022 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/setup.py
-drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 15:20:21.519487 tf-gnns-0.1.5/tf_gnns/
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      821 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/__init__.py
-drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 15:20:21.519487 tf-gnns-0.1.5/tf_gnns/assets/
-drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 15:20:21.523487 tf-gnns-0.1.5/tf_gnns/assets/html_css/
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      557 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/assets/html_css/accordion.js
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      658 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/assets/html_css/pretty_print_accordion.css
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    18665 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/datastructures.py
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    82635 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/graphnet_utils.py
-drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 15:20:21.523487 tf-gnns-0.1.5/tf_gnns/lib/
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/lib/__init__.py
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     4148 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/lib/gt_ops.py
-drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 15:20:21.523487 tf-gnns-0.1.5/tf_gnns/models/
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/models/__init__.py
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    11175 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/models/graphnet.py
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     8155 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/utils.py
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     2259 2023-04-09 15:20:20.000000 tf-gnns-0.1.5/tf_gnns/utils_train.py
-drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 15:20:21.523487 tf-gnns-0.1.5/tf_gnns.egg-info/
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     3652 2023-04-09 15:20:21.000000 tf-gnns-0.1.5/tf_gnns.egg-info/PKG-INFO
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      450 2023-04-09 15:20:21.000000 tf-gnns-0.1.5/tf_gnns.egg-info/SOURCES.txt
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        1 2023-04-09 15:20:21.000000 tf-gnns-0.1.5/tf_gnns.egg-info/dependency_links.txt
--rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        8 2023-04-09 15:20:21.000000 tf-gnns-0.1.5/tf_gnns.egg-info/top_level.txt
+drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:12:30.826301 tf-gnns-0.1.5a0/
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    11347 2023-04-09 18:12:30.000000 tf-gnns-0.1.5a0/LICENSE
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     3654 2023-04-09 18:12:30.826301 tf-gnns-0.1.5a0/PKG-INFO
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     3141 2023-04-09 18:12:30.000000 tf-gnns-0.1.5a0/README.md
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)       38 2023-04-09 18:12:30.826301 tf-gnns-0.1.5a0/setup.cfg
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     1023 2023-04-09 18:12:30.000000 tf-gnns-0.1.5a0/setup.py
+drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:12:30.826301 tf-gnns-0.1.5a0/tf_gnns/
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      821 2023-04-09 18:12:30.000000 tf-gnns-0.1.5a0/tf_gnns/__init__.py
+drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:12:30.826301 tf-gnns-0.1.5a0/tf_gnns/assets/
+drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:12:30.826301 tf-gnns-0.1.5a0/tf_gnns/assets/html_css/
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      557 2023-04-09 18:12:30.000000 tf-gnns-0.1.5a0/tf_gnns/assets/html_css/accordion.js
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      658 2023-04-09 18:12:30.000000 tf-gnns-0.1.5a0/tf_gnns/assets/html_css/pretty_print_accordion.css
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    18665 2023-04-09 18:12:30.000000 tf-gnns-0.1.5a0/tf_gnns/datastructures.py
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    82873 2023-04-09 18:12:30.000000 tf-gnns-0.1.5a0/tf_gnns/graphnet_utils.py
+drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:12:30.826301 tf-gnns-0.1.5a0/tf_gnns/lib/
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:12:30.000000 tf-gnns-0.1.5a0/tf_gnns/lib/__init__.py
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     4148 2023-04-09 18:12:30.000000 tf-gnns-0.1.5a0/tf_gnns/lib/gt_ops.py
+drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:12:30.826301 tf-gnns-0.1.5a0/tf_gnns/models/
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:12:30.000000 tf-gnns-0.1.5a0/tf_gnns/models/__init__.py
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)    16947 2023-04-09 18:12:30.000000 tf-gnns-0.1.5a0/tf_gnns/models/graphnet.py
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     8155 2023-04-09 18:12:30.000000 tf-gnns-0.1.5a0/tf_gnns/utils.py
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     2259 2023-04-09 18:12:30.000000 tf-gnns-0.1.5a0/tf_gnns/utils_train.py
+drwxrwxr-x   0 charilaos  (1000) charilaos  (1000)        0 2023-04-09 18:12:30.826301 tf-gnns-0.1.5a0/tf_gnns.egg-info/
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)     3654 2023-04-09 18:12:30.000000 tf-gnns-0.1.5a0/tf_gnns.egg-info/PKG-INFO
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)      450 2023-04-09 18:12:30.000000 tf-gnns-0.1.5a0/tf_gnns.egg-info/SOURCES.txt
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        1 2023-04-09 18:12:30.000000 tf-gnns-0.1.5a0/tf_gnns.egg-info/dependency_links.txt
+-rw-rw-r--   0 charilaos  (1000) charilaos  (1000)        8 2023-04-09 18:12:30.000000 tf-gnns-0.1.5a0/tf_gnns.egg-info/top_level.txt
```

### Comparing `tf-gnns-0.1.5/LICENSE` & `tf-gnns-0.1.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.5/PKG-INFO` & `tf-gnns-0.1.5a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-gnns
-Version: 0.1.5
+Version: 0.1.5a0
 Summary: A hackable graphnets library for tensorflow-keras.
 Home-page: https://github.com/mylonasc/tf_gnns.git
 Author: Charilaos Mylonas
 Author-email: mylonas.charilaos@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tf-gnns-0.1.5/README.md` & `tf-gnns-0.1.5a0/README.md`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.5/setup.py` & `tf-gnns-0.1.5a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     return result.group(1)
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tf-gnns", # Replace with your own username
-    version="0.1.5",
+    version="0.1.5a",
     author="Charilaos Mylonas",
     author_email="mylonas.charilaos@gmail.com",
     description="A hackable graphnets library for tensorflow-keras.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mylonasc/tf_gnns.git",
     packages=setuptools.find_packages(),
```

### Comparing `tf-gnns-0.1.5/tf_gnns/__init__.py` & `tf-gnns-0.1.5a0/tf_gnns/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.5/tf_gnns/assets/html_css/accordion.js` & `tf-gnns-0.1.5a0/tf_gnns/assets/html_css/accordion.js`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.5/tf_gnns/assets/html_css/pretty_print_accordion.css` & `tf-gnns-0.1.5a0/tf_gnns/assets/html_css/pretty_print_accordion.css`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.5/tf_gnns/datastructures.py` & `tf-gnns-0.1.5a0/tf_gnns/datastructures.py`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.5/tf_gnns/graphnet_utils.py` & `tf-gnns-0.1.5a0/tf_gnns/graphnet_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1647,14 +1647,16 @@
         node_or_core_input_size,
         node_or_core_output_size = None,
         edge_input_size = None,
         edge_output_size = None,
         global_input_size = None,
         global_output_size = None,
         aggregation_function = 'mean',
+        create_global_function = True,
+        use_global_input= True,
         **kwargs):
 
     """
     A wrapper that creates the functions that are needed for a graph-independent GN block. 
     Takes care of some flags that control a more general factory method for avoiding clutter.
     Usage:
       gn_core = GraphNet(**make_graph_indep_graphnet_functions(15, 20))
@@ -1703,14 +1705,16 @@
                                         global_input_size = global_input_size,
                                         use_global_input = True,
                                         use_global_to_edge=False,
                                         use_global_to_node=False,
                                         create_global_function=True, 
                                         graph_indep=True,
                                         aggregation_function = aggregation_function,
+                                        create_global_function = create_global_function,
+                                        use_global_input = use_global_input, 
                                         **kwargs)
 
 
 
 def make_full_graphnet_functions(units,
         node_or_core_input_size, 
         node_or_core_output_size = None,
```

### Comparing `tf-gnns-0.1.5/tf_gnns/lib/gt_ops.py` & `tf-gnns-0.1.5a0/tf_gnns/lib/gt_ops.py`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.5/tf_gnns/models/graphnet.py` & `tf-gnns-0.1.5a0/tf_gnns/models/graphnet.py`

 * *Files 26% similar despite different names*

```diff
@@ -276,7 +276,142 @@
         self.gn_graph_indep = GraphNet(**gnfns)
         self.all_weights = self.gn_graph_indep.weights
         self.is_built = True
         
     def call(self, g_):
         return self.gn_graph_indep.eval_tensor_dict(g_)
 
+class GraphNetMPNN_MLP(tf.keras.layers.Layer):
+    """
+    A GraphNet with all functions implemented as MLPs - no global state and 
+    no message passing to global
+
+    """
+    def __init__(self,
+                 units = 32,
+                 core_units = None,
+                 core_size = None,
+                 gi_units = None,
+                 core_steps = 1,
+                 edge_input_size = None,
+                 node_input_size = None,
+                 edge_output_size = None,
+                 node_output_size = None,
+                 recurrent = False,
+                 residual = True,
+                 aggregation_function = 'mean',
+                 *args, **kwargs):
+        super(GraphNetMPNN_MLP, self).__init__(*args, **kwargs)
+        """
+        This is similar to the `GraphNetMLP` which also creates an "encode-process-decode" 
+        stack, but with the difference that this network does not process "global variables" 
+        and there is no message to passing to "global variables". 
+
+        ("Global" -> graph level)
+
+        """
+
+        self.aggregation_function = aggregation_function
+
+        if core_units is None: 
+            core_units = units
+        if gi_units is None:
+            gi_units = units
+        if core_size is None:
+            core_size = units
+
+        self.core_units = core_units
+        self.gi_units   = gi_units
+
+        self.edge_output_size   = edge_output_size
+        self.node_output_size   = node_output_size
+        self._is_recurrent      = recurrent
+        self.core = core_size
+        self.is_built = False
+        self.is_residual = residual
+        self.core_steps = core_steps
+
+        if edge_input_size is not None  and node_input_size is not None:
+            self.build(edge_input_size, node_input_size)
+            self.is_built = True
+
+        self.all_weights = []
+
+    def build(self,  d_shapes):
+        node_input_size, edge_input_size = d_shapes['nodes'][-1], d_shapes['edges'][-1]
+        if self.edge_output_size is None:
+            self.edge_output_size = edge_input_size
+        if self.node_output_size is None:
+            self.node_output_size = node_input_size
+        self.g_enc_determ = GraphNet(
+            **make_graph_indep_graphnet_functions(self.gi_units,
+                                                    node_or_core_input_size = node_input_size,
+                                                    node_or_core_output_size= self.core,
+                                                    edge_input_size         = edge_input_size,
+                                                    global_output_size      = self.core,
+                                                    edge_output_size        = self.core,
+                                                    use_global_input=False, 
+                                                    create_global_function=False))
+        g_core_determ_list = [];
+        core_params = {'node_input_size' : self.core,
+                   'node_output_size' : self.core,
+                   'use_global_to_edge' : False,
+                   'use_global_to_node' : False, 
+                   'use_global_input' : False,
+                   'edge_input_size' : self.core,
+                   'edge_output_size' : self.core,
+                   'create_global_function' : False,
+                   'global_input_size' : None,
+                   'global_output_size' : None,
+                   'graph_indep' : False}
+        for c_ in range(self.core_steps):
+            if (c_ == 0) or ((not self._is_recurrent) and c_ > 0):
+                g = make_mlp_graphnet_functions(self.core_units,**core_params)
+
+            g_core_determ_list.append(GraphNet(**g)) # if it is recurrent, it's multiple times the same network.
+
+        self.g_dec_determ = GraphNet(
+            **make_graph_indep_graphnet_functions(self.core_units,
+                                            node_or_core_input_size = self.core,
+                                            node_or_core_output_size=  self.node_output_size,
+                                            edge_input_size         = self.core,
+                                            global_input_size       = self.core,
+                                            edge_output_size        = self.edge_output_size,
+                                            aggregation_function = self.aggregation_function, 
+                                            use_global_input=False, 
+                                            create_global_function=False))
+        self.is_built = True
+        if self._is_recurrent:
+            core_weights = g_core_determ_list[0].weights
+        else:
+            core_weights = []
+            for w in g_core_determ_list:
+                core_weights.extend(w.weights)
+        self.all_weights.extend([*self.g_enc_determ.weights, *core_weights, *self.g_dec_determ.weights])
+        self.g_core_determ = g_core_determ_list
+
+
+    def _repr_html_(self):
+        s = ''
+        s += "<h> GN Deterministic path containing the following GNs (%s,%s): </h> "%(self.name,id(self))
+        if not self.is_built:
+            s += "Layer not yet built."
+            return s
+        s += self.g_enc_determ._repr_html_()
+        for g_ in self.g_core_determ:
+            s += g_._repr_html_()
+        s += self.g_dec_determ._repr_html_()
+        return s
+
+    def call(self, g_):
+        g_ = self.g_enc_determ.eval_tensor_dict(g_)
+        for _gn in self.g_core_determ:
+            go_ = _gn.eval_tensor_dict(g_)
+            if self.is_residual:
+                g_['nodes'] = g_['nodes'] + go_['nodes']
+                g_['edges'] = g_['edges'] + go_['edges']
+            else:
+                g_ = go_
+        g_ = self.g_dec_determ.eval_tensor_dict(g_)
+        return g_
+
+
```

### Comparing `tf-gnns-0.1.5/tf_gnns/utils.py` & `tf-gnns-0.1.5a0/tf_gnns/utils.py`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.5/tf_gnns/utils_train.py` & `tf-gnns-0.1.5a0/tf_gnns/utils_train.py`

 * *Files identical despite different names*

### Comparing `tf-gnns-0.1.5/tf_gnns.egg-info/PKG-INFO` & `tf-gnns-0.1.5a0/tf_gnns.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-gnns
-Version: 0.1.5
+Version: 0.1.5a0
 Summary: A hackable graphnets library for tensorflow-keras.
 Home-page: https://github.com/mylonasc/tf_gnns.git
 Author: Charilaos Mylonas
 Author-email: mylonas.charilaos@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

