# Comparing `tmp/pacup-1.0.3.tar.gz` & `tmp/pacup-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pacup-1.0.3.tar", max compression
+gzip compressed data, was "pacup-1.1.0.tar", max compression
```

## Comparing `pacup-1.0.3.tar` & `pacup-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-02-25 15:42:28.350065 pacup-1.0.3/LICENSE
--rw-r--r--   0        0        0      829 2023-02-25 15:42:28.350065 pacup-1.0.3/LICENSE_BOILERPLATE
--rw-r--r--   0        0        0     7904 2023-02-25 15:42:28.350065 pacup-1.0.3/README.md
--rw-r--r--   0        0        0      870 2023-02-25 15:42:28.350065 pacup-1.0.3/pacup/__init__.py
--rw-r--r--   0        0        0    33149 2023-02-25 15:42:28.350065 pacup-1.0.3/pacup/__main__.py
--rw-r--r--   0        0        0    10396 2023-02-25 15:42:28.354065 pacup-1.0.3/pacup/parser.py
--rw-r--r--   0        0        0     6617 2023-02-25 15:42:28.354065 pacup-1.0.3/pacup/release_notes.py
--rw-r--r--   0        0        0     1207 2023-02-25 15:42:28.354065 pacup-1.0.3/pacup/utils.py
--rw-r--r--   0        0        0     7683 2023-02-25 15:42:28.354065 pacup-1.0.3/pacup/version.py
--rw-r--r--   0        0        0     1928 2023-02-25 15:42:28.354065 pacup-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     8871 1970-01-01 00:00:00.000000 pacup-1.0.3/setup.py
--rw-r--r--   0        0        0     9480 1970-01-01 00:00:00.000000 pacup-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-09 18:28:38.038072 pacup-1.1.0/LICENSE
+-rw-r--r--   0        0        0      829 2023-04-09 18:28:38.038072 pacup-1.1.0/LICENSE_BOILERPLATE
+-rw-r--r--   0        0        0     7904 2023-04-09 18:28:38.038072 pacup-1.1.0/README.md
+-rw-r--r--   0        0        0      870 2023-04-09 18:28:38.038072 pacup-1.1.0/pacup/__init__.py
+-rw-r--r--   0        0        0    33430 2023-04-09 18:28:38.038072 pacup-1.1.0/pacup/__main__.py
+-rw-r--r--   0        0        0    10404 2023-04-09 18:28:38.038072 pacup-1.1.0/pacup/parser.py
+-rw-r--r--   0        0        0     6617 2023-04-09 18:28:38.038072 pacup-1.1.0/pacup/release_notes.py
+-rw-r--r--   0        0        0     1207 2023-04-09 18:28:38.038072 pacup-1.1.0/pacup/utils.py
+-rw-r--r--   0        0        0     7683 2023-04-09 18:28:38.038072 pacup-1.1.0/pacup/version.py
+-rw-r--r--   0        0        0     1951 2023-04-09 18:28:38.038072 pacup-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9480 1970-01-01 00:00:00.000000 pacup-1.1.0/PKG-INFO
```

### Comparing `pacup-1.0.3/LICENSE` & `pacup-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pacup-1.0.3/LICENSE_BOILERPLATE` & `pacup-1.1.0/LICENSE_BOILERPLATE`

 * *Files identical despite different names*

### Comparing `pacup-1.0.3/README.md` & `pacup-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pacup-1.0.3/pacup/__init__.py` & `pacup-1.1.0/pacup/__init__.py`

 * *Files identical despite different names*

### Comparing `pacup-1.0.3/pacup/__main__.py` & `pacup-1.1.0/pacup/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 from rich.syntax import Syntax
 from rich.table import Table
 
 from pacup.parser import Pacscript
 from pacup.utils import level
 from pacup.version import VersionStatuses
 
-__version__ = "1.0.3 Chiron"
+__version__ = "1.1.0 Io"
 
 app = typer.Typer(name="pacup")
 
 
 basicConfig(level="CRITICAL", format="%(message)s", handlers=[RichHandler(markup=True)])
 log = getLogger("rich")
 
@@ -512,18 +512,20 @@
                 TimeRemainingColumn(),
                 "•",
                 TransferSpeedColumn(),
             ) as downloading_package_progress:
                 task = downloading_package_progress.add_task(
                     "Downloading package", start=False
                 )
+                latest_url = url.value.replace(version.current, version.latest)
+                file_name = latest_url.split("/")[-1]
                 try:
                     latest_hash = loop.run_until_complete(
                         download(
-                            url.value.replace(version.current, version.latest),
+                            latest_url,
                             downloading_package_progress,
                             task,
                         )
                     )
                 except HTTPStatusError as error:
                     downloading_package_progress.advance(task)
                     rprint(
@@ -539,18 +541,14 @@
                     rprint(
                         f"{padding}[bold red]❌[/bold red] Could not download package: {error}"
                     )
                     failed_to_update_pacscripts[
                         pacscript
                     ] = f"{str(error) or type(error).__name__}"
                     continue
-                finally:
-                    # Clear downloaded packages
-                    log.info("Clearing downloaded package...")
-                    rmtree("/tmp/pacup", ignore_errors=True)
 
             # Edit the pacscript file with the new version and hash
             log.info("Editing pacscript file...")
             rprint(f"{padding}[bold blue]=>[/bold blue] Editing pacscript")
             edited_lines = lines.copy()
             edited_lines[version.line_number] = f'version="{version.latest}"\n'
 
@@ -574,28 +572,28 @@
                     ),
                     title="Diff",
                     border_style="bold blue",
                 )
             )
 
             if ship:
-                log.info(f"Checking out [bold blue]master[/bold blue] branch...")
+                log.info("Checking out [bold blue]master[/bold blue] branch...")
 
                 try:
                     subprocess.run(
                         ["git", "checkout", "master"], check=True, capture_output=True
                     )
                 except subprocess.CalledProcessError as error:
                     log.error(
                         f"Could not checkout master branch: [bold red]{error.stderr.decode()}[/bold red]"
                     )
 
                     failed_to_update_pacscripts[
                         pacscript
-                    ] = f"Failed to checkout master branch"
+                    ] = "Failed to checkout master branch"
                     break
 
                 # Checkout the ship branch
                 try:
                     log.info(f"Checking out [bold blue]ship-{path.stem} branch...")
                     subprocess.run(
                         ["git", "checkout", "-b", f"ship-{path.stem}"],
@@ -686,31 +684,44 @@
 
             rprint(
                 f"{padding}[bold blue]=>[/bold blue] Installing pacscript using pacstall"
             )
             rprint(f"[bold blue]{'─' * get_terminal_size().columns}[/bold blue]")
 
             try:
-                subprocess.run(["pacstall", "-I", path], check=True)
+                subprocess.run(
+                    [
+                        "bash",
+                        "-c",
+                        f"PACSTALL_PAYLOAD=/tmp/pacup/{file_name} pacstall -I {path}",
+                    ],
+                    check=True,
+                )
             except subprocess.CalledProcessError:
                 log.warning(f"Could not install {path.name}")
                 rprint(f"[bold red]{'─' * get_terminal_size().columns}\n[/bold red]")
                 rprint(
                     f"{padding}[bold red]❌[/bold red]Failed to install pacscript [bold red]{path.stem}[/bold red] pacscript\n"
                 )
                 failed_to_update_pacscripts[
                     pacscript
                 ] = "Installation using pacstall failed"
                 continue
+
             else:
                 rprint(f"[bold blue]{'─' * get_terminal_size().columns}[/bold blue]")
                 rprint(
                     f"{padding}[bold green]:heavy_check_mark:[/bold green] Successfully installed [bold blue]{path.stem}[/bold blue] pacscript",
                 )
 
+            finally:
+                # Clear downloaded packages
+                log.info("Clearing downloaded package...")
+                rmtree("/tmp/pacup", ignore_errors=True)
+
             # Ask the user to check the installed package
             # Succeed if the user confirms
             log.info("Asking user to check installed pacscript...")
             if Confirm.ask(f"{padding}[bold blue]::[/bold blue] Does {pkgname} work?"):
                 rprint(
                     f"{padding}[bold blue]=>[/bold blue] Finished updating pacscript [bold blue]{path.stem}[/bold blue] pacscript!"
                 )
```

### Comparing `pacup-1.0.3/pacup/parser.py` & `pacup-1.1.0/pacup/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         url = Url()
         hash_line = -1  # Which line contains the hash
         maintainer = ""
         repology_filters: Dict[str, str] = {}
         release_notes = {}
 
         pacscript_reader_process = await create_subprocess_shell(
-            "/bin/bash", stdin=PIPE, stdout=PIPE
+            "/usr/bin/env bash", stdin=PIPE, stdout=PIPE
         )
 
         assert pacscript_reader_process.stdin is not None
         log.info(f"Sourcing {path.name}...")
         pacscript_reader_process.stdin.write(f"source {path.absolute()}\n".encode())
         await pacscript_reader_process.stdin.drain()
```

### Comparing `pacup-1.0.3/pacup/release_notes.py` & `pacup-1.1.0/pacup/release_notes.py`

 * *Files identical despite different names*

### Comparing `pacup-1.0.3/pacup/utils.py` & `pacup-1.1.0/pacup/utils.py`

 * *Files identical despite different names*

### Comparing `pacup-1.0.3/pacup/version.py` & `pacup-1.1.0/pacup/version.py`

 * *Files identical despite different names*

### Comparing `pacup-1.0.3/pyproject.toml` & `pacup-1.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 [tool.poetry]
 name = "pacup"
-version = "1.0.3"
+version = "1.1.0"
 description = "Help maintainers update pacscripts"
 readme = "README.md"
 authors = ["Sourajyoti Basak <wiz28@protonmail.com>"]
 license = "GPL-3.0-or-later"
 repository = "https://github.com/pacstall/pacup"
 documentation = "https://github.com/pacstall/pacup/wiki"
 keywords = [
-	"aur",
-	"cli",
-	"command line",
-	"console",
-	"debian",
-	"pacscript",
-	"pacstall",
-	"ubuntu",
-	"repology",
+  "aur",
+  "cli",
+  "command line",
+  "console",
+  "debian",
+  "pacscript",
+  "pacstall",
+  "ubuntu",
+  "repology",
 ]
 classifiers = [
-	"Development Status :: 4 - Beta",
-	"Environment :: Console",
-	"Intended Audience :: Developers",
-	"License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-	"Operating System :: POSIX :: Linux",
-	"Programming Language :: Python :: 3 :: Only",
-	"Programming Language :: Python :: 3.8",
-	"Programming Language :: Python :: 3.9",
-	"Programming Language :: Python :: 3.10",
-	"Programming Language :: Python :: 3.11",
-	"Programming Language :: Python :: Implementation :: CPython",
-	"Topic :: System",
-	"Topic :: Utilities",
-	"Typing :: Typed",
+  "Development Status :: 4 - Beta",
+  "Environment :: Console",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+  "Operating System :: POSIX :: Linux",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: Implementation :: CPython",
+  "Topic :: System",
+  "Topic :: Utilities",
+  "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 httpx = ">=0.22,<0.24"
 rich = "^13.0.0"
 typer = ">=0.4.1,<0.8.0"
```

### Comparing `pacup-1.0.3/setup.py` & `pacup-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,167 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pacup
+Version: 1.1.0
+Summary: Help maintainers update pacscripts
+Home-page: https://github.com/pacstall/pacup
+License: GPL-3.0-or-later
+Keywords: aur,cli,command line,console,debian,pacscript,pacstall,ubuntu,repology
+Author: Sourajyoti Basak
+Author-email: wiz28@protonmail.com
+Requires-Python: >=3.8,<3.12
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: System
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Dist: httpx (>=0.22,<0.24)
+Requires-Dist: packaging (>=23,<23.1)
+Requires-Dist: rich (>=13.0.0,<14.0.0)
+Requires-Dist: typer (>=0.4.1,<0.8.0)
+Project-URL: Documentation, https://github.com/pacstall/pacup/wiki
+Project-URL: Repository, https://github.com/pacstall/pacup
+Description-Content-Type: text/markdown
+
+<p align="center"><img alt="logo" src="https://raw.githubusercontent.com/pacstall/pacup/master/imgs/logo.png"></p>
+<h1 align="center">Pacup</h1>
+<p align="center">
+  <a href="https://www.python.org/"><img alt="Python: 3.8+" src="https://img.shields.io/badge/python-3.8%2B-306998?logo=python&logoColor=white&style=for-the-badge"></a>
+  <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-black?style=for-the-badge"/></a>
+  <a href="https://www.codacy.com/gh/pacstall/pacup/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pacstall/pacup&amp;utm_campaign=Badge_Grade"><img alt="Codacy: grade" src="https://img.shields.io/codacy/grade/4b1365e6f7d2474283243f62b2c5973d?label=Codacy&logo=codacy&style=for-the-badge"></a>
+  <a href="https://pypi.org/project/pacup/"><img alt="PyPI: version" src="https://img.shields.io/pypi/v/pacup?color=%233775a9&logo=pypi&logoColor=white&style=for-the-badge"></a>
+<p/>
+<p align="center">
+  <!-- Social -->
+  <a href="https://discord.gg/yzrjXJV6K8"><img alt="join discord" src="https://img.shields.io/discord/839818021207801878?color=5865F2&label=Discord&logo=discord&logoColor=FFFFFF&style=for-the-badge"></a>
+  <a href="https://reddit.com/r/pacstall"><img src="https://img.shields.io/reddit/subreddit-subscribers/pacstall?label=Reddit&color=FF4301&style=for-the-badge&logo=reddit&logoColor=FFFFFF" loading="lazy"></a>
+  <a href="https://social.linux.pizza/web/@pacstall"><img alt="Mastodon Follow" src="https://img.shields.io/mastodon/follow/107278715447740005?color=3088d4&domain=https%3A%2F%2Fsocial.linux.pizza&label=Mastodon&logo=mastodon&logoColor=white&style=for-the-badge" loading="lazy"></a>
+  <a href="https://matrix.to/#/#pacstall:matrix.org"><img alt="join matrix" src="https://img.shields.io/matrix/pacstall:matrix.org?color=888888&label=Matrix&logo=Matrix&style=for-the-badge"></a>
+<p/>
+
+## What is this?
+
+Pacup (**Pac**script **Up**dater) is a maintainer helper tool to help
+maintainers update their pacscripts. It semi-automates the tedious task of
+updating pacscripts, and aims to make it a fun process for the maintainer!
+
+## Installation
+
+To install the latest release run:
+
+```console
+$ pacstall -I pacup-bin # or pip install pacup
+```
+
+To install the latest development build run:
+
+```console
+$ pip install git+https://github.com/pacstall/pacup
+```
+
+## Usage
+
+```console
+Usage: pacup [OPTIONS] PACSCRIPTS...
+
+Updates specified pacscripts.
+If ship flag is passed, the pacscript will be prepared for shipping to upstream.
+After the pacscript is prepared, it will be committed and pushed to the origin remote.
+This requires you to be present in your cloned fork.
+
+╭─ Arguments ──────────────────────────────────────────────────────────────────────────────────────────╮
+│ *    pacscripts      PACSCRIPTS...  The pacscripts to update. [default: None] [required]             │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --show-repology       -r                                       Show the parsed repology data and     │
+│                                                                exit.                                 │
+│ --debug               -d                                       Turn on debugging mode.               │
+│ --version             -v                                       Show the version and exit.            │
+│ --ship                -s                                       Prepare the pacscript for shipping to │
+│                                                                upstream.                             │
+│ --install-completion          [bash|zsh|fish|powershell|pwsh]  Install completion for the specified  │
+│                                                                shell.                                │
+│                                                                [default: None]                       │
+│ --show-completion             [bash|zsh|fish|powershell|pwsh]  Show completion for the specified     │
+│                                                                shell, to copy it or customize the    │
+│                                                                installation.                         │
+│                                                                [default: None]                       │
+│ --help                                                         Show this message and exit.           │
+╰──────────────────────────────────────────────────────────────────────────────────────────────────────╯
+```
+
+You can get this help text by running `pacup --help`.
+
+You should visit our [wiki](https://github.com/pacstall/pacup/wiki/Wiki), for
+more information on how to use the `repology` key.
+
+## How does it work?
+
+Suppose `foo.pacscript` is outdated.
+
+On running `pacup foo.pacscript` Pacup will parse the pacscript's variables,
+then it compiles a list of filters specified in the `repology` variable in the
+pacscript. Then it queries the [Repology API](https://repology.org/api) to get
+all the repositories which have packaged that package. After which it applies
+the filter to the response, and from the filtrate it considers the most common
+version to be the latest.
+
+Then it replaces all occurrences of the previous `version`'s value in the `url`
+with the latest one placeholder's value with the latest version, and downloads
+the new package, and generates it's hash.
+
+Then writes the edited pacscript and installs it with
+[Pacstall](https://github.com/pacstall/pacstall), after installation it asks
+the user to confirm that the installed package works. On approval the pacscript
+is considered successfully upgraded and the program ends.
+
+## Caveats
+
+* Does not work with `-git` pacscripts as those pacscripts are auto updating.
+* Doesn't work if a pacscript doesn't have an equivalent
+  [Repology](https://repology.org/) package.
+
+## Stats
+
+<p align="center"><img alt="Repobeats analytics image" src="https://repobeats.axiom.co/api/embed/80bc45a6d65fbfb43905aa22b3950badc09edd97.svg" /></p>
+
+## License
+
+```monospace
+    ____             __  __
+   / __ \____ ______/ / / /___
+  / /_/ / __ `/ ___/ / / / __ \
+ / ____/ /_/ / /__/ /_/ / /_/ /
+/_/    \__,_/\___/\____/ .___/
+                      /_/
+
+Copyright (C) 2022-present
+
+This file is part of PacUp
+
+PacUp is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+PacUp is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with PacUp.  If not, see <https://www.gnu.org/licenses/>.
+```
 
-packages = \
-['pacup']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['httpx>=0.22,<0.24',
- 'packaging>=23,<23.1',
- 'rich>=13.0.0,<14.0.0',
- 'typer>=0.4.1,<0.8.0']
-
-entry_points = \
-{'console_scripts': ['pacup = pacup.__main__:main']}
-
-setup_kwargs = {
-    'name': 'pacup',
-    'version': '1.0.3',
-    'description': 'Help maintainers update pacscripts',
-    'long_description': '<p align="center"><img alt="logo" src="https://raw.githubusercontent.com/pacstall/pacup/master/imgs/logo.png"></p>\n<h1 align="center">Pacup</h1>\n<p align="center">\n  <a href="https://www.python.org/"><img alt="Python: 3.8+" src="https://img.shields.io/badge/python-3.8%2B-306998?logo=python&logoColor=white&style=for-the-badge"></a>\n  <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-black?style=for-the-badge"/></a>\n  <a href="https://www.codacy.com/gh/pacstall/pacup/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pacstall/pacup&amp;utm_campaign=Badge_Grade"><img alt="Codacy: grade" src="https://img.shields.io/codacy/grade/4b1365e6f7d2474283243f62b2c5973d?label=Codacy&logo=codacy&style=for-the-badge"></a>\n  <a href="https://pypi.org/project/pacup/"><img alt="PyPI: version" src="https://img.shields.io/pypi/v/pacup?color=%233775a9&logo=pypi&logoColor=white&style=for-the-badge"></a>\n<p/>\n<p align="center">\n  <!-- Social -->\n  <a href="https://discord.gg/yzrjXJV6K8"><img alt="join discord" src="https://img.shields.io/discord/839818021207801878?color=5865F2&label=Discord&logo=discord&logoColor=FFFFFF&style=for-the-badge"></a>\n  <a href="https://reddit.com/r/pacstall"><img src="https://img.shields.io/reddit/subreddit-subscribers/pacstall?label=Reddit&color=FF4301&style=for-the-badge&logo=reddit&logoColor=FFFFFF" loading="lazy"></a>\n  <a href="https://social.linux.pizza/web/@pacstall"><img alt="Mastodon Follow" src="https://img.shields.io/mastodon/follow/107278715447740005?color=3088d4&domain=https%3A%2F%2Fsocial.linux.pizza&label=Mastodon&logo=mastodon&logoColor=white&style=for-the-badge" loading="lazy"></a>\n  <a href="https://matrix.to/#/#pacstall:matrix.org"><img alt="join matrix" src="https://img.shields.io/matrix/pacstall:matrix.org?color=888888&label=Matrix&logo=Matrix&style=for-the-badge"></a>\n<p/>\n\n## What is this?\n\nPacup (**Pac**script **Up**dater) is a maintainer helper tool to help\nmaintainers update their pacscripts. It semi-automates the tedious task of\nupdating pacscripts, and aims to make it a fun process for the maintainer!\n\n## Installation\n\nTo install the latest release run:\n\n```console\n$ pacstall -I pacup-bin # or pip install pacup\n```\n\nTo install the latest development build run:\n\n```console\n$ pip install git+https://github.com/pacstall/pacup\n```\n\n## Usage\n\n```console\nUsage: pacup [OPTIONS] PACSCRIPTS...\n\nUpdates specified pacscripts.\nIf ship flag is passed, the pacscript will be prepared for shipping to upstream.\nAfter the pacscript is prepared, it will be committed and pushed to the origin remote.\nThis requires you to be present in your cloned fork.\n\n╭─ Arguments ──────────────────────────────────────────────────────────────────────────────────────────╮\n│ *    pacscripts      PACSCRIPTS...  The pacscripts to update. [default: None] [required]             │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────╮\n│ --show-repology       -r                                       Show the parsed repology data and     │\n│                                                                exit.                                 │\n│ --debug               -d                                       Turn on debugging mode.               │\n│ --version             -v                                       Show the version and exit.            │\n│ --ship                -s                                       Prepare the pacscript for shipping to │\n│                                                                upstream.                             │\n│ --install-completion          [bash|zsh|fish|powershell|pwsh]  Install completion for the specified  │\n│                                                                shell.                                │\n│                                                                [default: None]                       │\n│ --show-completion             [bash|zsh|fish|powershell|pwsh]  Show completion for the specified     │\n│                                                                shell, to copy it or customize the    │\n│                                                                installation.                         │\n│                                                                [default: None]                       │\n│ --help                                                         Show this message and exit.           │\n╰──────────────────────────────────────────────────────────────────────────────────────────────────────╯\n```\n\nYou can get this help text by running `pacup --help`.\n\nYou should visit our [wiki](https://github.com/pacstall/pacup/wiki/Wiki), for\nmore information on how to use the `repology` key.\n\n## How does it work?\n\nSuppose `foo.pacscript` is outdated.\n\nOn running `pacup foo.pacscript` Pacup will parse the pacscript\'s variables,\nthen it compiles a list of filters specified in the `repology` variable in the\npacscript. Then it queries the [Repology API](https://repology.org/api) to get\nall the repositories which have packaged that package. After which it applies\nthe filter to the response, and from the filtrate it considers the most common\nversion to be the latest.\n\nThen it replaces all occurrences of the previous `version`\'s value in the `url`\nwith the latest one placeholder\'s value with the latest version, and downloads\nthe new package, and generates it\'s hash.\n\nThen writes the edited pacscript and installs it with\n[Pacstall](https://github.com/pacstall/pacstall), after installation it asks\nthe user to confirm that the installed package works. On approval the pacscript\nis considered successfully upgraded and the program ends.\n\n## Caveats\n\n* Does not work with `-git` pacscripts as those pacscripts are auto updating.\n* Doesn\'t work if a pacscript doesn\'t have an equivalent\n  [Repology](https://repology.org/) package.\n\n## Stats\n\n<p align="center"><img alt="Repobeats analytics image" src="https://repobeats.axiom.co/api/embed/80bc45a6d65fbfb43905aa22b3950badc09edd97.svg" /></p>\n\n## License\n\n```monospace\n    ____             __  __\n   / __ \\____ ______/ / / /___\n  / /_/ / __ `/ ___/ / / / __ \\\n / ____/ /_/ / /__/ /_/ / /_/ /\n/_/    \\__,_/\\___/\\____/ .___/\n                      /_/\n\nCopyright (C) 2022-present\n\nThis file is part of PacUp\n\nPacUp is free software: you can redistribute it and/or modify\nit under the terms of the GNU General Public License as published by\nthe Free Software Foundation, either version 3 of the License, or\n(at your option) any later version.\n\nPacUp is distributed in the hope that it will be useful,\nbut WITHOUT ANY WARRANTY; without even the implied warranty of\nMERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the\nGNU General Public License for more details.\n\nYou should have received a copy of the GNU General Public License\nalong with PacUp.  If not, see <https://www.gnu.org/licenses/>.\n```\n',
-    'author': 'Sourajyoti Basak',
-    'author_email': 'wiz28@protonmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/pacstall/pacup',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.12',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,77 +1,84 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['pacup']
-package_data = \ {'': ['*']} install_requires = \ ['httpx>=0.22,<0.24',
-'packaging>=23,<23.1', 'rich>=13.0.0,<14.0.0', 'typer>=0.4.1,<0.8.0']
-entry_points = \ {'console_scripts': ['pacup = pacup.__main__:main']}
-setup_kwargs = { 'name': 'pacup', 'version': '1.0.3', 'description': 'Help
-maintainers update pacscripts', 'long_description': '
+Metadata-Version: 2.1 Name: pacup Version: 1.1.0 Summary: Help maintainers
+update pacscripts Home-page: https://github.com/pacstall/pacup License: GPL-
+3.0-or-later Keywords: aur,cli,command
+line,console,debian,pacscript,pacstall,ubuntu,repology Author: Sourajyoti Basak
+Author-email: wiz28@protonmail.com Requires-Python: >=3.8,<3.12 Classifier:
+Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
+Intended Audience :: Developers Classifier: License :: OSI Approved :: GNU
+General Public License v3 or later (GPLv3+) Classifier: Operating System ::
+POSIX :: Linux Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: System Classifier: Topic :: Utilities Classifier: Typing
+:: Typed Requires-Dist: httpx (>=0.22,<0.24) Requires-Dist: packaging
+(>=23,<23.1) Requires-Dist: rich (>=13.0.0,<14.0.0) Requires-Dist: typer
+(>=0.4.1,<0.8.0) Project-URL: Documentation, https://github.com/pacstall/pacup/
+wiki Project-URL: Repository, https://github.com/pacstall/pacup Description-
+Content-Type: text/markdown
                                     [logo]
-\n
                               ****** Pacup ******
-\n
- \n [Python:_3.8+]\n [Code_style:_black]\n [Codacy:_grade]\n [PyPI:_version]\n
-\n
- \n \n [join_discord]\n [https://img.shields.io/reddit/subreddit-subscribers/
+      [Python:_3.8+] [Code_style:_black] [Codacy:_grade] [PyPI:_version]
+      [join_discord] [https://img.shields.io/reddit/subreddit-subscribers/
                pacstall?label=Reddit&color=FF4301&style=for-the-
-   badge&logo=reddit&logoColor=FFFFFF]\n [Mastodon_Follow]\n [join_matrix]\n
-\n\n## What is this?\n\nPacup (**Pac**script **Up**dater) is a maintainer
-helper tool to help\nmaintainers update their pacscripts. It semi-automates the
-tedious task of\nupdating pacscripts, and aims to make it a fun process for the
-maintainer!\n\n## Installation\n\nTo install the latest release run:
-\n\n```console\n$ pacstall -I pacup-bin # or pip install pacup\n```\n\nTo
-install the latest development build run:\n\n```console\n$ pip install
-git+https://github.com/pacstall/pacup\n```\n\n## Usage\n\n```console\nUsage:
-pacup [OPTIONS] PACSCRIPTS...\n\nUpdates specified pacscripts.\nIf ship flag is
-passed, the pacscript will be prepared for shipping to upstream.\nAfter the
-pacscript is prepared, it will be committed and pushed to the origin
-remote.\nThis requires you to be present in your cloned fork.\n\nâ­â
-Arguments
-âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®\nâ
-* pacscripts PACSCRIPTS... The pacscripts to update. [default: None] [required]
-â\nâ°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯\nâ­â
-Options
-âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®\nâ
---show-repology -r Show the parsed repology data and â\nâ exit. â\nâ --
-debug -d Turn on debugging mode. â\nâ --version -v Show the version and
-exit. â\nâ --ship -s Prepare the pacscript for shipping to â\nâ
-upstream. â\nâ --install-completion [bash|zsh|fish|powershell|pwsh] Install
-completion for the specified â\nâ shell. â\nâ [default: None] â\nâ
---show-completion [bash|zsh|fish|powershell|pwsh] Show completion for the
-specified â\nâ shell, to copy it or customize the â\nâ installation.
-â\nâ [default: None] â\nâ --help Show this message and exit.
-â\nâ°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯\n```\n\nYou
-can get this help text by running `pacup --help`.\n\nYou should visit our
-[wiki](https://github.com/pacstall/pacup/wiki/Wiki), for\nmore information on
-how to use the `repology` key.\n\n## How does it work?\n\nSuppose
-`foo.pacscript` is outdated.\n\nOn running `pacup foo.pacscript` Pacup will
-parse the pacscript\'s variables,\nthen it compiles a list of filters specified
-in the `repology` variable in the\npacscript. Then it queries the [Repology
-API](https://repology.org/api) to get\nall the repositories which have packaged
-that package. After which it applies\nthe filter to the response, and from the
-filtrate it considers the most common\nversion to be the latest.\n\nThen it
-replaces all occurrences of the previous `version`\'s value in the `url`\nwith
-the latest one placeholder\'s value with the latest version, and downloads\nthe
-new package, and generates it\'s hash.\n\nThen writes the edited pacscript and
-installs it with\n[Pacstall](https://github.com/pacstall/pacstall), after
-installation it asks\nthe user to confirm that the installed package works. On
-approval the pacscript\nis considered successfully upgraded and the program
-ends.\n\n## Caveats\n\n* Does not work with `-git` pacscripts as those
-pacscripts are auto updating.\n* Doesn\'t work if a pacscript doesn\'t have an
-equivalent\n [Repology](https://repology.org/) package.\n\n## Stats\n\n
+      badge&logo=reddit&logoColor=FFFFFF] [Mastodon_Follow] [join_matrix]
+## What is this? Pacup (**Pac**script **Up**dater) is a maintainer helper tool
+to help maintainers update their pacscripts. It semi-automates the tedious task
+of updating pacscripts, and aims to make it a fun process for the maintainer!
+## Installation To install the latest release run: ```console $ pacstall -
+I pacup-bin # or pip install pacup ``` To install the latest development build
+run: ```console $ pip install git+https://github.com/pacstall/pacup ``` ##
+Usage ```console Usage: pacup [OPTIONS] PACSCRIPTS... Updates specified
+pacscripts. If ship flag is passed, the pacscript will be prepared for shipping
+to upstream. After the pacscript is prepared, it will be committed and pushed
+to the origin remote. This requires you to be present in your cloned fork.
+â­â Arguments
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â * pacscripts PACSCRIPTS... The pacscripts to update. [default: None]
+[required] â
+â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â Options
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â --show-repology -r Show the parsed repology data and â â exit. â â
+--debug -d Turn on debugging mode. â â --version -v Show the version and
+exit. â â --ship -s Prepare the pacscript for shipping to â â upstream.
+â â --install-completion [bash|zsh|fish|powershell|pwsh] Install completion
+for the specified â â shell. â â [default: None] â â --show-
+completion [bash|zsh|fish|powershell|pwsh] Show completion for the specified
+â â shell, to copy it or customize the â â installation. â â
+[default: None] â â --help Show this message and exit. â
+â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` You can get this help text by running `pacup --help`. You should visit our
+[wiki](https://github.com/pacstall/pacup/wiki/Wiki), for more information on
+how to use the `repology` key. ## How does it work? Suppose `foo.pacscript` is
+outdated. On running `pacup foo.pacscript` Pacup will parse the pacscript's
+variables, then it compiles a list of filters specified in the `repology`
+variable in the pacscript. Then it queries the [Repology API](https://
+repology.org/api) to get all the repositories which have packaged that package.
+After which it applies the filter to the response, and from the filtrate it
+considers the most common version to be the latest. Then it replaces all
+occurrences of the previous `version`'s value in the `url` with the latest one
+placeholder's value with the latest version, and downloads the new package, and
+generates it's hash. Then writes the edited pacscript and installs it with
+[Pacstall](https://github.com/pacstall/pacstall), after installation it asks
+the user to confirm that the installed package works. On approval the pacscript
+is considered successfully upgraded and the program ends. ## Caveats * Does not
+work with `-git` pacscripts as those pacscripts are auto updating. * Doesn't
+work if a pacscript doesn't have an equivalent [Repology](https://repology.org/
+) package. ## Stats
                           [Repobeats analytics image]
-\n\n## License\n\n```monospace\n ____ __ __\n / __ \\____ ______/ / / /___\n /
-/_/ / __ `/ ___/ / / / __ \\\n / ____/ /_/ / /__/ /_/ / /_/ /\n/_/ \\__,_/
-\\___/\\____/ .___/\n /_/\n\nCopyright (C) 2022-present\n\nThis file is part of
-PacUp\n\nPacUp is free software: you can redistribute it and/or modify\nit
-under the terms of the GNU General Public License as published by\nthe Free
-Software Foundation, either version 3 of the License, or\n(at your option) any
-later version.\n\nPacUp is distributed in the hope that it will be useful,\nbut
-WITHOUT ANY WARRANTY; without even the implied warranty of\nMERCHANTABILITY or
-FITNESS FOR A PARTICULAR PURPOSE. See the\nGNU General Public License for more
-details.\n\nYou should have received a copy of the GNU General Public
-License\nalong with PacUp. If not, see
-www.gnu.org/licenses/>.\n```\n', 'author': 'Sourajyoti Basak', 'author_email':
-'wiz28@protonmail.com', 'maintainer': 'None', 'maintainer_email': 'None',
-'url': 'https://github.com/pacstall/pacup', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'entry_points': entry_points, 'python_requires': '>=3.8,<3.12', } setup
-(**setup_kwargs)
+## License ```monospace ____ __ __ / __ \____ ______/ / / /___ / /_/ / __ `/
+___/ / / / __ \ / ____/ /_/ / /__/ /_/ / /_/ / /_/ \__,_/\___/\____/ .___/ /_/
+Copyright (C) 2022-present This file is part of PacUp PacUp is free software:
+you can redistribute it and/or modify it under the terms of the GNU General
+Public License as published by the Free Software Foundation, either version 3
+of the License, or (at your option) any later version. PacUp is distributed in
+the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the
+implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See
+the GNU General Public License for more details. You should have received a
+copy of the GNU General Public License along with PacUp. If not, see
+www.gnu.org/licenses/>. ```
```

