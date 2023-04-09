# Comparing `tmp/tuneflow-py-0.4.5.tar.gz` & `tmp/tuneflow-py-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneflow-py-0.4.5.tar", last modified: Sun Apr  9 01:20:10 2023, max compression
+gzip compressed data, was "tuneflow-py-0.4.6.tar", last modified: Sun Apr  9 02:41:02 2023, max compression
```

## Comparing `tuneflow-py-0.4.5.tar` & `tuneflow-py-0.4.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 01:20:10.869295 tuneflow-py-0.4.5/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1065 2023-01-10 14:03:44.000000 tuneflow-py-0.4.5/LICENSE
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-09 01:20:10.869295 tuneflow-py-0.4.5/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3809 2023-03-06 23:39:23.000000 tuneflow-py-0.4.5/README.md
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1288 2023-04-09 01:19:44.000000 tuneflow-py-0.4.5/pyproject.toml
--rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-04-09 01:20:10.869295 tuneflow-py-0.4.5/setup.cfg
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 01:20:10.859295 tuneflow-py-0.4.5/src/
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 01:20:10.859295 tuneflow-py-0.4.5/src/tuneflow_py/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1086 2023-03-31 16:35:25.000000 tuneflow-py-0.4.5/src/tuneflow_py/__init__.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1987 2023-02-28 00:04:43.000000 tuneflow-py-0.4.5/src/tuneflow_py/base_plugin.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 01:20:10.869295 tuneflow-py-0.4.5/src/tuneflow_py/descriptors/
--rw-r--r--   0 panacea   (1000) panacea   (1000)      922 2023-03-30 21:40:36.000000 tuneflow-py-0.4.5/src/tuneflow_py/descriptors/audio_plugin_descriptor.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1579 2023-03-30 21:53:02.000000 tuneflow-py-0.4.5/src/tuneflow_py/descriptors/clip_descriptor.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      439 2023-03-30 21:53:05.000000 tuneflow-py-0.4.5/src/tuneflow_py/descriptors/common.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4221 2023-03-30 21:53:07.000000 tuneflow-py-0.4.5/src/tuneflow_py/descriptors/param.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4407 2023-03-30 21:53:10.000000 tuneflow-py-0.4.5/src/tuneflow_py/descriptors/plugin.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)       71 2023-03-30 21:53:12.000000 tuneflow-py-0.4.5/src/tuneflow_py/descriptors/text.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     5575 2023-03-31 22:25:01.000000 tuneflow-py-0.4.5/src/tuneflow_py/descriptors/widget.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 01:20:10.869295 tuneflow-py-0.4.5/src/tuneflow_py/models/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3128 2023-03-01 03:02:02.000000 tuneflow-py-0.4.5/src/tuneflow_py/models/audio_plugin.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    17158 2023-03-31 07:33:41.000000 tuneflow-py-0.4.5/src/tuneflow_py/models/automation.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    23875 2023-03-31 07:45:07.000000 tuneflow-py-0.4.5/src/tuneflow_py/models/clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     5275 2023-02-22 00:50:28.000000 tuneflow-py-0.4.5/src/tuneflow_py/models/note.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 01:20:10.869295 tuneflow-py-0.4.5/src/tuneflow_py/models/protos/
--rw-r--r--   0 panacea   (1000) panacea   (1000)    69366 2023-03-31 16:43:26.000000 tuneflow-py-0.4.5/src/tuneflow_py/models/protos/song_pb2.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    22269 2023-04-05 05:19:38.000000 tuneflow-py-0.4.5/src/tuneflow_py/models/song.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      873 2023-03-01 22:09:14.000000 tuneflow-py-0.4.5/src/tuneflow_py/models/tempo.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1093 2023-02-22 00:28:50.000000 tuneflow-py-0.4.5/src/tuneflow_py/models/time_signature.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    16387 2023-03-31 16:53:25.000000 tuneflow-py-0.4.5/src/tuneflow_py/models/track.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     6210 2023-03-29 01:48:05.000000 tuneflow-py-0.4.5/src/tuneflow_py/utils.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 01:20:10.869295 tuneflow-py-0.4.5/src/tuneflow_py.egg-info/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-09 01:20:10.000000 tuneflow-py-0.4.5/src/tuneflow_py.egg-info/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1060 2023-04-09 01:20:10.000000 tuneflow-py-0.4.5/src/tuneflow_py.egg-info/SOURCES.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-04-09 01:20:10.000000 tuneflow-py-0.4.5/src/tuneflow_py.egg-info/dependency_links.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       96 2023-04-09 01:20:10.000000 tuneflow-py-0.4.5/src/tuneflow_py.egg-info/requires.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       12 2023-04-09 01:20:10.000000 tuneflow-py-0.4.5/src/tuneflow_py.egg-info/top_level.txt
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 01:20:10.869295 tuneflow-py-0.4.5/test/
--rw-r--r--   0 panacea   (1000) panacea   (1000)    21690 2023-02-24 04:10:42.000000 tuneflow-py-0.4.5/test/test_audio_clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    24170 2023-03-31 07:02:16.000000 tuneflow-py-0.4.5/test/test_automation.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    33568 2023-03-09 18:17:16.000000 tuneflow-py-0.4.5/test/test_midi_clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    24300 2023-02-22 00:33:25.000000 tuneflow-py-0.4.5/test/test_note.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    14091 2023-03-31 16:54:59.000000 tuneflow-py-0.4.5/test/test_song.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3583 2023-03-31 08:05:14.000000 tuneflow-py-0.4.5/test/test_track.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2071 2023-02-16 23:10:13.000000 tuneflow-py-0.4.5/test/test_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 02:41:02.839069 tuneflow-py-0.4.6/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1065 2023-01-10 14:03:44.000000 tuneflow-py-0.4.6/LICENSE
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-09 02:41:02.839069 tuneflow-py-0.4.6/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3809 2023-03-06 23:39:23.000000 tuneflow-py-0.4.6/README.md
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1288 2023-04-09 02:35:25.000000 tuneflow-py-0.4.6/pyproject.toml
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-04-09 02:41:02.839069 tuneflow-py-0.4.6/setup.cfg
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 02:41:02.839069 tuneflow-py-0.4.6/src/
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 02:41:02.839069 tuneflow-py-0.4.6/src/tuneflow_py/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1086 2023-03-31 16:35:25.000000 tuneflow-py-0.4.6/src/tuneflow_py/__init__.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1987 2023-02-28 00:04:43.000000 tuneflow-py-0.4.6/src/tuneflow_py/base_plugin.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 02:41:02.839069 tuneflow-py-0.4.6/src/tuneflow_py/descriptors/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      922 2023-03-30 21:40:36.000000 tuneflow-py-0.4.6/src/tuneflow_py/descriptors/audio_plugin_descriptor.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1579 2023-03-30 21:53:02.000000 tuneflow-py-0.4.6/src/tuneflow_py/descriptors/clip_descriptor.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      439 2023-03-30 21:53:05.000000 tuneflow-py-0.4.6/src/tuneflow_py/descriptors/common.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4221 2023-03-30 21:53:07.000000 tuneflow-py-0.4.6/src/tuneflow_py/descriptors/param.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4407 2023-03-30 21:53:10.000000 tuneflow-py-0.4.6/src/tuneflow_py/descriptors/plugin.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       71 2023-03-30 21:53:12.000000 tuneflow-py-0.4.6/src/tuneflow_py/descriptors/text.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5575 2023-03-31 22:25:01.000000 tuneflow-py-0.4.6/src/tuneflow_py/descriptors/widget.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 02:41:02.839069 tuneflow-py-0.4.6/src/tuneflow_py/models/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3128 2023-03-01 03:02:02.000000 tuneflow-py-0.4.6/src/tuneflow_py/models/audio_plugin.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    17158 2023-03-31 07:33:41.000000 tuneflow-py-0.4.6/src/tuneflow_py/models/automation.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    23875 2023-03-31 07:45:07.000000 tuneflow-py-0.4.6/src/tuneflow_py/models/clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5275 2023-02-22 00:50:28.000000 tuneflow-py-0.4.6/src/tuneflow_py/models/note.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 02:41:02.839069 tuneflow-py-0.4.6/src/tuneflow_py/models/protos/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    69366 2023-03-31 16:43:26.000000 tuneflow-py-0.4.6/src/tuneflow_py/models/protos/song_pb2.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    22269 2023-04-05 05:19:38.000000 tuneflow-py-0.4.6/src/tuneflow_py/models/song.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      873 2023-03-01 22:09:14.000000 tuneflow-py-0.4.6/src/tuneflow_py/models/tempo.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1093 2023-02-22 00:28:50.000000 tuneflow-py-0.4.6/src/tuneflow_py/models/time_signature.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    16387 2023-03-31 16:53:25.000000 tuneflow-py-0.4.6/src/tuneflow_py/models/track.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     6210 2023-03-29 01:48:05.000000 tuneflow-py-0.4.6/src/tuneflow_py/utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 02:41:02.839069 tuneflow-py-0.4.6/src/tuneflow_py.egg-info/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-09 02:41:02.000000 tuneflow-py-0.4.6/src/tuneflow_py.egg-info/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1060 2023-04-09 02:41:02.000000 tuneflow-py-0.4.6/src/tuneflow_py.egg-info/SOURCES.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-04-09 02:41:02.000000 tuneflow-py-0.4.6/src/tuneflow_py.egg-info/dependency_links.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       96 2023-04-09 02:41:02.000000 tuneflow-py-0.4.6/src/tuneflow_py.egg-info/requires.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       12 2023-04-09 02:41:02.000000 tuneflow-py-0.4.6/src/tuneflow_py.egg-info/top_level.txt
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-09 02:41:02.839069 tuneflow-py-0.4.6/test/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    21690 2023-02-24 04:10:42.000000 tuneflow-py-0.4.6/test/test_audio_clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    24170 2023-03-31 07:02:16.000000 tuneflow-py-0.4.6/test/test_automation.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    33568 2023-03-09 18:17:16.000000 tuneflow-py-0.4.6/test/test_midi_clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    24300 2023-02-22 00:33:25.000000 tuneflow-py-0.4.6/test/test_note.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    14091 2023-03-31 16:54:59.000000 tuneflow-py-0.4.6/test/test_song.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3583 2023-03-31 08:05:14.000000 tuneflow-py-0.4.6/test/test_track.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2071 2023-02-16 23:10:13.000000 tuneflow-py-0.4.6/test/test_utils.py
```

### Comparing `tuneflow-py-0.4.5/LICENSE` & `tuneflow-py-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/PKG-INFO` & `tuneflow-py-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-py
-Version: 0.4.5
+Version: 0.4.6
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: TuneFlow <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-py-0.4.5/README.md` & `tuneflow-py-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/pyproject.toml` & `tuneflow-py-0.4.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "tuneflow-py"
-version = "0.4.5"
+version = "0.4.6"
 authors = [{ name = "TuneFlow", email = "contact@info.tuneflow.com" }]
 description = "Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = [
   "AI",
   "music",
@@ -29,15 +29,15 @@
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 dependencies = [
   'protobuf <= 3.19.4',
   'nanoid >= 2.0.0',
-  'numpy>=1.20.0',
+  'numpy>=1.19.0',
   'miditoolkit-light >= 0.1.19',
   'typing_extensions >= 4.5.0'
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/tuneflow/tuneflow-py"
 "Bug Tracker" = "https://github.com/tuneflow/tuneflow-py/issues"
```

### Comparing `tuneflow-py-0.4.5/src/tuneflow_py/__init__.py` & `tuneflow-py-0.4.6/src/tuneflow_py/__init__.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/src/tuneflow_py/base_plugin.py` & `tuneflow-py-0.4.6/src/tuneflow_py/base_plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/src/tuneflow_py/descriptors/audio_plugin_descriptor.py` & `tuneflow-py-0.4.6/src/tuneflow_py/descriptors/audio_plugin_descriptor.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/src/tuneflow_py/descriptors/clip_descriptor.py` & `tuneflow-py-0.4.6/src/tuneflow_py/descriptors/clip_descriptor.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/src/tuneflow_py/descriptors/param.py` & `tuneflow-py-0.4.6/src/tuneflow_py/descriptors/param.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/src/tuneflow_py/descriptors/plugin.py` & `tuneflow-py-0.4.6/src/tuneflow_py/descriptors/plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/src/tuneflow_py/descriptors/widget.py` & `tuneflow-py-0.4.6/src/tuneflow_py/descriptors/widget.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/src/tuneflow_py/models/audio_plugin.py` & `tuneflow-py-0.4.6/src/tuneflow_py/models/audio_plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/src/tuneflow_py/models/automation.py` & `tuneflow-py-0.4.6/src/tuneflow_py/models/automation.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/src/tuneflow_py/models/clip.py` & `tuneflow-py-0.4.6/src/tuneflow_py/models/clip.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/src/tuneflow_py/models/note.py` & `tuneflow-py-0.4.6/src/tuneflow_py/models/note.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/src/tuneflow_py/models/protos/song_pb2.py` & `tuneflow-py-0.4.6/src/tuneflow_py/models/protos/song_pb2.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/src/tuneflow_py/models/song.py` & `tuneflow-py-0.4.6/src/tuneflow_py/models/song.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/src/tuneflow_py/models/tempo.py` & `tuneflow-py-0.4.6/src/tuneflow_py/models/tempo.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/src/tuneflow_py/models/time_signature.py` & `tuneflow-py-0.4.6/src/tuneflow_py/models/time_signature.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/src/tuneflow_py/models/track.py` & `tuneflow-py-0.4.6/src/tuneflow_py/models/track.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/src/tuneflow_py/utils.py` & `tuneflow-py-0.4.6/src/tuneflow_py/utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/src/tuneflow_py.egg-info/PKG-INFO` & `tuneflow-py-0.4.6/src/tuneflow_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-py
-Version: 0.4.5
+Version: 0.4.6
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: TuneFlow <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-py-0.4.5/src/tuneflow_py.egg-info/SOURCES.txt` & `tuneflow-py-0.4.6/src/tuneflow_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/test/test_audio_clip.py` & `tuneflow-py-0.4.6/test/test_audio_clip.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/test/test_automation.py` & `tuneflow-py-0.4.6/test/test_automation.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/test/test_midi_clip.py` & `tuneflow-py-0.4.6/test/test_midi_clip.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/test/test_note.py` & `tuneflow-py-0.4.6/test/test_note.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/test/test_song.py` & `tuneflow-py-0.4.6/test/test_song.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/test/test_track.py` & `tuneflow-py-0.4.6/test/test_track.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.4.5/test/test_utils.py` & `tuneflow-py-0.4.6/test/test_utils.py`

 * *Files identical despite different names*

