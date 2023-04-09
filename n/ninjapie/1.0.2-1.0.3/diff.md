# Comparing `tmp/ninjapie-1.0.2.tar.gz` & `tmp/ninjapie-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninjapie-1.0.2.tar", last modified: Sun Apr  9 17:47:34 2023, max compression
+gzip compressed data, was "ninjapie-1.0.3.tar", last modified: Sun Apr  9 18:13:50 2023, max compression
```

## Comparing `ninjapie-1.0.2.tar` & `ninjapie-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-09 17:47:34.859796 ninjapie-1.0.2/
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    17987 2023-03-26 07:31:08.000000 ninjapie-1.0.2/LICENSE
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27518 2023-04-09 17:47:34.859796 ninjapie-1.0.2/PKG-INFO
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     6139 2023-04-09 11:30:25.000000 ninjapie-1.0.2/README.md
-drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-09 17:47:34.856462 ninjapie-1.0.2/ninjapie/
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)      158 2023-04-09 16:37:33.000000 ninjapie-1.0.2/ninjapie/__init__.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     4644 2023-04-09 15:55:05.000000 ninjapie-1.0.2/ninjapie/__main__.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27728 2023-04-09 16:36:42.000000 ninjapie-1.0.2/ninjapie/env.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    19340 2023-04-09 15:57:25.000000 ninjapie-1.0.2/ninjapie/generator.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     3894 2023-04-09 16:06:55.000000 ninjapie-1.0.2/ninjapie/path.py
-drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-09 17:47:34.859796 ninjapie-1.0.2/ninjapie.egg-info/
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27518 2023-04-09 17:47:34.000000 ninjapie-1.0.2/ninjapie.egg-info/PKG-INFO
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)      292 2023-04-09 17:47:34.000000 ninjapie-1.0.2/ninjapie.egg-info/SOURCES.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)        1 2023-04-09 17:47:34.000000 ninjapie-1.0.2/ninjapie.egg-info/dependency_links.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)       52 2023-04-09 17:47:34.000000 ninjapie-1.0.2/ninjapie.egg-info/entry_points.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)       14 2023-04-09 17:47:34.000000 ninjapie-1.0.2/ninjapie.egg-info/top_level.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     1339 2023-04-09 16:37:33.000000 ninjapie-1.0.2/pyproject.toml
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)       38 2023-04-09 17:47:34.859796 ninjapie-1.0.2/setup.cfg
+drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-09 18:13:50.010150 ninjapie-1.0.3/
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    17987 2023-03-26 07:31:08.000000 ninjapie-1.0.3/LICENSE
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27518 2023-04-09 18:13:50.010150 ninjapie-1.0.3/PKG-INFO
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     6139 2023-04-09 11:30:25.000000 ninjapie-1.0.3/README.md
+drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-09 18:13:50.006817 ninjapie-1.0.3/ninjapie/
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)      158 2023-04-09 18:13:41.000000 ninjapie-1.0.3/ninjapie/__init__.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     4644 2023-04-09 15:55:05.000000 ninjapie-1.0.3/ninjapie/__main__.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27728 2023-04-09 16:36:42.000000 ninjapie-1.0.3/ninjapie/env.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    19340 2023-04-09 15:57:25.000000 ninjapie-1.0.3/ninjapie/generator.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     3894 2023-04-09 16:06:55.000000 ninjapie-1.0.3/ninjapie/path.py
+drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-09 18:13:50.006817 ninjapie-1.0.3/ninjapie.egg-info/
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27518 2023-04-09 18:13:50.000000 ninjapie-1.0.3/ninjapie.egg-info/PKG-INFO
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)      292 2023-04-09 18:13:50.000000 ninjapie-1.0.3/ninjapie.egg-info/SOURCES.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)        1 2023-04-09 18:13:50.000000 ninjapie-1.0.3/ninjapie.egg-info/dependency_links.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       52 2023-04-09 18:13:50.000000 ninjapie-1.0.3/ninjapie.egg-info/entry_points.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       14 2023-04-09 18:13:50.000000 ninjapie-1.0.3/ninjapie.egg-info/top_level.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     1339 2023-04-09 18:13:41.000000 ninjapie-1.0.3/pyproject.toml
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       38 2023-04-09 18:13:50.010150 ninjapie-1.0.3/setup.cfg
```

### Comparing `ninjapie-1.0.2/LICENSE` & `ninjapie-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ninjapie-1.0.2/PKG-INFO` & `ninjapie-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjapie
-Version: 1.0.2
+Version: 1.0.3
 Summary: Ninja-based build system with a Python API
 Author-email: Nils Asmussen <nils.asmussen@barkhauseninstitut.org>
 License: 		    GNU GENERAL PUBLIC LICENSE
         		       Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -347,15 +347,15 @@
 Keywords: build system,ninja
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.5
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Ninjapie
 ========
 
 Ninjapie is a tool for automating the building of software. It builds upon [Ninja](https://ninja-build.org) and provides a Python API to describe the build. The basic idea is to take the flexibility and simplicity of [SCons](https://scons.org) and combine it with the performance of Ninja.
```

### Comparing `ninjapie-1.0.2/README.md` & `ninjapie-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ninjapie-1.0.2/ninjapie/__main__.py` & `ninjapie-1.0.3/ninjapie/__main__.py`

 * *Files identical despite different names*

### Comparing `ninjapie-1.0.2/ninjapie/env.py` & `ninjapie-1.0.3/ninjapie/env.py`

 * *Files identical despite different names*

### Comparing `ninjapie-1.0.2/ninjapie/generator.py` & `ninjapie-1.0.3/ninjapie/generator.py`

 * *Files identical despite different names*

### Comparing `ninjapie-1.0.2/ninjapie/path.py` & `ninjapie-1.0.3/ninjapie/path.py`

 * *Files identical despite different names*

### Comparing `ninjapie-1.0.2/ninjapie.egg-info/PKG-INFO` & `ninjapie-1.0.3/ninjapie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjapie
-Version: 1.0.2
+Version: 1.0.3
 Summary: Ninja-based build system with a Python API
 Author-email: Nils Asmussen <nils.asmussen@barkhauseninstitut.org>
 License: 		    GNU GENERAL PUBLIC LICENSE
         		       Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -347,15 +347,15 @@
 Keywords: build system,ninja
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.5
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Ninjapie
 ========
 
 Ninjapie is a tool for automating the building of software. It builds upon [Ninja](https://ninja-build.org) and provides a Python API to describe the build. The basic idea is to take the flexibility and simplicity of [SCons](https://scons.org) and combine it with the performance of Ninja.
```

### Comparing `ninjapie-1.0.2/pyproject.toml` & `ninjapie-1.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ninjapie"
-version = "1.0.2"
+version = "1.0.3"
 description = "Ninja-based build system with a Python API"
 readme = "README.md"
 authors = [{ name = "Nils Asmussen", email = "nils.asmussen@barkhauseninstitut.org" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["build system", "ninja"]
 dependencies = []
-requires-python = ">=3.5"
+requires-python = ">=3.9"
 
 [project.urls]
 Homepage = "https://github.com/Barkhausen-Institut/Ninjapie"
 
 [project.scripts]
 ninjapie = "ninjapie.__main__:main"
 
 [tool.setuptools]
 include-package-data = false
 
 [tool.setuptools.packages.find]
 exclude = ["coverage*", "tests*"]
 
 [tool.bumpver]
-current_version = "1.0.2"
+current_version = "1.0.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}."
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

