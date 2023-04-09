# Comparing `tmp/pynocaptcha-1.3.6.tar.gz` & `tmp/pynocaptcha-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pynocaptcha-1.3.6.tar", last modified: Sat Apr  8 15:48:30 2023, max compression
+gzip compressed data, was "dist/pynocaptcha-1.3.7.tar", last modified: Sun Apr  9 05:44:17 2023, max compression
```

## Comparing `pynocaptcha-1.3.6.tar` & `pynocaptcha-1.3.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-08 15:48:30.000000 pynocaptcha-1.3.6/
--rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-04-08 15:48:30.000000 pynocaptcha-1.3.6/PKG-INFO
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-08 15:48:30.000000 pynocaptcha-1.3.6/pynocaptcha/
--rw-r--r--   0 esbiya     (501) staff       (20)      440 2023-04-04 08:12:16.000000 pynocaptcha-1.3.6/pynocaptcha/__init__.py
-drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-08 15:48:30.000000 pynocaptcha-1.3.6/pynocaptcha/crackers/
--rw-r--r--   0 esbiya     (501) staff       (20)     3603 2023-04-08 15:46:14.000000 pynocaptcha-1.3.6/pynocaptcha/crackers/base.py
--rw-r--r--   0 esbiya     (501) staff       (20)     5367 2023-04-03 02:00:17.000000 pynocaptcha-1.3.6/pynocaptcha/crackers/cloudflare.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.3.6/pynocaptcha/crackers/hcaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)     1454 2023-03-20 05:38:09.000000 pynocaptcha-1.3.6/pynocaptcha/crackers/incapsula.py
--rw-r--r--   0 esbiya     (501) staff       (20)     2893 2023-03-24 04:08:51.000000 pynocaptcha-1.3.6/pynocaptcha/crackers/recaptcha.py
--rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-04-08 15:48:29.000000 pynocaptcha-1.3.6/setup.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-09 05:44:17.000000 pynocaptcha-1.3.7/
+-rw-r--r--   0 esbiya     (501) staff       (20)      566 2023-04-09 05:44:17.000000 pynocaptcha-1.3.7/PKG-INFO
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-09 05:44:17.000000 pynocaptcha-1.3.7/pynocaptcha/
+-rw-r--r--   0 esbiya     (501) staff       (20)      440 2023-04-04 08:12:16.000000 pynocaptcha-1.3.7/pynocaptcha/__init__.py
+drwxr-xr-x   0 esbiya     (501) staff       (20)        0 2023-04-09 05:44:17.000000 pynocaptcha-1.3.7/pynocaptcha/crackers/
+-rw-r--r--   0 esbiya     (501) staff       (20)     3602 2023-04-09 05:43:24.000000 pynocaptcha-1.3.7/pynocaptcha/crackers/base.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     5367 2023-04-03 02:00:17.000000 pynocaptcha-1.3.7/pynocaptcha/crackers/cloudflare.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1339 2023-04-05 02:45:58.000000 pynocaptcha-1.3.7/pynocaptcha/crackers/hcaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     1454 2023-03-20 05:38:09.000000 pynocaptcha-1.3.7/pynocaptcha/crackers/incapsula.py
+-rw-r--r--   0 esbiya     (501) staff       (20)     2893 2023-03-24 04:08:51.000000 pynocaptcha-1.3.7/pynocaptcha/crackers/recaptcha.py
+-rw-r--r--   0 esbiya     (501) staff       (20)      846 2023-04-09 05:44:08.000000 pynocaptcha-1.3.7/setup.py
```

### Comparing `pynocaptcha-1.3.6/PKG-INFO` & `pynocaptcha-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pynocaptcha
-Version: 1.3.6
+Version: 1.3.7
 Summary: nocaptcha.io api
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: nocaptcha.io python api
 Keywords: nocaptcha
```

### Comparing `pynocaptcha-1.3.6/pynocaptcha/crackers/base.py` & `pynocaptcha-1.3.7/pynocaptcha/crackers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         developer_id: str = "",   
         user_agent: str = "",
         proxy: str = None, 
         timeout: int = 30,
         debug: bool = False,
         check_useful: bool = False,
         max_retry_times: int = 3,
-        internal_proxy=False,
+        internal_proxy=True,
         **kwargs
     ) -> None:
         """
         :param user_token: nocaptcha.io 用户 token
         :param developer_id: nocaptcha.io 用户上级代理 token
         :param user_agent: 请求流程使用 ua
         :param proxy: 请求流程代理, 不传默认使用系统代理, 某些强制要求代理一致或者特定区域的站点请传代理, 支持协议 http/https/socks5, 代理格式: {protocol}://{ip}:{port}（如有账号验证：{protocol}://{user}:{password}@{ip}:{port}）
```

### Comparing `pynocaptcha-1.3.6/pynocaptcha/crackers/cloudflare.py` & `pynocaptcha-1.3.7/pynocaptcha/crackers/cloudflare.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.3.6/pynocaptcha/crackers/hcaptcha.py` & `pynocaptcha-1.3.7/pynocaptcha/crackers/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.3.6/pynocaptcha/crackers/incapsula.py` & `pynocaptcha-1.3.7/pynocaptcha/crackers/incapsula.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.3.6/pynocaptcha/crackers/recaptcha.py` & `pynocaptcha-1.3.7/pynocaptcha/crackers/recaptcha.py`

 * *Files identical despite different names*

### Comparing `pynocaptcha-1.3.6/setup.py` & `pynocaptcha-1.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 
 
 setup(
     name='pynocaptcha',
-    version='1.3.6',
+    version='1.3.7',
     description='nocaptcha.io api',
     long_description='nocaptcha.io python api',
     install_requires=["pyhttpx", "loguru"],
     license='MIT',
     packages=["pynocaptcha/crackers", "pynocaptcha"],
     package_dir={'pynocaptcha': 'pynocaptcha'},
     platforms=["all"],
```

