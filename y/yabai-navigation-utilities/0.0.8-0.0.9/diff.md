# Comparing `tmp/yabai_navigation_utilities-0.0.8.tar.gz` & `tmp/yabai_navigation_utilities-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yabai_navigation_utilities-0.0.8.tar", last modified: Mon Sep 12 21:34:36 2022, max compression
+gzip compressed data, was "yabai_navigation_utilities-0.0.9.tar", last modified: Tue Sep 13 03:39:01 2022, max compression
```

## Comparing `yabai_navigation_utilities-0.0.8.tar` & `yabai_navigation_utilities-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sendhil    (501) staff       (20)        0 2022-09-12 21:34:36.358761 yabai_navigation_utilities-0.0.8/
--rw-r--r--   0 sendhil    (501) staff       (20)      415 2022-09-12 21:34:36.358627 yabai_navigation_utilities-0.0.8/PKG-INFO
--rw-r--r--   0 sendhil    (501) staff       (20)     4352 2022-05-29 22:09:50.000000 yabai_navigation_utilities-0.0.8/README.md
--rw-r--r--   0 sendhil    (501) staff       (20)       38 2022-09-12 21:34:36.358801 yabai_navigation_utilities-0.0.8/setup.cfg
--rw-r--r--   0 sendhil    (501) staff       (20)      927 2022-09-12 21:34:29.000000 yabai_navigation_utilities-0.0.8/setup.py
-drwxr-xr-x   0 sendhil    (501) staff       (20)        0 2022-09-12 21:34:36.357653 yabai_navigation_utilities-0.0.8/yabai_navigation_utilities/
--rw-r--r--   0 sendhil    (501) staff       (20)        0 2022-05-29 22:09:50.000000 yabai_navigation_utilities-0.0.8/yabai_navigation_utilities/__init__.py
--rw-r--r--   0 sendhil    (501) staff       (20)       87 2022-05-29 23:19:04.000000 yabai_navigation_utilities-0.0.8/yabai_navigation_utilities/__main__.py
--rw-r--r--   0 sendhil    (501) staff       (20)     9061 2022-09-12 21:08:55.000000 yabai_navigation_utilities-0.0.8/yabai_navigation_utilities/cli.py
--rw-r--r--   0 sendhil    (501) staff       (20)     1034 2022-06-05 02:15:20.000000 yabai_navigation_utilities-0.0.8/yabai_navigation_utilities/config.py
-drwxr-xr-x   0 sendhil    (501) staff       (20)        0 2022-09-12 21:34:36.358450 yabai_navigation_utilities-0.0.8/yabai_navigation_utilities.egg-info/
--rw-r--r--   0 sendhil    (501) staff       (20)      415 2022-09-12 21:34:36.000000 yabai_navigation_utilities-0.0.8/yabai_navigation_utilities.egg-info/PKG-INFO
--rw-r--r--   0 sendhil    (501) staff       (20)      469 2022-09-12 21:34:36.000000 yabai_navigation_utilities-0.0.8/yabai_navigation_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 sendhil    (501) staff       (20)        1 2022-09-12 21:34:36.000000 yabai_navigation_utilities-0.0.8/yabai_navigation_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 sendhil    (501) staff       (20)       83 2022-09-12 21:34:36.000000 yabai_navigation_utilities-0.0.8/yabai_navigation_utilities.egg-info/entry_points.txt
--rw-r--r--   0 sendhil    (501) staff       (20)       13 2022-09-12 21:34:36.000000 yabai_navigation_utilities-0.0.8/yabai_navigation_utilities.egg-info/requires.txt
--rw-r--r--   0 sendhil    (501) staff       (20)       27 2022-09-12 21:34:36.000000 yabai_navigation_utilities-0.0.8/yabai_navigation_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 sendhil    (501) staff       (20)        0 2022-09-13 03:39:01.112105 yabai_navigation_utilities-0.0.9/
+-rw-r--r--   0 sendhil    (501) staff       (20)      415 2022-09-13 03:39:01.111978 yabai_navigation_utilities-0.0.9/PKG-INFO
+-rw-r--r--   0 sendhil    (501) staff       (20)     4352 2022-05-29 22:09:50.000000 yabai_navigation_utilities-0.0.9/README.md
+-rw-r--r--   0 sendhil    (501) staff       (20)       38 2022-09-13 03:39:01.112144 yabai_navigation_utilities-0.0.9/setup.cfg
+-rw-r--r--   0 sendhil    (501) staff       (20)      927 2022-09-13 03:38:46.000000 yabai_navigation_utilities-0.0.9/setup.py
+drwxr-xr-x   0 sendhil    (501) staff       (20)        0 2022-09-13 03:39:01.111060 yabai_navigation_utilities-0.0.9/yabai_navigation_utilities/
+-rw-r--r--   0 sendhil    (501) staff       (20)        0 2022-05-29 22:09:50.000000 yabai_navigation_utilities-0.0.9/yabai_navigation_utilities/__init__.py
+-rw-r--r--   0 sendhil    (501) staff       (20)       87 2022-05-29 23:19:04.000000 yabai_navigation_utilities-0.0.9/yabai_navigation_utilities/__main__.py
+-rw-r--r--   0 sendhil    (501) staff       (20)     8924 2022-09-12 21:37:27.000000 yabai_navigation_utilities-0.0.9/yabai_navigation_utilities/cli.py
+-rw-r--r--   0 sendhil    (501) staff       (20)     1034 2022-06-05 02:15:20.000000 yabai_navigation_utilities-0.0.9/yabai_navigation_utilities/config.py
+drwxr-xr-x   0 sendhil    (501) staff       (20)        0 2022-09-13 03:39:01.111805 yabai_navigation_utilities-0.0.9/yabai_navigation_utilities.egg-info/
+-rw-r--r--   0 sendhil    (501) staff       (20)      415 2022-09-13 03:39:00.000000 yabai_navigation_utilities-0.0.9/yabai_navigation_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 sendhil    (501) staff       (20)      469 2022-09-13 03:39:01.000000 yabai_navigation_utilities-0.0.9/yabai_navigation_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 sendhil    (501) staff       (20)        1 2022-09-13 03:39:00.000000 yabai_navigation_utilities-0.0.9/yabai_navigation_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 sendhil    (501) staff       (20)       83 2022-09-13 03:39:00.000000 yabai_navigation_utilities-0.0.9/yabai_navigation_utilities.egg-info/entry_points.txt
+-rw-r--r--   0 sendhil    (501) staff       (20)       13 2022-09-13 03:39:00.000000 yabai_navigation_utilities-0.0.9/yabai_navigation_utilities.egg-info/requires.txt
+-rw-r--r--   0 sendhil    (501) staff       (20)       27 2022-09-13 03:39:01.000000 yabai_navigation_utilities-0.0.9/yabai_navigation_utilities.egg-info/top_level.txt
```

### Comparing `yabai_navigation_utilities-0.0.8/README.md` & `yabai_navigation_utilities-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `yabai_navigation_utilities-0.0.8/setup.py` & `yabai_navigation_utilities-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='yabai_navigation_utilities',
     packages=find_packages(),
-    version='0.0.8',
+    version='0.0.9',
     description='Collection of scripts to make navigating Yabai easier.',
     author='Sendhil Panchadsaram',
     license='MIT',
     long_description=
     "A set of utilities to make navigating around Yabai(https://github.com/koekeishiya/yabai) easier. Details at https://github.com/sendhil/yabai-navigation-utilities.",
     install_requires=['click==8.1.3'],
     setup_requires=[],
```

### Comparing `yabai_navigation_utilities-0.0.8/yabai_navigation_utilities/cli.py` & `yabai_navigation_utilities-0.0.9/yabai_navigation_utilities/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,14 @@
 
 @dataclass
 class WindowDetails(object):
     window_id: int
     app: Optional[str]
     space_id: int
 
-    def __str__(self):
-        return json.dumps(dict(self), ensure_ascii=False)
-
-    def __repr__(self):
-        return self.__str__()
-
 
 @dataclass
 class WindowState(object):
     windows: List[WindowDetails]
     current_window_index: int
```

### Comparing `yabai_navigation_utilities-0.0.8/yabai_navigation_utilities/config.py` & `yabai_navigation_utilities-0.0.9/yabai_navigation_utilities/config.py`

 * *Files identical despite different names*

