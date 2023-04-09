# Comparing `tmp/addok-1.1.0rc2.tar.gz` & `tmp/addok-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "addok-1.1.0rc2.tar", last modified: Fri Nov 25 14:20:53 2022, max compression
+gzip compressed data, was "addok-1.1.1.tar", last modified: Sun Apr  9 20:27:41 2023, max compression
```

## Comparing `addok-1.1.0rc2.tar` & `addok-1.1.1.tar`

### file list

```diff
@@ -1,65 +1,56 @@
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2022-11-25 14:20:53.047168 addok-1.1.0rc2/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1069 2022-11-23 17:30:28.000000 addok-1.1.0rc2/LICENSE
--rw-r--r--   0 ybon      (1000) ybon      (1000)      117 2017-01-19 15:42:09.000000 addok-1.1.0rc2/MANIFEST.in
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2032 2022-11-25 14:20:53.047168 addok-1.1.0rc2/PKG-INFO
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1314 2022-11-23 17:30:28.000000 addok-1.1.0rc2/README.md
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2022-11-25 14:20:53.040502 addok-1.1.0rc2/addok/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      191 2017-03-14 18:36:42.000000 addok-1.1.0rc2/addok/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5100 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/autocomplete.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1878 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/batch.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2022-11-25 14:20:53.043835 addok-1.1.0rc2/addok/bin/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      947 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/bin/__init__.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2022-11-25 14:20:53.043835 addok-1.1.0rc2/addok/config/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4643 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/config/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5660 2022-11-25 14:16:30.000000 addok-1.1.0rc2/addok/config/default.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2375 2022-03-13 17:34:00.000000 addok-1.1.0rc2/addok/config/local.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1357 2016-05-31 07:25:03.000000 addok-1.1.0rc2/addok/config/local_geozones.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1602 2016-09-13 19:30:14.000000 addok-1.1.0rc2/addok/config/local_openaddress.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      205 2016-11-01 11:38:42.000000 addok-1.1.0rc2/addok/config/local_stable.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      734 2017-04-20 13:59:02.000000 addok-1.1.0rc2/addok/config/local_trigrams.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)       79 2017-02-27 14:58:03.000000 addok-1.1.0rc2/addok/config/test.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11499 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/core.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      796 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/db.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2312 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/ds.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4955 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/fuzzy.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2022-11-25 14:20:53.047168 addok-1.1.0rc2/addok/helpers/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4379 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/helpers/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7410 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/helpers/collectors.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      891 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/helpers/formatters.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1733 2019-05-09 13:53:45.000000 addok-1.1.0rc2/addok/helpers/http.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6576 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/helpers/index.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      241 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/helpers/keys.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2022-11-25 14:20:53.047168 addok-1.1.0rc2/addok/helpers/lua/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      316 2016-11-17 16:20:35.000000 addok-1.1.0rc2/addok/helpers/lua/filter_indexed.lua
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1477 2017-06-20 17:28:08.000000 addok-1.1.0rc2/addok/helpers/lua/manual_scan.lua
--rw-r--r--   0 ybon      (1000) ybon      (1000)      225 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/helpers/lua/order_by_frequency.lua
--rw-r--r--   0 ybon      (1000) ybon      (1000)      367 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/helpers/lua/order_by_max_score.lua
--rw-r--r--   0 ybon      (1000) ybon      (1000)      526 2016-11-17 16:46:58.000000 addok-1.1.0rc2/addok/helpers/lua/zinter.lua
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5044 2022-11-25 14:16:30.000000 addok-1.1.0rc2/addok/helpers/results.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      321 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/helpers/scripts.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1383 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/helpers/search.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      249 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/helpers/serializers.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6477 2022-11-25 14:16:30.000000 addok-1.1.0rc2/addok/helpers/text.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1595 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/hooks.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2022-11-25 14:20:53.047168 addok-1.1.0rc2/addok/http/
--rw-r--r--   0 ybon      (1000) ybon      (1000)       97 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/http/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6387 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/http/base.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      792 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/http/wsgi.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1546 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/pairs.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3775 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/pytest.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)    18216 2022-11-23 17:30:28.000000 addok-1.1.0rc2/addok/shell.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2022-11-25 14:20:53.043835 addok-1.1.0rc2/addok.egg-info/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2032 2022-11-25 14:20:52.000000 addok-1.1.0rc2/addok.egg-info/PKG-INFO
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1237 2022-11-25 14:20:52.000000 addok-1.1.0rc2/addok.egg-info/SOURCES.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)        1 2022-11-25 14:20:52.000000 addok-1.1.0rc2/addok.egg-info/dependency_links.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)       74 2022-11-25 14:20:52.000000 addok-1.1.0rc2/addok.egg-info/entry_points.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)      178 2022-11-25 14:20:52.000000 addok-1.1.0rc2/addok.egg-info/requires.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)       14 2022-11-25 14:20:52.000000 addok-1.1.0rc2/addok.egg-info/top_level.txt
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2022-11-25 14:20:53.047168 addok-1.1.0rc2/fabfile/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5193 2017-07-21 17:34:46.000000 addok-1.1.0rc2/fabfile/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      860 2022-11-23 17:30:28.000000 addok-1.1.0rc2/fabfile/france.local.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1124 2018-02-16 18:27:45.000000 addok-1.1.0rc2/fabfile/prod.local.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)       81 2022-10-22 07:50:10.000000 addok-1.1.0rc2/pyproject.toml
--rw-r--r--   0 ybon      (1000) ybon      (1000)      148 2022-11-25 14:16:30.000000 addok-1.1.0rc2/requirements.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)       38 2022-11-25 14:20:53.047168 addok-1.1.0rc2/setup.cfg
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2939 2022-11-25 14:18:46.000000 addok-1.1.0rc2/setup.py
+drwxr-xr-x   0 jerome     (501) staff       (20)        0 2023-04-09 20:27:41.044800 addok-1.1.1/
+-rw-r--r--   0 jerome     (501) staff       (20)     1069 2022-12-05 12:32:41.000000 addok-1.1.1/LICENSE
+-rw-r--r--   0 jerome     (501) staff       (20)      117 2022-10-22 08:32:59.000000 addok-1.1.1/MANIFEST.in
+-rw-r--r--   0 jerome     (501) staff       (20)     1931 2023-04-09 20:27:41.044660 addok-1.1.1/PKG-INFO
+-rw-r--r--   0 jerome     (501) staff       (20)     1114 2023-04-09 20:07:24.000000 addok-1.1.1/README.md
+drwxr-xr-x   0 jerome     (501) staff       (20)        0 2023-04-09 20:27:41.040837 addok-1.1.1/addok/
+-rw-r--r--   0 jerome     (501) staff       (20)      191 2023-03-23 14:16:16.000000 addok-1.1.1/addok/__init__.py
+-rw-r--r--   0 jerome     (501) staff       (20)     5100 2023-03-23 14:16:16.000000 addok-1.1.1/addok/autocomplete.py
+-rw-r--r--   0 jerome     (501) staff       (20)     1878 2023-04-06 15:41:10.000000 addok-1.1.1/addok/batch.py
+drwxr-xr-x   0 jerome     (501) staff       (20)        0 2023-04-09 20:27:41.041761 addok-1.1.1/addok/bin/
+-rw-r--r--   0 jerome     (501) staff       (20)      947 2023-03-23 14:16:16.000000 addok-1.1.1/addok/bin/__init__.py
+drwxr-xr-x   0 jerome     (501) staff       (20)        0 2023-04-09 20:27:41.042116 addok-1.1.1/addok/config/
+-rw-r--r--   0 jerome     (501) staff       (20)     4643 2023-03-23 14:16:16.000000 addok-1.1.1/addok/config/__init__.py
+-rw-r--r--   0 jerome     (501) staff       (20)     5663 2023-03-23 14:16:16.000000 addok-1.1.1/addok/config/default.py
+-rw-r--r--   0 jerome     (501) staff       (20)       79 2023-03-23 14:16:16.000000 addok-1.1.1/addok/config/test.py
+-rw-r--r--   0 jerome     (501) staff       (20)    11499 2023-04-07 14:58:14.000000 addok-1.1.1/addok/core.py
+-rw-r--r--   0 jerome     (501) staff       (20)      796 2023-03-23 14:16:16.000000 addok-1.1.1/addok/db.py
+-rw-r--r--   0 jerome     (501) staff       (20)     2312 2023-03-23 14:16:16.000000 addok-1.1.1/addok/ds.py
+-rw-r--r--   0 jerome     (501) staff       (20)     4955 2023-03-23 14:16:16.000000 addok-1.1.1/addok/fuzzy.py
+drwxr-xr-x   0 jerome     (501) staff       (20)        0 2023-04-09 20:27:41.043322 addok-1.1.1/addok/helpers/
+-rw-r--r--   0 jerome     (501) staff       (20)     4679 2023-04-06 15:43:31.000000 addok-1.1.1/addok/helpers/__init__.py
+-rw-r--r--   0 jerome     (501) staff       (20)     7410 2023-03-23 14:16:16.000000 addok-1.1.1/addok/helpers/collectors.py
+-rw-r--r--   0 jerome     (501) staff       (20)      891 2023-03-23 14:16:16.000000 addok-1.1.1/addok/helpers/formatters.py
+-rw-r--r--   0 jerome     (501) staff       (20)     6576 2023-03-23 14:16:16.000000 addok-1.1.1/addok/helpers/index.py
+-rw-r--r--   0 jerome     (501) staff       (20)      241 2023-03-23 14:16:16.000000 addok-1.1.1/addok/helpers/keys.py
+drwxr-xr-x   0 jerome     (501) staff       (20)        0 2023-04-09 20:27:41.043795 addok-1.1.1/addok/helpers/lua/
+-rw-r--r--   0 jerome     (501) staff       (20)     1477 2023-03-23 14:16:16.000000 addok-1.1.1/addok/helpers/lua/manual_scan.lua
+-rw-r--r--   0 jerome     (501) staff       (20)      225 2023-03-23 14:16:16.000000 addok-1.1.1/addok/helpers/lua/order_by_frequency.lua
+-rw-r--r--   0 jerome     (501) staff       (20)      367 2023-03-23 14:16:16.000000 addok-1.1.1/addok/helpers/lua/order_by_max_score.lua
+-rw-r--r--   0 jerome     (501) staff       (20)      526 2023-03-23 14:16:16.000000 addok-1.1.1/addok/helpers/lua/zinter.lua
+-rw-r--r--   0 jerome     (501) staff       (20)     5044 2023-03-23 14:16:16.000000 addok-1.1.1/addok/helpers/results.py
+-rw-r--r--   0 jerome     (501) staff       (20)      321 2023-03-23 14:16:16.000000 addok-1.1.1/addok/helpers/scripts.py
+-rw-r--r--   0 jerome     (501) staff       (20)     1383 2023-03-23 14:16:16.000000 addok-1.1.1/addok/helpers/search.py
+-rw-r--r--   0 jerome     (501) staff       (20)      249 2023-03-23 14:16:16.000000 addok-1.1.1/addok/helpers/serializers.py
+-rw-r--r--   0 jerome     (501) staff       (20)     6477 2023-03-23 14:16:16.000000 addok-1.1.1/addok/helpers/text.py
+-rw-r--r--   0 jerome     (501) staff       (20)     1595 2023-03-23 14:16:16.000000 addok-1.1.1/addok/hooks.py
+drwxr-xr-x   0 jerome     (501) staff       (20)        0 2023-04-09 20:27:41.044205 addok-1.1.1/addok/http/
+-rw-r--r--   0 jerome     (501) staff       (20)       97 2023-03-23 14:16:16.000000 addok-1.1.1/addok/http/__init__.py
+-rw-r--r--   0 jerome     (501) staff       (20)     6660 2023-03-23 14:16:16.000000 addok-1.1.1/addok/http/base.py
+-rw-r--r--   0 jerome     (501) staff       (20)      792 2023-03-23 14:16:16.000000 addok-1.1.1/addok/http/wsgi.py
+-rw-r--r--   0 jerome     (501) staff       (20)     1546 2023-03-23 14:16:16.000000 addok-1.1.1/addok/pairs.py
+-rw-r--r--   0 jerome     (501) staff       (20)     3775 2023-03-23 14:16:16.000000 addok-1.1.1/addok/pytest.py
+-rw-r--r--   0 jerome     (501) staff       (20)    18216 2023-03-23 14:16:16.000000 addok-1.1.1/addok/shell.py
+drwxr-xr-x   0 jerome     (501) staff       (20)        0 2023-04-09 20:27:41.041615 addok-1.1.1/addok.egg-info/
+-rw-r--r--   0 jerome     (501) staff       (20)     1931 2023-04-09 20:27:41.000000 addok-1.1.1/addok.egg-info/PKG-INFO
+-rw-r--r--   0 jerome     (501) staff       (20)      994 2023-04-09 20:27:41.000000 addok-1.1.1/addok.egg-info/SOURCES.txt
+-rw-r--r--   0 jerome     (501) staff       (20)        1 2023-04-09 20:27:41.000000 addok-1.1.1/addok.egg-info/dependency_links.txt
+-rw-r--r--   0 jerome     (501) staff       (20)       74 2023-04-09 20:27:41.000000 addok-1.1.1/addok.egg-info/entry_points.txt
+-rw-r--r--   0 jerome     (501) staff       (20)      197 2023-04-09 20:27:41.000000 addok-1.1.1/addok.egg-info/requires.txt
+-rw-r--r--   0 jerome     (501) staff       (20)       14 2023-04-09 20:27:41.000000 addok-1.1.1/addok.egg-info/top_level.txt
+drwxr-xr-x   0 jerome     (501) staff       (20)        0 2023-04-09 20:27:41.044451 addok-1.1.1/fabfile/
+-rw-r--r--   0 jerome     (501) staff       (20)     5193 2022-10-22 08:32:59.000000 addok-1.1.1/fabfile/__init__.py
+-rw-r--r--   0 jerome     (501) staff       (20)      860 2022-12-05 12:32:41.000000 addok-1.1.1/fabfile/france.local.py
+-rw-r--r--   0 jerome     (501) staff       (20)      148 2023-04-09 20:07:24.000000 addok-1.1.1/requirements.txt
+-rw-r--r--   0 jerome     (501) staff       (20)       38 2023-04-09 20:27:41.044847 addok-1.1.1/setup.cfg
+-rw-r--r--   0 jerome     (501) staff       (20)     3032 2023-04-09 20:23:29.000000 addok-1.1.1/setup.py
```

### Comparing `addok-1.1.0rc2/LICENSE` & `addok-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/addok/autocomplete.py` & `addok-1.1.1/addok/autocomplete.py`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/addok/batch.py` & `addok-1.1.1/addok/batch.py`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/addok/bin/__init__.py` & `addok-1.1.1/addok/bin/__init__.py`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/addok/config/__init__.py` & `addok-1.1.1/addok/config/__init__.py`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/addok/config/default.py` & `addok-1.1.1/addok/config/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,18 @@
     },
 }
 
 # Min/max number of results to be retrieved from db and scored.
 BUCKET_MIN = 10
 BUCKET_MAX = 100
 
-# Above this treshold, terms are considered commons.
+# Above this threshold, terms are considered commons.
 COMMON_THRESHOLD = 10000
 
-# Above this treshold, we avoid intersecting sets.
+# Above this threshold, we avoid intersecting sets.
 INTERSECT_LIMIT = 100000
 
 # Min score considered matching the query.
 MATCH_THRESHOLD = 0.9
 
 # Do not consider result if final score is below this threshold.
 MIN_SCORE = 0.1
@@ -156,15 +156,15 @@
 
 LOG_QUERIES = False
 LOG_NOT_FOUND = False
 SLOW_QUERIES = False  # False or time in ms to consider query as slow
 
 INDEX_EDGE_NGRAMS = True
 
-# surrouding letters on a standard keyboard (default french azerty)
+# surrounding letters on a standard keyboard (default french azerty)
 FUZZY_KEY_MAP = {
     "a": "ezqop",
     "z": "aqse",
     "e": "azsdryu",
     "r": "edft",
     "t": "rfgy",
     "y": "teghu",
```

### Comparing `addok-1.1.0rc2/addok/core.py` & `addok-1.1.1/addok/core.py`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/addok/db.py` & `addok-1.1.1/addok/db.py`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/addok/ds.py` & `addok-1.1.1/addok/ds.py`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/addok/fuzzy.py` & `addok-1.1.1/addok/fuzzy.py`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/addok/helpers/__init__.py` & `addok-1.1.1/addok/helpers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import csv
 import sys
+from itertools import islice
 from functools import wraps
 from importlib import import_module
 from math import asin, cos, exp, radians, sin, sqrt
 from multiprocessing.pool import RUN, IMapUnorderedIterator, Pool
 
 from progressist import ProgressBar
 
@@ -170,11 +171,22 @@
         )
         self._taskqueue.put((tasks, result._set_length))
         return result
 
 
 def parallelize(func, iterable, chunk_size, **bar_kwargs):
     bar = Bar(prefix="Processing…", **bar_kwargs)
-    with ChunkedPool(processes=config.BATCH_WORKERS) as pool:
-        for chunk in pool.imap_unordered(func, iterable, chunk_size):
+
+    if sys.platform == "darwin":
+        while True:
+            chunk = list(islice(iterable, chunk_size))
+            if not chunk:
+                bar.finish()
+                break
+
+            func(*chunk)
             bar(step=len(chunk))
-        bar.finish()
+    else:
+        with ChunkedPool(processes=config.BATCH_WORKERS) as pool:
+            for chunk in pool.imap_unordered(func, iterable, chunk_size):
+                bar(step=len(chunk))
+            bar.finish()
```

### Comparing `addok-1.1.0rc2/addok/helpers/collectors.py` & `addok-1.1.1/addok/helpers/collectors.py`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/addok/helpers/formatters.py` & `addok-1.1.1/addok/helpers/formatters.py`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/addok/helpers/index.py` & `addok-1.1.1/addok/helpers/index.py`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/addok/helpers/lua/manual_scan.lua` & `addok-1.1.1/addok/helpers/lua/manual_scan.lua`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/addok/helpers/lua/zinter.lua` & `addok-1.1.1/addok/helpers/lua/zinter.lua`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/addok/helpers/results.py` & `addok-1.1.1/addok/helpers/results.py`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/addok/helpers/search.py` & `addok-1.1.1/addok/helpers/search.py`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/addok/helpers/text.py` & `addok-1.1.1/addok/helpers/text.py`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/addok/hooks.py` & `addok-1.1.1/addok/hooks.py`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/addok/http/base.py` & `addok-1.1.1/addok/http/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pathlib import Path
 import time
 
 import falcon
 
 from addok.config import config
 from addok.core import reverse, search
+from addok.db import DB
 from addok.helpers.text import EntityTooLarge
 
 notfound_logger = None
 query_logger = None
 slow_query_logger = None
 
 
@@ -187,17 +188,27 @@
             raise falcon.HTTPMissingParam("lat")
         limit = req.get_param_as_int("limit") or 1
         filters = self.match_filters(req)
         results = reverse(lat=lat, lon=lon, limit=limit, **filters)
         self.render(req, resp, results, filters=filters, limit=limit)
 
 
+class Health(View):
+    def on_get(self, req, resp):
+        return self.json(
+            req,
+            resp,
+            {"status": "HEALTHY", "redis_version": DB.info().get("redis_version")},
+        )
+
+
 def register_http_endpoint(api):
     api.add_route("/search", Search())
     api.add_route("/reverse", Reverse())
+    api.add_route("/health", Health())
 
 
 def register_command(subparsers):
     parser = subparsers.add_parser("serve", help="Run debug server")
     parser.set_defaults(func=run)
     parser.add_argument(
         "--host", default="127.0.0.1", help="Host to expose the demo serve on"
```

### Comparing `addok-1.1.0rc2/addok/http/wsgi.py` & `addok-1.1.1/addok/http/wsgi.py`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/addok/pairs.py` & `addok-1.1.1/addok/pairs.py`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/addok/pytest.py` & `addok-1.1.1/addok/pytest.py`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/addok/shell.py` & `addok-1.1.1/addok/shell.py`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/fabfile/__init__.py` & `addok-1.1.1/fabfile/__init__.py`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/fabfile/france.local.py` & `addok-1.1.1/fabfile/france.local.py`

 * *Files identical despite different names*

### Comparing `addok-1.1.0rc2/setup.py` & `addok-1.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     ext_modules.extend([
         Extension('addok.helpers.' + ext,
                   [path.join('addok', 'helpers', ext + '.py')])
         for ext in list_modules(path.join(here, 'addok', 'helpers'))])
 
     cmdclass = {'build_ext': build_ext}
 
-VERSION = (1, 1, 0, 'rc2')
+VERSION = (1, 1, 1)
 
 __author__ = 'Yohan Boniface'
 __contact__ = "yohan.boniface@data.gouv.fr"
 __homepage__ = "https://github.com/addok/addok"
 __version__ = ".".join(map(str, VERSION))
 
 setup(
@@ -78,17 +78,19 @@
     classifiers=[
         'Development Status :: 5 - Production/Stable',
 
         'Intended Audience :: Developers',
         'Topic :: Scientific/Engineering :: GIS',
 
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     keywords='address openstreetmap geocoding',
     packages=find_packages(exclude=['tests']),
     install_requires=install_requires,
     extras_require={'test': ['pytest'], 'docs': 'mkdocs'},
     include_package_data=True,
     ext_modules=ext_modules,
```

