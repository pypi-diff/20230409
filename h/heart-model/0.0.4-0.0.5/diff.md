# Comparing `tmp/heart-model-0.0.4.tar.gz` & `tmp/heart-model-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heart-model-0.0.4.tar", last modified: Sun Apr  9 16:30:36 2023, max compression
+gzip compressed data, was "heart-model-0.0.5.tar", last modified: Sun Apr  9 17:19:46 2023, max compression
```

## Comparing `heart-model-0.0.4.tar` & `heart-model-0.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 16:30:36.760371 heart-model-0.0.4/
--rw-rw-rw-   0        0        0      447 2023-03-26 15:00:13.000000 heart-model-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      664 2023-04-09 16:30:36.759372 heart-model-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-09 16:30:36.723956 heart-model-0.0.4/heart_model/
--rw-rw-rw-   0        0        0        7 2023-04-09 16:29:37.000000 heart-model-0.0.4/heart_model/VERSION
--rw-rw-rw-   0        0        0      870 2023-03-19 12:28:33.000000 heart-model-0.0.4/heart_model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:30:36.735438 heart-model-0.0.4/heart_model/config/
--rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.4/heart_model/config/__init__.py
--rw-rw-rw-   0        0        0     2410 2023-04-09 15:45:08.000000 heart-model-0.0.4/heart_model/config/core.py
--rw-rw-rw-   0        0        0     1179 2023-03-26 14:01:09.000000 heart-model-0.0.4/heart_model/config.yml
-drwxrwxrwx   0        0        0        0 2023-04-09 16:30:36.742418 heart-model-0.0.4/heart_model/datasets/
--rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.4/heart_model/datasets/__init__.py
--rw-rw-rw-   0        0        0   249813 2023-03-26 14:25:31.000000 heart-model-0.0.4/heart_model/datasets/test.csv
--rw-rw-rw-   0        0        0   263185 2023-03-19 07:44:02.000000 heart-model-0.0.4/heart_model/datasets/train.csv
--rw-rw-rw-   0        0        0     2183 2023-04-09 16:26:50.000000 heart-model-0.0.4/heart_model/pipeline.py
--rw-rw-rw-   0        0        0     1090 2023-03-26 11:24:03.000000 heart-model-0.0.4/heart_model/predict.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:30:36.747437 heart-model-0.0.4/heart_model/processing/
--rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.4/heart_model/processing/__init__.py
--rw-rw-rw-   0        0        0     1913 2023-03-19 21:06:52.000000 heart-model-0.0.4/heart_model/processing/data_manager.py
--rw-rw-rw-   0        0        0     1594 2023-03-20 20:09:04.000000 heart-model-0.0.4/heart_model/processing/features.py
--rw-rw-rw-   0        0        0     2121 2023-04-09 15:36:53.000000 heart-model-0.0.4/heart_model/processing/validation.py
--rw-rw-rw-   0        0        0     2771 2023-04-09 16:26:50.000000 heart-model-0.0.4/heart_model/train_pipeline.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:30:36.749400 heart-model-0.0.4/heart_model/trained_models/
--rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.4/heart_model/trained_models/__init__.py
--rw-rw-rw-   0        0        0    79440 2023-04-09 16:06:00.000000 heart-model-0.0.4/heart_model/trained_models/heart_model_output_v0.0.4.pkl
-drwxrwxrwx   0        0        0        0 2023-04-09 16:30:36.732446 heart-model-0.0.4/heart_model.egg-info/
--rw-rw-rw-   0        0        0      664 2023-04-09 16:30:36.000000 heart-model-0.0.4/heart_model.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      860 2023-04-09 16:30:36.000000 heart-model-0.0.4/heart_model.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 16:30:36.000000 heart-model-0.0.4/heart_model.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2023-04-09 16:30:36.000000 heart-model-0.0.4/heart_model.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-09 16:30:36.000000 heart-model-0.0.4/heart_model.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2169 2023-04-09 15:39:23.000000 heart-model-0.0.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-09 16:30:36.753395 heart-model-0.0.4/requirements/
--rw-rw-rw-   0        0        0      546 2023-04-09 16:25:34.000000 heart-model-0.0.4/requirements/requirements.txt
--rw-rw-rw-   0        0        0      158 2023-03-20 20:06:07.000000 heart-model-0.0.4/requirements/test_requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 16:30:36.760371 heart-model-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2126 2023-03-26 15:04:11.000000 heart-model-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:30:36.758377 heart-model-0.0.4/tests/
--rw-rw-rw-   0        0        0      700 2023-03-26 14:36:25.000000 heart-model-0.0.4/tests/test_features.py
--rw-rw-rw-   0        0        0      580 2023-03-26 14:32:57.000000 heart-model-0.0.4/tests/test_prediction.py
+drwxrwxrwx   0        0        0        0 2023-04-09 17:19:46.641522 heart-model-0.0.5/
+-rw-rw-rw-   0        0        0      447 2023-03-26 15:00:13.000000 heart-model-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      664 2023-04-09 17:19:46.641522 heart-model-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-09 17:19:46.609878 heart-model-0.0.5/heart_model/
+-rw-rw-rw-   0        0        0        7 2023-04-09 17:19:21.000000 heart-model-0.0.5/heart_model/VERSION
+-rw-rw-rw-   0        0        0      870 2023-03-19 12:28:33.000000 heart-model-0.0.5/heart_model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 17:19:46.625501 heart-model-0.0.5/heart_model/config/
+-rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.5/heart_model/config/__init__.py
+-rw-rw-rw-   0        0        0     2410 2023-04-09 15:45:08.000000 heart-model-0.0.5/heart_model/config/core.py
+-rw-rw-rw-   0        0        0     1179 2023-03-26 14:01:09.000000 heart-model-0.0.5/heart_model/config.yml
+drwxrwxrwx   0        0        0        0 2023-04-09 17:19:46.632511 heart-model-0.0.5/heart_model/datasets/
+-rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.5/heart_model/datasets/__init__.py
+-rw-rw-rw-   0        0        0   249813 2023-03-26 14:25:31.000000 heart-model-0.0.5/heart_model/datasets/test.csv
+-rw-rw-rw-   0        0        0   263185 2023-03-19 07:44:02.000000 heart-model-0.0.5/heart_model/datasets/train.csv
+-rw-rw-rw-   0        0        0     2183 2023-04-09 17:08:21.000000 heart-model-0.0.5/heart_model/pipeline.py
+-rw-rw-rw-   0        0        0     1090 2023-03-26 11:24:03.000000 heart-model-0.0.5/heart_model/predict.py
+drwxrwxrwx   0        0        0        0 2023-04-09 17:19:46.641522 heart-model-0.0.5/heart_model/processing/
+-rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.5/heart_model/processing/__init__.py
+-rw-rw-rw-   0        0        0     1913 2023-03-19 21:06:52.000000 heart-model-0.0.5/heart_model/processing/data_manager.py
+-rw-rw-rw-   0        0        0     1594 2023-03-20 20:09:04.000000 heart-model-0.0.5/heart_model/processing/features.py
+-rw-rw-rw-   0        0        0     2121 2023-04-09 15:36:53.000000 heart-model-0.0.5/heart_model/processing/validation.py
+-rw-rw-rw-   0        0        0     2968 2023-04-09 17:08:21.000000 heart-model-0.0.5/heart_model/train_pipeline.py
+drwxrwxrwx   0        0        0        0 2023-04-09 17:19:46.641522 heart-model-0.0.5/heart_model/trained_models/
+-rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.5/heart_model/trained_models/__init__.py
+-rw-rw-rw-   0        0        0     3738 2023-04-09 17:07:07.000000 heart-model-0.0.5/heart_model/trained_models/heart_model_output_v0.0.4.pkl
+drwxrwxrwx   0        0        0        0 2023-04-09 17:19:46.609878 heart-model-0.0.5/heart_model.egg-info/
+-rw-rw-rw-   0        0        0      664 2023-04-09 17:19:46.000000 heart-model-0.0.5/heart_model.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      860 2023-04-09 17:19:46.000000 heart-model-0.0.5/heart_model.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 17:19:46.000000 heart-model-0.0.5/heart_model.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2023-04-09 17:19:46.000000 heart-model-0.0.5/heart_model.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-09 17:19:46.000000 heart-model-0.0.5/heart_model.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2169 2023-04-09 15:39:23.000000 heart-model-0.0.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-09 17:19:46.641522 heart-model-0.0.5/requirements/
+-rw-rw-rw-   0        0        0      546 2023-04-09 16:25:34.000000 heart-model-0.0.5/requirements/requirements.txt
+-rw-rw-rw-   0        0        0      158 2023-03-20 20:06:07.000000 heart-model-0.0.5/requirements/test_requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 17:19:46.657148 heart-model-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2126 2023-03-26 15:04:11.000000 heart-model-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 17:19:46.641522 heart-model-0.0.5/tests/
+-rw-rw-rw-   0        0        0      700 2023-03-26 14:36:25.000000 heart-model-0.0.5/tests/test_features.py
+-rw-rw-rw-   0        0        0      580 2023-03-26 14:32:57.000000 heart-model-0.0.5/tests/test_prediction.py
```

### Comparing `heart-model-0.0.4/PKG-INFO` & `heart-model-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heart-model
-Version: 0.0.4
+Version: 0.0.5
 Summary: Heart decease model package.
 Home-page: https://github.com/Ra7777/heart_model
 Author: Rashid Meylanov
 Author-email: rashmeilll@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `heart-model-0.0.4/heart_model/__init__.py` & `heart-model-0.0.5/heart_model/__init__.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.4/heart_model/config/core.py` & `heart-model-0.0.5/heart_model/config/core.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.4/heart_model/config.yml` & `heart-model-0.0.5/heart_model/config.yml`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.4/heart_model/datasets/test.csv` & `heart-model-0.0.5/heart_model/datasets/test.csv`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.4/heart_model/datasets/train.csv` & `heart-model-0.0.5/heart_model/datasets/train.csv`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.4/heart_model/pipeline.py` & `heart-model-0.0.5/heart_model/pipeline.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.4/heart_model/predict.py` & `heart-model-0.0.5/heart_model/predict.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.4/heart_model/processing/data_manager.py` & `heart-model-0.0.5/heart_model/processing/data_manager.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.4/heart_model/processing/features.py` & `heart-model-0.0.5/heart_model/processing/features.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.4/heart_model/processing/validation.py` & `heart-model-0.0.5/heart_model/processing/validation.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.4/heart_model/train_pipeline.py` & `heart-model-0.0.5/heart_model/train_pipeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import logging
 import sys
+import typing as t
 from pathlib import Path
 
 from config.core import LOG_DIR, config
 from pipeline import heart_pipe, k_neighbors_step, logit_step, svc_step, tree_step
 from processing.data_manager import load_dataset, save_pipeline
 from sklearn.metrics import accuracy_score, roc_auc_score
 from sklearn.model_selection import train_test_split
 
 from heart_model import __version__ as _version
 
 
-def run_training(model_type: int) -> None:
+def run_training(model_type: int) -> dict:
     if model_type not in range(0, 4):
         print("argument must be in range [0, 3]")
         exit()
     """Train the model."""
     # Update logs
     log_path = Path(f"{LOG_DIR}/log_{_version}.log")
     if Path.exists(log_path):
@@ -35,16 +36,18 @@
         test_size=config.model_config.test_size,
         # we are setting the random seed here
         # for reproducibility
         random_state=config.model_config.random_state,
     )
 
     steps = [logit_step, k_neighbors_step, svc_step, tree_step]
+    names = ["Logistic Regression", "K Neighbors", "SVC", "Tree"]
     # fit model
     heart_pipe.steps.append(steps[model_type])
+    results: t.Dict[str, t.Any] = {"model_type": names[model_type], "version": _version}
     heart_pipe.fit(X_train, y_train)
 
     # make predictions for train set
     class_ = heart_pipe.predict(X_train)
     pred = heart_pipe.predict_proba(X_train)[:, 1]
 
     # determine train accuracy and roc-auc
@@ -71,11 +74,12 @@
     print()
 
     logging.info(f"test accuracy: {test_accuracy}")
     logging.info(f"test roc-auc: {test_roc_auc}")
 
     # persist trained model
     save_pipeline(pipeline_to_persist=heart_pipe)
+    return results
 
 
 if __name__ == "__main__":
     run_training(int(sys.argv[1]))
```

### Comparing `heart-model-0.0.4/heart_model.egg-info/PKG-INFO` & `heart-model-0.0.5/heart_model.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heart-model
-Version: 0.0.4
+Version: 0.0.5
 Summary: Heart decease model package.
 Home-page: https://github.com/Ra7777/heart_model
 Author: Rashid Meylanov
 Author-email: rashmeilll@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `heart-model-0.0.4/heart_model.egg-info/SOURCES.txt` & `heart-model-0.0.5/heart_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.4/pyproject.toml` & `heart-model-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.4/requirements/requirements.txt` & `heart-model-0.0.5/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.4/setup.py` & `heart-model-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.4/tests/test_features.py` & `heart-model-0.0.5/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.4/tests/test_prediction.py` & `heart-model-0.0.5/tests/test_prediction.py`

 * *Files identical despite different names*

