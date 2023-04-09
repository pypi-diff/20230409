# Comparing `tmp/pyprojectx-0.9.9.tar.gz` & `tmp/pyprojectx-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprojectx-0.9.9.tar", max compression
+gzip compressed data, was "pyprojectx-1.0.0b1.tar", max compression
```

## Comparing `pyprojectx-0.9.9.tar` & `pyprojectx-1.0.0b1.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0     1071 2022-03-14 19:18:40.753664 pyprojectx-0.9.9/LICENSE
--rw-r--r--   0        0        0     4529 2022-03-14 19:18:40.753664 pyprojectx-0.9.9/README.md
--rw-r--r--   0        0        0     3162 2022-03-14 19:18:55.733895 pyprojectx-0.9.9/pyproject.toml
--rw-r--r--   0        0        0        0 2022-03-14 19:18:40.757664 pyprojectx-0.9.9/src/pyprojectx/__init__.py
--rw-r--r--   0        0        0     4168 2022-03-14 19:18:40.757664 pyprojectx-0.9.9/src/pyprojectx/cli.py
--rw-r--r--   0        0        0     6435 2022-03-14 19:18:40.757664 pyprojectx-0.9.9/src/pyprojectx/config.py
--rw-r--r--   0        0        0     5536 2022-03-14 19:18:40.757664 pyprojectx-0.9.9/src/pyprojectx/env.py
--rw-r--r--   0        0        0        0 2022-03-14 19:18:40.757664 pyprojectx-0.9.9/src/pyprojectx/initializer/__init__.py
--rw-r--r--   0        0        0      348 2022-03-14 19:18:40.757664 pyprojectx-0.9.9/src/pyprojectx/initializer/global-template.toml
--rw-r--r--   0        0        0     7223 2022-03-14 19:18:40.757664 pyprojectx-0.9.9/src/pyprojectx/initializer/initializers.py
--rw-r--r--   0        0        0      839 2022-03-14 19:18:40.757664 pyprojectx-0.9.9/src/pyprojectx/initializer/pdm-template.toml
--rw-r--r--   0        0        0      858 2022-03-14 19:18:40.757664 pyprojectx-0.9.9/src/pyprojectx/initializer/poetry-template.toml
--rw-r--r--   0        0        0       32 2022-03-14 19:18:40.757664 pyprojectx-0.9.9/src/pyprojectx/initializer/poetry.toml
--rw-r--r--   0        0        0      863 2022-03-14 19:18:40.757664 pyprojectx-0.9.9/src/pyprojectx/initializer/project-template.toml
--rw-r--r--   0        0        0      303 2022-03-14 19:18:40.757664 pyprojectx-0.9.9/src/pyprojectx/log.py
--rw-r--r--   0        0        0        0 2022-03-14 19:18:40.757664 pyprojectx-0.9.9/src/pyprojectx/wrapper/__init__.py
--rw-r--r--   0        0        0       30 2022-03-14 19:18:40.757664 pyprojectx-0.9.9/src/pyprojectx/wrapper/pw.bat
--rwxr-xr-x   0        0        0     5802 2022-03-14 19:18:55.809895 pyprojectx-0.9.9/src/pyprojectx/wrapper/pw.py
--rwxr-xr-x   0        0        0      253 2022-03-14 19:18:40.757664 pyprojectx-0.9.9/src/pyprojectx/wrapper/px
--rw-r--r--   0        0        0      373 2022-03-14 19:18:40.757664 pyprojectx-0.9.9/src/pyprojectx/wrapper/px.bat
--rwxr-xr-x   0        0        0      275 2022-03-14 19:18:40.757664 pyprojectx-0.9.9/src/pyprojectx/wrapper/pxg
--rw-r--r--   0        0        0      264 2022-03-14 19:18:40.757664 pyprojectx-0.9.9/src/pyprojectx/wrapper/pxg.bat
--rw-r--r--   0        0        0     5626 2022-03-14 19:21:02.516789 pyprojectx-0.9.9/setup.py
--rw-r--r--   0        0        0     5487 2022-03-14 19:21:02.517144 pyprojectx-0.9.9/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-09 21:51:00.235975 pyprojectx-1.0.0b1/LICENSE
+-rw-r--r--   0        0        0     4600 2023-04-09 21:51:00.235975 pyprojectx-1.0.0b1/README.md
+-rw-r--r--   0        0        0     3228 2023-04-09 21:51:19.068231 pyprojectx-1.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/__init__.py
+-rw-r--r--   0        0        0     4218 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/cli.py
+-rw-r--r--   0        0        0     6435 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/config.py
+-rw-r--r--   0        0        0     5537 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/env.py
+-rw-r--r--   0        0        0        0 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/initializer/__init__.py
+-rw-r--r--   0        0        0      348 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/initializer/global-template.toml
+-rw-r--r--   0        0        0     7226 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/initializer/initializers.py
+-rw-r--r--   0        0        0      839 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/initializer/pdm-template.toml
+-rw-r--r--   0        0        0      858 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/initializer/poetry-template.toml
+-rw-r--r--   0        0        0       32 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/initializer/poetry.toml
+-rw-r--r--   0        0        0      863 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/initializer/project-template.toml
+-rw-r--r--   0        0        0      303 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/log.py
+-rw-r--r--   0        0        0        0 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/wrapper/__init__.py
+-rw-r--r--   0        0        0       30 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/wrapper/pw.bat
+-rwxr-xr-x   0        0        0     5804 2023-04-09 21:51:19.168232 pyprojectx-1.0.0b1/src/pyprojectx/wrapper/pw.py
+-rwxr-xr-x   0        0        0      253 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/wrapper/px
+-rw-r--r--   0        0        0      373 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/wrapper/px.bat
+-rwxr-xr-x   0        0        0      275 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/wrapper/pxg
+-rw-r--r--   0        0        0      270 2023-04-09 21:51:00.239975 pyprojectx-1.0.0b1/src/pyprojectx/wrapper/pxg.bat
+-rw-r--r--   0        0        0     5583 1970-01-01 00:00:00.000000 pyprojectx-1.0.0b1/PKG-INFO
```

### Comparing `pyprojectx-0.9.9/LICENSE` & `pyprojectx-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprojectx-0.9.9/README.md` & `pyprojectx-1.0.0b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,22 +34,22 @@
 **Linux/Mac**
 ```bash
 curl -LO https://github.com/pyprojectx/pyprojectx/releases/latest/download/wrappers.zip && unzip wrappers.zip && rm -f wrappers.zip
 ```
 
 **Windows**
 ```powershell
-(Invoke-WebRequest https://github.com/pyprojectx/pyprojectx/releases/latest/download/wrappers.zip).Content | Expand-Archive -DestinationPath .
+Invoke-WebRequest https://github.com/pyprojectx/pyprojectx/releases/latest/download/wrappers.zip -OutFile wrappers.zip; Expand-Archive -Path wrappers.zip -DestinationPath .; Remove-Item -Path wrappers.zip
 ```
 
 ## Project initialization
 Initialize a new or existing project with the _--init_ option (on Windows, replace `./pw` with `pw`):
 * `./pw --init project`: add pyprojectx example sections to an existing or new _pyproject.toml_ in the current directory.
-* `./pw --init poetry`: initialize a [Poetry](https://python-poetry.org/) project and add pyprojectx example sections to _pyproject.toml_.
 * `./pw --init pdm`: initialize a [PDM](https://pdm.fming.dev/) project and add pyprojectx example sections to _pyproject.toml_.
+* `./pw --init poetry`: initialize a [Poetry](https://python-poetry.org/) project and add pyprojectx example sections to _pyproject.toml_.
 
 ## Configuration
 Add the _tool.pyprojectx_ section inside _pyproject.toml_ in your project's root directory.
 
 Each entry has the form `tool = "pip-requirements"`, where _pip-requirements_ adheres to the
 [requirements file format](https://pip.pypa.io/en/stable/reference/requirements-file-format/).
 
@@ -66,15 +66,15 @@
 
 The _tool.pyprojectx.aliases_ section can contain optional commandline aliases in the form
 
 `alias = [@tool_key:] command`
 
 Example:
 ```toml
-[tool.pyprojectx.alias]
+[tool.pyprojectx.aliases]
 # convenience shortcuts
 run = "poetry run"
 test = "poetry run pytest"
 
 # flake8-black also contains the black script
 black = "@flake8: black"
 
@@ -108,15 +108,15 @@
 # same as above, but using the run alias
 ./pw run my-script --foo bar
 ```
 
 ## Why yet another tool?
 * As Python noob I had hard times setting up a project and building existing projects
 * There is always someone in the team having issues with his setup, either with a specific tool, with Homebrew, pipx, ...
-* Using (Poetry) dev-dependencies to install tools, impacts your production dependencies and can even lead to dependency conflicts
+* Using (PDM or Poetry) dev-dependencies to install tools, impacts your production dependencies and can even lead to dependency conflicts
 * Different projects often require different versions of the same tool
 
 ## Example projects
 * This project (using Poetry)
 * [px-demo](https://github.com/pyprojectx/px-demo) (using PDM)
 
 ## Development
```

### Comparing `pyprojectx-0.9.9/pyproject.toml` & `pyprojectx-1.0.0b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyprojectx"
-version = "0.9.9"
+version = "1.0.0b1"
 description = "Execute scripts from pyproject.toml, installing tools on-the-fly"
 license = "MIT"
 authors = ["Houbie <ivo@houbrechts-it.be>"]
 readme = "README.md"
 homepage = "https://github.com/pyprojectx/pyprojectx"
 documentation = "https://pyprojectx.github.io"
 keywords = ["build", "dependency", "pyprojectx"]
@@ -14,52 +14,54 @@
 ]
 
 [tool.poetry.scripts]
 pyprojectx = "pyprojectx.cli:main"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
-tomli = "^2.0.1"
-virtualenv = "^20.13.3"
-userpath = "^1.8.0"
+tomli = ">=2.0"
+virtualenv = ">=20.21"
+userpath = ">=1.8"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.0.1"
-pytest-mock = "^3.7.0"
+pytest = ">=7.3"
+pytest-mock = ">=3.10"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
 profile = "black"
 
 [tool.pylint.format]
 max-line-length = 120
 variable-rgx = '^[a-z_][a-z0-9_]*$'
+[tool.pylint.similarities]
+ignore-imports= true
 [tool.pylint.master]
 init-hook = """
 import sys
 sys.path.append(f".venv/lib/python{sys.version_info.major}.{sys.version_info.minor}/site-packages")
 sys.path.append(f".venv/Lib/site-packages")
 """
 [tool.pylint.messages_control]
 disable = [
     "missing-docstring",
     "unspecified-encoding"
 ]
 
 [tool.pyprojectx]
-poetry = { requirements = "poetry==1.1.13", post-install = "pw@pre-commit install" }
-black = "black==22.1.0"
-isort = "isort==5.10.1"
-pylint = "pylint==2.12.2"
+poetry = { requirements = "poetry==1.4.2", post-install = "pw@pre-commit install" }
+black = "black==23.3.0"
+isort = "isort==5.12.0"
+pylint = "pylint==2.17.2"
 pre-commit = "pre-commit"
 mkdocs = ["mkdocs ~=1.2", "mkdocs-material ~=8.2", "mkdocstrings[python] ~=0.18", "markdown-include ~=0.6", ]
 
 [tool.pyprojectx.aliases]
 install = "poetry install"
 run = "poetry run pyprojectx -t pyproject.toml "
 outdated = "poetry show --outdated"
@@ -94,15 +96,15 @@
 cp src/pyprojectx/wrapper/pw.bat dist-zip/pw.bat
 zip -j wrappers.zip dist-zip/pw*
 awk '/-{3,}/{flag=1;next}/Release/{if (flag==1)exit}flag' CHANGELOG.md > .changelog.md
 """
 
 generate-usage = "pw@ --help > docs/docs/usage.txt"
 serve-docs = "@mkdocs: cd docs && mkdocs serve"
-generate-docs = "@mkdocs: cd docs && mkdocs build"
+generate-docs = "@mkdocs: pw@generate-usage && cd docs && mkdocs build"
 deploy-docs = "@mkdocs: cd docs && mkdocs gh-deploy"
 
 [tool.pyprojectx.os.win.aliases]
 clean = "rmdir /s/q .venv .pytest_cache dist"
 clean-all = """\
 pw@clean
 rmdir /s/q .pyprojectx"""
```

### Comparing `pyprojectx-0.9.9/src/pyprojectx/cli.py` & `pyprojectx-1.0.0b1/src/pyprojectx/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,16 @@
     tool: Optional[str],
     alias_cmd: str,
     pw_args: List[str],
     requirements: dict,
     options,
 ) -> None:
     logger.debug("Running alias command, tool: %s, command: %s, arguments: %s", tool, alias_cmd, options.cmd_args)
-    full_cmd = " ".join([_replace_pw_references(alias_cmd, pw_args)] + options.cmd_args)
+    quoted_args = [f'"{a}"' for a in options.cmd_args]
+    full_cmd = " ".join([_replace_pw_references(alias_cmd, pw_args)] + quoted_args)
     if tool:
         _run_in_tool_venv(tool, full_cmd, requirements=requirements, options=options, pw_args=pw_args)
     else:
         try:
             subprocess.run(full_cmd, shell=True, check=True)
         except subprocess.CalledProcessError as e:
             raise SystemExit(e.returncode) from e
```

### Comparing `pyprojectx-0.9.9/src/pyprojectx/config.py` & `pyprojectx-1.0.0b1/src/pyprojectx/config.py`

 * *Files identical despite different names*

### Comparing `pyprojectx-0.9.9/src/pyprojectx/env.py` & `pyprojectx-1.0.0b1/src/pyprojectx/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         Remove the entire virtual environment
         """
         logger.info("Removing isolated environment in %s", self.path)
         shutil.rmtree(self.path)
 
     def run(self, cmd: Union[str, List[str]]) -> subprocess.CompletedProcess:
         """
-        Run a command inside the virual environment.
+        Run a command inside the virtual environment.
         :param cmd: The command string to run
         :return: The subprocess.CompletedProcess instance
         """
         logger.info("Running command in isolated venv %s: %s", self.name, cmd)
         if isinstance(cmd, List):
             extension = ".exe" if sys.platform.startswith("win") else ""
             cmd[0] = str(self.scripts_path.joinpath(cmd[0] + extension))
```

### Comparing `pyprojectx-0.9.9/src/pyprojectx/initializer/initializers.py` & `pyprojectx-1.0.0b1/src/pyprojectx/initializer/initializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     DEFAULT_INSTALL_DIR,
     PYPROJECT_TOML,
     RED,
     RESET,
 )
 
 SCRIPT_EXTENSION = ".bat" if sys.platform.startswith("win") else ""
-SCRIPT_PREFIX = "" if sys.platform.startswith("win") else "./"
+SCRIPT_PREFIX = ".\\" if sys.platform.startswith("win") else "./"
 
 HOME_DIR = Path(os.environ.get("PYPROJECTX_HOME_DIR", Path.home()))
 
 
 def initialize(options):
     return INIT_COMMANDS.get(options.cmd, show_help)(options)
```

### Comparing `pyprojectx-0.9.9/src/pyprojectx/initializer/pdm-template.toml` & `pyprojectx-1.0.0b1/src/pyprojectx/initializer/pdm-template.toml`

 * *Files identical despite different names*

### Comparing `pyprojectx-0.9.9/src/pyprojectx/initializer/poetry-template.toml` & `pyprojectx-1.0.0b1/src/pyprojectx/initializer/poetry-template.toml`

 * *Files identical despite different names*

### Comparing `pyprojectx-0.9.9/src/pyprojectx/initializer/project-template.toml` & `pyprojectx-1.0.0b1/src/pyprojectx/initializer/project-template.toml`

 * *Files identical despite different names*

### Comparing `pyprojectx-0.9.9/src/pyprojectx/wrapper/pw.py` & `pyprojectx-1.0.0b1/src/pyprojectx/wrapper/pw.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import argparse
 import os
 import subprocess
 import sys
 from pathlib import Path
 from venv import EnvBuilder
 
-VERSION = "0.9.9"
+VERSION = "1.0.0b1"
 
 PYPROJECTX_INSTALL_DIR_ENV_VAR = "PYPROJECTX_INSTALL_DIR"
 PYPROJECTX_PACKAGE_ENV_VAR = "PYPROJECTX_PACKAGE"
 PYPROJECT_TOML = "pyproject.toml"
 DEFAULT_INSTALL_DIR = ".pyprojectx"
 
 CYAN = "\033[96m"
```

### Comparing `pyprojectx-0.9.9/setup.py` & `pyprojectx-1.0.0b1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,163 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyprojectx
+Version: 1.0.0b1
+Summary: Execute scripts from pyproject.toml, installing tools on-the-fly
+Home-page: https://github.com/pyprojectx/pyprojectx
+License: MIT
+Keywords: build,dependency,pyprojectx
+Author: Houbie
+Author-email: ivo@houbrechts-it.be
+Requires-Python: >=3.7
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: tomli (>=2.0)
+Requires-Dist: userpath (>=1.8)
+Requires-Dist: virtualenv (>=20.21)
+Project-URL: Documentation, https://pyprojectx.github.io
+Description-Content-Type: text/markdown
+
+![pyprojectx](docs/docs/assets/px.png)
+
+# Pyprojectx: All-inclusive Python Projects
+
+Execute scripts from pyproject.toml, installing tools on-the-fly
+
+## [Full documentation](https://pyprojectx.github.io)
+
+## Introduction
+Pyprojectx makes it easy to create all-inclusive Python projects; no need to install any tools upfront,
+not even Pyprojectx itself!
+
+## Feature highlights
+* Reproducible builds by treating tools and utilities as (versioned) dev-dependencies
+* No global installs, everything is stored inside your project directory (like npm's _node_modules_)
+* Bootstrap your entire build process with a small wrapper script (like Gradle's _gradlew_ wrapper)
+* Configure shortcuts for routine tasks
+* Simple configuration in _pyproject.toml_
+
+Projects can be build/tested/used immediately without explicit installation nor initialization:
+```bash
+git clone https://github.com/pyprojectx/px-demo.git
+cd px-demo
+./pw build
+```
+![Clone and Build](https://raw.githubusercontent.com/pyprojectx/pyprojectx/main/docs/docs/assets/build.png)
+
+## Installation
+One of the key features is that there is no need to install anything explicitly (except a Python 3.7+ interpreter).
+
+`cd` into your project directory and download the
+[wrapper scripts](https://github.com/pyprojectx/pyprojectx/releases/latest/download/wrappers.zip):
+
+**Linux/Mac**
+```bash
+curl -LO https://github.com/pyprojectx/pyprojectx/releases/latest/download/wrappers.zip && unzip wrappers.zip && rm -f wrappers.zip
+```
+
+**Windows**
+```powershell
+Invoke-WebRequest https://github.com/pyprojectx/pyprojectx/releases/latest/download/wrappers.zip -OutFile wrappers.zip; Expand-Archive -Path wrappers.zip -DestinationPath .; Remove-Item -Path wrappers.zip
+```
+
+## Project initialization
+Initialize a new or existing project with the _--init_ option (on Windows, replace `./pw` with `pw`):
+* `./pw --init project`: add pyprojectx example sections to an existing or new _pyproject.toml_ in the current directory.
+* `./pw --init pdm`: initialize a [PDM](https://pdm.fming.dev/) project and add pyprojectx example sections to _pyproject.toml_.
+* `./pw --init poetry`: initialize a [Poetry](https://python-poetry.org/) project and add pyprojectx example sections to _pyproject.toml_.
+
+## Configuration
+Add the _tool.pyprojectx_ section inside _pyproject.toml_ in your project's root directory.
+
+Each entry has the form `tool = "pip-requirements"`, where _pip-requirements_ adheres to the
+[requirements file format](https://pip.pypa.io/en/stable/reference/requirements-file-format/).
+
+Example:
+```toml
+[tool.pyprojectx]
+# require a specific poetry version
+poetry = "poetry==1.1.13"
+# use the latest black
+isort = "isort"
+# install flake8 in combination with plugins
+flake8 = ["flake8", "flake8-black"]
+```
+
+The _tool.pyprojectx.aliases_ section can contain optional commandline aliases in the form
+
+`alias = [@tool_key:] command`
+
+Example:
+```toml
+[tool.pyprojectx.aliases]
+# convenience shortcuts
+run = "poetry run"
+test = "poetry run pytest"
+
+# flake8-black also contains the black script
+black = "@flake8: black"
+
+# simple shell commands
+clean = "rm -f .coverage .pytest_cache"
+
+# when running an alias from within another alias, prefix it with `pw@`
+check = "pw@flake8 && pw@test"
+```
+
+## Usage
+Instead of calling the commandline of a tool directly, prefix it with `path\to\pw`.
+
+Examples:
+```shell
+./pw poetry add -D pytest
+cd src
+../pw black *.py
+```
+
+... or on Windows:
+```shell
+pw poetry add -D pytest
+cd src
+..\pw black *.py
+```
+
+Aliases can be invoked as is or with extra arguments:
+```shell
+./pw poetry run my-script --foo bar
+# same as above, but using the run alias
+./pw run my-script --foo bar
+```
+
+## Why yet another tool?
+* As Python noob I had hard times setting up a project and building existing projects
+* There is always someone in the team having issues with his setup, either with a specific tool, with Homebrew, pipx, ...
+* Using (PDM or Poetry) dev-dependencies to install tools, impacts your production dependencies and can even lead to dependency conflicts
+* Different projects often require different versions of the same tool
+
+## Example projects
+* This project (using Poetry)
+* [px-demo](https://github.com/pyprojectx/px-demo) (using PDM)
+
+## Development
+* Build/test:
+```shell
+git clone https://github.com/pyprojectx/pyprojectx.git
+cd pyprojectx
+./pw build
+```
+
+* Set the path to pyprojectx in the _PYPROJECTX_PACKAGE_ environment variable
+  to use your local pyprojectx copy in another project.
+```shell
+# Linux, Mac
+export PYPROJECTX_PACKAGE=path/to/pyprojectx
+# windows
+set PYPROJECTX_PACKAGE=path/to/pyprojectx
+```
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['pyprojectx', 'pyprojectx.initializer', 'pyprojectx.wrapper']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['tomli>=2.0.1,<3.0.0', 'userpath>=1.8.0,<2.0.0', 'virtualenv>=20.13.3,<21.0.0']
-
-entry_points = \
-{'console_scripts': ['pyprojectx = pyprojectx.cli:main']}
-
-setup_kwargs = {
-    'name': 'pyprojectx',
-    'version': '0.9.9',
-    'description': 'Execute scripts from pyproject.toml, installing tools on-the-fly',
-    'long_description': '![pyprojectx](docs/docs/assets/px.png)\n\n# Pyprojectx: All-inclusive Python Projects\n\nExecute scripts from pyproject.toml, installing tools on-the-fly\n\n## [Full documentation](https://pyprojectx.github.io)\n\n## Introduction\nPyprojectx makes it easy to create all-inclusive Python projects; no need to install any tools upfront,\nnot even Pyprojectx itself!\n\n## Feature highlights\n* Reproducible builds by treating tools and utilities as (versioned) dev-dependencies\n* No global installs, everything is stored inside your project directory (like npm\'s _node_modules_)\n* Bootstrap your entire build process with a small wrapper script (like Gradle\'s _gradlew_ wrapper)\n* Configure shortcuts for routine tasks\n* Simple configuration in _pyproject.toml_\n\nProjects can be build/tested/used immediately without explicit installation nor initialization:\n```bash\ngit clone https://github.com/pyprojectx/px-demo.git\ncd px-demo\n./pw build\n```\n![Clone and Build](https://raw.githubusercontent.com/pyprojectx/pyprojectx/main/docs/docs/assets/build.png)\n\n## Installation\nOne of the key features is that there is no need to install anything explicitly (except a Python 3.7+ interpreter).\n\n`cd` into your project directory and download the\n[wrapper scripts](https://github.com/pyprojectx/pyprojectx/releases/latest/download/wrappers.zip):\n\n**Linux/Mac**\n```bash\ncurl -LO https://github.com/pyprojectx/pyprojectx/releases/latest/download/wrappers.zip && unzip wrappers.zip && rm -f wrappers.zip\n```\n\n**Windows**\n```powershell\n(Invoke-WebRequest https://github.com/pyprojectx/pyprojectx/releases/latest/download/wrappers.zip).Content | Expand-Archive -DestinationPath .\n```\n\n## Project initialization\nInitialize a new or existing project with the _--init_ option (on Windows, replace `./pw` with `pw`):\n* `./pw --init project`: add pyprojectx example sections to an existing or new _pyproject.toml_ in the current directory.\n* `./pw --init poetry`: initialize a [Poetry](https://python-poetry.org/) project and add pyprojectx example sections to _pyproject.toml_.\n* `./pw --init pdm`: initialize a [PDM](https://pdm.fming.dev/) project and add pyprojectx example sections to _pyproject.toml_.\n\n## Configuration\nAdd the _tool.pyprojectx_ section inside _pyproject.toml_ in your project\'s root directory.\n\nEach entry has the form `tool = "pip-requirements"`, where _pip-requirements_ adheres to the\n[requirements file format](https://pip.pypa.io/en/stable/reference/requirements-file-format/).\n\nExample:\n```toml\n[tool.pyprojectx]\n# require a specific poetry version\npoetry = "poetry==1.1.13"\n# use the latest black\nisort = "isort"\n# install flake8 in combination with plugins\nflake8 = ["flake8", "flake8-black"]\n```\n\nThe _tool.pyprojectx.aliases_ section can contain optional commandline aliases in the form\n\n`alias = [@tool_key:] command`\n\nExample:\n```toml\n[tool.pyprojectx.alias]\n# convenience shortcuts\nrun = "poetry run"\ntest = "poetry run pytest"\n\n# flake8-black also contains the black script\nblack = "@flake8: black"\n\n# simple shell commands\nclean = "rm -f .coverage .pytest_cache"\n\n# when running an alias from within another alias, prefix it with `pw@`\ncheck = "pw@flake8 && pw@test"\n```\n\n## Usage\nInstead of calling the commandline of a tool directly, prefix it with `path\\to\\pw`.\n\nExamples:\n```shell\n./pw poetry add -D pytest\ncd src\n../pw black *.py\n```\n\n... or on Windows:\n```shell\npw poetry add -D pytest\ncd src\n..\\pw black *.py\n```\n\nAliases can be invoked as is or with extra arguments:\n```shell\n./pw poetry run my-script --foo bar\n# same as above, but using the run alias\n./pw run my-script --foo bar\n```\n\n## Why yet another tool?\n* As Python noob I had hard times setting up a project and building existing projects\n* There is always someone in the team having issues with his setup, either with a specific tool, with Homebrew, pipx, ...\n* Using (Poetry) dev-dependencies to install tools, impacts your production dependencies and can even lead to dependency conflicts\n* Different projects often require different versions of the same tool\n\n## Example projects\n* This project (using Poetry)\n* [px-demo](https://github.com/pyprojectx/px-demo) (using PDM)\n\n## Development\n* Build/test:\n```shell\ngit clone https://github.com/pyprojectx/pyprojectx.git\ncd pyprojectx\n./pw build\n```\n\n* Set the path to pyprojectx in the _PYPROJECTX_PACKAGE_ environment variable\n  to use your local pyprojectx copy in another project.\n```shell\n# Linux, Mac\nexport PYPROJECTX_PACKAGE=path/to/pyprojectx\n# windows\nset PYPROJECTX_PACKAGE=path/to/pyprojectx\n```\n',
-    'author': 'Houbie',
-    'author_email': 'ivo@houbrechts-it.be',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/pyprojectx/pyprojectx',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7',
-}
-
-
-setup(**setup_kwargs)
```

