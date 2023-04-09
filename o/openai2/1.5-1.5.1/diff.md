# Comparing `tmp/openai2-1.5.tar.gz` & `tmp/openai2-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai2-1.5.tar", last modified: Thu Mar 30 12:17:23 2023, max compression
+gzip compressed data, was "openai2-1.5.1.tar", last modified: Sun Apr  9 11:43:44 2023, max compression
```

## Comparing `openai2-1.5.tar` & `openai2-1.5.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    10953 2023-03-07 16:01:05.491907 openai2-1.5/LICENSE
--rw-r--r--   0        0        0     2360 2023-03-30 06:34:56.662498 openai2-1.5/README.md
--rw-r--r--   0        0        0       25 2023-03-07 03:18:11.476857 openai2-1.5/openai2/__init__.py
--rw-r--r--   0        0        0     2016 2023-03-28 03:12:38.016827 openai2-1.5/openai2/openai2.py
--rw-r--r--   0        0        0      506 2023-03-30 12:17:01.812049 openai2-1.5/pyproject.toml
--rw-r--r--   0        0        0     2618 1970-01-01 00:00:00.000000 openai2-1.5/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-03-07 16:01:05.491907 openai2-1.5.1/LICENSE
+-rw-r--r--   0        0        0     2353 2023-04-09 11:34:19.920750 openai2-1.5.1/README.md
+-rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.5.1/openai2/Licenses of dependent packages/openai/LICENSE
+-rw-r--r--   0        0        0       25 2023-03-07 03:18:11.476857 openai2-1.5.1/openai2/__init__.py
+-rw-r--r--   0        0        0     2016 2023-03-28 03:12:38.016827 openai2-1.5.1/openai2/openai2.py
+-rw-r--r--   0        0        0      618 2023-04-09 11:33:28.584926 openai2-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2707 1970-01-01 00:00:00.000000 openai2-1.5.1/PKG-INFO
```

### Comparing `openai2-1.5/LICENSE` & `openai2-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.5/README.md` & `openai2-1.5.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # 项目描述
 
 根据openai官方接口‘openai’改造的‘openai2’，比官方接口更好用一点。
 
 # 安装
 
-安装：`pip install openai2`
+```
+pip install openai2
+```
 
 # 获取api_key
 
 [获取链接1](https://platform.openai.com/account/api-keys)
 
 [获取链接2](https://www.baidu.com/s?wd=%E8%8E%B7%E5%8F%96%20openai%20api_key)
 
-# 文档
+# 教程
 
 导入：
 
 ```python
 from openai2 import Chat
 ```
 
@@ -96,8 +98,8 @@
 
 作者：许灿标
 
 邮箱：lcctoor@outlook.com
 
 [主页](https://github.com/lcctoor/me/blob/main/home.md) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg)
 
-开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme) | [史上最优雅的 mysql ORM](https://github.com/lcctoor/lccpy/blob/main/coolmysql/docs/doc_zh.md)
+开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme) | [史上最优雅的 mysql ORM](https://github.com/lcctoor/lccpy/tree/main/coolmysql#readme)
```

### Comparing `openai2-1.5/openai2/openai2.py` & `openai2-1.5.1/openai2/openai2.py`

 * *Files identical despite different names*

### Comparing `openai2-1.5/PKG-INFO` & `openai2-1.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 Metadata-Version: 2.1
 Name: openai2
-Version: 1.5
+Version: 1.5.1
 Summary: 根据openai官方接口‘openai’改造的‘openai2’，比官方接口更好用一点。
 Keywords: openai2,openai
 Author-email: 许灿标 <lcctoor@outlook.com>
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: openai >=0.27.0
+Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/openai2
 
 # 项目描述
 
 根据openai官方接口‘openai’改造的‘openai2’，比官方接口更好用一点。
 
 # 安装
 
-安装：`pip install openai2`
+```
+pip install openai2
+```
 
 # 获取api_key
 
 [获取链接1](https://platform.openai.com/account/api-keys)
 
 [获取链接2](https://www.baidu.com/s?wd=%E8%8E%B7%E5%8F%96%20openai%20api_key)
 
-# 文档
+# 教程
 
 导入：
 
 ```python
 from openai2 import Chat
 ```
 
@@ -106,8 +110,9 @@
 
 作者：许灿标
 
 邮箱：lcctoor@outlook.com
 
 [主页](https://github.com/lcctoor/me/blob/main/home.md) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR.jpg) | [Python技术微信交流群](https://raw.githubusercontent.com/lcctoor/me/main/ExchangeGroup/PythonTecQR.jpg)
 
-开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme) | [史上最优雅的 mysql ORM](https://github.com/lcctoor/lccpy/blob/main/coolmysql/docs/doc_zh.md)
+开源项目：[让 Python 更简单一点](https://github.com/lcctoor/lccpy#readme) | [史上最优雅的 mysql ORM](https://github.com/lcctoor/lccpy/tree/main/coolmysql#readme)
+
```

