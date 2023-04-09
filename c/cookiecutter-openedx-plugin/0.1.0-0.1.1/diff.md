# Comparing `tmp/cookiecutter-openedx-plugin-0.1.0.tar.gz` & `tmp/cookiecutter-openedx-plugin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiecutter-openedx-plugin-0.1.0.tar", last modified: Sun Apr  9 14:45:55 2023, max compression
+gzip compressed data, was "cookiecutter-openedx-plugin-0.1.1.tar", last modified: Sun Apr  9 15:00:03 2023, max compression
```

## Comparing `cookiecutter-openedx-plugin-0.1.0.tar` & `cookiecutter-openedx-plugin-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-09 14:45:55.228232 cookiecutter-openedx-plugin-0.1.0/
--rw-r--r--   0 mcdaniel   (501) staff       (20)    35136 2023-04-08 00:07:20.000000 cookiecutter-openedx-plugin-0.1.0/LICENSE.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)     6702 2023-04-09 14:45:55.228079 cookiecutter-openedx-plugin-0.1.0/PKG-INFO
--rw-r--r--   0 mcdaniel   (501) staff       (20)     4901 2023-04-09 14:39:23.000000 cookiecutter-openedx-plugin-0.1.0/README.md
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-09 14:45:55.225113 cookiecutter-openedx-plugin-0.1.0/cookiecutter_openedx_plugin.egg-info/
--rw-r--r--   0 mcdaniel   (501) staff       (20)     6702 2023-04-09 14:45:55.000000 cookiecutter-openedx-plugin-0.1.0/cookiecutter_openedx_plugin.egg-info/PKG-INFO
--rw-r--r--   0 mcdaniel   (501) staff       (20)      814 2023-04-09 14:45:55.000000 cookiecutter-openedx-plugin-0.1.0/cookiecutter_openedx_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2023-04-09 14:45:55.000000 cookiecutter-openedx-plugin-0.1.0/cookiecutter_openedx_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       88 2023-04-09 14:45:55.000000 cookiecutter-openedx-plugin-0.1.0/cookiecutter_openedx_plugin.egg-info/entry_points.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2023-04-09 14:45:55.000000 cookiecutter-openedx-plugin-0.1.0/cookiecutter_openedx_plugin.egg-info/not-zip-safe
--rw-r--r--   0 mcdaniel   (501) staff       (20)      107 2023-04-09 14:45:55.000000 cookiecutter-openedx-plugin-0.1.0/cookiecutter_openedx_plugin.egg-info/requires.txt
--rw-r--r--   0 mcdaniel   (501) staff       (20)       20 2023-04-09 14:45:55.000000 cookiecutter-openedx-plugin-0.1.0/cookiecutter_openedx_plugin.egg-info/top_level.txt
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-09 14:45:55.226424 cookiecutter-openedx-plugin-0.1.0/cookiecutter_plugin/
--rw-r--r--   0 mcdaniel   (501) staff       (20)       88 2023-04-08 00:24:18.000000 cookiecutter-openedx-plugin-0.1.0/cookiecutter_plugin/__init__.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     6347 2023-04-08 19:11:42.000000 cookiecutter-openedx-plugin-0.1.0/cookiecutter_plugin/apps.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-09 14:45:55.226671 cookiecutter-openedx-plugin-0.1.0/cookiecutter_plugin/badges/
--rw-r--r--   0 mcdaniel   (501) staff       (20)       88 2023-04-08 03:00:13.000000 cookiecutter-openedx-plugin-0.1.0/cookiecutter_plugin/badges/__init__.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-09 14:45:55.227146 cookiecutter-openedx-plugin-0.1.0/cookiecutter_plugin/badges/backends/
--rw-r--r--   0 mcdaniel   (501) staff       (20)       88 2023-04-08 03:00:07.000000 cookiecutter-openedx-plugin-0.1.0/cookiecutter_plugin/badges/backends/__init__.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     6862 2023-04-08 13:52:53.000000 cookiecutter-openedx-plugin-0.1.0/cookiecutter_plugin/badges/backends/badgr_boto3.py
-drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-09 14:45:55.227757 cookiecutter-openedx-plugin-0.1.0/cookiecutter_plugin/settings/
--rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-04-08 00:07:20.000000 cookiecutter-openedx-plugin-0.1.0/cookiecutter_plugin/settings/__init__.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)      887 2023-04-08 14:05:20.000000 cookiecutter-openedx-plugin-0.1.0/cookiecutter_plugin/settings/common.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)      166 2023-04-08 14:14:37.000000 cookiecutter-openedx-plugin-0.1.0/cookiecutter_plugin/settings/production.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)    16571 2023-04-08 19:02:36.000000 cookiecutter-openedx-plugin-0.1.0/cookiecutter_plugin/signals.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2498 2023-04-08 00:19:59.000000 cookiecutter-openedx-plugin-0.1.0/cookiecutter_plugin/utils.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     4800 2023-04-08 14:09:07.000000 cookiecutter-openedx-plugin-0.1.0/cookiecutter_plugin/waffle.py
--rw-r--r--   0 mcdaniel   (501) staff       (20)     2718 2023-04-08 00:43:39.000000 cookiecutter-openedx-plugin-0.1.0/pyproject.toml
--rw-r--r--   0 mcdaniel   (501) staff       (20)       38 2023-04-09 14:45:55.228276 cookiecutter-openedx-plugin-0.1.0/setup.cfg
--rw-r--r--   0 mcdaniel   (501) staff       (20)     4458 2023-04-08 00:43:51.000000 cookiecutter-openedx-plugin-0.1.0/setup.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-09 15:00:03.813953 cookiecutter-openedx-plugin-0.1.1/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    35136 2023-04-08 00:07:20.000000 cookiecutter-openedx-plugin-0.1.1/LICENSE.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     6554 2023-04-09 15:00:03.813804 cookiecutter-openedx-plugin-0.1.1/PKG-INFO
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     4761 2023-04-09 14:59:18.000000 cookiecutter-openedx-plugin-0.1.1/README.md
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-09 15:00:03.811007 cookiecutter-openedx-plugin-0.1.1/cookiecutter_openedx_plugin.egg-info/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     6554 2023-04-09 15:00:03.000000 cookiecutter-openedx-plugin-0.1.1/cookiecutter_openedx_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      814 2023-04-09 15:00:03.000000 cookiecutter-openedx-plugin-0.1.1/cookiecutter_openedx_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2023-04-09 15:00:03.000000 cookiecutter-openedx-plugin-0.1.1/cookiecutter_openedx_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       88 2023-04-09 15:00:03.000000 cookiecutter-openedx-plugin-0.1.1/cookiecutter_openedx_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        1 2023-04-09 15:00:03.000000 cookiecutter-openedx-plugin-0.1.1/cookiecutter_openedx_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      107 2023-04-09 15:00:03.000000 cookiecutter-openedx-plugin-0.1.1/cookiecutter_openedx_plugin.egg-info/requires.txt
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       20 2023-04-09 15:00:03.000000 cookiecutter-openedx-plugin-0.1.1/cookiecutter_openedx_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-09 15:00:03.812214 cookiecutter-openedx-plugin-0.1.1/cookiecutter_plugin/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       88 2023-04-08 00:24:18.000000 cookiecutter-openedx-plugin-0.1.1/cookiecutter_plugin/__init__.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     6347 2023-04-08 19:11:42.000000 cookiecutter-openedx-plugin-0.1.1/cookiecutter_plugin/apps.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-09 15:00:03.812441 cookiecutter-openedx-plugin-0.1.1/cookiecutter_plugin/badges/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       88 2023-04-08 03:00:13.000000 cookiecutter-openedx-plugin-0.1.1/cookiecutter_plugin/badges/__init__.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-09 15:00:03.812879 cookiecutter-openedx-plugin-0.1.1/cookiecutter_plugin/badges/backends/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       88 2023-04-08 03:00:07.000000 cookiecutter-openedx-plugin-0.1.1/cookiecutter_plugin/badges/backends/__init__.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     6862 2023-04-08 13:52:53.000000 cookiecutter-openedx-plugin-0.1.1/cookiecutter_plugin/badges/backends/badgr_boto3.py
+drwxr-xr-x   0 mcdaniel   (501) staff       (20)        0 2023-04-09 15:00:03.813493 cookiecutter-openedx-plugin-0.1.1/cookiecutter_plugin/settings/
+-rw-r--r--   0 mcdaniel   (501) staff       (20)        0 2023-04-08 00:07:20.000000 cookiecutter-openedx-plugin-0.1.1/cookiecutter_plugin/settings/__init__.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      887 2023-04-08 14:05:20.000000 cookiecutter-openedx-plugin-0.1.1/cookiecutter_plugin/settings/common.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)      166 2023-04-08 14:14:37.000000 cookiecutter-openedx-plugin-0.1.1/cookiecutter_plugin/settings/production.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)    16571 2023-04-08 19:02:36.000000 cookiecutter-openedx-plugin-0.1.1/cookiecutter_plugin/signals.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2498 2023-04-08 00:19:59.000000 cookiecutter-openedx-plugin-0.1.1/cookiecutter_plugin/utils.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     4800 2023-04-08 14:09:07.000000 cookiecutter-openedx-plugin-0.1.1/cookiecutter_plugin/waffle.py
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     2707 2023-04-09 14:54:49.000000 cookiecutter-openedx-plugin-0.1.1/pyproject.toml
+-rw-r--r--   0 mcdaniel   (501) staff       (20)       38 2023-04-09 15:00:03.813996 cookiecutter-openedx-plugin-0.1.1/setup.cfg
+-rw-r--r--   0 mcdaniel   (501) staff       (20)     4458 2023-04-08 00:43:51.000000 cookiecutter-openedx-plugin-0.1.1/setup.py
```

### Comparing `cookiecutter-openedx-plugin-0.1.0/LICENSE.txt` & `cookiecutter-openedx-plugin-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cookiecutter-openedx-plugin-0.1.0/PKG-INFO` & `cookiecutter-openedx-plugin-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cookiecutter-openedx-plugin
-Version: 0.1.0
+Version: 0.1.1
 Summary: An open edx plugin that implements customizations for deployment to Kubernetes
 Home-page: https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin
 Download-URL: https://github.com/cookiecutter-openedx/cookiecutter-openedx-devops.git
 Author: Lawrence McDaniel
 Author-email: Lawrence McDaniel <lpm0073@gmail.com>
 License: AGPLv3
 Project-URL: Homepage, https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin
 Project-URL: Documentation, https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin
 Project-URL: Repository, https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin
 Project-URL: Changelog, https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin/issues
-Keywords: Python,Django,Open edX,Plugin,REST API
-Classifier: Development Status :: 4 - Beta
+Keywords: Python,Django,Open edX,Plugin
+Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -53,27 +53,24 @@
 
 ### Install using Tutor
 
 See [Installing extra xblocks and requirements](https://docs.tutor.overhang.io/configuration.html)
 
 ```bash
 tutor config save       # to ensure that tutor's root folder system has been created
-echo "git+https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin.git" >> "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
+
+# OPTION 1: install as a PyPi package
+echo "cookiecutter-openedx-plugin==0.1.1" >> "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
+
+# OPTION 2: install as an editable requirement
+echo "-e git+https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin.git" >> "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
+
 cat "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
 tutor images build openedx
 tutor local quickstart
-
-# you'll also need to run this on your very first install
-# -----------------------------------------------------------------------------
-
-# run migrations
-tutor local run lms ./manage.py lms makemigrations
-tutor local run lms ./manage.py lms migrate
-tutor local run cms ./manage.py cms makemigrations
-tutor local run cms ./manage.py cms migrate
 ```
 
 ### Documentation
 
 Documentation is available here: [Documentation](https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin)
 
 ### Support
```

### Comparing `cookiecutter-openedx-plugin-0.1.0/README.md` & `cookiecutter-openedx-plugin-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -17,27 +17,24 @@
 
 ### Install using Tutor
 
 See [Installing extra xblocks and requirements](https://docs.tutor.overhang.io/configuration.html)
 
 ```bash
 tutor config save       # to ensure that tutor's root folder system has been created
-echo "git+https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin.git" >> "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
+
+# OPTION 1: install as a PyPi package
+echo "cookiecutter-openedx-plugin==0.1.1" >> "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
+
+# OPTION 2: install as an editable requirement
+echo "-e git+https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin.git" >> "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
+
 cat "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
 tutor images build openedx
 tutor local quickstart
-
-# you'll also need to run this on your very first install
-# -----------------------------------------------------------------------------
-
-# run migrations
-tutor local run lms ./manage.py lms makemigrations
-tutor local run lms ./manage.py lms migrate
-tutor local run cms ./manage.py cms makemigrations
-tutor local run cms ./manage.py cms migrate
 ```
 
 ### Documentation
 
 Documentation is available here: [Documentation](https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin)
 
 ### Support
```

### Comparing `cookiecutter-openedx-plugin-0.1.0/cookiecutter_openedx_plugin.egg-info/PKG-INFO` & `cookiecutter-openedx-plugin-0.1.1/cookiecutter_openedx_plugin.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: cookiecutter-openedx-plugin
-Version: 0.1.0
+Version: 0.1.1
 Summary: An open edx plugin that implements customizations for deployment to Kubernetes
 Home-page: https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin
 Download-URL: https://github.com/cookiecutter-openedx/cookiecutter-openedx-devops.git
 Author: Lawrence McDaniel
 Author-email: Lawrence McDaniel <lpm0073@gmail.com>
 License: AGPLv3
 Project-URL: Homepage, https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin
 Project-URL: Documentation, https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin
 Project-URL: Repository, https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin
 Project-URL: Changelog, https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin/blob/main/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin/issues
-Keywords: Python,Django,Open edX,Plugin,REST API
-Classifier: Development Status :: 4 - Beta
+Keywords: Python,Django,Open edX,Plugin
+Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -53,27 +53,24 @@
 
 ### Install using Tutor
 
 See [Installing extra xblocks and requirements](https://docs.tutor.overhang.io/configuration.html)
 
 ```bash
 tutor config save       # to ensure that tutor's root folder system has been created
-echo "git+https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin.git" >> "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
+
+# OPTION 1: install as a PyPi package
+echo "cookiecutter-openedx-plugin==0.1.1" >> "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
+
+# OPTION 2: install as an editable requirement
+echo "-e git+https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin.git" >> "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
+
 cat "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
 tutor images build openedx
 tutor local quickstart
-
-# you'll also need to run this on your very first install
-# -----------------------------------------------------------------------------
-
-# run migrations
-tutor local run lms ./manage.py lms makemigrations
-tutor local run lms ./manage.py lms migrate
-tutor local run cms ./manage.py cms makemigrations
-tutor local run cms ./manage.py cms migrate
 ```
 
 ### Documentation
 
 Documentation is available here: [Documentation](https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin)
 
 ### Support
```

### Comparing `cookiecutter-openedx-plugin-0.1.0/cookiecutter_openedx_plugin.egg-info/SOURCES.txt` & `cookiecutter-openedx-plugin-0.1.1/cookiecutter_openedx_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cookiecutter-openedx-plugin-0.1.0/cookiecutter_plugin/apps.py` & `cookiecutter-openedx-plugin-0.1.1/cookiecutter_plugin/apps.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-openedx-plugin-0.1.0/cookiecutter_plugin/badges/backends/badgr_boto3.py` & `cookiecutter-openedx-plugin-0.1.1/cookiecutter_plugin/badges/backends/badgr_boto3.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-openedx-plugin-0.1.0/cookiecutter_plugin/settings/common.py` & `cookiecutter-openedx-plugin-0.1.1/cookiecutter_plugin/settings/common.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-openedx-plugin-0.1.0/cookiecutter_plugin/signals.py` & `cookiecutter-openedx-plugin-0.1.1/cookiecutter_plugin/signals.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-openedx-plugin-0.1.0/cookiecutter_plugin/utils.py` & `cookiecutter-openedx-plugin-0.1.1/cookiecutter_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-openedx-plugin-0.1.0/cookiecutter_plugin/waffle.py` & `cookiecutter-openedx-plugin-0.1.1/cookiecutter_plugin/waffle.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-openedx-plugin-0.1.0/pyproject.toml` & `cookiecutter-openedx-plugin-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 build-backend = "setuptools.build_meta:__legacy__"
 
 #------------------------------------------------------------------------------
 # PyPi meta data
 #------------------------------------------------------------------------------
 [project]
 name = "cookiecutter-openedx-plugin"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Lawrence McDaniel", email="lpm0073@gmail.com" }
 ]
 description = "An open edx plugin that implements customizations for deployment to Kubernetes"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 3 - Alpha",
     "Framework :: Django",
     "Framework :: Django :: 2.2",
     "Framework :: Django :: 3.0",
     "Framework :: Django :: 3.1",
     "Framework :: Django :: 3.2",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
@@ -50,15 +50,15 @@
 ]
 dependencies = [
   "Django>=3.2,<=3.3",
   "validators",
   "django-environ"
 ]
 
-keywords = ["Python", "Django", "Open edX", "Plugin", "REST API"]
+keywords = ["Python", "Django", "Open edX", "Plugin"]
 
 [project.urls]
 Homepage = "https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin"
 Documentation = "https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin"
 Repository = "https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin"
 Changelog = "https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin/blob/main/CHANGELOG.md"
 "Bug Tracker" = "https://github.com/cookiecutter-openedx/cookiecutter-openedx-plugin/issues"
```

### Comparing `cookiecutter-openedx-plugin-0.1.0/setup.py` & `cookiecutter-openedx-plugin-0.1.1/setup.py`

 * *Files identical despite different names*

