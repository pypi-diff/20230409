# Comparing `tmp/pychan-0.5.0.tar.gz` & `tmp/pychan-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychan-0.5.0.tar", last modified: Wed Apr  5 06:12:10 2023, max compression
+gzip compressed data, was "pychan-0.6.0.tar", last modified: Sun Apr  9 20:53:43 2023, max compression
```

## Comparing `pychan-0.5.0.tar` & `pychan-0.6.0.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:12:10.603929 pychan-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-05 06:11:58.000000 pychan-0.5.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-05 06:11:58.000000 pychan-0.5.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:12:10.595929 pychan-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:12:10.599929 pychan-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-05 06:11:58.000000 pychan-0.5.0/.github/workflows/master.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-05 06:11:58.000000 pychan-0.5.0/.github/workflows/pull-requests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-05 06:11:58.000000 pychan-0.5.0/.github/workflows/tags.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-05 06:11:58.000000 pychan-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-05 06:11:58.000000 pychan-0.5.0/.style.yapf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 06:11:58.000000 pychan-0.5.0/.yapfignore
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-04-05 06:11:58.000000 pychan-0.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-05 06:11:58.000000 pychan-0.5.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-04-05 06:11:58.000000 pychan-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-05 06:11:58.000000 pychan-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9788 2023-04-05 06:12:10.603929 pychan-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-05 06:11:58.000000 pychan-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-05 06:11:58.000000 pychan-0.5.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-05 06:11:58.000000 pychan-0.5.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-05 06:11:58.000000 pychan-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-05 06:12:10.603929 pychan-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:12:10.595929 pychan-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:12:10.599929 pychan-0.5.0/src/pychan/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-05 06:11:58.000000 pychan-0.5.0/src/pychan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-05 06:11:58.000000 pychan-0.5.0/src/pychan/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20225 2023-04-05 06:11:58.000000 pychan-0.5.0/src/pychan/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-05 06:11:58.000000 pychan-0.5.0/src/pychan/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-04-05 06:11:58.000000 pychan-0.5.0/src/pychan/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-05 06:11:58.000000 pychan-0.5.0/src/pychan/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:12:10.599929 pychan-0.5.0/src/pychan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9788 2023-04-05 06:12:10.000000 pychan-0.5.0/src/pychan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-05 06:12:10.000000 pychan-0.5.0/src/pychan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 06:12:10.000000 pychan-0.5.0/src/pychan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 06:12:10.000000 pychan-0.5.0/src/pychan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-05 06:12:10.000000 pychan-0.5.0/src/pychan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-05 06:12:10.000000 pychan-0.5.0/src/pychan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:12:10.599929 pychan-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 06:11:58.000000 pychan-0.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:12:10.599929 pychan-0.5.0/tests/html/
--rw-r--r--   0 runner    (1001) docker     (123)   739214 2023-04-05 06:11:58.000000 pychan-0.5.0/tests/html/pol_archive.html
--rw-r--r--   0 runner    (1001) docker     (123)   136571 2023-04-05 06:11:58.000000 pychan-0.5.0/tests/html/pol_catalog.html
--rw-r--r--   0 runner    (1001) docker     (123)    14557 2023-04-05 06:11:58.000000 pychan-0.5.0/tests/html/pol_moderator_post.html
--rw-r--r--   0 runner    (1001) docker     (123)    22135 2023-04-05 06:11:58.000000 pychan-0.5.0/tests/html/pol_thread_posts.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 06:12:10.603929 pychan-0.5.0/tests/json/
--rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-04-05 06:11:58.000000 pychan-0.5.0/tests/json/search_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-04-05 06:11:58.000000 pychan-0.5.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-05 06:11:58.000000 pychan-0.5.0/tests/test_api_no_mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-05 06:11:58.000000 pychan-0.5.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-05 06:11:58.000000 pychan-0.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:53:43.653557 pychan-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-09 20:53:34.000000 pychan-0.6.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-09 20:53:34.000000 pychan-0.6.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:53:43.645557 pychan-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:53:43.649557 pychan-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-09 20:53:34.000000 pychan-0.6.0/.github/workflows/master.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-09 20:53:34.000000 pychan-0.6.0/.github/workflows/pull-requests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-09 20:53:34.000000 pychan-0.6.0/.github/workflows/tags.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-09 20:53:34.000000 pychan-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-09 20:53:34.000000 pychan-0.6.0/.style.yapf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 20:53:34.000000 pychan-0.6.0/.yapfignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-04-09 20:53:34.000000 pychan-0.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-09 20:53:34.000000 pychan-0.6.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-04-09 20:53:34.000000 pychan-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-09 20:53:34.000000 pychan-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-04-09 20:53:43.653557 pychan-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-04-09 20:53:34.000000 pychan-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-09 20:53:34.000000 pychan-0.6.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-09 20:53:34.000000 pychan-0.6.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-09 20:53:34.000000 pychan-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-09 20:53:43.653557 pychan-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:53:43.645557 pychan-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:53:43.649557 pychan-0.6.0/src/pychan/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-09 20:53:34.000000 pychan-0.6.0/src/pychan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-09 20:53:34.000000 pychan-0.6.0/src/pychan/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21647 2023-04-09 20:53:34.000000 pychan-0.6.0/src/pychan/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-09 20:53:34.000000 pychan-0.6.0/src/pychan/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-04-09 20:53:34.000000 pychan-0.6.0/src/pychan/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-09 20:53:34.000000 pychan-0.6.0/src/pychan/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:53:43.649557 pychan-0.6.0/src/pychan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-04-09 20:53:43.000000 pychan-0.6.0/src/pychan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-09 20:53:43.000000 pychan-0.6.0/src/pychan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 20:53:43.000000 pychan-0.6.0/src/pychan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 20:53:43.000000 pychan-0.6.0/src/pychan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-09 20:53:43.000000 pychan-0.6.0/src/pychan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-09 20:53:43.000000 pychan-0.6.0/src/pychan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:53:43.649557 pychan-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 20:53:34.000000 pychan-0.6.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:53:43.653557 pychan-0.6.0/tests/html/
+-rw-r--r--   0 runner    (1001) docker     (123)   739214 2023-04-09 20:53:34.000000 pychan-0.6.0/tests/html/pol_archive.html
+-rw-r--r--   0 runner    (1001) docker     (123)   136571 2023-04-09 20:53:34.000000 pychan-0.6.0/tests/html/pol_catalog.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14557 2023-04-09 20:53:34.000000 pychan-0.6.0/tests/html/pol_moderator_post.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22135 2023-04-09 20:53:34.000000 pychan-0.6.0/tests/html/pol_thread_posts.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 20:53:43.653557 pychan-0.6.0/tests/json/
+-rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-04-09 20:53:34.000000 pychan-0.6.0/tests/json/search_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17254 2023-04-09 20:53:34.000000 pychan-0.6.0/tests/json/search_results_unparsable_partial.json
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-09 20:53:34.000000 pychan-0.6.0/tests/json/search_results_unparsable_whole.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13207 2023-04-09 20:53:34.000000 pychan-0.6.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-09 20:53:34.000000 pychan-0.6.0/tests/test_api_no_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-09 20:53:34.000000 pychan-0.6.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-09 20:53:34.000000 pychan-0.6.0/tox.ini
```

### Comparing `pychan-0.5.0/.github/workflows/master.yml` & `pychan-0.6.0/.github/workflows/master.yml`

 * *Files identical despite different names*

### Comparing `pychan-0.5.0/.github/workflows/pull-requests.yml` & `pychan-0.6.0/.github/workflows/pull-requests.yml`

 * *Files identical despite different names*

### Comparing `pychan-0.5.0/.github/workflows/tags.yml` & `pychan-0.6.0/.github/workflows/tags.yml`

 * *Files identical despite different names*

### Comparing `pychan-0.5.0/.gitignore` & `pychan-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pychan-0.5.0/.style.yapf` & `pychan-0.6.0/.style.yapf`

 * *Files identical despite different names*

### Comparing `pychan-0.5.0/CHANGELOG.md` & `pychan-0.6.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,37 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
 Nothing currently!
 
+## v0.6.0 - 2023-04-09
+
+### Added
+
+* The `Thread` and `Post` models each now have a `url` property which contains a complete URL
+  linking directly to that particular thread or post in 4chan (by
+  [@cooperwalbrun](https://github.com/cooperwalbrun))
+
+### Fixed
+
+* The `search()` method will now raise a `ParsingError` when the data returned from 4chan is in an
+  unexpected format (by [@cooperwalbrun](https://github.com/cooperwalbrun))
+* The `search()` method will no longer induce HTTP 403 errors (thanks to its new Cloudflare-oriented
+  arguments) (by [@cooperwalbrun](https://github.com/cooperwalbrun))
+
+### Changed
+
+* Whitespace-only thread titles will now be converted into `None` within the `get_threads()` method
+  (by [@cooperwalbrun](https://github.com/cooperwalbrun))
+* The `search()` method now expects `user_agent` and `cloudflare_cookies` arguments containing the
+  `User-Agent` and `Cookie` header data needed to bypass the Cloudflare firewall in front of 4chan's
+  REST API (by [@cooperwalbrun](https://github.com/cooperwalbrun))
+
 ## v0.5.0 - 2023-04-05
 
 ### Added
 
 * The `File` model now has an `is_spoiler` field indicating whether the image was a "spoiler" image
   (by [@cooperwalbrun](https://github.com/cooperwalbrun))
 
@@ -20,15 +43,15 @@
 
 * The `get_threads()` method no longer iterates through a board's pages; instead, it directly
   scrapes threads from the catalog for the given board (by
   [@cooperwalbrun](https://github.com/cooperwalbrun))
 
 ### Removed
 
-* Support for Python 3.9 has been removed: `pychan` will now only build for Python 3.10 and 3.11 (by
+* Support for Python 3.9 has been removed; `pychan` will now only build for Python 3.10 and 3.11 (by
   [@cooperwalbrun](https://github.com/cooperwalbrun))
 
 ## v0.4.2 - 2023-04-04
 
 ### Fixed
 
 * The `get_boards()` method will no longer induce HTTP 403 errors (by
```

### Comparing `pychan-0.5.0/CONTRIBUTING.md` & `pychan-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pychan-0.5.0/LICENSE` & `pychan-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pychan-0.5.0/PKG-INFO` & `pychan-0.6.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,20 @@
-Metadata-Version: 2.1
-Name: pychan
-Version: 0.5.0
-Summary: A Python library for interacting with 4chan in a programmatically-friendly way.
-Home-page: https://github.com/cooperwalbrun/pychan
-Author: cooperwalbrun
-Author-email: mail@cooperwalbrun.io
-Platform: any
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: <4,>=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-Provides-Extra: github_actions
-Provides-Extra: development
-License-File: LICENSE
-
 # pychan [![master](https://github.com/cooperwalbrun/pychan/actions/workflows/master.yml/badge.svg)](https://github.com/cooperwalbrun/pychan/actions/workflows/master.yml) [![PyPI](https://img.shields.io/pypi/v/pychan)](https://pypi.org/project/pychan) [![codecov](https://codecov.io/gh/cooperwalbrun/pychan/branch/master/graph/badge.svg?token=BJEJOMIYWY)](https://codecov.io/gh/cooperwalbrun/pychan)
 
 1. [Overview](#overview)
 2. [Installation](#installation)
 3. [Usage](#usage)
    1. [General Notes](#general-notes)
    2. [Setup](#setup)
    3. [Fetch Board Names](#fetch-board-names)
    4. [Fetch Threads](#fetch-threads)
    5. [Fetch Archived Threads](#fetch-archived-threads)
    6. [Search 4chan](#search-4chan)
+      1. [About Cloudflare](#about-cloudflare)
+      2. [Search 4chan Code Example](#search-4chan-code-example)
    7. [Fetch Posts for a Specific Thread](#fetch-posts-for-a-specific-thread)
 4. [pychan Models](#pychan-models)
    1. [Threads](#threads)
    2. [Posts](#posts)
       1. [A Note About Replies](#a-note-about-replies)
    3. [Posters](#posters)
    4. [Files](#files)
@@ -137,19 +120,54 @@
     for post in fourchan.get_posts(thread):
         # Do stuff with the post - refer to the model documentation in pychan's README for details
         print(post.text)
 ```
 
 ### Search 4chan
 
+#### About Cloudflare
+
+Performing searches against 4chan is much more cumbersome than accessing the rest of 4chan's data.
+This is because 4chan has a Cloudflare firewall in front of its REST API, so the only way to get
+data back from searches is to supply the HTTP request information needed to bypass Cloudflare's
+anti-bot checks. Ultimately, this amounts to passing certain headers along with the HTTP request,
+but the challenge comes from actually acquiring such headers.
+
+It is currently beyond the scope of `pychan` to generate these headers for you, so if you would like
+to automate the circumvention of Cloudflare's protections, you may want to look into using a project
+like one of the following (this list is alphabetized and not exhaustive):
+
+* [ultrafunkamsterdam/undetected-chromedriver](https://github.com/ultrafunkamsterdam/undetected-chromedriver)
+* [VeNoMouS/cloudscraper](https://github.com/VeNoMouS/cloudscraper)
+* [wkeeling/selenium-wire](https://github.com/wkeeling/selenium-wire)
+
+A manual way to acquire these values is to perform a 4chan search using a web browser and leverage
+the browser's Developer Tools to trace the network requests that were made during the search. The
+request that contains the Cloudflare values will have been made to `https://find.4channel.org/api`
+with some query parameters. Once you have found this request, copy the `User-Agent` and `Cookie`
+values that were sent in your request, then pass them to `pychan`'s `search()` method. Be aware that
+the Cloudflare cookie(s) have an expiration on them, so this manual workaround will only return
+results until Cloudflare invalidates your cookie(s). After that, you will need to acquire new
+values.
+
+#### Search 4chan Code Example
+
 >Note: closed/stickied/archived threads are never returned in search results.
 
 ```python
-# Iterate over all threads returned in the search results lazily (Python Generator)
-for thread in fourchan.search(board="b", text="ylyl"):
+# This "threads" variable will contain a Python Generator (not a list) in order to facilitate laziness
+threads = fourchan.search(
+   board="b",
+   text="ylyl",
+   user_agent="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36",
+   cloudflare_cookies={
+      "cf_clearance": "bm2RICpcDeR4cXoC2nfI_cnZcbAkN4UYpN6c1zzeb8g-1440859602-0-160"
+   }
+)
+for thread in threads:
     # The thread object is the same class as the one returned by get_threads()
     for post in fourchan.get_posts(thread):
        # Do stuff with the post - refer to the model documentation in pychan's README for details
        print(post.text)
 ```
 
 ### Fetch Posts for a Specific Thread
@@ -189,29 +207,31 @@
 | ----- | ---- | ---------------- |
 | `thread.board` | `str` | `"b"`, `"int"`
 | `thread.number` | `int` | `882774935`, `168484869`
 | `thread.title` | `Optional[str]` | `None`, `"YLYL thread"`
 | `thread.is_stickied` | `bool` | `True`, `False`
 | `thread.is_closed` | `bool` | `True`, `False`
 | `thread.is_archived` | `bool` | `True`, `False`
+| `thread.url` | `str` | `"https://boards.4channel.org/a/thread/251097344"`
 
 ### Posts
 
 The table below corresponds to the `pychan.models.Post` class.
 
 | Field | Type | Example Value(s) |
 | ----- | ---- | ---------------- |
-`post.thread` | `Thread` | `pychan.models.Thread`
-`post.number` | `int` | `882774935`, `882774974`
-`post.timestamp` | [datetime.datetime](https://docs.python.org/3/library/datetime.html#datetime.datetime) | [datetime.datetime](https://docs.python.org/3/library/datetime.html#datetime.datetime)
-`post.poster` | `Poster` | `pychan.models.Poster`
-`post.text` | `str` | `">be me\n>be bored\n>write pychan\n>somehow it works"`
-`post.is_original_post` | `bool` | `True`, `False`
-`post.file` | `Optional[File]` | `None`, `pychan.models.File`
-`post.replies` | `list[Post]` | `[]`, `[pychan.models.Post, pychan.models.Post]`
+| `post.thread` | `Thread` | `pychan.models.Thread`
+| `post.number` | `int` | `882774935`, `882774974`
+| `post.timestamp` | [datetime.datetime](https://docs.python.org/3/library/datetime.html#datetime.datetime) | [datetime.datetime](https://docs.python.org/3/library/datetime.html#datetime.datetime)
+| `post.poster` | `Poster` | `pychan.models.Poster`
+| `post.text` | `str` | `">be me\n>be bored\n>write pychan\n>somehow it works"`
+| `post.is_original_post` | `bool` | `True`, `False`
+| `post.file` | `Optional[File]` | `None`, `pychan.models.File`
+| `post.replies` | `list[Post]` | `[]`, `[pychan.models.Post, pychan.models.Post]`
+| `post.url` | `str` | `"https://boards.4channel.org/a/thread/251097344#p251097419"`
 
 #### A Note About Replies
 
 The `replies` field shown above is purely a convenience feature `pychan` provides for accessing all
 posts within a thread which used the `>>` operator to "reply" to the current post. When you call the
 `get_posts()` method, you will still receive every available post and reply (in the order they were
 all posted) as a single, flat list.
```

### Comparing `pychan-0.5.0/README.md` & `pychan-0.6.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,39 @@
+Metadata-Version: 2.1
+Name: pychan
+Version: 0.6.0
+Summary: A Python library for interacting with 4chan in a programmatically-friendly way.
+Home-page: https://github.com/cooperwalbrun/pychan
+Author: cooperwalbrun
+Author-email: mail@cooperwalbrun.io
+Platform: any
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: <4,>=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+Provides-Extra: github_actions
+Provides-Extra: development
+License-File: LICENSE
+
 # pychan [![master](https://github.com/cooperwalbrun/pychan/actions/workflows/master.yml/badge.svg)](https://github.com/cooperwalbrun/pychan/actions/workflows/master.yml) [![PyPI](https://img.shields.io/pypi/v/pychan)](https://pypi.org/project/pychan) [![codecov](https://codecov.io/gh/cooperwalbrun/pychan/branch/master/graph/badge.svg?token=BJEJOMIYWY)](https://codecov.io/gh/cooperwalbrun/pychan)
 
 1. [Overview](#overview)
 2. [Installation](#installation)
 3. [Usage](#usage)
    1. [General Notes](#general-notes)
    2. [Setup](#setup)
    3. [Fetch Board Names](#fetch-board-names)
    4. [Fetch Threads](#fetch-threads)
    5. [Fetch Archived Threads](#fetch-archived-threads)
    6. [Search 4chan](#search-4chan)
+      1. [About Cloudflare](#about-cloudflare)
+      2. [Search 4chan Code Example](#search-4chan-code-example)
    7. [Fetch Posts for a Specific Thread](#fetch-posts-for-a-specific-thread)
 4. [pychan Models](#pychan-models)
    1. [Threads](#threads)
    2. [Posts](#posts)
       1. [A Note About Replies](#a-note-about-replies)
    3. [Posters](#posters)
    4. [Files](#files)
@@ -118,19 +139,54 @@
     for post in fourchan.get_posts(thread):
         # Do stuff with the post - refer to the model documentation in pychan's README for details
         print(post.text)
 ```
 
 ### Search 4chan
 
+#### About Cloudflare
+
+Performing searches against 4chan is much more cumbersome than accessing the rest of 4chan's data.
+This is because 4chan has a Cloudflare firewall in front of its REST API, so the only way to get
+data back from searches is to supply the HTTP request information needed to bypass Cloudflare's
+anti-bot checks. Ultimately, this amounts to passing certain headers along with the HTTP request,
+but the challenge comes from actually acquiring such headers.
+
+It is currently beyond the scope of `pychan` to generate these headers for you, so if you would like
+to automate the circumvention of Cloudflare's protections, you may want to look into using a project
+like one of the following (this list is alphabetized and not exhaustive):
+
+* [ultrafunkamsterdam/undetected-chromedriver](https://github.com/ultrafunkamsterdam/undetected-chromedriver)
+* [VeNoMouS/cloudscraper](https://github.com/VeNoMouS/cloudscraper)
+* [wkeeling/selenium-wire](https://github.com/wkeeling/selenium-wire)
+
+A manual way to acquire these values is to perform a 4chan search using a web browser and leverage
+the browser's Developer Tools to trace the network requests that were made during the search. The
+request that contains the Cloudflare values will have been made to `https://find.4channel.org/api`
+with some query parameters. Once you have found this request, copy the `User-Agent` and `Cookie`
+values that were sent in your request, then pass them to `pychan`'s `search()` method. Be aware that
+the Cloudflare cookie(s) have an expiration on them, so this manual workaround will only return
+results until Cloudflare invalidates your cookie(s). After that, you will need to acquire new
+values.
+
+#### Search 4chan Code Example
+
 >Note: closed/stickied/archived threads are never returned in search results.
 
 ```python
-# Iterate over all threads returned in the search results lazily (Python Generator)
-for thread in fourchan.search(board="b", text="ylyl"):
+# This "threads" variable will contain a Python Generator (not a list) in order to facilitate laziness
+threads = fourchan.search(
+   board="b",
+   text="ylyl",
+   user_agent="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36",
+   cloudflare_cookies={
+      "cf_clearance": "bm2RICpcDeR4cXoC2nfI_cnZcbAkN4UYpN6c1zzeb8g-1440859602-0-160"
+   }
+)
+for thread in threads:
     # The thread object is the same class as the one returned by get_threads()
     for post in fourchan.get_posts(thread):
        # Do stuff with the post - refer to the model documentation in pychan's README for details
        print(post.text)
 ```
 
 ### Fetch Posts for a Specific Thread
@@ -170,29 +226,31 @@
 | ----- | ---- | ---------------- |
 | `thread.board` | `str` | `"b"`, `"int"`
 | `thread.number` | `int` | `882774935`, `168484869`
 | `thread.title` | `Optional[str]` | `None`, `"YLYL thread"`
 | `thread.is_stickied` | `bool` | `True`, `False`
 | `thread.is_closed` | `bool` | `True`, `False`
 | `thread.is_archived` | `bool` | `True`, `False`
+| `thread.url` | `str` | `"https://boards.4channel.org/a/thread/251097344"`
 
 ### Posts
 
 The table below corresponds to the `pychan.models.Post` class.
 
 | Field | Type | Example Value(s) |
 | ----- | ---- | ---------------- |
-`post.thread` | `Thread` | `pychan.models.Thread`
-`post.number` | `int` | `882774935`, `882774974`
-`post.timestamp` | [datetime.datetime](https://docs.python.org/3/library/datetime.html#datetime.datetime) | [datetime.datetime](https://docs.python.org/3/library/datetime.html#datetime.datetime)
-`post.poster` | `Poster` | `pychan.models.Poster`
-`post.text` | `str` | `">be me\n>be bored\n>write pychan\n>somehow it works"`
-`post.is_original_post` | `bool` | `True`, `False`
-`post.file` | `Optional[File]` | `None`, `pychan.models.File`
-`post.replies` | `list[Post]` | `[]`, `[pychan.models.Post, pychan.models.Post]`
+| `post.thread` | `Thread` | `pychan.models.Thread`
+| `post.number` | `int` | `882774935`, `882774974`
+| `post.timestamp` | [datetime.datetime](https://docs.python.org/3/library/datetime.html#datetime.datetime) | [datetime.datetime](https://docs.python.org/3/library/datetime.html#datetime.datetime)
+| `post.poster` | `Poster` | `pychan.models.Poster`
+| `post.text` | `str` | `">be me\n>be bored\n>write pychan\n>somehow it works"`
+| `post.is_original_post` | `bool` | `True`, `False`
+| `post.file` | `Optional[File]` | `None`, `pychan.models.File`
+| `post.replies` | `list[Post]` | `[]`, `[pychan.models.Post, pychan.models.Post]`
+| `post.url` | `str` | `"https://boards.4channel.org/a/thread/251097344#p251097419"`
 
 #### A Note About Replies
 
 The `replies` field shown above is purely a convenience feature `pychan` provides for accessing all
 posts within a thread which used the `>>` operator to "reply" to the current post. When you call the
 `get_posts()` method, you will still receive every available post and reply (in the order they were
 all posted) as a single, flat list.
```

### Comparing `pychan-0.5.0/setup.cfg` & `pychan-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pychan-0.5.0/src/pychan/api.py` & `pychan-0.6.0/src/pychan/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 class ParsingError(Exception):
     pass
 
 
 class FourChan:
     _UNPARSABLE_BOARDS = ["f"]
     _POST_TEXT_SELECTOR = "blockquote.postMessage"
+    _USER_AGENT_HEADER_NAME = "User-Agent"
 
     def __init__(
         self,
         *,
         logger: Optional[PychanLogger] = None,
         raise_http_exceptions: bool = True,
         raise_parsing_exceptions: bool = True
@@ -85,15 +86,14 @@
                                       500) should be raised so that users of this FourChan instance
                                       will see them.
         :param raise_parsing_exceptions: Whether internal exceptions related to parsing errors (e.g.
                                          due to invalid/unrecognized HTML on HTTP responses) should
                                          be raised so that users of this FourChan instance will see
                                          them.
         """
-
         self._agent = str(uuid4())
         self._logger = logger if logger is not None else PychanLogger(LogLevel.OFF)
         self._raise_http_exceptions = raise_http_exceptions
         self._raise_parsing_exceptions = raise_parsing_exceptions
 
     def _parse_error(self, message: str) -> None:
         if self._raise_parsing_exceptions:
@@ -223,30 +223,27 @@
         # mocked in unit tests in a straightforward manner
         return
 
     def _request_helper(
         self,
         url: str,
         *,
-        expect_404: bool = False,
         headers: Optional[dict[str, str]] = None,
         params: Optional[dict[str, str]] = None
     ) -> Optional[Response]:
         self._throttle_request()
 
         h = {} if headers is None else headers
-        response = requests.get(url, headers={"User-Agent": self._agent, **h}, params=params)
+        response = requests.get(
+            url, headers={
+                self._USER_AGENT_HEADER_NAME: self._agent, **h
+            }, params=params
+        )
         if response.status_code == 200:
             return response
-        elif response.status_code == 404:
-            if not expect_404:
-                self._logger.warn(f"Received a 404 status code from {url}")
-                if self._raise_http_exceptions:
-                    response.raise_for_status()
-            return None
         else:
             self._logger.error(f"Unexpected status code {response.status_code} when fetching {url}")
             if self._raise_http_exceptions:
                 response.raise_for_status()
             return None
 
     def get_boards(self) -> list[str]:
@@ -255,17 +252,16 @@
 
         :return: The board names (without slashes in their names) currently available on 4chan.
         """
 
         ret = []
         self._logger.info("Fetching all boards from 4chan...")
 
-        # Below, we use https://boards.4channel.org/pol/catalog instead of the homepage of 4chan due
-        # to CloudFlare (and at the time of this writing, the VeNoMouS/cloudscraper repository on
-        # GitHub does not work and seems to have disabled GitHub issues entirely)
+        # Below, we just choose a random 4chan page which includes the header/footer containing the
+        # list of boards
         response = self._request_helper("https://boards.4channel.org/pol/catalog")
         if response is not None:
             soup = BeautifulSoup(response.text, "html.parser")
             board_list = _find_first(soup, ".boardList")
             if board_list is not None:
                 for anchor in board_list.select("a"):
                     board = anchor.text
@@ -300,21 +296,23 @@
                     for id, thread in json_data["threads"].items():
                         parsed_id = _safe_id_parse(id, offset=0)
                         if parsed_id is not None:
                             title = thread.get("sub")
                             if isinstance(title, bool):
                                 # The title will only be a boolean if no title exists (False)
                                 title = None
+                            title = title if title is not None and len(title.strip()) > 0 else None
                             ret.append(
                                 Thread(
                                     sanitized_board,
                                     parsed_id,
-                                    title=title if title is not None and len(title) > 0 else None,
+                                    title=title,
                                     is_stickied=thread.get("sticky") == 1,
-                                    is_closed=thread.get("closed") == 1
+                                    is_closed=thread.get("closed") == 1,
+                                    is_archived=False
                                 )
                             )
 
                     if len(ret) > 0:
                         return ret
         message = (
             f"No thread data could be parsed out of the HTML for the catalog page of the board "
@@ -407,35 +405,51 @@
                     t.is_archived = _find_first(post, ".desktop .archivedIcon") is not None
                     p.thread = t
 
                 ret.append(p)
 
         return ret
 
-    def search(self, *, board: str, text: str) -> Generator[Thread, None, None]:
+    def search(self, *, board: str, text: str, user_agent: str,
+               cloudflare_cookies: dict[str, str]) -> Generator[Thread, None, None]:
         """
         Executes a given text query in a given board. This method leverages 4chan's native search
         functionality.
 
         :param board: The board within which to perform the search. You may include slashes.
                       Examples: "/b/", "b", "vg/", "/vg"
         :param text: The text against which to search.
+        :param user_agent: The User-Agent header value to use in the HTTP request. If this value is
+                           not the same one that is tied to the provided user_agent, you will
+                           receive HTTP 403 errors.
+        :param cloudflare_cookies: A dictionary mapping cookie names to their values, where these
+                                   cookies are appropriate for bypassing the Cloudflare checks in
+                                   front of the 4chan API. If this value is not the same one that is
+                                   tied to the provided user_agent, you will receive HTTP 403
+                                   errors.
         :return: A Generator which yields threads one at a time until every thread in the search
                  results has been returned.
         """
         sanitized_board = _sanitize_board(board)
         if self._is_unparsable_board(sanitized_board):
             return
 
         query = text.strip()
 
         def get(o: int) -> Optional[Response]:
+            cookie = "; ".join([f"{k}={v}" for k, v in cloudflare_cookies.items()])
             return self._request_helper(
                 "https://find.4channel.org/api",
-                headers={"Accept": "application/json"},
+                headers={
+                    "Accept": "application/json",
+                    "Origin": "https://boards.4channel.org",
+                    "Referer": "https://boards.4channel.org/",
+                    self._USER_AGENT_HEADER_NAME: user_agent,
+                    "Cookie": cookie
+                },
                 params={
                     "o": str(o), "q": query, "b": sanitized_board
                 }
             )
 
         seen_thread_numbers = set()
 
@@ -449,30 +463,39 @@
                 f'"{text}"...'
             ))
 
             response = get(offset)
             offset += 10
 
             if response is not None:
-                for t in response.json().get("threads", []):
-                    number = t.get("thread", "")
-                    posts = t.get("posts", [])
-                    if len(number) > 1 and len(posts) > 0:
-                        title = posts[0].get("sub", "")
-                        title = title if len(title.strip()) > 0 else None
-                        thread = Thread(
-                            t.get("board", sanitized_board),
-                            int(number[1:]),
-                            title=title,
-                            # Closed/stickied/archived threads are not returned in search results
-                            is_stickied=False,
-                            is_closed=False,
-                            is_archived=False
-                        )
-                        if thread.number not in seen_thread_numbers:
-                            new_this_iteration = True
-                            seen_thread_numbers.add(thread.number)
-                            yield thread
-                        else:
-                            self._logger.debug(
-                                f"Skipping a duplicate thread in the search results: {thread}"
-                            )
+                threads = response.json().get("threads", [])
+                if isinstance(threads, list):
+                    for t in threads:
+                        try:
+                            number = t.get("thread", "")
+                            posts = t.get("posts", [])
+                            if len(number) > 1 and len(posts) > 0:
+                                title = posts[0].get("sub", "")
+                                title = title if len(title.strip()) > 0 else None
+                                thread = Thread(
+                                    t.get("board", sanitized_board),
+                                    int(number[1:]),
+                                    title=title,
+                                    # Closed/stickied/archived threads are not returned in search results
+                                    is_stickied=False,
+                                    is_closed=False,
+                                    is_archived=False
+                                )
+                                if thread.number not in seen_thread_numbers:
+                                    new_this_iteration = True
+                                    seen_thread_numbers.add(thread.number)
+                                    yield thread
+                                else:
+                                    self._logger.debug(
+                                        f"Skipping a duplicate thread in the search results: {thread}"
+                                    )
+                        except Exception as e:
+                            self._parse_error(str(e))
+                else:
+                    self._parse_error(
+                        f'Detected an unexpected structure in the "threads" JSON field: {threads}'
+                    )
```

### Comparing `pychan-0.5.0/src/pychan/logger.py` & `pychan-0.6.0/src/pychan/logger.py`

 * *Files identical despite different names*

### Comparing `pychan-0.5.0/src/pychan/models.py` & `pychan-0.6.0/src/pychan/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,16 +17,20 @@
         self.board = board
         self.number = number
         self.title = title
         self.is_stickied = is_stickied
         self.is_closed = is_closed
         self.is_archived = is_archived
 
+    @property
+    def url(self) -> str:
+        return f"https://boards.4channel.org/{self.board}/thread/{self.number}"
+
     def __repr__(self) -> str:
-        return f"Thread(https://boards.4channel.org/{self.board}/thread/{self.number})"
+        return f"Thread({self.url})"
 
     def __str__(self) -> str:
         return repr(self)
 
     def __hash__(self) -> int:
         return hash((self.board, self.number))
 
@@ -180,19 +184,23 @@
         self.timestamp = timestamp
         self.poster = poster
         self.text = text
         self.is_original_post = is_original_post
         self.file = file
         self.replies: list[Post] = replies if replies is not None else []
 
-    def __repr__(self) -> str:
-        return "Post(https://boards.4channel.org/{})".format(
+    @property
+    def url(self) -> str:
+        return "https://boards.4channel.org/{}".format(
             f"{self.thread.board}/thread/{self.thread.number}#p{self.number}"
         )
 
+    def __repr__(self) -> str:
+        return f"Post({self.url})"
+
     def __str__(self) -> str:
         return repr(self)
 
     def __hash__(self) -> int:
         return hash((self.number, self.thread.number))
 
     def __eq__(self, other: Any) -> bool:
```

### Comparing `pychan-0.5.0/src/pychan.egg-info/PKG-INFO` & `pychan-0.6.0/src/pychan.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychan
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Python library for interacting with 4chan in a programmatically-friendly way.
 Home-page: https://github.com/cooperwalbrun/pychan
 Author: cooperwalbrun
 Author-email: mail@cooperwalbrun.io
 Platform: any
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -24,14 +24,16 @@
 3. [Usage](#usage)
    1. [General Notes](#general-notes)
    2. [Setup](#setup)
    3. [Fetch Board Names](#fetch-board-names)
    4. [Fetch Threads](#fetch-threads)
    5. [Fetch Archived Threads](#fetch-archived-threads)
    6. [Search 4chan](#search-4chan)
+      1. [About Cloudflare](#about-cloudflare)
+      2. [Search 4chan Code Example](#search-4chan-code-example)
    7. [Fetch Posts for a Specific Thread](#fetch-posts-for-a-specific-thread)
 4. [pychan Models](#pychan-models)
    1. [Threads](#threads)
    2. [Posts](#posts)
       1. [A Note About Replies](#a-note-about-replies)
    3. [Posters](#posters)
    4. [Files](#files)
@@ -137,19 +139,54 @@
     for post in fourchan.get_posts(thread):
         # Do stuff with the post - refer to the model documentation in pychan's README for details
         print(post.text)
 ```
 
 ### Search 4chan
 
+#### About Cloudflare
+
+Performing searches against 4chan is much more cumbersome than accessing the rest of 4chan's data.
+This is because 4chan has a Cloudflare firewall in front of its REST API, so the only way to get
+data back from searches is to supply the HTTP request information needed to bypass Cloudflare's
+anti-bot checks. Ultimately, this amounts to passing certain headers along with the HTTP request,
+but the challenge comes from actually acquiring such headers.
+
+It is currently beyond the scope of `pychan` to generate these headers for you, so if you would like
+to automate the circumvention of Cloudflare's protections, you may want to look into using a project
+like one of the following (this list is alphabetized and not exhaustive):
+
+* [ultrafunkamsterdam/undetected-chromedriver](https://github.com/ultrafunkamsterdam/undetected-chromedriver)
+* [VeNoMouS/cloudscraper](https://github.com/VeNoMouS/cloudscraper)
+* [wkeeling/selenium-wire](https://github.com/wkeeling/selenium-wire)
+
+A manual way to acquire these values is to perform a 4chan search using a web browser and leverage
+the browser's Developer Tools to trace the network requests that were made during the search. The
+request that contains the Cloudflare values will have been made to `https://find.4channel.org/api`
+with some query parameters. Once you have found this request, copy the `User-Agent` and `Cookie`
+values that were sent in your request, then pass them to `pychan`'s `search()` method. Be aware that
+the Cloudflare cookie(s) have an expiration on them, so this manual workaround will only return
+results until Cloudflare invalidates your cookie(s). After that, you will need to acquire new
+values.
+
+#### Search 4chan Code Example
+
 >Note: closed/stickied/archived threads are never returned in search results.
 
 ```python
-# Iterate over all threads returned in the search results lazily (Python Generator)
-for thread in fourchan.search(board="b", text="ylyl"):
+# This "threads" variable will contain a Python Generator (not a list) in order to facilitate laziness
+threads = fourchan.search(
+   board="b",
+   text="ylyl",
+   user_agent="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36",
+   cloudflare_cookies={
+      "cf_clearance": "bm2RICpcDeR4cXoC2nfI_cnZcbAkN4UYpN6c1zzeb8g-1440859602-0-160"
+   }
+)
+for thread in threads:
     # The thread object is the same class as the one returned by get_threads()
     for post in fourchan.get_posts(thread):
        # Do stuff with the post - refer to the model documentation in pychan's README for details
        print(post.text)
 ```
 
 ### Fetch Posts for a Specific Thread
@@ -189,29 +226,31 @@
 | ----- | ---- | ---------------- |
 | `thread.board` | `str` | `"b"`, `"int"`
 | `thread.number` | `int` | `882774935`, `168484869`
 | `thread.title` | `Optional[str]` | `None`, `"YLYL thread"`
 | `thread.is_stickied` | `bool` | `True`, `False`
 | `thread.is_closed` | `bool` | `True`, `False`
 | `thread.is_archived` | `bool` | `True`, `False`
+| `thread.url` | `str` | `"https://boards.4channel.org/a/thread/251097344"`
 
 ### Posts
 
 The table below corresponds to the `pychan.models.Post` class.
 
 | Field | Type | Example Value(s) |
 | ----- | ---- | ---------------- |
-`post.thread` | `Thread` | `pychan.models.Thread`
-`post.number` | `int` | `882774935`, `882774974`
-`post.timestamp` | [datetime.datetime](https://docs.python.org/3/library/datetime.html#datetime.datetime) | [datetime.datetime](https://docs.python.org/3/library/datetime.html#datetime.datetime)
-`post.poster` | `Poster` | `pychan.models.Poster`
-`post.text` | `str` | `">be me\n>be bored\n>write pychan\n>somehow it works"`
-`post.is_original_post` | `bool` | `True`, `False`
-`post.file` | `Optional[File]` | `None`, `pychan.models.File`
-`post.replies` | `list[Post]` | `[]`, `[pychan.models.Post, pychan.models.Post]`
+| `post.thread` | `Thread` | `pychan.models.Thread`
+| `post.number` | `int` | `882774935`, `882774974`
+| `post.timestamp` | [datetime.datetime](https://docs.python.org/3/library/datetime.html#datetime.datetime) | [datetime.datetime](https://docs.python.org/3/library/datetime.html#datetime.datetime)
+| `post.poster` | `Poster` | `pychan.models.Poster`
+| `post.text` | `str` | `">be me\n>be bored\n>write pychan\n>somehow it works"`
+| `post.is_original_post` | `bool` | `True`, `False`
+| `post.file` | `Optional[File]` | `None`, `pychan.models.File`
+| `post.replies` | `list[Post]` | `[]`, `[pychan.models.Post, pychan.models.Post]`
+| `post.url` | `str` | `"https://boards.4channel.org/a/thread/251097344#p251097419"`
 
 #### A Note About Replies
 
 The `replies` field shown above is purely a convenience feature `pychan` provides for accessing all
 posts within a thread which used the `>>` operator to "reply" to the current post. When you call the
 `get_posts()` method, you will still receive every available post and reply (in the order they were
 all posted) as a single, flat list.
```

### Comparing `pychan-0.5.0/src/pychan.egg-info/SOURCES.txt` & `pychan-0.6.0/src/pychan.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -32,8 +32,10 @@
 tests/test_api.py
 tests/test_api_no_mocks.py
 tests/test_models.py
 tests/html/pol_archive.html
 tests/html/pol_catalog.html
 tests/html/pol_moderator_post.html
 tests/html/pol_thread_posts.html
-tests/json/search_results.json
+tests/json/search_results.json
+tests/json/search_results_unparsable_partial.json
+tests/json/search_results_unparsable_whole.json
```

### Comparing `pychan-0.5.0/tests/html/pol_archive.html` & `pychan-0.6.0/tests/html/pol_archive.html`

 * *Files identical despite different names*

### Comparing `pychan-0.5.0/tests/html/pol_catalog.html` & `pychan-0.6.0/tests/html/pol_catalog.html`

 * *Files identical despite different names*

### Comparing `pychan-0.5.0/tests/html/pol_moderator_post.html` & `pychan-0.6.0/tests/html/pol_moderator_post.html`

 * *Files identical despite different names*

### Comparing `pychan-0.5.0/tests/html/pol_thread_posts.html` & `pychan-0.6.0/tests/html/pol_thread_posts.html`

 * *Files identical despite different names*

### Comparing `pychan-0.5.0/tests/json/search_results.json` & `pychan-0.6.0/tests/json/search_results.json`

 * *Files identical despite different names*

### Comparing `pychan-0.5.0/tests/test_api.py` & `pychan-0.6.0/tests/test_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -295,51 +295,67 @@
     with_mocks(403, helper_no_raises)
     with_mocks(404, helper_no_raises)
     with_mocks(500, helper_no_raises)
     with_mocks(403, helper)
     with_mocks(500, helper)
 
 
-@responses.activate
-def test_search(fourchan: FourChan) -> None:
-    with open(f"{os.path.dirname(__file__)}/json/search_results.json", "r",
-              encoding="utf-8") as file:
-        test_data = file.read()
-
+def test_search(fourchan_no_raises: FourChan) -> None:
     board = "news"
     search_text = "democrat"
 
-    responses.add(
-        responses.GET,
-        f"https://find.4channel.org/api?q={parse.quote(search_text)}&b={board}&o=0",
-        status=200,
-        body=test_data
+    @responses.activate
+    def helper(file_name: str, *, expected_threads: list[Thread]) -> None:
+        with open(f"{os.path.dirname(__file__)}/json/{file_name}", "r", encoding="utf-8") as file:
+            test_data = file.read()
+
+        responses.add(
+            responses.GET,
+            f"https://find.4channel.org/api?q={parse.quote(search_text)}&b={board}&o=0",
+            status=200,
+            body=test_data
+        )
+        responses.add(
+            # This response terminates the iteration within the generator (the generator halts when
+            # it encounters a "page" of results which have all already been seen, so we simply mock
+            # the results on the second "page" as being identical to the results on the first "page"
+            # above)
+            responses.GET,
+            f"https://find.4channel.org/api?q={parse.quote(search_text)}&b={board}&o=10",
+            status=200,
+            body=test_data
+        )
+
+        actual = list(
+            fourchan_no_raises.search(
+                board=board, text=search_text, user_agent="test", cloudflare_cookies={}
+            )
+        )
+        assert len(expected_threads) == len(actual)
+        for i, thread in enumerate(expected_threads):
+            assert tuple(thread) == tuple(actual[i])
+
+    helper(
+        "search_results.json",
+        expected_threads=[
+            Thread(board, 1077597, title="Democrat corruption and grooming."),
+            Thread(board, 1077143, title="In Reality, All The Actual Groomers Are Republicans")
+        ]
     )
-    responses.add(
-        # This response terminates the iteration within the generator (the generator halts when it
-        # encounters a "page" of results which have all already been seen, so we simply mock the
-        # results on the second "page" as being identical to the results on the first "page" above)
-        responses.GET,
-        f"https://find.4channel.org/api?q={parse.quote(search_text)}&b={board}&o=10",
-        status=200,
-        body=test_data
+    helper(
+        "search_results_unparsable_partial.json",
+        expected_threads=[
+            Thread(board, 1077143, title="In Reality, All The Actual Groomers Are Republicans")
+        ]
     )
-
-    expected = [
-        Thread(board, 1077597, title="Democrat corruption and grooming."),
-        Thread(board, 1077143, title="In Reality, All The Actual Groomers Are Republicans")
-    ]
-    actual = list(fourchan.search(board=board, text=search_text))
-    assert len(expected) == len(actual)
-    for i, thread in enumerate(expected):
-        assert tuple(thread) == tuple(actual[i])
+    helper("search_results_unparsable_whole.json", expected_threads=[])
 
 
 def test_search_unparsable_board(fourchan: FourChan) -> None:
-    assert len(list(fourchan.search(board="f", text=""))) == 0
+    assert len(list(fourchan.get_threads("f"))) == 0
 
 
 def test_search_http_errors(fourchan: FourChan, fourchan_no_raises: FourChan) -> None:
     board = "news"
     search_text = "democrat"
 
     @responses.activate
@@ -348,21 +364,29 @@
             responses.GET,
             f"https://find.4channel.org/api?q={parse.quote(search_text)}&b={board}&o=0",
             status=status,
         )
         function()
 
     def helper_no_raises() -> None:
-        actual = list(fourchan_no_raises.search(board=board, text=search_text))
+        actual = list(
+            fourchan_no_raises.search(
+                board=board, text=search_text, user_agent="test", cloudflare_cookies={}
+            )
+        )
         assert len(actual) == 0
 
     def helper() -> None:
         with pytest.raises(HTTPError):
             # The call to list() below forces the generator to execute; without it, the actual HTTP
             # call never happens
-            list(fourchan.search(board=board, text=search_text))
+            list(
+                fourchan.search(
+                    board=board, text=search_text, user_agent="test", cloudflare_cookies={}
+                )
+            )
 
     with_mocks(403, helper_no_raises)
     with_mocks(404, helper_no_raises)
     with_mocks(500, helper_no_raises)
     with_mocks(403, helper)
     with_mocks(500, helper)
```

### Comparing `pychan-0.5.0/tests/test_api_no_mocks.py` & `pychan-0.6.0/tests/test_api_no_mocks.py`

 * *Files identical despite different names*

### Comparing `pychan-0.5.0/tests/test_models.py` & `pychan-0.6.0/tests/test_models.py`

 * *Files identical despite different names*

