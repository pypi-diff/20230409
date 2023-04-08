# Comparing `tmp/hubitatcontrol-1.1.2.tar.gz` & `tmp/hubitatcontrol-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubitatcontrol-1.1.2.tar", max compression
+gzip compressed data, was "hubitatcontrol-2.0.0.tar", max compression
```

## Comparing `hubitatcontrol-1.1.2.tar` & `hubitatcontrol-2.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-03-12 19:21:22.061753 hubitatcontrol-1.1.2/LICENSE
--rw-r--r--   0        0        0     3378 2023-03-31 06:10:13.391655 hubitatcontrol-1.1.2/README.md
--rw-r--r--   0        0        0     1426 2023-03-30 01:32:16.534352 hubitatcontrol-1.1.2/hubitatcontrol/__init__.py
--rw-r--r--   0        0        0     1740 2023-03-31 06:28:02.095021 hubitatcontrol-1.1.2/hubitatcontrol/__main__.py
--rw-r--r--   0        0        0     1060 2023-03-30 01:32:16.534352 hubitatcontrol-1.1.2/hubitatcontrol/generic.py
--rw-r--r--   0        0        0     2764 2023-03-30 01:32:16.534352 hubitatcontrol-1.1.2/hubitatcontrol/hub.py
--rw-r--r--   0        0        0     2774 2023-03-30 01:32:16.534352 hubitatcontrol-1.1.2/hubitatcontrol/lights.py
--rw-r--r--   0        0        0      336 2023-03-30 01:32:16.534352 hubitatcontrol-1.1.2/hubitatcontrol/sensors.py
--rw-r--r--   0        0        0     2394 2023-03-31 06:24:39.823143 hubitatcontrol-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     4217 1970-01-01 00:00:00.000000 hubitatcontrol-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-03-12 19:21:22.061753 hubitatcontrol-2.0.0/LICENSE
+-rw-r--r--   0        0        0     6247 2023-04-08 21:56:56.885073 hubitatcontrol-2.0.0/README.md
+-rw-r--r--   0        0        0     1483 2023-04-08 21:56:56.889073 hubitatcontrol-2.0.0/hubitatcontrol/__init__.py
+-rw-r--r--   0        0        0     3765 2023-04-08 21:56:56.889073 hubitatcontrol-2.0.0/hubitatcontrol/__main__.py
+-rw-r--r--   0        0        0     1060 2023-03-30 01:32:16.534352 hubitatcontrol-2.0.0/hubitatcontrol/generic.py
+-rw-r--r--   0        0        0     2902 2023-04-08 21:56:56.889073 hubitatcontrol-2.0.0/hubitatcontrol/hub.py
+-rw-r--r--   0        0        0     2774 2023-03-30 01:32:16.534352 hubitatcontrol-2.0.0/hubitatcontrol/lights.py
+-rw-r--r--   0        0        0      336 2023-03-30 01:32:16.534352 hubitatcontrol-2.0.0/hubitatcontrol/sensors.py
+-rw-r--r--   0        0        0     2415 2023-04-08 21:57:32.752590 hubitatcontrol-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7129 1970-01-01 00:00:00.000000 hubitatcontrol-2.0.0/PKG-INFO
```

### Comparing `hubitatcontrol-1.1.2/LICENSE` & `hubitatcontrol-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-1.1.2/hubitatcontrol/__init__.py` & `hubitatcontrol-2.0.0/hubitatcontrol/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 
 
 def get_hub(host, token, app_id, cloud_token=None) -> Hub:
     return Hub(host=host, token=token, app_id=app_id, cloud_token=cloud_token)
 
 
 def lookup_device(hub_in, device_lookup):
+    """
+    Takes device NAME, not ID for lookup
+    """
     d = hub_in.get_device(device_lookup)
     if d is None:
         raise Exception("Device Not Found")
     if "ColorControl" in d["capabilities"] and "ColorMode" in d["capabilities"]:
         return hubitatcontrol.lights.RGBWBulb(device_from_hub=d, hub=hub_in)
     if "ColorTemperature" in d["capabilities"]:
         return hubitatcontrol.lights.ColorTempBulb(device_from_hub=d, hub=hub_in)
```

### Comparing `hubitatcontrol-1.1.2/hubitatcontrol/generic.py` & `hubitatcontrol-2.0.0/hubitatcontrol/generic.py`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-1.1.2/hubitatcontrol/hub.py` & `hubitatcontrol-2.0.0/hubitatcontrol/hub.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,19 @@
         return r.json()
 
     def get_device(self, name: str):
         for i in self.devices:
             if i["label"] == name:
                 return i
 
+    def get_device_id(self, dev_id: int):
+        for i in self.devices:
+            if i["id"] == str(dev_id):
+                return i
+
 
 class Device:
     def __init__(self, hub: Hub, device_from_hub: dict):
         self.token = hub.token
         self.base_url_prefix = hub.base_url_prefix
         self.name = device_from_hub["name"]
         self.label = device_from_hub["label"]
```

### Comparing `hubitatcontrol-1.1.2/hubitatcontrol/lights.py` & `hubitatcontrol-2.0.0/hubitatcontrol/lights.py`

 * *Files identical despite different names*

### Comparing `hubitatcontrol-1.1.2/pyproject.toml` & `hubitatcontrol-2.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hubitatcontrol"
-version = "1.1.2"
+version = "2.0.0"
 description = "Hubitat Maker API Interface"
 authors = ["Jesse Schoepfer <jelloeater@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/Jelloeater/hubitatcontrol"
 keywords = ["hubitat", "makerapi","requests"]
 classifiers = ["Development Status :: 5 - Production/Stable",
@@ -19,14 +19,15 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "*"
 typer = "*"
 prettytable = "*"
+keyring = "^23.13.1"
 
 [tool.pytest.ini_options]
 pythonpath = ["."]
 testpaths = "test/"
 log_cli = true
 log_cli_level = "DEBUG"
 log_cli_format = "[%(asctime)s] [%(levelname)8s] --- %(message)s (%(filename)s:%(funcName)s():%(lineno)s)"
```

