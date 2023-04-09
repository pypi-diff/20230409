# Comparing `tmp/pyCryptomusAPI-0.0.2.tar.gz` & `tmp/pyCryptomusAPI-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyCryptomusAPI-0.0.2.tar", last modified: Mon Jan 30 19:29:50 2023, max compression
+gzip compressed data, was "pyCryptomusAPI-0.0.3.tar", last modified: Sun Apr  9 09:10:02 2023, max compression
```

## Comparing `pyCryptomusAPI-0.0.2.tar` & `pyCryptomusAPI-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-01-30 19:29:50.809697 pyCryptomusAPI-0.0.2/
--rw-rw-rw-   0        0        0     1085 2022-12-10 18:10:42.000000 pyCryptomusAPI-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2174 2023-01-30 19:29:50.808697 pyCryptomusAPI-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1672 2022-12-12 17:35:04.000000 pyCryptomusAPI-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-01-30 19:29:50.800700 pyCryptomusAPI-0.0.2/pyCryptomusAPI/
--rw-rw-rw-   0        0        0       20 2022-12-10 22:13:53.000000 pyCryptomusAPI-0.0.2/pyCryptomusAPI/__init__.py
--rw-rw-rw-   0        0        0    16776 2023-01-29 22:56:30.000000 pyCryptomusAPI-0.0.2/pyCryptomusAPI/api.py
--rw-rw-rw-   0        0        0     9897 2023-01-21 14:08:46.000000 pyCryptomusAPI-0.0.2/pyCryptomusAPI/cryto_types.py
--rw-rw-rw-   0        0        0      374 2022-12-10 21:59:32.000000 pyCryptomusAPI-0.0.2/pyCryptomusAPI/private_keys.py
--rw-rw-rw-   0        0        0     2314 2023-01-29 22:51:47.000000 pyCryptomusAPI-0.0.2/pyCryptomusAPI/tests.py
--rw-rw-rw-   0        0        0       95 2023-01-21 14:18:45.000000 pyCryptomusAPI-0.0.2/pyCryptomusAPI/version.py
-drwxrwxrwx   0        0        0        0 2023-01-30 19:29:50.807697 pyCryptomusAPI-0.0.2/pyCryptomusAPI.egg-info/
--rw-rw-rw-   0        0        0     2174 2023-01-30 19:29:50.000000 pyCryptomusAPI-0.0.2/pyCryptomusAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-01-30 19:29:50.000000 pyCryptomusAPI-0.0.2/pyCryptomusAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-30 19:29:50.000000 pyCryptomusAPI-0.0.2/pyCryptomusAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-01-30 19:29:50.000000 pyCryptomusAPI-0.0.2/pyCryptomusAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-30 19:29:50.809697 pyCryptomusAPI-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1053 2022-12-10 18:13:01.000000 pyCryptomusAPI-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 09:10:02.958784 pyCryptomusAPI-0.0.3/
+-rw-rw-rw-   0        0        0     1085 2022-12-10 18:10:42.000000 pyCryptomusAPI-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2174 2023-04-09 09:10:02.958784 pyCryptomusAPI-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1672 2022-12-12 17:35:04.000000 pyCryptomusAPI-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 09:10:02.958784 pyCryptomusAPI-0.0.3/pyCryptomusAPI/
+-rw-rw-rw-   0        0        0       20 2022-12-10 22:13:53.000000 pyCryptomusAPI-0.0.3/pyCryptomusAPI/__init__.py
+-rw-rw-rw-   0        0        0    17058 2023-04-09 09:06:52.000000 pyCryptomusAPI-0.0.3/pyCryptomusAPI/api.py
+-rw-rw-rw-   0        0        0     9897 2023-01-21 14:08:46.000000 pyCryptomusAPI-0.0.3/pyCryptomusAPI/cryto_types.py
+-rw-rw-rw-   0        0        0      374 2023-02-14 14:49:00.000000 pyCryptomusAPI-0.0.3/pyCryptomusAPI/private_keys.py
+-rw-rw-rw-   0        0        0     2314 2023-02-14 14:48:55.000000 pyCryptomusAPI-0.0.3/pyCryptomusAPI/tests.py
+-rw-rw-rw-   0        0        0       95 2023-04-09 09:05:01.000000 pyCryptomusAPI-0.0.3/pyCryptomusAPI/version.py
+drwxrwxrwx   0        0        0        0 2023-04-09 09:10:02.958784 pyCryptomusAPI-0.0.3/pyCryptomusAPI.egg-info/
+-rw-rw-rw-   0        0        0     2174 2023-04-09 09:10:02.000000 pyCryptomusAPI-0.0.3/pyCryptomusAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-04-09 09:10:02.000000 pyCryptomusAPI-0.0.3/pyCryptomusAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 09:10:02.000000 pyCryptomusAPI-0.0.3/pyCryptomusAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-09 09:10:02.000000 pyCryptomusAPI-0.0.3/pyCryptomusAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 09:10:02.958784 pyCryptomusAPI-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1053 2022-12-10 18:13:01.000000 pyCryptomusAPI-0.0.3/setup.py
```

### Comparing `pyCryptomusAPI-0.0.2/LICENSE` & `pyCryptomusAPI-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyCryptomusAPI-0.0.2/PKG-INFO` & `pyCryptomusAPI-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCryptomusAPI
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python implementation of Cryptomus (https://cryptomus.com) pubilc API
 Home-page: https://github.com/Badiboy/pyCryptomusAPI
 Author: Badiboy
 License: MIT license
 Keywords: Crypto Pay API Cryptomus
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyCryptomusAPI-0.0.2/README.md` & `pyCryptomusAPI-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyCryptomusAPI-0.0.2/pyCryptomusAPI/api.py` & `pyCryptomusAPI-0.0.3/pyCryptomusAPI/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from hashlib import md5
+from time import sleep
 import base64
 import requests
 
 from .cryto_types import *
 
 API_URL = "https://api.cryptomus.com/v1/"
 
@@ -301,15 +302,15 @@
         else:
             resp = self.__request(method, 1).get("result")
         return PaymentsHistory.de_json(resp)
 
     def payment_history_filtered(
             self, max_results = 15, max_pages = 10,
             currencies = None, networks = None, addresses = None,
-            statuses = None, is_final = None):
+            statuses = None, is_final = None, page_delay = 1):
         """
         Payment history (advanced mode)
 
         Based on: payment_history
         https://doc.cryptomus.com/payments/payment-history
         Requires PAYMENT API key
 
@@ -319,21 +320,23 @@
         max_results: (Int) Max number of results to collect
         max_pages: (Int, Optional, default=10) Max number of pages to process
         currencies: (List of Strings, Optional) List of accepted currencies. Codes: https://doc.cryptomus.com/reference
         networks: (List of Strings, Optional) List of accepted networks. Codes: https://doc.cryptomus.com/reference
         addresses: (List of Strings, Optional) List of accepted addresses
         statuses: (List of Strings, Optional) List of accepted statuses. Codes: https://doc.cryptomus.com/payments/payment-statuses
         is_final: (Bool, Optional) If True, only final payments will be collected, if False - only non-final
+        page_delay: (Int, Optional, default=1) Delay between pages (in seconds)
         """
 
         result = PaymentsHistory()
 
         page_number = 0
         cursor = None
         while page_number < max_pages:
+            if page_number > 0: sleep(1)
             resp = self.payment_history(cursor = cursor)
 
             if not resp.items:
                 # No (more) payments
                 break
 
             for payment in resp.items:
@@ -349,14 +352,18 @@
                     continue
                 result.items.append(payment)
 
                 if len(result.items) >= max_results:
                     # Enough results collected
                     break
 
+            if len(result.items) >= max_results:
+                # Enough results collected
+                break
+
             cursor = resp.paginate.nextCursor
             if not cursor:
                 # No more pages
                 break
             page_number += 1
 
         return result
```

### Comparing `pyCryptomusAPI-0.0.2/pyCryptomusAPI/cryto_types.py` & `pyCryptomusAPI-0.0.3/pyCryptomusAPI/cryto_types.py`

 * *Files identical despite different names*

### Comparing `pyCryptomusAPI-0.0.2/pyCryptomusAPI/tests.py` & `pyCryptomusAPI-0.0.3/pyCryptomusAPI/tests.py`

 * *Files identical despite different names*

### Comparing `pyCryptomusAPI-0.0.2/pyCryptomusAPI.egg-info/PKG-INFO` & `pyCryptomusAPI-0.0.3/pyCryptomusAPI.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCryptomusAPI
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python implementation of Cryptomus (https://cryptomus.com) pubilc API
 Home-page: https://github.com/Badiboy/pyCryptomusAPI
 Author: Badiboy
 License: MIT license
 Keywords: Crypto Pay API Cryptomus
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyCryptomusAPI-0.0.2/setup.py` & `pyCryptomusAPI-0.0.3/setup.py`

 * *Files identical despite different names*

