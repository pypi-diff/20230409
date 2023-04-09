# Comparing `tmp/vibe-chart.py-1.0.0.tar.gz` & `tmp/vibe-chart.py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vibe-chart.py-1.0.0.tar", last modified: Sun Apr  9 09:32:56 2023, max compression
+gzip compressed data, was "vibe-chart.py-1.0.1.tar", last modified: Sun Apr  9 12:08:57 2023, max compression
```

## Comparing `vibe-chart.py-1.0.0.tar` & `vibe-chart.py-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jieunpark   (501) staff       (20)        0 2023-04-09 09:32:56.643967 vibe-chart.py-1.0.0/
--rw-r--r--   0 jieunpark   (501) staff       (20)     1065 2023-04-09 09:32:19.000000 vibe-chart.py-1.0.0/LICENSE
--rw-r--r--   0 jieunpark   (501) staff       (20)     2055 2023-04-09 09:32:56.625563 vibe-chart.py-1.0.0/PKG-INFO
--rw-r--r--   0 jieunpark   (501) staff       (20)     1752 2023-04-09 09:28:59.000000 vibe-chart.py-1.0.0/README.md
--rw-r--r--   0 jieunpark   (501) staff       (20)       38 2023-04-09 09:32:56.644081 vibe-chart.py-1.0.0/setup.cfg
--rw-r--r--   0 jieunpark   (501) staff       (20)      548 2023-04-09 09:31:57.000000 vibe-chart.py-1.0.0/setup.py
--rw-r--r--   0 jieunpark   (501) staff       (20)     4944 2023-04-09 09:28:09.000000 vibe-chart.py-1.0.0/vibe.py
-drwxr-xr-x   0 jieunpark   (501) staff       (20)        0 2023-04-09 09:32:56.625357 vibe-chart.py-1.0.0/vibe_chart.py.egg-info/
--rw-r--r--   0 jieunpark   (501) staff       (20)     2055 2023-04-09 09:32:56.000000 vibe-chart.py-1.0.0/vibe_chart.py.egg-info/PKG-INFO
--rw-r--r--   0 jieunpark   (501) staff       (20)      218 2023-04-09 09:32:56.000000 vibe-chart.py-1.0.0/vibe_chart.py.egg-info/SOURCES.txt
--rw-r--r--   0 jieunpark   (501) staff       (20)        1 2023-04-09 09:32:56.000000 vibe-chart.py-1.0.0/vibe_chart.py.egg-info/dependency_links.txt
--rw-r--r--   0 jieunpark   (501) staff       (20)       17 2023-04-09 09:32:56.000000 vibe-chart.py-1.0.0/vibe_chart.py.egg-info/requires.txt
--rw-r--r--   0 jieunpark   (501) staff       (20)        5 2023-04-09 09:32:56.000000 vibe-chart.py-1.0.0/vibe_chart.py.egg-info/top_level.txt
+drwxr-xr-x   0 jieunpark   (501) staff       (20)        0 2023-04-09 12:08:57.831218 vibe-chart.py-1.0.1/
+-rw-r--r--   0 jieunpark   (501) staff       (20)     1065 2023-04-09 09:32:19.000000 vibe-chart.py-1.0.1/LICENSE
+-rw-r--r--   0 jieunpark   (501) staff       (20)     2190 2023-04-09 12:08:57.831085 vibe-chart.py-1.0.1/PKG-INFO
+-rw-r--r--   0 jieunpark   (501) staff       (20)     1887 2023-04-09 12:08:21.000000 vibe-chart.py-1.0.1/README.md
+-rw-r--r--   0 jieunpark   (501) staff       (20)       38 2023-04-09 12:08:57.831266 vibe-chart.py-1.0.1/setup.cfg
+-rw-r--r--   0 jieunpark   (501) staff       (20)      548 2023-04-09 12:08:35.000000 vibe-chart.py-1.0.1/setup.py
+-rw-r--r--   0 jieunpark   (501) staff       (20)     5267 2023-04-09 12:07:25.000000 vibe-chart.py-1.0.1/vibe.py
+drwxr-xr-x   0 jieunpark   (501) staff       (20)        0 2023-04-09 12:08:57.830901 vibe-chart.py-1.0.1/vibe_chart.py.egg-info/
+-rw-r--r--   0 jieunpark   (501) staff       (20)     2190 2023-04-09 12:08:57.000000 vibe-chart.py-1.0.1/vibe_chart.py.egg-info/PKG-INFO
+-rw-r--r--   0 jieunpark   (501) staff       (20)      218 2023-04-09 12:08:57.000000 vibe-chart.py-1.0.1/vibe_chart.py.egg-info/SOURCES.txt
+-rw-r--r--   0 jieunpark   (501) staff       (20)        1 2023-04-09 12:08:57.000000 vibe-chart.py-1.0.1/vibe_chart.py.egg-info/dependency_links.txt
+-rw-r--r--   0 jieunpark   (501) staff       (20)       17 2023-04-09 12:08:57.000000 vibe-chart.py-1.0.1/vibe_chart.py.egg-info/requires.txt
+-rw-r--r--   0 jieunpark   (501) staff       (20)        5 2023-04-09 12:08:57.000000 vibe-chart.py-1.0.1/vibe_chart.py.egg-info/top_level.txt
```

### Comparing `vibe-chart.py-1.0.0/LICENSE` & `vibe-chart.py-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vibe-chart.py-1.0.0/PKG-INFO` & `vibe-chart.py-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vibe-chart.py
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python API for downloading Naver Vibe charts
 Home-page: https://github.com/gold24park/vibe-chart.py
 Author: Lou Park
 Author-email: gold24park@gmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -29,17 +29,23 @@
     "artist": "IVE(아이브)",
     "image": "https://musicmeta-phinf.pstatic.net/album/009/334/9334427.jpg?type=r500Fll&v=20230404132130",
     "isNew": false,
     "lastPos": 1,
     "rank": 1,
     "title": "Kitsch"
 }
+>>> print(chart.name)
+오늘 Top 100
+>>> print(chart.date)
+2023-04-09 07:00:00
 ```
 
 ### ChartData Arguments
+- `name` – The chart name
+- `date` – The chart date
 - `queryStart` – The starting index of the chart entries to be retrieved from the Vibe API. (default: 1)
 - `queryCount` – The number of items to retrieve from the API response, starting from `queryStart`. (default: 100)
 - `imageSize` – The size of cover image for the track. (default: 256)
 - `fetch` – A boolean value that indicates whether to retrieve the chart data immediately. If set to `False`, you can fetch the data later using the `fetchEntries()` method.
 
 ### Chart entry attributes
 `ChartEntry` can be accessed using the `ChartData[index]` syntax. A `ChartEntry` instance has the following attributes:
```

### Comparing `vibe-chart.py-1.0.0/README.md` & `vibe-chart.py-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,23 @@
     "artist": "IVE(아이브)",
     "image": "https://musicmeta-phinf.pstatic.net/album/009/334/9334427.jpg?type=r500Fll&v=20230404132130",
     "isNew": false,
     "lastPos": 1,
     "rank": 1,
     "title": "Kitsch"
 }
+>>> print(chart.name)
+오늘 Top 100
+>>> print(chart.date)
+2023-04-09 07:00:00
 ```
 
 ### ChartData Arguments
+- `name` – The chart name
+- `date` – The chart date
 - `queryStart` – The starting index of the chart entries to be retrieved from the Vibe API. (default: 1)
 - `queryCount` – The number of items to retrieve from the API response, starting from `queryStart`. (default: 100)
 - `imageSize` – The size of cover image for the track. (default: 256)
 - `fetch` – A boolean value that indicates whether to retrieve the chart data immediately. If set to `False`, you can fetch the data later using the `fetchEntries()` method.
 
 ### Chart entry attributes
 `ChartEntry` can be accessed using the `ChartData[index]` syntax. A `ChartEntry` instance has the following attributes:
```

### Comparing `vibe-chart.py-1.0.0/setup.py` & `vibe-chart.py-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="vibe-chart.py",
-    version="1.0.0",
+    version="1.0.1",
     description="Python API for downloading Naver Vibe charts",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Lou Park",
     author_email="gold24park@gmail.com",
     url="https://github.com/gold24park/vibe-chart.py",
     py_modules=["vibe"],
```

### Comparing `vibe-chart.py-1.0.0/vibe.py` & `vibe-chart.py-1.0.1/vibe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import sys
 import urllib.parse
+from datetime import datetime
 
 import requests
 
 _USER_AGENT = "Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Mobile Safari/537.36"
 _ACCEPT = "application/json"
 _CHART_API_URL = "https://apis.naver.com/vibeWeb/musicapiweb/vibe/v1/chart/track/total"
 
@@ -27,14 +28,15 @@
         title: The title of the track
         artist: The name of the artist.
         image: The URL of the cover image for the track
         lastPos: The track's last position on the previous period.
         rank: The track's current rank position on the chart.
         isNew: Whether the track is new to the chart.
     """
+
     def __init__(self, title: str, artist: str, image: str, lastPos: int, rank: int, isNew: bool):
         self.title = title
         self.artist = artist
         self.image = image
         self.lastPos = lastPos
         self.rank = rank
         self.isNew = isNew
@@ -59,19 +61,22 @@
     def json(self):
         return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=4, ensure_ascii=False)
 
 
 class ChartData:
     """Represents a particular Bugs chart by a particular period.
     Attributes:
+        name: The chart name
+        date: The chart date
         queryStart: The starting index of the chart entries to be retrieved from the Vibe API. (default: 1)
         queryCount: The number of items to retrieve from the API response, starting from `queryStart`. (default: 100)
         imageSize: The size of cover image for the track. (default: 256)
         fetch: A boolean value that indicates whether to retrieve the chart data immediately. If set to `False`, you can fetch the data later using the `fetchEntries()` method.
     """
+
     def __init__(self, queryStart: int = 1, queryCount: int = 100, imageSize: int = 256, fetch: bool = True):
         self.maxQueryCount = 0
         self.queryStart = queryStart
         self.queryCount = queryCount
         self.imageSize = imageSize
         self.entries = []
 
@@ -108,14 +113,16 @@
         data = res.json()
 
         self._parseEntries(data)
 
     def _parseEntries(self, data):
         try:
             c_data = data['response']['result']['chart']
+            self.name = c_data['title']
+            self.date = self._parseDate(c_data['date'])
             self.maxQueryCount = int(c_data['chartTotalCount'])
 
             for item in c_data['items']['tracks']:
                 entry = ChartEntry(
                     title=item['trackTitle'],
                     artist=item['artists'][0]['artistName'],
                     image=self._getResizedImageUrl(item['album']['imageUrl']),
@@ -125,14 +132,18 @@
                 )
                 entry.lastPos = entry.rank + int(item['rank']['rankVariation'])
                 self.entries.append(entry)
 
         except Exception as e:
             raise VibeChartParseException(e)
 
+    def _parseDate(self, timestamp_ms):
+        timestamp_s = timestamp_ms / 1000
+        return datetime.utcfromtimestamp(timestamp_s)
+
     def _getResizedImageUrl(self, url):
         parsed_url = urllib.parse.urlparse(url)
         query_params = urllib.parse.parse_qs(parsed_url.query)
         query_params['type'] = f'r{self.imageSize}Fll'
 
         new_query_string = urllib.parse.urlencode(query_params, doseq=True)
         return urllib.parse.urlunparse(
```

### Comparing `vibe-chart.py-1.0.0/vibe_chart.py.egg-info/PKG-INFO` & `vibe-chart.py-1.0.1/vibe_chart.py.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vibe-chart.py
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python API for downloading Naver Vibe charts
 Home-page: https://github.com/gold24park/vibe-chart.py
 Author: Lou Park
 Author-email: gold24park@gmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -29,17 +29,23 @@
     "artist": "IVE(아이브)",
     "image": "https://musicmeta-phinf.pstatic.net/album/009/334/9334427.jpg?type=r500Fll&v=20230404132130",
     "isNew": false,
     "lastPos": 1,
     "rank": 1,
     "title": "Kitsch"
 }
+>>> print(chart.name)
+오늘 Top 100
+>>> print(chart.date)
+2023-04-09 07:00:00
 ```
 
 ### ChartData Arguments
+- `name` – The chart name
+- `date` – The chart date
 - `queryStart` – The starting index of the chart entries to be retrieved from the Vibe API. (default: 1)
 - `queryCount` – The number of items to retrieve from the API response, starting from `queryStart`. (default: 100)
 - `imageSize` – The size of cover image for the track. (default: 256)
 - `fetch` – A boolean value that indicates whether to retrieve the chart data immediately. If set to `False`, you can fetch the data later using the `fetchEntries()` method.
 
 ### Chart entry attributes
 `ChartEntry` can be accessed using the `ChartData[index]` syntax. A `ChartEntry` instance has the following attributes:
```

