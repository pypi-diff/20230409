# Comparing `tmp/pytip-0.0.9-py2.py3-none-any.whl.zip` & `tmp/pytip-0.1.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,16 @@
-Zip file size: 8961 bytes, number of entries: 13
--rw-rw-r--  2.0 unx        0 b- defN 23-Apr-02 08:07 pytip/__init__.py
--rw-rw-r--  2.0 unx      373 b- defN 23-Apr-02 07:53 pytip/tools/__init__.py
--rw-rw-r--  2.0 unx     3142 b- defN 23-Apr-04 11:05 pytip/tools/item.py
--rw-rw-r--  2.0 unx      859 b- defN 23-Apr-02 06:21 pytip/tools/plot.py
+Zip file size: 10625 bytes, number of entries: 14
+-rw-rw-r--  2.0 unx      606 b- defN 23-Apr-09 03:58 pytip/__init__.py
+-rw-rw-r--  2.0 unx      389 b- defN 23-Apr-09 02:24 pytip/tools/__init__.py
+-rw-rw-r--  2.0 unx     3268 b- defN 23-Apr-09 01:31 pytip/tools/item.py
+-rw-rw-r--  2.0 unx      854 b- defN 23-Apr-09 01:59 pytip/tools/plot.py
 -rw-rw-r--  2.0 unx     1539 b- defN 23-Apr-02 06:28 pytip/tools/table.py
--rw-rw-r--  2.0 unx      407 b- defN 23-Apr-02 09:46 pytip/utils/__init__.py
+-rw-rw-r--  2.0 unx      423 b- defN 23-Apr-09 02:30 pytip/utils/__init__.py
+-rw-rw-r--  2.0 unx     3831 b- defN 23-Apr-09 05:24 pytip/utils/celery.py
 -rw-rw-r--  2.0 unx     2463 b- defN 23-Apr-02 07:57 pytip/utils/checker.py
--rw-rw-r--  2.0 unx     1293 b- defN 23-Apr-02 05:48 pytip/utils/deco.py
--rw-rw-r--  2.0 unx     2908 b- defN 23-Apr-08 04:38 pytip/utils/file.py
--rw-rw-r--  2.0 unx     1118 b- defN 23-Apr-08 04:46 pytip-0.0.9.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Apr-08 04:46 pytip-0.0.9.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 23-Apr-08 04:46 pytip-0.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      978 b- defN 23-Apr-08 04:46 pytip-0.0.9.dist-info/RECORD
-13 files, 15196 bytes uncompressed, 7349 bytes compressed:  51.6%
+-rw-rw-r--  2.0 unx     1292 b- defN 23-Apr-09 01:24 pytip/utils/deco.py
+-rw-rw-r--  2.0 unx     2658 b- defN 23-Apr-09 03:49 pytip/utils/file.py
+-rw-rw-r--  2.0 unx     1118 b- defN 23-Apr-09 05:31 pytip-0.1.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Apr-09 05:31 pytip-0.1.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 23-Apr-09 05:31 pytip-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1058 b- defN 23-Apr-09 05:31 pytip-0.1.0.dist-info/RECORD
+14 files, 19615 bytes uncompressed, 8895 bytes compressed:  54.7%
```

## zipnote {}

```diff
@@ -12,29 +12,32 @@
 
 Filename: pytip/tools/table.py
 Comment: 
 
 Filename: pytip/utils/__init__.py
 Comment: 
 
+Filename: pytip/utils/celery.py
+Comment: 
+
 Filename: pytip/utils/checker.py
 Comment: 
 
 Filename: pytip/utils/deco.py
 Comment: 
 
 Filename: pytip/utils/file.py
 Comment: 
 
-Filename: pytip-0.0.9.dist-info/METADATA
+Filename: pytip-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: pytip-0.0.9.dist-info/WHEEL
+Filename: pytip-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: pytip-0.0.9.dist-info/top_level.txt
+Filename: pytip-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pytip-0.0.9.dist-info/RECORD
+Filename: pytip-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytip/__init__.py

```diff
@@ -0,0 +1,38 @@
+00000000: 2320 6874 7470 733a 2f2f 7769 6b69 6469  # https://wikidi
+00000010: 6666 2e63 6f6d 2f75 7469 6c69 7479 2f74  ff.com/utility/t
+00000020: 6f6f 6c0a 2320 6075 7469 6c69 7479 6020  ool.# `utility` 
+00000030: 6973 2061 2070 726f 6772 616d 2064 6573  is a program des
+00000040: 6967 6e65 6420 746f 2070 6572 666f 726d  igned to perform
+00000050: 2061 2073 696e 676c 6520 6f72 2061 2073   a single or a s
+00000060: 6d61 6c6c 2072 616e 6765 206f 6620 7461  mall range of ta
+00000070: 736b 730a 2320 6074 6f6f 6c60 2069 7320  sks.# `tool` is 
+00000080: 4120 6d65 6368 616e 6963 616c 2064 6576  A mechanical dev
+00000090: 6963 6520 696e 7465 6e64 6564 2074 6f20  ice intended to 
+000000a0: 6d61 6b65 2061 2074 6173 6b20 6561 7369  make a task easi
+000000b0: 6572 2e0a 0a23 2075 7469 6c69 7479 203a  er...# utility :
+000000c0: 20eb 8f85 eba6 bdec a081 20ed 9484 eba1   ......... .....
+000000d0: 9cea b7b8 eb9e a80a 2320 746f 6f6c 7320  ........# tools 
+000000e0: 2020 3a20 ebb6 80ea b080 eca0 810a 0a66    : ...........f
+000000f0: 726f 6d20 2e75 7469 6c73 2e63 656c 6572  rom .utils.celer
+00000100: 7920 696d 706f 7274 2043 656c 6572 790a  y import Celery.
+00000110: 6672 6f6d 202e 7574 696c 732e 6368 6563  from .utils.chec
+00000120: 6b65 7220 696d 706f 7274 204d 6573 7361  ker import Messa
+00000130: 6765 2c20 6368 6563 6b5f 666f 6c64 6572  ge, check_folder
+00000140: 5f66 696c 652c 2063 6865 636b 5f69 700a  _file, check_ip.
+00000150: 6672 6f6d 202e 7574 696c 732e 6669 6c65  from .utils.file
+00000160: 2069 6d70 6f72 7420 6d75 6c74 6970 726f   import multipro
+00000170: 6365 7373 5f69 7465 6d73 2c20 6669 6c65  cess_items, file
+00000180: 5f64 6f77 6e6c 6f61 642c 2066 696c 655f  _download, file_
+00000190: 7069 636b 6c65 0a66 726f 6d20 2e75 7469  pickle.from .uti
+000001a0: 6c73 2e64 6563 6f20 696d 706f 7274 2077  ls.deco import w
+000001b0: 6562 5f72 6574 7269 6573 2c20 656c 6170  eb_retries, elap
+000001c0: 7365 645f 7469 6d65 0a0a 6672 6f6d 202e  sed_time..from .
+000001d0: 746f 6f6c 732e 6974 656d 2069 6d70 6f72  tools.item impor
+000001e0: 7420 6461 7465 5f74 6f5f 7374 7269 6e67  t date_to_string
+000001f0: 2c20 7374 7269 6e67 5f74 6f5f 6461 7465  , string_to_date
+00000200: 7469 6d65 2c20 6469 7669 6465 5f63 6875  time, divide_chu
+00000210: 6e6b 730a 6672 6f6d 202e 746f 6f6c 732e  nks.from .tools.
+00000220: 706c 6f74 2069 6d70 6f72 7420 706c 745f  plot import plt_
+00000230: 6b6f 0a66 726f 6d20 2e74 6f6f 6c73 2e74  ko.from .tools.t
+00000240: 6162 6c65 2069 6d70 6f72 7420 6466 5f6e  able import df_n
+00000250: 756d 6265 725f 636f 6c75 6d6e 0a0a       umber_column..
```

## pytip/tools/__init__.py

```diff
@@ -1,10 +1,10 @@
-# https://wikidiff.com/utility/tool
-# `utility` is a program designed to perform a single or a small range of tasks
-# `tool` is A mechanical device intended to make a task easier.
+# # https://wikidiff.com/utility/tool
+# # `utility` is a program designed to perform a single or a small range of tasks
+# # `tool` is A mechanical device intended to make a task easier.
 
-# utility : 독립적 프로그램
-# tools   : 부가적
-from .item import date_to_string, string_to_datetime, divide_chunks
-from .plot import matplot_plt
-from .table import df_number_column
+# # utility : 독립적 프로그램
+# # tools   : 부가적
+# from .item import date_to_string, string_to_datetime, divide_chunks
+# from .plot import matplot_plt
+# from .table import df_number_column
```

## pytip/tools/item.py

```diff
@@ -3,15 +3,17 @@
 import itertools
 
 
 REGEX_DATETIME = {
     '[\d]{4}-[\d]{2}-[\d]{2}.[A-Z]{2}[\d]{1,2}:[\d]{1,2}:[\d]{1,2}':
     '%Y-%m-%d.%p%I:%M:%S', # '2022-07-31.AM3:02:30'
     '[\d]{4}\.[\d]{2}\.[\d]{2}\.[A-Z]{2}[\d]{1,2}:[\d]{1,2}':
-    '%Y.%m.%d.%p%I:%M',    # '2022.07.31.AM3:02'
+    '%Y.%m.%d.%p%I:%M',    # '2022.07.31.AM3:02',
+    "^[0-9]{4}/[0-9]{1,2}/[0-9]{1,2} [0-9]{1,2}:[0-9]{1,2}:[0-9]{1,2}":
+    '%Y/%m/%d %H:%M:%S',    # '2023/03/28 10:40:00',
 }
 
 
 # Input params 전처리 작업용
 def date_to_string(
         date:any=None, 
         only_number:bool=False,
```

## pytip/tools/plot.py

```diff
@@ -1,13 +1,13 @@
 import matplotlib.pyplot as plt
 from matplotlib.font_manager import fontManager
 
 
 # matplotlib font & style
-def matplot_plt(
+def plt_ko(
         font_list:list=['D2Coding', 'NanumGothicCoding', 'NanumGothic'],
         index:int=-1,
         style='seaborn',
         dpi=150,
     ) -> plt:
 
     r"""matplotlib 에 적용 가능한 한글폰트 검색기
```

## pytip/utils/__init__.py

```diff
@@ -1,11 +1,11 @@
-# https://wikidiff.com/utility/tool
-# `utility` is a program designed to perform a single or a small range of tasks
-# `tool` is A mechanical device intended to make a task easier.
+# # https://wikidiff.com/utility/tool
+# # `utility` is a program designed to perform a single or a small range of tasks
+# # `tool` is A mechanical device intended to make a task easier.
 
-# utility : 독립적 프로그램
-# tools   : 부가적
+# # utility : 독립적 프로그램
+# # tools   : 부가적
 
-from .checker import check_folder_file, Message, check_ip
-from .deco import web_retries, elapsed_time
-from .file import multiprocess_items, pickle_data, download_file
+# from .checker import check_folder_file, Message, check_ip
+# from .deco import web_retries, elapsed_time
+# from .file import multiprocess_items, pickle_data, download_file
```

## pytip/utils/deco.py

```diff
@@ -39,8 +39,7 @@
                 # https://help.acmicpc.net/judge/rte/RecursionError
                 except Exception as e: # except gaierror as e:
                     print(termcolor.colored(e, 'red'))
                     time.sleep(0.8)
             return None
         return wrapper
     return decorator
-
```

## pytip/utils/file.py

```diff
@@ -5,83 +5,80 @@
 import requests
 import subprocess
 from tqdm import tqdm
 from urllib import request
 from multiprocessing import Pool
 
 
-# https://stackoverflow.com/questions/16694907/download-large-file-in-python-with-requests
-def download_file(
-        url:str=None, 
-        file_name:str=None,
-        folder:str=None, 
-        chunk_size:int=8192, 
-        overwite=False
-    ) -> str:
-    r"""웹사이트 파일 다운로드
-    url (str) : 다운로드 파일 url 주소
-    foler (str) : `./data` 파일 저장 경로
-    file_name (str) : 저장할 파일 이름
-    chunk_size (int) : encoded response set chunk_size parameter to None.
-    overwrite (bool) : download file overwrite"""
-
-    local_filename = None
-    if file_name is None:
-        file_name = url.split('/')[-1]
-    if folder is None:
-        local_filename = f"{file_name}"
-    else:
-        local_filename = f"{folder}/{file_name}"
-
-    if overwite == False:
-        if os.path.exists(local_filename):
-            print(f'{local_filename} is existed\n`overwrite` changes to `True`')
-            return local_filename
-
-    assert local_filename is not None, "file_path is not Set ..."
-    headers = {
-        "Referer":url,
-        "User-Agent":"Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:94.0) Gecko/20100101 Firefox/94.0",
-    }
-    with requests.get(url, headers=headers,stream=True) as r:
-        r.raise_for_status()
-        with open(local_filename, 'wb') as f:
-            for chunk in r.iter_content(chunk_size=chunk_size):
-                f.write(chunk)
-    print(f'{local_filename} downloading is done.')
-    return local_filename
-
-
 def multiprocess_items(funcion, items:int, worker:list, display=False):
     r"""list() 데이터를  function 에 multiprocessing 반복적용
     function : 반복적용할 함수
     items    : function 에 입력할 데이터"""
 
     with Pool(worker) as pool:
         if display:
             items = list(tqdm(pool.imap(funcion, items), total=len(items)))
         else:
             items = pool.map(funcion, items)
         return items
 
 
 # http://taewan.kim/tip/python_pickle/
-def pickle_data(file_path:str=None, option='w', data=None):
+def file_pickle(
+        file_path:str=None,
+        option='w', 
+        data=None
+    ):
     r"""파이썬 객체를 Pickle 로 저장하고 호출
     file (str) : 파일이름
     option (str) : w,r (Write / Read)
     data (any) : pickle 로 저장할 
     """
-    
+
     assert option in ['w', 'r'], f"`option` 은 `w`,`r` 하나를 입력하세요."
     option = {'w':'wb', 'r':'rb'}[option]
-    
+
     with open(file_path, option) as f:
         if option == 'wb':
             assert data is not None, f"{data} 값을 저장 할 수 없습니다."
             pickle.dump(data, f)
             print(f"{file_path} saving done.")
             return None
 
         elif option == 'rb':
             assert data is None, f"불러오는 경우, {data}는 필요 없습니다."
             return pickle.load(f)
+
+
+# https://stackoverflow.com/questions/16694907/download-large-file-in-python-with-requests
+def file_download(
+        url:str=None, 
+        file_path:str=None,
+        chunk_size:int=8192, 
+        overwite=False
+    ) -> str:
+
+    r"""웹사이트 파일 다운로드
+    url (str) : 다운로드 파일 url 주소
+    foler (str) : `./data` 파일 저장 경로
+    file_name (str) : 저장할 파일 이름
+    chunk_size (int) : encoded response set chunk_size parameter to None.
+    overwrite (bool) : download file overwrite"""
+
+    assert file_path is not None, "file_path is not Set ..."
+    if overwite == False:
+        if os.path.exists(file_path):
+            print(f'{file_path} is existed\n`overwrite` changes to `True`')
+            return file_path
+
+    headers = {
+        "Referer":url,
+        "User-Agent":"Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:94.0) Gecko/20100101 Firefox/94.0",
+    }
+    with requests.get(url, headers=headers,stream=True) as r:
+        r.raise_for_status()
+        with open(file_path, 'wb') as f:
+            for chunk in r.iter_content(chunk_size=chunk_size):
+                f.write(chunk)
+    print(f'{file_path} downloading is done.')
+    return file_path
+
```

## Comparing `pytip-0.0.9.dist-info/METADATA` & `pytip-0.1.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytip
-Version: 0.0.9
+Version: 0.1.0
 Summary: UNKNOWN
 Home-page: https://github.com/YongBeomKim/pytip
 Author: momukji lab
 Author-email: ybkim@momukji.com
 License: MIT
 Keywords: pytip
 Platform: UNKNOWN
```

