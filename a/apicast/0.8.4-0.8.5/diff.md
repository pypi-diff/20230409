# Comparing `tmp/apicast-0.8.4.tar.gz` & `tmp/apicast-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apicast-0.8.4.tar", last modified: Sun Apr  9 12:44:37 2023, max compression
+gzip compressed data, was "apicast-0.8.5.tar", last modified: Sun Apr  9 12:48:41 2023, max compression
```

## Comparing `apicast-0.8.4.tar` & `apicast-0.8.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-09 12:44:37.916535 apicast-0.8.4/
--rw-r--r--   0 amo        (501) staff       (20)     7359 2023-04-09 12:44:37.916258 apicast-0.8.4/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     3572 2023-04-09 12:43:09.000000 apicast-0.8.4/README.rst
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-09 12:44:37.913661 apicast-0.8.4/apicast/
--rw-r--r--   0 amo        (501) staff       (20)      133 2023-04-09 12:44:34.000000 apicast-0.8.4/apicast/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     6711 2021-03-05 22:27:00.000000 apicast-0.8.4/apicast/api.py
--rw-r--r--   0 amo        (501) staff       (20)     4030 2021-03-05 21:56:14.000000 apicast-0.8.4/apicast/cli.py
--rw-r--r--   0 amo        (501) staff       (20)     4810 2023-04-09 12:43:09.000000 apicast-0.8.4/apicast/core.py
--rw-r--r--   0 amo        (501) staff       (20)     2665 2021-03-05 22:34:57.000000 apicast-0.8.4/apicast/format.py
--rw-r--r--   0 amo        (501) staff       (20)     1124 2021-03-05 21:56:14.000000 apicast-0.8.4/apicast/util.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-09 12:44:37.915372 apicast-0.8.4/apicast.egg-info/
--rw-r--r--   0 amo        (501) staff       (20)     7359 2023-04-09 12:44:37.000000 apicast-0.8.4/apicast.egg-info/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)      348 2023-04-09 12:44:37.000000 apicast-0.8.4/apicast.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2023-04-09 12:44:37.000000 apicast-0.8.4/apicast.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (501) staff       (20)       45 2023-04-09 12:44:37.000000 apicast-0.8.4/apicast.egg-info/entry_points.txt
--rw-r--r--   0 amo        (501) staff       (20)      250 2023-04-09 12:44:37.000000 apicast-0.8.4/apicast.egg-info/requires.txt
--rw-r--r--   0 amo        (501) staff       (20)        8 2023-04-09 12:44:37.000000 apicast-0.8.4/apicast.egg-info/top_level.txt
--rw-r--r--   0 amo        (501) staff       (20)       38 2023-04-09 12:44:37.916638 apicast-0.8.4/setup.cfg
--rw-r--r--   0 amo        (501) staff       (20)     3376 2023-04-09 12:44:34.000000 apicast-0.8.4/setup.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-09 12:44:37.915844 apicast-0.8.4/test/
--rw-r--r--   0 amo        (501) staff       (20)     1081 2021-03-05 00:45:04.000000 apicast-0.8.4/test/test_data.py
--rw-r--r--   0 amo        (501) staff       (20)     1344 2021-03-05 00:44:44.000000 apicast-0.8.4/test/test_locations.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-09 12:48:41.952903 apicast-0.8.5/
+-rw-r--r--   0 amo        (501) staff       (20)    32386 2021-03-02 20:42:57.000000 apicast-0.8.5/LICENSE
+-rw-r--r--   0 amo        (501) staff       (20)     6030 2023-04-09 12:48:41.952630 apicast-0.8.5/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     3572 2023-04-09 12:43:09.000000 apicast-0.8.5/README.rst
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-09 12:48:41.949982 apicast-0.8.5/apicast/
+-rw-r--r--   0 amo        (501) staff       (20)      133 2023-04-09 12:48:31.000000 apicast-0.8.5/apicast/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     6711 2021-03-05 22:27:00.000000 apicast-0.8.5/apicast/api.py
+-rw-r--r--   0 amo        (501) staff       (20)     4030 2021-03-05 21:56:14.000000 apicast-0.8.5/apicast/cli.py
+-rw-r--r--   0 amo        (501) staff       (20)     4810 2023-04-09 12:43:09.000000 apicast-0.8.5/apicast/core.py
+-rw-r--r--   0 amo        (501) staff       (20)     2665 2021-03-05 22:34:57.000000 apicast-0.8.5/apicast/format.py
+-rw-r--r--   0 amo        (501) staff       (20)     1124 2021-03-05 21:56:14.000000 apicast-0.8.5/apicast/util.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-09 12:48:41.951802 apicast-0.8.5/apicast.egg-info/
+-rw-r--r--   0 amo        (501) staff       (20)     6030 2023-04-09 12:48:41.000000 apicast-0.8.5/apicast.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)      356 2023-04-09 12:48:41.000000 apicast-0.8.5/apicast.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2023-04-09 12:48:41.000000 apicast-0.8.5/apicast.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (501) staff       (20)       44 2023-04-09 12:48:41.000000 apicast-0.8.5/apicast.egg-info/entry_points.txt
+-rw-r--r--   0 amo        (501) staff       (20)      251 2023-04-09 12:48:41.000000 apicast-0.8.5/apicast.egg-info/requires.txt
+-rw-r--r--   0 amo        (501) staff       (20)        8 2023-04-09 12:48:41.000000 apicast-0.8.5/apicast.egg-info/top_level.txt
+-rw-r--r--   0 amo        (501) staff       (20)       38 2023-04-09 12:48:41.952986 apicast-0.8.5/setup.cfg
+-rw-r--r--   0 amo        (501) staff       (20)     3377 2023-04-09 12:48:31.000000 apicast-0.8.5/setup.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-09 12:48:41.952299 apicast-0.8.5/test/
+-rw-r--r--   0 amo        (501) staff       (20)     1081 2021-03-05 00:45:04.000000 apicast-0.8.5/test/test_data.py
+-rw-r--r--   0 amo        (501) staff       (20)     1344 2021-03-05 00:44:44.000000 apicast-0.8.5/test/test_locations.py
```

### Comparing `apicast-0.8.4/PKG-INFO` & `apicast-0.8.5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,183 +1,16 @@
 Metadata-Version: 2.1
 Name: apicast
-Version: 0.8.4
+Version: 0.8.5
 Summary: Python client and HTTP service to access bee flight forecast information published by Deutscher Wetterdienst (DWD), the federal meteorological service in Germany.
 Home-page: https://github.com/hiveeyes/apicast
 Author: Andreas Motl
 Author-email: andreas@hiveeyes.org
 License: AGPL 3, EUPL 1.2
-Description: .. image:: https://github.com/hiveeyes/apicast/workflows/Tests/badge.svg
-            :target: https://github.com/hiveeyes/apicast/actions?workflow=Tests
-        
-        .. image:: https://img.shields.io/pypi/pyversions/apicast.svg
-            :target: https://python.org
-        
-        .. image:: https://img.shields.io/pypi/v/apicast.svg
-            :target: https://pypi.org/project/apicast/
-        
-        .. image:: https://img.shields.io/pypi/status/apicast.svg
-            :target: https://pypi.org/project/apicast/
-        
-        .. image:: https://img.shields.io/pypi/l/apicast.svg
-            :target: https://pypi.org/project/apicast/
-        
-        .. image:: https://static.pepy.tech/badge/apicast/month
-            :target: https://pepy.tech/project/apicast
-        
-        |
-        
-        #######
-        Apicast
-        #######
-        
-        
-        *****
-        About
-        *****
-        
-        Apicast acquires bee flight forecast information published by Deutscher Wetterdienst (DWD).
-        
-        - **Live API**: http://apicast.hiveeyes.org/
-        - **Development**: https://community.hiveeyes.org/t/dwd-prognose-bienenflug/787
-        
-        
-        *****
-        Setup
-        *****
-        
-        CLI version::
-        
-            pip install apicast
-        
-        HTTP API::
-        
-            pip install apicast[service]
-        
-        
-        ********
-        Synopsis
-        ********
-        
-        Display list of states and sites::
-        
-            apicast beeflight stations
-        
-        Display list of location slugs::
-        
-            apicast beeflight stations --slugs
-        
-        Acquire information for given location slug ``brandenburg/potsdam``::
-        
-            apicast beeflight forecast --station=brandenburg/potsdam
-        
-        Acquire information for given location slug ``brandenburg/potsdam``, output as table in Markdown format::
-        
-            apicast beeflight forecast --station=brandenburg/potsdam --format=table-markdown
-        
-        Output as table in JSON machine readable format::
-        
-            apicast beeflight forecast --station=brandenburg/potsdam --format=json-machine
-        
-        
-        
-        ********
-        HTTP API
-        ********
-        
-        Start HTTP API service::
-        
-            apicast service
-        
-        Start HTTP service with dynamic code reloading::
-        
-            apicast service --reload
-        
-        Then navigate to::
-        
-            open http://localhost:24640/
-        
-        
-        
-        *******
-        Example
-        *******
-        
-        ::
-        
-            apicast beeflight forecast --station=brandenburg/potsdam
-        
-        ::
-        
-            [
-                {
-                    "Datum": "Mo 01.06.",
-                    "morgens": "stark",
-                    "mittags": "intensiv",
-                    "abends": "stark"
-                },
-                {
-                    "Datum": "Di 02.06.",
-                    "morgens": "stark",
-                    "mittags": "intensiv",
-                    "abends": "intensiv"
-                },
-                {
-                    "Datum": "Mi 03.06.",
-                    "morgens": "intensiv",
-                    "mittags": "intensiv",
-                    "abends": "intensiv"
-                }
-            ]
-        
-        
-        *****
-        Tests
-        *****
-        
-        ::
-        
-            make test
-        
-        
-        ********************
-        Content attributions
-        ********************
-        
-        The copyright of data, particular images and pictograms are held by their respective owners, unless otherwise noted.
-        
-        Data
-        ====
-        
-        - **Source**:
-        
-          - https://www.dwd.de/DE/leistungen/biene_flug/bienenflug.html
-          - https://www.dwd.de/DE/fachnutzer/freizeitgaertner/1_gartenwetter/_node.html
-        
-        - **Documentation**:
-        
-          - https://www.dwd.de/DE/fachnutzer/freizeitgaertner/dokumentation/gw_bienenflug
-          - https://www.dwd.de/DE/fachnutzer/freizeitgaertner/dokumentation/gw_bienenflug.pdf?__blob=publicationFile
-        
-        - **Data copyright**: © Deutscher Wetterdienst (DWD), Agricultural Meteorology Department
-        
-        
-        Logo picture
-        ============
-        
-        - **Description**:     	A bee swarm on an oak tree in Plymouth, UK
-        - **Date**:    	        21 June 2009
-        - **Source**: 	        Own work
-        - **Author**: 	        Nilfanion
-        - **Camera location**:	50° 24′ 38.3″ N, 4° 09′ 28.2″ W
-        - **License**:          Creative Commons Attribution-Share Alike 3.0 Unported
-        - **URL**:              https://commons.wikimedia.org/wiki/File:Bee_swarm_in_Plymouth.jpg
-        
 Keywords: honey bee apis mellifera flight forecast information dwd cdc deutscher wetterdienst climate data center weather opendata data acquisition transformation export geospatial temporal timeseries sensor network observation http rest api json markdown
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -206,7 +39,174 @@
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Provides-Extra: service
+License-File: LICENSE
+
+.. image:: https://github.com/hiveeyes/apicast/workflows/Tests/badge.svg
+    :target: https://github.com/hiveeyes/apicast/actions?workflow=Tests
+
+.. image:: https://img.shields.io/pypi/pyversions/apicast.svg
+    :target: https://python.org
+
+.. image:: https://img.shields.io/pypi/v/apicast.svg
+    :target: https://pypi.org/project/apicast/
+
+.. image:: https://img.shields.io/pypi/status/apicast.svg
+    :target: https://pypi.org/project/apicast/
+
+.. image:: https://img.shields.io/pypi/l/apicast.svg
+    :target: https://pypi.org/project/apicast/
+
+.. image:: https://static.pepy.tech/badge/apicast/month
+    :target: https://pepy.tech/project/apicast
+
+|
+
+#######
+Apicast
+#######
+
+
+*****
+About
+*****
+
+Apicast acquires bee flight forecast information published by Deutscher Wetterdienst (DWD).
+
+- **Live API**: http://apicast.hiveeyes.org/
+- **Development**: https://community.hiveeyes.org/t/dwd-prognose-bienenflug/787
+
+
+*****
+Setup
+*****
+
+CLI version::
+
+    pip install apicast
+
+HTTP API::
+
+    pip install apicast[service]
+
+
+********
+Synopsis
+********
+
+Display list of states and sites::
+
+    apicast beeflight stations
+
+Display list of location slugs::
+
+    apicast beeflight stations --slugs
+
+Acquire information for given location slug ``brandenburg/potsdam``::
+
+    apicast beeflight forecast --station=brandenburg/potsdam
+
+Acquire information for given location slug ``brandenburg/potsdam``, output as table in Markdown format::
+
+    apicast beeflight forecast --station=brandenburg/potsdam --format=table-markdown
+
+Output as table in JSON machine readable format::
+
+    apicast beeflight forecast --station=brandenburg/potsdam --format=json-machine
+
+
+
+********
+HTTP API
+********
+
+Start HTTP API service::
+
+    apicast service
+
+Start HTTP service with dynamic code reloading::
+
+    apicast service --reload
+
+Then navigate to::
+
+    open http://localhost:24640/
+
+
+
+*******
+Example
+*******
+
+::
+
+    apicast beeflight forecast --station=brandenburg/potsdam
+
+::
+
+    [
+        {
+            "Datum": "Mo 01.06.",
+            "morgens": "stark",
+            "mittags": "intensiv",
+            "abends": "stark"
+        },
+        {
+            "Datum": "Di 02.06.",
+            "morgens": "stark",
+            "mittags": "intensiv",
+            "abends": "intensiv"
+        },
+        {
+            "Datum": "Mi 03.06.",
+            "morgens": "intensiv",
+            "mittags": "intensiv",
+            "abends": "intensiv"
+        }
+    ]
+
+
+*****
+Tests
+*****
+
+::
+
+    make test
+
+
+********************
+Content attributions
+********************
+
+The copyright of data, particular images and pictograms are held by their respective owners, unless otherwise noted.
+
+Data
+====
+
+- **Source**:
+
+  - https://www.dwd.de/DE/leistungen/biene_flug/bienenflug.html
+  - https://www.dwd.de/DE/fachnutzer/freizeitgaertner/1_gartenwetter/_node.html
+
+- **Documentation**:
+
+  - https://www.dwd.de/DE/fachnutzer/freizeitgaertner/dokumentation/gw_bienenflug
+  - https://www.dwd.de/DE/fachnutzer/freizeitgaertner/dokumentation/gw_bienenflug.pdf?__blob=publicationFile
+
+- **Data copyright**: © Deutscher Wetterdienst (DWD), Agricultural Meteorology Department
+
+
+Logo picture
+============
+
+- **Description**:     	A bee swarm on an oak tree in Plymouth, UK
+- **Date**:    	        21 June 2009
+- **Source**: 	        Own work
+- **Author**: 	        Nilfanion
+- **Camera location**:	50° 24′ 38.3″ N, 4° 09′ 28.2″ W
+- **License**:          Creative Commons Attribution-Share Alike 3.0 Unported
+- **URL**:              https://commons.wikimedia.org/wiki/File:Bee_swarm_in_Plymouth.jpg
```

### Comparing `apicast-0.8.4/README.rst` & `apicast-0.8.5/README.rst`

 * *Files identical despite different names*

### Comparing `apicast-0.8.4/apicast/api.py` & `apicast-0.8.5/apicast/api.py`

 * *Files identical despite different names*

### Comparing `apicast-0.8.4/apicast/cli.py` & `apicast-0.8.5/apicast/cli.py`

 * *Files identical despite different names*

### Comparing `apicast-0.8.4/apicast/core.py` & `apicast-0.8.5/apicast/core.py`

 * *Files identical despite different names*

### Comparing `apicast-0.8.4/apicast/format.py` & `apicast-0.8.5/apicast/format.py`

 * *Files identical despite different names*

### Comparing `apicast-0.8.4/apicast/util.py` & `apicast-0.8.5/apicast/util.py`

 * *Files identical despite different names*

### Comparing `apicast-0.8.4/apicast.egg-info/PKG-INFO` & `apicast-0.8.5/apicast.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,183 +1,16 @@
 Metadata-Version: 2.1
 Name: apicast
-Version: 0.8.4
+Version: 0.8.5
 Summary: Python client and HTTP service to access bee flight forecast information published by Deutscher Wetterdienst (DWD), the federal meteorological service in Germany.
 Home-page: https://github.com/hiveeyes/apicast
 Author: Andreas Motl
 Author-email: andreas@hiveeyes.org
 License: AGPL 3, EUPL 1.2
-Description: .. image:: https://github.com/hiveeyes/apicast/workflows/Tests/badge.svg
-            :target: https://github.com/hiveeyes/apicast/actions?workflow=Tests
-        
-        .. image:: https://img.shields.io/pypi/pyversions/apicast.svg
-            :target: https://python.org
-        
-        .. image:: https://img.shields.io/pypi/v/apicast.svg
-            :target: https://pypi.org/project/apicast/
-        
-        .. image:: https://img.shields.io/pypi/status/apicast.svg
-            :target: https://pypi.org/project/apicast/
-        
-        .. image:: https://img.shields.io/pypi/l/apicast.svg
-            :target: https://pypi.org/project/apicast/
-        
-        .. image:: https://static.pepy.tech/badge/apicast/month
-            :target: https://pepy.tech/project/apicast
-        
-        |
-        
-        #######
-        Apicast
-        #######
-        
-        
-        *****
-        About
-        *****
-        
-        Apicast acquires bee flight forecast information published by Deutscher Wetterdienst (DWD).
-        
-        - **Live API**: http://apicast.hiveeyes.org/
-        - **Development**: https://community.hiveeyes.org/t/dwd-prognose-bienenflug/787
-        
-        
-        *****
-        Setup
-        *****
-        
-        CLI version::
-        
-            pip install apicast
-        
-        HTTP API::
-        
-            pip install apicast[service]
-        
-        
-        ********
-        Synopsis
-        ********
-        
-        Display list of states and sites::
-        
-            apicast beeflight stations
-        
-        Display list of location slugs::
-        
-            apicast beeflight stations --slugs
-        
-        Acquire information for given location slug ``brandenburg/potsdam``::
-        
-            apicast beeflight forecast --station=brandenburg/potsdam
-        
-        Acquire information for given location slug ``brandenburg/potsdam``, output as table in Markdown format::
-        
-            apicast beeflight forecast --station=brandenburg/potsdam --format=table-markdown
-        
-        Output as table in JSON machine readable format::
-        
-            apicast beeflight forecast --station=brandenburg/potsdam --format=json-machine
-        
-        
-        
-        ********
-        HTTP API
-        ********
-        
-        Start HTTP API service::
-        
-            apicast service
-        
-        Start HTTP service with dynamic code reloading::
-        
-            apicast service --reload
-        
-        Then navigate to::
-        
-            open http://localhost:24640/
-        
-        
-        
-        *******
-        Example
-        *******
-        
-        ::
-        
-            apicast beeflight forecast --station=brandenburg/potsdam
-        
-        ::
-        
-            [
-                {
-                    "Datum": "Mo 01.06.",
-                    "morgens": "stark",
-                    "mittags": "intensiv",
-                    "abends": "stark"
-                },
-                {
-                    "Datum": "Di 02.06.",
-                    "morgens": "stark",
-                    "mittags": "intensiv",
-                    "abends": "intensiv"
-                },
-                {
-                    "Datum": "Mi 03.06.",
-                    "morgens": "intensiv",
-                    "mittags": "intensiv",
-                    "abends": "intensiv"
-                }
-            ]
-        
-        
-        *****
-        Tests
-        *****
-        
-        ::
-        
-            make test
-        
-        
-        ********************
-        Content attributions
-        ********************
-        
-        The copyright of data, particular images and pictograms are held by their respective owners, unless otherwise noted.
-        
-        Data
-        ====
-        
-        - **Source**:
-        
-          - https://www.dwd.de/DE/leistungen/biene_flug/bienenflug.html
-          - https://www.dwd.de/DE/fachnutzer/freizeitgaertner/1_gartenwetter/_node.html
-        
-        - **Documentation**:
-        
-          - https://www.dwd.de/DE/fachnutzer/freizeitgaertner/dokumentation/gw_bienenflug
-          - https://www.dwd.de/DE/fachnutzer/freizeitgaertner/dokumentation/gw_bienenflug.pdf?__blob=publicationFile
-        
-        - **Data copyright**: © Deutscher Wetterdienst (DWD), Agricultural Meteorology Department
-        
-        
-        Logo picture
-        ============
-        
-        - **Description**:     	A bee swarm on an oak tree in Plymouth, UK
-        - **Date**:    	        21 June 2009
-        - **Source**: 	        Own work
-        - **Author**: 	        Nilfanion
-        - **Camera location**:	50° 24′ 38.3″ N, 4° 09′ 28.2″ W
-        - **License**:          Creative Commons Attribution-Share Alike 3.0 Unported
-        - **URL**:              https://commons.wikimedia.org/wiki/File:Bee_swarm_in_Plymouth.jpg
-        
 Keywords: honey bee apis mellifera flight forecast information dwd cdc deutscher wetterdienst climate data center weather opendata data acquisition transformation export geospatial temporal timeseries sensor network observation http rest api json markdown
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -206,7 +39,174 @@
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Provides-Extra: service
+License-File: LICENSE
+
+.. image:: https://github.com/hiveeyes/apicast/workflows/Tests/badge.svg
+    :target: https://github.com/hiveeyes/apicast/actions?workflow=Tests
+
+.. image:: https://img.shields.io/pypi/pyversions/apicast.svg
+    :target: https://python.org
+
+.. image:: https://img.shields.io/pypi/v/apicast.svg
+    :target: https://pypi.org/project/apicast/
+
+.. image:: https://img.shields.io/pypi/status/apicast.svg
+    :target: https://pypi.org/project/apicast/
+
+.. image:: https://img.shields.io/pypi/l/apicast.svg
+    :target: https://pypi.org/project/apicast/
+
+.. image:: https://static.pepy.tech/badge/apicast/month
+    :target: https://pepy.tech/project/apicast
+
+|
+
+#######
+Apicast
+#######
+
+
+*****
+About
+*****
+
+Apicast acquires bee flight forecast information published by Deutscher Wetterdienst (DWD).
+
+- **Live API**: http://apicast.hiveeyes.org/
+- **Development**: https://community.hiveeyes.org/t/dwd-prognose-bienenflug/787
+
+
+*****
+Setup
+*****
+
+CLI version::
+
+    pip install apicast
+
+HTTP API::
+
+    pip install apicast[service]
+
+
+********
+Synopsis
+********
+
+Display list of states and sites::
+
+    apicast beeflight stations
+
+Display list of location slugs::
+
+    apicast beeflight stations --slugs
+
+Acquire information for given location slug ``brandenburg/potsdam``::
+
+    apicast beeflight forecast --station=brandenburg/potsdam
+
+Acquire information for given location slug ``brandenburg/potsdam``, output as table in Markdown format::
+
+    apicast beeflight forecast --station=brandenburg/potsdam --format=table-markdown
+
+Output as table in JSON machine readable format::
+
+    apicast beeflight forecast --station=brandenburg/potsdam --format=json-machine
+
+
+
+********
+HTTP API
+********
+
+Start HTTP API service::
+
+    apicast service
+
+Start HTTP service with dynamic code reloading::
+
+    apicast service --reload
+
+Then navigate to::
+
+    open http://localhost:24640/
+
+
+
+*******
+Example
+*******
+
+::
+
+    apicast beeflight forecast --station=brandenburg/potsdam
+
+::
+
+    [
+        {
+            "Datum": "Mo 01.06.",
+            "morgens": "stark",
+            "mittags": "intensiv",
+            "abends": "stark"
+        },
+        {
+            "Datum": "Di 02.06.",
+            "morgens": "stark",
+            "mittags": "intensiv",
+            "abends": "intensiv"
+        },
+        {
+            "Datum": "Mi 03.06.",
+            "morgens": "intensiv",
+            "mittags": "intensiv",
+            "abends": "intensiv"
+        }
+    ]
+
+
+*****
+Tests
+*****
+
+::
+
+    make test
+
+
+********************
+Content attributions
+********************
+
+The copyright of data, particular images and pictograms are held by their respective owners, unless otherwise noted.
+
+Data
+====
+
+- **Source**:
+
+  - https://www.dwd.de/DE/leistungen/biene_flug/bienenflug.html
+  - https://www.dwd.de/DE/fachnutzer/freizeitgaertner/1_gartenwetter/_node.html
+
+- **Documentation**:
+
+  - https://www.dwd.de/DE/fachnutzer/freizeitgaertner/dokumentation/gw_bienenflug
+  - https://www.dwd.de/DE/fachnutzer/freizeitgaertner/dokumentation/gw_bienenflug.pdf?__blob=publicationFile
+
+- **Data copyright**: © Deutscher Wetterdienst (DWD), Agricultural Meteorology Department
+
+
+Logo picture
+============
+
+- **Description**:     	A bee swarm on an oak tree in Plymouth, UK
+- **Date**:    	        21 June 2009
+- **Source**: 	        Own work
+- **Author**: 	        Nilfanion
+- **Camera location**:	50° 24′ 38.3″ N, 4° 09′ 28.2″ W
+- **License**:          Creative Commons Attribution-Share Alike 3.0 Unported
+- **URL**:              https://commons.wikimedia.org/wiki/File:Bee_swarm_in_Plymouth.jpg
```

### Comparing `apicast-0.8.4/setup.py` & `apicast-0.8.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 README = open(os.path.join(here, "README.rst"), encoding="UTF-8").read()
 
 setup(
     name="apicast",
-    version="0.8.4",
+    version="0.8.5",
     description="Python client and HTTP service to access bee flight forecast "
                 "information published by Deutscher Wetterdienst (DWD), the "
                 "federal meteorological service in Germany.",
     long_description=README,
     license="AGPL 3, EUPL 1.2",
     classifiers=[
         "Programming Language :: Python",
@@ -64,15 +64,15 @@
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "beautifulsoup4>=4,<5",
         "dateparser>=0.7.4,<1",
         "docopt>=0.6,<1",
         "html-table-extractor>=1,<2",
-        "jsonpickle>=2,<3"
+        "jsonpickle>=2,<3",
         "munch>=2.5,<3",
         "python-slugify>=4,<5",
         "requests>=2,<3",
         "tabulate>=0.8,<0.9",
         "ttl-cache>=1.6,<2",
         "tzlocal>=2,<3",
     ],
```

### Comparing `apicast-0.8.4/test/test_data.py` & `apicast-0.8.5/test/test_data.py`

 * *Files identical despite different names*

### Comparing `apicast-0.8.4/test/test_locations.py` & `apicast-0.8.5/test/test_locations.py`

 * *Files identical despite different names*

