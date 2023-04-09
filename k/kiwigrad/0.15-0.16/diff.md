# Comparing `tmp/kiwigrad-0.15.tar.gz` & `tmp/kiwigrad-0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwigrad-0.15.tar", last modified: Sun Apr  9 09:18:48 2023, max compression
+gzip compressed data, was "kiwigrad-0.16.tar", last modified: Sun Apr  9 13:08:51 2023, max compression
```

## Comparing `kiwigrad-0.15.tar` & `kiwigrad-0.16.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-09 09:18:48.319818 kiwigrad-0.15/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.15/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       22 2023-04-08 12:11:45.000000 kiwigrad-0.15/MANIFEST.in
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1933 2023-04-09 09:18:48.319491 kiwigrad-0.15/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      177 2023-04-03 14:22:56.000000 kiwigrad-0.15/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-09 09:18:48.317545 kiwigrad-0.15/kiwigrad/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      424 2023-04-09 09:18:10.000000 kiwigrad-0.15/kiwigrad/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     5274 2023-04-08 16:31:22.000000 kiwigrad-0.15/kiwigrad/engine.pyx
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2940 2023-04-09 08:38:37.000000 kiwigrad-0.15/kiwigrad/nn.pyx
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-09 09:18:48.319072 kiwigrad-0.15/kiwigrad.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1933 2023-04-09 09:18:48.000000 kiwigrad-0.15/kiwigrad.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      260 2023-04-09 09:18:48.000000 kiwigrad-0.15/kiwigrad.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-09 09:18:48.000000 kiwigrad-0.15/kiwigrad.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-09 09:18:48.000000 kiwigrad-0.15/kiwigrad.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-09 09:18:48.000000 kiwigrad-0.15/kiwigrad.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      666 2023-04-09 09:18:23.000000 kiwigrad-0.15/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-09 09:18:48.319911 kiwigrad-0.15/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-09 13:08:51.688492 kiwigrad-0.16/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.16/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       22 2023-04-08 12:11:45.000000 kiwigrad-0.16/MANIFEST.in
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1933 2023-04-09 13:08:51.688051 kiwigrad-0.16/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      177 2023-04-03 14:22:56.000000 kiwigrad-0.16/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-09 13:08:51.685555 kiwigrad-0.16/kiwigrad/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      193 2023-04-09 13:07:23.000000 kiwigrad-0.16/kiwigrad/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4222 2023-04-09 13:04:30.000000 kiwigrad-0.16/kiwigrad/engine.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      970 2023-04-09 13:06:00.000000 kiwigrad-0.16/kiwigrad/graph.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3963 2023-04-09 13:05:19.000000 kiwigrad-0.16/kiwigrad/nn.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-09 13:08:51.687480 kiwigrad-0.16/kiwigrad.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1933 2023-04-09 13:08:51.000000 kiwigrad-0.16/kiwigrad.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      276 2023-04-09 13:08:51.000000 kiwigrad-0.16/kiwigrad.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-09 13:08:51.000000 kiwigrad-0.16/kiwigrad.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-09 13:08:51.000000 kiwigrad-0.16/kiwigrad.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-09 13:08:51.000000 kiwigrad-0.16/kiwigrad.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      666 2023-04-09 13:08:03.000000 kiwigrad-0.16/pyproject.toml
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-09 13:08:51.688640 kiwigrad-0.16/setup.cfg
```

### Comparing `kiwigrad-0.15/LICENSE` & `kiwigrad-0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.15/PKG-INFO` & `kiwigrad-0.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwigrad
-Version: 0.15
+Version: 0.16
 Summary: Mini deep learning framework
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `kiwigrad-0.15/kiwigrad/nn.pyx` & `kiwigrad-0.16/kiwigrad/nn.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# cython: warning_errors=-Wno-fallthrough
-# cython: language_level=3
-
 import random
 from .engine import Value
 import pickle
 
 
 class Module:
 
@@ -67,34 +64,75 @@
     def parameters(self):
         return [p for layer in self.layers for p in layer.parameters()]
     
     def __repr__(self):
         return f"MLP of [{', '.join(str(layer) for layer in self.layers)}]"
     
     def save(self, save_name: str = "weights"):
-        cdef list weights = []
+        weights = []
         for layer in self.layers:
             for neuron in layer.neurons:
                 weights.append([i.data for i in neuron.w])
                 weights.append(neuron.b.data)
         file_name = f'{save_name}.pkl'
         with open(file_name, 'wb') as f:
             pickle.dump(weights, f)
-
+    
     def load(self, save_name: str = "weights"):
         file_name = f'{save_name}.pkl'
         with open(file_name, 'rb') as f:
             params = pickle.load(f)
-        cdef list load_weights = []
+        load_weights = []
         for param in params:
             if isinstance(param, list):
                 load_param = [Value(i) for i in param]
                 load_weights.append(load_param)
             else:
                 load_param = Value(param)
                 load_weights.append(load_param)
-        cdef int i = 0
+        i = 0
         for layer in self.layers:
             for neuron in layer.neurons:
                 neuron.w = load_weights[i]
                 neuron.b = load_weights[i+1]
-                i += 2
+                i += 2
+
+
+if __name__ == "__main__":
+
+    import numpy as np
+    import matplotlib.pyplot as plt
+    import pandas as pd
+    from sklearn.metrics import r2_score
+    df_x = pd.read_csv("../../test/data/x.csv", sep=";")
+    xs = df_x.to_numpy()
+    print(xs.shape)
+    df_y = pd.read_csv("../../test/data/x.csv/y.csv", sep=";")
+    y = df_y.to_numpy().squeeze()
+    print(y.shape)
+    model = MLP(6, [16, 1], bias=True) # 1-layer neural network
+    print(model)
+    print("number of parameters", len(model.parameters()))
+
+    # loop
+    for k in range(30):
+        for i in range(len(xs)):
+            output = model(xs[i])
+            target = y[i]
+            loss = ((output - target) ** 2)
+            loss.backward()
+            for p in model.parameters():
+                p.data += -0.001 * p.grad 
+            model.zero_grad()
+        if k%5 == 0:
+            print(k, loss)
+    
+    print('\nTEST')
+    output = model(xs[0])
+    target = y[0]
+    print(f'output: {output.data}', f'target: {target}')
+
+    # r2 score
+    output = [model(x).data for x in xs]
+    r2 = r2_score(y, output)
+    print(f'r2 score: {r2}')
+
```

### Comparing `kiwigrad-0.15/kiwigrad.egg-info/PKG-INFO` & `kiwigrad-0.16/kiwigrad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwigrad
-Version: 0.15
+Version: 0.16
 Summary: Mini deep learning framework
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `kiwigrad-0.15/pyproject.toml` & `kiwigrad-0.16/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kiwigrad"
-version = "0.15"
+version = "0.16"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Mini deep learning framework"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

