# Comparing `tmp/test_yolo-0.0.10-py3-none-any.whl.zip` & `tmp/test_yolo-0.0.11-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 97929 bytes, number of entries: 29
--rw-r--r--  2.0 unx       54 b- defN 22-Sep-21 10:26 test_yolo/__init__.py
+-rw-r--r--  2.0 unx       49 b- defN 23-Apr-09 08:12 test_yolo/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Sep-21 10:25 test_yolo/detect.py
 -rw-r--r--  2.0 unx      238 b- defN 22-Sep-21 10:16 test_yolo/load_utils.py
 -rw-r--r--  2.0 unx    14484 b- defN 22-Sep-21 10:57 test_yolo/model_utils.py
 -rw-r--r--  2.0 unx        6 b- defN 22-Aug-18 08:56 test_yolo/models/__init__.py
 -rw-r--r--  2.0 unx    84459 b- defN 22-Aug-18 09:19 test_yolo/models/common.py
 -rw-r--r--  2.0 unx    10290 b- defN 22-Aug-18 09:15 test_yolo/models/experimental.py
 -rw-r--r--  2.0 unx    40083 b- defN 22-Sep-21 11:00 test_yolo/models/yolo.py
@@ -19,13 +19,13 @@
 -rw-r--r--  2.0 unx    20944 b- defN 22-Aug-18 09:02 test_yolo/utils/plots.py
 -rw-r--r--  2.0 unx    15467 b- defN 22-Aug-22 11:37 test_yolo/utils/torch_utils.py
 -rw-r--r--  2.0 unx        5 b- defN 22-Aug-18 08:56 test_yolo/utils/aws/__init__.py
 -rw-r--r--  2.0 unx     1112 b- defN 22-Aug-18 09:13 test_yolo/utils/aws/resume.py
 -rw-r--r--  2.0 unx        6 b- defN 22-Aug-18 08:56 test_yolo/utils/wandb_logging/__init__.py
 -rw-r--r--  2.0 unx      815 b- defN 22-Aug-18 08:56 test_yolo/utils/wandb_logging/log_dataset.py
 -rw-r--r--  2.0 unx    16265 b- defN 22-Aug-18 08:56 test_yolo/utils/wandb_logging/wandb_utils.py
--rw-rw-r--  2.0 unx     1062 b- defN 23-Apr-09 08:05 test_yolo-0.0.10.dist-info/LICENSE
--rw-r--r--  2.0 unx     3269 b- defN 23-Apr-09 08:05 test_yolo-0.0.10.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 08:05 test_yolo-0.0.10.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-09 08:05 test_yolo-0.0.10.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2446 b- defN 23-Apr-09 08:05 test_yolo-0.0.10.dist-info/RECORD
-29 files, 406438 bytes uncompressed, 93985 bytes compressed:  76.9%
+-rw-rw-r--  2.0 unx     1062 b- defN 23-Apr-09 08:13 test_yolo-0.0.11.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3269 b- defN 23-Apr-09 08:13 test_yolo-0.0.11.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 08:13 test_yolo-0.0.11.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-09 08:13 test_yolo-0.0.11.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2446 b- defN 23-Apr-09 08:13 test_yolo-0.0.11.dist-info/RECORD
+29 files, 406433 bytes uncompressed, 93985 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -66,23 +66,23 @@
 
 Filename: test_yolo/utils/wandb_logging/log_dataset.py
 Comment: 
 
 Filename: test_yolo/utils/wandb_logging/wandb_utils.py
 Comment: 
 
-Filename: test_yolo-0.0.10.dist-info/LICENSE
+Filename: test_yolo-0.0.11.dist-info/LICENSE
 Comment: 
 
-Filename: test_yolo-0.0.10.dist-info/METADATA
+Filename: test_yolo-0.0.11.dist-info/METADATA
 Comment: 
 
-Filename: test_yolo-0.0.10.dist-info/WHEEL
+Filename: test_yolo-0.0.11.dist-info/WHEEL
 Comment: 
 
-Filename: test_yolo-0.0.10.dist-info/top_level.txt
+Filename: test_yolo-0.0.11.dist-info/top_level.txt
 Comment: 
 
-Filename: test_yolo-0.0.10.dist-info/RECORD
+Filename: test_yolo-0.0.11.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## test_yolo/__init__.py

```diff
@@ -1 +1 @@
-from yolov7_package.model_utils import Yolov7Detector
+from test_yolo.model_utils import Yolov7Detector
```

## Comparing `test_yolo-0.0.10.dist-info/LICENSE` & `test_yolo-0.0.11.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `test_yolo-0.0.10.dist-info/METADATA` & `test_yolo-0.0.11.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-yolo
-Version: 0.0.10
+Version: 0.0.11
 Summary: Bindings for yolov7 in one class
 Home-page: https://github.com/maxwolf8852/yolov7_package.git
 Author: Maxim Volkovskiy
 Author-email: maxwolf8852@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `test_yolo-0.0.10.dist-info/RECORD` & `test_yolo-0.0.11.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-test_yolo/__init__.py,sha256=9DPNaujN0OzQYzSPMEeStjMzDLPvoPAyNFCTvakwFBM,54
+test_yolo/__init__.py,sha256=IEX5qbCfSfH2qSfsOo33dG48pUc2PmDE_66xWnlqeCA,49
 test_yolo/detect.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test_yolo/load_utils.py,sha256=nmulu5GjXnYMcRpwr-PoQp1MU7EvE1h9rur70BxQW7Y,238
 test_yolo/model_utils.py,sha256=qgejYk3ucGQboqJEdEdFPv7APDLnEptPvRm22sVeBLE,14484
 test_yolo/models/__init__.py,sha256=BIYCj6TRzGWCEbYG5ZNaTHQ4am6c9QVbgS80hLG0blc,6
 test_yolo/models/common.py,sha256=cTtVefnJfbQihKbJ0vi_pDkrZ9Q2M87dtu9L3LXsb8U,84459
 test_yolo/models/experimental.py,sha256=cDY_rb1kLSWyGfQ3Biwsk-bQMnw9gAFqMztQZ5Zvbv0,10290
 test_yolo/models/yolo.py,sha256=eHxSL6srTCvO-76N6hE13bUIhWYamWxjOuUW3W7cwcE,40083
@@ -18,12 +18,12 @@
 test_yolo/utils/plots.py,sha256=Czpuq4HYIZztIzSRNpusuXrnAHyq_VE_TybjuLybrL4,20944
 test_yolo/utils/torch_utils.py,sha256=7r4uhQSYmEChWUrNENskL0_ujH-DbEoFQEgoL32eqWw,15467
 test_yolo/utils/aws/__init__.py,sha256=GAMHpH0PAwUCxr_GSctfv1fxgkqvy9mpU1FBafhJmkk,5
 test_yolo/utils/aws/resume.py,sha256=B0GvCUzMxCA0uKWZwfyFxAbr6Rss5FG9ETf5yOh8Wuc,1112
 test_yolo/utils/wandb_logging/__init__.py,sha256=BIYCj6TRzGWCEbYG5ZNaTHQ4am6c9QVbgS80hLG0blc,6
 test_yolo/utils/wandb_logging/log_dataset.py,sha256=5LydLM7wFuLKrzW7UTgUovK-OuWHCwRIoWoKMKHbSag,815
 test_yolo/utils/wandb_logging/wandb_utils.py,sha256=aJLCp542HTWk6yXygizIkCSeTobYoK2ajQ6cce5OFqI,16265
-test_yolo-0.0.10.dist-info/LICENSE,sha256=IlU2zzPZa0Z3DTTluArAr-vnftTkdKuJR4Uo-lFV9E4,1062
-test_yolo-0.0.10.dist-info/METADATA,sha256=c73U-vb-YnguZd8JeIP--ELY-NiWA41QU-qj8xEsDDE,3269
-test_yolo-0.0.10.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-test_yolo-0.0.10.dist-info/top_level.txt,sha256=6yZONYUtmu1g7R6EL_f6zTsMjXlWvwiZ0qipI9nhaAg,10
-test_yolo-0.0.10.dist-info/RECORD,,
+test_yolo-0.0.11.dist-info/LICENSE,sha256=IlU2zzPZa0Z3DTTluArAr-vnftTkdKuJR4Uo-lFV9E4,1062
+test_yolo-0.0.11.dist-info/METADATA,sha256=8PdXvjexQteBpzqiOFE7x_GH0Bpi1x9IXwnTh17bS0E,3269
+test_yolo-0.0.11.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+test_yolo-0.0.11.dist-info/top_level.txt,sha256=6yZONYUtmu1g7R6EL_f6zTsMjXlWvwiZ0qipI9nhaAg,10
+test_yolo-0.0.11.dist-info/RECORD,,
```

