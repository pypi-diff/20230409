# Comparing `tmp/pohan-0.0.2.tar.gz` & `tmp/pohan-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pohan-0.0.2.tar", last modified: Thu Apr  6 14:36:58 2023, max compression
+gzip compressed data, was "pohan-0.0.3.tar", last modified: Sun Apr  9 05:48:11 2023, max compression
```

## Comparing `pohan-0.0.2.tar` & `pohan-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 14:36:58.695425 pohan-0.0.2/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 pohan-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2019 2023-04-06 14:36:58.695425 pohan-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1494 2023-04-05 16:44:51.000000 pohan-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 14:36:58.648331 pohan-0.0.2/pohan/
--rw-rw-rw-   0        0        0       29 2023-04-05 16:47:11.000000 pohan-0.0.2/pohan/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:36:58.683441 pohan-0.0.2/pohan/api/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pohan-0.0.2/pohan/api/__init__.py
--rw-rw-rw-   0        0        0      251 2023-04-06 14:36:34.000000 pohan-0.0.2/pohan/api/ood.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:36:58.685426 pohan-0.0.2/pohan/lib/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pohan-0.0.2/pohan/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:36:58.680625 pohan-0.0.2/pohan.egg-info/
--rw-rw-rw-   0        0        0     2019 2023-04-06 14:36:58.000000 pohan-0.0.2/pohan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-04-06 14:36:58.000000 pohan-0.0.2/pohan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 14:36:58.000000 pohan-0.0.2/pohan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-05 16:47:39.000000 pohan-0.0.2/pohan.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-04-06 14:36:58.000000 pohan-0.0.2/pohan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-06 14:36:58.000000 pohan-0.0.2/pohan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      700 2023-04-06 14:36:58.697423 pohan-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 pohan-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 14:36:58.694426 pohan-0.0.2/tests/
--rw-rw-rw-   0        0        0      181 2023-04-05 16:44:51.000000 pohan-0.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0      386 2023-04-06 14:33:25.000000 pohan-0.0.2/tests/test_pohan.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:48:11.807372 pohan-0.0.3/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 pohan-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2923 2023-04-09 05:48:11.807372 pohan-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2400 2023-04-08 15:58:00.000000 pohan-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 05:48:11.727238 pohan-0.0.3/pohan/
+-rw-rw-rw-   0        0        0       25 2023-04-07 14:38:11.000000 pohan-0.0.3/pohan/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:48:11.783367 pohan-0.0.3/pohan/api/
+-rw-rw-rw-   0        0        0       15 2023-04-07 16:46:51.000000 pohan-0.0.3/pohan/api/__init__.py
+-rw-rw-rw-   0        0        0      276 2023-04-09 05:45:05.000000 pohan-0.0.3/pohan/api/普通话.py
+-rw-rw-rw-   0        0        0      231 2023-04-07 14:40:42.000000 pohan-0.0.3/pohan/api/重庆话.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:48:11.787365 pohan-0.0.3/pohan/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pohan-0.0.3/pohan/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:48:11.756368 pohan-0.0.3/pohan.egg-info/
+-rw-rw-rw-   0        0        0     2923 2023-04-09 05:48:11.000000 pohan-0.0.3/pohan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-04-09 05:48:11.000000 pohan-0.0.3/pohan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 05:48:11.000000 pohan-0.0.3/pohan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-07 14:19:04.000000 pohan-0.0.3/pohan.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-04-09 05:48:11.000000 pohan-0.0.3/pohan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      688 2023-04-09 05:48:11.811370 pohan-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 pohan-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 05:48:11.804368 pohan-0.0.3/tests/
+-rw-rw-rw-   0        0        0      181 2023-04-05 16:44:51.000000 pohan-0.0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      392 2023-04-07 14:16:56.000000 pohan-0.0.3/tests/test_pohan.py
```

### Comparing `pohan-0.0.2/LICENSE` & `pohan-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pohan-0.0.2/PKG-INFO` & `pohan-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,61 @@
-Metadata-Version: 2.1
-Name: pohan
-Version: 0.0.2
-Summary: pip install pohan
-Home-page: https://www.python-office.com/
-Author: CoderWanFeng
-Author-email: 1957875073@qq.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/CoderWanFeng/pohan/issues
-Project-URL: Documentation, https://github.com/CoderWanFeng/pohan/blob/master/README.md
-Project-URL: Source Code, https://github.com/CoderWanFeng/pohan
-Platform: any
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 <p align="center">
 	👉 <a target="_blank" href="https://www.python-office.com/">项目官网：https://www.python-office.com/</a> 👈
 </p>
 <p align="center">
 	👉 <a target="_blank" href="https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-office.jpg">本开源项目的交流群</a> 👈
 </p>
 
 
 
 -------------------------------------------------------------------------------
 
-
 ## 📚简介
 
 
-pohan是查看第三方库下载数据的小工具。
+pohan是汇集了普通话和各地方言的中文编程Python库。
 
 -------------------------------------------------------------------------------
 
 ## 📦安装
 
 ### 🍊pip 自动下载&更新
 
-已同步到清华镜像
+已同步到阿里镜像
 
 ```
 pip install -i https://mirrors.aliyun.com/pypi/simple/ pohan -U
 ```
 
 
 -------------------------------------------------------------------------------
 
 ## 📝功能
 
 [📘官网：https://www.python-office.com/](https://www.python-office.com/)
 
 参考资料：
 
-- https://github.com/hugovk/pypistats
-- https://github.com/CoderWanFeng/pohan
+- 本来想参考这里面的做法，结果发现不可行：https://www.bilibili.com/video/BV1SU4y1C7L9
+- 发现了周蟒的资料：https://cloud.tencent.com/developer/news/377312
+- 周蟒的GitHub：https://github.com/gasolin/zhpy
 ### 🐞提供bug反馈或建议
 
-提交问题反馈时，请务必填写和python-office代码本身有关的问题，不进行有关python学习，甚至是个人练习的知识答疑和讨论。
+提交问题反馈时，请务必填写和 **pohan** 代码本身有关的问题。
+
+- 提交Bug的链接👉[Github issue](https://github.com/CoderWanFeng/pohan/issues)
 
-- [Github issue](https://github.com/CoderWanFeng/wftools/issues)
+- 如果想进行有关python入门学习，或者是个人练习的知识答疑和讨论，请加读者交流群👇[扫码](http://www.python4office.cn/wechat-group/)
+
+![CoderWanFeng](https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-office-qr.jpg)
 
 -------------------------------------------------------------------------------
 
 
 ## 📌联系作者
 
+你好，我是程序员晚枫，C++程序员，业余时间做了一些好玩的开源项目。我的B站/小红书/知乎/抖音/公众号，都叫：程序员晚枫请多多点赞支持~
 
-![CoderWanFeng](https://python-office-1300615378.cos.ap-chongqing.myqcloud.com/python-office-qr.jpg)
+- [开源中国推荐：python-office自动化办公，每个功能只需一行代码，做到了真正的开箱即用。](https://mp.weixin.qq.com/s/d2m7xYCLXF8QUlr-5sSuPA)
+- [又一个微信聊天机器人发布了，人人可用！不需要网页版微信](https://www.bilibili.com/video/BV1Xa411u7yU)
+- [3大措施，整治程序员高薪现象！大快人心，人人有责](https://www.bilibili.com/video/BV1sd4y1c7T9)
```

### Comparing `pohan-0.0.2/setup.cfg` & `pohan-0.0.3/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f68 616e 0d0a 7665 7273 696f   = pohan..versio
-00000020: 6e20 3d20 302e 302e 320d 0a64 6573 6372  n = 0.0.2..descr
+00000020: 6e20 3d20 302e 302e 330d 0a64 6573 6372  n = 0.0.3..descr
 00000030: 6970 7469 6f6e 203d 2070 6970 2069 6e73  iption = pip ins
 00000040: 7461 6c6c 2070 6f68 616e 0d0a 6c6f 6e67  tall pohan..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
@@ -29,16 +29,15 @@
 000001c0: 6d61 7374 6572 2f52 4541 444d 452e 6d64  master/README.md
 000001d0: 0d0a 0953 6f75 7263 6520 436f 6465 203d  ...Source Code =
 000001e0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 000001f0: 636f 6d2f 436f 6465 7257 616e 4665 6e67  com/CoderWanFeng
 00000200: 2f70 6f68 616e 0d0a 0d0a 5b6f 7074 696f  /pohan....[optio
 00000210: 6e73 5d0d 0a70 6163 6b61 6765 7320 3d20  ns]..packages = 
 00000220: 6669 6e64 3a0d 0a69 6e73 7461 6c6c 5f72  find:..install_r
-00000230: 6571 7569 7265 7320 3d20 0d0a 0970 7970  equires = ...pyp
-00000240: 6973 7461 7473 0d0a 7079 7468 6f6e 5f72  istats..python_r
-00000250: 6571 7569 7265 7320 3d20 3e3d 332e 360d  equires = >=3.6.
-00000260: 0a69 6e63 6c75 6465 5f70 6163 6b61 6765  .include_package
-00000270: 5f64 6174 6120 3d20 5472 7565 0d0a 7a69  _data = True..zi
-00000280: 705f 7361 6665 203d 2046 616c 7365 0d0a  p_safe = False..
-00000290: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-000002a0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-000002b0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000230: 6571 7569 7265 7320 3d20 0d0a 7079 7468  equires = ..pyth
+00000240: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
+00000250: 332e 360d 0a69 6e63 6c75 6465 5f70 6163  3.6..include_pac
+00000260: 6b61 6765 5f64 6174 6120 3d20 5472 7565  kage_data = True
+00000270: 0d0a 7a69 705f 7361 6665 203d 2046 616c  ..zip_safe = Fal
+00000280: 7365 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  se....[egg_info]
+00000290: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
+000002a0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
```

