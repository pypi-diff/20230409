# Comparing `tmp/knightswhosayni-0.1.0.tar.gz` & `tmp/knightswhosayni-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knightswhosayni-0.1.0.tar", last modified: Tue Mar 28 06:33:40 2023, max compression
+gzip compressed data, was "knightswhosayni-0.2.0.tar", last modified: Sun Apr  9 05:03:25 2023, max compression
```

## Comparing `knightswhosayni-0.1.0.tar` & `knightswhosayni-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 06:33:40.445091 knightswhosayni-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-03-28 06:33:40.445091 knightswhosayni-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 06:33:40.445091 knightswhosayni-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 06:33:40.441090 knightswhosayni-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 06:33:40.445091 knightswhosayni-0.1.0/src/knightswhosayni/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/src/knightswhosayni/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/src/knightswhosayni/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/src/knightswhosayni/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/src/knightswhosayni/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/src/knightswhosayni/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 06:33:40.445091 knightswhosayni-0.1.0/src/knightswhosayni/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/src/knightswhosayni/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/src/knightswhosayni/migrations/0002_auto_20230307_0633.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/src/knightswhosayni/migrations/0003_project_module_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/src/knightswhosayni/migrations/0004_sale.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/src/knightswhosayni/migrations/0005_sale_license.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/src/knightswhosayni/migrations/0006_auto_20230321_0442.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/src/knightswhosayni/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/src/knightswhosayni/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/src/knightswhosayni/template_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/src/knightswhosayni/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/src/knightswhosayni/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/src/knightswhosayni/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 06:33:40.445091 knightswhosayni-0.1.0/src/knightswhosayni.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-03-28 06:33:40.000000 knightswhosayni-0.1.0/src/knightswhosayni.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-03-28 06:33:40.000000 knightswhosayni-0.1.0/src/knightswhosayni.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 06:33:40.000000 knightswhosayni-0.1.0/src/knightswhosayni.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-28 06:33:40.000000 knightswhosayni-0.1.0/src/knightswhosayni.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-28 06:33:40.000000 knightswhosayni-0.1.0/src/knightswhosayni.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-28 06:33:40.000000 knightswhosayni-0.1.0/src/knightswhosayni.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 06:33:40.445091 knightswhosayni-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-28 06:33:06.000000 knightswhosayni-0.1.0/tests/test_knightswhosayni.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 05:03:25.156582 knightswhosayni-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-04-09 05:03:25.152582 knightswhosayni-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 05:03:25.156582 knightswhosayni-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 05:03:25.148582 knightswhosayni-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 05:03:25.152582 knightswhosayni-0.2.0/src/knightswhosayni/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/src/knightswhosayni/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/src/knightswhosayni/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/src/knightswhosayni/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/src/knightswhosayni/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/src/knightswhosayni/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 05:03:25.152582 knightswhosayni-0.2.0/src/knightswhosayni/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/src/knightswhosayni/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/src/knightswhosayni/migrations/0002_auto_20230307_0633.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/src/knightswhosayni/migrations/0003_project_module_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/src/knightswhosayni/migrations/0004_sale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/src/knightswhosayni/migrations/0005_sale_license.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/src/knightswhosayni/migrations/0006_auto_20230321_0442.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/src/knightswhosayni/migrations/0007_project_logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/src/knightswhosayni/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/src/knightswhosayni/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/src/knightswhosayni/template_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/src/knightswhosayni/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/src/knightswhosayni/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/src/knightswhosayni/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 05:03:25.152582 knightswhosayni-0.2.0/src/knightswhosayni.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-04-09 05:03:25.000000 knightswhosayni-0.2.0/src/knightswhosayni.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-09 05:03:25.000000 knightswhosayni-0.2.0/src/knightswhosayni.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 05:03:25.000000 knightswhosayni-0.2.0/src/knightswhosayni.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-09 05:03:25.000000 knightswhosayni-0.2.0/src/knightswhosayni.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-09 05:03:25.000000 knightswhosayni-0.2.0/src/knightswhosayni.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-09 05:03:25.000000 knightswhosayni-0.2.0/src/knightswhosayni.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 05:03:25.152582 knightswhosayni-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-09 05:02:51.000000 knightswhosayni-0.2.0/tests/test_knightswhosayni.py
```

### Comparing `knightswhosayni-0.1.0/LICENSE` & `knightswhosayni-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `knightswhosayni-0.1.0/PKG-INFO` & `knightswhosayni-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knightswhosayni
-Version: 0.1.0
+Version: 0.2.0
 Summary: Ni! Ni! Ni!
 Author-email: Grant Jenks <contact@grantjenks.com>
 License: Apache 2.0
 Project-URL: Documentation, https://grantjenks.com/docs/knightswhosayni/
 Project-URL: Funding, https://gum.co/knightswhosayni
 Project-URL: Source, https://github.com/grantjenks/knights-who-say-ni
 Project-URL: Tracker, https://github.com/grantjenks/knights-who-say-ni/issues
```

### Comparing `knightswhosayni-0.1.0/README.rst` & `knightswhosayni-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `knightswhosayni-0.1.0/pyproject.toml` & `knightswhosayni-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
-dependencies = ["Django", "requests"]
+dependencies = ["Django", "Pillow", "requests"]
 dynamic = ["version"]
 
 [project.scripts]
 knightswhosayni = "knightswhosayni.main:main"
 
 [project.urls]
 Documentation = "https://grantjenks.com/docs/knightswhosayni/"
```

### Comparing `knightswhosayni-0.1.0/src/knightswhosayni/admin.py` & `knightswhosayni-0.2.0/src/knightswhosayni/admin.py`

 * *Files identical despite different names*

### Comparing `knightswhosayni-0.1.0/src/knightswhosayni/main.py` & `knightswhosayni-0.2.0/src/knightswhosayni/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 {'message': 'The resource_subscription '
             'was deleted successfully.',
  'success': True}
 
 
 TODO
 
-* Support customization of the project logo.
-
 * Add license legal details to template.
 
 * Provide reusable GitHub workflow for testing and releasing code.
+
+* Add some tests and stamp it v1
 """
 
 import argparse
 import base64
 import functools
 import hashlib
 import itertools
```

### Comparing `knightswhosayni-0.1.0/src/knightswhosayni/migrations/0001_initial.py` & `knightswhosayni-0.2.0/src/knightswhosayni/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `knightswhosayni-0.1.0/src/knightswhosayni/migrations/0002_auto_20230307_0633.py` & `knightswhosayni-0.2.0/src/knightswhosayni/migrations/0002_auto_20230307_0633.py`

 * *Files identical despite different names*

### Comparing `knightswhosayni-0.1.0/src/knightswhosayni/migrations/0004_sale.py` & `knightswhosayni-0.2.0/src/knightswhosayni/migrations/0004_sale.py`

 * *Files identical despite different names*

### Comparing `knightswhosayni-0.1.0/src/knightswhosayni/migrations/0005_sale_license.py` & `knightswhosayni-0.2.0/src/knightswhosayni/migrations/0005_sale_license.py`

 * *Files identical despite different names*

### Comparing `knightswhosayni-0.1.0/src/knightswhosayni/migrations/0006_auto_20230321_0442.py` & `knightswhosayni-0.2.0/src/knightswhosayni/migrations/0006_auto_20230321_0442.py`

 * *Files identical despite different names*

### Comparing `knightswhosayni-0.1.0/src/knightswhosayni/models.py` & `knightswhosayni-0.2.0/src/knightswhosayni/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     create_time = models.DateTimeField(auto_now_add=True)
     modify_time = models.DateTimeField(auto_now=True)
     name = models.CharField(max_length=100)
     slug = models.CharField(max_length=100)
     module_name = models.CharField(max_length=100)
     contact_name = models.CharField(max_length=100)
     contact_email = models.CharField(max_length=100)
+    logo = models.ImageField(blank=True, null=True, upload_to='logos')
 
     def __str__(self):
         return self.name
 
 
 class Key(models.Model):
     create_time = models.DateTimeField(auto_now_add=True)
```

### Comparing `knightswhosayni-0.1.0/src/knightswhosayni/template_init.py` & `knightswhosayni-0.2.0/src/knightswhosayni/template_init.py`

 * *Files identical despite different names*

### Comparing `knightswhosayni-0.1.0/src/knightswhosayni/utils.py` & `knightswhosayni-0.2.0/src/knightswhosayni/utils.py`

 * *Files identical despite different names*

### Comparing `knightswhosayni-0.1.0/src/knightswhosayni/views.py` & `knightswhosayni-0.2.0/src/knightswhosayni/views.py`

 * *Files identical despite different names*

### Comparing `knightswhosayni-0.1.0/src/knightswhosayni.egg-info/PKG-INFO` & `knightswhosayni-0.2.0/src/knightswhosayni.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knightswhosayni
-Version: 0.1.0
+Version: 0.2.0
 Summary: Ni! Ni! Ni!
 Author-email: Grant Jenks <contact@grantjenks.com>
 License: Apache 2.0
 Project-URL: Documentation, https://grantjenks.com/docs/knightswhosayni/
 Project-URL: Funding, https://gum.co/knightswhosayni
 Project-URL: Source, https://github.com/grantjenks/knights-who-say-ni
 Project-URL: Tracker, https://github.com/grantjenks/knights-who-say-ni/issues
```

### Comparing `knightswhosayni-0.1.0/src/knightswhosayni.egg-info/SOURCES.txt` & `knightswhosayni-0.2.0/src/knightswhosayni.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -20,9 +20,10 @@
 src/knightswhosayni.egg-info/top_level.txt
 src/knightswhosayni/migrations/0001_initial.py
 src/knightswhosayni/migrations/0002_auto_20230307_0633.py
 src/knightswhosayni/migrations/0003_project_module_name.py
 src/knightswhosayni/migrations/0004_sale.py
 src/knightswhosayni/migrations/0005_sale_license.py
 src/knightswhosayni/migrations/0006_auto_20230321_0442.py
+src/knightswhosayni/migrations/0007_project_logo.py
 src/knightswhosayni/migrations/__init__.py
 tests/test_knightswhosayni.py
```

### Comparing `knightswhosayni-0.1.0/tests/test_knightswhosayni.py` & `knightswhosayni-0.2.0/tests/test_knightswhosayni.py`

 * *Files identical despite different names*

