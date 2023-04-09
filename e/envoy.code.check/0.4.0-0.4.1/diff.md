# Comparing `tmp/envoy.code.check-0.4.0.tar.gz` & `tmp/envoy.code.check-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envoy.code.check-0.4.0.tar", last modified: Sat Feb  4 18:54:25 2023, max compression
+gzip compressed data, was "envoy.code.check-0.4.1.tar", last modified: Sun Apr  9 17:23:52 2023, max compression
```

## Comparing `envoy.code.check-0.4.0.tar` & `envoy.code.check-0.4.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 18:54:25.982502 envoy.code.check-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-02-04 18:54:25.982502 envoy.code.check-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 18:54:25.978502 envoy.code.check-0.4.0/envoy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 18:54:25.978502 envoy.code.check-0.4.0/envoy/code/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 18:54:25.982502 envoy.code.check-0.4.0/envoy/code/check/
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy/code/check/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 18:54:25.982502 envoy.code.check-0.4.0/envoy/code/check/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy/code/check/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy/code/check/abstract/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy/code/check/abstract/changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    13710 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy/code/check/abstract/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy/code/check/abstract/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy/code/check/abstract/flake8.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy/code/check/abstract/glint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy/code/check/abstract/rst.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy/code/check/abstract/runtime_guards.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy/code/check/abstract/shellcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy/code/check/abstract/yamllint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy/code/check/abstract/yapf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy/code/check/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy/code/check/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy/code/check/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy/code/check/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy/code/check/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy/code/check/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 18:54:25.982502 envoy.code.check-0.4.0/envoy.code.check.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy.code.check.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy.code.check.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy.code.check.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy.code.check.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy.code.check.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy.code.check.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/envoy.code.check.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-04 18:54:25.982502 envoy.code.check-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-02-04 18:54:25.000000 envoy.code.check-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:23:52.621906 envoy.code.check-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-09 17:23:52.621906 envoy.code.check-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:23:52.617906 envoy.code.check-0.4.1/envoy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:23:52.617906 envoy.code.check-0.4.1/envoy/code/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:23:52.617906 envoy.code.check-0.4.1/envoy/code/check/
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:23:52.621906 envoy.code.check-0.4.1/envoy/code/check/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14358 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/flake8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/glint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/gofmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/runtime_guards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/shellcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/yamllint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/abstract/yapf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy/code/check/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 17:23:52.617906 envoy.code.check-0.4.1/envoy.code.check.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy.code.check.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy.code.check.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy.code.check.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy.code.check.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy.code.check.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy.code.check.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/envoy.code.check.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 17:23:52.621906 envoy.code.check-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-09 17:23:52.000000 envoy.code.check-0.4.1/setup.py
```

### Comparing `envoy.code.check-0.4.0/backend_shim.py` & `envoy.code.check-0.4.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.0/envoy/code/check/__init__.py` & `envoy.code.check-0.4.1/envoy/code/check/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     AChangelogStatus,
     ACodeCheck,
     ACodeChecker,
     AExtensionsCheck,
     AFlake8Check,
     AFileCodeCheck,
     AGlintCheck,
+    AGofmtCheck,
     AProjectCodeCheck,
     APunctuationCheck,
     AReflinksCheck,
     ARuntimeGuardsCheck,
     AShellcheckCheck,
     AYamllintCheck,
     AYapfCheck)
@@ -22,14 +23,15 @@
     ChangelogChangesChecker,
     ChangelogCheck,
     ChangelogStatus,
     CodeChecker,
     ExtensionsCheck,
     Flake8Check,
     GlintCheck,
+    GofmtCheck,
     RuntimeGuardsCheck,
     ShellcheckCheck,
     YamllintCheck,
     YapfCheck)
 from .cmd import run, main
 from . import checker, interface
 
@@ -42,14 +44,15 @@
     "AChangelogStatus",
     "ACodeCheck",
     "ACodeChecker",
     "AExtensionsCheck",
     "AFileCodeCheck",
     "AFlake8Check",
     "AGlintCheck",
+    "AGofmtCheck",
     "AProjectCodeCheck",
     "APunctuationCheck",
     "AReflinksCheck",
     "ARuntimeGuardsCheck",
     "AShellcheckCheck",
     "AYamllintCheck",
     "AYapfCheck",
@@ -58,14 +61,15 @@
     "ChangelogStatus",
     "checker",
     "CodeChecker",
     "exceptions",
     "ExtensionsCheck",
     "Flake8Check",
     "GlintCheck",
+    "GofmtCheck",
     "interface",
     "main",
     "run",
     "main",
     "run",
     "RuntimeGuardsCheck",
     "ShellcheckCheck",
```

### Comparing `envoy.code.check-0.4.0/envoy/code/check/abstract/__init__.py` & `envoy.code.check-0.4.1/envoy/code/check/abstract/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,28 +4,30 @@
     AChangelogCheck,
     AChangelogChangesChecker,
     AChangelogStatus)
 from .checker import ACodeChecker
 from .extensions import AExtensionsCheck
 from .flake8 import AFlake8Check
 from .glint import AGlintCheck
+from .gofmt import AGofmtCheck
 from .rst import (
     ABackticksCheck,
     APunctuationCheck,
     AReflinksCheck)
 from .runtime_guards import ARuntimeGuardsCheck
 from .shellcheck import AShellcheckCheck
 from .yamllint import AYamllintCheck
 from .yapf import AYapfCheck
 from . import (
     base,
     checker,
     extensions,
     flake8,
     glint,
+    gofmt,
     shellcheck,
     changelog,
     yamllint,
     yapf)
 
 
 __all__ = (
@@ -35,23 +37,25 @@
     "AChangelogStatus",
     "ACodeCheck",
     "ACodeChecker",
     "AExtensionsCheck",
     "AFileCodeCheck",
     "AFlake8Check",
     "AGlintCheck",
+    "AGofmtCheck",
     "AProjectCodeCheck",
     "APunctuationCheck",
     "AReflinksCheck",
     "ARuntimeGuardsCheck",
     "AShellcheckCheck",
     "AYamllintCheck",
     "AYapfCheck",
     "base",
     "checker",
     "flake8",
     "glint",
+    "gofmt",
     "extensions",
     "shellcheck",
     "changelog",
     "yamllint",
     "yapf")
```

### Comparing `envoy.code.check-0.4.0/envoy/code/check/abstract/base.py` & `envoy.code.check-0.4.1/envoy/code/check/abstract/base.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.0/envoy/code/check/abstract/changelog.py` & `envoy.code.check-0.4.1/envoy/code/check/abstract/changelog.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.0/envoy/code/check/abstract/checker.py` & `envoy.code.check-0.4.1/envoy/code/check/abstract/checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
     checks = (
         "changelog",
         "extensions_fuzzed",
         "extensions_metadata",
         "extensions_registered",
         "glint",
+        "gofmt",
         "python_yapf",
         "python_flake8",
         "runtime_guards",
         "shellcheck",
         "yamllint")
 
     @property
@@ -163,14 +164,24 @@
         return self.glint_class(self.directory, **self.check_kwargs)
 
     @property  # type:ignore
     @abstracts.interfacemethod
     def glint_class(self) -> Type["interface.IGlintCheck"]:
         raise NotImplementedError
 
+    @cached_property
+    def gofmt(self) -> "interface.IGofmtCheck":
+        """Gofmt checker."""
+        return self.gofmt_class(self.directory, **self.check_kwargs)
+
+    @property  # type:ignore
+    @abstracts.interfacemethod
+    def gofmt_class(self) -> Type["interface.IGofmtCheck"]:
+        raise NotImplementedError
+
     @property
     def grep_excluding_re(self) -> Optional[Pattern[str]]:
         return self._grep_re(self.args.excluding)
 
     @property
     def grep_matching_re(self) -> Optional[Pattern[str]]:
         return self._grep_re(self.args.matching)
@@ -285,14 +296,18 @@
                 "extensions_registered",
                 ["Registered metadata matches found extensions"])
 
     async def check_glint(self) -> None:
         """Check for glint issues."""
         await self._code_check(self.glint)
 
+    async def check_gofmt(self) -> None:
+        """Check for gofmt issues."""
+        await self._code_check(self.gofmt)
+
     # TODO: catch errors in checkers as well as preloaders
     async def check_python_flake8(self) -> None:
         """Check for flake8 issues."""
         await self._code_check(self.flake8)
 
     async def check_python_yapf(self) -> None:
         """Check for yapf issues."""
@@ -349,14 +364,20 @@
     @checker.preload(
         when=["glint"],
         catches=[subprocess.exceptions.OSCommandError])
     async def preload_glint(self) -> None:
         await self.glint.problem_files
 
     @checker.preload(
+        when=["gofmt"],
+        catches=[subprocess.exceptions.OSCommandError])
+    async def preload_gofmt(self) -> None:
+        await self.gofmt.problem_files
+
+    @checker.preload(
         when=["shellcheck"],
         catches=[subprocess.exceptions.OSCommandError])
     async def preload_shellcheck(self) -> None:
         await self.shellcheck.problem_files
 
     @checker.preload(
         when=["runtime_guards"],
```

### Comparing `envoy.code.check-0.4.0/envoy/code/check/abstract/extensions.py` & `envoy.code.check-0.4.1/envoy/code/check/abstract/extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from functools import cached_property
 from typing import Any, cast, Dict, List, Pattern, Set, Tuple, Type, Union
 
 import yaml as _yaml
 
 import abstracts
 
+from aio.core import functional, utils
 from aio.core.functional import async_property
 
-from envoy.base import utils
 from envoy.code.check import abstract, exceptions, interface, typing
 
 
 logger = logging.getLogger(__name__)
 
 
 FILTER_NAMES_PATTERN = "NetworkFilterNames::get()"
@@ -235,15 +235,15 @@
             warn_message: str) -> Any:
         # Parse JSON, handling errors
         try:
             return utils.from_json(path, type)
         except (json.JSONDecodeError, FileNotFoundError) as e:
             raise exceptions.ExtensionsConfigurationError(
                 err_message.format(path=path, e=e))
-        except utils.TypeCastingError as e:
+        except functional.exceptions.TypeCastingError as e:
             logger.warning(warn_message.format(path=path, e=e))
             return e.value
 
     def _from_yaml(
             self,
             path: Union[str, pathlib.Path],
             type: Type,
@@ -251,21 +251,22 @@
             warn_message: str) -> Any:
         # Parse YAML, handling errors
         try:
             return utils.from_yaml(path, type)
         except (_yaml.reader.ReaderError, FileNotFoundError) as e:
             raise exceptions.ExtensionsConfigurationError(
                 err_message.format(path=path, e=e))
-        except utils.TypeCastingError as e:
+        except functional.exceptions.TypeCastingError as e:
             logger.warning(warn_message.format(path=path, e=e))
             return e.value
 
     async def _metadata(self, path) -> typing.ExtensionsMetadataDict:
+        errors = (functional.exceptions.TypeCastingError, FileNotFoundError)
         try:
             return await self.execute(
                 utils.from_yaml,
                 path,
                 typing.ExtensionsMetadataDict)
-        except (utils.exceptions.TypeCastingError, FileNotFoundError) as e:
+        except errors as e:
             raise exceptions.ExtensionsConfigurationError(
                 "Failed to parse extensions metadata "
                 f"({path}): {e}")
```

### Comparing `envoy.code.check-0.4.0/envoy/code/check/abstract/flake8.py` & `envoy.code.check-0.4.1/envoy/code/check/abstract/flake8.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.0/envoy/code/check/abstract/glint.py` & `envoy.code.check-0.4.1/envoy/code/check/abstract/glint.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.0/envoy/code/check/abstract/rst.py` & `envoy.code.check-0.4.1/envoy/code/check/abstract/rst.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.0/envoy/code/check/abstract/runtime_guards.py` & `envoy.code.check-0.4.1/envoy/code/check/abstract/runtime_guards.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.0/envoy/code/check/abstract/shellcheck.py` & `envoy.code.check-0.4.1/envoy/code/check/abstract/shellcheck.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.0/envoy/code/check/abstract/yamllint.py` & `envoy.code.check-0.4.1/envoy/code/check/abstract/yamllint.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.0/envoy/code/check/abstract/yapf.py` & `envoy.code.check-0.4.1/envoy/code/check/abstract/yapf.py`

 * *Files identical despite different names*

### Comparing `envoy.code.check-0.4.0/envoy/code/check/checker.py` & `envoy.code.check-0.4.1/envoy/code/check/checker.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,19 @@
 
 
 @abstracts.implementer(interface.IGlintCheck)
 class GlintCheck(abstract.AGlintCheck):
     pass
 
 
+@abstracts.implementer(interface.IGofmtCheck)
+class GofmtCheck(abstract.AGofmtCheck):
+    pass
+
+
 @abstracts.implementer(interface.IShellcheckCheck)
 class ShellcheckCheck(abstract.AShellcheckCheck):
     pass
 
 
 @abstracts.implementer(interface.IYapfCheck)
 class YapfCheck(abstract.AYapfCheck):
@@ -109,14 +114,18 @@
     def git_directory_class(self):
         return directory.GitDirectory
 
     @property
     def glint_class(self):
         return GlintCheck
 
+    @property
+    def gofmt_class(self):
+        return GofmtCheck
+
     @cached_property
     def path(self) -> pathlib.Path:
         return super().path
 
     @property
     def project_class(self) -> Type[IProject]:
         return Project
```

### Comparing `envoy.code.check-0.4.0/envoy/code/check/interface.py` & `envoy.code.check-0.4.1/envoy/code/check/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,18 @@
     pass
 
 
 class IGlintCheck(IFileCodeCheck, metaclass=abstracts.Interface):
     pass
 
 
+class IGofmtCheck(IFileCodeCheck, metaclass=abstracts.Interface):
+    pass
+
+
 class IShellcheckCheck(IFileCodeCheck, metaclass=abstracts.Interface):
     pass
 
 
 class IYamllintCheck(IFileCodeCheck, metaclass=abstracts.Interface):
     pass
```

### Comparing `envoy.code.check-0.4.0/envoy/code/check/typing.py` & `envoy.code.check-0.4.1/envoy/code/check/typing.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 YamllintProblemTuple = Tuple[str, checker.interface.IProblems]
 
 YapfProblemTuple = Tuple[str, checker.interface.IProblems]
 YapfResultTuple = Tuple[str, str, bool]
 YapfCheckResultTuple = Tuple[str, YapfResultTuple]
 
+GofmtProblemTuple = Tuple[str, checker.interface.IProblems]
+
 
 class BaseExtensionMetadataDict(TypedDict):
     categories: List[str]
     security_posture: str
     status: str
```

### Comparing `envoy.code.check-0.4.0/envoy.code.check.egg-info/SOURCES.txt` & `envoy.code.check-0.4.1/envoy.code.check.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,12 +18,13 @@
 envoy/code/check/abstract/__init__.py
 envoy/code/check/abstract/base.py
 envoy/code/check/abstract/changelog.py
 envoy/code/check/abstract/checker.py
 envoy/code/check/abstract/extensions.py
 envoy/code/check/abstract/flake8.py
 envoy/code/check/abstract/glint.py
+envoy/code/check/abstract/gofmt.py
 envoy/code/check/abstract/rst.py
 envoy/code/check/abstract/runtime_guards.py
 envoy/code/check/abstract/shellcheck.py
 envoy/code/check/abstract/yamllint.py
 envoy/code/check/abstract/yapf.py
```

### Comparing `envoy.code.check-0.4.0/setup.py` & `envoy.code.check-0.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'entry_points': {
         'console_scripts': [
             'envoy.code.check=envoy.code.check:run',
         ],
     },
     'install_requires': (
         'abstracts>=0.0.12',
-        'aio.core>=0.9.1',
+        'aio.core>=0.10.0',
         'aio.run.checker>=0.5.7',
         'envoy.base.utils>=0.4.1',
         'flake8>=6',
         'packaging>=23.0',
         'yamllint',
         'yapf',
     ),
@@ -42,9 +42,9 @@
     },
     'packages': (
         'envoy.code.check',
         'envoy.code.check.abstract',
     ),
     'python_requires': '>=3.10.0',
     'url': 'https://github.com/envoyproxy/pytooling/tree/main/envoy.code.check',
-    'version': '0.4.0',
+    'version': '0.4.1',
 })
```

