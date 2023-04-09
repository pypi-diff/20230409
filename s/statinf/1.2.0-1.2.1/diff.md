# Comparing `tmp/statinf-1.2.0.tar.gz` & `tmp/statinf-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statinf-1.2.0.tar", last modified: Sun Feb  5 14:11:14 2023, max compression
+gzip compressed data, was "statinf-1.2.1.tar", last modified: Sun Apr  9 11:19:11 2023, max compression
```

## Comparing `statinf-1.2.0.tar` & `statinf-1.2.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-02-05 14:11:14.421115 statinf-1.2.0/
--rw-r--r--   0 florian   (1000) florian   (1000)     1070 2020-10-01 18:31:13.000000 statinf-1.2.0/LICENSE
--rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-02-05 14:11:14.421115 statinf-1.2.0/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)     8337 2020-10-01 18:31:13.000000 statinf-1.2.0/README.md
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-02-05 14:11:14.421115 statinf-1.2.0/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)      781 2020-10-01 18:31:13.000000 statinf-1.2.0/setup.py
--rw-r--r--   0 florian   (1000) florian   (1000)      889 2023-02-05 14:11:13.000000 statinf-1.2.0/setup_new.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-02-05 14:11:14.401115 statinf-1.2.0/statinf/
--rw-r--r--   0 florian   (1000) florian   (1000)       22 2023-02-05 14:11:13.000000 statinf-1.2.0/statinf/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-02-05 14:11:14.401115 statinf-1.2.0/statinf/data/
--rw-r--r--   0 florian   (1000) florian   (1000)     2701 2023-02-03 18:48:52.000000 statinf-1.2.0/statinf/data/GenerateData.py
--rw-r--r--   0 florian   (1000) florian   (1000)    27132 2021-03-24 14:33:31.000000 statinf-1.2.0/statinf/data/ProcessData.py
--rw-r--r--   0 florian   (1000) florian   (1000)       55 2020-10-01 18:31:13.000000 statinf-1.2.0/statinf/data/__init__.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-02-05 14:11:14.401115 statinf-1.2.0/statinf/distributions/
--rw-r--r--   0 florian   (1000) florian   (1000)       24 2023-02-03 18:27:09.000000 statinf-1.2.0/statinf/distributions/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    19084 2023-02-05 14:09:04.000000 statinf-1.2.0/statinf/distributions/discrete.py
--rw-r--r--   0 florian   (1000) florian   (1000)       26 2021-06-27 12:48:10.000000 statinf-1.2.0/statinf/init_template.py
--rw-r--r--   0 florian   (1000) florian   (1000)     5107 2021-06-27 13:22:48.000000 statinf-1.2.0/statinf/misc.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-02-05 14:11:14.411115 statinf-1.2.0/statinf/ml/
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2020-10-01 18:31:13.000000 statinf-1.2.0/statinf/ml/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2522 2021-03-07 06:24:49.000000 statinf-1.2.0/statinf/ml/activations.py
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2020-10-17 16:20:51.000000 statinf-1.2.0/statinf/ml/generative.py
--rw-r--r--   0 florian   (1000) florian   (1000)     2892 2021-03-07 06:09:35.000000 statinf-1.2.0/statinf/ml/initializations.py
--rw-r--r--   0 florian   (1000) florian   (1000)     3152 2021-03-07 06:45:42.000000 statinf-1.2.0/statinf/ml/losses.py
--rw-r--r--   0 florian   (1000) florian   (1000)    16863 2022-08-21 10:47:32.000000 statinf-1.2.0/statinf/ml/neuralnetwork.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11152 2021-03-07 08:40:43.000000 statinf-1.2.0/statinf/ml/optimizers.py
--rw-r--r--   0 florian   (1000) florian   (1000)     6141 2021-06-27 13:22:59.000000 statinf-1.2.0/statinf/ml/performance.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-02-05 14:11:14.411115 statinf-1.2.0/statinf/nonparametrics/
--rw-r--r--   0 florian   (1000) florian   (1000)       23 2020-11-01 11:38:35.000000 statinf-1.2.0/statinf/nonparametrics/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)      842 2020-11-01 18:05:22.000000 statinf-1.2.0/statinf/nonparametrics/kernels.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-02-05 14:11:14.411115 statinf-1.2.0/statinf/regressions/
--rw-r--r--   0 florian   (1000) florian   (1000)    19249 2021-03-24 15:58:55.000000 statinf-1.2.0/statinf/regressions/LinearModels.py
--rw-r--r--   0 florian   (1000) florian   (1000)       51 2023-02-03 18:26:31.000000 statinf-1.2.0/statinf/regressions/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)    18168 2021-03-24 15:54:37.000000 statinf-1.2.0/statinf/regressions/glm.py
--rw-r--r--   0 florian   (1000) florian   (1000)     7060 2020-10-01 18:31:13.000000 statinf-1.2.0/statinf/regressions/glm_test.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-02-05 14:11:14.411115 statinf-1.2.0/statinf/stats/
--rw-r--r--   0 florian   (1000) florian   (1000)      126 2020-11-01 12:20:16.000000 statinf-1.2.0/statinf/stats/__init__.py
--rw-r--r--   0 florian   (1000) florian   (1000)     6950 2020-11-01 18:03:36.000000 statinf-1.2.0/statinf/stats/bayesian.py
--rw-r--r--   0 florian   (1000) florian   (1000)     4185 2020-10-01 18:31:13.000000 statinf-1.2.0/statinf/stats/descriptive.py
--rw-r--r--   0 florian   (1000) florian   (1000)    21520 2023-02-03 18:58:48.000000 statinf-1.2.0/statinf/stats/tests.py
--rw-r--r--   0 florian   (1000) florian   (1000)    11524 2020-10-27 02:35:31.000000 statinf-1.2.0/statinf/stats/timeseries.py
--rw-r--r--   0 florian   (1000) florian   (1000)    10469 2020-11-01 18:02:58.000000 statinf-1.2.0/statinf/stats/unsupervised.py
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-02-05 14:11:14.401115 statinf-1.2.0/statinf.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-02-05 14:11:14.000000 statinf-1.2.0/statinf.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      966 2023-02-05 14:11:14.000000 statinf-1.2.0/statinf.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-02-05 14:11:14.000000 statinf-1.2.0/statinf.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)      101 2023-02-05 14:11:14.000000 statinf-1.2.0/statinf.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-02-05 14:11:14.000000 statinf-1.2.0/statinf.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-09 11:19:11.321976 statinf-1.2.1/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1070 2020-10-01 18:31:13.000000 statinf-1.2.1/LICENSE
+-rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-04-09 11:19:11.321976 statinf-1.2.1/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)     8337 2020-10-01 18:31:13.000000 statinf-1.2.1/README.md
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-04-09 11:19:11.321976 statinf-1.2.1/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)      781 2020-10-01 18:31:13.000000 statinf-1.2.1/setup.py
+-rw-r--r--   0 florian   (1000) florian   (1000)      889 2023-04-09 11:19:10.000000 statinf-1.2.1/setup_new.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-09 11:19:11.301976 statinf-1.2.1/statinf/
+-rw-r--r--   0 florian   (1000) florian   (1000)       22 2023-04-09 11:19:10.000000 statinf-1.2.1/statinf/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-09 11:19:11.311976 statinf-1.2.1/statinf/data/
+-rw-r--r--   0 florian   (1000) florian   (1000)     2701 2023-02-03 18:48:52.000000 statinf-1.2.1/statinf/data/GenerateData.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    27132 2021-03-24 14:33:31.000000 statinf-1.2.1/statinf/data/ProcessData.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       55 2020-10-01 18:31:13.000000 statinf-1.2.1/statinf/data/__init__.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-09 11:19:11.311976 statinf-1.2.1/statinf/distributions/
+-rw-r--r--   0 florian   (1000) florian   (1000)       24 2023-02-03 18:27:09.000000 statinf-1.2.1/statinf/distributions/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    22095 2023-04-09 10:59:39.000000 statinf-1.2.1/statinf/distributions/discrete.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       26 2021-06-27 12:48:10.000000 statinf-1.2.1/statinf/init_template.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     5107 2021-06-27 13:22:48.000000 statinf-1.2.1/statinf/misc.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-09 11:19:11.311976 statinf-1.2.1/statinf/ml/
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2020-10-01 18:31:13.000000 statinf-1.2.1/statinf/ml/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2522 2021-03-07 06:24:49.000000 statinf-1.2.1/statinf/ml/activations.py
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2020-10-17 16:20:51.000000 statinf-1.2.1/statinf/ml/generative.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     2892 2021-03-07 06:09:35.000000 statinf-1.2.1/statinf/ml/initializations.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     3152 2021-03-07 06:45:42.000000 statinf-1.2.1/statinf/ml/losses.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    16863 2022-08-21 10:47:32.000000 statinf-1.2.1/statinf/ml/neuralnetwork.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11152 2021-03-07 08:40:43.000000 statinf-1.2.1/statinf/ml/optimizers.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     6141 2021-06-27 13:22:59.000000 statinf-1.2.1/statinf/ml/performance.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-09 11:19:11.311976 statinf-1.2.1/statinf/nonparametrics/
+-rw-r--r--   0 florian   (1000) florian   (1000)       23 2020-11-01 11:38:35.000000 statinf-1.2.1/statinf/nonparametrics/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)      842 2020-11-01 18:05:22.000000 statinf-1.2.1/statinf/nonparametrics/kernels.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-09 11:19:11.311976 statinf-1.2.1/statinf/regressions/
+-rw-r--r--   0 florian   (1000) florian   (1000)    19249 2021-03-24 15:58:55.000000 statinf-1.2.1/statinf/regressions/LinearModels.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       51 2023-02-03 18:26:31.000000 statinf-1.2.1/statinf/regressions/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    18168 2021-03-24 15:54:37.000000 statinf-1.2.1/statinf/regressions/glm.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     7060 2020-10-01 18:31:13.000000 statinf-1.2.1/statinf/regressions/glm_test.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-09 11:19:11.321976 statinf-1.2.1/statinf/stats/
+-rw-r--r--   0 florian   (1000) florian   (1000)      126 2020-11-01 12:20:16.000000 statinf-1.2.1/statinf/stats/__init__.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     6950 2020-11-01 18:03:36.000000 statinf-1.2.1/statinf/stats/bayesian.py
+-rw-r--r--   0 florian   (1000) florian   (1000)     4185 2020-10-01 18:31:13.000000 statinf-1.2.1/statinf/stats/descriptive.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    21520 2023-02-03 18:58:48.000000 statinf-1.2.1/statinf/stats/tests.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    11524 2020-10-27 02:35:31.000000 statinf-1.2.1/statinf/stats/timeseries.py
+-rw-r--r--   0 florian   (1000) florian   (1000)    10469 2020-11-01 18:02:58.000000 statinf-1.2.1/statinf/stats/unsupervised.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-04-09 11:19:11.311976 statinf-1.2.1/statinf.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     8825 2023-04-09 11:19:11.000000 statinf-1.2.1/statinf.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      966 2023-04-09 11:19:11.000000 statinf-1.2.1/statinf.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-04-09 11:19:11.000000 statinf-1.2.1/statinf.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)      101 2023-04-09 11:19:11.000000 statinf-1.2.1/statinf.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-04-09 11:19:11.000000 statinf-1.2.1/statinf.egg-info/top_level.txt
```

### Comparing `statinf-1.2.0/LICENSE` & `statinf-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `statinf-1.2.0/PKG-INFO` & `statinf-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statinf
-Version: 1.2.0
+Version: 1.2.1
 Summary: A library for statistics and causal inference
 Home-page: https://www.florianfelice.com/statinf
 Author: Florian Felice
 Author-email: florian.felice@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `statinf-1.2.0/README.md` & `statinf-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `statinf-1.2.0/setup.py` & `statinf-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.0/setup_new.py` & `statinf-1.2.1/setup_new.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="statinf",
-    version="1.2.0",
+    version="1.2.1",
     author="Florian Felice",
     author_email="florian.felice@outlook.com",
     description="A library for statistics and causal inference",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.florianfelice.com/statinf",
     packages=setuptools.find_packages(),
```

### Comparing `statinf-1.2.0/statinf/data/GenerateData.py` & `statinf-1.2.1/statinf/data/GenerateData.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.0/statinf/data/ProcessData.py` & `statinf-1.2.1/statinf/data/ProcessData.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.0/statinf/distributions/discrete.py` & `statinf-1.2.1/statinf/distributions/discrete.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import math
 from decimal import Decimal
 
 import datetime
 
 import scipy
 from scipy import optimize
+import warnings
 
 
 scipy_methods = ['BFGS', 'L-BFGS-B', 'Newton-CG', 'CG', 'Powell', 'Nelder-Mead']
 
 # Empty object with future attributes
 class Object(object):
     pass
@@ -68,22 +69,26 @@
         _seed = seed if seed else datetime.datetime.now().microsecond
         np.random.seed(_seed)
         return [self._generate(_pmf, seed=_seed + i) for i in range(size)]
 
     def _fast_fit(self):
         return ValueError('Fast or auto fit is not allowed for this distribution, please chose another value')
 
-    def _fit(self, data, bounds=None, init_params=np.array([1]), verbose=False, method='auto'):
+    def _fit(self, data, bounds=None, init_params=np.array([1]), verbose=False, method='auto', args=()):
         if method.lower() in ['auto', 'fast']:
             res = self._fast_fit(data)
         elif method in scipy_methods:
+            if args == ():
+                nll_args = (data,)
+            else:
+                nll_args = sum(((data,), args), ())
             res = scipy.optimize.minimize(
                 fun=self.nll_fun,
                 x0=init_params,
-                args=(data,),
+                args=nll_args,
                 method=method,
                 bounds=bounds
             )
             self.nll = res.fun
 
             if verbose:
                 print(res)
@@ -300,15 +305,19 @@
         self.j = j
 
         self._Z = None
 
         if (self.lambda_ is not None) & (self.nu_ is not None):
             assert self.lambda_ >= 0, ValueError('Value for parameter lambda must be strictly greater to 0 (lambda_ > 0)')
             assert self.nu_ >= 0, ValueError('Value for parameter nu must be greater or equal to 0 (nu_ >= 0)')
+            warnings.filterwarnings("error")
             self._Z = self.Z()
+            warnings.resetwarnings()
+
+        self.nll_fun = lambda params, data, j: self.nloglike(params=params, data=data, j=j)
 
     def Z(self, j=None) -> float:
         """Compute the :math:`Z` factor, normalizing constant.
 
         The factor :math:`Z(\\lambda, \\nu)` serves as a normalizing constant such that the distribution satisfies the basic probability axioms (i.e. the probability mass function sums up to 1).
 
         .. math::
@@ -327,23 +336,38 @@
 
         :return: Z factor
         :rtype: :obj:`float`
         """
         j = j if j else self.j
         z_i = 0
         for i in range(j):
+            _dec = False
+            # We use a decimal placeholder variable in case we encounter overflow errors (number is too long).
+            # We don't use decimal as a default but only in case of error because it slows down computations,
+            # therefore, by default we use light and simple format and call Decimal when needed.
+            # For instances where we need Decimal, we will transform back the ratio of decimals to float as
+            # the value will be of reasonable size and not too long for a classical float.
+
+            # Compute the denominator
             try:
-                _denom = math.factorial(i)**self.nu_
-                _dec = False
+                _denom = math.factorial(i) ** self.nu_
             except OverflowError:
-                _denom = Decimal(math.factorial(i))**Decimal(self.nu_)
+                # If overflow error (i.e. output is too long), use Decimal format
+                _denom = Decimal(math.factorial(i)) ** Decimal(self.nu_)
+                _dec = True
+            # Compute the numerator
+            try:
+                _num = self.lambda_ ** i
+            except RuntimeWarning:
+                # If runtime warning it is similar to overflow error (i.e. output is too long), use Decimal format
+                _num = Decimal(self.lambda_) ** Decimal(i)
                 _dec = True
 
-            _num = self.lambda_**i
             if _dec:
+                _denom = Decimal(_denom)
                 _num = Decimal(_num)
             z_i += float(_num / _denom)
 
         return float(np.sum(z_i))
 
     def pmf(self, x) -> float:
         """Computes the probability mass function for selected value :obj:`x`.
@@ -361,17 +385,17 @@
         :rtype: :obj:`float`
         """
         x = [x] if type(x) in [float, int] else x
 
         # Compute $\lambda^{x}$
         _pow = [pow(self.lambda_, _x) for _x in x]
 
+        _dec = False
         try:
             _pow = [float(p) for p in _pow]
-            _dec = False
         except OverflowError:
             # Inf the integers to compute are too large, we use decimal format
             # Ref: https://stackoverflow.com/questions/16174399/overflowerror-long-int-too-large-to-convert-to-float-in-python
             _pow = [Decimal(p) for p in _pow]
             _dec = True
 
         # Compute $(x!)^{\nu}$
@@ -397,29 +421,61 @@
         :type data: :obj:`numpy.array` or :obj:`list` or :obj:`pandas.Series`
         :param j: Length of the inifinite sum for the normalizing factor :math:`Z`, defaults to 100
         :type j: :obj:`int`, optional
 
         :return: Negative log-likelihood
         :rtype: :obj:`float`
         """
-        # TODO: improve function so param j can be changed from calling fit() function
         lambda_ = params[0]
         nu_ = params[1]
         X = np.asarray(data)
 
-        z_i = []
+        z_i = 0
         for i in range(j):
-            z_i += [(lambda_**i) / (math.factorial(i)**nu_)]
-        log_Z = np.log(np.sum(z_i))
+            _dec = False
+            # We use a decimal placeholder variable in case we encounter overflow errors (number is too long).
+            # We don't use decimal as a default but only in case of error because it slows down computations,
+            # therefore, by default we use light and simple format and call Decimal when needed.
+            # For instances where we need Decimal, we will transform back the ratio of decimals to float as
+            # the value will be of reasonable size and not too long for a classical float.
+
+            # Compute denominator
+            try:
+                # Try normal formula
+                _denom = math.factorial(i) ** nu_
+            except OverflowError:
+                # If overflow error (i.e. output is too long), use Decimal format
+                _denom = Decimal(math.factorial(i)) ** Decimal(nu_)
+                _dec = True
+
+            # Compute numerator
+            try:
+                _num = lambda_ ** i
+            except RuntimeWarning:
+                # If runtime warning it is similar to overflow error (i.e. output is too long), use Decimal format
+                _num = Decimal(lambda_) ** Decimal(i)
+                _dec = True
+
+            # If decimal was used
+            if _dec:
+                # If decimal was used for one of denominator or denominator, we apply decimal to all (for format consistency)
+                _denom = Decimal(_denom)
+                _num = Decimal(_num)
+
+            # Then compute the ratio and transform to float (whether decimal was used or not)
+            z_i += float(_num / _denom)
+
+        # Compute log(Z)
+        log_Z = np.log(z_i)
 
         _log_fact = np.asarray([math.log(math.factorial(_x)) for _x in X])
         ll = (math.log(lambda_) * np.sum(X)) - (nu_ * np.sum(_log_fact)) - (len(X) * log_Z)
         return -ll
 
-    def fit(self, data, method='L-BFGS-B', init_params=np.array([1., 1.]), **kwargs) -> dict:
+    def fit(self, data, method='L-BFGS-B', init_params=np.array([1., 1.]), j=None) -> dict:
         """Estimates the parameters :math:`\\lambda` and :math:`\\nu` of the distribution from empirical data based on Maximum Likelihood Estimation.
 
         .. note::
 
             There is no close form to estimate the parameters nor a direct relation between the empirical moments (:math:`\\bar{X}`) and the theoretical ones.
             Therefore, only MLE is available (no fast method).
 
@@ -429,20 +485,24 @@
         :type method: obj:`str`, optional
         :param init_params: Initial parameters for the optimization method, defaults to obj:`np.array([1., 1.])`
         :type init_params: obj:`numpy.array`, optional
 
         :return: Estimated parameters
         :rtype: obj:`dict`
         """
+        # We transform warnings as error (for overflow) to handle in try / except: https://stackoverflow.com/questions/5644836/
+        warnings.filterwarnings("error")
+        j = j if j else self.j
         bounds = [(self.eps, None), (self.eps, None)]
 
-        res = self._fit(data=data, bounds=bounds, method=method, init_params=init_params, **kwargs)
+        res = self._fit(data=data, bounds=bounds, method=method, init_params=init_params, args=(j,))
         self.lambda_ = res.x[0]
         self.nu_ = res.x[1]
         self._Z = self.Z()
+        warnings.resetwarnings()
 
         out = {'lambda_': self.lambda_, 'nu_': self.nu_}
 
         if method in scipy_methods:
             out.update({'nll': self.nll})
 
         return out
```

### Comparing `statinf-1.2.0/statinf/misc.py` & `statinf-1.2.1/statinf/misc.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.0/statinf/ml/activations.py` & `statinf-1.2.1/statinf/ml/activations.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.0/statinf/ml/initializations.py` & `statinf-1.2.1/statinf/ml/initializations.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.0/statinf/ml/losses.py` & `statinf-1.2.1/statinf/ml/losses.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.0/statinf/ml/neuralnetwork.py` & `statinf-1.2.1/statinf/ml/neuralnetwork.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.0/statinf/ml/optimizers.py` & `statinf-1.2.1/statinf/ml/optimizers.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.0/statinf/ml/performance.py` & `statinf-1.2.1/statinf/ml/performance.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.0/statinf/nonparametrics/kernels.py` & `statinf-1.2.1/statinf/nonparametrics/kernels.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.0/statinf/regressions/LinearModels.py` & `statinf-1.2.1/statinf/regressions/LinearModels.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.0/statinf/regressions/glm.py` & `statinf-1.2.1/statinf/regressions/glm.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.0/statinf/regressions/glm_test.py` & `statinf-1.2.1/statinf/regressions/glm_test.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.0/statinf/stats/bayesian.py` & `statinf-1.2.1/statinf/stats/bayesian.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.0/statinf/stats/descriptive.py` & `statinf-1.2.1/statinf/stats/descriptive.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.0/statinf/stats/tests.py` & `statinf-1.2.1/statinf/stats/tests.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.0/statinf/stats/timeseries.py` & `statinf-1.2.1/statinf/stats/timeseries.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.0/statinf/stats/unsupervised.py` & `statinf-1.2.1/statinf/stats/unsupervised.py`

 * *Files identical despite different names*

### Comparing `statinf-1.2.0/statinf.egg-info/PKG-INFO` & `statinf-1.2.1/statinf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statinf
-Version: 1.2.0
+Version: 1.2.1
 Summary: A library for statistics and causal inference
 Home-page: https://www.florianfelice.com/statinf
 Author: Florian Felice
 Author-email: florian.felice@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `statinf-1.2.0/statinf.egg-info/SOURCES.txt` & `statinf-1.2.1/statinf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

