# Comparing `tmp/f1_22_telemetry-0.1.1.tar.gz` & `tmp/f1_22_telemetry-0.1.2.tar.gz`

## Comparing `f1_22_telemetry-0.1.1.tar` & `f1_22_telemetry-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.1/setup.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.1/test_requirements.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.1/f1_22_telemetry/__init__.py
--rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.1/f1_22_telemetry/appendices.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.1/f1_22_telemetry/listener.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.1/f1_22_telemetry/main.py
--rw-r--r--   0        0        0    34843 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.1/f1_22_telemetry/packets.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.1/LICENSE
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.1/README.md
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.2/.pdm-python
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    24554 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.2/1
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0   108366 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.2/pdm.lock
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.2/setup.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.2/test_requirements.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.2/f1_22_telemetry/__init__.py
+-rw-r--r--   0        0        0    14212 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.2/f1_22_telemetry/appendices.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.2/f1_22_telemetry/listener.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.2/f1_22_telemetry/main.py
+-rw-r--r--   0        0        0    34843 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.2/f1_22_telemetry/packets.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.2/LICENSE
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.2/README.md
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 f1_22_telemetry-0.1.2/PKG-INFO
```

### Comparing `f1_22_telemetry-0.1.1/.pre-commit-config.yaml` & `f1_22_telemetry-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `f1_22_telemetry-0.1.1/setup.py` & `f1_22_telemetry-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `f1_22_telemetry-0.1.1/f1_22_telemetry/appendices.py` & `f1_22_telemetry-0.1.2/f1_22_telemetry/appendices.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 More info is available here:
-https://answers.ea.com/t5/General-Discussion/F1-22-UDP-Specification/td-p/11551274?attachment-id=607611
+https://answers.ea.com/t5/General-Discussion/F1-22-UDP-Specification/td-p/11551274?attachment-id=657933
 """
 
-
 TEAM_IDS = {
     0: 'Mercedes',
     1: 'Ferrari',
     2: 'Red Bull Racing',
     3: 'Williams',
     4: 'Aston Martin',
     5: 'Alpine',
@@ -43,17 +42,27 @@
     111: 'MP Motorsport ‘21',
     112: 'Charouz ‘21',
     113: 'Dams ‘21',
     114: 'Campos ‘21',
     115: 'BWT ‘21',
     116: 'Trident ‘21',
     117: 'Mercedes AMG GT Black Series',
+    118: "Prema ‘22",
+    119: "Virtuosi ‘22",
+    120: "Carlin ‘22",
+    121: "Hitech ‘22",
+    122: "Art GP ‘22",
+    123: "MP Motorsport ‘22",
+    124: "Charouz ‘22",
+    125: "Dams ‘22",
+    126: "Campos ‘22",
+    127: "Van Amersfoort Racing ‘22",
+    128: "Trident ‘22",
 }
 
-
 DRIVER_IDS = {
     0: 'Carlos Sainz',
     1: 'Daniil Kvyat',
     2: 'Daniel Ricciardo',
     3: 'Fernando Alonso',
     4: 'Felipe Massa',
     6: 'Kimi Räikkönen',
@@ -171,17 +180,17 @@
     131: "Cem Bölükbasi",
     132: "Ayumu Iwasa",
     133: "Clément Novalak",
     134: "Dennis Hauger",
     135: "Calan Williams",
     136: "Jack Doohan",
     137: "Amaury Cordeel",
+    138: "Mika Hakkinen",
 }
 
-
 TRACK_IDS = {
     0: 'Melbourne',
     1: 'Paul Ricard',
     2: 'Shanghai',
     3: 'Sakhir (Bahrain)',
     4: 'Catalunya',
     5: 'Monaco',
@@ -208,15 +217,14 @@
     26: 'Zandvoort',
     27: 'Imola',
     28: 'Portimão',
     29: 'Jeddah',
     30: 'Miami',
 }
 
-
 NATIONALITY_IDS = {
     1: 'American',
     2: 'Argentinean',
     3: 'Australian',
     4: 'Austrian',
     5: 'Azerbaijani',
     6: 'Bahraini',
@@ -299,16 +307,15 @@
     83: 'Ukrainian',
     84: 'Venezuelan',
     85: 'Barbadian',
     86: 'Welsh',
     87: 'Vietnamese',
 }
 
-
-GAME_MODE = {
+GAME_MODE_IDS = {
     0: 'Event Mode',
     3: 'Grand Prix',
     5: 'Time Trial',
     6: 'Splitscreen',
     7: 'Online Custom',
     8: 'Online League',
     11: 'Career Invitational',
@@ -317,44 +324,41 @@
     14: 'Online Championship',
     15: 'Online Weekly Event',
     19: 'Career ‘22',
     20: 'Career ’22 Online',
     127: 'Benchmark',
 }
 
-
 RULESET_IDS = {
     0: 'Practice & Qualifying',
     1: 'Race',
     2: 'Time Trial',
     4: 'Time Attack',
     6: 'Checkpoint Challenge',
     8: 'Autocross',
     9: 'Drift',
     10: 'Average Speed Zone',
     11: 'Rival Duel',
 }
 
-
 SURFACE_TYPES = {
     0: 'Tarmac',
     1: 'Rumble strip',
     2: 'Concrete',
     3: 'Rock',
     4: 'Gravel',
     5: 'Mud',
     6: 'Sand',
     7: 'Grass',
     8: 'Water',
     9: 'Cobblestone',
     10: 'Metal',
-    11: 'Ridge',
+    11: 'Ridged',
 }
 
-
 PENALTY_TYPES = {
     0: 'Drive through',
     1: 'Stop Go',
     2: 'Grid penalty',
     3: 'Penalty reminder',
     4: 'Time penalty',
     5: 'Warning',
@@ -368,15 +372,14 @@
     13: 'This and next lap invalidated without reason',
     14: 'This and previous lap invalidated',
     15: 'This and previous lap invalidated without reason',
     16: 'Retired',
     17: 'Black flag timer',
 }
 
-
 INFRINGEMENT_TYPES = {
     0: 'Blocking by slow driving',
     1: 'Blocking by wrong way driving',
     2: 'Reversing off the start line',
     3: 'Big Collision',
     4: 'Small Collision',
     5: 'Collision failed to hand back position single',
@@ -433,28 +436,28 @@
 
 ACTUAL_TYRE_COMPOUND = {
     16: 'C5',  # super soft
     17: 'C4',
     18: 'C3',
     19: 'C2',
     20: 'C1',  # hard
-    7: 'intermediates',
-    8: 'wet',
+    7: 'Intermediates',
+    8: 'Wet',
     # F1 Classic
-    9: 'dry',
-    10: 'wet',
+    9: 'Dry',
+    10: 'Wet',
     # F2
-    11: 'super soft',
-    12: 'soft',
-    13: 'medium',
-    14: 'hard',
-    15: 'wet',
+    11: 'Super soft',
+    12: 'Soft',
+    13: 'Medium',
+    14: 'Hard',
+    15: 'Wet',
 }
 
-# 3 compounds are chosen each weekend so they might not be a one to one match.
+# 3 compounds are chosen each weekend, so they might not be a one to one match.
 VISUAL_TYRE_COMPOUND = {
     16: 'soft',
     17: 'medium',
     18: 'hard',
     7: 'intermediates',
     8: 'wet',
     # F1 Classic
@@ -464,43 +467,210 @@
     15: 'wet',
     19: 'super soft',
     20: 'soft',
     21: 'medium',
     22: 'hard',
 }
 
-
 WEATHER = {
-    0: 'clear',
-    1: 'light_cloud',
-    2: 'overcast',
-    3: 'light_rain',
-    4: 'heavy_rain',
-    5: 'storm',
+    0: 'Clear',
+    1: 'Light cloud',
+    2: 'Overcast',
+    3: 'Light rain',
+    4: 'Heavy rain',
+    5: 'Storm',
+}
+
+TRACK_TEMPERATURE_CHANGE = {
+    0: "Up",
+    1: "Down",
+    2: "No change",
+}
+
+AIR_TEMPERATURE_CHANGE = {
+    0: "Up",
+    1: "Down",
+    2: "No change",
 }
 
-
 DRIVER_STATUS = {
-    0: 'in_garage',
-    1: 'flying_lap',
-    2: 'in_lap',
-    3: 'out_lap',
-    4: 'on_track',
+    0: 'In garage',
+    1: 'Flying lap',
+    2: 'In lap',
+    3: 'Out lap',
+    4: 'On track',
 }
 
-
 SESSION_TYPE = {
-    0: 'unknown',
-    1: 'practice_1',
-    2: 'practice_2',
-    3: 'practice_3',
-    4: 'short_practice',
-    5: 'qualifying_1',
-    6: 'qualifying_2',
-    7: 'qualifying_3',
-    8: 'short_qualifying',
-    9: 'osq',
-    10: 'race',
-    11: 'race_2',
-    12: 'race_3',
-    13: 'time_trial',
+    0: 'Unknown',
+    1: 'Practice 1',
+    2: 'Practice 2',
+    3: 'Practice 3',
+    4: 'Short Practice',
+    5: 'Qualifying 1',
+    6: 'Qualifying 2',
+    7: 'Qualifying 3',
+    8: 'Short Qualifying',
+    9: 'One Shot Qualifying',
+    10: 'Race',
+    11: 'Race 2',
+    12: 'Race 3',
+    13: 'Time Trial',
+}
+
+FORMULA = {
+    0: "F1 Modern",
+    1: "F1 Classic",
+    2: "F2",
+    3: "F1 Generic",
+    4: "Beta",
+    5: "Supercars",
+    6: "Esports",
+    7: "F2 2021",
+}
+
+SAFETY_CAR_STATUS = {0: "No safety car", 1: "Full", 2: "Virtual", 3: "Formation lap"}
+
+FORECAST_ACCURACY = {0: "Perfect", 1: "Approximate"}
+
+ERS_DEPLOYMENT_MODE = {
+    0: "None",
+    1: "Medium",
+    2: "Hot lap",
+    3: "Overtake",
+}
+
+RESULT_STATUS = {
+    0: "Invalid",
+    1: "Inactive",
+    2: "Active",
+    3: "Finished",
+    4: "Did not finish",
+    5: "Disqualified",
+    6: "Not classified",
+    7: "Retired",
+}
+
+ERS_FAULT = {
+    0: "Ok",
+    1: "Fault",
+}
+
+DRS_FAULT = {
+    0: "Ok",
+    1: "Fault",
+}
+
+ENGINE_BLOWN = {
+    0: "Ok",
+    1: "Fault",
+}
+
+ENGINE_SEIZED = {
+    0: "Ok",
+    1: "Fault",
+}
+
+LAP_VALID_BIT_FLAGS = {
+    "0x01": "lap valid",
+    "0x02": "Sector 1 valid",
+    "0x04": "Sector 2 valid",
+    "0x08": "Sector 3 valid",
+}
+
+VEHICLE_FIA_FLAGS = {
+    -1: "Invalid/unknown",
+    0: "None",
+    1: "Green",
+    2: "Blue",
+    3: "Yellow",
+    4: "Red",
+}
+
+DRS_ALLOWED = {
+    0: "Not allowed",
+    1: "Allowed",
+}
+
+SECTOR = {
+    0: "Sector 1",
+    1: "Sector 2",
+    2: "Sector 3",
+}
+
+CURRENT_LAP_INVALID = {
+    0: "Valid",
+    1: "Invalid",
+}
+
+PIT_STATUS = {
+    0: "None",
+    1: "Pitting",
+    2: "In pit area",
+}
+
+SESSION_LENGTH = {
+    0: "None",
+    2: "Very short",
+    3: "Short",
+    4: "Medium",
+    5: "Medium long",
+    6: "Long",
+    7: "Full",
+}
+
+SLI_PRO_SUPPORT = {
+    0: "Inactive",
+    1: "Active",
+}
+
+STEERING_ASSIST = {
+    0: "Off",
+    1: "On",
+}
+
+BRAKING_ASSIST = {
+    0: "Off",
+    1: "On",
+}
+
+GEARBOX_ASSIST = {
+    0: "Off",
+    1: "On",
+}
+
+PIT_ASSIST = {
+    0: "Off",
+    1: "On",
+}
+
+PIT_RELEASE_ASSIST = {
+    0: "Off",
+    1: "On",
+}
+
+ERS_ASSIST = {
+    0: "Off",
+    1: "On",
+}
+
+DRS_ASSIST = {
+    0: "Off",
+    1: "On",
+}
+
+DYNAMIC_RACING_LINE = {
+    0: "Off",
+    1: "Corners only",
+    2: "Full",
+}
+
+DYNAMIC_RACING_LINE_TYPE = {
+    0: "2D",
+    1: "3D",
+}
+
+# telemetry
+DRS = {
+    0: "Off",
+    1: "On",
 }
```

### Comparing `f1_22_telemetry-0.1.1/f1_22_telemetry/listener.py` & `f1_22_telemetry-0.1.2/f1_22_telemetry/listener.py`

 * *Files identical despite different names*

### Comparing `f1_22_telemetry-0.1.1/f1_22_telemetry/main.py` & `f1_22_telemetry-0.1.2/f1_22_telemetry/main.py`

 * *Files identical despite different names*

### Comparing `f1_22_telemetry-0.1.1/f1_22_telemetry/packets.py` & `f1_22_telemetry-0.1.2/f1_22_telemetry/packets.py`

 * *Files identical despite different names*

### Comparing `f1_22_telemetry-0.1.1/.gitignore` & `f1_22_telemetry-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `f1_22_telemetry-0.1.1/LICENSE` & `f1_22_telemetry-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `f1_22_telemetry-0.1.1/pyproject.toml` & `f1_22_telemetry-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "f1-22-telemetry"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Chris Hannam", email="ch@chrishannam.co.uk" },
 ]
 description = "Decode F1 22 telemetry data."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
@@ -36,8 +36,8 @@
     | _build
     | buck-out
     | build
     | dist
   )/
 )
 '''
-skip-string-normalization = true
+skip-string-normalization = true
```

### Comparing `f1_22_telemetry-0.1.1/PKG-INFO` & `f1_22_telemetry-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f1-22-telemetry
-Version: 0.1.1
+Version: 0.1.2
 Summary: Decode F1 22 telemetry data.
 Project-URL: Homepage, https://github.com/chrishannam/f1-22-telemetry
 Project-URL: Bug Tracker, https://github.com/chrishannam/f1-22-telemetry/issues
 Author-email: Chris Hannam <ch@chrishannam.co.uk>
 License: MIT License
         
         Copyright (c) 2022 Chris Hannam
@@ -32,21 +32,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # F1 22 Telemetry
 
 # Main Source for this Project
-To speed up the building of this project, the packet format was taken from
-[this](https://forums.codemasters.com/topic/80231-f1-2021-udp-specification/?do=findComment&comment=624274)
-post on the Codemasters forums. Which oddly works for F1 22, which is nice.
-
-Thanks to the hard work of the poster I was able to skip the tedious packet decoding.
-
-The updated F1 22 UDP specification is available [here](https://answers.ea.com/t5/General-Discussion/F1-22-UDP-Specification/td-p/11551274?attachment-id=607611)
+The F1 22 UDP specification is available [here](https://answers.ea.com/t5/General-Discussion/F1-22-UDP-Specification/td-p/11551274?attachment-id=607611)
 
 # Installing
 
 ```commandline
 pip install f1-22-telemetry
 ```
 
@@ -62,11 +56,11 @@
 
 listener = TelemetryListener(port=20777, host='localhost')
 packet = listener.get()
 ```
 
 # Releasing
 ```commandline
-pip install --upgrade build twine
+pip install --upgrade build twine pip
 python -m build
-python3 -m twine upload f1-22-telemetry
+python -m twine upload dist/f1-22-telemetry
 ```
```

