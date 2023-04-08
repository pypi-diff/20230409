# Comparing `tmp/ufbt-0.2.1rc0.tar.gz` & `tmp/ufbt-0.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ufbt-0.2.1rc0.tar", last modified: Sat Apr  8 20:13:55 2023, max compression
+gzip compressed data, was "ufbt-0.2.1rc1.tar", last modified: Sat Apr  8 22:53:28 2023, max compression
```

## Comparing `ufbt-0.2.1rc0.tar` & `ufbt-0.2.1rc1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:13:55.665080 ufbt-0.2.1rc0/
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-08 20:13:55.665080 ufbt-0.2.1rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-08 20:13:40.000000 ufbt-0.2.1rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-08 20:13:40.000000 ufbt-0.2.1rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 20:13:55.665080 ufbt-0.2.1rc0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:13:55.665080 ufbt-0.2.1rc0/ufbt/
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-08 20:13:40.000000 ufbt-0.2.1rc0/ufbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-08 20:13:40.000000 ufbt-0.2.1rc0/ufbt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25056 2023-04-08 20:13:40.000000 ufbt-0.2.1rc0/ufbt/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:13:55.665080 ufbt-0.2.1rc0/ufbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-08 20:13:55.000000 ufbt-0.2.1rc0/ufbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-08 20:13:55.000000 ufbt-0.2.1rc0/ufbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 20:13:55.000000 ufbt-0.2.1rc0/ufbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-08 20:13:55.000000 ufbt-0.2.1rc0/ufbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-08 20:13:55.000000 ufbt-0.2.1rc0/ufbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:53:28.441876 ufbt-0.2.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-08 22:53:28.441876 ufbt-0.2.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-08 22:53:15.000000 ufbt-0.2.1rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-08 22:53:15.000000 ufbt-0.2.1rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 22:53:28.441876 ufbt-0.2.1rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:53:28.441876 ufbt-0.2.1rc1/ufbt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-08 22:53:15.000000 ufbt-0.2.1rc1/ufbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-08 22:53:15.000000 ufbt-0.2.1rc1/ufbt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25093 2023-04-08 22:53:15.000000 ufbt-0.2.1rc1/ufbt/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 22:53:28.441876 ufbt-0.2.1rc1/ufbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-08 22:53:28.000000 ufbt-0.2.1rc1/ufbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-08 22:53:28.000000 ufbt-0.2.1rc1/ufbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 22:53:28.000000 ufbt-0.2.1rc1/ufbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-08 22:53:28.000000 ufbt-0.2.1rc1/ufbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-08 22:53:28.000000 ufbt-0.2.1rc1/ufbt.egg-info/top_level.txt
```

### Comparing `ufbt-0.2.1rc0/PKG-INFO` & `ufbt-0.2.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufbt
-Version: 0.2.1rc0
+Version: 0.2.1rc1
 Summary: uFBT - micro Flipper Build Tool. Tool for building and developing applications (.fap) for Flipper Zero and its device family.
 Author-email: "Flipper Devices Inc." <pypi@flipperdevices.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: documentation, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: repository, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: issues, https://github.com/flipperdevices/flipperzero-ufbt/issues
```

### Comparing `ufbt-0.2.1rc0/README.md` & `ufbt-0.2.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.1rc0/pyproject.toml` & `ufbt-0.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.1rc0/ufbt/__init__.py` & `ufbt-0.2.1rc1/ufbt/__init__.py`

 * *Files identical despite different names*

### Comparing `ufbt-0.2.1rc0/ufbt/bootstrap.py` & `ufbt-0.2.1rc1/ufbt/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -638,46 +638,46 @@
             shutil.rmtree(sdk_deployer.current_sdk_dir, ignore_errors=True)
         log.info("Done")
         return 0
 
 
 class StatusSubcommand(CliSubcommand):
     COMMAND = "status"
+    STATUS_FIELDS = {
+        "ufbt_version": "uFBT version",
+        "state_dir": "State dir",
+        "download_dir": "Download dir",
+        "sdk_dir": "SDK dir",
+        "target": "Target",
+        "mode": "Mode",
+        "version": "Version",
+        "details": "Details",
+        "error": "Error",
+    }
 
     def __init__(self):
         super().__init__(self.COMMAND, "Show uFBT SDK status")
 
     def _add_arguments(self, parser: argparse.ArgumentParser) -> None:
         parser.add_argument(
             "--json",
             help="Print status in JSON format",
             action="store_true",
             default=False,
         )
 
         parser.add_argument(
             "status_key",
-            help="Print only specific status key",
+            help="Print only a single value for a specific status key",
             nargs="?",
+            choices=self.STATUS_FIELDS.keys(),
         )
 
     def _func(self, args) -> int:
-        fields = {
-            "ufbt_version": "uFBT version",
-            "state_dir": "State dir",
-            "download_dir": "Download dir",
-            "sdk_dir": "SDK dir",
-            "target": "Target",
-            "mode": "Mode",
-            "version": "Version",
-            "details": "Details",
-            "error": "Error",
-        }
-
-        ufbt_version = self.get_ufbt_package_version()
+        ufbt_version = get_ufbt_package_version()
 
         sdk_deployer = UfbtSdkDeployer(args.ufbt_home)
         state_data = {
             "ufbt_version": ufbt_version,
             "state_dir": str(sdk_deployer.ufbt_state_dir.absolute()),
             "download_dir": str(sdk_deployer.download_dir.absolute()),
             "sdk_dir": str(sdk_deployer.current_sdk_dir.absolute()),
@@ -706,15 +706,15 @@
             else:
                 print(state_data.get(key, ""))
         else:
             if args.json:
                 print(json.dumps(state_data, indent=4))
             else:
                 for key, value in state_data.items():
-                    log.info(f"{fields[key]:<15} {value}")
+                    log.info(f"{self.STATUS_FIELDS[key]:<15} {value}")
 
         return 1 if state_data.get("error") else 0
 
 
 bootstrap_subcommand_classes = (UpdateSubcommand, CleanSubcommand, StatusSubcommand)
 
 bootstrap_subcommands = (
```

### Comparing `ufbt-0.2.1rc0/ufbt.egg-info/PKG-INFO` & `ufbt-0.2.1rc1/ufbt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufbt
-Version: 0.2.1rc0
+Version: 0.2.1rc1
 Summary: uFBT - micro Flipper Build Tool. Tool for building and developing applications (.fap) for Flipper Zero and its device family.
 Author-email: "Flipper Devices Inc." <pypi@flipperdevices.com>
 License: GPL-3.0
 Project-URL: homepage, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: documentation, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: repository, https://github.com/flipperdevices/flipperzero-ufbt
 Project-URL: issues, https://github.com/flipperdevices/flipperzero-ufbt/issues
```

