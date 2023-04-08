# Comparing `tmp/spectrometer_reading_plugin-0.2.0-py3-none-any.whl.zip` & `tmp/spectrometer_reading_plugin-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,12 @@
-Zip file size: 6278 bytes, number of entries: 11
--rw-r--r--  2.0 unx     5677 b- defN 22-Nov-02 00:55 spectrometer_reading_plugin/__init__.py
+Zip file size: 5987 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     5729 b- defN 23-Mar-24 12:29 spectrometer_reading_plugin/__init__.py
 -rw-r--r--  2.0 unx      162 b- defN 22-Nov-02 00:54 spectrometer_reading_plugin/additional_config.ini
 -rw-r--r--  2.0 unx      257 b- defN 22-Oct-11 16:21 spectrometer_reading_plugin/additional_sql.sql
 -rw-r--r--  2.0 unx      231 b- defN 22-Oct-07 17:24 spectrometer_reading_plugin/ui/contrib/jobs/spectrometer_reading.yaml
--rw-r--r--  2.0 unx      231 b- defN 22-Oct-07 17:24 ui/contrib/jobs/spectrometer_reading.yaml
--rw-r--r--  2.0 unx     1049 b- defN 22-Nov-02 00:56 spectrometer_reading_plugin-0.2.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1854 b- defN 22-Nov-02 00:56 spectrometer_reading_plugin-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-02 00:56 spectrometer_reading_plugin-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       79 b- defN 22-Nov-02 00:56 spectrometer_reading_plugin-0.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       28 b- defN 22-Nov-02 00:56 spectrometer_reading_plugin-0.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1130 b- defN 22-Nov-02 00:56 spectrometer_reading_plugin-0.2.0.dist-info/RECORD
-11 files, 10790 bytes uncompressed, 4286 bytes compressed:  60.3%
+-rw-r--r--  2.0 unx     1049 b- defN 23-Apr-08 23:52 spectrometer_reading_plugin-0.2.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1854 b- defN 23-Apr-08 23:52 spectrometer_reading_plugin-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-08 23:52 spectrometer_reading_plugin-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       79 b- defN 23-Apr-08 23:52 spectrometer_reading_plugin-0.2.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       28 b- defN 23-Apr-08 23:52 spectrometer_reading_plugin-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1033 b- defN 23-Apr-08 23:52 spectrometer_reading_plugin-0.2.1.dist-info/RECORD
+10 files, 10514 bytes uncompressed, 4153 bytes compressed:  60.5%
```

## zipnote {}

```diff
@@ -6,29 +6,26 @@
 
 Filename: spectrometer_reading_plugin/additional_sql.sql
 Comment: 
 
 Filename: spectrometer_reading_plugin/ui/contrib/jobs/spectrometer_reading.yaml
 Comment: 
 
-Filename: ui/contrib/jobs/spectrometer_reading.yaml
+Filename: spectrometer_reading_plugin-0.2.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: spectrometer_reading_plugin-0.2.0.dist-info/LICENSE.txt
+Filename: spectrometer_reading_plugin-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: spectrometer_reading_plugin-0.2.0.dist-info/METADATA
+Filename: spectrometer_reading_plugin-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: spectrometer_reading_plugin-0.2.0.dist-info/WHEEL
+Filename: spectrometer_reading_plugin-0.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: spectrometer_reading_plugin-0.2.0.dist-info/entry_points.txt
+Filename: spectrometer_reading_plugin-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: spectrometer_reading_plugin-0.2.0.dist-info/top_level.txt
-Comment: 
-
-Filename: spectrometer_reading_plugin-0.2.0.dist-info/RECORD
+Filename: spectrometer_reading_plugin-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spectrometer_reading_plugin/__init__.py

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import adafruit_as7341
 import board
 import click
-from pioreactor.background_jobs.base import BackgroundJobWithDodging
+from pioreactor.background_jobs.base import BackgroundJobWithDodgingContrib
 from pioreactor.background_jobs.leader.mqtt_to_db_streaming import produce_metadata
 from pioreactor.background_jobs.leader.mqtt_to_db_streaming import register_source_to_sink
 from pioreactor.background_jobs.leader.mqtt_to_db_streaming import TopicToParserToTable
 from pioreactor.config import config
 from pioreactor.exc import HardwareNotFoundError
 from pioreactor.utils.timing import current_utc_datetime
 from pioreactor.whoami import get_latest_experiment_name
@@ -41,15 +41,15 @@
         ],
         parser,
         "as7341_spectrum_readings",
     )
 )
 
 
-class SpectrometerReading(BackgroundJobWithDodging):
+class SpectrometerReading(BackgroundJobWithDodgingContrib):
 
     job_name = "spectrometer_reading"
 
     published_settings = {
         "band_415": {"datatype": "float", "unit": "AU", "settable": False},
         "band_445": {"datatype": "float", "unit": "AU", "settable": False},
         "band_480": {"datatype": "float", "unit": "AU", "settable": False},
@@ -57,15 +57,15 @@
         "band_555": {"datatype": "float", "unit": "AU", "settable": False},
         "band_590": {"datatype": "float", "unit": "AU", "settable": False},
         "band_630": {"datatype": "float", "unit": "AU", "settable": False},
         "band_680": {"datatype": "float", "unit": "AU", "settable": False},
     }
 
     def __init__(self, unit, experiment):
-        super().__init__(unit=unit, experiment=experiment)
+        super().__init__(unit=unit, experiment=experiment, source="spectrometer_reading_plugin")
 
         try:
             i2c = board.I2C()
             self.sensor = adafruit_as7341.AS7341(i2c)
         except Exception:
             self.logger.error("Is the AS7341 board attached to the Pioreactor HAT?")
             raise HardwareNotFoundError("Is the AS7341 board attached to the Pioreactor HAT?")
```

## Comparing `spectrometer_reading_plugin-0.2.0.dist-info/LICENSE.txt` & `spectrometer_reading_plugin-0.2.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `spectrometer_reading_plugin-0.2.0.dist-info/METADATA` & `spectrometer_reading_plugin-0.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrometer-reading-plugin
-Version: 0.2.0
+Version: 0.2.1
 Summary: Take spectrometer readings (between OD readings) from the Adafruit AS7341 attached to your Pioreactor
 Home-page: https://github.com/Pioreactor/spectrometer-reading-plugin
 Author: Kelly Tran, Cam Davidson-Pilon
 Author-email: cam@pioreactor.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

## Comparing `spectrometer_reading_plugin-0.2.0.dist-info/RECORD` & `spectrometer_reading_plugin-0.2.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-spectrometer_reading_plugin/__init__.py,sha256=Qe7np0KuW4pX4JSzQlME7dhnEyRHmktePbsFMxreMqU,5677
+spectrometer_reading_plugin/__init__.py,sha256=OsVSLH82gN9agzStbFXdjTUK6DhMHe_dyUX_uNaKrmQ,5729
 spectrometer_reading_plugin/additional_config.ini,sha256=zusPtu2mxGGmHGCmKIuuP8dgiNDhrTDGWZ_CRUTTGPs,162
 spectrometer_reading_plugin/additional_sql.sql,sha256=xwPkGPUj1YffR7zgiLGgJCu13LOX_nVX9LOrFQIV7VI,257
 spectrometer_reading_plugin/ui/contrib/jobs/spectrometer_reading.yaml,sha256=Q6MTjv1UV8WWfiDTDQNhV_mN0W6dXwJqrr5drHqWEP8,231
-ui/contrib/jobs/spectrometer_reading.yaml,sha256=Q6MTjv1UV8WWfiDTDQNhV_mN0W6dXwJqrr5drHqWEP8,231
-spectrometer_reading_plugin-0.2.0.dist-info/LICENSE.txt,sha256=Kjuo1wEzXBxtIQm3yLYJLIRO6hgWkMopAOs91wiCZqg,1049
-spectrometer_reading_plugin-0.2.0.dist-info/METADATA,sha256=na4DCJr7xyJqoiSEs7OUqi3zOjfeKU73PBinDuUGylU,1854
-spectrometer_reading_plugin-0.2.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-spectrometer_reading_plugin-0.2.0.dist-info/entry_points.txt,sha256=ujD4vhE60iMCiKQZE_3OcriPnJhN--ah4KsdplJa3uo,79
-spectrometer_reading_plugin-0.2.0.dist-info/top_level.txt,sha256=ShLg-ZsLHo8U1XlEMIrHN6uYQgpeu-LBnGCt8aEWz1A,28
-spectrometer_reading_plugin-0.2.0.dist-info/RECORD,,
+spectrometer_reading_plugin-0.2.1.dist-info/LICENSE.txt,sha256=Kjuo1wEzXBxtIQm3yLYJLIRO6hgWkMopAOs91wiCZqg,1049
+spectrometer_reading_plugin-0.2.1.dist-info/METADATA,sha256=YEFAt2BeznWZbzmch-vv-OYqS1V1FNlLOBHKxm7hl1w,1854
+spectrometer_reading_plugin-0.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+spectrometer_reading_plugin-0.2.1.dist-info/entry_points.txt,sha256=ujD4vhE60iMCiKQZE_3OcriPnJhN--ah4KsdplJa3uo,79
+spectrometer_reading_plugin-0.2.1.dist-info/top_level.txt,sha256=ShLg-ZsLHo8U1XlEMIrHN6uYQgpeu-LBnGCt8aEWz1A,28
+spectrometer_reading_plugin-0.2.1.dist-info/RECORD,,
```

