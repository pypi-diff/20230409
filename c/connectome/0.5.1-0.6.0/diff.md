# Comparing `tmp/connectome-0.5.1.tar.gz` & `tmp/connectome-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectome-0.5.1.tar", last modified: Wed Mar 29 11:45:50 2023, max compression
+gzip compressed data, was "connectome-0.6.0.tar", last modified: Sun Apr  9 19:36:32 2023, max compression
```

## Comparing `connectome-0.5.1.tar` & `connectome-0.6.0.tar`

### file list

```diff
@@ -1,69 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:45:50.354613 connectome-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-03-29 11:45:46.000000 connectome-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-29 11:45:46.000000 connectome-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-03-29 11:45:50.354613 connectome-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-03-29 11:45:46.000000 connectome-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:45:50.346613 connectome-0.5.1/connectome/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:45:50.346613 connectome-0.5.1/connectome/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/cache/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/cache/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:45:50.346613 connectome-0.5.1/connectome/containers/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/containers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/containers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/containers/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/containers/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/containers/reversible.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:45:50.350613 connectome-0.5.1/connectome/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/engine/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/engine/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/engine/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/engine/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/engine/node_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/engine/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/engine/vm.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:45:50.350613 connectome-0.5.1/connectome/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/interface/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/interface/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/interface/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/interface/complex_edges.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/interface/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/interface/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/interface/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/interface/factory_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/interface/metaclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/interface/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/interface/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:45:50.354613 connectome-0.5.1/connectome/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/layers/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/layers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/layers/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/layers/columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/layers/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/layers/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/layers/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/layers/join.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/layers/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-03-29 11:45:46.000000 connectome-0.5.1/connectome/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 11:45:50.346613 connectome-0.5.1/connectome.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-03-29 11:45:50.000000 connectome-0.5.1/connectome.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-03-29 11:45:50.000000 connectome-0.5.1/connectome.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 11:45:50.000000 connectome-0.5.1/connectome.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-29 11:45:50.000000 connectome-0.5.1/connectome.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-29 11:45:50.000000 connectome-0.5.1/connectome.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-03-29 11:45:46.000000 connectome-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-29 11:45:46.000000 connectome-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 11:45:50.354613 connectome-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-03-29 11:45:46.000000 connectome-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:36:32.310780 connectome-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10763 2023-04-09 19:36:30.000000 connectome-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-09 19:36:30.000000 connectome-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-09 19:36:32.310780 connectome-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-09 19:36:30.000000 connectome-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:36:32.302780 connectome-0.6.0/connectome/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:36:32.306780 connectome-0.6.0/connectome/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/cache/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/cache/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:36:32.306780 connectome-0.6.0/connectome/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/containers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/containers/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/containers/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/containers/reversible.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:36:32.306780 connectome-0.6.0/connectome/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/engine/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/engine/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/engine/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/engine/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/engine/node_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/engine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/engine/vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:36:32.306780 connectome-0.6.0/connectome/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/complex_edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/factory_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/metaclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/interface/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:36:32.310780 connectome-0.6.0/connectome/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/layers/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-09 19:36:30.000000 connectome-0.6.0/connectome/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:36:32.306780 connectome-0.6.0/connectome.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-04-09 19:36:32.000000 connectome-0.6.0/connectome.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-09 19:36:32.000000 connectome-0.6.0/connectome.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 19:36:32.000000 connectome-0.6.0/connectome.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-09 19:36:32.000000 connectome-0.6.0/connectome.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 19:36:32.000000 connectome-0.6.0/connectome.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-09 19:36:30.000000 connectome-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-09 19:36:30.000000 connectome-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 19:36:32.310780 connectome-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-09 19:36:30.000000 connectome-0.6.0/setup.py
```

### Comparing `connectome-0.5.1/LICENSE` & `connectome-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connectome-0.5.1/PKG-INFO` & `connectome-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: connectome
-Version: 0.5.1
+Version: 0.6.0
 Summary: A library for datasets containing heterogeneous data
 Home-page: https://github.com/neuro-ml/connectome
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/connectome/archive/v0.5.1.tar.gz
+Download-URL: https://github.com/neuro-ml/connectome/archive/v0.6.0.tar.gz
 Keywords: dag,dataset,cache,consistency
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `connectome-0.5.1/README.md` & `connectome-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `connectome-0.5.1/connectome/cache/base.py` & `connectome-0.6.0/connectome/cache/base.py`

 * *Files identical despite different names*

### Comparing `connectome-0.5.1/connectome/containers/base.py` & `connectome-0.6.0/connectome/containers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ..engine import (
     BoundEdges, Details, FunctionEdge, GraphCompiler, IdentityEdge, Node, Nodes, NodeSet, ProductEdge, TreeNode
 )
 from ..engine.compiler import find_dependencies
 from ..exceptions import GraphError
 from ..utils import NameSet, StringsLike, check_for_duplicates, node_to_dict
-from .context import ChainContext, Context, NoContext, update_map, BagContext
+from .context import BagContext, ChainContext, Context, NoContext, update_map
 
 __all__ = 'Container', 'EdgesBag'
 
 logger = logging.getLogger(__name__)
 
 
 class Container:
```

### Comparing `connectome-0.5.1/connectome/containers/context.py` & `connectome-0.6.0/connectome/containers/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
-from typing import Tuple, AbstractSet, Dict
+from typing import AbstractSet, Dict, Tuple
 
-from ..engine import Node, Nodes, BoundEdges, IdentityEdge, Details, NodeSet
+from ..engine import BoundEdges, Details, IdentityEdge, Node, Nodes, NodeSet
 from ..utils import node_to_dict
 
 __all__ = 'Context', 'NoContext', 'IdentityContext', 'BagContext', 'ChainContext'
 
 
 class Context(ABC):
     @abstractmethod
```

### Comparing `connectome-0.5.1/connectome/containers/group.py` & `connectome-0.6.0/connectome/containers/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from collections import defaultdict
 from hashlib import sha256
-from typing import Sequence, Any, Generator
+from typing import Any, Generator, Sequence
 
-from .base import EdgesBag, Container
-from ..engine import NodeHash
-from ..engine import Node, TreeNode, NodeHashes, Command, Request, Response, Details
-from ..engine.edges import FunctionEdge, ProductEdge, StaticHash, StaticGraph, StaticEdge
+from ..engine import Command, Details, Node, NodeHash, NodeHashes, Request, Response, TreeNode
+from ..engine.edges import FunctionEdge, ProductEdge, StaticEdge, StaticGraph, StaticHash
 from ..engine.graph import Graph
-from ..engine.node_hash import LeafHash, CustomHash
+from ..engine.node_hash import CustomHash, LeafHash
+from .base import Container, EdgesBag
 
 
 class GroupContainer(Container):
     def __init__(self, name: str):
         self.name = name
 
     @staticmethod
```

### Comparing `connectome-0.5.1/connectome/containers/reversible.py` & `connectome-0.6.0/connectome/containers/reversible.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import defaultdict
-from typing import Tuple, Union, Iterable
+from typing import Iterable, Tuple, Union
 
-from ..engine import Nodes, BoundEdges, TreeNode
+from ..engine import BoundEdges, Nodes, TreeNode
 from ..engine.compiler import find_dependencies
 from ..exceptions import GraphError
-from ..utils import NameSet, node_to_dict, check_for_duplicates, AntiSet
+from ..utils import AntiSet, NameSet, check_for_duplicates, node_to_dict
 from .base import EdgesBag, normalize_bag
 from .context import BagContext
 
 
 class ReversibleContainer(EdgesBag):
     def __init__(self, inputs: Nodes, outputs: Nodes, edges: BoundEdges, backward_inputs: Nodes = (),
                  backward_outputs: Nodes = (), *, optional_inputs: NameSet = None, optional_outputs: NameSet = None,
```

### Comparing `connectome-0.5.1/connectome/engine/base.py` & `connectome-0.6.0/connectome/engine/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from enum import Enum
-from typing import Sequence, Tuple, Union, NamedTuple, Optional, Any, Generator, Collection, Iterable, Set, Dict, Type
+from typing import Any, Collection, Dict, Generator, Iterable, NamedTuple, Optional, Sequence, Set, Tuple, Type, Union
 
 from ..exceptions import GraphError
 from .node_hash import NodeHash, NodeHashes
 
 __all__ = (
     'Command', 'HashOutput', 'Request', 'Response', 'HashError',
     'Edge', 'Node', 'Nodes', 'NodeSet', 'BoundEdge', 'BoundEdges', 'TreeNode', 'TreeNodes', 'Details',
```

### Comparing `connectome-0.5.1/connectome/engine/compiler.py` & `connectome-0.6.0/connectome/engine/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from concurrent.futures import Executor
-from typing import Union, Tuple
+from typing import Tuple, Union
 
-from ..exceptions import FieldError, DependencyError
+from ..exceptions import DependencyError, FieldError
 from ..utils import NameSet, check_for_duplicates
-from .base import TreeNode, Nodes, BoundEdges, TreeNodes
+from .base import BoundEdges, Nodes, TreeNode, TreeNodes
 from .edges import ProductEdge
 from .graph import Graph
 
 
 class GraphCompiler:
     def __init__(self, inputs: Nodes, outputs: Nodes, edges: BoundEdges, virtuals: NameSet, optionals: Nodes,
                  executor: Executor):
```

### Comparing `connectome-0.5.1/connectome/engine/edges.py` & `connectome-0.6.0/connectome/engine/edges.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from abc import ABC, abstractmethod
-from typing import Sequence, Callable, Any, Generator, Tuple
+from typing import Any, Callable, Generator, Sequence, Tuple
 
-from .base import Edge, HashOutput, HashError, Request, Response
-from .node_hash import NodeHash, NodeHashes
+from .base import Edge, HashError, HashOutput, Request, Response
 from .graph import Command
-from .node_hash import LeafHash, ApplyHash
+from .node_hash import ApplyHash, LeafHash, NodeHash, NodeHashes
 
 __all__ = (
     'StaticHash', 'StaticGraph', 'StaticEdge',
     'ImpureEdge', 'CacheEdge', 'IdentityEdge', 'FunctionEdge', 'ComputableHashEdge',
     'ConstantEdge', 'ComputableHashBase', 'ProductEdge', 'HashBarrier',
 )
```

### Comparing `connectome-0.5.1/connectome/engine/executor.py` & `connectome-0.6.0/connectome/engine/executor.py`

 * *Files identical despite different names*

### Comparing `connectome-0.5.1/connectome/engine/graph.py` & `connectome-0.6.0/connectome/engine/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import inspect
 from collections import defaultdict
 from concurrent.futures import Executor
-from typing import Sequence, Any
+from typing import Any, Sequence
 
-from .base import TreeNode, NodeHash, TreeNodes, Command
+from .base import Command, TreeNode, TreeNodes
 from .executor import DefaultExecutor
-from .node_hash import LeafHash, GraphHash
+from .node_hash import GraphHash, LeafHash, NodeHash
 from .utils import EvictionCache
 from .vm import execute
 
 
 class Graph:
     def __init__(self, inputs: TreeNodes, output: TreeNode, executor: Executor = None):
         validate_graph(inputs, output)
```

### Comparing `connectome-0.5.1/connectome/engine/node_hash.py` & `connectome-0.6.0/connectome/engine/node_hash.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import warnings
-from typing import Sequence, Callable, Tuple, Any
+from typing import Any, Callable, Sequence, Tuple
 
 NODE_TYPES = set()
 
 
 class NodeHash:
     type: int
```

### Comparing `connectome-0.5.1/connectome/engine/utils.py` & `connectome-0.6.0/connectome/engine/utils.py`

 * *Files identical despite different names*

### Comparing `connectome-0.5.1/connectome/engine/vm.py` & `connectome-0.6.0/connectome/engine/vm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from concurrent.futures import Executor
 
 from .base import Command
-from .executor import Frame, AsyncLoop
+from .executor import AsyncLoop, Frame
 
 
 # TODO: replace cache by a thunk tree
 def execute(cmd, node, hashes, cache, executor: Executor):
     root = Frame([node], [(Command.Return,), (cmd,)])
     loop = AsyncLoop(root)
     push, pop, peek = loop.push, loop.pop, loop.peek
```

### Comparing `connectome-0.5.1/connectome/interface/blocks.py` & `connectome-0.6.0/connectome/interface/blocks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import operator
 
 from ..containers.base import EdgesBag
 from ..containers.group import GroupContainer, MultiGroupLayer
 from ..layers import *  # noqa
-from ..utils import deprecation_warn, StringsLike, to_seq  # noqa
+from ..utils import StringsLike, deprecation_warn, to_seq  # noqa
 
 
 class LegacyContainer(Layer):
     def __init__(self, container):
         deprecation_warn()
         self._container = container
```

### Comparing `connectome-0.5.1/connectome/interface/complex_edges.py` & `connectome-0.6.0/connectome/interface/complex_edges.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, Iterable
 
-from .edges import EdgeFactory, TypedEdge, Function, FunctionWrapper, FunctionBase
-from .nodes import Intermediate, Default, NodeTypes, NodeType
-from ..engine import Edge, ComputableHashEdge
+from ..engine import ComputableHashEdge, Edge
+from .edges import EdgeFactory, Function, FunctionBase, FunctionWrapper, TypedEdge
+from .nodes import Default, Intermediate, NodeType, NodeTypes
 
 
 class HashByValue(FunctionWrapper):
     def _wrap(self, edge: Edge, inputs: NodeTypes, output: NodeType) -> Iterable[TypedEdge]:
         yield TypedEdge(ComputableHashEdge(edge), inputs, output)
```

### Comparing `connectome-0.5.1/connectome/interface/edges.py` & `connectome-0.6.0/connectome/interface/edges.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import inspect
 from abc import ABC, abstractmethod
-from typing import Iterable, Callable, NamedTuple
+from typing import Callable, Iterable, NamedTuple
 
 from ..engine import Edge, FunctionEdge, ImpureEdge
 from ..exceptions import FieldError
 from .decorators import RuntimeAnnotation
-from .utils import replace_annotation
 from .nodes import *
+from .utils import replace_annotation
 
 __all__ = (
     'TypedEdge', 'EdgeFactory',
     'Function', 'FunctionWrapper', 'FunctionBase',
     'Inverse', 'inverse', 'Impure', 'impure', 'Positional', 'positional'
 )
```

### Comparing `connectome-0.5.1/connectome/interface/factory.py` & `connectome-0.6.0/connectome/interface/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import inspect
 import logging
 import warnings
-from typing import Dict, Any, Iterable, Callable, Type
+from typing import Any, Callable, Dict, Iterable, Type
 
+from ..containers import EdgesBag, ReversibleContainer
+from ..containers.reversible import normalize_inherit
+from ..engine import ConstantEdge, Details, IdentityEdge
+from ..exceptions import FieldError, GraphError
+from ..layers import CallableLayer, Layer
+from ..utils import AntiSet, MultiDict
 from .decorators import Meta, Optional, RuntimeAnnotation
 from .edges import EdgeFactory, Function
 from .factory_utils import add_quals, to_argument
 from .nodes import (
     NodeStorage, Input, InverseInput, Parameter, InverseOutput, Output, NodeTypes, NodeType, Default, Intermediate,
     FinalNodeType, is_private
 )
-from ..containers import EdgesBag, ReversibleContainer
-from ..containers.reversible import normalize_inherit
-from ..engine import IdentityEdge, ConstantEdge, Details
-from ..exceptions import GraphError, FieldError
-from ..utils import MultiDict, AntiSet
-from ..layers import Layer, CallableLayer
 
 logger = logging.getLogger(__name__)
 
 
 def add_from_mixins(namespace, mixins):
     # we have 2 scopes here:
     # 1. the `namespace`
```

### Comparing `connectome-0.5.1/connectome/interface/metaclasses.py` & `connectome-0.6.0/connectome/interface/metaclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import logging
-from typing import Callable, Dict, Type, Union, Iterable, Tuple, Collection
+from typing import Callable, Collection, Dict, Iterable, Tuple, Type, Union
 
+from ..layers import CallableLayer, Layer
 from ..utils import MultiDict
-from ..layers import Layer, CallableLayer
 from .compat import SafeMeta
-from .factory import (
-    SourceFactory, TransformFactory, add_from_mixins, add_quals, GraphFactory, items_to_container
-)
+from .factory import GraphFactory, SourceFactory, TransformFactory, add_from_mixins, add_quals, items_to_container
 
 logger = logging.getLogger(__name__)
 BASES: Dict[Type[Layer], GraphFactory] = {}
 
 
 class APIMeta(SafeMeta):
     @classmethod
```

### Comparing `connectome-0.5.1/connectome/interface/nodes.py` & `connectome-0.6.0/connectome/interface/nodes.py`

 * *Files identical despite different names*

### Comparing `connectome-0.5.1/connectome/interface/utils.py` & `connectome-0.6.0/connectome/interface/utils.py`

 * *Files identical despite different names*

### Comparing `connectome-0.5.1/connectome/layers/apply.py` & `connectome-0.6.0/connectome/layers/apply.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Callable
 
 from ..containers import ReversibleContainer
-from ..engine import Node, FunctionEdge, Details
+from ..engine import Details, FunctionEdge, Node
 from ..utils import AntiSet
 from .base import CallableLayer
 
 
 class Apply(CallableLayer):
     """
     A layer that applies separate functions to each of the specified names.
```

### Comparing `connectome-0.5.1/connectome/layers/base.py` & `connectome-0.6.0/connectome/layers/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import functools
 import logging
-import warnings
 from typing import Callable, Iterable
 
-from .chain import connect
 from ..containers.base import EdgesBag
 from ..engine import Details
 from ..exceptions import FieldError
 from ..interface.utils import format_arguments
 from ..utils import StringsLike
+from .chain import connect
 
 logger = logging.getLogger(__name__)
 
 
 class Layer:
     def _connect(self, previous: EdgesBag) -> EdgesBag:
         """
@@ -43,26 +42,15 @@
             raise AttributeError(name) from e
 
         if name in self._properties:
             return method()
         return method
 
     def _connect(self, previous: EdgesBag) -> EdgesBag:
-        if not hasattr(self._container, 'wrap'):
-            return connect(previous, self._container)
-
-        warnings.warn(
-            f'The method Container.wrap is deprecated and will be removed soon: {type(self._container).__name__}',
-            UserWarning
-        )
-        warnings.warn(
-            f'The method Container.wrap is deprecated and will be removed soon: {type(self._container).__name__}',
-            DeprecationWarning
-        )
-        return self._container.wrap(previous)
+        return connect(previous, self._container)
 
     def __rshift__(self, layer: Layer) -> 'Chain':
         return Chain(self, layer)
 
     def __call__(self, *args, **kwargs) -> 'Instance':
         return Instance(self, args, kwargs)
```

### Comparing `connectome-0.5.1/connectome/layers/cache.py` & `connectome-0.6.0/connectome/layers/cache.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,32 @@
-import warnings
 import weakref
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Union, Sequence, Container as ContainerType
+from typing import Container as ContainerType, Sequence, Union
 
 import numpy as np
-from tarn import RemoteStorage
-from tarn.cache import CacheIndex
-from tarn.config import init_storage, StorageConfig
+from tarn import DiskDict, HashKeyStorage, PickleKeyStorage
+from tarn.config import StorageConfig, init_storage
 
+from ..cache import Cache, DiskCache, MemoryCache
+from ..containers import EdgesBag, IdentityContext
+from ..engine import CacheEdge, Details, ImpureEdge, Node, TreeNode
+from ..serializers import ChainSerializer, JsonSerializer, NumpySerializer, PickleSerializer, Serializer
+from ..utils import AntiSet, PathLike, StringsLike, node_to_dict, to_seq
 from .base import Layer
 from .dynamic import DynamicConnectLayer
-from ..containers import EdgesBag, Container, IdentityContext
-from ..serializers import Serializer, ChainSerializer, JsonSerializer, NumpySerializer, PickleSerializer
-from ..storage import Storage, Disk
-from ..utils import PathLike, StringsLike, node_to_dict, to_seq, AntiSet
-from ..engine import TreeNode, Node, ImpureEdge, CacheEdge, Details
-from ..cache import Cache, MemoryCache, DiskCache
 
 PathLikes = Union[PathLike, Sequence[PathLike]]
-RemoteStorageLike = Union[RemoteStorage, Sequence[RemoteStorage]]
 SerializersLike = Union[Serializer, Sequence[Serializer]]
 
 
 class CacheLayer(Layer, ABC):
-    def __init__(self, container: Container = None):
-        # TODO: legacy
-        if container is not None:
-            warnings.warn('Passing a container to CacheLayer is deprecated', UserWarning)
-            warnings.warn('Passing a container to CacheLayer is deprecated', DeprecationWarning)
-
-        self._container = container
-
     def __repr__(self):
         return self.__class__.__name__
 
-    def _connect(self, previous: EdgesBag) -> EdgesBag:
-        if self._container is None:
-            raise NotImplementedError
-        # TODO: legacy
-        return self._container.wrap(previous)
-
 
 class CacheToStorage(DynamicConnectLayer, CacheLayer):
     def __init__(self, names: Union[ContainerType[str], None], impure: bool = False):
         super().__init__()
         if names is None:
             names = AntiSet()
         self.names = names
@@ -127,19 +109,19 @@
         field names that will be cached
     impure
         whether to allow caching of `impure` functions
     remote
         remote locations that are used to fetch the cache from (if available)
     """
 
-    def __init__(self, index: PathLikes, storage: Storage, serializer: SerializersLike, names: StringsLike, *,
-                 impure: bool = False, remote: RemoteStorageLike = ()):
-        names, local, remote = _normalize_disk_arguments(index, remote, names, serializer, storage)
+    def __init__(self, index: PathLikes, storage: HashKeyStorage, serializer: SerializersLike, names: StringsLike, *,
+                 impure: bool = False):
         super().__init__(names=names, impure=impure)
-        self.storage = DiskCache(local, remote, fetch=bool(remote))
+        names, serializer = _normalize_disk_arguments(names, serializer)
+        self.storage = DiskCache(PickleKeyStorage(index, storage, serializer))
 
     def _get_storage(self) -> Cache:
         return self.storage
 
     @classmethod
     def simple(cls, *names, root: PathLike, serializer: Union[Serializer, Sequence[Serializer]] = None):
         """
@@ -172,25 +154,18 @@
         if serializer is None:
             serializer = ChainSerializer(
                 JsonSerializer(),
                 NumpySerializer({np.bool_: 1, np.int_: 1}),
                 PickleSerializer(),
             )
 
-        return cls(index, Storage([Disk(storage)]), serializer, names)
+        return cls(index, HashKeyStorage(DiskDict(storage)), serializer, names)
 
 
-def _normalize_disk_arguments(local, remote, names, serializer, storage):
-    names = to_seq(names)
-    serializer = _resolve_serializer(serializer)
-    if isinstance(local, (str, Path)):
-        local = local,
-    if isinstance(remote, RemoteStorage):
-        remote = remote,
-    local = [CacheIndex(root, storage, serializer) for root in local]
-    return names, local, remote
+def _normalize_disk_arguments(names, serializer):
+    return to_seq(names), _resolve_serializer(serializer)
 
 
 def _resolve_serializer(serializer):
     if not isinstance(serializer, Serializer):
         serializer = ChainSerializer(*serializer)
     return serializer
```

### Comparing `connectome-0.5.1/connectome/layers/columns.py` & `connectome-0.6.0/connectome/layers/columns.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from itertools import starmap
 from math import ceil
-from typing import Union, Generator, Any
+from typing import Any, Generator, Union
 
+from tarn import HashKeyStorage, PickleKeyStorage
 from tqdm.auto import tqdm
 
-from .cache import CacheLayer, SerializersLike, PathLikes, RemoteStorageLike, _normalize_disk_arguments
-from .dynamic import DynamicConnectLayer
 from ..cache import DiskCache, MemoryCache
 from ..containers import EdgesBag, IdentityContext
-from ..engine import (
-    Edge, TreeNode, Node, Graph, Request, Response, HashOutput, Command, NodeHashes, NodeHash, Details
-)
+from ..engine import Command, Details, Edge, Graph, HashOutput, Node, NodeHash, NodeHashes, Request, Response, TreeNode
 from ..engine.node_hash import ApplyHash
 from ..exceptions import DependencyError
-from ..storage import Storage
-from ..utils import StringsLike, node_to_dict, AntiSet
+from ..utils import AntiSet, StringsLike, node_to_dict
+from .cache import CacheLayer, PathLikes, SerializersLike, _normalize_disk_arguments
+from .dynamic import DynamicConnectLayer
 
 
 class CacheColumns(DynamicConnectLayer, CacheLayer):
     """
     A combination of a persistent cache stored on disk and a memory cache.
     The entries are stored on disk in shards, which speeds up read/write operations for large numbers of small files.
 
@@ -38,24 +36,25 @@
         whether to show a progressbar during cache generation
     shard_size
         the size of a disk storage shard. If int - an absolute size value is used,
         if float - a portion relative to the dataset is used,
         if None - all the entries are grouped in a single shard
     """
 
-    def __init__(self, index: PathLikes, storage: Storage, serializer: SerializersLike, names: StringsLike, *,
-                 verbose: bool = False, shard_size: Union[int, float, None] = None, remote: RemoteStorageLike = ()):
+    def __init__(self, index: PathLikes, storage: HashKeyStorage, serializer: SerializersLike, names: StringsLike, *,
+                 verbose: bool = False, shard_size: Union[int, float, None] = None):
         if shard_size == 1:
             raise ValueError(f'Shard size of 1 is ambiguous. Use None if you want to have a single shard')
-        names, local, remote = _normalize_disk_arguments(index, remote, names, serializer, storage)
+        names, serializer = _normalize_disk_arguments(names, serializer)
+
         super().__init__()
         self.names = names
         self.shard_size = shard_size
         self.verbose = verbose
-        self.disk = DiskCache(local, remote, bool(remote))
+        self.disk = DiskCache(PickleKeyStorage(index, storage, serializer))
         self.ram = MemoryCache(None)
 
     def _prepare_container(self, previous: EdgesBag) -> EdgesBag:
         details = Details(type(self))
         copy = previous.freeze(details)
         mapping = TreeNode.from_edges(copy.edges)
         outputs_copy = node_to_dict(copy.outputs)
```

### Comparing `connectome-0.5.1/connectome/layers/debug.py` & `connectome-0.6.0/connectome/layers/debug.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import hashlib
-from typing import Generator, Any
+from typing import Any, Generator
 
 from tarn.cache.storage import key_to_digest
 
 from ..containers import EdgesBag
-from ..engine import Node, Request, Response, Command, StaticGraph, StaticHash, NodeHashes, NodeHash, Details
-from .cache import to_seq
+from ..engine import Command, Details, Node, NodeHash, NodeHashes, Request, Response, StaticGraph, StaticHash
 from ..utils import StringsLike
 from .base import CallableLayer
+from .cache import to_seq
 
 
 class HashDigest(CallableLayer):
     def __init__(self, names: StringsLike, algorithm):
         if isinstance(algorithm, str):
             algorithm = getattr(hashlib, algorithm)
```

### Comparing `connectome-0.5.1/connectome/layers/filter.py` & `connectome-0.6.0/connectome/layers/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Callable, Sequence, Any, Iterable
+from typing import Any, Callable, Iterable, Sequence
 
 from tqdm.auto import tqdm
 
 from ..containers import BagContext
-from ..engine import Node, TreeNode, Graph, FunctionEdge, StaticEdge, StaticGraph, Details
+from ..engine import Details, FunctionEdge, Graph, Node, StaticEdge, StaticGraph, TreeNode
 from ..engine.node_hash import ApplyHash
 from ..exceptions import DependencyError
-from ..utils import extract_signature, node_to_dict, AntiSet
+from ..utils import AntiSet, extract_signature, node_to_dict
 from .base import EdgesBag, Layer
 from .dynamic import DynamicConnectLayer
 
 
 class Filter(DynamicConnectLayer, Layer):
     """
     Filters the `keys` of the current pipeline given a `predicate`.
```

### Comparing `connectome-0.5.1/connectome/layers/join.py` & `connectome-0.6.0/connectome/layers/join.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import hashlib
 import itertools
 from collections import defaultdict
 from enum import Enum
-from typing import Generator, Any, Callable, Union, Sequence
+from typing import Any, Callable, Generator, Sequence, Union
 
 from jboc import composed
 from tqdm.auto import tqdm
 
-from .cache import MemoryCache
 from ..containers import EdgesBag
 from ..engine import (
     Request, Response, Command, Node, Edge, TreeNode, StaticGraph, StaticHash, FunctionEdge, ProductEdge, CacheEdge,
     Graph, HashOutput, NodeHashes, Details, IdentityEdge, NodeHash, LeafHash, CustomHash, HashBarrier
 )
-from ..interface.blocks import to_seq
 from ..layers import CallableLayer
-from ..utils import Strings, node_to_dict, StringsLike
+from ..utils import Strings, StringsLike, node_to_dict, to_seq
+from .cache import MemoryCache
 
 
 class JoinMode(Enum):
     inner, left, right, outer = 'inner', 'left', 'right', 'outer'
 
 
 def _maybe_to_hash_id(values):
```

### Comparing `connectome-0.5.1/connectome/layers/merge.py` & `connectome-0.6.0/connectome/layers/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Sequence, Any, Generator
+from typing import Any, Generator, Sequence
 
 from ..containers import EdgesBag
 from ..engine import (
     ConstantEdge, IdentityEdge, Node, NodeHash, Edge, NodeHashes, HashOutput, Request, Response, Command, Details,
     CustomHash,
 )
-from ..utils import node_to_dict
 from ..interface.utils import format_arguments
+from ..utils import node_to_dict
 from .base import CallableLayer
 
 
 class Merge(CallableLayer):
     def __init__(self, *layers: CallableLayer):
         properties = [set(layer._properties) for layer in layers]
         inter = set.intersection(*properties)
```

### Comparing `connectome-0.5.1/connectome/utils.py` & `connectome-0.6.0/connectome/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 import warnings
 from collections import Counter
 from pathlib import Path
-from typing import Union, Dict, List, Sequence, AbstractSet, Iterable
+from typing import AbstractSet, Dict, Iterable, List, Sequence, Union
 
 PathLike = Union[Path, str]
 Strings = Sequence[str]
 StringsLike = Union[str, Strings]
 NameSet = AbstractSet[str]
```

### Comparing `connectome-0.5.1/connectome.egg-info/PKG-INFO` & `connectome-0.6.0/connectome.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: connectome
-Version: 0.5.1
+Version: 0.6.0
 Summary: A library for datasets containing heterogeneous data
 Home-page: https://github.com/neuro-ml/connectome
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/connectome/archive/v0.5.1.tar.gz
+Download-URL: https://github.com/neuro-ml/connectome/archive/v0.6.0.tar.gz
 Keywords: dag,dataset,cache,consistency
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `connectome-0.5.1/connectome.egg-info/SOURCES.txt` & `connectome-0.6.0/connectome.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,42 +4,39 @@
 pyproject.toml
 requirements.txt
 setup.py
 connectome/__init__.py
 connectome/__version__.py
 connectome/exceptions.py
 connectome/serializers.py
-connectome/storage.py
 connectome/utils.py
 connectome.egg-info/PKG-INFO
 connectome.egg-info/SOURCES.txt
 connectome.egg-info/dependency_links.txt
 connectome.egg-info/requires.txt
 connectome.egg-info/top_level.txt
 connectome/cache/__init__.py
 connectome/cache/base.py
 connectome/cache/disk.py
 connectome/cache/memory.py
 connectome/containers/__init__.py
 connectome/containers/base.py
-connectome/containers/cache.py
 connectome/containers/context.py
 connectome/containers/group.py
 connectome/containers/reversible.py
 connectome/engine/__init__.py
 connectome/engine/base.py
 connectome/engine/compiler.py
 connectome/engine/edges.py
 connectome/engine/executor.py
 connectome/engine/graph.py
 connectome/engine/node_hash.py
 connectome/engine/utils.py
 connectome/engine/vm.py
 connectome/interface/__init__.py
-connectome/interface/base.py
 connectome/interface/blocks.py
 connectome/interface/compat.py
 connectome/interface/complex_edges.py
 connectome/interface/decorators.py
 connectome/interface/edges.py
 connectome/interface/factory.py
 connectome/interface/factory_utils.py
```

### Comparing `connectome-0.5.1/pyproject.toml` & `connectome-0.6.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -48,7 +48,12 @@
 ignore = ['W503', 'E203', 'B028']
 per-file-ignores = [
     '**/__init__.py:F401',
     'tests/*:I251',
 ]
 max-line-length = 120
 banned-modules = 'connectome.* = Use relative imports'
+
+[tool.isort]
+line_length = 120
+profile = 'black'
+combine_as_imports = true
```

### Comparing `connectome-0.5.1/setup.py` & `connectome-0.6.0/setup.py`

 * *Files identical despite different names*

