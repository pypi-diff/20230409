# Comparing `tmp/cdk8s-plus-25-2.6.8.tar.gz` & `tmp/cdk8s-plus-25-2.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-plus-25-2.6.8.tar", last modified: Wed Mar 22 13:41:52 2023, max compression
+gzip compressed data, was "cdk8s-plus-25-2.6.9.tar", last modified: Wed Mar 22 13:51:35 2023, max compression
```

## Comparing `cdk8s-plus-25-2.6.8.tar` & `cdk8s-plus-25-2.6.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:41:52.439226 cdk8s-plus-25-2.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-22 13:41:40.000000 cdk8s-plus-25-2.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-22 13:41:40.000000 cdk8s-plus-25-2.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-22 13:41:40.000000 cdk8s-plus-25-2.6.8/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-03-22 13:41:52.439226 cdk8s-plus-25-2.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-03-22 13:41:40.000000 cdk8s-plus-25-2.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-22 13:41:40.000000 cdk8s-plus-25-2.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 13:41:52.439226 cdk8s-plus-25-2.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-03-22 13:41:40.000000 cdk8s-plus-25-2.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:41:52.435227 cdk8s-plus-25-2.6.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:41:52.435227 cdk8s-plus-25-2.6.8/src/cdk8s_plus_25/
--rw-r--r--   0 runner    (1001) docker     (123)  1122587 2023-03-22 13:41:40.000000 cdk8s-plus-25-2.6.8/src/cdk8s_plus_25/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:41:52.435227 cdk8s-plus-25-2.6.8/src/cdk8s_plus_25/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-22 13:41:40.000000 cdk8s-plus-25-2.6.8/src/cdk8s_plus_25/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1262837 2023-03-22 13:41:40.000000 cdk8s-plus-25-2.6.8/src/cdk8s_plus_25/_jsii/cdk8s-plus-25@2.6.8.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:41:52.439226 cdk8s-plus-25-2.6.8/src/cdk8s_plus_25/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)  2644402 2023-03-22 13:41:40.000000 cdk8s-plus-25-2.6.8/src/cdk8s_plus_25/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 13:41:40.000000 cdk8s-plus-25-2.6.8/src/cdk8s_plus_25/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:41:52.435227 cdk8s-plus-25-2.6.8/src/cdk8s_plus_25.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-03-22 13:41:52.000000 cdk8s-plus-25-2.6.8/src/cdk8s_plus_25.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-22 13:41:52.000000 cdk8s-plus-25-2.6.8/src/cdk8s_plus_25.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 13:41:52.000000 cdk8s-plus-25-2.6.8/src/cdk8s_plus_25.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-22 13:41:52.000000 cdk8s-plus-25-2.6.8/src/cdk8s_plus_25.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-22 13:41:52.000000 cdk8s-plus-25-2.6.8/src/cdk8s_plus_25.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:51:35.044888 cdk8s-plus-25-2.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-22 13:51:20.000000 cdk8s-plus-25-2.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-22 13:51:20.000000 cdk8s-plus-25-2.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-22 13:51:20.000000 cdk8s-plus-25-2.6.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-03-22 13:51:35.044888 cdk8s-plus-25-2.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-03-22 13:51:20.000000 cdk8s-plus-25-2.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-22 13:51:20.000000 cdk8s-plus-25-2.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 13:51:35.044888 cdk8s-plus-25-2.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-03-22 13:51:20.000000 cdk8s-plus-25-2.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:51:35.036888 cdk8s-plus-25-2.6.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:51:35.036888 cdk8s-plus-25-2.6.9/src/cdk8s_plus_25/
+-rw-r--r--   0 runner    (1001) docker     (123)  1122587 2023-03-22 13:51:20.000000 cdk8s-plus-25-2.6.9/src/cdk8s_plus_25/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:51:35.040888 cdk8s-plus-25-2.6.9/src/cdk8s_plus_25/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-22 13:51:20.000000 cdk8s-plus-25-2.6.9/src/cdk8s_plus_25/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1262836 2023-03-22 13:51:20.000000 cdk8s-plus-25-2.6.9/src/cdk8s_plus_25/_jsii/cdk8s-plus-25@2.6.9.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:51:35.040888 cdk8s-plus-25-2.6.9/src/cdk8s_plus_25/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)  2644402 2023-03-22 13:51:20.000000 cdk8s-plus-25-2.6.9/src/cdk8s_plus_25/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 13:51:20.000000 cdk8s-plus-25-2.6.9/src/cdk8s_plus_25/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:51:35.040888 cdk8s-plus-25-2.6.9/src/cdk8s_plus_25.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-03-22 13:51:35.000000 cdk8s-plus-25-2.6.9/src/cdk8s_plus_25.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-22 13:51:35.000000 cdk8s-plus-25-2.6.9/src/cdk8s_plus_25.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 13:51:35.000000 cdk8s-plus-25-2.6.9/src/cdk8s_plus_25.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-22 13:51:35.000000 cdk8s-plus-25-2.6.9/src/cdk8s_plus_25.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-22 13:51:35.000000 cdk8s-plus-25-2.6.9/src/cdk8s_plus_25.egg-info/top_level.txt
```

### Comparing `cdk8s-plus-25-2.6.8/LICENSE` & `cdk8s-plus-25-2.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-25-2.6.8/PKG-INFO` & `cdk8s-plus-25-2.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-25
-Version: 2.6.8
+Version: 2.6.9
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-25 synthesizes Kubernetes manifests for Kubernetes 1.25.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-plus-25-2.6.8/README.md` & `cdk8s-plus-25-2.6.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-25-2.6.8/setup.py` & `cdk8s-plus-25-2.6.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-plus-25",
-    "version": "2.6.8",
+    "version": "2.6.9",
     "description": "cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-25 synthesizes Kubernetes manifests for Kubernetes 1.25.0",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-plus.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -23,24 +23,24 @@
     "packages": [
         "cdk8s_plus_25",
         "cdk8s_plus_25._jsii",
         "cdk8s_plus_25.k8s"
     ],
     "package_data": {
         "cdk8s_plus_25._jsii": [
-            "cdk8s-plus-25@2.6.8.jsii.tgz"
+            "cdk8s-plus-25@2.6.9.jsii.tgz"
         ],
         "cdk8s_plus_25": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdk8s>=2.7.39, <3.0.0",
-        "constructs>=10.1.284, <11.0.0",
+        "cdk8s>=2.7.41, <3.0.0",
+        "constructs>=10.1.286, <11.0.0",
         "jsii>=1.78.1, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `cdk8s-plus-25-2.6.8/src/cdk8s_plus_25/__init__.py` & `cdk8s-plus-25-2.6.9/src/cdk8s_plus_25/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-25-2.6.8/src/cdk8s_plus_25/k8s/__init__.py` & `cdk8s-plus-25-2.6.9/src/cdk8s_plus_25/k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-25-2.6.8/src/cdk8s_plus_25.egg-info/PKG-INFO` & `cdk8s-plus-25-2.6.9/src/cdk8s_plus_25.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-25
-Version: 2.6.8
+Version: 2.6.9
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-25 synthesizes Kubernetes manifests for Kubernetes 1.25.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

