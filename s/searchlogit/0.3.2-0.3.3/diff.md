# Comparing `tmp/searchlogit-0.3.2.tar.gz` & `tmp/searchlogit-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchlogit-0.3.2.tar", last modified: Sun Apr  9 07:23:46 2023, max compression
+gzip compressed data, was "searchlogit-0.3.3.tar", last modified: Sun Apr  9 07:26:32 2023, max compression
```

## Comparing `searchlogit-0.3.2.tar` & `searchlogit-0.3.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:23:46.877846 searchlogit-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-09 07:23:37.000000 searchlogit-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-09 07:23:46.877846 searchlogit-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-09 07:23:37.000000 searchlogit-0.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:23:46.877846 searchlogit-0.3.2/searchlogit/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-09 07:23:37.000000 searchlogit-0.3.2/searchlogit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29646 2023-04-09 07:23:37.000000 searchlogit-0.3.2/searchlogit/_choice_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-09 07:23:37.000000 searchlogit-0.3.2/searchlogit/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-09 07:23:37.000000 searchlogit-0.3.2/searchlogit/boxcox_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    50431 2023-04-09 07:23:37.000000 searchlogit-0.3.2/searchlogit/latent_class_mixed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    35382 2023-04-09 07:23:37.000000 searchlogit-0.3.2/searchlogit/latent_class_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    60055 2023-04-09 07:23:37.000000 searchlogit-0.3.2/searchlogit/mixed_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)    15251 2023-04-09 07:23:37.000000 searchlogit-0.3.2/searchlogit/multinomial_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)   168244 2023-04-09 07:23:37.000000 searchlogit-0.3.2/searchlogit/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:23:46.877846 searchlogit-0.3.2/searchlogit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-09 07:23:46.000000 searchlogit-0.3.2/searchlogit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-09 07:23:46.000000 searchlogit-0.3.2/searchlogit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 07:23:46.000000 searchlogit-0.3.2/searchlogit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 07:23:46.000000 searchlogit-0.3.2/searchlogit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-09 07:23:46.000000 searchlogit-0.3.2/searchlogit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-09 07:23:46.000000 searchlogit-0.3.2/searchlogit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-09 07:23:46.877846 searchlogit-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-09 07:23:37.000000 searchlogit-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:23:46.877846 searchlogit-0.3.2/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-04-09 07:23:37.000000 searchlogit-0.3.2/tests/test__choice_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-04-09 07:23:37.000000 searchlogit-0.3.2/tests/test__device.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-09 07:23:37.000000 searchlogit-0.3.2/tests/test_latent_class_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-09 07:23:37.000000 searchlogit-0.3.2/tests/test_mixed_logit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2862 2023-04-09 07:23:37.000000 searchlogit-0.3.2/tests/test_multinomial_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 07:23:37.000000 searchlogit-0.3.2/tests/test_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:26:32.078702 searchlogit-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-09 07:26:23.000000 searchlogit-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-09 07:26:32.078702 searchlogit-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-09 07:26:23.000000 searchlogit-0.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:26:32.074702 searchlogit-0.3.3/searchlogit/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-09 07:26:23.000000 searchlogit-0.3.3/searchlogit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29646 2023-04-09 07:26:23.000000 searchlogit-0.3.3/searchlogit/_choice_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-09 07:26:23.000000 searchlogit-0.3.3/searchlogit/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-09 07:26:23.000000 searchlogit-0.3.3/searchlogit/boxcox_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50431 2023-04-09 07:26:23.000000 searchlogit-0.3.3/searchlogit/latent_class_mixed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35382 2023-04-09 07:26:23.000000 searchlogit-0.3.3/searchlogit/latent_class_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60055 2023-04-09 07:26:23.000000 searchlogit-0.3.3/searchlogit/mixed_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14368 2023-04-09 07:26:23.000000 searchlogit-0.3.3/searchlogit/multinomial_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)   168244 2023-04-09 07:26:23.000000 searchlogit-0.3.3/searchlogit/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:26:32.078702 searchlogit-0.3.3/searchlogit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-09 07:26:32.000000 searchlogit-0.3.3/searchlogit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-09 07:26:32.000000 searchlogit-0.3.3/searchlogit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 07:26:32.000000 searchlogit-0.3.3/searchlogit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 07:26:31.000000 searchlogit-0.3.3/searchlogit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-09 07:26:32.000000 searchlogit-0.3.3/searchlogit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-09 07:26:32.000000 searchlogit-0.3.3/searchlogit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-09 07:26:32.078702 searchlogit-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-09 07:26:23.000000 searchlogit-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:26:32.078702 searchlogit-0.3.3/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-04-09 07:26:23.000000 searchlogit-0.3.3/tests/test__choice_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-04-09 07:26:23.000000 searchlogit-0.3.3/tests/test__device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-09 07:26:23.000000 searchlogit-0.3.3/tests/test_latent_class_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-09 07:26:23.000000 searchlogit-0.3.3/tests/test_mixed_logit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2862 2023-04-09 07:26:23.000000 searchlogit-0.3.3/tests/test_multinomial_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 07:26:23.000000 searchlogit-0.3.3/tests/test_search.py
```

### Comparing `searchlogit-0.3.2/LICENSE` & `searchlogit-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.2/PKG-INFO` & `searchlogit-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchlogit
-Version: 0.3.2
+Version: 0.3.3
 Summary: Extensions for a Python package for                               GPU-accelerated estimation of mixed logit models.
 Home-page: https://github.com/RyanJafefKelly/searchlogit
 Author: Ryan Kelly, Prithvi Beeramoole and Alexander Paz
 Author-email: ryan@kiiii.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
```

### Comparing `searchlogit-0.3.2/README.rst` & `searchlogit-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.2/searchlogit/_choice_model.py` & `searchlogit-0.3.3/searchlogit/_choice_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.2/searchlogit/_device.py` & `searchlogit-0.3.3/searchlogit/_device.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.2/searchlogit/boxcox_functions.py` & `searchlogit-0.3.3/searchlogit/boxcox_functions.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.2/searchlogit/latent_class_mixed_model.py` & `searchlogit-0.3.3/searchlogit/latent_class_mixed_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.2/searchlogit/latent_class_model.py` & `searchlogit-0.3.3/searchlogit/latent_class_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.2/searchlogit/mixed_logit.py` & `searchlogit-0.3.3/searchlogit/mixed_logit.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.2/searchlogit/multinomial_logit.py` & `searchlogit-0.3.3/searchlogit/multinomial_logit.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,15 +134,14 @@
                 if var in transvars:
                     self.fxidx.append(False)
                     self.fxtransidx.append(True)
                 else:
                     self.fxtransidx.append(False)
                     self.fxidx.append(True)
 
-        # X, y, panels = self._arrange_long_format(X, y, ids, alts)
         self.grad = grad
         self.hess = hess
         self.gtol = gtol
         self.ftol = ftol
         self.method = method
 
         jac = True if self.grad else False
@@ -176,36 +175,20 @@
 
         if weights is not None:
             weights = weights.reshape(X.shape[0], X.shape[1])
 
         if avail is not None:
             avail = avail.reshape(X.shape[0], X.shape[1])
 
-        # saved to self to allow loglik calls outside fit without setuping up
-        # self.X = X
-        # self.weights = weights
-        # self.avail = avail
-
-        #  add transformation vars and corresponding lambdas
-        # lambda_names = ["lambda.{}".format(transvar) for transvar in transvars]
-        # transnames = np.concatenate((transvars, lambda_names))
-        # Xnames = np.concatenate((Xnames, transnames))
-        # self.Xnames = Xnames
-
         # Note: taken from mixed logit code for LCM  # TODO? restructure
-        # if panels is None and self.panels is not None:
-        #     panels = self.panels
         if self.panels is not None:  # If panels
             _, _, panel_info = self._balance_panels(X, y, self.panels)
             self.panel_info = panel_info
-            # N, _ = panel_info.shape
             N = X.shape[0]
-        # else:
-        #     N, _ = X.shape[0], 1
-        #     panel_info = np.ones((N, 1))
+
         y = y.reshape(-1, self.J)
         X = X.astype('float64')
         y = y.astype('float64')
 
         self.y = y
 
         self.obs_prob = np.mean(y, axis=0)
@@ -265,26 +248,24 @@
         self.total_fun_eval += 1
 
         p, Xtrans_lmda = self._compute_probabilities(betas, X, avail)
         # Log likelihood
         lik = np.sum(y*p, axis=1, dtype="float64")
         lik[lik == 0] = min_comp_val
         loglik = np.log(lik)
-        # if loglik.ndim == 2:  # case panels in LCCM
-        #     loglik =np.sum()
+
         if weights is not None:
             loglik = loglik * weights[:, 0]  # doesn't matter which col.
         loglik = np.sum(loglik, dtype="float64")
 
         # Individual contribution to the gradient
 
         transpos = [self.varnames.tolist().index(i) for i in self.transvars]  # Position of trans vars
         B_trans = betas[self.Kf:self.Kf+self.Kftrans]
         lambdas = betas[self.Kf+self.Kftrans:]
-        # X_trans = self.initialData[:, transpos]
         X_trans = X[:, :, transpos]
         X_trans = X_trans.reshape(self.N, len(self.alternatives), len(transpos))
         X_trans = X_trans.astype('float64')
         ymp = y - p
         ymp = ymp.astype('float64')
         if self.Kf > 0:
             Xf = X[:, :, self.fxidx]
```

### Comparing `searchlogit-0.3.2/searchlogit/search.py` & `searchlogit-0.3.3/searchlogit/search.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.2/searchlogit.egg-info/PKG-INFO` & `searchlogit-0.3.3/searchlogit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchlogit
-Version: 0.3.2
+Version: 0.3.3
 Summary: Extensions for a Python package for                               GPU-accelerated estimation of mixed logit models.
 Home-page: https://github.com/RyanJafefKelly/searchlogit
 Author: Ryan Kelly, Prithvi Beeramoole and Alexander Paz
 Author-email: ryan@kiiii.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
```

### Comparing `searchlogit-0.3.2/searchlogit.egg-info/SOURCES.txt` & `searchlogit-0.3.3/searchlogit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.2/setup.py` & `searchlogit-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import setuptools
 
 with codecs.open("README.rst", encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(name='searchlogit',
-                 version='0.3.2',
+                 version='0.3.3',
                  description='Extensions for a Python package for \
                               GPU-accelerated estimation of mixed logit models.',
                  long_description=long_description,
                  long_description_content_type="text/x-rst",
                  url='https://github.com/RyanJafefKelly/searchlogit',
                  author='Ryan Kelly, Prithvi Beeramoole and Alexander Paz',
                  author_email='ryan@kiiii.com',
```

### Comparing `searchlogit-0.3.2/tests/test__choice_model.py` & `searchlogit-0.3.3/tests/test__choice_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.2/tests/test__device.py` & `searchlogit-0.3.3/tests/test__device.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.2/tests/test_latent_class_model.py` & `searchlogit-0.3.3/tests/test_latent_class_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.2/tests/test_mixed_logit.py` & `searchlogit-0.3.3/tests/test_mixed_logit.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.2/tests/test_multinomial_logit.py` & `searchlogit-0.3.3/tests/test_multinomial_logit.py`

 * *Files identical despite different names*

