# Comparing `tmp/diagralhomekit-0.9.4.tar.gz` & `tmp/diagralhomekit-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diagralhomekit-0.9.4.tar", max compression
+gzip compressed data, was "diagralhomekit-0.9.5.tar", max compression
```

## Comparing `diagralhomekit-0.9.4.tar` & `diagralhomekit-0.9.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    21393 2023-04-03 19:32:16.506454 diagralhomekit-0.9.4/LICENSE
--rw-r--r--   0        0        0     3336 2023-04-06 16:01:35.043604 diagralhomekit-0.9.4/README.md
--rw-r--r--   0        0        0      455 2023-04-05 18:45:00.080586 diagralhomekit-0.9.4/diagralhomekit/__init__.py
--rw-r--r--   0        0        0      584 2023-04-06 08:43:32.341564 diagralhomekit-0.9.4/diagralhomekit/__main__.py
--rw-r--r--   0        0        0     2352 2023-04-06 12:46:44.557883 diagralhomekit-0.9.4/diagralhomekit/alarm_system.py
--rw-r--r--   0        0        0     2456 2023-04-06 15:42:16.478616 diagralhomekit-0.9.4/diagralhomekit/config.py
--rw-r--r--   0        0        0    26793 2023-04-06 16:34:03.553032 diagralhomekit-0.9.4/diagralhomekit/diagral.py
--rw-r--r--   0        0        0     6674 2023-04-06 12:23:10.592110 diagralhomekit-0.9.4/diagralhomekit/homekit_alarm.py
--rw-r--r--   0        0        0     4243 2023-04-06 14:01:59.443690 diagralhomekit-0.9.4/diagralhomekit/http_plugin.py
--rw-r--r--   0        0        0     4530 2023-04-06 16:35:35.719387 diagralhomekit-0.9.4/diagralhomekit/main.py
--rw-r--r--   0        0        0     7518 2023-04-06 15:59:40.754133 diagralhomekit-0.9.4/diagralhomekit/meteofrance.py
--rw-r--r--   0        0        0     4452 2023-04-06 15:48:02.383331 diagralhomekit-0.9.4/diagralhomekit/nut.py
--rw-r--r--   0        0        0     8497 2023-04-06 13:39:39.849006 diagralhomekit-0.9.4/diagralhomekit/plex.py
--rw-r--r--   0        0        0     1044 2023-04-06 13:50:15.159321 diagralhomekit-0.9.4/diagralhomekit/plugin.py
--rw-r--r--   0        0        0     2524 2023-04-06 13:38:00.533738 diagralhomekit-0.9.4/diagralhomekit/utils.py
--rw-r--r--   0        0        0      586 2023-04-06 16:36:40.140629 diagralhomekit-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     4423 1970-01-01 00:00:00.000000 diagralhomekit-0.9.4/setup.py
--rw-r--r--   0        0        0     4215 1970-01-01 00:00:00.000000 diagralhomekit-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0    21393 2023-04-03 19:32:16.506454 diagralhomekit-0.9.5/LICENSE
+-rw-r--r--   0        0        0     3336 2023-04-06 16:01:35.043604 diagralhomekit-0.9.5/README.md
+-rw-r--r--   0        0        0      455 2023-04-05 18:45:00.080586 diagralhomekit-0.9.5/diagralhomekit/__init__.py
+-rw-r--r--   0        0        0      584 2023-04-06 08:43:32.341564 diagralhomekit-0.9.5/diagralhomekit/__main__.py
+-rw-r--r--   0        0        0     2352 2023-04-06 12:46:44.557883 diagralhomekit-0.9.5/diagralhomekit/alarm_system.py
+-rw-r--r--   0        0        0     2453 2023-04-09 07:56:45.202374 diagralhomekit-0.9.5/diagralhomekit/config.py
+-rw-r--r--   0        0        0    27456 2023-04-09 08:03:25.957046 diagralhomekit-0.9.5/diagralhomekit/diagral.py
+-rw-r--r--   0        0        0     7313 2023-04-09 08:08:56.032072 diagralhomekit-0.9.5/diagralhomekit/homekit_alarm.py
+-rw-r--r--   0        0        0     4243 2023-04-06 14:01:59.443690 diagralhomekit-0.9.5/diagralhomekit/http_plugin.py
+-rw-r--r--   0        0        0     4508 2023-04-09 07:59:07.847736 diagralhomekit-0.9.5/diagralhomekit/main.py
+-rw-r--r--   0        0        0     7518 2023-04-06 15:59:40.754133 diagralhomekit-0.9.5/diagralhomekit/meteofrance.py
+-rw-r--r--   0        0        0     4452 2023-04-06 15:48:02.383331 diagralhomekit-0.9.5/diagralhomekit/nut.py
+-rw-r--r--   0        0        0     8497 2023-04-06 13:39:39.849006 diagralhomekit-0.9.5/diagralhomekit/plex.py
+-rw-r--r--   0        0        0     1044 2023-04-06 13:50:15.159321 diagralhomekit-0.9.5/diagralhomekit/plugin.py
+-rw-r--r--   0        0        0     2524 2023-04-06 13:38:00.533738 diagralhomekit-0.9.5/diagralhomekit/utils.py
+-rw-r--r--   0        0        0      586 2023-04-09 07:39:47.620151 diagralhomekit-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     4423 1970-01-01 00:00:00.000000 diagralhomekit-0.9.5/setup.py
+-rw-r--r--   0        0        0     4215 1970-01-01 00:00:00.000000 diagralhomekit-0.9.5/PKG-INFO
```

### Comparing `diagralhomekit-0.9.4/LICENSE` & `diagralhomekit-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.4/README.md` & `diagralhomekit-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.4/diagralhomekit/__main__.py` & `diagralhomekit-0.9.5/diagralhomekit/__main__.py`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.4/diagralhomekit/alarm_system.py` & `diagralhomekit-0.9.5/diagralhomekit/alarm_system.py`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.4/diagralhomekit/config.py` & `diagralhomekit-0.9.5/diagralhomekit/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     max_request_tries = 3
 
     def __init__(self):
         """init function."""
         from diagralhomekit.diagral import DiagralHomekitPlugin
 
-        self.log_requests = False
+        self.verbosity = False
         self.plugins = [
             DiagralHomekitPlugin(self),
             PlexHomekitPlugin(self),
             HttpMonitoringPlugin(self),
             MeteoFrancePlugin(self),
             UPSMonitoringPlugin(self),
         ]
```

### Comparing `diagralhomekit-0.9.4/diagralhomekit/diagral.py` & `diagralhomekit-0.9.5/diagralhomekit/diagral.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             self.ttm_session_id = content["ttmSessionId"]
             self.set_active_groups(set(content["groups"]))
             return self.ttm_session_id
         message = content["message"]
         if message == "transmitter.connection.badpincode":
             raise ValueError("MasterCode invalid; please verify your configuration.")
         elif message == "transmitter.connection.overlimit":
-            self.account.sleep_while_run(180)
+            self.account.sleep_while_run(180, log=True)
             return self.create_new_session(count=count + 1)
         elif message == "transmitter.connection.sessionalreadyopen":
             last_ttm_session_id = self.get_last_ttm_session_id()
             self.disconnect_session(last_ttm_session_id)
             return self.create_new_session(count=count + 1)
         raise ValueError("Unable to create session; please verify your configuration.")
 
@@ -122,15 +122,15 @@
                 "centralId": self.central_id,
                 "transmitterId": self.transmitter_id,
                 "systemId": self.system_id,
                 "ttmSessionId": self.ttm_session_id,
             },
         )
         if r.status_code != 200:
-            self.account.sleep_while_run(10)
+            self.account.sleep_while_run(10, log=True)
             return self.get_central_status(count + 1)
         return r.json()
 
     def analyze_central_status(self, data):
         """Analyze the result provided by get_central_status(), looking for faults."""
         had_fault = self.status_fault
         self.status_fault = False
@@ -193,15 +193,15 @@
             "/status/getSystemState",
             json_data={
                 "centralId": self.central_id,
                 "ttmSessionId": self.ttm_session_id,
             },
         )
         if r.status_code != 200:
-            self.account.sleep_while_run(10)
+            self.account.sleep_while_run(10, log=True)
             return self.update_status(count + 1)
         content = r.json()
         self.set_active_groups(set(content["groups"]))
 
     def activate_groups(self, groups: Set[int]):
         """Activate some groups."""
         self.account.change_alarm_state(self, groups)
@@ -227,15 +227,15 @@
                 "group": groups_l,
                 "currentGroup": [],
                 "nbGroups": "4",
                 "ttmSessionId": self.ttm_session_id,
             },
         )
         if r.status_code != 200:
-            self.account.sleep_while_run(10)
+            self.account.sleep_while_run(10, log=True)
             return self.send_activation_command(groups=groups, count=count + 1)
         content = r.json()
         if content["commandStatus"] != "CMD_OK":
             raise ValueError("Error during activation.")
         self.set_active_groups(set(content["groups"]))
 
     def deactivate_alarm(self, count=0):
@@ -251,15 +251,15 @@
                 "group": [],
                 "currentGroup": [],
                 "nbGroups": "4",
                 "ttmSessionId": self.ttm_session_id,
             },
         )
         if r.status_code != 200:
-            self.account.sleep_while_run(10)
+            self.account.sleep_while_run(10, log=True)
             return self.deactivate_alarm(count=count + 1)
         content = r.json()
         if content["commandStatus"] != "CMD_OK":
             raise ValueError("Unable to complete deactivation.")
 
 
 class DiagralAccount:
@@ -336,18 +336,20 @@
         r = requests.request(
             method.lower(),
             url,
             json=json_data,
             headers=headers,
             timeout=60,
         )
-        if self.config.log_requests:
-            logger.debug(f"{url}: {r.status_code}")
-            if r.status_code != 500:
-                logger.debug(f"{r.text}")
+        if self.config.verbosity >= 4:
+            logger.debug(
+                f"{url}: {r.status_code}", self.extra_log_data(action="api-request")
+            )
+            if r.status_code != 500 and self.config.verbosity >= 5:
+                logger.debug(f"{r.text}", self.extra_log_data(action="api-request"))
         if self.show_mockup_requests:
             try:
                 json_out = r.json()
             except requests.exceptions.JSONDecodeError:
                 json_out = None
             print(
                 f"""register('{endpoint}', {json_out!r}, {json_data!r}, {r.status_code})"""
@@ -424,33 +426,41 @@
             to_expunge = False
             index = 0
             while index < check_count and self.is_running:
                 to_expunge = self._perform_imap_search(imap_client) or to_expunge
                 self.sleep_while_run(check_interval_in_s)
                 index += 1
             if to_expunge:
-                logger.debug(
-                    f"Apply IMAP commands to {self.imap_login}@{self.imap_hostname}:{self.imap_port}",
-                    extra=self.extra_log_data(action="imap", detail="apply"),
-                )
+                if self.config.verbosity >= 4:
+                    logger.debug(
+                        f"Apply IMAP commands to {self.imap_login}@{self.imap_hostname}:{self.imap_port}",
+                        extra=self.extra_log_data(action="imap", detail="apply"),
+                    )
                 imap_client.expunge()
 
-    def sleep_while_run(self, interval_in_s: int):
+    def sleep_while_run(self, interval_in_s: int, log: bool = False):
         """Sleep for the given interval if active."""
+        if log:
+            logger.info(
+                "Sleeping for %d seconds",
+                interval_in_s,
+                self.extra_log_data(action="sleep"),
+            )
         for __ in range(interval_in_s * 10):
             if not self.is_running:
                 return
             time.sleep(0.1)
 
     def _perform_imap_search(self, imap_client):
         """Perform an IMAP search to check for alarm emails."""
-        logger.debug(
-            f"Search in {self.imap_login}@{self.imap_hostname}:{self.imap_port}",
-            extra=self.extra_log_data(action="imap", detail="search"),
-        )
+        if self.config.verbosity >= 4:
+            logger.debug(
+                f"Search in {self.imap_login}@{self.imap_hostname}:{self.imap_port}",
+                extra=self.extra_log_data(action="imap", detail="search"),
+            )
         typ, data = imap_client.search(None, "NOT DELETED")
         if typ != "OK":
             raise ValueError("Unable to perform an IMAP search for new messages.")
         max_document_size = 100000
         to_expunge = False
         # noinspection PyUnresolvedReferences
         for message_num in data[0].decode().split():
@@ -527,27 +537,29 @@
                     system.create_new_session()
                     status = system.get_central_status()
                     system.analyze_central_status(status)
                     system.disconnect_session()
                 except Exception as e:
                     logger.exception(e, extra=system.extra_log_data())
                     capture_some_exception(e)
-                    self.sleep_while_run(5)
+                    self.sleep_while_run(5, log=True)
             self.do_logout()
-            self.sleep_while_run(1)
+        self.sleep_while_run(1)
 
     def change_alarm_state(self, system: DiagralAlarmSystem, groups: Set[int]):
         """Change the alarm state."""
+        extra = self.extra_log_data(action="alarm_state")
+        logger.info(f"Change alarm state of {system.name} to {groups}", extra=extra)
         with self.request_lock:
             self.do_login()
             system.create_new_session()
             system.send_activation_command(groups)
             system.disconnect_session()
             self.do_logout()
-            time.sleep(1)
+        time.sleep(1)
 
     def run(self):
         """Continuously update the systems and looks for alarms."""
         extra = self.extra_log_data()
         logger.debug(f"Initialize system data for {self.login}", extra=extra)
         self.do_login()
         self.initialize_systems()
```

### Comparing `diagralhomekit-0.9.4/diagralhomekit/homekit_alarm.py` & `diagralhomekit-0.9.5/diagralhomekit/homekit_alarm.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,15 +106,22 @@
         except Exception as e:
             logger.exception(e, extra=extra)
             capture_some_exception(e)
 
     @Accessory.run_at_interval(10)
     def run(self):
         """Check if something has changed."""
+        current_fault = self.sensor_status_fault.get_value()
         fault = 1 if self.alarm_system.status_fault else 0
+        if current_fault != fault:
+            extra = self.alarm_system.extra_log_data(fault=str(fault), action="run")
+            logger.info(
+                f"Fault state {fault} set for {self.alarm_system.name}.",
+                extra=extra,
+            )
         self.sensor_status_fault.set_value(fault)
         self.alarm_status_fault.set_value(fault)
         active_groups = self.alarm_system.get_active_groups()
         stay_groups = self.alarm_system.get_stay_groups()
         night_groups = self.alarm_system.get_night_groups()
 
         log_level = logging.INFO
@@ -146,20 +153,27 @@
                 extra=extra,
             )
         if (
             self.alarm_target_state.get_value() != state
             and state != self.STATE_ALARM_TRIGGERED
         ):
             if self.required_target_state is None:
-                # indicate an external change (through the native app)
-                self.alarm_target_state.set_value(state)
+                # an external change happened (through the native app)
+                extra = self.alarm_system.extra_log_data(
+                    state=self.state_texts[state], action="set"
+                )
+                logger.info(
+                    f"State {self.state_texts[state]} externally set at {self.alarm_system.name}.",
+                    extra=extra,
+                )
             elif self.required_target_state == state:
                 extra = self.alarm_system.extra_log_data(
                     state=self.state_texts[state], action="reached"
                 )
                 logger.info(
                     f"State {self.state_texts[state]} reached by {self.alarm_system.name}.",
                     extra=extra,
                 )
                 self.required_target_state = None
+            self.alarm_target_state.set_value(state)
 
         self.alarm_current_state.set_value(state)
```

### Comparing `diagralhomekit-0.9.4/diagralhomekit/http_plugin.py` & `diagralhomekit-0.9.5/diagralhomekit/http_plugin.py`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.4/diagralhomekit/main.py` & `diagralhomekit-0.9.5/diagralhomekit/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,33 +96,33 @@
     if args.sentry_dsn:
         sentry_sdk.init(args.sentry_dsn)
         logger.debug("Sentry DSN configured.")
 
     run_daemons(
         config_dir,
         listen_port,
-        log_requests=args.verbosity >= 3,
+        verbosity=args.verbosity,
     )
 
 
-def run_daemons(config_dir, listen_port, log_requests: bool = False):
+def run_daemons(config_dir, listen_port, verbosity: int = 1):
     """launch all processes: Homekit and Diagral checker."""
     persist_file = config_dir / "persist.json"
     config_file = config_dir / "config.ini"
     logger.info(f"configuration file: {config_file}")
     logger.info(f"persistence file: {persist_file}")
     logger.info(f"listen port: {listen_port}")
 
     driver = AccessoryDriver(
         port=listen_port,
         persist_file=persist_file,
     )
     bridge = Bridge(driver, "Diagral e-One")
     config = HomekitConfig()
-    config.log_requests = log_requests
+    config.verbosity = verbosity
     try:
         config.load_config(config_file)
         config.load_accessories(bridge)
         driver.add_accessory(accessory=bridge)
         signal.signal(signal.SIGTERM, driver.signal_handler)
         config.run_all()
         driver.start()
```

### Comparing `diagralhomekit-0.9.4/diagralhomekit/meteofrance.py` & `diagralhomekit-0.9.5/diagralhomekit/meteofrance.py`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.4/diagralhomekit/nut.py` & `diagralhomekit-0.9.5/diagralhomekit/nut.py`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.4/diagralhomekit/plex.py` & `diagralhomekit-0.9.5/diagralhomekit/plex.py`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.4/diagralhomekit/plugin.py` & `diagralhomekit-0.9.5/diagralhomekit/plugin.py`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.4/diagralhomekit/utils.py` & `diagralhomekit-0.9.5/diagralhomekit/utils.py`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.4/pyproject.toml` & `diagralhomekit-0.9.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.poetry]
 authors = ["d9pouces <github@19pouces.net>"]
 description = "Apple HomeKit integration for Diagral alarm systems"
 license = "CeCILL-B"
 name = "diagralhomekit"
 readme = "README.md"
-version = "0.9.4"
+version = "0.9.5"
 
 [tool.poetry.dependencies]
 HAP-python = "^4.6.0"
 base36 = "^0.1.1"
 meteofrance-api = "^1.2.0"
 nut2 = "^2.1.1"
 pyqrcode = "^1.2.1"
```

### Comparing `diagralhomekit-0.9.4/setup.py` & `diagralhomekit-0.9.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'sentry-sdk>=1.18.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['diagral-homekit = diagralhomekit.main:main']}
 
 setup_kwargs = {
     'name': 'diagralhomekit',
-    'version': '0.9.4',
+    'version': '0.9.5',
     'description': 'Apple HomeKit integration for Diagral alarm systems',
     'long_description': "DiagralHomekit\n==============\n\n[![PyPI version](https://badge.fury.io/py/diagralhomekit.svg)](https://badge.fury.io/py/diagralhomekit)\n\nAllow to control your Diagral alarm systems through Apple Homekit.\n\n\nFirst, you need to create a configuration file `~/.diagralhomekit/config.ini` with connection details for all Diagral systems.\n\n```ini\n[diagral:Home]\nname=[an explicit name for this system]\nlogin=[email address of the Diagral account]\npassword=[password for the Diagral account]\nimap_login=[IMAP login for the email address receiving alarm alerts]\nimap_password=[IMAP password]\nimap_hostname=[IMAP server]\nimap_port=[IMAP port]\nimap_use_tls=[true/1/on if you use SSL for the IMAP connection]\nmaster_code=[a Diagral master code, able to arm or disarm the alarm]\nsystem_id=[system id — see below]\ntransmitter_id=[transmitter id — see below]\ncentral_id=[central id — see below]\n\n```\n`system_id`, `transmitter_id` and `central_id` can be retrieved with the following command, that prepares a configuration file:\n\n```bash\npython3 -m diagralhomekit --config-dir ~/.diagralhomekit --create-config 'diagral@account.com:password'\n```\n\nThen you can run the script:\n\n```bash\npython3 -m diagralhomekit --port 6666 --config-dir ~/.diagralhomekit -v 2\n```\nOn the first launch, a QR code is displayed and can be scanned in Homekit, like any Homekit-compatible device.\n\n\nYou can send logs to [Loki](https://grafana.com/oss/loki/) with `--loki-url=https://username:password@my.loki.server/loki/api/v1/push`.\nYou can also send alerts to [Sentry](https://sentry.io/) with `--sentry-dsn=my_sentry_dsn`.\n\nEverything can be configured by environment variables instead of arguments:\n\n```bash\nDIAGRAL_PORT=6666\nDIAGRAL_CONFIG=/etc/diagralhomekit\nDIAGRAL_SENTRY_DSN=https://sentry_dsn@sentry.io/42\nDIAGRAL_LOKI_URL=https://username:password@my.loki.server/loki/api/v1/push\nDIAGRAL_VERBOSITY=1\n```\n\n\n**As many sensitive data must be stored in this configuration file, so you should create a dedicated email address and Diagral account.**\n\n\nPlex sensor\n-----------\n\nA presence can be detected when a specified Plex player is playing something:\n```ini\n[plex:appletv_web]\nserver_token=[authentication token]\nserver_url=[url of your Plex server]\nplayer_name=[Displayed name for the player]\nplayer_device=None,\nplayer_product=[Product name of the targeted player]\nplayer_title=[Title of the targeted player]\nplayer_address=[IP address of the targeted player]\n```\nOnly one of the last four properties is required to match with the targeted player.\nTo get actual property values, you can use `curl`:\n\n```bash\ncurl -H Accept:application/json -H X-Plex-Token:[authentication token] [url of your Plex server]/status/sessions\n```\n\nHTTP monitoring\n---------------\n\nYou can monitor some websites, as air purifier sensors (no Homekit sensor is available for HTTP monitoring…):\n```ini\n[internet:website]\nurl=[url to check]\nname=[Displayed name]\n```\n\nWeather monitoring\n------------------\n\nYou can monitor weather, and emulate a presence when it will rain in the next 10 minutes:\n\n```ini\n[meteofrance:paris]\nname=Paris\nlatitude=48.866667\nlongitude=2.333333\ncountry=FR\nregion=Île-de-France\n```\n\nUPS monitoring\n--------------\n\nUPS can also be monitoring, as soon as NUT is locally installed (standard UPS monitoring server on Linux.\n```\n[ups:home]\nname=eaton650\n```\n",
     'author': 'd9pouces',
     'author_email': 'github@19pouces.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `diagralhomekit-0.9.4/PKG-INFO` & `diagralhomekit-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diagralhomekit
-Version: 0.9.4
+Version: 0.9.5
 Summary: Apple HomeKit integration for Diagral alarm systems
 License: CECILL-B
 Author: d9pouces
 Author-email: github@19pouces.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: CeCILL-B Free Software License Agreement (CECILL-B)
 Classifier: Programming Language :: Python :: 3
```

