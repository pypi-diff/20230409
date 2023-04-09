# Comparing `tmp/hnvlearn-0.0.1-py3-none-any.whl.zip` & `tmp/hnvlearn-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 31206 bytes, number of entries: 33
+Zip file size: 31091 bytes, number of entries: 33
 -rw-r--r--  2.0 unx      207 b- defN 22-Dec-21 09:52 hnvlearn/__init__.py
 -rw-r--r--  2.0 unx     1643 b- defN 23-Apr-09 14:34 hnvlearn/datasets.py
 -rw-r--r--  2.0 unx     3306 b- defN 22-Dec-21 09:52 hnvlearn/make_blobs.py
 -rw-r--r--  2.0 unx     5487 b- defN 22-Dec-21 09:52 hnvlearn/plot_2d_separator.py
 -rw-r--r--  2.0 unx     3449 b- defN 22-Dec-21 09:52 hnvlearn/plot_agglomerative.py
 -rw-r--r--  2.0 unx      890 b- defN 22-Dec-21 09:52 hnvlearn/plot_animal_tree.py
 -rw-r--r--  2.0 unx     8867 b- defN 22-Dec-21 09:52 hnvlearn/plot_cross_validation.py
@@ -19,17 +19,17 @@
 -rw-r--r--  2.0 unx     1005 b- defN 22-Dec-21 09:52 hnvlearn/plot_linear_regression.py
 -rw-r--r--  2.0 unx     1104 b- defN 22-Dec-21 09:52 hnvlearn/plot_linear_svc_regularization.py
 -rw-r--r--  2.0 unx     4121 b- defN 22-Dec-21 09:52 hnvlearn/plot_metrics.py
 -rw-r--r--  2.0 unx     3156 b- defN 22-Dec-21 09:52 hnvlearn/plot_nmf.py
 -rw-r--r--  2.0 unx     3510 b- defN 22-Dec-21 09:52 hnvlearn/plot_nn_graphs.py
 -rw-r--r--  2.0 unx     4715 b- defN 22-Dec-21 09:52 hnvlearn/plot_pca.py
 -rw-r--r--  2.0 unx     1178 b- defN 22-Dec-21 09:52 hnvlearn/plot_rbf_svm_parameters.py
--rw-r--r--  2.0 unx     1017 b- defN 22-Dec-21 09:52 hnvlearn/plot_ridge.py
+-rw-r--r--  2.0 unx      762 b- defN 23-Apr-09 16:38 hnvlearn/plot_ridge.py
 -rw-r--r--  2.0 unx     1505 b- defN 22-Dec-21 09:52 hnvlearn/plot_scaling.py
 -rw-r--r--  2.0 unx      894 b- defN 22-Dec-21 09:52 hnvlearn/plot_tree_nonmonotonous.py
--rw-r--r--  2.0 unx     3272 b- defN 22-Dec-21 09:52 hnvlearn/plots.py
+-rw-r--r--  2.0 unx     3192 b- defN 23-Apr-09 16:38 hnvlearn/plots.py
 -rw-r--r--  2.0 unx     4801 b- defN 22-Dec-21 09:52 hnvlearn/tools.py
--rw-r--r--  2.0 unx      769 b- defN 23-Apr-09 16:16 hnvlearn-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 16:16 hnvlearn-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-09 16:16 hnvlearn-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2755 b- defN 23-Apr-09 16:16 hnvlearn-0.0.1.dist-info/RECORD
-33 files, 82895 bytes uncompressed, 26800 bytes compressed:  67.7%
+-rw-r--r--  2.0 unx      769 b- defN 23-Apr-09 16:40 hnvlearn-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 16:40 hnvlearn-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-09 16:40 hnvlearn-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2754 b- defN 23-Apr-09 16:40 hnvlearn-0.0.2.dist-info/RECORD
+33 files, 82559 bytes uncompressed, 26685 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -81,20 +81,20 @@
 
 Filename: hnvlearn/plots.py
 Comment: 
 
 Filename: hnvlearn/tools.py
 Comment: 
 
-Filename: hnvlearn-0.0.1.dist-info/METADATA
+Filename: hnvlearn-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: hnvlearn-0.0.1.dist-info/WHEEL
+Filename: hnvlearn-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: hnvlearn-0.0.1.dist-info/top_level.txt
+Filename: hnvlearn-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: hnvlearn-0.0.1.dist-info/RECORD
+Filename: hnvlearn-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hnvlearn/plot_ridge.py

```diff
@@ -1,28 +1,19 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
 from sklearn.linear_model import Ridge, LinearRegression
 from sklearn.model_selection import learning_curve, KFold
 
-from .datasets import load_extended_boston
 
 
 def plot_learning_curve(est, X, y):
     training_set_size, train_scores, test_scores = learning_curve(
         est, X, y, train_sizes=np.linspace(.1, 1, 20), cv=KFold(20, shuffle=True, random_state=1))
     estimator_name = est.__class__.__name__
     line = plt.plot(training_set_size, train_scores.mean(axis=1), '--',
                     label="training " + estimator_name)
     plt.plot(training_set_size, test_scores.mean(axis=1), '-',
              label="test " + estimator_name, c=line[0].get_color())
     plt.xlabel('Training set size')
     plt.ylabel('Score (R^2)')
     plt.ylim(0, 1.1)
-
-
-def plot_ridge_n_samples():
-    X, y = load_extended_boston()
-
-    plot_learning_curve(Ridge(alpha=1), X, y)
-    plot_learning_curve(LinearRegression(), X, y)
-    plt.legend(loc=(0, 1.05), ncol=2, fontsize=11)
```

## hnvlearn/plots.py

```diff
@@ -23,15 +23,14 @@
                                     plot_stratified_cross_validation)
 
 from .plot_grid_search import plot_grid_search_overview, plot_cross_val_selection
 from .plot_metrics import (plot_confusion_matrix_illustration,
                            plot_binary_confusion_matrix,
                            plot_decision_threshold)
 from .plot_dbscan import plot_dbscan
-from .plot_ridge import plot_ridge_n_samples
 
 __all__ = ['plot_linear_svc_regularization',
            "plot_animal_tree", "plot_tree_progressive",
            'plot_tree_partition', 'plot_svm',
            'plot_knn_regression',
            'plot_logistic_regression_graph',
            'plot_single_hidden_layer_graph',
@@ -60,10 +59,9 @@
            'plot_threefold_split',
            'plot_cross_validation',
            'plot_grid_search_overview',
            'plot_cross_val_selection',
            'plot_confusion_matrix_illustration',
            'plot_binary_confusion_matrix',
            'plot_decision_threshold',
-           'plot_dbscan',
-           'plot_ridge_n_samples'
+           'plot_dbscan'
            ]
```

## Comparing `hnvlearn-0.0.1.dist-info/METADATA` & `hnvlearn-0.0.2.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hnvlearn
-Version: 0.0.1
+Version: 0.0.2
 Summary: hnvlearn Python library
 Home-page: https://github.com/Vikram-kr/hnvlearn
 Author: hnvlearn
 Author-email: hnv@hnv.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `hnvlearn-0.0.1.dist-info/RECORD` & `hnvlearn-0.0.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 hnvlearn/plot_linear_regression.py,sha256=_8ZTr3OTicHURSroE-QcJUzRymW8R0AsLpoYYcKk8aQ,1005
 hnvlearn/plot_linear_svc_regularization.py,sha256=wVXqjTf9TvoLr6H6NbmDmRf9XeBs6ZuT2O2Dby5-Tpc,1104
 hnvlearn/plot_metrics.py,sha256=XtQpGnFBgDehwhqUjmfFZZOvMjaOFC8w4YT36_EaaPA,4121
 hnvlearn/plot_nmf.py,sha256=OM7C3ZMObVRwSLdcG2nfhYiiHZ0pNfxATyHCAhm51Is,3156
 hnvlearn/plot_nn_graphs.py,sha256=nkMubFW734POfLUK4Hp_fJCgCHULLB8Ybh3mhGQ2JRY,3510
 hnvlearn/plot_pca.py,sha256=kX926ASOGmaNAzw4dJ3KyMjqZ0oHAuCMAdFKwZnr1Ik,4715
 hnvlearn/plot_rbf_svm_parameters.py,sha256=5FGQ2q862XR8F38lgYf9NxQIcd9Sdx7QxbJAPsFpwnc,1178
-hnvlearn/plot_ridge.py,sha256=Ozt6L3iT5ItrtyUelGYNGxNZ2iW5SgWM3jUfzK84USE,1017
+hnvlearn/plot_ridge.py,sha256=oe1sF70v1YQu6CAF6X-jV9ne0b2sycGv7n0hpQh4ujE,762
 hnvlearn/plot_scaling.py,sha256=oidDADjQXuCyah1TBPgUMQn0Rl_ELlPaVE1_d9i-P_8,1505
 hnvlearn/plot_tree_nonmonotonous.py,sha256=uh7nUMjmJauRxDCI-yfdfXuGIchUewTYl5e2twiw8SY,894
-hnvlearn/plots.py,sha256=LKCy6uhpporfNblsNj9iAWg4I3i7vYK2HD3GMGhwrKo,3272
+hnvlearn/plots.py,sha256=L-aAn4Io4GNSSk3tkaWzoAk3zxA5B2X5-k25sIbhheI,3192
 hnvlearn/tools.py,sha256=duEQLvvWt5yHBvTdS1YO-c2bH4AZOozchy1sKNO1CGg,4801
-hnvlearn-0.0.1.dist-info/METADATA,sha256=pU7vrfgmEw57YfLMzQp-REte7iK2bZ-Hek0tJrmdOno,769
-hnvlearn-0.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-hnvlearn-0.0.1.dist-info/top_level.txt,sha256=MQeYioSHVaR0bTz7Ya2Xwe8ADRGu_DhVq-a0k5qHaA0,9
-hnvlearn-0.0.1.dist-info/RECORD,,
+hnvlearn-0.0.2.dist-info/METADATA,sha256=G7Q0FjlzX0jup1JRWLMSv_C_xC0FezA4DNMwAIbBEn4,769
+hnvlearn-0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+hnvlearn-0.0.2.dist-info/top_level.txt,sha256=MQeYioSHVaR0bTz7Ya2Xwe8ADRGu_DhVq-a0k5qHaA0,9
+hnvlearn-0.0.2.dist-info/RECORD,,
```

