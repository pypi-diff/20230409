# Comparing `tmp/TerminalPrinter-2.0.0.tar.gz` & `tmp/TerminalPrinter-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/TerminalPrinter-2.0.0.tar", last modified: Fri Apr  7 15:04:45 2023, max compression
+gzip compressed data, was "dist/TerminalPrinter-2.1.0.tar", last modified: Sun Apr  9 00:38:39 2023, max compression
```

## Comparing `TerminalPrinter-2.0.0.tar` & `TerminalPrinter-2.1.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-07 15:04:45.000000 TerminalPrinter-2.0.0/
--rw-r--r--   0 hellflame   (501) staff       (20)      959 2023-04-07 15:04:45.000000 TerminalPrinter-2.0.0/PKG-INFO
--rw-r--r--   0 hellflame   (501) staff       (20)     1077 2021-05-18 14:35:42.000000 TerminalPrinter-2.0.0/LICENSE
-drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-07 15:04:45.000000 TerminalPrinter-2.0.0/printer/
--rw-r--r--   0 hellflame   (501) staff       (20)     4131 2023-04-06 23:49:58.000000 TerminalPrinter-2.0.0/printer/run.py
--rw-r--r--   0 hellflame   (501) staff       (20)      105 2023-04-07 00:01:41.000000 TerminalPrinter-2.0.0/printer/version.py
--rw-r--r--   0 hellflame   (501) staff       (20)     6542 2023-04-07 00:00:47.000000 TerminalPrinter-2.0.0/printer/painter.py
--rw-r--r--   0 hellflame   (501) staff       (20)     2523 2023-04-07 15:03:33.000000 TerminalPrinter-2.0.0/printer/resource.py
--rw-r--r--   0 hellflame   (501) staff       (20)        0 2021-05-18 14:35:43.000000 TerminalPrinter-2.0.0/printer/__init__.py
--rw-r--r--   0 hellflame   (501) staff       (20)    17831 2021-05-18 14:35:43.000000 TerminalPrinter-2.0.0/printer/http.py
-drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-07 15:04:45.000000 TerminalPrinter-2.0.0/TerminalPrinter.egg-info/
--rw-r--r--   0 hellflame   (501) staff       (20)      959 2023-04-07 15:04:45.000000 TerminalPrinter-2.0.0/TerminalPrinter.egg-info/PKG-INFO
--rw-r--r--   0 hellflame   (501) staff       (20)      395 2023-04-07 15:04:45.000000 TerminalPrinter-2.0.0/TerminalPrinter.egg-info/SOURCES.txt
--rw-r--r--   0 hellflame   (501) staff       (20)       51 2023-04-07 15:04:45.000000 TerminalPrinter-2.0.0/TerminalPrinter.egg-info/entry_points.txt
--rw-r--r--   0 hellflame   (501) staff       (20)        7 2023-04-07 15:04:45.000000 TerminalPrinter-2.0.0/TerminalPrinter.egg-info/requires.txt
--rw-r--r--   0 hellflame   (501) staff       (20)        8 2023-04-07 15:04:45.000000 TerminalPrinter-2.0.0/TerminalPrinter.egg-info/top_level.txt
--rw-r--r--   0 hellflame   (501) staff       (20)        1 2023-04-07 15:04:45.000000 TerminalPrinter-2.0.0/TerminalPrinter.egg-info/dependency_links.txt
--rw-r--r--   0 hellflame   (501) staff       (20)       52 2021-05-18 14:35:42.000000 TerminalPrinter-2.0.0/MANIFEST.in
--rw-r--r--   0 hellflame   (501) staff       (20)     8012 2021-05-18 15:51:42.000000 TerminalPrinter-2.0.0/README.md
--rw-r--r--   0 hellflame   (501) staff       (20)      478 2021-05-18 14:35:42.000000 TerminalPrinter-2.0.0/CHANGES.txt
--rw-r--r--   0 hellflame   (501) staff       (20)     1186 2023-04-06 23:51:05.000000 TerminalPrinter-2.0.0/setup.py
--rw-r--r--   0 hellflame   (501) staff       (20)       38 2023-04-07 15:04:45.000000 TerminalPrinter-2.0.0/setup.cfg
+drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/
+-rw-r--r--   0 hellflame   (501) staff       (20)      959 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/PKG-INFO
+-rw-r--r--   0 hellflame   (501) staff       (20)     1077 2021-05-18 14:35:42.000000 TerminalPrinter-2.1.0/LICENSE
+drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/printer/
+-rw-r--r--   0 hellflame   (501) staff       (20)     4265 2023-04-09 00:20:29.000000 TerminalPrinter-2.1.0/printer/run.py
+-rw-r--r--   0 hellflame   (501) staff       (20)      105 2023-04-09 00:36:47.000000 TerminalPrinter-2.1.0/printer/version.py
+-rw-r--r--   0 hellflame   (501) staff       (20)     6542 2023-04-07 00:00:47.000000 TerminalPrinter-2.1.0/printer/painter.py
+-rw-r--r--   0 hellflame   (501) staff       (20)     2523 2023-04-07 15:03:33.000000 TerminalPrinter-2.1.0/printer/resource.py
+-rw-r--r--   0 hellflame   (501) staff       (20)        0 2021-05-18 14:35:43.000000 TerminalPrinter-2.1.0/printer/__init__.py
+-rw-r--r--   0 hellflame   (501) staff       (20)      589 2023-04-09 00:27:18.000000 TerminalPrinter-2.1.0/printer/utils.py
+-rw-r--r--   0 hellflame   (501) staff       (20)    17831 2021-05-18 14:35:43.000000 TerminalPrinter-2.1.0/printer/http.py
+drwxr-xr-x   0 hellflame   (501) staff       (20)        0 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/TerminalPrinter.egg-info/
+-rw-r--r--   0 hellflame   (501) staff       (20)      959 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/TerminalPrinter.egg-info/PKG-INFO
+-rw-r--r--   0 hellflame   (501) staff       (20)      412 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/TerminalPrinter.egg-info/SOURCES.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)       51 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/TerminalPrinter.egg-info/entry_points.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)        7 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/TerminalPrinter.egg-info/requires.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)        8 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/TerminalPrinter.egg-info/top_level.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)        1 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/TerminalPrinter.egg-info/dependency_links.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)       52 2021-05-18 14:35:42.000000 TerminalPrinter-2.1.0/MANIFEST.in
+-rw-r--r--   0 hellflame   (501) staff       (20)     8153 2023-04-09 00:35:29.000000 TerminalPrinter-2.1.0/README.md
+-rw-r--r--   0 hellflame   (501) staff       (20)      478 2021-05-18 14:35:42.000000 TerminalPrinter-2.1.0/CHANGES.txt
+-rw-r--r--   0 hellflame   (501) staff       (20)     1186 2023-04-06 23:51:05.000000 TerminalPrinter-2.1.0/setup.py
+-rw-r--r--   0 hellflame   (501) staff       (20)       38 2023-04-09 00:38:39.000000 TerminalPrinter-2.1.0/setup.cfg
```

### Comparing `TerminalPrinter-2.0.0/PKG-INFO` & `TerminalPrinter-2.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: TerminalPrinter
-Version: 2.0.0
+Version: 2.1.0
 Summary: 终端图片、文字生成器
 Home-page: https://github.com/hellflame/terminal_printer
 Author: hellflame
 Author-email: hellflamedly@gmail.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `TerminalPrinter-2.0.0/LICENSE` & `TerminalPrinter-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TerminalPrinter-2.0.0/printer/run.py` & `TerminalPrinter-2.1.0/printer/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # coding=utf8
 
 import os
 import argparse
 
-from printer.version import __url__, __version__
+from printer.version import __url__
 from printer.painter import MESS_FILTERS, FONT_LIST, FONT_DIR, \
     FONT_URL, make_terminal_img, text_drawer, get_img
 from printer.resource import font_handle
+from printer.utils import print_version, print_debug
 
 __all__ = ['parser']
 
 
 def command(args, parse):
+    if args.debug:
+        print_debug(args)
     if args.init:
         font_handle(FONT_DIR, FONT_URL)
     elif args.version:
-        print("TerminalPrinter v{}".format(__version__))
+        print_version()
     elif args.picture:
         pic_path = args.picture
         if os.path.exists(pic_path) and os.path.isfile(pic_path):
             print(make_terminal_img(
                 get_img(pic_path, gray=args.gray),
                 filter_type=args.filter, width=args.width, height=args.height,
                 dye=args.color, reverse=args.reverse, keep_ratio=args.keep_ratio,
@@ -65,14 +68,15 @@
             if os.path.exists(s):
                 return s
             raise argparse.ArgumentTypeError("字体路径不存在，请检查路径或使用数字")
 
     basic = parse.add_argument_group("basics")
     basic.add_argument("-i", "--init", action="store_true", help="初始化程序，下载字体")
     basic.add_argument("-v", '--version', action="store_true", help="输出版本信息")
+    basic.add_argument("--debug", action="store_true", help="输出调试信息")
 
     picture = parse.add_argument_group("pictures")
     picture.add_argument("picture", nargs="?", help="可选的图片")
     picture.add_argument("-kr", '--keep-ratio', action="store_true", help="保持图片比例")
 
     text = parse.add_argument_group("text")
     text.add_argument("-t", '--text', default="HellFlame", help="设置将要处理的文本内容，默认为 HellFlame")
```

### Comparing `TerminalPrinter-2.0.0/printer/painter.py` & `TerminalPrinter-2.1.0/printer/painter.py`

 * *Files identical despite different names*

### Comparing `TerminalPrinter-2.0.0/printer/resource.py` & `TerminalPrinter-2.1.0/printer/resource.py`

 * *Files identical despite different names*

### Comparing `TerminalPrinter-2.0.0/printer/http.py` & `TerminalPrinter-2.1.0/printer/http.py`

 * *Files identical despite different names*

### Comparing `TerminalPrinter-2.0.0/TerminalPrinter.egg-info/PKG-INFO` & `TerminalPrinter-2.1.0/TerminalPrinter.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: TerminalPrinter
-Version: 2.0.0
+Version: 2.1.0
 Summary: 终端图片、文字生成器
 Home-page: https://github.com/hellflame/terminal_printer
 Author: hellflame
 Author-email: hellflamedly@gmail.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: UNKNOWN
```

### Comparing `TerminalPrinter-2.0.0/README.md` & `TerminalPrinter-2.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,61 +18,66 @@
 
 ### 使用
 
 ```bash
 $ terminalprint
 ```
 
-以上命令，将输出默认的字符图到终端(命令太长？为什么不用*tab*)
+以上命令，将输出默认的字符图到终端(命令太长？可使用用 *tab* 进行自动补全)
 
 ![](./images/sample.png)
 
 (分辨率较高的图片可能要花点时间来生成了)
 
 #### i. 帮助信息
 
 ```bash
 $ terminalprint -h
 ```
 
 得到类似输出:
 
 ```bash
-usage: terminalprint [-h] [-i] [-v] [-kr] [-t TEXT] [-c i] [-g] [-F path] [-r]
-                     [-W WIDTH] [-H HEIGHT] [-f i]
-                     [picture]
+usage: run.py [-h] [-i] [-v] [--debug] [-kr] [-t TEXT] [-c i] [-g] [-F path]
+              [-r] [-W w] [-H h] [-f i]
+              [picture]
 
 Terminal Printer
 
 optional arguments:
   -h, --help            show this help message and exit
+
 basics:
   -i, --init            初始化程序，下载字体
   -v, --version         输出版本信息
+  --debug               输出调试信息
+
 pictures:
   picture               可选的图片
   -kr, --keep-ratio     保持图片比例
+
 text:
   -t TEXT, --text TEXT  设置将要处理的文本内容，默认为 HellFlame
   -c i, --color i       设置颜色
   -g, --gray            图像转换为灰度图(若指定图)
   -F path, --font path  设置书写字体
   -r, --reverse         反色(对彩色输出无效)
+
 common:
-  -W WIDTH, --width WIDTH
-                        设置输出宽度，需要与高度一起设置
-  -H HEIGHT, --height HEIGHT
-                        设置输出高度，需要与宽度一起设置
+  -W w, --width w       设置输出宽度，需要与高度一起设置
+  -H h, --height h      设置输出高度，需要与宽度一起设置
   -f i, --filter i      设置打印填充方式
 
-初次使用，需要初始化字体下载
-执行 terminalprint -i 初始化
-更多帮助信息请访问: https://github.com/hellflame/terminal_printer
+首次进行文字处理
+需要执行 terminalprint -i 初始化或指定字体
+更多帮助信息请参考: https://github.com/hellflame/terminal_printer
 ```
 
+> v2.1.0 新增 `--debug` 参数，可与其他命令一起使用，输出调试信息
+
 #### ii. 版本信息
 
 ```bash
 $ terminalprint -v # terminalprint --version
 ```
 
 #### iii. 初始化字体库
@@ -237,10 +242,18 @@
 
   修复带透明度图片输出bug
 
 - v1.6.0
 
   兼容py3下面的问题
 
+- v2.0.0
+
+  易用性更新
+
+- v2.1.0
+
+  新增调试入口
+
 ------
 
 嗯，以上，Just For Fun!
```

### Comparing `TerminalPrinter-2.0.0/setup.py` & `TerminalPrinter-2.1.0/setup.py`

 * *Files identical despite different names*

