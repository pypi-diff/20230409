# Comparing `tmp/cript-0.6.2.tar.gz` & `tmp/cript-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cript-0.6.2.tar", last modified: Wed Feb  8 00:24:31 2023, max compression
+gzip compressed data, was "cript-0.6.3.tar", last modified: Sat Apr  8 22:39:34 2023, max compression
```

## Comparing `cript-0.6.2.tar` & `cript-0.6.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:31.175169 cript-0.6.2/
--rw-rw-rw-   0        0        0     1079 2022-10-14 17:59:38.000000 cript-0.6.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2811 2023-02-08 00:24:31.175169 cript-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     2279 2023-02-08 00:21:48.000000 cript-0.6.2/README.md
--rw-rw-rw-   0        0        0      316 2023-02-07 23:16:13.000000 cript-0.6.2/pyproject.toml
--rw-rw-rw-   0        0        0      792 2023-02-08 00:24:31.175169 cript-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0       75 2023-02-07 23:16:13.000000 cript-0.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:31.048149 cript-0.6.2/src/
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:31.073459 cript-0.6.2/src/cript/
--rw-rw-rw-   0        0        0     1909 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:31.114596 cript-0.6.2/src/cript/api/
--rw-rw-rw-   0        0        0        0 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/api/__init__.py
--rw-rw-rw-   0        0        0      145 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/api/base.py
--rw-rw-rw-   0        0        0      983 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/api/exceptions.py
--rw-rw-rw-   0        0        0     6490 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/api/local.py
--rw-rw-rw-   0        0        0     5116 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/api/rest.py
--rw-rw-rw-   0        0        0     1354 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/api/utils.py
--rw-rw-rw-   0        0        0     1233 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/cache.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:31.114596 cript-0.6.2/src/cript/data_model/
--rw-rw-rw-   0        0        0     1542 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/__init__.py
--rw-rw-rw-   0        0        0     4756 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/base.py
--rw-rw-rw-   0        0        0     3010 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:31.151103 cript-0.6.2/src/cript/data_model/nodes/
--rw-rw-rw-   0        0        0        0 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/nodes/__init__.py
--rw-rw-rw-   0        0        0    10006 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/nodes/base_node.py
--rw-rw-rw-   0        0        0     2110 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/nodes/collection.py
--rw-rw-rw-   0        0        0     3483 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/nodes/computation.py
--rw-rw-rw-   0        0        0     4334 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/nodes/computational_process.py
--rw-rw-rw-   0        0        0     2737 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/nodes/data.py
--rw-rw-rw-   0        0        0     2692 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/nodes/experiment.py
--rw-rw-rw-   0        0        0     5390 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/nodes/file.py
--rw-rw-rw-   0        0        0      861 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/nodes/group.py
--rw-rw-rw-   0        0        0     3485 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/nodes/inventory.py
--rw-rw-rw-   0        0        0     2671 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/nodes/material.py
--rw-rw-rw-   0        0        0     4749 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/nodes/process.py
--rw-rw-rw-   0        0        0     1682 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/nodes/project.py
--rw-rw-rw-   0        0        0     3044 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/nodes/reference.py
--rw-rw-rw-   0        0        0      921 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/nodes/software.py
--rw-rw-rw-   0        0        0      844 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/nodes/user.py
--rw-rw-rw-   0        0        0     4146 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/paginator.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:31.159119 cript-0.6.2/src/cript/data_model/subobjects/
--rw-rw-rw-   0        0        0        0 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/subobjects/__init__.py
--rw-rw-rw-   0        0        0     1474 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/subobjects/algorithm.py
--rw-rw-rw-   0        0        0     2607 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/subobjects/base_subobject.py
--rw-rw-rw-   0        0        0      759 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/subobjects/citation.py
--rw-rw-rw-   0        0        0     1269 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/subobjects/computational_forcefield.py
--rw-rw-rw-   0        0        0     1499 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/subobjects/condition.py
--rw-rw-rw-   0        0        0     1074 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/subobjects/equipment.py
--rw-rw-rw-   0        0        0      575 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/subobjects/identifier.py
--rw-rw-rw-   0        0        0     1117 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/subobjects/ingredient.py
--rw-rw-rw-   0        0        0      627 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/subobjects/parameter.py
--rw-rw-rw-   0        0        0     3701 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/subobjects/property.py
--rw-rw-rw-   0        0        0      872 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/subobjects/quantity.py
--rw-rw-rw-   0        0        0     1644 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/data_model/subobjects/software_configuration.py
--rw-rw-rw-   0        0        0     2437 2023-02-08 00:21:48.000000 cript-0.6.2/src/cript/data_model/utils.py
--rw-rw-rw-   0        0        0       75 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:31.175169 cript-0.6.2/src/cript/storage_clients/
--rw-rw-rw-   0        0        0       66 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/storage_clients/__init__.py
--rw-rw-rw-   0        0        0      765 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/storage_clients/exceptions.py
--rw-rw-rw-   0        0        0     7982 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/storage_clients/globus.py
--rw-rw-rw-   0        0        0     3741 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/storage_clients/s3.py
--rw-rw-rw-   0        0        0     1320 2023-02-07 23:16:13.000000 cript-0.6.2/src/cript/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:31.095655 cript-0.6.2/src/cript.egg-info/
--rw-rw-rw-   0        0        0     2811 2023-02-08 00:24:31.000000 cript-0.6.2/src/cript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2020 2023-02-08 00:24:31.000000 cript-0.6.2/src/cript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-08 00:24:31.000000 cript-0.6.2/src/cript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-02-08 00:24:31.000000 cript-0.6.2/src/cript.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-02-08 00:24:31.000000 cript-0.6.2/src/cript.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-08 00:24:31.175169 cript-0.6.2/tests/
--rw-rw-rw-   0        0        0     9281 2023-02-07 23:16:13.000000 cript-0.6.2/tests/test_nodes.py
+drwxrwxrwx   0        0        0        0 2023-04-08 22:39:34.336094 cript-0.6.3/
+-rw-rw-rw-   0        0        0     1079 2022-10-14 17:59:38.000000 cript-0.6.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2811 2023-04-08 22:39:34.336094 cript-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2279 2023-04-08 22:37:47.000000 cript-0.6.3/README.md
+-rw-rw-rw-   0        0        0      316 2023-04-08 22:37:47.000000 cript-0.6.3/pyproject.toml
+-rw-rw-rw-   0        0        0      792 2023-04-08 22:39:34.341453 cript-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0       75 2023-04-08 22:37:47.000000 cript-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 22:39:33.374684 cript-0.6.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-08 22:39:33.473679 cript-0.6.3/src/cript/
+-rw-rw-rw-   0        0        0     1909 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-08 22:39:33.629993 cript-0.6.3/src/cript/api/
+-rw-rw-rw-   0        0        0        0 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/api/__init__.py
+-rw-rw-rw-   0        0        0      145 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/api/base.py
+-rw-rw-rw-   0        0        0      983 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/api/exceptions.py
+-rw-rw-rw-   0        0        0     6490 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/api/local.py
+-rw-rw-rw-   0        0        0     5116 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/api/rest.py
+-rw-rw-rw-   0        0        0     1354 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/api/utils.py
+-rw-rw-rw-   0        0        0     1233 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/cache.py
+drwxrwxrwx   0        0        0        0 2023-04-08 22:39:33.728916 cript-0.6.3/src/cript/data_model/
+-rw-rw-rw-   0        0        0     1542 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/__init__.py
+-rw-rw-rw-   0        0        0     4937 2023-04-08 22:37:52.000000 cript-0.6.3/src/cript/data_model/base.py
+-rw-rw-rw-   0        0        0     3010 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-08 22:39:34.048314 cript-0.6.3/src/cript/data_model/nodes/
+-rw-rw-rw-   0        0        0        0 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/nodes/__init__.py
+-rw-rw-rw-   0        0        0    10006 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/nodes/base_node.py
+-rw-rw-rw-   0        0        0     2110 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/nodes/collection.py
+-rw-rw-rw-   0        0        0     3483 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/nodes/computation.py
+-rw-rw-rw-   0        0        0     4334 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/nodes/computational_process.py
+-rw-rw-rw-   0        0        0     2737 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/nodes/data.py
+-rw-rw-rw-   0        0        0     2692 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/nodes/experiment.py
+-rw-rw-rw-   0        0        0     5390 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/nodes/file.py
+-rw-rw-rw-   0        0        0      861 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/nodes/group.py
+-rw-rw-rw-   0        0        0     3485 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/nodes/inventory.py
+-rw-rw-rw-   0        0        0     2671 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/nodes/material.py
+-rw-rw-rw-   0        0        0     4749 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/nodes/process.py
+-rw-rw-rw-   0        0        0     1682 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/nodes/project.py
+-rw-rw-rw-   0        0        0     3044 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/nodes/reference.py
+-rw-rw-rw-   0        0        0      921 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/nodes/software.py
+-rw-rw-rw-   0        0        0      844 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/nodes/user.py
+-rw-rw-rw-   0        0        0     4146 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/paginator.py
+drwxrwxrwx   0        0        0        0 2023-04-08 22:39:34.245733 cript-0.6.3/src/cript/data_model/subobjects/
+-rw-rw-rw-   0        0        0        0 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/subobjects/__init__.py
+-rw-rw-rw-   0        0        0     1474 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/subobjects/algorithm.py
+-rw-rw-rw-   0        0        0     2607 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/subobjects/base_subobject.py
+-rw-rw-rw-   0        0        0      759 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/subobjects/citation.py
+-rw-rw-rw-   0        0        0     1269 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/subobjects/computational_forcefield.py
+-rw-rw-rw-   0        0        0     1499 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/subobjects/condition.py
+-rw-rw-rw-   0        0        0     1074 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/subobjects/equipment.py
+-rw-rw-rw-   0        0        0      575 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/subobjects/identifier.py
+-rw-rw-rw-   0        0        0     1117 2023-04-08 22:37:52.000000 cript-0.6.3/src/cript/data_model/subobjects/ingredient.py
+-rw-rw-rw-   0        0        0      627 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/subobjects/parameter.py
+-rw-rw-rw-   0        0        0     3701 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/subobjects/property.py
+-rw-rw-rw-   0        0        0      872 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/subobjects/quantity.py
+-rw-rw-rw-   0        0        0     1644 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/subobjects/software_configuration.py
+-rw-rw-rw-   0        0        0     2437 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/data_model/utils.py
+-rw-rw-rw-   0        0        0       75 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-08 22:39:34.311894 cript-0.6.3/src/cript/storage_clients/
+-rw-rw-rw-   0        0        0       66 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/storage_clients/__init__.py
+-rw-rw-rw-   0        0        0      765 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/storage_clients/exceptions.py
+-rw-rw-rw-   0        0        0     7982 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/storage_clients/globus.py
+-rw-rw-rw-   0        0        0     3741 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/storage_clients/s3.py
+-rw-rw-rw-   0        0        0     1320 2023-04-08 22:37:47.000000 cript-0.6.3/src/cript/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-08 22:39:33.531206 cript-0.6.3/src/cript.egg-info/
+-rw-rw-rw-   0        0        0     2811 2023-04-08 22:39:33.000000 cript-0.6.3/src/cript.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2020 2023-04-08 22:39:33.000000 cript-0.6.3/src/cript.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 22:39:33.000000 cript-0.6.3/src/cript.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-08 22:39:33.000000 cript-0.6.3/src/cript.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-08 22:39:33.000000 cript-0.6.3/src/cript.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-08 22:39:34.328075 cript-0.6.3/tests/
+-rw-rw-rw-   0        0        0     9281 2023-04-08 22:37:47.000000 cript-0.6.3/tests/test_nodes.py
```

### Comparing `cript-0.6.2/LICENSE.txt` & `cript-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/PKG-INFO` & `cript-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cript
-Version: 0.6.2
+Version: 0.6.3
 Summary: CRIPT Python SDK
 Home-page: https://github.com/C-Accel-CRIPT/cript
 Author: CRIPT Development Team
 License: MIT
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `cript-0.6.2/README.md` & `cript-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/setup.cfg` & `cript-0.6.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 7269 7074 0d0a 7665 7273 696f   = cript..versio
-00000020: 6e20 3d20 302e 362e 320d 0a64 6573 6372  n = 0.6.2..descr
+00000020: 6e20 3d20 302e 362e 330d 0a64 6573 6372  n = 0.6.3..descr
 00000030: 6970 7469 6f6e 203d 2043 5249 5054 2050  iption = CRIPT P
 00000040: 7974 686f 6e20 5344 4b0d 0a6c 6f6e 675f  ython SDK..long_
 00000050: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 00000060: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
 00000070: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
 00000080: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
 00000090: 6578 742f 6d61 726b 646f 776e 0d0a 6175  ext/markdown..au
```

### Comparing `cript-0.6.2/src/cript/__init__.py` & `cript-0.6.3/src/cript/__init__.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/api/exceptions.py` & `cript-0.6.3/src/cript/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/api/local.py` & `cript-0.6.3/src/cript/api/local.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/api/rest.py` & `cript-0.6.3/src/cript/api/rest.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/api/utils.py` & `cript-0.6.3/src/cript/api/utils.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/cache.py` & `cript-0.6.3/src/cript/cache.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/__init__.py` & `cript-0.6.3/src/cript/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/base.py` & `cript-0.6.3/src/cript/data_model/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,17 +64,22 @@
 
         # Limit recursive node generation
         skip_nodes = False
         if level > get_level:
             skip_nodes = True
 
         node_dict = self.__dict__
+        fields_to_skip = {
+            "url",
+            "_Inventory__index_table",
+            "_Inventory__degenerate_index_table",
+        }
         for key, value in node_dict.items():
-            # Skip empty values and the url field
-            if not value or key == "url":
+            # Skip empty values and other fields that should be skipped
+            if not value or key in fields_to_skip:
                 continue
 
             # Generate nodes
             api = get_cached_api_session()
             if isinstance(value, str) and api.url in value and not skip_nodes:
                 # Check if node already exists in memory
                 local_node = get_cached_node(value)
```

### Comparing `cript-0.6.2/src/cript/data_model/exceptions.py` & `cript-0.6.3/src/cript/data_model/exceptions.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/nodes/base_node.py` & `cript-0.6.3/src/cript/data_model/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/nodes/collection.py` & `cript-0.6.3/src/cript/data_model/nodes/collection.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/nodes/computation.py` & `cript-0.6.3/src/cript/data_model/nodes/computation.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/nodes/computational_process.py` & `cript-0.6.3/src/cript/data_model/nodes/computational_process.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/nodes/data.py` & `cript-0.6.3/src/cript/data_model/nodes/data.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/nodes/experiment.py` & `cript-0.6.3/src/cript/data_model/nodes/experiment.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/nodes/file.py` & `cript-0.6.3/src/cript/data_model/nodes/file.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/nodes/group.py` & `cript-0.6.3/src/cript/data_model/nodes/group.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/nodes/inventory.py` & `cript-0.6.3/src/cript/data_model/nodes/inventory.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/nodes/material.py` & `cript-0.6.3/src/cript/data_model/nodes/material.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/nodes/process.py` & `cript-0.6.3/src/cript/data_model/nodes/process.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/nodes/project.py` & `cript-0.6.3/src/cript/data_model/nodes/project.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/nodes/reference.py` & `cript-0.6.3/src/cript/data_model/nodes/reference.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/nodes/software.py` & `cript-0.6.3/src/cript/data_model/nodes/software.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/nodes/user.py` & `cript-0.6.3/src/cript/data_model/nodes/user.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/paginator.py` & `cript-0.6.3/src/cript/data_model/paginator.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/subobjects/algorithm.py` & `cript-0.6.3/src/cript/data_model/subobjects/algorithm.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/subobjects/base_subobject.py` & `cript-0.6.3/src/cript/data_model/subobjects/base_subobject.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/subobjects/citation.py` & `cript-0.6.3/src/cript/data_model/subobjects/citation.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/subobjects/computational_forcefield.py` & `cript-0.6.3/src/cript/data_model/subobjects/computational_forcefield.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/subobjects/condition.py` & `cript-0.6.3/src/cript/data_model/subobjects/condition.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/subobjects/equipment.py` & `cript-0.6.3/src/cript/data_model/subobjects/equipment.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/subobjects/identifier.py` & `cript-0.6.3/src/cript/data_model/subobjects/identifier.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/subobjects/ingredient.py` & `cript-0.6.3/src/cript/data_model/subobjects/ingredient.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     node_name = "Ingredient"
     alt_names = ["ingredients"]
 
     @beartype
     def __init__(
         self,
         material: Union[Material, str],
-        keyword: str,
-        quantities: list[Union[Quantity, dict]] = None,
+        quantities: list[Union[Quantity, dict]],
+        keyword: str = None,
     ):
         super().__init__()
         self.material = material
         self.keyword = keyword
         self.quantities = quantities if quantities else []
 
     @beartype
```

### Comparing `cript-0.6.2/src/cript/data_model/subobjects/parameter.py` & `cript-0.6.3/src/cript/data_model/subobjects/parameter.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/subobjects/property.py` & `cript-0.6.3/src/cript/data_model/subobjects/property.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/subobjects/quantity.py` & `cript-0.6.3/src/cript/data_model/subobjects/quantity.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/subobjects/software_configuration.py` & `cript-0.6.3/src/cript/data_model/subobjects/software_configuration.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/data_model/utils.py` & `cript-0.6.3/src/cript/data_model/utils.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/storage_clients/exceptions.py` & `cript-0.6.3/src/cript/storage_clients/exceptions.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/storage_clients/globus.py` & `cript-0.6.3/src/cript/storage_clients/globus.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/storage_clients/s3.py` & `cript-0.6.3/src/cript/storage_clients/s3.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript/utils.py` & `cript-0.6.3/src/cript/utils.py`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/src/cript.egg-info/PKG-INFO` & `cript-0.6.3/src/cript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cript
-Version: 0.6.2
+Version: 0.6.3
 Summary: CRIPT Python SDK
 Home-page: https://github.com/C-Accel-CRIPT/cript
 Author: CRIPT Development Team
 License: MIT
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `cript-0.6.2/src/cript.egg-info/SOURCES.txt` & `cript-0.6.3/src/cript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cript-0.6.2/tests/test_nodes.py` & `cript-0.6.3/tests/test_nodes.py`

 * *Files identical despite different names*

