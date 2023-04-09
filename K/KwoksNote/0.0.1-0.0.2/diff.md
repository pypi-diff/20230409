# Comparing `tmp/KwoksNote-0.0.1.tar.gz` & `tmp/KwoksNote-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KwoksNote-0.0.1.tar", last modified: Sun Apr  9 00:31:41 2023, max compression
+gzip compressed data, was "KwoksNote-0.0.2.tar", last modified: Sun Apr  9 00:52:23 2023, max compression
```

## Comparing `KwoksNote-0.0.1.tar` & `KwoksNote-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 00:31:41.736055 KwoksNote-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-04-09 00:31:41.720434 KwoksNote-0.0.1/KwoksNote/
--rw-rw-rw-   0        0        0      170 2023-04-09 00:31:10.000000 KwoksNote-0.0.1/KwoksNote/__init__.py
--rw-rw-rw-   0        0        0       23 2023-04-09 00:29:09.000000 KwoksNote-0.0.1/KwoksNote/_version.py
-drwxrwxrwx   0        0        0        0 2023-04-09 00:31:41.736055 KwoksNote-0.0.1/KwoksNote.egg-info/
--rw-rw-rw-   0        0        0       56 2023-04-09 00:31:41.000000 KwoksNote-0.0.1/KwoksNote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-04-09 00:31:41.000000 KwoksNote-0.0.1/KwoksNote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 00:31:41.000000 KwoksNote-0.0.1/KwoksNote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-09 00:31:41.000000 KwoksNote-0.0.1/KwoksNote.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       56 2023-04-09 00:31:41.736055 KwoksNote-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       65 2023-04-09 00:29:47.000000 KwoksNote-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-09 00:31:41.736055 KwoksNote-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-09 00:52:23.733411 KwoksNote-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-04-09 00:52:23.733411 KwoksNote-0.0.2/KwoksNote/
+-rw-rw-rw-   0        0        0      191 2023-04-09 00:49:33.000000 KwoksNote-0.0.2/KwoksNote/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-04-09 00:51:36.000000 KwoksNote-0.0.2/KwoksNote/_version.py
+-rw-rw-rw-   0        0        0       23 2023-04-09 00:29:09.000000 KwoksNote-0.0.2/KwoksNote/数据分析.py
+drwxrwxrwx   0        0        0        0 2023-04-09 00:52:23.733411 KwoksNote-0.0.2/KwoksNote.egg-info/
+-rw-rw-rw-   0        0        0       56 2023-04-09 00:52:23.000000 KwoksNote-0.0.2/KwoksNote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-04-09 00:52:23.000000 KwoksNote-0.0.2/KwoksNote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 00:52:23.000000 KwoksNote-0.0.2/KwoksNote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-09 00:52:23.000000 KwoksNote-0.0.2/KwoksNote.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       56 2023-04-09 00:52:23.733411 KwoksNote-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       65 2023-04-09 00:51:47.000000 KwoksNote-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-09 00:52:23.733411 KwoksNote-0.0.2/setup.cfg
```

