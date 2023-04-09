# Comparing `tmp/led_calibration_plugin-1.1.0-py3-none-any.whl.zip` & `tmp/led_calibration_plugin-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 10629 bytes, number of entries: 11
--rw-r--r--  2.0 unx      249 b- defN 22-Nov-02 00:06 led_calibration_plugin/__init__.py
+Zip file size: 10917 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      258 b- defN 23-Apr-09 00:02 led_calibration_plugin/__init__.py
 -rw-r--r--  2.0 unx     4163 b- defN 22-Nov-02 00:25 led_calibration_plugin/calibrated_light_dark_cycle.py
--rw-r--r--  2.0 unx    11511 b- defN 22-Nov-02 00:19 led_calibration_plugin/led_calibration.py
--rw-r--r--  2.0 unx     6651 b- defN 22-Nov-02 00:23 led_calibration_plugin/test_led_calibration.py
+-rw-r--r--  2.0 unx    12926 b- defN 23-Mar-31 00:07 led_calibration_plugin/led_calibration.py
+-rw-r--r--  2.0 unx     6885 b- defN 23-Mar-30 23:51 led_calibration_plugin/test_led_calibration.py
 -rw-r--r--  2.0 unx      518 b- defN 22-Nov-02 00:06 led_calibration_plugin/ui/contrib/automations/led/calibrated_light_dark_cycle.yaml
--rw-r--r--  2.0 unx     1062 b- defN 22-Nov-02 00:29 led_calibration_plugin-1.1.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     4152 b- defN 22-Nov-02 00:29 led_calibration_plugin-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-02 00:29 led_calibration_plugin-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       69 b- defN 22-Nov-02 00:29 led_calibration_plugin-1.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 22-Nov-02 00:29 led_calibration_plugin-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1115 b- defN 22-Nov-02 00:29 led_calibration_plugin-1.1.0.dist-info/RECORD
-11 files, 29605 bytes uncompressed, 8673 bytes compressed:  70.7%
+-rw-r--r--  2.0 unx     1062 b- defN 23-Apr-09 00:03 led_calibration_plugin-1.2.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     4152 b- defN 23-Apr-09 00:03 led_calibration_plugin-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 00:03 led_calibration_plugin-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       69 b- defN 23-Apr-09 00:03 led_calibration_plugin-1.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Apr-09 00:03 led_calibration_plugin-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1115 b- defN 23-Apr-09 00:03 led_calibration_plugin-1.2.0.dist-info/RECORD
+11 files, 31263 bytes uncompressed, 8961 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: led_calibration_plugin/test_led_calibration.py
 Comment: 
 
 Filename: led_calibration_plugin/ui/contrib/automations/led/calibrated_light_dark_cycle.yaml
 Comment: 
 
-Filename: led_calibration_plugin-1.1.0.dist-info/LICENSE.txt
+Filename: led_calibration_plugin-1.2.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: led_calibration_plugin-1.1.0.dist-info/METADATA
+Filename: led_calibration_plugin-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: led_calibration_plugin-1.1.0.dist-info/WHEEL
+Filename: led_calibration_plugin-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: led_calibration_plugin-1.1.0.dist-info/entry_points.txt
+Filename: led_calibration_plugin-1.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: led_calibration_plugin-1.1.0.dist-info/top_level.txt
+Filename: led_calibration_plugin-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: led_calibration_plugin-1.1.0.dist-info/RECORD
+Filename: led_calibration_plugin-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## led_calibration_plugin/__init__.py

```diff
@@ -1,5 +1,7 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
-from led_calibration_plugin.calibrated_light_dark_cycle import CalibratedLightDarkCycle  # noqa: F401
+from led_calibration_plugin.calibrated_light_dark_cycle import (
+    CalibratedLightDarkCycle,
+)  # noqa: F401
 from led_calibration_plugin.led_calibration import click_led_calibration  # noqa: F401
```

## led_calibration_plugin/led_calibration.py

```diff
@@ -5,26 +5,28 @@
 
 import click
 from msgspec.json import decode
 from msgspec.json import encode
 from pioreactor import structs
 from pioreactor import types as pt
 from pioreactor.actions.led_intensity import led_intensity
-from pioreactor.pubsub import publish
+from pioreactor.config import leader_address
+from pioreactor.mureq import patch
+from pioreactor.mureq import put
 from pioreactor.utils import is_pio_job_running
 from pioreactor.utils import local_persistant_storage
 from pioreactor.utils import publish_ready_to_disconnected_state
 from pioreactor.utils.timing import current_utc_datetime
 from pioreactor.whoami import get_latest_testing_experiment_name
 from pioreactor.whoami import get_unit_name
-from pioreactor.whoami import UNIVERSAL_EXPERIMENT
 
 
 class LEDCalibration(structs.Calibration):
-    timestamp: datetime
+    created_at: datetime
+    pioreactor_unit: str
     name: str
     max_intensity: float
     min_intensity: float
     min_lightprobe_readings: float
     max_lightprobe_readings: float
     curve_data_: list[float]
     curve_type: str
@@ -94,15 +96,15 @@
     plt.theme("pro")
     plt.title(title)
     plt.plot_size(105, 22)
     plt.xlim(x_min, x_max)
     plt.show()
 
 
-def start_recording(channel, min_intensity, max_intensity):
+def start_recording(channel: pt.LedChannel, min_intensity, max_intensity):
     led_intensity(
         desired_state={"A": 0, "B": 0, "C": 0, "D": 0},
         unit=get_unit_name(),
         experiment=get_latest_testing_experiment_name(),
         verbose=False,
     )
 
@@ -184,26 +186,28 @@
         interpolation_curve=curve_callable,
         highlight_recent_point=False,
     )
 
     click.confirm("Confirm and save to disk?", abort=True, default=True)
 
 
-def save_results_locally(
+def save_results(
     curve_data_: list[float],
     curve_type: str,
     lightprobe_readings: list[float],
     led_intensities: list[float],
     name: str,
     max_intensity: float,
     min_intensity: float,
-    channel,
-) -> structs.LEDCalibration:
+    channel: pt.LedChannel,
+    unit: str,
+) -> LEDCalibration:
     data_blob = LEDCalibration(
-        timestamp=current_utc_datetime(),
+        created_at=current_utc_datetime(),
+        pioreactor_unit=unit,
         name=name,
         max_intensity=max_intensity,
         min_intensity=0,
         min_lightprobe_readings=min(lightprobe_readings),
         max_lightprobe_readings=max(lightprobe_readings),
         curve_data_=curve_data_,
         curve_type=curve_type,
@@ -211,19 +215,16 @@
         led_intensities=led_intensities,
         channel=channel,
     )
 
     with local_persistant_storage("led_calibrations") as cache:
         cache[name] = encode(data_blob)
 
-    with local_persistant_storage("current_led_calibration") as cache:
-        cache[channel] = encode(data_blob)
-
-    # send to MQTT
-    publish(f"pioreactor/{get_unit_name()}/{UNIVERSAL_EXPERIMENT}/calibrations", encode(data_blob))
+    publish_to_leader(name)
+    change_current(name)
 
     return data_blob
 
 
 ## general schematic of what's gonna happen
 def led_calibration(min_intensity: float, max_intensity: float):
     unit = get_unit_name()
@@ -242,23 +243,24 @@
         lightprobe_readings, led_intensities = start_recording(
             channel, min_intensity, max_intensity
         )
 
         curve, curve_type = calculate_curve_of_best_fit(lightprobe_readings, led_intensities, 1)
         show_results_and_confirm_with_user(curve, curve_type, lightprobe_readings, led_intensities)
 
-        data_blob = save_results_locally(
+        data_blob = save_results(
             curve,
             curve_type,
             lightprobe_readings,
             led_intensities,
             name,
             max_intensity,
             min_intensity,
             channel,
+            unit,
         )
         click.echo(click.style(f"Data for {name}", underline=True, bold=True))
         click.echo(data_blob)
         click.echo(f"Finished calibration of {name} ✅")
         return
 
 
@@ -286,47 +288,87 @@
             for channel in c.keys():
                 display_from_calibration_blob(decode(c[channel]))
                 click.echo()
                 click.echo()
                 click.echo()
 
 
+def publish_to_leader(name: str) -> bool:
+    success = True
+
+    with local_persistant_storage("led_calibrations") as all_calibrations:
+        calibration_result = decode(all_calibrations[name], type=LEDCalibration)
+
+    try:
+        res = put(
+            f"http://{leader_address}/api/calibrations",
+            encode(calibration_result),
+            headers={"Content-Type": "application/json"},
+        )
+        if not res.ok:
+            success = False
+    except Exception as e:
+        print(e)
+        success = False
+    if not success:
+        click.echo(
+            f"Could not update in database on leader at http://{leader_address}/api/calibrations ❌"
+        )
+    return success
+
+
 def change_current(name: str) -> None:
     try:
-        with local_persistant_storage("led_calibrations") as c:
-            calibration = decode(c[name], type=LEDCalibration)
+        with local_persistant_storage("led_calibrations") as all_calibrations:
+            new_calibration = decode(all_calibrations[name], type=LEDCalibration)
 
-        channel = calibration.channel
-        with local_persistant_storage("current_led_calibration") as c:
-            name_being_bumped = decode(c[channel], type=LEDCalibration).name
-            c[channel] = encode(calibration)
-        click.echo(f"Swapped {name_being_bumped} for {name} ✅")
-    except Exception as e:
-        click.echo(f"Failed to swap. {e}")
+        channel = new_calibration.channel
+        with local_persistant_storage("current_led_calibration") as current_calibrations:
+            if channel in current_calibrations:
+                old_calibration = decode(current_calibrations[channel], type=LEDCalibration)
+            else:
+                old_calibration = None
+
+            current_calibrations[channel] = encode(new_calibration)
+
+        res = patch(
+            f"http://{leader_address}/api/calibrations/{get_unit_name()}/{new_calibration.type}/{new_calibration.name}",
+            json={"current": 1},
+        )
+        if not res.ok:
+            click.echo("Could not update in database on leader ❌")
+
+        if old_calibration:
+            click.echo(f"Replaced {old_calibration.name} with {new_calibration.name}   ✅")
+        else:
+            click.echo(f"Set {new_calibration.name} to current calibration  ✅")
+
+    except Exception:
+        click.echo("Failed to swap.")
         raise click.Abort()
 
 
 def list_() -> None:
     # get current calibrations
     current = []
     with local_persistant_storage("current_led_calibration") as c:
         for ch in c.keys():
             cal = decode(c[ch], type=LEDCalibration)
             current.append(cal.name)
 
     click.secho(
-        f"{'Name':15s} {'Date':18s} {'Pump type':12s} {'Currently in use?':20s}",
+        f"{'Name':15s} {'Date':18s} {'Channel':12s} {'Currently in use?':20s}",
         bold=True,
     )
     with local_persistant_storage("led_calibrations") as c:
         for name in c.keys():
             try:
                 cal = decode(c[name], type=LEDCalibration)
                 click.secho(
-                    f"{cal.name:15s} {cal.timestamp:%d %b, %Y}       {cal.channel:12s} {'✅' if cal.name in current else ''}",
+                    f"{cal.name:15s} {cal.created_at:%d %b, %Y}       {cal.channel:12s} {'✅' if cal.name in current else ''}",
                 )
             except Exception as e:
                 raise e
 
 
 ### This part displays the current led calibration
 @click.group(invoke_without_command=True, name="led_calibration")
@@ -361,9 +403,15 @@
 
 
 @click_led_calibration.command(name="list")
 def click_list():
     list_()
 
 
+@click_led_calibration.command(name="publish")
+@click.argument("name", type=click.STRING)
+def click_publish(name: str):
+    publish_to_leader(name)
+
+
 if __name__ == "__main__":
     click_led_calibration()
```

## led_calibration_plugin/test_led_calibration.py

```diff
@@ -47,15 +47,16 @@
 def test_set_intensity_au_above_max() -> None:
     experiment = "test_set_intensity_au_above_max"
     unit = get_unit_name()
 
     with local_persistant_storage("current_led_calibration") as cache:
         cache["C"] = encode(
             LEDCalibration(
-                timestamp=current_utc_timestamp(),
+                created_at=current_utc_timestamp(),
+                pioreactor_unit=unit,
                 name=experiment,
                 max_intensity=100,
                 min_intensity=0,
                 min_lightprobe_readings=0,
                 max_lightprobe_readings=1000,
                 curve_data_=[1, 0],
                 curve_type="poly",
@@ -63,15 +64,16 @@
                 led_intensities=[],
                 channel="C",
             )
         )
 
         cache["D"] = encode(
             LEDCalibration(
-                timestamp=current_utc_timestamp(),
+                created_at=current_utc_timestamp(),
+                pioreactor_unit=unit,
                 name=experiment,
                 max_intensity=100,
                 min_intensity=0,
                 min_lightprobe_readings=0,
                 max_lightprobe_readings=1000,
                 curve_data_=[1, 0],
                 curve_type="poly",
@@ -101,15 +103,16 @@
 def test_set_intensity_au_negative() -> None:
     experiment = "test_set_intensity_au_negative"
     unit = get_unit_name()
 
     with local_persistant_storage("current_led_calibration") as cache:
         cache["C"] = encode(
             LEDCalibration(
-                timestamp=current_utc_timestamp(),
+                created_at=current_utc_timestamp(),
+                pioreactor_unit=unit,
                 name=experiment,
                 max_intensity=100,
                 min_intensity=0,
                 min_lightprobe_readings=0,
                 max_lightprobe_readings=1000,
                 curve_data_=[1, 0],
                 curve_type="poly",
@@ -117,15 +120,16 @@
                 led_intensities=[],
                 channel="C",
             )
         )
 
         cache["D"] = encode(
             LEDCalibration(
-                timestamp=current_utc_timestamp(),
+                created_at=current_utc_timestamp(),
+                pioreactor_unit=unit,
                 name=experiment,
                 max_intensity=100,
                 min_intensity=0,
                 min_lightprobe_readings=0,
                 max_lightprobe_readings=1000,
                 curve_data_=[10, 0],
                 curve_type="poly",
@@ -156,15 +160,16 @@
 def test_set_curve_data_negative() -> None:
     experiment = "test_set_curve_data_negative"
     unit = get_unit_name()
 
     with local_persistant_storage("current_led_calibration") as cache:
         cache["C"] = encode(
             LEDCalibration(
-                timestamp=current_utc_timestamp(),
+                created_at=current_utc_timestamp(),
+                pioreactor_unit=unit,
                 name=experiment,
                 max_intensity=100,
                 min_intensity=0,
                 min_lightprobe_readings=0,
                 max_lightprobe_readings=1000,
                 curve_data_=[1, -4],
                 curve_type="poly",
@@ -173,15 +178,16 @@
                 channel="C",
             )
         )
 
     with local_persistant_storage("current_led_calibration") as cache:
         cache["D"] = encode(
             LEDCalibration(
-                timestamp=current_utc_timestamp(),
+                created_at=current_utc_timestamp(),
+                pioreactor_unit=unit,
                 name=experiment,
                 max_intensity=100,
                 min_intensity=0,
                 min_lightprobe_readings=0,
                 max_lightprobe_readings=1000,
                 curve_data_=[1, -4],
                 curve_type="poly",
```

## Comparing `led_calibration_plugin-1.1.0.dist-info/LICENSE.txt` & `led_calibration_plugin-1.2.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `led_calibration_plugin-1.1.0.dist-info/METADATA` & `led_calibration_plugin-1.2.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: led-calibration-plugin
-Version: 1.1.0
+Version: 1.2.0
 Summary: Calibrate your LEDs using an external light probe.
 Home-page: https://github.com/pioreactor/pioreactor-led-calibration-plugin
 Author: Kelly Tran, Cameron Davidson-Pilon
 Author-email: cam@pioreactor.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

## Comparing `led_calibration_plugin-1.1.0.dist-info/RECORD` & `led_calibration_plugin-1.2.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-led_calibration_plugin/__init__.py,sha256=pVi1O3kB9UxFjV2aKJ6KbtOjM-7dVuqzm_jIdZP_YlA,249
+led_calibration_plugin/__init__.py,sha256=S8sdwK13ZJvxnOuaAd1u5YIF_jbPK2FeubcDgN3QEvE,258
 led_calibration_plugin/calibrated_light_dark_cycle.py,sha256=KSYmATQIqEuER7LdfohnLX2Bwk2XNJsGoZz0Vc5ywv4,4163
-led_calibration_plugin/led_calibration.py,sha256=71jmhHqmDh1e7jaCOh57YpNqwafZPRCJ3pd8T1xImLc,11511
-led_calibration_plugin/test_led_calibration.py,sha256=DgiPmKBcoIZaAnt0gKAc74Vpu545dI4Lvhj1jbpzzhI,6651
+led_calibration_plugin/led_calibration.py,sha256=nOLAQil4hK3jsgmkRxY389K3uTBuVVbrR-tH_KPLdzA,12926
+led_calibration_plugin/test_led_calibration.py,sha256=J2CqdM3SVxWQWzJBIOJHZ5xzU1X7E392XQ4rBrXuWSw,6885
 led_calibration_plugin/ui/contrib/automations/led/calibrated_light_dark_cycle.yaml,sha256=cmo03wMtqB7wKY6X3tevSl6KjUhRqLPEAjd5PtFppnI,518
-led_calibration_plugin-1.1.0.dist-info/LICENSE.txt,sha256=ipJf_7c1vobIyTbjJZBpBepQJtAIu2fAxMOP9SYjWps,1062
-led_calibration_plugin-1.1.0.dist-info/METADATA,sha256=ndomAjBM5dbpIkIJSKyX60euMpnIPPCNa82793j-T3c,4152
-led_calibration_plugin-1.1.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-led_calibration_plugin-1.1.0.dist-info/entry_points.txt,sha256=jjNBY8vhrvrlCrCQzmVlSzxqrbjlFT5oxqInfPF27rk,69
-led_calibration_plugin-1.1.0.dist-info/top_level.txt,sha256=aG26kKd4yawYfIL4rWWdKgkH6yv-VPTne3ld2CueFSQ,23
-led_calibration_plugin-1.1.0.dist-info/RECORD,,
+led_calibration_plugin-1.2.0.dist-info/LICENSE.txt,sha256=ipJf_7c1vobIyTbjJZBpBepQJtAIu2fAxMOP9SYjWps,1062
+led_calibration_plugin-1.2.0.dist-info/METADATA,sha256=YPTfFEYCCQc759TJmj2hEqrImH7hEbC3kPd_d56lbPY,4152
+led_calibration_plugin-1.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+led_calibration_plugin-1.2.0.dist-info/entry_points.txt,sha256=jjNBY8vhrvrlCrCQzmVlSzxqrbjlFT5oxqInfPF27rk,69
+led_calibration_plugin-1.2.0.dist-info/top_level.txt,sha256=aG26kKd4yawYfIL4rWWdKgkH6yv-VPTne3ld2CueFSQ,23
+led_calibration_plugin-1.2.0.dist-info/RECORD,,
```

