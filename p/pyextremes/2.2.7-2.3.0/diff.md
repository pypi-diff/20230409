# Comparing `tmp/pyextremes-2.2.7.tar.gz` & `tmp/pyextremes-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyextremes-2.2.7.tar", max compression
+gzip compressed data, was "pyextremes-2.3.0.tar", max compression
```

## Comparing `pyextremes-2.2.7.tar` & `pyextremes-2.3.0.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0     1056 2023-01-15 20:59:49.395148 pyextremes-2.2.7/LICENSE
--rw-r--r--   0        0        0     4361 2023-01-15 20:59:49.395148 pyextremes-2.2.7/README.md
--rw-r--r--   0        0        0     2753 2023-01-15 20:59:49.403148 pyextremes-2.2.7/pyproject.toml
--rw-r--r--   0        0        0      533 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/__init__.py
--rw-r--r--   0        0        0    63915 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/eva.py
--rw-r--r--   0        0        0      275 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/extremes/__init__.py
--rw-r--r--   0        0        0     5130 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/extremes/block_maxima.py
--rw-r--r--   0        0        0     3134 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/extremes/extremes.py
--rw-r--r--   0        0        0     3934 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/extremes/peaks_over_threshold.py
--rw-r--r--   0        0        0     5599 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/extremes/return_periods.py
--rw-r--r--   0        0        0     2318 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/extremes/transformation.py
--rw-r--r--   0        0        0      252 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/models/__init__.py
--rw-r--r--   0        0        0    16196 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/models/distribution.py
--rw-r--r--   0        0        0     6562 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/models/model_base.py
--rw-r--r--   0        0        0     8988 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/models/model_emcee.py
--rw-r--r--   0        0        0    10946 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/models/model_mle.py
--rw-r--r--   0        0        0     3586 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/models/models.py
--rw-r--r--   0        0        0        0 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/multivariate/__init__.py
--rw-r--r--   0        0        0        0 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/multivariate/meva.py
--rw-r--r--   0        0        0      444 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/plotting/__init__.py
--rw-r--r--   0        0        0     6661 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/plotting/extremes.py
--rw-r--r--   0        0        0    11766 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/plotting/mcmc.py
--rw-r--r--   0        0        0     2796 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/plotting/probability_plots.py
--rw-r--r--   0        0        0     4381 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/plotting/return_values.py
--rw-r--r--   0        0        0     1523 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/plotting/style.py
--rw-r--r--   0        0        0        1 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/py.typed
--rw-r--r--   0        0        0       88 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/tests/__init__.py
--rw-r--r--   0        0        0     3018 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/tests/ks_test.py
--rw-r--r--   0        0        0     2827 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/tests/test_base.py
--rw-r--r--   0        0        0      365 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/tuning/__init__.py
--rw-r--r--   0        0        0      259 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/tuning/hyperparameters.py
--rw-r--r--   0        0        0      148 2023-01-15 20:59:49.403148 pyextremes-2.2.7/src/pyextremes/tuning/model_comparison.py
--rw-r--r--   0        0        0    32733 2023-01-15 20:59:49.407148 pyextremes-2.2.7/src/pyextremes/tuning/threshold_selection.py
--rw-r--r--   0        0        0     5537 1970-01-01 00:00:00.000000 pyextremes-2.2.7/setup.py
--rw-r--r--   0        0        0     5857 1970-01-01 00:00:00.000000 pyextremes-2.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-04-09 21:48:52.099873 pyextremes-2.3.0/LICENSE
+-rw-r--r--   0        0        0     4380 2023-04-09 21:48:52.099873 pyextremes-2.3.0/README.md
+-rw-r--r--   0        0        0     2774 2023-04-09 21:48:52.103873 pyextremes-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      533 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/__init__.py
+-rw-r--r--   0        0        0    63915 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/eva.py
+-rw-r--r--   0        0        0      275 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/extremes/__init__.py
+-rw-r--r--   0        0        0     5130 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/extremes/block_maxima.py
+-rw-r--r--   0        0        0     3134 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/extremes/extremes.py
+-rw-r--r--   0        0        0     3934 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/extremes/peaks_over_threshold.py
+-rw-r--r--   0        0        0     5599 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/extremes/return_periods.py
+-rw-r--r--   0        0        0     2318 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/extremes/transformation.py
+-rw-r--r--   0        0        0      252 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/models/__init__.py
+-rw-r--r--   0        0        0    16195 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/models/distribution.py
+-rw-r--r--   0        0        0     6562 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/models/model_base.py
+-rw-r--r--   0        0        0     8988 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/models/model_emcee.py
+-rw-r--r--   0        0        0    10946 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/models/model_mle.py
+-rw-r--r--   0        0        0     3586 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/models/models.py
+-rw-r--r--   0        0        0        0 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/multivariate/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/multivariate/meva.py
+-rw-r--r--   0        0        0      444 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/plotting/__init__.py
+-rw-r--r--   0        0        0     6661 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/plotting/extremes.py
+-rw-r--r--   0        0        0    11766 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/plotting/mcmc.py
+-rw-r--r--   0        0        0     2796 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/plotting/probability_plots.py
+-rw-r--r--   0        0        0     4381 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/plotting/return_values.py
+-rw-r--r--   0        0        0     1523 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/plotting/style.py
+-rw-r--r--   0        0        0        1 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/py.typed
+-rw-r--r--   0        0        0       88 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/tests/__init__.py
+-rw-r--r--   0        0        0     3018 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/tests/ks_test.py
+-rw-r--r--   0        0        0     2827 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/tests/test_base.py
+-rw-r--r--   0        0        0      365 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/tuning/__init__.py
+-rw-r--r--   0        0        0      259 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/tuning/hyperparameters.py
+-rw-r--r--   0        0        0      148 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/tuning/model_comparison.py
+-rw-r--r--   0        0        0    32873 2023-04-09 21:48:52.107873 pyextremes-2.3.0/src/pyextremes/tuning/threshold_selection.py
+-rw-r--r--   0        0        0     5827 1970-01-01 00:00:00.000000 pyextremes-2.3.0/PKG-INFO
```

### Comparing `pyextremes-2.2.7/LICENSE` & `pyextremes-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyextremes-2.2.7/README.md` & `pyextremes-2.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     <em>pyextremes</em>
 </p>
 <p align="center">
     <em>Extreme Value Analysis (EVA) in Python</em>
 </p>
 <p align="center">
 <a href="https://github.com/georgebv/pyextremes/actions/workflows/test.yml" target="_blank">
-    <img src="https://github.com/georgebv/pyextremes/actions/workflows/test.yml/badge.svg" alt="Test">
+    <img src="https://github.com/georgebv/pyextremes/actions/workflows/test.yml/badge.svg?event=pull_request" alt="Test">
 </a>
 <a href="https://codecov.io/gh/georgebv/pyextremes" target="_blank">
     <img src="https://codecov.io/gh/georgebv/pyextremes/branch/master/graph/badge.svg" alt="Coverage">
 </a>
 <a href="https://pypi.org/project/pyextremes" target="_blank">
     <img src="https://badge.fury.io/py/pyextremes.svg" alt="PyPI Package">
 </a>
```

### Comparing `pyextremes-2.2.7/pyproject.toml` & `pyextremes-2.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyextremes"
-version = "2.2.7"
+version = "2.3.0"
 description = "Extreme Value Analysis (EVA) in Python"
 license = "MIT"
 authors = ["George Bocharov <bocharovgeorgii@gmail.com>"]
 readme = "README.md"
 homepage = "https://georgebv.github.io/pyextremes"
 repository = "https://github.com/georgebv/pyextremes"
 keywords=[
@@ -20,60 +20,60 @@
 ]
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Hydrology",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
 packages = [
     { include = "pyextremes", from = "src" }
 ]
 include = [
     "LICENSE",
     "README.md",
     "src/pyextremes/py.typed",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 numpy = "^1.19.0"
 scipy = "^1.5.0"
-pandas = "^1.0.0"
+pandas = ">=1.0.0,<3.0.0"
 emcee = "^3.0.3"
 matplotlib = "^3.3.0"
 tqdm = { version = "^4.0.0", optional = true }
 
 [tool.poetry.extras]
 full = ["tqdm"]
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^2.20.0"
+pre-commit = "^3.2.2"
 
 [tool.poetry.group.lint.dependencies]
-black = "^22.8.0"
-pylint = "^2.15.3"
-flake8 = "^5.0.4"
-mypy = "^0.981"
-isort = "^5.10.1"
+black = "^23.0.0"
+pylint = "^2.0.0"
+flake8 = "^6.0.0"
+mypy = "^1.0.0"
+isort = "^5.0.0"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.1.3"
+pytest = "^7.0.0"
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "^1.4.0"
-mkdocs-material = "^8.5.3"
-mkdocs-material-extensions = "^1.0.3"
-mkdocstrings = { version = "^0.19.1", extras = ["python"]}
+mkdocs = "^1.4.2"
+mkdocs-material = "^9.1.6"
+mkdocs-material-extensions = "^1.1.1"
+mkdocstrings = { version = "^0.20.0", extras = ["python"]}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 # Development tool configuration
 
@@ -114,12 +114,13 @@
 [tool.coverage.report]
 exclude_lines = [
     'pragma: no cover',
     'raise AssertionError',
     'raise NotImplementedError',
     'if __name__ == .__main__.:',
     'def __repr__',
+    '    ...',
 ]
 fail_under = 90
 precision = 1
 skip_empty = true
 sort = "-Cover"
```

### Comparing `pyextremes-2.2.7/src/pyextremes/__init__.py` & `pyextremes-2.3.0/src/pyextremes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.2.7"
+__version__ = "2.3.0"
 __all__ = [
     "EVA",
     "get_extremes",
     "get_return_periods",
     "get_model",
     "plot_mean_residual_life",
     "plot_parameter_stability",
```

### Comparing `pyextremes-2.2.7/src/pyextremes/eva.py` & `pyextremes-2.3.0/src/pyextremes/eva.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.2.7/src/pyextremes/extremes/block_maxima.py` & `pyextremes-2.3.0/src/pyextremes/extremes/block_maxima.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.2.7/src/pyextremes/extremes/extremes.py` & `pyextremes-2.3.0/src/pyextremes/extremes/extremes.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.2.7/src/pyextremes/extremes/peaks_over_threshold.py` & `pyextremes-2.3.0/src/pyextremes/extremes/peaks_over_threshold.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.2.7/src/pyextremes/extremes/return_periods.py` & `pyextremes-2.3.0/src/pyextremes/extremes/return_periods.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.2.7/src/pyextremes/extremes/transformation.py` & `pyextremes-2.3.0/src/pyextremes/extremes/transformation.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.2.7/src/pyextremes/models/distribution.py` & `pyextremes-2.3.0/src/pyextremes/models/distribution.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import pandas as pd
 import scipy.stats
 
 logger = logging.getLogger(__name__)
 
 
 class Distribution:
-
     __slots__ = [
         "extremes",
         "distribution",
         "distribution_parameters",
         "fixed_parameters",
         "_fixed_parameters",
         "free_parameters",
```

### Comparing `pyextremes-2.2.7/src/pyextremes/models/model_base.py` & `pyextremes-2.3.0/src/pyextremes/models/model_base.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.2.7/src/pyextremes/models/model_emcee.py` & `pyextremes-2.3.0/src/pyextremes/models/model_emcee.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.2.7/src/pyextremes/models/model_mle.py` & `pyextremes-2.3.0/src/pyextremes/models/model_mle.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.2.7/src/pyextremes/models/models.py` & `pyextremes-2.3.0/src/pyextremes/models/models.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.2.7/src/pyextremes/plotting/extremes.py` & `pyextremes-2.3.0/src/pyextremes/plotting/extremes.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.2.7/src/pyextremes/plotting/mcmc.py` & `pyextremes-2.3.0/src/pyextremes/plotting/mcmc.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.2.7/src/pyextremes/plotting/probability_plots.py` & `pyextremes-2.3.0/src/pyextremes/plotting/probability_plots.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.2.7/src/pyextremes/plotting/return_values.py` & `pyextremes-2.3.0/src/pyextremes/plotting/return_values.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.2.7/src/pyextremes/plotting/style.py` & `pyextremes-2.3.0/src/pyextremes/plotting/style.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.2.7/src/pyextremes/tests/ks_test.py` & `pyextremes-2.3.0/src/pyextremes/tests/ks_test.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.2.7/src/pyextremes/tests/test_base.py` & `pyextremes-2.3.0/src/pyextremes/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pyextremes-2.2.7/src/pyextremes/tuning/threshold_selection.py` & `pyextremes-2.3.0/src/pyextremes/tuning/threshold_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,27 +326,29 @@
             extremes_type=extremes_type,
             num=100,
         )
 
     # List of unique seeds - ensures same seed is not reused across sub-processes
     seeds: typing.List[int] = []
 
-    def _input_generator() -> typing.Generator[
-        typing.Tuple[
-            pd.Series,  # ts (time series)
-            str,  # extremes_type
-            float,  # threshold
-            typing.Union[str, pd.Timedelta],  # r
-            typing.Optional[float],  # alpha
-            int,  # n_samples
-            int,  # seed
-        ],
-        None,
-        None,
-    ]:
+    def _input_generator() -> (
+        typing.Generator[
+            typing.Tuple[
+                pd.Series,  # ts (time series)
+                str,  # extremes_type
+                float,  # threshold
+                typing.Union[str, pd.Timedelta],  # r
+                typing.Optional[float],  # alpha
+                int,  # n_samples
+                int,  # seed
+            ],
+            None,
+            None,
+        ]
+    ):
         for threshold in thresholds:
             seed = np.random.randint(low=0, high=1e6, size=None)
             while seed in seeds:
                 seed = np.random.randint(low=0, high=1e6, size=None)
             seeds.append(seed)
             yield (ts, extremes_type, threshold, r, alpha, n_samples, seed)
 
@@ -614,30 +616,32 @@
     distribution_names: typing.List[str] = []
     for distribution in distributions:
         if isinstance(distribution, str):
             distribution_names.append(distribution)
         else:
             distribution_names.append(distribution.name)
 
-    def _input_generator() -> typing.Generator[
-        typing.Tuple[
-            pd.Series,  # ts (time series)
-            float,  # return_period
-            typing.Union[str, pd.Timedelta],  # return_period_size
-            float,  # threshold
-            typing.Union[str, pd.Timedelta],  # r
-            str,  # extremes_type
-            typing.Union[str, scipy.stats.rv_continuous],  # distribution
-            str,  # distribution_name
-            typing.Optional[float],  # alpha
-            int,  # n_samples
-        ],
-        None,
-        None,
-    ]:
+    def _input_generator() -> (
+        typing.Generator[
+            typing.Tuple[
+                pd.Series,  # ts (time series)
+                float,  # return_period
+                typing.Union[str, pd.Timedelta],  # return_period_size
+                float,  # threshold
+                typing.Union[str, pd.Timedelta],  # r
+                str,  # extremes_type
+                typing.Union[str, scipy.stats.rv_continuous],  # distribution
+                str,  # distribution_name
+                typing.Optional[float],  # alpha
+                int,  # n_samples
+            ],
+            None,
+            None,
+        ]
+    ):
         for distribution, distribution_name in zip(distributions, distribution_names):
             for threshold in thresholds:
                 yield (
                     ts,
                     return_period,
                     return_period_size,
                     threshold,
```

### Comparing `pyextremes-2.2.7/setup.py` & `pyextremes-2.3.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,143 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyextremes
+Version: 2.3.0
+Summary: Extreme Value Analysis (EVA) in Python
+Home-page: https://georgebv.github.io/pyextremes
+License: MIT
+Keywords: statistics,extreme,extreme value analysis,eva,coastal,ocean,marine,environmental,engineering
+Author: George Bocharov
+Author-email: bocharovgeorgii@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Hydrology
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Provides-Extra: full
+Requires-Dist: emcee (>=3.0.3,<4.0.0)
+Requires-Dist: matplotlib (>=3.3.0,<4.0.0)
+Requires-Dist: numpy (>=1.19.0,<2.0.0)
+Requires-Dist: pandas (>=1.0.0,<3.0.0)
+Requires-Dist: scipy (>=1.5.0,<2.0.0)
+Requires-Dist: tqdm (>=4.0.0,<5.0.0) ; extra == "full"
+Project-URL: Repository, https://github.com/georgebv/pyextremes
+Description-Content-Type: text/markdown
+
+<p align="center" style="font-size:40px; margin:0px 10px 0px 10px">
+    <em>pyextremes</em>
+</p>
+<p align="center">
+    <em>Extreme Value Analysis (EVA) in Python</em>
+</p>
+<p align="center">
+<a href="https://github.com/georgebv/pyextremes/actions/workflows/test.yml" target="_blank">
+    <img src="https://github.com/georgebv/pyextremes/actions/workflows/test.yml/badge.svg?event=pull_request" alt="Test">
+</a>
+<a href="https://codecov.io/gh/georgebv/pyextremes" target="_blank">
+    <img src="https://codecov.io/gh/georgebv/pyextremes/branch/master/graph/badge.svg" alt="Coverage">
+</a>
+<a href="https://pypi.org/project/pyextremes" target="_blank">
+    <img src="https://badge.fury.io/py/pyextremes.svg" alt="PyPI Package">
+</a>
+<a href="https://anaconda.org/conda-forge/pyextremes" target="_blank">
+    <img src="https://img.shields.io/conda/vn/conda-forge/pyextremes.svg" alt="Anaconda Package">
+</a>
+</p>
+
+# About
+
+**Documentation:** https://georgebv.github.io/pyextremes/
+
+**License:** [MIT](https://opensource.org/licenses/MIT)
+
+**Support:** [ask a question](https://github.com/georgebv/pyextremes/discussions)
+or [create an issue](https://github.com/georgebv/pyextremes/issues/new/choose),
+any input is appreciated and would help develop the project
+
+**pyextremes** is a Python library aimed at performing univariate
+[Extreme Value Analysis (EVA)](https://en.wikipedia.org/wiki/Extreme_value_theory).
+It provides tools necessary to perform a wide range of tasks required to
+perform EVA, such as:
+
+- extraction of extreme events from time series using methods such as
+Block Maxima (BM) or Peaks Over Threshold (POT)
+- fitting continuous distributions, such as GEVD, GPD, or user-specified
+continous distributions to the extracted extreme events
+- visualization of model inputs, results, and goodness-of-fit statistics
+- estimation of extreme events of given probability or return period
+(e.g. 100-year event) and of corresponding confidence intervals
+- tools assisting with model selection and tuning, such as selection of
+block size in BM and threshold in POT
+
+Check out [this repository](https://github.com/georgebv/pyextremes-notebooks)
+with Jupyter notebooks used to produce figures for this readme
+and for the official documentation.
+
+# Installation
+
+Get latest version from PyPI:
+
+```shell
+pip install pyextremes
+```
+
+Install with optional dependencies:
+
+```shell
+pip install pyextremes[full]
+```
+
+Get latest experimental build from GitHub:
+
+```shell
+pip install "git+https://github.com/georgebv/pyextremes.git#egg=pyextremes"
+```
+
+Get pyextremes for the Anaconda Python distribution:
+
+```shell
+conda install -c conda-forge pyextremes
+```
+
+# Illustrations
+
+<p align="center" style="font-size:20px; margin:10px 10px 0px 10px">
+    <em>Model diagnostic</em>
+</p>
+<p align="center" style="font-size:20px; margin:10px 10px 40px 10px">
+  <img src="https://raw.githubusercontent.com/georgebv/pyextremes-notebooks/master/notebooks/documentation/readme%20figures/diagnostic.png" alt="Diagnostic plot" width="600px">
+</p>
+
+<p align="center" style="font-size:20px; margin:10px 10px 0px 10px">
+    <em>Extreme value extraction</em>
+</p>
+<p align="center" style="font-size:20px; margin:10px 10px 40px 10px">
+  <img src="https://raw.githubusercontent.com/georgebv/pyextremes-notebooks/master/notebooks/documentation/readme%20figures/extremes.png" alt="Diagnostic plot" width="600px">
+</p>
+
+<p align="center" style="font-size:20px; margin:10px 10px 0px 10px">
+    <em>Trace plot</em>
+</p>
+<p align="center" style="font-size:20px; margin:10px 10px 40px 10px">
+  <img src="https://raw.githubusercontent.com/georgebv/pyextremes-notebooks/master/notebooks/documentation/readme%20figures/trace.png" alt="Diagnostic plot" width="600px">
+</p>
+
+<p align="center" style="font-size:20px; margin:10px 10px 0px 10px">
+    <em>Corner plot</em>
+</p>
+<p align="center" style="font-size:20px; margin:10px 10px 40px 10px">
+  <img src="https://raw.githubusercontent.com/georgebv/pyextremes-notebooks/master/notebooks/documentation/readme%20figures/corner.png" alt="Diagnostic plot" width="600px">
+</p>
 
-package_dir = \
-{'': 'src'}
+# Acknowledgements
+I wanted to give kudos to [Jean Toilliez](https://github.com/jtoilliez) who has inspired me to develop this open-source project and who taught me a lot about the extreme value theory. Also big thanks to Max Larson who has introduced me to software development and statistics.
 
-packages = \
-['pyextremes',
- 'pyextremes.extremes',
- 'pyextremes.models',
- 'pyextremes.multivariate',
- 'pyextremes.plotting',
- 'pyextremes.tests',
- 'pyextremes.tuning']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['emcee>=3.0.3,<4.0.0',
- 'matplotlib>=3.3.0,<4.0.0',
- 'numpy>=1.19.0,<2.0.0',
- 'pandas>=1.0.0,<2.0.0',
- 'scipy>=1.5.0,<2.0.0']
-
-extras_require = \
-{'full': ['tqdm>=4.0.0,<5.0.0']}
-
-setup_kwargs = {
-    'name': 'pyextremes',
-    'version': '2.2.7',
-    'description': 'Extreme Value Analysis (EVA) in Python',
-    'long_description': '<p align="center" style="font-size:40px; margin:0px 10px 0px 10px">\n    <em>pyextremes</em>\n</p>\n<p align="center">\n    <em>Extreme Value Analysis (EVA) in Python</em>\n</p>\n<p align="center">\n<a href="https://github.com/georgebv/pyextremes/actions/workflows/test.yml" target="_blank">\n    <img src="https://github.com/georgebv/pyextremes/actions/workflows/test.yml/badge.svg" alt="Test">\n</a>\n<a href="https://codecov.io/gh/georgebv/pyextremes" target="_blank">\n    <img src="https://codecov.io/gh/georgebv/pyextremes/branch/master/graph/badge.svg" alt="Coverage">\n</a>\n<a href="https://pypi.org/project/pyextremes" target="_blank">\n    <img src="https://badge.fury.io/py/pyextremes.svg" alt="PyPI Package">\n</a>\n<a href="https://anaconda.org/conda-forge/pyextremes" target="_blank">\n    <img src="https://img.shields.io/conda/vn/conda-forge/pyextremes.svg" alt="Anaconda Package">\n</a>\n</p>\n\n# About\n\n**Documentation:** https://georgebv.github.io/pyextremes/\n\n**License:** [MIT](https://opensource.org/licenses/MIT)\n\n**Support:** [ask a question](https://github.com/georgebv/pyextremes/discussions)\nor [create an issue](https://github.com/georgebv/pyextremes/issues/new/choose),\nany input is appreciated and would help develop the project\n\n**pyextremes** is a Python library aimed at performing univariate\n[Extreme Value Analysis (EVA)](https://en.wikipedia.org/wiki/Extreme_value_theory).\nIt provides tools necessary to perform a wide range of tasks required to\nperform EVA, such as:\n\n- extraction of extreme events from time series using methods such as\nBlock Maxima (BM) or Peaks Over Threshold (POT)\n- fitting continuous distributions, such as GEVD, GPD, or user-specified\ncontinous distributions to the extracted extreme events\n- visualization of model inputs, results, and goodness-of-fit statistics\n- estimation of extreme events of given probability or return period\n(e.g. 100-year event) and of corresponding confidence intervals\n- tools assisting with model selection and tuning, such as selection of\nblock size in BM and threshold in POT\n\nCheck out [this repository](https://github.com/georgebv/pyextremes-notebooks)\nwith Jupyter notebooks used to produce figures for this readme\nand for the official documentation.\n\n# Installation\n\nGet latest version from PyPI:\n\n```shell\npip install pyextremes\n```\n\nInstall with optional dependencies:\n\n```shell\npip install pyextremes[full]\n```\n\nGet latest experimental build from GitHub:\n\n```shell\npip install "git+https://github.com/georgebv/pyextremes.git#egg=pyextremes"\n```\n\nGet pyextremes for the Anaconda Python distribution:\n\n```shell\nconda install -c conda-forge pyextremes\n```\n\n# Illustrations\n\n<p align="center" style="font-size:20px; margin:10px 10px 0px 10px">\n    <em>Model diagnostic</em>\n</p>\n<p align="center" style="font-size:20px; margin:10px 10px 40px 10px">\n  <img src="https://raw.githubusercontent.com/georgebv/pyextremes-notebooks/master/notebooks/documentation/readme%20figures/diagnostic.png" alt="Diagnostic plot" width="600px">\n</p>\n\n<p align="center" style="font-size:20px; margin:10px 10px 0px 10px">\n    <em>Extreme value extraction</em>\n</p>\n<p align="center" style="font-size:20px; margin:10px 10px 40px 10px">\n  <img src="https://raw.githubusercontent.com/georgebv/pyextremes-notebooks/master/notebooks/documentation/readme%20figures/extremes.png" alt="Diagnostic plot" width="600px">\n</p>\n\n<p align="center" style="font-size:20px; margin:10px 10px 0px 10px">\n    <em>Trace plot</em>\n</p>\n<p align="center" style="font-size:20px; margin:10px 10px 40px 10px">\n  <img src="https://raw.githubusercontent.com/georgebv/pyextremes-notebooks/master/notebooks/documentation/readme%20figures/trace.png" alt="Diagnostic plot" width="600px">\n</p>\n\n<p align="center" style="font-size:20px; margin:10px 10px 0px 10px">\n    <em>Corner plot</em>\n</p>\n<p align="center" style="font-size:20px; margin:10px 10px 40px 10px">\n  <img src="https://raw.githubusercontent.com/georgebv/pyextremes-notebooks/master/notebooks/documentation/readme%20figures/corner.png" alt="Diagnostic plot" width="600px">\n</p>\n\n# Acknowledgements\nI wanted to give kudos to [Jean Toilliez](https://github.com/jtoilliez) who has inspired me to develop this open-source project and who taught me a lot about the extreme value theory. Also big thanks to Max Larson who has introduced me to software development and statistics.\n',
-    'author': 'George Bocharov',
-    'author_email': 'bocharovgeorgii@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://georgebv.github.io/pyextremes',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,64 +1,58 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['pyextremes', 'pyextremes.extremes', 'pyextremes.models',
-'pyextremes.multivariate', 'pyextremes.plotting', 'pyextremes.tests',
-'pyextremes.tuning'] package_data = \ {'': ['*']} install_requires = \
-['emcee>=3.0.3,<4.0.0', 'matplotlib>=3.3.0,<4.0.0', 'numpy>=1.19.0,<2.0.0',
-'pandas>=1.0.0,<2.0.0', 'scipy>=1.5.0,<2.0.0'] extras_require = \ {'full':
-['tqdm>=4.0.0,<5.0.0']} setup_kwargs = { 'name': 'pyextremes', 'version':
-'2.2.7', 'description': 'Extreme Value Analysis (EVA) in Python',
-'long_description': '
-                                \n pyextremes\n
-\n
-                  \n Extreme Value Analysis (EVA) in Python\n
-\n
-\n\n_[Test]\n\n\n_[Coverage]\n\n\n_[PyPI_Package]\n\n\n_[Anaconda_Package]\n\n
-\n\n# About\n\n**Documentation:** https://georgebv.github.io/pyextremes/
-\n\n**License:** [MIT](https://opensource.org/licenses/MIT)\n\n**Support:**
-[ask a question](https://github.com/georgebv/pyextremes/discussions)\nor
-[create an issue](https://github.com/georgebv/pyextremes/issues/new/
-choose),\nany input is appreciated and would help develop the
-project\n\n**pyextremes** is a Python library aimed at performing univariate\n
-[Extreme Value Analysis (EVA)](https://en.wikipedia.org/wiki/
-Extreme_value_theory).\nIt provides tools necessary to perform a wide range of
-tasks required to\nperform EVA, such as:\n\n- extraction of extreme events from
-time series using methods such as\nBlock Maxima (BM) or Peaks Over Threshold
-(POT)\n- fitting continuous distributions, such as GEVD, GPD, or user-
-specified\ncontinous distributions to the extracted extreme events\n-
-visualization of model inputs, results, and goodness-of-fit statistics\n-
-estimation of extreme events of given probability or return period\n(e.g. 100-
-year event) and of corresponding confidence intervals\n- tools assisting with
-model selection and tuning, such as selection of\nblock size in BM and
-threshold in POT\n\nCheck out [this repository](https://github.com/georgebv/
-pyextremes-notebooks)\nwith Jupyter notebooks used to produce figures for this
-readme\nand for the official documentation.\n\n# Installation\n\nGet latest
-version from PyPI:\n\n```shell\npip install pyextremes\n```\n\nInstall with
-optional dependencies:\n\n```shell\npip install pyextremes[full]\n```\n\nGet
-latest experimental build from GitHub:\n\n```shell\npip install "git+https://
-github.com/georgebv/pyextremes.git#egg=pyextremes"\n```\n\nGet pyextremes for
-the Anaconda Python distribution:\n\n```shell\nconda install -c conda-forge
-pyextremes\n```\n\n# Illustrations\n\n
-                             \n Model diagnostic\n
-\n
-                            \n [Diagnostic plot]\n
-\n\n
-                         \n Extreme value extraction\n
-\n
-                            \n [Diagnostic plot]\n
-\n\n
-                                \n Trace plot\n
-\n
-                            \n [Diagnostic plot]\n
-\n\n
-                               \n Corner plot\n
-\n
-                            \n [Diagnostic plot]\n
-\n\n# Acknowledgements\nI wanted to give kudos to [Jean Toilliez](https://
+Metadata-Version: 2.1 Name: pyextremes Version: 2.3.0 Summary: Extreme Value
+Analysis (EVA) in Python Home-page: https://georgebv.github.io/pyextremes
+License: MIT Keywords: statistics,extreme,extreme value
+analysis,eva,coastal,ocean,marine,environmental,engineering Author: George
+Bocharov Author-email: bocharovgeorgii@gmail.com Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
+Scientific/Engineering :: Hydrology Classifier: Topic :: Scientific/Engineering
+:: Mathematics Provides-Extra: full Requires-Dist: emcee (>=3.0.3,<4.0.0)
+Requires-Dist: matplotlib (>=3.3.0,<4.0.0) Requires-Dist: numpy
+(>=1.19.0,<2.0.0) Requires-Dist: pandas (>=1.0.0,<3.0.0) Requires-Dist: scipy
+(>=1.5.0,<2.0.0) Requires-Dist: tqdm (>=4.0.0,<5.0.0) ; extra == "full"
+Project-URL: Repository, https://github.com/georgebv/pyextremes Description-
+Content-Type: text/markdown
+                                  pyextremes
+                    Extreme Value Analysis (EVA) in Python
+              [Test] [Coverage] [PyPI_Package] [Anaconda_Package]
+# About **Documentation:** https://georgebv.github.io/pyextremes/ **License:**
+[MIT](https://opensource.org/licenses/MIT) **Support:** [ask a question](https:
+//github.com/georgebv/pyextremes/discussions) or [create an issue](https://
+github.com/georgebv/pyextremes/issues/new/choose), any input is appreciated and
+would help develop the project **pyextremes** is a Python library aimed at
+performing univariate [Extreme Value Analysis (EVA)](https://en.wikipedia.org/
+wiki/Extreme_value_theory). It provides tools necessary to perform a wide range
+of tasks required to perform EVA, such as: - extraction of extreme events from
+time series using methods such as Block Maxima (BM) or Peaks Over Threshold
+(POT) - fitting continuous distributions, such as GEVD, GPD, or user-specified
+continous distributions to the extracted extreme events - visualization of
+model inputs, results, and goodness-of-fit statistics - estimation of extreme
+events of given probability or return period (e.g. 100-year event) and of
+corresponding confidence intervals - tools assisting with model selection and
+tuning, such as selection of block size in BM and threshold in POT Check out
+[this repository](https://github.com/georgebv/pyextremes-notebooks) with
+Jupyter notebooks used to produce figures for this readme and for the official
+documentation. # Installation Get latest version from PyPI: ```shell pip
+install pyextremes ``` Install with optional dependencies: ```shell pip install
+pyextremes[full] ``` Get latest experimental build from GitHub: ```shell pip
+install "git+https://github.com/georgebv/pyextremes.git#egg=pyextremes" ``` Get
+pyextremes for the Anaconda Python distribution: ```shell conda install -
+c conda-forge pyextremes ``` # Illustrations
+                               Model diagnostic
+                               [Diagnostic plot]
+                           Extreme value extraction
+                               [Diagnostic plot]
+                                  Trace plot
+                               [Diagnostic plot]
+                                  Corner plot
+                               [Diagnostic plot]
+# Acknowledgements I wanted to give kudos to [Jean Toilliez](https://
 github.com/jtoilliez) who has inspired me to develop this open-source project
 and who taught me a lot about the extreme value theory. Also big thanks to Max
-Larson who has introduced me to software development and statistics.\n',
-'author': 'George Bocharov', 'author_email': 'bocharovgeorgii@gmail.com',
-'maintainer': 'None', 'maintainer_email': 'None', 'url': 'https://
-georgebv.github.io/pyextremes', 'package_dir': package_dir, 'packages':
-packages, 'package_data': package_data, 'install_requires': install_requires,
-'extras_require': extras_require, 'python_requires': '>=3.8,<4.0', } setup
-(**setup_kwargs)
+Larson who has introduced me to software development and statistics.
```

