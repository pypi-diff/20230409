# Comparing `tmp/AutoThaliX-0.0.2.tar.gz` & `tmp/AutoThaliX-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoThaliX-0.0.2.tar", last modified: Sat Apr  8 21:18:52 2023, max compression
+gzip compressed data, was "AutoThaliX-0.1.0.tar", last modified: Sun Apr  9 08:12:44 2023, max compression
```

## Comparing `AutoThaliX-0.0.2.tar` & `AutoThaliX-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:18:52.413480 AutoThaliX-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:18:52.409480 AutoThaliX-0.0.2/AutoThaliX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-08 21:18:52.000000 AutoThaliX-0.0.2/AutoThaliX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-08 21:18:52.000000 AutoThaliX-0.0.2/AutoThaliX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 21:18:52.000000 AutoThaliX-0.0.2/AutoThaliX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-08 21:18:52.000000 AutoThaliX-0.0.2/AutoThaliX.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-08 21:18:52.000000 AutoThaliX-0.0.2/AutoThaliX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-08 21:18:52.413480 AutoThaliX-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:18:52.409480 AutoThaliX-0.0.2/autothalix/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/autothalix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/autothalix/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    13553 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/autothalix/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/autothalix/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 21:18:52.413480 AutoThaliX-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-08 21:18:04.000000 AutoThaliX-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:18:52.413480 AutoThaliX-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/tests/test_cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/tests/test_imp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/tests/test_lsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-08 21:17:46.000000 AutoThaliX-0.0.2/tests/test_ocp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:12:44.509395 AutoThaliX-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:12:44.501395 AutoThaliX-0.1.0/AutoThaliX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-09 08:12:44.000000 AutoThaliX-0.1.0/AutoThaliX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-09 08:12:44.000000 AutoThaliX-0.1.0/AutoThaliX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 08:12:44.000000 AutoThaliX-0.1.0/AutoThaliX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-09 08:12:44.000000 AutoThaliX-0.1.0/AutoThaliX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-09 08:12:44.000000 AutoThaliX-0.1.0/AutoThaliX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-09 08:12:44.509395 AutoThaliX-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:12:44.505395 AutoThaliX-0.1.0/autothalix/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/autothalix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/autothalix/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/autothalix/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/autothalix/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 08:12:44.509395 AutoThaliX-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 08:12:44.509395 AutoThaliX-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/tests/test_cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/tests/test_imp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/tests/test_lsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-09 08:11:27.000000 AutoThaliX-0.1.0/tests/test_ocp.py
```

### Comparing `AutoThaliX-0.0.2/AutoThaliX.egg-info/PKG-INFO` & `AutoThaliX-0.1.0/AutoThaliX.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: AutoThaliX
-Version: 0.0.2
+Version: 0.1.0
 Summary: A set of tools to work with tales potentiostats. Uses tales_remote
 Home-page: https://github.com/Arkady-A/autothalix
 Author: ArkadyA
 Author-email: arkadymirz@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![AutoThalix](logo.png)
 
 Repository that contains a toolkit to coduct complex operations on potentiostat.
```

### Comparing `AutoThaliX-0.0.2/LICENSE` & `AutoThaliX-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoThaliX-0.0.2/PKG-INFO` & `AutoThaliX-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: AutoThaliX
-Version: 0.0.2
+Version: 0.1.0
 Summary: A set of tools to work with tales potentiostats. Uses tales_remote
 Home-page: https://github.com/Arkady-A/autothalix
 Author: ArkadyA
 Author-email: arkadymirz@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![AutoThalix](logo.png)
 
 Repository that contains a toolkit to coduct complex operations on potentiostat.
```

### Comparing `AutoThaliX-0.0.2/README.md` & `AutoThaliX-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `AutoThaliX-0.0.2/autothalix/measurements.py` & `AutoThaliX-0.1.0/autothalix/measurements.py`

 * *Files 4% similar despite different names*

```diff
@@ -216,48 +216,14 @@
         self.wr_connection.setIEThirdEdgePotentialRelation(self.third_edge_potential_relation)
 
     def _start_measurements(self):
         self.wr_connection.checkIESetup()
         self.wr_connection.measureIE()
 
 
-class ElectrochemicalImpedanceSpectroscopy(BaseMeasurement):
-    """WIP"""
-
-    _measurement_name = 'ie'
-
-    def __str__(self):
-        return self._measurement_name
-
-    # setUpperFrequencyLimit
-    # setLowerFrequencyLimit
-    # setStartFrequency
-    # setUpperStepsPerDecade
-    # setLowerStepsPerDecade
-    # setUpperNumberOfPeriods
-    # setLowerNumberOfPeriods
-    # setScanStrategy
-    # setScanDirection
-    # setEISNaming
-    # setEISOutputPath
-    # setEISCounter
-    def parameters(self):
-        return [
-            'counter',
-            'end_frequency',
-            'maximum_current',
-            'minimum_current',
-            'naming',
-            'ohmic_drop',
-            'output_path',
-            'start_frequency',
-            'sweep_mode',
-        ]
-
-
 class BaseManualMeasurements(BaseMeasurement, ABC):
     """
     Base class for manual measurements
     """
 
     def __init__(self, wr_connection: ThalesRemoteScriptWrapper, measurement_id: str, **kwargs):
         super().__init__(wr_connection, measurement_id, **kwargs)
```

### Comparing `AutoThaliX-0.0.2/autothalix/utils.py` & `AutoThaliX-0.1.0/autothalix/utils.py`

 * *Files identical despite different names*

### Comparing `AutoThaliX-0.0.2/setup.py` & `AutoThaliX-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 with open("requirements.txt", "r") as f:
     requirements = f.readlines()
 
 install_requires = [req.strip() for req in requirements]
 
 setuptools.setup(
     name="AutoThaliX",
-    version="0.0.2",
+    version="0.1.0",
     author="ArkadyA",
     author_email="arkadymirz@gmail.com",
     description="A set of tools to work with tales potentiostats. Uses tales_remote",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Arkady-A/autothalix",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.9",
     install_requires=install_requires,
 )
```

### Comparing `AutoThaliX-0.0.2/tests/test_cv.py` & `AutoThaliX-0.1.0/tests/test_cv.py`

 * *Files identical despite different names*

### Comparing `AutoThaliX-0.0.2/tests/test_imp.py` & `AutoThaliX-0.1.0/tests/test_imp.py`

 * *Files identical despite different names*

### Comparing `AutoThaliX-0.0.2/tests/test_lsv.py` & `AutoThaliX-0.1.0/tests/test_lsv.py`

 * *Files identical despite different names*

### Comparing `AutoThaliX-0.0.2/tests/test_ocp.py` & `AutoThaliX-0.1.0/tests/test_ocp.py`

 * *Files identical despite different names*

