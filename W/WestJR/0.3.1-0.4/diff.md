# Comparing `tmp/WestJR-0.3.1.tar.gz` & `tmp/WestJR-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WestJR-0.3.1.tar", last modified: Wed Aug  3 12:55:58 2022, max compression
+gzip compressed data, was "WestJR-0.4.tar", last modified: Sun Apr  9 08:51:50 2023, max compression
```

## Comparing `WestJR-0.3.1.tar` & `WestJR-0.4.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-08-03 12:55:58.377107 WestJR-0.3.1/
--rw-rw-rw-   0        0        0     1235 2022-06-05 08:26:55.000000 WestJR-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     3598 2022-08-03 12:55:58.377107 WestJR-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     2912 2022-08-03 12:48:01.000000 WestJR-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2022-08-03 12:55:58.366105 WestJR-0.3.1/WestJR.egg-info/
--rw-rw-rw-   0        0        0     3598 2022-08-03 12:55:58.000000 WestJR-0.3.1/WestJR.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2022-08-03 12:55:58.000000 WestJR-0.3.1/WestJR.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-03 12:55:58.000000 WestJR-0.3.1/WestJR.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      157 2022-08-03 12:55:58.000000 WestJR-0.3.1/WestJR.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-08-03 12:55:58.000000 WestJR-0.3.1/WestJR.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1311 2022-08-03 12:55:58.379107 WestJR-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0       83 2022-06-05 08:26:55.000000 WestJR-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-03 12:55:58.370106 WestJR-0.3.1/westjr/
--rw-rw-rw-   0        0        0       97 2022-08-03 12:54:19.000000 WestJR-0.3.1/westjr/__init__.py
--rw-rw-rw-   0        0        0     5855 2022-08-03 12:48:01.000000 WestJR-0.3.1/westjr/api.py
--rw-rw-rw-   0        0        0    27332 2022-06-05 08:26:55.000000 WestJR-0.3.1/westjr/const.py
--rw-rw-rw-   0        0        0        0 2022-06-05 08:26:55.000000 WestJR-0.3.1/westjr/py.typed
-drwxrwxrwx   0        0        0        0 2022-08-03 12:55:58.376105 WestJR-0.3.1/westjr/response_types/
--rw-rw-rw-   0        0        0      665 2022-08-03 12:48:01.000000 WestJR-0.3.1/westjr/response_types/__init__.py
--rw-rw-rw-   0        0        0     1139 2022-06-05 08:26:55.000000 WestJR-0.3.1/westjr/response_types/area_master.py
--rw-rw-rw-   0        0        0      909 2022-06-05 08:26:55.000000 WestJR-0.3.1/westjr/response_types/stations.py
--rw-rw-rw-   0        0        0      640 2022-06-05 08:26:55.000000 WestJR-0.3.1/westjr/response_types/train_info.py
--rw-rw-rw-   0        0        0      400 2022-08-03 12:48:01.000000 WestJR-0.3.1/westjr/response_types/train_monitor_info.py
--rw-rw-rw-   0        0        0      490 2022-06-05 08:26:55.000000 WestJR-0.3.1/westjr/response_types/train_pos.py
+drwxr-xr-x   0 y-endo     (501) staff       (20)        0 2023-04-09 08:51:50.084756 WestJR-0.4/
+-rw-r--r--   0 y-endo     (501) staff       (20)     1211 2023-04-09 08:51:21.000000 WestJR-0.4/LICENSE
+-rw-r--r--   0 y-endo     (501) staff       (20)     3924 2023-04-09 08:51:50.084845 WestJR-0.4/PKG-INFO
+-rw-r--r--   0 y-endo     (501) staff       (20)     3282 2023-04-09 08:51:21.000000 WestJR-0.4/README.md
+drwxr-xr-x   0 y-endo     (501) staff       (20)        0 2023-04-09 08:51:50.083112 WestJR-0.4/WestJR.egg-info/
+-rw-r--r--   0 y-endo     (501) staff       (20)     3924 2023-04-09 08:51:50.000000 WestJR-0.4/WestJR.egg-info/PKG-INFO
+-rw-r--r--   0 y-endo     (501) staff       (20)      534 2023-04-09 08:51:50.000000 WestJR-0.4/WestJR.egg-info/SOURCES.txt
+-rw-r--r--   0 y-endo     (501) staff       (20)        1 2023-04-09 08:51:50.000000 WestJR-0.4/WestJR.egg-info/dependency_links.txt
+-rw-r--r--   0 y-endo     (501) staff       (20)      174 2023-04-09 08:51:50.000000 WestJR-0.4/WestJR.egg-info/requires.txt
+-rw-r--r--   0 y-endo     (501) staff       (20)        7 2023-04-09 08:51:50.000000 WestJR-0.4/WestJR.egg-info/top_level.txt
+-rw-r--r--   0 y-endo     (501) staff       (20)     1286 2023-04-09 08:51:50.085271 WestJR-0.4/setup.cfg
+-rw-r--r--   0 y-endo     (501) staff       (20)       61 2023-04-09 08:51:21.000000 WestJR-0.4/setup.py
+drwxr-xr-x   0 y-endo     (501) staff       (20)        0 2023-04-09 08:51:50.083248 WestJR-0.4/tests/
+-rw-r--r--   0 y-endo     (501) staff       (20)     2284 2023-04-09 08:51:21.000000 WestJR-0.4/tests/test_example.py
+drwxr-xr-x   0 y-endo     (501) staff       (20)        0 2023-04-09 08:51:50.083816 WestJR-0.4/westjr/
+-rw-r--r--   0 y-endo     (501) staff       (20)       66 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/__init__.py
+-rw-r--r--   0 y-endo     (501) staff       (20)     5905 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/api.py
+-rw-r--r--   0 y-endo     (501) staff       (20)    26317 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/const.py
+-rw-r--r--   0 y-endo     (501) staff       (20)        0 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/py.typed
+drwxr-xr-x   0 y-endo     (501) staff       (20)        0 2023-04-09 08:51:50.084648 WestJR-0.4/westjr/response_types/
+-rw-r--r--   0 y-endo     (501) staff       (20)      620 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/response_types/__init__.py
+-rw-r--r--   0 y-endo     (501) staff       (20)      381 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/response_types/area_maintenance.py
+-rw-r--r--   0 y-endo     (501) staff       (20)     1003 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/response_types/area_master.py
+-rw-r--r--   0 y-endo     (501) staff       (20)      895 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/response_types/stations.py
+-rw-r--r--   0 y-endo     (501) staff       (20)      580 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/response_types/train_info.py
+-rw-r--r--   0 y-endo     (501) staff       (20)      364 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/response_types/train_monitor_info.py
+-rw-r--r--   0 y-endo     (501) staff       (20)      441 2023-04-09 08:51:21.000000 WestJR-0.4/westjr/response_types/train_pos.py
```

### Comparing `WestJR-0.3.1/LICENSE` & `WestJR-0.4/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-This is free and unencumbered software released into the public domain.
-
-Anyone is free to copy, modify, publish, use, compile, sell, or
-distribute this software, either in source code form or as a compiled
-binary, for any purpose, commercial or non-commercial, and by any
-means.
-
-In jurisdictions that recognize copyright laws, the author or authors
-of this software dedicate any and all copyright interest in the
-software to the public domain. We make this dedication for the benefit
-of the public at large and to the detriment of our heirs and
-successors. We intend this dedication to be an overt act of
-relinquishment in perpetuity of all present and future rights to this
-software under copyright law.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
-IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
-OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-OTHER DEALINGS IN THE SOFTWARE.
-
-For more information, please refer to <https://unlicense.org>
+This is free and unencumbered software released into the public domain.
+
+Anyone is free to copy, modify, publish, use, compile, sell, or
+distribute this software, either in source code form or as a compiled
+binary, for any purpose, commercial or non-commercial, and by any
+means.
+
+In jurisdictions that recognize copyright laws, the author or authors
+of this software dedicate any and all copyright interest in the
+software to the public domain. We make this dedication for the benefit
+of the public at large and to the detriment of our heirs and
+successors. We intend this dedication to be an overt act of
+relinquishment in perpetuity of all present and future rights to this
+software under copyright law.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
+OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+OTHER DEALINGS IN THE SOFTWARE.
+
+For more information, please refer to <https://unlicense.org>
```

### Comparing `WestJR-0.3.1/PKG-INFO` & `WestJR-0.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,137 +1,130 @@
-Metadata-Version: 2.1
-Name: WestJR
-Version: 0.3.1
-Summary: Handling of train operation information of JR West, a railroad company in Japan
-Home-page: https://github.com/unyacat/westjr
-Author: unyacat
-Author-email: admin@unyacat.net
-License: Unlicense
-Keywords: westjr
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# WestJR
-
-![Python Versions](https://img.shields.io/pypi/pyversions/WestJR.svg)
-![PyPI](https://badge.fury.io/py/WestJR.svg)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/unyacat/westjr/master.svg)](https://results.pre-commit.ci/latest/github/unyacat/westjr/master)
-![GitHubActions](https://github.com/unyacat/westjr/workflows/Test/badge.svg)
-
-JR西日本列車走行位置 非公式API Pythonライブラリ
-
-* 列車走行位置取得 (`/api/v3/{LINE}.json`)
-* 路線名取得 (`/api/v3/area_{AREA}_master.json`)
-* 駅一覧取得 (`/api/v3/{LINE}_st.json`)
-* 運行情報取得 (`/api/v3/area_{AREA}_trafficinfo.json`)
-* 列車環境取得 (`/api/v3/trainmonitorinfo.json`)
-* 列車走行位置駅名，列車停車種別の変換
-
-## Notice
-
-* 動作を完全には確認していません．
-
-## Installation
-
-```bash
-pip install WestJR
-```
-
-## Usage
-
-[Wiki](https://github.com/unyacat/westjr/wiki) に情報があります．
-
-```python
-import westjr
-jr = westjr.WestJR()
-
-# あらかじめ area や line をセットする
-jr = westjr.WestJR(line="kobesanyo", area="kinki")
-```
-
-### Example
-
-#### 列車走行位置取得
-
-```python
-print(jr.get_trains())
-# {'update': '2021-03-31T08:14:34.313Z', 'trains': [{'no': '798T', 'pos': '0414_0415', ...```
-```
-
-#### 駅一覧取得
-
-```python
-print(jr.get_stations())
-# {'stations': [{'info': {'name': '新大阪', 'code': '0415', 'stopTrains': [1, 2, 5], 'typeNotice': None, ...
-```
-
-#### 路線一覧取得
-
-```python
-print(jr.get_lines())
-# {'lines': {'ako': {'name': '赤穂線', 'range': '相生〜播州赤穂', 'st': ...
-```
-
-#### 運行情報取得
-
-```Python
-print(jr.get_traffic_info())
-# {'lines': {}, 'express': {}}
-```
-
-#### エリア名一覧表示
-
-```python
-print(jr.areas)
-# ['hokuriku', 'kinki', 'okayama', 'hiroshima', 'sanin']
-```
-
-#### 路線名一覧表示
-
-```python
-print(jr.lines)
-# ['hokuriku', 'kobesanyo', 'hokurikubiwako', 'kyoto', 'ako', 'kosei', 'kusatsu', 'nara', 'sagano', 'sanin1', 'sanin2', 'osakahigashi', 'takarazuka']
-```
-
-#### 列車環境取得
-
-```python
-print(jr.get_train_monitor_info()["trains"]["3489M"][0]["cars"][0]["congestion"])
-# 26(%)
-print(jr.get_train_monitor_info()["trains"]["3489M"][0]["cars"][0]["temp"])
-# 23(°C)
-```
-
-#### 駅に停車する種別を id から名称に変換する
-
-```python
-station = jr.get_stations(line="kyoto")["stations"][0]
-print(station["info"]["name"])
-print(jr.convert_stopTrains(station["info"]["stopTrains"]))
-# 山科
-# ['新快速', '快速', '特急']
-
-```
-
-#### 列車走行位置の場所を前駅と次駅の名前に変換する
-
-```python
-train = jr.get_trains(line="kobesanyo")["trains"]
-tr = train[0]
-prev, next = jr.convert_pos(train=tr)
-print(prev)
-# 塚本
-```
-
-## Contribution
-
-* develop ブランチにお願いします
-
-
+# WestJR
+
+![Python Versions](https://img.shields.io/pypi/pyversions/WestJR.svg)
+![PyPI](https://badge.fury.io/py/WestJR.svg)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/unyacat/westjr/master.svg)](https://results.pre-commit.ci/latest/github/unyacat/westjr/master)
+![GitHubActions](https://github.com/unyacat/westjr/workflows/Test/badge.svg)
+
+JR西日本列車走行位置 非公式API Pythonライブラリ
+
+* 列車走行位置取得 (`/api/v3/{LINE}.json`)
+* メンテナンス予定取得 (`/api/v3/area_{AREA}_maintenance.json`)
+* 路線名取得 (`/api/v3/area_{AREA}_master.json`)
+* 駅一覧取得 (`/api/v3/{LINE}_st.json`)
+* 運行情報取得 (`/api/v3/area_{AREA}_trafficinfo.json`)
+* 列車環境取得 (`/api/v3/trainmonitorinfo.json`)
+* 列車走行位置駅名，列車停車種別の変換
+
+## Notice
+
+* 動作を完全には確認していません．
+
+## Installation
+
+```bash
+pip install WestJR
+```
+
+## Usage
+
+[Wiki](https://github.com/unyacat/westjr/wiki) に情報があります．
+
+```python
+import westjr
+jr = westjr.WestJR()
+
+# あらかじめ area や line をセットする
+jr = westjr.WestJR(line="kobesanyo", area="kinki")
+```
+
+### Example
+
+#### 列車走行位置取得
+
+```python
+print(jr.get_trains())
+# TrainPos(update='2023-03-21T16:54:54.612Z', trains=[TrainsItem(no='502C', ...
+```
+
+#### メンテナンス予定取得
+
+```python
+print(jr.get_maintenance())
+# 平常時:
+# AreaMaintenance(status=0, notification=Notification(groupId=0, text='', duration=''), ...
+# 異常時:
+# AreaMaintenance(status=1, notification=Notification(groupId=2023012802, text='1月24日から1月31日を, ...
+```
+
+#### 路線一覧取得
+
+```python
+print(jr.get_lines())
+# AreaMaster(lines={'ako': Line(name='赤穂線', range='相生〜播州赤穂', relatelines=None, st='...
+```
+
+#### 駅一覧取得
+
+```python
+print(jr.get_stations())
+# Stations(stations=[StationsItem(info=Info(name='新大阪', code='0415', stopTrains=[1, 2, 5], typeNotice=None, ...
+```
+
+#### 運行情報取得
+
+```Python
+print(jr.get_traffic_info())
+# 平常時:
+# TrainInfo(lines={}, express={})
+# 異常時:
+# TrainInfo(lines={'bantan': Info_LineItem(...)}, express={'bantan': Info_ExpressItem(...)})
+```
+
+#### エリア名一覧表示
+
+```python
+print(jr.areas)
+# ['hokuriku', 'kinki', 'okayama', 'hiroshima', 'sanin']
+```
+
+#### 路線名一覧表示
+
+```python
+print(jr.lines)
+# ['hokuriku', 'kobesanyo', 'hokurikubiwako', 'kyoto', 'ako', 'kosei', 'kusatsu', 'nara', 'sagano', 'sanin1', 'sanin2', 'osakahigashi', 'takarazuka']
+```
+
+#### 列車環境取得
+
+```python
+print(jr.get_train_monitor_info().trains["3489M"][0].cars[0].congestion)
+# 26(%)
+print(jr.get_train_monitor_info().trains["3489M"][0].cars[0].temp)
+# 23(°C)
+```
+
+#### 駅に停車する種別を id から名称に変換する
+
+```python
+station = jr.get_stations(line="kyoto").stations[0]
+
+print(station.info.name)
+# 山科
+
+print(jr.convert_stopTrains(station.info.stopTrains))
+# ['新快速', '快速', '特急']
+```
+
+#### 列車走行位置の場所を前駅と次駅の名前に変換する
+
+```python
+train = jr.get_trains(line="kobesanyo").trains
+tr = train[0]
+prev, next = jr.convert_pos(train=tr)
+print(prev)
+# 塚本
+```
+
+## Contribution
+
+* develop ブランチにお願いします
```

