# Comparing `tmp/heart-model-0.0.7.tar.gz` & `tmp/heart-model-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heart-model-0.0.7.tar", last modified: Sun Apr  9 17:44:40 2023, max compression
+gzip compressed data, was "heart-model-0.0.8.tar", last modified: Sun Apr  9 17:54:07 2023, max compression
```

## Comparing `heart-model-0.0.7.tar` & `heart-model-0.0.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 17:44:40.350971 heart-model-0.0.7/
--rw-rw-rw-   0        0        0      447 2023-03-26 15:00:13.000000 heart-model-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      664 2023-04-09 17:44:40.350971 heart-model-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-09 17:44:40.319698 heart-model-0.0.7/heart_model/
--rw-rw-rw-   0        0        0        7 2023-04-09 17:44:28.000000 heart-model-0.0.7/heart_model/VERSION
--rw-rw-rw-   0        0        0      870 2023-03-19 12:28:33.000000 heart-model-0.0.7/heart_model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 17:44:40.335321 heart-model-0.0.7/heart_model/config/
--rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.7/heart_model/config/__init__.py
--rw-rw-rw-   0        0        0     2410 2023-04-09 15:45:08.000000 heart-model-0.0.7/heart_model/config/core.py
--rw-rw-rw-   0        0        0     1179 2023-03-26 14:01:09.000000 heart-model-0.0.7/heart_model/config.yml
-drwxrwxrwx   0        0        0        0 2023-04-09 17:44:40.335321 heart-model-0.0.7/heart_model/datasets/
--rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.7/heart_model/datasets/__init__.py
--rw-rw-rw-   0        0        0   249813 2023-03-26 14:25:31.000000 heart-model-0.0.7/heart_model/datasets/test.csv
--rw-rw-rw-   0        0        0   263185 2023-03-19 07:44:02.000000 heart-model-0.0.7/heart_model/datasets/train.csv
--rw-rw-rw-   0        0        0     2183 2023-04-09 17:08:21.000000 heart-model-0.0.7/heart_model/pipeline.py
--rw-rw-rw-   0        0        0     1090 2023-03-26 11:24:03.000000 heart-model-0.0.7/heart_model/predict.py
-drwxrwxrwx   0        0        0        0 2023-04-09 17:44:40.350971 heart-model-0.0.7/heart_model/processing/
--rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.7/heart_model/processing/__init__.py
--rw-rw-rw-   0        0        0     1913 2023-03-19 21:06:52.000000 heart-model-0.0.7/heart_model/processing/data_manager.py
--rw-rw-rw-   0        0        0     1594 2023-03-20 20:09:04.000000 heart-model-0.0.7/heart_model/processing/features.py
--rw-rw-rw-   0        0        0     2121 2023-04-09 15:36:53.000000 heart-model-0.0.7/heart_model/processing/validation.py
--rw-rw-rw-   0        0        0     3004 2023-04-09 17:42:38.000000 heart-model-0.0.7/heart_model/train_pipeline.py
-drwxrwxrwx   0        0        0        0 2023-04-09 17:44:40.350971 heart-model-0.0.7/heart_model/trained_models/
--rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.7/heart_model/trained_models/__init__.py
--rw-rw-rw-   0        0        0     3738 2023-04-09 17:07:07.000000 heart-model-0.0.7/heart_model/trained_models/heart_model_output_v0.0.7.pkl
-drwxrwxrwx   0        0        0        0 2023-04-09 17:44:40.335321 heart-model-0.0.7/heart_model.egg-info/
--rw-rw-rw-   0        0        0      664 2023-04-09 17:44:40.000000 heart-model-0.0.7/heart_model.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      860 2023-04-09 17:44:40.000000 heart-model-0.0.7/heart_model.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 17:44:40.000000 heart-model-0.0.7/heart_model.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2023-04-09 17:44:40.000000 heart-model-0.0.7/heart_model.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-09 17:44:40.000000 heart-model-0.0.7/heart_model.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2169 2023-04-09 15:39:23.000000 heart-model-0.0.7/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-09 17:44:40.350971 heart-model-0.0.7/requirements/
--rw-rw-rw-   0        0        0      546 2023-04-09 16:25:34.000000 heart-model-0.0.7/requirements/requirements.txt
--rw-rw-rw-   0        0        0      158 2023-03-20 20:06:07.000000 heart-model-0.0.7/requirements/test_requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 17:44:40.366565 heart-model-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2126 2023-03-26 15:04:11.000000 heart-model-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 17:44:40.350971 heart-model-0.0.7/tests/
--rw-rw-rw-   0        0        0      700 2023-03-26 14:36:25.000000 heart-model-0.0.7/tests/test_features.py
--rw-rw-rw-   0        0        0      580 2023-03-26 14:32:57.000000 heart-model-0.0.7/tests/test_prediction.py
+drwxrwxrwx   0        0        0        0 2023-04-09 17:54:07.598243 heart-model-0.0.8/
+-rw-rw-rw-   0        0        0      447 2023-03-26 15:00:13.000000 heart-model-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      664 2023-04-09 17:54:07.598243 heart-model-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-09 17:54:07.566996 heart-model-0.0.8/heart_model/
+-rw-rw-rw-   0        0        0        7 2023-04-09 17:53:47.000000 heart-model-0.0.8/heart_model/VERSION
+-rw-rw-rw-   0        0        0      870 2023-03-19 12:28:33.000000 heart-model-0.0.8/heart_model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 17:54:07.566996 heart-model-0.0.8/heart_model/config/
+-rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.8/heart_model/config/__init__.py
+-rw-rw-rw-   0        0        0     2410 2023-04-09 15:45:08.000000 heart-model-0.0.8/heart_model/config/core.py
+-rw-rw-rw-   0        0        0     1179 2023-03-26 14:01:09.000000 heart-model-0.0.8/heart_model/config.yml
+drwxrwxrwx   0        0        0        0 2023-04-09 17:54:07.582619 heart-model-0.0.8/heart_model/datasets/
+-rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.8/heart_model/datasets/__init__.py
+-rw-rw-rw-   0        0        0   249813 2023-03-26 14:25:31.000000 heart-model-0.0.8/heart_model/datasets/test.csv
+-rw-rw-rw-   0        0        0   263185 2023-03-19 07:44:02.000000 heart-model-0.0.8/heart_model/datasets/train.csv
+-rw-rw-rw-   0        0        0     2183 2023-04-09 17:08:21.000000 heart-model-0.0.8/heart_model/pipeline.py
+-rw-rw-rw-   0        0        0     1090 2023-03-26 11:24:03.000000 heart-model-0.0.8/heart_model/predict.py
+drwxrwxrwx   0        0        0        0 2023-04-09 17:54:07.582619 heart-model-0.0.8/heart_model/processing/
+-rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.8/heart_model/processing/__init__.py
+-rw-rw-rw-   0        0        0     1913 2023-03-19 21:06:52.000000 heart-model-0.0.8/heart_model/processing/data_manager.py
+-rw-rw-rw-   0        0        0     1594 2023-03-20 20:09:04.000000 heart-model-0.0.8/heart_model/processing/features.py
+-rw-rw-rw-   0        0        0     2121 2023-04-09 15:36:53.000000 heart-model-0.0.8/heart_model/processing/validation.py
+-rw-rw-rw-   0        0        0     3159 2023-04-09 17:53:16.000000 heart-model-0.0.8/heart_model/train_pipeline.py
+drwxrwxrwx   0        0        0        0 2023-04-09 17:54:07.582619 heart-model-0.0.8/heart_model/trained_models/
+-rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.8/heart_model/trained_models/__init__.py
+-rw-rw-rw-   0        0        0     3738 2023-04-09 17:07:07.000000 heart-model-0.0.8/heart_model/trained_models/heart_model_output_v0.0.8.pkl
+drwxrwxrwx   0        0        0        0 2023-04-09 17:54:07.566996 heart-model-0.0.8/heart_model.egg-info/
+-rw-rw-rw-   0        0        0      664 2023-04-09 17:54:07.000000 heart-model-0.0.8/heart_model.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      860 2023-04-09 17:54:07.000000 heart-model-0.0.8/heart_model.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 17:54:07.000000 heart-model-0.0.8/heart_model.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2023-04-09 17:54:07.000000 heart-model-0.0.8/heart_model.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-09 17:54:07.000000 heart-model-0.0.8/heart_model.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2169 2023-04-09 15:39:23.000000 heart-model-0.0.8/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-09 17:54:07.598243 heart-model-0.0.8/requirements/
+-rw-rw-rw-   0        0        0      546 2023-04-09 16:25:34.000000 heart-model-0.0.8/requirements/requirements.txt
+-rw-rw-rw-   0        0        0      158 2023-03-20 20:06:07.000000 heart-model-0.0.8/requirements/test_requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 17:54:07.598243 heart-model-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2126 2023-03-26 15:04:11.000000 heart-model-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 17:54:07.598243 heart-model-0.0.8/tests/
+-rw-rw-rw-   0        0        0      700 2023-03-26 14:36:25.000000 heart-model-0.0.8/tests/test_features.py
+-rw-rw-rw-   0        0        0      580 2023-03-26 14:32:57.000000 heart-model-0.0.8/tests/test_prediction.py
```

### Comparing `heart-model-0.0.7/PKG-INFO` & `heart-model-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heart-model
-Version: 0.0.7
+Version: 0.0.8
 Summary: Heart decease model package.
 Home-page: https://github.com/Ra7777/heart_model
 Author: Rashid Meylanov
 Author-email: rashmeilll@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `heart-model-0.0.7/heart_model/__init__.py` & `heart-model-0.0.8/heart_model/__init__.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.7/heart_model/config/core.py` & `heart-model-0.0.8/heart_model/config/core.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.7/heart_model/config.yml` & `heart-model-0.0.8/heart_model/config.yml`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.7/heart_model/datasets/test.csv` & `heart-model-0.0.8/heart_model/datasets/test.csv`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.7/heart_model/datasets/train.csv` & `heart-model-0.0.8/heart_model/datasets/train.csv`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.7/heart_model/pipeline.py` & `heart-model-0.0.8/heart_model/pipeline.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.7/heart_model/predict.py` & `heart-model-0.0.8/heart_model/predict.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.7/heart_model/processing/data_manager.py` & `heart-model-0.0.8/heart_model/processing/data_manager.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.7/heart_model/processing/features.py` & `heart-model-0.0.8/heart_model/processing/features.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.7/heart_model/processing/validation.py` & `heart-model-0.0.8/heart_model/processing/validation.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.7/heart_model/train_pipeline.py` & `heart-model-0.0.8/heart_model/train_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 from heart_model import __version__ as _version
 
 
 def run_training(model_type: int) -> dict:
     if model_type not in range(0, 4):
         print("argument must be in range [0, 3]")
-        exit()
+        results: t.Dict[str, t.Any] = {"model_type": "no model", "msg": "argument must be in range [0, 3]", "version": _version}
+        return results
     """Train the model."""
     # Update logs
     log_path = Path(f"{LOG_DIR}/log_{_version}.log")
     if Path.exists(log_path):
         log_path.unlink()
     logging.basicConfig(filename=log_path, level=logging.DEBUG)
 
@@ -39,15 +40,15 @@
         random_state=config.model_config.random_state,
     )
 
     steps = [logit_step, k_neighbors_step, svc_step, tree_step]
     names = ["Logistic Regression", "K Neighbors", "SVC", "Tree"]
     # fit model
     heart_pipe.steps.append(steps[model_type])
-    results: t.Dict[str, t.Any] = {"model_type": names[model_type], "version": _version}
+    results: t.Dict[str, t.Any] = {"model_type": names[model_type], "msg": "no msg", "version": _version}
     heart_pipe.fit(X_train, y_train)
 
     # make predictions for train set
     class_ = heart_pipe.predict(X_train)
     pred = heart_pipe.predict_proba(X_train)[:, 1]
 
     # determine train accuracy and roc-auc
```

### Comparing `heart-model-0.0.7/heart_model/trained_models/heart_model_output_v0.0.7.pkl` & `heart-model-0.0.8/heart_model/trained_models/heart_model_output_v0.0.8.pkl`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.7/heart_model.egg-info/PKG-INFO` & `heart-model-0.0.8/heart_model.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heart-model
-Version: 0.0.7
+Version: 0.0.8
 Summary: Heart decease model package.
 Home-page: https://github.com/Ra7777/heart_model
 Author: Rashid Meylanov
 Author-email: rashmeilll@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `heart-model-0.0.7/heart_model.egg-info/SOURCES.txt` & `heart-model-0.0.8/heart_model.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 heart_model/datasets/test.csv
 heart_model/datasets/train.csv
 heart_model/processing/__init__.py
 heart_model/processing/data_manager.py
 heart_model/processing/features.py
 heart_model/processing/validation.py
 heart_model/trained_models/__init__.py
-heart_model/trained_models/heart_model_output_v0.0.7.pkl
+heart_model/trained_models/heart_model_output_v0.0.8.pkl
 requirements/requirements.txt
 requirements/test_requirements.txt
 tests/test_features.py
 tests/test_prediction.py
```

### Comparing `heart-model-0.0.7/pyproject.toml` & `heart-model-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.7/requirements/requirements.txt` & `heart-model-0.0.8/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.7/setup.py` & `heart-model-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.7/tests/test_features.py` & `heart-model-0.0.8/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.7/tests/test_prediction.py` & `heart-model-0.0.8/tests/test_prediction.py`

 * *Files identical despite different names*

