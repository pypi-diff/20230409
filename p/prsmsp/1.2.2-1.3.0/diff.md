# Comparing `tmp/prsmsp-1.2.2.tar.gz` & `tmp/prsmsp-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prsmsp-1.2.2.tar", last modified: Sat Apr  8 19:20:55 2023, max compression
+gzip compressed data, was "prsmsp-1.3.0.tar", last modified: Sun Apr  9 15:57:09 2023, max compression
```

## Comparing `prsmsp-1.2.2.tar` & `prsmsp-1.3.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:55.817584 prsmsp-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-08 19:20:55.817584 prsmsp-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-08 19:20:46.000000 prsmsp-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:55.813584 prsmsp-1.2.2/prsmsp/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:55.813584 prsmsp-1.2.2/prsmsp/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/abstracts/abcpanel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:55.813584 prsmsp-1.2.2/prsmsp/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/exceptions/abstracts.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/exceptions/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/exceptions/panels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:55.813584 prsmsp-1.2.2/prsmsp/factories/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/factories/auth_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:55.813584 prsmsp-1.2.2/prsmsp/models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/models/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/models/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:55.817584 prsmsp-1.2.2/prsmsp/panels/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/panels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/panels/ghasedaksms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/panels/kavenegar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/panels/mediana.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/panels/melipayamak.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/panels/smsdotir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-08 19:20:46.000000 prsmsp-1.2.2/prsmsp/panels/webonesms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:55.813584 prsmsp-1.2.2/prsmsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-08 19:20:55.000000 prsmsp-1.2.2/prsmsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-08 19:20:55.000000 prsmsp-1.2.2/prsmsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 19:20:55.000000 prsmsp-1.2.2/prsmsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 19:20:55.000000 prsmsp-1.2.2/prsmsp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-08 19:20:55.000000 prsmsp-1.2.2/prsmsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-08 19:20:55.000000 prsmsp-1.2.2/prsmsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-08 19:20:55.817584 prsmsp-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-08 19:20:46.000000 prsmsp-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:55.817584 prsmsp-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 19:20:46.000000 prsmsp-1.2.2/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:57:09.349088 prsmsp-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-09 15:57:09.349088 prsmsp-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-09 15:56:59.000000 prsmsp-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:57:09.345088 prsmsp-1.3.0/prsmsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:57:09.345088 prsmsp-1.3.0/prsmsp/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/abstracts/abcpanel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:57:09.345088 prsmsp-1.3.0/prsmsp/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/exceptions/abstracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/exceptions/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/exceptions/panels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:57:09.349088 prsmsp-1.3.0/prsmsp/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/factories/auth_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:57:09.349088 prsmsp-1.3.0/prsmsp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/models/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/models/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:57:09.349088 prsmsp-1.3.0/prsmsp/panels/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/panels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/panels/farazsms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/panels/ghasedaksms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/panels/kavenegar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/panels/mediana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/panels/melipayamak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/panels/smsdotir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-09 15:56:59.000000 prsmsp-1.3.0/prsmsp/panels/webonesms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:57:09.345088 prsmsp-1.3.0/prsmsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-09 15:57:09.000000 prsmsp-1.3.0/prsmsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-09 15:57:09.000000 prsmsp-1.3.0/prsmsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 15:57:09.000000 prsmsp-1.3.0/prsmsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 15:57:09.000000 prsmsp-1.3.0/prsmsp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-09 15:57:09.000000 prsmsp-1.3.0/prsmsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-09 15:57:09.000000 prsmsp-1.3.0/prsmsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-09 15:57:09.349088 prsmsp-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-09 15:56:59.000000 prsmsp-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:57:09.349088 prsmsp-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 15:56:59.000000 prsmsp-1.3.0/tests/test_app.py
```

### Comparing `prsmsp-1.2.2/PKG-INFO` & `prsmsp-1.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prsmsp
-Version: 1.2.2
+Version: 1.3.0
 Summary: Package to work with sms panels
 Home-page: https://github.com/parsariyahi/prsmsp
 Author: Parsa Riyahi
 Author-email: pany.parsariyahi@gmail.com
 License: MIT License
 Project-URL: Homepage, https://github.com/parsariyahi/prsmsp
 Project-URL: Documentation, https://prsmsp.readthedocs.io/en/latest/
@@ -23,14 +23,15 @@
 
 * [Kavenegar](http://kavenegar.com)
 * [Sms.ir](http://sms.ir)
 * [Web one](http://webone-sms.ir)
 * [Meli Payamak](https://www.melipayamak.com)
 * [Mediana](https://mediana.ir)
 * [Ghasedak Sms](https://ghasedak.me)
+* [Faraz Sms](https://farazsms.com/)
 
 ## Why use this package?
 
 1.  You have all the famous and well designed sms panels ready to go.
 2.  When you have to work with several sms panels.
 3.  Don't need to build the wheel of your bicycle each time ☺.
```

### Comparing `prsmsp-1.2.2/README.md` & `prsmsp-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 * [Kavenegar](http://kavenegar.com)
 * [Sms.ir](http://sms.ir)
 * [Web one](http://webone-sms.ir)
 * [Meli Payamak](https://www.melipayamak.com)
 * [Mediana](https://mediana.ir)
 * [Ghasedak Sms](https://ghasedak.me)
+* [Faraz Sms](https://farazsms.com/)
 
 ## Why use this package?
 
 1.  You have all the famous and well designed sms panels ready to go.
 2.  When you have to work with several sms panels.
 3.  Don't need to build the wheel of your bicycle each time ☺.
```

### Comparing `prsmsp-1.2.2/prsmsp/factories/auth_factory.py` & `prsmsp-1.3.0/prsmsp/factories/auth_factory.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.2.2/prsmsp/models/response.py` & `prsmsp-1.3.0/prsmsp/models/response.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.2.2/prsmsp/panels/ghasedaksms.py` & `prsmsp-1.3.0/prsmsp/panels/ghasedaksms.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.2.2/prsmsp/panels/kavenegar.py` & `prsmsp-1.3.0/prsmsp/panels/kavenegar.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.2.2/prsmsp/panels/mediana.py` & `prsmsp-1.3.0/prsmsp/panels/mediana.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.2.2/prsmsp/panels/melipayamak.py` & `prsmsp-1.3.0/prsmsp/panels/melipayamak.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.2.2/prsmsp/panels/smsdotir.py` & `prsmsp-1.3.0/prsmsp/panels/smsdotir.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.2.2/prsmsp/panels/webonesms.py` & `prsmsp-1.3.0/prsmsp/panels/webonesms.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.2.2/prsmsp.egg-info/PKG-INFO` & `prsmsp-1.3.0/prsmsp.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prsmsp
-Version: 1.2.2
+Version: 1.3.0
 Summary: Package to work with sms panels
 Home-page: https://github.com/parsariyahi/prsmsp
 Author: Parsa Riyahi
 Author-email: pany.parsariyahi@gmail.com
 License: MIT License
 Project-URL: Homepage, https://github.com/parsariyahi/prsmsp
 Project-URL: Documentation, https://prsmsp.readthedocs.io/en/latest/
@@ -23,14 +23,15 @@
 
 * [Kavenegar](http://kavenegar.com)
 * [Sms.ir](http://sms.ir)
 * [Web one](http://webone-sms.ir)
 * [Meli Payamak](https://www.melipayamak.com)
 * [Mediana](https://mediana.ir)
 * [Ghasedak Sms](https://ghasedak.me)
+* [Faraz Sms](https://farazsms.com/)
 
 ## Why use this package?
 
 1.  You have all the famous and well designed sms panels ready to go.
 2.  When you have to work with several sms panels.
 3.  Don't need to build the wheel of your bicycle each time ☺.
```

### Comparing `prsmsp-1.2.2/prsmsp.egg-info/SOURCES.txt` & `prsmsp-1.3.0/prsmsp.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 prsmsp/exceptions/panels.py
 prsmsp/factories/__init__.py
 prsmsp/factories/auth_factory.py
 prsmsp/models/__init__.py
 prsmsp/models/auth.py
 prsmsp/models/response.py
 prsmsp/panels/__init__.py
+prsmsp/panels/farazsms.py
 prsmsp/panels/ghasedaksms.py
 prsmsp/panels/kavenegar.py
 prsmsp/panels/mediana.py
 prsmsp/panels/melipayamak.py
 prsmsp/panels/smsdotir.py
 prsmsp/panels/webonesms.py
 tests/test_app.py
```

### Comparing `prsmsp-1.2.2/setup.cfg` & `prsmsp-1.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prsmsp
-version = 1.2.2
+version = 1.3.0
 author = Parsa Riyahi
 author_email = pany.parsariyahi@gmail.com
 description = Package to work with sms panels
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 license_files = file: LICENSE
```

