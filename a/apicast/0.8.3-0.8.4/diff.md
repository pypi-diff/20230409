# Comparing `tmp/apicast-0.8.3.tar.gz` & `tmp/apicast-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apicast-0.8.3.tar", last modified: Fri Mar  5 22:35:54 2021, max compression
+gzip compressed data, was "apicast-0.8.4.tar", last modified: Sun Apr  9 12:44:37 2023, max compression
```

## Comparing `apicast-0.8.3.tar` & `apicast-0.8.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2021-03-05 22:35:54.428547 apicast-0.8.3/
--rw-r--r--   0 amo        (501) staff       (20)     7236 2021-03-05 22:35:54.428207 apicast-0.8.3/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     3567 2021-03-05 21:42:36.000000 apicast-0.8.3/README.rst
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2021-03-05 22:35:54.424377 apicast-0.8.3/apicast/
--rw-r--r--   0 amo        (501) staff       (20)      133 2021-03-05 22:35:48.000000 apicast-0.8.3/apicast/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     6711 2021-03-05 22:27:00.000000 apicast-0.8.3/apicast/api.py
--rw-r--r--   0 amo        (501) staff       (20)     4030 2021-03-05 21:56:14.000000 apicast-0.8.3/apicast/cli.py
--rw-r--r--   0 amo        (501) staff       (20)     4816 2021-03-05 22:19:12.000000 apicast-0.8.3/apicast/core.py
--rw-r--r--   0 amo        (501) staff       (20)     2665 2021-03-05 22:34:57.000000 apicast-0.8.3/apicast/format.py
--rw-r--r--   0 amo        (501) staff       (20)     1124 2021-03-05 21:56:14.000000 apicast-0.8.3/apicast/util.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2021-03-05 22:35:54.426563 apicast-0.8.3/apicast.egg-info/
--rw-r--r--   0 amo        (501) staff       (20)     7236 2021-03-05 22:35:54.000000 apicast-0.8.3/apicast.egg-info/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)      348 2021-03-05 22:35:54.000000 apicast-0.8.3/apicast.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2021-03-05 22:35:54.000000 apicast-0.8.3/apicast.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (501) staff       (20)       45 2021-03-05 22:35:54.000000 apicast-0.8.3/apicast.egg-info/entry_points.txt
--rw-r--r--   0 amo        (501) staff       (20)      269 2021-03-05 22:35:54.000000 apicast-0.8.3/apicast.egg-info/requires.txt
--rw-r--r--   0 amo        (501) staff       (20)        8 2021-03-05 22:35:54.000000 apicast-0.8.3/apicast.egg-info/top_level.txt
--rw-r--r--   0 amo        (501) staff       (20)       38 2021-03-05 22:35:54.428658 apicast-0.8.3/setup.cfg
--rw-r--r--   0 amo        (501) staff       (20)     3306 2021-03-05 22:35:48.000000 apicast-0.8.3/setup.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2021-03-05 22:35:54.427439 apicast-0.8.3/test/
--rw-r--r--   0 amo        (501) staff       (20)     1081 2021-03-05 00:45:04.000000 apicast-0.8.3/test/test_data.py
--rw-r--r--   0 amo        (501) staff       (20)     1344 2021-03-05 00:44:44.000000 apicast-0.8.3/test/test_locations.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-09 12:44:37.916535 apicast-0.8.4/
+-rw-r--r--   0 amo        (501) staff       (20)     7359 2023-04-09 12:44:37.916258 apicast-0.8.4/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     3572 2023-04-09 12:43:09.000000 apicast-0.8.4/README.rst
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-09 12:44:37.913661 apicast-0.8.4/apicast/
+-rw-r--r--   0 amo        (501) staff       (20)      133 2023-04-09 12:44:34.000000 apicast-0.8.4/apicast/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     6711 2021-03-05 22:27:00.000000 apicast-0.8.4/apicast/api.py
+-rw-r--r--   0 amo        (501) staff       (20)     4030 2021-03-05 21:56:14.000000 apicast-0.8.4/apicast/cli.py
+-rw-r--r--   0 amo        (501) staff       (20)     4810 2023-04-09 12:43:09.000000 apicast-0.8.4/apicast/core.py
+-rw-r--r--   0 amo        (501) staff       (20)     2665 2021-03-05 22:34:57.000000 apicast-0.8.4/apicast/format.py
+-rw-r--r--   0 amo        (501) staff       (20)     1124 2021-03-05 21:56:14.000000 apicast-0.8.4/apicast/util.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-09 12:44:37.915372 apicast-0.8.4/apicast.egg-info/
+-rw-r--r--   0 amo        (501) staff       (20)     7359 2023-04-09 12:44:37.000000 apicast-0.8.4/apicast.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)      348 2023-04-09 12:44:37.000000 apicast-0.8.4/apicast.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2023-04-09 12:44:37.000000 apicast-0.8.4/apicast.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (501) staff       (20)       45 2023-04-09 12:44:37.000000 apicast-0.8.4/apicast.egg-info/entry_points.txt
+-rw-r--r--   0 amo        (501) staff       (20)      250 2023-04-09 12:44:37.000000 apicast-0.8.4/apicast.egg-info/requires.txt
+-rw-r--r--   0 amo        (501) staff       (20)        8 2023-04-09 12:44:37.000000 apicast-0.8.4/apicast.egg-info/top_level.txt
+-rw-r--r--   0 amo        (501) staff       (20)       38 2023-04-09 12:44:37.916638 apicast-0.8.4/setup.cfg
+-rw-r--r--   0 amo        (501) staff       (20)     3376 2023-04-09 12:44:34.000000 apicast-0.8.4/setup.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-09 12:44:37.915844 apicast-0.8.4/test/
+-rw-r--r--   0 amo        (501) staff       (20)     1081 2021-03-05 00:45:04.000000 apicast-0.8.4/test/test_data.py
+-rw-r--r--   0 amo        (501) staff       (20)     1344 2021-03-05 00:44:44.000000 apicast-0.8.4/test/test_locations.py
```

### Comparing `apicast-0.8.3/PKG-INFO` & `apicast-0.8.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: apicast
-Version: 0.8.3
+Version: 0.8.4
 Summary: Python client and HTTP service to access bee flight forecast information published by Deutscher Wetterdienst (DWD), the federal meteorological service in Germany.
 Home-page: https://github.com/hiveeyes/apicast
 Author: Andreas Motl
 Author-email: andreas@hiveeyes.org
 License: AGPL 3, EUPL 1.2
-Description: #######
-        Apicast
-        #######
-        
-        .. image:: https://github.com/hiveeyes/apicast/workflows/Tests/badge.svg
+Description: .. image:: https://github.com/hiveeyes/apicast/workflows/Tests/badge.svg
             :target: https://github.com/hiveeyes/apicast/actions?workflow=Tests
         
         .. image:: https://img.shields.io/pypi/pyversions/apicast.svg
             :target: https://python.org
         
         .. image:: https://img.shields.io/pypi/v/apicast.svg
             :target: https://pypi.org/project/apicast/
         
         .. image:: https://img.shields.io/pypi/status/apicast.svg
             :target: https://pypi.org/project/apicast/
         
         .. image:: https://img.shields.io/pypi/l/apicast.svg
             :target: https://pypi.org/project/apicast/
         
-        .. image:: https://img.shields.io/pypi/dm/apicast.svg
-            :target: https://pypi.org/project/apicast/
+        .. image:: https://static.pepy.tech/badge/apicast/month
+            :target: https://pepy.tech/project/apicast
+        
+        |
+        
+        #######
+        Apicast
+        #######
         
         
         *****
         About
         *****
         
         Apicast acquires bee flight forecast information published by Deutscher Wetterdienst (DWD).
@@ -174,14 +176,16 @@
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `apicast-0.8.3/README.rst` & `apicast-0.8.4/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-#######
-Apicast
-#######
-
 .. image:: https://github.com/hiveeyes/apicast/workflows/Tests/badge.svg
     :target: https://github.com/hiveeyes/apicast/actions?workflow=Tests
 
 .. image:: https://img.shields.io/pypi/pyversions/apicast.svg
     :target: https://python.org
 
 .. image:: https://img.shields.io/pypi/v/apicast.svg
@@ -13,16 +9,22 @@
 
 .. image:: https://img.shields.io/pypi/status/apicast.svg
     :target: https://pypi.org/project/apicast/
 
 .. image:: https://img.shields.io/pypi/l/apicast.svg
     :target: https://pypi.org/project/apicast/
 
-.. image:: https://img.shields.io/pypi/dm/apicast.svg
-    :target: https://pypi.org/project/apicast/
+.. image:: https://static.pepy.tech/badge/apicast/month
+    :target: https://pepy.tech/project/apicast
+
+|
+
+#######
+Apicast
+#######
 
 
 *****
 About
 *****
 
 Apicast acquires bee flight forecast information published by Deutscher Wetterdienst (DWD).
```

### Comparing `apicast-0.8.3/apicast/api.py` & `apicast-0.8.4/apicast/api.py`

 * *Files identical despite different names*

### Comparing `apicast-0.8.3/apicast/cli.py` & `apicast-0.8.4/apicast/cli.py`

 * *Files identical despite different names*

### Comparing `apicast-0.8.3/apicast/core.py` & `apicast-0.8.4/apicast/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 
 import requests
 import ttl_cache
 from bs4 import BeautifulSoup
 from html_table_extractor.extractor import Extractor
 from slugify import slugify
 
-user_agent = (
-    "Mozilla/5.0 (Macintosh; Intel Mac OS X 10.15; rv:86.0) Gecko/20100101 Firefox/86.0"
-)
+from apicast import __appname__, __version__
+
+
+user_agent = f"{__appname__}/{__version__}"
 dwd_source = "https://www.dwd.de/DE/leistungen/biene_flug/bienenflug.html"
 dwd_copyright = "© Deutscher Wetterdienst (DWD), Agricultural Meteorology Department"
 producer_name = "Hiveeyes Apicast"
 producer_link = "https://github.com/hiveeyes/apicast"
 
 
 @dataclasses.dataclass
@@ -138,15 +139,15 @@
                 "cl2Categories_Station": station.identifier,
             },
         )
 
         soup = BeautifulSoup(markup=response.content, features="html.parser")
 
         # Find content section and extract elements.
-        headline = soup.find(string="Prognose des Bienenfluges")
+        headline = soup.find(string="Prognose der Bienenflugintensität")
         if not headline:
             raise ValueError("No forecast available for this station")
         station_name = headline.find_next("section").attrs.get("aria-label")
         table = soup.find("table")
 
         footnote = soup.find("aside").find("p").text
```

### Comparing `apicast-0.8.3/apicast/format.py` & `apicast-0.8.4/apicast/format.py`

 * *Files identical despite different names*

### Comparing `apicast-0.8.3/apicast/util.py` & `apicast-0.8.4/apicast/util.py`

 * *Files identical despite different names*

### Comparing `apicast-0.8.3/apicast.egg-info/PKG-INFO` & `apicast-0.8.4/apicast.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: apicast
-Version: 0.8.3
+Version: 0.8.4
 Summary: Python client and HTTP service to access bee flight forecast information published by Deutscher Wetterdienst (DWD), the federal meteorological service in Germany.
 Home-page: https://github.com/hiveeyes/apicast
 Author: Andreas Motl
 Author-email: andreas@hiveeyes.org
 License: AGPL 3, EUPL 1.2
-Description: #######
-        Apicast
-        #######
-        
-        .. image:: https://github.com/hiveeyes/apicast/workflows/Tests/badge.svg
+Description: .. image:: https://github.com/hiveeyes/apicast/workflows/Tests/badge.svg
             :target: https://github.com/hiveeyes/apicast/actions?workflow=Tests
         
         .. image:: https://img.shields.io/pypi/pyversions/apicast.svg
             :target: https://python.org
         
         .. image:: https://img.shields.io/pypi/v/apicast.svg
             :target: https://pypi.org/project/apicast/
         
         .. image:: https://img.shields.io/pypi/status/apicast.svg
             :target: https://pypi.org/project/apicast/
         
         .. image:: https://img.shields.io/pypi/l/apicast.svg
             :target: https://pypi.org/project/apicast/
         
-        .. image:: https://img.shields.io/pypi/dm/apicast.svg
-            :target: https://pypi.org/project/apicast/
+        .. image:: https://static.pepy.tech/badge/apicast/month
+            :target: https://pepy.tech/project/apicast
+        
+        |
+        
+        #######
+        Apicast
+        #######
         
         
         *****
         About
         *****
         
         Apicast acquires bee flight forecast information published by Deutscher Wetterdienst (DWD).
@@ -174,14 +176,16 @@
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `apicast-0.8.3/setup.py` & `apicast-0.8.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 README = open(os.path.join(here, "README.rst"), encoding="UTF-8").read()
 
 setup(
     name="apicast",
-    version="0.8.3",
+    version="0.8.4",
     description="Python client and HTTP service to access bee flight forecast "
                 "information published by Deutscher Wetterdienst (DWD), the "
                 "federal meteorological service in Germany.",
     long_description=README,
     license="AGPL 3, EUPL 1.2",
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)",
         "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Environment :: Web Environment",
@@ -58,25 +60,24 @@
     "geospatial temporal timeseries "
     "sensor network observation "
     "http rest api "
     "json markdown",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
-        "requests>=2,<3",
-        "ttl-cache>=1.6,<2",
         "beautifulsoup4>=4,<5",
-        "html-table-extractor>=1,<2",
-        "python-slugify>=4,<5",
+        "dateparser>=0.7.4,<1",
         "docopt>=0.6,<1",
-        "munch>=2.5,<3",
+        "html-table-extractor>=1,<2",
         "jsonpickle>=2,<3"
+        "munch>=2.5,<3",
         "python-slugify>=4,<5",
-        "tabulate>=0.8,<1",
-        "dateparser>=0.7.4,<1",
+        "requests>=2,<3",
+        "tabulate>=0.8,<0.9",
+        "ttl-cache>=1.6,<2",
         "tzlocal>=2,<3",
     ],
     extras_require={
         "service": [
             "fastapi>=0.55.1,<0.64",
             "uvicorn<=0.13.3",
         ],
```

### Comparing `apicast-0.8.3/test/test_data.py` & `apicast-0.8.4/test/test_data.py`

 * *Files identical despite different names*

### Comparing `apicast-0.8.3/test/test_locations.py` & `apicast-0.8.4/test/test_locations.py`

 * *Files identical despite different names*

