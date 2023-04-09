# Comparing `tmp/frozendict-2.3.6.tar.gz` & `tmp/frozendict-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frozendict-2.3.6.tar", last modified: Tue Mar 21 23:23:02 2023, max compression
+gzip compressed data, was "frozendict-2.3.7.tar", last modified: Sun Apr  9 19:35:25 2023, max compression
```

## Comparing `frozendict-2.3.6.tar` & `frozendict-2.3.7.tar`

### file list

```diff
@@ -1,34 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:23:02.547039 frozendict-2.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-03-21 23:22:55.000000 frozendict-2.3.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-21 23:22:55.000000 frozendict-2.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-03-21 23:23:02.547039 frozendict-2.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19173 2023-03-21 23:22:55.000000 frozendict-2.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 23:23:02.547039 frozendict-2.3.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     5749 2023-03-21 23:22:55.000000 frozendict-2.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:23:02.543039 frozendict-2.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:23:02.543039 frozendict-2.3.6/src/frozendict/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-21 23:22:55.000000 frozendict-2.3.6/src/frozendict/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:23:02.543039 frozendict-2.3.6/src/frozendict/c_src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:23:02.547039 frozendict-2.3.6/src/frozendict/c_src/3_10/
--rw-r--r--   0 runner    (1001) docker     (123)    60336 2023-03-21 23:22:55.000000 frozendict-2.3.6/src/frozendict/c_src/3_10/frozendictobject.c
--rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-03-21 23:22:55.000000 frozendict-2.3.6/src/frozendict/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-21 23:22:55.000000 frozendict-2.3.6/src/frozendict/frozendict.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-03-21 23:22:55.000000 frozendict-2.3.6/src/frozendict/monkeypatch.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 23:22:55.000000 frozendict-2.3.6/src/frozendict/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-21 23:22:55.000000 frozendict-2.3.6/src/frozendict/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:23:02.547039 frozendict-2.3.6/src/frozendict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-03-21 23:23:02.000000 frozendict-2.3.6/src/frozendict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-21 23:23:02.000000 frozendict-2.3.6/src/frozendict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 23:23:02.000000 frozendict-2.3.6/src/frozendict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-21 23:23:02.000000 frozendict-2.3.6/src/frozendict.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 23:23:02.547039 frozendict-2.3.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 23:22:55.000000 frozendict-2.3.6/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-03-21 23:22:55.000000 frozendict-2.3.6/test/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7524 2023-03-21 23:22:55.000000 frozendict-2.3.6/test/bench.py
--rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-03-21 23:22:55.000000 frozendict-2.3.6/test/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13230 2023-03-21 23:22:55.000000 frozendict-2.3.6/test/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-21 23:22:55.000000 frozendict-2.3.6/test/frozendict_only.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-03-21 23:22:55.000000 frozendict-2.3.6/test/subclass_only.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-21 23:22:55.000000 frozendict-2.3.6/test/test_frozendict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-21 23:22:55.000000 frozendict-2.3.6/test/test_frozendict_subclass.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-21 23:22:55.000000 frozendict-2.3.6/test/typed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.722411 frozendict-2.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-09 19:35:17.000000 frozendict-2.3.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-09 19:35:17.000000 frozendict-2.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-04-09 19:35:25.722411 frozendict-2.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19173 2023-04-09 19:35:17.000000 frozendict-2.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 19:35:25.722411 frozendict-2.3.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5749 2023-04-09 19:35:17.000000 frozendict-2.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.702409 frozendict-2.3.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.706410 frozendict-2.3.7/src/frozendict/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.706410 frozendict-2.3.7/src/frozendict/c_src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.706410 frozendict-2.3.7/src/frozendict/c_src/3_10/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.706410 frozendict-2.3.7/src/frozendict/c_src/3_10/Include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_10/Include/cpython/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_10/Include/cpython/frozendictobject.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_10/Include/frozendictobject.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/Objects/clinic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/Objects/clinic/dictobject.c.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/Objects/dict-common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    57234 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject.c
+-rw-r--r--   0 runner    (1001) docker     (123)   152447 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/Objects/dictobject_original.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/Objects/stringlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/Objects/stringlib/eq.h
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_10/cpython_src/other.c
+-rw-r--r--   0 runner    (1001) docker     (123)    60336 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_10/frozendictobject.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_6/Include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_6/Include/cpython/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_6/Include/cpython/frozendictobject.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_6/Include/frozendictobject.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/Objects/clinic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/Objects/clinic/dictobject.c.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/Objects/dict-common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    63009 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject.c
+-rw-r--r--   0 runner    (1001) docker     (123)   135061 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/Objects/dictobject_original.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/Objects/stringlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/Objects/stringlib/eq.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_6/cpython_src/other.c
+-rw-r--r--   0 runner    (1001) docker     (123)    58155 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_6/frozendictobject.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_7/Include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_7/Include/cpython/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_7/Include/cpython/frozendictobject.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_7/Include/frozendictobject.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.710410 frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/Objects/clinic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/Objects/clinic/dictobject.c.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/Objects/dict-common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    61834 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject.c
+-rw-r--r--   0 runner    (1001) docker     (123)   132228 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/Objects/dictobject_original.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/Objects/stringlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/Objects/stringlib/eq.h
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_7/cpython_src/other.c
+-rw-r--r--   0 runner    (1001) docker     (123)    58478 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_7/frozendictobject.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_8/Include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_8/Include/cpython/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_8/Include/cpython/frozendictobject.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_8/Include/frozendictobject.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/Objects/clinic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/Objects/clinic/dictobject.c.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/Objects/dict-common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    58062 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject.c
+-rw-r--r--   0 runner    (1001) docker     (123)   141374 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/Objects/dictobject_original.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/Objects/stringlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/Objects/stringlib/eq.h
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_8/cpython_src/other.c
+-rw-r--r--   0 runner    (1001) docker     (123)    60418 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_8/frozendictobject.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_9/Include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_9/Include/cpython/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_9/Include/cpython/frozendictobject.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_9/Include/frozendictobject.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.714410 frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.718410 frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/Objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.718410 frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/Objects/clinic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/Objects/clinic/dictobject.c.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/Objects/dict-common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    58099 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject.c
+-rw-r--r--   0 runner    (1001) docker     (123)   145558 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/Objects/dictobject_original.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.718410 frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/Objects/stringlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/Objects/stringlib/eq.h
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_9/cpython_src/other.c
+-rw-r--r--   0 runner    (1001) docker     (123)    60489 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/c_src/3_9/frozendictobject.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/frozendict.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/monkeypatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-09 19:35:17.000000 frozendict-2.3.7/src/frozendict/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.706410 frozendict-2.3.7/src/frozendict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20302 2023-04-09 19:35:25.000000 frozendict-2.3.7/src/frozendict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-09 19:35:25.000000 frozendict-2.3.7/src/frozendict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 19:35:25.000000 frozendict-2.3.7/src/frozendict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 19:35:25.000000 frozendict-2.3.7/src/frozendict.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:25.722411 frozendict-2.3.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:35:17.000000 frozendict-2.3.7/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-09 19:35:17.000000 frozendict-2.3.7/test/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7524 2023-04-09 19:35:17.000000 frozendict-2.3.7/test/bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-04-09 19:35:17.000000 frozendict-2.3.7/test/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13297 2023-04-09 19:35:17.000000 frozendict-2.3.7/test/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-09 19:35:17.000000 frozendict-2.3.7/test/frozendict_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-09 19:35:17.000000 frozendict-2.3.7/test/subclass_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-09 19:35:17.000000 frozendict-2.3.7/test/test_frozendict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-09 19:35:17.000000 frozendict-2.3.7/test/test_frozendict_subclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-09 19:35:17.000000 frozendict-2.3.7/test/typed.py
```

### Comparing `frozendict-2.3.6/LICENSE.txt` & `frozendict-2.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.6/PKG-INFO` & `frozendict-2.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frozendict
-Version: 2.3.6
+Version: 2.3.7
 Summary: A simple immutable dictionary
 Home-page: https://github.com/Marco-Sulla/python-frozendict
 Author: Marco Sulla
 Author-email: marcosullaroma@gmail.com
 License: LGPL v3
 Project-URL: Bug Reports, https://github.com/Marco-Sulla/python-frozendict/issues
 Project-URL: Source, https://github.com/Marco-Sulla/python-frozendict
```

### Comparing `frozendict-2.3.6/README.md` & `frozendict-2.3.7/README.md`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.6/setup.py` & `frozendict-2.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.6/src/frozendict/__init__.py` & `frozendict-2.3.7/src/frozendict/__init__.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.6/src/frozendict/c_src/3_10/frozendictobject.c` & `frozendict-2.3.7/src/frozendict/c_src/3_10/frozendictobject.c`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.6/src/frozendict/core.py` & `frozendict-2.3.7/src/frozendict/core.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.6/src/frozendict/monkeypatch.py` & `frozendict-2.3.7/src/frozendict/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.6/src/frozendict.egg-info/PKG-INFO` & `frozendict-2.3.7/src/frozendict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frozendict
-Version: 2.3.6
+Version: 2.3.7
 Summary: A simple immutable dictionary
 Home-page: https://github.com/Marco-Sulla/python-frozendict
 Author: Marco Sulla
 Author-email: marcosullaroma@gmail.com
 License: LGPL v3
 Project-URL: Bug Reports, https://github.com/Marco-Sulla/python-frozendict/issues
 Project-URL: Source, https://github.com/Marco-Sulla/python-frozendict
```

### Comparing `frozendict-2.3.6/test/base.py` & `frozendict-2.3.7/test/base.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.6/test/bench.py` & `frozendict-2.3.7/test/bench.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.6/test/common.py` & `frozendict-2.3.7/test/common.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.6/test/debug.py` & `frozendict-2.3.7/test/debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 def print_sep():
     print(
         "------------------------------------------------------------------------------", 
         flush=True
     )
 
-def trace(iterations=100):
+def trace(iterations = 100, mult = 10):
     def decorator(func):
         def wrapper():
             print(
                 f"Loops: {iterations} - Evaluating: {func.__name__}", 
                 flush = True
             )
             
@@ -87,15 +87,15 @@
                 (tracemalloc.Filter(True, __file__), )
             )
 
             top_stats = snapshot2.compare_to(snapshot1, 'lineno')
             tracemalloc.stop()
             
             for stat in top_stats:
-                if stat.count_diff * 10 > iterations:
+                if stat.count_diff * mult > iterations:
                     print(
                         f"Error. count diff: {stat.count_diff}, stat: {stat}", 
                         flush = True
                     )
                     
                     sys.exit(1)
         
@@ -117,35 +117,35 @@
 dict_unashable.update({getUuid(): []})
 dict_1_items = tuple(dict_1.items())
 dict_1_keys = tuple(dict_1.keys())
 dict_1_keys_set = set(dict_1_keys)
 
 functions = []
 
-@trace()
+@trace(iterations = 300, mult = 1.5)
 def func_1():
-    frozendict_class(dict_1)
+    pickle.loads(pickle.dumps(fd_1))
 
 functions.append(func_1)
 
-@trace()
+@trace(iterations = 200, mult = 1.7)
 def func_2():
-    frozendict_class(dict_unashable)
+    pickle.loads(pickle.dumps(iter(fd_1.keys())))
 
 functions.append(func_2)
 
-@trace()
+@trace(iterations = 200, mult = 1.5)
 def func_3():
-    frozendict_class(dict_3)
+    pickle.loads(pickle.dumps(iter(fd_1.items())))
 
 functions.append(func_3)
 
-@trace()
+@trace(iterations = 300, mult = 1.4)
 def func_4():
-    frozendict_class()
+    pickle.loads(pickle.dumps(iter(fd_1.values())))
 
 functions.append(func_4)
 
 @trace()
 def func_5():
     frozendict_class({})
 
@@ -232,17 +232,17 @@
 
 @trace()
 def func_20():
     fd_1 == dict_2
 
 functions.append(func_20)
 
-@trace(iterations=1500)
+@trace()
 def func_21():
-    pickle.loads(pickle.dumps(fd_1))
+    frozendict_class(dict_1)
 
 functions.append(func_21)
 
 @trace()
 def func_22():
     frozendict_class(dict_1_items)
 
@@ -564,29 +564,29 @@
 
 @trace()
 def func_75():
     fd_1.items() ^ frozendict_class(dict_hole).items()
 
 functions.append(func_75)
 
-@trace(iterations=1700)
+@trace()
 def func_76():
-    pickle.loads(pickle.dumps(iter(fd_1.keys())))
+    frozendict_class(dict_unashable)
 
 functions.append(func_76)
 
-@trace(iterations=1500)
+@trace()
 def func_77():
-    pickle.loads(pickle.dumps(iter(fd_1.items())))
+    frozendict_class(dict_3)
 
 functions.append(func_77)
 
-@trace(iterations=2000)
+@trace()
 def func_78():
-    pickle.loads(pickle.dumps(iter(fd_1.values())))
+    frozendict_class()
 
 functions.append(func_78)
 
 @trace()
 def func_79():
     frozendict_class(dict_hole).keys() < fd_1.keys()
```

### Comparing `frozendict-2.3.6/test/frozendict_only.py` & `frozendict-2.3.7/test/frozendict_only.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.6/test/subclass_only.py` & `frozendict-2.3.7/test/subclass_only.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.6/test/test_frozendict.py` & `frozendict-2.3.7/test/test_frozendict.py`

 * *Files identical despite different names*

### Comparing `frozendict-2.3.6/test/test_frozendict_subclass.py` & `frozendict-2.3.7/test/test_frozendict_subclass.py`

 * *Files identical despite different names*

