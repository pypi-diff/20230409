# Comparing `tmp/coolmysql-1.2.tar.gz` & `tmp/coolmysql-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolmysql-1.2.tar", last modified: Thu Mar 30 12:16:45 2023, max compression
+gzip compressed data, was "coolmysql-1.2.1.tar", last modified: Sun Apr  9 11:43:22 2023, max compression
```

## Comparing `coolmysql-1.2.tar` & `coolmysql-1.2.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmysql-1.2/LICENSE
--rw-r--r--   0        0        0     7104 2023-03-30 06:19:55.400452 coolmysql-1.2/README.md
--rw-r--r--   0        0        0       73 2023-02-27 13:47:12.329777 coolmysql-1.2/coolmysql/__init__.py
--rw-r--r--   0        0        0    19839 2023-03-11 05:27:30.756063 coolmysql-1.2/coolmysql/_coolmysql.py
--rw-r--r--   0        0        0      578 2023-03-30 12:16:36.030991 coolmysql-1.2/pyproject.toml
--rw-r--r--   0        0        0     7354 1970-01-01 00:00:00.000000 coolmysql-1.2/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmysql-1.2.1/LICENSE
+-rw-r--r--   0        0        0     4351 2023-04-09 11:16:42.051321 coolmysql-1.2.1/README.md
+-rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 coolmysql-1.2.1/coolmysql/Licenses of dependent packages/pymysql/LICENSE
+-rw-r--r--   0        0        0       73 2023-02-27 13:47:12.329777 coolmysql-1.2.1/coolmysql/__init__.py
+-rw-r--r--   0        0        0    19839 2023-03-11 05:27:30.756063 coolmysql-1.2.1/coolmysql/_coolmysql.py
+-rw-r--r--   0        0        0      581 2023-04-09 10:43:44.395068 coolmysql-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4646 1970-01-01 00:00:00.000000 coolmysql-1.2.1/PKG-INFO
```

### Comparing `coolmysql-1.2/LICENSE` & `coolmysql-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coolmysql-1.2/coolmysql/_coolmysql.py` & `coolmysql-1.2.1/coolmysql/_coolmysql.py`

 * *Files identical despite different names*

