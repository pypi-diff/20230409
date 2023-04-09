# Comparing `tmp/aiopioneer-0.4.0rc1.tar.gz` & `tmp/aiopioneer-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopioneer-0.4.0rc1.tar", last modified: Wed Apr  5 21:55:59 2023, max compression
+gzip compressed data, was "aiopioneer-0.4.1.tar", last modified: Sun Apr  9 09:23:07 2023, max compression
```

## Comparing `aiopioneer-0.4.0rc1.tar` & `aiopioneer-0.4.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwx---   0 root         (0) adm          (4)        0 2023-04-05 21:55:59.668516 aiopioneer-0.4.0rc1/
--rw-rw----   0 root         (0) adm          (4)    11357 2022-11-17 13:13:29.000000 aiopioneer-0.4.0rc1/LICENSE
--rw-rw----   0 root         (0) adm          (4)    13464 2023-04-05 21:55:59.678343 aiopioneer-0.4.0rc1/PKG-INFO
--rw-rw----   0 root         (0) adm          (4)    12812 2023-03-11 20:27:45.000000 aiopioneer-0.4.0rc1/README.md
-drwxrwx---   0 root         (0) adm          (4)        0 2023-04-05 21:55:59.368520 aiopioneer-0.4.0rc1/aiopioneer/
--rw-rw----   0 root         (0) adm          (4)       68 2022-11-17 13:13:41.000000 aiopioneer-0.4.0rc1/aiopioneer/__init__.py
--rw-rw----   0 root         (0) adm          (4)     9864 2023-03-11 16:24:54.000000 aiopioneer-0.4.0rc1/aiopioneer/cli.py
--rw-rw----   0 root         (0) adm          (4)    12167 2023-04-04 00:22:07.000000 aiopioneer-0.4.0rc1/aiopioneer/commands.py
--rw-rw----   0 root         (0) adm          (4)    14914 2023-04-05 21:55:53.000000 aiopioneer-0.4.0rc1/aiopioneer/const.py
--rw-rw----   0 root         (0) adm          (4)    43747 2023-04-03 17:59:18.000000 aiopioneer-0.4.0rc1/aiopioneer/param.py
-drwxrwx---   0 root         (0) adm          (4)        0 2023-04-05 21:55:59.648516 aiopioneer-0.4.0rc1/aiopioneer/parsers/
--rw-rw----   0 root         (0) adm          (4)       35 2023-04-03 17:44:13.000000 aiopioneer-0.4.0rc1/aiopioneer/parsers/__init__.py
--rw-rw----   0 root         (0) adm          (4)     3205 2023-04-03 17:44:13.000000 aiopioneer-0.4.0rc1/aiopioneer/parsers/audio.py
--rw-rw----   0 root         (0) adm          (4)       41 2023-04-03 17:44:13.000000 aiopioneer-0.4.0rc1/aiopioneer/parsers/const.py
--rw-rw----   0 root         (0) adm          (4)    20107 2023-04-03 17:44:13.000000 aiopioneer-0.4.0rc1/aiopioneer/parsers/dsp.py
--rw-rw----   0 root         (0) adm          (4)    26292 2023-04-03 17:44:13.000000 aiopioneer-0.4.0rc1/aiopioneer/parsers/information.py
--rw-rw----   0 root         (0) adm          (4)     7566 2023-04-04 00:22:07.000000 aiopioneer-0.4.0rc1/aiopioneer/parsers/parse.py
--rw-rw----   0 root         (0) adm          (4)      630 2023-04-03 17:44:13.000000 aiopioneer-0.4.0rc1/aiopioneer/parsers/response.py
--rw-rw----   0 root         (0) adm          (4)    23791 2023-04-03 17:44:13.000000 aiopioneer-0.4.0rc1/aiopioneer/parsers/settings.py
--rw-rw----   0 root         (0) adm          (4)    15501 2023-04-03 17:44:13.000000 aiopioneer-0.4.0rc1/aiopioneer/parsers/system.py
--rw-rw----   0 root         (0) adm          (4)     3667 2023-04-04 00:22:07.000000 aiopioneer-0.4.0rc1/aiopioneer/parsers/tuner.py
--rw-rw----   0 root         (0) adm          (4)     8753 2023-04-03 17:44:13.000000 aiopioneer-0.4.0rc1/aiopioneer/parsers/video.py
--rw-rw----   0 root         (0) adm          (4)    74435 2023-04-04 00:22:07.000000 aiopioneer-0.4.0rc1/aiopioneer/pioneer_avr.py
--rw-rw----   0 root         (0) adm          (4)     5015 2023-03-29 19:15:30.000000 aiopioneer-0.4.0rc1/aiopioneer/util.py
-drwxrwx---   0 root         (0) adm          (4)        0 2023-04-05 21:55:59.458518 aiopioneer-0.4.0rc1/aiopioneer.egg-info/
--rw-rw----   0 root         (0) adm          (4)    13464 2023-04-05 21:55:58.000000 aiopioneer-0.4.0rc1/aiopioneer.egg-info/PKG-INFO
--rw-rw----   0 root         (0) adm          (4)      670 2023-04-05 21:55:59.000000 aiopioneer-0.4.0rc1/aiopioneer.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) adm          (4)        1 2023-04-05 21:55:58.000000 aiopioneer-0.4.0rc1/aiopioneer.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) adm          (4)       51 2023-04-05 21:55:58.000000 aiopioneer-0.4.0rc1/aiopioneer.egg-info/entry_points.txt
--rw-rw----   0 root         (0) adm          (4)       11 2023-04-05 21:55:58.000000 aiopioneer-0.4.0rc1/aiopioneer.egg-info/top_level.txt
--rw-rw----   0 root         (0) adm          (4)       38 2023-04-05 21:55:59.687411 aiopioneer-0.4.0rc1/setup.cfg
--rw-rw----   0 root         (0) adm          (4)     1100 2023-03-10 20:49:55.000000 aiopioneer-0.4.0rc1/setup.py
+drwxrwx---   0 root         (0) adm          (4)        0 2023-04-09 09:23:07.931850 aiopioneer-0.4.1/
+-rw-rw----   0 root         (0) adm          (4)    11357 2022-11-17 13:13:29.000000 aiopioneer-0.4.1/LICENSE
+-rw-rw----   0 root         (0) adm          (4)    13768 2023-04-09 09:23:07.933886 aiopioneer-0.4.1/PKG-INFO
+-rw-rw----   0 root         (0) adm          (4)    13119 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/README.md
+drwxrwx---   0 root         (0) adm          (4)        0 2023-04-09 09:23:07.551855 aiopioneer-0.4.1/aiopioneer/
+-rw-rw----   0 root         (0) adm          (4)       68 2022-11-17 13:13:41.000000 aiopioneer-0.4.1/aiopioneer/__init__.py
+-rw-rw----   0 root         (0) adm          (4)     9864 2023-03-11 16:24:54.000000 aiopioneer-0.4.1/aiopioneer/cli.py
+-rw-rw----   0 root         (0) adm          (4)    12266 2023-04-09 09:09:39.000000 aiopioneer-0.4.1/aiopioneer/commands.py
+-rw-rw----   0 root         (0) adm          (4)    14911 2023-04-09 09:21:39.000000 aiopioneer-0.4.1/aiopioneer/const.py
+-rw-rw----   0 root         (0) adm          (4)    43747 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/param.py
+drwxrwx---   0 root         (0) adm          (4)        0 2023-04-09 09:23:07.901851 aiopioneer-0.4.1/aiopioneer/parsers/
+-rw-rw----   0 root         (0) adm          (4)       35 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/__init__.py
+-rw-rw----   0 root         (0) adm          (4)     3205 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/audio.py
+-rw-rw----   0 root         (0) adm          (4)       41 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/const.py
+-rw-rw----   0 root         (0) adm          (4)    20107 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/dsp.py
+-rw-rw----   0 root         (0) adm          (4)    26292 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/information.py
+-rw-rw----   0 root         (0) adm          (4)     7566 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/parse.py
+-rw-rw----   0 root         (0) adm          (4)      630 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/response.py
+-rw-rw----   0 root         (0) adm          (4)    23791 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/settings.py
+-rw-rw----   0 root         (0) adm          (4)    15501 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/system.py
+-rw-rw----   0 root         (0) adm          (4)     3667 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/tuner.py
+-rw-rw----   0 root         (0) adm          (4)     8753 2023-04-07 14:25:01.000000 aiopioneer-0.4.1/aiopioneer/parsers/video.py
+-rw-rw----   0 root         (0) adm          (4)    75319 2023-04-09 09:09:39.000000 aiopioneer-0.4.1/aiopioneer/pioneer_avr.py
+-rw-rw----   0 root         (0) adm          (4)     5015 2023-03-29 19:15:30.000000 aiopioneer-0.4.1/aiopioneer/util.py
+drwxrwx---   0 root         (0) adm          (4)        0 2023-04-09 09:23:07.641854 aiopioneer-0.4.1/aiopioneer.egg-info/
+-rw-rw----   0 root         (0) adm          (4)    13768 2023-04-09 09:23:07.000000 aiopioneer-0.4.1/aiopioneer.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) adm          (4)      670 2023-04-09 09:23:07.000000 aiopioneer-0.4.1/aiopioneer.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) adm          (4)        1 2023-04-09 09:23:07.000000 aiopioneer-0.4.1/aiopioneer.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) adm          (4)       51 2023-04-09 09:23:07.000000 aiopioneer-0.4.1/aiopioneer.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) adm          (4)       11 2023-04-09 09:23:07.000000 aiopioneer-0.4.1/aiopioneer.egg-info/top_level.txt
+-rw-rw----   0 root         (0) adm          (4)       38 2023-04-09 09:23:07.945261 aiopioneer-0.4.1/setup.cfg
+-rw-rw----   0 root         (0) adm          (4)     1100 2023-03-10 20:49:55.000000 aiopioneer-0.4.1/setup.py
```

### Comparing `aiopioneer-0.4.0rc1/LICENSE` & `aiopioneer-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.0rc1/PKG-INFO` & `aiopioneer-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopioneer
-Version: 0.4.0rc1
+Version: 0.4.1
 Summary: Asyncio Python library for controlling a Pioneer AVR via its API
 Home-page: https://github.com/crowbarz/aiopioneer.git
 Author: Crowbar Z
 Author-email: crowbarz@outlook.com
 Keywords: pioneer avr asyncio
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
@@ -49,51 +49,52 @@
 
 ## Params
 
 A `params` object may be passed to the library that modifies its functionality.
 
 The default parameters listed below are for AVR models that do not match any custom profile. Custom profiles apply additional default parameters based on the model identifier retrieved from the AVR, and are defined in [`aiopioneer/param.py`](https://github.com/crowbarz/aiopioneer/blob/main/aiopioneer/param.py). If you need to modify parameters for the library to work for your AVR model, then please create a PR to add a custom profile for your AVR model, or log an issue containing your model number and the parameters that were modified requesting a custom profile to be created.
 
-> **NOTE:** YAML syntax is used in the table below. Use Python equivalents (`false` -> `False`, `true` -> `True`, `null` -> `None` etc.) when calling the Python API directly.
+> **NOTE:** YAML syntax is used in the table below. Use Python equivalents (`false` -> `False`, `true` -> `True`, `null` -> `None` etc.) when calling the Python API directly, and JSON syntax if manually specifying via the Home Assistant integration.
 
 | Name | Type | Default | Description
 | ---- | ---- | ------- | -----------
 | `ignored_zones` | list | `[]` | List of zones to ignore even if they are auto-discovered. Specify Zone IDs as strings: "1", "2", "3" and "Z".
 | `command_delay` | float | `0.1` | Insert a delay between sequential commands that are sent to the AVR. This appears to make the AVR behave more reliably during status polls. Increase this value if debug logging shows that your AVR times out between commands.
 | `max_source_id` | int | `60` | Maximum source ID that the source discovery queries. Reduce this if your AVR returns errors.
 | `max_volume` | int | `185` | Maximum volume for the Main Zone.
 | `max_volume_zonex` | int | `185` | Maximum volume for zones other than the Main Zone.
 | `power_on_volume_bounce` | bool | `false` | On some AVRs (eg. VSX-930) where a power-on is set, the initial volume is not reported by the AVR correctly until a volume change is made. This option enables a workaround that sends a volume up and down command to the AVR on power-on to correct the reported volume without affecting the power-on volume.
 | `volume_step_only` | bool | `false` | On some AVRs (eg. VSX-S510), setting the volume level is not supported natively by the API. This option emulates setting the volume level using volume up and down commands.
 | `ignore_volume_check` | bool | `false` | Don't check volume when determining whether a zone exists on the AVR. Useful for AVRs with an HDZone that passes through audio.
-| `zone_2_sources` | list | `["04", "06", "15", "26", "38", "53", "41", "44", "45", "17", "13", "05", "01", "02", "33", "46", "47", "99", "10"]` | Customizes the available sources for use with Zone 2 (some AVRs do not support all sources).
-| `zone_3_sources` | list | `["04", "06", "15", "26", "38", "53", "41", "44", "45", "17", "13", "05", "01", "02", "33", "46", "47", "99", "10"]` | Customizes the available sources for use with Zone 3 (some AVRs do not support all sources).
-| `zone_z_sources` | list | `["25", "04", "06", "10", "15", "19", "20", "21", "22", "23", "24", "34", "35", "26", "38", "53", "41", "44", "45", "17", "13", "33", "31", "46", "47", "48"]` | Customizes the available sources for use with HDZone (some AVRs do not support all sources).
+| `zone_1_sources` | list | `[]` | (>0.4) Customises the available sources for use with Zone 1. Defaults to all available sources.
+| `zone_2_sources` | list | `["04", "06", "15", "26", "38", "53", "41", "44", "45", "17", "13", "05", "01", "02", "33", "46", "47", "99", "10"]` | Customises the available sources for use with Zone 2 (some AVRs do not support all sources).
+| `zone_3_sources` | list | `["04", "06", "15", "26", "38", "53", "41", "44", "45", "17", "13", "05", "01", "02", "33", "46", "47", "99", "10"]` | Customises the available sources for use with Zone 3 (some AVRs do not support all sources).
+| `hdzone_sources` | list | `["25", "04", "06", "10", "15", "19", "20", "21", "22", "23", "24", "34", "35", "26", "38", "53", "41", "44", "45", "17", "13", "33", "31", "46", "47", "48"]` | Customises the available sources for use with HDZone (some AVRs do not support all sources).
 | `hdzone_volume_requirements` | list | `["13", "15", "05", "25"]` | A list of sources that HDZone must be set to for volume control, some AVRs do not support HDZone volume at all (see `ignore_volume_check` above) and some only allow control of certain sources.
-| `amplifier_speaker_system_modes` | dict | `....` | Customizes the names of speaker system modes. Different generations of AVR will name zones slighty differently. For example, the SC-LX57 names speaker system mode `15` as `5.1ch Bi-Amp + ZONE2` however this can also be called `5.2ch Bi-Amp + HDZONE` on newer AVRs.
+| `amplifier_speaker_system_modes` | dict | `....` | Customises the names of speaker system modes. Different generations of AVR will name zones slighty differently. For example, the SC-LX57 names speaker system mode `15` as `5.1ch Bi-Amp + ZONE2` however this can also be called `5.2ch Bi-Amp + HDZONE` on newer AVRs.
 | `disabled_amplifier_listening_modes` | list | `[]` | A list of disabled listening modes / sound modes, all modes are enabled by default, some AVRs have definitions already to disable unsupported modes. If you try to change sound mode to a mode that has not been enabled, the AVR will return an error (usually `E02`).
 | `video_resolution_modes` | list | `['0', '1', '3', '4', '5', '6', '7', '8', '9']` | Sets the available video resolutions. Not all AVRs support the same resolution settings. This defaults to all of the latest resolutions from FY16.
 | `mhl_source` | string | `null` | Sets the MHL source ID. This is used for media controls. This information cannot be queried automatically
 | `enabled_functions` | list | `["amp", "dsp", "tuner", "tone", "channels", "video", "system", "audio"]` | Change the functions that are enabled by the API, adding more functions will increase the amount of time it takes to complete a full init and update.
 | `disable_autoquery` | bool | `false` | Setting to `true` will disable auto queries on init for all functions apart from basic functionality (power, source, volume and mute). If you only need those functions, you can set this to `true`
 | `am_frequency_step` | int | `null` | Optional setting to configure the AM frequency step. If this is set to `null`, a function is queued to detect this information by stepping up and down the frequency when the tuner is first used while set to AM.
 | `debug_listener` | bool | `false` | Enables additional debug logging for the listener task.
 | `debug_responder` | bool | `false` | Enables additional debug logging for the responder task.
 | `debug_updater` | bool | `false` | Enables additional debug logging for the updater task.
 | `debug_command` | bool | `false` | Enables additional debug logging for commands sent and responses received.
 
-## Command line interface (CLI) (>= 0.1.3)
+## Command line interface (CLI) (>= 0.1.3, CLI arguments >= 0.3)
 
 A very simple command line interface `aiopioneer` is available to connect to the AVR, send commands and receive responses. It can be used to test the capabilities of the library against your specific AVR.
 
 On Home Assistant, you can run the CLI when the `pioneer_async` Home Assistant integration has been installed. On Home Assistant Supervised or Container, start the CLI from within the HA container: `docker exec -it homeassistant aiopioneer`.
 
-Invoke the CLI with the following optional parameters:
+Invoke the CLI with the following arguments:
 
-| Option | Default | Description
+| Argument | Default | Description
 | --- | --- | ---
 | hostname | required | hostname for AVR connection
 | `-p`<br>`--port` | 8102 | port for AVR connection
 | `+Q`<br>`--no-query-device-info` | None | skip AVR device info query
 | `+Z`<br>`--no-query-zones` | None | skip AVR zone query
 
 The CLI accepts all API commands, as well as the following:
@@ -167,14 +168,17 @@
 
 ## Known issues and future plans
 
 - Document PioneerAVR API
 
 ## Breaking changes
 
+- **0.4**\
+  `zone_z_sources` was renamed `hdzone_sources` for even more consistency.
+
 - **0.3**\
   `zone_h_sources` was renamed `zone_z_sources` for consistency.
 
 - **0.2**\
   `volume_step_delta` has been removed entirely.
 
   By default, a number of additional queries are sent at module startup to the AVR to gather amp, tuner and channel levels attributes. If your AVR does not handle these additional queries well, they can be disabled by setting parameter `disable_autoquery` to `true`.
```

### Comparing `aiopioneer-0.4.0rc1/README.md` & `aiopioneer-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,51 +31,52 @@
 
 ## Params
 
 A `params` object may be passed to the library that modifies its functionality.
 
 The default parameters listed below are for AVR models that do not match any custom profile. Custom profiles apply additional default parameters based on the model identifier retrieved from the AVR, and are defined in [`aiopioneer/param.py`](https://github.com/crowbarz/aiopioneer/blob/main/aiopioneer/param.py). If you need to modify parameters for the library to work for your AVR model, then please create a PR to add a custom profile for your AVR model, or log an issue containing your model number and the parameters that were modified requesting a custom profile to be created.
 
-> **NOTE:** YAML syntax is used in the table below. Use Python equivalents (`false` -> `False`, `true` -> `True`, `null` -> `None` etc.) when calling the Python API directly.
+> **NOTE:** YAML syntax is used in the table below. Use Python equivalents (`false` -> `False`, `true` -> `True`, `null` -> `None` etc.) when calling the Python API directly, and JSON syntax if manually specifying via the Home Assistant integration.
 
 | Name | Type | Default | Description
 | ---- | ---- | ------- | -----------
 | `ignored_zones` | list | `[]` | List of zones to ignore even if they are auto-discovered. Specify Zone IDs as strings: "1", "2", "3" and "Z".
 | `command_delay` | float | `0.1` | Insert a delay between sequential commands that are sent to the AVR. This appears to make the AVR behave more reliably during status polls. Increase this value if debug logging shows that your AVR times out between commands.
 | `max_source_id` | int | `60` | Maximum source ID that the source discovery queries. Reduce this if your AVR returns errors.
 | `max_volume` | int | `185` | Maximum volume for the Main Zone.
 | `max_volume_zonex` | int | `185` | Maximum volume for zones other than the Main Zone.
 | `power_on_volume_bounce` | bool | `false` | On some AVRs (eg. VSX-930) where a power-on is set, the initial volume is not reported by the AVR correctly until a volume change is made. This option enables a workaround that sends a volume up and down command to the AVR on power-on to correct the reported volume without affecting the power-on volume.
 | `volume_step_only` | bool | `false` | On some AVRs (eg. VSX-S510), setting the volume level is not supported natively by the API. This option emulates setting the volume level using volume up and down commands.
 | `ignore_volume_check` | bool | `false` | Don't check volume when determining whether a zone exists on the AVR. Useful for AVRs with an HDZone that passes through audio.
-| `zone_2_sources` | list | `["04", "06", "15", "26", "38", "53", "41", "44", "45", "17", "13", "05", "01", "02", "33", "46", "47", "99", "10"]` | Customizes the available sources for use with Zone 2 (some AVRs do not support all sources).
-| `zone_3_sources` | list | `["04", "06", "15", "26", "38", "53", "41", "44", "45", "17", "13", "05", "01", "02", "33", "46", "47", "99", "10"]` | Customizes the available sources for use with Zone 3 (some AVRs do not support all sources).
-| `zone_z_sources` | list | `["25", "04", "06", "10", "15", "19", "20", "21", "22", "23", "24", "34", "35", "26", "38", "53", "41", "44", "45", "17", "13", "33", "31", "46", "47", "48"]` | Customizes the available sources for use with HDZone (some AVRs do not support all sources).
+| `zone_1_sources` | list | `[]` | (>0.4) Customises the available sources for use with Zone 1. Defaults to all available sources.
+| `zone_2_sources` | list | `["04", "06", "15", "26", "38", "53", "41", "44", "45", "17", "13", "05", "01", "02", "33", "46", "47", "99", "10"]` | Customises the available sources for use with Zone 2 (some AVRs do not support all sources).
+| `zone_3_sources` | list | `["04", "06", "15", "26", "38", "53", "41", "44", "45", "17", "13", "05", "01", "02", "33", "46", "47", "99", "10"]` | Customises the available sources for use with Zone 3 (some AVRs do not support all sources).
+| `hdzone_sources` | list | `["25", "04", "06", "10", "15", "19", "20", "21", "22", "23", "24", "34", "35", "26", "38", "53", "41", "44", "45", "17", "13", "33", "31", "46", "47", "48"]` | Customises the available sources for use with HDZone (some AVRs do not support all sources).
 | `hdzone_volume_requirements` | list | `["13", "15", "05", "25"]` | A list of sources that HDZone must be set to for volume control, some AVRs do not support HDZone volume at all (see `ignore_volume_check` above) and some only allow control of certain sources.
-| `amplifier_speaker_system_modes` | dict | `....` | Customizes the names of speaker system modes. Different generations of AVR will name zones slighty differently. For example, the SC-LX57 names speaker system mode `15` as `5.1ch Bi-Amp + ZONE2` however this can also be called `5.2ch Bi-Amp + HDZONE` on newer AVRs.
+| `amplifier_speaker_system_modes` | dict | `....` | Customises the names of speaker system modes. Different generations of AVR will name zones slighty differently. For example, the SC-LX57 names speaker system mode `15` as `5.1ch Bi-Amp + ZONE2` however this can also be called `5.2ch Bi-Amp + HDZONE` on newer AVRs.
 | `disabled_amplifier_listening_modes` | list | `[]` | A list of disabled listening modes / sound modes, all modes are enabled by default, some AVRs have definitions already to disable unsupported modes. If you try to change sound mode to a mode that has not been enabled, the AVR will return an error (usually `E02`).
 | `video_resolution_modes` | list | `['0', '1', '3', '4', '5', '6', '7', '8', '9']` | Sets the available video resolutions. Not all AVRs support the same resolution settings. This defaults to all of the latest resolutions from FY16.
 | `mhl_source` | string | `null` | Sets the MHL source ID. This is used for media controls. This information cannot be queried automatically
 | `enabled_functions` | list | `["amp", "dsp", "tuner", "tone", "channels", "video", "system", "audio"]` | Change the functions that are enabled by the API, adding more functions will increase the amount of time it takes to complete a full init and update.
 | `disable_autoquery` | bool | `false` | Setting to `true` will disable auto queries on init for all functions apart from basic functionality (power, source, volume and mute). If you only need those functions, you can set this to `true`
 | `am_frequency_step` | int | `null` | Optional setting to configure the AM frequency step. If this is set to `null`, a function is queued to detect this information by stepping up and down the frequency when the tuner is first used while set to AM.
 | `debug_listener` | bool | `false` | Enables additional debug logging for the listener task.
 | `debug_responder` | bool | `false` | Enables additional debug logging for the responder task.
 | `debug_updater` | bool | `false` | Enables additional debug logging for the updater task.
 | `debug_command` | bool | `false` | Enables additional debug logging for commands sent and responses received.
 
-## Command line interface (CLI) (>= 0.1.3)
+## Command line interface (CLI) (>= 0.1.3, CLI arguments >= 0.3)
 
 A very simple command line interface `aiopioneer` is available to connect to the AVR, send commands and receive responses. It can be used to test the capabilities of the library against your specific AVR.
 
 On Home Assistant, you can run the CLI when the `pioneer_async` Home Assistant integration has been installed. On Home Assistant Supervised or Container, start the CLI from within the HA container: `docker exec -it homeassistant aiopioneer`.
 
-Invoke the CLI with the following optional parameters:
+Invoke the CLI with the following arguments:
 
-| Option | Default | Description
+| Argument | Default | Description
 | --- | --- | ---
 | hostname | required | hostname for AVR connection
 | `-p`<br>`--port` | 8102 | port for AVR connection
 | `+Q`<br>`--no-query-device-info` | None | skip AVR device info query
 | `+Z`<br>`--no-query-zones` | None | skip AVR zone query
 
 The CLI accepts all API commands, as well as the following:
@@ -149,14 +150,17 @@
 
 ## Known issues and future plans
 
 - Document PioneerAVR API
 
 ## Breaking changes
 
+- **0.4**\
+  `zone_z_sources` was renamed `hdzone_sources` for even more consistency.
+
 - **0.3**\
   `zone_h_sources` was renamed `zone_z_sources` for consistency.
 
 - **0.2**\
   `volume_step_delta` has been removed entirely.
 
   By default, a number of additional queries are sent at module startup to the AVR to gather amp, tuner and channel levels attributes. If your AVR does not handle these additional queries well, they can be disabled by setting parameter `disable_autoquery` to `true`.
```

### Comparing `aiopioneer-0.4.0rc1/aiopioneer/cli.py` & `aiopioneer-0.4.1/aiopioneer/cli.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.0rc1/aiopioneer/commands.py` & `aiopioneer-0.4.1/aiopioneer/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,8 +284,10 @@
     "operation_amp_cursor_return": {"1": "CRT"},
     "operation_amp_audio_parameter": {"1": "ATA"},
     "operation_amp_output_parameter": {"1": "HPA"},
     "operation_amp_video_parameter": {"1": "VPA"},
     "operation_amp_channel_select": {"1": "CLC"},
     "operation_amp_home_menu": {"1": "HM"},
     "operation_amp_key_off": {"1": "KOF"},
+    "set_input_name": {"1": ["1RGB", "RGB"]},
+    "set_default_input_name": {"1": ["0RGB", "RGB"]}
 }
```

### Comparing `aiopioneer-0.4.0rc1/aiopioneer/const.py` & `aiopioneer-0.4.1/aiopioneer/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Constants for aiopioneer."""
 
 from enum import Enum
 
 DEFAULT_PORT = 8102
-VERSION = "0.4.0rc1"
+VERSION = "0.4.1"
 
 
 class Zones(Enum):
     """Valid aiopioneer zones"""
 
     Z1 = "1"
     Z2 = "2"
```

### Comparing `aiopioneer-0.4.0rc1/aiopioneer/param.py` & `aiopioneer-0.4.1/aiopioneer/param.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.0rc1/aiopioneer/parsers/audio.py` & `aiopioneer-0.4.1/aiopioneer/parsers/audio.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.0rc1/aiopioneer/parsers/dsp.py` & `aiopioneer-0.4.1/aiopioneer/parsers/dsp.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.0rc1/aiopioneer/parsers/information.py` & `aiopioneer-0.4.1/aiopioneer/parsers/information.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.0rc1/aiopioneer/parsers/parse.py` & `aiopioneer-0.4.1/aiopioneer/parsers/parse.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.0rc1/aiopioneer/parsers/response.py` & `aiopioneer-0.4.1/aiopioneer/parsers/response.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.0rc1/aiopioneer/parsers/settings.py` & `aiopioneer-0.4.1/aiopioneer/parsers/settings.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.0rc1/aiopioneer/parsers/system.py` & `aiopioneer-0.4.1/aiopioneer/parsers/system.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.0rc1/aiopioneer/parsers/tuner.py` & `aiopioneer-0.4.1/aiopioneer/parsers/tuner.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.0rc1/aiopioneer/parsers/video.py` & `aiopioneer-0.4.1/aiopioneer/parsers/video.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.0rc1/aiopioneer/pioneer_avr.py` & `aiopioneer-0.4.1/aiopioneer/pioneer_avr.py`

 * *Files 1% similar despite different names*

```diff
@@ -596,50 +596,51 @@
                         _LOGGER.error(err)
                         return False
                     elif ignore_error:
                         _LOGGER.debug(err)
                         return False
 
     async def send_command(
-        self, command, zone="1", prefix="", ignore_error=None, rate_limit=True
+        self, command, zone="1", prefix="", ignore_error=None, rate_limit=True, suffix=""
     ):
         """Send a command or request to the device."""
         # pylint: disable=unidiomatic-typecheck disable=logging-not-lazy
         debug_command = self._params[PARAM_DEBUG_COMMAND]
         if debug_command:
             _LOGGER.debug(
                 '>> PioneerAVR.send_command("%s", zone="%s", prefix="%s", '
-                + "ignore_error=%s, rate_limit=%s)",
+                + "ignore_error=%s, rate_limit=%s, suffix=%s)",
                 command,
                 zone,
                 prefix,
                 ignore_error,
                 rate_limit,
+                suffix,
             )
         raw_command = PIONEER_COMMANDS.get(command, {}).get(zone)
         try:
             if type(raw_command) is list:
                 if len(raw_command) == 2:
                     # Handle command as request
                     expected_response = raw_command[1]
                     raw_command = raw_command[0]
                     response = await self.send_raw_request(
-                        prefix + raw_command,
+                        prefix + raw_command + suffix,
                         expected_response,
                         ignore_error,
                         rate_limit,
                     )
                     if debug_command:
                         _LOGGER.debug("send_command received response: %s", response)
                     return response
                 else:
                     _LOGGER.error("invalid request %s for zone %s", raw_command, zone)
                     return None
             elif type(raw_command) is str:
-                return await self.send_raw_command(prefix + raw_command, rate_limit)
+                return await self.send_raw_command(prefix + raw_command + suffix, rate_limit)
             else:
                 _LOGGER.warning("invalid command %s for zone %s", command, zone)
                 return None
         except RuntimeError as exc:
             _LOGGER.error("cannot execute %s command: %s", command, exc)
             return False
 
@@ -1363,15 +1364,15 @@
         self._check_zone(zone)
         return await self.send_command("mute_off", zone, ignore_error=False)
 
     async def set_listening_mode(self, listening_mode: str, zone="1"):
         """Set the listening mode using the predefined list of options in params."""
         self._check_zone(zone)
 
-        if self.audio.get(zone).get("input_multichannel"):
+        if self.audio.get("input_multichannel"):
             listening_mode_key = [
                 k
                 for k, v in LISTENING_MODES.items()
                 if bool(v[2]) and v[0] == listening_mode
             ]
         else:
             listening_mode_key = [
@@ -1791,7 +1792,27 @@
                     f"Current source ({self.source.get(zone)} does not support action {action}"
                 )
         else:
             raise NotImplementedError(
                 f"Current source ({self.source.get(zone)}) does not support "
                 "media_control activities."
             )
+
+    async def set_input_name(self, input_id: str, name: str = "", default: bool = False):
+        """Renames a given input, set the default parameter to true to reset to default."""
+        if default:
+            await self.send_command(
+                command="set_default_input_name",
+                zone="1",
+                suffix=input_id)
+        else:
+            if len(name) > 14:
+                raise ValueError(f"New input name ({name}) length too long. "
+                                 "Up to 14 characters are allowed")
+            if self._source_id_to_name.get(input_id) is not name:
+                await self.send_command(
+                    command="set_input_name",
+                    zone="1",
+                    prefix=name,
+                    suffix=input_id
+                )
+        return True
```

### Comparing `aiopioneer-0.4.0rc1/aiopioneer/util.py` & `aiopioneer-0.4.1/aiopioneer/util.py`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.0rc1/aiopioneer.egg-info/PKG-INFO` & `aiopioneer-0.4.1/aiopioneer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopioneer
-Version: 0.4.0rc1
+Version: 0.4.1
 Summary: Asyncio Python library for controlling a Pioneer AVR via its API
 Home-page: https://github.com/crowbarz/aiopioneer.git
 Author: Crowbar Z
 Author-email: crowbarz@outlook.com
 Keywords: pioneer avr asyncio
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
@@ -49,51 +49,52 @@
 
 ## Params
 
 A `params` object may be passed to the library that modifies its functionality.
 
 The default parameters listed below are for AVR models that do not match any custom profile. Custom profiles apply additional default parameters based on the model identifier retrieved from the AVR, and are defined in [`aiopioneer/param.py`](https://github.com/crowbarz/aiopioneer/blob/main/aiopioneer/param.py). If you need to modify parameters for the library to work for your AVR model, then please create a PR to add a custom profile for your AVR model, or log an issue containing your model number and the parameters that were modified requesting a custom profile to be created.
 
-> **NOTE:** YAML syntax is used in the table below. Use Python equivalents (`false` -> `False`, `true` -> `True`, `null` -> `None` etc.) when calling the Python API directly.
+> **NOTE:** YAML syntax is used in the table below. Use Python equivalents (`false` -> `False`, `true` -> `True`, `null` -> `None` etc.) when calling the Python API directly, and JSON syntax if manually specifying via the Home Assistant integration.
 
 | Name | Type | Default | Description
 | ---- | ---- | ------- | -----------
 | `ignored_zones` | list | `[]` | List of zones to ignore even if they are auto-discovered. Specify Zone IDs as strings: "1", "2", "3" and "Z".
 | `command_delay` | float | `0.1` | Insert a delay between sequential commands that are sent to the AVR. This appears to make the AVR behave more reliably during status polls. Increase this value if debug logging shows that your AVR times out between commands.
 | `max_source_id` | int | `60` | Maximum source ID that the source discovery queries. Reduce this if your AVR returns errors.
 | `max_volume` | int | `185` | Maximum volume for the Main Zone.
 | `max_volume_zonex` | int | `185` | Maximum volume for zones other than the Main Zone.
 | `power_on_volume_bounce` | bool | `false` | On some AVRs (eg. VSX-930) where a power-on is set, the initial volume is not reported by the AVR correctly until a volume change is made. This option enables a workaround that sends a volume up and down command to the AVR on power-on to correct the reported volume without affecting the power-on volume.
 | `volume_step_only` | bool | `false` | On some AVRs (eg. VSX-S510), setting the volume level is not supported natively by the API. This option emulates setting the volume level using volume up and down commands.
 | `ignore_volume_check` | bool | `false` | Don't check volume when determining whether a zone exists on the AVR. Useful for AVRs with an HDZone that passes through audio.
-| `zone_2_sources` | list | `["04", "06", "15", "26", "38", "53", "41", "44", "45", "17", "13", "05", "01", "02", "33", "46", "47", "99", "10"]` | Customizes the available sources for use with Zone 2 (some AVRs do not support all sources).
-| `zone_3_sources` | list | `["04", "06", "15", "26", "38", "53", "41", "44", "45", "17", "13", "05", "01", "02", "33", "46", "47", "99", "10"]` | Customizes the available sources for use with Zone 3 (some AVRs do not support all sources).
-| `zone_z_sources` | list | `["25", "04", "06", "10", "15", "19", "20", "21", "22", "23", "24", "34", "35", "26", "38", "53", "41", "44", "45", "17", "13", "33", "31", "46", "47", "48"]` | Customizes the available sources for use with HDZone (some AVRs do not support all sources).
+| `zone_1_sources` | list | `[]` | (>0.4) Customises the available sources for use with Zone 1. Defaults to all available sources.
+| `zone_2_sources` | list | `["04", "06", "15", "26", "38", "53", "41", "44", "45", "17", "13", "05", "01", "02", "33", "46", "47", "99", "10"]` | Customises the available sources for use with Zone 2 (some AVRs do not support all sources).
+| `zone_3_sources` | list | `["04", "06", "15", "26", "38", "53", "41", "44", "45", "17", "13", "05", "01", "02", "33", "46", "47", "99", "10"]` | Customises the available sources for use with Zone 3 (some AVRs do not support all sources).
+| `hdzone_sources` | list | `["25", "04", "06", "10", "15", "19", "20", "21", "22", "23", "24", "34", "35", "26", "38", "53", "41", "44", "45", "17", "13", "33", "31", "46", "47", "48"]` | Customises the available sources for use with HDZone (some AVRs do not support all sources).
 | `hdzone_volume_requirements` | list | `["13", "15", "05", "25"]` | A list of sources that HDZone must be set to for volume control, some AVRs do not support HDZone volume at all (see `ignore_volume_check` above) and some only allow control of certain sources.
-| `amplifier_speaker_system_modes` | dict | `....` | Customizes the names of speaker system modes. Different generations of AVR will name zones slighty differently. For example, the SC-LX57 names speaker system mode `15` as `5.1ch Bi-Amp + ZONE2` however this can also be called `5.2ch Bi-Amp + HDZONE` on newer AVRs.
+| `amplifier_speaker_system_modes` | dict | `....` | Customises the names of speaker system modes. Different generations of AVR will name zones slighty differently. For example, the SC-LX57 names speaker system mode `15` as `5.1ch Bi-Amp + ZONE2` however this can also be called `5.2ch Bi-Amp + HDZONE` on newer AVRs.
 | `disabled_amplifier_listening_modes` | list | `[]` | A list of disabled listening modes / sound modes, all modes are enabled by default, some AVRs have definitions already to disable unsupported modes. If you try to change sound mode to a mode that has not been enabled, the AVR will return an error (usually `E02`).
 | `video_resolution_modes` | list | `['0', '1', '3', '4', '5', '6', '7', '8', '9']` | Sets the available video resolutions. Not all AVRs support the same resolution settings. This defaults to all of the latest resolutions from FY16.
 | `mhl_source` | string | `null` | Sets the MHL source ID. This is used for media controls. This information cannot be queried automatically
 | `enabled_functions` | list | `["amp", "dsp", "tuner", "tone", "channels", "video", "system", "audio"]` | Change the functions that are enabled by the API, adding more functions will increase the amount of time it takes to complete a full init and update.
 | `disable_autoquery` | bool | `false` | Setting to `true` will disable auto queries on init for all functions apart from basic functionality (power, source, volume and mute). If you only need those functions, you can set this to `true`
 | `am_frequency_step` | int | `null` | Optional setting to configure the AM frequency step. If this is set to `null`, a function is queued to detect this information by stepping up and down the frequency when the tuner is first used while set to AM.
 | `debug_listener` | bool | `false` | Enables additional debug logging for the listener task.
 | `debug_responder` | bool | `false` | Enables additional debug logging for the responder task.
 | `debug_updater` | bool | `false` | Enables additional debug logging for the updater task.
 | `debug_command` | bool | `false` | Enables additional debug logging for commands sent and responses received.
 
-## Command line interface (CLI) (>= 0.1.3)
+## Command line interface (CLI) (>= 0.1.3, CLI arguments >= 0.3)
 
 A very simple command line interface `aiopioneer` is available to connect to the AVR, send commands and receive responses. It can be used to test the capabilities of the library against your specific AVR.
 
 On Home Assistant, you can run the CLI when the `pioneer_async` Home Assistant integration has been installed. On Home Assistant Supervised or Container, start the CLI from within the HA container: `docker exec -it homeassistant aiopioneer`.
 
-Invoke the CLI with the following optional parameters:
+Invoke the CLI with the following arguments:
 
-| Option | Default | Description
+| Argument | Default | Description
 | --- | --- | ---
 | hostname | required | hostname for AVR connection
 | `-p`<br>`--port` | 8102 | port for AVR connection
 | `+Q`<br>`--no-query-device-info` | None | skip AVR device info query
 | `+Z`<br>`--no-query-zones` | None | skip AVR zone query
 
 The CLI accepts all API commands, as well as the following:
@@ -167,14 +168,17 @@
 
 ## Known issues and future plans
 
 - Document PioneerAVR API
 
 ## Breaking changes
 
+- **0.4**\
+  `zone_z_sources` was renamed `hdzone_sources` for even more consistency.
+
 - **0.3**\
   `zone_h_sources` was renamed `zone_z_sources` for consistency.
 
 - **0.2**\
   `volume_step_delta` has been removed entirely.
 
   By default, a number of additional queries are sent at module startup to the AVR to gather amp, tuner and channel levels attributes. If your AVR does not handle these additional queries well, they can be disabled by setting parameter `disable_autoquery` to `true`.
```

### Comparing `aiopioneer-0.4.0rc1/aiopioneer.egg-info/SOURCES.txt` & `aiopioneer-0.4.1/aiopioneer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiopioneer-0.4.0rc1/setup.py` & `aiopioneer-0.4.1/setup.py`

 * *Files identical despite different names*

