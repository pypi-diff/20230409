# Comparing `tmp/precious_lotr_sdk-1.0.tar.gz` & `tmp/precious_lotr_sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "precious_lotr_sdk-1.0.tar", last modified: Sun Apr  9 02:34:27 2023, max compression
+gzip compressed data, was "precious_lotr_sdk-1.0.2.tar", last modified: Sun Apr  9 03:10:29 2023, max compression
```

## Comparing `precious_lotr_sdk-1.0.tar` & `precious_lotr_sdk-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 suhaibalfageeh   (501) staff       (20)        0 2023-04-09 02:34:27.584817 precious_lotr_sdk-1.0/
--rw-r--r--   0 suhaibalfageeh   (501) staff       (20)      235 2023-04-09 02:34:27.584707 precious_lotr_sdk-1.0/PKG-INFO
-drwxr-xr-x   0 suhaibalfageeh   (501) staff       (20)        0 2023-04-09 02:34:27.583965 precious_lotr_sdk-1.0/precious_lotr_sdk/
--rw-r--r--   0 suhaibalfageeh   (501) staff       (20)        0 2023-04-08 01:29:02.000000 precious_lotr_sdk-1.0/precious_lotr_sdk/__init__.py
--rw-r--r--   0 suhaibalfageeh   (501) staff       (20)      675 2023-04-08 01:29:38.000000 precious_lotr_sdk-1.0/precious_lotr_sdk/lotr.py
-drwxr-xr-x   0 suhaibalfageeh   (501) staff       (20)        0 2023-04-09 02:34:27.584551 precious_lotr_sdk-1.0/precious_lotr_sdk.egg-info/
--rw-r--r--   0 suhaibalfageeh   (501) staff       (20)      235 2023-04-09 02:34:27.000000 precious_lotr_sdk-1.0/precious_lotr_sdk.egg-info/PKG-INFO
--rw-r--r--   0 suhaibalfageeh   (501) staff       (20)      268 2023-04-09 02:34:27.000000 precious_lotr_sdk-1.0/precious_lotr_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 suhaibalfageeh   (501) staff       (20)        1 2023-04-09 02:34:27.000000 precious_lotr_sdk-1.0/precious_lotr_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 suhaibalfageeh   (501) staff       (20)        9 2023-04-09 02:34:27.000000 precious_lotr_sdk-1.0/precious_lotr_sdk.egg-info/requires.txt
--rw-r--r--   0 suhaibalfageeh   (501) staff       (20)       18 2023-04-09 02:34:27.000000 precious_lotr_sdk-1.0/precious_lotr_sdk.egg-info/top_level.txt
--rw-r--r--   0 suhaibalfageeh   (501) staff       (20)       38 2023-04-09 02:34:27.584857 precious_lotr_sdk-1.0/setup.cfg
--rw-r--r--   0 suhaibalfageeh   (501) staff       (20)      317 2023-04-09 02:33:42.000000 precious_lotr_sdk-1.0/setup.py
+drwxr-xr-x   0 suhaibalfageeh   (501) staff       (20)        0 2023-04-09 03:10:29.233611 precious_lotr_sdk-1.0.2/
+-rw-r--r--   0 suhaibalfageeh   (501) staff       (20)      237 2023-04-09 03:10:29.233497 precious_lotr_sdk-1.0.2/PKG-INFO
+drwxr-xr-x   0 suhaibalfageeh   (501) staff       (20)        0 2023-04-09 03:10:29.232578 precious_lotr_sdk-1.0.2/precious_lotr_sdk/
+-rw-r--r--   0 suhaibalfageeh   (501) staff       (20)       25 2023-04-09 02:52:32.000000 precious_lotr_sdk-1.0.2/precious_lotr_sdk/__init__.py
+-rw-r--r--   0 suhaibalfageeh   (501) staff       (20)     1621 2023-04-09 03:08:04.000000 precious_lotr_sdk-1.0.2/precious_lotr_sdk/lotr.py
+drwxr-xr-x   0 suhaibalfageeh   (501) staff       (20)        0 2023-04-09 03:10:29.233209 precious_lotr_sdk-1.0.2/precious_lotr_sdk.egg-info/
+-rw-r--r--   0 suhaibalfageeh   (501) staff       (20)      237 2023-04-09 03:10:29.000000 precious_lotr_sdk-1.0.2/precious_lotr_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 suhaibalfageeh   (501) staff       (20)      281 2023-04-09 03:10:29.000000 precious_lotr_sdk-1.0.2/precious_lotr_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 suhaibalfageeh   (501) staff       (20)        1 2023-04-09 03:10:29.000000 precious_lotr_sdk-1.0.2/precious_lotr_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 suhaibalfageeh   (501) staff       (20)        9 2023-04-09 03:10:29.000000 precious_lotr_sdk-1.0.2/precious_lotr_sdk.egg-info/requires.txt
+-rw-r--r--   0 suhaibalfageeh   (501) staff       (20)       18 2023-04-09 03:10:29.000000 precious_lotr_sdk-1.0.2/precious_lotr_sdk.egg-info/top_level.txt
+-rw-r--r--   0 suhaibalfageeh   (501) staff       (20)       38 2023-04-09 03:10:29.233658 precious_lotr_sdk-1.0.2/setup.cfg
+-rw-r--r--   0 suhaibalfageeh   (501) staff       (20)      319 2023-04-09 03:09:56.000000 precious_lotr_sdk-1.0.2/setup.py
+drwxr-xr-x   0 suhaibalfageeh   (501) staff       (20)        0 2023-04-09 03:10:29.233333 precious_lotr_sdk-1.0.2/test/
+-rw-r--r--   0 suhaibalfageeh   (501) staff       (20)     3154 2023-04-09 02:50:50.000000 precious_lotr_sdk-1.0.2/test/test.py
```

