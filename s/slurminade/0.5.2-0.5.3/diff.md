# Comparing `tmp/slurminade-0.5.2.tar.gz` & `tmp/slurminade-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurminade-0.5.2.tar", last modified: Thu Oct 27 16:52:19 2022, max compression
+gzip compressed data, was "slurminade-0.5.3.tar", last modified: Sun Apr  9 12:42:00 2023, max compression
```

## Comparing `slurminade-0.5.2.tar` & `slurminade-0.5.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 16:52:19.008433 slurminade-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-10-27 16:52:12.000000 slurminade-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7900 2022-10-27 16:52:19.008433 slurminade-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7418 2022-10-27 16:52:12.000000 slurminade-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-27 16:52:12.000000 slurminade-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-27 16:52:19.008433 slurminade-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-10-27 16:52:12.000000 slurminade-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 16:52:19.004433 slurminade-0.5.2/slurminade/
--rw-r--r--   0 runner    (1001) docker     (121)     2113 2022-10-27 16:52:12.000000 slurminade-0.5.2/slurminade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3875 2022-10-27 16:52:12.000000 slurminade-0.5.2/slurminade/batch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-10-27 16:52:12.000000 slurminade-0.5.2/slurminade/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)    10982 2022-10-27 16:52:12.000000 slurminade-0.5.2/slurminade/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-10-27 16:52:12.000000 slurminade-0.5.2/slurminade/execute.py
--rw-r--r--   0 runner    (1001) docker     (121)     5302 2022-10-27 16:52:12.000000 slurminade-0.5.2/slurminade/function.py
--rw-r--r--   0 runner    (1001) docker     (121)     3824 2022-10-27 16:52:12.000000 slurminade-0.5.2/slurminade/function_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     2077 2022-10-27 16:52:12.000000 slurminade-0.5.2/slurminade/guard.py
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-10-27 16:52:12.000000 slurminade-0.5.2/slurminade/options.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 16:52:19.008433 slurminade-0.5.2/slurminade.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7900 2022-10-27 16:52:18.000000 slurminade-0.5.2/slurminade.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      444 2022-10-27 16:52:18.000000 slurminade-0.5.2/slurminade.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 16:52:18.000000 slurminade-0.5.2/slurminade.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 16:52:18.000000 slurminade-0.5.2/slurminade.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-27 16:52:18.000000 slurminade-0.5.2/slurminade.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-27 16:52:18.000000 slurminade-0.5.2/slurminade.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:42:00.976688 slurminade-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-09 12:41:57.000000 slurminade-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-04-09 12:42:00.972688 slurminade-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-04-09 12:41:57.000000 slurminade-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-09 12:41:57.000000 slurminade-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 12:42:00.976688 slurminade-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-09 12:41:57.000000 slurminade-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:42:00.972688 slurminade-0.5.3/slurminade/
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-09 12:41:57.000000 slurminade-0.5.3/slurminade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-09 12:41:57.000000 slurminade-0.5.3/slurminade/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-09 12:41:57.000000 slurminade-0.5.3/slurminade/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-04-09 12:41:57.000000 slurminade-0.5.3/slurminade/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-09 12:41:57.000000 slurminade-0.5.3/slurminade/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-09 12:41:57.000000 slurminade-0.5.3/slurminade/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-09 12:41:57.000000 slurminade-0.5.3/slurminade/function_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-09 12:41:57.000000 slurminade-0.5.3/slurminade/guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-09 12:41:57.000000 slurminade-0.5.3/slurminade/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:42:00.972688 slurminade-0.5.3/slurminade.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-04-09 12:42:00.000000 slurminade-0.5.3/slurminade.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-09 12:42:00.000000 slurminade-0.5.3/slurminade.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 12:42:00.000000 slurminade-0.5.3/slurminade.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 12:42:00.000000 slurminade-0.5.3/slurminade.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-09 12:42:00.000000 slurminade-0.5.3/slurminade.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 12:42:00.000000 slurminade-0.5.3/slurminade.egg-info/top_level.txt
```

### Comparing `slurminade-0.5.2/LICENSE` & `slurminade-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.2/PKG-INFO` & `slurminade-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurminade
-Version: 0.5.2
+Version: 0.5.3
 Summary: A decorator-based slurm runner
 Home-page: https://github.com/d-krupke/slurminade
 Author: Dominik Krupke
 Author-email: krupke@ibr.cs.tu-bs.de
 License: MIT
 Keywords: slurm
 Platform: UNKNOWN
@@ -206,20 +206,21 @@
 The project is reasonably easy:
 
 - batch.py: Contains code for bundling tasks, so we don't spam slurm with too many.
 - conf.py: Contains code for managing the configuration of slurm.
 - dispatcher.py: Contains code for actually dispatching tasks to slurm.
 - execute.py: Contains code to execute the task on the slurm node.
 - function.py: Contains the code for making a function slurm-compatible.
-- function_map.py: Saves all the slurified functions.
+- function_map.py: Saves all the slurmified functions.
 - guard.py: Contains code to prevent you accidentally DDoSing your infrastructure.
 - options.py: Contains a simple data structure to save slurm options.
 
 ## Changes
 
+* 0.5.3: Fixed a bug that caused the dispatch limit to have no effect.
 * 0.5.2: Added pyproject.toml for PEP compliance
 * 0.5.1: `Batch` will now flush on delete, in case you forgot.
 * 0.5.0:
   * Functions now have a `wait_for`-option and return job ids. 
   * Braking changes: Batches have a new API.
     * `add` is no longer needed.
     * `AutoBatch` is now called `Batch`.
```

### Comparing `slurminade-0.5.2/README.md` & `slurminade-0.5.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -189,20 +189,21 @@
 The project is reasonably easy:
 
 - batch.py: Contains code for bundling tasks, so we don't spam slurm with too many.
 - conf.py: Contains code for managing the configuration of slurm.
 - dispatcher.py: Contains code for actually dispatching tasks to slurm.
 - execute.py: Contains code to execute the task on the slurm node.
 - function.py: Contains the code for making a function slurm-compatible.
-- function_map.py: Saves all the slurified functions.
+- function_map.py: Saves all the slurmified functions.
 - guard.py: Contains code to prevent you accidentally DDoSing your infrastructure.
 - options.py: Contains a simple data structure to save slurm options.
 
 ## Changes
 
+* 0.5.3: Fixed a bug that caused the dispatch limit to have no effect.
 * 0.5.2: Added pyproject.toml for PEP compliance
 * 0.5.1: `Batch` will now flush on delete, in case you forgot.
 * 0.5.0:
   * Functions now have a `wait_for`-option and return job ids. 
   * Braking changes: Batches have a new API.
     * `add` is no longer needed.
     * `AutoBatch` is now called `Batch`.
```

### Comparing `slurminade-0.5.2/setup.py` & `slurminade-0.5.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open("README.md") as f:
         return f.read()
 
 
 setup(
     name="slurminade",
-    version="0.5.2",
+    version="0.5.3",
     description="A decorator-based slurm runner",
     long_description=readme(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

### Comparing `slurminade-0.5.2/slurminade/__init__.py` & `slurminade-0.5.3/slurminade/__init__.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.2/slurminade/batch.py` & `slurminade-0.5.3/slurminade/batch.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.2/slurminade/conf.py` & `slurminade-0.5.3/slurminade/conf.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.2/slurminade/dispatcher.py` & `slurminade-0.5.3/slurminade/dispatcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 import typing
 
 import simple_slurm
 
 from slurminade.conf import _get_conf
 from slurminade.function_map import FunctionMap, get_entry_point
+from slurminade.guard import dispatch_guard
 from slurminade.options import SlurmOptions
 
 
 class FunctionCall:
     """
     A function call to be dispatched.
     """
@@ -129,28 +130,31 @@
         self.calls = []
         self.sbatches = []
         self.sruns = []
 
     def _dispatch(
         self, funcs: typing.Iterable[FunctionCall], options: SlurmOptions
     ) -> int:
+        dispatch_guard()
         funcs = list(funcs)
         print(
             f"{sys.executable} -m slurminade.execute"
             f" {shlex.quote(get_entry_point())}"
             f" {shlex.quote(json.dumps([f.to_json() for f in funcs]))}"
         )
         self.calls.append(funcs)
         return -1
 
     def srun(self, command: str, conf: dict = None, simple_slurm_kwargs: dict = None):
+        dispatch_guard()
         self.sruns.append(command)
         print("SRUN", command)
 
     def sbatch(self, command: str, conf: dict = None, simple_slurm_kwargs: dict = None):
+        dispatch_guard()
         self.sbatches.append(command)
         print("SBATCH", command)
 
     def is_sequential(self):
         return True
 
 
@@ -168,30 +172,33 @@
         conf = _get_conf(special_slurm_opts)
         slurm = simple_slurm.Slurm(**conf)
         return slurm
 
     def _dispatch(
         self, funcs: typing.Iterable[FunctionCall], options: SlurmOptions
     ) -> int:
+        dispatch_guard()
         slurm = self._create_slurm_api(options)
         return slurm.sbatch(
             f"{sys.executable} -m slurminade.execute"
             f" {shlex.quote(get_entry_point())}"
             f" {shlex.quote(json.dumps([f.to_json() for f in funcs]))}"
         )
 
     def sbatch(self, command: str, conf: dict = None, simple_slurm_kwargs: dict = None):
+        dispatch_guard()
         conf = _get_conf(conf)
         slurm = simple_slurm.Slurm(**conf)
         if simple_slurm_kwargs:
             return slurm.sbatch(command, **simple_slurm_kwargs)
         else:
             return slurm.sbatch(command)
 
     def srun(self, command: str, conf: dict = None, simple_slurm_kwargs: dict = None):
+        dispatch_guard()
         conf = _get_conf(conf)
         slurm = simple_slurm.Slurm(**conf)
         if simple_slurm_kwargs:
             return slurm.srun(command, **simple_slurm_kwargs)
         else:
             return slurm.srun(command)
 
@@ -212,14 +219,15 @@
             f"{sys.executable} -m slurminade.execute"
             f" {shlex.quote(get_entry_point())}"
             f" {shlex.quote(json.dumps([f.to_json() for f in funcs]))}"
         )
         return -1
 
     def srun(self, command: str, conf: dict = None, simple_slurm_kwargs: dict = None):
+        dispatch_guard()
         subprocess.run(command, check=True)
 
     def sbatch(self, command: str, conf: dict = None, simple_slurm_kwargs: dict = None):
         self.srun(command)
 
     def is_sequential(self):
         return True
@@ -231,19 +239,21 @@
     This allows compatibility of scripts also on computers not integrated into
     the slurm network.
     """
 
     def _dispatch(
         self, funcs: typing.Iterable[FunctionCall], options: SlurmOptions
     ) -> int:
+        dispatch_guard()
         for func in funcs:
             FunctionMap.call(func.func_id, func.args, func.kwargs)
         return -1
 
     def srun(self, command: str, conf: dict = None, simple_slurm_kwargs: dict = None):
+        dispatch_guard()
         subprocess.run(command, check=True)
 
     def sbatch(self, command: str, conf: dict = None, simple_slurm_kwargs: dict = None):
         self.srun(command)
 
     def is_sequential(self):
         return True
```

### Comparing `slurminade-0.5.2/slurminade/execute.py` & `slurminade-0.5.3/slurminade/execute.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.2/slurminade/function.py` & `slurminade-0.5.3/slurminade/function.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.2/slurminade/function_map.py` & `slurminade-0.5.3/slurminade/function_map.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.2/slurminade/guard.py` & `slurminade-0.5.3/slurminade/guard.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.2/slurminade/options.py` & `slurminade-0.5.3/slurminade/options.py`

 * *Files identical despite different names*

### Comparing `slurminade-0.5.2/slurminade.egg-info/PKG-INFO` & `slurminade-0.5.3/slurminade.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurminade
-Version: 0.5.2
+Version: 0.5.3
 Summary: A decorator-based slurm runner
 Home-page: https://github.com/d-krupke/slurminade
 Author: Dominik Krupke
 Author-email: krupke@ibr.cs.tu-bs.de
 License: MIT
 Keywords: slurm
 Platform: UNKNOWN
@@ -206,20 +206,21 @@
 The project is reasonably easy:
 
 - batch.py: Contains code for bundling tasks, so we don't spam slurm with too many.
 - conf.py: Contains code for managing the configuration of slurm.
 - dispatcher.py: Contains code for actually dispatching tasks to slurm.
 - execute.py: Contains code to execute the task on the slurm node.
 - function.py: Contains the code for making a function slurm-compatible.
-- function_map.py: Saves all the slurified functions.
+- function_map.py: Saves all the slurmified functions.
 - guard.py: Contains code to prevent you accidentally DDoSing your infrastructure.
 - options.py: Contains a simple data structure to save slurm options.
 
 ## Changes
 
+* 0.5.3: Fixed a bug that caused the dispatch limit to have no effect.
 * 0.5.2: Added pyproject.toml for PEP compliance
 * 0.5.1: `Batch` will now flush on delete, in case you forgot.
 * 0.5.0:
   * Functions now have a `wait_for`-option and return job ids. 
   * Braking changes: Batches have a new API.
     * `add` is no longer needed.
     * `AutoBatch` is now called `Batch`.
```

