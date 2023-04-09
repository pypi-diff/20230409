# Comparing `tmp/buildarr-0.4.0.tar.gz` & `tmp/buildarr-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildarr-0.4.0.tar", max compression
+gzip compressed data, was "buildarr-0.4.1.tar", max compression
```

## Comparing `buildarr-0.4.0.tar` & `buildarr-0.4.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0    35149 2023-03-31 12:16:00.253111 buildarr-0.4.0/LICENSE
--rw-r--r--   0        0        0    14431 2023-03-31 12:16:00.257111 buildarr-0.4.0/README.md
--rw-r--r--   0        0        0      946 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/__init__.py
--rw-r--r--   0        0        0     1783 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/cli/__init__.py
--rw-r--r--   0        0        0    11234 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/cli/compose.py
--rw-r--r--   0        0        0    17167 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/cli/daemon.py
--rw-r--r--   0        0        0     2521 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/cli/exceptions.py
--rw-r--r--   0        0        0     1254 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/cli/main.py
--rw-r--r--   0        0        0    12498 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/cli/run.py
--rw-r--r--   0        0        0     8779 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/cli/test_config.py
--rw-r--r--   0        0        0     1310 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/config/__init__.py
--rw-r--r--   0        0        0    32740 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/config/base.py
--rw-r--r--   0        0        0     5429 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/config/buildarr.py
--rw-r--r--   0        0        0     1071 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/config/exceptions.py
--rw-r--r--   0        0        0     7213 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/config/load.py
--rw-r--r--   0        0        0     8853 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/config/models.py
--rw-r--r--   0        0        0     5338 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/config/resolve_instance_dependencies.py
--rw-r--r--   0        0        0     2164 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/config/types.py
--rw-r--r--   0        0        0      827 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/exceptions.py
--rw-r--r--   0        0        0     3046 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/logging.py
--rw-r--r--   0        0        0     6639 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/manager/__init__.py
--rw-r--r--   0        0        0      877 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/manager/exceptions.py
--rw-r--r--   0        0        0      872 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/plugins/dummy/__init__.py
--rw-r--r--   0        0        0     8838 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/plugins/dummy/api.py
--rw-r--r--   0        0        0     2922 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/plugins/dummy/cli.py
--rw-r--r--   0        0        0     7264 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/plugins/dummy/config/__init__.py
--rw-r--r--   0        0        0     7783 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/plugins/dummy/config/settings.py
--rw-r--r--   0        0        0     1184 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/plugins/dummy/config/types.py
--rw-r--r--   0        0        0     1178 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/plugins/dummy/exceptions.py
--rw-r--r--   0        0        0      932 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/plugins/dummy/manager.py
--rw-r--r--   0        0        0     1160 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/plugins/dummy/plugin.py
--rw-r--r--   0        0        0     3570 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/plugins/dummy/secrets.py
--rw-r--r--   0        0        0     5934 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/plugins/dummy/server.py
--rw-r--r--   0        0        0     1386 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/plugins/dummy/types.py
--rw-r--r--   0        0        0     2236 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/plugins/load.py
--rw-r--r--   0        0        0     3728 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/plugins/models.py
--rw-r--r--   0        0        0     1239 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/plugins/types.py
--rw-r--r--   0        0        0        0 2023-03-31 12:16:00.257111 buildarr-0.4.0/buildarr/py.typed
--rw-r--r--   0        0        0      925 2023-03-31 12:16:00.261111 buildarr-0.4.0/buildarr/secrets/__init__.py
--rw-r--r--   0        0        0     1889 2023-03-31 12:16:00.261111 buildarr-0.4.0/buildarr/secrets/base.py
--rw-r--r--   0        0        0     2466 2023-03-31 12:16:00.261111 buildarr-0.4.0/buildarr/secrets/load.py
--rw-r--r--   0        0        0     3723 2023-03-31 12:16:00.261111 buildarr-0.4.0/buildarr/secrets/models.py
--rw-r--r--   0        0        0     7065 2023-03-31 12:16:00.261111 buildarr-0.4.0/buildarr/state.py
--rw-r--r--   0        0        0     4734 2023-03-31 12:16:00.261111 buildarr-0.4.0/buildarr/trash.py
--rw-r--r--   0        0        0    12955 2023-03-31 12:16:00.261111 buildarr-0.4.0/buildarr/types.py
--rw-r--r--   0        0        0     4183 2023-03-31 12:16:00.261111 buildarr-0.4.0/buildarr/util.py
--rw-r--r--   0        0        0     2326 2023-03-31 12:16:00.261111 buildarr-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    15933 1970-01-01 00:00:00.000000 buildarr-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-09 00:59:49.037268 buildarr-0.4.1/LICENSE
+-rw-r--r--   0        0        0    14660 2023-04-09 00:59:49.037268 buildarr-0.4.1/README.md
+-rw-r--r--   0        0        0      946 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/__init__.py
+-rw-r--r--   0        0        0     1783 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/cli/__init__.py
+-rw-r--r--   0        0        0    11235 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/cli/compose.py
+-rw-r--r--   0        0        0    17974 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/cli/daemon.py
+-rw-r--r--   0        0        0     2521 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/cli/exceptions.py
+-rw-r--r--   0        0        0     1254 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/cli/main.py
+-rw-r--r--   0        0        0    12498 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/cli/run.py
+-rw-r--r--   0        0        0     8779 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/cli/test_config.py
+-rw-r--r--   0        0        0     1310 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/config/__init__.py
+-rw-r--r--   0        0        0    33589 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/config/base.py
+-rw-r--r--   0        0        0     5429 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/config/buildarr.py
+-rw-r--r--   0        0        0     1071 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/config/exceptions.py
+-rw-r--r--   0        0        0     7213 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/config/load.py
+-rw-r--r--   0        0        0     8853 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/config/models.py
+-rw-r--r--   0        0        0     5338 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/config/resolve_instance_dependencies.py
+-rw-r--r--   0        0        0     2164 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/config/types.py
+-rw-r--r--   0        0        0      827 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/exceptions.py
+-rw-r--r--   0        0        0     3046 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/logging.py
+-rw-r--r--   0        0        0     6639 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/manager/__init__.py
+-rw-r--r--   0        0        0      877 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/manager/exceptions.py
+-rw-r--r--   0        0        0      872 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/plugins/dummy/__init__.py
+-rw-r--r--   0        0        0     8838 2023-04-09 00:59:49.037268 buildarr-0.4.1/buildarr/plugins/dummy/api.py
+-rw-r--r--   0        0        0     2922 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/dummy/cli.py
+-rw-r--r--   0        0        0     7264 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/dummy/config/__init__.py
+-rw-r--r--   0        0        0     7783 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/dummy/config/settings.py
+-rw-r--r--   0        0        0     1184 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/dummy/config/types.py
+-rw-r--r--   0        0        0     1178 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/dummy/exceptions.py
+-rw-r--r--   0        0        0      932 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/dummy/manager.py
+-rw-r--r--   0        0        0     1160 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/dummy/plugin.py
+-rw-r--r--   0        0        0     3570 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/dummy/secrets.py
+-rw-r--r--   0        0        0     5934 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/dummy/server.py
+-rw-r--r--   0        0        0     1386 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/dummy/types.py
+-rw-r--r--   0        0        0     2236 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/load.py
+-rw-r--r--   0        0        0     3728 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/models.py
+-rw-r--r--   0        0        0     1239 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/plugins/types.py
+-rw-r--r--   0        0        0        0 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/py.typed
+-rw-r--r--   0        0        0      925 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/secrets/__init__.py
+-rw-r--r--   0        0        0     1889 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/secrets/base.py
+-rw-r--r--   0        0        0     2466 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/secrets/load.py
+-rw-r--r--   0        0        0     3723 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/secrets/models.py
+-rw-r--r--   0        0        0     7065 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/state.py
+-rw-r--r--   0        0        0     4734 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/trash.py
+-rw-r--r--   0        0        0    12955 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/types.py
+-rw-r--r--   0        0        0     4183 2023-04-09 00:59:49.041268 buildarr-0.4.1/buildarr/util.py
+-rw-r--r--   0        0        0     2326 2023-04-09 00:59:49.041268 buildarr-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    16162 1970-01-01 00:00:00.000000 buildarr-0.4.1/PKG-INFO
```

### Comparing `buildarr-0.4.0/LICENSE` & `buildarr-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/README.md` & `buildarr-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 * [Recyclarr](https://github.com/recyclarr/recyclarr) - Automatically syncs recommended TRaSH-Guides settings to Sonarr/Radarr instances
     * Buildarr has support for this built-in, and in the case of Sonarr release profiles, supports the same filtering syntax.
 
 ## Installation
 
 Buildarr is available on Docker Hub as a Docker image.
 
-A plugin for Sonarr is bundled into the official Docker container for Buildarr, so you can manage Sonarr instances right away.
+Plugins for Sonarr and Prowlarr are bundled into the official Docker container for Buildarr, so you can manage instances of those types right away.
 
 ```bash
 $ docker pull callum027/buildarr:latest
 ```
 
 Buildarr can also be installed using `pip`. Python 3.8 or later is required. Windows is natively supported.
 
@@ -52,14 +52,15 @@
 ## Plugins
 
 Buildarr supports external plugins to allow additional applications to be supported.
 
 At the time of this release the following plugins are available:
 
 * [`buildarr-sonarr`](https://buildarr.github.io/plugins/sonarr) - [Sonarr](https://sonarr.tv) PVR for TV shows
+* [`buildarr-prowlarr`](https://buildarr.github.io/plugins/prowlarr) - [Prowlarr](https://prowlarr.com) indexer manager for Arr applications
 
 For more information on installing plugins, check the [plugin documentation](http://buildarr.github.io/plugins).
 
 ## Configuration
 
 Buildarr uses YAML as its configuration file format. By default, Buildarr looks for `buildarr.yml` in the current directory.
 
@@ -179,17 +180,16 @@
 * Add a dry-run mode for testing configurations (added in [version 0.4.0](https://buildarr.github.io/release-notes/#v040-2023-03-31))
 * Test updates for all available attributes in the existing Sonarr plugin
 * Unit tests and code coverage
 * Split Sonarr plugin to its own repository (completed in [version 0.4.0](https://buildarr.github.io/release-notes/#v040-2023-03-31))
 * Create plugins for the following applications:
     * Sonarr V4
     * Radarr
-    * Prowlarr
+    * Prowlarr (now available as [`buildarr-prowlarr`](https://buildarr.github.io/plugins/prowlarr))
     * Bazarr
-    * FlareSolverr
     * Unmanic
     * Tdarr (maybe)
     * Unpackerr
     * Lidarr
 * Instance linking (e.g. Prowlarr-to-Sonarr/Radarr) and dependency resolution (added in [version 0.3.0](https://buildarr.github.io/release-notes/#v030-2023-03-15))
 * Stable plugin API between major versions
 * Auto-generation of Docker Compose environment files reflecting the Buildarr configuration (added in [version 0.4.0](https://buildarr.github.io/release-notes/#v040-2023-03-31))
```

### Comparing `buildarr-0.4.0/buildarr/__init__.py` & `buildarr-0.4.1/buildarr/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/cli/__init__.py` & `buildarr-0.4.1/buildarr/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/cli/compose.py` & `buildarr-0.4.1/buildarr/cli/compose.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
                     "Expected hostname, got IP address",
                 )
             except ValueError:
                 pass
             if hostname == "localhost":
                 raise ComposeInvalidHostnameError(
                     f"Invalid hostname '{hostname}' for {plugin_name} instance '{instance_name}': "
-                    "Hostname must not be localhost for Docker Compose servies",
+                    "Hostname must not be localhost for Docker Compose services",
                 )
             if hostname in hostnames:
                 raise ComposeInvalidHostnameError(
                     f"Invalid hostname '{hostname}' for {plugin_name} instance '{instance_name}': "
                     f"Hostname already used by service '{hostnames[hostname]}'",
                 )
             hostnames[hostname] = service_name
```

### Comparing `buildarr-0.4.0/buildarr/cli/daemon.py` & `buildarr-0.4.1/buildarr/cli/daemon.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from time import sleep
 from typing import TYPE_CHECKING, cast
 
 import click
 
 from schedule import Job as SchedulerJob, Scheduler  # type: ignore[import]
 from watchdog.events import FileSystemEventHandler
-from watchdog.observers import Observer
+from watchdog.observers.polling import PollingObserver
 
 from .. import __version__
 from ..config import load_config
 from ..logging import get_log_level
 from ..state import state
 from ..types import DayOfWeek
 from ..util import get_absolute_path
@@ -87,15 +87,15 @@
         self._default_watch_config = watch_config
         self._default_update_days = set(update_days)
         self._default_update_times = set(update_times)
         # Load the Buildarr configuration from the given file, and set appropriate values
         # for Buildarr daemon configuration fields.
         self._load_config()
         # Create the config file observer and update job scheduler objects.
-        self.observer = Observer()
+        self.observer = self._create_observer()
         self.scheduler = Scheduler()
         # Internal variables for tracking daemon state.
         self._stopped = False
 
     def _load_config(self) -> None:
         """
         Load the Buildarr configuration from the given file, and set daemon configuration fields.
@@ -130,14 +130,25 @@
             (update_day, update_time)
             for update_day, update_time in itertools.product(
                 sorted(self.update_days),
                 sorted(self.update_times),
             )
         ]
 
+    def _create_observer(self) -> PollingObserver:
+        """
+        Create an empty `Observer` object for monitoring for file changes.
+
+        Handlers will need to be added to start listening for changes.
+
+        Returns:
+            Empty filesystem observer object
+        """
+        return PollingObserver()
+
     def start(self) -> None:
         """
         Start the Buildarr daemon main loop.
         """
         # Run the initial run routine.
         self.initial_run()
         # Setup SIGINT, SIGTERM, and SIGHUP signal handers.
@@ -207,17 +218,15 @@
         )
         # If configuration watching is enabled, setup event handlers
         # for when the active configuration files are modified.
         # When they are modified, the configuration is reloaded
         # and another initial run is performed.
         if self.watch_config:
             logger.info("Setting up config file monitoring")
-            # TODO: Remove ignore when the following issue is fixed.
-            # https://github.com/gorakhargosh/watchdog/issues/982
-            self.observer = Observer()  # type: ignore[assignment]
+            self.observer = self._create_observer()
             config_dirs: Dict[Path, Set[str]] = {}
             for config_file in state.config_files:
                 if config_file.parent not in config_dirs:
                     config_dirs[config_file.parent] = set()
                 config_dirs[config_file.parent].add(config_file.name)
             for config_dir, filenames in config_dirs.items():
                 logger.debug(
@@ -255,14 +264,15 @@
         This method is called by the config file monitor and SIGHUP handler.
         """
         logger.info("Reloading config")
         self._stop_handlers()
         self._load_config()
         self.initial_run()
         logger.info("Finished reloading config")
+        logger.info("Buildarr ready.")
 
     def stop(self) -> None:
         """
         Signal the daemon to stop, and shutdown job schedulers and monitors.
 
         This method is called by the SIGINT and SIGHNUP handlers.
         """
@@ -314,14 +324,28 @@
             filenames (Set[str]): Names of config files to monitor
         """
         self.daemon = daemon
         self.config_dir = config_dir
         self.filenames = filenames
         super().__init__()
 
+    def on_created(self, event: Union[DirModifiedEvent, FileModifiedEvent]) -> None:
+        """
+        On recreation of a config file within the monitored directory,
+        reload the Buildarr daemon.
+
+        Args:
+            event (Union[DirModifiedEvent, FileModifiedEvent]): Event metadata
+        """
+        if not event.is_directory and Path(event.src_path) in (
+            (self.config_dir / filename) for filename in self.filenames
+        ):
+            logger.info("Config file '%s' has been recreated", event.src_path)
+            self.daemon.reload()
+
     def on_modified(self, event: Union[DirModifiedEvent, FileModifiedEvent]) -> None:
         """
         On modification of a config file within the monitored directory,
         reload the Buildarr daemon.
 
         Args:
             event (Union[DirModifiedEvent, FileModifiedEvent]): Event metadata
@@ -354,15 +378,15 @@
     """
 
     times: List[time] = []
     for time_str in time_strs:
         try:
             times.append(datetime.strptime(time_str, "%H:%M").time())
         except ValueError:
-            raise click.BadParameter(f"Invalid 24 hour time '{time_str}") from None
+            raise click.BadParameter(f"Invalid 24 hour time '{time_str}'") from None
     return tuple(times)
 
 
 @cli.command(
     help=(
         "Run as a daemon and periodically update defined instances.\n\n"
         "If CONFIG-PATH is not defined, use `buildarr.yml' from the current directory."
```

### Comparing `buildarr-0.4.0/buildarr/cli/exceptions.py` & `buildarr-0.4.1/buildarr/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/cli/main.py` & `buildarr-0.4.1/buildarr/cli/main.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/cli/run.py` & `buildarr-0.4.1/buildarr/cli/run.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/cli/test_config.py` & `buildarr-0.4.1/buildarr/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/config/__init__.py` & `buildarr-0.4.1/buildarr/config/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/config/base.py` & `buildarr-0.4.1/buildarr/config/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from typing import (
     Any,
     Callable,
     Dict,
     Generic,
     Iterable,
     Mapping,
+    Optional,
     Set,
     Tuple,
     Type,
     Union,
     get_args as get_type_args,
     get_origin as get_type_origin,
 )
@@ -208,15 +209,15 @@
                                 # otherwise raise an error.
                                 if "field_default" in attr_metadata:
                                     local_attrs[attr_name] = attr_metadata["field_default"]
                                     field_default_set = True
                                 else:
                                     raise ValueError(
                                         "'value' attribute not included "
-                                        f"for remote field '{remote_attr_name}'"
+                                        f"for remote field '{remote_attr_name}' "
                                         "and 'field_default' not defined in local attribute",
                                     ) from None
                             break
                     else:
                         if attr_metadata.get("optional", False):
                             local_attrs[attr_name] = cls.__fields__[attr_name].default
                             continue
@@ -508,14 +509,18 @@
                 if changed:
                     self._api_put(secrets, remote_attrs)
                 return changed
         ```
 
         Supported `RemoteMapEntry` optional parameters:
 
+        * `equals` (`Callable[[Any, Any], bool], default: (use `a == b`))
+            * Callable function for comparing the local and remote values,
+              and return if they are equal or not, with `True` being returned
+              if they are equal, and `False` if not
         * `encoder` (`Callable[[Any], Any]`, default: (use internal function))
             * Callable function for parsing the local value to its remote equivalent
         * `root_encoder` (`Callable[[Self], Any]`, default: (undefined))
             * Similar to `encoder`, but `self` is passed instead of just the value
               being parsed, to give access to the full local configuration context
         * `formatter` (`Callable[[Any], str]`, default: (use internal function))
             * Function to convert the local value to a string, used in logging
@@ -546,14 +551,17 @@
         remote_attrs: Dict[str, Any] = {}
         already_logged: Set[str] = set()
         for attr_name, remote_attr_name, attr_metadata in remote_map:
             #
             set_value = False
 
             #
+            def equals(a: Any, b: Any) -> bool:
+                return a == b
+
             def formatter(v: Any) -> str:
                 return repr(attr_metadata.get("formatter", self._format_attr)(v))
 
             #
             remote_value = getattr(remote, attr_name)
             # Handle the case where the attribute is managed, either
             # by virtue of it being explicitly set in the Buildarr config,
@@ -561,15 +569,15 @@
             if (
                 attr_metadata.get("check_unmanaged", check_unmanaged)
                 or attr_name in self.__fields_set__
             ):
                 local_value = getattr(self, attr_name)
                 # If the local and remote attributes are set to the same
                 # value, unless set_unchanged is set to True, do nothing.
-                if local_value == remote_value:
+                if attr_metadata.get("equals", equals)(local_value, remote_value):
                     if attr_name not in already_logged:
                         logger.debug(
                             "%s.%s: %s (up to date)",
                             tree,
                             attr_name,
                             formatter(remote_value),
                         )
@@ -708,25 +716,38 @@
             return value.get_secret_value()
         elif isinstance(value, UUID):
             return str(value)
         elif isinstance(value, (list, set)):
             return [cls._encode_attr(v) for v in value]
         return value
 
-    def yaml(self, *args, **kwargs) -> str:
+    def yaml(
+        self,
+        *args,
+        sort_keys: bool = False,
+        yaml_kwargs: Optional[Mapping[str, Any]] = None,
+        **kwargs,
+    ) -> str:
         """
         Generate a YAML representation of the model.
 
         Internally this uses the Pydantic JSON generation function, with all arguments
         forwarded to `BaseModel.json()`. The JSON output is then re-processed using PyYAML.
 
+        Args:
+            sort_keys (bool, optional): Sort keys in the output YAML file. Defaults to `False`.
+            yaml_kwargs (Optional[Mapping[str, Any]], optional): YAML encoder keyword args.
+
         Returns:
             YAML representation of the model
         """
-        return yaml.safe_dump(json.loads(self.json(*args, **kwargs)))
+        return yaml.safe_dump(  # type: ignore[call-overload]
+            json.loads(self.json(*args, **kwargs)),
+            **{**(yaml_kwargs or {}), "sort_keys": sort_keys},
+        )
 
     class Config:
         """
         Buildarr base Pydantic model configuration.
 
         Sets some required configuration parameters for
         serialisation and parsing to work correctly.
```

### Comparing `buildarr-0.4.0/buildarr/config/buildarr.py` & `buildarr-0.4.1/buildarr/config/buildarr.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/config/exceptions.py` & `buildarr-0.4.1/buildarr/config/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/config/load.py` & `buildarr-0.4.1/buildarr/config/load.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/config/models.py` & `buildarr-0.4.1/buildarr/config/models.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/config/resolve_instance_dependencies.py` & `buildarr-0.4.1/buildarr/config/resolve_instance_dependencies.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/config/types.py` & `buildarr-0.4.1/buildarr/config/types.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/exceptions.py` & `buildarr-0.4.1/buildarr/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/logging.py` & `buildarr-0.4.1/buildarr/logging.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/manager/__init__.py` & `buildarr-0.4.1/buildarr/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/manager/exceptions.py` & `buildarr-0.4.1/buildarr/manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/plugins/__init__.py` & `buildarr-0.4.1/buildarr/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/plugins/dummy/api.py` & `buildarr-0.4.1/buildarr/plugins/dummy/api.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/plugins/dummy/cli.py` & `buildarr-0.4.1/buildarr/plugins/dummy/cli.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/plugins/dummy/config/__init__.py` & `buildarr-0.4.1/buildarr/plugins/dummy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/plugins/dummy/config/settings.py` & `buildarr-0.4.1/buildarr/plugins/dummy/config/settings.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/plugins/dummy/config/types.py` & `buildarr-0.4.1/buildarr/plugins/dummy/config/types.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/plugins/dummy/exceptions.py` & `buildarr-0.4.1/buildarr/plugins/dummy/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/plugins/dummy/manager.py` & `buildarr-0.4.1/buildarr/plugins/dummy/manager.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/plugins/dummy/plugin.py` & `buildarr-0.4.1/buildarr/plugins/dummy/plugin.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/plugins/dummy/secrets.py` & `buildarr-0.4.1/buildarr/plugins/dummy/secrets.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/plugins/dummy/server.py` & `buildarr-0.4.1/buildarr/plugins/dummy/server.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/plugins/dummy/types.py` & `buildarr-0.4.1/buildarr/plugins/dummy/types.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/plugins/load.py` & `buildarr-0.4.1/buildarr/plugins/load.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/plugins/models.py` & `buildarr-0.4.1/buildarr/plugins/models.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/plugins/types.py` & `buildarr-0.4.1/buildarr/plugins/types.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/secrets/__init__.py` & `buildarr-0.4.1/buildarr/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/secrets/base.py` & `buildarr-0.4.1/buildarr/secrets/base.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/secrets/load.py` & `buildarr-0.4.1/buildarr/secrets/load.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/secrets/models.py` & `buildarr-0.4.1/buildarr/secrets/models.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/state.py` & `buildarr-0.4.1/buildarr/state.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/trash.py` & `buildarr-0.4.1/buildarr/trash.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/types.py` & `buildarr-0.4.1/buildarr/types.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/buildarr/util.py` & `buildarr-0.4.1/buildarr/util.py`

 * *Files identical despite different names*

### Comparing `buildarr-0.4.0/pyproject.toml` & `buildarr-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.3.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "buildarr"
-version = "0.4.0"
+version = "0.4.1"
 description = "Constructs and configures Arr PVR stacks"
 authors = ["Callum Dickinson <callum.dickinson.nz@gmail.com>"]
 license = "GPL-3.0-or-later"
 homepage = "https://buildarr.github.io"
 repository = "https://github.com/buildarr/buildarr"
 documentation = "https://buildarr.github.io"
 keywords = ["buildarr", "sonarr", "radarr", "prowlarr"]
```

### Comparing `buildarr-0.4.0/PKG-INFO` & `buildarr-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildarr
-Version: 0.4.0
+Version: 0.4.1
 Summary: Constructs and configures Arr PVR stacks
 Home-page: https://buildarr.github.io
 License: GPL-3.0-or-later
 Keywords: buildarr,sonarr,radarr,prowlarr
 Author: Callum Dickinson
 Author-email: callum.dickinson.nz@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -63,15 +63,15 @@
 * [Recyclarr](https://github.com/recyclarr/recyclarr) - Automatically syncs recommended TRaSH-Guides settings to Sonarr/Radarr instances
     * Buildarr has support for this built-in, and in the case of Sonarr release profiles, supports the same filtering syntax.
 
 ## Installation
 
 Buildarr is available on Docker Hub as a Docker image.
 
-A plugin for Sonarr is bundled into the official Docker container for Buildarr, so you can manage Sonarr instances right away.
+Plugins for Sonarr and Prowlarr are bundled into the official Docker container for Buildarr, so you can manage instances of those types right away.
 
 ```bash
 $ docker pull callum027/buildarr:latest
 ```
 
 Buildarr can also be installed using `pip`. Python 3.8 or later is required. Windows is natively supported.
 
@@ -90,14 +90,15 @@
 ## Plugins
 
 Buildarr supports external plugins to allow additional applications to be supported.
 
 At the time of this release the following plugins are available:
 
 * [`buildarr-sonarr`](https://buildarr.github.io/plugins/sonarr) - [Sonarr](https://sonarr.tv) PVR for TV shows
+* [`buildarr-prowlarr`](https://buildarr.github.io/plugins/prowlarr) - [Prowlarr](https://prowlarr.com) indexer manager for Arr applications
 
 For more information on installing plugins, check the [plugin documentation](http://buildarr.github.io/plugins).
 
 ## Configuration
 
 Buildarr uses YAML as its configuration file format. By default, Buildarr looks for `buildarr.yml` in the current directory.
 
@@ -217,17 +218,16 @@
 * Add a dry-run mode for testing configurations (added in [version 0.4.0](https://buildarr.github.io/release-notes/#v040-2023-03-31))
 * Test updates for all available attributes in the existing Sonarr plugin
 * Unit tests and code coverage
 * Split Sonarr plugin to its own repository (completed in [version 0.4.0](https://buildarr.github.io/release-notes/#v040-2023-03-31))
 * Create plugins for the following applications:
     * Sonarr V4
     * Radarr
-    * Prowlarr
+    * Prowlarr (now available as [`buildarr-prowlarr`](https://buildarr.github.io/plugins/prowlarr))
     * Bazarr
-    * FlareSolverr
     * Unmanic
     * Tdarr (maybe)
     * Unpackerr
     * Lidarr
 * Instance linking (e.g. Prowlarr-to-Sonarr/Radarr) and dependency resolution (added in [version 0.3.0](https://buildarr.github.io/release-notes/#v030-2023-03-15))
 * Stable plugin API between major versions
 * Auto-generation of Docker Compose environment files reflecting the Buildarr configuration (added in [version 0.4.0](https://buildarr.github.io/release-notes/#v040-2023-03-31))
```

