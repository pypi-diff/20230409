# Comparing `tmp/ovos-vad-plugin-webrtcvad-0.0.1a1.tar.gz` & `tmp/ovos-vad-plugin-webrtcvad-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-vad-plugin-webrtcvad-0.0.1a1.tar", last modified: Thu Sep  8 11:10:52 2022, max compression
+gzip compressed data, was "ovos-vad-plugin-webrtcvad-0.0.1a2.tar", last modified: Sun Apr  9 18:08:12 2023, max compression
```

## Comparing `ovos-vad-plugin-webrtcvad-0.0.1a1.tar` & `ovos-vad-plugin-webrtcvad-0.0.1a2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 11:10:52.153913 ovos-vad-plugin-webrtcvad-0.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-09-08 11:10:52.153913 ovos-vad-plugin-webrtcvad-0.0.1a1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 11:10:52.153913 ovos-vad-plugin-webrtcvad-0.0.1a1/ovos_vad_plugin_webrtcvad/
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-09-08 11:10:41.000000 ovos-vad-plugin-webrtcvad-0.0.1a1/ovos_vad_plugin_webrtcvad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-09-08 11:10:44.000000 ovos-vad-plugin-webrtcvad-0.0.1a1/ovos_vad_plugin_webrtcvad/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 11:10:52.153913 ovos-vad-plugin-webrtcvad-0.0.1a1/ovos_vad_plugin_webrtcvad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-09-08 11:10:51.000000 ovos-vad-plugin-webrtcvad-0.0.1a1/ovos_vad_plugin_webrtcvad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-09-08 11:10:52.000000 ovos-vad-plugin-webrtcvad-0.0.1a1/ovos_vad_plugin_webrtcvad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 11:10:51.000000 ovos-vad-plugin-webrtcvad-0.0.1a1/ovos_vad_plugin_webrtcvad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-09-08 11:10:51.000000 ovos-vad-plugin-webrtcvad-0.0.1a1/ovos_vad_plugin_webrtcvad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-08 11:10:51.000000 ovos-vad-plugin-webrtcvad-0.0.1a1/ovos_vad_plugin_webrtcvad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-09-08 11:10:51.000000 ovos-vad-plugin-webrtcvad-0.0.1a1/ovos_vad_plugin_webrtcvad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 11:10:51.000000 ovos-vad-plugin-webrtcvad-0.0.1a1/ovos_vad_plugin_webrtcvad.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-08 11:10:52.153913 ovos-vad-plugin-webrtcvad-0.0.1a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     3102 2022-09-08 11:10:41.000000 ovos-vad-plugin-webrtcvad-0.0.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:08:12.441069 ovos-vad-plugin-webrtcvad-0.0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-09 18:08:12.441069 ovos-vad-plugin-webrtcvad-0.0.1a2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:08:12.441069 ovos-vad-plugin-webrtcvad-0.0.1a2/ovos_vad_plugin_webrtcvad/
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-04-09 18:08:02.000000 ovos-vad-plugin-webrtcvad-0.0.1a2/ovos_vad_plugin_webrtcvad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-09 18:08:06.000000 ovos-vad-plugin-webrtcvad-0.0.1a2/ovos_vad_plugin_webrtcvad/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:08:12.441069 ovos-vad-plugin-webrtcvad-0.0.1a2/ovos_vad_plugin_webrtcvad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-09 18:08:12.000000 ovos-vad-plugin-webrtcvad-0.0.1a2/ovos_vad_plugin_webrtcvad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-09 18:08:12.000000 ovos-vad-plugin-webrtcvad-0.0.1a2/ovos_vad_plugin_webrtcvad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 18:08:12.000000 ovos-vad-plugin-webrtcvad-0.0.1a2/ovos_vad_plugin_webrtcvad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-09 18:08:12.000000 ovos-vad-plugin-webrtcvad-0.0.1a2/ovos_vad_plugin_webrtcvad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 18:08:12.000000 ovos-vad-plugin-webrtcvad-0.0.1a2/ovos_vad_plugin_webrtcvad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-09 18:08:12.000000 ovos-vad-plugin-webrtcvad-0.0.1a2/ovos_vad_plugin_webrtcvad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 18:08:12.000000 ovos-vad-plugin-webrtcvad-0.0.1a2/ovos_vad_plugin_webrtcvad.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 18:08:12.441069 ovos-vad-plugin-webrtcvad-0.0.1a2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3102 2023-04-09 18:08:02.000000 ovos-vad-plugin-webrtcvad-0.0.1a2/setup.py
```

### Comparing `ovos-vad-plugin-webrtcvad-0.0.1a1/PKG-INFO` & `ovos-vad-plugin-webrtcvad-0.0.1a2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-vad-plugin-webrtcvad
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: webrtcvad VAD plugin for OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/ovos-vad-plugin-webrtcvad
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft plugin VAD OVOS OpenVoiceOS
```

### Comparing `ovos-vad-plugin-webrtcvad-0.0.1a1/ovos_vad_plugin_webrtcvad.egg-info/PKG-INFO` & `ovos-vad-plugin-webrtcvad-0.0.1a2/ovos_vad_plugin_webrtcvad.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-vad-plugin-webrtcvad
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: webrtcvad VAD plugin for OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/ovos-vad-plugin-webrtcvad
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft plugin VAD OVOS OpenVoiceOS
```

### Comparing `ovos-vad-plugin-webrtcvad-0.0.1a1/setup.py` & `ovos-vad-plugin-webrtcvad-0.0.1a2/setup.py`

 * *Files identical despite different names*

