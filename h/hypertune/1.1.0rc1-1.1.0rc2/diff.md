# Comparing `tmp/hypertune-1.1.0rc1.tar.gz` & `tmp/hypertune-1.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypertune-1.1.0rc1.tar", last modified: Sun Apr  9 14:57:45 2023, max compression
+gzip compressed data, was "hypertune-1.1.0rc2.tar", last modified: Sun Apr  9 15:47:59 2023, max compression
```

## Comparing `hypertune-1.1.0rc1.tar` & `hypertune-1.1.0rc2.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:57:45.585673 hypertune-1.1.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-09 14:57:45.585673 hypertune-1.1.0rc1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:57:45.581673 hypertune-1.1.0rc1/hypertune/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/iteration_lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:57:45.581673 hypertune-1.1.0rc1/hypertune/matrix/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/matrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/matrix/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/matrix/hyperopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/matrix/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/pkg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:57:45.581673 hypertune-1.1.0rc1/hypertune/search_managers/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/search_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/search_managers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:57:45.581673 hypertune-1.1.0rc1/hypertune/search_managers/bayesian_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/search_managers/bayesian_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/search_managers/bayesian_optimization/acquisition_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/search_managers/bayesian_optimization/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/search_managers/bayesian_optimization/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/search_managers/bayesian_optimization/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:57:45.581673 hypertune-1.1.0rc1/hypertune/search_managers/grid_search/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/search_managers/grid_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/search_managers/grid_search/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:57:45.581673 hypertune-1.1.0rc1/hypertune/search_managers/hyperband/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/search_managers/hyperband/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/search_managers/hyperband/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:57:45.581673 hypertune-1.1.0rc1/hypertune/search_managers/hyperopt/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/search_managers/hyperopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/search_managers/hyperopt/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:57:45.585673 hypertune-1.1.0rc1/hypertune/search_managers/mapping/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/search_managers/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/search_managers/mapping/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:57:45.585673 hypertune-1.1.0rc1/hypertune/search_managers/random_search/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/search_managers/random_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/search_managers/random_search/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/search_managers/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/hypertune/search_managers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:57:45.581673 hypertune-1.1.0rc1/hypertune.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-09 14:57:45.000000 hypertune-1.1.0rc1/hypertune.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-09 14:57:45.000000 hypertune-1.1.0rc1/hypertune.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:57:45.000000 hypertune-1.1.0rc1/hypertune.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-09 14:57:45.000000 hypertune-1.1.0rc1/hypertune.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 14:57:45.000000 hypertune-1.1.0rc1/hypertune.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-09 14:57:45.585673 hypertune-1.1.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-09 14:57:36.000000 hypertune-1.1.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:59.193773 hypertune-1.1.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-09 15:47:59.193773 hypertune-1.1.0rc2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:59.189772 hypertune-1.1.0rc2/hypertune/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/iteration_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:59.193773 hypertune-1.1.0rc2/hypertune/matrix/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/matrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/matrix/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/matrix/hyperopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/matrix/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/pkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:59.193773 hypertune-1.1.0rc2/hypertune/search_managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/search_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/search_managers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:59.193773 hypertune-1.1.0rc2/hypertune/search_managers/bayesian_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/search_managers/bayesian_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/search_managers/bayesian_optimization/acquisition_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/search_managers/bayesian_optimization/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/search_managers/bayesian_optimization/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/search_managers/bayesian_optimization/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:59.193773 hypertune-1.1.0rc2/hypertune/search_managers/grid_search/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/search_managers/grid_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/search_managers/grid_search/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:59.193773 hypertune-1.1.0rc2/hypertune/search_managers/hyperband/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/search_managers/hyperband/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/search_managers/hyperband/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:59.193773 hypertune-1.1.0rc2/hypertune/search_managers/hyperopt/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/search_managers/hyperopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/search_managers/hyperopt/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:59.193773 hypertune-1.1.0rc2/hypertune/search_managers/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/search_managers/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/search_managers/mapping/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:59.193773 hypertune-1.1.0rc2/hypertune/search_managers/random_search/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/search_managers/random_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/search_managers/random_search/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/search_managers/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/hypertune/search_managers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:47:59.189772 hypertune-1.1.0rc2/hypertune.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-09 15:47:59.000000 hypertune-1.1.0rc2/hypertune.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-09 15:47:59.000000 hypertune-1.1.0rc2/hypertune.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 15:47:59.000000 hypertune-1.1.0rc2/hypertune.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-09 15:47:59.000000 hypertune-1.1.0rc2/hypertune.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 15:47:59.000000 hypertune-1.1.0rc2/hypertune.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-09 15:47:59.193773 hypertune-1.1.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-09 15:47:50.000000 hypertune-1.1.0rc2/setup.py
```

### Comparing `hypertune-1.1.0rc1/PKG-INFO` & `hypertune-1.1.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypertune
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: A library for performing hyperparameter optimization with Polyaxon.
 Home-page: https://github.com/polyaxon/hypertune
 Author: Polyaxon, Inc.
 Author-email: contact@polyaxon.com
 Maintainer: Polyaxon, Inc.
 Maintainer-email: contact@polyaxon.com
 License: Apache 2.0
```

### Comparing `hypertune-1.1.0rc1/hypertune/__init__.py` & `hypertune-1.1.0rc2/hypertune/__init__.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/iteration_lineage.py` & `hypertune-1.1.0rc2/hypertune/iteration_lineage.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/logger.py` & `hypertune-1.1.0rc2/hypertune/logger.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/matrix/__init__.py` & `hypertune-1.1.0rc2/hypertune/matrix/__init__.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/matrix/dist.py` & `hypertune-1.1.0rc2/hypertune/matrix/dist.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/matrix/hyperopt.py` & `hypertune-1.1.0rc2/hypertune/matrix/hyperopt.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/matrix/utils.py` & `hypertune-1.1.0rc2/hypertune/matrix/utils.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/pkg.py` & `hypertune-1.1.0rc2/hypertune/pkg.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 NAME = "hypertune"
-VERSION = "1.1.0-rc1"
+VERSION = "1.1.0-rc2"
 DESC = "A library for performing hyperparameter optimization with Polyaxon."
 URL = "https://github.com/polyaxon/hypertune"
 AUTHOR = "Polyaxon, Inc."
 EMAIL = "contact@polyaxon.com"
 LICENSE = "Apache 2.0"
```

### Comparing `hypertune-1.1.0rc1/hypertune/search_managers/__init__.py` & `hypertune-1.1.0rc2/hypertune/search_managers/__init__.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/search_managers/base.py` & `hypertune-1.1.0rc2/hypertune/search_managers/base.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/search_managers/bayesian_optimization/__init__.py` & `hypertune-1.1.0rc2/hypertune/search_managers/bayesian_optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/search_managers/bayesian_optimization/acquisition_function.py` & `hypertune-1.1.0rc2/hypertune/search_managers/bayesian_optimization/acquisition_function.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/search_managers/bayesian_optimization/manager.py` & `hypertune-1.1.0rc2/hypertune/search_managers/bayesian_optimization/manager.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/search_managers/bayesian_optimization/optimizer.py` & `hypertune-1.1.0rc2/hypertune/search_managers/bayesian_optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/search_managers/bayesian_optimization/space.py` & `hypertune-1.1.0rc2/hypertune/search_managers/bayesian_optimization/space.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/search_managers/grid_search/__init__.py` & `hypertune-1.1.0rc2/hypertune/search_managers/grid_search/__init__.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/search_managers/grid_search/manager.py` & `hypertune-1.1.0rc2/hypertune/search_managers/grid_search/manager.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/search_managers/hyperband/__init__.py` & `hypertune-1.1.0rc2/hypertune/search_managers/hyperband/__init__.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/search_managers/hyperband/manager.py` & `hypertune-1.1.0rc2/hypertune/search_managers/hyperband/manager.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/search_managers/hyperopt/__init__.py` & `hypertune-1.1.0rc2/hypertune/search_managers/hyperopt/__init__.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/search_managers/hyperopt/manager.py` & `hypertune-1.1.0rc2/hypertune/search_managers/hyperopt/manager.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/search_managers/mapping/__init__.py` & `hypertune-1.1.0rc2/hypertune/search_managers/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/search_managers/mapping/manager.py` & `hypertune-1.1.0rc2/hypertune/search_managers/mapping/manager.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/search_managers/random_search/__init__.py` & `hypertune-1.1.0rc2/hypertune/search_managers/random_search/__init__.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/search_managers/random_search/manager.py` & `hypertune-1.1.0rc2/hypertune/search_managers/random_search/manager.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/search_managers/spec.py` & `hypertune-1.1.0rc2/hypertune/search_managers/spec.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune/search_managers/utils.py` & `hypertune-1.1.0rc2/hypertune/search_managers/utils.py`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/hypertune.egg-info/PKG-INFO` & `hypertune-1.1.0rc2/hypertune.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypertune
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: A library for performing hyperparameter optimization with Polyaxon.
 Home-page: https://github.com/polyaxon/hypertune
 Author: Polyaxon, Inc.
 Author-email: contact@polyaxon.com
 Maintainer: Polyaxon, Inc.
 Maintainer-email: contact@polyaxon.com
 License: Apache 2.0
```

### Comparing `hypertune-1.1.0rc1/hypertune.egg-info/SOURCES.txt` & `hypertune-1.1.0rc2/hypertune.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 ../LICENSE
 ../README.md
 hypertune/__init__.py
 hypertune/iteration_lineage.py
 hypertune/logger.py
 hypertune/pkg.py
+hypertune/py.typed
 hypertune.egg-info/PKG-INFO
 hypertune.egg-info/SOURCES.txt
 hypertune.egg-info/dependency_links.txt
 hypertune.egg-info/requires.txt
 hypertune.egg-info/top_level.txt
 hypertune/matrix/__init__.py
 hypertune/matrix/dist.py
```

### Comparing `hypertune-1.1.0rc1/setup.cfg` & `hypertune-1.1.0rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `hypertune-1.1.0rc1/setup.py` & `hypertune-1.1.0rc2/setup.py`

 * *Files identical despite different names*

