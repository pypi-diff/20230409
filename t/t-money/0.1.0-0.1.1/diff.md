# Comparing `tmp/t_money-0.1.0.tar.gz` & `tmp/t_money-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t_money-0.1.0.tar", max compression
+gzip compressed data, was "t_money-0.1.1.tar", max compression
```

## Comparing `t_money-0.1.0.tar` & `t_money-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     7048 2023-04-09 19:47:55.609852 t_money-0.1.0/LICENSE
--rw-r--r--   0        0        0     1069 2023-04-09 20:49:37.437534 t_money-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2668 2023-04-09 20:23:38.186847 t_money-0.1.0/src/t_money.py
--rw-r--r--   0        0        0      623 2023-04-09 20:49:42.622174 t_money-0.1.0/setup.py
--rw-r--r--   0        0        0      951 2023-04-09 20:49:42.622343 t_money-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7048 2023-04-09 19:47:55.609852 t_money-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1970 2023-04-09 20:54:05.445094 t_money-0.1.1/README.md
+-rw-r--r--   0        0        0     1106 2023-04-09 20:55:25.485999 t_money-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2668 2023-04-09 20:23:38.186847 t_money-0.1.1/src/t_money.py
+-rw-r--r--   0        0        0     2677 2023-04-09 20:55:27.453349 t_money-0.1.1/setup.py
+-rw-r--r--   0        0        0     2963 2023-04-09 20:55:27.453566 t_money-0.1.1/PKG-INFO
```

### Comparing `t_money-0.1.0/LICENSE` & `t_money-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `t_money-0.1.0/pyproject.toml` & `t_money-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "t_money"
-version = "0.1.0"
+version = "0.1.1"
 description = "Advanced Python 3.10 Dataclass for handling monetary values, keeping amount and currency together"
 authors = ["Jordan Dimov <jdimov@a115.co.uk>"]
 license = "Creative Commons"
 homepage = "https://github.com/jordan-dimov/t_money"
 repository = "https://github.com/jordan-dimov/t_money"
 # documentation = "https://t_money.readthedocs.io/"
 keywords = ["money", "currency", "finance", "accounting"]
@@ -14,19 +14,21 @@
     "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.10",
     "Topic :: Office/Business :: Financial",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
+readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 pytest = "^7.3.0"
+m2r2 = "^0.3.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `t_money-0.1.0/src/t_money.py` & `t_money-0.1.1/src/t_money.py`

 * *Files identical despite different names*

