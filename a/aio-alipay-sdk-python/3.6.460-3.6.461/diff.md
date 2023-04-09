# Comparing `tmp/aio-alipay-sdk-python-3.6.460.tar.gz` & `tmp/aio-alipay-sdk-python-3.6.461.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio-alipay-sdk-python-3.6.460.tar", last modified: Sun Apr  9 02:50:22 2023, max compression
+gzip compressed data, was "aio-alipay-sdk-python-3.6.461.tar", last modified: Sun Apr  9 03:27:48 2023, max compression
```

## Comparing `aio-alipay-sdk-python-3.6.460.tar` & `aio-alipay-sdk-python-3.6.461.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 02:50:22.316708 aio-alipay-sdk-python-3.6.460/
--rw-rw-rw-   0        0        0     1091 2022-12-12 08:56:02.000000 aio-alipay-sdk-python-3.6.460/LICENSE
--rw-rw-rw-   0        0        0     9597 2023-04-09 02:50:22.315711 aio-alipay-sdk-python-3.6.460/PKG-INFO
--rw-rw-rw-   0        0        0     8688 2022-12-12 10:24:54.000000 aio-alipay-sdk-python-3.6.460/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-09 02:50:22.306767 aio-alipay-sdk-python-3.6.460/aio_alipay/
--rw-rw-rw-   0        0        0     1720 2023-04-09 02:25:36.000000 aio-alipay-sdk-python-3.6.460/aio_alipay/AioAlipayClient.py
--rw-rw-rw-   0        0        0     2832 2022-12-12 07:32:24.000000 aio-alipay-sdk-python-3.6.460/aio_alipay/AioWebUtils.py
--rw-rw-rw-   0        0        0      179 2023-04-09 02:30:34.000000 aio-alipay-sdk-python-3.6.460/aio_alipay/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 02:50:22.314714 aio-alipay-sdk-python-3.6.460/aio_alipay_sdk_python.egg-info/
--rw-rw-rw-   0        0        0     9597 2023-04-09 02:50:22.000000 aio-alipay-sdk-python-3.6.460/aio_alipay_sdk_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-04-09 02:50:22.000000 aio-alipay-sdk-python-3.6.460/aio_alipay_sdk_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 02:50:22.000000 aio-alipay-sdk-python-3.6.460/aio_alipay_sdk_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-09 02:50:22.000000 aio-alipay-sdk-python-3.6.460/aio_alipay_sdk_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-09 02:50:22.000000 aio-alipay-sdk-python-3.6.460/aio_alipay_sdk_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 02:50:22.316708 aio-alipay-sdk-python-3.6.460/setup.cfg
--rw-rw-rw-   0        0        0     1593 2022-12-12 09:26:05.000000 aio-alipay-sdk-python-3.6.460/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:27:48.652364 aio-alipay-sdk-python-3.6.461/
+-rw-rw-rw-   0        0        0     1091 2022-12-12 08:56:02.000000 aio-alipay-sdk-python-3.6.461/LICENSE
+-rw-rw-rw-   0        0        0     9597 2023-04-09 03:27:48.650369 aio-alipay-sdk-python-3.6.461/PKG-INFO
+-rw-rw-rw-   0        0        0     8688 2022-12-12 10:24:54.000000 aio-alipay-sdk-python-3.6.461/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-09 03:27:48.638401 aio-alipay-sdk-python-3.6.461/aio_alipay/
+-rw-rw-rw-   0        0        0     9732 2023-04-09 03:23:42.000000 aio-alipay-sdk-python-3.6.461/aio_alipay/AioAlipayClient.py
+-rw-rw-rw-   0        0        0     2832 2022-12-12 07:32:24.000000 aio-alipay-sdk-python-3.6.461/aio_alipay/AioWebUtils.py
+-rw-rw-rw-   0        0        0      179 2023-04-09 03:25:51.000000 aio-alipay-sdk-python-3.6.461/aio_alipay/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 03:27:48.645384 aio-alipay-sdk-python-3.6.461/aio_alipay_sdk_python.egg-info/
+-rw-rw-rw-   0        0        0     9597 2023-04-09 03:27:48.000000 aio-alipay-sdk-python-3.6.461/aio_alipay_sdk_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-04-09 03:27:48.000000 aio-alipay-sdk-python-3.6.461/aio_alipay_sdk_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 03:27:48.000000 aio-alipay-sdk-python-3.6.461/aio_alipay_sdk_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-09 03:27:48.000000 aio-alipay-sdk-python-3.6.461/aio_alipay_sdk_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-09 03:27:48.000000 aio-alipay-sdk-python-3.6.461/aio_alipay_sdk_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 03:27:48.652364 aio-alipay-sdk-python-3.6.461/setup.cfg
+-rw-rw-rw-   0        0        0     1593 2022-12-12 09:26:05.000000 aio-alipay-sdk-python-3.6.461/setup.py
```

### Comparing `aio-alipay-sdk-python-3.6.460/LICENSE` & `aio-alipay-sdk-python-3.6.461/LICENSE`

 * *Files identical despite different names*

### Comparing `aio-alipay-sdk-python-3.6.460/PKG-INFO` & `aio-alipay-sdk-python-3.6.461/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-alipay-sdk-python
-Version: 3.6.460
+Version: 3.6.461
 Summary: The official Aliyun SDK for Python.
 Home-page: https://github.com/Pig-Tong/aio-alipay-sdk-python
 Author: zhut96
 Author-email: zhut96@outlook.com
 License: Apache
 Keywords: alipay,sdk,aio
 Platform: any
```

### Comparing `aio-alipay-sdk-python-3.6.460/README.rst` & `aio-alipay-sdk-python-3.6.461/README.rst`

 * *Files identical despite different names*

### Comparing `aio-alipay-sdk-python-3.6.460/aio_alipay/AioWebUtils.py` & `aio-alipay-sdk-python-3.6.461/aio_alipay/AioWebUtils.py`

 * *Files identical despite different names*

### Comparing `aio-alipay-sdk-python-3.6.460/aio_alipay_sdk_python.egg-info/PKG-INFO` & `aio-alipay-sdk-python-3.6.461/aio_alipay_sdk_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-alipay-sdk-python
-Version: 3.6.460
+Version: 3.6.461
 Summary: The official Aliyun SDK for Python.
 Home-page: https://github.com/Pig-Tong/aio-alipay-sdk-python
 Author: zhut96
 Author-email: zhut96@outlook.com
 License: Apache
 Keywords: alipay,sdk,aio
 Platform: any
```

### Comparing `aio-alipay-sdk-python-3.6.460/setup.py` & `aio-alipay-sdk-python-3.6.461/setup.py`

 * *Files identical despite different names*

