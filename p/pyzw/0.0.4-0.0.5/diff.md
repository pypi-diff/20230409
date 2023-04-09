# Comparing `tmp/pyzw-0.0.4.tar.gz` & `tmp/pyzw-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzw-0.0.4.tar", last modified: Sun Apr  9 06:19:42 2023, max compression
+gzip compressed data, was "pyzw-0.0.5.tar", last modified: Sun Apr  9 06:37:25 2023, max compression
```

## Comparing `pyzw-0.0.4.tar` & `pyzw-0.0.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 06:19:42.542004 pyzw-0.0.4/
--rw-rw-rw-   0        0        0     5690 2023-04-09 06:19:42.542004 pyzw-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3947 2023-04-09 06:19:05.000000 pyzw-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 06:19:42.519012 pyzw-0.0.4/pyzw/
--rw-rw-rw-   0        0        0        0 2023-04-08 07:44:13.000000 pyzw-0.0.4/pyzw/Dm大漠命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:08:27.000000 pyzw-0.0.4/pyzw/Excel表格命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:07:19.000000 pyzw-0.0.4/pyzw/HTTP请求命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:04:39.000000 pyzw-0.0.4/pyzw/OCR命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:08:46.000000 pyzw-0.0.4/pyzw/PPT演示命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:06:37.000000 pyzw-0.0.4/pyzw/Tk界面命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:08:14.000000 pyzw-0.0.4/pyzw/Word文档命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 03:48:43.000000 pyzw-0.0.4/pyzw/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:05:37.000000 pyzw-0.0.4/pyzw/内存命令.py
--rw-rw-rw-   0        0        0     1321 2023-04-08 06:59:16.000000 pyzw-0.0.4/pyzw/内置命令.py
--rw-rw-rw-   0        0        0        2 2023-04-08 03:12:13.000000 pyzw-0.0.4/pyzw/列表命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:24:08.000000 pyzw-0.0.4/pyzw/剪切板命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:32:53.000000 pyzw-0.0.4/pyzw/图片命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 05:07:45.000000 pyzw-0.0.4/pyzw/字符串命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:23:58.000000 pyzw-0.0.4/pyzw/字节串命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:06:20.000000 pyzw-0.0.4/pyzw/打包命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:07:05.000000 pyzw-0.0.4/pyzw/数据库命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:04:50.000000 pyzw-0.0.4/pyzw/文件命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:05:16.000000 pyzw-0.0.4/pyzw/时间命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:06:03.000000 pyzw-0.0.4/pyzw/校验命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:05:08.000000 pyzw-0.0.4/pyzw/目录命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:31:56.000000 pyzw-0.0.4/pyzw/窗口命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:06:11.000000 pyzw-0.0.4/pyzw/系统命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:05:46.000000 pyzw-0.0.4/pyzw/线程命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:32:18.000000 pyzw-0.0.4/pyzw/编码命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:05:28.000000 pyzw-0.0.4/pyzw/运算命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:05:52.000000 pyzw-0.0.4/pyzw/进程命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:32:30.000000 pyzw-0.0.4/pyzw/键盘命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:33:01.000000 pyzw-0.0.4/pyzw/颜色命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:32:38.000000 pyzw-0.0.4/pyzw/鼠标命令.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:19:42.540005 pyzw-0.0.4/pyzw.egg-info/
--rw-rw-rw-   0        0        0     5690 2023-04-09 06:19:42.000000 pyzw-0.0.4/pyzw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      785 2023-04-09 06:19:42.000000 pyzw-0.0.4/pyzw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 06:19:42.000000 pyzw-0.0.4/pyzw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-09 06:19:42.000000 pyzw-0.0.4/pyzw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 06:19:42.542004 pyzw-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2142 2023-04-09 06:19:24.000000 pyzw-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:37:25.941398 pyzw-0.0.5/
+-rw-rw-rw-   0        0        0     5754 2023-04-09 06:37:25.940412 pyzw-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3947 2023-04-09 06:19:05.000000 pyzw-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 06:37:25.916417 pyzw-0.0.5/pyzw/
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:44:13.000000 pyzw-0.0.5/pyzw/Dm大漠命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:08:27.000000 pyzw-0.0.5/pyzw/Excel表格命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:07:19.000000 pyzw-0.0.5/pyzw/HTTP请求命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:04:39.000000 pyzw-0.0.5/pyzw/OCR命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:08:46.000000 pyzw-0.0.5/pyzw/PPT演示命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:06:37.000000 pyzw-0.0.5/pyzw/Tk界面命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:08:14.000000 pyzw-0.0.5/pyzw/Word文档命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 03:48:43.000000 pyzw-0.0.5/pyzw/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:05:37.000000 pyzw-0.0.5/pyzw/内存命令.py
+-rw-rw-rw-   0        0        0     1321 2023-04-08 06:59:16.000000 pyzw-0.0.5/pyzw/内置命令.py
+-rw-rw-rw-   0        0        0        2 2023-04-08 03:12:13.000000 pyzw-0.0.5/pyzw/列表命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:24:08.000000 pyzw-0.0.5/pyzw/剪切板命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:32:53.000000 pyzw-0.0.5/pyzw/图片命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 05:07:45.000000 pyzw-0.0.5/pyzw/字符串命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:23:58.000000 pyzw-0.0.5/pyzw/字节串命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:06:20.000000 pyzw-0.0.5/pyzw/打包命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:07:05.000000 pyzw-0.0.5/pyzw/数据库命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:04:50.000000 pyzw-0.0.5/pyzw/文件命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:05:16.000000 pyzw-0.0.5/pyzw/时间命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:06:03.000000 pyzw-0.0.5/pyzw/校验命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:05:08.000000 pyzw-0.0.5/pyzw/目录命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:31:56.000000 pyzw-0.0.5/pyzw/窗口命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:06:11.000000 pyzw-0.0.5/pyzw/系统命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:05:46.000000 pyzw-0.0.5/pyzw/线程命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:32:18.000000 pyzw-0.0.5/pyzw/编码命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:05:28.000000 pyzw-0.0.5/pyzw/运算命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:05:52.000000 pyzw-0.0.5/pyzw/进程命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:32:30.000000 pyzw-0.0.5/pyzw/键盘命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:33:01.000000 pyzw-0.0.5/pyzw/颜色命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:32:38.000000 pyzw-0.0.5/pyzw/鼠标命令.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:37:25.938413 pyzw-0.0.5/pyzw.egg-info/
+-rw-rw-rw-   0        0        0     5754 2023-04-09 06:37:25.000000 pyzw-0.0.5/pyzw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      785 2023-04-09 06:37:25.000000 pyzw-0.0.5/pyzw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 06:37:25.000000 pyzw-0.0.5/pyzw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-09 06:37:25.000000 pyzw-0.0.5/pyzw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 06:37:25.941398 pyzw-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2232 2023-04-09 06:37:05.000000 pyzw-0.0.5/setup.py
```

### Comparing `pyzw-0.0.4/PKG-INFO` & `pyzw-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyzw
-Version: 0.0.4
-Summary: Python中文库（PyZW）是基于Python标准库和诸多第三方库再次封装的中文模块，其函数命令超过1000余个，涵盖了键鼠操作、找图找色、OCR、Word文档、Excel表格、PPT演示等多个领域。封装目的仅仅是为了将英文内容翻译成中文，从而使得生活、工作语言是中文的人群也能很好地学习、使用Python，享受编程带来的便利与乐趣！
+Version: 0.0.5
+Summary: Python中文库（PyZW）是基于Python标准库和诸多第三方库再次封装的中文模块，其函数命令超过1000个，涵盖了人工智能、键鼠操作、找图找色、网页自动化、手机自动化、OCR、YOLO、OpenCV、Word文档、Excel表格、PPT演示等多个领域。封装目的仅仅是为了将英文内容翻译成中文，从而使得生活、工作语言是中文的人群也能很好地学习、使用Python，享受编程带来的便利与乐趣！
 Home-page: https://github.com/XueLiren/PyZW
 Author: XueLiren
 Author-email: liren1029@gmail.com
 Maintainer: XueLiren
 Maintainer-email: liren1029@gmail.com
 License: Apache Software License 2.0
 Keywords: 中文编程
```

### Comparing `pyzw-0.0.4/README.md` & `pyzw-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyzw-0.0.4/pyzw/内置命令.py` & `pyzw-0.0.5/pyzw/内置命令.py`

 * *Files identical despite different names*

### Comparing `pyzw-0.0.4/pyzw.egg-info/PKG-INFO` & `pyzw-0.0.5/pyzw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyzw
-Version: 0.0.4
-Summary: Python中文库（PyZW）是基于Python标准库和诸多第三方库再次封装的中文模块，其函数命令超过1000余个，涵盖了键鼠操作、找图找色、OCR、Word文档、Excel表格、PPT演示等多个领域。封装目的仅仅是为了将英文内容翻译成中文，从而使得生活、工作语言是中文的人群也能很好地学习、使用Python，享受编程带来的便利与乐趣！
+Version: 0.0.5
+Summary: Python中文库（PyZW）是基于Python标准库和诸多第三方库再次封装的中文模块，其函数命令超过1000个，涵盖了人工智能、键鼠操作、找图找色、网页自动化、手机自动化、OCR、YOLO、OpenCV、Word文档、Excel表格、PPT演示等多个领域。封装目的仅仅是为了将英文内容翻译成中文，从而使得生活、工作语言是中文的人群也能很好地学习、使用Python，享受编程带来的便利与乐趣！
 Home-page: https://github.com/XueLiren/PyZW
 Author: XueLiren
 Author-email: liren1029@gmail.com
 Maintainer: XueLiren
 Maintainer-email: liren1029@gmail.com
 License: Apache Software License 2.0
 Keywords: 中文编程
```

### Comparing `pyzw-0.0.4/pyzw.egg-info/SOURCES.txt` & `pyzw-0.0.5/pyzw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyzw-0.0.4/setup.py` & `pyzw-0.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import os
 import codecs
 from setuptools import setup
 
-
+# 读取指定文件内容
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding='utf-8').read()
 
 
 setup(
     name='pyzw',
-    version='0.0.4',
+    version='0.0.5',
     author='XueLiren',
     author_email='liren1029@gmail.com',
     maintainer='XueLiren',
     maintainer_email='liren1029@gmail.com',
     license='Apache Software License 2.0',
     keywords="中文编程 ",
     url='https://github.com/XueLiren/PyZW',
-    description='Python中文库（PyZW）是基于Python标准库和诸多第三方库再次封装的中文模块，其函数命令超过1000余个，涵盖了键鼠操作、找图找色、OCR、Word文档、'
-                'Excel表格、PPT演示等多个领域。封装目的仅仅是为了将英文内容翻译成中文，从而使得生活、工作语言是中文的人群也能很好地学习、使用Python，'
-                '享受编程带来的便利与乐趣！',
+    description='Python中文库（PyZW）是基于Python标准库和诸多第三方库再次封装的中文模块，其函数命令超过1000个，涵盖了人工智能、键鼠操作、找图找色、'
+                '网页自动化、手机自动化、OCR、YOLO、OpenCV、Word文档、Excel表格、PPT演示等多个领域。封装目的仅仅是为了将英文内容翻译成中文，'
+                '从而使得生活、工作语言是中文的人群也能很好地学习、使用Python，享受编程带来的便利与乐趣！',
     long_description=read('README.md'),
     long_description_content_type="text/markdown",
     packages=['pyzw'],
     python_requires='>=3.5',
     install_requires=[''],
     classifiers=[
         'Development Status :: 4 - Beta',
```

