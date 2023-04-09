# Comparing `tmp/aio-alipay-sdk-python-3.6.461.tar.gz` & `tmp/aio-alipay-sdk-python-3.6.462.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio-alipay-sdk-python-3.6.461.tar", last modified: Sun Apr  9 03:27:48 2023, max compression
+gzip compressed data, was "aio-alipay-sdk-python-3.6.462.tar", last modified: Sun Apr  9 03:40:32 2023, max compression
```

## Comparing `aio-alipay-sdk-python-3.6.461.tar` & `aio-alipay-sdk-python-3.6.462.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 03:27:48.652364 aio-alipay-sdk-python-3.6.461/
--rw-rw-rw-   0        0        0     1091 2022-12-12 08:56:02.000000 aio-alipay-sdk-python-3.6.461/LICENSE
--rw-rw-rw-   0        0        0     9597 2023-04-09 03:27:48.650369 aio-alipay-sdk-python-3.6.461/PKG-INFO
--rw-rw-rw-   0        0        0     8688 2022-12-12 10:24:54.000000 aio-alipay-sdk-python-3.6.461/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-09 03:27:48.638401 aio-alipay-sdk-python-3.6.461/aio_alipay/
--rw-rw-rw-   0        0        0     9732 2023-04-09 03:23:42.000000 aio-alipay-sdk-python-3.6.461/aio_alipay/AioAlipayClient.py
--rw-rw-rw-   0        0        0     2832 2022-12-12 07:32:24.000000 aio-alipay-sdk-python-3.6.461/aio_alipay/AioWebUtils.py
--rw-rw-rw-   0        0        0      179 2023-04-09 03:25:51.000000 aio-alipay-sdk-python-3.6.461/aio_alipay/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 03:27:48.645384 aio-alipay-sdk-python-3.6.461/aio_alipay_sdk_python.egg-info/
--rw-rw-rw-   0        0        0     9597 2023-04-09 03:27:48.000000 aio-alipay-sdk-python-3.6.461/aio_alipay_sdk_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-04-09 03:27:48.000000 aio-alipay-sdk-python-3.6.461/aio_alipay_sdk_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 03:27:48.000000 aio-alipay-sdk-python-3.6.461/aio_alipay_sdk_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-09 03:27:48.000000 aio-alipay-sdk-python-3.6.461/aio_alipay_sdk_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-09 03:27:48.000000 aio-alipay-sdk-python-3.6.461/aio_alipay_sdk_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 03:27:48.652364 aio-alipay-sdk-python-3.6.461/setup.cfg
--rw-rw-rw-   0        0        0     1593 2022-12-12 09:26:05.000000 aio-alipay-sdk-python-3.6.461/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:40:32.674318 aio-alipay-sdk-python-3.6.462/
+-rw-rw-rw-   0        0        0     1091 2022-12-12 08:56:02.000000 aio-alipay-sdk-python-3.6.462/LICENSE
+-rw-rw-rw-   0        0        0     9597 2023-04-09 03:40:32.673321 aio-alipay-sdk-python-3.6.462/PKG-INFO
+-rw-rw-rw-   0        0        0     8688 2022-12-12 10:24:54.000000 aio-alipay-sdk-python-3.6.462/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-09 03:40:32.665346 aio-alipay-sdk-python-3.6.462/aio_alipay/
+-rw-rw-rw-   0        0        0     9732 2023-04-09 03:23:42.000000 aio-alipay-sdk-python-3.6.462/aio_alipay/AioAlipayClient.py
+-rw-rw-rw-   0        0        0     2932 2023-04-09 03:39:55.000000 aio-alipay-sdk-python-3.6.462/aio_alipay/AioWebUtils.py
+-rw-rw-rw-   0        0        0      179 2023-04-09 03:40:05.000000 aio-alipay-sdk-python-3.6.462/aio_alipay/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:40:32.671327 aio-alipay-sdk-python-3.6.462/aio_alipay_sdk_python.egg-info/
+-rw-rw-rw-   0        0        0     9597 2023-04-09 03:40:32.000000 aio-alipay-sdk-python-3.6.462/aio_alipay_sdk_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-04-09 03:40:32.000000 aio-alipay-sdk-python-3.6.462/aio_alipay_sdk_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 03:40:32.000000 aio-alipay-sdk-python-3.6.462/aio_alipay_sdk_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-09 03:40:32.000000 aio-alipay-sdk-python-3.6.462/aio_alipay_sdk_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-09 03:40:32.000000 aio-alipay-sdk-python-3.6.462/aio_alipay_sdk_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 03:40:32.674318 aio-alipay-sdk-python-3.6.462/setup.cfg
+-rw-rw-rw-   0        0        0     1593 2022-12-12 09:26:05.000000 aio-alipay-sdk-python-3.6.462/setup.py
```

### Comparing `aio-alipay-sdk-python-3.6.461/LICENSE` & `aio-alipay-sdk-python-3.6.462/LICENSE`

 * *Files identical despite different names*

### Comparing `aio-alipay-sdk-python-3.6.461/PKG-INFO` & `aio-alipay-sdk-python-3.6.462/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-alipay-sdk-python
-Version: 3.6.461
+Version: 3.6.462
 Summary: The official Aliyun SDK for Python.
 Home-page: https://github.com/Pig-Tong/aio-alipay-sdk-python
 Author: zhut96
 Author-email: zhut96@outlook.com
 License: Apache
 Keywords: alipay,sdk,aio
 Platform: any
```

### Comparing `aio-alipay-sdk-python-3.6.461/README.rst` & `aio-alipay-sdk-python-3.6.462/README.rst`

 * *Files identical despite different names*

### Comparing `aio-alipay-sdk-python-3.6.461/aio_alipay/AioAlipayClient.py` & `aio-alipay-sdk-python-3.6.462/aio_alipay/AioAlipayClient.py`

 * *Files identical despite different names*

### Comparing `aio-alipay-sdk-python-3.6.461/aio_alipay/AioWebUtils.py` & `aio-alipay-sdk-python-3.6.462/aio_alipay/AioWebUtils.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from alipay.aop.api.constant.CommonConstants import THREAD_LOCAL
 from alipay.aop.api.exception.Exception import RequestException, ResponseException
 from alipay.aop.api.util.WebUtils import get_http_connection, url_encode, MultiPartForm
 
 
 async def do_post(url, query_string=None, headers=None, params=None, charset='utf-8', timeout=15):
     url, connection = get_http_connection(url, query_string, timeout)
+    connection = aiohttp.TCPConnector(limit=100)
     body = None
     if params:
         body = url_encode(params, charset)
     try:
         async with aiohttp.ClientSession(headers=headers, connector=connection, timeout=ClientTimeout(total=2 * 60)) as session:
             async with session.post(url, data=body) as res:
                 response_status = res.status  # 获取返回的状态码
@@ -26,15 +27,15 @@
     if response_status != 200:
         raise ResponseException('[' + THREAD_LOCAL.uuid + ']invalid http status ' + str(response_status) + ',detail body:' + response.decode(encoding=charset))
     return response
 
 
 async def do_multipart_post(url, query_string=None, headers=None, params=None, multipart_params=None, charset='utf-8', timeout=30):
     url, connection = get_http_connection(url, query_string, timeout)
-
+    connection = aiohttp.TCPConnector(limit=100)
     form = MultiPartForm(charset)
     for key, value in params.items():
         form.add_field(key, value)
     for key, value in multipart_params.items():
         file_item = value
         if file_item and isinstance(file_item, FileItem):
             form.add_file(field_name=key, file_name=file_item.get_file_name(),
@@ -49,8 +50,8 @@
             async with session.post(url, data=body) as res:
                 response_status = res.status  # 获取返回的状态码
                 response = await res.read()  # 获取返回内容
     except Exception as e:
         raise RequestException('[' + THREAD_LOCAL.uuid + ']post request failed. ' + str(e))
     if response_status != 200:
         raise ResponseException('[' + THREAD_LOCAL.uuid + ']invalid http status ' + str(response_status) + ',detail body:' + response.decode(encoding=charset))
-    return response
+    return response
```

### Comparing `aio-alipay-sdk-python-3.6.461/aio_alipay_sdk_python.egg-info/PKG-INFO` & `aio-alipay-sdk-python-3.6.462/aio_alipay_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-alipay-sdk-python
-Version: 3.6.461
+Version: 3.6.462
 Summary: The official Aliyun SDK for Python.
 Home-page: https://github.com/Pig-Tong/aio-alipay-sdk-python
 Author: zhut96
 Author-email: zhut96@outlook.com
 License: Apache
 Keywords: alipay,sdk,aio
 Platform: any
```

### Comparing `aio-alipay-sdk-python-3.6.461/setup.py` & `aio-alipay-sdk-python-3.6.462/setup.py`

 * *Files identical despite different names*

