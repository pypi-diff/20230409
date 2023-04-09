# Comparing `tmp/pdm_conda-0.8.0.tar.gz` & `tmp/pdm_conda-0.8.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_conda-0.8.0.tar", last modified: Sun Apr  9 20:30:11 2023, max compression
+gzip compressed data, was "pdm_conda-0.8.0b0.tar", last modified: Sun Apr  9 20:06:47 2023, max compression
```

## Comparing `pdm_conda-0.8.0.tar` & `pdm_conda-0.8.0b0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.8.0/LICENSE
--rw-r--r--   0        0        0     4832 2023-04-09 20:29:55.601420 pdm_conda-0.8.0/README.md
--rw-r--r--   0        0        0     1925 2023-04-09 20:30:11.867472 pdm_conda-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      593 2023-04-09 20:29:55.602628 pdm_conda-0.8.0/src/pdm_conda/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.8.0/src/pdm_conda/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.8.0/src/pdm_conda/cli/commands/__init__.py
--rw-r--r--   0        0        0     3219 2023-04-09 20:29:55.603310 pdm_conda-0.8.0/src/pdm_conda/cli/commands/add.py
--rw-r--r--   0        0        0     1681 2023-04-09 20:29:55.604146 pdm_conda-0.8.0/src/pdm_conda/cli/commands/remove.py
--rw-r--r--   0        0        0     2183 2023-04-09 20:29:55.604925 pdm_conda-0.8.0/src/pdm_conda/cli/utils.py
--rw-r--r--   0        0        0    11001 2023-04-09 20:29:55.605692 pdm_conda-0.8.0/src/pdm_conda/conda.py
--rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.8.0/src/pdm_conda/installers/__init__.py
--rw-r--r--   0        0        0     2482 2023-04-09 20:29:55.606525 pdm_conda-0.8.0/src/pdm_conda/installers/manager.py
--rw-r--r--   0        0        0     2130 2023-04-09 20:29:55.607169 pdm_conda-0.8.0/src/pdm_conda/installers/synchronizers.py
--rw-r--r--   0        0        0     3132 2023-01-17 17:44:51.337923 pdm_conda-0.8.0/src/pdm_conda/mapping.py
--rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.8.0/src/pdm_conda/models/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.8.0/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
--rw-r--r--   0        0        0     6776 2023-04-09 20:29:55.608074 pdm_conda-0.8.0/src/pdm_conda/models/candidates.py
--rw-r--r--   0        0        0     7145 2023-04-09 20:29:55.608846 pdm_conda-0.8.0/src/pdm_conda/models/config.py
--rw-r--r--   0        0        0     3234 2023-04-09 20:29:55.609532 pdm_conda-0.8.0/src/pdm_conda/models/environment.py
--rw-r--r--   0        0        0     3863 2023-04-09 20:29:55.610491 pdm_conda-0.8.0/src/pdm_conda/models/repositories.py
--rw-r--r--   0        0        0     9046 2023-04-09 20:29:55.611231 pdm_conda-0.8.0/src/pdm_conda/models/requirements.py
--rw-r--r--   0        0        0      900 2023-04-09 20:29:55.611942 pdm_conda-0.8.0/src/pdm_conda/models/setup.py
--rw-r--r--   0        0        0     7518 2023-04-09 20:29:55.612631 pdm_conda-0.8.0/src/pdm_conda/project.py
--rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.8.0/src/pdm_conda/resolver/__init__.py
--rw-r--r--   0        0        0     1134 2023-02-23 00:47:35.312247 pdm_conda-0.8.0/src/pdm_conda/resolver/providers.py
--rw-r--r--   0        0        0     5740 2023-04-09 20:29:55.613268 pdm_conda-0.8.0/src/pdm_conda/resolvers.py
--rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.8.0/src/pdm_conda/utils.py
--rw-r--r--   0        0        0     6661 1970-01-01 00:00:00.000000 pdm_conda-0.8.0/PKG-INFO
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

### Comparing `pdm_conda-0.8.0/LICENSE` & `pdm_conda-0.8.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0/README.md` & `pdm_conda-0.8.0b0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ## Configuration
 
 | Config item                       | Description                                                                                          | Default value       | Possible values                | Environment variable        |
 |-----------------------------------|------------------------------------------------------------------------------------------------------|---------------------|--------------------------------|-----------------------------|
 | `conda.runner`                    | Conda runner executable                                                                              | `conda`             | `conda`, `mamba`, `micromamba` | `CONDA_RUNNER`              |
 | `conda.channels`                  | Conda channels to use, order will be enforced                                                        | `[]`                |                                |                             |
 | `conda.as-default-manager`        | Use Conda to install all possible requirements                                                       | `False`             |                                | `CONDA_AS_DEFAULT_MANAGER`  |
-| `conda.batched-commands`          | Execute batched install and remove Conda commands, when True the command is executed only at the end | `False`             |                                | `CONDA_BATCHED_COMMANDS`    |
+| `conda.use-batched`               | Execute batched install and remove Conda commands, when True the command is executed only at the end | `False`             |                                | `CONDA_BATCHED_COMMANDS`    |
 | `conda.excludes`                  | Array of dependencies to exclude from Conda resolution                                               | `[]`                |                                |                             |
 | `conda.installation-method`       | Installation method to use when installing dependencies with Conda                                   | `hard-link`         | `hard-link`, `copy`            | `CONDA_INSTALLATION_METHOD` |
 | `conda.dependencies`              | Array of dependencies to install with Conda, analogue to `project.dependencies`                      | `[]`                |                                |                             |
 | `conda.optional-dependencies`     | Groups of optional dependencies to install with Conda, analogue to `project.optional-dependencies`   | `{}`                |                                |                             |
 | `conda.dev-dependencies`          | Groups of development dependencies to install with Conda, analogue to `tool.pdm.dev-dependencies`    | `{}`                |                                |                             |
 | `conda.pypi-mapping.download-dir` | PyPI-Conda mapping download directory                                                                | `$HOME/.pdm-conda/` |                                | `PYPI_MAPPING_DIR`          |
 
@@ -23,15 +23,15 @@
 [tool.pdm.conda]
 runner = "micromamba"
 channels = ["conda-forge/noarch", "conda-forge", "anaconda"]
 dependencies = ["pdm"]
 as-default-manager = true
 excludes = ["pytest-cov"] # don't install with conda even if it's a dependency from other packages
 installation-method = "copy"
-batched-commands = true
+use-batched = true
 
 [tool.pdm.conda.pypi-mapping]
 download-dir = "/tmp"
 
 [tool.pdm.conda.optional-dependencies]
 extra = ["anaconda:ffmpeg"] # non python dependency, obtained from anaconda channel
```

### Comparing `pdm_conda-0.8.0/pyproject.toml` & `pdm_conda-0.8.0b0/pyproject.toml`

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
-version = "0.8.0"
+version = "0.8.0b0"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/macro128/pdm-conda"
 Changelog = "https://github.com/macro128/pdm-conda/blob/main/CHANGELOG.md"
```

### Comparing `pdm_conda-0.8.0/src/pdm_conda/__init__.py` & `pdm_conda-0.8.0b0/src/pdm_conda/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,8 +14,8 @@
     core.register_command(AddCommand)
     core.register_command(RemoveCommand)
 
     for name, config in CONFIGS:
         core.add_config(name, config)
 
 
-__version__ = "0.8.0"
+__version__ = "0.8.0b0"
```

### Comparing `pdm_conda-0.8.0/src/pdm_conda/cli/commands/add.py` & `pdm_conda-0.8.0b0/src/pdm_conda/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0/src/pdm_conda/cli/commands/remove.py` & `pdm_conda-0.8.0b0/src/pdm_conda/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0/src/pdm_conda/cli/utils.py` & `pdm_conda-0.8.0b0/src/pdm_conda/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0/src/pdm_conda/conda.py` & `pdm_conda-0.8.0b0/src/pdm_conda/conda.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0/src/pdm_conda/installers/manager.py` & `pdm_conda-0.8.0b0/src/pdm_conda/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0/src/pdm_conda/installers/synchronizers.py` & `pdm_conda-0.8.0b0/src/pdm_conda/installers/synchronizers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0/src/pdm_conda/mapping.py` & `pdm_conda-0.8.0b0/src/pdm_conda/mapping.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0/src/pdm_conda/models/candidates.py` & `pdm_conda-0.8.0b0/src/pdm_conda/models/candidates.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0/src/pdm_conda/models/config.py` & `pdm_conda-0.8.0b0/src/pdm_conda/models/config.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0/src/pdm_conda/models/environment.py` & `pdm_conda-0.8.0b0/src/pdm_conda/models/environment.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0/src/pdm_conda/models/repositories.py` & `pdm_conda-0.8.0b0/src/pdm_conda/models/repositories.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0/src/pdm_conda/models/requirements.py` & `pdm_conda-0.8.0b0/src/pdm_conda/models/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0/src/pdm_conda/models/setup.py` & `pdm_conda-0.8.0b0/src/pdm_conda/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0/src/pdm_conda/project.py` & `pdm_conda-0.8.0b0/src/pdm_conda/project.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0/src/pdm_conda/resolver/providers.py` & `pdm_conda-0.8.0b0/src/pdm_conda/resolver/providers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0/src/pdm_conda/resolvers.py` & `pdm_conda-0.8.0b0/src/pdm_conda/resolvers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0/src/pdm_conda/utils.py` & `pdm_conda-0.8.0b0/src/pdm_conda/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.0/PKG-INFO` & `pdm_conda-0.8.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-conda
-Version: 0.8.0
+Version: 0.8.0b0
 Summary:  A PDM plugin to install project dependencies with Conda
 Keywords: pdm plugin conda
 Author: Marcos Pastorini
 License: MIT License
         
         Copyright (c) 2022 macro128
         
@@ -42,15 +42,15 @@
 ## Configuration
 
 | Config item                       | Description                                                                                          | Default value       | Possible values                | Environment variable        |
 |-----------------------------------|------------------------------------------------------------------------------------------------------|---------------------|--------------------------------|-----------------------------|
 | `conda.runner`                    | Conda runner executable                                                                              | `conda`             | `conda`, `mamba`, `micromamba` | `CONDA_RUNNER`              |
 | `conda.channels`                  | Conda channels to use, order will be enforced                                                        | `[]`                |                                |                             |
 | `conda.as-default-manager`        | Use Conda to install all possible requirements                                                       | `False`             |                                | `CONDA_AS_DEFAULT_MANAGER`  |
-| `conda.batched-commands`          | Execute batched install and remove Conda commands, when True the command is executed only at the end | `False`             |                                | `CONDA_BATCHED_COMMANDS`    |
+| `conda.use-batched`               | Execute batched install and remove Conda commands, when True the command is executed only at the end | `False`             |                                | `CONDA_BATCHED_COMMANDS`    |
 | `conda.excludes`                  | Array of dependencies to exclude from Conda resolution                                               | `[]`                |                                |                             |
 | `conda.installation-method`       | Installation method to use when installing dependencies with Conda                                   | `hard-link`         | `hard-link`, `copy`            | `CONDA_INSTALLATION_METHOD` |
 | `conda.dependencies`              | Array of dependencies to install with Conda, analogue to `project.dependencies`                      | `[]`                |                                |                             |
 | `conda.optional-dependencies`     | Groups of optional dependencies to install with Conda, analogue to `project.optional-dependencies`   | `{}`                |                                |                             |
 | `conda.dev-dependencies`          | Groups of development dependencies to install with Conda, analogue to `tool.pdm.dev-dependencies`    | `{}`                |                                |                             |
 | `conda.pypi-mapping.download-dir` | PyPI-Conda mapping download directory                                                                | `$HOME/.pdm-conda/` |                                | `PYPI_MAPPING_DIR`          |
 
@@ -60,15 +60,15 @@
 [tool.pdm.conda]
 runner = "micromamba"
 channels = ["conda-forge/noarch", "conda-forge", "anaconda"]
 dependencies = ["pdm"]
 as-default-manager = true
 excludes = ["pytest-cov"] # don't install with conda even if it's a dependency from other packages
 installation-method = "copy"
-batched-commands = true
+use-batched = true
 
 [tool.pdm.conda.pypi-mapping]
 download-dir = "/tmp"
 
 [tool.pdm.conda.optional-dependencies]
 extra = ["anaconda:ffmpeg"] # non python dependency, obtained from anaconda channel
```

