# Comparing `tmp/pymchelper-2.4.0.tar.gz` & `tmp/pymchelper-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymchelper-2.4.0.tar", last modified: Thu Apr  6 14:27:25 2023, max compression
+gzip compressed data, was "pymchelper-2.4.1.tar", last modified: Sun Apr  9 19:24:14 2023, max compression
```

## Comparing `pymchelper-2.4.0.tar` & `pymchelper-2.4.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:27:25.195409 pymchelper-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-06 14:26:37.000000 pymchelper-2.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-06 14:27:25.195409 pymchelper-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-06 14:26:37.000000 pymchelper-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:27:25.175409 pymchelper-2.4.0/pymchelper/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-06 14:27:24.000000 pymchelper-2.4.0/pymchelper/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/axis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:27:25.179409 pymchelper-2.4.0/pymchelper/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/executor/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/executor/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:27:25.179409 pymchelper-2.4.0/pymchelper/flair/
--rw-r--r--   0 runner    (1001) docker     (123)    30952 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/flair/Data.py
--rw-r--r--   0 runner    (1001) docker     (123)   219827 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/flair/Input.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/flair/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:27:25.183409 pymchelper-2.4.0/pymchelper/flair/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/flair/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68308 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/flair/common/bmath.py
--rw-r--r--   0 runner    (1001) docker     (123)    21373 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/flair/common/csg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/flair/common/fortran.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/flair/common/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    10264 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/flair/common/rexx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:27:25.183409 pymchelper-2.4.0/pymchelper/flair/db/
--rw-r--r--   0 runner    (1001) docker     (123)   183075 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/flair/db/card.db
--rw-r--r--   0 runner    (1001) docker     (123)   234077 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/flair/db/card.ini
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/flair/db/db2ini.r
--rw-r--r--   0 runner    (1001) docker     (123)     8922 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/input_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:27:25.187409 pymchelper-2.4.0/pymchelper/readers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/readers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/readers/fluka.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:27:25.191409 pymchelper-2.4.0/pymchelper/readers/shieldhit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/readers/shieldhit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/readers/shieldhit/binary_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/readers/shieldhit/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/readers/shieldhit/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/readers/shieldhit/reader_bdo2016.py
--rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/readers/shieldhit/reader_bdo2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/readers/shieldhit/reader_bin2010.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:27:25.191409 pymchelper-2.4.0/pymchelper/shieldhit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/shieldhit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:27:25.191409 pymchelper-2.4.0/pymchelper/shieldhit/detector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/shieldhit/detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/shieldhit/detector/detector_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/shieldhit/detector/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/shieldhit/detector/estimator_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/shieldhit/detector/fortran_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/shieldhit/detector/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/shieldhit/particle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:27:25.191409 pymchelper-2.4.0/pymchelper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/utils/mcscripter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:27:25.191409 pymchelper-2.4.0/pymchelper/utils/radiotherapy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/utils/radiotherapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28096 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/utils/radiotherapy/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/utils/runmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:27:25.195409 pymchelper-2.4.0/pymchelper/writers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/writers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/writers/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/writers/fortranformatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/writers/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/writers/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/writers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/writers/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/writers/shieldhit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/writers/sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/writers/trip98cube.py
--rw-r--r--   0 runner    (1001) docker     (123)    36804 2023-04-06 14:26:37.000000 pymchelper-2.4.0/pymchelper/writers/trip98ddd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:27:25.179409 pymchelper-2.4.0/pymchelper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-06 14:27:25.000000 pymchelper-2.4.0/pymchelper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-06 14:27:25.000000 pymchelper-2.4.0/pymchelper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 14:27:25.000000 pymchelper-2.4.0/pymchelper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-06 14:27:25.000000 pymchelper-2.4.0/pymchelper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-06 14:27:25.000000 pymchelper-2.4.0/pymchelper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-06 14:27:25.000000 pymchelper-2.4.0/pymchelper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-06 14:27:25.199409 pymchelper-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-04-06 14:26:37.000000 pymchelper-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.518134 pymchelper-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-09 19:23:50.000000 pymchelper-2.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-09 19:24:14.518134 pymchelper-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-04-09 19:23:50.000000 pymchelper-2.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.502134 pymchelper-2.4.1/pymchelper/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 19:24:14.000000 pymchelper-2.4.1/pymchelper/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.506134 pymchelper-2.4.1/pymchelper/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/executor/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/executor/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.506134 pymchelper-2.4.1/pymchelper/flair/
+-rw-r--r--   0 runner    (1001) docker     (123)    30952 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)   219827 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/Input.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.510134 pymchelper-2.4.1/pymchelper/flair/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68308 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/common/bmath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21373 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/common/csg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/common/fortran.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10264 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/common/rexx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.510134 pymchelper-2.4.1/pymchelper/flair/db/
+-rw-r--r--   0 runner    (1001) docker     (123)   183075 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/db/card.db
+-rw-r--r--   0 runner    (1001) docker     (123)   234077 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/db/card.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/flair/db/db2ini.r
+-rw-r--r--   0 runner    (1001) docker     (123)     8922 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/input_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.514134 pymchelper-2.4.1/pymchelper/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/readers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/readers/fluka.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.514134 pymchelper-2.4.1/pymchelper/readers/shieldhit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/readers/shieldhit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/readers/shieldhit/binary_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/readers/shieldhit/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/readers/shieldhit/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/readers/shieldhit/reader_bdo2016.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/readers/shieldhit/reader_bdo2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/readers/shieldhit/reader_bin2010.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.518134 pymchelper-2.4.1/pymchelper/shieldhit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/shieldhit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.518134 pymchelper-2.4.1/pymchelper/shieldhit/detector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/shieldhit/detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/shieldhit/detector/detector_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/shieldhit/detector/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/shieldhit/detector/estimator_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/shieldhit/detector/fortran_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/shieldhit/detector/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/shieldhit/particle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.518134 pymchelper-2.4.1/pymchelper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12066 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/utils/mcscripter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.518134 pymchelper-2.4.1/pymchelper/utils/radiotherapy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/utils/radiotherapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28096 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/utils/radiotherapy/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/utils/runmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.518134 pymchelper-2.4.1/pymchelper/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/fortranformatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/shieldhit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/trip98cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36804 2023-04-09 19:23:50.000000 pymchelper-2.4.1/pymchelper/writers/trip98ddd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:24:14.506134 pymchelper-2.4.1/pymchelper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-04-09 19:24:14.000000 pymchelper-2.4.1/pymchelper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-09 19:24:14.000000 pymchelper-2.4.1/pymchelper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 19:24:14.000000 pymchelper-2.4.1/pymchelper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-09 19:24:14.000000 pymchelper-2.4.1/pymchelper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-09 19:24:14.000000 pymchelper-2.4.1/pymchelper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 19:24:14.000000 pymchelper-2.4.1/pymchelper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-09 19:24:14.522134 pymchelper-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-04-09 19:23:50.000000 pymchelper-2.4.1/setup.py
```

### Comparing `pymchelper-2.4.0/PKG-INFO` & `pymchelper-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymchelper
-Version: 2.4.0
+Version: 2.4.1
 Summary: Python toolkit for SHIELD-HIT12A and FLUKA
 Home-page: https://github.com/DataMedSci/pymchelper
 Author: pymchelper team
 Author-email: leszek.grzanka@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pymchelper-2.4.0/README.md` & `pymchelper-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/__init__.py` & `pymchelper-2.4.1/pymchelper/__init__.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/axis.py` & `pymchelper-2.4.1/pymchelper/axis.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/estimator.py` & `pymchelper-2.4.1/pymchelper/estimator.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/executor/options.py` & `pymchelper-2.4.1/pymchelper/executor/options.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/executor/runner.py` & `pymchelper-2.4.1/pymchelper/executor/runner.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/flair/Data.py` & `pymchelper-2.4.1/pymchelper/flair/Data.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/flair/Input.py` & `pymchelper-2.4.1/pymchelper/flair/Input.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/flair/common/bmath.py` & `pymchelper-2.4.1/pymchelper/flair/common/bmath.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/flair/common/csg.py` & `pymchelper-2.4.1/pymchelper/flair/common/csg.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/flair/common/fortran.py` & `pymchelper-2.4.1/pymchelper/flair/common/fortran.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/flair/common/log.py` & `pymchelper-2.4.1/pymchelper/flair/common/log.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/flair/common/rexx.py` & `pymchelper-2.4.1/pymchelper/flair/common/rexx.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/flair/db/card.db` & `pymchelper-2.4.1/pymchelper/flair/db/card.db`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/flair/db/card.ini` & `pymchelper-2.4.1/pymchelper/flair/db/card.ini`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/flair/db/db2ini.r` & `pymchelper-2.4.1/pymchelper/flair/db/db2ini.r`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/input_output.py` & `pymchelper-2.4.1/pymchelper/input_output.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/page.py` & `pymchelper-2.4.1/pymchelper/page.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/readers/common.py` & `pymchelper-2.4.1/pymchelper/readers/common.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/readers/fluka.py` & `pymchelper-2.4.1/pymchelper/readers/fluka.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/readers/shieldhit/binary_spec.py` & `pymchelper-2.4.1/pymchelper/readers/shieldhit/binary_spec.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/readers/shieldhit/general.py` & `pymchelper-2.4.1/pymchelper/readers/shieldhit/general.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/readers/shieldhit/reader_base.py` & `pymchelper-2.4.1/pymchelper/readers/shieldhit/reader_base.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/readers/shieldhit/reader_bdo2016.py` & `pymchelper-2.4.1/pymchelper/readers/shieldhit/reader_bdo2016.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/readers/shieldhit/reader_bdo2019.py` & `pymchelper-2.4.1/pymchelper/readers/shieldhit/reader_bdo2019.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/readers/shieldhit/reader_bin2010.py` & `pymchelper-2.4.1/pymchelper/readers/shieldhit/reader_bin2010.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/run.py` & `pymchelper-2.4.1/pymchelper/run.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/shieldhit/detector/detector_type.py` & `pymchelper-2.4.1/pymchelper/shieldhit/detector/detector_type.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/shieldhit/detector/estimator.py` & `pymchelper-2.4.1/pymchelper/shieldhit/detector/estimator.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/shieldhit/detector/fortran_card.py` & `pymchelper-2.4.1/pymchelper/shieldhit/detector/fortran_card.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/shieldhit/detector/geometry.py` & `pymchelper-2.4.1/pymchelper/shieldhit/detector/geometry.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/shieldhit/particle.py` & `pymchelper-2.4.1/pymchelper/shieldhit/particle.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/utils/mcscripter.py` & `pymchelper-2.4.1/pymchelper/utils/mcscripter.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/utils/radiotherapy/plan.py` & `pymchelper-2.4.1/pymchelper/utils/radiotherapy/plan.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/utils/runmc.py` & `pymchelper-2.4.1/pymchelper/utils/runmc.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/version.py` & `pymchelper-2.4.1/pymchelper/version.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/writers/common.py` & `pymchelper-2.4.1/pymchelper/writers/common.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/writers/excel.py` & `pymchelper-2.4.1/pymchelper/writers/excel.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/writers/fortranformatter.py` & `pymchelper-2.4.1/pymchelper/writers/fortranformatter.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/writers/hdf.py` & `pymchelper-2.4.1/pymchelper/writers/hdf.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/writers/inspector.py` & `pymchelper-2.4.1/pymchelper/writers/inspector.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/writers/json.py` & `pymchelper-2.4.1/pymchelper/writers/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             if page.dimension == 0:
                 page_dict["data"]["values"] = [page.data_raw.tolist()]
             else:
                 page_dict["data"]["values"] = page.data_raw.tolist()
 
             for i in range(page.dimension):
                 axis: MeshAxis = page.plot_axis(i)
-                page_dict[f"{i+1}_axis"] = {
+                page_dict[f"axis_dim{i+1}"] = {
                     "unit": str(axis.unit),
                     "name": str(axis.name),
                     "values": axis.data.tolist(),
                 }
 
             est_dict["pages"].append(page_dict)
```

### Comparing `pymchelper-2.4.0/pymchelper/writers/plots.py` & `pymchelper-2.4.1/pymchelper/writers/plots.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/writers/shieldhit.py` & `pymchelper-2.4.1/pymchelper/writers/shieldhit.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/writers/sparse.py` & `pymchelper-2.4.1/pymchelper/writers/sparse.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/writers/trip98cube.py` & `pymchelper-2.4.1/pymchelper/writers/trip98cube.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper/writers/trip98ddd.py` & `pymchelper-2.4.1/pymchelper/writers/trip98ddd.py`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper.egg-info/PKG-INFO` & `pymchelper-2.4.1/pymchelper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymchelper
-Version: 2.4.0
+Version: 2.4.1
 Summary: Python toolkit for SHIELD-HIT12A and FLUKA
 Home-page: https://github.com/DataMedSci/pymchelper
 Author: pymchelper team
 Author-email: leszek.grzanka@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pymchelper-2.4.0/pymchelper.egg-info/SOURCES.txt` & `pymchelper-2.4.1/pymchelper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymchelper-2.4.0/pymchelper.egg-info/requires.txt` & `pymchelper-2.4.1/pymchelper.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 [dicom:python_version == "3.11"]
 pydicom>=2.3.1
 
 [excel]
 xlwt
 
 [full]
+matplotlib
 h5py
 xlwt
 scipy
-matplotlib
 hipsterplot
 bashplotlib
 
 [full:python_version < "3.11"]
 pydicom
 
 [full:python_version == "3.11"]
```

### Comparing `pymchelper-2.4.0/setup.py` & `pymchelper-2.4.1/setup.py`

 * *Files identical despite different names*

