# Comparing `tmp/ovos-vad-plugin-silero-0.0.1.tar.gz` & `tmp/ovos-vad-plugin-silero-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-vad-plugin-silero-0.0.1.tar", last modified: Sun Apr  9 18:05:33 2023, max compression
+gzip compressed data, was "ovos-vad-plugin-silero-0.0.1a2.tar", last modified: Sun Apr  9 18:03:59 2023, max compression
```

## Comparing `ovos-vad-plugin-silero-0.0.1.tar` & `ovos-vad-plugin-silero-0.0.1a2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:05:33.125702 ovos-vad-plugin-silero-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-09 18:05:33.125702 ovos-vad-plugin-silero-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:05:33.121702 ovos-vad-plugin-silero-0.0.1/ovos_vad_plugin_silero/
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-09 18:05:25.000000 ovos-vad-plugin-silero-0.0.1/ovos_vad_plugin_silero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   797513 2023-04-09 18:05:25.000000 ovos-vad-plugin-silero-0.0.1/ovos_vad_plugin_silero/silero_vad.onnx
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-09 18:05:27.000000 ovos-vad-plugin-silero-0.0.1/ovos_vad_plugin_silero/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:05:33.125702 ovos-vad-plugin-silero-0.0.1/ovos_vad_plugin_silero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-09 18:05:33.000000 ovos-vad-plugin-silero-0.0.1/ovos_vad_plugin_silero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-09 18:05:33.000000 ovos-vad-plugin-silero-0.0.1/ovos_vad_plugin_silero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 18:05:33.000000 ovos-vad-plugin-silero-0.0.1/ovos_vad_plugin_silero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-09 18:05:33.000000 ovos-vad-plugin-silero-0.0.1/ovos_vad_plugin_silero.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-09 18:05:33.000000 ovos-vad-plugin-silero-0.0.1/ovos_vad_plugin_silero.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-09 18:05:33.000000 ovos-vad-plugin-silero-0.0.1/ovos_vad_plugin_silero.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 18:05:33.000000 ovos-vad-plugin-silero-0.0.1/ovos_vad_plugin_silero.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 18:05:33.125702 ovos-vad-plugin-silero-0.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3147 2023-04-09 18:05:25.000000 ovos-vad-plugin-silero-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:59.066524 ovos-vad-plugin-silero-0.0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-09 18:03:59.066524 ovos-vad-plugin-silero-0.0.1a2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:59.062524 ovos-vad-plugin-silero-0.0.1a2/ovos_vad_plugin_silero/
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-09 18:03:46.000000 ovos-vad-plugin-silero-0.0.1a2/ovos_vad_plugin_silero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   797513 2023-04-09 18:03:46.000000 ovos-vad-plugin-silero-0.0.1a2/ovos_vad_plugin_silero/silero_vad.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-09 18:03:53.000000 ovos-vad-plugin-silero-0.0.1a2/ovos_vad_plugin_silero/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 18:03:59.066524 ovos-vad-plugin-silero-0.0.1a2/ovos_vad_plugin_silero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-09 18:03:58.000000 ovos-vad-plugin-silero-0.0.1a2/ovos_vad_plugin_silero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-09 18:03:59.000000 ovos-vad-plugin-silero-0.0.1a2/ovos_vad_plugin_silero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 18:03:58.000000 ovos-vad-plugin-silero-0.0.1a2/ovos_vad_plugin_silero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-09 18:03:58.000000 ovos-vad-plugin-silero-0.0.1a2/ovos_vad_plugin_silero.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-09 18:03:58.000000 ovos-vad-plugin-silero-0.0.1a2/ovos_vad_plugin_silero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-09 18:03:58.000000 ovos-vad-plugin-silero-0.0.1a2/ovos_vad_plugin_silero.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 18:03:58.000000 ovos-vad-plugin-silero-0.0.1a2/ovos_vad_plugin_silero.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 18:03:59.066524 ovos-vad-plugin-silero-0.0.1a2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3147 2023-04-09 18:03:46.000000 ovos-vad-plugin-silero-0.0.1a2/setup.py
```

### Comparing `ovos-vad-plugin-silero-0.0.1/PKG-INFO` & `ovos-vad-plugin-silero-0.0.1a2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-vad-plugin-silero
-Version: 0.0.1
+Version: 0.0.1a2
 Summary: silero VAD plugin for OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/ovos-vad-plugin-silero
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft plugin VAD OVOS OpenVoiceOS
```

### Comparing `ovos-vad-plugin-silero-0.0.1/ovos_vad_plugin_silero/__init__.py` & `ovos-vad-plugin-silero-0.0.1a2/ovos_vad_plugin_silero/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-vad-plugin-silero-0.0.1/ovos_vad_plugin_silero/silero_vad.onnx` & `ovos-vad-plugin-silero-0.0.1a2/ovos_vad_plugin_silero/silero_vad.onnx`

 * *Files identical despite different names*

### Comparing `ovos-vad-plugin-silero-0.0.1/ovos_vad_plugin_silero.egg-info/PKG-INFO` & `ovos-vad-plugin-silero-0.0.1a2/ovos_vad_plugin_silero.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-vad-plugin-silero
-Version: 0.0.1
+Version: 0.0.1a2
 Summary: silero VAD plugin for OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/ovos-vad-plugin-silero
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft plugin VAD OVOS OpenVoiceOS
```

### Comparing `ovos-vad-plugin-silero-0.0.1/setup.py` & `ovos-vad-plugin-silero-0.0.1a2/setup.py`

 * *Files identical despite different names*

