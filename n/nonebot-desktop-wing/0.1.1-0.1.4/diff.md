# Comparing `tmp/nonebot-desktop-wing-0.1.1.tar.gz` & `tmp/nonebot-desktop-wing-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-desktop-wing-0.1.1.tar", last modified: Sun Apr  9 10:54:48 2023, max compression
+gzip compressed data, was "nonebot-desktop-wing-0.1.4.tar", last modified: Sun Apr  9 11:55:51 2023, max compression
```

## Comparing `nonebot-desktop-wing-0.1.1.tar` & `nonebot-desktop-wing-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:54:48.836254 nonebot-desktop-wing-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-09 10:54:37.000000 nonebot-desktop-wing-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-09 10:54:48.832254 nonebot-desktop-wing-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-09 10:54:37.000000 nonebot-desktop-wing-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:54:48.832254 nonebot-desktop-wing-0.1.1/nonebot_desktop_wing/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-09 10:54:37.000000 nonebot-desktop-wing-0.1.1/nonebot_desktop_wing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-09 10:54:37.000000 nonebot-desktop-wing-0.1.1/nonebot_desktop_wing/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-09 10:54:37.000000 nonebot-desktop-wing-0.1.1/nonebot_desktop_wing/hindsight.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-09 10:54:37.000000 nonebot-desktop-wing-0.1.1/nonebot_desktop_wing/lazylib.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-09 10:54:37.000000 nonebot-desktop-wing-0.1.1/nonebot_desktop_wing/lazylib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-09 10:54:37.000000 nonebot-desktop-wing-0.1.1/nonebot_desktop_wing/molecules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-04-09 10:54:37.000000 nonebot-desktop-wing-0.1.1/nonebot_desktop_wing/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-09 10:54:37.000000 nonebot-desktop-wing-0.1.1/nonebot_desktop_wing/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:54:48.832254 nonebot-desktop-wing-0.1.1/nonebot_desktop_wing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-09 10:54:48.000000 nonebot-desktop-wing-0.1.1/nonebot_desktop_wing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-09 10:54:48.000000 nonebot-desktop-wing-0.1.1/nonebot_desktop_wing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 10:54:48.000000 nonebot-desktop-wing-0.1.1/nonebot_desktop_wing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-09 10:54:48.000000 nonebot-desktop-wing-0.1.1/nonebot_desktop_wing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-09 10:54:48.000000 nonebot-desktop-wing-0.1.1/nonebot_desktop_wing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-09 10:54:37.000000 nonebot-desktop-wing-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 10:54:48.836254 nonebot-desktop-wing-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:51.437413 nonebot-desktop-wing-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-09 11:55:51.437413 nonebot-desktop-wing-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:51.437413 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/hindsight.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/lazylib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/lazylib.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:55:51.437413 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-09 11:55:51.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-09 11:55:51.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 11:55:51.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-09 11:55:51.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-09 11:55:51.000000 nonebot-desktop-wing-0.1.4/nonebot_desktop_wing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-09 11:55:39.000000 nonebot-desktop-wing-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 11:55:51.437413 nonebot-desktop-wing-0.1.4/setup.cfg
```

### Comparing `nonebot-desktop-wing-0.1.1/LICENSE` & `nonebot-desktop-wing-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.1.1/PKG-INFO` & `nonebot-desktop-wing-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-desktop-wing
-Version: 0.1.1
+Version: 0.1.4
 Summary: Wings for NoneBot desktop applications.
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonedesktop/nonebot-desktop-wing
 Project-URL: Repository, https://github.com/nonedesktop/nonebot-desktop-wing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `nonebot-desktop-wing-0.1.1/README.md` & `nonebot-desktop-wing-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.1.1/nonebot_desktop_wing/__init__.py` & `nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.1.1/nonebot_desktop_wing/constants.py` & `nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/constants.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.1.1/nonebot_desktop_wing/hindsight.py` & `nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/hindsight.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.1.1/nonebot_desktop_wing/lazylib.py` & `nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/lazylib.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.1.1/nonebot_desktop_wing/lazylib.pyi` & `nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/lazylib.pyi`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.1.1/nonebot_desktop_wing/molecules.py` & `nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/molecules.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.1.1/nonebot_desktop_wing/project.py` & `nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/project.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.1.1/nonebot_desktop_wing/resources.py` & `nonebot-desktop-wing-0.1.4/nonebot_desktop_wing/resources.py`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.1.1/nonebot_desktop_wing.egg-info/PKG-INFO` & `nonebot-desktop-wing-0.1.4/nonebot_desktop_wing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-desktop-wing
-Version: 0.1.1
+Version: 0.1.4
 Summary: Wings for NoneBot desktop applications.
 Author-email: HivertMoZara <worldmozara@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonedesktop/nonebot-desktop-wing
 Project-URL: Repository, https://github.com/nonedesktop/nonebot-desktop-wing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `nonebot-desktop-wing-0.1.1/nonebot_desktop_wing.egg-info/SOURCES.txt` & `nonebot-desktop-wing-0.1.4/nonebot_desktop_wing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-desktop-wing-0.1.1/pyproject.toml` & `nonebot-desktop-wing-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-desktop-wing"
-version = "0.1.1"
+version = "0.1.4"
 description = "Wings for NoneBot desktop applications."
 authors = [
     {name = "HivertMoZara", email = "worldmozara@163.com"},
 ]
 license = {text = "MIT"}
 dependencies = ["nb_cli~=1.0.0", "python-dotenv~=1.0.0", "httpx>=0.23"]
 requires-python = ">=3.8"
```

