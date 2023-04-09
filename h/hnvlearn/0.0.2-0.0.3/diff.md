# Comparing `tmp/hnvlearn-0.0.2-py3-none-any.whl.zip` & `tmp/hnvlearn-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 31091 bytes, number of entries: 33
--rw-r--r--  2.0 unx      207 b- defN 22-Dec-21 09:52 hnvlearn/__init__.py
+Zip file size: 31101 bytes, number of entries: 33
+-rw-r--r--  2.0 unx      229 b- defN 23-Apr-09 16:51 hnvlearn/__init__.py
 -rw-r--r--  2.0 unx     1643 b- defN 23-Apr-09 14:34 hnvlearn/datasets.py
 -rw-r--r--  2.0 unx     3306 b- defN 22-Dec-21 09:52 hnvlearn/make_blobs.py
 -rw-r--r--  2.0 unx     5487 b- defN 22-Dec-21 09:52 hnvlearn/plot_2d_separator.py
 -rw-r--r--  2.0 unx     3449 b- defN 22-Dec-21 09:52 hnvlearn/plot_agglomerative.py
 -rw-r--r--  2.0 unx      890 b- defN 22-Dec-21 09:52 hnvlearn/plot_animal_tree.py
 -rw-r--r--  2.0 unx     8867 b- defN 22-Dec-21 09:52 hnvlearn/plot_cross_validation.py
 -rw-r--r--  2.0 unx     1798 b- defN 22-Dec-21 09:52 hnvlearn/plot_dbscan.py
@@ -24,12 +24,12 @@
 -rw-r--r--  2.0 unx     4715 b- defN 22-Dec-21 09:52 hnvlearn/plot_pca.py
 -rw-r--r--  2.0 unx     1178 b- defN 22-Dec-21 09:52 hnvlearn/plot_rbf_svm_parameters.py
 -rw-r--r--  2.0 unx      762 b- defN 23-Apr-09 16:38 hnvlearn/plot_ridge.py
 -rw-r--r--  2.0 unx     1505 b- defN 22-Dec-21 09:52 hnvlearn/plot_scaling.py
 -rw-r--r--  2.0 unx      894 b- defN 22-Dec-21 09:52 hnvlearn/plot_tree_nonmonotonous.py
 -rw-r--r--  2.0 unx     3192 b- defN 23-Apr-09 16:38 hnvlearn/plots.py
 -rw-r--r--  2.0 unx     4801 b- defN 22-Dec-21 09:52 hnvlearn/tools.py
--rw-r--r--  2.0 unx      769 b- defN 23-Apr-09 16:40 hnvlearn-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 16:40 hnvlearn-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-09 16:40 hnvlearn-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2754 b- defN 23-Apr-09 16:40 hnvlearn-0.0.2.dist-info/RECORD
-33 files, 82559 bytes uncompressed, 26685 bytes compressed:  67.7%
+-rw-r--r--  2.0 unx      769 b- defN 23-Apr-09 16:53 hnvlearn-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 16:53 hnvlearn-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-09 16:53 hnvlearn-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2754 b- defN 23-Apr-09 16:53 hnvlearn-0.0.3.dist-info/RECORD
+33 files, 82581 bytes uncompressed, 26695 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -81,20 +81,20 @@
 
 Filename: hnvlearn/plots.py
 Comment: 
 
 Filename: hnvlearn/tools.py
 Comment: 
 
-Filename: hnvlearn-0.0.2.dist-info/METADATA
+Filename: hnvlearn-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: hnvlearn-0.0.2.dist-info/WHEEL
+Filename: hnvlearn-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: hnvlearn-0.0.2.dist-info/top_level.txt
+Filename: hnvlearn-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: hnvlearn-0.0.2.dist-info/RECORD
+Filename: hnvlearn-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hnvlearn/__init__.py

```diff
@@ -1,7 +1,9 @@
 from . import plots
 from . import tools
 from .plots import cm3, cm2
 from .tools import discrete_scatter
 from .plot_helpers import ReBl
 
 __all__ = ['tools', 'plots', 'cm3', 'cm2', 'discrete_scatter', 'ReBl']
+
+__version__ = '0.0.3'
```

## Comparing `hnvlearn-0.0.2.dist-info/METADATA` & `hnvlearn-0.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hnvlearn
-Version: 0.0.2
+Version: 0.0.3
 Summary: hnvlearn Python library
 Home-page: https://github.com/Vikram-kr/hnvlearn
 Author: hnvlearn
 Author-email: hnv@hnv.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `hnvlearn-0.0.2.dist-info/RECORD` & `hnvlearn-0.0.3.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-hnvlearn/__init__.py,sha256=uiQ6TxwNqNJzmp8kwq7JOF89Xr_8PIPYxhxfT1WWevI,207
+hnvlearn/__init__.py,sha256=OkEc221xZU0p3yA5F8wP7851_vE6GGtMpJPID9RzFmM,229
 hnvlearn/datasets.py,sha256=rLntwPZpf-Yv76LvPWxUVHng09B82NcRirtHrPwiaEU,1643
 hnvlearn/make_blobs.py,sha256=goYwreJiQzHZ_d3VoPcYmW6k0Tpr4_6-SxyUEK-hsv4,3306
 hnvlearn/plot_2d_separator.py,sha256=_lqmIdxOOMUpDprlaQMvCrL9D-e2LqM4vpu9sqcmaBg,5487
 hnvlearn/plot_agglomerative.py,sha256=QZ0K91SowTACjpg9WvQYuWwr-la6hrPSRc3rgMtn5Ww,3449
 hnvlearn/plot_animal_tree.py,sha256=s0XT947jorrwhppias2VsJK7Gn0gi0mq7RCbFCAPvPc,890
 hnvlearn/plot_cross_validation.py,sha256=ncdrxE41MGyDDfl0sAnSL1Kt72Kgdsen7aN1Bnm13HY,8867
 hnvlearn/plot_dbscan.py,sha256=pYTwrLvETSNOtbK3BboM6Gk7IaSB_p9W9Dq7Hnxi58Y,1798
@@ -23,11 +23,11 @@
 hnvlearn/plot_pca.py,sha256=kX926ASOGmaNAzw4dJ3KyMjqZ0oHAuCMAdFKwZnr1Ik,4715
 hnvlearn/plot_rbf_svm_parameters.py,sha256=5FGQ2q862XR8F38lgYf9NxQIcd9Sdx7QxbJAPsFpwnc,1178
 hnvlearn/plot_ridge.py,sha256=oe1sF70v1YQu6CAF6X-jV9ne0b2sycGv7n0hpQh4ujE,762
 hnvlearn/plot_scaling.py,sha256=oidDADjQXuCyah1TBPgUMQn0Rl_ELlPaVE1_d9i-P_8,1505
 hnvlearn/plot_tree_nonmonotonous.py,sha256=uh7nUMjmJauRxDCI-yfdfXuGIchUewTYl5e2twiw8SY,894
 hnvlearn/plots.py,sha256=L-aAn4Io4GNSSk3tkaWzoAk3zxA5B2X5-k25sIbhheI,3192
 hnvlearn/tools.py,sha256=duEQLvvWt5yHBvTdS1YO-c2bH4AZOozchy1sKNO1CGg,4801
-hnvlearn-0.0.2.dist-info/METADATA,sha256=G7Q0FjlzX0jup1JRWLMSv_C_xC0FezA4DNMwAIbBEn4,769
-hnvlearn-0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-hnvlearn-0.0.2.dist-info/top_level.txt,sha256=MQeYioSHVaR0bTz7Ya2Xwe8ADRGu_DhVq-a0k5qHaA0,9
-hnvlearn-0.0.2.dist-info/RECORD,,
+hnvlearn-0.0.3.dist-info/METADATA,sha256=ZOjjsY0NUNH-VZvR3WtMj2XudMdQivWlYF28bZhnKFA,769
+hnvlearn-0.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+hnvlearn-0.0.3.dist-info/top_level.txt,sha256=MQeYioSHVaR0bTz7Ya2Xwe8ADRGu_DhVq-a0k5qHaA0,9
+hnvlearn-0.0.3.dist-info/RECORD,,
```

