# Comparing `tmp/pdm_conda-0.7.1b0.tar.gz` & `tmp/pdm_conda-0.8.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_conda-0.7.1b0.tar", last modified: Tue Apr  4 20:48:37 2023, max compression
+gzip compressed data, was "pdm_conda-0.8.0b0.tar", last modified: Sun Apr  9 20:06:47 2023, max compression
```

## Comparing `pdm_conda-0.7.1b0.tar` & `pdm_conda-0.8.0b0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.7.1b0/LICENSE
--rw-r--r--   0        0        0     4545 2023-01-25 13:56:30.940438 pdm_conda-0.7.1b0/README.md
--rw-r--r--   0        0        0     1927 2023-04-04 20:48:38.324259 pdm_conda-0.7.1b0/pyproject.toml
--rw-r--r--   0        0        0      595 2023-04-04 20:48:29.030192 pdm_conda-0.7.1b0/src/pdm_conda/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.7.1b0/src/pdm_conda/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.7.1b0/src/pdm_conda/cli/commands/__init__.py
--rw-r--r--   0        0        0     2882 2023-04-04 17:40:11.935437 pdm_conda-0.7.1b0/src/pdm_conda/cli/commands/add.py
--rw-r--r--   0        0        0     1632 2023-01-17 20:25:57.041130 pdm_conda-0.7.1b0/src/pdm_conda/cli/commands/remove.py
--rw-r--r--   0        0        0     2009 2023-01-17 20:23:20.772922 pdm_conda-0.7.1b0/src/pdm_conda/cli/utils.py
--rw-r--r--   0        0        0    11106 2023-04-04 19:45:52.375656 pdm_conda-0.7.1b0/src/pdm_conda/conda.py
--rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.7.1b0/src/pdm_conda/installers/__init__.py
--rw-r--r--   0        0        0     1767 2023-03-29 14:37:48.378545 pdm_conda-0.7.1b0/src/pdm_conda/installers/manager.py
--rw-r--r--   0        0        0     1840 2023-04-04 18:32:51.656583 pdm_conda-0.7.1b0/src/pdm_conda/installers/synchronizers.py
--rw-r--r--   0        0        0     3132 2023-01-17 17:44:51.337923 pdm_conda-0.7.1b0/src/pdm_conda/mapping.py
--rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.7.1b0/src/pdm_conda/models/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.7.1b0/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
--rw-r--r--   0        0        0     6493 2023-04-04 03:59:08.190836 pdm_conda-0.7.1b0/src/pdm_conda/models/candidates.py
--rw-r--r--   0        0        0     6901 2023-04-04 18:55:59.440896 pdm_conda-0.7.1b0/src/pdm_conda/models/config.py
--rw-r--r--   0        0        0     2452 2023-03-29 14:37:48.384012 pdm_conda-0.7.1b0/src/pdm_conda/models/environment.py
--rw-r--r--   0        0        0     3775 2023-03-29 14:37:48.386011 pdm_conda-0.7.1b0/src/pdm_conda/models/repositories.py
--rw-r--r--   0        0        0     9162 2023-04-04 20:46:00.214416 pdm_conda-0.7.1b0/src/pdm_conda/models/requirements.py
--rw-r--r--   0        0        0      900 2023-04-04 03:59:08.192367 pdm_conda-0.7.1b0/src/pdm_conda/models/setup.py
--rw-r--r--   0        0        0     7313 2023-04-04 17:41:47.277165 pdm_conda-0.7.1b0/src/pdm_conda/project.py
--rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.7.1b0/src/pdm_conda/resolver/__init__.py
--rw-r--r--   0        0        0     1134 2023-02-23 00:47:35.312247 pdm_conda-0.7.1b0/src/pdm_conda/resolver/providers.py
--rw-r--r--   0        0        0     5113 2023-04-03 14:54:30.788827 pdm_conda-0.7.1b0/src/pdm_conda/resolvers.py
--rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.7.1b0/src/pdm_conda/utils.py
--rw-r--r--   0        0        0     6376 1970-01-01 00:00:00.000000 pdm_conda-0.7.1b0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.8.0b0/LICENSE
+-rw-r--r--   0        0        0     4827 2023-04-09 20:05:34.908555 pdm_conda-0.8.0b0/README.md
+-rw-r--r--   0        0        0     1927 2023-04-09 20:06:47.733625 pdm_conda-0.8.0b0/pyproject.toml
+-rw-r--r--   0        0        0      595 2023-04-09 20:06:03.212447 pdm_conda-0.8.0b0/src/pdm_conda/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.8.0b0/src/pdm_conda/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.8.0b0/src/pdm_conda/cli/commands/__init__.py
+-rw-r--r--   0        0        0     3219 2023-04-09 20:03:17.811169 pdm_conda-0.8.0b0/src/pdm_conda/cli/commands/add.py
+-rw-r--r--   0        0        0     1681 2023-04-09 18:24:04.763264 pdm_conda-0.8.0b0/src/pdm_conda/cli/commands/remove.py
+-rw-r--r--   0        0        0     2183 2023-04-09 18:47:54.197518 pdm_conda-0.8.0b0/src/pdm_conda/cli/utils.py
+-rw-r--r--   0        0        0    11001 2023-04-09 20:02:13.031492 pdm_conda-0.8.0b0/src/pdm_conda/conda.py
+-rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.8.0b0/src/pdm_conda/installers/__init__.py
+-rw-r--r--   0        0        0     2482 2023-04-09 19:02:43.417017 pdm_conda-0.8.0b0/src/pdm_conda/installers/manager.py
+-rw-r--r--   0        0        0     2130 2023-04-09 20:03:17.811387 pdm_conda-0.8.0b0/src/pdm_conda/installers/synchronizers.py
+-rw-r--r--   0        0        0     3132 2023-01-17 17:44:51.337923 pdm_conda-0.8.0b0/src/pdm_conda/mapping.py
+-rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.8.0b0/src/pdm_conda/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.8.0b0/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
+-rw-r--r--   0        0        0     6776 2023-04-09 18:57:52.527833 pdm_conda-0.8.0b0/src/pdm_conda/models/candidates.py
+-rw-r--r--   0        0        0     7145 2023-04-09 20:05:09.458459 pdm_conda-0.8.0b0/src/pdm_conda/models/config.py
+-rw-r--r--   0        0        0     3234 2023-04-09 18:57:09.987590 pdm_conda-0.8.0b0/src/pdm_conda/models/environment.py
+-rw-r--r--   0        0        0     3863 2023-04-09 20:03:17.811832 pdm_conda-0.8.0b0/src/pdm_conda/models/repositories.py
+-rw-r--r--   0        0        0     9046 2023-04-09 18:57:52.528315 pdm_conda-0.8.0b0/src/pdm_conda/models/requirements.py
+-rw-r--r--   0        0        0      900 2023-04-04 03:59:08.192367 pdm_conda-0.8.0b0/src/pdm_conda/models/setup.py
+-rw-r--r--   0        0        0     7518 2023-04-09 20:03:17.812051 pdm_conda-0.8.0b0/src/pdm_conda/project.py
+-rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.8.0b0/src/pdm_conda/resolver/__init__.py
+-rw-r--r--   0        0        0     1134 2023-02-23 00:47:35.312247 pdm_conda-0.8.0b0/src/pdm_conda/resolver/providers.py
+-rw-r--r--   0        0        0     5740 2023-04-09 20:03:17.812247 pdm_conda-0.8.0b0/src/pdm_conda/resolvers.py
+-rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.8.0b0/src/pdm_conda/utils.py
+-rw-r--r--   0        0        0     6658 1970-01-01 00:00:00.000000 pdm_conda-0.8.0b0/PKG-INFO
```

### Comparing `pdm_conda-0.7.1b0/LICENSE` & `pdm_conda-0.8.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.7.1b0/README.md` & `pdm_conda-0.8.0b0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # pdm-conda
 
 A PDM plugin to install project dependencies with Conda.
 
 ## Configuration
 
-| Config item                       | Description                                                                                        | Default value       | Possible values                | Environment variable        |
-|-----------------------------------|----------------------------------------------------------------------------------------------------|---------------------|--------------------------------|-----------------------------|
-| `conda.runner`                    | Conda runner executable                                                                            | `conda`             | `conda`, `mamba`, `micromamba` | `CONDA_RUNNER`              |
-| `conda.channels`                  | Conda channels to use, order will be enforced                                                      | `[]`                |                                |                             |
-| `conda.as-default-manager`        | Use Conda to install all possible requirements                                                     | `False`             |                                | `CONDA_AS_DEFAULT_MANAGER`  |
-| `conda.excluded`                  | Array of dependencies to exclude from Conda resolution                                             | `[]`                |                                |                             |
-| `conda.installation-method`       | Installation method to use when installing dependencies with Conda                                 | `hard-link`         | `hard-link`, `copy`            | `CONDA_INSTALLATION_METHOD` |
-| `conda.dependencies`              | Array of dependencies to install with Conda, analogue to `project.dependencies`                    | `[]`                |                                |                             |
-| `conda.optional-dependencies`     | Groups of optional dependencies to install with Conda, analogue to `project.optional-dependencies` | `{}`                |                                |                             |
-| `conda.dev-dependencies`          | Groups of development dependencies to install with Conda, analogue to `tool.pdm.dev-dependencies`  | `{}`                |                                |                             |
-| `conda.pypi-mapping.download-dir` | PyPI-Conda mapping download directory                                                              | `$HOME/.pdm-conda/` |                                | `PYPI_MAPPING_DIR`          |
+| Config item                       | Description                                                                                          | Default value       | Possible values                | Environment variable        |
+|-----------------------------------|------------------------------------------------------------------------------------------------------|---------------------|--------------------------------|-----------------------------|
+| `conda.runner`                    | Conda runner executable                                                                              | `conda`             | `conda`, `mamba`, `micromamba` | `CONDA_RUNNER`              |
+| `conda.channels`                  | Conda channels to use, order will be enforced                                                        | `[]`                |                                |                             |
+| `conda.as-default-manager`        | Use Conda to install all possible requirements                                                       | `False`             |                                | `CONDA_AS_DEFAULT_MANAGER`  |
+| `conda.use-batched`               | Execute batched install and remove Conda commands, when True the command is executed only at the end | `False`             |                                | `CONDA_BATCHED_COMMANDS`    |
+| `conda.excludes`                  | Array of dependencies to exclude from Conda resolution                                               | `[]`                |                                |                             |
+| `conda.installation-method`       | Installation method to use when installing dependencies with Conda                                   | `hard-link`         | `hard-link`, `copy`            | `CONDA_INSTALLATION_METHOD` |
+| `conda.dependencies`              | Array of dependencies to install with Conda, analogue to `project.dependencies`                      | `[]`                |                                |                             |
+| `conda.optional-dependencies`     | Groups of optional dependencies to install with Conda, analogue to `project.optional-dependencies`   | `{}`                |                                |                             |
+| `conda.dev-dependencies`          | Groups of development dependencies to install with Conda, analogue to `tool.pdm.dev-dependencies`    | `{}`                |                                |                             |
+| `conda.pypi-mapping.download-dir` | PyPI-Conda mapping download directory                                                                | `$HOME/.pdm-conda/` |                                | `PYPI_MAPPING_DIR`          |
 
 All configuration items use prefix `pdm.tool`, this is a viable configuration:
 
 ```toml
 [tool.pdm.conda]
 runner = "micromamba"
 channels = ["conda-forge/noarch", "conda-forge", "anaconda"]
 dependencies = ["pdm"]
 as-default-manager = true
-excluded = ["pytest-cov"] # don't install with conda even if it's a dependency from other packages
+excludes = ["pytest-cov"] # don't install with conda even if it's a dependency from other packages
 installation-method = "copy"
-
+use-batched = true
 
 [tool.pdm.conda.pypi-mapping]
 download-dir = "/tmp"
 
 [tool.pdm.conda.optional-dependencies]
 extra = ["anaconda:ffmpeg"] # non python dependency, obtained from anaconda channel
 
@@ -52,21 +53,22 @@
     * To add a Conda managed package `--conda` flag can be used multiple times followed a package (analogue
       to `--editable`).
     * You can specify per package Conda channel using conda notation `channel::package`.
     * You also can specify a default Conda channel with `-c` or `--channel`.
     * With flag `-r` or `--runner` you can specify the Conda runner to use.
 * `pdm remove`
 * `pdm list`
+* `pdm info`
 
 ### How it works
 
-When PDM detects a Conda managed package, it gets Candidates with Conda and then tries to resolve the environment as
+When PDM detects a Conda managed package, it gets candidates with Conda and then tries to resolve the environment as
 with any other requirement.
 
-To keep the resolution consistent with Conda, PDM uses resolution rules from Conda as good as possible.
+To keep the resolution consistent with Conda, PDM follows resolution rules from Conda as good as possible.
 
 ### Settings overriden
 
 In order to use Conda to install packages some settings were overriden:
 
 * `install.parallel` if some Conda managed packages are to be uninstalled or updated this option is disabled
   momentarily.
```

### Comparing `pdm_conda-0.7.1b0/pyproject.toml` & `pdm_conda-0.8.0b0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
     "pdm~=2.4.0",
     "requests>=2.28.1",
 ]
-version = "0.7.1b0"
+version = "0.8.0b0"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/macro128/pdm-conda"
 Changelog = "https://github.com/macro128/pdm-conda/blob/main/CHANGELOG.md"
```

### Comparing `pdm_conda-0.7.1b0/src/pdm_conda/__init__.py` & `pdm_conda-0.8.0b0/src/pdm_conda/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,8 +14,8 @@
     core.register_command(AddCommand)
     core.register_command(RemoveCommand)
 
     for name, config in CONFIGS:
         core.add_config(name, config)
 
 
-__version__ = "0.7.1b0"
+__version__ = "0.8.0b0"
```

### Comparing `pdm_conda-0.7.1b0/src/pdm_conda/cli/commands/add.py` & `pdm_conda-0.8.0b0/src/pdm_conda/cli/commands/add.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import argparse
 from typing import cast
 
 from pdm.cli.commands.add import Command as BaseCommand
 from pdm.cli.options import ArgumentGroup
+from pdm.exceptions import RequirementError
 
+from pdm_conda.cli.utils import remove_quotes
 from pdm_conda.models.requirements import CondaRequirement, parse_requirement
 from pdm_conda.project import CondaProject, Project
 
 conda_group = ArgumentGroup("Conda Arguments")
 conda_group.add_argument(
     "--conda",
     dest="conda_packages",
@@ -55,23 +57,29 @@
                 config.runner = options.conda_runner
             if channel and channel not in existing_channels:
                 existing_channels.append(channel)
                 config.channels = existing_channels
 
             for package in conda_packages:
                 package_channel = None
+                package = remove_quotes(package)
+
                 if "::" in package:
                     package_channel, package = package.split("conda:", maxsplit=1)[-1].split("::", maxsplit=1)
 
-                _p = parse_requirement(package)
-                if isinstance(_p, CondaRequirement):
-                    _p = _p.as_named_requirement()
+                try:
+                    _p = parse_requirement(package)
+                    if isinstance(_p, CondaRequirement):
+                        _p = _p.as_named_requirement()
+                except RequirementError:
+                    # if requirement error it can have an unparsable version
+                    _p = None
 
                 # if not named we can't use Conda
-                if _p.is_named and _p.name not in config.excluded:
+                if _p is None or (_p.is_named and _p.name not in config.excludes):
                     if package.startswith("conda:"):
                         package = package[len("conda:") :]
                     if not package_channel and channel:
                         package_channel = channel
 
                     if package_channel:
                         package = f"{package_channel}::{package}"
```

### Comparing `pdm_conda-0.7.1b0/src/pdm_conda/cli/commands/remove.py` & `pdm_conda-0.8.0b0/src/pdm_conda/cli/commands/remove.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 from typing import cast
 
 from pdm.cli.commands.remove import Command as BaseCommand
 
+from pdm_conda.cli.utils import remove_quotes
 from pdm_conda.models.requirements import parse_requirement
 from pdm_conda.project import CondaProject, Project
 
 
 class Command(BaseCommand):
     description = BaseCommand.__doc__
     name = "remove"
@@ -16,17 +17,17 @@
             options.group = "dev" if options.dev else "default"
 
         project = cast(CondaProject, project)
         conda_dependencies = project.get_conda_pyproject_dependencies(options.group, options.dev)
         dependencies, _ = project.get_pyproject_dependencies(options.group, options.dev)
         _dependencies = [parse_requirement(d).conda_name for d in dependencies]
         # add conda dependencies to common dependencies if going to remove it
-        for i in range(len(options.packages)):
+        for i, pkg in enumerate(options.packages):
             # parse it as conda, if found add it to dependencies
-            conda_package = f"conda:{options.packages[i]}"
+            conda_package = f"conda:{remove_quotes(pkg)}"
             package = parse_requirement(conda_package)
             idx = None
             for dep_idx, dep in enumerate(conda_dependencies):
                 dep = parse_requirement(f"conda:{dep}")
                 if package.name == dep.name:
                     if package.name not in _dependencies:
                         dependencies.append(conda_package)
```

### Comparing `pdm_conda-0.7.1b0/src/pdm_conda/cli/utils.py` & `pdm_conda-0.8.0b0/src/pdm_conda/cli/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,26 +5,33 @@
 from pdm.project import Project
 
 from pdm_conda.models.requirements import CondaRequirement
 
 _patched = False
 
 
+def remove_quotes(req: str) -> str:
+    for quote in ("'", '"'):
+        if req.startswith(quote) and req.endswith(quote):
+            req = req[1:-1]
+    return req
+
+
 def wrap_save_version_specifiers(func):
     @functools.wraps(func)
     def wrapper(
         requirements: dict[str, dict[str, Requirement]],
         resolved: dict[str, Candidate],
         save_strategy: str,
     ) -> None:
         func(requirements, resolved, save_strategy)
         for reqs in requirements.values():
             for name, r in reqs.items():
                 if isinstance(r, CondaRequirement):
-                    r.version_mapping = resolved[name].req.version_mapping
+                    r.version_mapping.update(resolved[name].req.version_mapping)
                     r.is_python_package = resolved[name].req.is_python_package
 
     return wrapper
 
 
 def wrap_format_lockfile(func):
     @functools.wraps(func)
```

### Comparing `pdm_conda-0.7.1b0/src/pdm_conda/conda.py` & `pdm_conda-0.8.0b0/src/pdm_conda/conda.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,33 @@
 import subprocess
 from functools import lru_cache
 from tempfile import NamedTemporaryFile
 from typing import Iterable
 from urllib.parse import urlparse
 
 from packaging.version import Version
+from pdm import termui
 from pdm.exceptions import RequirementError
 from pdm.models.setup import Setup
+from pdm.termui import Verbosity
 
 from pdm_conda.models.candidates import CondaCandidate
 from pdm_conda.models.config import CondaRunner
 from pdm_conda.models.requirements import (
     CondaRequirement,
     Requirement,
     parse_conda_version,
     parse_requirement,
 )
 from pdm_conda.models.setup import CondaSetupDistribution
 from pdm_conda.project import CondaProject
 from pdm_conda.utils import normalize_name
 
+logger = termui.logger
+
 
 @contextlib.contextmanager
 def _optional_temporary_file(environment: dict):
     if environment:
         with NamedTemporaryFile(mode="w+", suffix=".yml") as f:
             yield f
     else:
@@ -44,14 +48,17 @@
             for name, options in environment.items():
                 if options:
                     f.write(f"{name}:\n")
                     for v in options:
                         f.write(f"  - {v}\n")
             f.seek(0)
             cmd = cmd + ["-f", f.name]
+        logger.debug(f"cmd: {' '.join(cmd)}")
+        if environment:
+            logger.debug(f"env: {environment}")
         process = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, encoding="utf-8")
     if "--json" in cmd:
         try:
             response = json.loads(process.stdout)
         except:
             response = {}
     else:
@@ -78,46 +85,24 @@
     Sort packages following mamba specification
     (https://mamba.readthedocs.io/en/latest/advanced_usage/package_resolution.html).
     :param packages: list of conda packages
     :return: sorted conda packages
     """
     if len(packages) <= 1:
         return packages
-    _with_track_features = []
-    _sorted = []
-    _by_version: dict[str, list] = dict()
-
-    # get most recent version with timestamp
-    for p in packages:
-        _by_version.setdefault(p["version"], []).append(p)
-
-    name = packages[0].get("name", "")
-    # sort by version
-    for _, pkgs in sorted(
-        _by_version.items(),
-        key=lambda x: Version(parse_conda_version(x[0], inverse=name != "openssl")),
-    ):
-        # sort same version packages using build number
-        if len(pkgs) > 1:
-            _by_build_number: dict[int, list] = dict()
-            for p in pkgs:
-                _by_build_number.setdefault(p.get("build_number", 0), []).append(p)
-            pkgs.clear()
-            # sort same build number by timestamp
-            for n in sorted(_by_build_number.keys()):
-                pkgs.extend(sorted(_by_build_number[n], key=lambda p: p.get("timestamp", 0)))
-
-        # track_feature to bottom
-        for p in pkgs:
-            if p.get("track_feature", ""):
-                _with_track_features.append(p)
-            else:
-                _sorted.append(p)
 
-    return reversed(_with_track_features + _sorted)
+    def get_preference(package):
+        return (
+            not package.get("track_feature", ""),
+            Version(parse_conda_version(package["version"], inverse=package.get("name", "") == "openssl")),
+            package.get("build_number", 0),
+            package.get("timestamp", 0),
+        )
+
+    return sorted(packages, key=get_preference, reverse=True)
 
 
 @lru_cache(maxsize=None)
 def _conda_search(
     requirement: str,
     project: CondaProject,
     channels: tuple[str],
@@ -191,14 +176,16 @@
     """
     if isinstance(requirement, CondaRequirement):
         channel = channel or requirement.channel
         requirement = requirement.as_line(with_build_string=True, conda_compatible=True).replace(" ", "=")
     if "::" in requirement:
         channel, requirement = requirement.split("::", maxsplit=1)
     channels = [channel] if channel else project.conda_config.channels
+    if not channels:
+        project.core.ui.echo(f"No channel specified for searching [success]{requirement}[/]", verbosity=Verbosity.DEBUG)
     return _conda_search(requirement, project, tuple(channels))
 
 
 def update_requirements(requirements: list[Requirement], conda_packages: dict[str, CondaCandidate]):
     """
     Update requirements list with conda_packages
     :param requirements: requirements list
@@ -279,28 +266,35 @@
     :param verbose: show conda response if true
     :param dry_run: don't uninstall if dry run
     :param no_deps: don't uninstall dependencies if true
     """
     config = project.conda_config
     command = config.command("remove")
     if no_deps:
-        _prune = "no-prune"
-        if config.runner != CondaRunner.MICROMAMBA:
-            _prune = "force-remove"
-        command.append(f"--{_prune}")
+        if config.runner == CondaRunner.MICROMAMBA:
+            command.append("--no-prune")
+        elif config.runner == CondaRunner.MAMBA:
+            command[0] = "conda"
+        command.append("--force")
     if dry_run:
         command.append("--dry-run")
     if isinstance(packages, str):
         packages = [packages]
     command.extend(packages)
     command.append("--json")
 
     _conda_install(project, command, verbose=verbose)
 
 
+def not_initialized_warning(project):
+    project.core.ui.echo(
+        "[warning]Tried to execute a conda command but no pdm-conda configs were found on pyproject.toml.[/]",
+    )
+
+
 def conda_virtual_packages(project: CondaProject) -> set[CondaRequirement]:
     """
     Get conda virtual packages
     :param project: PDM project
     :return: set of virtual packages
     """
     config = project.conda_config
@@ -309,14 +303,16 @@
         info = run_conda(config.command("info") + ["--json"])
         if config.runner != CondaRunner.MICROMAMBA:
             _virtual_packages = {"=".join(p) for p in info["virtual_pkgs"]}
         else:
             _virtual_packages = set(info["virtual packages"])
 
         virtual_packages = {parse_requirement(f"conda:{p.replace('=', '==', 1)}") for p in _virtual_packages}
+    else:
+        not_initialized_warning(project)
     return virtual_packages
 
 
 def conda_list(project: CondaProject) -> dict[str, CondaSetupDistribution]:
     """
     List conda installed packages
     :param project: PDM project
@@ -332,9 +328,10 @@
                 Setup(
                     name=name,
                     summary="",
                     version=parse_conda_version(version),
                 ),
                 package=package,
             )
-
+    else:
+        not_initialized_warning(project)
     return distributions
```

### Comparing `pdm_conda-0.7.1b0/src/pdm_conda/installers/manager.py` & `pdm_conda-0.8.0b0/src/pdm_conda/installers/manager.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,33 +11,47 @@
 from pdm_conda.models.setup import CondaSetupDistribution
 
 
 class CondaInstallManager(InstallManager):
     def __init__(self, environment: Environment, *, use_install_cache: bool = False) -> None:
         super().__init__(environment, use_install_cache=use_install_cache)
         self.environment = cast(CondaEnvironment, environment)
+        self._num_install = 0
+        self._num_remove = 0
+        self._batch_install: list[CondaCandidate] = []
+        self._batch_remove: list[CondaSetupDistribution] = []
+
+    def prepare_batch_operations(self, num_install: int, num_remove: int):
+        self._num_install = num_install
+        self._num_remove = num_remove
 
     def install(self, candidate: Candidate) -> None:
         """
         Install candidate, use conda if conda package else default installer
         :param candidate: candidate to install
         """
         if isinstance(candidate, CondaCandidate):
             try:
-                conda_install(self.environment.project, candidate.link.url, no_deps=True)
+                self._batch_install.append(candidate)
+                if len(self._batch_install) >= self._num_install:
+                    conda_install(self.environment.project, [c.link.url for c in self._batch_install], no_deps=True)
+                    self._batch_install.clear()
             except (RequirementError, ValueError) as e:
                 raise InstallerError(e) from e
         else:
             super().install(candidate)
 
     def uninstall(self, dist: Distribution) -> None:
         """
         Uninstall distribution, use conda if conda package else default uninstaller
         :param dist: distribution to uninstall
         """
         if isinstance(dist, CondaSetupDistribution):
             try:
-                conda_uninstall(self.environment.project, dist.name, no_deps=True)
+                self._batch_remove.append(dist)
+                if len(self._batch_remove) >= self._num_remove:
+                    conda_uninstall(self.environment.project, [d.name for d in self._batch_remove], no_deps=True)
+                    self._batch_remove.clear()
             except RequirementError as e:
                 raise UninstallError(e) from e
         else:
             super().uninstall(dist)
```

### Comparing `pdm_conda-0.7.1b0/src/pdm_conda/installers/synchronizers.py` & `pdm_conda-0.8.0b0/src/pdm_conda/installers/synchronizers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Collection, cast
 
 from pdm.installers import Synchronizer
 from pdm.models.candidates import Candidate
 
+from pdm_conda.models.candidates import CondaCandidate
 from pdm_conda.models.environment import CondaEnvironment, Environment
-from pdm_conda.models.setup import CondaSetupDistribution
 
 
 class CondaSynchronizer(Synchronizer):
     def __init__(
         self,
         candidates: dict[str, Candidate],
         environment: Environment,
@@ -37,16 +37,23 @@
         self.parallel = bool(self.parallel)  # type: ignore
 
     def compare_with_working_set(self) -> tuple[list[str], list[str], list[str]]:
         to_add, to_update, to_remove = super().compare_with_working_set()
 
         # deactivate parallel execution if uninstall
         self.parallel = self.environment.project.config["install.parallel"]
-        if to_remove or to_update:
-            if to_remove:
-                to_remove = [p for p in to_remove if p not in self.environment.python_dependencies]
-
-            if self.parallel and any(True for d in to_remove + to_update if isinstance(d, CondaSetupDistribution)):
-                self.environment.project.core.ui.echo("Deactivating parallel uninstall.")
-                self.parallel = False
+        if to_remove:
+            to_remove = [p for p in to_remove if p not in self.environment.python_dependencies]
+
+        if self.parallel and any(True for d in to_remove + to_update if isinstance(self.candidates[d], CondaCandidate)):
+            self.environment.project.core.ui.echo("Deactivating parallel uninstall.")
+            self.parallel = False
+
+        if self.environment.project.conda_config.batched_commands:
+            self.manager.prepare_batch_operations(
+                *(
+                    len([p for p in pkgs if isinstance(self.candidates[p], CondaCandidate)])
+                    for pkgs in (to_add + to_update, to_remove + to_update)
+                )
+            )
 
         return to_add, to_update, to_remove
```

### Comparing `pdm_conda-0.7.1b0/src/pdm_conda/mapping.py` & `pdm_conda-0.8.0b0/src/pdm_conda/mapping.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.7.1b0/src/pdm_conda/models/candidates.py` & `pdm_conda-0.8.0b0/src/pdm_conda/models/candidates.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         self.constrains: dict[str, CondaRequirement] = dict()
         for r in constrains or []:
             c = cast(CondaRequirement, parse_requirement(f"conda:{r}"))
             self.constrains[str(c.conda_name)] = c
         self.build_string = build_string
         self.channel = channel
         self.conda_version = version
-        self.version = parse_conda_version(version, name != "openssl")
+        self.version = parse_conda_version(version, name == "openssl")
 
     @property
     def req(self):
         return self._req
 
     @req.setter
     def req(self, value):
@@ -157,14 +157,23 @@
             ),
             channel=channel,
             dependencies=dependencies,
             constrains=package.get("constrains", []),
             build_string=build_string,
         )
 
+    def __str__(self) -> str:
+        if self.req.is_named:
+            return f"{self.name}@{self.conda_version}"
+        return super().__str__()
+
+    def format(self) -> str:
+        """Format for output."""
+        return f"[req]{self.name}[/] [warning]{self.conda_version}[/]"
+
 
 def wrap_as_lockfile_entry(func):
     @functools.wraps(func)
     def wrapper(self, *args, **kwargs) -> dict[str, Any]:
         res = func(self, *args, **kwargs)
         if (conda_name := self.req.conda_name) is not None and conda_name != self.name:
             res["conda_name"] = conda_name
```

### Comparing `pdm_conda-0.7.1b0/src/pdm_conda/models/config.py` & `pdm_conda-0.8.0b0/src/pdm_conda/models/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,25 +17,29 @@
     ("runner", ConfigItem("Conda runner executable", "conda", env_var="CONDA_RUNNER")),
     ("channels", ConfigItem("Conda channels to use")),
     (
         "as-default-manager",
         ConfigItem("Use Conda to install all possible requirements", False, env_var="CONDA_AS_DEFAULT_MANAGER"),
     ),
     (
+        "batched-commands",
+        ConfigItem("Execute batched install and remove commands", False, env_var="CONDA_BATCHED_COMMANDS"),
+    ),
+    (
         "installation-method",
         ConfigItem(
             "Whether to use hard-link or copy when installing",
             "hard-link",
             env_var="CONDA_INSTALLATION_METHOD",
         ),
     ),
     ("dependencies", ConfigItem("Dependencies to install with Conda")),
     ("optional-dependencies", ConfigItem("Optional dependencies to install with Conda")),
     ("dev-dependencies", ConfigItem("Development dependencies to install with Conda")),
-    ("excluded", ConfigItem("Excluded dependencies from Conda")),
+    ("excludes", ConfigItem("Excluded dependencies from Conda")),
     (
         "pypi-mapping.download-dir",
         ConfigItem(
             "PyPI-Conda mapping download directory",
             Path().home() / ".pdm-conda/",
             env_var=DOWNLOAD_DIR_ENV_VAR,
         ),
@@ -63,16 +67,17 @@
     _project: Project = field(repr=False, default=None)
     _initialized: bool = field(repr=False, default=False, compare=False)
     _set_project_config: bool = field(repr=False, default=False, compare=False)
 
     channels: list[str] = field(default_factory=list)
     runner: str = "conda"
     as_default_manager: bool = False
+    batched_commands: bool = False
     installation_method: str = "hard-link"
-    excluded: list[str] = field(default_factory=list, repr=False)
+    excludes: list[str] = field(default_factory=list, repr=False)
     dependencies: list[str] = field(default_factory=list, repr=False)
     optional_dependencies: dict[str, list] = field(default_factory=dict)
     dev_dependencies: dict[str, list] = field(default_factory=dict)
     mapping_download_dir: Path = field(repr=False, default=Path())
 
     def __post_init__(self):
         if self.runner not in list(CondaRunner):
@@ -134,16 +139,18 @@
     def omit_set_project_config(self):
         """
         Context manager that deactivates updating pyproject settings
         :return:
         """
         old_value = self._set_project_config
         self._set_project_config = False
-        yield
-        self._set_project_config = old_value
+        try:
+            yield
+        finally:
+            self._set_project_config = old_value
 
     @property
     def is_initialized(self):
         return self._initialized
 
     @classmethod
     def load_config(cls, project: Project, **kwargs) -> "PluginConfig":
@@ -157,15 +164,15 @@
         kwargs["_initialized"] = is_conda_config_initialized(project)
         for n, c in CONFIGS:
             n = n[len("conda.") :]
             if (prop_name := _CONFIG_MAP.get(n, n)) not in config and c.env_var:
                 value = project.config[f"conda.{n}"]
                 if prop_name == "mapping_download_dir":
                     value = Path(value)
-                elif prop_name == "as-default-manager":
+                elif prop_name in ("as-default-manager", "batched-commands"):
                     value = str(value).lower() in ("true", "1")
                 config[prop_name] = value
         config = {k.replace("-", "_"): v for k, v in config.items()}
         return PluginConfig(_project=project, **(config | kwargs))
 
     def command(self, cmd="install"):
         """
```

### Comparing `pdm_conda-0.7.1b0/src/pdm_conda/models/repositories.py` & `pdm_conda-0.8.0b0/src/pdm_conda/models/repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,19 +23,21 @@
 
     def _uses_conda(self, requirement: Requirement) -> bool:
         """
         True if requirement is conda requirement or (not excluded and named requirement
         and conda as default manager or used by another conda requirement)
         :param requirement: requirement to evaluate
         """
+        if not isinstance(self.environment, CondaEnvironment):
+            return False
         conda_config = self.environment.project.conda_config
         return isinstance(requirement, CondaRequirement) or (
             isinstance(requirement, NamedRequirement)
             and conda_config.as_default_manager
-            and requirement.name not in conda_config.excluded
+            and requirement.name not in conda_config.excludes
         )
 
     def get_dependencies(self, candidate: Candidate) -> tuple[list[Requirement], PySpecSet, str]:
         if isinstance(candidate, CondaCandidate):
             dependencies = list(candidate.dependencies)
             # if dep in constrains use constrain
             if candidate.constrains:
```

### Comparing `pdm_conda-0.7.1b0/src/pdm_conda/models/requirements.py` & `pdm_conda-0.8.0b0/src/pdm_conda/models/requirements.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,29 +22,27 @@
 
 
 @dataclasses.dataclass(eq=False)
 class CondaRequirement(NamedRequirement):
     channel: str | None = None
     _is_python_package: bool = dataclasses.field(default=True, repr=False, init=False)
     version_mapping: dict = dataclasses.field(default_factory=dict, repr=False)
-    mapping_excluded: bool = dataclasses.field(default=False, repr=False)
     build_string: str | None = None
 
     @property
     def conda_name(self) -> str | None:
         return self.name
 
     @property
     def is_python_package(self):
         return self._is_python_package
 
     @is_python_package.setter
     def is_python_package(self, value):
         self._is_python_package = value
-        self.mapping_excluded = not value
 
     @classmethod
     def create(cls: type[T], **kwargs: Any) -> T:
         kwargs.pop("conda_managed", None)
         if build_string := kwargs.get("build_string", None):
             kwargs["build_string"] = build_string.strip()
 
@@ -189,15 +187,15 @@
                                 s = "="
                             conda_version_or = f"{s}={conda_version_or}"
                         _version = conda_version_or
                         if not _version.startswith("=="):
                             _version = _conda_specifier_star_re.sub(correct_specifier_star, _version)
                             if _version.startswith("~") and "." not in _version:
                                 _version += ".0"
-                        _version = parse_conda_version(_version, name != "openssl")
+                        _version = parse_conda_version(_version, name == "openssl")
                         version_mapping[remove_operator(_version)] = remove_operator(conda_version_or)
                     version_or[j] = _version
             version_and[i] = max((v for v in version_or if v), key=comparable_version, default="")
         version = ",".join(version_and)
         req = CondaRequirement.create(
             name=strip_extras(name.strip())[0],
             specifier=SpecifierSet(version),
```

### Comparing `pdm_conda-0.7.1b0/src/pdm_conda/models/setup.py` & `pdm_conda-0.8.0b0/src/pdm_conda/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.7.1b0/src/pdm_conda/project.py` & `pdm_conda-0.8.0b0/src/pdm_conda/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,25 +45,29 @@
         self.locked_repository_class = LockedCondaRepository
         self.environment_class = CondaEnvironment
         self.virtual_packages: set[CondaRequirement] = set()
         self._conda_mapping: dict[str, str] = dict()
         self._pypi_mapping: dict[str, str] = dict()
         self.conda_config = PluginConfig.load_config(self)
 
-    def get_conda_pyproject_dependencies(self, group: str, dev: bool = False) -> list[str]:
+    def get_conda_pyproject_dependencies(self, group: str, dev: bool = False, set_defaults=False) -> list[str]:
         """
         Get the conda dependencies array in the pyproject.toml
         """
-        settings = self.pyproject.settings.setdefault("conda", dict())
+
+        def _getter(conf, name, default, set_defaults=False):
+            return (conf.setdefault if set_defaults else conf.get)(name, default)
+
+        settings = _getter(self.pyproject.settings, "conda", dict(), set_defaults)
         if group == "default":
-            deps = settings.setdefault("dependencies", [])
+            group = "dependencies"
         else:
             name = "optional" if not dev else "dev"
-            deps = settings.setdefault(f"{name}-dependencies", dict()).setdefault(group, [])
-        return deps
+            settings = _getter(settings, f"{name}-dependencies", dict(), set_defaults)
+        return _getter(settings, group, [], set_defaults)
 
     def iter_groups(self) -> Iterable[str]:
         groups = set(super().iter_groups())
         config = self.conda_config
         for deps in (config.optional_dependencies, config.dev_dependencies):
             if deps:
                 groups.update(deps.keys())
@@ -97,15 +101,15 @@
                 if not req.specifier:
                     req.specifier = pypi_req.specifier
             result[req.identify()] = req
 
         if self.conda_config.as_default_manager:
             for k in list(result):
                 req = result[k]
-                if req.name not in self.conda_config.excluded and not isinstance(req, CondaRequirement):
+                if req.name not in self.conda_config.excludes and not isinstance(req, CondaRequirement):
                     result[k] = as_conda_requirement(req)
 
         return result
 
     @property
     def locked_repository(self) -> LockedRepository:
         try:
@@ -125,15 +129,15 @@
         conda_requirements = {n: r for n, r in requirements.items() if isinstance(r, CondaRequirement)}
         requirements = {n: r for n, r in requirements.items() if n not in conda_requirements} | {
             n: r.as_named_requirement() for n, r in conda_requirements.items() if r.is_python_package
         }
         if self.conda_config.as_default_manager:
             conda_requirements = {n: r for n, r in conda_requirements.items() if not r.is_python_package}
         if conda_requirements:
-            deps = self.get_conda_pyproject_dependencies(to_group, dev)
+            deps = self.get_conda_pyproject_dependencies(to_group, dev, set_defaults=True)
             cast(Array, deps).multiline(True)
             for _, dep in conda_requirements.items():
                 matched_index = next((i for i, r in enumerate(deps) if dep.matches(f"conda:{r}")), None)
                 req = dep.as_line(with_channel=True)
                 if matched_index is None:
                     deps.append(req)
                 else:
```

### Comparing `pdm_conda-0.7.1b0/src/pdm_conda/resolver/providers.py` & `pdm_conda-0.8.0b0/src/pdm_conda/resolver/providers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.7.1b0/src/pdm_conda/resolvers.py` & `pdm_conda-0.8.0b0/src/pdm_conda/resolvers.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,17 @@
     mapping: dict
     criteria: dict
     backtrack_causes: list
     constrains: dict = field(default_factory=dict)
 
 
 class CondaResolution(Resolution):
-    def __init__(self, *args, base_constrains: dict | None, **kwargs) -> None:
+    def __init__(self, *args, base_constrains: dict | None, is_conda_environment: bool = True, **kwargs) -> None:
         super().__init__(*args, **kwargs)
+        self._is_conda_environment = is_conda_environment
         self._base_constrains = base_constrains or dict()
 
     @property
     def state(self):
         if self._states and not isinstance(state := self._states[-1], State):
             self._states[-1] = State(state.mapping, state.criteria, state.backtrack_causes, self._base_constrains)
         return super().state
@@ -36,59 +37,61 @@
             criteria=base.criteria.copy(),
             backtrack_causes=base.backtrack_causes[:],
             constrains=base.constrains.copy(),
         )
         self._states.append(state)
 
     def _add_to_criteria(self, criteria, requirement, parent):
-        constrains = self.state.constrains
         _req = requirement
-        if (constrain := constrains.get(requirement.conda_name, None)) is not None:
-            _req = copy(constrain)
-            _req.specifier &= requirement.specifier
-            if isinstance(requirement, CondaRequirement):
-                _req.channel = requirement.channel
-        identifier = self._p.identify(_req)
-        if criterion := criteria.get(identifier):
-            excluded = self._p.repository.environment.project.conda_config.excluded
-            if isinstance(_req, CondaRequirement):
-                # if conda requirement but other not conda requirement and excluded
-                # then transform to named requirement
-                if any(
-                    not isinstance(i.requirement, CondaRequirement) and i.requirement.name in excluded
-                    for i in criterion.information
-                ):
-                    _req = _req.as_named_requirement()
-                # else any other to conda
-                else:
-                    criterion.information = [
-                        RequirementInformation(as_conda_requirement(i.requirement), i.parent)
+        if self._is_conda_environment:
+            constrains = self.state.constrains
+            if (constrain := constrains.get(requirement.conda_name, None)) is not None:
+                _req = copy(constrain)
+                _req.specifier &= requirement.specifier
+                _req.version_mapping.update(getattr(requirement, "version_mapping", dict()))
+                if isinstance(requirement, CondaRequirement):
+                    _req.channel = requirement.channel
+            identifier = self._p.identify(_req)
+            if criterion := criteria.get(identifier):
+                excluded = self._p.repository.environment.project.conda_config.excludes
+                if isinstance(_req, CondaRequirement):
+                    # if conda requirement but other not conda requirement and excluded
+                    # then transform to named requirement
+                    if any(
+                        not isinstance(i.requirement, CondaRequirement) and i.requirement.name in excluded
                         for i in criterion.information
-                    ]
+                    ):
+                        _req = _req.as_named_requirement()
+                    # else any other to conda
+                    else:
+                        criterion.information = [
+                            RequirementInformation(as_conda_requirement(i.requirement), i.parent)
+                            for i in criterion.information
+                        ]
 
-            # if excluded then delete conda related information else if other conda requirement transform to conda
-            else:
-                if requirement.name in excluded:
-                    criterion.information = [
-                        RequirementInformation(i.requirement.as_named_requirement(), i.parent)
-                        if isinstance(
-                            i.requirement,
-                            CondaRequirement,
-                        )
-                        else i
-                        for i in criterion.information
-                    ]
-                elif any(isinstance(i.requirement, CondaRequirement) for i in criterion.information):
-                    _req = as_conda_requirement(requirement)
+                # if excluded then delete conda related information else if other conda requirement transform to conda
+                else:
+                    if requirement.name in excluded:
+                        criterion.information = [
+                            RequirementInformation(i.requirement.as_named_requirement(), i.parent)
+                            if isinstance(
+                                i.requirement,
+                                CondaRequirement,
+                            )
+                            else i
+                            for i in criterion.information
+                        ]
+                    elif any(isinstance(i.requirement, CondaRequirement) for i in criterion.information):
+                        _req = as_conda_requirement(requirement)
         super()._add_to_criteria(criteria, _req, parent)
 
     def _get_updated_criteria(self, candidate):
         criteria = super()._get_updated_criteria(candidate)
         # update previous constrain if exists
-        if isinstance(candidate, CondaCandidate):
+        if isinstance(candidate, CondaCandidate) and self._is_conda_environment:
             for identifier, constrain in candidate.constrains.items():
                 if identifier != "python":
                     # keep most restrictive constrain
                     if (existing_constrain := self.state.constrains.get(identifier, None)) is not None and all(
                         Version(s.version) < Version(e.version)
                         for e in existing_constrain.specifier
                         for s in constrain.specifier
@@ -100,16 +103,24 @@
 
         return criteria
 
 
 class CondaResolver(Resolver):
     def resolve(self, requirements, max_rounds=100):
         base_constrains = dict()
-        if isinstance(environment := self.provider.repository.environment, CondaEnvironment):
+
+        if is_conda_environment := isinstance(environment := self.provider.repository.environment, CondaEnvironment):
             # add installed python constrains
             if (can := environment.python_candidate) is not None:
                 base_constrains |= can.constrains
                 base_constrains |= {d.conda_name: d for d in can.dependencies}
+        else:
+            assert not any(isinstance(r, CondaRequirement) for r in requirements)
 
-        resolution = CondaResolution(self.provider, self.reporter, base_constrains=base_constrains)
+        resolution = CondaResolution(
+            self.provider,
+            self.reporter,
+            base_constrains=base_constrains,
+            is_conda_environment=is_conda_environment,
+        )
         state = resolution.resolve(requirements, max_rounds=max_rounds)
         return _build_result(state)
```

### Comparing `pdm_conda-0.7.1b0/src/pdm_conda/utils.py` & `pdm_conda-0.8.0b0/src/pdm_conda/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.7.1b0/PKG-INFO` & `pdm_conda-0.8.0b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-conda
-Version: 0.7.1b0
+Version: 0.8.0b0
 Summary:  A PDM plugin to install project dependencies with Conda
 Keywords: pdm plugin conda
 Author: Marcos Pastorini
 License: MIT License
         
         Copyright (c) 2022 macro128
         
@@ -37,37 +37,38 @@
 
 # pdm-conda
 
 A PDM plugin to install project dependencies with Conda.
 
 ## Configuration
 
-| Config item                       | Description                                                                                        | Default value       | Possible values                | Environment variable        |
-|-----------------------------------|----------------------------------------------------------------------------------------------------|---------------------|--------------------------------|-----------------------------|
-| `conda.runner`                    | Conda runner executable                                                                            | `conda`             | `conda`, `mamba`, `micromamba` | `CONDA_RUNNER`              |
-| `conda.channels`                  | Conda channels to use, order will be enforced                                                      | `[]`                |                                |                             |
-| `conda.as-default-manager`        | Use Conda to install all possible requirements                                                     | `False`             |                                | `CONDA_AS_DEFAULT_MANAGER`  |
-| `conda.excluded`                  | Array of dependencies to exclude from Conda resolution                                             | `[]`                |                                |                             |
-| `conda.installation-method`       | Installation method to use when installing dependencies with Conda                                 | `hard-link`         | `hard-link`, `copy`            | `CONDA_INSTALLATION_METHOD` |
-| `conda.dependencies`              | Array of dependencies to install with Conda, analogue to `project.dependencies`                    | `[]`                |                                |                             |
-| `conda.optional-dependencies`     | Groups of optional dependencies to install with Conda, analogue to `project.optional-dependencies` | `{}`                |                                |                             |
-| `conda.dev-dependencies`          | Groups of development dependencies to install with Conda, analogue to `tool.pdm.dev-dependencies`  | `{}`                |                                |                             |
-| `conda.pypi-mapping.download-dir` | PyPI-Conda mapping download directory                                                              | `$HOME/.pdm-conda/` |                                | `PYPI_MAPPING_DIR`          |
+| Config item                       | Description                                                                                          | Default value       | Possible values                | Environment variable        |
+|-----------------------------------|------------------------------------------------------------------------------------------------------|---------------------|--------------------------------|-----------------------------|
+| `conda.runner`                    | Conda runner executable                                                                              | `conda`             | `conda`, `mamba`, `micromamba` | `CONDA_RUNNER`              |
+| `conda.channels`                  | Conda channels to use, order will be enforced                                                        | `[]`                |                                |                             |
+| `conda.as-default-manager`        | Use Conda to install all possible requirements                                                       | `False`             |                                | `CONDA_AS_DEFAULT_MANAGER`  |
+| `conda.use-batched`               | Execute batched install and remove Conda commands, when True the command is executed only at the end | `False`             |                                | `CONDA_BATCHED_COMMANDS`    |
+| `conda.excludes`                  | Array of dependencies to exclude from Conda resolution                                               | `[]`                |                                |                             |
+| `conda.installation-method`       | Installation method to use when installing dependencies with Conda                                   | `hard-link`         | `hard-link`, `copy`            | `CONDA_INSTALLATION_METHOD` |
+| `conda.dependencies`              | Array of dependencies to install with Conda, analogue to `project.dependencies`                      | `[]`                |                                |                             |
+| `conda.optional-dependencies`     | Groups of optional dependencies to install with Conda, analogue to `project.optional-dependencies`   | `{}`                |                                |                             |
+| `conda.dev-dependencies`          | Groups of development dependencies to install with Conda, analogue to `tool.pdm.dev-dependencies`    | `{}`                |                                |                             |
+| `conda.pypi-mapping.download-dir` | PyPI-Conda mapping download directory                                                                | `$HOME/.pdm-conda/` |                                | `PYPI_MAPPING_DIR`          |
 
 All configuration items use prefix `pdm.tool`, this is a viable configuration:
 
 ```toml
 [tool.pdm.conda]
 runner = "micromamba"
 channels = ["conda-forge/noarch", "conda-forge", "anaconda"]
 dependencies = ["pdm"]
 as-default-manager = true
-excluded = ["pytest-cov"] # don't install with conda even if it's a dependency from other packages
+excludes = ["pytest-cov"] # don't install with conda even if it's a dependency from other packages
 installation-method = "copy"
-
+use-batched = true
 
 [tool.pdm.conda.pypi-mapping]
 download-dir = "/tmp"
 
 [tool.pdm.conda.optional-dependencies]
 extra = ["anaconda:ffmpeg"] # non python dependency, obtained from anaconda channel
 
@@ -89,21 +90,22 @@
     * To add a Conda managed package `--conda` flag can be used multiple times followed a package (analogue
       to `--editable`).
     * You can specify per package Conda channel using conda notation `channel::package`.
     * You also can specify a default Conda channel with `-c` or `--channel`.
     * With flag `-r` or `--runner` you can specify the Conda runner to use.
 * `pdm remove`
 * `pdm list`
+* `pdm info`
 
 ### How it works
 
-When PDM detects a Conda managed package, it gets Candidates with Conda and then tries to resolve the environment as
+When PDM detects a Conda managed package, it gets candidates with Conda and then tries to resolve the environment as
 with any other requirement.
 
-To keep the resolution consistent with Conda, PDM uses resolution rules from Conda as good as possible.
+To keep the resolution consistent with Conda, PDM follows resolution rules from Conda as good as possible.
 
 ### Settings overriden
 
 In order to use Conda to install packages some settings were overriden:
 
 * `install.parallel` if some Conda managed packages are to be uninstalled or updated this option is disabled
   momentarily.
```

