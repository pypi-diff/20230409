# Comparing `tmp/pytip-0.1.0-py2.py3-none-any.whl.zip` & `tmp/pytip-0.1.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 10625 bytes, number of entries: 14
+Zip file size: 10643 bytes, number of entries: 14
 -rw-rw-r--  2.0 unx      606 b- defN 23-Apr-09 03:58 pytip/__init__.py
 -rw-rw-r--  2.0 unx      389 b- defN 23-Apr-09 02:24 pytip/tools/__init__.py
 -rw-rw-r--  2.0 unx     3268 b- defN 23-Apr-09 01:31 pytip/tools/item.py
 -rw-rw-r--  2.0 unx      854 b- defN 23-Apr-09 01:59 pytip/tools/plot.py
--rw-rw-r--  2.0 unx     1539 b- defN 23-Apr-02 06:28 pytip/tools/table.py
+-rw-rw-r--  2.0 unx     1597 b- defN 23-Apr-09 10:43 pytip/tools/table.py
 -rw-rw-r--  2.0 unx      423 b- defN 23-Apr-09 02:30 pytip/utils/__init__.py
 -rw-rw-r--  2.0 unx     3831 b- defN 23-Apr-09 05:24 pytip/utils/celery.py
 -rw-rw-r--  2.0 unx     2463 b- defN 23-Apr-02 07:57 pytip/utils/checker.py
 -rw-rw-r--  2.0 unx     1292 b- defN 23-Apr-09 01:24 pytip/utils/deco.py
 -rw-rw-r--  2.0 unx     2658 b- defN 23-Apr-09 03:49 pytip/utils/file.py
--rw-rw-r--  2.0 unx     1118 b- defN 23-Apr-09 05:31 pytip-0.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Apr-09 05:31 pytip-0.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 23-Apr-09 05:31 pytip-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1058 b- defN 23-Apr-09 05:31 pytip-0.1.0.dist-info/RECORD
-14 files, 19615 bytes uncompressed, 8895 bytes compressed:  54.7%
+-rw-rw-r--  2.0 unx     1118 b- defN 23-Apr-09 10:45 pytip-0.1.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Apr-09 10:45 pytip-0.1.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 23-Apr-09 10:45 pytip-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1058 b- defN 23-Apr-09 10:45 pytip-0.1.1.dist-info/RECORD
+14 files, 19673 bytes uncompressed, 8913 bytes compressed:  54.7%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: pytip/utils/deco.py
 Comment: 
 
 Filename: pytip/utils/file.py
 Comment: 
 
-Filename: pytip-0.1.0.dist-info/METADATA
+Filename: pytip-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pytip-0.1.0.dist-info/WHEEL
+Filename: pytip-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pytip-0.1.0.dist-info/top_level.txt
+Filename: pytip-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pytip-0.1.0.dist-info/RECORD
+Filename: pytip-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytip/tools/table.py

```diff
@@ -1,30 +1,31 @@
 import numpy
 import pandas
 
 
 def df_number_column(
-        df : pandas.DataFrame=None, 
-        columns : list=None, 
+        df          : pandas.DataFrame=None, 
+        columns     : list=None, 
         except_list : list=['-','','.'],
-        none_value : any=numpy.nan,
+        none_value  : any=numpy.nan,
     ):
 
     r"""DataFrame 데이터를, 숫자 데이터 int/float 으로 변경
     df (DataFrame)     : 작업할 DataFrame
     columns (list)     : 작업할 대상 Column list
     except_item (list) : NaN 으로 변환할 예외처리 값 `ex) '-', '' ...
     none_value (any)   : NaN 대신 입력할 데이터 값 default) Numpy.NaN"""
     
     # Removing thousand comma
     # Converting `int` or `float`
     # [ (조건 만족 시 출력값)  if 조건 else (조건 불만족 시 출력 값)  for i in data ]
     # isdigit() : `integer` 를 구분해서 True 출력하는 기본 메서드
 
-    lambda_to_number = lambda x: int(x.replace(',','')) \
+    lambda_to_number = lambda x: x \
+        if type(x) in [int, float] else int(x.replace(',','')) \
         if x.replace(',','').isdigit() else float(x.replace(',','')) \
         if x not in except_list + ['-','','.'] else none_value
 
     if len(columns) > 0:
         for column in columns:
             df[column]  = list(map(lambda_to_number, df[column].tolist()))
```

## Comparing `pytip-0.1.0.dist-info/METADATA` & `pytip-0.1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytip
-Version: 0.1.0
+Version: 0.1.1
 Summary: UNKNOWN
 Home-page: https://github.com/YongBeomKim/pytip
 Author: momukji lab
 Author-email: ybkim@momukji.com
 License: MIT
 Keywords: pytip
 Platform: UNKNOWN
```

## Comparing `pytip-0.1.0.dist-info/RECORD` & `pytip-0.1.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 pytip/__init__.py,sha256=YQGvcoSAR1GVhIIfdyk1GkaRZ2ds7SpV9W4OF7sXrxs,606
 pytip/tools/__init__.py,sha256=KKqbkgk5EkEh_2jwQdxUtXATP6peuk43t9zGBN0lQE8,389
 pytip/tools/item.py,sha256=JPF-meLFzP1iwam3jDqeQrPGGfY4fFFYd67jtIfX674,3268
 pytip/tools/plot.py,sha256=2pmcMkz5HZ5fD5A5OgPr1_Cs2nTZP1DMcuqSyiSMCZk,854
-pytip/tools/table.py,sha256=U0dA8GjdhO-sMZ0EyzsysSQTV8dgjs5y_d0eXAv_Np4,1539
+pytip/tools/table.py,sha256=ddAvODKP7SExPgeEBmeW4QCcZXkDi-aaM3saxqw6vDo,1597
 pytip/utils/__init__.py,sha256=ptGGMFwDewyV4fCaRR3BSwZIGAlug5Z_8xs-scpEDYk,423
 pytip/utils/celery.py,sha256=dEPGQtdQjixd6bL1vuCPkZjZA80-1l1yPSWnu4tpab0,3831
 pytip/utils/checker.py,sha256=dKi5FJhpCpxIakfdrnRMcdhjWsN_MfejuUhfk8Wq4jI,2463
 pytip/utils/deco.py,sha256=lGPcGmr0n_8uMi3dCoiHCUkfNzg5BJN3DReP2lTrIxA,1292
 pytip/utils/file.py,sha256=B8CSuXPFj61WBg9w4cm-g6cT-eIWQrmxSo_8Lwbj6VM,2658
-pytip-0.1.0.dist-info/METADATA,sha256=KRhY0DOoYu_fDqNmZvQl5S4YIvy5oSFawdrS1GEXtXM,1118
-pytip-0.1.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-pytip-0.1.0.dist-info/top_level.txt,sha256=jF2tKdrfqmRq7kr--QAKzT5DpQOqrfwdSBO9WrauNHE,6
-pytip-0.1.0.dist-info/RECORD,,
+pytip-0.1.1.dist-info/METADATA,sha256=YFx50433ncwr5rOa1NiJ6M9dqPhCTtFtDHFaJfbnLmQ,1118
+pytip-0.1.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+pytip-0.1.1.dist-info/top_level.txt,sha256=jF2tKdrfqmRq7kr--QAKzT5DpQOqrfwdSBO9WrauNHE,6
+pytip-0.1.1.dist-info/RECORD,,
```

