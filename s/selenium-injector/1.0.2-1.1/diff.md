# Comparing `tmp/selenium_injector-1.0.2.tar.gz` & `tmp/selenium_injector-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\selenium_injector-1.0.2.tar", last modified: Thu Apr  6 21:49:46 2023, max compression
+gzip compressed data, was "dist\selenium_injector-1.1.tar", last modified: Sun Apr  9 11:09:41 2023, max compression
```

## Comparing `selenium_injector-1.0.2.tar` & `selenium_injector-1.1.tar`

### file list

```diff
@@ -1,37 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 21:49:46.000000 selenium_injector-1.0.2/
--rw-rw-rw-   0        0        0      641 2022-11-24 08:41:11.000000 selenium_injector-1.0.2/LICENSE.md
--rw-rw-rw-   0        0        0      199 2023-04-06 20:52:34.000000 selenium_injector-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5135 2023-04-06 21:49:46.000000 selenium_injector-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3822 2023-04-06 21:40:15.000000 selenium_injector-1.0.2/README.md
--rw-rw-rw-   0        0        0      522 2023-04-06 21:41:47.000000 selenium_injector-1.0.2/build_upload.md
--rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_injector-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      131 2023-04-06 21:49:46.000000 selenium_injector-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1831 2023-04-06 21:42:12.000000 selenium_injector-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 21:49:46.000000 selenium_injector-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-06 21:49:46.000000 selenium_injector-1.0.2/src/selenium_injector/
--rw-rw-rw-   0        0        0       23 2023-01-13 12:14:35.000000 selenium_injector-1.0.2/src/selenium_injector/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 21:49:46.000000 selenium_injector-1.0.2/src/selenium_injector/files/
-drwxrwxrwx   0        0        0        0 2023-04-06 21:49:46.000000 selenium_injector-1.0.2/src/selenium_injector/files/injector_extension/
--rw-rw-rw-   0        0        0     6311 2023-04-06 21:00:52.000000 selenium_injector-1.0.2/src/selenium_injector/files/injector_extension/background.js
-drwxrwxrwx   0        0        0        0 2023-04-06 21:49:46.000000 selenium_injector-1.0.2/src/selenium_injector/files/tmp/
-drwxrwxrwx   0        0        0        0 2023-04-06 21:49:46.000000 selenium_injector-1.0.2/src/selenium_injector/files/tmp/injector_extension/
--rw-rw-rw-   0        0        0     6478 2023-04-06 21:01:04.000000 selenium_injector-1.0.2/src/selenium_injector/files/tmp/injector_extension/background.js
--rw-rw-rw-   0        0        0        0 2023-04-06 20:20:08.000000 selenium_injector-1.0.2/src/selenium_injector/files/tmp/injector_extension/content_helper.js
--rw-rw-rw-   0        0        0     2019 2023-03-26 16:12:21.000000 selenium_injector-1.0.2/src/selenium_injector/files/tmp/injector_extension/manifest.json
--rw-rw-rw-   0        0        0      899 2023-04-06 20:55:01.000000 selenium_injector-1.0.2/src/selenium_injector/injector.py
-drwxrwxrwx   0        0        0        0 2023-04-06 21:49:46.000000 selenium_injector-1.0.2/src/selenium_injector/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_injector-1.0.2/src/selenium_injector/scripts/__init__.py
--rw-rw-rw-   0        0        0     1449 2023-03-25 22:43:40.000000 selenium_injector-1.0.2/src/selenium_injector/scripts/multi_thread.py
--rw-rw-rw-   0        0        0     1100 2023-04-06 20:02:29.000000 selenium_injector-1.0.2/src/selenium_injector/scripts/socket.py
--rw-rw-rw-   0        0        0     3169 2023-04-06 20:15:45.000000 selenium_injector-1.0.2/src/selenium_injector/scripts/sync_websocket.py
-drwxrwxrwx   0        0        0        0 2023-04-06 21:49:46.000000 selenium_injector-1.0.2/src/selenium_injector/utils/
--rw-rw-rw-   0        0        0       19 2022-11-24 10:40:41.000000 selenium_injector-1.0.2/src/selenium_injector/utils/__init__.py
--rw-rw-rw-   0        0        0     1260 2023-04-06 20:48:06.000000 selenium_injector-1.0.2/src/selenium_injector/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-06 21:49:46.000000 selenium_injector-1.0.2/src/selenium_injector.egg-info/
--rw-rw-rw-   0        0        0     5135 2023-04-06 21:49:46.000000 selenium_injector-1.0.2/src/selenium_injector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      913 2023-04-06 21:49:46.000000 selenium_injector-1.0.2/src/selenium_injector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 21:49:46.000000 selenium_injector-1.0.2/src/selenium_injector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-04-06 21:49:46.000000 selenium_injector-1.0.2/src/selenium_injector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-06 21:49:46.000000 selenium_injector-1.0.2/src/selenium_injector.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-06 21:49:46.000000 selenium_injector-1.0.2/tests/
--rw-rw-rw-   0        0        0     3232 2023-02-25 14:04:13.000000 selenium_injector-1.0.2/tests/test_interceptor.py
+drwxrwxrwx   0        0        0        0 2023-04-09 11:09:41.000000 selenium_injector-1.1/
+-rw-rw-rw-   0        0        0      641 2022-11-24 08:41:11.000000 selenium_injector-1.1/LICENSE.md
+-rw-rw-rw-   0        0        0      199 2023-04-06 20:52:34.000000 selenium_injector-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5556 2023-04-09 11:09:41.000000 selenium_injector-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4245 2023-04-09 11:09:12.000000 selenium_injector-1.1/README.md
+-rw-rw-rw-   0        0        0      522 2023-04-06 21:41:47.000000 selenium_injector-1.1/build_upload.md
+-rw-rw-rw-   0        0        0      101 2022-11-24 08:05:09.000000 selenium_injector-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      131 2023-04-09 11:09:41.000000 selenium_injector-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1831 2023-04-06 21:42:12.000000 selenium_injector-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 11:09:41.000000 selenium_injector-1.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-09 11:09:41.000000 selenium_injector-1.1/src/selenium_injector/
+-rw-rw-rw-   0        0        0       21 2023-04-09 11:08:40.000000 selenium_injector-1.1/src/selenium_injector/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 11:09:41.000000 selenium_injector-1.1/src/selenium_injector/files/
+drwxrwxrwx   0        0        0        0 2023-04-09 11:09:41.000000 selenium_injector-1.1/src/selenium_injector/files/injector_extension/
+-rw-rw-rw-   0        0        0     7901 2023-04-09 10:13:44.000000 selenium_injector-1.1/src/selenium_injector/files/injector_extension/background.js
+drwxrwxrwx   0        0        0        0 2023-04-09 11:09:41.000000 selenium_injector-1.1/src/selenium_injector/files/tmp/
+drwxrwxrwx   0        0        0        0 2023-04-09 11:09:41.000000 selenium_injector-1.1/src/selenium_injector/files/tmp/injector_extension/
+-rw-rw-rw-   0        0        0     8071 2023-04-09 11:04:53.000000 selenium_injector-1.1/src/selenium_injector/files/tmp/injector_extension/background.js
+-rw-rw-rw-   0        0        0        0 2023-04-06 20:20:08.000000 selenium_injector-1.1/src/selenium_injector/files/tmp/injector_extension/content_helper.js
+-rw-rw-rw-   0        0        0     2046 2023-04-07 07:59:51.000000 selenium_injector-1.1/src/selenium_injector/files/tmp/injector_extension/manifest.json
+-rw-rw-rw-   0        0        0    88326 2023-04-07 07:15:12.000000 selenium_injector-1.1/src/selenium_injector/files/tmp/injector_extension/peg.min.js
+-rw-rw-rw-   0        0        0     4765 2023-04-09 10:53:20.000000 selenium_injector-1.1/src/selenium_injector/injector.py
+drwxrwxrwx   0        0        0        0 2023-04-09 11:09:41.000000 selenium_injector-1.1/src/selenium_injector/scripts/
+-rw-rw-rw-   0        0        0        0 2022-11-29 13:10:11.000000 selenium_injector-1.1/src/selenium_injector/scripts/__init__.py
+-rw-rw-rw-   0        0        0     1305 2023-04-09 10:46:23.000000 selenium_injector-1.1/src/selenium_injector/scripts/socket.py
+-rw-rw-rw-   0        0        0     3488 2023-04-09 10:58:34.000000 selenium_injector-1.1/src/selenium_injector/scripts/sync_websocket.py
+drwxrwxrwx   0        0        0        0 2023-04-09 11:09:41.000000 selenium_injector-1.1/src/selenium_injector/utils/
+-rw-rw-rw-   0        0        0       19 2022-11-24 10:40:41.000000 selenium_injector-1.1/src/selenium_injector/utils/__init__.py
+-rw-rw-rw-   0        0        0     1258 2023-04-07 06:27:15.000000 selenium_injector-1.1/src/selenium_injector/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-09 11:09:41.000000 selenium_injector-1.1/src/selenium_injector.egg-info/
+-rw-rw-rw-   0        0        0     5556 2023-04-09 11:09:40.000000 selenium_injector-1.1/src/selenium_injector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      903 2023-04-09 11:09:40.000000 selenium_injector-1.1/src/selenium_injector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 11:09:40.000000 selenium_injector-1.1/src/selenium_injector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-04-09 11:09:40.000000 selenium_injector-1.1/src/selenium_injector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-09 11:09:40.000000 selenium_injector-1.1/src/selenium_injector.egg-info/top_level.txt
```

### Comparing `selenium_injector-1.0.2/LICENSE.md` & `selenium_injector-1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `selenium_injector-1.0.2/PKG-INFO` & `selenium_injector-1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_injector
-Version: 1.0.2
+Version: 1.1
 Summary: Remote controll a chrome extension
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Injector
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Injector
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Injector/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Injector
@@ -51,85 +51,94 @@
 
 ### Example script
 
 ```python
 from selenium_profiles import driver as mydriver
 from selenium_profiles.profiles import profiles
 
-from selenium_injector.injector import injector
+from selenium_injector.injector import mv3_injector as injector
 
 injector = injector()
 
 mydriver = mydriver()
 profile = profiles.Windows()
 profile["options"]["extensions"] = {"extension_paths": [injector.path]}
 
 driver = mydriver.start(profile, uc_driver=False)
 
 
 input("Enable proxy\n")
-injector.exec_command("proxy.set", ["http", "host", 41149])
-injector.exec_command("proxy.set_auth", ["username", "password"])
+injector.proxy.set("host", 41149, scheme="http", username="username",password="password")
 
 input("Disable proxy\n")
-injector.exec_command("proxy.clear")
+injector.proxy.clear()
 
 input("Press ENTER to quit")
 injector.stop()
 driver.quit()
 ```
 Don't forget to execute
 `driver.quit()`
 in the End. Else-wise your temporary folder will get flooded! and it keeps running
 
 ### Change proxy while running
 
 ```python
-from selenium_injector.injector import injector
+from selenium_injector.injector import mv3_injector as injector
 injector = injector(host="localhost", port = 8001)
 
 # initialize chrome here & load the extension
 # options.add_argument("--load-extension="+injector.path) # as argument
 # profile["options"]["extensions"] = {"extension_paths": [injector.path]} # selenium-profiles
 
-injector.exec_command("proxy.set", ["http", "host", 41149, True, True]) # patch_webrtc = True, patch_location=True by default
-injector.exec_command("proxy.set_auth", ["username", "password"])
+injector.proxy.set("host", 41149, scheme="http", username="username",password="password") # patch_webrtc = True, patch_location=True by default
 
 input("Disable proxy\n")
-injector.exec_command("proxy.clear")
+injector.proxy.clear()
 ```
 
 ### Disable webrtc-ip-leak
 ```python
-from selenium_injector.injector import injector
+from selenium_injector.injector import mv3_injector as injector
 injector = injector()
 
 # initialize chrome here & load the extension here
 
-injector.exec_command("webrtc_leak.disable")
-injector.exec_command("webrtc_leak.clear") # reset webrtc
+injector.webrtc_leak.disable()
+injector.webrtc_leak.clear() # reset webrtc
 ```
 ### block location api
 ```python
-from selenium_injector.injector import injector
+from selenium_injector.injector import mv3_injector as injector
 injector = injector()
 
 # initialize chrome here & load the extension here
 
-injector.exec_command("contentsettings.set_location", ["block"])
-injector.exec_command("contentsettings.set_location", ["allow"]) # reset api policies
+injector.contentsettings.set_location(setting="ask")
+injector.contentsettings.set_location(setting="allow")# reset api policies
 ```
 
+for all available scripts, have a look at [selenium_injector/files/injector_extension/background.js](https://github.com/kaliiiiiiiiii/Selenium-Injector/blob/master/src/selenium_injector/files/injector_extension/background.js)
+
 ## Help
 
 Please feel free to open an issue or fork!
 
 ## Todo
 
-
+- [ ] Add MV2 extension
+  - [ ] change headers
+- [ ] add events
+- [x] types.eval
+  - [ ] for-loops
+  - [ ] async execution
+- [x] authentificaten proxies
+  - [x] manage webrtc-leak
+  - [x] manage locatiom api leak
+  - [ ] proxy per request
 
 ## Deprecated
 
 ## Authors
 
 [Aurin Aegerter](mailto:aurinliun@gmx.ch)
 
@@ -154,7 +163,8 @@
 
 Inspiration, code snippets, etc.
 * [Selenium-Profiles](https://github.com/kaliiiiiiiiii/Selenium-Profiles)
 * [Chrome-devtools-protocol](https://chromedevtools.github.io/devtools-protocol/tot/Fetch/#method-enable)
 * [cdp_event_listeners](https://stackoverflow.com/questions/66227508/selenium-4-0-0-beta-1-how-add-event-listeners-in-cdp)
 * [sync websocket server](https://stackoverflow.com/questions/68939894/implement-a-python-websocket-listener-without-async-asyncio)
 * [chrome-extension-docs](https://developer.chrome.com/docs/extensions/reference/)
+* [PEG-parser](https://github.com/pegjs/pegjs)
```

### Comparing `selenium_injector-1.0.2/README.md` & `selenium_injector-1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -21,85 +21,94 @@
 
 ### Example script
 
 ```python
 from selenium_profiles import driver as mydriver
 from selenium_profiles.profiles import profiles
 
-from selenium_injector.injector import injector
+from selenium_injector.injector import mv3_injector as injector
 
 injector = injector()
 
 mydriver = mydriver()
 profile = profiles.Windows()
 profile["options"]["extensions"] = {"extension_paths": [injector.path]}
 
 driver = mydriver.start(profile, uc_driver=False)
 
 
 input("Enable proxy\n")
-injector.exec_command("proxy.set", ["http", "host", 41149])
-injector.exec_command("proxy.set_auth", ["username", "password"])
+injector.proxy.set("host", 41149, scheme="http", username="username",password="password")
 
 input("Disable proxy\n")
-injector.exec_command("proxy.clear")
+injector.proxy.clear()
 
 input("Press ENTER to quit")
 injector.stop()
 driver.quit()
 ```
 Don't forget to execute
 `driver.quit()`
 in the End. Else-wise your temporary folder will get flooded! and it keeps running
 
 ### Change proxy while running
 
 ```python
-from selenium_injector.injector import injector
+from selenium_injector.injector import mv3_injector as injector
 injector = injector(host="localhost", port = 8001)
 
 # initialize chrome here & load the extension
 # options.add_argument("--load-extension="+injector.path) # as argument
 # profile["options"]["extensions"] = {"extension_paths": [injector.path]} # selenium-profiles
 
-injector.exec_command("proxy.set", ["http", "host", 41149, True, True]) # patch_webrtc = True, patch_location=True by default
-injector.exec_command("proxy.set_auth", ["username", "password"])
+injector.proxy.set("host", 41149, scheme="http", username="username",password="password") # patch_webrtc = True, patch_location=True by default
 
 input("Disable proxy\n")
-injector.exec_command("proxy.clear")
+injector.proxy.clear()
 ```
 
 ### Disable webrtc-ip-leak
 ```python
-from selenium_injector.injector import injector
+from selenium_injector.injector import mv3_injector as injector
 injector = injector()
 
 # initialize chrome here & load the extension here
 
-injector.exec_command("webrtc_leak.disable")
-injector.exec_command("webrtc_leak.clear") # reset webrtc
+injector.webrtc_leak.disable()
+injector.webrtc_leak.clear() # reset webrtc
 ```
 ### block location api
 ```python
-from selenium_injector.injector import injector
+from selenium_injector.injector import mv3_injector as injector
 injector = injector()
 
 # initialize chrome here & load the extension here
 
-injector.exec_command("contentsettings.set_location", ["block"])
-injector.exec_command("contentsettings.set_location", ["allow"]) # reset api policies
+injector.contentsettings.set_location(setting="ask")
+injector.contentsettings.set_location(setting="allow")# reset api policies
 ```
 
+for all available scripts, have a look at [selenium_injector/files/injector_extension/background.js](https://github.com/kaliiiiiiiiii/Selenium-Injector/blob/master/src/selenium_injector/files/injector_extension/background.js)
+
 ## Help
 
 Please feel free to open an issue or fork!
 
 ## Todo
 
-
+- [ ] Add MV2 extension
+  - [ ] change headers
+- [ ] add events
+- [x] types.eval
+  - [ ] for-loops
+  - [ ] async execution
+- [x] authentificaten proxies
+  - [x] manage webrtc-leak
+  - [x] manage locatiom api leak
+  - [ ] proxy per request
 
 ## Deprecated
 
 ## Authors
 
 [Aurin Aegerter](mailto:aurinliun@gmx.ch)
 
@@ -124,7 +133,8 @@
 
 Inspiration, code snippets, etc.
 * [Selenium-Profiles](https://github.com/kaliiiiiiiiii/Selenium-Profiles)
 * [Chrome-devtools-protocol](https://chromedevtools.github.io/devtools-protocol/tot/Fetch/#method-enable)
 * [cdp_event_listeners](https://stackoverflow.com/questions/66227508/selenium-4-0-0-beta-1-how-add-event-listeners-in-cdp)
 * [sync websocket server](https://stackoverflow.com/questions/68939894/implement-a-python-websocket-listener-without-async-asyncio)
 * [chrome-extension-docs](https://developer.chrome.com/docs/extensions/reference/)
+* [PEG-parser](https://github.com/pegjs/pegjs)
```

### Comparing `selenium_injector-1.0.2/build_upload.md` & `selenium_injector-1.1/build_upload.md`

 * *Files identical despite different names*

### Comparing `selenium_injector-1.0.2/setup.py` & `selenium_injector-1.1/setup.py`

 * *Files identical despite different names*

### Comparing `selenium_injector-1.0.2/src/selenium_injector/files/injector_extension/background.js` & `selenium_injector-1.1/src/selenium_injector/files/tmp/injector_extension/background.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -10,18 +10,18 @@
 
 function isFunction(functionToCheck) {
     return functionToCheck && {}.toString.call(functionToCheck) === '[object Function]';
 }
 
 
 // connection to python
-connection = {}
+globalThis.connection = {}
 connection.host = "localhost"
 connection.port = 8001
-connection.username = "selenium_injector"
+connection.username = "selenium_injector-mv3"
 
 connection.connect = function() {
     connection.socket = new WebSocket("ws://" + connection.host + ":" + parseInt(connection.port));
     connection.socket.addEventListener("open", (event) => {
         connection.socket.send(connection.username);
         connection.socket.addEventListener("message", (event) => {
             connection.socket.send(connection.handler(event.data))
@@ -32,59 +32,68 @@
     });
     connection.socket.addEventListener("close", (event) => {
         connection.connect()
     });
 };
 
 connection.handler = function(request) {
-    request = JSON.parse(request);
+    var request = JSON.parse(request);
     types.status = 200
     try {
-        result = types.eval(request)
+        var result = types.eval(request)
     } catch (e) {
-        result = {
+        var result = {
             "message": e.message,
             "stack": e.stack
         };
         types.status = "error"
     };
-    response = '{"result":' + types.stringify(result) + ', "status":' + JSON.stringify(types.status) + '}';
+    var response = '{"result":' + types.stringify(result) + ', "status":' + JSON.stringify(types.status) + '}';
     console.log({
         "request": request,
         "response": JSON.parse(response)
     });
     return response;
 }
 
 
-// perser for unsafe-eval bypass
-types = {}
+// parser for unsafe-eval bypass
+globalThis.types = {};
 
 types.eval = function(type_json) {
     var defaultdict = new DefaultDict(undefined)
-    type_json = Object.assign({}, defaultdict, type_json)
+    var type_json = Object.assign({}, defaultdict, type_json)
     var type = type_json["type"];
-    if (type == "type") {
-        var result = types.eval(type_json["type_json"])
-    } else if (type == "path") {
-        var result = types.path(type_json["path"], type_json["obj"])
-    } else if (type == "exec") {
-        var result = types.exec(type_json["func"], type_json["args"])
-    } else if (type == "val") {
-        var result = type_json["val"]
-    } else if (type == "not") {
-        var result = types.not(type_json["type_json"])
-    } else if (type == "if") {
-        var result = types.if_else(type_json["if"], type_json["do"], type_json["else"])
-    } else if (type == "list") {
-        var result = types.list(type_json["list"])
-    } else if (type == "dict") {
-        var result = types.dict(type_json["dict_list"])
-    } else {
-        reportError(TypeError("Expected type_json, but got " + types.stringify(type_json)))
+    switch (type) {
+        case "type":
+            var result = types.eval(type_json["type_json"]);
+            break;
+        case "path":
+            var result = types.path(type_json["path"], type_json["obj"]);
+            break;
+        case "exec":
+            var result = types.exec(type_json["func"], type_json["args"]);
+            break;
+        case "val":
+            var result = type_json["val"];
+            break;
+        case "if":
+            var result = types.if_else(type_json["if"], type_json["do"], type_json["else"]);
+            break;
+        case "list":
+            var result = types.list(type_json["list"]);
+            break;
+        case "dict":
+            var result = types.dict(type_json["dict_list"]);
+            break;
+        case "op":
+            var result = types.op(type_json["op"], types.eval(type_json["a"]), types.eval(type_json["b"]));
+            break;
+        default:
+            reportError(TypeError("Expected type_json, but got " + types.stringify(type_json)));
     }
     return result;
 }
 
 types.path = function(path, obj = undefined) {
     if (obj == undefined) {
         obj = globalThis
@@ -92,90 +101,131 @@
     for (var i = 0, path = path.split('.'), len = path.length; i < len; i++) {
         obj = obj[path[i]];
     };
     return obj;
 };
 
 types.exec = function(func, args = []) {
-    res_args = [];
+    var res_args = [];
     args.forEach(function(item, index) {
         res_args.push(types.eval(item))
     });
-    res_func = types.eval(func)
+    var res_func = types.eval(func)
     if (isFunction(res_func)) {
         res_func(...res_args)
     } else {
-        reportError(TypeError("Expected a function, got " + types.stringify(res_func)))
+        throw TypeError("Expected a function, got " + types.stringify(res_func))
     };
-}
+};
 
 types.list = function(list) {
     var results = [];
     list.forEach(function(item, index) {
         results.push(types.eval(item))
     });
     return results
-}
+};
 
 types.dict = function(dict_list) {
-    res_dict = {};
+    var res_dict = {};
     dict_list.forEach(function(item) {
         res_dict[types.eval(item["key"])] = types.eval(item["val"])
     });
     return res_dict
-}
-
-types.not = function(type_json) {
-    return !(types.eval(type_json))
-}
+};
 
 types.if_else = function(condition, statement, else_statement = undefined) {
     if (types.eval(condition)) {
-        result = types.eval(statement)
+        var result = types.eval(statement)
     } else {
         if (else_statement == undefined) {
-            result = undefined
+            var result = undefined
         } else {
-            result = types.eval(else_statement)
+            var result = types.eval(else_statement)
         }
     };
     return result
-}
+};
 
 types.stringify = function(obj) {
     var result = JSON.stringify(obj, types.replacer)
     return result
-}
+};
 
 types.replacer = function replacer(key, value) {
     // Filtering out properties
     if (isFunction(value)) {
         types.status = "func_to_str"
         return value.toLocaleString();
     } else if (value == undefined) {
         return null
     } else {
         return value
     }
+};
+
+types.op = function apply_op(op, a, b) {
+    function num(x) {
+        if (typeof x != "number")
+            throw new Error("Expected number but got " + x);
+        return x;
+    }
+
+    function div(x) {
+        if (num(x) == 0)
+            throw new Error("Divide by zero");
+        return x;
+    }
+    switch (op) {
+        case "+":
+            return num(a) + num(b);
+        case "-":
+            return num(a) - num(b);
+        case "*":
+            return num(a) * num(b);
+        case "/":
+            return num(a) / div(b);
+        case "%":
+            return num(a) % div(b);
+        case "&&":
+            return a && b;
+        case "||":
+            return a || b;
+        case "|":
+            return a | b;
+        case "<":
+            return num(a) < num(b);
+        case ">":
+            return num(a) > num(b);
+        case "<=":
+            return num(a) <= num(b);
+        case ">=":
+            return num(a) >= num(b);
+        case "==":
+            return a == b;
+        case "!=":
+            return a != b;
+    }
+    throw new Error("Can't apply operator " + op);
 }
 
 // chrome extension libs
 
-proxy = {}
+globalThis.proxy = {}
 
-proxy.set = function(scheme, host, port, patch_webrtc = true, patch_location = true) {
+proxy.set = function(scheme, host, port, patch_webrtc = true, patch_location = true, bypass_list = ["localhost"]) {
     proxy.config = {
         mode: "fixed_servers",
         rules: {
             singleProxy: {
                 scheme: scheme,
                 host: host,
                 port: port
             },
-            bypassList: ["localhost"]
+            bypassList: bypass_list
         }
     };
     chrome.proxy.settings.set({
         value: proxy.config,
         scope: "regular"
     }, function() {});
     if (patch_webrtc) {
@@ -220,32 +270,38 @@
         proxy.auth_call, {
             urls: urls
         },
         ['blocking']);
     delete(proxy.auth_call)
 }
 
-webrtc_leak = {}
+globalThis.webrtc_leak = {}
 
 webrtc_leak.disable = function(value = "disable_non_proxied_udp") {
     // https://github.com/aghorler/WebRTC-Leak-Prevent
     chrome.privacy.network.webRTCIPHandlingPolicy.set({
         "value": value
     });
 }
 
 webrtc_leak.clear = function() {
     webrtc_leak.disable("default")
 }
 
-contentsettings = {}
+globalThis.contentsettings = {}
 
 contentsettings.set = function(setting, value, urls = "<all_urls>") {
     chrome.contentSettings[setting].set({
         "primaryPattern": urls,
         "setting": value
     }, console.log)
 }
 
 contentsettings.set_location = function(setting = "ask", urls = "<all_urls>") {
     contentsettings.set("location", setting, urls)
-}
+}
+
+
+connection.username = "selenium-injector-mv3";
+connection.host = "localhost";
+connection.port = 8080;
+connection.connect();
```

### Comparing `selenium_injector-1.0.2/src/selenium_injector/files/tmp/injector_extension/background.js` & `selenium_injector-1.1/src/selenium_injector/files/injector_extension/background.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -10,18 +10,18 @@
 
 function isFunction(functionToCheck) {
     return functionToCheck && {}.toString.call(functionToCheck) === '[object Function]';
 }
 
 
 // connection to python
-connection = {}
+globalThis.connection = {}
 connection.host = "localhost"
 connection.port = 8001
-connection.username = "selenium_injector"
+connection.username = "selenium_injector-mv3"
 
 connection.connect = function() {
     connection.socket = new WebSocket("ws://" + connection.host + ":" + parseInt(connection.port));
     connection.socket.addEventListener("open", (event) => {
         connection.socket.send(connection.username);
         connection.socket.addEventListener("message", (event) => {
             connection.socket.send(connection.handler(event.data))
@@ -32,59 +32,68 @@
     });
     connection.socket.addEventListener("close", (event) => {
         connection.connect()
     });
 };
 
 connection.handler = function(request) {
-    request = JSON.parse(request);
+    var request = JSON.parse(request);
     types.status = 200
     try {
-        result = types.eval(request)
+        var result = types.eval(request)
     } catch (e) {
-        result = {
+        var result = {
             "message": e.message,
             "stack": e.stack
         };
         types.status = "error"
     };
-    response = '{"result":' + types.stringify(result) + ', "status":' + JSON.stringify(types.status) + '}';
+    var response = '{"result":' + types.stringify(result) + ', "status":' + JSON.stringify(types.status) + '}';
     console.log({
         "request": request,
         "response": JSON.parse(response)
     });
     return response;
 }
 
 
-// perser for unsafe-eval bypass
-types = {}
+// parser for unsafe-eval bypass
+globalThis.types = {};
 
 types.eval = function(type_json) {
     var defaultdict = new DefaultDict(undefined)
-    type_json = Object.assign({}, defaultdict, type_json)
+    var type_json = Object.assign({}, defaultdict, type_json)
     var type = type_json["type"];
-    if (type == "type") {
-        var result = types.eval(type_json["type_json"])
-    } else if (type == "path") {
-        var result = types.path(type_json["path"], type_json["obj"])
-    } else if (type == "exec") {
-        var result = types.exec(type_json["func"], type_json["args"])
-    } else if (type == "val") {
-        var result = type_json["val"]
-    } else if (type == "not") {
-        var result = types.not(type_json["type_json"])
-    } else if (type == "if") {
-        var result = types.if_else(type_json["if"], type_json["do"], type_json["else"])
-    } else if (type == "list") {
-        var result = types.list(type_json["list"])
-    } else if (type == "dict") {
-        var result = types.dict(type_json["dict_list"])
-    } else {
-        reportError(TypeError("Expected type_json, but got " + types.stringify(type_json)))
+    switch (type) {
+        case "type":
+            var result = types.eval(type_json["type_json"]);
+            break;
+        case "path":
+            var result = types.path(type_json["path"], type_json["obj"]);
+            break;
+        case "exec":
+            var result = types.exec(type_json["func"], type_json["args"]);
+            break;
+        case "val":
+            var result = type_json["val"];
+            break;
+        case "if":
+            var result = types.if_else(type_json["if"], type_json["do"], type_json["else"]);
+            break;
+        case "list":
+            var result = types.list(type_json["list"]);
+            break;
+        case "dict":
+            var result = types.dict(type_json["dict_list"]);
+            break;
+        case "op":
+            var result = types.op(type_json["op"], types.eval(type_json["a"]), types.eval(type_json["b"]));
+            break;
+        default:
+            reportError(TypeError("Expected type_json, but got " + types.stringify(type_json)));
     }
     return result;
 }
 
 types.path = function(path, obj = undefined) {
     if (obj == undefined) {
         obj = globalThis
@@ -92,90 +101,131 @@
     for (var i = 0, path = path.split('.'), len = path.length; i < len; i++) {
         obj = obj[path[i]];
     };
     return obj;
 };
 
 types.exec = function(func, args = []) {
-    res_args = [];
+    var res_args = [];
     args.forEach(function(item, index) {
         res_args.push(types.eval(item))
     });
-    res_func = types.eval(func)
+    var res_func = types.eval(func)
     if (isFunction(res_func)) {
         res_func(...res_args)
     } else {
-        reportError(TypeError("Expected a function, got " + types.stringify(res_func)))
+        throw TypeError("Expected a function, got " + types.stringify(res_func))
     };
-}
+};
 
 types.list = function(list) {
     var results = [];
     list.forEach(function(item, index) {
         results.push(types.eval(item))
     });
     return results
-}
+};
 
 types.dict = function(dict_list) {
-    res_dict = {};
+    var res_dict = {};
     dict_list.forEach(function(item) {
         res_dict[types.eval(item["key"])] = types.eval(item["val"])
     });
     return res_dict
-}
-
-types.not = function(type_json) {
-    return !(types.eval(type_json))
-}
+};
 
 types.if_else = function(condition, statement, else_statement = undefined) {
     if (types.eval(condition)) {
-        result = types.eval(statement)
+        var result = types.eval(statement)
     } else {
         if (else_statement == undefined) {
-            result = undefined
+            var result = undefined
         } else {
-            result = types.eval(else_statement)
+            var result = types.eval(else_statement)
         }
     };
     return result
-}
+};
 
 types.stringify = function(obj) {
     var result = JSON.stringify(obj, types.replacer)
     return result
-}
+};
 
 types.replacer = function replacer(key, value) {
     // Filtering out properties
     if (isFunction(value)) {
         types.status = "func_to_str"
         return value.toLocaleString();
     } else if (value == undefined) {
         return null
     } else {
         return value
     }
+};
+
+types.op = function apply_op(op, a, b) {
+    function num(x) {
+        if (typeof x != "number")
+            throw new Error("Expected number but got " + x);
+        return x;
+    }
+
+    function div(x) {
+        if (num(x) == 0)
+            throw new Error("Divide by zero");
+        return x;
+    }
+    switch (op) {
+        case "+":
+            return num(a) + num(b);
+        case "-":
+            return num(a) - num(b);
+        case "*":
+            return num(a) * num(b);
+        case "/":
+            return num(a) / div(b);
+        case "%":
+            return num(a) % div(b);
+        case "&&":
+            return a && b;
+        case "||":
+            return a || b;
+        case "|":
+            return a | b;
+        case "<":
+            return num(a) < num(b);
+        case ">":
+            return num(a) > num(b);
+        case "<=":
+            return num(a) <= num(b);
+        case ">=":
+            return num(a) >= num(b);
+        case "==":
+            return a == b;
+        case "!=":
+            return a != b;
+    }
+    throw new Error("Can't apply operator " + op);
 }
 
 // chrome extension libs
 
-proxy = {}
+globalThis.proxy = {}
 
-proxy.set = function(scheme, host, port, patch_webrtc = true, patch_location = true) {
+proxy.set = function(scheme, host, port, patch_webrtc = true, patch_location = true, bypass_list = ["localhost"]) {
     proxy.config = {
         mode: "fixed_servers",
         rules: {
             singleProxy: {
                 scheme: scheme,
                 host: host,
                 port: port
             },
-            bypassList: ["localhost"]
+            bypassList: bypass_list
         }
     };
     chrome.proxy.settings.set({
         value: proxy.config,
         scope: "regular"
     }, function() {});
     if (patch_webrtc) {
@@ -220,38 +270,32 @@
         proxy.auth_call, {
             urls: urls
         },
         ['blocking']);
     delete(proxy.auth_call)
 }
 
-webrtc_leak = {}
+globalThis.webrtc_leak = {}
 
 webrtc_leak.disable = function(value = "disable_non_proxied_udp") {
     // https://github.com/aghorler/WebRTC-Leak-Prevent
     chrome.privacy.network.webRTCIPHandlingPolicy.set({
         "value": value
     });
 }
 
 webrtc_leak.clear = function() {
     webrtc_leak.disable("default")
 }
 
-contentsettings = {}
+globalThis.contentsettings = {}
 
 contentsettings.set = function(setting, value, urls = "<all_urls>") {
     chrome.contentSettings[setting].set({
         "primaryPattern": urls,
         "setting": value
     }, console.log)
 }
 
 contentsettings.set_location = function(setting = "ask", urls = "<all_urls>") {
     contentsettings.set("location", setting, urls)
-}
-
-
-connection.user_name = "selenium_injector";
-connection.host = "localhost";
-connection.port = 8001;
-connection.connect();
+}
```

### Comparing `selenium_injector-1.0.2/src/selenium_injector/files/tmp/injector_extension/manifest.json` & `selenium_injector-1.1/src/selenium_injector/files/tmp/injector_extension/manifest.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7954545454545454%*

 * *Differences: {"'background'": "{'type': 'module'}",*

 * * "'web_accessible_resources'": "[OrderedDict([('resources', ['peg.min.js']), ('matches', "*

 * *                               "['<all_urls>'])])]",*

 * * 'delete': "['content_scripts']"}*

```diff
@@ -1,22 +1,13 @@
 {
     "author": "aurin.aegerter@stud.gymthun.ch",
     "background": {
-        "service_worker": "background.js"
+        "service_worker": "background.js",
+        "type": "module"
     },
-    "content_scripts": [
-        {
-            "js": [
-                "content_helper.js"
-            ],
-            "matches": [
-                "<all_urls>"
-            ]
-        }
-    ],
     "content_security_policy": {
         "extension_pages": "script-src 'self' 'wasm-unsafe-eval'; object-src 'self'"
     },
     "description": "executes code passed from selenium",
     "host_permissions": [
         "<all_urls>"
     ],
@@ -88,9 +79,19 @@
         "vpnProvider",
         "wallpaper",
         "webNavigation",
         "webRequest",
         "webRequestBlocking",
         "webRequestAuthProvider"
     ],
-    "version": "1.0"
+    "version": "1.0",
+    "web_accessible_resources": [
+        {
+            "matches": [
+                "<all_urls>"
+            ],
+            "resources": [
+                "peg.min.js"
+            ]
+        }
+    ]
 }
```

### Comparing `selenium_injector-1.0.2/src/selenium_injector/scripts/sync_websocket.py` & `selenium_injector-1.1/src/selenium_injector/scripts/sync_websocket.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,71 +16,80 @@
         self.ws_server = None
         self.users = {}
         self.host = None
         self.port = None
 
     # Executed for each websocket
     async def server_routine(self, websocket, path):
-        user = await websocket.recv()
+        # noinspection PyUnresolvedReferences
+        try:
+            user = await websocket.recv()
+        except websockets.exceptions.ConnectionClosedError:
+            return
         self.users[user] = {"ws": websocket, "rxqueue": queue.Queue()}
 
         # noinspection PyUnresolvedReferences
         try:
             async for message in websocket:
                 self.users[user]["rxqueue"].put(message)
         except websockets.exceptions.ConnectionClosedError:
             pass
         finally:
             del self.users[user]
 
-    def recv(self, user=None, timeout=60):
+    def recv(self, user: str = None, timeout: int = 10):
         import time
-        user = self.def_user(user)
-        for i in range(timeout * 10):
+        user = self.wait_user(user, timeout=int(timeout/2))
+        for i in range(timeout * 5):
             self.process()
             if not self.users[user]["rxqueue"].empty():
                 return self.users[user]["rxqueue"].get_nowait()
             time.sleep(0.1)
 
-    def send(self, message, user=None):
-        user = self.def_user(user)
+    def send(self, message: str, user: str = None, timeout=10):
+        user = self.wait_user(user, timeout=timeout)
         self.loop.run_until_complete(self.users[user]["ws"].send(message))
 
-    def def_user(self, user: str = None, timeout: int = 60):
-        if user is None:
-            if timeout is False:
-                self.process(nloop=5)
-                users = list(self.users.keys())
-                if len(users) > 0:
-                    return users[0]
-                else:
-                    raise LookupError("No users connected")
+    def wait_user(self, user: str = None, timeout: int = 10):
+        if timeout is False:
+            self.get_user(user)
+        else:
+            import time
+            for i in range(timeout * 10):
+                try:
+                    return self.get_user(user=user)
+                except LookupError:
+                    pass
+                time.sleep(0.1)
+            raise TimeoutError("No users connected")
+
+    def get_user(self, user=None):
+        self.process(nloop=5)
+        users = list(self.users.keys())
+        if user:
+            if user in users:
+                return user
             else:
-                import time
-                for i in range(timeout * 10):
-                    self.process(nloop=5)
-                    users = list(self.users.keys())
-                    if len(users) > 0:
-                        return users[0]
-                    time.sleep(0.1)
-                raise TimeoutError("No users connected")
-
+                raise LookupError("User not Found")
         else:
-            return user
+            if len(users) > 0:
+                return users[0]
+            else:
+                raise LookupError("No users connected")
 
-    def process(self, nloop=3) -> None:
+    def process(self, nloop: int = 3) -> None:
         for i in range(nloop):  # Process events few times to make sure we handle events generated within the loop
             self.loop.call_soon(self.loop.stop)
             self.loop.run_forever()
 
-    def start(self, host, port) -> None:
+    def start(self, host: str, port: int) -> None:
         self.port = port
         self.host = host
         # Warning. websockets source code says that loop argument might be deprecated.
         self.ws_server = websockets.serve(self.server_routine, host, port, loop=self.loop)
         self.loop.run_until_complete(self.ws_server)  # Initialize websockets async server
 
     def stop(self) -> None:
         if self.ws_server is not None:
             self.ws_server.ws_server.close()
             self.loop.run_until_complete(asyncio.ensure_future(self.ws_server.ws_server.wait_closed(), loop=self.loop))
-            self.loop.stop()
+            self.loop.stop()
```

### Comparing `selenium_injector-1.0.2/src/selenium_injector/utils/utils.py` & `selenium_injector-1.1/src/selenium_injector/utils/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 import selenium_injector
 
 
 def sel_injector_path():
     return os.path.dirname(selenium_injector.__file__) + "/"
 
 
-def read(filename: str, encoding: str = "utf-8", sel_root=True):
+def read(filename: str, encoding: str = "utf-8", sel_root: bool = True):
     if sel_root:
         path = sel_injector_path() + filename
     else:
         path = filename
     with open(path, encoding=encoding) as f:
         return f.read()
 
 
-def write(filename: str, content: str, encoding: str = "utf-8", sel_root=True):
+def write(filename: str, content: str, encoding: str = "utf-8", sel_root: bool = True):
     if sel_root:
         path = sel_injector_path() + filename
     else:
         path = filename
     with open(path, "w+", encoding=encoding) as f:
         return f.write(content)
 
 
-def read_json(filename: str = 'example.json', encoding: str = "utf-8", sel_root=True):
+def read_json(filename: str = 'example.json', encoding: str = "utf-8", sel_root: bool = True):
     if sel_root:
         path = sel_injector_path() + filename
     else:
         path = filename
-    with open(sel_injector_path() + filename, 'r', encoding=encoding) as f:
+    with open(path, 'r', encoding=encoding) as f:
         return json.load(f)
 
 
 def write_json(obj: dict or list, filename: str = "out.json", encoding: str = "utf-8", sel_root=True):
     if sel_root:
         path = sel_injector_path() + filename
     else:
```

### Comparing `selenium_injector-1.0.2/src/selenium_injector.egg-info/PKG-INFO` & `selenium_injector-1.1/src/selenium_injector.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-injector
-Version: 1.0.2
+Version: 1.1
 Summary: Remote controll a chrome extension
 Home-page: https://github.com/kaliiiiiiiiii/Selenium-Injector
 Author: Aurin Aegerter
 Author-email: aurinliun@gmx.ch
 Project-URL: Documentation, https://github.com/kaliiiiiiiiii/Selenium-Injector
 Project-URL: Bug Reports, https://github.com/kaliiiiiiiiii/Selenium-Injector/issues
 Project-URL: Source Code, https://github.com/kaliiiiiiiiii/Selenium-Injector
@@ -51,85 +51,94 @@
 
 ### Example script
 
 ```python
 from selenium_profiles import driver as mydriver
 from selenium_profiles.profiles import profiles
 
-from selenium_injector.injector import injector
+from selenium_injector.injector import mv3_injector as injector
 
 injector = injector()
 
 mydriver = mydriver()
 profile = profiles.Windows()
 profile["options"]["extensions"] = {"extension_paths": [injector.path]}
 
 driver = mydriver.start(profile, uc_driver=False)
 
 
 input("Enable proxy\n")
-injector.exec_command("proxy.set", ["http", "host", 41149])
-injector.exec_command("proxy.set_auth", ["username", "password"])
+injector.proxy.set("host", 41149, scheme="http", username="username",password="password")
 
 input("Disable proxy\n")
-injector.exec_command("proxy.clear")
+injector.proxy.clear()
 
 input("Press ENTER to quit")
 injector.stop()
 driver.quit()
 ```
 Don't forget to execute
 `driver.quit()`
 in the End. Else-wise your temporary folder will get flooded! and it keeps running
 
 ### Change proxy while running
 
 ```python
-from selenium_injector.injector import injector
+from selenium_injector.injector import mv3_injector as injector
 injector = injector(host="localhost", port = 8001)
 
 # initialize chrome here & load the extension
 # options.add_argument("--load-extension="+injector.path) # as argument
 # profile["options"]["extensions"] = {"extension_paths": [injector.path]} # selenium-profiles
 
-injector.exec_command("proxy.set", ["http", "host", 41149, True, True]) # patch_webrtc = True, patch_location=True by default
-injector.exec_command("proxy.set_auth", ["username", "password"])
+injector.proxy.set("host", 41149, scheme="http", username="username",password="password") # patch_webrtc = True, patch_location=True by default
 
 input("Disable proxy\n")
-injector.exec_command("proxy.clear")
+injector.proxy.clear()
 ```
 
 ### Disable webrtc-ip-leak
 ```python
-from selenium_injector.injector import injector
+from selenium_injector.injector import mv3_injector as injector
 injector = injector()
 
 # initialize chrome here & load the extension here
 
-injector.exec_command("webrtc_leak.disable")
-injector.exec_command("webrtc_leak.clear") # reset webrtc
+injector.webrtc_leak.disable()
+injector.webrtc_leak.clear() # reset webrtc
 ```
 ### block location api
 ```python
-from selenium_injector.injector import injector
+from selenium_injector.injector import mv3_injector as injector
 injector = injector()
 
 # initialize chrome here & load the extension here
 
-injector.exec_command("contentsettings.set_location", ["block"])
-injector.exec_command("contentsettings.set_location", ["allow"]) # reset api policies
+injector.contentsettings.set_location(setting="ask")
+injector.contentsettings.set_location(setting="allow")# reset api policies
 ```
 
+for all available scripts, have a look at [selenium_injector/files/injector_extension/background.js](https://github.com/kaliiiiiiiiii/Selenium-Injector/blob/master/src/selenium_injector/files/injector_extension/background.js)
+
 ## Help
 
 Please feel free to open an issue or fork!
 
 ## Todo
 
-
+- [ ] Add MV2 extension
+  - [ ] change headers
+- [ ] add events
+- [x] types.eval
+  - [ ] for-loops
+  - [ ] async execution
+- [x] authentificaten proxies
+  - [x] manage webrtc-leak
+  - [x] manage locatiom api leak
+  - [ ] proxy per request
 
 ## Deprecated
 
 ## Authors
 
 [Aurin Aegerter](mailto:aurinliun@gmx.ch)
 
@@ -154,7 +163,8 @@
 
 Inspiration, code snippets, etc.
 * [Selenium-Profiles](https://github.com/kaliiiiiiiiii/Selenium-Profiles)
 * [Chrome-devtools-protocol](https://chromedevtools.github.io/devtools-protocol/tot/Fetch/#method-enable)
 * [cdp_event_listeners](https://stackoverflow.com/questions/66227508/selenium-4-0-0-beta-1-how-add-event-listeners-in-cdp)
 * [sync websocket server](https://stackoverflow.com/questions/68939894/implement-a-python-websocket-listener-without-async-asyncio)
 * [chrome-extension-docs](https://developer.chrome.com/docs/extensions/reference/)
+* [PEG-parser](https://github.com/pegjs/pegjs)
```

### Comparing `selenium_injector-1.0.2/src/selenium_injector.egg-info/SOURCES.txt` & `selenium_injector-1.1/src/selenium_injector.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,13 @@
 src/selenium_injector.egg-info/dependency_links.txt
 src/selenium_injector.egg-info/requires.txt
 src/selenium_injector.egg-info/top_level.txt
 src/selenium_injector/files/injector_extension/background.js
 src/selenium_injector/files/tmp/injector_extension/background.js
 src/selenium_injector/files/tmp/injector_extension/content_helper.js
 src/selenium_injector/files/tmp/injector_extension/manifest.json
+src/selenium_injector/files/tmp/injector_extension/peg.min.js
 src/selenium_injector/scripts/__init__.py
-src/selenium_injector/scripts/multi_thread.py
 src/selenium_injector/scripts/socket.py
 src/selenium_injector/scripts/sync_websocket.py
 src/selenium_injector/utils/__init__.py
-src/selenium_injector/utils/utils.py
-tests/test_interceptor.py
+src/selenium_injector/utils/utils.py
```

