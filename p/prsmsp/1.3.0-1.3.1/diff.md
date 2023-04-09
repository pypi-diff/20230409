# Comparing `tmp/prsmsp-1.3.0.tar.gz` & `tmp/prsmsp-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prsmsp-1.3.0.tar", last modified: Sun Apr  9 15:57:09 2023, max compression
+gzip compressed data, was "prsmsp-1.3.1.tar", last modified: Sun Apr  9 21:55:41 2023, max compression
```

## Comparing `prsmsp-1.3.0.tar` & `prsmsp-1.3.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:57:09.349088 prsmsp-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-09 15:57:09.349088 prsmsp-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-09 15:56:59.000000 prsmsp-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:57:09.345088 prsmsp-1.3.0/prsmsp/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:57:09.345088 prsmsp-1.3.0/prsmsp/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/abstracts/abcpanel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:57:09.345088 prsmsp-1.3.0/prsmsp/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/exceptions/abstracts.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/exceptions/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/exceptions/panels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:57:09.349088 prsmsp-1.3.0/prsmsp/factories/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/factories/auth_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:57:09.349088 prsmsp-1.3.0/prsmsp/models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/models/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/models/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:57:09.349088 prsmsp-1.3.0/prsmsp/panels/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/panels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/panels/farazsms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/panels/ghasedaksms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/panels/kavenegar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/panels/mediana.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/panels/melipayamak.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/panels/smsdotir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/panels/webonesms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:57:09.345088 prsmsp-1.3.0/prsmsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-09 15:57:09.000000 prsmsp-1.3.0/prsmsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-09 15:57:09.000000 prsmsp-1.3.0/prsmsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 15:57:09.000000 prsmsp-1.3.0/prsmsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 15:57:09.000000 prsmsp-1.3.0/prsmsp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-09 15:57:09.000000 prsmsp-1.3.0/prsmsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-09 15:57:09.000000 prsmsp-1.3.0/prsmsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-09 15:57:09.349088 prsmsp-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-09 15:56:59.000000 prsmsp-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:57:09.349088 prsmsp-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:56:59.000000 prsmsp-1.3.0/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:55:41.806903 prsmsp-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-09 21:55:41.806903 prsmsp-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-09 21:55:30.000000 prsmsp-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:55:41.798903 prsmsp-1.3.1/prsmsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-09 21:55:30.000000 prsmsp-1.3.1/prsmsp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:55:41.802903 prsmsp-1.3.1/prsmsp/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-09 21:55:30.000000 prsmsp-1.3.1/prsmsp/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-09 21:55:30.000000 prsmsp-1.3.1/prsmsp/abstracts/abcpanel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:55:41.802903 prsmsp-1.3.1/prsmsp/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:55:30.000000 prsmsp-1.3.1/prsmsp/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:55:30.000000 prsmsp-1.3.1/prsmsp/exceptions/abstracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-09 21:55:30.000000 prsmsp-1.3.1/prsmsp/exceptions/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:55:30.000000 prsmsp-1.3.1/prsmsp/exceptions/panels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:55:41.802903 prsmsp-1.3.1/prsmsp/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-09 21:55:30.000000 prsmsp-1.3.1/prsmsp/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-09 21:55:30.000000 prsmsp-1.3.1/prsmsp/factories/auth_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:55:41.802903 prsmsp-1.3.1/prsmsp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-09 21:55:30.000000 prsmsp-1.3.1/prsmsp/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-09 21:55:30.000000 prsmsp-1.3.1/prsmsp/models/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-09 21:55:30.000000 prsmsp-1.3.1/prsmsp/models/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:55:41.806903 prsmsp-1.3.1/prsmsp/panels/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-09 21:55:30.000000 prsmsp-1.3.1/prsmsp/panels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-09 21:55:30.000000 prsmsp-1.3.1/prsmsp/panels/farazsms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-09 21:55:30.000000 prsmsp-1.3.1/prsmsp/panels/ghasedaksms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-09 21:55:30.000000 prsmsp-1.3.1/prsmsp/panels/kavenegar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-09 21:55:30.000000 prsmsp-1.3.1/prsmsp/panels/mediana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-09 21:55:30.000000 prsmsp-1.3.1/prsmsp/panels/melipayamak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-09 21:55:30.000000 prsmsp-1.3.1/prsmsp/panels/smsdotir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-09 21:55:30.000000 prsmsp-1.3.1/prsmsp/panels/webonesms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:55:41.802903 prsmsp-1.3.1/prsmsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-09 21:55:41.000000 prsmsp-1.3.1/prsmsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-09 21:55:41.000000 prsmsp-1.3.1/prsmsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 21:55:41.000000 prsmsp-1.3.1/prsmsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 21:55:41.000000 prsmsp-1.3.1/prsmsp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-09 21:55:41.000000 prsmsp-1.3.1/prsmsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-09 21:55:41.000000 prsmsp-1.3.1/prsmsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-09 21:55:41.806903 prsmsp-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-09 21:55:30.000000 prsmsp-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 21:55:41.806903 prsmsp-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 21:55:30.000000 prsmsp-1.3.1/tests/test_app.py
```

### Comparing `prsmsp-1.3.0/PKG-INFO` & `prsmsp-1.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prsmsp
-Version: 1.3.0
+Version: 1.3.1
 Summary: Package to work with sms panels
 Home-page: https://github.com/parsariyahi/prsmsp
 Author: Parsa Riyahi
 Author-email: pany.parsariyahi@gmail.com
 License: MIT License
 Project-URL: Homepage, https://github.com/parsariyahi/prsmsp
 Project-URL: Documentation, https://prsmsp.readthedocs.io/en/latest/
```

### Comparing `prsmsp-1.3.0/README.md` & `prsmsp-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `prsmsp-1.3.0/prsmsp/factories/auth_factory.py` & `prsmsp-1.3.1/prsmsp/factories/auth_factory.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.3.0/prsmsp/models/response.py` & `prsmsp-1.3.1/prsmsp/models/response.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.3.0/prsmsp/panels/farazsms.py` & `prsmsp-1.3.1/prsmsp/panels/farazsms.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         :type api_key: str
 
         :rtype None
         :return: None
         """
         self.auth = AuthFactory.get("api_key")(api_key)
 
-    def _response_parser(self, resp) -> Response:
+    def _response_parser(self, resp: requests.Response) -> Response:
         status_code = int(resp.status_code)
         try: 
             real_response = json.loads(resp.text)
         except Exception:
             real_response = resp.text
```

### Comparing `prsmsp-1.3.0/prsmsp/panels/ghasedaksms.py` & `prsmsp-1.3.1/prsmsp/panels/ghasedaksms.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         :type api_key: str
 
         :rtype None
         :return: None
         """
         self.auth = AuthFactory.get("api_key")(api_key)
 
-    def _response_parser(self, resp):
+    def _response_parser(self, resp: requests.Response) -> Response:
         status_code = int(resp.status_code)
         real_response = json.loads(resp.text)
 
         return Response(status_code, real_response)
 
     def send_sms(self, receptor: str, message: str, originator: str) -> Response:
         """send sms with ghasedak sms panel
```

### Comparing `prsmsp-1.3.0/prsmsp/panels/kavenegar.py` & `prsmsp-1.3.1/prsmsp/panels/kavenegar.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         :type api_key: str
 
         :rtype None
         :return: None
         """
         self.auth = AuthFactory.get("api_key")(api_key)
 
-    def _response_parser(self, resp):
+    def _response_parser(self, resp: requests.Response) -> Response:
         status_code = int(resp.status_code)
         real_response = json.loads(resp.text)
 
         return Response(status_code, real_response)
 
     def send_sms(self, receptor: str, message: str) -> Response:
         """send sms with kavenegar sms panel
```

### Comparing `prsmsp-1.3.0/prsmsp/panels/mediana.py` & `prsmsp-1.3.1/prsmsp/panels/mediana.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         :type api_key: str
 
         :rtype None
         :return: None
         """
         self.auth = AuthFactory.get("api_key")(api_key)
 
-    def _response_parser(self, resp):
+    def _response_parser(self, resp: requests.Response) -> Response:
         status_code = int(resp.status_code)
         real_response = json.loads(resp.text)
 
         return Response(status_code, real_response)
 
     def send_sms(self, receptor: str, message: str, originator: str) -> Response:
         """send sms with mediana sms panel
```

### Comparing `prsmsp-1.3.0/prsmsp/panels/melipayamak.py` & `prsmsp-1.3.1/prsmsp/panels/melipayamak.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 
 from prsmsp.abstracts.abcpanel import ABCSmsPanel
 from prsmsp.factories import AuthFactory
 from prsmsp.models import Response
 
 
 class MeliPayamak(ABCSmsPanel):
-    def __init__(self, username, password):
+    def __init__(self, username, password) -> None:
         """Take the auth info
 
         :param username: webonesms username
         :type username: str
 
         :param password: webonesms password
         :type password: str
 
         :rtype None
         :return: None
         """
         self.auth = AuthFactory.get("username_pass")(username, password)
 
-    def _response_parser(self, resp):
+    def _response_parser(self, resp: requests.Response) -> Response:
         status_code = int(resp.status_code)
         real_response = json.loads(resp.text)
 
         return Response(status_code, real_response)
 
     def send_sms(self, receptor: str, message: str, originator: str) -> Response:
         """send sms with melipayamak sms panel
```

### Comparing `prsmsp-1.3.0/prsmsp/panels/smsdotir.py` & `prsmsp-1.3.1/prsmsp/panels/smsdotir.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 
 from prsmsp.abstracts.abcpanel import ABCSmsPanel
 from prsmsp.factories import AuthFactory
 from prsmsp.models import Response
 
 
 class SmsDotIr(ABCSmsPanel):
-    def __init__(self, api_key: str):
+    def __init__(self, api_key: str) -> None:
         """Take the auth info
 
         :param api_key: your smsir api key auth
         :type api_key: str
 
         :rtype None
         :return: None
         """
         self.auth = AuthFactory.get("api_key")(api_key)
 
-    def _response_parser(self, resp):
+    def _response_parser(self, resp: requests.Response) -> Response:
         status_code = int(resp.status_code)
         real_response = json.loads(resp.text)
 
         return Response(status_code, real_response)
 
     def send_sms(
         self, receptor: str, message: str, originator: str
```

### Comparing `prsmsp-1.3.0/prsmsp/panels/webonesms.py` & `prsmsp-1.3.1/prsmsp/panels/webonesms.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 
 from prsmsp.abstracts.abcpanel import ABCSmsPanel
 from prsmsp.factories import AuthFactory
 from prsmsp.models import Response
 
 
 class WebOneSms(ABCSmsPanel):
-    def __init__(self, username, password):
+    def __init__(self, username, password) -> None:
         """Take the auth info
 
         :param username: webonesms username
         :type username: str
 
         :param password: webonesms password
         :type password: str
 
         :rtype None
         :return: None
         """
         self.auth = AuthFactory.get("username_pass")(username, password)
 
-    def _response_parser(self, resp):
+    def _response_parser(self, resp: requests.Response) -> Response:
         status_code = int(resp.status_code)
         try:
             real_response = json.loads(resp.text)
         except json.JSONDecodeError:
             # if the json coder couldn't decode,
             # we just put it like what is is
             real_response = {"resp": resp.text}
```

### Comparing `prsmsp-1.3.0/prsmsp.egg-info/PKG-INFO` & `prsmsp-1.3.1/prsmsp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prsmsp
-Version: 1.3.0
+Version: 1.3.1
 Summary: Package to work with sms panels
 Home-page: https://github.com/parsariyahi/prsmsp
 Author: Parsa Riyahi
 Author-email: pany.parsariyahi@gmail.com
 License: MIT License
 Project-URL: Homepage, https://github.com/parsariyahi/prsmsp
 Project-URL: Documentation, https://prsmsp.readthedocs.io/en/latest/
```

### Comparing `prsmsp-1.3.0/prsmsp.egg-info/SOURCES.txt` & `prsmsp-1.3.1/prsmsp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prsmsp-1.3.0/setup.cfg` & `prsmsp-1.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prsmsp
-version = 1.3.0
+version = 1.3.1
 author = Parsa Riyahi
 author_email = pany.parsariyahi@gmail.com
 description = Package to work with sms panels
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 license_files = file: LICENSE
```

