# Comparing `tmp/bugs-chart.py-1.0.2.tar.gz` & `tmp/bugs-chart.py-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bugs-chart.py-1.0.2.tar", last modified: Sun Apr  9 05:11:59 2023, max compression
+gzip compressed data, was "bugs-chart.py-1.0.3.tar", last modified: Sun Apr  9 09:39:22 2023, max compression
```

## Comparing `bugs-chart.py-1.0.2.tar` & `bugs-chart.py-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jieunpark   (501) staff       (20)        0 2023-04-09 05:11:59.498734 bugs-chart.py-1.0.2/
--rw-r--r--   0 jieunpark   (501) staff       (20)     1074 2023-04-09 04:50:14.000000 bugs-chart.py-1.0.2/LICENSE
--rw-r--r--   0 jieunpark   (501) staff       (20)     1855 2023-04-09 05:11:59.498634 bugs-chart.py-1.0.2/PKG-INFO
--rw-r--r--   0 jieunpark   (501) staff       (20)     1561 2023-04-09 04:49:16.000000 bugs-chart.py-1.0.2/README.md
--rw-r--r--   0 jieunpark   (501) staff       (20)     4439 2023-04-09 04:58:38.000000 bugs-chart.py-1.0.2/bugs.py
-drwxr-xr-x   0 jieunpark   (501) staff       (20)        0 2023-04-09 05:11:59.498471 bugs-chart.py-1.0.2/bugs_chart.py.egg-info/
--rw-r--r--   0 jieunpark   (501) staff       (20)     1855 2023-04-09 05:11:59.000000 bugs-chart.py-1.0.2/bugs_chart.py.egg-info/PKG-INFO
--rw-r--r--   0 jieunpark   (501) staff       (20)      218 2023-04-09 05:11:59.000000 bugs-chart.py-1.0.2/bugs_chart.py.egg-info/SOURCES.txt
--rw-r--r--   0 jieunpark   (501) staff       (20)        1 2023-04-09 05:11:59.000000 bugs-chart.py-1.0.2/bugs_chart.py.egg-info/dependency_links.txt
--rw-r--r--   0 jieunpark   (501) staff       (20)       17 2023-04-09 05:11:59.000000 bugs-chart.py-1.0.2/bugs_chart.py.egg-info/requires.txt
--rw-r--r--   0 jieunpark   (501) staff       (20)        5 2023-04-09 05:11:59.000000 bugs-chart.py-1.0.2/bugs_chart.py.egg-info/top_level.txt
--rw-r--r--   0 jieunpark   (501) staff       (20)       38 2023-04-09 05:11:59.498770 bugs-chart.py-1.0.2/setup.cfg
--rw-r--r--   0 jieunpark   (501) staff       (20)      539 2023-04-09 05:10:37.000000 bugs-chart.py-1.0.2/setup.py
+drwxr-xr-x   0 jieunpark   (501) staff       (20)        0 2023-04-09 09:39:22.363717 bugs-chart.py-1.0.3/
+-rw-r--r--   0 jieunpark   (501) staff       (20)     1074 2023-04-09 04:50:14.000000 bugs-chart.py-1.0.3/LICENSE
+-rw-r--r--   0 jieunpark   (501) staff       (20)     2070 2023-04-09 09:39:22.363612 bugs-chart.py-1.0.3/PKG-INFO
+-rw-r--r--   0 jieunpark   (501) staff       (20)     1774 2023-04-09 09:39:14.000000 bugs-chart.py-1.0.3/README.md
+-rw-r--r--   0 jieunpark   (501) staff       (20)     4464 2023-04-09 09:35:50.000000 bugs-chart.py-1.0.3/bugs.py
+drwxr-xr-x   0 jieunpark   (501) staff       (20)        0 2023-04-09 09:39:22.363436 bugs-chart.py-1.0.3/bugs_chart.py.egg-info/
+-rw-r--r--   0 jieunpark   (501) staff       (20)     2070 2023-04-09 09:39:22.000000 bugs-chart.py-1.0.3/bugs_chart.py.egg-info/PKG-INFO
+-rw-r--r--   0 jieunpark   (501) staff       (20)      218 2023-04-09 09:39:22.000000 bugs-chart.py-1.0.3/bugs_chart.py.egg-info/SOURCES.txt
+-rw-r--r--   0 jieunpark   (501) staff       (20)        1 2023-04-09 09:39:22.000000 bugs-chart.py-1.0.3/bugs_chart.py.egg-info/dependency_links.txt
+-rw-r--r--   0 jieunpark   (501) staff       (20)       17 2023-04-09 09:39:22.000000 bugs-chart.py-1.0.3/bugs_chart.py.egg-info/requires.txt
+-rw-r--r--   0 jieunpark   (501) staff       (20)        5 2023-04-09 09:39:22.000000 bugs-chart.py-1.0.3/bugs_chart.py.egg-info/top_level.txt
+-rw-r--r--   0 jieunpark   (501) staff       (20)       38 2023-04-09 09:39:22.363756 bugs-chart.py-1.0.3/setup.cfg
+-rw-r--r--   0 jieunpark   (501) staff       (20)      542 2023-04-09 09:35:30.000000 bugs-chart.py-1.0.3/setup.py
```

### Comparing `bugs-chart.py-1.0.2/LICENSE` & `bugs-chart.py-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bugs-chart.py-1.0.2/PKG-INFO` & `bugs-chart.py-1.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 Metadata-Version: 2.1
 Name: bugs-chart.py
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python API for downloading Bugs charts
-Home-page: https://github.com/gold24park/bugs-chart
+Home-page: https://github.com/gold24park/bugs-chart.py
 Author: Lou Park
 Author-email: gold24park@gmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bugs-chart.py
-bugs-chart.py is a Python API that retrieves the TOP 100 information from the 'Bugs'.
+![bugs](./image.png)
+
+bugs-chart.py is a Python API that retrieves the TOP 100 information from the [Bugs](https://music.bugs.co.kr/).
 
 ## Installation
 ```commandline
 pip install bugs-chart.py
 ```
 
 ## Quickstart
-The main usage of bugs-chart.py is similar to [billboard.py](https://github.com/guoguo12/billboard-chart).
+The main usage of bugs-chart.py is similar to [billboard.py](https://github.com/guoguo12/billboard-charts).
 ```commandline
 >>> from bugs import *
->>> chart = ChartData(chart_type=BugsChartType.Domestic)
->>> print(chart[0])
-'Kitsch' by IVE (아이브)
+>>> chart = ChartData(chartType=BugsChartType.Domestic)
+>>> print(chart[0].json())
+{
+    "artist": "IVE (아이브)",
+    "image": "https://image.bugsm.co.kr/album/images/256/40849/4084947.jpg",
+    "lastPos": 1,
+    "peakPos": 1,
+    "rank": 1,
+    "title": "Kitsch"
+}
 ```
 
 ### ChartData Arguments
-- `chart_type`
+- `chartType`
   - BugsChartType.All – 전체
   - BugsChartType.Domestic – 국내
   - BugsChartType.International – 해외
-- `chart_preiod`
+- `chartPeriod`
   - BugsChartPeriod.Realtime – 실시간
   - BugsChartPeriod.Daily – 일간
   - BugsChartPeriod.Weekly – 주간
-- `image_size` – The size of cover image for the track. (default: 256)
+- `imageSize` – The size of cover image for the track. (default: 256)
 - `fetch` – A boolean value that indicates whether to retrieve the chart data immediately. If set to `False`, you can fetch the data later using the `fetchEntries()` method.
 
 ### Chart entry attributes
 `ChartEntry` can be accessed using the `ChartData[index]` syntax. A `ChartEntry` instance has the following attributes:
 - `title` – The title of the track
 - `artist` – The name of the artist
 - `image` – The URL of the cover image for the track
```

### Comparing `bugs-chart.py-1.0.2/bugs.py` & `bugs-chart.py-1.0.3/bugs.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,53 +60,53 @@
 
         if sys.version_info.major < 3:
             return s.encode(getattr(sys.stdout, "encoding", "") or "utf8")
         else:
             return s
 
     def json(self):
-        return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=4)
+        return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=4, ensure_ascii=False)
 
 
 class ChartData:
     """Represents a particular Bugs chart by a particular period.
     Attributes:
-        chart_type: The chart type.
-        chart_preiod: The period for the chart.
-        image_size: The size of cover image for the track. (default: 256)
+        chartType: The chart type.
+        chartPeriod: The period for the chart.
+        imageSize: The size of cover image for the track. (default: 256)
         fetch: A boolean value that indicates whether to retrieve the chart data immediately. If set to `False`, you can fetch the data later using the `fetchEntries()` method.
     """
-    def __init__(self, chart_type: BugsChartType = BugsChartType.All,
-                 chart_period: BugsChartPeriod = BugsChartPeriod.Realtime, image_size: int = 256,
+    def __init__(self, chartType: BugsChartType = BugsChartType.All,
+                 chartPeriod: BugsChartPeriod = BugsChartPeriod.Realtime, imageSize: int = 256,
                  fetch: bool = True):
-        self.chart_type = chart_type
-        self.chart_period = chart_period
-        self.image_size = image_size
+        self.chartType = chartType
+        self.chartPeriod = chartPeriod
+        self.imageSize = imageSize
         self.entries = []
 
         if fetch:
             self.fetchEntries()
 
     def __getitem__(self, key):
         return self.entries[key]
 
     def __len__(self):
         return len(self.entries)
 
     def json(self):
-        return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=4)
+        return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=4, ensure_ascii=False)
 
     def fetchEntries(self):
         headers = {
             "User-Agent": _USER_AGENT
         }
 
         data = {
-            "period_tp": self.chart_period,
-            "svc_type": self.chart_type,
+            "period_tp": self.chartPeriod,
+            "svc_type": self.chartType,
             "size": 100,
         }
 
         res = requests.post(
             _CHART_API_URL,
             headers=headers,
             data=data
@@ -126,15 +126,15 @@
     def _parseEntries(self, data):
         try:
             list = data['list']
             for item in list:
                 entry = ChartEntry(
                     title=item['track_title'],
                     artist=item['artists'][0]['artist_nm'],
-                    image=f"{_IMAGE_PREFIX_URL}/{self.image_size}{item['album']['image']['path']}",
+                    image=f"{_IMAGE_PREFIX_URL}/{self.imageSize}{item['album']['image']['path']}",
                     rank=int(item['list_attr']['rank']),
                     peakPos=int(item['list_attr']['rank_peak']),
                     lastPos=int(item['list_attr']['rank_last']),
                 )
                 self.entries.append(entry)
         except Exception as e:
             raise BugsChartParseException(e)
```

### Comparing `bugs-chart.py-1.0.2/bugs_chart.py.egg-info/PKG-INFO` & `bugs-chart.py-1.0.3/bugs_chart.py.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 Metadata-Version: 2.1
 Name: bugs-chart.py
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python API for downloading Bugs charts
-Home-page: https://github.com/gold24park/bugs-chart
+Home-page: https://github.com/gold24park/bugs-chart.py
 Author: Lou Park
 Author-email: gold24park@gmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bugs-chart.py
-bugs-chart.py is a Python API that retrieves the TOP 100 information from the 'Bugs'.
+![bugs](./image.png)
+
+bugs-chart.py is a Python API that retrieves the TOP 100 information from the [Bugs](https://music.bugs.co.kr/).
 
 ## Installation
 ```commandline
 pip install bugs-chart.py
 ```
 
 ## Quickstart
-The main usage of bugs-chart.py is similar to [billboard.py](https://github.com/guoguo12/billboard-chart).
+The main usage of bugs-chart.py is similar to [billboard.py](https://github.com/guoguo12/billboard-charts).
 ```commandline
 >>> from bugs import *
->>> chart = ChartData(chart_type=BugsChartType.Domestic)
->>> print(chart[0])
-'Kitsch' by IVE (아이브)
+>>> chart = ChartData(chartType=BugsChartType.Domestic)
+>>> print(chart[0].json())
+{
+    "artist": "IVE (아이브)",
+    "image": "https://image.bugsm.co.kr/album/images/256/40849/4084947.jpg",
+    "lastPos": 1,
+    "peakPos": 1,
+    "rank": 1,
+    "title": "Kitsch"
+}
 ```
 
 ### ChartData Arguments
-- `chart_type`
+- `chartType`
   - BugsChartType.All – 전체
   - BugsChartType.Domestic – 국내
   - BugsChartType.International – 해외
-- `chart_preiod`
+- `chartPeriod`
   - BugsChartPeriod.Realtime – 실시간
   - BugsChartPeriod.Daily – 일간
   - BugsChartPeriod.Weekly – 주간
-- `image_size` – The size of cover image for the track. (default: 256)
+- `imageSize` – The size of cover image for the track. (default: 256)
 - `fetch` – A boolean value that indicates whether to retrieve the chart data immediately. If set to `False`, you can fetch the data later using the `fetchEntries()` method.
 
 ### Chart entry attributes
 `ChartEntry` can be accessed using the `ChartData[index]` syntax. A `ChartEntry` instance has the following attributes:
 - `title` – The title of the track
 - `artist` – The name of the artist
 - `image` – The URL of the cover image for the track
```

### Comparing `bugs-chart.py-1.0.2/setup.py` & `bugs-chart.py-1.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="bugs-chart.py",
-    version="1.0.2",
+    version="1.0.3",
     description="Python API for downloading Bugs charts",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Lou Park",
     author_email="gold24park@gmail.com",
-    url="https://github.com/gold24park/bugs-chart",
+    url="https://github.com/gold24park/bugs-chart.py",
     py_modules=["bugs"],
     license="MIT License",
     install_requires=["requests >= 2.28.2"],
 )
```

