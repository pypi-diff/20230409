# Comparing `tmp/coolmongo-1.2.tar.gz` & `tmp/coolmongo-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolmongo-1.2.tar", last modified: Thu Mar 30 12:16:20 2023, max compression
+gzip compressed data, was "coolmongo-1.2.1.tar", last modified: Sun Apr  9 11:42:59 2023, max compression
```

## Comparing `coolmongo-1.2.tar` & `coolmongo-1.2.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmongo-1.2/LICENSE
--rw-r--r--   0        0        0     7326 2023-03-30 06:18:01.743640 coolmongo-1.2/README.md
--rw-r--r--   0        0        0      147 2023-02-25 07:43:51.350884 coolmongo-1.2/coolmongo/__init__.py
--rw-r--r--   0        0        0    20928 2023-03-17 12:19:46.091354 coolmongo-1.2/coolmongo/_coolmongo.py
--rw-r--r--   0        0        0      570 2023-03-30 12:16:10.284843 coolmongo-1.2/pyproject.toml
--rw-r--r--   0        0        0     7573 1970-01-01 00:00:00.000000 coolmongo-1.2/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmongo-1.2.1/LICENSE
+-rw-r--r--   0        0        0     5124 2023-04-09 11:28:09.647580 coolmongo-1.2.1/README.md
+-rw-r--r--   0        0        0    11357 2022-11-17 21:35:25.000000 coolmongo-1.2.1/coolmongo/Licenses of dependent packages/pymongo/LICENSE
+-rw-r--r--   0        0        0      147 2023-02-25 07:43:51.350884 coolmongo-1.2.1/coolmongo/__init__.py
+-rw-r--r--   0        0        0    20928 2023-03-17 12:19:46.091354 coolmongo-1.2.1/coolmongo/_coolmongo.py
+-rw-r--r--   0        0        0      573 2023-04-09 10:59:33.879233 coolmongo-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5401 1970-01-01 00:00:00.000000 coolmongo-1.2.1/PKG-INFO
```

### Comparing `coolmongo-1.2/LICENSE` & `coolmongo-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coolmongo-1.2/coolmongo/_coolmongo.py` & `coolmongo-1.2.1/coolmongo/_coolmongo.py`

 * *Files identical despite different names*

