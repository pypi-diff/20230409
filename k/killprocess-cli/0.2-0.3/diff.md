# Comparing `tmp/killprocess_cli-0.2.tar.gz` & `tmp/killprocess_cli-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "killprocess_cli-0.2.tar", last modified: Sat Nov 26 11:34:33 2022, max compression
+gzip compressed data, was "killprocess_cli-0.3.tar", last modified: Sun Apr  9 18:51:45 2023, max compression
```

## Comparing `killprocess_cli-0.2.tar` & `killprocess_cli-0.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 tushar    (1000) tushar    (1000)        0 2022-11-26 11:34:33.576027 killprocess_cli-0.2/
--rw-rw-r--   0 tushar    (1000) tushar    (1000)      238 2022-11-26 11:34:33.576027 killprocess_cli-0.2/PKG-INFO
-drwxrwxr-x   0 tushar    (1000) tushar    (1000)        0 2022-11-26 11:34:33.576027 killprocess_cli-0.2/killprocess_cli/
--rw-rw-r--   0 tushar    (1000) tushar    (1000)      541 2022-11-26 11:15:23.000000 killprocess_cli-0.2/killprocess_cli/__init__.py
-drwxrwxr-x   0 tushar    (1000) tushar    (1000)        0 2022-11-26 11:34:33.576027 killprocess_cli-0.2/killprocess_cli.egg-info/
--rw-rw-r--   0 tushar    (1000) tushar    (1000)      238 2022-11-26 11:34:33.000000 killprocess_cli-0.2/killprocess_cli.egg-info/PKG-INFO
--rw-rw-r--   0 tushar    (1000) tushar    (1000)      234 2022-11-26 11:34:33.000000 killprocess_cli-0.2/killprocess_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 tushar    (1000) tushar    (1000)        1 2022-11-26 11:34:33.000000 killprocess_cli-0.2/killprocess_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 tushar    (1000) tushar    (1000)       63 2022-11-26 11:34:33.000000 killprocess_cli-0.2/killprocess_cli.egg-info/entry_points.txt
--rw-rw-r--   0 tushar    (1000) tushar    (1000)       16 2022-11-26 11:34:33.000000 killprocess_cli-0.2/killprocess_cli.egg-info/top_level.txt
--rw-rw-r--   0 tushar    (1000) tushar    (1000)       38 2022-11-26 11:34:33.576027 killprocess_cli-0.2/setup.cfg
--rw-rw-r--   0 tushar    (1000) tushar    (1000)      449 2022-11-26 11:34:26.000000 killprocess_cli-0.2/setup.py
+drwxrwxr-x   0 tushar    (1000) tushar    (1000)        0 2023-04-09 18:51:45.246048 killprocess_cli-0.3/
+-rw-rw-r--   0 tushar    (1000) tushar    (1000)     1660 2023-04-09 18:51:45.242047 killprocess_cli-0.3/PKG-INFO
+-rw-rw-r--   0 tushar    (1000) tushar    (1000)      959 2023-04-09 18:49:39.000000 killprocess_cli-0.3/README.md
+drwxrwxr-x   0 tushar    (1000) tushar    (1000)        0 2023-04-09 18:51:45.242047 killprocess_cli-0.3/killprocess_cli/
+-rw-rw-r--   0 tushar    (1000) tushar    (1000)      541 2022-11-26 11:15:23.000000 killprocess_cli-0.3/killprocess_cli/__init__.py
+drwxrwxr-x   0 tushar    (1000) tushar    (1000)        0 2023-04-09 18:51:45.242047 killprocess_cli-0.3/killprocess_cli.egg-info/
+-rw-rw-r--   0 tushar    (1000) tushar    (1000)     1660 2023-04-09 18:51:45.000000 killprocess_cli-0.3/killprocess_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 tushar    (1000) tushar    (1000)      244 2023-04-09 18:51:45.000000 killprocess_cli-0.3/killprocess_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 tushar    (1000) tushar    (1000)        1 2023-04-09 18:51:45.000000 killprocess_cli-0.3/killprocess_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 tushar    (1000) tushar    (1000)       63 2023-04-09 18:51:45.000000 killprocess_cli-0.3/killprocess_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 tushar    (1000) tushar    (1000)       16 2023-04-09 18:51:45.000000 killprocess_cli-0.3/killprocess_cli.egg-info/top_level.txt
+-rw-rw-r--   0 tushar    (1000) tushar    (1000)       38 2023-04-09 18:51:45.246048 killprocess_cli-0.3/setup.cfg
+-rw-rw-r--   0 tushar    (1000) tushar    (1000)      839 2023-04-09 18:47:58.000000 killprocess_cli-0.3/setup.py
```

### Comparing `killprocess_cli-0.2/killprocess_cli/__init__.py` & `killprocess_cli-0.3/killprocess_cli/__init__.py`

 * *Files identical despite different names*

