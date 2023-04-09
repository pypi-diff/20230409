# Comparing `tmp/mycroft_dinkum_listener-0.0.0a3-py3-none-any.whl.zip` & `tmp/mycroft_dinkum_listener-0.0.1a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1655 bytes, number of entries: 5
--rw-r--r--  2.0 unx      522 b- defN 23-Apr-09 00:31 mycroft_dinkum_listener-0.0.0a3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 00:31 mycroft_dinkum_listener-0.0.0a3.dist-info/WHEEL
--rw-r--r--  2.0 unx       83 b- defN 23-Apr-09 00:31 mycroft_dinkum_listener-0.0.0a3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-09 00:31 mycroft_dinkum_listener-0.0.0a3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      481 b- defN 23-Apr-09 00:31 mycroft_dinkum_listener-0.0.0a3.dist-info/RECORD
-5 files, 1179 bytes uncompressed, 737 bytes compressed:  37.5%
+Zip file size: 1652 bytes, number of entries: 5
+-rw-r--r--  2.0 unx      534 b- defN 23-Apr-09 05:18 mycroft_dinkum_listener-0.0.1a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 05:18 mycroft_dinkum_listener-0.0.1a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       83 b- defN 23-Apr-09 05:18 mycroft_dinkum_listener-0.0.1a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-09 05:18 mycroft_dinkum_listener-0.0.1a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      481 b- defN 23-Apr-09 05:18 mycroft_dinkum_listener-0.0.1a1.dist-info/RECORD
+5 files, 1191 bytes uncompressed, 734 bytes compressed:  38.4%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: mycroft_dinkum_listener-0.0.0a3.dist-info/METADATA
+Filename: mycroft_dinkum_listener-0.0.1a1.dist-info/METADATA
 Comment: 
 
-Filename: mycroft_dinkum_listener-0.0.0a3.dist-info/WHEEL
+Filename: mycroft_dinkum_listener-0.0.1a1.dist-info/WHEEL
 Comment: 
 
-Filename: mycroft_dinkum_listener-0.0.0a3.dist-info/entry_points.txt
+Filename: mycroft_dinkum_listener-0.0.1a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: mycroft_dinkum_listener-0.0.0a3.dist-info/top_level.txt
+Filename: mycroft_dinkum_listener-0.0.1a1.dist-info/top_level.txt
 Comment: 
 
-Filename: mycroft_dinkum_listener-0.0.0a3.dist-info/RECORD
+Filename: mycroft_dinkum_listener-0.0.1a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mycroft_dinkum_listener-0.0.0a3.dist-info/METADATA` & `mycroft_dinkum_listener-0.0.1a1.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mycroft-dinkum-listener
-Version: 0.0.0a3
+Version: 0.0.1a1
 Summary: ovos-core listener daemon client
 Home-page: https://github.com/OpenVoiceOS/mycroft-dinkum-listener
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: numpy
-Requires-Dist: sonopy (~=0.1.0)
+Requires-Dist: ovos-plugin-manager
+Requires-Dist: ovos-utils
+Requires-Dist: ovos-bus-client
 Requires-Dist: sdnotify
-Requires-Dist: onnxruntime
 
 UNKNOWN
```

