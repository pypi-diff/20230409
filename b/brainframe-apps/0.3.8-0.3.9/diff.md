# Comparing `tmp/brainframe_apps-0.3.8.tar.gz` & `tmp/brainframe_apps-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainframe_apps-0.3.8.tar", max compression
+gzip compressed data, was "brainframe_apps-0.3.9.tar", max compression
```

## Comparing `brainframe_apps-0.3.8.tar` & `brainframe_apps-0.3.9.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0    16384 2023-04-08 06:41:18.520580 brainframe_apps-0.3.8/brainframe_apps/.add_stream.py.swp
--rw-r--r--   0        0        0      573 2023-04-08 04:43:59.581232 brainframe_apps-0.3.8/brainframe_apps/__init__.py
--rw-r--r--   0        0        0     4817 2023-04-08 06:21:09.934999 brainframe_apps-0.3.8/brainframe_apps/add_stream.py
--rw-r--r--   0        0        0      665 2022-12-19 23:19:56.515826 brainframe_apps-0.3.8/brainframe_apps/bf_log_print.py
--rw-r--r--   0        0        0    15026 2023-04-08 06:35:37.058992 brainframe_apps-0.3.8/brainframe_apps/capsule_control.py
--rw-r--r--   0        0        0      571 2023-04-08 04:43:59.581232 brainframe_apps-0.3.8/brainframe_apps/command_utils.py
--rw-r--r--   0        0        0     2582 2023-04-08 06:39:20.092029 brainframe_apps-0.3.8/brainframe_apps/delete_stream.py
--rw-r--r--   0        0        0     4691 2022-12-19 23:19:56.515826 brainframe_apps-0.3.8/brainframe_apps/fps_report.py
--rw-r--r--   0        0        0     6343 2023-04-08 06:35:12.074876 brainframe_apps-0.3.8/brainframe_apps/get_configuration.py
--rw-r--r--   0        0        0     8146 2023-04-08 06:35:51.659060 brainframe_apps-0.3.8/brainframe_apps/get_zone_statuses.py
--rw-r--r--   0        0        0     4733 2023-04-08 06:36:26.419221 brainframe_apps-0.3.8/brainframe_apps/identity_control.py
--rw-r--r--   0        0        0     2434 2023-04-08 06:34:33.690698 brainframe_apps-0.3.8/brainframe_apps/license_control.py
--rw-r--r--   0        0        0     6305 2023-04-08 06:28:34.341034 brainframe_apps-0.3.8/brainframe_apps/list_stream.py
--rw-r--r--   0        0        0     2903 2023-04-08 06:30:51.065666 brainframe_apps-0.3.8/brainframe_apps/logger_factory.py
--rw-r--r--   0        0        0     4455 2023-04-08 06:36:38.115275 brainframe_apps-0.3.8/brainframe_apps/process_image.py
--rw-r--r--   0        0        0     9547 2023-04-08 06:34:50.898778 brainframe_apps-0.3.8/brainframe_apps/set_configuration.py
--rw-r--r--   0        0        0     1797 2023-04-08 01:22:50.977592 brainframe_apps-0.3.8/brainframe_apps/settings.json
--rw-r--r--   0        0        0     3919 2023-04-08 06:36:09.515143 brainframe_apps-0.3.8/brainframe_apps/start_analyzing.py
--rw-r--r--   0        0        0     2153 2023-04-08 06:36:53.411347 brainframe_apps-0.3.8/brainframe_apps/stop_analyzing.py
--rw-r--r--   0        0        0     1046 2022-12-19 23:19:56.519826 brainframe_apps-0.3.8/brainframe_apps/time_utils.py
--rw-r--r--   0        0        0     3064 2023-04-08 06:32:28.746118 brainframe_apps-0.3.8/brainframe_apps/urls.py
--rw-r--r--   0        0        0     1037 2023-04-08 06:35:25.386938 brainframe_apps-0.3.8/brainframe_apps/wait_for_ready.py
--rw-r--r--   0        0        0     1701 2023-04-08 06:44:54.301585 brainframe_apps-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1777 1970-01-01 00:00:00.000000 brainframe_apps-0.3.8/setup.py
--rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 brainframe_apps-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      573 2023-04-08 04:43:59.581232 brainframe_apps-0.3.9/brainframe_apps/__init__.py
+-rw-r--r--   0        0        0     4817 2023-04-08 06:21:09.934999 brainframe_apps-0.3.9/brainframe_apps/add_stream.py
+-rw-r--r--   0        0        0      665 2022-12-19 23:19:56.515826 brainframe_apps-0.3.9/brainframe_apps/bf_log_print.py
+-rw-r--r--   0        0        0    15026 2023-04-08 06:35:37.058992 brainframe_apps-0.3.9/brainframe_apps/capsule_control.py
+-rw-r--r--   0        0        0      571 2023-04-08 04:43:59.581232 brainframe_apps-0.3.9/brainframe_apps/command_utils.py
+-rw-r--r--   0        0        0     2582 2023-04-08 06:39:20.092029 brainframe_apps-0.3.9/brainframe_apps/delete_stream.py
+-rw-r--r--   0        0        0     4691 2022-12-19 23:19:56.515826 brainframe_apps-0.3.9/brainframe_apps/fps_report.py
+-rw-r--r--   0        0        0     6343 2023-04-08 06:35:12.074876 brainframe_apps-0.3.9/brainframe_apps/get_configuration.py
+-rw-r--r--   0        0        0     8146 2023-04-08 06:35:51.659060 brainframe_apps-0.3.9/brainframe_apps/get_zone_statuses.py
+-rw-r--r--   0        0        0     4733 2023-04-08 06:36:26.419221 brainframe_apps-0.3.9/brainframe_apps/identity_control.py
+-rw-r--r--   0        0        0     2434 2023-04-08 06:34:33.690698 brainframe_apps-0.3.9/brainframe_apps/license_control.py
+-rw-r--r--   0        0        0     6305 2023-04-08 06:28:34.341034 brainframe_apps-0.3.9/brainframe_apps/list_stream.py
+-rw-r--r--   0        0        0     2903 2023-04-08 06:30:51.065666 brainframe_apps-0.3.9/brainframe_apps/logger_factory.py
+-rw-r--r--   0        0        0     4455 2023-04-08 06:36:38.115275 brainframe_apps-0.3.9/brainframe_apps/process_image.py
+-rw-r--r--   0        0        0     9547 2023-04-08 06:34:50.898778 brainframe_apps-0.3.9/brainframe_apps/set_configuration.py
+-rw-r--r--   0        0        0     1797 2023-04-08 01:22:50.977592 brainframe_apps-0.3.9/brainframe_apps/settings.json
+-rw-r--r--   0        0        0     3919 2023-04-08 06:36:09.515143 brainframe_apps-0.3.9/brainframe_apps/start_analyzing.py
+-rw-r--r--   0        0        0     2153 2023-04-08 06:36:53.411347 brainframe_apps-0.3.9/brainframe_apps/stop_analyzing.py
+-rw-r--r--   0        0        0     1046 2022-12-19 23:19:56.519826 brainframe_apps-0.3.9/brainframe_apps/time_utils.py
+-rw-r--r--   0        0        0     3064 2023-04-08 06:32:28.746118 brainframe_apps-0.3.9/brainframe_apps/urls.py
+-rw-r--r--   0        0        0     1037 2023-04-08 06:35:25.386938 brainframe_apps-0.3.9/brainframe_apps/wait_for_ready.py
+-rw-r--r--   0        0        0     1769 2023-04-08 06:47:48.126655 brainframe_apps-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 brainframe_apps-0.3.9/setup.py
+-rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 brainframe_apps-0.3.9/PKG-INFO
```

### Comparing `brainframe_apps-0.3.8/brainframe_apps/__init__.py` & `brainframe_apps-0.3.9/brainframe_apps/__init__.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.8/brainframe_apps/add_stream.py` & `brainframe_apps-0.3.9/brainframe_apps/add_stream.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.8/brainframe_apps/bf_log_print.py` & `brainframe_apps-0.3.9/brainframe_apps/bf_log_print.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.8/brainframe_apps/capsule_control.py` & `brainframe_apps-0.3.9/brainframe_apps/capsule_control.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.8/brainframe_apps/command_utils.py` & `brainframe_apps-0.3.9/brainframe_apps/command_utils.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.8/brainframe_apps/delete_stream.py` & `brainframe_apps-0.3.9/brainframe_apps/delete_stream.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.8/brainframe_apps/fps_report.py` & `brainframe_apps-0.3.9/brainframe_apps/fps_report.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.8/brainframe_apps/get_configuration.py` & `brainframe_apps-0.3.9/brainframe_apps/get_configuration.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.8/brainframe_apps/get_zone_statuses.py` & `brainframe_apps-0.3.9/brainframe_apps/get_zone_statuses.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.8/brainframe_apps/identity_control.py` & `brainframe_apps-0.3.9/brainframe_apps/identity_control.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.8/brainframe_apps/license_control.py` & `brainframe_apps-0.3.9/brainframe_apps/license_control.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.8/brainframe_apps/list_stream.py` & `brainframe_apps-0.3.9/brainframe_apps/list_stream.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.8/brainframe_apps/logger_factory.py` & `brainframe_apps-0.3.9/brainframe_apps/logger_factory.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.8/brainframe_apps/process_image.py` & `brainframe_apps-0.3.9/brainframe_apps/process_image.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.8/brainframe_apps/set_configuration.py` & `brainframe_apps-0.3.9/brainframe_apps/set_configuration.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.8/brainframe_apps/settings.json` & `brainframe_apps-0.3.9/brainframe_apps/settings.json`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.8/brainframe_apps/start_analyzing.py` & `brainframe_apps-0.3.9/brainframe_apps/start_analyzing.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.8/brainframe_apps/stop_analyzing.py` & `brainframe_apps-0.3.9/brainframe_apps/stop_analyzing.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.8/brainframe_apps/time_utils.py` & `brainframe_apps-0.3.9/brainframe_apps/time_utils.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.8/brainframe_apps/urls.py` & `brainframe_apps-0.3.9/brainframe_apps/urls.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.8/brainframe_apps/wait_for_ready.py` & `brainframe_apps-0.3.9/brainframe_apps/wait_for_ready.py`

 * *Files identical despite different names*

### Comparing `brainframe_apps-0.3.8/pyproject.toml` & `brainframe_apps-0.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brainframe-apps"
-version = "0.3.8"
+version = "0.3.9"
 description = "BrainFrame Apps use BrainFrame REST API to interact with the BrainFrame OS"
 authors = ["Stephen Li <stephen@dilililabs.com>"]
 license = "BSD License"
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -15,16 +15,17 @@
 brainframe-api = "^0.29.1"
 
 [tool.poetry.dev-dependencies]
 black = "^21.9b0"
 isort = "^5.9.3"
 
 [tool.poetry.scripts]
-add-stream                           = 'brainframe_apps.add_stream:main'
-brainframe-apps-add-stream           = 'brainframe_apps.add_stream:main'
+brainframe-apps                      = 'main'
+add-stream                           = 'brainframe_apps.add_stream:add_stream_main'
+brainframe-apps-add-stream           = 'brainframe_apps.add_stream:add_stream_main'
 
 delete-stream                        = 'brainframe_apps.delete_stream:main'
 brainframe-apps-delete-stream        = 'brainframe_apps.delete_stream:main'
 
 # list_stream
 
 load-settings                        = 'brainframe_apps.set:main'
```

### Comparing `brainframe_apps-0.3.8/setup.py` & `brainframe_apps-0.3.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['brainframe-api>=0.29.1,<0.30.0']
 
 entry_points = \
-{'console_scripts': ['add-stream = brainframe_apps.add_stream:main',
+{'console_scripts': ['add-stream = brainframe_apps.add_stream:add_stream_main',
+                     'brainframe-apps = main',
                      'brainframe-apps-add-stream = '
-                     'brainframe_apps.add_stream:main',
+                     'brainframe_apps.add_stream:add_stream_main',
                      'brainframe-apps-delete-stream = '
                      'brainframe_apps.delete_stream:main',
                      'brainframe-apps-get = brainframe_apps.get:main',
                      'brainframe-apps-set = brainframe_apps.set:main',
                      'brainframe-apps-start-analyzing = '
                      'brainframe_apps.start_analyzing:main',
                      'brainframe-apps-stop-analyzing = '
@@ -26,15 +27,15 @@
                      'load-settings = brainframe_apps.set:main',
                      'save-settings = brainframe_apps.get:main',
                      'start-analyzing = brainframe_apps.start_analyzing:main',
                      'stop-analyzing = brainframe_apps.stop_analyzing:main']}
 
 setup_kwargs = {
     'name': 'brainframe-apps',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'BrainFrame Apps use BrainFrame REST API to interact with the BrainFrame OS',
     'long_description': 'None',
     'author': 'Stephen Li',
     'author_email': 'stephen@dilililabs.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `brainframe_apps-0.3.8/PKG-INFO` & `brainframe_apps-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainframe-apps
-Version: 0.3.8
+Version: 0.3.9
 Summary: BrainFrame Apps use BrainFrame REST API to interact with the BrainFrame OS
 License: BSD License
 Author: Stephen Li
 Author-email: stephen@dilililabs.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
```

