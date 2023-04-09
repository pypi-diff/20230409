# Comparing `tmp/pychlorinator-0.2.2.tar.gz` & `tmp/pychlorinator-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychlorinator-0.2.2.tar", max compression
+gzip compressed data, was "pychlorinator-0.2.3.tar", max compression
```

## Comparing `pychlorinator-0.2.2.tar` & `pychlorinator-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1078 2023-03-16 09:28:44.460144 pychlorinator-0.2.2/LICENSE
--rw-r--r--   0        0        0        0 2023-03-16 09:00:19.424705 pychlorinator-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-03-16 09:00:19.424641 pychlorinator-0.2.2/pychlorinator/__init__.py
--rw-r--r--   0        0        0     6149 2023-03-28 21:02:26.233399 pychlorinator-0.2.2/pychlorinator/chlorinator.py
--rw-r--r--   0        0        0    11337 2023-03-30 01:57:58.336733 pychlorinator-0.2.2/pychlorinator/chlorinator_parsers.py
--rw-r--r--   0        0        0      538 2023-03-30 23:19:12.466123 pychlorinator-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 pychlorinator-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-03-16 09:28:44.460144 pychlorinator-0.2.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-03-16 09:00:19.424705 pychlorinator-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-03-16 09:00:19.424641 pychlorinator-0.2.3/pychlorinator/__init__.py
+-rw-r--r--   0        0        0     6151 2023-04-09 01:45:46.868754 pychlorinator-0.2.3/pychlorinator/chlorinator.py
+-rw-r--r--   0        0        0    11337 2023-03-30 01:57:58.336733 pychlorinator-0.2.3/pychlorinator/chlorinator_parsers.py
+-rw-r--r--   0        0        0      538 2023-04-09 01:46:42.786174 pychlorinator-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 pychlorinator-0.2.3/PKG-INFO
```

### Comparing `pychlorinator-0.2.2/LICENSE` & `pychlorinator-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pychlorinator-0.2.2/pychlorinator/chlorinator.py` & `pychlorinator-0.2.3/pychlorinator/chlorinator.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         self._ble_device = ble_device
         self._access_code = access_code
         self._session_key = None
         self._result: dict[str, Any] = None
 
     async def async_write_action(self, action: ChlorinatorActions):
         """Connect to the Chlorinator and write an action command to it"""
-        async with BleakClient(self._ble_device, timeout=3) as client:
+        async with BleakClient(self._ble_device, timeout=10) as client:
             self._session_key = await client.read_gatt_char(UUID_SLAVE_SESSION_KEY)
             _LOGGER.info(f"got session key {self._session_key.hex()}")
 
             mac = encrypt_mac_key(self._session_key, bytes(self._access_code, "utf_8"))
             _LOGGER.info(f"mac key to write {mac}")
             await client.write_gatt_char(UUID_MASTER_AUTHENTICATION, mac)
 
@@ -129,15 +129,15 @@
             UUID_CHLORINATOR_SETUP: ChlorinatorSetup,
             UUID_CHLORINATOR_CAPABILITIES: ChlorinatorCapabilities,
             UUID_CHLORINATOR_TIMERS: ChlorinatorTimers,
             UUID_CHLORINATOR_STATISTICS: ChlorinatorStatistics,
             UUID_CHLORINATOR_SETTINGS: ChlorinatorSettings,
         }
 
-        async with BleakClient(self._ble_device, timeout=3) as client:
+        async with BleakClient(self._ble_device, timeout=10) as client:
             self._session_key = await client.read_gatt_char(UUID_SLAVE_SESSION_KEY)
             _LOGGER.info(f"got session key {self._session_key.hex()}")
 
             mac = encrypt_mac_key(self._session_key, bytes(self._access_code, "utf_8"))
             _LOGGER.info(f"mac key to write {mac.hex()}")
             await client.write_gatt_char(UUID_MASTER_AUTHENTICATION, mac)
```

### Comparing `pychlorinator-0.2.2/pychlorinator/chlorinator_parsers.py` & `pychlorinator-0.2.3/pychlorinator/chlorinator_parsers.py`

 * *Files identical despite different names*

### Comparing `pychlorinator-0.2.2/pyproject.toml` & `pychlorinator-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pychlorinator"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["pbutterworth <3683210+pbutterworth@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/pbutterworth/pychlorinator"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pychlorinator-0.2.2/PKG-INFO` & `pychlorinator-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychlorinator
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Home-page: https://github.com/pbutterworth/pychlorinator
 Author: pbutterworth
 Author-email: 3683210+pbutterworth@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

