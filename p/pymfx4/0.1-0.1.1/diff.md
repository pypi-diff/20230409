# Comparing `tmp/pymfx4-0.1.tar.gz` & `tmp/pymfx4-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymfx4-0.1.tar", last modified: Sun Apr  9 15:27:00 2023, max compression
+gzip compressed data, was "pymfx4-0.1.1.tar", last modified: Sun Apr  9 15:54:36 2023, max compression
```

## Comparing `pymfx4-0.1.tar` & `pymfx4-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 15:27:00.681094 pymfx4-0.1/
--rw-rw-rw-   0        0        0     1063 2023-04-09 14:40:28.000000 pymfx4-0.1/LICENSE
--rw-rw-rw-   0        0        0       16 2019-07-20 17:06:16.000000 pymfx4-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1998 2023-04-09 15:27:00.680095 pymfx4-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-04-09 14:49:57.000000 pymfx4-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 15:27:00.658096 pymfx4-0.1/pymfx4/
--rw-rw-rw-   0        0        0      468 2023-03-23 16:03:35.000000 pymfx4-0.1/pymfx4/__init__.py
--rw-rw-rw-   0        0        0    12085 2023-03-23 15:36:47.000000 pymfx4-0.1/pymfx4/mfconnection.py
--rw-rw-rw-   0        0        0     9523 2023-03-23 15:38:08.000000 pymfx4-0.1/pymfx4/mfdatastorage.py
--rw-rw-rw-   0        0        0     2157 2023-03-17 10:59:56.000000 pymfx4-0.1/pymfx4/mfenums.py
--rw-rw-rw-   0        0        0     1109 2023-03-17 11:00:43.000000 pymfx4-0.1/pymfx4/mffullindex.py
--rw-rw-rw-   0        0        0     3112 2023-03-17 11:02:47.000000 pymfx4-0.1/pymfx4/mfkeyboard.py
--rw-rw-rw-   0        0        0     5981 2023-03-23 15:37:06.000000 pymfx4-0.1/pymfx4/mfparameters.py
--rw-rw-rw-   0        0        0    20681 2023-03-24 10:53:22.000000 pymfx4-0.1/pymfx4/mfx4ARMadillo.py
--rw-rw-rw-   0        0        0    26880 2023-03-17 11:19:09.000000 pymfx4-0.1/pymfx4/mfx4ARMadilloConfigurationDefinitions.py
--rw-rw-rw-   0        0        0    39268 2023-03-30 11:53:27.000000 pymfx4-0.1/pymfx4/mfx4ARMadilloEnums.py
--rw-rw-rw-   0        0        0    12978 2023-03-23 15:38:08.000000 pymfx4-0.1/pymfx4/mfx4device.py
--rw-rw-rw-   0        0        0     1475 2023-03-17 09:33:54.000000 pymfx4-0.1/pymfx4/mfx4driver.py
--rw-rw-rw-   0        0        0  2358847 2023-03-17 11:05:22.000000 pymfx4-0.1/pymfx4/mfxdd.py
-drwxrwxrwx   0        0        0        0 2023-04-09 15:27:00.676096 pymfx4-0.1/pymfx4.egg-info/
--rw-rw-rw-   0        0        0     1998 2023-04-09 15:27:00.000000 pymfx4-0.1/pymfx4.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      554 2023-04-09 15:27:00.000000 pymfx4-0.1/pymfx4.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 15:27:00.000000 pymfx4-0.1/pymfx4.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-09 15:27:00.000000 pymfx4-0.1/pymfx4.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-09 15:27:00.000000 pymfx4-0.1/pymfx4.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      570 2023-04-09 14:51:00.000000 pymfx4-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-09 15:27:00.681094 pymfx4-0.1/setup.cfg
--rw-rw-rw-   0        0        0      637 2023-04-09 15:26:59.000000 pymfx4-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 15:27:00.679095 pymfx4-0.1/tests/
--rw-rw-rw-   0        0        0      249 2023-04-09 14:42:30.000000 pymfx4-0.1/tests/test_advanced.py
--rw-rw-rw-   0        0        0      283 2023-04-09 14:42:43.000000 pymfx4-0.1/tests/test_basic.py
+drwxrwxrwx   0        0        0        0 2023-04-09 15:54:36.704392 pymfx4-0.1.1/
+-rw-rw-rw-   0        0        0     1063 2023-04-09 14:40:28.000000 pymfx4-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       16 2019-07-20 17:06:16.000000 pymfx4-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2000 2023-04-09 15:54:36.703394 pymfx4-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-04-09 14:49:57.000000 pymfx4-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 15:54:36.681393 pymfx4-0.1.1/pymfx4/
+-rw-rw-rw-   0        0        0      468 2023-03-23 16:03:35.000000 pymfx4-0.1.1/pymfx4/__init__.py
+-rw-rw-rw-   0        0        0    12085 2023-03-23 15:36:47.000000 pymfx4-0.1.1/pymfx4/mfconnection.py
+-rw-rw-rw-   0        0        0     9523 2023-03-23 15:38:08.000000 pymfx4-0.1.1/pymfx4/mfdatastorage.py
+-rw-rw-rw-   0        0        0     2157 2023-03-17 10:59:56.000000 pymfx4-0.1.1/pymfx4/mfenums.py
+-rw-rw-rw-   0        0        0     1109 2023-03-17 11:00:43.000000 pymfx4-0.1.1/pymfx4/mffullindex.py
+-rw-rw-rw-   0        0        0     3112 2023-03-17 11:02:47.000000 pymfx4-0.1.1/pymfx4/mfkeyboard.py
+-rw-rw-rw-   0        0        0     5981 2023-03-23 15:37:06.000000 pymfx4-0.1.1/pymfx4/mfparameters.py
+-rw-rw-rw-   0        0        0    20681 2023-03-24 10:53:22.000000 pymfx4-0.1.1/pymfx4/mfx4ARMadillo.py
+-rw-rw-rw-   0        0        0    26880 2023-03-17 11:19:09.000000 pymfx4-0.1.1/pymfx4/mfx4ARMadilloConfigurationDefinitions.py
+-rw-rw-rw-   0        0        0    39268 2023-03-30 11:53:27.000000 pymfx4-0.1.1/pymfx4/mfx4ARMadilloEnums.py
+-rw-rw-rw-   0        0        0    13262 2023-04-09 15:44:41.000000 pymfx4-0.1.1/pymfx4/mfx4device.py
+-rw-rw-rw-   0        0        0     1475 2023-03-17 09:33:54.000000 pymfx4-0.1.1/pymfx4/mfx4driver.py
+-rw-rw-rw-   0        0        0  2358847 2023-03-17 11:05:22.000000 pymfx4-0.1.1/pymfx4/mfxdd.py
+drwxrwxrwx   0        0        0        0 2023-04-09 15:54:36.700392 pymfx4-0.1.1/pymfx4.egg-info/
+-rw-rw-rw-   0        0        0     2000 2023-04-09 15:54:36.000000 pymfx4-0.1.1/pymfx4.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-04-09 15:54:36.000000 pymfx4-0.1.1/pymfx4.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 15:54:36.000000 pymfx4-0.1.1/pymfx4.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-09 15:54:36.000000 pymfx4-0.1.1/pymfx4.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-09 15:54:36.000000 pymfx4-0.1.1/pymfx4.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      572 2023-04-09 15:54:08.000000 pymfx4-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-09 15:54:36.704392 pymfx4-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      637 2023-04-09 15:53:02.000000 pymfx4-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 15:54:36.702392 pymfx4-0.1.1/tests/
+-rw-rw-rw-   0        0        0      249 2023-04-09 14:42:30.000000 pymfx4-0.1.1/tests/test_advanced.py
+-rw-rw-rw-   0        0        0      283 2023-04-09 14:42:43.000000 pymfx4-0.1.1/tests/test_basic.py
```

### Comparing `pymfx4-0.1/LICENSE` & `pymfx4-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymfx4-0.1/PKG-INFO` & `pymfx4-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymfx4
-Version: 0.1
+Version: 0.1.1
 Summary: Access MFX_4 devices.
 Home-page: https://www.m-f.tech/
 Author: Alexander Angold
 Author-email: Alexander Angold <pymfx4@infodb.eu>
 License: MIT License
         
         Copyright (c) 2023 AAngold
```

### Comparing `pymfx4-0.1/pymfx4/mfconnection.py` & `pymfx4-0.1.1/pymfx4/mfconnection.py`

 * *Files identical despite different names*

### Comparing `pymfx4-0.1/pymfx4/mfdatastorage.py` & `pymfx4-0.1.1/pymfx4/mfdatastorage.py`

 * *Files identical despite different names*

### Comparing `pymfx4-0.1/pymfx4/mfenums.py` & `pymfx4-0.1.1/pymfx4/mfenums.py`

 * *Files identical despite different names*

### Comparing `pymfx4-0.1/pymfx4/mffullindex.py` & `pymfx4-0.1.1/pymfx4/mffullindex.py`

 * *Files identical despite different names*

### Comparing `pymfx4-0.1/pymfx4/mfkeyboard.py` & `pymfx4-0.1.1/pymfx4/mfkeyboard.py`

 * *Files identical despite different names*

### Comparing `pymfx4-0.1/pymfx4/mfparameters.py` & `pymfx4-0.1.1/pymfx4/mfparameters.py`

 * *Files identical despite different names*

### Comparing `pymfx4-0.1/pymfx4/mfx4ARMadillo.py` & `pymfx4-0.1.1/pymfx4/mfx4ARMadillo.py`

 * *Files identical despite different names*

### Comparing `pymfx4-0.1/pymfx4/mfx4ARMadilloConfigurationDefinitions.py` & `pymfx4-0.1.1/pymfx4/mfx4ARMadilloConfigurationDefinitions.py`

 * *Files identical despite different names*

### Comparing `pymfx4-0.1/pymfx4/mfx4ARMadilloEnums.py` & `pymfx4-0.1.1/pymfx4/mfx4ARMadilloEnums.py`

 * *Files identical despite different names*

### Comparing `pymfx4-0.1/pymfx4/mfx4device.py` & `pymfx4-0.1.1/pymfx4/mfx4device.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     IxManufacturerSoftwareVersion = mff.FullIndex(0, 0x100A, 0x00)
     IxManufacturerSoftwareDate = mff.FullIndex(0, 0x100A, 0x01)
     IxManufacturerSoftwareTime = mff.FullIndex(0, 0x100A, 0x02)
 
     IxStoreParameterSaveAll = mff.FullIndex(0, 0x1010, 0x01)
     IxRestoreDefaultParametersIx = mff.FullIndex(0, 0x1011, 3)
 
+    IxAliveTime = mff.FullIndex(0, 0x200B, 14)
+
     # device soft reset
     DEVICE_REBOOT = 0x64616F6F
     DEVICE_SAVE_ALL_PARAMETERS = 0x65766173
 
     def __init__(self, NodeId):
         self._Node = NodeId
         ds.storage.AddGenericDevice(NodeId)
@@ -109,14 +111,20 @@
         ds.storage.Set(FI.Node(self.TheNode()), Value)
 
     def Get(self, FI):
         FI = FI.Node(self.TheNode())
         ds.storage.Get(FI)
         time.sleep(0.8)
         return ds.storage.GetNative(FI)
+    
+    def SetNotification(self, FI, Value, Func):
+        ds.storage.SetNotification(FI.Node(self.TheNode()), Value, Func)
+
+    def RemoveNotification(self, FI):
+        ds.storage.RemoveNotification(FI.Node(self.TheNode()))
 
     def DeployAndCheckEntrywise(self, package, iter=4):
         if isinstance(package, mfp.mfparameters):
             for i in range(iter):
                 if mfp.mfParameterManager.DeployAndCheckEntrywise(package, self):
                     return True
                 mfl.info("Check failed! Trying again.")
```

### Comparing `pymfx4-0.1/pymfx4/mfx4driver.py` & `pymfx4-0.1.1/pymfx4/mfx4driver.py`

 * *Files identical despite different names*

### Comparing `pymfx4-0.1/pymfx4/mfxdd.py` & `pymfx4-0.1.1/pymfx4/mfxdd.py`

 * *Files identical despite different names*

### Comparing `pymfx4-0.1/pymfx4.egg-info/PKG-INFO` & `pymfx4-0.1.1/pymfx4.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymfx4
-Version: 0.1
+Version: 0.1.1
 Summary: Access MFX_4 devices.
 Home-page: https://www.m-f.tech/
 Author: Alexander Angold
 Author-email: Alexander Angold <pymfx4@infodb.eu>
 License: MIT License
         
         Copyright (c) 2023 AAngold
```

### Comparing `pymfx4-0.1/pymfx4.egg-info/SOURCES.txt` & `pymfx4-0.1.1/pymfx4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymfx4-0.1/pyproject.toml` & `pymfx4-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pymfx4"
-version = "0.1"
+version = "0.1.1"
 authors = [
   { name="Alexander Angold", email="pymfx4@infodb.eu" },
 ]
 description = "Access MFX_4 devices."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pymfx4-0.1/setup.py` & `pymfx4-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = f.read()
 
 with open('LICENSE') as f:
     license = f.read()
 
 setup(
     name='pymfx4',
-    version='0.1.0',
+    version='0.1.1',
     description='Control of MFX_4 Series Devices',
     long_description=readme,
     author='Alexander Angold',
     author_email='pymfx4@infodb.eu',
     url='https://www.m-f.tech/',
     license=license,
     packages=find_packages(exclude=('tests', 'docs')),
```

