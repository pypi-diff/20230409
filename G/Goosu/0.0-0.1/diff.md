# Comparing `tmp/Goosu-0.0.tar.gz` & `tmp/Goosu-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Goosu-0.0.tar", last modified: Sun Apr  9 07:51:06 2023, max compression
+gzip compressed data, was "Goosu-0.1.tar", last modified: Sun Apr  9 08:04:34 2023, max compression
```

## Comparing `Goosu-0.0.tar` & `Goosu-0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 aleksejmetlusko   (501) staff       (20)        0 2023-04-09 07:51:06.188133 Goosu-0.0/
-drwxr-xr-x   0 aleksejmetlusko   (501) staff       (20)        0 2023-04-09 07:51:06.187395 Goosu-0.0/Goosu/
--rw-r--r--   0 aleksejmetlusko   (501) staff       (20)      539 2023-04-09 07:20:49.000000 Goosu-0.0/Goosu/_init_.py
-drwxr-xr-x   0 aleksejmetlusko   (501) staff       (20)        0 2023-04-09 07:51:06.188051 Goosu-0.0/Goosu.egg-info/
--rw-r--r--   0 aleksejmetlusko   (501) staff       (20)      243 2023-04-09 07:51:06.000000 Goosu-0.0/Goosu.egg-info/PKG-INFO
--rw-r--r--   0 aleksejmetlusko   (501) staff       (20)      178 2023-04-09 07:51:06.000000 Goosu-0.0/Goosu.egg-info/SOURCES.txt
--rw-r--r--   0 aleksejmetlusko   (501) staff       (20)        1 2023-04-09 07:51:06.000000 Goosu-0.0/Goosu.egg-info/dependency_links.txt
--rw-r--r--   0 aleksejmetlusko   (501) staff       (20)       14 2023-04-09 07:51:06.000000 Goosu-0.0/Goosu.egg-info/requires.txt
--rw-r--r--   0 aleksejmetlusko   (501) staff       (20)        6 2023-04-09 07:51:06.000000 Goosu-0.0/Goosu.egg-info/top_level.txt
--rw-r--r--   0 aleksejmetlusko   (501) staff       (20)      243 2023-04-09 07:51:06.188179 Goosu-0.0/PKG-INFO
--rw-r--r--   0 aleksejmetlusko   (501) staff       (20)       38 2023-04-09 07:51:06.188362 Goosu-0.0/setup.cfg
--rw-r--r--   0 aleksejmetlusko   (501) staff       (20)      318 2023-04-09 07:44:21.000000 Goosu-0.0/setup.py
+drwxr-xr-x   0 aleksejmetlusko   (501) staff       (20)        0 2023-04-09 08:04:34.389265 Goosu-0.1/
+drwxr-xr-x   0 aleksejmetlusko   (501) staff       (20)        0 2023-04-09 08:04:34.388329 Goosu-0.1/Goosu/
+-rw-r--r--   0 aleksejmetlusko   (501) staff       (20)      539 2023-04-09 07:20:49.000000 Goosu-0.1/Goosu/_init_.py
+drwxr-xr-x   0 aleksejmetlusko   (501) staff       (20)        0 2023-04-09 08:04:34.389161 Goosu-0.1/Goosu.egg-info/
+-rw-r--r--   0 aleksejmetlusko   (501) staff       (20)      243 2023-04-09 08:04:34.000000 Goosu-0.1/Goosu.egg-info/PKG-INFO
+-rw-r--r--   0 aleksejmetlusko   (501) staff       (20)      178 2023-04-09 08:04:34.000000 Goosu-0.1/Goosu.egg-info/SOURCES.txt
+-rw-r--r--   0 aleksejmetlusko   (501) staff       (20)        1 2023-04-09 08:04:34.000000 Goosu-0.1/Goosu.egg-info/dependency_links.txt
+-rw-r--r--   0 aleksejmetlusko   (501) staff       (20)        9 2023-04-09 08:04:34.000000 Goosu-0.1/Goosu.egg-info/requires.txt
+-rw-r--r--   0 aleksejmetlusko   (501) staff       (20)        6 2023-04-09 08:04:34.000000 Goosu-0.1/Goosu.egg-info/top_level.txt
+-rw-r--r--   0 aleksejmetlusko   (501) staff       (20)      243 2023-04-09 08:04:34.389318 Goosu-0.1/PKG-INFO
+-rw-r--r--   0 aleksejmetlusko   (501) staff       (20)       38 2023-04-09 08:04:34.389521 Goosu-0.1/setup.cfg
+-rw-r--r--   0 aleksejmetlusko   (501) staff       (20)      285 2023-04-09 08:03:42.000000 Goosu-0.1/setup.py
```

### Comparing `Goosu-0.0/Goosu/_init_.py` & `Goosu-0.1/Goosu/_init_.py`

 * *Files identical despite different names*

