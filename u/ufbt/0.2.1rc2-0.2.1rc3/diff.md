# Comparing `tmp/ufbt-0.2.1rc2.tar.gz` & `tmp/ufbt-0.2.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufbt-0.2.1rc2.tar", last modified: Sun Apr  9 12:59:58 2023, max compression
+gzip compressed data, was "ufbt-0.2.1rc3.tar", last modified: Sun Apr  9 14:57:43 2023, max compression
```

## Comparing `ufbt-0.2.1rc2.tar` & `ufbt-0.2.1rc3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:59:58.982588 ufbt-0.2.1rc2/
--rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-04-09 12:59:47.000000 ufbt-0.2.1rc2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-09 12:59:58.982588 ufbt-0.2.1rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-09 12:59:47.000000 ufbt-0.2.1rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-09 12:59:47.000000 ufbt-0.2.1rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 12:59:58.982588 ufbt-0.2.1rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:59:58.982588 ufbt-0.2.1rc2/ufbt/
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-09 12:59:47.000000 ufbt-0.2.1rc2/ufbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-09 12:59:47.000000 ufbt-0.2.1rc2/ufbt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25878 2023-04-09 12:59:47.000000 ufbt-0.2.1rc2/ufbt/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:59:58.982588 ufbt-0.2.1rc2/ufbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-09 12:59:58.000000 ufbt-0.2.1rc2/ufbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-09 12:59:58.000000 ufbt-0.2.1rc2/ufbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 12:59:58.000000 ufbt-0.2.1rc2/ufbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-09 12:59:58.000000 ufbt-0.2.1rc2/ufbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 12:59:58.000000 ufbt-0.2.1rc2/ufbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:57:43.555873 ufbt-0.2.1rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-04-09 14:57:32.000000 ufbt-0.2.1rc3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-09 14:57:43.555873 ufbt-0.2.1rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-09 14:57:32.000000 ufbt-0.2.1rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-09 14:57:32.000000 ufbt-0.2.1rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 14:57:43.555873 ufbt-0.2.1rc3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:57:43.555873 ufbt-0.2.1rc3/ufbt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-09 14:57:32.000000 ufbt-0.2.1rc3/ufbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-09 14:57:32.000000 ufbt-0.2.1rc3/ufbt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26207 2023-04-09 14:57:32.000000 ufbt-0.2.1rc3/ufbt/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:57:43.555873 ufbt-0.2.1rc3/ufbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-09 14:57:43.000000 ufbt-0.2.1rc3/ufbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-09 14:57:43.000000 ufbt-0.2.1rc3/ufbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:57:43.000000 ufbt-0.2.1rc3/ufbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-09 14:57:43.000000 ufbt-0.2.1rc3/ufbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-09 14:57:43.000000 ufbt-0.2.1rc3/ufbt.egg-info/top_level.txt
```

### Comparing `ufbt-0.2.1rc2/LICENSE.md` & `ufbt-0.2.1rc3/LICENSE.md`

 * *Files 2% similar despite different names*

```diff
@@ -613,63 +613,7 @@
 above cannot be given local legal effect according to their terms,
 reviewing courts shall apply local law that most closely approximates
 an absolute waiver of all civil liability in connection with the
 Program, unless a warranty or assumption of liability accompanies a
 copy of the Program in return for a fee.
 
 END OF TERMS AND CONDITIONS
-
-### How to Apply These Terms to Your New Programs
-
-If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these
-terms.
-
-To do so, attach the following notices to the program. It is safest to
-attach them to the start of each source file to most effectively state
-the exclusion of warranty; and each file should have at least the
-"copyright" line and a pointer to where the full notice is found.
-
-        <one line to give the program's name and a brief idea of what it does.>
-        Copyright (C) <year>  <name of author>
-
-        This program is free software: you can redistribute it and/or modify
-        it under the terms of the GNU General Public License as published by
-        the Free Software Foundation, either version 3 of the License, or
-        (at your option) any later version.
-
-        This program is distributed in the hope that it will be useful,
-        but WITHOUT ANY WARRANTY; without even the implied warranty of
-        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-        GNU General Public License for more details.
-
-        You should have received a copy of the GNU General Public License
-        along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper
-mail.
-
-If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-        <program>  Copyright (C) <year>  <name of author>
-        This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-        This is free software, and you are welcome to redistribute it
-        under certain conditions; type `show c' for details.
-
-The hypothetical commands \`show w' and \`show c' should show the
-appropriate parts of the General Public License. Of course, your
-program's commands might be different; for a GUI interface, you would
-use an "about box".
-
-You should also get your employer (if you work as a programmer) or
-school, if any, to sign a "copyright disclaimer" for the program, if
-necessary. For more information on this, and how to apply and follow
-the GNU GPL, see <https://www.gnu.org/licenses/>.
-
-The GNU General Public License does not permit incorporating your
-program into proprietary programs. If your program is a subroutine
-library, you may consider it more useful to permit linking proprietary
-applications with the library. If this is what you want to do, use the
-GNU Lesser General Public License instead of this License. But first,
-please read <https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `ufbt-0.2.1rc2/PKG-INFO` & `ufbt-0.2.1rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufbt
-Version: 0.2.1rc2
+Version: 0.2.1rc3
 Summary: uFBT - micro Flipper Build Tool. Tool for building and developing applications (.fap) for Flipper Zero and its device family.
 Author-email: "Flipper Devices Inc." <pypi@flipperdevices.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: documentation, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: repository, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: issues, https://github.com/flipperdevices/flipperzero-ufbt/issues
```

### Comparing `ufbt-0.2.1rc2/README.md` & `ufbt-0.2.1rc3/README.md`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.1rc2/pyproject.toml` & `ufbt-0.2.1rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.1rc2/ufbt/__init__.py` & `ufbt-0.2.1rc3/ufbt/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,23 +18,31 @@
 #
 
 import os
 import pathlib
 import platform
 import sys
 
-from .bootstrap import bootstrap_cli, bootstrap_subcommands, get_ufbt_package_version
+from .bootstrap import (
+    bootstrap_cli,
+    bootstrap_subcommands,
+    get_ufbt_package_version,
+    DEFAULT_UFBT_HOME,
+)
 
 __version__ = get_ufbt_package_version()
 
 
 def ufbt_cli():
-    if not os.environ.get("UFBT_STATE_DIR"):
-        os.environ["UFBT_STATE_DIR"] = os.path.expanduser("~/.ufbt")
+    if not os.environ.get("UFBT_HOME"):
+        os.environ["UFBT_HOME"] = DEFAULT_UFBT_HOME
+    # ufbt impl uses UFBT_STATE_DIR internally, not UFBT_HOME
+    os.environ["UFBT_STATE_DIR"] = os.environ["UFBT_HOME"]
     if not os.environ.get("FBT_TOOLCHAIN_PATH"):
+        # fbtenv.sh appends /toolchain/{PLATFORM} to FBT_TOOLCHAIN_PATH
         os.environ["FBT_TOOLCHAIN_PATH"] = os.environ["UFBT_STATE_DIR"]
 
     ufbt_state_dir = pathlib.Path(os.environ["UFBT_STATE_DIR"])
 
     # if any of bootstrap subcommands are in the arguments - call it instead
     # kept for compatibility with old scripts, better use `ufbt-bootstrap` directly
     if any(map(sys.argv.__contains__, bootstrap_subcommands)):
```

### Comparing `ufbt-0.2.1rc2/ufbt/__main__.py` & `ufbt-0.2.1rc3/ufbt/__main__.py`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.1rc2/ufbt/bootstrap.py` & `ufbt-0.2.1rc3/ufbt/bootstrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,23 +30,20 @@
 from pathlib import Path, PurePosixPath
 from typing import ClassVar, Dict, Optional
 from urllib.parse import unquote, urlparse
 from urllib.request import Request, urlopen
 from zipfile import ZipFile
 from importlib.metadata import version
 
-logging.basicConfig(
-    format="%(asctime)s.%(msecs)03d [%(levelname).1s] %(message)s",
-    level=logging.INFO,
-    datefmt="%H:%M:%S",
-)
-log = logging.getLogger(__name__)
 
 ##############################################################################
 
+log = logging.getLogger(__name__)
+DEFAULT_UFBT_HOME = os.path.expanduser("~/.ufbt")
+
 
 def get_ufbt_package_version():
     try:
         return version("ufbt")
     except Exception as e:
         log.debug(f"Failed to get ufbt version: {e}")
         return "unknown"
@@ -232,26 +229,26 @@
 
     class UpdateChannel(enum.Enum):
         DEV = "development"
         RC = "release-candidate"
         RELEASE = "release"
 
     def __init__(
-        self, download_dir: str, channel: UpdateChannel, index_html_url: str = None
+        self, download_dir: str, channel: UpdateChannel, json_index_url: str = None
     ):
         super().__init__(download_dir)
         self.channel = channel
-        self.index_html_url = index_html_url or self.OFFICIAL_INDEX_URL
+        self.json_index_url = json_index_url or self.OFFICIAL_INDEX_URL
         self.version_info = self._fetch_version(self.channel)
 
     def _fetch_version(self, channel: UpdateChannel) -> dict:
-        log.info(f"Fetching version info for {channel} from {self.index_html_url}")
+        log.info(f"Fetching version info for {channel} from {self.json_index_url}")
         try:
             data = json.loads(
-                self._open_url(self.index_html_url).read().decode("utf-8")
+                self._open_url(self.json_index_url).read().decode("utf-8")
             )
         except json.decoder.JSONDecodeError as e:
             raise ValueError(f"Invalid JSON: {e}")
 
         if not (channels := data.get("channels", [])):
             raise ValueError(f"Invalid channel: {channel}")
 
@@ -292,34 +289,34 @@
 
         return self._fetch_file(file_url)
 
     def get_metadata(self) -> Dict[str, str]:
         return {
             "mode": self.LOADER_MODE_KEY,
             "channel": self.channel.name.lower(),
-            "index_html": self.index_html_url,
+            "json_index": self.json_index_url,
             "version": self.version_info["version"],
         }
 
     @classmethod
     def metadata_to_init_kwargs(cls, metadata: dict) -> Dict[str, str]:
         return {
             "channel": UpdateChannelSdkLoader.UpdateChannel[
                 metadata["channel"].upper()
             ],
-            "index_html_url": metadata.get("index_html", None),
+            "json_index_url": metadata.get("json_index", None),
         }
 
     @classmethod
     def args_namespace_to_metadata(
         cls, namespace: argparse.Namespace
     ) -> Dict[str, str]:
         return {
             "channel": namespace.channel,
-            "index_html": namespace.index_url,
+            "json_index": namespace.index_url,
         }
 
     @classmethod
     def add_args_to_mode_group(cls, mode_group):
         mode_group.add_argument(
             "--channel",
             "-c",
@@ -499,14 +496,18 @@
 class UfbtSdkDeployer:
     UFBT_STATE_FILE_NAME = "ufbt_state.json"
 
     def __init__(self, ufbt_state_dir: str):
         self.ufbt_state_dir = Path(ufbt_state_dir)
         self.download_dir = self.ufbt_state_dir / "download"
         self.current_sdk_dir = self.ufbt_state_dir / "current"
+        self.toolchain_dir = (
+            Path(os.environ.get("FBT_TOOLCHAIN_PATH", self.ufbt_state_dir.absolute()))
+            / "toolchain"
+        )
         self.state_file = self.current_sdk_dir / self.UFBT_STATE_FILE_NAME
 
     def get_previous_task(self) -> Optional[SdkDeployTask]:
         if not os.path.exists(self.state_file):
             return None
         with open(self.state_file, "r") as f:
             ufbt_state = json.load(f)
@@ -657,14 +658,15 @@
 
 class StatusSubcommand(CliSubcommand):
     COMMAND = "status"
     STATUS_FIELDS = {
         "ufbt_version": "uFBT version",
         "state_dir": "State dir",
         "download_dir": "Download dir",
+        "toolchain_dir": "Toolchain dir",
         "sdk_dir": "SDK dir",
         "target": "Target",
         "mode": "Mode",
         "version": "Version",
         "details": "Details",
         "error": "Error",
     }
@@ -692,14 +694,15 @@
 
         sdk_deployer = UfbtSdkDeployer(args.ufbt_home)
         state_data = {
             "ufbt_version": ufbt_version,
             "state_dir": str(sdk_deployer.ufbt_state_dir.absolute()),
             "download_dir": str(sdk_deployer.download_dir.absolute()),
             "sdk_dir": str(sdk_deployer.current_sdk_dir.absolute()),
+            "toolchain_dir": str(sdk_deployer.toolchain_dir.absolute()),
         }
 
         if previous_task := sdk_deployer.get_previous_task():
             state_data.update(
                 {
                     "target": previous_task.hw_target,
                     "mode": previous_task.mode,
@@ -734,26 +737,32 @@
 
 bootstrap_subcommands = (
     subcommand_cls.COMMAND for subcommand_cls in bootstrap_subcommand_classes
 )
 
 
 def bootstrap_cli() -> Optional[int]:
+    logging.basicConfig(
+        format="%(asctime)s.%(msecs)03d [%(levelname).1s] %(message)s",
+        level=logging.INFO,
+        datefmt="%H:%M:%S",
+    )
+
     root_parser = argparse.ArgumentParser()
     root_parser.add_argument(
         "--no-check-certificate",
         help="Disable SSL certificate verification",
         action="store_true",
         default=False,
     )
     root_parser.add_argument(
         "--ufbt-home",
         "-d",
         help="uFBT state directory",
-        default=os.environ.get("UFBT_HOME", os.path.expanduser("~/.ufbt")),
+        default=os.environ.get("UFBT_HOME", DEFAULT_UFBT_HOME),
     )
     root_parser.add_argument(
         "--force",
         "-f",
         help="Force operation",
         action="store_true",
         default=False,
```

### Comparing `ufbt-0.2.1rc2/ufbt.egg-info/PKG-INFO` & `ufbt-0.2.1rc3/ufbt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufbt
-Version: 0.2.1rc2
+Version: 0.2.1rc3
 Summary: uFBT - micro Flipper Build Tool. Tool for building and developing applications (.fap) for Flipper Zero and its device family.
 Author-email: "Flipper Devices Inc." <pypi@flipperdevices.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: documentation, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: repository, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: issues, https://github.com/flipperdevices/flipperzero-ufbt/issues
```

