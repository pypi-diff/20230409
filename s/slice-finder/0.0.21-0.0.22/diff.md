# Comparing `tmp/slice_finder-0.0.21.tar.gz` & `tmp/slice_finder-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slice_finder-0.0.21.tar", max compression
+gzip compressed data, was "slice_finder-0.0.22.tar", max compression
```

## Comparing `slice_finder-0.0.21.tar` & `slice_finder-0.0.22.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1174 2023-04-04 15:56:25.623355 slice_finder-0.0.21/pyproject.toml
--rw-r--r--   0        0        0     4445 2023-04-04 15:53:38.376421 slice_finder-0.0.21/README.md
--rw-r--r--   0        0        0      549 2023-04-03 05:00:12.310797 slice_finder-0.0.21/src/slice_finder/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 09:24:08.253976 slice_finder-0.0.21/src/slice_finder/data_connectors/__init__.py
--rw-r--r--   0        0        0      858 2023-04-03 05:51:36.019217 slice_finder-0.0.21/src/slice_finder/data_connectors/data_connector.py
--rw-r--r--   0        0        0     3045 2023-04-04 07:33:10.145135 slice_finder-0.0.21/src/slice_finder/data_connectors/pandas.py
--rw-r--r--   0        0        0        0 2023-03-30 19:25:35.554085 slice_finder-0.0.21/src/slice_finder/data_structures/__init__.py
--rw-r--r--   0        0        0      682 2023-04-03 05:51:47.754811 slice_finder-0.0.21/src/slice_finder/data_structures/data_structure.py
--rw-r--r--   0        0        0     3739 2023-04-04 07:45:11.368148 slice_finder-0.0.21/src/slice_finder/data_structures/flattened_lgbm.py
--rw-r--r--   0        0        0     4514 2023-04-04 07:18:14.009023 slice_finder-0.0.21/src/slice_finder/data_structures/lgbm.py
--rw-r--r--   0        0        0        0 2023-04-02 07:03:40.459724 slice_finder-0.0.21/src/slice_finder/slice_finders/__init__.py
--rw-r--r--   0        0        0     7366 2023-04-04 07:09:52.233788 slice_finder-0.0.21/src/slice_finder/slice_finders/ga.py
--rw-r--r--   0        0        0     1015 2023-04-04 07:16:53.561879 slice_finder-0.0.21/src/slice_finder/slice_finders/slice_finder.py
--rw-r--r--   0        0        0     3275 2023-04-04 06:41:58.754093 slice_finder-0.0.21/src/slice_finder/slice_finders/uniform.py
--rw-r--r--   0        0        0      885 2023-04-04 06:41:58.754093 slice_finder-0.0.21/src/slice_finder/types.py
--rw-r--r--   0        0        0     5350 1970-01-01 00:00:00.000000 slice_finder-0.0.21/setup.py
--rw-r--r--   0        0        0     5224 1970-01-01 00:00:00.000000 slice_finder-0.0.21/PKG-INFO
+-rw-r--r--   0        0        0     1273 2023-04-09 04:37:31.881727 slice_finder-0.0.22/pyproject.toml
+-rw-r--r--   0        0        0     4917 2023-04-09 04:37:31.863709 slice_finder-0.0.22/README.md
+-rw-r--r--   0        0        0      633 2023-04-09 04:37:31.882833 slice_finder-0.0.22/src/slice_finder/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-31 09:24:08.253976 slice_finder-0.0.22/src/slice_finder/data_connectors/__init__.py
+-rw-r--r--   0        0        0      868 2023-04-09 04:37:31.883463 slice_finder-0.0.22/src/slice_finder/data_connectors/data_connector.py
+-rw-r--r--   0        0        0     3054 2023-04-09 04:37:31.884467 slice_finder-0.0.22/src/slice_finder/data_connectors/pandas.py
+-rw-r--r--   0        0        0        0 2023-03-30 19:25:35.554085 slice_finder-0.0.22/src/slice_finder/data_structures/__init__.py
+-rw-r--r--   0        0        0      821 2023-04-09 04:37:31.884467 slice_finder-0.0.22/src/slice_finder/data_structures/data_structure.py
+-rw-r--r--   0        0        0     3727 2023-04-09 04:37:31.885470 slice_finder-0.0.22/src/slice_finder/data_structures/flattened_lgbm.py
+-rw-r--r--   0        0        0     4505 2023-04-09 04:37:31.886467 slice_finder-0.0.22/src/slice_finder/data_structures/lgbm.py
+-rw-r--r--   0        0        0        0 2023-04-02 07:03:40.459724 slice_finder-0.0.22/src/slice_finder/slice_finders/__init__.py
+-rw-r--r--   0        0        0      969 2023-04-09 04:37:31.886467 slice_finder-0.0.22/src/slice_finder/slice_finders/ga.py
+-rw-r--r--   0        0        0     7233 2023-04-09 04:37:31.887468 slice_finder-0.0.22/src/slice_finder/slice_finders/ga_mu_plus_lambda.py
+-rw-r--r--   0        0        0     1015 2023-04-09 04:37:31.887468 slice_finder-0.0.22/src/slice_finder/slice_finders/slice_finder.py
+-rw-r--r--   0        0        0     3618 2023-04-09 04:37:31.888924 slice_finder-0.0.22/src/slice_finder/slice_finders/uniform.py
+-rw-r--r--   0        0        0     1090 2023-04-09 04:37:31.889465 slice_finder-0.0.22/src/slice_finder/types.py
+-rw-r--r--   0        0        0     5838 1970-01-01 00:00:00.000000 slice_finder-0.0.22/setup.py
+-rw-r--r--   0        0        0     5761 1970-01-01 00:00:00.000000 slice_finder-0.0.22/PKG-INFO
```

### Comparing `slice_finder-0.0.21/pyproject.toml` & `slice_finder-0.0.22/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 [tool.poetry]
 name = "slice_finder"
-version = "0.0.21"
-description = "A Framework for Slice Discovery"
+version = "0.0.22"
+description = "Slice Finder: A Framework for Slice Discovery"
 authors = ["Igal Leikin <igaloly@gmail.com>"]
-keywords = ["slice discovery", "slice finding"]
+keywords = [
+  "slice discovery", 
+  "slice detection", 
+  "subgroup discovery", 
+  "subgroup detection", 
+  "slice finding"
+]
 readme = "README.md"
 homepage = "https://github.com/igaloly/slice_finder"
 repository = "https://github.com/igaloly/slice_finder"
 license = "MIT"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `slice_finder-0.0.21/README.md` & `slice_finder-0.0.22/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Slice Finder: A Framework for Slice Discovery
 
 Slice Finder is a versatile and highly configurable framework designed for the discovery of explainable, anomalous data subsets, which exhibit substantially divergent metric values in comparison to the entire dataset.
 
+> To illustrate, imagine that you have developed a model for identifying fraudulent transactions. The model's overall accuracy across the entire dataset is 0.95. However, when transactions occur more than 100 km away from the previous transaction and involve cash (2 filters), the model's accuracy drops significantly to 0.54.
+
 Slice Finder is a crucial investigative instrument, as it enables data scientists to identify regions where their models demonstrate over- or under-performance.
 
 ## Algorithmic achievements
 * Tackling data quantization can be complex, particularly when transforming continuous values into discrete space. Slice Finder overcomes this challenge by fitting an LGBM model to the data and extracting the appropriate splits.
 * As the number of filters, columns, and values increases, so does the combinatorial search space. Slice Finder addresses this issue in two ways:
     * By fitting an LGBM model to the data, the most critical fields and values for splitting are identified, significantly reducing the search space.
     * Incorporating Genetic Algorithm heuristics to converge towards global minima/maxima, which outperforms both the time-consuming "try-it-all" approach and uniform filter sampling in terms of efficiency and results.
@@ -22,21 +24,21 @@
 pip install slice_finder
 ```
 
 # Quick Start
 ```python
 import pandas as pd
 from sklearn import metrics
-from slice_finder import GASliceFinder, FlattenedLGBMDataStructure, PandasDataConnector
+from slice_finder import GAMuPlusLambdaSliceFinder, FlattenedLGBMDataStructure, PandasDataConnector
 
 # Load data
 df = pd.read_csv('your_data.csv')
 
 # Initialize Genetic Algorithm Slice Finder with desired data connector and data structure
-slice_finder = GASliceFinder(
+slice_finder = GAMuPlusLambdaSliceFinder(
     data_connector=PandasDataConnector(
         df=df,
         X_cols=df.drop(['pred', 'target'], axis=1).columns,
         y_col='target',
         pred_col='pred',
     ),
     data_structure=FlattenedLGBMDataStructure(),
@@ -75,19 +77,20 @@
 
 More data structures will be added as demand grows.
 
 You can create your custom data structure by extending the base classes and implementing the necessary methods.
 
 ## Slice Finders
 Built in:
-* `GASliceFinder` - Utilizes `eaMuPlusLambda` evolutionary algorithm to search for the most anomalous slice
+* `GAMuPlusLambdaSliceFinder` - Utilizes `eaMuPlusLambda` evolutionary algorithm to search for the most anomalous slice
 * `UniformSliceFinder` - Utilizes uniform sampling out of the data structure
 
 Base classes:
 * `SliceFinder` - Base slice finder
+* `GASliceFinder` - Extends `SliceFinder` and enables the use of genetic algorithms as search heuristics
 
 More algorithms will be added based on demand. 
 
 You can create your custom data structure by extending the base class and implementing the necessary methods.
 
 ## Metrics
 Metrics are passed as functions to the `find_extreme` method, allowing you to use any metric or implement your custom logic.
```

### Comparing `slice_finder-0.0.21/src/slice_finder/__init__.py` & `slice_finder-0.0.22/src/slice_finder/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from slice_finder.data_connectors.data_connector import DataConnector
 from slice_finder.data_connectors.pandas import PandasDataConnector
 from slice_finder.data_structures.data_structure import DataStructure
 from slice_finder.data_structures.flattened_lgbm import FlattenedLGBMDataStructure
 from slice_finder.data_structures.lgbm import LGBMDataStructure
 from slice_finder.slice_finders.ga import GASliceFinder
+from slice_finder.slice_finders.ga_mu_plus_lambda import GAMuPlusLambdaSliceFinder
 from slice_finder.slice_finders.slice_finder import SliceFinder
 from slice_finder.slice_finders.uniform import UniformSliceFinder
```

### Comparing `slice_finder-0.0.21/src/slice_finder/data_connectors/data_connector.py` & `slice_finder-0.0.22/src/slice_finder/data_connectors/data_connector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from abc import abstractmethod, abstractproperty
+
 from slice_finder.types import Filter
 
+
 class DataConnector:
     """Base DataConnector object."""
 
     @abstractmethod
     def init(
         self,
         verbose: bool,
         random_state: int | None,
     ):
         """This function will run in the __init__ of the the SliceFinder."""
         raise NotImplementedError()
 
     @abstractmethod
-    def filter(self, filters: list[Filter]):
+    def filter(self, data, filters: list[Filter]):
         """Custom login to filter the data."""
         raise NotImplementedError()
 
     @abstractproperty
     def data(self):
         """Return the data object."""
         raise NotImplementedError()
```

### Comparing `slice_finder-0.0.21/src/slice_finder/data_connectors/pandas.py` & `slice_finder-0.0.22/src/slice_finder/data_connectors/pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         self,
         df: pd.DataFrame,
         X_cols: list[str],
         y_col: str,
         pred_col: str,
     ):
         """Data connector for using Pandas."""
-        
+
         self.df = df
         self.X_cols = X_cols
         self.y_col = y_col
         self.pred_col = pred_col
 
     def init(self, verbose=False, random_state: int | None = None):
         self.verbose = verbose
@@ -36,17 +36,17 @@
         elif filter.operator == "<=":
             return df[filter.feature] <= filter.value
         elif filter.operator == ">=":
             return df[filter.feature] >= filter.value
         else:
             raise ValueError(f"Invalid operator {filter.operator}")
 
-    def filter(self, filters: list[Filter]) -> pd.DataFrame:
+    def filter(self, data: pd.DataFrame, filters: list[Filter]) -> pd.DataFrame:
         """Filters the DF."""
-        df = self.df
+        df = data
         for filter in filters:
             df = df[self.apply_filter(df, filter)]
         return df
 
     def parse_data_for_lgbm(
         self,
         max_unique_to_categorical: int,
```

### Comparing `slice_finder-0.0.21/src/slice_finder/data_structures/flattened_lgbm.py` & `slice_finder-0.0.22/src/slice_finder/data_structures/flattened_lgbm.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,26 +26,26 @@
     def __init__(
         self,
         task: str | None = None,
         tree_kwargs: dict[str, Any] | None = None,
         max_unique_to_categorical=200,
     ):
         """Flattened representation of an LGBM tree.
-    
+
         Notes:
         Currenly works only as a base class for flattened LGBM.
 
         Args:
             task: `classification`, `regression` or None. If None, huristic
             will be applied to determine the task
             tree_kwargs: Parameters for the tree
             max_unique_to_categorical: The number of maximum unique values
             for a column to be considered as categorical
         """
-        
+
         super().__init__(
             task=task,
             tree_kwargs=tree_kwargs,
             max_unique_to_categorical=max_unique_to_categorical,
         )
         self.flattened_rules_tree: dict[str, FlattenedRulesTreeValue] | None = None
```

### Comparing `slice_finder-0.0.21/src/slice_finder/data_structures/lgbm.py` & `slice_finder-0.0.22/src/slice_finder/data_structures/lgbm.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         Args:
             task: `classification`, `regression` or None. If None, huristic
             will be applied to determine the task
             tree_kwargs: Parameters for the tree
             max_unique_to_categorical: The number of maximum unique values
             for a column to be considered as categorical
         """
-         
+
         self.task = task
         self.tree: LGBMRegressor | LGBMClassifier | None = None
         self.tree_dict: dict[str, Any] | None = None
         self.rules_trees: list[RulesTree] = []
         self.tree_kwargs = tree_kwargs if tree_kwargs is not None else {}
         self.max_unique_to_categorical = max_unique_to_categorical
         if "max_cat_to_onehot" not in self.tree_kwargs:
```

### Comparing `slice_finder-0.0.21/src/slice_finder/slice_finders/ga.py` & `slice_finder-0.0.22/src/slice_finder/slice_finders/ga_mu_plus_lambda.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,23 @@
-import random
 from typing import Any, Callable
 
 from deap import base, creator, tools
 from deap.algorithms import varOr
 import numpy as np
 
-from slice_finder.slice_finders.slice_finder import SliceFinder
-from slice_finder.types import Extreme, Filter
+from slice_finder.slice_finders.ga import GASliceFinder
+from slice_finder.types import Extreme
 
 
-class GASliceFinder(SliceFinder):
-    """Slice discovery using Genetic algorithm."""
+class GAMuPlusLambdaSliceFinder(GASliceFinder):
+    """Slice discovery using Genetic algorithm.
+    Utilized Mu Plus Lambda algorithm.
+    https://deap.readthedocs.io/en/master/api/algo.html#deap.algorithms.eaMuPlusLambda"""
 
-    def create_individual(self, n_filters: int):
-        return creator.Individual(self.data_structure.get_n_filters(n_filters))
-
-    def mutate_individual(self, individual: list[Filter], indpb: float):
-        for i in range(len(individual)):
-            if random.random() < indpb:
-                individual[i] = self.data_structure.get_filter()
-        return (individual,)
-
-    def eval_individual(
-        self,
-        individual: list[Filter],
-        **kwargs,
-    ):
-        df = self.data_connector.filter(individual)
-        if len(df) < len(self.data_connector.data) * kwargs["min_size"]:
-            return None
-        return (kwargs["metric"](df),)
-
-    def eaMuPlusLambda(
+    def run(
         self,
         population: list[Any],
         toolbox: base.Toolbox,
         mu: int,
         lambda_: int,
         cxpb: float,
         mutpb: float,
@@ -103,19 +85,25 @@
                 return population, logbook
 
         return population, logbook
 
     def create_toolbox(
         self,
         maximize: bool,
-        n_filters: int,
+        n_filters: int | tuple[int, int],
         metric: Callable[[Any], float],
         min_size: float,
         indpb: float,
     ):
+        try:
+            del creator.FitnessMulti
+            del creator.Individual
+        except Exception:
+            pass
+
         creator.create("FitnessMulti", base.Fitness, weights=(1.0,) if maximize else (-1.0,))
         creator.create("Individual", list, fitness=creator.FitnessMulti)
 
         toolbox = base.Toolbox()
         toolbox.register("individual", self.create_individual, n_filters)
         toolbox.register("population", tools.initRepeat, list, toolbox.individual)
         toolbox.register("mate", tools.cxTwoPoint)
@@ -132,44 +120,47 @@
 
     def find_extreme(
         self,
         metric: Callable[[Any], float],
         n_hof=1,
         n_generations=10,
         population_size=100,
-        n_filters=3,
+        n_filters: int | tuple[int, int] = 3,
         maximize=False,
         min_size=0.01,
         cxpb=0.5,
         mutpb=0.5,
         indpb=0.5,
         maximum=float("inf"),
         minimum=float("-inf"),
     ) -> list[Extreme]:
         """Find slice with an extreme value of a metric.
-        
+
         Args:
             metric: Function that calculates metric value over data
             n_hof: Number of extreme values to return
             n_generations: Number of iterations
             population_size: Population size
-            n_filters: Number of filters
+            n_filters: Number of filters. If a tuple, that means n_filters
+            will be in the range [n_filters[0], n_filters[1]]
             maximize: `True` will search for the maximum
             metric's value, and `False` will search for the minumum one
             min_size: Minimum size, in fractions, of the extreme subset.
             For exmaple, for value `0.01`, the extreme subset must be at
             least 1% of the data, in size, to be considered
             cxpb: The probability of mating two individuals
             mutpb: The probability of mutating an individual
             indpb: The probability of mutating an individual's filter
             maximum: If `maximize`, and `maximum` is reached, the search stoppes
             minimum: If `not maximize`, and `minimum` is reached, the search stoppes
         """
 
-        if n_filters <= 1:
+        if (isinstance(n_filters, int) and n_filters <= 1) or (
+            isinstance(n_filters, tuple) and n_filters[0] <= 1
+        ):
             raise ValueError("n_filters must be larger than 1.")
 
         toolbox = self.create_toolbox(
             n_filters=n_filters,
             maximize=maximize,
             metric=metric,
             min_size=min_size,
@@ -178,28 +169,31 @@
         pop = toolbox.population(n=population_size)
         hof = tools.HallOfFame(n_hof)
         stats = tools.Statistics(lambda ind: ind.fitness.values)
         stats.register("avg", np.mean)
         stats.register("min", np.min)
         stats.register("max", np.max)
 
-        self.eaMuPlusLambda(
+        self.run(
             pop,
             toolbox,
             mu=population_size,
             lambda_=population_size,
             cxpb=cxpb,
             mutpb=mutpb,
             ngen=n_generations,
             stats=stats,
             halloffame=hof,
             maximize=maximize,
             maximum=maximum,
             minimum=minimum,
         )
 
-        return [Extreme(
-            data_metric_value=metric(self.data_connector.data),
-            filtered_data=self.data_connector.filter(best_filters),
-            filtered_data_metric_value=best_filters.fitness.values[0],
-            filters=best_filters,
-        ) for best_filters in hof]
+        return [
+            Extreme(
+                data_metric_value=metric(self.data_connector.data),
+                filtered_data=self.data_connector.filter(self.data_connector.data, best_filters),
+                filtered_data_metric_value=best_filters.fitness.values[0],
+                filters=best_filters,
+            )
+            for best_filters in hof
+        ]
```

### Comparing `slice_finder-0.0.21/src/slice_finder/slice_finders/slice_finder.py` & `slice_finder-0.0.22/src/slice_finder/slice_finders/slice_finder.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+from abc import abstractmethod
 import random
+
 import numpy as np
 
 from slice_finder.data_connectors.data_connector import DataConnector
 from slice_finder.data_structures.data_structure import DataStructure
 
-from abc import abstractmethod
-
 
 class SliceFinder:
     def __init__(
         self,
         data_connector: DataConnector,
         data_structure: DataStructure,
         verbose=False,
```

### Comparing `slice_finder-0.0.21/src/slice_finder/slice_finders/uniform.py` & `slice_finder-0.0.22/src/slice_finder/slice_finders/uniform.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,74 +7,83 @@
 class UniformSliceFinder(SliceFinder):
     """Slice discovery using uniform sampling."""
 
     def find_extreme(
         self,
         metric: Callable[[Any], float],
         n_iters=300,
-        n_filters=3,
+        n_filters: int | tuple[int, int] = 3,
         min_size=0.01,
         n_hof=1,
         maximize=False,
         maximum=float("inf"),
         minimum=float("-inf"),
     ) -> list[Extreme]:
         """Find slice with an extreme value of a metric.
-        
+
         Args:
             metric: Function that calculates metric value over data
             n_hof: Number of extreme values to return
             n_iters: Number of iterations
-            n_filters: Number of filters
+            n_filters: Number of filters. If a tuple, that means n_filters
+            will be in the range [n_filters[0], n_filters[1]]
             maximize: `True` will search for the maximum
             metric's value, and `False` will search for the minumum one
             min_size: Minimum size, in fractions, of the extreme subset.
             For exmaple, for value `0.01`, the extreme subset must be at
             least 1% of the data, in size, to be considered
             maximum: If `maximize`, and `maximum` is reached, the search stoppes
             minimum: If `not maximize`, and `minimum` is reached, the search stoppes
         """
 
         data_metric_value = metric(self.data_connector.data)
-        hof = [Extreme(
-            data_metric_value=data_metric_value,
-            filtered_data=self.data_connector.data,
-            filtered_data_metric_value=float("-inf") if maximize else float("inf"),
-            filters=[],
-        )]
+        hof = [
+            Extreme(
+                data_metric_value=data_metric_value,
+                filtered_data=self.data_connector.data,
+                filtered_data_metric_value=float("-inf") if maximize else float("inf"),
+                filters=[],
+            )
+        ]
 
         for _ in range(n_iters):
             filters = self.data_structure.get_n_filters(n_filters)
-            filtered_data = self.data_connector.filter(filters)
+            filtered_data = self.data_connector.filter(self.data_connector, filters)
             is_passing_size_threshold = (
                 len(filtered_data) >= len(self.data_connector.data) * min_size
             )
 
             if not is_passing_size_threshold:
                 continue
 
             filtered_data_metric_value = metric(filtered_data)
 
             if maximize and filtered_data_metric_value > hof[0].filtered_data_metric_value:
-                hof.insert(0, Extreme(
-                    data_metric_value=data_metric_value,
-                    filtered_data=filtered_data,
-                    filtered_data_metric_value=filtered_data_metric_value,
-                    filters=filters,
-                ))
+                hof.insert(
+                    0,
+                    Extreme(
+                        data_metric_value=data_metric_value,
+                        filtered_data=filtered_data,
+                        filtered_data_metric_value=filtered_data_metric_value,
+                        filters=filters,
+                    ),
+                )
                 if self.verbose:
                     print(hof[0].filtered_data_metric_value, hof[0].filters)
                 if filtered_data_metric_value >= maximum:
                     break
             elif not maximize and filtered_data_metric_value < hof[0].filtered_data_metric_value:
-                hof.insert(0, Extreme(
-                    data_metric_value=data_metric_value,
-                    filtered_data=filtered_data,
-                    filtered_data_metric_value=filtered_data_metric_value,
-                    filters=filters,
-                ))
+                hof.insert(
+                    0,
+                    Extreme(
+                        data_metric_value=data_metric_value,
+                        filtered_data=filtered_data,
+                        filtered_data_metric_value=filtered_data_metric_value,
+                        filters=filters,
+                    ),
+                )
                 if self.verbose:
                     print(hof[0].filtered_data_metric_value, hof[0].filters)
                 if filtered_data_metric_value <= minimum:
                     break
 
         return hof[:n_hof]
```

### Comparing `slice_finder-0.0.21/src/slice_finder/types.py` & `slice_finder-0.0.22/src/slice_finder/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,22 +16,28 @@
     """Extreme object."""
 
     data_metric_value: float
     filtered_data: Any
     filtered_data_metric_value: float
     filters: list[Filter]
 
-    def get_prettified_view(self) -> str:
-        """Replace the default behavior of `print`.
+    def get_human_readable(self) -> str:
+        """Returns a human readable format of the object.
 
-                Returns:
-                    Prettified text."""
+        Returns:
+            Human readable object.
+        """
 
-        return f"""Value of the metric on the whole dataset: {self.data_metric_value}
-Value of the metric on the filtered data: {self.filtered_data_metric_value}
-Filters: {self.filters}"""
+        textual_filters = [
+            f"{filter.feature} {filter.operator} {filter.value}" for filter in self.filters
+        ]
+        textual_composite_filter = "\nAND ".join(textual_filters)
+        return f"""When {textual_composite_filter},
+the value of the metric on the filtered data is {self.filtered_data_metric_value}
+compared to {self.data_metric_value} on the whole data.
+"""
 
     def __str__(self) -> str:
-         return self.get_prettified_view()
-    
+        return self.get_human_readable()
+
     def __repr__(self) -> str:
-         return self.get_prettified_view()
+        return self.get_human_readable()
```

### Comparing `slice_finder-0.0.21/setup.py` & `slice_finder-0.0.22/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 ['deap>=1.3,<2.0',
  'lightgbm>=3.0.0,<4.0.0',
  'numpy>=1.20.0,<2.0.0',
  'pandas>=1.2.5,<2.0.0']
 
 setup_kwargs = {
     'name': 'slice-finder',
-    'version': '0.0.21',
-    'description': 'A Framework for Slice Discovery',
-    'long_description': '# Slice Finder: A Framework for Slice Discovery\n\nSlice Finder is a versatile and highly configurable framework designed for the discovery of explainable, anomalous data subsets, which exhibit substantially divergent metric values in comparison to the entire dataset.\n\nSlice Finder is a crucial investigative instrument, as it enables data scientists to identify regions where their models demonstrate over- or under-performance.\n\n## Algorithmic achievements\n* Tackling data quantization can be complex, particularly when transforming continuous values into discrete space. Slice Finder overcomes this challenge by fitting an LGBM model to the data and extracting the appropriate splits.\n* As the number of filters, columns, and values increases, so does the combinatorial search space. Slice Finder addresses this issue in two ways:\n    * By fitting an LGBM model to the data, the most critical fields and values for splitting are identified, significantly reducing the search space.\n    * Incorporating Genetic Algorithm heuristics to converge towards global minima/maxima, which outperforms both the time-consuming "try-it-all" approach and uniform filter sampling in terms of efficiency and results.\n\n## Engineering achievements\nBy separating data connectors, data structures, and slice finders, SliceFinder offers a flexible framework that enables seamless modifications and replacement of components. Furthermore, by detaching metric mechanism from the system, SliceFinder supports any custom logic metrics.\n\n## Demo\n![GA search for anomalous subset with high MSE](./examples/demo.gif)\n\n## Installation\nInstall Slice Finder via pip:\n```python\npip install slice_finder\n```\n\n# Quick Start\n```python\nimport pandas as pd\nfrom sklearn import metrics\nfrom slice_finder import GASliceFinder, FlattenedLGBMDataStructure, PandasDataConnector\n\n# Load data\ndf = pd.read_csv(\'your_data.csv\')\n\n# Initialize Genetic Algorithm Slice Finder with desired data connector and data structure\nslice_finder = GASliceFinder(\n    data_connector=PandasDataConnector(\n        df=df,\n        X_cols=df.drop([\'pred\', \'target\'], axis=1).columns,\n        y_col=\'target\',\n        pred_col=\'pred\',\n    ),\n    data_structure=FlattenedLGBMDataStructure(),\n    verbose=True,\n    random_state=42,\n)\n\n# Find anomalous slice\nextreme = slice_finder.find_extreme(\n    metric=lambda df: metrics.mean_absolute_error(df[\'target\'], df[\'pred\']),\n    n_filters=3,\n    maximize=True,\n)\nextreme[0]\n```\n\n## Data Connectors\nBuilt in:\n* `PandasDataConnector` - allow you to use Pandas\n\nBase Classes:\n* `DataConnector` - Base data connector\n\nMore connectors will be added as demand grows.\n\nYou can create your custom data connector by extending the base class and implementing the necessary methods.\n\n## Data Structures\nBuilt in:\n* `FlattenedLGBMDataStructure` - Utilizes LightGBM decision trees to quantize and partition the data.\nNote: Currently, `FlattenedLGBMDataStructure` must work with `PandasDataConnector` because of LGBM constraints. Moreover, this data structure is coupled to pandas connector because categorical values must be modified to `pd.Categorical` class.\n\nBase classes:\n* `DataStructure` - Base data structure\n* `LGBMDataStructure` - Handles the fitting and partitioning the LGBM trees\n\nMore data structures will be added as demand grows.\n\nYou can create your custom data structure by extending the base classes and implementing the necessary methods.\n\n## Slice Finders\nBuilt in:\n* `GASliceFinder` - Utilizes `eaMuPlusLambda` evolutionary algorithm to search for the most anomalous slice\n* `UniformSliceFinder` - Utilizes uniform sampling out of the data structure\n\nBase classes:\n* `SliceFinder` - Base slice finder\n\nMore algorithms will be added based on demand. \n\nYou can create your custom data structure by extending the base class and implementing the necessary methods.\n\n## Metrics\nMetrics are passed as functions to the `find_extreme` method, allowing you to use any metric or implement your custom logic.\n\n## Neat things to implement\n* Calculation parallelism\n* More search algorithms. Ant colony optimization?\n\n## License\nThis project is licensed under the MIT License.\n\n## Contributing\nContributions are welcome!\nClone the repo, run `poetry install` and start hacking.\n\n## Support\nFor any questions, bug reports, or feature requests, please open an issue.',
+    'version': '0.0.22',
+    'description': 'Slice Finder: A Framework for Slice Discovery',
+    'long_description': '# Slice Finder: A Framework for Slice Discovery\n\nSlice Finder is a versatile and highly configurable framework designed for the discovery of explainable, anomalous data subsets, which exhibit substantially divergent metric values in comparison to the entire dataset.\n\n> To illustrate, imagine that you have developed a model for identifying fraudulent transactions. The model\'s overall accuracy across the entire dataset is 0.95. However, when transactions occur more than 100 km away from the previous transaction and involve cash (2 filters), the model\'s accuracy drops significantly to 0.54.\n\nSlice Finder is a crucial investigative instrument, as it enables data scientists to identify regions where their models demonstrate over- or under-performance.\n\n## Algorithmic achievements\n* Tackling data quantization can be complex, particularly when transforming continuous values into discrete space. Slice Finder overcomes this challenge by fitting an LGBM model to the data and extracting the appropriate splits.\n* As the number of filters, columns, and values increases, so does the combinatorial search space. Slice Finder addresses this issue in two ways:\n    * By fitting an LGBM model to the data, the most critical fields and values for splitting are identified, significantly reducing the search space.\n    * Incorporating Genetic Algorithm heuristics to converge towards global minima/maxima, which outperforms both the time-consuming "try-it-all" approach and uniform filter sampling in terms of efficiency and results.\n\n## Engineering achievements\nBy separating data connectors, data structures, and slice finders, SliceFinder offers a flexible framework that enables seamless modifications and replacement of components. Furthermore, by detaching metric mechanism from the system, SliceFinder supports any custom logic metrics.\n\n## Demo\n![GA search for anomalous subset with high MSE](./examples/demo.gif)\n\n## Installation\nInstall Slice Finder via pip:\n```python\npip install slice_finder\n```\n\n# Quick Start\n```python\nimport pandas as pd\nfrom sklearn import metrics\nfrom slice_finder import GAMuPlusLambdaSliceFinder, FlattenedLGBMDataStructure, PandasDataConnector\n\n# Load data\ndf = pd.read_csv(\'your_data.csv\')\n\n# Initialize Genetic Algorithm Slice Finder with desired data connector and data structure\nslice_finder = GAMuPlusLambdaSliceFinder(\n    data_connector=PandasDataConnector(\n        df=df,\n        X_cols=df.drop([\'pred\', \'target\'], axis=1).columns,\n        y_col=\'target\',\n        pred_col=\'pred\',\n    ),\n    data_structure=FlattenedLGBMDataStructure(),\n    verbose=True,\n    random_state=42,\n)\n\n# Find anomalous slice\nextreme = slice_finder.find_extreme(\n    metric=lambda df: metrics.mean_absolute_error(df[\'target\'], df[\'pred\']),\n    n_filters=3,\n    maximize=True,\n)\nextreme[0]\n```\n\n## Data Connectors\nBuilt in:\n* `PandasDataConnector` - allow you to use Pandas\n\nBase Classes:\n* `DataConnector` - Base data connector\n\nMore connectors will be added as demand grows.\n\nYou can create your custom data connector by extending the base class and implementing the necessary methods.\n\n## Data Structures\nBuilt in:\n* `FlattenedLGBMDataStructure` - Utilizes LightGBM decision trees to quantize and partition the data.\nNote: Currently, `FlattenedLGBMDataStructure` must work with `PandasDataConnector` because of LGBM constraints. Moreover, this data structure is coupled to pandas connector because categorical values must be modified to `pd.Categorical` class.\n\nBase classes:\n* `DataStructure` - Base data structure\n* `LGBMDataStructure` - Handles the fitting and partitioning the LGBM trees\n\nMore data structures will be added as demand grows.\n\nYou can create your custom data structure by extending the base classes and implementing the necessary methods.\n\n## Slice Finders\nBuilt in:\n* `GAMuPlusLambdaSliceFinder` - Utilizes `eaMuPlusLambda` evolutionary algorithm to search for the most anomalous slice\n* `UniformSliceFinder` - Utilizes uniform sampling out of the data structure\n\nBase classes:\n* `SliceFinder` - Base slice finder\n* `GASliceFinder` - Extends `SliceFinder` and enables the use of genetic algorithms as search heuristics\n\nMore algorithms will be added based on demand. \n\nYou can create your custom data structure by extending the base class and implementing the necessary methods.\n\n## Metrics\nMetrics are passed as functions to the `find_extreme` method, allowing you to use any metric or implement your custom logic.\n\n## Neat things to implement\n* Calculation parallelism\n* More search algorithms. Ant colony optimization?\n\n## License\nThis project is licensed under the MIT License.\n\n## Contributing\nContributions are welcome!\nClone the repo, run `poetry install` and start hacking.\n\n## Support\nFor any questions, bug reports, or feature requests, please open an issue.',
     'author': 'Igal Leikin',
     'author_email': 'igaloly@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/igaloly/slice_finder',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `slice_finder-0.0.21/PKG-INFO` & `slice_finder-0.0.22/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: slice-finder
-Version: 0.0.21
-Summary: A Framework for Slice Discovery
+Version: 0.0.22
+Summary: Slice Finder: A Framework for Slice Discovery
 Home-page: https://github.com/igaloly/slice_finder
 License: MIT
-Keywords: slice discovery,slice finding
+Keywords: slice discovery,slice detection,subgroup discovery,subgroup detection,slice finding
 Author: Igal Leikin
 Author-email: igaloly@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -22,14 +22,16 @@
 Project-URL: Repository, https://github.com/igaloly/slice_finder
 Description-Content-Type: text/markdown
 
 # Slice Finder: A Framework for Slice Discovery
 
 Slice Finder is a versatile and highly configurable framework designed for the discovery of explainable, anomalous data subsets, which exhibit substantially divergent metric values in comparison to the entire dataset.
 
+> To illustrate, imagine that you have developed a model for identifying fraudulent transactions. The model's overall accuracy across the entire dataset is 0.95. However, when transactions occur more than 100 km away from the previous transaction and involve cash (2 filters), the model's accuracy drops significantly to 0.54.
+
 Slice Finder is a crucial investigative instrument, as it enables data scientists to identify regions where their models demonstrate over- or under-performance.
 
 ## Algorithmic achievements
 * Tackling data quantization can be complex, particularly when transforming continuous values into discrete space. Slice Finder overcomes this challenge by fitting an LGBM model to the data and extracting the appropriate splits.
 * As the number of filters, columns, and values increases, so does the combinatorial search space. Slice Finder addresses this issue in two ways:
     * By fitting an LGBM model to the data, the most critical fields and values for splitting are identified, significantly reducing the search space.
     * Incorporating Genetic Algorithm heuristics to converge towards global minima/maxima, which outperforms both the time-consuming "try-it-all" approach and uniform filter sampling in terms of efficiency and results.
@@ -46,21 +48,21 @@
 pip install slice_finder
 ```
 
 # Quick Start
 ```python
 import pandas as pd
 from sklearn import metrics
-from slice_finder import GASliceFinder, FlattenedLGBMDataStructure, PandasDataConnector
+from slice_finder import GAMuPlusLambdaSliceFinder, FlattenedLGBMDataStructure, PandasDataConnector
 
 # Load data
 df = pd.read_csv('your_data.csv')
 
 # Initialize Genetic Algorithm Slice Finder with desired data connector and data structure
-slice_finder = GASliceFinder(
+slice_finder = GAMuPlusLambdaSliceFinder(
     data_connector=PandasDataConnector(
         df=df,
         X_cols=df.drop(['pred', 'target'], axis=1).columns,
         y_col='target',
         pred_col='pred',
     ),
     data_structure=FlattenedLGBMDataStructure(),
@@ -99,19 +101,20 @@
 
 More data structures will be added as demand grows.
 
 You can create your custom data structure by extending the base classes and implementing the necessary methods.
 
 ## Slice Finders
 Built in:
-* `GASliceFinder` - Utilizes `eaMuPlusLambda` evolutionary algorithm to search for the most anomalous slice
+* `GAMuPlusLambdaSliceFinder` - Utilizes `eaMuPlusLambda` evolutionary algorithm to search for the most anomalous slice
 * `UniformSliceFinder` - Utilizes uniform sampling out of the data structure
 
 Base classes:
 * `SliceFinder` - Base slice finder
+* `GASliceFinder` - Extends `SliceFinder` and enables the use of genetic algorithms as search heuristics
 
 More algorithms will be added based on demand. 
 
 You can create your custom data structure by extending the base class and implementing the necessary methods.
 
 ## Metrics
 Metrics are passed as functions to the `find_extreme` method, allowing you to use any metric or implement your custom logic.
```

