# Comparing `tmp/apicast-0.8.5.tar.gz` & `tmp/apicast-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apicast-0.8.5.tar", last modified: Sun Apr  9 12:48:41 2023, max compression
+gzip compressed data, was "apicast-0.8.6.tar", last modified: Sun Apr  9 14:53:59 2023, max compression
```

## Comparing `apicast-0.8.5.tar` & `apicast-0.8.6.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-09 12:48:41.952903 apicast-0.8.5/
--rw-r--r--   0 amo        (501) staff       (20)    32386 2021-03-02 20:42:57.000000 apicast-0.8.5/LICENSE
--rw-r--r--   0 amo        (501) staff       (20)     6030 2023-04-09 12:48:41.952630 apicast-0.8.5/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     3572 2023-04-09 12:43:09.000000 apicast-0.8.5/README.rst
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-09 12:48:41.949982 apicast-0.8.5/apicast/
--rw-r--r--   0 amo        (501) staff       (20)      133 2023-04-09 12:48:31.000000 apicast-0.8.5/apicast/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     6711 2021-03-05 22:27:00.000000 apicast-0.8.5/apicast/api.py
--rw-r--r--   0 amo        (501) staff       (20)     4030 2021-03-05 21:56:14.000000 apicast-0.8.5/apicast/cli.py
--rw-r--r--   0 amo        (501) staff       (20)     4810 2023-04-09 12:43:09.000000 apicast-0.8.5/apicast/core.py
--rw-r--r--   0 amo        (501) staff       (20)     2665 2021-03-05 22:34:57.000000 apicast-0.8.5/apicast/format.py
--rw-r--r--   0 amo        (501) staff       (20)     1124 2021-03-05 21:56:14.000000 apicast-0.8.5/apicast/util.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-09 12:48:41.951802 apicast-0.8.5/apicast.egg-info/
--rw-r--r--   0 amo        (501) staff       (20)     6030 2023-04-09 12:48:41.000000 apicast-0.8.5/apicast.egg-info/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)      356 2023-04-09 12:48:41.000000 apicast-0.8.5/apicast.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2023-04-09 12:48:41.000000 apicast-0.8.5/apicast.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (501) staff       (20)       44 2023-04-09 12:48:41.000000 apicast-0.8.5/apicast.egg-info/entry_points.txt
--rw-r--r--   0 amo        (501) staff       (20)      251 2023-04-09 12:48:41.000000 apicast-0.8.5/apicast.egg-info/requires.txt
--rw-r--r--   0 amo        (501) staff       (20)        8 2023-04-09 12:48:41.000000 apicast-0.8.5/apicast.egg-info/top_level.txt
--rw-r--r--   0 amo        (501) staff       (20)       38 2023-04-09 12:48:41.952986 apicast-0.8.5/setup.cfg
--rw-r--r--   0 amo        (501) staff       (20)     3377 2023-04-09 12:48:31.000000 apicast-0.8.5/setup.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-09 12:48:41.952299 apicast-0.8.5/test/
--rw-r--r--   0 amo        (501) staff       (20)     1081 2021-03-05 00:45:04.000000 apicast-0.8.5/test/test_data.py
--rw-r--r--   0 amo        (501) staff       (20)     1344 2021-03-05 00:44:44.000000 apicast-0.8.5/test/test_locations.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-09 14:53:59.598785 apicast-0.8.6/
+-rw-r--r--   0 amo        (501) staff       (20)    32386 2021-03-02 20:42:57.000000 apicast-0.8.6/LICENSE
+-rw-r--r--   0 amo        (501) staff       (20)     6303 2023-04-09 14:53:59.598493 apicast-0.8.6/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     3845 2023-04-09 14:48:19.000000 apicast-0.8.6/README.rst
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-09 14:53:59.593140 apicast-0.8.6/apicast/
+-rw-r--r--   0 amo        (501) staff       (20)      133 2023-04-09 14:53:48.000000 apicast-0.8.6/apicast/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     6711 2021-03-05 22:27:00.000000 apicast-0.8.6/apicast/api.py
+-rw-r--r--   0 amo        (501) staff       (20)     4030 2021-03-05 21:56:14.000000 apicast-0.8.6/apicast/cli.py
+-rw-r--r--   0 amo        (501) staff       (20)     4810 2023-04-09 12:43:09.000000 apicast-0.8.6/apicast/core.py
+-rw-r--r--   0 amo        (501) staff       (20)     3032 2023-04-09 14:17:06.000000 apicast-0.8.6/apicast/format.py
+-rw-r--r--   0 amo        (501) staff       (20)     1124 2021-03-05 21:56:14.000000 apicast-0.8.6/apicast/util.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-09 14:53:59.595748 apicast-0.8.6/apicast.egg-info/
+-rw-r--r--   0 amo        (501) staff       (20)     6303 2023-04-09 14:53:59.000000 apicast-0.8.6/apicast.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)      390 2023-04-09 14:53:59.000000 apicast-0.8.6/apicast.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2023-04-09 14:53:59.000000 apicast-0.8.6/apicast.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (501) staff       (20)       44 2023-04-09 14:53:59.000000 apicast-0.8.6/apicast.egg-info/entry_points.txt
+-rw-r--r--   0 amo        (501) staff       (20)      252 2023-04-09 14:53:59.000000 apicast-0.8.6/apicast.egg-info/requires.txt
+-rw-r--r--   0 amo        (501) staff       (20)        8 2023-04-09 14:53:59.000000 apicast-0.8.6/apicast.egg-info/top_level.txt
+-rw-r--r--   0 amo        (501) staff       (20)       38 2023-04-09 14:53:59.598879 apicast-0.8.6/setup.cfg
+-rw-r--r--   0 amo        (501) staff       (20)     3378 2023-04-09 14:53:48.000000 apicast-0.8.6/setup.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-09 14:53:59.597866 apicast-0.8.6/test/
+-rw-r--r--   0 amo        (501) staff       (20)      938 2023-04-09 14:17:06.000000 apicast-0.8.6/test/test_api.py
+-rw-r--r--   0 amo        (501) staff       (20)     1852 2023-04-09 14:17:06.000000 apicast-0.8.6/test/test_cli.py
+-rw-r--r--   0 amo        (501) staff       (20)     1833 2023-04-09 14:17:06.000000 apicast-0.8.6/test/test_data.py
+-rw-r--r--   0 amo        (501) staff       (20)     1863 2023-04-09 14:17:06.000000 apicast-0.8.6/test/test_locations.py
```

### Comparing `apicast-0.8.5/LICENSE` & `apicast-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `apicast-0.8.5/PKG-INFO` & `apicast-0.8.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apicast
-Version: 0.8.5
+Version: 0.8.6
 Summary: Python client and HTTP service to access bee flight forecast information published by Deutscher Wetterdienst (DWD), the federal meteorological service in Germany.
 Home-page: https://github.com/hiveeyes/apicast
 Author: Andreas Motl
 Author-email: andreas@hiveeyes.org
 License: AGPL 3, EUPL 1.2
 Keywords: honey bee apis mellifera flight forecast information dwd cdc deutscher wetterdienst climate data center weather opendata data acquisition transformation export geospatial temporal timeseries sensor network observation http rest api json markdown
 Classifier: Programming Language :: Python
@@ -44,14 +44,18 @@
 Classifier: Operating System :: MacOS
 Provides-Extra: service
 License-File: LICENSE
 
 .. image:: https://github.com/hiveeyes/apicast/workflows/Tests/badge.svg
     :target: https://github.com/hiveeyes/apicast/actions?workflow=Tests
 
+.. image:: https://codecov.io/gh/hiveeyes/apicast/branch/main/graph/badge.svg
+    :target: https://codecov.io/gh/hiveeyes/apicast
+    :alt: Test suite code coverage
+
 .. image:: https://img.shields.io/pypi/pyversions/apicast.svg
     :target: https://python.org
 
 .. image:: https://img.shields.io/pypi/v/apicast.svg
     :target: https://pypi.org/project/apicast/
 
 .. image:: https://img.shields.io/pypi/status/apicast.svg
@@ -72,16 +76,16 @@
 
 *****
 About
 *****
 
 Apicast acquires bee flight forecast information published by Deutscher Wetterdienst (DWD).
 
-- **Live API**: http://apicast.hiveeyes.org/
-- **Development**: https://community.hiveeyes.org/t/dwd-prognose-bienenflug/787
+- **Development**: `Hiveeyes » DWD-Prognose Bienenflug`_
+- **Live API**: https://apicast.hiveeyes.org/ (also on HTTP)
 
 
 *****
 Setup
 *****
 
 CLI version::
@@ -190,23 +194,26 @@
 - **Source**:
 
   - https://www.dwd.de/DE/leistungen/biene_flug/bienenflug.html
   - https://www.dwd.de/DE/fachnutzer/freizeitgaertner/1_gartenwetter/_node.html
 
 - **Documentation**:
 
-  - https://www.dwd.de/DE/fachnutzer/freizeitgaertner/dokumentation/gw_bienenflug
-  - https://www.dwd.de/DE/fachnutzer/freizeitgaertner/dokumentation/gw_bienenflug.pdf?__blob=publicationFile
+  - https://www.dwd.de/DE/fachnutzer/landwirtschaft/dokumentationen/allgemein/bienenflug_doku.html
+  - https://www.dwd.de/DE/fachnutzer/landwirtschaft/dokumentationen/isabel/meinagrar_bienenflug.html
 
 - **Data copyright**: © Deutscher Wetterdienst (DWD), Agricultural Meteorology Department
 
 
 Logo picture
 ============
 
 - **Description**:     	A bee swarm on an oak tree in Plymouth, UK
 - **Date**:    	        21 June 2009
 - **Source**: 	        Own work
 - **Author**: 	        Nilfanion
 - **Camera location**:	50° 24′ 38.3″ N, 4° 09′ 28.2″ W
 - **License**:          Creative Commons Attribution-Share Alike 3.0 Unported
 - **URL**:              https://commons.wikimedia.org/wiki/File:Bee_swarm_in_Plymouth.jpg
+
+
+.. _Hiveeyes » DWD-Prognose Bienenflug: https://community.hiveeyes.org/t/dwd-prognose-bienenflug/787
```

### Comparing `apicast-0.8.5/README.rst` & `apicast-0.8.6/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 .. image:: https://github.com/hiveeyes/apicast/workflows/Tests/badge.svg
     :target: https://github.com/hiveeyes/apicast/actions?workflow=Tests
 
+.. image:: https://codecov.io/gh/hiveeyes/apicast/branch/main/graph/badge.svg
+    :target: https://codecov.io/gh/hiveeyes/apicast
+    :alt: Test suite code coverage
+
 .. image:: https://img.shields.io/pypi/pyversions/apicast.svg
     :target: https://python.org
 
 .. image:: https://img.shields.io/pypi/v/apicast.svg
     :target: https://pypi.org/project/apicast/
 
 .. image:: https://img.shields.io/pypi/status/apicast.svg
@@ -25,16 +29,16 @@
 
 *****
 About
 *****
 
 Apicast acquires bee flight forecast information published by Deutscher Wetterdienst (DWD).
 
-- **Live API**: http://apicast.hiveeyes.org/
-- **Development**: https://community.hiveeyes.org/t/dwd-prognose-bienenflug/787
+- **Development**: `Hiveeyes » DWD-Prognose Bienenflug`_
+- **Live API**: https://apicast.hiveeyes.org/ (also on HTTP)
 
 
 *****
 Setup
 *****
 
 CLI version::
@@ -143,23 +147,26 @@
 - **Source**:
 
   - https://www.dwd.de/DE/leistungen/biene_flug/bienenflug.html
   - https://www.dwd.de/DE/fachnutzer/freizeitgaertner/1_gartenwetter/_node.html
 
 - **Documentation**:
 
-  - https://www.dwd.de/DE/fachnutzer/freizeitgaertner/dokumentation/gw_bienenflug
-  - https://www.dwd.de/DE/fachnutzer/freizeitgaertner/dokumentation/gw_bienenflug.pdf?__blob=publicationFile
+  - https://www.dwd.de/DE/fachnutzer/landwirtschaft/dokumentationen/allgemein/bienenflug_doku.html
+  - https://www.dwd.de/DE/fachnutzer/landwirtschaft/dokumentationen/isabel/meinagrar_bienenflug.html
 
 - **Data copyright**: © Deutscher Wetterdienst (DWD), Agricultural Meteorology Department
 
 
 Logo picture
 ============
 
 - **Description**:     	A bee swarm on an oak tree in Plymouth, UK
 - **Date**:    	        21 June 2009
 - **Source**: 	        Own work
 - **Author**: 	        Nilfanion
 - **Camera location**:	50° 24′ 38.3″ N, 4° 09′ 28.2″ W
 - **License**:          Creative Commons Attribution-Share Alike 3.0 Unported
 - **URL**:              https://commons.wikimedia.org/wiki/File:Bee_swarm_in_Plymouth.jpg
+
+
+.. _Hiveeyes » DWD-Prognose Bienenflug: https://community.hiveeyes.org/t/dwd-prognose-bienenflug/787
```

### Comparing `apicast-0.8.5/apicast/api.py` & `apicast-0.8.6/apicast/api.py`

 * *Files identical despite different names*

### Comparing `apicast-0.8.5/apicast/cli.py` & `apicast-0.8.6/apicast/cli.py`

 * *Files identical despite different names*

### Comparing `apicast-0.8.5/apicast/core.py` & `apicast-0.8.6/apicast/core.py`

 * *Files identical despite different names*

### Comparing `apicast-0.8.5/apicast/format.py` & `apicast-0.8.6/apicast/format.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,27 +10,34 @@
 
 
 class Formatter:
     """
     Die Bedingungen für den Bienenflug werden in 5 Intensitätsstufen angegeben
     (kein - gering - mittel - stark - intensiv).
 
-    -- https://www.dwd.de/DE/fachnutzer/freizeitgaertner/dokumentation/gw_bienenflug
+    Die Flugaktivität reicht von geringer, über mittlerer und hoher bis sehr hoher Flugaktivität.
+
+    - https://www.dwd.de/DE/fachnutzer/landwirtschaft/dokumentationen/allgemein/bienenflug_doku.html
+    - https://www.dwd.de/DE/fachnutzer/landwirtschaft/dokumentationen/isabel/meinagrar_bienenflug.html?nn=629500
     """
 
     LABEL_MAP = {
         "Datum": "date",
         "morgens": "morning",
         "mittags": "noon",
         "abends": "evening",
         "kein": "no",
         "gering": "low",
         "mittel": "medium",
         "stark": "strong",
         "intensiv": "intensive",
+        # Added 2023
+        # https://github.com/hiveeyes/apicast/issues/4
+        "hoch": "strong",
+        "sehr hoch": "intensive",
     }
 
     STRENGTH_MACHINE_MAP = {
         "no": 0,
         "low": 1,
         "medium": 2,
         "strong": 3,
```

### Comparing `apicast-0.8.5/apicast/util.py` & `apicast-0.8.6/apicast/util.py`

 * *Files identical despite different names*

### Comparing `apicast-0.8.5/apicast.egg-info/PKG-INFO` & `apicast-0.8.6/apicast.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apicast
-Version: 0.8.5
+Version: 0.8.6
 Summary: Python client and HTTP service to access bee flight forecast information published by Deutscher Wetterdienst (DWD), the federal meteorological service in Germany.
 Home-page: https://github.com/hiveeyes/apicast
 Author: Andreas Motl
 Author-email: andreas@hiveeyes.org
 License: AGPL 3, EUPL 1.2
 Keywords: honey bee apis mellifera flight forecast information dwd cdc deutscher wetterdienst climate data center weather opendata data acquisition transformation export geospatial temporal timeseries sensor network observation http rest api json markdown
 Classifier: Programming Language :: Python
@@ -44,14 +44,18 @@
 Classifier: Operating System :: MacOS
 Provides-Extra: service
 License-File: LICENSE
 
 .. image:: https://github.com/hiveeyes/apicast/workflows/Tests/badge.svg
     :target: https://github.com/hiveeyes/apicast/actions?workflow=Tests
 
+.. image:: https://codecov.io/gh/hiveeyes/apicast/branch/main/graph/badge.svg
+    :target: https://codecov.io/gh/hiveeyes/apicast
+    :alt: Test suite code coverage
+
 .. image:: https://img.shields.io/pypi/pyversions/apicast.svg
     :target: https://python.org
 
 .. image:: https://img.shields.io/pypi/v/apicast.svg
     :target: https://pypi.org/project/apicast/
 
 .. image:: https://img.shields.io/pypi/status/apicast.svg
@@ -72,16 +76,16 @@
 
 *****
 About
 *****
 
 Apicast acquires bee flight forecast information published by Deutscher Wetterdienst (DWD).
 
-- **Live API**: http://apicast.hiveeyes.org/
-- **Development**: https://community.hiveeyes.org/t/dwd-prognose-bienenflug/787
+- **Development**: `Hiveeyes » DWD-Prognose Bienenflug`_
+- **Live API**: https://apicast.hiveeyes.org/ (also on HTTP)
 
 
 *****
 Setup
 *****
 
 CLI version::
@@ -190,23 +194,26 @@
 - **Source**:
 
   - https://www.dwd.de/DE/leistungen/biene_flug/bienenflug.html
   - https://www.dwd.de/DE/fachnutzer/freizeitgaertner/1_gartenwetter/_node.html
 
 - **Documentation**:
 
-  - https://www.dwd.de/DE/fachnutzer/freizeitgaertner/dokumentation/gw_bienenflug
-  - https://www.dwd.de/DE/fachnutzer/freizeitgaertner/dokumentation/gw_bienenflug.pdf?__blob=publicationFile
+  - https://www.dwd.de/DE/fachnutzer/landwirtschaft/dokumentationen/allgemein/bienenflug_doku.html
+  - https://www.dwd.de/DE/fachnutzer/landwirtschaft/dokumentationen/isabel/meinagrar_bienenflug.html
 
 - **Data copyright**: © Deutscher Wetterdienst (DWD), Agricultural Meteorology Department
 
 
 Logo picture
 ============
 
 - **Description**:     	A bee swarm on an oak tree in Plymouth, UK
 - **Date**:    	        21 June 2009
 - **Source**: 	        Own work
 - **Author**: 	        Nilfanion
 - **Camera location**:	50° 24′ 38.3″ N, 4° 09′ 28.2″ W
 - **License**:          Creative Commons Attribution-Share Alike 3.0 Unported
 - **URL**:              https://commons.wikimedia.org/wiki/File:Bee_swarm_in_Plymouth.jpg
+
+
+.. _Hiveeyes » DWD-Prognose Bienenflug: https://community.hiveeyes.org/t/dwd-prognose-bienenflug/787
```

### Comparing `apicast-0.8.5/setup.py` & `apicast-0.8.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 README = open(os.path.join(here, "README.rst"), encoding="UTF-8").read()
 
 setup(
     name="apicast",
-    version="0.8.5",
+    version="0.8.6",
     description="Python client and HTTP service to access bee flight forecast "
                 "information published by Deutscher Wetterdienst (DWD), the "
                 "federal meteorological service in Germany.",
     long_description=README,
     license="AGPL 3, EUPL 1.2",
     classifiers=[
         "Programming Language :: Python",
@@ -61,26 +61,26 @@
     "sensor network observation "
     "http rest api "
     "json markdown",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "beautifulsoup4>=4,<5",
-        "dateparser>=0.7.4,<1",
+        "dateparser>=0.7.4,<2",
         "docopt>=0.6,<1",
         "html-table-extractor>=1,<2",
-        "jsonpickle>=2,<3",
+        "jsonpickle>=2,<4",
         "munch>=2.5,<3",
-        "python-slugify>=4,<5",
+        "python-slugify>=4,<9",
         "requests>=2,<3",
-        "tabulate>=0.8,<0.9",
+        "tabulate>=0.8,<0.10",
         "ttl-cache>=1.6,<2",
         "tzlocal>=2,<3",
     ],
     extras_require={
         "service": [
-            "fastapi>=0.55.1,<0.64",
-            "uvicorn<=0.13.3",
+            "fastapi>=0.55.1,<0.96",
+            "uvicorn<=0.21.1",
         ],
     },
     entry_points={"console_scripts": ["apicast = apicast.cli:run"]},
 )
```

### Comparing `apicast-0.8.5/test/test_data.py` & `apicast-0.8.6/test/test_data.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import dataclasses
 
 import pytest
 from datadiff.tools import assert_equal
 
-from apicast.core import DwdBeeflightForecast
+from apicast.core import DwdBeeflightForecast, Station, State
 
 dbf = DwdBeeflightForecast()
 
 
 @pytest.mark.data
-def test_get_data():
+def test_get_data_success():
 
     stations = dbf.get_stations()
     bavaria_hof = [
         station for station in stations if station.identifier == "bifl_0042"
     ][0]
 
     data_hof = dbf.get_data(station=bavaria_hof)
@@ -38,7 +38,34 @@
                 "slug": "bayern/hof",
             },
             "station_name": "Hof",
             "data": None,
             "footnote": None,
         },
     )
+
+
+@pytest.mark.data
+def test_get_data_invalid_station():
+    station = Station(
+        state=State(label='Nordrhein-Westfalen', identifier='bifl_bl999'),
+        label='Bielefeld',
+        identifier='bifl_bl999',
+        slug='nordrhein-westfalen/bielefeld',
+    )
+    with pytest.raises(ValueError) as ex:
+        dbf.get_data(station=station)
+    assert ex.match("No forecast available for this station")
+
+
+@pytest.mark.data
+def test_get_data_copy():
+
+    stations = dbf.get_stations()
+    bavaria_hof = [
+        station for station in stations if station.identifier == "bifl_0042"
+    ][0]
+
+    data_hof = dbf.get_data(station=bavaria_hof)
+    data_hof_copy = data_hof.copy()
+
+    assert id(data_hof) != id(data_hof_copy)
```

### Comparing `apicast-0.8.5/test/test_locations.py` & `apicast-0.8.6/test/test_locations.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import dataclasses
 
+import pytest
 from datadiff.tools import assert_equal
 
-from apicast.core import DwdBeeflightForecast
+from apicast.core import DwdBeeflightForecast, Station, State
 
 dbf = DwdBeeflightForecast()
 
 
 def test_get_states():
 
     states = dbf.get_states()
@@ -52,7 +53,25 @@
             "slug": "berlin/berlin-tempelhof",
             "state": {
                 "label": "Berlin",
                 "identifier": "bifl_bl03",
             },
         },
     )
+
+
+def test_get_station_by_slug_success():
+    station = dbf.get_station_by_slug("brandenburg/potsdam")
+
+    reference = Station(
+        state=State(label='Brandenburg', identifier='bifl_bl04'),
+        label='Potsdam',
+        identifier='bifl_0021',
+        slug='brandenburg/potsdam',
+    )
+    assert station == reference
+
+
+def test_get_station_by_slug_failure():
+    with pytest.raises(KeyError) as ex:
+        dbf.get_station_by_slug("foobar")
+    assert ex.match("No such station")
```

