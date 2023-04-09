# Comparing `tmp/searchlogit-0.3.3.tar.gz` & `tmp/searchlogit-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchlogit-0.3.3.tar", last modified: Sun Apr  9 07:26:32 2023, max compression
+gzip compressed data, was "searchlogit-0.3.4.tar", last modified: Sun Apr  9 07:39:11 2023, max compression
```

## Comparing `searchlogit-0.3.3.tar` & `searchlogit-0.3.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:26:32.078702 searchlogit-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-09 07:26:23.000000 searchlogit-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-09 07:26:32.078702 searchlogit-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-09 07:26:23.000000 searchlogit-0.3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:26:32.074702 searchlogit-0.3.3/searchlogit/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-09 07:26:23.000000 searchlogit-0.3.3/searchlogit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29646 2023-04-09 07:26:23.000000 searchlogit-0.3.3/searchlogit/_choice_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-09 07:26:23.000000 searchlogit-0.3.3/searchlogit/_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-09 07:26:23.000000 searchlogit-0.3.3/searchlogit/boxcox_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    50431 2023-04-09 07:26:23.000000 searchlogit-0.3.3/searchlogit/latent_class_mixed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    35382 2023-04-09 07:26:23.000000 searchlogit-0.3.3/searchlogit/latent_class_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    60055 2023-04-09 07:26:23.000000 searchlogit-0.3.3/searchlogit/mixed_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)    14368 2023-04-09 07:26:23.000000 searchlogit-0.3.3/searchlogit/multinomial_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)   168244 2023-04-09 07:26:23.000000 searchlogit-0.3.3/searchlogit/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:26:32.078702 searchlogit-0.3.3/searchlogit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-09 07:26:32.000000 searchlogit-0.3.3/searchlogit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-09 07:26:32.000000 searchlogit-0.3.3/searchlogit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 07:26:32.000000 searchlogit-0.3.3/searchlogit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 07:26:31.000000 searchlogit-0.3.3/searchlogit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-09 07:26:32.000000 searchlogit-0.3.3/searchlogit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-09 07:26:32.000000 searchlogit-0.3.3/searchlogit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-09 07:26:32.078702 searchlogit-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-09 07:26:23.000000 searchlogit-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:26:32.078702 searchlogit-0.3.3/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-04-09 07:26:23.000000 searchlogit-0.3.3/tests/test__choice_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-04-09 07:26:23.000000 searchlogit-0.3.3/tests/test__device.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-09 07:26:23.000000 searchlogit-0.3.3/tests/test_latent_class_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-09 07:26:23.000000 searchlogit-0.3.3/tests/test_mixed_logit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2862 2023-04-09 07:26:23.000000 searchlogit-0.3.3/tests/test_multinomial_logit.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 07:26:23.000000 searchlogit-0.3.3/tests/test_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:39:11.129745 searchlogit-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-09 07:39:01.000000 searchlogit-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-09 07:39:11.129745 searchlogit-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-09 07:39:01.000000 searchlogit-0.3.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:39:11.129745 searchlogit-0.3.4/searchlogit/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-09 07:39:02.000000 searchlogit-0.3.4/searchlogit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29646 2023-04-09 07:39:02.000000 searchlogit-0.3.4/searchlogit/_choice_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-09 07:39:02.000000 searchlogit-0.3.4/searchlogit/_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-09 07:39:02.000000 searchlogit-0.3.4/searchlogit/boxcox_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50431 2023-04-09 07:39:02.000000 searchlogit-0.3.4/searchlogit/latent_class_mixed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35382 2023-04-09 07:39:02.000000 searchlogit-0.3.4/searchlogit/latent_class_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60055 2023-04-09 07:39:02.000000 searchlogit-0.3.4/searchlogit/mixed_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14368 2023-04-09 07:39:02.000000 searchlogit-0.3.4/searchlogit/multinomial_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)   168245 2023-04-09 07:39:02.000000 searchlogit-0.3.4/searchlogit/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:39:11.129745 searchlogit-0.3.4/searchlogit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-09 07:39:11.000000 searchlogit-0.3.4/searchlogit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-09 07:39:11.000000 searchlogit-0.3.4/searchlogit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 07:39:11.000000 searchlogit-0.3.4/searchlogit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 07:39:10.000000 searchlogit-0.3.4/searchlogit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-09 07:39:11.000000 searchlogit-0.3.4/searchlogit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-09 07:39:11.000000 searchlogit-0.3.4/searchlogit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-09 07:39:11.129745 searchlogit-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-09 07:39:02.000000 searchlogit-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 07:39:11.129745 searchlogit-0.3.4/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2391 2023-04-09 07:39:02.000000 searchlogit-0.3.4/tests/test__choice_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-04-09 07:39:02.000000 searchlogit-0.3.4/tests/test__device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-09 07:39:02.000000 searchlogit-0.3.4/tests/test_latent_class_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-09 07:39:02.000000 searchlogit-0.3.4/tests/test_mixed_logit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2862 2023-04-09 07:39:02.000000 searchlogit-0.3.4/tests/test_multinomial_logit.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 07:39:02.000000 searchlogit-0.3.4/tests/test_search.py
```

### Comparing `searchlogit-0.3.3/LICENSE` & `searchlogit-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.3/PKG-INFO` & `searchlogit-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchlogit
-Version: 0.3.3
+Version: 0.3.4
 Summary: Extensions for a Python package for                               GPU-accelerated estimation of mixed logit models.
 Home-page: https://github.com/RyanJafefKelly/searchlogit
 Author: Ryan Kelly, Prithvi Beeramoole and Alexander Paz
 Author-email: ryan@kiiii.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
```

### Comparing `searchlogit-0.3.3/README.rst` & `searchlogit-0.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.3/searchlogit/_choice_model.py` & `searchlogit-0.3.4/searchlogit/_choice_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.3/searchlogit/_device.py` & `searchlogit-0.3.4/searchlogit/_device.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.3/searchlogit/boxcox_functions.py` & `searchlogit-0.3.4/searchlogit/boxcox_functions.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.3/searchlogit/latent_class_mixed_model.py` & `searchlogit-0.3.4/searchlogit/latent_class_mixed_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.3/searchlogit/latent_class_model.py` & `searchlogit-0.3.4/searchlogit/latent_class_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.3/searchlogit/mixed_logit.py` & `searchlogit-0.3.4/searchlogit/mixed_logit.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.3/searchlogit/multinomial_logit.py` & `searchlogit-0.3.4/searchlogit/multinomial_logit.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.3/searchlogit/search.py` & `searchlogit-0.3.4/searchlogit/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -3005,15 +3005,15 @@
         else:
             best_varnames = best_asvarnames + best_isvarnames
 
         # delete '_inter' bug fix
         if '_inter' in best_varnames:
             best_varnames = np.delete(best_varnames, np.argwhere(best_varnames == '_inter'))
         logger.info("Estimating best solution with entire dataset.")
-        d_all = self.df
+        df_all = self.df
         if self.multi_objective:
             df_all = self.df.append(self.df_test)
 
         X = df_all[best_varnames]
         y = self.choice_var.append(self.test_choice_var)
         seed = self.random_state.randint(2**31 - 1)
```

### Comparing `searchlogit-0.3.3/searchlogit.egg-info/PKG-INFO` & `searchlogit-0.3.4/searchlogit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchlogit
-Version: 0.3.3
+Version: 0.3.4
 Summary: Extensions for a Python package for                               GPU-accelerated estimation of mixed logit models.
 Home-page: https://github.com/RyanJafefKelly/searchlogit
 Author: Ryan Kelly, Prithvi Beeramoole and Alexander Paz
 Author-email: ryan@kiiii.com
 License: MIT
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
```

### Comparing `searchlogit-0.3.3/searchlogit.egg-info/SOURCES.txt` & `searchlogit-0.3.4/searchlogit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.3/setup.py` & `searchlogit-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import setuptools
 
 with codecs.open("README.rst", encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(name='searchlogit',
-                 version='0.3.3',
+                 version='0.3.4',
                  description='Extensions for a Python package for \
                               GPU-accelerated estimation of mixed logit models.',
                  long_description=long_description,
                  long_description_content_type="text/x-rst",
                  url='https://github.com/RyanJafefKelly/searchlogit',
                  author='Ryan Kelly, Prithvi Beeramoole and Alexander Paz',
                  author_email='ryan@kiiii.com',
```

### Comparing `searchlogit-0.3.3/tests/test__choice_model.py` & `searchlogit-0.3.4/tests/test__choice_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.3/tests/test__device.py` & `searchlogit-0.3.4/tests/test__device.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.3/tests/test_latent_class_model.py` & `searchlogit-0.3.4/tests/test_latent_class_model.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.3/tests/test_mixed_logit.py` & `searchlogit-0.3.4/tests/test_mixed_logit.py`

 * *Files identical despite different names*

### Comparing `searchlogit-0.3.3/tests/test_multinomial_logit.py` & `searchlogit-0.3.4/tests/test_multinomial_logit.py`

 * *Files identical despite different names*

