# Comparing `tmp/adaptix-3.0.0a2.tar.gz` & `tmp/adaptix-3.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptix-3.0.0a2.tar", last modified: Sun Apr  2 22:38:21 2023, max compression
+gzip compressed data, was "adaptix-3.0.0a3.tar", last modified: Sun Apr  9 16:52:08 2023, max compression
```

## Comparing `adaptix-3.0.0a2.tar` & `adaptix-3.0.0a3.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-02 22:38:21.370280 adaptix-3.0.0a2/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    11357 2021-06-13 21:15:36.000000 adaptix-3.0.0a2/LICENSE
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2830 2023-04-02 22:38:21.370280 adaptix-3.0.0a2/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2232 2023-02-18 09:38:02.000000 adaptix-3.0.0a2/README.md
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1440 2023-04-02 22:36:55.000000 adaptix-3.0.0a2/pyproject.toml
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       38 2023-04-02 22:38:21.370280 adaptix-3.0.0a2/setup.cfg
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-02 22:38:21.362280 adaptix-3.0.0a2/src/
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-02 22:38:21.366279 adaptix-3.0.0a2/src/adaptix/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1499 2023-04-02 22:24:55.000000 adaptix-3.0.0a2/src/adaptix/__init__.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-02 22:38:21.366279 adaptix-3.0.0a2/src/adaptix/_internal/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/__init__.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-02 22:38:21.366279 adaptix-3.0.0a2/src/adaptix/_internal/code_tools/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      313 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/code_tools/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2252 2023-03-11 08:07:13.000000 adaptix-3.0.0a2/src/adaptix/_internal/code_tools/code_builder.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1517 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/code_tools/compiler.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      559 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/code_tools/context_namespace.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1586 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/code_tools/prefix_mangler.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2206 2023-03-03 19:55:26.000000 adaptix-3.0.0a2/src/adaptix/_internal/code_tools/utils.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      573 2023-02-24 21:22:09.000000 adaptix-3.0.0a2/src/adaptix/_internal/common.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-02 22:38:21.366279 adaptix-3.0.0a2/src/adaptix/_internal/facade/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      283 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/facade/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    11128 2023-04-02 19:56:21.000000 adaptix-3.0.0a2/src/adaptix/_internal/facade/provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7574 2023-04-02 19:56:52.000000 adaptix-3.0.0a2/src/adaptix/_internal/facade/retort.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1845 2023-04-02 21:56:31.000000 adaptix-3.0.0a2/src/adaptix/_internal/feature_requirement.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1349 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/load_error.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-02 22:38:21.366279 adaptix-3.0.0a2/src/adaptix/_internal/model_tools/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      673 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/model_tools/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7831 2023-03-12 10:02:27.000000 adaptix-3.0.0a2/src/adaptix/_internal/model_tools/definitions.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    14337 2023-03-12 10:02:22.000000 adaptix-3.0.0a2/src/adaptix/_internal/model_tools/introspection.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-02 22:38:21.366279 adaptix-3.0.0a2/src/adaptix/_internal/provider/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2201 2023-04-02 22:23:58.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    10567 2023-04-02 22:23:58.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/concrete_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2355 2023-03-03 19:55:26.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/essential.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    21567 2023-04-02 22:23:58.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/generic_provider.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-02 22:38:21.366279 adaptix-3.0.0a2/src/adaptix/_internal/provider/model/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1316 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/model/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7716 2023-03-12 06:49:43.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/model/basic_gen.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4287 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/model/crown_definitions.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      883 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/model/definitions.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     6667 2023-03-24 07:52:20.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/model/dumper_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5609 2023-03-24 20:20:12.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/model/figure_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2145 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/model/input_creation_gen.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    14884 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/model/input_extraction_gen.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     8056 2023-03-24 20:56:07.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/model/loader_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    10405 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/model/output_creation_gen.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     9932 2023-03-11 08:07:13.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/model/output_extraction_gen.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      610 2023-03-28 18:27:05.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/model/request_filtering.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-02 22:38:21.370280 adaptix-3.0.0a2/src/adaptix/_internal/provider/name_layout/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      240 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/name_layout/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2013 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/name_layout/base.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    13397 2023-03-24 07:52:20.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/name_layout/component.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     5010 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/name_layout/crown_builder.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2907 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/name_layout/provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2862 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/name_style.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4238 2023-03-24 20:55:51.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/overlay_schema.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3897 2023-03-21 22:13:56.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/provider_basics.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2731 2023-04-02 22:30:42.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/provider_template.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1400 2023-03-10 23:07:49.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/request_cls.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    11507 2023-04-02 22:22:57.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/request_filtering.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     6191 2023-03-21 22:13:56.000000 adaptix-3.0.0a2/src/adaptix/_internal/provider/static_provider.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-02 22:38:21.370280 adaptix-3.0.0a2/src/adaptix/_internal/retort/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      319 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/retort/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3217 2023-03-21 22:13:56.000000 adaptix-3.0.0a2/src/adaptix/_internal/retort/base_retort.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7332 2023-03-21 22:13:56.000000 adaptix-3.0.0a2/src/adaptix/_internal/retort/mediator.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1541 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/retort/operating_retort.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     4066 2023-03-03 19:55:26.000000 adaptix-3.0.0a2/src/adaptix/_internal/struct_path.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-02 22:38:21.370280 adaptix-3.0.0a2/src/adaptix/_internal/type_tools/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      382 2023-03-11 08:07:13.000000 adaptix-3.0.0a2/src/adaptix/_internal/type_tools/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2878 2023-03-11 21:00:18.000000 adaptix-3.0.0a2/src/adaptix/_internal/type_tools/basic_utils.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2918 2023-03-12 10:01:39.000000 adaptix-3.0.0a2/src/adaptix/_internal/type_tools/generic_resolver.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2206 2023-03-21 22:13:56.000000 adaptix-3.0.0a2/src/adaptix/_internal/type_tools/implicit_params.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      633 2023-03-11 08:07:13.000000 adaptix-3.0.0a2/src/adaptix/_internal/type_tools/norm_utils.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    20603 2023-03-11 20:52:01.000000 adaptix-3.0.0a2/src/adaptix/_internal/type_tools/normalize_type.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7307 2023-04-02 21:48:08.000000 adaptix-3.0.0a2/src/adaptix/_internal/utils.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      648 2023-03-04 08:02:22.000000 adaptix-3.0.0a2/src/adaptix/load_error.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-02 22:38:21.370280 adaptix-3.0.0a2/src/adaptix/provider/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1058 2023-04-02 22:24:29.000000 adaptix-3.0.0a2/src/adaptix/provider/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      163 2023-03-03 19:55:26.000000 adaptix-3.0.0a2/src/adaptix/provider/static_provider.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2023-02-18 14:53:08.000000 adaptix-3.0.0a2/src/adaptix/py.typed
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      167 2023-03-03 19:55:26.000000 adaptix-3.0.0a2/src/adaptix/retort.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      441 2023-03-03 19:55:26.000000 adaptix-3.0.0a2/src/adaptix/struct_path.py
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-02 22:38:21.366279 adaptix-3.0.0a2/src/adaptix.egg-info/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     2830 2023-04-02 22:38:21.000000 adaptix-3.0.0a2/src/adaptix.egg-info/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3092 2023-04-02 22:38:21.000000 adaptix-3.0.0a2/src/adaptix.egg-info/SOURCES.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-04-02 22:38:21.000000 adaptix-3.0.0a2/src/adaptix.egg-info/dependency_links.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        8 2023-04-02 22:38:21.000000 adaptix-3.0.0a2/src/adaptix.egg-info/top_level.txt
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.111447 adaptix-3.0.0a3/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    11357 2021-06-13 21:15:36.000000 adaptix-3.0.0a3/LICENSE
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4466 2023-04-09 16:52:08.111447 adaptix-3.0.0a3/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3076 2023-04-09 16:47:10.000000 adaptix-3.0.0a3/README.md
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2153 2023-04-09 16:45:47.000000 adaptix-3.0.0a3/pyproject.toml
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       38 2023-04-09 16:52:08.111447 adaptix-3.0.0a3/setup.cfg
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.091447 adaptix-3.0.0a3/src/
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.095447 adaptix-3.0.0a3/src/adaptix/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1541 2023-04-08 09:30:44.000000 adaptix-3.0.0a3/src/adaptix/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.099447 adaptix-3.0.0a3/src/adaptix/_internal/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/__init__.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.099447 adaptix-3.0.0a3/src/adaptix/_internal/code_tools/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      313 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/code_tools/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2252 2023-03-11 08:07:13.000000 adaptix-3.0.0a3/src/adaptix/_internal/code_tools/code_builder.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1517 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/code_tools/compiler.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      559 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/code_tools/context_namespace.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1586 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/code_tools/prefix_mangler.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2206 2023-03-03 19:55:26.000000 adaptix-3.0.0a3/src/adaptix/_internal/code_tools/utils.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      573 2023-02-24 21:22:09.000000 adaptix-3.0.0a3/src/adaptix/_internal/common.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.099447 adaptix-3.0.0a3/src/adaptix/_internal/facade/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      283 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/facade/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    11128 2023-04-02 19:56:21.000000 adaptix-3.0.0a3/src/adaptix/_internal/facade/provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7574 2023-04-05 08:41:54.000000 adaptix-3.0.0a3/src/adaptix/_internal/facade/retort.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1845 2023-04-02 21:56:31.000000 adaptix-3.0.0a3/src/adaptix/_internal/feature_requirement.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1349 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/load_error.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.099447 adaptix-3.0.0a3/src/adaptix/_internal/model_tools/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      673 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/model_tools/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7831 2023-03-12 10:02:27.000000 adaptix-3.0.0a3/src/adaptix/_internal/model_tools/definitions.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    14421 2023-04-08 14:50:16.000000 adaptix-3.0.0a3/src/adaptix/_internal/model_tools/introspection.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.103447 adaptix-3.0.0a3/src/adaptix/_internal/provider/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2201 2023-04-02 22:23:58.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    10588 2023-04-04 21:35:50.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/concrete_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2355 2023-03-03 19:55:26.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/essential.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    21566 2023-04-08 10:27:34.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/generic_provider.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.107447 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1316 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7716 2023-03-12 06:49:43.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/basic_gen.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4287 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/crown_definitions.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      883 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/definitions.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     6667 2023-03-24 07:52:20.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/dumper_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5609 2023-03-24 20:20:12.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/figure_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2145 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/input_creation_gen.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    14884 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/input_extraction_gen.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     8056 2023-03-24 20:56:07.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/loader_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    10405 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/output_creation_gen.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     9932 2023-03-11 08:07:13.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/output_extraction_gen.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      610 2023-03-28 18:27:05.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/model/request_filtering.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.107447 adaptix-3.0.0a3/src/adaptix/_internal/provider/name_layout/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      240 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/name_layout/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2013 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/name_layout/base.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    13397 2023-03-24 07:52:20.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/name_layout/component.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     5010 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/name_layout/crown_builder.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2907 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/name_layout/provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2862 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/name_style.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4238 2023-03-24 20:55:51.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/overlay_schema.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3897 2023-03-21 22:13:56.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/provider_basics.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2731 2023-04-02 22:30:42.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/provider_template.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1400 2023-03-10 23:07:49.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/request_cls.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    12026 2023-04-08 10:12:42.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/request_filtering.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     6191 2023-03-21 22:13:56.000000 adaptix-3.0.0a3/src/adaptix/_internal/provider/static_provider.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.111447 adaptix-3.0.0a3/src/adaptix/_internal/retort/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      319 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/retort/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3217 2023-03-21 22:13:56.000000 adaptix-3.0.0a3/src/adaptix/_internal/retort/base_retort.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7318 2023-04-04 19:15:15.000000 adaptix-3.0.0a3/src/adaptix/_internal/retort/mediator.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1541 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/retort/operating_retort.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4066 2023-03-03 19:55:26.000000 adaptix-3.0.0a3/src/adaptix/_internal/struct_path.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.111447 adaptix-3.0.0a3/src/adaptix/_internal/type_tools/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      382 2023-03-11 08:07:13.000000 adaptix-3.0.0a3/src/adaptix/_internal/type_tools/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2878 2023-03-11 21:00:18.000000 adaptix-3.0.0a3/src/adaptix/_internal/type_tools/basic_utils.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2918 2023-03-12 10:01:39.000000 adaptix-3.0.0a3/src/adaptix/_internal/type_tools/generic_resolver.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     2206 2023-03-21 22:13:56.000000 adaptix-3.0.0a3/src/adaptix/_internal/type_tools/implicit_params.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      557 2023-04-04 19:15:15.000000 adaptix-3.0.0a3/src/adaptix/_internal/type_tools/norm_utils.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    20650 2023-04-08 16:16:31.000000 adaptix-3.0.0a3/src/adaptix/_internal/type_tools/normalize_type.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7307 2023-04-02 21:48:08.000000 adaptix-3.0.0a3/src/adaptix/_internal/utils.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      648 2023-03-04 08:02:22.000000 adaptix-3.0.0a3/src/adaptix/load_error.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.111447 adaptix-3.0.0a3/src/adaptix/provider/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1096 2023-04-07 22:37:17.000000 adaptix-3.0.0a3/src/adaptix/provider/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      163 2023-03-03 19:55:26.000000 adaptix-3.0.0a3/src/adaptix/provider/static_provider.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        0 2023-02-18 14:53:08.000000 adaptix-3.0.0a3/src/adaptix/py.typed
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      167 2023-03-03 19:55:26.000000 adaptix-3.0.0a3/src/adaptix/retort.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      441 2023-03-03 19:55:26.000000 adaptix-3.0.0a3/src/adaptix/struct_path.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2023-04-09 16:52:08.099447 adaptix-3.0.0a3/src/adaptix.egg-info/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4466 2023-04-09 16:52:08.000000 adaptix-3.0.0a3/src/adaptix.egg-info/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3092 2023-04-09 16:52:08.000000 adaptix-3.0.0a3/src/adaptix.egg-info/SOURCES.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2023-04-09 16:52:08.000000 adaptix-3.0.0a3/src/adaptix.egg-info/dependency_links.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        8 2023-04-09 16:52:08.000000 adaptix-3.0.0a3/src/adaptix.egg-info/top_level.txt
```

### Comparing `adaptix-3.0.0a2/LICENSE` & `adaptix-3.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/__init__.py` & `adaptix-3.0.0a3/src/adaptix/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     ExtraOut,
     ExtraSkip,
     Mediator,
     NameStyle,
     P,
     Provider,
     Request,
+    RequestPattern,
     Saturator,
     create_request_checker,
 )
 from .retort import NoSuitableProvider
 
 __all__ = (
     'Dumper',
@@ -68,14 +69,15 @@
     'ExtraForbid',
     'ExtraIn',
     'ExtraKwargs',
     'ExtraOut',
     'ExtraSkip',
     'Mediator',
     'NameStyle',
+    'RequestPattern',
     'P',
     'Saturator',
     'create_request_checker',
     'retort',
     'Provider',
     'NoSuitableProvider',
     'Request',
```

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/code_tools/code_builder.py` & `adaptix-3.0.0a3/src/adaptix/_internal/code_tools/code_builder.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/code_tools/compiler.py` & `adaptix-3.0.0a3/src/adaptix/_internal/code_tools/compiler.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/code_tools/context_namespace.py` & `adaptix-3.0.0a3/src/adaptix/_internal/code_tools/context_namespace.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/code_tools/prefix_mangler.py` & `adaptix-3.0.0a3/src/adaptix/_internal/code_tools/prefix_mangler.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/code_tools/utils.py` & `adaptix-3.0.0a3/src/adaptix/_internal/code_tools/utils.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/common.py` & `adaptix-3.0.0a3/src/adaptix/_internal/common.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/facade/provider.py` & `adaptix-3.0.0a3/src/adaptix/_internal/facade/provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/facade/retort.py` & `adaptix-3.0.0a3/src/adaptix/_internal/facade/retort.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/feature_requirement.py` & `adaptix-3.0.0a3/src/adaptix/_internal/feature_requirement.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/load_error.py` & `adaptix-3.0.0a3/src/adaptix/_internal/load_error.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/model_tools/__init__.py` & `adaptix-3.0.0a3/src/adaptix/_internal/model_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/model_tools/definitions.py` & `adaptix-3.0.0a3/src/adaptix/_internal/model_tools/definitions.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/model_tools/introspection.py` & `adaptix-3.0.0a3/src/adaptix/_internal/model_tools/introspection.py`

 * *Files 3% similar despite different names*

```diff
@@ -340,34 +340,34 @@
     )
 
 # =================
 #       Attrs
 # =================
 
 
-def _get_attrs_default(field) -> Default:
-    default: Any = field.default
+def _get_attrs_default(attrs_field) -> Default:
+    default: Any = attrs_field.default
 
     if isinstance(default, attrs.Factory):  # type: ignore
         if default.takes_self:
             # TODO: add support
             raise ValueError("Factory with self parameter does not supported yet")
         return DefaultFactory(default.factory)
 
     if default is attrs.NOTHING:
         return NoDefault()
 
     return DefaultValue(default)
 
 
-def _get_attrs_field_type(field, type_hints):
+def _get_attrs_field_type(attrs_field, type_hints):
     try:
-        return type_hints[field.name]
+        return type_hints[attrs_field.name]
     except KeyError:
-        return Any if field.type is None else field.type
+        return Any if attrs_field.type is None else attrs_field.type
 
 
 NoneType = type(None)
 
 
 def _process_attr_input_field(
     field: InputField,
@@ -394,19 +394,21 @@
             field.default
         ),
         metadata=base_field.metadata,
         name=base_field.name,
     )
 
 
-def _get_attr_param_name(field):
+def _get_attrs_param_name(attrs_field):
+    if hasattr(attrs_field, 'alias'):
+        return attrs_field.alias
     return (
-        field.name[1:]
-        if field.name.startswith("_") and not field.name.startswith("__") else
-        field.name
+        attrs_field.name[1:]
+        if attrs_field.name.startswith("_") and not attrs_field.name.startswith("__") else
+        attrs_field.name
     )
 
 
 def get_attrs_figure(tp) -> FullFigure:
     if not HAS_ATTRS_PKG:
         raise NoTargetPackage
 
@@ -424,25 +426,22 @@
     except (TypeError, attrs.exceptions.NotAnAttrsClassError):
         raise IntrospectionImpossible
 
     attrs_fields_dict = {
         field.name: field for field in attrs_fields
     }
     param_name_to_base_field = {
-        _get_attr_param_name(field): field
-        for field in (
-            BaseField(
-                # if field is not annotated, type attribute will store None value
-                type=_get_attrs_field_type(field, type_hints),
-                default=_get_attrs_default(field),
-                metadata=field.metadata,
-                name=field.name,
-            )
-            for field in attrs_fields
+        _get_attrs_param_name(attrs_fld): BaseField(
+            # if field is not annotated, type attribute will store None value
+            type=_get_attrs_field_type(attrs_fld, type_hints),
+            default=_get_attrs_default(attrs_fld),
+            metadata=attrs_fld.metadata,
+            name=attrs_fld.name,
         )
+        for attrs_fld in attrs_fields
     }
 
     has_custom_init = hasattr(tp, '__attrs_init__')
 
     figure = get_class_init_figure(tp)
     input_fields = tuple(
         _process_attr_input_field(field, param_name_to_base_field, has_custom_init)
```

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/__init__.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/concrete_provider.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/concrete_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     _OK_TYPES = (int, float, Decimal)
 
     def _provide_loader(self, mediator: Mediator, request: LoaderRequest) -> Loader:
         ok_types = self._OK_TYPES
 
         def timedelta_loader(data):
             if type(data) not in ok_types:
-                raise TypeLoadError(float)
+                raise TypeLoadError(Union[int, float, Decimal])
             return timedelta(seconds=int(data), microseconds=int(data % 1 * 10 ** 6))
 
         return timedelta_loader
 
     def _provide_dumper(self, mediator: Mediator, request: DumperRequest) -> Dumper:
         return timedelta.total_seconds
```

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/essential.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/essential.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/generic_provider.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/generic_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -523,15 +523,14 @@
 
     def _make_dumper(self, key_dumper: Dumper, value_dumper: Dumper, debug_path: bool):
         if debug_path:
             return self._get_dumper_dp(
                 key_dumper=key_dumper,
                 value_dumper=value_dumper,
             )
-
         return self._get_dumper_non_dp(
             key_dumper=key_dumper,
             value_dumper=value_dumper,
         )
 
     def _get_dumper_dp(self, key_dumper, value_dumper):
         def dict_dumper_dp(data: Mapping):
```

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/model/__init__.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/__init__.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/model/basic_gen.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/basic_gen.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/model/crown_definitions.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/crown_definitions.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/model/definitions.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/definitions.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/model/dumper_provider.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/dumper_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/model/figure_provider.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/figure_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/model/input_creation_gen.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/input_creation_gen.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/model/input_extraction_gen.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/input_extraction_gen.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/model/loader_provider.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/loader_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/model/output_creation_gen.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/output_creation_gen.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/model/output_extraction_gen.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/output_extraction_gen.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/model/request_filtering.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/model/request_filtering.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/name_layout/base.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/name_layout/base.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/name_layout/component.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/name_layout/component.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/name_layout/crown_builder.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/name_layout/crown_builder.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/name_layout/provider.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/name_layout/provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/name_style.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/name_style.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/overlay_schema.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/overlay_schema.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/provider_basics.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/provider_basics.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/provider_template.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/provider_template.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/request_cls.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/request_cls.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/request_filtering.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/request_filtering.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from inspect import isabstract
 from typing import Any, ClassVar, Iterable, Optional, Pattern, Protocol, Sequence, Tuple, Type, TypeVar, Union
 
 from ..common import TypeHint, VarTuple
 from ..type_tools import BaseNormType, NormTV, is_parametrized, is_protocol, is_subclass_soft, normalize_type
 from ..type_tools.normalize_type import NotSubscribedError
 from .essential import CannotProvide, Mediator, Provider, Request
-from .request_cls import FieldLoc, LocatedRequest, Location, TypeHintLoc
+from .request_cls import FieldLoc, GenericParamLoc, LocatedRequest, Location, TypeHintLoc
 
 T = TypeVar('T')
 
 
 class DirectMediator(Protocol):
     """This is copy of Mediator protocol but without provide_from_next() method"""
 
@@ -235,14 +235,25 @@
         for i, (checker, stack_request) in enumerate(zip(self.request_checkers, stack[offset:]), start=0):
             checker.check_request(
                 RequestStackCutter(mediator, i),
                 stack_request,
             )
 
 
+@dataclass
+class GenericParamRC(LocatedRequestChecker):
+    LOCATION = GenericParamLoc
+    pos: int
+
+    def _check_location(self, mediator: DirectMediator, loc: GenericParamLoc) -> None:
+        if loc.pos == self.pos:
+            return
+        raise CannotProvide(f'Generic param position {loc.pos} must be equal to {self.pos}')
+
+
 class AnyRequestChecker(RequestChecker):
     def check_request(self, mediator: DirectMediator, request: Request) -> None:
         return
 
 
 Pred = Union[str, re.Pattern, type, TypeHint, RequestChecker, 'RequestPattern']
 
@@ -276,20 +287,20 @@
         return ExactOriginRC(pred)
     except ValueError:
         raise ValueError(f'Can not create RequestChecker from {pred}')
 
     if isinstance(norm, NormTV):
         raise ValueError(f'Can not create RequestChecker from {pred} type var')
 
-    if not is_parametrized(pred):
-        if is_protocol(norm.origin) or isabstract(norm.origin):
-            return OriginSubclassRC(norm.origin)
-        return ExactOriginRC(norm.origin)
+    if is_parametrized(pred):
+        return ExactTypeRC(norm)
 
-    return ExactTypeRC(norm)
+    if is_protocol(norm.origin) or isabstract(norm.origin):
+        return OriginSubclassRC(norm.origin)
+    return ExactOriginRC(norm.origin)
 
 
 Pat = TypeVar('Pat', bound='RequestPattern')
 
 
 class RequestPattern:
     def __init__(self, stack: VarTuple[RequestChecker]):
@@ -308,15 +319,15 @@
         if item.startswith('__') and item.endswith('__'):
             raise AttributeError
         return self[item]
 
     def __getitem__(self: Pat, item: Union[Pred, VarTuple[Pred]]) -> Pat:
         if isinstance(item, tuple):
             return self._extend_stack(
-                [OrRequestChecker(self._ensure_request_checker(el) for el in item)]
+                [OrRequestChecker([self._ensure_request_checker(el) for el in item])]
             )
         return self._extend_stack([self._ensure_request_checker(item)])
 
     def __or__(self: Pat, other: Pat) -> Pat:
         return self._from_rc(
             self.build_request_checker() | other.build_request_checker()
         )
@@ -344,14 +355,19 @@
             raise TypeError(
                 "Can not use RequestPattern as predicate inside RequestPattern."
                 " If you want to combine several RequestPattern, you can use `+` operator"
             )
 
         return create_request_checker(pred)
 
+    def generic_arg(self: Pat, pos: int, pred: Pred) -> Pat:
+        return self._extend_stack(
+            [GenericParamRC(pos) & self._ensure_request_checker(pred)]
+        )
+
     def build_request_checker(self) -> RequestChecker:
         if len(self._stack) == 1:
             return self._stack[0]
         return StackEndRC(self._stack)
 
 
 P = RequestPattern(stack=())
```

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/provider/static_provider.py` & `adaptix-3.0.0a3/src/adaptix/_internal/provider/static_provider.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/retort/base_retort.py` & `adaptix-3.0.0a3/src/adaptix/_internal/retort/base_retort.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/retort/mediator.py` & `adaptix-3.0.0a3/src/adaptix/_internal/retort/mediator.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         if combiner.has_elements():
             result.extend(combiner.combine_elements())
         return result
 
     def _collect_candidates(self, request_cls: Type[Request], recipe: Sequence[Provider]) -> Sequence[Provider]:
         candidates = [
             provider
-            for i, provider in enumerate(recipe)
+            for provider in recipe
             if (
                 not isinstance(provider, RequestClassDeterminedProvider)
                 or provider.maybe_can_process_request_cls(request_cls)
             )
         ]
         return self._merge_providers(candidates)
```

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/retort/operating_retort.py` & `adaptix-3.0.0a3/src/adaptix/_internal/retort/operating_retort.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/struct_path.py` & `adaptix-3.0.0a3/src/adaptix/_internal/struct_path.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/type_tools/basic_utils.py` & `adaptix-3.0.0a3/src/adaptix/_internal/type_tools/basic_utils.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/type_tools/generic_resolver.py` & `adaptix-3.0.0a3/src/adaptix/_internal/type_tools/generic_resolver.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/type_tools/implicit_params.py` & `adaptix-3.0.0a3/src/adaptix/_internal/type_tools/implicit_params.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/type_tools/norm_utils.py` & `adaptix-3.0.0a3/src/adaptix/_internal/type_tools/norm_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 # pylint: disable=import-outside-toplevel
 import typing
 from dataclasses import InitVar
 from typing import ClassVar, Final
 
-from ..feature_requirement import HAS_ANNOTATED, HAS_TYPE_GUARD
+from ..feature_requirement import HAS_ANNOTATED
 from .normalize_type import BaseNormType
 
 _TYPE_TAGS = [Final, ClassVar, InitVar]
 
 if HAS_ANNOTATED:
     _TYPE_TAGS.append(typing.Annotated)
 
-if HAS_TYPE_GUARD:
-    _TYPE_TAGS.append(typing.TypeGuard)
-
 
 def strip_tags(norm: BaseNormType) -> BaseNormType:
     """Removes type hints that does not represent type
     and that only indicates metadata
     """
     if norm.origin in _TYPE_TAGS:
         return strip_tags(norm.args[0])
```

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/type_tools/normalize_type.py` & `adaptix-3.0.0a3/src/adaptix/_internal/type_tools/normalize_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,21 +197,21 @@
 
 
 @dataclass
 class Constraints:
     value: VarTuple[BaseNormType]
 
 
-TVLimit = Union[Bound, Constraints]
+TypeVarLimit = Union[Bound, Constraints]  # pylint: disable=invalid-name
 
 
 class NormTV(BaseNormType):
     __slots__ = ('_var', '_limit', '_variance', '_source')
 
-    def __init__(self, var: Any, limit: TVLimit, *, source: TypeHint):
+    def __init__(self, var: Any, limit: TypeVarLimit, *, source: TypeHint):
         self._var = var
         self._source = source
         self._limit = limit
 
         if var.__covariant__:
             self._variance = Variance.COVARIANT
         if var.__contravariant__:
@@ -235,15 +235,15 @@
         return self._var.__name__
 
     @property
     def variance(self) -> Variance:
         return self._variance
 
     @property
-    def limit(self) -> TVLimit:
+    def limit(self) -> TypeVarLimit:
         return self._limit
 
     def __repr__(self):
         return f'<{type(self).__name__}({self._var})>'
 
     def __hash__(self):
         return hash(self._var)
```

### Comparing `adaptix-3.0.0a2/src/adaptix/_internal/utils.py` & `adaptix-3.0.0a3/src/adaptix/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/load_error.py` & `adaptix-3.0.0a3/src/adaptix/load_error.py`

 * *Files identical despite different names*

### Comparing `adaptix-3.0.0a2/src/adaptix/provider/__init__.py` & `adaptix-3.0.0a3/src/adaptix/provider/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Saturator,
 )
 from adaptix._internal.provider.model.request_filtering import AnyModelRC
 from adaptix._internal.provider.name_layout.base import ExtraIn, ExtraOut
 from adaptix._internal.provider.name_layout.component import NameMapStack, RawKey, RawPath
 from adaptix._internal.provider.name_style import NameStyle
 from adaptix._internal.provider.provider_basics import Chain
-from adaptix._internal.provider.request_filtering import P, create_request_checker
+from adaptix._internal.provider.request_filtering import P, RequestPattern, create_request_checker
 
 __all__ = (
     'CannotProvide',
     'Mediator',
     'Provider',
     'Request',
     'ExtraCollect',
@@ -28,11 +28,12 @@
     'ExtraIn',
     'ExtraOut',
     'NameMapStack',
     'RawKey',
     'RawPath',
     'NameStyle',
     'Chain',
+    'RequestPattern',
     'P',
     'create_request_checker',
     'AnyModelRC',
 )
```

### Comparing `adaptix-3.0.0a2/src/adaptix.egg-info/SOURCES.txt` & `adaptix-3.0.0a3/src/adaptix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

