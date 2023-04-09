# Comparing `tmp/pyzw-0.0.2.tar.gz` & `tmp/pyzw-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzw-0.0.2.tar", last modified: Sat Apr  8 13:39:28 2023, max compression
+gzip compressed data, was "pyzw-0.0.3.tar", last modified: Sun Apr  9 06:15:17 2023, max compression
```

## Comparing `pyzw-0.0.2.tar` & `pyzw-0.0.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 13:39:28.146858 pyzw-0.0.2/
--rw-rw-rw-   0        0        0     3734 2023-04-08 13:39:28.146858 pyzw-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2321 2023-04-08 13:16:36.000000 pyzw-0.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-08 13:39:28.131248 pyzw-0.0.2/pyzw/
--rw-rw-rw-   0        0        0        0 2023-04-08 07:44:13.000000 pyzw-0.0.2/pyzw/Dm大漠命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:08:27.000000 pyzw-0.0.2/pyzw/Excel表格命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:07:19.000000 pyzw-0.0.2/pyzw/HTTP请求命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:04:39.000000 pyzw-0.0.2/pyzw/OCR命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:08:46.000000 pyzw-0.0.2/pyzw/PPT演示命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:06:37.000000 pyzw-0.0.2/pyzw/Tk界面命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:08:14.000000 pyzw-0.0.2/pyzw/Word文档命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 03:48:43.000000 pyzw-0.0.2/pyzw/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:05:37.000000 pyzw-0.0.2/pyzw/内存命令.py
--rw-rw-rw-   0        0        0     1321 2023-04-08 06:59:16.000000 pyzw-0.0.2/pyzw/内置命令.py
--rw-rw-rw-   0        0        0        2 2023-04-08 03:12:13.000000 pyzw-0.0.2/pyzw/列表命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:24:08.000000 pyzw-0.0.2/pyzw/剪切板命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:32:53.000000 pyzw-0.0.2/pyzw/图片命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 05:07:45.000000 pyzw-0.0.2/pyzw/字符串命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:23:58.000000 pyzw-0.0.2/pyzw/字节串命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:06:20.000000 pyzw-0.0.2/pyzw/打包命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:07:05.000000 pyzw-0.0.2/pyzw/数据库命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:04:50.000000 pyzw-0.0.2/pyzw/文件命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:05:16.000000 pyzw-0.0.2/pyzw/时间命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:06:03.000000 pyzw-0.0.2/pyzw/校验命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:05:08.000000 pyzw-0.0.2/pyzw/目录命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:31:56.000000 pyzw-0.0.2/pyzw/窗口命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:06:11.000000 pyzw-0.0.2/pyzw/系统命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:05:46.000000 pyzw-0.0.2/pyzw/线程命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:32:18.000000 pyzw-0.0.2/pyzw/编码命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:05:28.000000 pyzw-0.0.2/pyzw/运算命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:05:52.000000 pyzw-0.0.2/pyzw/进程命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:32:30.000000 pyzw-0.0.2/pyzw/键盘命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:33:01.000000 pyzw-0.0.2/pyzw/颜色命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:32:38.000000 pyzw-0.0.2/pyzw/鼠标命令.py
-drwxrwxrwx   0        0        0        0 2023-04-08 13:39:28.131248 pyzw-0.0.2/pyzw.egg-info/
--rw-rw-rw-   0        0        0     3734 2023-04-08 13:39:28.000000 pyzw-0.0.2/pyzw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      786 2023-04-08 13:39:28.000000 pyzw-0.0.2/pyzw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 13:39:28.000000 pyzw-0.0.2/pyzw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-08 13:39:28.000000 pyzw-0.0.2/pyzw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 13:39:28.146858 pyzw-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2142 2023-04-08 13:39:10.000000 pyzw-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:15:17.130267 pyzw-0.0.3/
+-rw-rw-rw-   0        0        0     5706 2023-04-09 06:15:17.130267 pyzw-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3957 2023-04-09 06:12:23.000000 pyzw-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 06:15:17.109186 pyzw-0.0.3/pyzw/
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:44:13.000000 pyzw-0.0.3/pyzw/Dm大漠命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:08:27.000000 pyzw-0.0.3/pyzw/Excel表格命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:07:19.000000 pyzw-0.0.3/pyzw/HTTP请求命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:04:39.000000 pyzw-0.0.3/pyzw/OCR命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:08:46.000000 pyzw-0.0.3/pyzw/PPT演示命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:06:37.000000 pyzw-0.0.3/pyzw/Tk界面命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:08:14.000000 pyzw-0.0.3/pyzw/Word文档命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 03:48:43.000000 pyzw-0.0.3/pyzw/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:05:37.000000 pyzw-0.0.3/pyzw/内存命令.py
+-rw-rw-rw-   0        0        0     1321 2023-04-08 06:59:16.000000 pyzw-0.0.3/pyzw/内置命令.py
+-rw-rw-rw-   0        0        0        2 2023-04-08 03:12:13.000000 pyzw-0.0.3/pyzw/列表命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:24:08.000000 pyzw-0.0.3/pyzw/剪切板命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:32:53.000000 pyzw-0.0.3/pyzw/图片命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 05:07:45.000000 pyzw-0.0.3/pyzw/字符串命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:23:58.000000 pyzw-0.0.3/pyzw/字节串命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:06:20.000000 pyzw-0.0.3/pyzw/打包命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:07:05.000000 pyzw-0.0.3/pyzw/数据库命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:04:50.000000 pyzw-0.0.3/pyzw/文件命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:05:16.000000 pyzw-0.0.3/pyzw/时间命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:06:03.000000 pyzw-0.0.3/pyzw/校验命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:05:08.000000 pyzw-0.0.3/pyzw/目录命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:31:56.000000 pyzw-0.0.3/pyzw/窗口命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:06:11.000000 pyzw-0.0.3/pyzw/系统命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:05:46.000000 pyzw-0.0.3/pyzw/线程命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:32:18.000000 pyzw-0.0.3/pyzw/编码命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:05:28.000000 pyzw-0.0.3/pyzw/运算命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:05:52.000000 pyzw-0.0.3/pyzw/进程命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:32:30.000000 pyzw-0.0.3/pyzw/键盘命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:33:01.000000 pyzw-0.0.3/pyzw/颜色命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:32:38.000000 pyzw-0.0.3/pyzw/鼠标命令.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:15:17.128607 pyzw-0.0.3/pyzw.egg-info/
+-rw-rw-rw-   0        0        0     5706 2023-04-09 06:15:17.000000 pyzw-0.0.3/pyzw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      785 2023-04-09 06:15:17.000000 pyzw-0.0.3/pyzw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 06:15:17.000000 pyzw-0.0.3/pyzw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-09 06:15:17.000000 pyzw-0.0.3/pyzw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 06:15:17.131269 pyzw-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2142 2023-04-09 06:14:09.000000 pyzw-0.0.3/setup.py
```

### Comparing `pyzw-0.0.2/pyzw/内置命令.py` & `pyzw-0.0.3/pyzw/内置命令.py`

 * *Files identical despite different names*

### Comparing `pyzw-0.0.2/pyzw.egg-info/SOURCES.txt` & `pyzw-0.0.3/pyzw.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-README.rst
+README.md
 setup.py
 pyzw/Dm大漠命令.py
 pyzw/Excel表格命令.py
 pyzw/HTTP请求命令.py
 pyzw/OCR命令.py
 pyzw/PPT演示命令.py
 pyzw/Tk界面命令.py
```

### Comparing `pyzw-0.0.2/setup.py` & `pyzw-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding='utf-8').read()
 
 
 setup(
     name='pyzw',
-    version='0.0.2',
+    version='0.0.3',
     author='XueLiren',
     author_email='liren1029@gmail.com',
     maintainer='XueLiren',
     maintainer_email='liren1029@gmail.com',
     license='Apache Software License 2.0',
     keywords="中文编程 ",
     url='https://github.com/XueLiren/PyZW',
```

