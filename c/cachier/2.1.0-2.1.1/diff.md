# Comparing `tmp/cachier-2.1.0.tar.gz` & `tmp/cachier-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachier-2.1.0.tar", last modified: Fri Mar 31 07:34:24 2023, max compression
+gzip compressed data, was "cachier-2.1.1.tar", last modified: Sun Apr  9 05:18:54 2023, max compression
```

## Comparing `cachier-2.1.0.tar` & `cachier-2.1.1.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-03-31 07:34:24.782755 cachier-2.1.0/
--rw-r--r--   0 shaypalachy   (501) staff       (20)      447 2021-06-17 12:08:06.000000 cachier-2.1.0/.codecov.yml
--rw-r--r--   0 shaypalachy   (501) staff       (20)      361 2021-06-17 12:08:06.000000 cachier-2.1.0/.coveragerc
--rw-r--r--   0 shaypalachy   (501) staff       (20)      195 2021-06-17 12:08:06.000000 cachier-2.1.0/.deepsource.toml
--rw-r--r--   0 shaypalachy   (501) staff       (20)       30 2021-10-10 23:14:34.000000 cachier-2.1.0/.fdignore
--rw-r--r--   0 shaypalachy   (501) staff       (20)      202 2022-12-02 11:10:23.000000 cachier-2.1.0/.flake8
--rw-r--r--   0 shaypalachy   (501) staff       (20)       33 2021-06-17 12:08:06.000000 cachier-2.1.0/.gitattributes
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-03-31 07:34:24.759464 cachier-2.1.0/.github/
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-03-31 07:34:24.772750 cachier-2.1.0/.github/workflows/
--rw-r--r--   0 shaypalachy   (501) staff       (20)      680 2023-03-16 11:40:57.000000 cachier-2.1.0/.github/workflows/checkdocs.yml
--rw-r--r--   0 shaypalachy   (501) staff       (20)      746 2023-03-16 11:40:57.000000 cachier-2.1.0/.github/workflows/lint.yml
--rw-r--r--   0 shaypalachy   (501) staff       (20)      982 2023-03-22 22:40:25.000000 cachier-2.1.0/.github/workflows/test.yml
--rw-r--r--   0 shaypalachy   (501) staff       (20)     1249 2021-06-17 12:08:06.000000 cachier-2.1.0/.gitignore
--rw-r--r--   0 shaypalachy   (501) staff       (20)       67 2022-12-02 11:08:24.000000 cachier-2.1.0/.ignore
--rw-r--r--   0 shaypalachy   (501) staff       (20)     8489 2021-10-10 23:14:34.000000 cachier-2.1.0/.pylintrc
--rw-r--r--   0 shaypalachy   (501) staff       (20)     1069 2021-06-17 12:08:06.000000 cachier-2.1.0/LICENSE
--rw-r--r--   0 shaypalachy   (501) staff       (20)       50 2021-06-17 12:08:06.000000 cachier-2.1.0/MANIFEST.in
--rw-r--r--   0 shaypalachy   (501) staff       (20)    15801 2023-03-31 07:34:24.782949 cachier-2.1.0/PKG-INFO
--rw-r--r--   0 shaypalachy   (501) staff       (20)    14757 2023-03-31 07:33:42.000000 cachier-2.1.0/README.rst
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-03-31 07:34:24.783770 cachier-2.1.0/cachier/
--rw-r--r--   0 shaypalachy   (501) staff       (20)      133 2022-12-02 11:07:34.000000 cachier-2.1.0/cachier/__init__.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)      471 2023-03-31 07:34:24.783835 cachier-2.1.0/cachier/_version.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     2663 2023-03-31 07:33:42.000000 cachier-2.1.0/cachier/base_core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)    11454 2023-03-31 07:33:42.000000 cachier-2.1.0/cachier/core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     3020 2023-03-31 07:33:42.000000 cachier-2.1.0/cachier/memory_core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     5114 2023-03-31 07:33:42.000000 cachier-2.1.0/cachier/mongo_core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)    10150 2023-03-31 07:33:42.000000 cachier-2.1.0/cachier/pickle_core.py
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-03-31 07:34:24.778178 cachier-2.1.0/cachier/scripts/
--rw-r--r--   0 shaypalachy   (501) staff       (20)        0 2021-06-17 12:08:06.000000 cachier-2.1.0/cachier/scripts/__init__.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)      429 2021-06-17 12:08:06.000000 cachier-2.1.0/cachier/scripts/cli.py
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-03-31 07:34:24.777659 cachier-2.1.0/cachier.egg-info/
--rw-r--r--   0 shaypalachy   (501) staff       (20)    15801 2023-03-31 07:34:24.000000 cachier-2.1.0/cachier.egg-info/PKG-INFO
--rw-r--r--   0 shaypalachy   (501) staff       (20)      883 2023-03-31 07:34:24.000000 cachier-2.1.0/cachier.egg-info/SOURCES.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)        1 2023-03-31 07:34:24.000000 cachier-2.1.0/cachier.egg-info/dependency_links.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)       71 2023-03-31 07:34:24.000000 cachier-2.1.0/cachier.egg-info/entry_points.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)      185 2023-03-31 07:34:24.000000 cachier-2.1.0/cachier.egg-info/requires.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)        8 2023-03-31 07:34:24.000000 cachier-2.1.0/cachier.egg-info/top_level.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)      289 2021-10-10 23:14:34.000000 cachier-2.1.0/pytest.ini
--rw-r--r--   0 shaypalachy   (501) staff       (20)      269 2023-03-31 07:34:24.783520 cachier-2.1.0/setup.cfg
--rw-r--r--   0 shaypalachy   (501) staff       (20)     2531 2023-03-23 18:10:50.000000 cachier-2.1.0/setup.py
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-03-31 07:34:24.782302 cachier-2.1.0/tests/
--rw-r--r--   0 shaypalachy   (501) staff       (20)        0 2021-06-17 12:08:06.000000 cachier-2.1.0/tests/__init__.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     1903 2023-03-22 22:40:25.000000 cachier-2.1.0/tests/speed_eval.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)      168 2023-03-31 07:33:42.000000 cachier-2.1.0/tests/standalone_script.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)      729 2021-10-10 23:14:34.000000 cachier-2.1.0/tests/test_core_lookup.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     6336 2023-03-31 07:33:42.000000 cachier-2.1.0/tests/test_general.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     8879 2023-03-31 07:33:42.000000 cachier-2.1.0/tests/test_memory_core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     8705 2023-03-31 07:33:42.000000 cachier-2.1.0/tests/test_mongo_core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)    17834 2023-03-31 07:33:42.000000 cachier-2.1.0/tests/test_pickle_core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)      482 2023-03-22 22:40:25.000000 cachier-2.1.0/tests/test_quality.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)      577 2023-03-22 22:40:25.000000 cachier-2.1.0/tests/test_security.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)    65747 2021-06-17 12:08:06.000000 cachier-2.1.0/versioneer.py
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-04-09 05:18:54.179899 cachier-2.1.1/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      447 2021-06-17 12:08:06.000000 cachier-2.1.1/.codecov.yml
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      394 2023-04-09 05:18:24.000000 cachier-2.1.1/.coveragerc
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      195 2021-06-17 12:08:06.000000 cachier-2.1.1/.deepsource.toml
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       30 2021-10-10 23:14:34.000000 cachier-2.1.1/.fdignore
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      202 2022-12-02 11:10:23.000000 cachier-2.1.1/.flake8
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       33 2021-06-17 12:08:06.000000 cachier-2.1.1/.gitattributes
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-04-09 05:18:54.158541 cachier-2.1.1/.github/
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-04-09 05:18:54.170232 cachier-2.1.1/.github/workflows/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      680 2023-03-16 11:40:57.000000 cachier-2.1.1/.github/workflows/checkdocs.yml
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      746 2023-03-16 11:40:57.000000 cachier-2.1.1/.github/workflows/lint.yml
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      982 2023-03-22 22:40:25.000000 cachier-2.1.1/.github/workflows/test.yml
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     1249 2021-06-17 12:08:06.000000 cachier-2.1.1/.gitignore
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       67 2022-12-02 11:08:24.000000 cachier-2.1.1/.ignore
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     8489 2021-10-10 23:14:34.000000 cachier-2.1.1/.pylintrc
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     1069 2021-06-17 12:08:06.000000 cachier-2.1.1/LICENSE
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       50 2021-06-17 12:08:06.000000 cachier-2.1.1/MANIFEST.in
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    17286 2023-04-09 05:18:54.180055 cachier-2.1.1/PKG-INFO
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    16242 2023-04-09 05:18:24.000000 cachier-2.1.1/README.rst
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-04-09 05:18:54.180849 cachier-2.1.1/cachier/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      232 2023-04-09 05:18:24.000000 cachier-2.1.1/cachier/__init__.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      471 2023-04-09 05:18:54.180904 cachier-2.1.1/cachier/_version.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     3062 2023-04-09 05:18:24.000000 cachier-2.1.1/cachier/base_core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    13492 2023-04-09 05:18:24.000000 cachier-2.1.1/cachier/core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     2846 2023-04-09 05:18:24.000000 cachier-2.1.1/cachier/memory_core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     5022 2023-04-09 05:18:24.000000 cachier-2.1.1/cachier/mongo_core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    10068 2023-04-09 05:18:24.000000 cachier-2.1.1/cachier/pickle_core.py
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-04-09 05:18:54.173958 cachier-2.1.1/cachier/scripts/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)        0 2021-06-17 12:08:06.000000 cachier-2.1.1/cachier/scripts/__init__.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      429 2021-06-17 12:08:06.000000 cachier-2.1.1/cachier/scripts/cli.py
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-04-09 05:18:54.173587 cachier-2.1.1/cachier.egg-info/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    17286 2023-04-09 05:18:53.000000 cachier-2.1.1/cachier.egg-info/PKG-INFO
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      906 2023-04-09 05:18:53.000000 cachier-2.1.1/cachier.egg-info/SOURCES.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)        1 2023-04-09 05:18:53.000000 cachier-2.1.1/cachier.egg-info/dependency_links.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       71 2023-04-09 05:18:53.000000 cachier-2.1.1/cachier.egg-info/entry_points.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      185 2023-04-09 05:18:53.000000 cachier-2.1.1/cachier.egg-info/requires.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)        8 2023-04-09 05:18:53.000000 cachier-2.1.1/cachier.egg-info/top_level.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      308 2023-04-09 05:18:24.000000 cachier-2.1.1/pytest.ini
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      269 2023-04-09 05:18:54.180603 cachier-2.1.1/setup.cfg
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     2531 2023-03-23 18:10:50.000000 cachier-2.1.1/setup.py
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-04-09 05:18:54.179375 cachier-2.1.1/tests/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)        0 2021-06-17 12:08:06.000000 cachier-2.1.1/tests/__init__.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     1903 2023-03-22 22:40:25.000000 cachier-2.1.1/tests/speed_eval.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      168 2023-03-31 07:33:42.000000 cachier-2.1.1/tests/standalone_script.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     1100 2023-04-09 05:18:24.000000 cachier-2.1.1/tests/test_core_lookup.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     5766 2023-04-09 05:18:24.000000 cachier-2.1.1/tests/test_defaults.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     6703 2023-04-09 05:18:24.000000 cachier-2.1.1/tests/test_general.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     8879 2023-03-31 07:33:42.000000 cachier-2.1.1/tests/test_memory_core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     8965 2023-04-09 05:18:24.000000 cachier-2.1.1/tests/test_mongo_core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    18208 2023-04-09 05:18:24.000000 cachier-2.1.1/tests/test_pickle_core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      482 2023-03-22 22:40:25.000000 cachier-2.1.1/tests/test_quality.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      577 2023-03-22 22:40:25.000000 cachier-2.1.1/tests/test_security.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    65747 2021-06-17 12:08:06.000000 cachier-2.1.1/versioneer.py
```

### Comparing `cachier-2.1.0/.github/workflows/checkdocs.yml` & `cachier-2.1.1/.github/workflows/checkdocs.yml`

 * *Files identical despite different names*

### Comparing `cachier-2.1.0/.github/workflows/lint.yml` & `cachier-2.1.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `cachier-2.1.0/.github/workflows/test.yml` & `cachier-2.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `cachier-2.1.0/.gitignore` & `cachier-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cachier-2.1.0/.pylintrc` & `cachier-2.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `cachier-2.1.0/LICENSE` & `cachier-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cachier-2.1.0/PKG-INFO` & `cachier-2.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachier
-Version: 2.1.0
+Version: 2.1.1
 Summary: Persistent, stale-free, local and cross-machine caching for Python functions.
 Home-page: https://github.com/python-cachier/cachier
 Author: Shay Palachy
 Author-email: shay.palachy@gmail.com
 License: MIT
 Keywords: cache,persistence,mongo,memoization,decorator
 Platform: linux
@@ -147,20 +147,51 @@
 .. code-block:: python
 
   foo.clear_cache()
 
 General Configuration
 ----------------------
 
+Global Defaults
+~~~~~~~~~~~~~~~
+
+Settings can be globally configured across all Cachier wrappers through the use of the `set_default_params` function. This function takes the same keyword parameters as the ones defined in the decorator, which can be passed all at once or with multiple calls. Parameters given directly to a decorator take precedence over any values set by this function.
+
+The following parameters will only be applied to decorators defined after `set_default_params` is called:
+
+*  `hash_func`
+*  `backend`
+*  `mongetter`
+*  `cache_dir`
+*  `pickle_reload`
+*  `separate_files`
+
+These parameters can be changed at any time and they will apply to all decorators:
+
+*  `caching_enabled`
+*  `stale_after`
+*  `next_time`
+*  `wait_for_calc_timeout`
+
+The current defaults can be fetched by calling `get_default_params`.
+
 Threads Limit
 ~~~~~~~~~~~~~
 
 To limit the number of threads Cachier is allowed to spawn, set the ``CACHIER_MAX_WORKERS`` with the desired number. The defeault is 8, so to enable Cachier to spawn even more threads, you'll have to set a higher limit explicitly.
 
 
+Global Enable/Disable
+---------------------
+
+Caching can be turned off across all decorators by calling `disable_caching`, and then re-activated by calling `enable_caching`.
+
+These functions are convenience wrappers around the `caching_enabled` default setting.
+
+
 Cache Shelf Life
 ----------------
 
 Setting Shelf Life
 ~~~~~~~~~~~~~~~~~~
 You can set any duration as the shelf life of cached return values of a function by providing a corresponding ``timedelta`` object to the ``stale_after`` parameter:
 
@@ -334,15 +365,15 @@
 
 Note, however, that ``cachier``'s in-memory core is simple, and has no monitoring or cap on cache size, and can thus lead to memory errors on large return values - it is mainly intended to be used with future multi-core functionality. As a rule, Python's built-in ``lru_cache`` is a much better stand-alone solution.
 
 
 Contributing
 ============
 
-Package author and current maintainer is Shay Palachy (shay.palachy@gmail.com); You are more than welcome to approach him for help. Contributions are very welcomed.
+Current maintainers are Shay Palachy Affek (`shay.palachy@gmail.com <mailto:shay.palachy@gmail.com>`_, `@shaypal5 <https://github.com/shaypal5>`_) and Judson Neer (`@lordjabez <https://github.com/lordjabez>`_); You are more than welcome to approach them for help. Contributions are very welcomed! :)
 
 Installing for development
 --------------------------
 
 Clone:
 
 .. code-block:: bash
@@ -403,35 +434,39 @@
 
 Additionally, if you update this ``README.rst`` file, use ``python setup.py checkdocs`` to validate it compiles.
 
 
 Credits
 =======
 
-Created by `Shay Palachy <https://github.com/shaypal5>`_ (shay.palachy@gmail.com).
+Created by `Shay Palachy Affek <https://github.com/shaypal5>`_ (shay.palachy@gmail.com).
+
+Current lead developer/contributor: `Judson Neer <https://github.com/lordjabez>`_ (`@lordjabez <https://github.com/lordjabez>`_ on GitHub).
 
 Other major contributors:
 
-  * `cthoyt <https://github.com/cthoyt>`_ - Base memory core implementation.
+* `Judson Neer <https://github.com/lordjabez>`_ - Precaching, method caching support and numerous improvements and bugfixes.
+
+* `cthoyt <https://github.com/cthoyt>`_ - Base memory core implementation.
 
-  * `amarczew <https://github.com/amarczew>`_ - The ``hash_func`` kwarg.
+* `amarczew <https://github.com/amarczew>`_ - The ``hash_func`` kwarg.
 
-  * `non-senses <https://github.com/non-senses>`_ - The ``wait_for_calc_timeout`` kwarg.
+* `non-senses <https://github.com/non-senses>`_ - The ``wait_for_calc_timeout`` kwarg.
 
-  * `Elad Rapapor <https://github.com/erap129>`_ - Multi-file Pickle core, a.k.a ``separate_files`` (released on ``v1.5.3``).
+* `Elad Rapapor <https://github.com/erap129>`_ - Multi-file Pickle core, a.k.a ``separate_files`` (released on ``v1.5.3``).
 
-  * `John Didion <https://github.com/jdidion>`_ - Support for pickle-based caching for cases where two identically-named methods of different classes are defined in the same module.
+* `John Didion <https://github.com/jdidion>`_ - Support for pickle-based caching for cases where two identically-named methods of different classes are defined in the same module.
 
 Notable bugfixers:
 
-  * `MichaelRazum <https://github.com/MichaelRazum>`_.
+* `MichaelRazum <https://github.com/MichaelRazum>`_.
 
-  * `Eric Ma <https://github.com/ericmjl>`_ - The iNotify bugfix (released on ``v1.5.3``).
+* `Eric Ma <https://github.com/ericmjl>`_ - The iNotify bugfix (released on ``v1.5.3``).
 
-  * `Ofir <https://github.com/ofirnk>`_ - The iNotify bugfix (released on ``v1.5.3``).
+* `Ofir <https://github.com/ofirnk>`_ - The iNotify bugfix (released on ``v1.5.3``).
 
 
 
 .. |PyPI-Status| image:: https://img.shields.io/pypi/v/cachier.svg
   :target: https://pypi.python.org/pypi/cachier
 
 .. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/cachier.svg
```

### Comparing `cachier-2.1.0/README.rst` & `cachier-2.1.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -119,20 +119,51 @@
 .. code-block:: python
 
   foo.clear_cache()
 
 General Configuration
 ----------------------
 
+Global Defaults
+~~~~~~~~~~~~~~~
+
+Settings can be globally configured across all Cachier wrappers through the use of the `set_default_params` function. This function takes the same keyword parameters as the ones defined in the decorator, which can be passed all at once or with multiple calls. Parameters given directly to a decorator take precedence over any values set by this function.
+
+The following parameters will only be applied to decorators defined after `set_default_params` is called:
+
+*  `hash_func`
+*  `backend`
+*  `mongetter`
+*  `cache_dir`
+*  `pickle_reload`
+*  `separate_files`
+
+These parameters can be changed at any time and they will apply to all decorators:
+
+*  `caching_enabled`
+*  `stale_after`
+*  `next_time`
+*  `wait_for_calc_timeout`
+
+The current defaults can be fetched by calling `get_default_params`.
+
 Threads Limit
 ~~~~~~~~~~~~~
 
 To limit the number of threads Cachier is allowed to spawn, set the ``CACHIER_MAX_WORKERS`` with the desired number. The defeault is 8, so to enable Cachier to spawn even more threads, you'll have to set a higher limit explicitly.
 
 
+Global Enable/Disable
+---------------------
+
+Caching can be turned off across all decorators by calling `disable_caching`, and then re-activated by calling `enable_caching`.
+
+These functions are convenience wrappers around the `caching_enabled` default setting.
+
+
 Cache Shelf Life
 ----------------
 
 Setting Shelf Life
 ~~~~~~~~~~~~~~~~~~
 You can set any duration as the shelf life of cached return values of a function by providing a corresponding ``timedelta`` object to the ``stale_after`` parameter:
 
@@ -306,15 +337,15 @@
 
 Note, however, that ``cachier``'s in-memory core is simple, and has no monitoring or cap on cache size, and can thus lead to memory errors on large return values - it is mainly intended to be used with future multi-core functionality. As a rule, Python's built-in ``lru_cache`` is a much better stand-alone solution.
 
 
 Contributing
 ============
 
-Package author and current maintainer is Shay Palachy (shay.palachy@gmail.com); You are more than welcome to approach him for help. Contributions are very welcomed.
+Current maintainers are Shay Palachy Affek (`shay.palachy@gmail.com <mailto:shay.palachy@gmail.com>`_, `@shaypal5 <https://github.com/shaypal5>`_) and Judson Neer (`@lordjabez <https://github.com/lordjabez>`_); You are more than welcome to approach them for help. Contributions are very welcomed! :)
 
 Installing for development
 --------------------------
 
 Clone:
 
 .. code-block:: bash
@@ -375,35 +406,39 @@
 
 Additionally, if you update this ``README.rst`` file, use ``python setup.py checkdocs`` to validate it compiles.
 
 
 Credits
 =======
 
-Created by `Shay Palachy <https://github.com/shaypal5>`_ (shay.palachy@gmail.com).
+Created by `Shay Palachy Affek <https://github.com/shaypal5>`_ (shay.palachy@gmail.com).
+
+Current lead developer/contributor: `Judson Neer <https://github.com/lordjabez>`_ (`@lordjabez <https://github.com/lordjabez>`_ on GitHub).
 
 Other major contributors:
 
-  * `cthoyt <https://github.com/cthoyt>`_ - Base memory core implementation.
+* `Judson Neer <https://github.com/lordjabez>`_ - Precaching, method caching support and numerous improvements and bugfixes.
+
+* `cthoyt <https://github.com/cthoyt>`_ - Base memory core implementation.
 
-  * `amarczew <https://github.com/amarczew>`_ - The ``hash_func`` kwarg.
+* `amarczew <https://github.com/amarczew>`_ - The ``hash_func`` kwarg.
 
-  * `non-senses <https://github.com/non-senses>`_ - The ``wait_for_calc_timeout`` kwarg.
+* `non-senses <https://github.com/non-senses>`_ - The ``wait_for_calc_timeout`` kwarg.
 
-  * `Elad Rapapor <https://github.com/erap129>`_ - Multi-file Pickle core, a.k.a ``separate_files`` (released on ``v1.5.3``).
+* `Elad Rapapor <https://github.com/erap129>`_ - Multi-file Pickle core, a.k.a ``separate_files`` (released on ``v1.5.3``).
 
-  * `John Didion <https://github.com/jdidion>`_ - Support for pickle-based caching for cases where two identically-named methods of different classes are defined in the same module.
+* `John Didion <https://github.com/jdidion>`_ - Support for pickle-based caching for cases where two identically-named methods of different classes are defined in the same module.
 
 Notable bugfixers:
 
-  * `MichaelRazum <https://github.com/MichaelRazum>`_.
+* `MichaelRazum <https://github.com/MichaelRazum>`_.
 
-  * `Eric Ma <https://github.com/ericmjl>`_ - The iNotify bugfix (released on ``v1.5.3``).
+* `Eric Ma <https://github.com/ericmjl>`_ - The iNotify bugfix (released on ``v1.5.3``).
 
-  * `Ofir <https://github.com/ofirnk>`_ - The iNotify bugfix (released on ``v1.5.3``).
+* `Ofir <https://github.com/ofirnk>`_ - The iNotify bugfix (released on ``v1.5.3``).
 
 
 
 .. |PyPI-Status| image:: https://img.shields.io/pypi/v/cachier.svg
   :target: https://pypi.python.org/pypi/cachier
 
 .. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/cachier.svg
```

### Comparing `cachier-2.1.0/cachier/base_core.py` & `cachier-2.1.1/cachier/base_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,55 +3,63 @@
 # https://github.com/python-cachier/cachier
 
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/MIT-license
 # Copyright (c) 2016, Shay Palachy <shaypal5@gmail.com>
 
 import abc  # for the _BaseCore abstract base class
-import functools
-import hashlib
 import inspect
-import pickle  # nosec: B403
 
 
-def _default_hash_func(args, kwds):
-    # pylint: disable-next=protected-access
-    key = functools._make_key(args, kwds, typed=True)
-    hash = hashlib.sha256()
-    for item in key:
-        hash.update(pickle.dumps(item))
-    return hash.hexdigest()
+class RecalculationNeeded(Exception):
+    pass
 
 
 class _BaseCore():
     __metaclass__ = abc.ABCMeta
 
-    def __init__(self, hash_func):
-        self.hash_func = hash_func if hash_func else _default_hash_func
-        self.func = None
+    def __init__(self, hash_func, default_params):
+        self.default_params = default_params
+        self.hash_func = hash_func
 
     def set_func(self, func):
         """Sets the function this core will use. This has to be set before any
         method is called. Also determine if the funtion is an object method."""
         func_params = list(inspect.signature(func).parameters)
         self.func_is_method = func_params and func_params[0] == 'self'
         self.func = func
 
+    def get_key(self, args, kwds):
+        """Returns a unique key based on the arguments provided."""
+        if self.hash_func is not None:
+            return self.hash_func(args, kwds)
+        else:
+            return self.default_params['hash_func'](args, kwds)
+
     def get_entry(self, args, kwds):
         """Returns the result mapped to the given arguments in this core's
         cache, if such a mapping exists."""
-        key = self.hash_func(args, kwds)
+        key = self.get_key(args, kwds)
         return self.get_entry_by_key(key)
 
     def precache_value(self, args, kwds, value_to_cache):
         """Writes a precomputed value into the cache."""
-        key = self.hash_func(args, kwds)
+        key = self.get_key(args, kwds)
         self.set_entry(key, value_to_cache)
         return value_to_cache
 
+    def check_calc_timeout(self, time_spent):
+        """Raise an exception if a recalulation is needed."""
+        if self.wait_for_calc_timeout is not None:
+            calc_timeout = self.wait_for_calc_timeout
+        else:
+            calc_timeout = self.default_params['wait_for_calc_timeout']
+        if calc_timeout > 0 and (time_spent >= calc_timeout):
+            raise RecalculationNeeded()
+
     @abc.abstractmethod
     def get_entry_by_key(self, key):
         """Returns the result mapped to the given key in this core's cache,
         if such a mapping exists."""
 
     @abc.abstractmethod
     def set_entry(self, key, func_res):
```

### Comparing `cachier-2.1.0/cachier/core.py` & `cachier-2.1.1/cachier/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,18 +13,22 @@
 from __future__ import print_function
 
 import os
 from functools import wraps
 from warnings import warn
 
 import datetime
+import functools
+import hashlib
+import pickle
 from concurrent.futures import ThreadPoolExecutor
 
+from .base_core import RecalculationNeeded
 from .pickle_core import _PickleCore
-from .mongo_core import _MongoCore, RecalculationNeeded
+from .mongo_core import _MongoCore
 from .memory_core import _MemoryCore
 
 
 MAX_WORKERS_ENVAR_NAME = 'CACHIER_MAX_WORKERS'
 DEFAULT_MAX_WORKERS = 8
 
 
@@ -71,112 +75,142 @@
         core.set_entry(key, func_res)
         # _get_executor().submit(core.set_entry, key, func_res)
         return func_res
     finally:
         core.mark_entry_not_calculated(key)
 
 
+def _default_hash_func(args, kwds):
+    # pylint: disable-next=protected-access
+    key = functools._make_key(args, kwds, typed=True)
+    hash = hashlib.sha256()
+    for item in key:
+        hash.update(pickle.dumps(item))
+    return hash.hexdigest()
+
+
 class MissingMongetter(ValueError):
     """Thrown when the mongetter keyword argument is missing."""
 
 
+_default_params = {
+    'caching_enabled': True,
+    'hash_func': _default_hash_func,
+    'backend': 'pickle',
+    'mongetter': None,
+    'stale_after': datetime.timedelta.max,
+    'next_time': False,
+    'cache_dir': '~/.cachier/',
+    'pickle_reload': True,
+    'separate_files': False,
+    'wait_for_calc_timeout': 0,
+}
+
+
 def cachier(
-    stale_after=None,
-    next_time=False,
-    pickle_reload=True,
+    hash_func=None,
+    hash_params=None,
     backend=None,
     mongetter=None,
+    stale_after=None,
+    next_time=None,
     cache_dir=None,
-    hash_func=None,
-    hash_params=None,
-    wait_for_calc_timeout=0,
-    separate_files=False,
+    pickle_reload=None,
+    separate_files=None,
+    wait_for_calc_timeout=None,
 ):
     """A persistent, stale-free memoization decorator.
 
     The positional and keyword arguments to the wrapped function must be
     hashable (i.e. Python's immutable built-in objects, not mutable
     containers). Also, notice that since objects which are instances of
     user-defined classes are hashable but all compare unequal (their hash
     value is their id), equal objects across different sessions will not yield
     identical keys.
 
     Arguments
     ---------
+    hash_func : callable, optional
+        A callable that gets the args and kwargs from the decorated function
+        and returns a hash key for them. This parameter can be used to enable
+        the use of cachier with functions that get arguments that are not
+        automatically hashable by Python.
+    backend : str, optional
+        The name of the backend to use. Valid options currently include
+        'pickle', 'mongo' and 'memory'. If not provided, defaults to
+        'pickle' unless the 'mongetter' argument is passed, in which
+        case the mongo backend is automatically selected.
+    mongetter : callable, optional
+        A callable that takes no arguments and returns a pymongo.Collection
+        object with writing permissions. If unset a local pickle cache is used
+        instead.
     stale_after : datetime.timedelta, optional
         The time delta afterwhich a cached result is considered stale. Calls
         made after the result goes stale will trigger a recalculation of the
         result, but whether a stale or fresh result will be returned is
         determined by the optional next_time argument.
     next_time : bool, optional
         If set to True, a stale result will be returned when finding one, not
         waiting for the calculation of the fresh result to return. Defaults to
         False.
-    pickle_reload : bool, optional
-        If set to True, in-memory cache will be reloaded on each cache read,
-        enabling different threads to share cache. Should be set to False for
-        faster reads in single-thread programs. Defaults to True.
-    mongetter : callable, optional
-        A callable that takes no arguments and returns a pymongo.Collection
-        object with writing permissions. If unset a local pickle cache is used
-        instead.
-    backend : str, optional
-        The name of the backend to use. If None, defaults to 'mongo' when
-        the ``mongetter`` argument is passed, otherwise defaults to 'pickle'.
-        Valid options currently include 'pickle', 'mongo' and 'memory'.
     cache_dir : str, optional
         A fully qualified path to a file directory to be used for cache files.
         The running process must have running permissions to this folder. If
         not provided, a default directory at `~/.cachier/` is used.
-    hash_func : callable, optional
-        A callable that gets the args and kwargs from the decorated function
-        and returns a hash key for them. This parameter can be used to enable
-        the use of cachier with functions that get arguments that are not
-        automatically hashable by Python.
+    pickle_reload : bool, optional
+        If set to True, in-memory cache will be reloaded on each cache read,
+        enabling different threads to share cache. Should be set to False for
+        faster reads in single-thread programs. Defaults to True.
+    separate_files: bool, default False, for Pickle cores only
+        Instead of a single cache file per-function, each function's cache is
+        split between several files, one for each argument set. This can help
+        if you per-function cache files become too large.
     wait_for_calc_timeout: int, optional, for MongoDB only
         The maximum time to wait for an ongoing calculation. When a
         process started to calculate the value setting being_calculated to
         True, any process trying to read the same entry will wait a maximum of
         seconds specified in this parameter. 0 means wait forever.
         Once the timeout expires the calculation will be triggered.
-    separate_files: bool, default False, for Pickle cores only
-        Instead of a single cache file per-function, each function's cache is
-        split between several files, one for each argument set. This can help
-        if you per-function cache files become too large.
     """
     # Check for deprecated parameters
     if hash_params is not None:
         message = 'hash_params will be removed in a future release, ' \
                   'please use hash_func instead'
         warn(message, DeprecationWarning, stacklevel=2)
         hash_func = hash_params
-    # The default is calculated dynamically to maintain previous behavior
-    # to default to pickle unless the ``mongetter`` argument is given.
+    # Override the backend parameter if a mongetter is provided.
+    if mongetter is None:
+        mongetter = _default_params['mongetter']
+    if callable(mongetter):
+        backend = 'mongo'
     if backend is None:
-        backend = 'pickle' if mongetter is None else 'mongo'
+        backend = _default_params['backend']
     if backend == 'pickle':
         core = _PickleCore(  # pylint: disable=R0204
             hash_func=hash_func,
-            reload=pickle_reload,
+            pickle_reload=pickle_reload,
             cache_dir=cache_dir,
             separate_files=separate_files,
             wait_for_calc_timeout=wait_for_calc_timeout,
+            default_params=_default_params,
         )
     elif backend == 'mongo':
         if mongetter is None:
             raise MissingMongetter(
                 'must specify ``mongetter`` when using the mongo core')
         core = _MongoCore(
             mongetter=mongetter,
             hash_func=hash_func,
             wait_for_calc_timeout=wait_for_calc_timeout,
+            default_params=_default_params,
         )
     elif backend == 'memory':
         core = _MemoryCore(
             hash_func=hash_func,
+            default_params=_default_params,
         )
     elif backend == 'redis':
         raise NotImplementedError(
             'A Redis backend has not yet been implemented. '
             'Please see https://github.com/python-cachier/cachier/issues/4'
         )
     else:
@@ -190,58 +224,59 @@
             # print('Inside general wrapper for {}.'.format(func.__name__))
             ignore_cache = kwds.pop('ignore_cache', False)
             overwrite_cache = kwds.pop('overwrite_cache', False)
             verbose_cache = kwds.pop('verbose_cache', False)
             _print = lambda x: None  # skipcq: FLK-E731  # noqa: E731
             if verbose_cache:
                 _print = print
-            if ignore_cache:
+            if ignore_cache or not _default_params['caching_enabled']:
                 return func(*args, **kwds)
             if core.func_is_method:
                 key, entry = core.get_entry(args[1:], kwds)
             else:
                 key, entry = core.get_entry(args, kwds)
             if overwrite_cache:
                 return _calc_entry(core, key, func, args, kwds)
             if entry is not None:  # pylint: disable=R0101
                 _print('Entry found.')
                 if entry.get('value', None) is not None:
                     _print('Cached result found.')
-                    if stale_after:
-                        now = datetime.datetime.now()
-                        if now - entry['time'] > stale_after:
-                            _print('But it is stale... :(')
-                            if entry['being_calculated']:
-                                if next_time:
-                                    _print('Returning stale.')
-                                    return entry['value']  # return stale val
-                                _print('Already calc. Waiting on change.')
-                                try:
-                                    return core.wait_on_entry_calc(key)
-                                except RecalculationNeeded:
-                                    return _calc_entry(
-                                        core, key, func, args, kwds
-                                    )
-                            if next_time:
-                                _print('Async calc and return stale')
-                                try:
-                                    core.mark_entry_being_calculated(key)
-                                    _get_executor().submit(
-                                        _function_thread,
-                                        core,
-                                        key,
-                                        func,
-                                        args,
-                                        kwds,
-                                    )
-                                finally:
-                                    core.mark_entry_not_calculated(key)
-                                return entry['value']
-                            _print('Calling decorated function and waiting')
-                            return _calc_entry(core, key, func, args, kwds)
+                    local_stale_after = stale_after if stale_after is not None else _default_params['stale_after']  # noqa: E501
+                    local_next_time = next_time if next_time is not None else _default_params['next_time']  # noqa: E501
+                    now = datetime.datetime.now()
+                    if now - entry['time'] > local_stale_after:
+                        _print('But it is stale... :(')
+                        if entry['being_calculated']:
+                            if local_next_time:
+                                _print('Returning stale.')
+                                return entry['value']  # return stale val
+                            _print('Already calc. Waiting on change.')
+                            try:
+                                return core.wait_on_entry_calc(key)
+                            except RecalculationNeeded:
+                                return _calc_entry(
+                                    core, key, func, args, kwds
+                                )
+                        if local_next_time:
+                            _print('Async calc and return stale')
+                            try:
+                                core.mark_entry_being_calculated(key)
+                                _get_executor().submit(
+                                    _function_thread,
+                                    core,
+                                    key,
+                                    func,
+                                    args,
+                                    kwds,
+                                )
+                            finally:
+                                core.mark_entry_not_calculated(key)
+                            return entry['value']
+                        _print('Calling decorated function and waiting')
+                        return _calc_entry(core, key, func, args, kwds)
                     _print('And it is fresh!')
                     return entry['value']
                 if entry['being_calculated']:
                     _print('No value but being calculated. Waiting.')
                     try:
                         return core.wait_on_entry_calc(key)
                     except RecalculationNeeded:
@@ -256,15 +291,15 @@
         def clear_being_calculated():
             """Marks all entries in this cache as not being calculated."""
             core.clear_being_calculated()
 
         def cache_dpath():
             """Returns the path to the cache dir, if exists; None if not."""
             try:
-                return core.expended_cache_dir
+                return core.cache_dir
             except AttributeError:
                 return None
 
         def precache_value(*args, value_to_cache, **kwds):
             """Add an initial value to the cache.
 
             Arguments
@@ -277,7 +312,38 @@
         func_wrapper.clear_cache = clear_cache
         func_wrapper.clear_being_calculated = clear_being_calculated
         func_wrapper.cache_dpath = cache_dpath
         func_wrapper.precache_value = precache_value
         return func_wrapper
 
     return _cachier_decorator
+
+
+def set_default_params(**params):
+    """Configure global parameters applicable to all memoized functions.
+
+    This function takes the same keyword parameters as the ones defined
+    in the decorator, which can be passed all at once or with multiple
+    calls. Parameters given directly to a decorator take precedence over
+    any values set by this function.
+
+    Only 'stale_after', 'next_time', and 'wait_for_calc_timeout' can be
+    changed after the memoization decorator has been applied. Other parameters
+    will only have an effect on decorators applied after this function is run.
+    """
+    valid_params = (p for p in params.items() if p[0] in _default_params)
+    _default_params.update(valid_params)
+
+
+def get_default_params():
+    """Get current set of default parameters."""
+    return _default_params
+
+
+def enable_caching():
+    """Enable caching globally."""
+    _default_params['caching_enabled'] = True
+
+
+def disable_caching():
+    """Disable caching globally."""
+    _default_params['caching_enabled'] = False
```

### Comparing `cachier-2.1.0/cachier/memory_core.py` & `cachier-2.1.1/cachier/memory_core.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,26 +3,18 @@
 import threading
 from datetime import datetime
 
 from .base_core import _BaseCore
 
 
 class _MemoryCore(_BaseCore):
-    """The pickle core class for cachier.
+    """The memory core class for cachier."""
 
-    Parameters
-    ----------
-    stale_after : datetime.timedelta, optional
-        See :class:`_BaseCore` documentation.
-    next_time : bool, optional
-        See :class:`_BaseCore` documentation.
-    """
-
-    def __init__(self, hash_func):
-        super().__init__(hash_func)
+    def __init__(self, hash_func, default_params):
+        super().__init__(hash_func, default_params)
         self.cache = {}
         self.lock = threading.RLock()
 
     def get_entry_by_key(self, key, reload=False):  # pylint: disable=W0221
         with self.lock:
             return key, self.cache.get(key, None)
 
@@ -70,18 +62,18 @@
             if cond:
                 cond.acquire()
                 cond.notify_all()
                 cond.release()
                 entry['condition'] = None
 
     def wait_on_entry_calc(self, key):
-        with self.lock:
+        with self.lock:  # pragma: no cover
             entry = self.cache[key]
             if not entry['being_calculated']:
-                return entry['value']  # pragma: no cover
+                return entry['value']
         entry['condition'].acquire()
         entry['condition'].wait()
         entry['condition'].release()
         return self.cache[key]['value']
 
     def clear_cache(self):
         with self.lock:
```

### Comparing `cachier-2.1.0/cachier/mongo_core.py` & `cachier-2.1.1/cachier/mongo_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,43 +10,37 @@
 import sys  # to make sure that pymongo was imported
 import pickle  # for serialization of python objects
 from datetime import datetime
 import time   # to sleep when waiting on Mongo cache\
 import warnings  # to warn if pymongo is missing
 
 try:
-    from pymongo import (
-        IndexModel,
-        ASCENDING
-    )
+    from pymongo import (IndexModel, ASCENDING)
     from pymongo.errors import OperationFailure
     from bson.binary import Binary  # to save binary data to mongodb
 except ImportError:  # pragma: no cover
     pass
 
-from .base_core import _BaseCore
+from .base_core import _BaseCore, RecalculationNeeded
 
 
 MONGO_SLEEP_DURATION_IN_SEC = 1
 
 
-class RecalculationNeeded(Exception):
-    pass
-
-
 class _MongoCore(_BaseCore):
 
     _INDEX_NAME = 'func_1_key_1'
 
-    def __init__(self, mongetter, hash_func, wait_for_calc_timeout):
+    def __init__(self, mongetter, hash_func,
+                 wait_for_calc_timeout, default_params):
         if 'pymongo' not in sys.modules:
             warnings.warn((
                 "Cachier warning: pymongo was not found. "
-                "MongoDB cores will not function."))
-        super().__init__(hash_func)
+                "MongoDB cores will not function."))  # pragma: no cover
+        super().__init__(hash_func, default_params)
         self.mongetter = mongetter
         self.mongo_collection = self.mongetter()
         self.wait_for_calc_timeout = wait_for_calc_timeout
         index_inf = self.mongo_collection.index_information()
         if _MongoCore._INDEX_NAME not in index_inf:
             func1key1 = IndexModel(
                 keys=[('func', ASCENDING), ('key', ASCENDING)],
@@ -133,17 +127,15 @@
             time.sleep(MONGO_SLEEP_DURATION_IN_SEC)
             time_spent += MONGO_SLEEP_DURATION_IN_SEC
             key, entry = self.get_entry_by_key(key)
             if entry is None:
                 raise RecalculationNeeded()
             if not entry['being_calculated']:
                 return entry['value']
-            if self.wait_for_calc_timeout > 0 and (
-                    time_spent >= self.wait_for_calc_timeout):
-                raise RecalculationNeeded()
+            self.check_calc_timeout(time_spent)
 
     def clear_cache(self):
         self.mongo_collection.delete_many(
             filter={'func': _MongoCore._get_func_str(self.func)}
         )
 
     def clear_being_calculated(self):
```

### Comparing `cachier-2.1.0/cachier/pickle_core.py` & `cachier-2.1.1/cachier/pickle_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,26 @@
 
 # This file is part of Cachier.
 # https://github.com/python-cachier/cachier
 
 # Licensed under the MIT license:
 # http://www.opensource.org/licenses/MIT-license
 # Copyright (c) 2016, Shay Palachy <shaypal5@gmail.com>
-import hashlib
 import os
 import pickle  # for local caching
 from datetime import datetime
 import threading
 
 import portalocker  # to lock on pickle cache IO
 from watchdog.observers import Observer
 from watchdog.events import PatternMatchingEventHandler
 
 # Altenative:  https://github.com/WoLpH/portalocker
 
 from .base_core import _BaseCore
-from .mongo_core import RecalculationNeeded
-
-DEF_CACHIER_DIR = '~/.cachier/'
 
 
 class _PickleCore(_BaseCore):
     """The pickle core class for cachier.
 
     Parameters
     ----------
@@ -75,47 +71,51 @@
             """A Watchdog Event Handler method."""
             self._check_calculation()  # pragma: no cover
 
         def on_modified(self, event):  # skipcq: PYL-W0613
             """A Watchdog Event Handler method."""
             self._check_calculation()
 
-    def __init__(
-            self, hash_func, reload, cache_dir,
-            separate_files, wait_for_calc_timeout,
-    ):
-        super().__init__(hash_func)
+    def __init__(self, hash_func, pickle_reload, cache_dir,
+                 separate_files, wait_for_calc_timeout, default_params):
+        super().__init__(hash_func, default_params)
         self.cache = None
-        self.reload = reload
-        self.cache_dir = DEF_CACHIER_DIR
+        if pickle_reload is not None:
+            self.reload = pickle_reload
+        else:
+            self.reload = self.default_params['pickle_reload']
         if cache_dir is not None:
-            self.cache_dir = cache_dir
-        self.expended_cache_dir = os.path.expanduser(self.cache_dir)
-        self.lock = threading.RLock()
+            self.cache_dir = os.path.expanduser(cache_dir)
+        else:
+            self.cache_dir = os.path.expanduser(self.default_params['cache_dir'])  # noqa: E501
+        if separate_files is not None:
+            self.separate_files = separate_files
+        else:
+            self.separate_files = self.default_params['separate_files']
+        self.wait_for_calc_timeout = wait_for_calc_timeout
         self.cache_fname = None
         self.cache_fpath = None
-        self.separate_files = separate_files
-        self.wait_for_calc_timeout = wait_for_calc_timeout
+        self.lock = threading.RLock()
 
     def _cache_fname(self):
         if self.cache_fname is None:
             self.cache_fname = '.{}.{}'.format(
                 self.func.__module__, self.func.__qualname__
             )
             self.cache_fname = self.cache_fname.replace('<', '_').replace(
                 '>', '_')
         return self.cache_fname
 
     def _cache_fpath(self):
         if self.cache_fpath is None:
-            if not os.path.exists(self.expended_cache_dir):
-                os.makedirs(self.expended_cache_dir)
+            if not os.path.exists(self.cache_dir):
+                os.makedirs(self.cache_dir)
             self.cache_fpath = os.path.abspath(
                 os.path.join(
-                    os.path.realpath(self.expended_cache_dir),
+                    os.path.realpath(self.cache_dir),
                     self._cache_fname(),
                 )
             )
         return self.cache_fpath
 
     def _reload_cache(self):
         with self.lock:
@@ -134,22 +134,22 @@
             if not self.cache:
                 self._reload_cache()
             return self.cache
 
     def _get_cache_by_key(self, key=None, hash=None):
         fpath = self._cache_fpath()
         if hash is None:
-            fpath += f'_{hashlib.sha256(pickle.dumps(key)).hexdigest()}'
+            fpath += f'_{key}'
         else:
             fpath += f'_{hash}'
         try:
             with portalocker.Lock(fpath, mode='rb') as cache_file:
                 try:
                     res = pickle.load(cache_file)
-                except EOFError:
+                except EOFError:  # pragma: no cover
                     res = None
         except FileNotFoundError:
             res = None
         return res
 
     def _clear_all_cache_files(self):
         fpath = self._cache_fpath()
@@ -169,15 +169,15 @@
                     self._save_cache(entry, hash=subpath.split('_')[-1])
 
     def _save_cache(self, cache, key=None, hash=None):
         with self.lock:
             self.cache = cache
             fpath = self._cache_fpath()
             if key is not None:
-                fpath += f'_{hashlib.sha256(pickle.dumps(key)).hexdigest()}'
+                fpath += f'_{key}'
             elif hash is not None:
                 fpath += f'_{hash}'
             with portalocker.Lock(fpath, mode='wb') as cache_file:
                 pickle.dump(cache, cache_file, protocol=4)
             if key is None:
                 self._reload_cache()
 
@@ -244,39 +244,36 @@
                 self._save_cache(cache)
             except KeyError:
                 pass  # that's ok, we don't need an entry in that case
 
     def wait_on_entry_calc(self, key):
         if self.separate_files:
             entry = self._get_cache_by_key(key)
-            hexdg = hashlib.sha256(pickle.dumps(key)).hexdigest()
-            filename = f'{self._cache_fname()}_{hexdg}'
+            filename = f'{self._cache_fname()}_{key}'
         else:
             with self.lock:
                 self._reload_cache()
                 entry = self._get_cache()[key]
             filename = self._cache_fname()
         if not entry['being_calculated']:
             return entry['value']
         event_handler = _PickleCore.CacheChangeHandler(
             filename=filename, core=self, key=key
         )
         observer = Observer()
         event_handler.inject_observer(observer)
         observer.schedule(
-            event_handler, path=self.expended_cache_dir, recursive=True
+            event_handler, path=self.cache_dir, recursive=True
         )
         observer.start()
         time_spent = 0
         while observer.is_alive():
             observer.join(timeout=1.0)
             time_spent += 1
-            if 0 < self.wait_for_calc_timeout < time_spent:
-                raise RecalculationNeeded()
-        # print("Returned value: {}".format(event_handler.value))
+            self.check_calc_timeout(time_spent)
         return event_handler.value
 
     def clear_cache(self):
         if self.separate_files:
             self._clear_all_cache_files()
         else:
             self._save_cache({})
```

### Comparing `cachier-2.1.0/cachier.egg-info/PKG-INFO` & `cachier-2.1.1/cachier.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachier
-Version: 2.1.0
+Version: 2.1.1
 Summary: Persistent, stale-free, local and cross-machine caching for Python functions.
 Home-page: https://github.com/python-cachier/cachier
 Author: Shay Palachy
 Author-email: shay.palachy@gmail.com
 License: MIT
 Keywords: cache,persistence,mongo,memoization,decorator
 Platform: linux
@@ -147,20 +147,51 @@
 .. code-block:: python
 
   foo.clear_cache()
 
 General Configuration
 ----------------------
 
+Global Defaults
+~~~~~~~~~~~~~~~
+
+Settings can be globally configured across all Cachier wrappers through the use of the `set_default_params` function. This function takes the same keyword parameters as the ones defined in the decorator, which can be passed all at once or with multiple calls. Parameters given directly to a decorator take precedence over any values set by this function.
+
+The following parameters will only be applied to decorators defined after `set_default_params` is called:
+
+*  `hash_func`
+*  `backend`
+*  `mongetter`
+*  `cache_dir`
+*  `pickle_reload`
+*  `separate_files`
+
+These parameters can be changed at any time and they will apply to all decorators:
+
+*  `caching_enabled`
+*  `stale_after`
+*  `next_time`
+*  `wait_for_calc_timeout`
+
+The current defaults can be fetched by calling `get_default_params`.
+
 Threads Limit
 ~~~~~~~~~~~~~
 
 To limit the number of threads Cachier is allowed to spawn, set the ``CACHIER_MAX_WORKERS`` with the desired number. The defeault is 8, so to enable Cachier to spawn even more threads, you'll have to set a higher limit explicitly.
 
 
+Global Enable/Disable
+---------------------
+
+Caching can be turned off across all decorators by calling `disable_caching`, and then re-activated by calling `enable_caching`.
+
+These functions are convenience wrappers around the `caching_enabled` default setting.
+
+
 Cache Shelf Life
 ----------------
 
 Setting Shelf Life
 ~~~~~~~~~~~~~~~~~~
 You can set any duration as the shelf life of cached return values of a function by providing a corresponding ``timedelta`` object to the ``stale_after`` parameter:
 
@@ -334,15 +365,15 @@
 
 Note, however, that ``cachier``'s in-memory core is simple, and has no monitoring or cap on cache size, and can thus lead to memory errors on large return values - it is mainly intended to be used with future multi-core functionality. As a rule, Python's built-in ``lru_cache`` is a much better stand-alone solution.
 
 
 Contributing
 ============
 
-Package author and current maintainer is Shay Palachy (shay.palachy@gmail.com); You are more than welcome to approach him for help. Contributions are very welcomed.
+Current maintainers are Shay Palachy Affek (`shay.palachy@gmail.com <mailto:shay.palachy@gmail.com>`_, `@shaypal5 <https://github.com/shaypal5>`_) and Judson Neer (`@lordjabez <https://github.com/lordjabez>`_); You are more than welcome to approach them for help. Contributions are very welcomed! :)
 
 Installing for development
 --------------------------
 
 Clone:
 
 .. code-block:: bash
@@ -403,35 +434,39 @@
 
 Additionally, if you update this ``README.rst`` file, use ``python setup.py checkdocs`` to validate it compiles.
 
 
 Credits
 =======
 
-Created by `Shay Palachy <https://github.com/shaypal5>`_ (shay.palachy@gmail.com).
+Created by `Shay Palachy Affek <https://github.com/shaypal5>`_ (shay.palachy@gmail.com).
+
+Current lead developer/contributor: `Judson Neer <https://github.com/lordjabez>`_ (`@lordjabez <https://github.com/lordjabez>`_ on GitHub).
 
 Other major contributors:
 
-  * `cthoyt <https://github.com/cthoyt>`_ - Base memory core implementation.
+* `Judson Neer <https://github.com/lordjabez>`_ - Precaching, method caching support and numerous improvements and bugfixes.
+
+* `cthoyt <https://github.com/cthoyt>`_ - Base memory core implementation.
 
-  * `amarczew <https://github.com/amarczew>`_ - The ``hash_func`` kwarg.
+* `amarczew <https://github.com/amarczew>`_ - The ``hash_func`` kwarg.
 
-  * `non-senses <https://github.com/non-senses>`_ - The ``wait_for_calc_timeout`` kwarg.
+* `non-senses <https://github.com/non-senses>`_ - The ``wait_for_calc_timeout`` kwarg.
 
-  * `Elad Rapapor <https://github.com/erap129>`_ - Multi-file Pickle core, a.k.a ``separate_files`` (released on ``v1.5.3``).
+* `Elad Rapapor <https://github.com/erap129>`_ - Multi-file Pickle core, a.k.a ``separate_files`` (released on ``v1.5.3``).
 
-  * `John Didion <https://github.com/jdidion>`_ - Support for pickle-based caching for cases where two identically-named methods of different classes are defined in the same module.
+* `John Didion <https://github.com/jdidion>`_ - Support for pickle-based caching for cases where two identically-named methods of different classes are defined in the same module.
 
 Notable bugfixers:
 
-  * `MichaelRazum <https://github.com/MichaelRazum>`_.
+* `MichaelRazum <https://github.com/MichaelRazum>`_.
 
-  * `Eric Ma <https://github.com/ericmjl>`_ - The iNotify bugfix (released on ``v1.5.3``).
+* `Eric Ma <https://github.com/ericmjl>`_ - The iNotify bugfix (released on ``v1.5.3``).
 
-  * `Ofir <https://github.com/ofirnk>`_ - The iNotify bugfix (released on ``v1.5.3``).
+* `Ofir <https://github.com/ofirnk>`_ - The iNotify bugfix (released on ``v1.5.3``).
 
 
 
 .. |PyPI-Status| image:: https://img.shields.io/pypi/v/cachier.svg
   :target: https://pypi.python.org/pypi/cachier
 
 .. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/cachier.svg
```

### Comparing `cachier-2.1.0/cachier.egg-info/SOURCES.txt` & `cachier-2.1.1/cachier.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -32,13 +32,14 @@
 cachier.egg-info/top_level.txt
 cachier/scripts/__init__.py
 cachier/scripts/cli.py
 tests/__init__.py
 tests/speed_eval.py
 tests/standalone_script.py
 tests/test_core_lookup.py
+tests/test_defaults.py
 tests/test_general.py
 tests/test_memory_core.py
 tests/test_mongo_core.py
 tests/test_pickle_core.py
 tests/test_quality.py
 tests/test_security.py
```

### Comparing `cachier-2.1.0/setup.py` & `cachier-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `cachier-2.1.0/tests/speed_eval.py` & `cachier-2.1.1/tests/speed_eval.py`

 * *Files identical despite different names*

### Comparing `cachier-2.1.0/tests/test_general.py` & `cachier-2.1.1/tests/test_general.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 import os
 import queue
 import subprocess  # nosec: B404
 import threading
 from random import random
 from time import sleep, time
 import pytest
-import cachier as cachier_dir
-from cachier import cachier
+import cachier
 from cachier.core import (
     MAX_WORKERS_ENVAR_NAME,
     DEFAULT_MAX_WORKERS,
     _max_workers,
     _set_max_workers,
     _get_executor
 )
@@ -22,15 +21,15 @@
     _test_mongetter,
     MONGO_DELTA_LONG,
 )
 
 
 def test_information():
     print("\ncachier version: ", end="")
-    print(cachier_dir.__version__)
+    print(cachier.__version__)
 
 
 def test_max_workers():
     """Just call this function for coverage."""
     try:
         del os.environ[MAX_WORKERS_ENVAR_NAME]
     except KeyError:
@@ -57,15 +56,15 @@
     (None, None, False),
     (None, None, True),
 ]
 
 
 @pytest.mark.parametrize(parametrize_keys, parametrize_values)
 def test_wait_for_calc_timeout_ok(mongetter, stale_after, separate_files):
-    @cachier(
+    @cachier.cachier(
         mongetter=mongetter,
         stale_after=stale_after,
         separate_files=separate_files,
         next_time=False,
         wait_for_calc_timeout=2
     )
     def _wait_for_calc_timeout_fast(arg_1, arg_2):
@@ -102,15 +101,15 @@
     res1 = res_queue.get()
     res2 = res_queue.get()
     assert res1 == res2  # Timeout did not kick in, a single call was done
 
 
 @pytest.mark.parametrize(parametrize_keys, parametrize_values)
 def test_wait_for_calc_timeout_slow(mongetter, stale_after, separate_files):
-    @cachier(
+    @cachier.cachier(
         mongetter=mongetter,
         stale_after=stale_after,
         separate_files=separate_files,
         next_time=False,
         wait_for_calc_timeout=2,
     )
     def _wait_for_calc_timeout_slow(arg_1, arg_2):
@@ -155,15 +154,15 @@
         (_test_mongetter, 'mongo'),
         (None, 'memory'),
         (None, 'pickle'),
     ]
 )
 def test_precache_value(mongetter, backend):
 
-    @cachier(backend=backend, mongetter=mongetter)
+    @cachier.cachier(backend=backend, mongetter=mongetter)
     def func(arg_1, arg_2):
         """Some function."""
         return arg_1 + arg_2
 
     result = func.precache_value(2, 2, value_to_cache=5)
     assert result == 5
     result = func(2, 2)
@@ -184,15 +183,15 @@
         (None, 'memory'),
         (None, 'pickle'),
     ]
 )
 def test_ignore_self_in_methods(mongetter, backend):
 
     class TestClass():
-        @cachier(backend=backend, mongetter=mongetter)
+        @cachier.cachier(backend=backend, mongetter=mongetter)
         def takes_2_seconds(self, arg_1, arg_2):
             """Some function."""
             sleep(2)
             return arg_1 + arg_2
 
     test_object_1 = TestClass()
     test_object_2 = TestClass()
@@ -205,15 +204,15 @@
     end = time()
     assert result_2 == 3
     assert end - start < 1
 
 
 def test_hash_params_deprecation():
     with pytest.deprecated_call(match='hash_params will be removed'):
-        @cachier(hash_params=lambda a, k: 'key')
+        @cachier.cachier(hash_params=lambda a, k: 'key')
         def test():
             return 'value'
     assert test() == 'value'
 
 
 def test_separate_processes():
     test_args = ('python', 'tests/standalone_script.py')
@@ -222,7 +221,22 @@
     result = run_process()
     assert result.stdout.strip() == 'two 2'
     start = time()
     result = run_process()
     end = time()
     assert result.stdout.strip() == 'two 2'
     assert end - start < 3
+
+
+def test_global_disable():
+    @cachier.cachier()
+    def get_random():
+        return random()
+    get_random.clear_cache()
+    result_1 = get_random()
+    result_2 = get_random()
+    cachier.disable_caching()
+    result_3 = get_random()
+    cachier.enable_caching()
+    result_4 = get_random()
+    assert result_1 == result_2 == result_4
+    assert result_1 != result_3
```

### Comparing `cachier-2.1.0/tests/test_memory_core.py` & `cachier-2.1.1/tests/test_memory_core.py`

 * *Files identical despite different names*

### Comparing `cachier-2.1.0/tests/test_mongo_core.py` & `cachier-2.1.1/tests/test_mongo_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 import pytest
 import pymongo
 import hashlib
 import pandas as pd
 from pymongo.errors import OperationFailure
 
 from cachier import cachier
-from cachier.mongo_core import _MongoCore, RecalculationNeeded
+from cachier.base_core import RecalculationNeeded
+from cachier.mongo_core import _MongoCore
 
 from pymongo_inmemory import MongoClient
 
 
 _COLLECTION_NAME = 'cachier_test_{}_{}.{}.{}'.format(
     platform.system(), sys.version_info[0], sys.version_info[1],
     sys.version_info[2])
@@ -209,15 +210,15 @@
 
 
 @pytest.mark.mongo
 def test_stalled_mongo_db_cache():
     @cachier(mongetter=_test_mongetter)
     def _stalled_func():
         return 1
-    core = _MongoCore(_test_mongetter, None, 0)
+    core = _MongoCore(_test_mongetter, None, 0, {})
     core.set_func(_stalled_func)
     core.clear_cache()
     with pytest.raises(RecalculationNeeded):
         core.wait_on_entry_calc(key=None)
 
 
 @pytest.mark.mongo
@@ -258,14 +259,23 @@
     def _stalled_func_2():
         """Testing stalled function"""
         return 2
 
     res = _stalled_func_2()
     assert res == 2
 
+    @cachier(mongetter=_test_mongetter,
+             stale_after=stale_after, next_time=True)
+    def _stalled_func_3():
+        """Testing stalled function"""
+        return 3
+
+    res = _stalled_func_3()
+    assert res == 1
+
 
 @pytest.mark.mongo
 def test_callable_hash_param():
 
     def _hash_func(args, kwargs):
         def _hash(obj):
             if isinstance(obj, pd.core.frame.DataFrame):
```

### Comparing `cachier-2.1.0/tests/test_pickle_core.py` & `cachier-2.1.1/tests/test_pickle_core.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:  # python 2
     import Queue as queue
 
 import hashlib
 import pandas as pd
 
 from cachier import cachier
-from cachier.pickle_core import DEF_CACHIER_DIR
+from cachier.core import _default_params
 
 
 def _get_decorated_func(func, **kwargs):
     cachier_decorator = cachier(**kwargs)
     decorated_func = cachier_decorator(func)
     return decorated_func
 
@@ -45,28 +45,32 @@
 
 def _takes_2_seconds(arg_1, arg_2):
     """Some function."""
     sleep(2)
     return 'arg_1:{}, arg_2:{}'.format(arg_1, arg_2)
 
 
+@pytest.mark.pickle
+@pytest.mark.parametrize('reload', [True, False])
 @pytest.mark.parametrize('separate_files', [True, False])
-def test_pickle_core(separate_files):
+def test_pickle_core(reload, separate_files):
     """Basic Pickle core functionality."""
     _takes_2_seconds_decorated = _get_decorated_func(
-        _takes_2_seconds, next_time=False, separate_files=separate_files)
+        _takes_2_seconds, next_time=False,
+        pickle_reload=reload, separate_files=separate_files)
     _takes_2_seconds_decorated.clear_cache()
     _takes_2_seconds_decorated('a', 'b')
     start = time()
     _takes_2_seconds_decorated('a', 'b', verbose_cache=True)
     end = time()
     assert end - start < 1
     _takes_2_seconds_decorated.clear_cache()
 
 
+@pytest.mark.pickle
 @pytest.mark.parametrize('separate_files', [True, False])
 def test_pickle_core_keywords(separate_files):
     """Basic Pickle core functionality with keyword arguments."""
     _takes_2_seconds_decorated = _get_decorated_func(
         _takes_2_seconds, next_time=False, separate_files=separate_files)
     _takes_2_seconds_decorated.clear_cache()
     _takes_2_seconds_decorated('a', arg_2='b')
@@ -82,14 +86,15 @@
 
 
 def _stale_after_seconds(arg_1, arg_2):
     """Some function."""
     return random()
 
 
+@pytest.mark.pickle
 @pytest.mark.parametrize('separate_files', [True, False])
 def test_stale_after(separate_files):
     """Testing the stale_after functionality."""
     _stale_after_seconds_decorated = _get_decorated_func(
         _stale_after_seconds, stale_after=DELTA, next_time=False,
         separate_files=separate_files,
     )
@@ -106,14 +111,15 @@
 
 
 def _stale_after_next_time(arg_1, arg_2):
     """Some function."""
     return random()
 
 
+@pytest.mark.pickle
 @pytest.mark.parametrize('separate_files', [True, False])
 def test_stale_after_next_time(separate_files):
     """Testing the stale_after with next_time functionality."""
     _stale_after_next_time_decorated = _get_decorated_func(
         _stale_after_next_time, stale_after=DELTA, next_time=True,
         separate_files=separate_files,
     )
@@ -137,14 +143,15 @@
 
 
 def _random_num_with_arg(a):
     # print(a)
     return random()
 
 
+@pytest.mark.pickle
 @pytest.mark.parametrize('separate_files', [True, False])
 def test_overwrite_cache(separate_files):
     """Tests that the overwrite feature works correctly."""
     _random_num_decorated = _get_decorated_func(
         _random_num, separate_files=separate_files)
     _random_num_with_arg_decorated = _get_decorated_func(
         _random_num_with_arg, separate_files=separate_files)
@@ -165,14 +172,15 @@
     int3 = _random_num_with_arg_decorated('a', overwrite_cache=True)
     assert int3 != int1
     int4 = _random_num_with_arg_decorated('a')
     assert int4 == int3
     _random_num_with_arg_decorated.clear_cache()
 
 
+@pytest.mark.pickle
 @pytest.mark.parametrize('separate_files', [True, False])
 def test_ignore_cache(separate_files):
     """Tests that the ignore_cache feature works correctly."""
     _random_num_decorated = _get_decorated_func(
         _random_num, separate_files=separate_files)
     _random_num_with_arg_decorated = _get_decorated_func(
         _random_num_with_arg, separate_files=separate_files)
@@ -206,14 +214,15 @@
 
 
 def _calls_takes_time(takes_time_func, res_queue):
     res = takes_time_func(0.13, 0.02)
     res_queue.put(res)
 
 
+@pytest.mark.pickle
 @pytest.mark.parametrize('separate_files', [True, False])
 def test_pickle_being_calculated(separate_files):
     """Testing pickle core handling of being calculated scenarios."""
     _takes_time_decorated = _get_decorated_func(
         _takes_time, separate_files=separate_files)
     _takes_time_decorated.clear_cache()
     res_queue = queue.Queue()
@@ -232,16 +241,16 @@
             'res_queue': res_queue,
         },
         daemon=True,
     )
     thread1.start()
     sleep(0.5)
     thread2.start()
-    thread1.join(timeout=3)
-    thread2.join(timeout=3)
+    thread1.join(timeout=4)
+    thread2.join(timeout=4)
     assert res_queue.qsize() == 2
     res1 = res_queue.get()
     res2 = res_queue.get()
     assert res1 == res2
 
 
 def _being_calc_next_time(arg_1, arg_2):
@@ -251,14 +260,15 @@
 
 
 def _calls_being_calc_next_time(being_calc_func, res_queue):
     res = being_calc_func(0.13, 0.02)
     res_queue.put(res)
 
 
+@pytest.mark.pickle
 @pytest.mark.parametrize('separate_files', [True, False])
 def test_being_calc_next_time(separate_files):
     """Testing pickle core handling of being calculated scenarios."""
     _being_calc_next_time_decorated = _get_decorated_func(
         _being_calc_next_time,
         stale_after=timedelta(seconds=1),
         next_time=True,
@@ -303,15 +313,15 @@
 
 # _BAD_CACHE_FNAME = '.__main__._bad_cache'
 _BAD_CACHE_FNAME = '.tests.test_pickle_core._bad_cache'
 _BAD_CACHE_FNAME_SEPARATE_FILES = (
     '.tests.test_pickle_core._bad_cache_'
     f'{hashlib.sha256(pickle.dumps((0.13, 0.02))).hexdigest()}'
 )
-EXPANDED_CACHIER_DIR = os.path.expanduser(DEF_CACHIER_DIR)
+EXPANDED_CACHIER_DIR = os.path.expanduser(_default_params['cache_dir'])
 _BAD_CACHE_FPATH = os.path.join(EXPANDED_CACHIER_DIR, _BAD_CACHE_FNAME)
 _BAD_CACHE_FPATH_SEPARATE_FILES = os.path.join(
     EXPANDED_CACHIER_DIR, _BAD_CACHE_FNAME_SEPARATE_FILES)
 _BAD_CACHE_FPATHS = {
     True: _BAD_CACHE_FPATH_SEPARATE_FILES,
     False: _BAD_CACHE_FPATH,
 }
@@ -368,14 +378,15 @@
     res2 = res_queue.get()
     if not (res2 is None) or isinstance(res2, KeyError):
         return False
     return True
 
 
 # we want this to succeed at leat once
+@pytest.mark.pickle
 @pytest.mark.xfail
 @pytest.mark.parametrize('separate_files', [True, False])
 def test_bad_cache_file(separate_files):
     """Test pickle core handling of bad cache files."""
     sleeptimes = [0.1, 0.2, 0.3, 0.5, 0.6, 0.7, 0.8, 1, 1.5, 2]
     sleeptimes = sleeptimes + sleeptimes
     for sleeptime in sleeptimes:
@@ -460,26 +471,28 @@
     if not ((isinstance(res2, KeyError)) or ((res2 is None))):
         return False
     return True
     # print(res2)
     # print(type(res2))
 
 
+@pytest.mark.pickle
 @pytest.mark.xfail
 @pytest.mark.parametrize('separate_files', [False, True])
 def test_delete_cache_file(separate_files):
     """Test pickle core handling of missing cache files."""
     sleeptimes = [0.1, 0.2, 0.3, 0.5, 0.7, 1]
     sleeptimes = sleeptimes * 4
     for sleeptime in sleeptimes:
         if _helper_delete_cache_file(sleeptime, separate_files):
             return
     assert False
 
 
+@pytest.mark.pickle
 @pytest.mark.parametrize('separate_files', [False, True])
 def test_clear_being_calculated(separate_files):
     """Test pickle core clear `being calculated` functionality."""
     _takes_time_decorated = _get_decorated_func(
         _takes_time, separate_files=separate_files)
     _takes_time_decorated.clear_being_calculated()
 
@@ -489,14 +502,15 @@
         _error_throwing_func.count = 0
     _error_throwing_func.count += 1
     if _error_throwing_func.count > 1:
         raise ValueError("Tiny Rick!")
     return 7
 
 
+@pytest.mark.pickle
 @pytest.mark.parametrize('separate_files', [True, False])
 def test_error_throwing_func(separate_files):
     # with
     _error_throwing_func.count = 0
     _error_throwing_func_decorated = _get_decorated_func(
         _error_throwing_func,
         stale_after=timedelta(seconds=1),
@@ -518,14 +532,15 @@
 
 def _takes_2_seconds_custom_dir(arg_1, arg_2):
     """Some function."""
     sleep(2)
     return 'arg_1:{}, arg_2:{}'.format(arg_1, arg_2)
 
 
+@pytest.mark.pickle
 @pytest.mark.parametrize('separate_files', [True, False])
 def test_pickle_core_custom_cache_dir(separate_files):
     """Basic Pickle core functionality."""
     _takes_2_seconds_custom_dir_decorated = _get_decorated_func(
         _takes_2_seconds_custom_dir, next_time=False,
         cache_dir=CUSTOM_DIR, separate_files=separate_files,
     )
@@ -536,14 +551,15 @@
     end = time()
     assert end - start < 1
     _takes_2_seconds_custom_dir_decorated.clear_cache()
     path2test = _takes_2_seconds_custom_dir_decorated.cache_dpath()
     assert path2test == EXPANDED_CUSTOM_DIR
 
 
+@pytest.mark.pickle
 @pytest.mark.parametrize('separate_files', [True, False])
 def test_callable_hash_param(separate_files):
     def _hash_func(args, kwargs):
         def _hash(obj):
             if isinstance(obj, pd.core.frame.DataFrame):
                 return hashlib.sha256(
                     pd.util.hash_pandas_object(obj).values.tobytes()
```

### Comparing `cachier-2.1.0/tests/test_security.py` & `cachier-2.1.1/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `cachier-2.1.0/versioneer.py` & `cachier-2.1.1/versioneer.py`

 * *Files identical despite different names*

