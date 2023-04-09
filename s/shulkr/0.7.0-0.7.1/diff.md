# Comparing `tmp/shulkr-0.7.0.tar.gz` & `tmp/shulkr-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shulkr-0.7.0.tar", last modified: Thu Sep  8 07:30:44 2022, max compression
+gzip compressed data, was "shulkr-0.7.1.tar", last modified: Sun Apr  9 03:21:55 2023, max compression
```

## Comparing `shulkr-0.7.0.tar` & `shulkr-0.7.1.tar`

### file list

```diff
@@ -1,90 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.642883 shulkr-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-09-08 07:20:32.000000 shulkr-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4563 2022-09-08 07:30:44.642883 shulkr-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3668 2022-09-08 07:20:32.000000 shulkr-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.630883 shulkr-0.7.0/java/
--rw-r--r--   0 runner    (1001) docker     (121)    10648 2022-09-08 07:20:32.000000 shulkr-0.7.0/java/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-09-08 07:20:32.000000 shulkr-0.7.0/java/blob.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.630883 shulkr-0.7.0/minecraft/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 07:20:32.000000 shulkr-0.7.0/minecraft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3135 2022-09-08 07:20:32.000000 shulkr-0.7.0/minecraft/source.py
--rw-r--r--   0 runner    (1001) docker     (121)     5946 2022-09-08 07:20:32.000000 shulkr-0.7.0/minecraft/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.634883 shulkr-0.7.0/mint/
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-08 07:20:32.000000 shulkr-0.7.0/mint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2061 2022-09-08 07:20:32.000000 shulkr-0.7.0/mint/command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2022-09-08 07:20:32.000000 shulkr-0.7.0/mint/repo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.634883 shulkr-0.7.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 07:20:32.000000 shulkr-0.7.0/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.634883 shulkr-0.7.0/scripts/bump/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 07:20:32.000000 shulkr-0.7.0/scripts/bump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-09-08 07:20:32.000000 shulkr-0.7.0/scripts/bump/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-08 07:30:44.642883 shulkr-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1728 2022-09-08 07:20:32.000000 shulkr-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.634883 shulkr-0.7.0/shulkr/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 07:20:32.000000 shulkr-0.7.0/shulkr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-09-08 07:20:32.000000 shulkr-0.7.0/shulkr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1991 2022-09-08 07:20:32.000000 shulkr-0.7.0/shulkr/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     1373 2022-09-08 07:20:32.000000 shulkr-0.7.0/shulkr/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-09-08 07:20:32.000000 shulkr-0.7.0/shulkr/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (121)     2841 2022-09-08 07:20:32.000000 shulkr-0.7.0/shulkr/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      751 2022-09-08 07:20:32.000000 shulkr-0.7.0/shulkr/gitignore.py
--rw-r--r--   0 runner    (1001) docker     (121)      835 2022-09-08 07:20:32.000000 shulkr-0.7.0/shulkr/repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2859 2022-09-08 07:20:33.000000 shulkr-0.7.0/shulkr/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.634883 shulkr-0.7.0/shulkr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4563 2022-09-08 07:30:44.000000 shulkr-0.7.0/shulkr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1805 2022-09-08 07:30:44.000000 shulkr-0.7.0/shulkr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 07:30:44.000000 shulkr-0.7.0/shulkr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-08 07:30:44.000000 shulkr-0.7.0/shulkr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-09-08 07:30:44.000000 shulkr-0.7.0/shulkr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-09-08 07:30:44.000000 shulkr-0.7.0/shulkr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.630883 shulkr-0.7.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.634883 shulkr-0.7.0/tests/java/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.634883 shulkr-0.7.0/tests/java/functional/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/java/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7068 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/java/functional/test__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.638883 shulkr-0.7.0/tests/minecraft/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/minecraft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.638883 shulkr-0.7.0/tests/minecraft/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/minecraft/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1175 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/minecraft/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3715 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/minecraft/unit/test_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     3840 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/minecraft/unit/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.638883 shulkr-0.7.0/tests/mint/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/mint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.638883 shulkr-0.7.0/tests/mint/smoke/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/mint/smoke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/mint/smoke/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/mint/smoke/test_command.py
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/mint/smoke/test_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.638883 shulkr-0.7.0/tests/mint/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/mint/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2848 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/mint/unit/test_command.py
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/mint/unit/test_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.638883 shulkr-0.7.0/tests/shulkr/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/shulkr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.638883 shulkr-0.7.0/tests/shulkr/functional/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/shulkr/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2087 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/shulkr/functional/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.638883 shulkr-0.7.0/tests/shulkr/functional/minecraft/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/shulkr/functional/minecraft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/shulkr/functional/minecraft/test_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      782 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/shulkr/functional/test_file_system.py
--rw-r--r--   0 runner    (1001) docker     (121)     1942 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/shulkr/functional/test_git.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.642883 shulkr-0.7.0/tests/shulkr/profile/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/shulkr/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/shulkr/profile/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/shulkr/profile/profile_java.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.642883 shulkr-0.7.0/tests/shulkr/smoke/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/shulkr/smoke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/shulkr/smoke/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/shulkr/smoke/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 07:30:44.642883 shulkr-0.7.0/tests/shulkr/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/shulkr/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3460 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/shulkr/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3607 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/shulkr/unit/test_app.py
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/shulkr/unit/test_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (121)     3919 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/shulkr/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1323 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/shulkr/unit/test_gitignore.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/shulkr/unit/test_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     4349 2022-09-08 07:20:33.000000 shulkr-0.7.0/tests/shulkr/unit/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:55.375297 shulkr-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 03:21:28.000000 shulkr-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-09 03:21:55.375297 shulkr-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-09 03:21:28.000000 shulkr-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 03:21:55.375297 shulkr-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-09 03:21:28.000000 shulkr-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:55.371297 shulkr-0.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:55.371297 shulkr-0.7.1/src/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:55.371297 shulkr-0.7.1/src/gradle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/gradle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/gradle/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/gradle/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/gradle/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:55.371297 shulkr-0.7.1/src/java/
+-rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/java/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/java/blob.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:55.371297 shulkr-0.7.1/src/minecraft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/minecraft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/minecraft/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/minecraft/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:55.371297 shulkr-0.7.1/src/mint/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/mint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/mint/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/mint/repo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:55.371297 shulkr-0.7.1/src/shulkr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/shulkr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/shulkr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/shulkr/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/shulkr/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/shulkr/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/shulkr/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/shulkr/gitignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/shulkr/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-09 03:21:28.000000 shulkr-0.7.1/src/shulkr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 03:21:55.375297 shulkr-0.7.1/src/shulkr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-09 03:21:55.000000 shulkr-0.7.1/src/shulkr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-09 03:21:55.000000 shulkr-0.7.1/src/shulkr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 03:21:55.000000 shulkr-0.7.1/src/shulkr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-09 03:21:55.000000 shulkr-0.7.1/src/shulkr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-09 03:21:55.000000 shulkr-0.7.1/src/shulkr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-09 03:21:55.000000 shulkr-0.7.1/src/shulkr.egg-info/top_level.txt
```

### Comparing `shulkr-0.7.0/LICENSE` & `shulkr-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shulkr-0.7.0/PKG-INFO` & `shulkr-0.7.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: shulkr
-Version: 0.7.0
-Summary: Decompile multiple versions of Minecraft with a single command (for research)
+Version: 0.7.1
+Summary: Diff decompiled versions of Minecraft
 Home-page: https://github.com/clabe45/shulkr
 Author: Caleb Sacks
 License: GPLv3
 Keywords: minecraft,git,decompile,game
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: Utilities
@@ -125,29 +125,24 @@
 ## Experimental Options
 
 ### `--undo-renamed-vars` / `-u`
 
 When this option is enabled, local variables that were renamed in new versions
 will be reverted to their original names.
 
-## Contributing
+## Changelog
 
-Pull requests are welcome. For major changes, please open an issue first to
-discuss what you would like to change.
+See the [changelog].
 
-Please make sure to update tests as appropriate.
+## Contributing
 
-At a high-level, shulkr does the following for each version of Minecraft
-resolved from the supplied version patterns:
-1. Generate the source code using [DecompilerMC]
-2. Commit the version to git
-3. Optionally, tag the version
+See the [contributing guide].
 
 ## License
 
 Licensed under the Apache License, Version 2.0.
 
 [yarn's]: https://github.com/FabricMC/yarn
 [Fork]: https://github.com/clabe45/shulkr/fork
-[changelog]: https://github.com/clabe45/shulkr/blob/main/docs/changelog.md
-[usage guidelines]: https://github.com/clabe45/shulkr/blob/main/docs/usage-guidelines.md
-[DecompilerMC]: https://github.com/hube12/DecompilerMC
+[changelog]: ./docs/changelog.md
+[usage guidelines]: ./docs/usage-guidelines.md
+[contributing guide]: ./docs/contributing.md
```

### Comparing `shulkr-0.7.0/README.md` & `shulkr-0.7.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -102,29 +102,24 @@
 ## Experimental Options
 
 ### `--undo-renamed-vars` / `-u`
 
 When this option is enabled, local variables that were renamed in new versions
 will be reverted to their original names.
 
-## Contributing
+## Changelog
 
-Pull requests are welcome. For major changes, please open an issue first to
-discuss what you would like to change.
+See the [changelog].
 
-Please make sure to update tests as appropriate.
+## Contributing
 
-At a high-level, shulkr does the following for each version of Minecraft
-resolved from the supplied version patterns:
-1. Generate the source code using [DecompilerMC]
-2. Commit the version to git
-3. Optionally, tag the version
+See the [contributing guide].
 
 ## License
 
 Licensed under the Apache License, Version 2.0.
 
 [yarn's]: https://github.com/FabricMC/yarn
 [Fork]: https://github.com/clabe45/shulkr/fork
-[changelog]: https://github.com/clabe45/shulkr/blob/main/docs/changelog.md
-[usage guidelines]: https://github.com/clabe45/shulkr/blob/main/docs/usage-guidelines.md
-[DecompilerMC]: https://github.com/hube12/DecompilerMC
+[changelog]: ./docs/changelog.md
+[usage guidelines]: ./docs/usage-guidelines.md
+[contributing guide]: ./docs/contributing.md
```

### Comparing `shulkr-0.7.0/java/__init__.py` & `shulkr-0.7.1/src/java/__init__.py`

 * *Files identical despite different names*

### Comparing `shulkr-0.7.0/minecraft/source.py` & `shulkr-0.7.1/src/minecraft/source.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import shutil
 import subprocess
 
 import click
 
+from gradle.project import Project
 from mint.repo import Repo
 
 from minecraft.version import Version
 
 
 DECOMPILER_MC_REMOTE_URL = 'https://github.com/hube12/DecompilerMC.git'
 YARN_REMOTE_URL = 'https://github.com/FabricMC/yarn.git'
@@ -22,15 +23,20 @@
 	else:
 		# Clone the yarn repo
 		click.echo(f'Cloning {remote_url} into {local_dir}')
 		return Repo.clone(remote_url, local_dir)
 
 
 def _generate_sources_with_yarn(version: Version, path: str) -> None:
-	decompiler_path = os.path.join(path, '.yarn')
+	# Remove decompiler generated by previous versions of shulkr
+	old_decompiler_path = os.path.join(path, '.yarn')
+	if os.path.exists(old_decompiler_path):
+		shutil.rmtree(old_decompiler_path)
+
+	decompiler_path = os.path.join(path, 'yarn')
 	decompiler_repo = _setup_decompiler(decompiler_path, YARN_REMOTE_URL)
 
 	click.echo(f'Updating mappings to version {version}')
 
 	# Get latest versions from remote
 	decompiler_repo.git.fetch(prune=True)
 
@@ -39,24 +45,19 @@
 
 	# Checkout version branch
 	decompiler_repo.git.checkout(f'origin/{version}')
 
 	click.echo('Running decompiler')
 
 	# Generate source code
-	gradlew_file_name = 'gradlew.bat' if os.name == 'nt' else 'gradlew'
-	gradlew_exec = os.path.join(decompiler_repo.path, gradlew_file_name)
-	p = subprocess.run(
-		[gradlew_exec, 'decompileCFR'],
-		stdout=subprocess.DEVNULL,
-		stderr=subprocess.PIPE,
-		cwd=decompiler_repo.path
-	)
-	if p.returncode != 0:
-		raise Exception(p.stderr.decode())
+	# Create gradle project
+	decompiler_project = Project(decompiler_repo.path)
+
+	# Call gradle task to generate sources
+	decompiler_project.gradle.decompileCFR()
 
 	click.echo('Moving generated sources')
 
 	src_path = os.path.join(path, 'src')
 
 	# Remove existing top-level destination directory
 	if os.path.exists(src_path):
@@ -77,15 +78,20 @@
 	Args:
 		version (Version):
 
 	Raises:
 		Exception: If DecompilerMC fails
 	"""
 
-	decompiler_path = os.path.join(path, '.DecompilerMC')
+	# Remove decompiler generated by previous versions of shulkr
+	old_decompiler_path = os.path.join(path, '.DecompilerMC')
+	if os.path.exists(old_decompiler_path):
+		shutil.rmtree(old_decompiler_path)
+
+	decompiler_path = os.path.join(path, 'DecompilerMC')
 	decompiler_repo = _setup_decompiler(decompiler_path, DECOMPILER_MC_REMOTE_URL)
 
 	click.echo('Running decompiler')
 
 	# Decompile client
 	p = subprocess.run(
 		[
```

### Comparing `shulkr-0.7.0/minecraft/version.py` & `shulkr-0.7.1/src/minecraft/version.py`

 * *Files identical despite different names*

### Comparing `shulkr-0.7.0/mint/command.py` & `shulkr-0.7.1/src/command/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,102 @@
 import os
+import shutil
 import subprocess
 from typing import Any, Dict, List
 
 
-class GitCommandError(Exception):
+class BaseCommandError(Exception):
+	pass
+
+
+class CommandError(BaseCommandError):
 	def __init__(self, command: str, stderr: str, *args: object) -> None:
 		super().__init__(*args)
 
 		self.command = command
 		self.stderr = stderr
 
 	def __str__(self) -> str:
 		return f'{self.command}:\n{self.stderr}'
 
 
-class GitCommand:
+class CommandNotFoundError(BaseCommandError):
+	def __init__(self, command: str, *args: object) -> None:
+		super().__init__(*args)
+
+		self.command = command
+
+	def __str__(self) -> str:
+		return f'Command not found: {self.command}'
+
+
+class Command:
 	"""
 	Context for running git commands
 
 	Sample usage:
 		git = GitCommand(PATH_TO_REPO)
 		if not git.status(porcelain=True):
 			git.commit(message='empty commit', allow_empty=True)
 
 	Currently, options that require an '=' between the key and the value must be
 	supplied as positional arguments:
 		git.log('--format=%B')
 	"""
 
-	def __init__(self, path: str = None) -> None:
-		if path is None:
-			path = os.getcwd()
+	def __init__(
+		self,
+		executabale: str,
+		working_dir: str = None,
+		capture_output: bool = True,
+		error=CommandError
+	) -> None:
+
+		if not shutil.which(executabale):
+			raise CommandNotFoundError(executabale)
+
+		self._executable = executabale
+
+		if working_dir is None:
+			working_dir = os.getcwd()
+
+		self._working_dir = working_dir
+		self._capture_output = capture_output
 
-		self._path = path
+		self._error = error
 
 	def _run_command(self, command: List[str]) -> str:
 		try:
 			proc = subprocess.run(
 				command,
-				cwd=self._path,
+				cwd=self._working_dir,
 				check=True,
-				capture_output=True,
+				capture_output=self._capture_output,
 				text=True
 			)
 
-			return proc.stdout.strip()
+			if self._capture_output:
+				return proc.stdout.strip()
 
 		except subprocess.CalledProcessError as e:
-			raise GitCommandError(
-				command,
-				e.stderr
-			)
+			# Convert the error to to the user-specified error type
+			raise self._error(command, e.stderr) from e
 
 	def __getattr__(self, name: str):
 		"""
 		Return the specified git subcommand as a function
 
 		Args:
 			name (str): Name of the subcommand
 		"""
 
 		def func(*args, **kwargs):
 			subcommand = name.replace('_', '-')
 
-			command = GitCommand._raw_command(
+			command = self._raw_command(
 				subcommand,
 				args,
 				kwargs
 			)
 			return self._run_command(command)
 
 		return func
@@ -83,20 +112,20 @@
 		elif value is False:
 			return []
 
 		else:
 			# Non-boolean value
 			return [f'{prefix}{option}', str(value)]
 
-	@staticmethod
 	def _raw_command(
+		self,
 		subcommand: str,
 		args: List[Any],
 		kwargs: Dict[str, Any]
 	) -> List[str]:
 
 		options = [
 			token for key, value in kwargs.items()
-			for token in GitCommand._format_option(key, value)
+			for token in Command._format_option(key, value)
 		]
 		args = [str(arg) for arg in args]
-		return ['git', subcommand, *options, *args]
+		return [self._executable, subcommand, *options, *args]
```

### Comparing `shulkr-0.7.0/mint/repo.py` & `shulkr-0.7.1/src/mint/repo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 import os
 
 import git
+from command import Command
 
-from mint.command import GitCommand
+from mint.error import GitError
 
 
 class NoSuchRepoError(Exception):
 	def __init__(self, path: str, *args: object) -> None:
 		super().__init__(*args)
 
 		self.path = path
@@ -35,15 +36,15 @@
 	"""
 
 	def __init__(self, path: str, check_path=True) -> None:
 		if check_path:
 			Repo._ensure_repo_path_is_valid(path)
 
 		self.path = path
-		self.git = GitCommand(path)
+		self.git = Command('git', working_dir=path, error=GitError)
 
 	def to_gitpython(self) -> git.Repo:
 		return git.Repo(self.path)
 
 	@staticmethod
 	def _ensure_repo_path_is_valid(path: str):
 		if not os.path.exists(path):
@@ -64,10 +65,10 @@
 
 		repo = Repo(path, check_path=False)
 		repo.git.init(**kwargs)
 		return repo
 
 	@staticmethod
 	def clone(remote: str, dest: str, **kwargs) -> Repo:
-		git = GitCommand()
+		git = Command('git', error=GitError)
 		git.clone(remote, dest, **kwargs)
 		return Repo(dest)
```

### Comparing `shulkr-0.7.0/setup.py` & `shulkr-0.7.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,42 @@
-from glob import glob
 import os.path
 from setuptools import find_packages, setup
-from typing import List
-
-
-def package_files(directory: str) -> List[str]:
-    paths = []
-    for (path, directories, filenames) in os.walk(directory):
-        for filename in filenames:
-            paths.append(os.path.join('..', path, filename))
-    return paths
 
 
 script_dir = os.path.dirname(os.path.realpath(__file__))
 with open(os.path.join(script_dir, 'README.md'), 'r') as f:
 	README = f.read()
 
 classifiers = [
-	'Development Status :: 2 - Pre-Alpha',
+	'Development Status :: 3 - Alpha',
 	'Environment :: Console',
 	'Intended Audience :: Developers',
 	'Intended Audience :: Science/Research',
-	'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
+	'License :: OSI Approved :: Apache Software License',
 	'Operating System :: OS Independent',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Topic :: Games/Entertainment',
 	'Topic :: Scientific/Engineering',
 	'Topic :: Software Development :: Version Control :: Git',
 	'Topic :: Utilities'
 ]
 
 setup(
 	name='shulkr',
-	version='0.7.0',
-	description='Decompile multiple versions of Minecraft with a single command (for research)',
+	version='0.7.1',
+	description='Diff decompiled versions of Minecraft',
 	long_description=README,
 	long_description_content_type='text/markdown',
 	url='https://github.com/clabe45/shulkr',
 	author='Caleb Sacks',
 	license='GPLv3',
 	classifiers=classifiers,
     keywords=['minecraft', 'git', 'decompile', 'game'],
-    packages=find_packages(exclude=['tests']),
+	package_dir={'': 'src'},
+    packages=find_packages(where='src'),
     py_modules=['colorama', 'java', 'minecraft', 'mint', 'shulkr'],
-	# include_package_data=True,
-	# package_data={'': package_files('shulkr/DecompilerMC')},
 	install_requires=['gitpython', 'javalang', 'unidiff', 'requests', 'toml', 'click'],
 	entry_points={
         'console_scripts': ['shulkr=shulkr.__main__:main']
     }
 )
```

### Comparing `shulkr-0.7.0/shulkr/app.py` & `shulkr-0.7.1/src/shulkr/app.py`

 * *Files identical despite different names*

### Comparing `shulkr-0.7.0/shulkr/cli.py` & `shulkr-0.7.1/src/shulkr/cli.py`

 * *Files identical despite different names*

### Comparing `shulkr-0.7.0/shulkr/config.py` & `shulkr-0.7.1/src/shulkr/config.py`

 * *Files identical despite different names*

### Comparing `shulkr-0.7.0/shulkr/gitignore.py` & `shulkr-0.7.1/src/shulkr/gitignore.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 def _create_gitignore() -> None:
 	click.echo('Creating gitignore')
 
 	repo = get_repo()
 
 	with open(_gitignore_path(), 'w+') as gitignore:
-		to_ignore = ['.yarn', '.DecompilerMC']
+		to_ignore = ['yarn', 'DecompilerMC']
 		gitignore.write('\n'.join(to_ignore) + '\n')
 
 	repo.git.add('.gitignore')
 	repo.git.commit(message='add .gitignore')
 
 
 def ensure_gitignore_exists() -> bool:
```

### Comparing `shulkr-0.7.0/shulkr/repo.py` & `shulkr-0.7.1/src/shulkr/repo.py`

 * *Files identical despite different names*

### Comparing `shulkr-0.7.0/shulkr/version.py` & `shulkr-0.7.1/src/shulkr/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import shutil
 
 import click
 from java import undo_renames
 from minecraft.source import generate_sources
 from minecraft.version import Version
-from mint.command import GitCommandError
+from mint.error import GitError
 
 from shulkr.config import get_config
 from shulkr.repo import get_repo
 
 
 def _commit_version(version: Version) -> None:
 	repo = get_repo()
@@ -97,15 +97,15 @@
 	try:
 		# List tags reachable by HEAD
 		repo.git.describe(tags=True)
 
 		# If we made it here, there is at least one tag.
 		return True
 
-	except GitCommandError as e:
+	except GitError as e:
 		if 'fatal: No names found, cannot describe anything.' in e.stderr:
 			return False
 
 		raise e
 
 
 def get_latest_generated_version() -> Version:
```

### Comparing `shulkr-0.7.0/shulkr.egg-info/PKG-INFO` & `shulkr-0.7.1/src/shulkr.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: shulkr
-Version: 0.7.0
-Summary: Decompile multiple versions of Minecraft with a single command (for research)
+Version: 0.7.1
+Summary: Diff decompiled versions of Minecraft
 Home-page: https://github.com/clabe45/shulkr
 Author: Caleb Sacks
 License: GPLv3
 Keywords: minecraft,git,decompile,game
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: Utilities
@@ -125,29 +125,24 @@
 ## Experimental Options
 
 ### `--undo-renamed-vars` / `-u`
 
 When this option is enabled, local variables that were renamed in new versions
 will be reverted to their original names.
 
-## Contributing
+## Changelog
 
-Pull requests are welcome. For major changes, please open an issue first to
-discuss what you would like to change.
+See the [changelog].
 
-Please make sure to update tests as appropriate.
+## Contributing
 
-At a high-level, shulkr does the following for each version of Minecraft
-resolved from the supplied version patterns:
-1. Generate the source code using [DecompilerMC]
-2. Commit the version to git
-3. Optionally, tag the version
+See the [contributing guide].
 
 ## License
 
 Licensed under the Apache License, Version 2.0.
 
 [yarn's]: https://github.com/FabricMC/yarn
 [Fork]: https://github.com/clabe45/shulkr/fork
-[changelog]: https://github.com/clabe45/shulkr/blob/main/docs/changelog.md
-[usage guidelines]: https://github.com/clabe45/shulkr/blob/main/docs/usage-guidelines.md
-[DecompilerMC]: https://github.com/hube12/DecompilerMC
+[changelog]: ./docs/changelog.md
+[usage guidelines]: ./docs/usage-guidelines.md
+[contributing guide]: ./docs/contributing.md
```

