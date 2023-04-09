# Comparing `tmp/Goosu-0.2.tar.gz` & `tmp/Goosu-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Goosu-0.2.tar", last modified: Sun Apr  9 08:07:00 2023, max compression
+gzip compressed data, was "Goosu-0.3.tar", last modified: Sun Apr  9 08:09:45 2023, max compression
```

## Comparing `Goosu-0.2.tar` & `Goosu-0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 aleksejmetlusko   (501) staff       (20)        0 2023-04-09 08:07:00.549874 Goosu-0.2/
-drwxr-xr-x   0 aleksejmetlusko   (501) staff       (20)        0 2023-04-09 08:07:00.549087 Goosu-0.2/Goosu/
--rw-r--r--   0 aleksejmetlusko   (501) staff       (20)      539 2023-04-09 07:20:49.000000 Goosu-0.2/Goosu/_init_.py
-drwxr-xr-x   0 aleksejmetlusko   (501) staff       (20)        0 2023-04-09 08:07:00.549792 Goosu-0.2/Goosu.egg-info/
--rw-r--r--   0 aleksejmetlusko   (501) staff       (20)      243 2023-04-09 08:07:00.000000 Goosu-0.2/Goosu.egg-info/PKG-INFO
--rw-r--r--   0 aleksejmetlusko   (501) staff       (20)      178 2023-04-09 08:07:00.000000 Goosu-0.2/Goosu.egg-info/SOURCES.txt
--rw-r--r--   0 aleksejmetlusko   (501) staff       (20)        1 2023-04-09 08:07:00.000000 Goosu-0.2/Goosu.egg-info/dependency_links.txt
--rw-r--r--   0 aleksejmetlusko   (501) staff       (20)        9 2023-04-09 08:07:00.000000 Goosu-0.2/Goosu.egg-info/requires.txt
--rw-r--r--   0 aleksejmetlusko   (501) staff       (20)        6 2023-04-09 08:07:00.000000 Goosu-0.2/Goosu.egg-info/top_level.txt
--rw-r--r--   0 aleksejmetlusko   (501) staff       (20)      243 2023-04-09 08:07:00.549922 Goosu-0.2/PKG-INFO
--rw-r--r--   0 aleksejmetlusko   (501) staff       (20)       38 2023-04-09 08:07:00.550107 Goosu-0.2/setup.cfg
--rw-r--r--   0 aleksejmetlusko   (501) staff       (20)      285 2023-04-09 08:06:54.000000 Goosu-0.2/setup.py
+drwxr-xr-x   0 aleksejmetlusko   (501) staff       (20)        0 2023-04-09 08:09:45.818826 Goosu-0.3/
+drwxr-xr-x   0 aleksejmetlusko   (501) staff       (20)        0 2023-04-09 08:09:45.818153 Goosu-0.3/Goosu/
+-rw-r--r--   0 aleksejmetlusko   (501) staff       (20)      427 2023-04-09 08:09:26.000000 Goosu-0.3/Goosu/_init_.py
+drwxr-xr-x   0 aleksejmetlusko   (501) staff       (20)        0 2023-04-09 08:09:45.818727 Goosu-0.3/Goosu.egg-info/
+-rw-r--r--   0 aleksejmetlusko   (501) staff       (20)      243 2023-04-09 08:09:45.000000 Goosu-0.3/Goosu.egg-info/PKG-INFO
+-rw-r--r--   0 aleksejmetlusko   (501) staff       (20)      178 2023-04-09 08:09:45.000000 Goosu-0.3/Goosu.egg-info/SOURCES.txt
+-rw-r--r--   0 aleksejmetlusko   (501) staff       (20)        1 2023-04-09 08:09:45.000000 Goosu-0.3/Goosu.egg-info/dependency_links.txt
+-rw-r--r--   0 aleksejmetlusko   (501) staff       (20)        9 2023-04-09 08:09:45.000000 Goosu-0.3/Goosu.egg-info/requires.txt
+-rw-r--r--   0 aleksejmetlusko   (501) staff       (20)        6 2023-04-09 08:09:45.000000 Goosu-0.3/Goosu.egg-info/top_level.txt
+-rw-r--r--   0 aleksejmetlusko   (501) staff       (20)      243 2023-04-09 08:09:45.818872 Goosu-0.3/PKG-INFO
+-rw-r--r--   0 aleksejmetlusko   (501) staff       (20)       38 2023-04-09 08:09:45.819049 Goosu-0.3/setup.cfg
+-rw-r--r--   0 aleksejmetlusko   (501) staff       (20)      285 2023-04-09 08:09:26.000000 Goosu-0.3/setup.py
```

