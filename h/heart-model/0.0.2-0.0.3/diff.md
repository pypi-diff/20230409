# Comparing `tmp/heart-model-0.0.2.tar.gz` & `tmp/heart-model-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heart-model-0.0.2.tar", last modified: Sun Mar 26 15:10:25 2023, max compression
+gzip compressed data, was "heart-model-0.0.3.tar", last modified: Sun Apr  9 16:07:42 2023, max compression
```

## Comparing `heart-model-0.0.2.tar` & `heart-model-0.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-03-26 15:10:25.024942 heart-model-0.0.2/
--rw-rw-rw-   0        0        0      447 2023-03-26 15:00:13.000000 heart-model-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      664 2023-03-26 15:10:25.024399 heart-model-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-26 15:10:24.994120 heart-model-0.0.2/heart_model/
--rw-rw-rw-   0        0        0        7 2023-03-26 15:02:44.000000 heart-model-0.0.2/heart_model/VERSION
--rw-rw-rw-   0        0        0      870 2023-03-19 12:28:33.000000 heart-model-0.0.2/heart_model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-26 15:10:25.001936 heart-model-0.0.2/heart_model/config/
--rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.2/heart_model/config/__init__.py
--rw-rw-rw-   0        0        0     2362 2023-03-26 14:22:26.000000 heart-model-0.0.2/heart_model/config/core.py
--rw-rw-rw-   0        0        0     1179 2023-03-26 14:01:09.000000 heart-model-0.0.2/heart_model/config.yml
-drwxrwxrwx   0        0        0        0 2023-03-26 15:10:25.007134 heart-model-0.0.2/heart_model/datasets/
--rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.2/heart_model/datasets/__init__.py
--rw-rw-rw-   0        0        0   249813 2023-03-26 14:25:31.000000 heart-model-0.0.2/heart_model/datasets/test.csv
--rw-rw-rw-   0        0        0   263185 2023-03-19 07:44:02.000000 heart-model-0.0.2/heart_model/datasets/train.csv
--rw-rw-rw-   0        0        0     2281 2023-03-26 14:07:43.000000 heart-model-0.0.2/heart_model/pipeline.py
--rw-rw-rw-   0        0        0     1090 2023-03-26 11:24:03.000000 heart-model-0.0.2/heart_model/predict.py
-drwxrwxrwx   0        0        0        0 2023-03-26 15:10:25.013117 heart-model-0.0.2/heart_model/processing/
--rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.2/heart_model/processing/__init__.py
--rw-rw-rw-   0        0        0     1913 2023-03-19 21:06:52.000000 heart-model-0.0.2/heart_model/processing/data_manager.py
--rw-rw-rw-   0        0        0     1594 2023-03-20 20:09:04.000000 heart-model-0.0.2/heart_model/processing/features.py
--rw-rw-rw-   0        0        0     2139 2023-03-26 14:32:25.000000 heart-model-0.0.2/heart_model/processing/validation.py
--rw-rw-rw-   0        0        0     2771 2023-03-26 14:07:43.000000 heart-model-0.0.2/heart_model/train_pipeline.py
-drwxrwxrwx   0        0        0        0 2023-03-26 15:10:25.015459 heart-model-0.0.2/heart_model/trained_models/
--rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.2/heart_model/trained_models/__init__.py
--rw-rw-rw-   0        0        0     3738 2023-03-20 20:29:06.000000 heart-model-0.0.2/heart_model/trained_models/heart_model_output_v0.0.1.pkl
-drwxrwxrwx   0        0        0        0 2023-03-26 15:10:24.997942 heart-model-0.0.2/heart_model.egg-info/
--rw-rw-rw-   0        0        0      664 2023-03-26 15:10:24.000000 heart-model-0.0.2/heart_model.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      860 2023-03-26 15:10:24.000000 heart-model-0.0.2/heart_model.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-26 15:10:24.000000 heart-model-0.0.2/heart_model.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      175 2023-03-26 15:10:24.000000 heart-model-0.0.2/heart_model.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-26 15:10:24.000000 heart-model-0.0.2/heart_model.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2176 2023-03-19 18:31:06.000000 heart-model-0.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-03-26 15:10:25.019948 heart-model-0.0.2/requirements/
--rw-rw-rw-   0        0        0      548 2023-03-20 20:22:35.000000 heart-model-0.0.2/requirements/requirements.txt
--rw-rw-rw-   0        0        0      158 2023-03-20 20:06:07.000000 heart-model-0.0.2/requirements/test_requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-26 15:10:25.024942 heart-model-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2126 2023-03-26 15:04:11.000000 heart-model-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-26 15:10:25.023398 heart-model-0.0.2/tests/
--rw-rw-rw-   0        0        0      700 2023-03-26 14:36:25.000000 heart-model-0.0.2/tests/test_features.py
--rw-rw-rw-   0        0        0      580 2023-03-26 14:32:57.000000 heart-model-0.0.2/tests/test_prediction.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:07:42.775098 heart-model-0.0.3/
+-rw-rw-rw-   0        0        0      447 2023-03-26 15:00:13.000000 heart-model-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      664 2023-04-09 16:07:42.774135 heart-model-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-09 16:07:42.742184 heart-model-0.0.3/heart_model/
+-rw-rw-rw-   0        0        0        7 2023-04-09 16:06:28.000000 heart-model-0.0.3/heart_model/VERSION
+-rw-rw-rw-   0        0        0      870 2023-03-19 12:28:33.000000 heart-model-0.0.3/heart_model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:07:42.751160 heart-model-0.0.3/heart_model/config/
+-rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.3/heart_model/config/__init__.py
+-rw-rw-rw-   0        0        0     2410 2023-04-09 15:45:08.000000 heart-model-0.0.3/heart_model/config/core.py
+-rw-rw-rw-   0        0        0     1179 2023-03-26 14:01:09.000000 heart-model-0.0.3/heart_model/config.yml
+drwxrwxrwx   0        0        0        0 2023-04-09 16:07:42.757144 heart-model-0.0.3/heart_model/datasets/
+-rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.3/heart_model/datasets/__init__.py
+-rw-rw-rw-   0        0        0   249813 2023-03-26 14:25:31.000000 heart-model-0.0.3/heart_model/datasets/test.csv
+-rw-rw-rw-   0        0        0   263185 2023-03-19 07:44:02.000000 heart-model-0.0.3/heart_model/datasets/train.csv
+-rw-rw-rw-   0        0        0     2327 2023-04-09 16:05:14.000000 heart-model-0.0.3/heart_model/pipeline.py
+-rw-rw-rw-   0        0        0     1090 2023-03-26 11:24:03.000000 heart-model-0.0.3/heart_model/predict.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:07:42.764125 heart-model-0.0.3/heart_model/processing/
+-rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.3/heart_model/processing/__init__.py
+-rw-rw-rw-   0        0        0     1913 2023-03-19 21:06:52.000000 heart-model-0.0.3/heart_model/processing/data_manager.py
+-rw-rw-rw-   0        0        0     1594 2023-03-20 20:09:04.000000 heart-model-0.0.3/heart_model/processing/features.py
+-rw-rw-rw-   0        0        0     2121 2023-04-09 15:36:53.000000 heart-model-0.0.3/heart_model/processing/validation.py
+-rw-rw-rw-   0        0        0     2771 2023-04-09 16:05:52.000000 heart-model-0.0.3/heart_model/train_pipeline.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:07:42.766120 heart-model-0.0.3/heart_model/trained_models/
+-rw-rw-rw-   0        0        0        0 2023-03-19 09:14:35.000000 heart-model-0.0.3/heart_model/trained_models/__init__.py
+-rw-rw-rw-   0        0        0    79440 2023-04-09 16:06:00.000000 heart-model-0.0.3/heart_model/trained_models/heart_model_output_v0.0.2.pkl
+drwxrwxrwx   0        0        0        0 2023-04-09 16:07:42.749165 heart-model-0.0.3/heart_model.egg-info/
+-rw-rw-rw-   0        0        0      664 2023-04-09 16:07:42.000000 heart-model-0.0.3/heart_model.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      860 2023-04-09 16:07:42.000000 heart-model-0.0.3/heart_model.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 16:07:42.000000 heart-model-0.0.3/heart_model.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      175 2023-04-09 16:07:42.000000 heart-model-0.0.3/heart_model.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-09 16:07:42.000000 heart-model-0.0.3/heart_model.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2169 2023-04-09 15:39:23.000000 heart-model-0.0.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-09 16:07:42.769112 heart-model-0.0.3/requirements/
+-rw-rw-rw-   0        0        0      548 2023-04-09 15:35:34.000000 heart-model-0.0.3/requirements/requirements.txt
+-rw-rw-rw-   0        0        0      158 2023-03-20 20:06:07.000000 heart-model-0.0.3/requirements/test_requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 16:07:42.775098 heart-model-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2126 2023-03-26 15:04:11.000000 heart-model-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:07:42.773104 heart-model-0.0.3/tests/
+-rw-rw-rw-   0        0        0      700 2023-03-26 14:36:25.000000 heart-model-0.0.3/tests/test_features.py
+-rw-rw-rw-   0        0        0      580 2023-03-26 14:32:57.000000 heart-model-0.0.3/tests/test_prediction.py
```

### Comparing `heart-model-0.0.2/PKG-INFO` & `heart-model-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heart-model
-Version: 0.0.2
+Version: 0.0.3
 Summary: Heart decease model package.
 Home-page: https://github.com/Ra7777/heart_model
 Author: Rashid Meylanov
 Author-email: rashmeilll@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `heart-model-0.0.2/heart_model/__init__.py` & `heart-model-0.0.3/heart_model/__init__.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.2/heart_model/config/core.py` & `heart-model-0.0.3/heart_model/config/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,17 @@
     variables_to_rename: Dict[str, str]
     categorical_vars: Sequence[str]
     numerical_vars: Sequence[str]
     numerical_vars_with_na: List[str]
     test_size: float
     random_state: int
     alpha: float
+    C: float
+    n_neighbors: int
+    p: int
     yes_no_vars: List[str]
     yes_no_mappings: Dict[str, int]
 
 
 class Config(BaseModel):
     """Master config object."""
```

### Comparing `heart-model-0.0.2/heart_model/config.yml` & `heart-model-0.0.3/heart_model/config.yml`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.2/heart_model/datasets/test.csv` & `heart-model-0.0.3/heart_model/datasets/test.csv`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.2/heart_model/datasets/train.csv` & `heart-model-0.0.3/heart_model/datasets/train.csv`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.2/heart_model/pipeline.py` & `heart-model-0.0.3/heart_model/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,37 +37,35 @@
         # encode categorical variables using one hot encoding into k-1 variables
         ("categorical_encoder", OneHotEncoder(drop_last=True, variables=config.model_config.categorical_vars)),
         # scale
         ("scaler", StandardScaler()),
     ]
 )
 
-logit_step = [
-    (
+logit_step = (
         "Logit",
         LogisticRegression(
             C=config.model_config.alpha, solver="liblinear", random_state=config.model_config.random_state
         ),
-    ),
-]
+    )
 
 
-k_neighbors_step = [
-    (
+k_neighbors_step = (
         "KNeighbors",
-        KNeighborsClassifier(n_neighbors=config.model_config.n_neighbors, p=config.model_config.p),
-    ),
-]
+        KNeighborsClassifier(
+            n_neighbors=config.model_config.n_neighbors, p=config.model_config.p
+        ),
+    )
 
-svc_step = [
-    (
+svc_step = (
         "SVC",
-        SVC(C=config.model_config.C, random_state=config.model_config.random_state),
-    ),
-]
+        SVC(
+            C=config.model_config.C, random_state=config.model_config.random_state, probability=True
+        ),
+    )
 
-tree_step = [
-    (
+tree_step = (
         "DecisionTree",
-        DecisionTreeClassifier(random_state=config.model_config.random_state),
-    ),
-]
+        DecisionTreeClassifier(
+            random_state=config.model_config.random_state
+        ),
+    )
```

### Comparing `heart-model-0.0.2/heart_model/predict.py` & `heart-model-0.0.3/heart_model/predict.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.2/heart_model/processing/data_manager.py` & `heart-model-0.0.3/heart_model/processing/data_manager.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.2/heart_model/processing/features.py` & `heart-model-0.0.3/heart_model/processing/features.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.2/heart_model/processing/validation.py` & `heart-model-0.0.3/heart_model/processing/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 
 def drop_na_inputs(*, input_data: pd.DataFrame) -> pd.DataFrame:
     """Check model inputs for na values and filter."""
     validated_data = input_data.copy()
     new_vars_with_na = [
         var
         for var in config.model_config.features
-        if var
-        not in config.model_config.numerical_vars_with_na
-        and validated_data[var].isnull().sum() > 0
+        if var not in config.model_config.numerical_vars_with_na and validated_data[var].isnull().sum() > 0
     ]
     validated_data.dropna(subset=new_vars_with_na, inplace=True)
 
     return validated_data
 
 
 def validate_inputs(*, input_data: pd.DataFrame) -> Tuple[pd.DataFrame, Optional[dict]]:
```

### Comparing `heart-model-0.0.2/heart_model/train_pipeline.py` & `heart-model-0.0.3/heart_model/train_pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sklearn.metrics import accuracy_score, roc_auc_score
 from sklearn.model_selection import train_test_split
 
 from heart_model import __version__ as _version
 
 
 def run_training(model_type: int) -> None:
-    if model_type not in range(0, 3):
+    if model_type not in range(0, 4):
         print("argument must be in range [0, 3]")
         exit()
     """Train the model."""
     # Update logs
     log_path = Path(f"{LOG_DIR}/log_{_version}.log")
     if Path.exists(log_path):
         log_path.unlink()
```

### Comparing `heart-model-0.0.2/heart_model.egg-info/PKG-INFO` & `heart-model-0.0.3/heart_model.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heart-model
-Version: 0.0.2
+Version: 0.0.3
 Summary: Heart decease model package.
 Home-page: https://github.com/Ra7777/heart_model
 Author: Rashid Meylanov
 Author-email: rashmeilll@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `heart-model-0.0.2/heart_model.egg-info/SOURCES.txt` & `heart-model-0.0.3/heart_model.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 heart_model/datasets/test.csv
 heart_model/datasets/train.csv
 heart_model/processing/__init__.py
 heart_model/processing/data_manager.py
 heart_model/processing/features.py
 heart_model/processing/validation.py
 heart_model/trained_models/__init__.py
-heart_model/trained_models/heart_model_output_v0.0.1.pkl
+heart_model/trained_models/heart_model_output_v0.0.2.pkl
 requirements/requirements.txt
 requirements/test_requirements.txt
 tests/test_features.py
 tests/test_prediction.py
```

### Comparing `heart-model-0.0.2/pyproject.toml` & `heart-model-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "default:invalid escape sequence:DeprecationWarning",
     # ignore use of unregistered marks, because we use many to test the implementation
     "ignore::_pytest.warning_types.PytestUnknownMarkWarning",
 ]
 
 [tool.black]
 line-length = 119
-target-version = ['py37', 'py38']
+target-version = ['py310']
 include = '\.pyi?$'
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.hg
   | \.mypy_cache
```

### Comparing `heart-model-0.0.2/setup.py` & `heart-model-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.2/tests/test_features.py` & `heart-model-0.0.3/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `heart-model-0.0.2/tests/test_prediction.py` & `heart-model-0.0.3/tests/test_prediction.py`

 * *Files identical despite different names*

