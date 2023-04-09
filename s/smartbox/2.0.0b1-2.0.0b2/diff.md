# Comparing `tmp/smartbox-2.0.0b1.tar.gz` & `tmp/smartbox-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartbox-2.0.0b1.tar", last modified: Fri Dec 30 12:11:49 2022, max compression
+gzip compressed data, was "smartbox-2.0.0b2.tar", last modified: Sun Apr  9 09:00:08 2023, max compression
```

## Comparing `smartbox-2.0.0b1.tar` & `smartbox-2.0.0b2.tar`

### file list

```diff
@@ -1,22 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-30 12:11:49.481350 smartbox-2.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (116)     1071 2022-12-30 12:11:40.000000 smartbox-2.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     4324 2022-12-30 12:11:49.481350 smartbox-2.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3805 2022-12-30 12:11:40.000000 smartbox-2.0.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      103 2022-12-30 12:11:40.000000 smartbox-2.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)     1411 2022-12-30 12:11:49.481350 smartbox-2.0.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-30 12:11:49.481350 smartbox-2.0.0b1/smartbox/
--rw-r--r--   0 runner    (1001) docker     (116)      224 2022-12-30 12:11:40.000000 smartbox-2.0.0b1/smartbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7085 2022-12-30 12:11:40.000000 smartbox-2.0.0b1/smartbox/cmd.py
--rw-r--r--   0 runner    (1001) docker     (116)       85 2022-12-30 12:11:40.000000 smartbox-2.0.0b1/smartbox/error.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-30 12:11:40.000000 smartbox-2.0.0b1/smartbox/py.typed
--rw-r--r--   0 runner    (1001) docker     (116)     7441 2022-12-30 12:11:40.000000 smartbox-2.0.0b1/smartbox/session.py
--rw-r--r--   0 runner    (1001) docker     (116)     7620 2022-12-30 12:11:40.000000 smartbox-2.0.0b1/smartbox/socket.py
--rw-r--r--   0 runner    (1001) docker     (116)     7318 2022-12-30 12:11:40.000000 smartbox-2.0.0b1/smartbox/update_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-30 12:11:49.481350 smartbox-2.0.0b1/smartbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4324 2022-12-30 12:11:49.000000 smartbox-2.0.0b1/smartbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      406 2022-12-30 12:11:49.000000 smartbox-2.0.0b1/smartbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-30 12:11:49.000000 smartbox-2.0.0b1/smartbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       51 2022-12-30 12:11:49.000000 smartbox-2.0.0b1/smartbox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-30 12:11:49.000000 smartbox-2.0.0b1/smartbox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       73 2022-12-30 12:11:49.000000 smartbox-2.0.0b1/smartbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2022-12-30 12:11:49.000000 smartbox-2.0.0b1/smartbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:00:08.264045 smartbox-2.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-09 08:59:57.000000 smartbox-2.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-04-09 09:00:08.264045 smartbox-2.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-04-09 08:59:57.000000 smartbox-2.0.0b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-09 08:59:57.000000 smartbox-2.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-09 09:00:08.264045 smartbox-2.0.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:00:08.264045 smartbox-2.0.0b2/smartbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-09 08:59:57.000000 smartbox-2.0.0b2/smartbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-04-09 08:59:57.000000 smartbox-2.0.0b2/smartbox/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-09 08:59:57.000000 smartbox-2.0.0b2/smartbox/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:59:57.000000 smartbox-2.0.0b2/smartbox/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-04-09 08:59:57.000000 smartbox-2.0.0b2/smartbox/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-04-09 08:59:57.000000 smartbox-2.0.0b2/smartbox/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-09 08:59:57.000000 smartbox-2.0.0b2/smartbox/update_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:00:08.264045 smartbox-2.0.0b2/smartbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-04-09 09:00:08.000000 smartbox-2.0.0b2/smartbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-09 09:00:08.000000 smartbox-2.0.0b2/smartbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 09:00:08.000000 smartbox-2.0.0b2/smartbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-09 09:00:08.000000 smartbox-2.0.0b2/smartbox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 09:00:08.000000 smartbox-2.0.0b2/smartbox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-09 09:00:08.000000 smartbox-2.0.0b2/smartbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 09:00:08.000000 smartbox-2.0.0b2/smartbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:00:08.264045 smartbox-2.0.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-04-09 08:59:57.000000 smartbox-2.0.0b2/tests/test_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-04-09 08:59:57.000000 smartbox-2.0.0b2/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-04-09 08:59:57.000000 smartbox-2.0.0b2/tests/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-04-09 08:59:57.000000 smartbox-2.0.0b2/tests/test_update_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-09 08:59:57.000000 smartbox-2.0.0b2/tests/test_update_manager_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-09 08:59:57.000000 smartbox-2.0.0b2/tests/test_version.py
```

### Comparing `smartbox-2.0.0b1/LICENSE` & `smartbox-2.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `smartbox-2.0.0b1/PKG-INFO` & `smartbox-2.0.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: smartbox
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: Python API to control heating 'smart boxes'
 Home-page: https://github.com/graham33/smartbox
 Author: Graham Bennett
 Author-email: graham@grahambennett.org
 Project-URL: Bug Tracker, https://github.com/graham33/smartbox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # smartbox ![build](https://github.com/graham33/smartbox/workflows/Python%20package/badge.svg) [![PyPI version](https://badge.fury.io/py/smartbox.svg)](https://badge.fury.io/py/smartbox) [![codecov](https://codecov.io/gh/graham33/smartbox/branch/main/graph/badge.svg?token=BMCS2E9OC7)](https://codecov.io/gh/graham33/smartbox) [![PyPI license](https://img.shields.io/pypi/l/smartbox.svg)](https://pypi.python.org/pypi/smartbox/) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/smartbox.svg)](https://pypi.python.org/pypi/smartbox/)
 
 Python API to control heating 'smart boxes'
```

### Comparing `smartbox-2.0.0b1/README.md` & `smartbox-2.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `smartbox-2.0.0b1/setup.cfg` & `smartbox-2.0.0b2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [metadata]
 name = smartbox
-version = 2.0.0-beta.1
+version = 2.0.0-beta.2
 author = Graham Bennett
 author_email = graham@grahambennett.org
 description = Python API to control heating 'smart boxes'
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/graham33/smartbox
 project_urls = 
 	Bug Tracker = https://github.com/graham33/smartbox/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
-python_requires = >=3.8
+python_requires = >=3.9
 packages = smartbox
 include_package_data = True
 install_requires = 
 	aiohttp
 	Click
 	jq
 	python-socketio>=4.6.0,<5.0.0
@@ -42,17 +42,14 @@
 [options.entry_points]
 console_scripts = 
 	smartbox = smartbox.cmd:smartbox
 
 [aliases]
 test = pytest
 
-[flake8]
-max-line-length = 120
-
 [mypy]
 
 [mypy-freezegun]
 ignore_missing_imports = True
 
 [mypy-jq]
 ignore_missing_imports = True
@@ -67,14 +64,11 @@
 ignore_missing_imports = True
 
 [tool:pytest]
 asyncio_mode = auto
 log_cli = true
 log_cli_level = warning
 
-[yapf]
-column_limit = 120
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `smartbox-2.0.0b1/smartbox/cmd.py` & `smartbox-2.0.0b2/smartbox/cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 @click.option(
     "-v", "--verbose/--no-verbose", default=False, help="Enable verbose logging"
 )
 @click.pass_context
 def smartbox(ctx, api_name, basic_auth_creds, username, password, verbose):
     ctx.ensure_object(dict)
     logging.basicConfig(
-        format="%(asctime)s %(levelname)-8s [%(name)s.%(funcName)s:%(lineno)d] %(message)s",
+        format="%(asctime)s %(levelname)-8s "
+        "[%(name)s.%(funcName)s:%(lineno)d] %(message)s",
         level=logging.DEBUG if verbose else logging.INFO,
         datefmt="%Y-%m-%d %H:%M:%S",
     )
     session = Session(api_name, basic_auth_creds, username, password)
     ctx.obj["session"] = session
     ctx.obj["verbose"] = verbose
 
@@ -208,18 +209,19 @@
         _LOGGER.info("Received dev_data:")
         _pretty_print(data)
 
     def on_update(data):
         _LOGGER.info("Received update:")
         _pretty_print(data)
 
+    event_loop = asyncio.new_event_loop()
+    asyncio.set_event_loop(event_loop)
     socket_session = SocketSession(
         session, device_id, on_dev_data, on_update, verbose, add_sigint_handler=True
     )
-    event_loop = asyncio.get_event_loop()
     task = event_loop.create_task(socket_session.run())
     event_loop.run_until_complete(task)
 
 
 # For debuggging
 if __name__ == "__main__":
     smartbox()
```

### Comparing `smartbox-2.0.0b1/smartbox/session.py` & `smartbox-2.0.0b2/smartbox/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,17 @@
             )
             raise SmartboxError("Received invalid auth response")
         self._access_token = r["access_token"]
         self._refresh_token = r["refresh_token"]
         if r["expires_in"] < _MIN_TOKEN_LIFETIME:
             _LOGGER.warning(
                 (
-                    f"Token expires in {r['expires_in']}s, which is below minimum lifetime "
-                    f"of {_MIN_TOKEN_LIFETIME}s - will refresh again on next operation"
+                    f"Token expires in {r['expires_in']}s"
+                    f", which is below minimum lifetime of {_MIN_TOKEN_LIFETIME}s"
+                    " - will refresh again on next operation"
                 )
             )
         self._expires_at = datetime.datetime.now() + datetime.timedelta(
             seconds=r["expires_in"]
         )
         _LOGGER.debug(
             (
```

### Comparing `smartbox-2.0.0b1/smartbox/socket.py` & `smartbox-2.0.0b2/smartbox/socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,16 +106,17 @@
         )
         self._sio.register_namespace(self._api_v2_ns)
 
         @self._sio.event
         async def connect():
             _LOGGER.debug("Received connect socket event")
             if add_sigint_handler:
-                # engineio sets a signal handler on connect, which means we have to set our
-                # own in the connect callback if we want to override it
+                # engineio sets a signal handler on connect, which means we
+                # have to set our own in the connect callback if we want to
+                # override it
                 _LOGGER.debug("Adding signal handler")
                 event_loop = asyncio.get_event_loop()
 
                 def sigint_handler():
                     _LOGGER.debug("Caught SIGINT, cancelling loop")
                     asyncio.ensure_future(self.cancel())
 
@@ -139,15 +140,18 @@
 
         _LOGGER.debug("Starting main loop")
         while not self._loop_should_exit:
             # TODO: accessors in session
             encoded_token = urllib.parse.quote(
                 self._session._access_token, safe="~()*!.'"
             )
-            url = f"{self._session._api_host}/?token={encoded_token}&dev_id={self._device_id}"
+            url = (
+                f"{self._session._api_host}"
+                + f"/?token={encoded_token}&dev_id={self._device_id}"
+            )
 
             # Try to connect
             _LOGGER.debug(
                 f"Connecting to {url} (will try {self._reconnect_attempts} times)"
             )
             for attempt in range(self._reconnect_attempts):
                 _LOGGER.debug(f"Connecting to {url} (attempt #{attempt})")
@@ -166,16 +170,16 @@
                         f", {remaining} retries remaining"
                         f", sleeping {sleep_time}s"
                     )
                     if remaining > 0:
                         await asyncio.sleep(sleep_time)
                     else:
                         logging.warning(
-                            f"Failed to connect after {self._reconnect_attempts} attempts"
-                            ", falling through to refresh token"
+                            f"Failed to connect after {self._reconnect_attempts}"
+                            " attempts, falling through to refresh token"
                         )
                 else:
                     _LOGGER.info(f"Successfully connected to {url}")
                     await self._sio.wait()
                     _LOGGER.info("Socket loop exited, disconnecting")
                     await self._sio.disconnect()
                     _LOGGER.debug("Breaking loop to refresh token")
```

### Comparing `smartbox-2.0.0b1/smartbox/update_manager.py` & `smartbox-2.0.0b2/smartbox/update_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,16 @@
 
 class UpdateSubscription(object):
     """Subscription for updates."""
 
     def __init__(
         self, path_regex: str, jq_expr: str, callback: Callable[[Dict[str, Any]], None]
     ):
-        """Create an update subscription for the given path regex and body jq expression."""
+        """Create an update subscription for the given path regex and body jq
+        expression."""
         self._path_regex = re.compile(path_regex)
         self._jq_matcher = OptimisedJQMatcher(jq_expr)
         self._callback = callback
 
     def match(self, input_data: Dict[str, Any]) -> bool:
         """Return matches for this subscription for the given update."""
         path_match = self._path_regex.search(input_data["path"])
```

### Comparing `smartbox-2.0.0b1/smartbox.egg-info/PKG-INFO` & `smartbox-2.0.0b2/smartbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: smartbox
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: Python API to control heating 'smart boxes'
 Home-page: https://github.com/graham33/smartbox
 Author: Graham Bennett
 Author-email: graham@grahambennett.org
 Project-URL: Bug Tracker, https://github.com/graham33/smartbox/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # smartbox ![build](https://github.com/graham33/smartbox/workflows/Python%20package/badge.svg) [![PyPI version](https://badge.fury.io/py/smartbox.svg)](https://badge.fury.io/py/smartbox) [![codecov](https://codecov.io/gh/graham33/smartbox/branch/main/graph/badge.svg?token=BMCS2E9OC7)](https://codecov.io/gh/graham33/smartbox) [![PyPI license](https://img.shields.io/pypi/l/smartbox.svg)](https://pypi.python.org/pypi/smartbox/) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/smartbox.svg)](https://pypi.python.org/pypi/smartbox/)
 
 Python API to control heating 'smart boxes'
```

