# Comparing `tmp/stockait-0.0.6-py3-none-any.whl.zip` & `tmp/stockait-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 14740 bytes, number of entries: 11
+Zip file size: 14723 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      128 b- defN 23-Apr-01 15:01 stockait/__init__.py
--rw-r--r--  2.0 unx     4446 b- defN 23-Apr-09 00:11 stockait/dataLoad.py
+-rw-r--r--  2.0 unx     4402 b- defN 23-Apr-09 00:44 stockait/dataLoad.py
 -rw-r--r--  2.0 unx    12051 b- defN 23-Apr-08 14:22 stockait/dataPreprocessing.py
 -rw-r--r--  2.0 unx     6006 b- defN 23-Apr-01 15:01 stockait/simulation.py
 -rw-r--r--  2.0 unx     4869 b- defN 23-Apr-01 15:01 stockait/trader.py
 -rw-r--r--  2.0 unx     9452 b- defN 23-Apr-02 01:59 stockait/training.py
--rw-r--r--  2.0 unx     1074 b- defN 23-Apr-09 00:13 stockait-0.0.6.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     5229 b- defN 23-Apr-09 00:13 stockait-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 00:13 stockait-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-09 00:13 stockait-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      864 b- defN 23-Apr-09 00:13 stockait-0.0.6.dist-info/RECORD
-11 files, 44220 bytes uncompressed, 13290 bytes compressed:  69.9%
+-rw-r--r--  2.0 unx     1074 b- defN 23-Apr-09 00:44 stockait-0.0.7.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     5229 b- defN 23-Apr-09 00:44 stockait-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-09 00:44 stockait-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-09 00:44 stockait-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      864 b- defN 23-Apr-09 00:44 stockait-0.0.7.dist-info/RECORD
+11 files, 44176 bytes uncompressed, 13273 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: stockait/trader.py
 Comment: 
 
 Filename: stockait/training.py
 Comment: 
 
-Filename: stockait-0.0.6.dist-info/LICENSE.md
+Filename: stockait-0.0.7.dist-info/LICENSE.md
 Comment: 
 
-Filename: stockait-0.0.6.dist-info/METADATA
+Filename: stockait-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: stockait-0.0.6.dist-info/WHEEL
+Filename: stockait-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: stockait-0.0.6.dist-info/top_level.txt
+Filename: stockait-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: stockait-0.0.6.dist-info/RECORD
+Filename: stockait-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stockait/dataLoad.py

```diff
@@ -3,16 +3,15 @@
 import warnings
 warnings.filterwarnings('ignore')
 from tqdm import tqdm
 import boto3
 import os
 import sqlalchemy 
 from sqlalchemy import create_engine
-from dotenv import load_dotenv
-load_dotenv()
+
 
 
 def get_countries(): 
     
     '''
     
     [ Explanation ]
```

## Comparing `stockait-0.0.6.dist-info/LICENSE.md` & `stockait-0.0.7.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `stockait-0.0.6.dist-info/METADATA` & `stockait-0.0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockait
-Version: 0.0.6
+Version: 0.0.7
 Summary: Make your stock investment smarter, join StockAit!
 Home-page: https://github.com/stockAI-py/stockait
 Author: Eunsu Kim, Sieun Kim, Eunji Cha, Yujin Cha
 Author-email: stockai2023@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `stockait-0.0.6.dist-info/RECORD` & `stockait-0.0.7.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 stockait/__init__.py,sha256=_a8leEVKkvtDF0-FwyVTF2Vyj0UUx81hy_7dFrBOqD8,128
-stockait/dataLoad.py,sha256=eYoR6kt3hHz3jdLZaVb-IC-FMZoi_ooJT7lQDzLSI8c,4446
+stockait/dataLoad.py,sha256=guclDcia5OaukINArfMynllgK3gSe45tzeo_pV8ENA4,4402
 stockait/dataPreprocessing.py,sha256=n_FPjr02yl6JzrpTg2peRUEAzg5KvBFNB9hQ_KL5G2g,12051
 stockait/simulation.py,sha256=YID0trWAYNN35eYf3eSNqUs5LZM1RUG4qkvLn1kQ6SA,6006
 stockait/trader.py,sha256=OuSow65YA_-vN3orhsMa5TXGYWdnqJmqs2V2C45SlQA,4869
 stockait/training.py,sha256=5BksvRlNDzv6GJx2OxbN9_qrUAOZ5XrMxDEuXQZ_A0A,9452
-stockait-0.0.6.dist-info/LICENSE.md,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
-stockait-0.0.6.dist-info/METADATA,sha256=wbRNgaedTZt1NEdx0W5XzflsdZrKgsr3dovCmF7I7dE,5229
-stockait-0.0.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-stockait-0.0.6.dist-info/top_level.txt,sha256=38J2n2dUfPQ7UZYE4dD-Hmyk8KmGSV00bDToFc7-bm4,9
-stockait-0.0.6.dist-info/RECORD,,
+stockait-0.0.7.dist-info/LICENSE.md,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
+stockait-0.0.7.dist-info/METADATA,sha256=3rikCWEDl2vPQcn54eolQWPzSLL_CIuP3jq9DvX_JK4,5229
+stockait-0.0.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+stockait-0.0.7.dist-info/top_level.txt,sha256=38J2n2dUfPQ7UZYE4dD-Hmyk8KmGSV00bDToFc7-bm4,9
+stockait-0.0.7.dist-info/RECORD,,
```

