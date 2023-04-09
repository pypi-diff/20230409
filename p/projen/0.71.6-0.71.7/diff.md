# Comparing `tmp/projen-0.71.6.tar.gz` & `tmp/projen-0.71.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projen-0.71.6.tar", last modified: Sat Apr  8 00:45:47 2023, max compression
+gzip compressed data, was "projen-0.71.7.tar", last modified: Sun Apr  9 00:51:06 2023, max compression
```

## Comparing `projen-0.71.6.tar` & `projen-0.71.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.644019 projen-0.71.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-08 00:45:32.000000 projen-0.71.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-08 00:45:32.000000 projen-0.71.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    55403 2023-04-08 00:45:47.644019 projen-0.71.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    54524 2023-04-08 00:45:32.000000 projen-0.71.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-08 00:45:32.000000 projen-0.71.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 00:45:47.644019 projen-0.71.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-08 00:45:32.000000 projen-0.71.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.624019 projen-0.71.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.628019 projen-0.71.6/src/projen/
--rw-r--r--   0 runner    (1001) docker     (123)   579961 2023-04-08 00:45:32.000000 projen-0.71.6/src/projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.628019 projen-0.71.6/src/projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-08 00:45:32.000000 projen-0.71.6/src/projen/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.632019 projen-0.71.6/src/projen/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-08 00:45:32.000000 projen-0.71.6/src/projen/_jsii/bin/projen
--rw-r--r--   0 runner    (1001) docker     (123)  3351678 2023-04-08 00:45:32.000000 projen-0.71.6/src/projen/_jsii/projen@0.71.6.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.632019 projen-0.71.6/src/projen/awscdk/
--rw-r--r--   0 runner    (1001) docker     (123)  1032331 2023-04-08 00:45:32.000000 projen-0.71.6/src/projen/awscdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.636019 projen-0.71.6/src/projen/build/
--rw-r--r--   0 runner    (1001) docker     (123)    39873 2023-04-08 00:45:32.000000 projen-0.71.6/src/projen/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.636019 projen-0.71.6/src/projen/cdk/
--rw-r--r--   0 runner    (1001) docker     (123)   475626 2023-04-08 00:45:32.000000 projen-0.71.6/src/projen/cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.636019 projen-0.71.6/src/projen/cdk8s/
--rw-r--r--   0 runner    (1001) docker     (123)   569172 2023-04-08 00:45:32.000000 projen-0.71.6/src/projen/cdk8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.636019 projen-0.71.6/src/projen/cdktf/
--rw-r--r--   0 runner    (1001) docker     (123)   210643 2023-04-08 00:45:32.000000 projen-0.71.6/src/projen/cdktf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.636019 projen-0.71.6/src/projen/circleci/
--rw-r--r--   0 runner    (1001) docker     (123)    75837 2023-04-08 00:45:32.000000 projen-0.71.6/src/projen/circleci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.636019 projen-0.71.6/src/projen/github/
--rw-r--r--   0 runner    (1001) docker     (123)   275214 2023-04-08 00:45:32.000000 projen-0.71.6/src/projen/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.640020 projen-0.71.6/src/projen/github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)   235582 2023-04-08 00:45:32.000000 projen-0.71.6/src/projen/github/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.640020 projen-0.71.6/src/projen/gitlab/
--rw-r--r--   0 runner    (1001) docker     (123)   192753 2023-04-08 00:45:32.000000 projen-0.71.6/src/projen/gitlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.640020 projen-0.71.6/src/projen/java/
--rw-r--r--   0 runner    (1001) docker     (123)   174928 2023-04-08 00:45:32.000000 projen-0.71.6/src/projen/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.640020 projen-0.71.6/src/projen/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)   586576 2023-04-08 00:45:32.000000 projen-0.71.6/src/projen/javascript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 00:45:32.000000 projen-0.71.6/src/projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.640020 projen-0.71.6/src/projen/python/
--rw-r--r--   0 runner    (1001) docker     (123)   187110 2023-04-08 00:45:32.000000 projen-0.71.6/src/projen/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.640020 projen-0.71.6/src/projen/release/
--rw-r--r--   0 runner    (1001) docker     (123)   246151 2023-04-08 00:45:32.000000 projen-0.71.6/src/projen/release/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.640020 projen-0.71.6/src/projen/typescript/
--rw-r--r--   0 runner    (1001) docker     (123)   423478 2023-04-08 00:45:32.000000 projen-0.71.6/src/projen/typescript/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.644019 projen-0.71.6/src/projen/vscode/
--rw-r--r--   0 runner    (1001) docker     (123)    54316 2023-04-08 00:45:32.000000 projen-0.71.6/src/projen/vscode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.644019 projen-0.71.6/src/projen/web/
--rw-r--r--   0 runner    (1001) docker     (123)   745940 2023-04-08 00:45:32.000000 projen-0.71.6/src/projen/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:45:47.628019 projen-0.71.6/src/projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    55403 2023-04-08 00:45:47.000000 projen-0.71.6/src/projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-08 00:45:47.000000 projen-0.71.6/src/projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 00:45:47.000000 projen-0.71.6/src/projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-08 00:45:47.000000 projen-0.71.6/src/projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-08 00:45:47.000000 projen-0.71.6/src/projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.987647 projen-0.71.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-09 00:50:55.000000 projen-0.71.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-09 00:50:55.000000 projen-0.71.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    55403 2023-04-09 00:51:06.987647 projen-0.71.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    54524 2023-04-09 00:50:55.000000 projen-0.71.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-09 00:50:55.000000 projen-0.71.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 00:51:06.987647 projen-0.71.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-09 00:50:55.000000 projen-0.71.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.975647 projen-0.71.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.975647 projen-0.71.7/src/projen/
+-rw-r--r--   0 runner    (1001) docker     (123)   579961 2023-04-09 00:50:55.000000 projen-0.71.7/src/projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.975647 projen-0.71.7/src/projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-09 00:50:55.000000 projen-0.71.7/src/projen/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.979647 projen-0.71.7/src/projen/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-09 00:50:55.000000 projen-0.71.7/src/projen/_jsii/bin/projen
+-rw-r--r--   0 runner    (1001) docker     (123)  3351678 2023-04-09 00:50:55.000000 projen-0.71.7/src/projen/_jsii/projen@0.71.7.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.979647 projen-0.71.7/src/projen/awscdk/
+-rw-r--r--   0 runner    (1001) docker     (123)  1032331 2023-04-09 00:50:55.000000 projen-0.71.7/src/projen/awscdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.983647 projen-0.71.7/src/projen/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    39873 2023-04-09 00:50:55.000000 projen-0.71.7/src/projen/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.983647 projen-0.71.7/src/projen/cdk/
+-rw-r--r--   0 runner    (1001) docker     (123)   475626 2023-04-09 00:50:55.000000 projen-0.71.7/src/projen/cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.983647 projen-0.71.7/src/projen/cdk8s/
+-rw-r--r--   0 runner    (1001) docker     (123)   569172 2023-04-09 00:50:55.000000 projen-0.71.7/src/projen/cdk8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.983647 projen-0.71.7/src/projen/cdktf/
+-rw-r--r--   0 runner    (1001) docker     (123)   210643 2023-04-09 00:50:55.000000 projen-0.71.7/src/projen/cdktf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.983647 projen-0.71.7/src/projen/circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)    75837 2023-04-09 00:50:55.000000 projen-0.71.7/src/projen/circleci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.983647 projen-0.71.7/src/projen/github/
+-rw-r--r--   0 runner    (1001) docker     (123)   275214 2023-04-09 00:50:55.000000 projen-0.71.7/src/projen/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.983647 projen-0.71.7/src/projen/github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)   235582 2023-04-09 00:50:55.000000 projen-0.71.7/src/projen/github/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.983647 projen-0.71.7/src/projen/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (123)   192753 2023-04-09 00:50:55.000000 projen-0.71.7/src/projen/gitlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.983647 projen-0.71.7/src/projen/java/
+-rw-r--r--   0 runner    (1001) docker     (123)   174928 2023-04-09 00:50:55.000000 projen-0.71.7/src/projen/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.983647 projen-0.71.7/src/projen/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)   586576 2023-04-09 00:50:55.000000 projen-0.71.7/src/projen/javascript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 00:50:55.000000 projen-0.71.7/src/projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.987647 projen-0.71.7/src/projen/python/
+-rw-r--r--   0 runner    (1001) docker     (123)   187110 2023-04-09 00:50:55.000000 projen-0.71.7/src/projen/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.987647 projen-0.71.7/src/projen/release/
+-rw-r--r--   0 runner    (1001) docker     (123)   246151 2023-04-09 00:50:55.000000 projen-0.71.7/src/projen/release/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.987647 projen-0.71.7/src/projen/typescript/
+-rw-r--r--   0 runner    (1001) docker     (123)   423478 2023-04-09 00:50:55.000000 projen-0.71.7/src/projen/typescript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.987647 projen-0.71.7/src/projen/vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)    54316 2023-04-09 00:50:55.000000 projen-0.71.7/src/projen/vscode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.987647 projen-0.71.7/src/projen/web/
+-rw-r--r--   0 runner    (1001) docker     (123)   745940 2023-04-09 00:50:55.000000 projen-0.71.7/src/projen/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 00:51:06.975647 projen-0.71.7/src/projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    55403 2023-04-09 00:51:06.000000 projen-0.71.7/src/projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-09 00:51:06.000000 projen-0.71.7/src/projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 00:51:06.000000 projen-0.71.7/src/projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-09 00:51:06.000000 projen-0.71.7/src/projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-09 00:51:06.000000 projen-0.71.7/src/projen.egg-info/top_level.txt
```

### Comparing `projen-0.71.6/LICENSE` & `projen-0.71.7/LICENSE`

 * *Files identical despite different names*

### Comparing `projen-0.71.6/PKG-INFO` & `projen-0.71.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.71.6
+Version: 0.71.7
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.71.6/README.md` & `projen-0.71.7/README.md`

 * *Files identical despite different names*

### Comparing `projen-0.71.6/setup.py` & `projen-0.71.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "projen",
-    "version": "0.71.6",
+    "version": "0.71.7",
     "description": "CDK for software projects",
     "license": "Apache-2.0",
     "url": "https://github.com/projen/projen.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -38,15 +38,15 @@
         "projen.release",
         "projen.typescript",
         "projen.vscode",
         "projen.web"
     ],
     "package_data": {
         "projen._jsii": [
-            "projen@0.71.6.jsii.tgz"
+            "projen@0.71.7.jsii.tgz"
         ],
         "projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `projen-0.71.6/src/projen/__init__.py` & `projen-0.71.7/src/projen/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.6/src/projen/awscdk/__init__.py` & `projen-0.71.7/src/projen/awscdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.6/src/projen/build/__init__.py` & `projen-0.71.7/src/projen/build/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.6/src/projen/cdk/__init__.py` & `projen-0.71.7/src/projen/cdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.6/src/projen/cdk8s/__init__.py` & `projen-0.71.7/src/projen/cdk8s/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.6/src/projen/cdktf/__init__.py` & `projen-0.71.7/src/projen/cdktf/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.6/src/projen/circleci/__init__.py` & `projen-0.71.7/src/projen/circleci/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.6/src/projen/github/__init__.py` & `projen-0.71.7/src/projen/github/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.6/src/projen/github/workflows/__init__.py` & `projen-0.71.7/src/projen/github/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.6/src/projen/gitlab/__init__.py` & `projen-0.71.7/src/projen/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.6/src/projen/java/__init__.py` & `projen-0.71.7/src/projen/java/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.6/src/projen/javascript/__init__.py` & `projen-0.71.7/src/projen/javascript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.6/src/projen/python/__init__.py` & `projen-0.71.7/src/projen/python/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.6/src/projen/release/__init__.py` & `projen-0.71.7/src/projen/release/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.6/src/projen/typescript/__init__.py` & `projen-0.71.7/src/projen/typescript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.6/src/projen/vscode/__init__.py` & `projen-0.71.7/src/projen/vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.6/src/projen/web/__init__.py` & `projen-0.71.7/src/projen/web/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.6/src/projen.egg-info/PKG-INFO` & `projen-0.71.7/src/projen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.71.6
+Version: 0.71.7
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.71.6/src/projen.egg-info/SOURCES.txt` & `projen-0.71.7/src/projen.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/projen/py.typed
 src/projen.egg-info/PKG-INFO
 src/projen.egg-info/SOURCES.txt
 src/projen.egg-info/dependency_links.txt
 src/projen.egg-info/requires.txt
 src/projen.egg-info/top_level.txt
 src/projen/_jsii/__init__.py
-src/projen/_jsii/projen@0.71.6.jsii.tgz
+src/projen/_jsii/projen@0.71.7.jsii.tgz
 src/projen/_jsii/bin/projen
 src/projen/awscdk/__init__.py
 src/projen/build/__init__.py
 src/projen/cdk/__init__.py
 src/projen/cdk8s/__init__.py
 src/projen/cdktf/__init__.py
 src/projen/circleci/__init__.py
```

