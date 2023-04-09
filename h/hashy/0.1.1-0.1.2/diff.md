# Comparing `tmp/hashy-0.1.1-py3-none-any.whl.zip` & `tmp/hashy-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,15 @@
-Zip file size: 6839 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat      417 b- defN 21-Nov-11 08:08 hashy/__init__.py
--rw-rw-rw-  2.0 fat      325 b- defN 21-Nov-11 08:26 hashy/__version__.py
--rw-rw-rw-  2.0 fat      511 b- defN 21-Nov-11 08:25 hashy/bytes.py
--rw-rw-rw-  2.0 fat     4035 b- defN 21-Mar-19 06:49 hashy/dls_hash.py
--rw-rw-rw-  2.0 fat      815 b- defN 21-Mar-19 02:56 hashy/file_hash.py
--rw-rw-rw-  2.0 fat     1233 b- defN 20-Aug-28 17:16 hashy/hashy.py
--rw-rw-rw-  2.0 fat        0 b- defN 21-Mar-26 05:00 hashy/py.typed
--rw-rw-rw-  2.0 fat      519 b- defN 21-Mar-19 06:46 hashy/string_hash.py
--rw-rw-rw-  2.0 fat     1088 b- defN 21-Nov-11 08:28 hashy-0.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1088 b- defN 21-Nov-11 08:28 hashy-0.1.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      888 b- defN 21-Nov-11 08:28 hashy-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 21-Nov-11 08:28 hashy-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 21-Nov-11 08:28 hashy-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1046 b- defN 21-Nov-11 08:28 hashy-0.1.1.dist-info/RECORD
-14 files, 12068 bytes uncompressed, 5121 bytes compressed:  57.6%
+Zip file size: 6382 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat      417 b- defN 23-Apr-09 03:01 hashy/__init__.py
+-rw-rw-rw-  2.0 fat      325 b- defN 23-Apr-09 03:08 hashy/__version__.py
+-rw-rw-rw-  2.0 fat      511 b- defN 23-Apr-09 03:01 hashy/bytes.py
+-rw-rw-rw-  2.0 fat     4104 b- defN 23-Apr-09 03:08 hashy/dls_hash.py
+-rw-rw-rw-  2.0 fat      815 b- defN 23-Apr-09 03:01 hashy/file_hash.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-09 03:01 hashy/py.typed
+-rw-rw-rw-  2.0 fat      519 b- defN 23-Apr-09 03:01 hashy/string_hash.py
+-rw-rw-rw-  2.0 fat     1088 b- defN 23-Apr-09 03:10 hashy-0.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1088 b- defN 23-Apr-09 03:10 hashy-0.1.2.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      954 b- defN 23-Apr-09 03:10 hashy-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-09 03:10 hashy-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-09 03:10 hashy-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      975 b- defN 23-Apr-09 03:10 hashy-0.1.2.dist-info/RECORD
+13 files, 10894 bytes uncompressed, 4768 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -9,35 +9,32 @@
 
 Filename: hashy/dls_hash.py
 Comment: 
 
 Filename: hashy/file_hash.py
 Comment: 
 
-Filename: hashy/hashy.py
-Comment: 
-
 Filename: hashy/py.typed
 Comment: 
 
 Filename: hashy/string_hash.py
 Comment: 
 
-Filename: hashy-0.1.1.dist-info/LICENSE
+Filename: hashy-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: hashy-0.1.1.dist-info/LICENSE.txt
+Filename: hashy-0.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: hashy-0.1.1.dist-info/METADATA
+Filename: hashy-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: hashy-0.1.1.dist-info/WHEEL
+Filename: hashy-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: hashy-0.1.1.dist-info/top_level.txt
+Filename: hashy-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: hashy-0.1.1.dist-info/RECORD
+Filename: hashy-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hashy/__version__.py

```diff
@@ -1,8 +1,8 @@
 __application_name__ = "hashy"
 __title__ = __application_name__
 __author__ = "abel"
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __author_email__ = "j@abel.co"
 __url__ = "https://github.com/jamesabel/hashy"
 __download_url__ = "https://github.com/jamesabel/hashy"
 __description__ = "simple hash library for string, file, dict, set and list"
```

## hashy/dls_hash.py

```diff
@@ -1,22 +1,21 @@
 import copy
-import collections
+from collections import OrderedDict
 from typing import Callable, Union, Any
 
 from hashy import get_string_md5, get_string_sha256, get_string_sha512
 
 
 import json
 
 from enum import Enum
 from decimal import Decimal
 
 
 def convert_serializable_special_cases(o) -> Union[str, int, float]:
-
     """
     Convert an object to a type that is fairly generally serializable (e.g. json serializable).
     This only handles the cases that need converting.  The json module handles all the rest.
     For JSON, with json.dump or json.dumps with argument default=convert_serializable.
     Example:
     json.dumps(my_animal, indent=4, default=_convert_serializable)
 
@@ -40,64 +39,64 @@
 
 
 def json_dumps(o: Any) -> str:
     separators = (",", ":")  # no whitespace
     return json.dumps(dls_sort(o), default=convert_serializable_special_cases, separators=separators)  # serialize the object (as json string)
 
 
-def dls_sort(orig: Union[dict, list, set]) -> Union[dict, list]:
+def dls_sort(orig: Union[dict, OrderedDict, list, set]) -> Union[dict, OrderedDict, list]:
     """
     Given a nested dictionary, set or list, return a sorted version.  Note that lists aren't sorted (they merely retain
     their original order).  Original data is unchanged.
     :param orig: original dict or list (may or may not be sorted)
     :return: sorted version of orig (note that we never return sets since they are unordered)
     """
     orig = copy.deepcopy(orig)
     if isinstance(orig, list):
         return [dls_sort(e) for e in orig]
     elif isinstance(orig, set):
         # have to sort sets to be consistent since they have no order
         return sorted(list(orig))
-    elif isinstance(orig, dict) or isinstance(orig, collections.OrderedDict):
-        sorted_dict = collections.OrderedDict()
+    elif isinstance(orig, dict) or isinstance(orig, OrderedDict):
+        sorted_dict = OrderedDict()
         for k in sorted(orig):
             sorted_dict[k] = dls_sort(orig[k])
         return sorted_dict
     return orig
 
 
-def _dls_hash(dls: Union[dict, list, set], string_hash_function: Callable) -> str:
+def _dls_hash(dls: Union[dict, OrderedDict, list, set], string_hash_function: Callable) -> str:
     """
     Given a possibly unordered nested dictionary, set or list, return a consistent hash of it.
     These hashes are specific to hashy (as opposed to the other hashy functions like string or file which will have a more conventional value).
     :param dls: dict or list
     :return: hash string corresponding to the dl input
     """
 
     return string_hash_function(json_dumps(dls))  # do a hash on the (consistent and repeatable) string
 
 
-def get_dls_md5(dl: Union[dict, list, set]) -> str:
+def get_dls_md5(dl: Union[dict, OrderedDict, list, set]) -> str:
     """
     Given a possibly unordered nested dictionary, set or list, return a consistent hash of it.
     :param dl: dist or list
     :return: md5 hash string corresponding to the dl input
     """
     return _dls_hash(dl, get_string_md5)
 
 
-def get_dls_sha256(dl: Union[dict, list, set]) -> str:
+def get_dls_sha256(dl: Union[dict, OrderedDict, list, set]) -> str:
     """
     Given a possibly unordered nested dictionary, set or list, return a consistent hash of it.
     :param dl: dist or list
     :return: sha256 hash string corresponding to the dl input
     """
     return _dls_hash(dl, get_string_sha256)
 
 
-def get_dls_sha512(dl: Union[dict, list, set]) -> str:
+def get_dls_sha512(dl: Union[dict, OrderedDict, list, set]) -> str:
     """
     Given a possibly unordered nested dictionary, set or list, return a consistent hash of it.
     :param dl: dist or list
     :return: sha512 hash string corresponding to the dl input
     """
     return _dls_hash(dl, get_string_sha512)
```

## Comparing `hashy-0.1.1.dist-info/LICENSE` & `hashy-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hashy-0.1.1.dist-info/LICENSE.txt` & `hashy-0.1.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

