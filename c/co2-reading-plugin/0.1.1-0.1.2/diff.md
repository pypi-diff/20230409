# Comparing `tmp/co2_reading_plugin-0.1.1-py3-none-any.whl.zip` & `tmp/co2_reading_plugin-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 6049 bytes, number of entries: 11
--rw-r--r--  2.0 unx     6024 b- defN 23-Feb-02 18:01 co2_reading_plugin/__init__.py
+Zip file size: 6245 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     6467 b- defN 23-Apr-08 23:56 co2_reading_plugin/__init__.py
 -rw-r--r--  2.0 unx      177 b- defN 23-Feb-02 18:01 co2_reading_plugin/additional_config.ini
 -rw-r--r--  2.0 unx      211 b- defN 22-Oct-11 18:10 co2_reading_plugin/additional_sql.sql
 -rw-r--r--  2.0 unx      270 b- defN 23-Feb-02 18:01 co2_reading_plugin/ui/contrib/charts/co2_readings.yaml
 -rw-r--r--  2.0 unx      471 b- defN 23-Feb-02 20:30 co2_reading_plugin/ui/contrib/jobs/co2_reading.yaml
--rw-r--r--  2.0 unx     1049 b- defN 23-Feb-02 20:33 co2_reading_plugin-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1147 b- defN 23-Feb-02 20:33 co2_reading_plugin-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-02 20:33 co2_reading_plugin-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 23-Feb-02 20:33 co2_reading_plugin-0.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       19 b- defN 23-Feb-02 20:33 co2_reading_plugin-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1044 b- defN 23-Feb-02 20:33 co2_reading_plugin-0.1.1.dist-info/RECORD
-11 files, 10565 bytes uncompressed, 4229 bytes compressed:  60.0%
+-rw-r--r--  2.0 unx     1049 b- defN 23-Apr-08 23:57 co2_reading_plugin-0.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1147 b- defN 23-Apr-08 23:57 co2_reading_plugin-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-08 23:57 co2_reading_plugin-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 23-Apr-08 23:57 co2_reading_plugin-0.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Apr-08 23:57 co2_reading_plugin-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1044 b- defN 23-Apr-08 23:57 co2_reading_plugin-0.1.2.dist-info/RECORD
+11 files, 11008 bytes uncompressed, 4425 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: co2_reading_plugin/ui/contrib/charts/co2_readings.yaml
 Comment: 
 
 Filename: co2_reading_plugin/ui/contrib/jobs/co2_reading.yaml
 Comment: 
 
-Filename: co2_reading_plugin-0.1.1.dist-info/LICENSE.txt
+Filename: co2_reading_plugin-0.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: co2_reading_plugin-0.1.1.dist-info/METADATA
+Filename: co2_reading_plugin-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: co2_reading_plugin-0.1.1.dist-info/WHEEL
+Filename: co2_reading_plugin-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: co2_reading_plugin-0.1.1.dist-info/entry_points.txt
+Filename: co2_reading_plugin-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: co2_reading_plugin-0.1.1.dist-info/top_level.txt
+Filename: co2_reading_plugin-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: co2_reading_plugin-0.1.1.dist-info/RECORD
+Filename: co2_reading_plugin-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## co2_reading_plugin/__init__.py

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import click
-from pioreactor.background_jobs.base import BackgroundJob
+from pioreactor.background_jobs.base import BackgroundJobContrib
 from pioreactor.background_jobs.leader.mqtt_to_db_streaming import produce_metadata
 from pioreactor.background_jobs.leader.mqtt_to_db_streaming import register_source_to_sink
 from pioreactor.background_jobs.leader.mqtt_to_db_streaming import TopicToParserToTable
 from pioreactor.config import config
 from pioreactor.exc import HardwareNotFoundError
 from pioreactor.hardware import SCL
 from pioreactor.hardware import SDA
@@ -32,15 +32,15 @@
         ["pioreactor/+/+/scd_reading/co2", "pioreactor/+/+/co2_reading/co2"],
         parser,
         "co2_readings",
     )
 )
 
 
-class SCDReading(BackgroundJob):
+class SCDReading(BackgroundJobContrib):
 
     job_name = "scd_reading"
 
     published_settings = {
         "interval": {"datatype": "float", "unit": "s", "settable": True},
         "co2": {"datatype": "float", "unit": "ppm", "settable": False},
         "temperature": {"datatype": "float", "unit": "°C", "settable": False},
@@ -52,15 +52,15 @@
         unit: str,
         experiment: str,
         interval: float,
         skip_co2: bool = False,
         skip_temperature: bool = False,
         skip_relative_humidity: bool = False,
     ) -> None:
-        super().__init__(unit=unit, experiment=experiment)
+        super().__init__(unit=unit, experiment=experiment, source="co2_reading_plugin")
 
         self.interval = interval
         self.skip_co2 = skip_co2
         self.skip_temperature = skip_temperature
         self.skip_relative_humidity = skip_relative_humidity
 
         if is_pio_job_running("co2_reading"):
@@ -104,14 +104,19 @@
         self.record_scd_timer = timing.RepeatedTimer(
             self.interval, self.record_from_scd, run_immediately=True
         )
 
         self.record_scd_timer.start()
 
     def set_interval(self, new_interval) -> None:
+        # TODO: this isn't a very accurate way to update the interval.
+        # you can get very short intervals when updating. Ex, changing from 60s to 45s.
+        # 2023-02-06T14:42:34  |  pioreactor/worker1/pwm tests2/co2_reading/co2   520
+        # 2023-02-06T14:42:50  |  pioreactor/worker1/pwm tests2/co2_reading/co2   517
+        # The reason is how ReaptedTimer computes `time_to_next_run`
         self.record_scd_timer.interval = new_interval
         self.interval = new_interval
 
     def on_sleeping(self) -> None:
         # user pauses
         self.record_scd_timer.pause()
```

## Comparing `co2_reading_plugin-0.1.1.dist-info/LICENSE.txt` & `co2_reading_plugin-0.1.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `co2_reading_plugin-0.1.1.dist-info/METADATA` & `co2_reading_plugin-0.1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: co2-reading-plugin
-Version: 0.1.1
+Version: 0.1.2
 Summary: Return a CO₂ reading every interval from an Adafruit CO₂ sensors SCD30, SCD40 or SCD41.
 Home-page: https://github.com/Pioreactor/co2_reading_plugin
 Author: Kelly Tran, Cameron Davidson-Pilon
 Author-email: cam@pioreactor.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

