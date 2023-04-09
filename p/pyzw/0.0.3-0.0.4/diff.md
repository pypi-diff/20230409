# Comparing `tmp/pyzw-0.0.3.tar.gz` & `tmp/pyzw-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzw-0.0.3.tar", last modified: Sun Apr  9 06:15:17 2023, max compression
+gzip compressed data, was "pyzw-0.0.4.tar", last modified: Sun Apr  9 06:19:42 2023, max compression
```

## Comparing `pyzw-0.0.3.tar` & `pyzw-0.0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 06:15:17.130267 pyzw-0.0.3/
--rw-rw-rw-   0        0        0     5706 2023-04-09 06:15:17.130267 pyzw-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3957 2023-04-09 06:12:23.000000 pyzw-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 06:15:17.109186 pyzw-0.0.3/pyzw/
--rw-rw-rw-   0        0        0        0 2023-04-08 07:44:13.000000 pyzw-0.0.3/pyzw/Dm大漠命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:08:27.000000 pyzw-0.0.3/pyzw/Excel表格命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:07:19.000000 pyzw-0.0.3/pyzw/HTTP请求命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:04:39.000000 pyzw-0.0.3/pyzw/OCR命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:08:46.000000 pyzw-0.0.3/pyzw/PPT演示命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:06:37.000000 pyzw-0.0.3/pyzw/Tk界面命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:08:14.000000 pyzw-0.0.3/pyzw/Word文档命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 03:48:43.000000 pyzw-0.0.3/pyzw/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:05:37.000000 pyzw-0.0.3/pyzw/内存命令.py
--rw-rw-rw-   0        0        0     1321 2023-04-08 06:59:16.000000 pyzw-0.0.3/pyzw/内置命令.py
--rw-rw-rw-   0        0        0        2 2023-04-08 03:12:13.000000 pyzw-0.0.3/pyzw/列表命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:24:08.000000 pyzw-0.0.3/pyzw/剪切板命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:32:53.000000 pyzw-0.0.3/pyzw/图片命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 05:07:45.000000 pyzw-0.0.3/pyzw/字符串命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:23:58.000000 pyzw-0.0.3/pyzw/字节串命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:06:20.000000 pyzw-0.0.3/pyzw/打包命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:07:05.000000 pyzw-0.0.3/pyzw/数据库命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:04:50.000000 pyzw-0.0.3/pyzw/文件命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:05:16.000000 pyzw-0.0.3/pyzw/时间命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:06:03.000000 pyzw-0.0.3/pyzw/校验命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:05:08.000000 pyzw-0.0.3/pyzw/目录命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:31:56.000000 pyzw-0.0.3/pyzw/窗口命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:06:11.000000 pyzw-0.0.3/pyzw/系统命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:05:46.000000 pyzw-0.0.3/pyzw/线程命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:32:18.000000 pyzw-0.0.3/pyzw/编码命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:05:28.000000 pyzw-0.0.3/pyzw/运算命令.py
--rw-rw-rw-   0        0        0        0 2023-04-08 07:05:52.000000 pyzw-0.0.3/pyzw/进程命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:32:30.000000 pyzw-0.0.3/pyzw/键盘命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:33:01.000000 pyzw-0.0.3/pyzw/颜色命令.py
--rw-rw-rw-   0        0        0        0 2023-04-07 06:32:38.000000 pyzw-0.0.3/pyzw/鼠标命令.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:15:17.128607 pyzw-0.0.3/pyzw.egg-info/
--rw-rw-rw-   0        0        0     5706 2023-04-09 06:15:17.000000 pyzw-0.0.3/pyzw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      785 2023-04-09 06:15:17.000000 pyzw-0.0.3/pyzw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 06:15:17.000000 pyzw-0.0.3/pyzw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-09 06:15:17.000000 pyzw-0.0.3/pyzw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 06:15:17.131269 pyzw-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2142 2023-04-09 06:14:09.000000 pyzw-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:19:42.542004 pyzw-0.0.4/
+-rw-rw-rw-   0        0        0     5690 2023-04-09 06:19:42.542004 pyzw-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3947 2023-04-09 06:19:05.000000 pyzw-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 06:19:42.519012 pyzw-0.0.4/pyzw/
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:44:13.000000 pyzw-0.0.4/pyzw/Dm大漠命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:08:27.000000 pyzw-0.0.4/pyzw/Excel表格命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:07:19.000000 pyzw-0.0.4/pyzw/HTTP请求命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:04:39.000000 pyzw-0.0.4/pyzw/OCR命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:08:46.000000 pyzw-0.0.4/pyzw/PPT演示命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:06:37.000000 pyzw-0.0.4/pyzw/Tk界面命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:08:14.000000 pyzw-0.0.4/pyzw/Word文档命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 03:48:43.000000 pyzw-0.0.4/pyzw/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:05:37.000000 pyzw-0.0.4/pyzw/内存命令.py
+-rw-rw-rw-   0        0        0     1321 2023-04-08 06:59:16.000000 pyzw-0.0.4/pyzw/内置命令.py
+-rw-rw-rw-   0        0        0        2 2023-04-08 03:12:13.000000 pyzw-0.0.4/pyzw/列表命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:24:08.000000 pyzw-0.0.4/pyzw/剪切板命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:32:53.000000 pyzw-0.0.4/pyzw/图片命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 05:07:45.000000 pyzw-0.0.4/pyzw/字符串命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:23:58.000000 pyzw-0.0.4/pyzw/字节串命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:06:20.000000 pyzw-0.0.4/pyzw/打包命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:07:05.000000 pyzw-0.0.4/pyzw/数据库命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:04:50.000000 pyzw-0.0.4/pyzw/文件命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:05:16.000000 pyzw-0.0.4/pyzw/时间命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:06:03.000000 pyzw-0.0.4/pyzw/校验命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:05:08.000000 pyzw-0.0.4/pyzw/目录命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:31:56.000000 pyzw-0.0.4/pyzw/窗口命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:06:11.000000 pyzw-0.0.4/pyzw/系统命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:05:46.000000 pyzw-0.0.4/pyzw/线程命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:32:18.000000 pyzw-0.0.4/pyzw/编码命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:05:28.000000 pyzw-0.0.4/pyzw/运算命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-08 07:05:52.000000 pyzw-0.0.4/pyzw/进程命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:32:30.000000 pyzw-0.0.4/pyzw/键盘命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:33:01.000000 pyzw-0.0.4/pyzw/颜色命令.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 06:32:38.000000 pyzw-0.0.4/pyzw/鼠标命令.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:19:42.540005 pyzw-0.0.4/pyzw.egg-info/
+-rw-rw-rw-   0        0        0     5690 2023-04-09 06:19:42.000000 pyzw-0.0.4/pyzw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      785 2023-04-09 06:19:42.000000 pyzw-0.0.4/pyzw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 06:19:42.000000 pyzw-0.0.4/pyzw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-09 06:19:42.000000 pyzw-0.0.4/pyzw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 06:19:42.542004 pyzw-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2142 2023-04-09 06:19:24.000000 pyzw-0.0.4/setup.py
```

### Comparing `pyzw-0.0.3/PKG-INFO` & `pyzw-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzw
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python中文库（PyZW）是基于Python标准库和诸多第三方库再次封装的中文模块，其函数命令超过1000余个，涵盖了键鼠操作、找图找色、OCR、Word文档、Excel表格、PPT演示等多个领域。封装目的仅仅是为了将英文内容翻译成中文，从而使得生活、工作语言是中文的人群也能很好地学习、使用Python，享受编程带来的便利与乐趣！
 Home-page: https://github.com/XueLiren/PyZW
 Author: XueLiren
 Author-email: liren1029@gmail.com
 Maintainer: XueLiren
 Maintainer-email: liren1029@gmail.com
 License: Apache Software License 2.0
@@ -27,20 +27,17 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
 # 欢迎使用 Python中文库（PyZW）
 ***
-![PyPI version](https://img.shields.io/pypi/v/pytest-pyzw.svg)
-![Python versions](https://img.shields.io/pypi/pyversions/pytest-pyzw.svg)
-![See Build Status on AppVeyor](https://ci.appveyor.com/api/projects/status/github/XueLiren/pytest-pyzw?branch=master)
+![PyPI version](https://img.shields.io/pypi/v/pytest-pyzw.svg) ![Python versions](https://img.shields.io/pypi/pyversions/pytest-pyzw.svg) ![See Build Status on AppVeyor](https://ci.appveyor.com/api/projects/status/github/XueLiren/pytest-pyzw?branch=master)
 
-&emsp;&emsp;Python中文库（PyZW）是基于Python标准库和诸多第三方库再次封装的中文模块，其函数命令超过1000个，涵盖了人工智能、键鼠操作、找图找色、
-网页自动化、手机自动化、OCR、YOLO、OpenCV、Word文档、Excel表格、PPT演示等多个领域。封装目的仅仅是为了将英文内容翻译成中文，从而使得生活、工作语言是中文的人群也能很好地学习、使用Python，享受编程带来的便利与乐趣！
+&emsp;&emsp;Python中文库（PyZW）是基于Python标准库和诸多第三方库再次封装的中文模块，其函数命令超过1000个，涵盖了人工智能、键鼠操作、找图找色、网页自动化、手机自动化、OCR、YOLO、OpenCV、Word文档、Excel表格、PPT演示等多个领域。封装目的仅仅是为了将英文内容翻译成中文，从而使得生活、工作语言是中文的人群也能很好地学习、使用Python，享受编程带来的便利与乐趣！
 
 ***
 ## Features
 
 * TODO
 ***
 ## Requirements
@@ -76,26 +73,23 @@
 
 `PyPI`: https://pypi.org/project
 
 ***
 ## 常见问题
 ### 学编程，到底要不要学英语？
 
-&emsp;&emsp;常说的“学编程，先学英语”，不是指需要很好的英语水平才能写代码，而是由于人工智能、深度学习、神经网络、目标检测等最新的前沿技术都是国外团队开发出来的，
-我们不得不先学他们使用的语言——英语，才能更好地学习他们发表的文档资料，与他们交流问题以及应用这些技术。
+&emsp;&emsp;常说的“学编程，先学英语”，不是指需要很好的英语水平才能写代码，而是由于人工智能、深度学习、神经网络、目标检测等最新的前沿技术都是国外团队开发出来的，我们不得不先学他们使用的语言——英语，才能更好地学习他们发表的文档资料，与他们交流问题以及应用这些技术。
 
 &emsp;&emsp;所以，如果你的目标是掌握各类前沿技术，那必须学好英语；如果你的目标只是实现传统的办公自动化、游戏自动化，那不需要学英语，因为这些传统的编程技术在国内各个平台上已经有了足够多的中文资料供大家学习。
 
 
 ### 使用中文编程，会不会很丢脸？被嘲笑？
 
-&emsp;&emsp;编程从初期的机器语言，到早期的汇编语言，再到如今的各类高级语言，以及现在提出的AI编程，这一路都是朝着“更加符合自然语言”的方向发展的，而使用中文编程是朝着“更加符合中国人自然语言”的方向发展，
-这个方向是正确无疑的。革命先烈撬动了核武霸权，如今人民币可以撬动美元霸权，有朝一日中文也一定能撬动英文霸权。中文编程与汉字简化一样对国民科技教育普及有重大意义。
+&emsp;&emsp;编程从初期的机器语言，到早期的汇编语言，再到如今的各类高级语言，以及现在提出的AI编程，这一路都是朝着“更加符合自然语言”的方向发展的，而使用中文编程是朝着“更加符合中国人自然语言”的方向发展，这个方向是正确无疑的。革命先烈撬动了核武霸权，如今人民币可以撬动美元霸权，有朝一日中文也一定能撬动英文霸权。中文编程与汉字简化一样对国民科技教育普及有重大意义。
 
-&emsp;&emsp;无论中文编程、英文编程还是使用其他国家的语言编程，最终都会被替换为“0”和“1”组成的机器语言，中文、英文都相当于给机器语言穿了一件外套，如果有人非说英文外套就是比中文外套好，
-国外的月亮就是比国内的月亮圆，这是不对的。
+&emsp;&emsp;无论中文编程、英文编程还是使用其他国家的语言编程，最终都会被替换为“0”和“1”组成的机器语言，中文、英文都相当于给机器语言穿了一件外套，如果有人非说英文外套就是比中文外套好，国外的月亮就是比国内的月亮圆，这是不对的。
 
 &emsp;&emsp;所以，中文编程不落后、不丢脸，是符合编程语言发展方向的，不应该被嘲笑。而实现不了需求、写不出功能的编程人，即使英语专八，也是丢脸的，但不应该被嘲笑。无论何时何事，我们都不应该嘲笑别人。
 
+
 ### 关于 PyZW 的争议
-&emsp;&emsp;难免有人会说，英文是给机器语言穿一件外套，那 PyZW 这个中文库是穿了两件外套。其实，是可以从源码上进行修改，使得 PyZW 也只穿一件外套的。之所以坚持如此，原因有三：
-一是尊重原作者的贡献；二是敬畏国外技术领先国内；三是警醒我辈编程人任重而道远。
+&emsp;&emsp;难免有人会说，英文是给机器语言穿一件外套，那 PyZW 这个中文库是穿了两件外套。其实，是可以从源码上进行修改，使得 PyZW 也只穿一件外套的。之所以坚持如此，原因有三：一是尊重原作者的贡献；二是敬畏国外技术领先国内；三是警醒我辈编程人任重而道远。
```

### Comparing `pyzw-0.0.3/README.md` & `pyzw-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 # 欢迎使用 Python中文库（PyZW）
 ***
-![PyPI version](https://img.shields.io/pypi/v/pytest-pyzw.svg)
-![Python versions](https://img.shields.io/pypi/pyversions/pytest-pyzw.svg)
-![See Build Status on AppVeyor](https://ci.appveyor.com/api/projects/status/github/XueLiren/pytest-pyzw?branch=master)
+![PyPI version](https://img.shields.io/pypi/v/pytest-pyzw.svg) ![Python versions](https://img.shields.io/pypi/pyversions/pytest-pyzw.svg) ![See Build Status on AppVeyor](https://ci.appveyor.com/api/projects/status/github/XueLiren/pytest-pyzw?branch=master)
 
-&emsp;&emsp;Python中文库（PyZW）是基于Python标准库和诸多第三方库再次封装的中文模块，其函数命令超过1000个，涵盖了人工智能、键鼠操作、找图找色、
-网页自动化、手机自动化、OCR、YOLO、OpenCV、Word文档、Excel表格、PPT演示等多个领域。封装目的仅仅是为了将英文内容翻译成中文，从而使得生活、工作语言是中文的人群也能很好地学习、使用Python，享受编程带来的便利与乐趣！
+&emsp;&emsp;Python中文库（PyZW）是基于Python标准库和诸多第三方库再次封装的中文模块，其函数命令超过1000个，涵盖了人工智能、键鼠操作、找图找色、网页自动化、手机自动化、OCR、YOLO、OpenCV、Word文档、Excel表格、PPT演示等多个领域。封装目的仅仅是为了将英文内容翻译成中文，从而使得生活、工作语言是中文的人群也能很好地学习、使用Python，享受编程带来的便利与乐趣！
 
 ***
 ## Features
 
 * TODO
 ***
 ## Requirements
@@ -45,26 +42,23 @@
 
 `PyPI`: https://pypi.org/project
 
 ***
 ## 常见问题
 ### 学编程，到底要不要学英语？
 
-&emsp;&emsp;常说的“学编程，先学英语”，不是指需要很好的英语水平才能写代码，而是由于人工智能、深度学习、神经网络、目标检测等最新的前沿技术都是国外团队开发出来的，
-我们不得不先学他们使用的语言——英语，才能更好地学习他们发表的文档资料，与他们交流问题以及应用这些技术。
+&emsp;&emsp;常说的“学编程，先学英语”，不是指需要很好的英语水平才能写代码，而是由于人工智能、深度学习、神经网络、目标检测等最新的前沿技术都是国外团队开发出来的，我们不得不先学他们使用的语言——英语，才能更好地学习他们发表的文档资料，与他们交流问题以及应用这些技术。
 
 &emsp;&emsp;所以，如果你的目标是掌握各类前沿技术，那必须学好英语；如果你的目标只是实现传统的办公自动化、游戏自动化，那不需要学英语，因为这些传统的编程技术在国内各个平台上已经有了足够多的中文资料供大家学习。
 
 
 ### 使用中文编程，会不会很丢脸？被嘲笑？
 
-&emsp;&emsp;编程从初期的机器语言，到早期的汇编语言，再到如今的各类高级语言，以及现在提出的AI编程，这一路都是朝着“更加符合自然语言”的方向发展的，而使用中文编程是朝着“更加符合中国人自然语言”的方向发展，
-这个方向是正确无疑的。革命先烈撬动了核武霸权，如今人民币可以撬动美元霸权，有朝一日中文也一定能撬动英文霸权。中文编程与汉字简化一样对国民科技教育普及有重大意义。
+&emsp;&emsp;编程从初期的机器语言，到早期的汇编语言，再到如今的各类高级语言，以及现在提出的AI编程，这一路都是朝着“更加符合自然语言”的方向发展的，而使用中文编程是朝着“更加符合中国人自然语言”的方向发展，这个方向是正确无疑的。革命先烈撬动了核武霸权，如今人民币可以撬动美元霸权，有朝一日中文也一定能撬动英文霸权。中文编程与汉字简化一样对国民科技教育普及有重大意义。
 
-&emsp;&emsp;无论中文编程、英文编程还是使用其他国家的语言编程，最终都会被替换为“0”和“1”组成的机器语言，中文、英文都相当于给机器语言穿了一件外套，如果有人非说英文外套就是比中文外套好，
-国外的月亮就是比国内的月亮圆，这是不对的。
+&emsp;&emsp;无论中文编程、英文编程还是使用其他国家的语言编程，最终都会被替换为“0”和“1”组成的机器语言，中文、英文都相当于给机器语言穿了一件外套，如果有人非说英文外套就是比中文外套好，国外的月亮就是比国内的月亮圆，这是不对的。
 
 &emsp;&emsp;所以，中文编程不落后、不丢脸，是符合编程语言发展方向的，不应该被嘲笑。而实现不了需求、写不出功能的编程人，即使英语专八，也是丢脸的，但不应该被嘲笑。无论何时何事，我们都不应该嘲笑别人。
 
+
 ### 关于 PyZW 的争议
-&emsp;&emsp;难免有人会说，英文是给机器语言穿一件外套，那 PyZW 这个中文库是穿了两件外套。其实，是可以从源码上进行修改，使得 PyZW 也只穿一件外套的。之所以坚持如此，原因有三：
-一是尊重原作者的贡献；二是敬畏国外技术领先国内；三是警醒我辈编程人任重而道远。
+&emsp;&emsp;难免有人会说，英文是给机器语言穿一件外套，那 PyZW 这个中文库是穿了两件外套。其实，是可以从源码上进行修改，使得 PyZW 也只穿一件外套的。之所以坚持如此，原因有三：一是尊重原作者的贡献；二是敬畏国外技术领先国内；三是警醒我辈编程人任重而道远。
```

### Comparing `pyzw-0.0.3/pyzw/内置命令.py` & `pyzw-0.0.4/pyzw/内置命令.py`

 * *Files identical despite different names*

### Comparing `pyzw-0.0.3/pyzw.egg-info/PKG-INFO` & `pyzw-0.0.4/pyzw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzw
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python中文库（PyZW）是基于Python标准库和诸多第三方库再次封装的中文模块，其函数命令超过1000余个，涵盖了键鼠操作、找图找色、OCR、Word文档、Excel表格、PPT演示等多个领域。封装目的仅仅是为了将英文内容翻译成中文，从而使得生活、工作语言是中文的人群也能很好地学习、使用Python，享受编程带来的便利与乐趣！
 Home-page: https://github.com/XueLiren/PyZW
 Author: XueLiren
 Author-email: liren1029@gmail.com
 Maintainer: XueLiren
 Maintainer-email: liren1029@gmail.com
 License: Apache Software License 2.0
@@ -27,20 +27,17 @@
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
 # 欢迎使用 Python中文库（PyZW）
 ***
-![PyPI version](https://img.shields.io/pypi/v/pytest-pyzw.svg)
-![Python versions](https://img.shields.io/pypi/pyversions/pytest-pyzw.svg)
-![See Build Status on AppVeyor](https://ci.appveyor.com/api/projects/status/github/XueLiren/pytest-pyzw?branch=master)
+![PyPI version](https://img.shields.io/pypi/v/pytest-pyzw.svg) ![Python versions](https://img.shields.io/pypi/pyversions/pytest-pyzw.svg) ![See Build Status on AppVeyor](https://ci.appveyor.com/api/projects/status/github/XueLiren/pytest-pyzw?branch=master)
 
-&emsp;&emsp;Python中文库（PyZW）是基于Python标准库和诸多第三方库再次封装的中文模块，其函数命令超过1000个，涵盖了人工智能、键鼠操作、找图找色、
-网页自动化、手机自动化、OCR、YOLO、OpenCV、Word文档、Excel表格、PPT演示等多个领域。封装目的仅仅是为了将英文内容翻译成中文，从而使得生活、工作语言是中文的人群也能很好地学习、使用Python，享受编程带来的便利与乐趣！
+&emsp;&emsp;Python中文库（PyZW）是基于Python标准库和诸多第三方库再次封装的中文模块，其函数命令超过1000个，涵盖了人工智能、键鼠操作、找图找色、网页自动化、手机自动化、OCR、YOLO、OpenCV、Word文档、Excel表格、PPT演示等多个领域。封装目的仅仅是为了将英文内容翻译成中文，从而使得生活、工作语言是中文的人群也能很好地学习、使用Python，享受编程带来的便利与乐趣！
 
 ***
 ## Features
 
 * TODO
 ***
 ## Requirements
@@ -76,26 +73,23 @@
 
 `PyPI`: https://pypi.org/project
 
 ***
 ## 常见问题
 ### 学编程，到底要不要学英语？
 
-&emsp;&emsp;常说的“学编程，先学英语”，不是指需要很好的英语水平才能写代码，而是由于人工智能、深度学习、神经网络、目标检测等最新的前沿技术都是国外团队开发出来的，
-我们不得不先学他们使用的语言——英语，才能更好地学习他们发表的文档资料，与他们交流问题以及应用这些技术。
+&emsp;&emsp;常说的“学编程，先学英语”，不是指需要很好的英语水平才能写代码，而是由于人工智能、深度学习、神经网络、目标检测等最新的前沿技术都是国外团队开发出来的，我们不得不先学他们使用的语言——英语，才能更好地学习他们发表的文档资料，与他们交流问题以及应用这些技术。
 
 &emsp;&emsp;所以，如果你的目标是掌握各类前沿技术，那必须学好英语；如果你的目标只是实现传统的办公自动化、游戏自动化，那不需要学英语，因为这些传统的编程技术在国内各个平台上已经有了足够多的中文资料供大家学习。
 
 
 ### 使用中文编程，会不会很丢脸？被嘲笑？
 
-&emsp;&emsp;编程从初期的机器语言，到早期的汇编语言，再到如今的各类高级语言，以及现在提出的AI编程，这一路都是朝着“更加符合自然语言”的方向发展的，而使用中文编程是朝着“更加符合中国人自然语言”的方向发展，
-这个方向是正确无疑的。革命先烈撬动了核武霸权，如今人民币可以撬动美元霸权，有朝一日中文也一定能撬动英文霸权。中文编程与汉字简化一样对国民科技教育普及有重大意义。
+&emsp;&emsp;编程从初期的机器语言，到早期的汇编语言，再到如今的各类高级语言，以及现在提出的AI编程，这一路都是朝着“更加符合自然语言”的方向发展的，而使用中文编程是朝着“更加符合中国人自然语言”的方向发展，这个方向是正确无疑的。革命先烈撬动了核武霸权，如今人民币可以撬动美元霸权，有朝一日中文也一定能撬动英文霸权。中文编程与汉字简化一样对国民科技教育普及有重大意义。
 
-&emsp;&emsp;无论中文编程、英文编程还是使用其他国家的语言编程，最终都会被替换为“0”和“1”组成的机器语言，中文、英文都相当于给机器语言穿了一件外套，如果有人非说英文外套就是比中文外套好，
-国外的月亮就是比国内的月亮圆，这是不对的。
+&emsp;&emsp;无论中文编程、英文编程还是使用其他国家的语言编程，最终都会被替换为“0”和“1”组成的机器语言，中文、英文都相当于给机器语言穿了一件外套，如果有人非说英文外套就是比中文外套好，国外的月亮就是比国内的月亮圆，这是不对的。
 
 &emsp;&emsp;所以，中文编程不落后、不丢脸，是符合编程语言发展方向的，不应该被嘲笑。而实现不了需求、写不出功能的编程人，即使英语专八，也是丢脸的，但不应该被嘲笑。无论何时何事，我们都不应该嘲笑别人。
 
+
 ### 关于 PyZW 的争议
-&emsp;&emsp;难免有人会说，英文是给机器语言穿一件外套，那 PyZW 这个中文库是穿了两件外套。其实，是可以从源码上进行修改，使得 PyZW 也只穿一件外套的。之所以坚持如此，原因有三：
-一是尊重原作者的贡献；二是敬畏国外技术领先国内；三是警醒我辈编程人任重而道远。
+&emsp;&emsp;难免有人会说，英文是给机器语言穿一件外套，那 PyZW 这个中文库是穿了两件外套。其实，是可以从源码上进行修改，使得 PyZW 也只穿一件外套的。之所以坚持如此，原因有三：一是尊重原作者的贡献；二是敬畏国外技术领先国内；三是警醒我辈编程人任重而道远。
```

### Comparing `pyzw-0.0.3/pyzw.egg-info/SOURCES.txt` & `pyzw-0.0.4/pyzw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyzw-0.0.3/setup.py` & `pyzw-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding='utf-8').read()
 
 
 setup(
     name='pyzw',
-    version='0.0.3',
+    version='0.0.4',
     author='XueLiren',
     author_email='liren1029@gmail.com',
     maintainer='XueLiren',
     maintainer_email='liren1029@gmail.com',
     license='Apache Software License 2.0',
     keywords="中文编程 ",
     url='https://github.com/XueLiren/PyZW',
```

