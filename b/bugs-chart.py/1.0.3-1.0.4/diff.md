# Comparing `tmp/bugs-chart.py-1.0.3.tar.gz` & `tmp/bugs-chart.py-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bugs-chart.py-1.0.3.tar", last modified: Sun Apr  9 09:39:22 2023, max compression
+gzip compressed data, was "bugs-chart.py-1.0.4.tar", last modified: Sun Apr  9 12:03:49 2023, max compression
```

## Comparing `bugs-chart.py-1.0.3.tar` & `bugs-chart.py-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jieunpark   (501) staff       (20)        0 2023-04-09 09:39:22.363717 bugs-chart.py-1.0.3/
--rw-r--r--   0 jieunpark   (501) staff       (20)     1074 2023-04-09 04:50:14.000000 bugs-chart.py-1.0.3/LICENSE
--rw-r--r--   0 jieunpark   (501) staff       (20)     2070 2023-04-09 09:39:22.363612 bugs-chart.py-1.0.3/PKG-INFO
--rw-r--r--   0 jieunpark   (501) staff       (20)     1774 2023-04-09 09:39:14.000000 bugs-chart.py-1.0.3/README.md
--rw-r--r--   0 jieunpark   (501) staff       (20)     4464 2023-04-09 09:35:50.000000 bugs-chart.py-1.0.3/bugs.py
-drwxr-xr-x   0 jieunpark   (501) staff       (20)        0 2023-04-09 09:39:22.363436 bugs-chart.py-1.0.3/bugs_chart.py.egg-info/
--rw-r--r--   0 jieunpark   (501) staff       (20)     2070 2023-04-09 09:39:22.000000 bugs-chart.py-1.0.3/bugs_chart.py.egg-info/PKG-INFO
--rw-r--r--   0 jieunpark   (501) staff       (20)      218 2023-04-09 09:39:22.000000 bugs-chart.py-1.0.3/bugs_chart.py.egg-info/SOURCES.txt
--rw-r--r--   0 jieunpark   (501) staff       (20)        1 2023-04-09 09:39:22.000000 bugs-chart.py-1.0.3/bugs_chart.py.egg-info/dependency_links.txt
--rw-r--r--   0 jieunpark   (501) staff       (20)       17 2023-04-09 09:39:22.000000 bugs-chart.py-1.0.3/bugs_chart.py.egg-info/requires.txt
--rw-r--r--   0 jieunpark   (501) staff       (20)        5 2023-04-09 09:39:22.000000 bugs-chart.py-1.0.3/bugs_chart.py.egg-info/top_level.txt
--rw-r--r--   0 jieunpark   (501) staff       (20)       38 2023-04-09 09:39:22.363756 bugs-chart.py-1.0.3/setup.cfg
--rw-r--r--   0 jieunpark   (501) staff       (20)      542 2023-04-09 09:35:30.000000 bugs-chart.py-1.0.3/setup.py
+drwxr-xr-x   0 jieunpark   (501) staff       (20)        0 2023-04-09 12:03:49.893569 bugs-chart.py-1.0.4/
+-rw-r--r--   0 jieunpark   (501) staff       (20)     1074 2023-04-09 04:50:14.000000 bugs-chart.py-1.0.4/LICENSE
+-rw-r--r--   0 jieunpark   (501) staff       (20)     2140 2023-04-09 12:03:49.893443 bugs-chart.py-1.0.4/PKG-INFO
+-rw-r--r--   0 jieunpark   (501) staff       (20)     1844 2023-04-09 12:03:30.000000 bugs-chart.py-1.0.4/README.md
+-rw-r--r--   0 jieunpark   (501) staff       (20)     4731 2023-04-09 12:01:58.000000 bugs-chart.py-1.0.4/bugs.py
+drwxr-xr-x   0 jieunpark   (501) staff       (20)        0 2023-04-09 12:03:49.893225 bugs-chart.py-1.0.4/bugs_chart.py.egg-info/
+-rw-r--r--   0 jieunpark   (501) staff       (20)     2140 2023-04-09 12:03:49.000000 bugs-chart.py-1.0.4/bugs_chart.py.egg-info/PKG-INFO
+-rw-r--r--   0 jieunpark   (501) staff       (20)      218 2023-04-09 12:03:49.000000 bugs-chart.py-1.0.4/bugs_chart.py.egg-info/SOURCES.txt
+-rw-r--r--   0 jieunpark   (501) staff       (20)        1 2023-04-09 12:03:49.000000 bugs-chart.py-1.0.4/bugs_chart.py.egg-info/dependency_links.txt
+-rw-r--r--   0 jieunpark   (501) staff       (20)       17 2023-04-09 12:03:49.000000 bugs-chart.py-1.0.4/bugs_chart.py.egg-info/requires.txt
+-rw-r--r--   0 jieunpark   (501) staff       (20)        5 2023-04-09 12:03:49.000000 bugs-chart.py-1.0.4/bugs_chart.py.egg-info/top_level.txt
+-rw-r--r--   0 jieunpark   (501) staff       (20)       38 2023-04-09 12:03:49.893630 bugs-chart.py-1.0.4/setup.cfg
+-rw-r--r--   0 jieunpark   (501) staff       (20)      542 2023-04-09 12:02:22.000000 bugs-chart.py-1.0.4/setup.py
```

### Comparing `bugs-chart.py-1.0.3/LICENSE` & `bugs-chart.py-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bugs-chart.py-1.0.3/PKG-INFO` & `bugs-chart.py-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bugs-chart.py
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python API for downloading Bugs charts
 Home-page: https://github.com/gold24park/bugs-chart.py
 Author: Lou Park
 Author-email: gold24park@gmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -29,17 +29,20 @@
     "artist": "IVE (아이브)",
     "image": "https://image.bugsm.co.kr/album/images/256/40849/4084947.jpg",
     "lastPos": 1,
     "peakPos": 1,
     "rank": 1,
     "title": "Kitsch"
 }
+>>> print(chart.date)
+2023-04-09 12:00:00
 ```
 
 ### ChartData Arguments
+- `date` – The chart date
 - `chartType`
   - BugsChartType.All – 전체
   - BugsChartType.Domestic – 국내
   - BugsChartType.International – 해외
 - `chartPeriod`
   - BugsChartPeriod.Realtime – 실시간
   - BugsChartPeriod.Daily – 일간
```

### Comparing `bugs-chart.py-1.0.3/README.md` & `bugs-chart.py-1.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,20 @@
     "artist": "IVE (아이브)",
     "image": "https://image.bugsm.co.kr/album/images/256/40849/4084947.jpg",
     "lastPos": 1,
     "peakPos": 1,
     "rank": 1,
     "title": "Kitsch"
 }
+>>> print(chart.date)
+2023-04-09 12:00:00
 ```
 
 ### ChartData Arguments
+- `date` – The chart date
 - `chartType`
   - BugsChartType.All – 전체
   - BugsChartType.Domestic – 국내
   - BugsChartType.International – 해외
 - `chartPeriod`
   - BugsChartPeriod.Realtime – 실시간
   - BugsChartPeriod.Daily – 일간
```

### Comparing `bugs-chart.py-1.0.3/bugs.py` & `bugs-chart.py-1.0.4/bugs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import sys
-
+from datetime import datetime
 import requests
 
 _USER_AGENT = "Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Mobile Safari/537.36"
 _IMAGE_PREFIX_URL = "https://image.bugsm.co.kr/album/images"
 _CHART_API_URL = "https://m.bugs.co.kr/api/getChartTrack"
 
 
@@ -34,14 +34,15 @@
         title: The title of the track
         artist: The name of the artist.
         image: The URL of the cover image for the track
         peakPos: The track's peak position on the chart.
         lastPos: The track's last position on the previous period.
         rank: The track's current rank position on the chart.
     """
+
     def __init__(self, title: str, artist: str, image: str, peakPos: int, lastPos: int, rank: int):
         self.title = title
         self.artist = artist
         self.image = image
         self.peakPos = peakPos
         self.lastPos = lastPos
         self.rank = rank
@@ -66,19 +67,21 @@
     def json(self):
         return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=4, ensure_ascii=False)
 
 
 class ChartData:
     """Represents a particular Bugs chart by a particular period.
     Attributes:
+        date: The chart date.
         chartType: The chart type.
         chartPeriod: The period for the chart.
         imageSize: The size of cover image for the track. (default: 256)
         fetch: A boolean value that indicates whether to retrieve the chart data immediately. If set to `False`, you can fetch the data later using the `fetchEntries()` method.
     """
+
     def __init__(self, chartType: BugsChartType = BugsChartType.All,
                  chartPeriod: BugsChartPeriod = BugsChartPeriod.Realtime, imageSize: int = 256,
                  fetch: bool = True):
         self.chartType = chartType
         self.chartPeriod = chartPeriod
         self.imageSize = imageSize
         self.entries = []
@@ -121,20 +124,25 @@
             message = f"Request is invalid. response message=${data.get('ret_msg')}"
             raise BugsChartRequestException(message)
 
         self._parseEntries(data)
 
     def _parseEntries(self, data):
         try:
+            self.date = self._parseDate(int(data['info']['end_dt']))
             list = data['list']
             for item in list:
                 entry = ChartEntry(
                     title=item['track_title'],
                     artist=item['artists'][0]['artist_nm'],
                     image=f"{_IMAGE_PREFIX_URL}/{self.imageSize}{item['album']['image']['path']}",
                     rank=int(item['list_attr']['rank']),
                     peakPos=int(item['list_attr']['rank_peak']),
                     lastPos=int(item['list_attr']['rank_last']),
                 )
                 self.entries.append(entry)
         except Exception as e:
             raise BugsChartParseException(e)
+
+    def _parseDate(self, timestamp_ms):
+        timestamp_s = timestamp_ms / 1000
+        return datetime.utcfromtimestamp(timestamp_s)
```

### Comparing `bugs-chart.py-1.0.3/bugs_chart.py.egg-info/PKG-INFO` & `bugs-chart.py-1.0.4/bugs_chart.py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bugs-chart.py
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python API for downloading Bugs charts
 Home-page: https://github.com/gold24park/bugs-chart.py
 Author: Lou Park
 Author-email: gold24park@gmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -29,17 +29,20 @@
     "artist": "IVE (아이브)",
     "image": "https://image.bugsm.co.kr/album/images/256/40849/4084947.jpg",
     "lastPos": 1,
     "peakPos": 1,
     "rank": 1,
     "title": "Kitsch"
 }
+>>> print(chart.date)
+2023-04-09 12:00:00
 ```
 
 ### ChartData Arguments
+- `date` – The chart date
 - `chartType`
   - BugsChartType.All – 전체
   - BugsChartType.Domestic – 국내
   - BugsChartType.International – 해외
 - `chartPeriod`
   - BugsChartPeriod.Realtime – 실시간
   - BugsChartPeriod.Daily – 일간
```

### Comparing `bugs-chart.py-1.0.3/setup.py` & `bugs-chart.py-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="bugs-chart.py",
-    version="1.0.3",
+    version="1.0.4",
     description="Python API for downloading Bugs charts",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Lou Park",
     author_email="gold24park@gmail.com",
     url="https://github.com/gold24park/bugs-chart.py",
     py_modules=["bugs"],
```

