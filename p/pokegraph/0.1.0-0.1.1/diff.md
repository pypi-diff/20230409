# Comparing `tmp/pokegraph-0.1.0-py3-none-any.whl.zip` & `tmp/pokegraph-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 14913 bytes, number of entries: 11
+Zip file size: 14829 bytes, number of entries: 11
 -rw-r--r--  2.0 unx       97 b- defN 23-Apr-09 08:18 pokegraph/__init__.py
 -rw-r--r--  2.0 unx      299 b- defN 23-Apr-06 08:54 pokegraph/example.py
 -rw-r--r--  2.0 unx    12749 b- defN 23-Apr-09 08:19 pokegraph/module.py
 -rw-r--r--  2.0 unx    21277 b- defN 23-Apr-09 09:13 pokegraph/pokegraph.py
 -rw-r--r--  2.0 unx      509 b- defN 23-Apr-09 08:48 pokegraph/utils.py
--rw-r--r--  2.0 unx     1075 b- defN 23-Apr-09 09:27 pokegraph-0.1.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     5585 b- defN 23-Apr-09 09:27 pokegraph-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 09:27 pokegraph-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 23-Apr-09 09:27 pokegraph-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-09 09:27 pokegraph-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      880 b- defN 23-Apr-09 09:27 pokegraph-0.1.0.dist-info/RECORD
-11 files, 42628 bytes uncompressed, 13425 bytes compressed:  68.5%
+-rw-r--r--  2.0 unx     1075 b- defN 23-Apr-09 09:51 pokegraph-0.1.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     5519 b- defN 23-Apr-09 09:51 pokegraph-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 09:51 pokegraph-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 23-Apr-09 09:51 pokegraph-0.1.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-09 09:51 pokegraph-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      880 b- defN 23-Apr-09 09:51 pokegraph-0.1.1.dist-info/RECORD
+11 files, 42562 bytes uncompressed, 13341 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: pokegraph/pokegraph.py
 Comment: 
 
 Filename: pokegraph/utils.py
 Comment: 
 
-Filename: pokegraph-0.1.0.dist-info/LICENSE.txt
+Filename: pokegraph-0.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pokegraph-0.1.0.dist-info/METADATA
+Filename: pokegraph-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pokegraph-0.1.0.dist-info/WHEEL
+Filename: pokegraph-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pokegraph-0.1.0.dist-info/entry_points.txt
+Filename: pokegraph-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: pokegraph-0.1.0.dist-info/top_level.txt
+Filename: pokegraph-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pokegraph-0.1.0.dist-info/RECORD
+Filename: pokegraph-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pokegraph-0.1.0.dist-info/LICENSE.txt` & `pokegraph-0.1.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pokegraph-0.1.0.dist-info/METADATA` & `pokegraph-0.1.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokegraph
-Version: 0.1.0
+Version: 0.1.1
 Summary: A command-line tool that draws Pokémon base stats graphs in the terminal.
 Home-page: https://github.com/starchildluke/pokegraph
 Download-URL: https://pypi.python.org/pypi/pokegraph/
 Author: starchildluke
 Author-email: Luke Davis <luke@lukealexdavis.co.uk>
 License: MIT
 Keywords: python,CLI,CLI tool,graphs,shell,terminal,pokemon
@@ -64,24 +64,22 @@
 special-defense: ▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇ 50.00
 speed          : ▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇▇ 90.00
 ```
 
 Most results can be copied and pasted wherever you like, since they use standard block characters. However the color charts will not show, since they use terminal escape codes for color. A couple images to show color examples:
 
 ```
-pokegraph data/pikachu.csv --color {red,green,blue,yellow}
+pokegraph data/pikachu.csv --color yellow
 ```
 
-<img src="https://user-images.githubusercontent.com/45363/43405623-1a2cc4d4-93cf-11e8-8c96-b7134d8986a2.png" width="655" alt="Multi variable bar chart with colors" />
-
-```
+<img src="https://github.com/starchildluke/pokegraph/blob/main/pikachu-yellow-base-stats.jpg" alt="Bar chart in yellow" />
 
 ### Install
 
-Requires Python 3.7+, install from [PyPI project](https://pypi.org/project/termgraph/)
+Requires Python 3.7+, install from [PyPI project](https://pypi.org/project/pokegraph/)
 
 ```
 python3 -m pip install pokegraph
 ```
 
 Note: Be sure your PATH includes the pypi install directory, for me it is `~/.local/bin/`
```

## Comparing `pokegraph-0.1.0.dist-info/RECORD` & `pokegraph-0.1.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 pokegraph/__init__.py,sha256=L8Ik0HW60byVDZEvCeNtGCHqwlnJq55bhNO4a7Nm3rc,97
 pokegraph/example.py,sha256=54SO-C-LiSg16HsLDoWdIY_mWv5-YJmkekIqQjdroCk,299
 pokegraph/module.py,sha256=4EvQcDqCC6sYZMzm7lDez4fTXGg2oqknwMEklJRBixI,12749
 pokegraph/pokegraph.py,sha256=6yBHq75wcT7LJMJZhDlyXneo0Opfh0_lwSFqk_ggZmM,21277
 pokegraph/utils.py,sha256=n_6_8K8-f8KYg7Khygz_oAm2HuR8Yrc0xS35bhN5tBY,509
-pokegraph-0.1.0.dist-info/LICENSE.txt,sha256=hADM3OiPC8iInhR7pv43tDHpXpK9eATM_wVQ74SdjXM,1075
-pokegraph-0.1.0.dist-info/METADATA,sha256=ef5Nr6ua_a3FWZLp1BQXYwgXC6j6LUObqi_QUFfaoZA,5585
-pokegraph-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pokegraph-0.1.0.dist-info/entry_points.txt,sha256=73PpcbifuuEPo8rK5Bd-RPtbG7_7K6KLzYdVfCCbEAY,55
-pokegraph-0.1.0.dist-info/top_level.txt,sha256=5Q6XkIgc5CHbFVXpDAhYIRDs2u0U2RpvDdsB6RwCUus,10
-pokegraph-0.1.0.dist-info/RECORD,,
+pokegraph-0.1.1.dist-info/LICENSE.txt,sha256=hADM3OiPC8iInhR7pv43tDHpXpK9eATM_wVQ74SdjXM,1075
+pokegraph-0.1.1.dist-info/METADATA,sha256=c9SbE7qmmZxaLFv6JQiAhkhCF8OhRwH8zrhcOMqTQJE,5519
+pokegraph-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pokegraph-0.1.1.dist-info/entry_points.txt,sha256=73PpcbifuuEPo8rK5Bd-RPtbG7_7K6KLzYdVfCCbEAY,55
+pokegraph-0.1.1.dist-info/top_level.txt,sha256=5Q6XkIgc5CHbFVXpDAhYIRDs2u0U2RpvDdsB6RwCUus,10
+pokegraph-0.1.1.dist-info/RECORD,,
```

