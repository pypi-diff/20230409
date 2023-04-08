# Comparing `tmp/pactus-0.2.0.tar.gz` & `tmp/pactus-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pactus/pactus/dist/.tmp-7mqlts45/pactus-0.2.0.tar", last modified: Thu Jan  5 21:40:45 2023, max compression
+gzip compressed data, was "/home/runner/work/pactus/pactus/dist/.tmp-nfx43jlq/pactus-0.3.0.tar", last modified: Sat Apr  8 22:05:00 2023, max compression
```

## Comparing `pactus-0.2.0.tar` & `pactus-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 21:40:45.491281 pactus-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-01-05 21:40:16.000000 pactus-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2463 2023-01-05 21:40:45.491281 pactus-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      617 2023-01-05 21:40:16.000000 pactus-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 21:40:45.487281 pactus-0.2.0/pactus/
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-01-05 21:40:27.000000 pactus-0.2.0/pactus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1020 2023-01-05 21:40:16.000000 pactus-0.2.0/pactus/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 21:40:45.487281 pactus-0.2.0/pactus/dataset/
--rw-r--r--   0 runner    (1001) docker     (122)       91 2023-01-05 21:40:16.000000 pactus-0.2.0/pactus/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4494 2023-01-05 21:40:16.000000 pactus-0.2.0/pactus/dataset/_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10775 2023-01-05 21:40:16.000000 pactus-0.2.0/pactus/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 21:40:45.491281 pactus-0.2.0/pactus/models/
--rw-r--r--   0 runner    (1001) docker     (122)      797 2023-01-05 21:40:16.000000 pactus-0.2.0/pactus/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-01-05 21:40:16.000000 pactus-0.2.0/pactus/models/decision_tree_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     7129 2023-01-05 21:40:16.000000 pactus-0.2.0/pactus/models/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-01-05 21:40:16.000000 pactus-0.2.0/pactus/models/evaluation_comparison.py
--rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-01-05 21:40:16.000000 pactus-0.2.0/pactus/models/kneighbors_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     5159 2023-01-05 21:40:16.000000 pactus-0.2.0/pactus/models/lstm_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-01-05 21:40:16.000000 pactus-0.2.0/pactus/models/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1215 2023-01-05 21:40:16.000000 pactus-0.2.0/pactus/models/random_forest_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-01-05 21:40:16.000000 pactus-0.2.0/pactus/models/svm_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2883 2023-01-05 21:40:16.000000 pactus-0.2.0/pactus/models/transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     8550 2023-01-05 21:40:16.000000 pactus-0.2.0/pactus/models/transformer_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     4898 2023-01-05 21:40:16.000000 pactus-0.2.0/pactus/models/zoom_transformer_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1719 2023-01-05 21:40:16.000000 pactus-0.2.0/pactus/models/zoomletizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 21:40:45.487281 pactus-0.2.0/pactus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2463 2023-01-05 21:40:45.000000 pactus-0.2.0/pactus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      707 2023-01-05 21:40:45.000000 pactus-0.2.0/pactus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-05 21:40:45.000000 pactus-0.2.0/pactus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-01-05 21:40:45.000000 pactus-0.2.0/pactus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-01-05 21:40:45.000000 pactus-0.2.0/pactus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1479 2023-01-05 21:40:27.000000 pactus-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-05 21:40:45.491281 pactus-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 22:05:00.643139 pactus-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-04-08 22:04:36.000000 pactus-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     2463 2023-04-08 22:05:00.643139 pactus-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      617 2023-04-08 22:04:36.000000 pactus-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 22:05:00.639140 pactus-0.3.0/pactus/
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-04-08 22:04:45.000000 pactus-0.3.0/pactus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1020 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 22:05:00.639140 pactus-0.3.0/pactus/dataset/
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4494 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/dataset/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10775 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 22:05:00.643139 pactus-0.3.0/pactus/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      870 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/decision_tree_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8800 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/evaluation_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/kneighbors_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5137 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/lstm_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1219 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/random_forest_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/svm_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2883 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8591 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/transformer_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1762 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/xgboost_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4898 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/zoom_transformer_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1719 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/zoomletizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 22:05:00.639140 pactus-0.3.0/pactus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2463 2023-04-08 22:05:00.000000 pactus-0.3.0/pactus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-04-08 22:05:00.000000 pactus-0.3.0/pactus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-08 22:05:00.000000 pactus-0.3.0/pactus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-04-08 22:05:00.000000 pactus-0.3.0/pactus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-08 22:05:00.000000 pactus-0.3.0/pactus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-04-08 22:04:45.000000 pactus-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-08 22:05:00.643139 pactus-0.3.0/setup.cfg
```

### Comparing `pactus-0.2.0/LICENSE` & `pactus-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pactus-0.2.0/PKG-INFO` & `pactus-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pactus
-Version: 0.2.0
+Version: 0.3.0
 Summary: Framework to evaluate Trajectory Classification Algorithms
 Author-email: Jorge Morgado Vega <jorge.morgadov@gmail.com>, Gustavo Viera-López <gvieralopez@gmail.com>, Alfredo Reyes <areyes@fisica.uh.cu>
 License: MIT License
         
         Copyright (c) 2022 yupidevs
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pactus-0.2.0/README.md` & `pactus-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pactus-0.2.0/pactus/__init__.py` & `pactus-0.3.0/pactus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from yupi import DiffMethod, Trajectory, WindowType
 from yupi.core import featurizers
 
 from pactus.dataset import Dataset
 from pactus.models import Evaluation, EvaluationComparison
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 __all__ = [
     "Dataset",
     "Evaluation",
     "EvaluationComparison",
     "featurizers",
 ]
```

### Comparing `pactus-0.2.0/pactus/config.py` & `pactus-0.3.0/pactus/config.py`

 * *Files identical despite different names*

### Comparing `pactus-0.2.0/pactus/dataset/_utils.py` & `pactus-0.3.0/pactus/dataset/_utils.py`

 * *Files identical despite different names*

### Comparing `pactus-0.2.0/pactus/dataset/dataset.py` & `pactus-0.3.0/pactus/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `pactus-0.2.0/pactus/models/__init__.py` & `pactus-0.3.0/pactus/models/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 from pactus.models.evaluation_comparison import EvaluationComparison
 from pactus.models.kneighbors_model import KNeighborsModel
 from pactus.models.lstm_model import LSTMModel
 from pactus.models.model import Model
 from pactus.models.random_forest_model import RandomForestModel
 from pactus.models.svm_model import SVMModel
 from pactus.models.transformer_model import TransformerModel
+from pactus.models.xgboost_model import XGBoostModel
 from pactus.models.zoom_transformer_model import ZoomTransformerModel
 
 __all__ = [
     "DecisionTreeModel",
     "Evaluation",
     "EvaluationComparison",
     "KNeighborsModel",
     "Model",
     "RandomForestModel",
     "SVMModel",
     "TransformerModel",
     "ZoomTransformerModel",
+    "XGBoostModel",
     "LSTMModel",
 ]
```

### Comparing `pactus-0.2.0/pactus/models/decision_tree_model.py` & `pactus-0.3.0/pactus/models/decision_tree_model.py`

 * *Files identical despite different names*

### Comparing `pactus-0.2.0/pactus/models/evaluation.py` & `pactus-0.3.0/pactus/models/evaluation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import json
 from pathlib import Path
 from string import Template
 from typing import Any, List
 
 import numpy as np
 from sklearn.metrics import (
@@ -46,39 +48,57 @@
 """
 )
 
 
 class Evaluation:
     def __init__(
         self,
+        dataset_name: str,
+        trajs_ids: List[str],
+        y_true,
+        y_pred,
         model_summary: dict,
-        data: Data,
-        predictions: List[Any],
     ):
-        self.dataset = data.dataset
-        self.trajs = data.trajs
-        self.y_true = data.labels
-        self.y_pred = predictions
+        self.dataset_name = dataset_name
+        self.traj_ids = trajs_ids
+        self.y_true = y_true if not isinstance(y_true, np.ndarray) else y_true.tolist()
+        self.y_pred = y_pred if not isinstance(y_pred, np.ndarray) else y_pred.tolist()
         self.model_summary = model_summary
         self.classes = list(set(self.y_true))
         self.classes.sort()
 
         self._confusion_matrix = confusion_matrix(
             self.y_true, self.y_pred, labels=self.classes
         ).T
         pre, rec, f_sc, sup = precision_recall_fscore_support(
-            self.y_true, self.y_pred, labels=self.classes
+            self.y_true, self.y_pred, labels=self.classes, zero_division=0
         )
         self.precision = np.asarray(pre)
         self.recall = np.asarray(rec)
         self.f_score = np.asarray(f_sc)
         self.support = np.asarray(sup)
 
         self.acc_overall = accuracy_score(self.y_true, self.y_pred, normalize=True)
-        self.f1_score = f1_score(self.y_true, self.y_pred, average="weighted")
+        self.f1_score = f1_score(
+            self.y_true, self.y_pred, average="macro", zero_division=0
+        )
+
+    @staticmethod
+    def from_data(
+        data: Data,
+        predictions: List[Any],
+        model_summary: dict,
+    ) -> Evaluation:
+        return Evaluation(
+            dataset_name=data.dataset.name,
+            trajs_ids=[traj.traj_id for traj in data.trajs if traj.traj_id is not None],
+            y_true=data.labels,
+            y_pred=predictions,
+            model_summary=model_summary,
+        )
 
     def _conf_matrix_perc(self) -> np.ndarray:
         c_matrix = self._confusion_matrix.astype("float")
         for i in range(c_matrix.shape[0]):
             c_matrix[:, i] /= c_matrix[:, i].sum()
         return c_matrix
 
@@ -112,55 +132,88 @@
         """Show the general statistics."""
         print("\nGeneral statistics:\n")
         print(f"Accuracy: {self.acc_overall:.3f}")
         print(f"F1-score: {self.f1_score:.3f}")
         print(f"Mean precision: {self.precision.mean():.3f}")
         print(f"Mean recall: {self.recall.mean():.3f}")
 
-    def save(self, file_name: str) -> Path:
-        """Save the evaluation to a file.
+    @staticmethod
+    def load(file_name: str) -> Evaluation:
+        """Loads an evaluation from a file.
 
         Parameters
         ----------
         file_name : str
-            The name of the file to save the evaluation to. It
+            The name of the file to load the evaluation from. It
             must end with '.json'.
 
         Returns
         -------
-        Path
-            The path to the saved file.
+        Evaluation
+            The loaded evaluation.
+        """
+
+        if not file_name.endswith(".json"):
+            raise ValueError("file_name extension must be '.json'")
+
+        with open(file_name, "r", encoding="utf-8") as data_fd:
+            data = json.load(data_fd)
+
+        assert len(data["indices"]) == len(data["y_pred"])
+        ds_name = data["dataset_name"]
+        indices = data["indices"]
+        y_pred = data["y_pred"]
+        y_true = data["y_true"]
+        summary = data["model_summary"]
+        return Evaluation(
+            dataset_name=ds_name,
+            trajs_ids=indices,
+            y_pred=y_pred,
+            y_true=y_true,
+            model_summary=summary,
+        )
+
+    def save(self, file_name: str):
+        """Save the evaluation to a file.
+
+        Parameters
+        ----------
+        file_name : str
+            The name of the file to save the evaluation to. It
+            must end with '.json'.
         """
 
         if not file_name.endswith(".json"):
             raise ValueError("file_name extension must be '.json'")
 
         data = {
-            "indices": [
-                int(traj.traj_id) for traj in self.trajs if traj.traj_id is not None
-            ],
-            "predictions": self.y_pred,
+            "dataset_name": self.dataset_name,
+            "indices": self.traj_ids,
+            "y_pred": self.y_pred,
+            "y_true": self.y_true,
+            "classes": self.classes,
             "model_summary": self.model_summary,
         }
 
-        assert len(data["indices"]) == len(data["predictions"])
+        assert len(data["indices"]) == len(data["y_pred"])
 
-        file_path = _get_path(config.DS_EVALS_DIR, self.dataset.name) / file_name
+        if "/" in file_name:
+            dir_name = "/".join(file_name.split("/")[:-1])
+            dir_path = Path(dir_name)
+            dir_path.mkdir(parents=True, exist_ok=True)
 
-        with open(file_path, "w", encoding="utf-8") as data_fd:
+        with open(file_name, "w", encoding="utf-8") as data_fd:
             json.dump(data, data_fd, ensure_ascii=False, indent=4)
 
-        return file_path
-
     def to_markdown(self) -> str:
         """Evaluation summary in markdown style."""
         summary = self.model_summary.copy()
         model_name = summary.pop("name")
         ans = "# Evaluation results\n\n"
-        ans += f"**Dataset:** {self.dataset.name} \\\n"
+        ans += f"**Dataset:** {self.dataset_name} \\\n"
         ans += f"**Model:** {model_name}\n"
         ans += "\n## Model Summary\n\n"
         for param, val in summary.items():
             ans += f"- `{param} = {val}`\n"
         ans += "\n## Confusion Matrix\n\n"
 
         c_matrix = self._conf_matrix_perc()
@@ -201,15 +254,15 @@
                 cls_name=classes[i],
                 cls_vals=" & ".join(str_row),
                 cls_prec=f"{str(round(self.precision[i] * 100, 2))} \\%",
             )
             cls_rows += row
 
         ans += LATEX_CM_TEMPLATE.substitute(
-            caption=f"Confusion matrix for {model_name}. Dataset: {self.dataset.name}",
+            caption=f"Confusion matrix for {model_name}. Dataset: {self.dataset_name}",
             model_name=model_name,
             c_cols="c" * len(classes),
             c_line_top=str(len(classes) + 1),
             cls_count=len(classes),
             cls_head=" & ".join(classes),
             cls_rows=cls_rows,
             recalls=" & ".join(
```

### Comparing `pactus-0.2.0/pactus/models/evaluation_comparison.py` & `pactus-0.3.0/pactus/models/evaluation_comparison.py`

 * *Files identical despite different names*

### Comparing `pactus-0.2.0/pactus/models/kneighbors_model.py` & `pactus-0.3.0/pactus/models/kneighbors_model.py`

 * *Files identical despite different names*

### Comparing `pactus-0.2.0/pactus/models/lstm_model.py` & `pactus-0.3.0/pactus/models/lstm_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,17 @@
         super().__init__(NAME)
         self.masking_value = cfg.MASK_VALUE if masking_value is None else masking_value
         self.encoder: Union[LabelEncoder, None] = None
         self.model: keras.Secuential
         self.max_len = 0
         metrics = ["accuracy"] if metrics is None else metrics
         self.units = [128, 64] if units is None else units
-        self.set_summary(loss=loss, optimizer=optimizer, metrics=metrics, **kwargs)
+        kwargs.update(dict(loss=loss, optimizer=optimizer, metrics=metrics))
+        self.compile_args = kwargs
+        self.set_summary(**self.compile_args)
 
     def _get_x_data(self, max_len: int, trajs: List[Trajectory]) -> np.ndarray:
         _X = np.empty(
             (
                 len(trajs),
                 max_len,
                 trajs[0].dim + 1,  # all pos dim plust time
@@ -76,19 +78,15 @@
         model.add(
             layers.Bidirectional(
                 layers.LSTM(32, input_shape=(max_len, traj_dim)), merge_mode="ave"
             )
         )
         model.add(layers.Dense(15, activation="relu"))
         model.add(layers.Dense(n_classes, activation="softmax"))
-        model.compile(
-            loss="sparse_categorical_crossentropy",
-            optimizer="rmsprop",
-            metrics=["accuracy"],
-        )
+        model.compile(**self.compile_args)
         return model
 
     def _prepare_data(self, data: Data) -> Tuple[np.ndarray, np.ndarray]:
         self.encoder = LabelEncoder()
         self.encoder.fit(data.labels)
         encoded_labels = self.encoder.transform(data.labels)
         y_data = np.array(encoded_labels)
@@ -98,15 +96,15 @@
         return x_data, y_data
 
     def train(
         self,
         data: Data,
         cross_validation=0,
         epochs=10,
-        batch_size=1,
+        batch_size=None,
         validation_split=None,
         callbacks: Union[list, None] = None,
         checkpoint: Union[keras.callbacks.ModelCheckpoint, None] = None,
     ):
         if cross_validation != 0:
             logging.warning("Cross validation is not supported yet for lstm")
         self.set_summary(epochs=epochs, validation_split=validation_split)
@@ -144,8 +142,8 @@
 
     def evaluate(self, data: Data) -> Evaluation:
         assert self.encoder is not None, "Encoder is not set."
         x_data = self._get_x_data(self.max_len, data.trajs)
         preds = self.model.predict(x_data)
         preds = [pred.argmax() for pred in preds]
         evals = self.encoder.inverse_transform(preds)
-        return Evaluation(self.summary, data, evals)
+        return Evaluation.from_data(data, evals, self.summary)
```

### Comparing `pactus-0.2.0/pactus/models/model.py` & `pactus-0.3.0/pactus/models/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,8 +53,8 @@
         return self.predict(data)
 
     def evaluate(self, data: Data) -> Evaluation:
         """Evaluate the trained model"""
 
         logging.info("Evaluating the %s model", self.name)
         predictions = self._predict(data)
-        return Evaluation(self.summary, data, predictions)
+        return Evaluation.from_data(data, predictions, self.summary)
```

### Comparing `pactus-0.2.0/pactus/models/random_forest_model.py` & `pactus-0.3.0/pactus/models/random_forest_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 
 class RandomForestModel(Model):
     """Implementation of a Random Forest Classifier."""
 
     def __init__(self, featurizer: featurizers.Featurizer, **kwargs):
         super().__init__(NAME)
         self.featurizer = featurizer
-        self.rfc = RandomForestClassifier(**kwargs)
+        self.model = RandomForestClassifier(**kwargs)
         self.grid: GridSearchCV
         self.set_summary(**kwargs)
 
     def train(self, data: Data, cross_validation: int = 0):
         self.set_summary(cross_validation=cross_validation)
         x_data = data.featurize(self.featurizer)
-        self.grid = GridSearchCV(self.rfc, {}, cv=cross_validation, verbose=3)
+        self.grid = GridSearchCV(self.model, {}, cv=cross_validation, verbose=3)
         self.grid.fit(x_data, data.labels)
 
     def predict(self, data: Data) -> List[Any]:
         x_data = data.featurize(self.featurizer)
         return self.grid.predict(x_data)
 
     def predict_single(self, traj: Trajectory) -> Any:
```

### Comparing `pactus-0.2.0/pactus/models/svm_model.py` & `pactus-0.3.0/pactus/models/svm_model.py`

 * *Files identical despite different names*

### Comparing `pactus-0.2.0/pactus/models/transformer.py` & `pactus-0.3.0/pactus/models/transformer.py`

 * *Files identical despite different names*

### Comparing `pactus-0.2.0/pactus/models/transformer_model.py` & `pactus-0.3.0/pactus/models/transformer_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             epochs=epochs,
             validation_split=validation_split,
             batch_size=batch_size,
         )
         self.encoder = None
         self.labels = data.labels
         x_train, y_train = self._get_input_data(data)
-        n_classes = len(data.dataset.classes)
+        n_classes = len(data.classes)
         input_shape = x_train.shape[1:]
         callbacks = DEFAULT_CALLBACKS.copy() if callbacks is None else callbacks
         model_path = None
         if checkpoint is not None:
             callbacks.append(checkpoint)
             if Path(checkpoint.filepath).exists():
                 logging.info("Loading model from checkpoint %s", checkpoint.filepath)
@@ -105,15 +105,17 @@
             model = (
                 self._get_model(
                     n_classes,
                     input_shape,
                     mask=self.mask_value,
                 )
                 if model_path is None
-                else keras.models.load_model(model_path, custom_objects={'TransformerBlock':TransformerBlock})
+                else keras.models.load_model(
+                    model_path, custom_objects={"TransformerBlock": TransformerBlock}
+                )
             )
             model.fit(
                 x_train,
                 y_train,
                 validation_split=validation_split,
                 epochs=epochs,
                 batch_size=batch_size,
@@ -227,8 +229,8 @@
 
     def evaluate(self, data: Data) -> Evaluation:
         assert self.encoder is not None, "Encoder is not set."
         x_data, _ = self._get_input_data(data)
         preds = self.model.predict(x_data)
         preds = [pred.argmax() for pred in preds]
         evals = self.encoder.inverse_transform(preds)
-        return Evaluation(self.summary, data, evals)
+        return Evaluation.from_data(data, evals, self.summary)
```

### Comparing `pactus-0.2.0/pactus/models/zoom_transformer_model.py` & `pactus-0.3.0/pactus/models/zoom_transformer_model.py`

 * *Files identical despite different names*

### Comparing `pactus-0.2.0/pactus/models/zoomletizer.py` & `pactus-0.3.0/pactus/models/zoomletizer.py`

 * *Files identical despite different names*

### Comparing `pactus-0.2.0/pactus.egg-info/PKG-INFO` & `pactus-0.3.0/pactus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pactus
-Version: 0.2.0
+Version: 0.3.0
 Summary: Framework to evaluate Trajectory Classification Algorithms
 Author-email: Jorge Morgado Vega <jorge.morgadov@gmail.com>, Gustavo Viera-López <gvieralopez@gmail.com>, Alfredo Reyes <areyes@fisica.uh.cu>
 License: MIT License
         
         Copyright (c) 2022 yupidevs
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pactus-0.2.0/pactus.egg-info/SOURCES.txt` & `pactus-0.3.0/pactus.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,9 +18,10 @@
 pactus/models/kneighbors_model.py
 pactus/models/lstm_model.py
 pactus/models/model.py
 pactus/models/random_forest_model.py
 pactus/models/svm_model.py
 pactus/models/transformer.py
 pactus/models/transformer_model.py
+pactus/models/xgboost_model.py
 pactus/models/zoom_transformer_model.py
 pactus/models/zoomletizer.py
```

### Comparing `pactus-0.2.0/pyproject.toml` & `pactus-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pactus"
-version = "0.2.0"
+version = "0.3.0"
 description = "Framework to evaluate Trajectory Classification Algorithms"
 readme = "README.md"
 authors = [
     { name = "Jorge Morgado Vega", email = "jorge.morgadov@gmail.com" },
     { name = "Gustavo Viera-López", email = "gvieralopez@gmail.com" },
     { name = "Alfredo Reyes", email = "areyes@fisica.uh.cu" },
 ]
@@ -16,14 +16,15 @@
 ]
 keywords = ["trajectory", "classification"]
 dependencies = [
     "numpy >= 1.20.0",
     "yupi >= 0.11.2",
     "tensorflow >= 2.9.1",
     "scikit-learn >= 1.1.1",
+    "xgboost >= 1.7.4",
     "GitPython >= 3.1.29"
 ]
 requires-python = ">=3.8"
 
 [project.optional-dependencies]
 dev = ["black", "pylint", "bumpver", "isort", "pytest"]
 
@@ -37,15 +38,15 @@
 [tool.black]
 target-version = ["py37"]
 
 [tool.pylint."MESSAGES CONTROL"]
 max-line-length = 88
 
 [tool.bumpver]
-current_version = "0.2.0"
+current_version = "0.3.0"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
```

