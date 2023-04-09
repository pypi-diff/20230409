# Comparing `tmp/Rickrack-2.7.25.tar.gz` & `tmp/Rickrack-2.7.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Rickrack-2.7.25.tar", last modified: Fri Mar 17 13:18:24 2023, max compression
+gzip compressed data, was "dist\Rickrack-2.7.26.tar", last modified: Sun Apr  9 10:14:15 2023, max compression
```

## Comparing `Rickrack-2.7.25.tar` & `Rickrack-2.7.26.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-17 13:18:24.000000 Rickrack-2.7.25/
--rw-rw-rw-   0        0        0       30 2023-03-17 13:18:23.000000 Rickrack-2.7.25/MANIFEST.in
--rw-rw-rw-   0        0        0    19155 2023-03-17 13:18:24.000000 Rickrack-2.7.25/PKG-INFO
--rw-rw-rw-   0        0        0    15877 2023-03-17 13:18:23.000000 Rickrack-2.7.25/README.md
-drwxrwxrwx   0        0        0        0 2023-03-17 13:18:24.000000 Rickrack-2.7.25/rickrack/
--rw-rw-rw-   0        0        0    33878 2023-03-17 13:18:23.000000 Rickrack-2.7.25/rickrack/color.py
--rw-rw-rw-   0        0        0     9871 2023-02-15 08:24:42.000000 Rickrack-2.7.25/rickrack/result.py
--rw-rw-rw-   0        0        0    34412 2023-03-17 10:18:24.000000 Rickrack-2.7.25/rickrack/rickrack.py
--rw-rw-rw-   0        0        0      600 2023-01-09 01:58:26.000000 Rickrack-2.7.25/rickrack/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-17 13:18:24.000000 Rickrack-2.7.25/Rickrack.egg-info/
--rw-rw-rw-   0        0        0        1 2023-03-17 13:18:23.000000 Rickrack-2.7.25/Rickrack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2023-03-17 13:18:23.000000 Rickrack-2.7.25/Rickrack.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0    19155 2023-03-17 13:18:23.000000 Rickrack-2.7.25/Rickrack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-03-17 13:18:23.000000 Rickrack-2.7.25/Rickrack.egg-info/requires.txt
--rw-rw-rw-   0        0        0      303 2023-03-17 13:18:23.000000 Rickrack-2.7.25/Rickrack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-03-17 13:18:23.000000 Rickrack-2.7.25/Rickrack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-17 13:18:24.000000 Rickrack-2.7.25/setup.cfg
--rw-rw-rw-   0        0        0     2076 2023-03-17 13:18:23.000000 Rickrack-2.7.25/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 10:14:15.000000 Rickrack-2.7.26/
+-rw-rw-rw-   0        0        0       30 2023-04-09 10:14:14.000000 Rickrack-2.7.26/MANIFEST.in
+-rw-rw-rw-   0        0        0    16391 2023-04-09 10:14:15.000000 Rickrack-2.7.26/PKG-INFO
+-rw-rw-rw-   0        0        0    13401 2023-04-09 10:14:14.000000 Rickrack-2.7.26/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 10:14:15.000000 Rickrack-2.7.26/rickrack/
+-rw-rw-rw-   0        0        0    33878 2023-04-09 10:14:14.000000 Rickrack-2.7.26/rickrack/color.py
+-rw-rw-rw-   0        0        0     9994 2023-04-07 06:01:22.000000 Rickrack-2.7.26/rickrack/result.py
+-rw-rw-rw-   0        0        0    34745 2023-04-07 13:03:47.000000 Rickrack-2.7.26/rickrack/rickrack.py
+-rw-rw-rw-   0        0        0      600 2023-01-09 01:58:26.000000 Rickrack-2.7.26/rickrack/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 10:14:15.000000 Rickrack-2.7.26/Rickrack.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-09 10:14:15.000000 Rickrack-2.7.26/Rickrack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      112 2023-04-09 10:14:15.000000 Rickrack-2.7.26/Rickrack.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0    16391 2023-04-09 10:14:15.000000 Rickrack-2.7.26/Rickrack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-04-09 10:14:15.000000 Rickrack-2.7.26/Rickrack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      303 2023-04-09 10:14:15.000000 Rickrack-2.7.26/Rickrack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-04-09 10:14:15.000000 Rickrack-2.7.26/Rickrack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 10:14:15.000000 Rickrack-2.7.26/setup.cfg
+-rw-rw-rw-   0        0        0     2076 2023-04-09 10:14:14.000000 Rickrack-2.7.26/setup.py
```

### Comparing `Rickrack-2.7.25/PKG-INFO` & `Rickrack-2.7.26/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: Rickrack
-Version: 2.7.25
+Version: 2.7.26
 Summary: Generate harmonious colors freely.
 Home-page: https://eigenmiao.github.io/rickrack/
 Author: Eigenmiao
 Author-email: eigenmiao@outlook.com
 License: UNKNOWN
 Description: <div align="center">
         <img width="100%" align="center" src="https://raw.githubusercontent.com/eigenmiao/Rickrack/master/src/main/icons/logo_long.png" alt="Rickrack">
         <br/><br/>
         Rickrack<br/>焰火十二卷<br/> ----- ----- ----- ----- ----- ----- ----- ----- <br/>
         Generate Harmonious Colors Freely.<br/>自由自在生成和谐色彩。
         <br/><br/>
-        [<a href="https://eigenmiao.com/yanhuo/zh.html">中文</a>] | [<a href="https://eigenmiao.com/yanhuo/en.html">English</a>] | [<a href="https://eigenmiao.com/yanhuo/ja.html">日本語</a>]
+        [<a href="https://eigenmiao.com/yanhuo/">中文</a>] | [<a href="https://eigenmiao.com/rickrack/">English</a>]
         <br/><br/>
         </div>
         
         # Rickrack
-        Rickrack (**R**e**a**l-t**i**me **C**olor **K**it) is a free and user-friendly color editor. It is designed to generate a set of harmonious colors from the color wheel or other places. You can share these colors with your friends, or apply them into your creative works.
+        In the age of digital creativity, the color palette has become an indispensable tool for designers. A good color palette can make a design more attractive and coordinated. Rickrack is designed for you if you are looking for an excellent color palette software! Rickrack has various color mixing functions and is suitable for various scenes. Rickrack is easy to use, and more importantly, it's completely free without networking or registration required.
+        
+        Rickrack (**R**e**a**l-t**i**me **C**olor **K**it) is a free and user-friendly color editor. It is designed to generate a set of harmonious colors from the color wheel or other places. You can share these colors with your friends, or apply them into your creative works. What’s more, you can export them into individual files and import them into other softwares such as Adobe Photoshop, GIMP, Krita, Pencil 2D and Clip Studio Paint. Rickrack can run normally on operating systems such as Windows, Linux, and macOS.
         
         # 焰火十二卷
-        焰火十二卷（实时色彩工具箱）是一款免费且实用的色彩编辑器。它可以帮助你从色轮或者其他地方生成一组和谐的色彩。你可以将这些色彩分享给其他人，或者应用到你自己的创作当中。
+        在数字创意的时代，调色板成为了设计师不可或缺的工具。一个好的调色板可以让设计更加有吸引力和协调性。如果你正在寻找一款优秀的调色板软件，那就试试焰火十二卷吧！焰火十二卷具有多种配色功能，适用于多种场景。焰火十二卷简单易上手，更重要的是，它完全免费，无需联网或注册。
+        
+        焰火十二卷（实时色彩工具箱）是一款免费且实用的色彩编辑器。它可以帮助你从色轮或者其他地方生成一组和谐的色彩。你可以将这些色彩分享给其他人，或者应用到你自己的创作当中。此外，你也可以将色彩组或者色彩仓库导出为单独的色彩文档并导入其他软件中（如 Adobe Photoshop、GIMP、Krita、Pencil 2D 以及优动漫 Paint 等）。焰火十二卷可以在 Windows、Linux、macOS 等操作系统上正常运行。
         
         # Table of Content
-        * [Introduction](#introduction)
         * [Feature](#feature)
         * [Demo](#demo)
           * [Basic Functions](#basic-functions)
           * [Reference Colors](#reference-colors)
           * [Color Palettes](#color-palettes)
           * [Export and Import Colors](#export-and-import-colors)
           * [Languages and Settings](#languages-and-settings)
         * [Reviews about Rickrack](#reviews-about-rickrack)
-        * [User Comments](#user-comments)
         * [Information](#information)
           * [Homepage](#homepage)
           * [Repository](#repository)
           * [Author](#author)
           * [Support](#support)
         * [Installation](#installation)
           * [Current Release](#current-release)
@@ -51,25 +53,14 @@
           * [How to Build the Software](#how-to-build-the-software)
           * [How to Build the Module](#how-to-build-the-module)
         * [Copyright](#copyright)
         * [License](#license)
           * [License for Rickrack](#license-for-rickrack)
         * [Acknowledgment](#acknowledgment)
         
-        # Introduction
-        Colors enrich our world and affect our emotions. For artists, they display objects and convey feelings by varied colors in photos, images and drawings. For scientist, they present data by distinguishable colors in figures and graphics. However, the majority of color softwares and websites put restrictions on users, which include the inability to export color palettes into individual files, not providing invocation interfaces, requiring registrations, regional limitations and (or) collecting users' personal information.
-        
-        If you are running into these issues, Rickrack is the perfect solution for you!
-        
-        Rickrack is a free and user-friendly color editor. It is designed to generate a set of harmonious colors from the color wheel or other places. You can share these colors with your friends, or apply them into your creative works. You can store the color sets and color boards in the software, and access them whenever you need. What's more, you can export them into individual files, back them up, share them with others or import them in to other softwares such as Adobe Photoshop, GIMP, Krita, Pencil 2D and Clip Studio Paint. Rickrack, written in PySide2, operates effectively on Windows, Linux and other mainstream operating systems.
-        
-        Rickrack consists of two parts: the Rickrack software and the Rickrack module; the Rickrack software is designed for producing and organizing harmonious colors, and the Rickrack module is utilized for obtaining colors from the software in real-time, along with the plotting of images combined with other modules such as Matplotlib and Turtle.
-        
-        <div align="right"><a href="#table-of-content">[-> Back to TOC <-]</a></div>
-        
         # Feature
         Rickrack has several features:
         * A strong and free color editor.
         * Create a set of colors from the color wheel.
         * Pick-up a set of colors from an image.
         * Generate a color board from the color set.
         * Attach the color set and color board into the depot.
@@ -100,22 +91,14 @@
         |     |     |
         | :---: | :---: |
         | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/204.gif) | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/205.gif) |
         | Convert: gradient palette &harr; fixed palette. | Convert: gradient palette &harr; reference palette. |
         | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/700.gif) | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/701.gif) |
         | Fixed palette: Chinese Traditional Colors. (Color Names: [Copyright (c) China Science Publishing & Media Ltd.](http://zhongguose.com/), Non-Commercial Usage) | Fixed palette: Nippon Traditional Colors. (Color Names: [Copyright (c) PIE BOOKS.](http://nipponcolors.com/), Non-Commercial Usage) |
         
-        ## Export and Import Colors
-        |     |     |
-        | :---: | :---: |
-        | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/704.gif) | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/702.gif) |
-        | Export colors into a Rickrack file. | Export colors into a Adobe swatch file. |
-        | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/705.gif) | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/703.gif) |
-        | Import colors from a Rickrack file. | Import colors from a Adobe swatch file. |
-        
         ## Languages and Settings
         |     |     |
         | :---: | :---: |
         | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/707.gif) | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/706.gif) |
         | Support multiple languages, including Chinese, English, Japanese, German, French, Russian, and so on. (Languages except Chinese and English are translated by [Google Translate](https://translate.google.cn/).) | Support multiple interface themes. |
         
         ## Notice
@@ -128,33 +111,14 @@
         
         > Rickrack is an easy to use desktop app for creating and saving color palettes. It supports many major color palette formats for import and export, and is a great tool for generating color palettes of colors that go well together. -- [TJ FREE @ Youtube](https://www.youtube.com/watch?v=OUnktTCtv3E)
         
         > ... and more!
         
         <div align="right"><a href="#table-of-content">[-> Back to TOC <-]</a></div>
         
-        # User Comments
-        > 作为一个配色软件，它本身的色彩，嗯，足够惊艳...你完全可以信得过作者。 -- User from [Open Source China](https://www.oschina.net/comment/news/231426)
-        
-        > 很棒！是一个不可多得的工具。 -- User from [Bilibili](https://www.bilibili.com/video/BV1VD4y157tX/)
-        
-        > 谢谢分享，说明写的太详细了。 -- User from [Baidu Tieba](https://tieba.baidu.com/p/8253007907)
-        
-        > Thanks a mil! All of my pallette creators were online. This a good offline tool to have with some additional features too. -- User from [Youtube](https://www.youtube.com/watch?v=OUnktTCtv3E)
-        
-        > I don't like online-apps, so this is a huge plus from the get-go. Thanks for sharing this great tool. -- User from [Youtube](https://www.youtube.com/watch?v=OUnktTCtv3E)
-        
-        > Thanks for sharing this! And - did I notice correctly that you are also the author of this software? This looks super exciting, can’t wait to investigate it more! -- User from [Krita Artists](https://krita-artists.org/t/alternatives-to-adobe-color-rickrack/60041)
-        
-        > Hello, your software (the deb package) runs fine on Xubuntu 22.04 and is quite impressive! Thanks for sharing. Next step is to study some tutorials. -- User from [PIXLS.US](https://discuss.pixls.us/t/alternatives-to-adobe-color-rickrack/35997)
-        
-        > ... and more!
-        
-        <div align="right"><a href="#table-of-content">[-> Back to TOC <-]</a></div>
-        
         # Information
         ## Homepage
         https://eigenmiao.com/rickrack/
         
         ## Repository
         https://github.com/eigenmiao/Rickrack
         
@@ -164,24 +128,24 @@
         ## Support
         [Support the Future of Rickrack!](https://afdian.net/a/eigenmiao)
         
         <div align="right"><a href="#table-of-content">[-> Back to TOC <-]</a></div>
         
         # Installation
         ## Current Release
-        The latest preview version is [v2.7.25](https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.25).
+        The latest preview version is [v2.7.26](https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.26).
         
         ## Install Software
         ### Recommend: Install on Windows 10 or 11 via WinGet tool
         ```
         winget install rickrack
         ```
         
         ## Install on other platforms
-        Download Software from [Github](https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.25) or [Sourceforge](https://sourceforge.net/projects/rickrack/files/v2.7.25/). The installation steps are presented in [tutorials](https://eigenmiao.com/2021/12/12/rickrack-tutorial-en-v2.3.4/#Installation).
+        Download Software from [Github](https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.26) or [Sourceforge](https://sourceforge.net/projects/rickrack/files/v2.7.26/). The installation steps are presented in [tutorials](https://eigenmiao.com/2021/12/12/rickrack-tutorial-en-v2.3.4/#Installation).
         
         Here is a [video tutorial](https://www.bilibili.com/video/BV17r4y1L7R6/).
         
         ## Install Module
         Install the latest [Rickrack](https://pypi.org/project/Rickrack/) from PyPI!
         
         ```Bash
@@ -281,15 +245,15 @@
         Rickrack is a free software, which is distributed in the hope that it will be useful, but without any warranty. You can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation. See the [GNU General Public License 3.0 (GPL 3.0)](https://www.gnu.org/licenses/) for more details.
         
         All images, documents and translations in Rickrack [code repository](https://github.com/eigenmiao/Rickrack) are licensed under [Creative Commons Attribution-NonCommercial-ShareAlike License 4.0 (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/) unless stating additionally.
         
         Rickrack default uses [Noto Serif](https://fonts.google.com/specimen/Noto+Serif) ([SC](https://fonts.google.com/specimen/Noto+Serif+SC)) fonts and [Noto Sans](https://fonts.google.com/specimen/Noto+Sans) ([SC](https://fonts.google.com/specimen/Noto+Sans+SC)) fonts for interface display, which are designed by Google and published in website [Google Fonts](https://fonts.google.com/). These fonts are open-sourced under [Apache 2.0](http://www.apache.org/licenses/) and [SIL Open Font License 1.1](http://scripts.sil.org/OFL), respectively.
         
         # Acknowledgment
-        * The Rickrack software is written in [Python](https://www.python.org/), constructed based on [PySide2](https://www.qt.io/qt-for-python) and packed up by [fbs (free edition)](https://build-system.fman.io/).
+        * The Rickrack software is written in [Python](https://www.python.org/), constructed based on [PyQt5](https://www.qt.io/qt-for-python) and packed up by [fbs (free edition)](https://build-system.fman.io/).
         * The localization (l10n) and internationalization (i18n) of Rickrack is based on [Google Translate](https://translate.google.cn/) and [Microsoft Translator](https://cn.bing.com/translator), deployed on [POEditor](https://poeditor.com/join/project?hash=kBeQjfxCES).
         * The code repository is deposited on [Github](https://github.com/eigenmiao/Rickrack) and [Gitee](https://gitee.com/eigenmiao/Rickrack).
         
         <div align="right"><a href="#rickrack">[-> Back to Top <-]</a> <a href="#table-of-content">[-> Back to TOC <-]</a></div>
         
 Keywords: Color-Editor,Color-Picker,Color-Palette,Digital-Palette,Desktop-Application
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,70 +1,59 @@
-Metadata-Version: 2.1 Name: Rickrack Version: 2.7.25 Summary: Generate
+Metadata-Version: 2.1 Name: Rickrack Version: 2.7.26 Summary: Generate
 harmonious colors freely. Home-page: https://eigenmiao.github.io/rickrack/
 Author: Eigenmiao Author-email: eigenmiao@outlook.com License: UNKNOWN
 Description:
                                   [Rickrack]
 
                                    Rickrack
                                 ç°ç«åäºå·
                ----- ----- ----- ----- ----- ----- ----- -----
                       Generate Harmonious Colors Freely.
                       èªç±èªå¨çæåè°è²å½©ã
 
-                      [ä¸­æ] | [English] | [æ¥æ¬èª]
+                             [ä¸­æ] | [English]
 
-# Rickrack Rickrack (**R**e**a**l-t**i**me **C**olor **K**it) is a free and
-user-friendly color editor. It is designed to generate a set of harmonious
-colors from the color wheel or other places. You can share these colors with
-your friends, or apply them into your creative works. # ç°ç«åäºå·
-ç°ç«åäºå·ï¼å®æ¶è²å½©å·¥å·ç®±ï¼æ¯ä¸æ¬¾åè´¹ä¸å®ç¨çè²å½©ç¼è¾å¨ãå®å¯ä»¥å¸®å©ä½ ä»è²è½®æèå¶ä»å°æ¹çæä¸ç»åè°çè²å½©ãä½ å¯ä»¥å°è¿äºè²å½©åäº«ç»å¶ä»äººï¼æèåºç¨å°ä½ èªå·±çåä½å½ä¸­ã
-# Table of Content * [Introduction](#introduction) * [Feature](#feature) *
+# Rickrack In the age of digital creativity, the color palette has become an
+indispensable tool for designers. A good color palette can make a design more
+attractive and coordinated. Rickrack is designed for you if you are looking for
+an excellent color palette software! Rickrack has various color mixing
+functions and is suitable for various scenes. Rickrack is easy to use, and more
+importantly, it's completely free without networking or registration required.
+Rickrack (**R**e**a**l-t**i**me **C**olor **K**it) is a free and user-friendly
+color editor. It is designed to generate a set of harmonious colors from the
+color wheel or other places. You can share these colors with your friends, or
+apply them into your creative works. Whatâs more, you can export them into
+individual files and import them into other softwares such as Adobe Photoshop,
+GIMP, Krita, Pencil 2D and Clip Studio Paint. Rickrack can run normally on
+operating systems such as Windows, Linux, and macOS. # ç°ç«åäºå·
+å¨æ°å­åæçæ¶ä»£ï¼è°è²æ¿æä¸ºäºè®¾è®¡å¸ä¸å¯æç¼ºçå·¥å·ãä¸ä¸ªå¥½çè°è²æ¿å¯ä»¥è®©è®¾è®¡æ´å æå¸å¼åååè°æ§ãå¦æä½ æ­£å¨å¯»æ¾ä¸æ¬¾ä¼ç§çè°è²æ¿è½¯ä»¶ï¼é£å°±è¯è¯ç°ç«åäºå·å§ï¼ç°ç«åäºå·å·æå¤ç§éè²åè½ï¼éç¨äºå¤ç§åºæ¯ãç°ç«åäºå·ç®åæä¸æï¼æ´éè¦çæ¯ï¼å®å®å¨åè´¹ï¼æ éèç½ææ³¨åã
+ç°ç«åäºå·ï¼å®æ¶è²å½©å·¥å·ç®±ï¼æ¯ä¸æ¬¾åè´¹ä¸å®ç¨çè²å½©ç¼è¾å¨ãå®å¯ä»¥å¸®å©ä½ ä»è²è½®æèå¶ä»å°æ¹çæä¸ç»åè°çè²å½©ãä½ å¯ä»¥å°è¿äºè²å½©åäº«ç»å¶ä»äººï¼æèåºç¨å°ä½ èªå·±çåä½å½ä¸­ãæ­¤å¤ï¼ä½ ä¹å¯ä»¥å°è²å½©ç»æèè²å½©ä»åºå¯¼åºä¸ºåç¬çè²å½©ææ¡£å¹¶å¯¼å¥å¶ä»è½¯ä»¶ä¸­ï¼å¦
+Adobe PhotoshopãGIMPãKritaãPencil 2D ä»¥åä¼å¨æ¼« Paint
+ç­ï¼ãç°ç«åäºå·å¯ä»¥å¨ WindowsãLinuxãmacOS
+ç­æä½ç³»ç»ä¸æ­£å¸¸è¿è¡ã # Table of Content * [Feature](#feature) *
 [Demo](#demo) * [Basic Functions](#basic-functions) * [Reference Colors]
 (#reference-colors) * [Color Palettes](#color-palettes) * [Export and Import
 Colors](#export-and-import-colors) * [Languages and Settings](#languages-and-
-settings) * [Reviews about Rickrack](#reviews-about-rickrack) * [User Comments]
-(#user-comments) * [Information](#information) * [Homepage](#homepage) *
-[Repository](#repository) * [Author](#author) * [Support](#support) *
-[Installation](#installation) * [Current Release](#current-release) * [Download
-Software](#download-software) * [Install Software](#install-software) *
-[Install Module](#install-module) * [Usage](#usage) * [How to Use the Software]
-(#how-to-use-the-software) * [How to Use the Module](#how-to-use-the-module) *
-[Development](#development) * [Install Requirement](#install-requirement) *
-[How to Build the Software](#how-to-build-the-software) * [How to Build the
-Module](#how-to-build-the-module) * [Copyright](#copyright) * [License]
-(#license) * [License for Rickrack](#license-for-rickrack) * [Acknowledgment]
-(#acknowledgment) # Introduction Colors enrich our world and affect our
-emotions. For artists, they display objects and convey feelings by varied
-colors in photos, images and drawings. For scientist, they present data by
-distinguishable colors in figures and graphics. However, the majority of color
-softwares and websites put restrictions on users, which include the inability
-to export color palettes into individual files, not providing invocation
-interfaces, requiring registrations, regional limitations and (or) collecting
-users' personal information. If you are running into these issues, Rickrack is
-the perfect solution for you! Rickrack is a free and user-friendly color
-editor. It is designed to generate a set of harmonious colors from the color
-wheel or other places. You can share these colors with your friends, or apply
-them into your creative works. You can store the color sets and color boards in
-the software, and access them whenever you need. What's more, you can export
-them into individual files, back them up, share them with others or import them
-in to other softwares such as Adobe Photoshop, GIMP, Krita, Pencil 2D and Clip
-Studio Paint. Rickrack, written in PySide2, operates effectively on Windows,
-Linux and other mainstream operating systems. Rickrack consists of two parts:
-the Rickrack software and the Rickrack module; the Rickrack software is
-designed for producing and organizing harmonious colors, and the Rickrack
-module is utilized for obtaining colors from the software in real-time, along
-with the plotting of images combined with other modules such as Matplotlib and
-Turtle.
-                                                            [->_Back_to_TOC_<-]
-# Feature Rickrack has several features: * A strong and free color editor. *
-Create a set of colors from the color wheel. * Pick-up a set of colors from an
-image. * Generate a color board from the color set. * Attach the color set and
-color board into the depot. * Import colors from elsewhere and manage them in
-depot. * Export colors and import them into other image processors. * Obtain
-colors through the Python module in real-time. * No function limitations and no
+settings) * [Reviews about Rickrack](#reviews-about-rickrack) * [Information]
+(#information) * [Homepage](#homepage) * [Repository](#repository) * [Author]
+(#author) * [Support](#support) * [Installation](#installation) * [Current
+Release](#current-release) * [Download Software](#download-software) * [Install
+Software](#install-software) * [Install Module](#install-module) * [Usage]
+(#usage) * [How to Use the Software](#how-to-use-the-software) * [How to Use
+the Module](#how-to-use-the-module) * [Development](#development) * [Install
+Requirement](#install-requirement) * [How to Build the Software](#how-to-build-
+the-software) * [How to Build the Module](#how-to-build-the-module) *
+[Copyright](#copyright) * [License](#license) * [License for Rickrack]
+(#license-for-rickrack) * [Acknowledgment](#acknowledgment) # Feature Rickrack
+has several features: * A strong and free color editor. * Create a set of
+colors from the color wheel. * Pick-up a set of colors from an image. *
+Generate a color board from the color set. * Attach the color set and color
+board into the depot. * Import colors from elsewhere and manage them in depot.
+* Export colors and import them into other image processors. * Obtain colors
+through the Python module in real-time. * No function limitations and no
 registration required. * ... and more!
                                                             [->_Back_to_TOC_<-]
 # Demo ## Basic Functions | | | | :---: | :---: | | ![](https://
 raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/000.gif) | ![]
 (https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/
 109.gif) | | Create a set of colors from the color wheel. | Pick-up a set of
 colors from an image. (Image inside: [Copyright (c) 2001 Studio Ghibli](https:/
@@ -84,74 +73,46 @@
 Convert: gradient palette ↔ fixed palette. | Convert: gradient palette ↔
 reference palette. | | ![](https://raw.githubusercontent.com/eigenmiao/
 Rickrack/master/demo/usage/700.gif) | ![](https://raw.githubusercontent.com/
 eigenmiao/Rickrack/master/demo/usage/701.gif) | | Fixed palette: Chinese
 Traditional Colors. (Color Names: [Copyright (c) China Science Publishing &
 Media Ltd.](http://zhongguose.com/), Non-Commercial Usage) | Fixed palette:
 Nippon Traditional Colors. (Color Names: [Copyright (c) PIE BOOKS.](http://
-nipponcolors.com/), Non-Commercial Usage) | ## Export and Import Colors | | | |
-:---: | :---: | | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/
-master/demo/usage/704.gif) | ![](https://raw.githubusercontent.com/eigenmiao/
-Rickrack/master/demo/usage/702.gif) | | Export colors into a Rickrack file. |
-Export colors into a Adobe swatch file. | | ![](https://
-raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/705.gif) | ![]
-(https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/
-703.gif) | | Import colors from a Rickrack file. | Import colors from a Adobe
-swatch file. | ## Languages and Settings | | | | :---: | :---: | | ![](https://
-raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/707.gif) | ![]
-(https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/
-706.gif) | | Support multiple languages, including Chinese, English, Japanese,
-German, French, Russian, and so on. (Languages except Chinese and English are
-translated by [Google Translate](https://translate.google.cn/).) | Support
-multiple interface themes. | ## Notice * The interface display in demo uses
-[LXGWWenKai (SIL Open Font License)](https://lxgw.github.io/2021/01/28/Klee-
-Simpchin/) font.
+nipponcolors.com/), Non-Commercial Usage) | ## Languages and Settings | | | | :
+---: | :---: | | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/
+master/demo/usage/707.gif) | ![](https://raw.githubusercontent.com/eigenmiao/
+Rickrack/master/demo/usage/706.gif) | | Support multiple languages, including
+Chinese, English, Japanese, German, French, Russian, and so on. (Languages
+except Chinese and English are translated by [Google Translate](https://
+translate.google.cn/).) | Support multiple interface themes. | ## Notice * The
+interface display in demo uses [LXGWWenKai (SIL Open Font License)](https://
+lxgw.github.io/2021/01/28/Klee-Simpchin/) font.
                                                             [->_Back_to_TOC_<-]
 # Reviews about Rickrack > All in all, Rickrack is a comprehensive tool for
 anything that requires color work. Experienced users have an exhaustive toolset
 to work with, while a more casual audience can improve the presentation of
 their art by quickly getting color synergy ideas. -- [Robert Condorache @
 Softpedia](https://www.softpedia.com/get/Multimedia/Graphic/Graphic-Others/
 RickRack.shtml) > Rickrack is an easy to use desktop app for creating and
 saving color palettes. It supports many major color palette formats for import
 and export, and is a great tool for generating color palettes of colors that go
 well together. -- [TJ FREE @ Youtube](https://www.youtube.com/
 watch?v=OUnktTCtv3E) > ... and more!
                                                             [->_Back_to_TOC_<-]
-# User Comments >
-ä½ä¸ºä¸ä¸ªéè²è½¯ä»¶ï¼å®æ¬èº«çè²å½©ï¼å¯ï¼è¶³å¤æè³...ä½ å®å¨å¯ä»¥ä¿¡å¾è¿ä½èã
--- User from [Open Source China](https://www.oschina.net/comment/news/231426) >
-å¾æ£ï¼æ¯ä¸ä¸ªä¸å¯å¤å¾çå·¥å·ã -- User from [Bilibili](https://
-www.bilibili.com/video/BV1VD4y157tX/) >
-è°¢è°¢åäº«ï¼è¯´æåçå¤ªè¯¦ç»äºã -- User from [Baidu Tieba](https://
-tieba.baidu.com/p/8253007907) > Thanks a mil! All of my pallette creators were
-online. This a good offline tool to have with some additional features too. -
-- User from [Youtube](https://www.youtube.com/watch?v=OUnktTCtv3E) > I don't
-like online-apps, so this is a huge plus from the get-go. Thanks for sharing
-this great tool. -- User from [Youtube](https://www.youtube.com/
-watch?v=OUnktTCtv3E) > Thanks for sharing this! And - did I notice correctly
-that you are also the author of this software? This looks super exciting,
-canât wait to investigate it more! -- User from [Krita Artists](https://
-krita-artists.org/t/alternatives-to-adobe-color-rickrack/60041) > Hello, your
-software (the deb package) runs fine on Xubuntu 22.04 and is quite impressive!
-Thanks for sharing. Next step is to study some tutorials. -- User from
-[PIXLS.US](https://discuss.pixls.us/t/alternatives-to-adobe-color-rickrack/
-35997) > ... and more!
-                                                            [->_Back_to_TOC_<-]
 # Information ## Homepage https://eigenmiao.com/rickrack/ ## Repository https:/
 /github.com/eigenmiao/Rickrack ## Author [Eigenmiao](mailto:
 eigenmiao@outlook.com) ## Support [Support the Future of Rickrack!](https://
 afdian.net/a/eigenmiao)
                                                             [->_Back_to_TOC_<-]
-# Installation ## Current Release The latest preview version is [v2.7.25]
-(https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.25). ## Install
+# Installation ## Current Release The latest preview version is [v2.7.26]
+(https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.26). ## Install
 Software ### Recommend: Install on Windows 10 or 11 via WinGet tool ``` winget
 install rickrack ``` ## Install on other platforms Download Software from
-[Github](https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.25) or
-[Sourceforge](https://sourceforge.net/projects/rickrack/files/v2.7.25/). The
+[Github](https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.26) or
+[Sourceforge](https://sourceforge.net/projects/rickrack/files/v2.7.26/). The
 installation steps are presented in [tutorials](https://eigenmiao.com/2021/12/
 12/rickrack-tutorial-en-v2.3.4/#Installation). Here is a [video tutorial]
 (https://www.bilibili.com/video/BV17r4y1L7R6/). ## Install Module Install the
 latest [Rickrack](https://pypi.org/project/Rickrack/) from PyPI! ```Bash #
 Install Rickrack. pip install Rickrack # Start the installed software. rickrack
 -d "/PATH/TO/RICKRACK/SOFTWARE" ```
                                                             [->_Back_to_TOC_<-]
@@ -200,15 +161,15 @@
 specimen/Noto+Serif) ([SC](https://fonts.google.com/specimen/Noto+Serif+SC))
 fonts and [Noto Sans](https://fonts.google.com/specimen/Noto+Sans) ([SC](https:
 //fonts.google.com/specimen/Noto+Sans+SC)) fonts for interface display, which
 are designed by Google and published in website [Google Fonts](https://
 fonts.google.com/). These fonts are open-sourced under [Apache 2.0](http://
 www.apache.org/licenses/) and [SIL Open Font License 1.1](http://
 scripts.sil.org/OFL), respectively. # Acknowledgment * The Rickrack software is
-written in [Python](https://www.python.org/), constructed based on [PySide2]
+written in [Python](https://www.python.org/), constructed based on [PyQt5]
 (https://www.qt.io/qt-for-python) and packed up by [fbs (free edition)](https:/
 /build-system.fman.io/). * The localization (l10n) and internationalization
 (i18n) of Rickrack is based on [Google Translate](https://translate.google.cn/
 ) and [Microsoft Translator](https://cn.bing.com/translator), deployed on
 [POEditor](https://poeditor.com/join/project?hash=kBeQjfxCES). * The code
 repository is deposited on [Github](https://github.com/eigenmiao/Rickrack) and
 [Gitee](https://gitee.com/eigenmiao/Rickrack).
```

### Comparing `Rickrack-2.7.25/README.md` & `Rickrack-2.7.26/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 <div align="center">
 <img width="100%" align="center" src="https://raw.githubusercontent.com/eigenmiao/Rickrack/master/src/main/icons/logo_long.png" alt="Rickrack">
 <br/><br/>
 Rickrack<br/>焰火十二卷<br/> ----- ----- ----- ----- ----- ----- ----- ----- <br/>
 Generate Harmonious Colors Freely.<br/>自由自在生成和谐色彩。
 <br/><br/>
-[<a href="https://eigenmiao.com/yanhuo/zh.html">中文</a>] | [<a href="https://eigenmiao.com/yanhuo/en.html">English</a>] | [<a href="https://eigenmiao.com/yanhuo/ja.html">日本語</a>]
+[<a href="https://eigenmiao.com/yanhuo/">中文</a>] | [<a href="https://eigenmiao.com/rickrack/">English</a>]
 <br/><br/>
 </div>
 
 # Rickrack
-Rickrack (**R**e**a**l-t**i**me **C**olor **K**it) is a free and user-friendly color editor. It is designed to generate a set of harmonious colors from the color wheel or other places. You can share these colors with your friends, or apply them into your creative works.
+In the age of digital creativity, the color palette has become an indispensable tool for designers. A good color palette can make a design more attractive and coordinated. Rickrack is designed for you if you are looking for an excellent color palette software! Rickrack has various color mixing functions and is suitable for various scenes. Rickrack is easy to use, and more importantly, it's completely free without networking or registration required.
+
+Rickrack (**R**e**a**l-t**i**me **C**olor **K**it) is a free and user-friendly color editor. It is designed to generate a set of harmonious colors from the color wheel or other places. You can share these colors with your friends, or apply them into your creative works. What’s more, you can export them into individual files and import them into other softwares such as Adobe Photoshop, GIMP, Krita, Pencil 2D and Clip Studio Paint. Rickrack can run normally on operating systems such as Windows, Linux, and macOS.
 
 # 焰火十二卷
-焰火十二卷（实时色彩工具箱）是一款免费且实用的色彩编辑器。它可以帮助你从色轮或者其他地方生成一组和谐的色彩。你可以将这些色彩分享给其他人，或者应用到你自己的创作当中。
+在数字创意的时代，调色板成为了设计师不可或缺的工具。一个好的调色板可以让设计更加有吸引力和协调性。如果你正在寻找一款优秀的调色板软件，那就试试焰火十二卷吧！焰火十二卷具有多种配色功能，适用于多种场景。焰火十二卷简单易上手，更重要的是，它完全免费，无需联网或注册。
+
+焰火十二卷（实时色彩工具箱）是一款免费且实用的色彩编辑器。它可以帮助你从色轮或者其他地方生成一组和谐的色彩。你可以将这些色彩分享给其他人，或者应用到你自己的创作当中。此外，你也可以将色彩组或者色彩仓库导出为单独的色彩文档并导入其他软件中（如 Adobe Photoshop、GIMP、Krita、Pencil 2D 以及优动漫 Paint 等）。焰火十二卷可以在 Windows、Linux、macOS 等操作系统上正常运行。
 
 # Table of Content
-* [Introduction](#introduction)
 * [Feature](#feature)
 * [Demo](#demo)
   * [Basic Functions](#basic-functions)
   * [Reference Colors](#reference-colors)
   * [Color Palettes](#color-palettes)
   * [Export and Import Colors](#export-and-import-colors)
   * [Languages and Settings](#languages-and-settings)
 * [Reviews about Rickrack](#reviews-about-rickrack)
-* [User Comments](#user-comments)
 * [Information](#information)
   * [Homepage](#homepage)
   * [Repository](#repository)
   * [Author](#author)
   * [Support](#support)
 * [Installation](#installation)
   * [Current Release](#current-release)
@@ -43,25 +45,14 @@
   * [How to Build the Software](#how-to-build-the-software)
   * [How to Build the Module](#how-to-build-the-module)
 * [Copyright](#copyright)
 * [License](#license)
   * [License for Rickrack](#license-for-rickrack)
 * [Acknowledgment](#acknowledgment)
 
-# Introduction
-Colors enrich our world and affect our emotions. For artists, they display objects and convey feelings by varied colors in photos, images and drawings. For scientist, they present data by distinguishable colors in figures and graphics. However, the majority of color softwares and websites put restrictions on users, which include the inability to export color palettes into individual files, not providing invocation interfaces, requiring registrations, regional limitations and (or) collecting users' personal information.
-
-If you are running into these issues, Rickrack is the perfect solution for you!
-
-Rickrack is a free and user-friendly color editor. It is designed to generate a set of harmonious colors from the color wheel or other places. You can share these colors with your friends, or apply them into your creative works. You can store the color sets and color boards in the software, and access them whenever you need. What's more, you can export them into individual files, back them up, share them with others or import them in to other softwares such as Adobe Photoshop, GIMP, Krita, Pencil 2D and Clip Studio Paint. Rickrack, written in PySide2, operates effectively on Windows, Linux and other mainstream operating systems.
-
-Rickrack consists of two parts: the Rickrack software and the Rickrack module; the Rickrack software is designed for producing and organizing harmonious colors, and the Rickrack module is utilized for obtaining colors from the software in real-time, along with the plotting of images combined with other modules such as Matplotlib and Turtle.
-
-<div align="right"><a href="#table-of-content">[-> Back to TOC <-]</a></div>
-
 # Feature
 Rickrack has several features:
 * A strong and free color editor.
 * Create a set of colors from the color wheel.
 * Pick-up a set of colors from an image.
 * Generate a color board from the color set.
 * Attach the color set and color board into the depot.
@@ -92,22 +83,14 @@
 |     |     |
 | :---: | :---: |
 | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/204.gif) | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/205.gif) |
 | Convert: gradient palette &harr; fixed palette. | Convert: gradient palette &harr; reference palette. |
 | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/700.gif) | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/701.gif) |
 | Fixed palette: Chinese Traditional Colors. (Color Names: [Copyright (c) China Science Publishing & Media Ltd.](http://zhongguose.com/), Non-Commercial Usage) | Fixed palette: Nippon Traditional Colors. (Color Names: [Copyright (c) PIE BOOKS.](http://nipponcolors.com/), Non-Commercial Usage) |
 
-## Export and Import Colors
-|     |     |
-| :---: | :---: |
-| ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/704.gif) | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/702.gif) |
-| Export colors into a Rickrack file. | Export colors into a Adobe swatch file. |
-| ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/705.gif) | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/703.gif) |
-| Import colors from a Rickrack file. | Import colors from a Adobe swatch file. |
-
 ## Languages and Settings
 |     |     |
 | :---: | :---: |
 | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/707.gif) | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/706.gif) |
 | Support multiple languages, including Chinese, English, Japanese, German, French, Russian, and so on. (Languages except Chinese and English are translated by [Google Translate](https://translate.google.cn/).) | Support multiple interface themes. |
 
 ## Notice
@@ -120,33 +103,14 @@
 
 > Rickrack is an easy to use desktop app for creating and saving color palettes. It supports many major color palette formats for import and export, and is a great tool for generating color palettes of colors that go well together. -- [TJ FREE @ Youtube](https://www.youtube.com/watch?v=OUnktTCtv3E)
 
 > ... and more!
 
 <div align="right"><a href="#table-of-content">[-> Back to TOC <-]</a></div>
 
-# User Comments
-> 作为一个配色软件，它本身的色彩，嗯，足够惊艳...你完全可以信得过作者。 -- User from [Open Source China](https://www.oschina.net/comment/news/231426)
-
-> 很棒！是一个不可多得的工具。 -- User from [Bilibili](https://www.bilibili.com/video/BV1VD4y157tX/)
-
-> 谢谢分享，说明写的太详细了。 -- User from [Baidu Tieba](https://tieba.baidu.com/p/8253007907)
-
-> Thanks a mil! All of my pallette creators were online. This a good offline tool to have with some additional features too. -- User from [Youtube](https://www.youtube.com/watch?v=OUnktTCtv3E)
-
-> I don't like online-apps, so this is a huge plus from the get-go. Thanks for sharing this great tool. -- User from [Youtube](https://www.youtube.com/watch?v=OUnktTCtv3E)
-
-> Thanks for sharing this! And - did I notice correctly that you are also the author of this software? This looks super exciting, can’t wait to investigate it more! -- User from [Krita Artists](https://krita-artists.org/t/alternatives-to-adobe-color-rickrack/60041)
-
-> Hello, your software (the deb package) runs fine on Xubuntu 22.04 and is quite impressive! Thanks for sharing. Next step is to study some tutorials. -- User from [PIXLS.US](https://discuss.pixls.us/t/alternatives-to-adobe-color-rickrack/35997)
-
-> ... and more!
-
-<div align="right"><a href="#table-of-content">[-> Back to TOC <-]</a></div>
-
 # Information
 ## Homepage
 https://eigenmiao.com/rickrack/
 
 ## Repository
 https://github.com/eigenmiao/Rickrack
 
@@ -156,24 +120,24 @@
 ## Support
 [Support the Future of Rickrack!](https://afdian.net/a/eigenmiao)
 
 <div align="right"><a href="#table-of-content">[-> Back to TOC <-]</a></div>
 
 # Installation
 ## Current Release
-The latest preview version is [v2.7.25](https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.25).
+The latest preview version is [v2.7.26](https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.26).
 
 ## Install Software
 ### Recommend: Install on Windows 10 or 11 via WinGet tool
 ```
 winget install rickrack
 ```
 
 ## Install on other platforms
-Download Software from [Github](https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.25) or [Sourceforge](https://sourceforge.net/projects/rickrack/files/v2.7.25/). The installation steps are presented in [tutorials](https://eigenmiao.com/2021/12/12/rickrack-tutorial-en-v2.3.4/#Installation).
+Download Software from [Github](https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.26) or [Sourceforge](https://sourceforge.net/projects/rickrack/files/v2.7.26/). The installation steps are presented in [tutorials](https://eigenmiao.com/2021/12/12/rickrack-tutorial-en-v2.3.4/#Installation).
 
 Here is a [video tutorial](https://www.bilibili.com/video/BV17r4y1L7R6/).
 
 ## Install Module
 Install the latest [Rickrack](https://pypi.org/project/Rickrack/) from PyPI!
 
 ```Bash
@@ -273,12 +237,12 @@
 Rickrack is a free software, which is distributed in the hope that it will be useful, but without any warranty. You can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation. See the [GNU General Public License 3.0 (GPL 3.0)](https://www.gnu.org/licenses/) for more details.
 
 All images, documents and translations in Rickrack [code repository](https://github.com/eigenmiao/Rickrack) are licensed under [Creative Commons Attribution-NonCommercial-ShareAlike License 4.0 (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/) unless stating additionally.
 
 Rickrack default uses [Noto Serif](https://fonts.google.com/specimen/Noto+Serif) ([SC](https://fonts.google.com/specimen/Noto+Serif+SC)) fonts and [Noto Sans](https://fonts.google.com/specimen/Noto+Sans) ([SC](https://fonts.google.com/specimen/Noto+Sans+SC)) fonts for interface display, which are designed by Google and published in website [Google Fonts](https://fonts.google.com/). These fonts are open-sourced under [Apache 2.0](http://www.apache.org/licenses/) and [SIL Open Font License 1.1](http://scripts.sil.org/OFL), respectively.
 
 # Acknowledgment
-* The Rickrack software is written in [Python](https://www.python.org/), constructed based on [PySide2](https://www.qt.io/qt-for-python) and packed up by [fbs (free edition)](https://build-system.fman.io/).
+* The Rickrack software is written in [Python](https://www.python.org/), constructed based on [PyQt5](https://www.qt.io/qt-for-python) and packed up by [fbs (free edition)](https://build-system.fman.io/).
 * The localization (l10n) and internationalization (i18n) of Rickrack is based on [Google Translate](https://translate.google.cn/) and [Microsoft Translator](https://cn.bing.com/translator), deployed on [POEditor](https://poeditor.com/join/project?hash=kBeQjfxCES).
 * The code repository is deposited on [Github](https://github.com/eigenmiao/Rickrack) and [Gitee](https://gitee.com/eigenmiao/Rickrack).
 
 <div align="right"><a href="#rickrack">[-> Back to Top <-]</a> <a href="#table-of-content">[-> Back to TOC <-]</a></div>
```

#### html2text {}

```diff
@@ -2,65 +2,54 @@
 
                                    Rickrack
                                 ç°ç«åäºå·
                ----- ----- ----- ----- ----- ----- ----- -----
                       Generate Harmonious Colors Freely.
                       èªç±èªå¨çæåè°è²å½©ã
 
-                      [ä¸­æ] | [English] | [æ¥æ¬èª]
+                             [ä¸­æ] | [English]
 
-# Rickrack Rickrack (**R**e**a**l-t**i**me **C**olor **K**it) is a free and
-user-friendly color editor. It is designed to generate a set of harmonious
-colors from the color wheel or other places. You can share these colors with
-your friends, or apply them into your creative works. # ç°ç«åäºå·
-ç°ç«åäºå·ï¼å®æ¶è²å½©å·¥å·ç®±ï¼æ¯ä¸æ¬¾åè´¹ä¸å®ç¨çè²å½©ç¼è¾å¨ãå®å¯ä»¥å¸®å©ä½ ä»è²è½®æèå¶ä»å°æ¹çæä¸ç»åè°çè²å½©ãä½ å¯ä»¥å°è¿äºè²å½©åäº«ç»å¶ä»äººï¼æèåºç¨å°ä½ èªå·±çåä½å½ä¸­ã
-# Table of Content * [Introduction](#introduction) * [Feature](#feature) *
+# Rickrack In the age of digital creativity, the color palette has become an
+indispensable tool for designers. A good color palette can make a design more
+attractive and coordinated. Rickrack is designed for you if you are looking for
+an excellent color palette software! Rickrack has various color mixing
+functions and is suitable for various scenes. Rickrack is easy to use, and more
+importantly, it's completely free without networking or registration required.
+Rickrack (**R**e**a**l-t**i**me **C**olor **K**it) is a free and user-friendly
+color editor. It is designed to generate a set of harmonious colors from the
+color wheel or other places. You can share these colors with your friends, or
+apply them into your creative works. Whatâs more, you can export them into
+individual files and import them into other softwares such as Adobe Photoshop,
+GIMP, Krita, Pencil 2D and Clip Studio Paint. Rickrack can run normally on
+operating systems such as Windows, Linux, and macOS. # ç°ç«åäºå·
+å¨æ°å­åæçæ¶ä»£ï¼è°è²æ¿æä¸ºäºè®¾è®¡å¸ä¸å¯æç¼ºçå·¥å·ãä¸ä¸ªå¥½çè°è²æ¿å¯ä»¥è®©è®¾è®¡æ´å æå¸å¼åååè°æ§ãå¦æä½ æ­£å¨å¯»æ¾ä¸æ¬¾ä¼ç§çè°è²æ¿è½¯ä»¶ï¼é£å°±è¯è¯ç°ç«åäºå·å§ï¼ç°ç«åäºå·å·æå¤ç§éè²åè½ï¼éç¨äºå¤ç§åºæ¯ãç°ç«åäºå·ç®åæä¸æï¼æ´éè¦çæ¯ï¼å®å®å¨åè´¹ï¼æ éèç½ææ³¨åã
+ç°ç«åäºå·ï¼å®æ¶è²å½©å·¥å·ç®±ï¼æ¯ä¸æ¬¾åè´¹ä¸å®ç¨çè²å½©ç¼è¾å¨ãå®å¯ä»¥å¸®å©ä½ ä»è²è½®æèå¶ä»å°æ¹çæä¸ç»åè°çè²å½©ãä½ å¯ä»¥å°è¿äºè²å½©åäº«ç»å¶ä»äººï¼æèåºç¨å°ä½ èªå·±çåä½å½ä¸­ãæ­¤å¤ï¼ä½ ä¹å¯ä»¥å°è²å½©ç»æèè²å½©ä»åºå¯¼åºä¸ºåç¬çè²å½©ææ¡£å¹¶å¯¼å¥å¶ä»è½¯ä»¶ä¸­ï¼å¦
+Adobe PhotoshopãGIMPãKritaãPencil 2D ä»¥åä¼å¨æ¼« Paint
+ç­ï¼ãç°ç«åäºå·å¯ä»¥å¨ WindowsãLinuxãmacOS
+ç­æä½ç³»ç»ä¸æ­£å¸¸è¿è¡ã # Table of Content * [Feature](#feature) *
 [Demo](#demo) * [Basic Functions](#basic-functions) * [Reference Colors]
 (#reference-colors) * [Color Palettes](#color-palettes) * [Export and Import
 Colors](#export-and-import-colors) * [Languages and Settings](#languages-and-
-settings) * [Reviews about Rickrack](#reviews-about-rickrack) * [User Comments]
-(#user-comments) * [Information](#information) * [Homepage](#homepage) *
-[Repository](#repository) * [Author](#author) * [Support](#support) *
-[Installation](#installation) * [Current Release](#current-release) * [Download
-Software](#download-software) * [Install Software](#install-software) *
-[Install Module](#install-module) * [Usage](#usage) * [How to Use the Software]
-(#how-to-use-the-software) * [How to Use the Module](#how-to-use-the-module) *
-[Development](#development) * [Install Requirement](#install-requirement) *
-[How to Build the Software](#how-to-build-the-software) * [How to Build the
-Module](#how-to-build-the-module) * [Copyright](#copyright) * [License]
-(#license) * [License for Rickrack](#license-for-rickrack) * [Acknowledgment]
-(#acknowledgment) # Introduction Colors enrich our world and affect our
-emotions. For artists, they display objects and convey feelings by varied
-colors in photos, images and drawings. For scientist, they present data by
-distinguishable colors in figures and graphics. However, the majority of color
-softwares and websites put restrictions on users, which include the inability
-to export color palettes into individual files, not providing invocation
-interfaces, requiring registrations, regional limitations and (or) collecting
-users' personal information. If you are running into these issues, Rickrack is
-the perfect solution for you! Rickrack is a free and user-friendly color
-editor. It is designed to generate a set of harmonious colors from the color
-wheel or other places. You can share these colors with your friends, or apply
-them into your creative works. You can store the color sets and color boards in
-the software, and access them whenever you need. What's more, you can export
-them into individual files, back them up, share them with others or import them
-in to other softwares such as Adobe Photoshop, GIMP, Krita, Pencil 2D and Clip
-Studio Paint. Rickrack, written in PySide2, operates effectively on Windows,
-Linux and other mainstream operating systems. Rickrack consists of two parts:
-the Rickrack software and the Rickrack module; the Rickrack software is
-designed for producing and organizing harmonious colors, and the Rickrack
-module is utilized for obtaining colors from the software in real-time, along
-with the plotting of images combined with other modules such as Matplotlib and
-Turtle.
-                                                            [->_Back_to_TOC_<-]
-# Feature Rickrack has several features: * A strong and free color editor. *
-Create a set of colors from the color wheel. * Pick-up a set of colors from an
-image. * Generate a color board from the color set. * Attach the color set and
-color board into the depot. * Import colors from elsewhere and manage them in
-depot. * Export colors and import them into other image processors. * Obtain
-colors through the Python module in real-time. * No function limitations and no
+settings) * [Reviews about Rickrack](#reviews-about-rickrack) * [Information]
+(#information) * [Homepage](#homepage) * [Repository](#repository) * [Author]
+(#author) * [Support](#support) * [Installation](#installation) * [Current
+Release](#current-release) * [Download Software](#download-software) * [Install
+Software](#install-software) * [Install Module](#install-module) * [Usage]
+(#usage) * [How to Use the Software](#how-to-use-the-software) * [How to Use
+the Module](#how-to-use-the-module) * [Development](#development) * [Install
+Requirement](#install-requirement) * [How to Build the Software](#how-to-build-
+the-software) * [How to Build the Module](#how-to-build-the-module) *
+[Copyright](#copyright) * [License](#license) * [License for Rickrack]
+(#license-for-rickrack) * [Acknowledgment](#acknowledgment) # Feature Rickrack
+has several features: * A strong and free color editor. * Create a set of
+colors from the color wheel. * Pick-up a set of colors from an image. *
+Generate a color board from the color set. * Attach the color set and color
+board into the depot. * Import colors from elsewhere and manage them in depot.
+* Export colors and import them into other image processors. * Obtain colors
+through the Python module in real-time. * No function limitations and no
 registration required. * ... and more!
                                                             [->_Back_to_TOC_<-]
 # Demo ## Basic Functions | | | | :---: | :---: | | ![](https://
 raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/000.gif) | ![]
 (https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/
 109.gif) | | Create a set of colors from the color wheel. | Pick-up a set of
 colors from an image. (Image inside: [Copyright (c) 2001 Studio Ghibli](https:/
@@ -80,74 +69,46 @@
 Convert: gradient palette ↔ fixed palette. | Convert: gradient palette ↔
 reference palette. | | ![](https://raw.githubusercontent.com/eigenmiao/
 Rickrack/master/demo/usage/700.gif) | ![](https://raw.githubusercontent.com/
 eigenmiao/Rickrack/master/demo/usage/701.gif) | | Fixed palette: Chinese
 Traditional Colors. (Color Names: [Copyright (c) China Science Publishing &
 Media Ltd.](http://zhongguose.com/), Non-Commercial Usage) | Fixed palette:
 Nippon Traditional Colors. (Color Names: [Copyright (c) PIE BOOKS.](http://
-nipponcolors.com/), Non-Commercial Usage) | ## Export and Import Colors | | | |
-:---: | :---: | | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/
-master/demo/usage/704.gif) | ![](https://raw.githubusercontent.com/eigenmiao/
-Rickrack/master/demo/usage/702.gif) | | Export colors into a Rickrack file. |
-Export colors into a Adobe swatch file. | | ![](https://
-raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/705.gif) | ![]
-(https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/
-703.gif) | | Import colors from a Rickrack file. | Import colors from a Adobe
-swatch file. | ## Languages and Settings | | | | :---: | :---: | | ![](https://
-raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/707.gif) | ![]
-(https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/
-706.gif) | | Support multiple languages, including Chinese, English, Japanese,
-German, French, Russian, and so on. (Languages except Chinese and English are
-translated by [Google Translate](https://translate.google.cn/).) | Support
-multiple interface themes. | ## Notice * The interface display in demo uses
-[LXGWWenKai (SIL Open Font License)](https://lxgw.github.io/2021/01/28/Klee-
-Simpchin/) font.
+nipponcolors.com/), Non-Commercial Usage) | ## Languages and Settings | | | | :
+---: | :---: | | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/
+master/demo/usage/707.gif) | ![](https://raw.githubusercontent.com/eigenmiao/
+Rickrack/master/demo/usage/706.gif) | | Support multiple languages, including
+Chinese, English, Japanese, German, French, Russian, and so on. (Languages
+except Chinese and English are translated by [Google Translate](https://
+translate.google.cn/).) | Support multiple interface themes. | ## Notice * The
+interface display in demo uses [LXGWWenKai (SIL Open Font License)](https://
+lxgw.github.io/2021/01/28/Klee-Simpchin/) font.
                                                             [->_Back_to_TOC_<-]
 # Reviews about Rickrack > All in all, Rickrack is a comprehensive tool for
 anything that requires color work. Experienced users have an exhaustive toolset
 to work with, while a more casual audience can improve the presentation of
 their art by quickly getting color synergy ideas. -- [Robert Condorache @
 Softpedia](https://www.softpedia.com/get/Multimedia/Graphic/Graphic-Others/
 RickRack.shtml) > Rickrack is an easy to use desktop app for creating and
 saving color palettes. It supports many major color palette formats for import
 and export, and is a great tool for generating color palettes of colors that go
 well together. -- [TJ FREE @ Youtube](https://www.youtube.com/
 watch?v=OUnktTCtv3E) > ... and more!
                                                             [->_Back_to_TOC_<-]
-# User Comments >
-ä½ä¸ºä¸ä¸ªéè²è½¯ä»¶ï¼å®æ¬èº«çè²å½©ï¼å¯ï¼è¶³å¤æè³...ä½ å®å¨å¯ä»¥ä¿¡å¾è¿ä½èã
--- User from [Open Source China](https://www.oschina.net/comment/news/231426) >
-å¾æ£ï¼æ¯ä¸ä¸ªä¸å¯å¤å¾çå·¥å·ã -- User from [Bilibili](https://
-www.bilibili.com/video/BV1VD4y157tX/) >
-è°¢è°¢åäº«ï¼è¯´æåçå¤ªè¯¦ç»äºã -- User from [Baidu Tieba](https://
-tieba.baidu.com/p/8253007907) > Thanks a mil! All of my pallette creators were
-online. This a good offline tool to have with some additional features too. -
-- User from [Youtube](https://www.youtube.com/watch?v=OUnktTCtv3E) > I don't
-like online-apps, so this is a huge plus from the get-go. Thanks for sharing
-this great tool. -- User from [Youtube](https://www.youtube.com/
-watch?v=OUnktTCtv3E) > Thanks for sharing this! And - did I notice correctly
-that you are also the author of this software? This looks super exciting,
-canât wait to investigate it more! -- User from [Krita Artists](https://
-krita-artists.org/t/alternatives-to-adobe-color-rickrack/60041) > Hello, your
-software (the deb package) runs fine on Xubuntu 22.04 and is quite impressive!
-Thanks for sharing. Next step is to study some tutorials. -- User from
-[PIXLS.US](https://discuss.pixls.us/t/alternatives-to-adobe-color-rickrack/
-35997) > ... and more!
-                                                            [->_Back_to_TOC_<-]
 # Information ## Homepage https://eigenmiao.com/rickrack/ ## Repository https:/
 /github.com/eigenmiao/Rickrack ## Author [Eigenmiao](mailto:
 eigenmiao@outlook.com) ## Support [Support the Future of Rickrack!](https://
 afdian.net/a/eigenmiao)
                                                             [->_Back_to_TOC_<-]
-# Installation ## Current Release The latest preview version is [v2.7.25]
-(https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.25). ## Install
+# Installation ## Current Release The latest preview version is [v2.7.26]
+(https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.26). ## Install
 Software ### Recommend: Install on Windows 10 or 11 via WinGet tool ``` winget
 install rickrack ``` ## Install on other platforms Download Software from
-[Github](https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.25) or
-[Sourceforge](https://sourceforge.net/projects/rickrack/files/v2.7.25/). The
+[Github](https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.26) or
+[Sourceforge](https://sourceforge.net/projects/rickrack/files/v2.7.26/). The
 installation steps are presented in [tutorials](https://eigenmiao.com/2021/12/
 12/rickrack-tutorial-en-v2.3.4/#Installation). Here is a [video tutorial]
 (https://www.bilibili.com/video/BV17r4y1L7R6/). ## Install Module Install the
 latest [Rickrack](https://pypi.org/project/Rickrack/) from PyPI! ```Bash #
 Install Rickrack. pip install Rickrack # Start the installed software. rickrack
 -d "/PATH/TO/RICKRACK/SOFTWARE" ```
                                                             [->_Back_to_TOC_<-]
@@ -196,15 +157,15 @@
 specimen/Noto+Serif) ([SC](https://fonts.google.com/specimen/Noto+Serif+SC))
 fonts and [Noto Sans](https://fonts.google.com/specimen/Noto+Sans) ([SC](https:
 //fonts.google.com/specimen/Noto+Sans+SC)) fonts for interface display, which
 are designed by Google and published in website [Google Fonts](https://
 fonts.google.com/). These fonts are open-sourced under [Apache 2.0](http://
 www.apache.org/licenses/) and [SIL Open Font License 1.1](http://
 scripts.sil.org/OFL), respectively. # Acknowledgment * The Rickrack software is
-written in [Python](https://www.python.org/), constructed based on [PySide2]
+written in [Python](https://www.python.org/), constructed based on [PyQt5]
 (https://www.qt.io/qt-for-python) and packed up by [fbs (free edition)](https:/
 /build-system.fman.io/). * The localization (l10n) and internationalization
 (i18n) of Rickrack is based on [Google Translate](https://translate.google.cn/
 ) and [Microsoft Translator](https://cn.bing.com/translator), deployed on
 [POEditor](https://poeditor.com/join/project?hash=kBeQjfxCES). * The code
 repository is deposited on [Github](https://github.com/eigenmiao/Rickrack) and
 [Gitee](https://gitee.com/eigenmiao/Rickrack).
```

### Comparing `Rickrack-2.7.25/rickrack/color.py` & `Rickrack-2.7.26/rickrack/color.py`

 * *Files identical despite different names*

### Comparing `Rickrack-2.7.25/rickrack/result.py` & `Rickrack-2.7.26/rickrack/result.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 Please visit https://github.com/eigenmiao/Rickrack for more infomation 
 about Rickrack.
 
 Copyright (c) 2019-2023 by Eigenmiao. All Rights Reserved.
 """
 
+import numpy as np
 from rickrack.color import Color
 
 
 class Box(object):
     """
     Box object. Storing a color and a name.
     """
@@ -78,57 +79,64 @@
         Args:
             color_grid (tuple or list): hex code color list.
             name_grid (tuple or list): name list.
             grid_size (tuple, or list): grid size.
         """
 
         if not isinstance(color_grid, (tuple, list)):
-            raise ValueError("Invalid color grid: {}".format(color_grid))
+            raise ValueError("Color grid is not a list: {}".format(color_grid))
 
         if not isinstance(name_grid, (tuple, list)):
-            raise ValueError("Invalid name grid: {}".format(name_grid))
+            raise ValueError("Name grid is not a list: {}".format(name_grid))
 
         if isinstance(grid_size, int) and grid_size >= 0:
             self._grid_size = (int(grid_size),)
 
         elif isinstance(grid_size, (tuple, list)) and len(grid_size) == 1 and isinstance(grid_size[0], int) and grid_size[0] >= 0:
             self._grid_size = (int(grid_size[0]),)
 
         elif isinstance(grid_size, (tuple, list)) and len(grid_size) == 2 and isinstance(grid_size[0], int) and isinstance(grid_size[1], int) and grid_size[0] >= 0 and grid_size[1] >= 0:
             self._grid_size = (int(grid_size[0]), int(grid_size[1]))
 
         else:
-            raise ValueError("Invalid grid size: {}".format(grid_size))
+            raise ValueError("Grid size is not a number list: {}".format(grid_size))
 
         if len(self._grid_size) == 1:
-            self._color_grid = ["FFFFFF" if i >= len(color_grid) else str(color_grid[i]) for i in range(self._grid_size[0])]
-            self._name_grid = ["RR-{}".format(i + 1) if i >= len(name_grid) else str(name_grid[i]) for i in range(self._grid_size[0])]
+            color_grid = ["FFFFFF" if i >= len(color_grid) else Color.fmt_hec(color_grid[i]) for i in range(self._grid_size[0])]
+            name_grid = ["RR-{}".format(i + 1) if i >= len(name_grid) else str(name_grid[i]) for i in range(self._grid_size[0])]
 
         else:
-            self._color_grid = [["FFFFFF" if i * self._grid_size[1] + j >= len(color_grid) else str(color_grid[i * self._grid_size[1] + j]) for j in range(self._grid_size[1])] for i in range(self._grid_size[0])]
-            self._name_grid = [["RR-{}-{}".format(i + 1, j + 1) if i * self._grid_size[1] + j >= len(name_grid) else str(name_grid[i * self._grid_size[1] + j]) for j in range(self._grid_size[1])] for i in range(self._grid_size[0])]
+            color_grid = [["FFFFFF" if i * self._grid_size[1] + j >= len(color_grid) else Color.fmt_hec(color_grid[i * self._grid_size[1] + j]) for j in range(self._grid_size[1])] for i in range(self._grid_size[0])]
+            name_grid = [["RR-{}-{}".format(i + 1, j + 1) if i * self._grid_size[1] + j >= len(name_grid) else str(name_grid[i * self._grid_size[1] + j]) for j in range(self._grid_size[1])] for i in range(self._grid_size[0])]
+
+        self._color_grid = np.array(color_grid, dtype=str).reshape(grid_size)
+        self._name_grid = np.array(name_grid, dtype=str).reshape(grid_size)
 
     # ---------- ---------- ---------- Inner Funcs ---------- ---------- ---------- #
 
     def __getitem__(self, idx):
         """
         Get color item in color grid.
 
         Args:
             idx (int or float): color index in grid.
         """
 
         curr_color = self._color_grid[idx]
         curr_name = self._name_grid[idx]
 
-        if isinstance(curr_color, str):
+        if isinstance(curr_color, str) and isinstance(curr_name, str):
             return Box(curr_color, curr_name)
 
-        else:
-            return Grid(curr_color, curr_name, len(curr_color))
+        elif isinstance(curr_color, np.ndarray) and isinstance(curr_name, np.ndarray):
+            curr_size = curr_color.shape
+            curr_color = curr_color.reshape(-1).tolist()
+            curr_name = curr_name.reshape(-1).tolist()
+
+            return Grid(curr_color, curr_name, curr_size)
 
     def __str__(self):
         """
         Str format.
         """
 
         return "Grid(size {})".format("x".join([str(i) for i in self.size]))
@@ -140,61 +148,52 @@
 
         return str(self)
 
     # ---------- ---------- ---------- Properties ---------- ---------- ---------- #
 
     @property
     def T(self):
-        if len(self.size) == 1:
-            return Grid(self._color_grid, self._name_grid, self.size)
+        curr_color = self._color_grid.T
+        curr_name = self._name_grid.T
 
-        else:
-            return Grid(*self.v_line.grid.values, (self.size[1], self.size[0]))
+        curr_size = curr_color.shape
+        curr_color = curr_color.reshape(-1).tolist()
+        curr_name = curr_name.reshape(-1).tolist()
+
+        return Grid(curr_color, curr_name, curr_size)
 
     @property
     def size(self):
         return self._grid_size
 
     @property
+    def shape(self):
+        return self.size
+
+    @property
     def values(self):
-        return tuple(self._color_grid), tuple(self._name_grid)
+        return self._color_grid.reshape(-1).tolist(), self._name_grid.reshape(-1).tolist()
 
     @property
     def grid(self):
         return Grid(*self.h_line.values, self.size)
 
     @property
     def h_line(self):
-        if len(self.size) == 1:
-            return Grid(self._color_grid, self._name_grid, self.size)
+        curr_color = self._color_grid.reshape(-1).tolist()
+        curr_name = self._name_grid.reshape(-1).tolist()
 
-        else:
-            color_grid = []
-            name_grid = []
-
-            for i in range(self.size[0]):
-                color_grid += self._color_grid[i]
-                name_grid += self._name_grid[i]
-
-            return Grid(color_grid, name_grid, self.size[0] * self.size[1])
+        return Grid(curr_color, curr_name, len(curr_color))
 
     @property
     def v_line(self):
-        if len(self.size) == 1:
-            return Grid(self._color_grid, self._name_grid, self.size)
-
-        else:
-            color_grid = []
-            name_grid = []
-
-            for j in range(self.size[1]):
-                color_grid += [self._color_grid[i][j] for i in range(self.size[0])]
-                name_grid += [self._name_grid[i][j] for i in range(self.size[0])]
+        curr_color = self._color_grid.T.reshape(-1).tolist()
+        curr_name = self._name_grid.T.reshape(-1).tolist()
 
-            return Grid(color_grid, name_grid, self.size[0] * self.size[1])
+        return Grid(curr_color, curr_name, len(curr_color))
 
 
 class Result(object):
     """
     Result object. Storing rickrack result.
     """
```

### Comparing `Rickrack-2.7.25/rickrack/rickrack.py` & `Rickrack-2.7.26/rickrack/rickrack.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 """
 
 __WEBSITE__ = """
 https://github.com/eigenmiao/Rickrack
 """
 
 __VERSION__ = """
-v2.7.25-x2d3s3-stable
+v2.7.26-x2d3s3-stable
 """
 
 __AUTHOR__ = """
 Eigenmiao (eigenmiao@outlook.com)
 """
 
 __DATE__ = """
-March 12, 2023
+April 9, 2023
 """
 
 __HELP__ = """
 INTRODUCTION:
   Rickrack-Startup provides the ability to operate Rickrack from the 
   command line or through Python code, allowing you to start it, close it, 
   and obtain color results from Rickrack.
@@ -369,14 +369,34 @@
         return self._result.colors_in_order
 
     @property
     def selected_color(self):
         return self._result.selected_color
 
     @property
+    def full_colors(self):
+        return self._result.full_colors
+
+    @property
+    def color_grid(self):
+        return self._result.color_grid
+
+    @property
+    def cset(self):
+        return self._result.cset
+
+    @property
+    def cset_in_order(self):
+        return self._result.cset_in_order
+
+    @property
+    def refs(self):
+        return self._result.refs
+
+    @property
     def grid(self):
         return self._result.grid
 
     @property
     def grid_h_line(self):
         return self._result.grid_h_line
 
@@ -387,27 +407,25 @@
     @property
     def is_connected(self):
         """
         Check if connected to server.
         """
 
         if not self._port:
-            self.is_started_by_script = False
             return False
 
         try:
             client = socket.socket()
             client.settimeout(self._timeout)
             client.connect((self._host, self._port))
 
             client.close()
 
         except Exception as err:
             print("Connect to server with port {} faild:\n{}".format(self._port, err))
-            self.is_started_by_script = False
             return False
 
         return True
 
     @property
     def is_choice_available(self):
         """
@@ -899,24 +917,24 @@
         Close Rickrack.
 
         Args:
             save_data (bool): if save data before close.
         """
 
         if self.is_started_by_script and self.is_connected:
-            client = socket.socket()
-            client.settimeout(self._timeout)
-            client.connect((self._host, self._port))
+            while self.is_connected:
+                client = socket.socket()
+                client.settimeout(self._timeout)
+                client.connect((self._host, self._port))
 
-            info = "exit{}".format(save_data)
-            client.sendall(info.encode("utf-8"))
+                info = "exit{}".format(save_data)
+                client.sendall(info.encode("utf-8"))
 
-            client.close()
+                client.close()
 
-            while self.is_connected:
                 time.sleep(1)
                 print("Waiting for closing Rickrack.")
 
         self.is_started_by_script = False
 
     def load_log(self, log_file):
         """
```

### Comparing `Rickrack-2.7.25/rickrack/__init__.py` & `Rickrack-2.7.26/rickrack/__init__.py`

 * *Files identical despite different names*

### Comparing `Rickrack-2.7.25/Rickrack.egg-info/PKG-INFO` & `Rickrack-2.7.26/Rickrack.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: Rickrack
-Version: 2.7.25
+Version: 2.7.26
 Summary: Generate harmonious colors freely.
 Home-page: https://eigenmiao.github.io/rickrack/
 Author: Eigenmiao
 Author-email: eigenmiao@outlook.com
 License: UNKNOWN
 Description: <div align="center">
         <img width="100%" align="center" src="https://raw.githubusercontent.com/eigenmiao/Rickrack/master/src/main/icons/logo_long.png" alt="Rickrack">
         <br/><br/>
         Rickrack<br/>焰火十二卷<br/> ----- ----- ----- ----- ----- ----- ----- ----- <br/>
         Generate Harmonious Colors Freely.<br/>自由自在生成和谐色彩。
         <br/><br/>
-        [<a href="https://eigenmiao.com/yanhuo/zh.html">中文</a>] | [<a href="https://eigenmiao.com/yanhuo/en.html">English</a>] | [<a href="https://eigenmiao.com/yanhuo/ja.html">日本語</a>]
+        [<a href="https://eigenmiao.com/yanhuo/">中文</a>] | [<a href="https://eigenmiao.com/rickrack/">English</a>]
         <br/><br/>
         </div>
         
         # Rickrack
-        Rickrack (**R**e**a**l-t**i**me **C**olor **K**it) is a free and user-friendly color editor. It is designed to generate a set of harmonious colors from the color wheel or other places. You can share these colors with your friends, or apply them into your creative works.
+        In the age of digital creativity, the color palette has become an indispensable tool for designers. A good color palette can make a design more attractive and coordinated. Rickrack is designed for you if you are looking for an excellent color palette software! Rickrack has various color mixing functions and is suitable for various scenes. Rickrack is easy to use, and more importantly, it's completely free without networking or registration required.
+        
+        Rickrack (**R**e**a**l-t**i**me **C**olor **K**it) is a free and user-friendly color editor. It is designed to generate a set of harmonious colors from the color wheel or other places. You can share these colors with your friends, or apply them into your creative works. What’s more, you can export them into individual files and import them into other softwares such as Adobe Photoshop, GIMP, Krita, Pencil 2D and Clip Studio Paint. Rickrack can run normally on operating systems such as Windows, Linux, and macOS.
         
         # 焰火十二卷
-        焰火十二卷（实时色彩工具箱）是一款免费且实用的色彩编辑器。它可以帮助你从色轮或者其他地方生成一组和谐的色彩。你可以将这些色彩分享给其他人，或者应用到你自己的创作当中。
+        在数字创意的时代，调色板成为了设计师不可或缺的工具。一个好的调色板可以让设计更加有吸引力和协调性。如果你正在寻找一款优秀的调色板软件，那就试试焰火十二卷吧！焰火十二卷具有多种配色功能，适用于多种场景。焰火十二卷简单易上手，更重要的是，它完全免费，无需联网或注册。
+        
+        焰火十二卷（实时色彩工具箱）是一款免费且实用的色彩编辑器。它可以帮助你从色轮或者其他地方生成一组和谐的色彩。你可以将这些色彩分享给其他人，或者应用到你自己的创作当中。此外，你也可以将色彩组或者色彩仓库导出为单独的色彩文档并导入其他软件中（如 Adobe Photoshop、GIMP、Krita、Pencil 2D 以及优动漫 Paint 等）。焰火十二卷可以在 Windows、Linux、macOS 等操作系统上正常运行。
         
         # Table of Content
-        * [Introduction](#introduction)
         * [Feature](#feature)
         * [Demo](#demo)
           * [Basic Functions](#basic-functions)
           * [Reference Colors](#reference-colors)
           * [Color Palettes](#color-palettes)
           * [Export and Import Colors](#export-and-import-colors)
           * [Languages and Settings](#languages-and-settings)
         * [Reviews about Rickrack](#reviews-about-rickrack)
-        * [User Comments](#user-comments)
         * [Information](#information)
           * [Homepage](#homepage)
           * [Repository](#repository)
           * [Author](#author)
           * [Support](#support)
         * [Installation](#installation)
           * [Current Release](#current-release)
@@ -51,25 +53,14 @@
           * [How to Build the Software](#how-to-build-the-software)
           * [How to Build the Module](#how-to-build-the-module)
         * [Copyright](#copyright)
         * [License](#license)
           * [License for Rickrack](#license-for-rickrack)
         * [Acknowledgment](#acknowledgment)
         
-        # Introduction
-        Colors enrich our world and affect our emotions. For artists, they display objects and convey feelings by varied colors in photos, images and drawings. For scientist, they present data by distinguishable colors in figures and graphics. However, the majority of color softwares and websites put restrictions on users, which include the inability to export color palettes into individual files, not providing invocation interfaces, requiring registrations, regional limitations and (or) collecting users' personal information.
-        
-        If you are running into these issues, Rickrack is the perfect solution for you!
-        
-        Rickrack is a free and user-friendly color editor. It is designed to generate a set of harmonious colors from the color wheel or other places. You can share these colors with your friends, or apply them into your creative works. You can store the color sets and color boards in the software, and access them whenever you need. What's more, you can export them into individual files, back them up, share them with others or import them in to other softwares such as Adobe Photoshop, GIMP, Krita, Pencil 2D and Clip Studio Paint. Rickrack, written in PySide2, operates effectively on Windows, Linux and other mainstream operating systems.
-        
-        Rickrack consists of two parts: the Rickrack software and the Rickrack module; the Rickrack software is designed for producing and organizing harmonious colors, and the Rickrack module is utilized for obtaining colors from the software in real-time, along with the plotting of images combined with other modules such as Matplotlib and Turtle.
-        
-        <div align="right"><a href="#table-of-content">[-> Back to TOC <-]</a></div>
-        
         # Feature
         Rickrack has several features:
         * A strong and free color editor.
         * Create a set of colors from the color wheel.
         * Pick-up a set of colors from an image.
         * Generate a color board from the color set.
         * Attach the color set and color board into the depot.
@@ -100,22 +91,14 @@
         |     |     |
         | :---: | :---: |
         | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/204.gif) | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/205.gif) |
         | Convert: gradient palette &harr; fixed palette. | Convert: gradient palette &harr; reference palette. |
         | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/700.gif) | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/701.gif) |
         | Fixed palette: Chinese Traditional Colors. (Color Names: [Copyright (c) China Science Publishing & Media Ltd.](http://zhongguose.com/), Non-Commercial Usage) | Fixed palette: Nippon Traditional Colors. (Color Names: [Copyright (c) PIE BOOKS.](http://nipponcolors.com/), Non-Commercial Usage) |
         
-        ## Export and Import Colors
-        |     |     |
-        | :---: | :---: |
-        | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/704.gif) | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/702.gif) |
-        | Export colors into a Rickrack file. | Export colors into a Adobe swatch file. |
-        | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/705.gif) | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/703.gif) |
-        | Import colors from a Rickrack file. | Import colors from a Adobe swatch file. |
-        
         ## Languages and Settings
         |     |     |
         | :---: | :---: |
         | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/707.gif) | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/706.gif) |
         | Support multiple languages, including Chinese, English, Japanese, German, French, Russian, and so on. (Languages except Chinese and English are translated by [Google Translate](https://translate.google.cn/).) | Support multiple interface themes. |
         
         ## Notice
@@ -128,33 +111,14 @@
         
         > Rickrack is an easy to use desktop app for creating and saving color palettes. It supports many major color palette formats for import and export, and is a great tool for generating color palettes of colors that go well together. -- [TJ FREE @ Youtube](https://www.youtube.com/watch?v=OUnktTCtv3E)
         
         > ... and more!
         
         <div align="right"><a href="#table-of-content">[-> Back to TOC <-]</a></div>
         
-        # User Comments
-        > 作为一个配色软件，它本身的色彩，嗯，足够惊艳...你完全可以信得过作者。 -- User from [Open Source China](https://www.oschina.net/comment/news/231426)
-        
-        > 很棒！是一个不可多得的工具。 -- User from [Bilibili](https://www.bilibili.com/video/BV1VD4y157tX/)
-        
-        > 谢谢分享，说明写的太详细了。 -- User from [Baidu Tieba](https://tieba.baidu.com/p/8253007907)
-        
-        > Thanks a mil! All of my pallette creators were online. This a good offline tool to have with some additional features too. -- User from [Youtube](https://www.youtube.com/watch?v=OUnktTCtv3E)
-        
-        > I don't like online-apps, so this is a huge plus from the get-go. Thanks for sharing this great tool. -- User from [Youtube](https://www.youtube.com/watch?v=OUnktTCtv3E)
-        
-        > Thanks for sharing this! And - did I notice correctly that you are also the author of this software? This looks super exciting, can’t wait to investigate it more! -- User from [Krita Artists](https://krita-artists.org/t/alternatives-to-adobe-color-rickrack/60041)
-        
-        > Hello, your software (the deb package) runs fine on Xubuntu 22.04 and is quite impressive! Thanks for sharing. Next step is to study some tutorials. -- User from [PIXLS.US](https://discuss.pixls.us/t/alternatives-to-adobe-color-rickrack/35997)
-        
-        > ... and more!
-        
-        <div align="right"><a href="#table-of-content">[-> Back to TOC <-]</a></div>
-        
         # Information
         ## Homepage
         https://eigenmiao.com/rickrack/
         
         ## Repository
         https://github.com/eigenmiao/Rickrack
         
@@ -164,24 +128,24 @@
         ## Support
         [Support the Future of Rickrack!](https://afdian.net/a/eigenmiao)
         
         <div align="right"><a href="#table-of-content">[-> Back to TOC <-]</a></div>
         
         # Installation
         ## Current Release
-        The latest preview version is [v2.7.25](https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.25).
+        The latest preview version is [v2.7.26](https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.26).
         
         ## Install Software
         ### Recommend: Install on Windows 10 or 11 via WinGet tool
         ```
         winget install rickrack
         ```
         
         ## Install on other platforms
-        Download Software from [Github](https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.25) or [Sourceforge](https://sourceforge.net/projects/rickrack/files/v2.7.25/). The installation steps are presented in [tutorials](https://eigenmiao.com/2021/12/12/rickrack-tutorial-en-v2.3.4/#Installation).
+        Download Software from [Github](https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.26) or [Sourceforge](https://sourceforge.net/projects/rickrack/files/v2.7.26/). The installation steps are presented in [tutorials](https://eigenmiao.com/2021/12/12/rickrack-tutorial-en-v2.3.4/#Installation).
         
         Here is a [video tutorial](https://www.bilibili.com/video/BV17r4y1L7R6/).
         
         ## Install Module
         Install the latest [Rickrack](https://pypi.org/project/Rickrack/) from PyPI!
         
         ```Bash
@@ -281,15 +245,15 @@
         Rickrack is a free software, which is distributed in the hope that it will be useful, but without any warranty. You can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation. See the [GNU General Public License 3.0 (GPL 3.0)](https://www.gnu.org/licenses/) for more details.
         
         All images, documents and translations in Rickrack [code repository](https://github.com/eigenmiao/Rickrack) are licensed under [Creative Commons Attribution-NonCommercial-ShareAlike License 4.0 (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/) unless stating additionally.
         
         Rickrack default uses [Noto Serif](https://fonts.google.com/specimen/Noto+Serif) ([SC](https://fonts.google.com/specimen/Noto+Serif+SC)) fonts and [Noto Sans](https://fonts.google.com/specimen/Noto+Sans) ([SC](https://fonts.google.com/specimen/Noto+Sans+SC)) fonts for interface display, which are designed by Google and published in website [Google Fonts](https://fonts.google.com/). These fonts are open-sourced under [Apache 2.0](http://www.apache.org/licenses/) and [SIL Open Font License 1.1](http://scripts.sil.org/OFL), respectively.
         
         # Acknowledgment
-        * The Rickrack software is written in [Python](https://www.python.org/), constructed based on [PySide2](https://www.qt.io/qt-for-python) and packed up by [fbs (free edition)](https://build-system.fman.io/).
+        * The Rickrack software is written in [Python](https://www.python.org/), constructed based on [PyQt5](https://www.qt.io/qt-for-python) and packed up by [fbs (free edition)](https://build-system.fman.io/).
         * The localization (l10n) and internationalization (i18n) of Rickrack is based on [Google Translate](https://translate.google.cn/) and [Microsoft Translator](https://cn.bing.com/translator), deployed on [POEditor](https://poeditor.com/join/project?hash=kBeQjfxCES).
         * The code repository is deposited on [Github](https://github.com/eigenmiao/Rickrack) and [Gitee](https://gitee.com/eigenmiao/Rickrack).
         
         <div align="right"><a href="#rickrack">[-> Back to Top <-]</a> <a href="#table-of-content">[-> Back to TOC <-]</a></div>
         
 Keywords: Color-Editor,Color-Picker,Color-Palette,Digital-Palette,Desktop-Application
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,70 +1,59 @@
-Metadata-Version: 2.1 Name: Rickrack Version: 2.7.25 Summary: Generate
+Metadata-Version: 2.1 Name: Rickrack Version: 2.7.26 Summary: Generate
 harmonious colors freely. Home-page: https://eigenmiao.github.io/rickrack/
 Author: Eigenmiao Author-email: eigenmiao@outlook.com License: UNKNOWN
 Description:
                                   [Rickrack]
 
                                    Rickrack
                                 ç°ç«åäºå·
                ----- ----- ----- ----- ----- ----- ----- -----
                       Generate Harmonious Colors Freely.
                       èªç±èªå¨çæåè°è²å½©ã
 
-                      [ä¸­æ] | [English] | [æ¥æ¬èª]
+                             [ä¸­æ] | [English]
 
-# Rickrack Rickrack (**R**e**a**l-t**i**me **C**olor **K**it) is a free and
-user-friendly color editor. It is designed to generate a set of harmonious
-colors from the color wheel or other places. You can share these colors with
-your friends, or apply them into your creative works. # ç°ç«åäºå·
-ç°ç«åäºå·ï¼å®æ¶è²å½©å·¥å·ç®±ï¼æ¯ä¸æ¬¾åè´¹ä¸å®ç¨çè²å½©ç¼è¾å¨ãå®å¯ä»¥å¸®å©ä½ ä»è²è½®æèå¶ä»å°æ¹çæä¸ç»åè°çè²å½©ãä½ å¯ä»¥å°è¿äºè²å½©åäº«ç»å¶ä»äººï¼æèåºç¨å°ä½ èªå·±çåä½å½ä¸­ã
-# Table of Content * [Introduction](#introduction) * [Feature](#feature) *
+# Rickrack In the age of digital creativity, the color palette has become an
+indispensable tool for designers. A good color palette can make a design more
+attractive and coordinated. Rickrack is designed for you if you are looking for
+an excellent color palette software! Rickrack has various color mixing
+functions and is suitable for various scenes. Rickrack is easy to use, and more
+importantly, it's completely free without networking or registration required.
+Rickrack (**R**e**a**l-t**i**me **C**olor **K**it) is a free and user-friendly
+color editor. It is designed to generate a set of harmonious colors from the
+color wheel or other places. You can share these colors with your friends, or
+apply them into your creative works. Whatâs more, you can export them into
+individual files and import them into other softwares such as Adobe Photoshop,
+GIMP, Krita, Pencil 2D and Clip Studio Paint. Rickrack can run normally on
+operating systems such as Windows, Linux, and macOS. # ç°ç«åäºå·
+å¨æ°å­åæçæ¶ä»£ï¼è°è²æ¿æä¸ºäºè®¾è®¡å¸ä¸å¯æç¼ºçå·¥å·ãä¸ä¸ªå¥½çè°è²æ¿å¯ä»¥è®©è®¾è®¡æ´å æå¸å¼åååè°æ§ãå¦æä½ æ­£å¨å¯»æ¾ä¸æ¬¾ä¼ç§çè°è²æ¿è½¯ä»¶ï¼é£å°±è¯è¯ç°ç«åäºå·å§ï¼ç°ç«åäºå·å·æå¤ç§éè²åè½ï¼éç¨äºå¤ç§åºæ¯ãç°ç«åäºå·ç®åæä¸æï¼æ´éè¦çæ¯ï¼å®å®å¨åè´¹ï¼æ éèç½ææ³¨åã
+ç°ç«åäºå·ï¼å®æ¶è²å½©å·¥å·ç®±ï¼æ¯ä¸æ¬¾åè´¹ä¸å®ç¨çè²å½©ç¼è¾å¨ãå®å¯ä»¥å¸®å©ä½ ä»è²è½®æèå¶ä»å°æ¹çæä¸ç»åè°çè²å½©ãä½ å¯ä»¥å°è¿äºè²å½©åäº«ç»å¶ä»äººï¼æèåºç¨å°ä½ èªå·±çåä½å½ä¸­ãæ­¤å¤ï¼ä½ ä¹å¯ä»¥å°è²å½©ç»æèè²å½©ä»åºå¯¼åºä¸ºåç¬çè²å½©ææ¡£å¹¶å¯¼å¥å¶ä»è½¯ä»¶ä¸­ï¼å¦
+Adobe PhotoshopãGIMPãKritaãPencil 2D ä»¥åä¼å¨æ¼« Paint
+ç­ï¼ãç°ç«åäºå·å¯ä»¥å¨ WindowsãLinuxãmacOS
+ç­æä½ç³»ç»ä¸æ­£å¸¸è¿è¡ã # Table of Content * [Feature](#feature) *
 [Demo](#demo) * [Basic Functions](#basic-functions) * [Reference Colors]
 (#reference-colors) * [Color Palettes](#color-palettes) * [Export and Import
 Colors](#export-and-import-colors) * [Languages and Settings](#languages-and-
-settings) * [Reviews about Rickrack](#reviews-about-rickrack) * [User Comments]
-(#user-comments) * [Information](#information) * [Homepage](#homepage) *
-[Repository](#repository) * [Author](#author) * [Support](#support) *
-[Installation](#installation) * [Current Release](#current-release) * [Download
-Software](#download-software) * [Install Software](#install-software) *
-[Install Module](#install-module) * [Usage](#usage) * [How to Use the Software]
-(#how-to-use-the-software) * [How to Use the Module](#how-to-use-the-module) *
-[Development](#development) * [Install Requirement](#install-requirement) *
-[How to Build the Software](#how-to-build-the-software) * [How to Build the
-Module](#how-to-build-the-module) * [Copyright](#copyright) * [License]
-(#license) * [License for Rickrack](#license-for-rickrack) * [Acknowledgment]
-(#acknowledgment) # Introduction Colors enrich our world and affect our
-emotions. For artists, they display objects and convey feelings by varied
-colors in photos, images and drawings. For scientist, they present data by
-distinguishable colors in figures and graphics. However, the majority of color
-softwares and websites put restrictions on users, which include the inability
-to export color palettes into individual files, not providing invocation
-interfaces, requiring registrations, regional limitations and (or) collecting
-users' personal information. If you are running into these issues, Rickrack is
-the perfect solution for you! Rickrack is a free and user-friendly color
-editor. It is designed to generate a set of harmonious colors from the color
-wheel or other places. You can share these colors with your friends, or apply
-them into your creative works. You can store the color sets and color boards in
-the software, and access them whenever you need. What's more, you can export
-them into individual files, back them up, share them with others or import them
-in to other softwares such as Adobe Photoshop, GIMP, Krita, Pencil 2D and Clip
-Studio Paint. Rickrack, written in PySide2, operates effectively on Windows,
-Linux and other mainstream operating systems. Rickrack consists of two parts:
-the Rickrack software and the Rickrack module; the Rickrack software is
-designed for producing and organizing harmonious colors, and the Rickrack
-module is utilized for obtaining colors from the software in real-time, along
-with the plotting of images combined with other modules such as Matplotlib and
-Turtle.
-                                                            [->_Back_to_TOC_<-]
-# Feature Rickrack has several features: * A strong and free color editor. *
-Create a set of colors from the color wheel. * Pick-up a set of colors from an
-image. * Generate a color board from the color set. * Attach the color set and
-color board into the depot. * Import colors from elsewhere and manage them in
-depot. * Export colors and import them into other image processors. * Obtain
-colors through the Python module in real-time. * No function limitations and no
+settings) * [Reviews about Rickrack](#reviews-about-rickrack) * [Information]
+(#information) * [Homepage](#homepage) * [Repository](#repository) * [Author]
+(#author) * [Support](#support) * [Installation](#installation) * [Current
+Release](#current-release) * [Download Software](#download-software) * [Install
+Software](#install-software) * [Install Module](#install-module) * [Usage]
+(#usage) * [How to Use the Software](#how-to-use-the-software) * [How to Use
+the Module](#how-to-use-the-module) * [Development](#development) * [Install
+Requirement](#install-requirement) * [How to Build the Software](#how-to-build-
+the-software) * [How to Build the Module](#how-to-build-the-module) *
+[Copyright](#copyright) * [License](#license) * [License for Rickrack]
+(#license-for-rickrack) * [Acknowledgment](#acknowledgment) # Feature Rickrack
+has several features: * A strong and free color editor. * Create a set of
+colors from the color wheel. * Pick-up a set of colors from an image. *
+Generate a color board from the color set. * Attach the color set and color
+board into the depot. * Import colors from elsewhere and manage them in depot.
+* Export colors and import them into other image processors. * Obtain colors
+through the Python module in real-time. * No function limitations and no
 registration required. * ... and more!
                                                             [->_Back_to_TOC_<-]
 # Demo ## Basic Functions | | | | :---: | :---: | | ![](https://
 raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/000.gif) | ![]
 (https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/
 109.gif) | | Create a set of colors from the color wheel. | Pick-up a set of
 colors from an image. (Image inside: [Copyright (c) 2001 Studio Ghibli](https:/
@@ -84,74 +73,46 @@
 Convert: gradient palette ↔ fixed palette. | Convert: gradient palette ↔
 reference palette. | | ![](https://raw.githubusercontent.com/eigenmiao/
 Rickrack/master/demo/usage/700.gif) | ![](https://raw.githubusercontent.com/
 eigenmiao/Rickrack/master/demo/usage/701.gif) | | Fixed palette: Chinese
 Traditional Colors. (Color Names: [Copyright (c) China Science Publishing &
 Media Ltd.](http://zhongguose.com/), Non-Commercial Usage) | Fixed palette:
 Nippon Traditional Colors. (Color Names: [Copyright (c) PIE BOOKS.](http://
-nipponcolors.com/), Non-Commercial Usage) | ## Export and Import Colors | | | |
-:---: | :---: | | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/
-master/demo/usage/704.gif) | ![](https://raw.githubusercontent.com/eigenmiao/
-Rickrack/master/demo/usage/702.gif) | | Export colors into a Rickrack file. |
-Export colors into a Adobe swatch file. | | ![](https://
-raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/705.gif) | ![]
-(https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/
-703.gif) | | Import colors from a Rickrack file. | Import colors from a Adobe
-swatch file. | ## Languages and Settings | | | | :---: | :---: | | ![](https://
-raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/707.gif) | ![]
-(https://raw.githubusercontent.com/eigenmiao/Rickrack/master/demo/usage/
-706.gif) | | Support multiple languages, including Chinese, English, Japanese,
-German, French, Russian, and so on. (Languages except Chinese and English are
-translated by [Google Translate](https://translate.google.cn/).) | Support
-multiple interface themes. | ## Notice * The interface display in demo uses
-[LXGWWenKai (SIL Open Font License)](https://lxgw.github.io/2021/01/28/Klee-
-Simpchin/) font.
+nipponcolors.com/), Non-Commercial Usage) | ## Languages and Settings | | | | :
+---: | :---: | | ![](https://raw.githubusercontent.com/eigenmiao/Rickrack/
+master/demo/usage/707.gif) | ![](https://raw.githubusercontent.com/eigenmiao/
+Rickrack/master/demo/usage/706.gif) | | Support multiple languages, including
+Chinese, English, Japanese, German, French, Russian, and so on. (Languages
+except Chinese and English are translated by [Google Translate](https://
+translate.google.cn/).) | Support multiple interface themes. | ## Notice * The
+interface display in demo uses [LXGWWenKai (SIL Open Font License)](https://
+lxgw.github.io/2021/01/28/Klee-Simpchin/) font.
                                                             [->_Back_to_TOC_<-]
 # Reviews about Rickrack > All in all, Rickrack is a comprehensive tool for
 anything that requires color work. Experienced users have an exhaustive toolset
 to work with, while a more casual audience can improve the presentation of
 their art by quickly getting color synergy ideas. -- [Robert Condorache @
 Softpedia](https://www.softpedia.com/get/Multimedia/Graphic/Graphic-Others/
 RickRack.shtml) > Rickrack is an easy to use desktop app for creating and
 saving color palettes. It supports many major color palette formats for import
 and export, and is a great tool for generating color palettes of colors that go
 well together. -- [TJ FREE @ Youtube](https://www.youtube.com/
 watch?v=OUnktTCtv3E) > ... and more!
                                                             [->_Back_to_TOC_<-]
-# User Comments >
-ä½ä¸ºä¸ä¸ªéè²è½¯ä»¶ï¼å®æ¬èº«çè²å½©ï¼å¯ï¼è¶³å¤æè³...ä½ å®å¨å¯ä»¥ä¿¡å¾è¿ä½èã
--- User from [Open Source China](https://www.oschina.net/comment/news/231426) >
-å¾æ£ï¼æ¯ä¸ä¸ªä¸å¯å¤å¾çå·¥å·ã -- User from [Bilibili](https://
-www.bilibili.com/video/BV1VD4y157tX/) >
-è°¢è°¢åäº«ï¼è¯´æåçå¤ªè¯¦ç»äºã -- User from [Baidu Tieba](https://
-tieba.baidu.com/p/8253007907) > Thanks a mil! All of my pallette creators were
-online. This a good offline tool to have with some additional features too. -
-- User from [Youtube](https://www.youtube.com/watch?v=OUnktTCtv3E) > I don't
-like online-apps, so this is a huge plus from the get-go. Thanks for sharing
-this great tool. -- User from [Youtube](https://www.youtube.com/
-watch?v=OUnktTCtv3E) > Thanks for sharing this! And - did I notice correctly
-that you are also the author of this software? This looks super exciting,
-canât wait to investigate it more! -- User from [Krita Artists](https://
-krita-artists.org/t/alternatives-to-adobe-color-rickrack/60041) > Hello, your
-software (the deb package) runs fine on Xubuntu 22.04 and is quite impressive!
-Thanks for sharing. Next step is to study some tutorials. -- User from
-[PIXLS.US](https://discuss.pixls.us/t/alternatives-to-adobe-color-rickrack/
-35997) > ... and more!
-                                                            [->_Back_to_TOC_<-]
 # Information ## Homepage https://eigenmiao.com/rickrack/ ## Repository https:/
 /github.com/eigenmiao/Rickrack ## Author [Eigenmiao](mailto:
 eigenmiao@outlook.com) ## Support [Support the Future of Rickrack!](https://
 afdian.net/a/eigenmiao)
                                                             [->_Back_to_TOC_<-]
-# Installation ## Current Release The latest preview version is [v2.7.25]
-(https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.25). ## Install
+# Installation ## Current Release The latest preview version is [v2.7.26]
+(https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.26). ## Install
 Software ### Recommend: Install on Windows 10 or 11 via WinGet tool ``` winget
 install rickrack ``` ## Install on other platforms Download Software from
-[Github](https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.25) or
-[Sourceforge](https://sourceforge.net/projects/rickrack/files/v2.7.25/). The
+[Github](https://github.com/eigenmiao/Rickrack/releases/tag/v2.7.26) or
+[Sourceforge](https://sourceforge.net/projects/rickrack/files/v2.7.26/). The
 installation steps are presented in [tutorials](https://eigenmiao.com/2021/12/
 12/rickrack-tutorial-en-v2.3.4/#Installation). Here is a [video tutorial]
 (https://www.bilibili.com/video/BV17r4y1L7R6/). ## Install Module Install the
 latest [Rickrack](https://pypi.org/project/Rickrack/) from PyPI! ```Bash #
 Install Rickrack. pip install Rickrack # Start the installed software. rickrack
 -d "/PATH/TO/RICKRACK/SOFTWARE" ```
                                                             [->_Back_to_TOC_<-]
@@ -200,15 +161,15 @@
 specimen/Noto+Serif) ([SC](https://fonts.google.com/specimen/Noto+Serif+SC))
 fonts and [Noto Sans](https://fonts.google.com/specimen/Noto+Sans) ([SC](https:
 //fonts.google.com/specimen/Noto+Sans+SC)) fonts for interface display, which
 are designed by Google and published in website [Google Fonts](https://
 fonts.google.com/). These fonts are open-sourced under [Apache 2.0](http://
 www.apache.org/licenses/) and [SIL Open Font License 1.1](http://
 scripts.sil.org/OFL), respectively. # Acknowledgment * The Rickrack software is
-written in [Python](https://www.python.org/), constructed based on [PySide2]
+written in [Python](https://www.python.org/), constructed based on [PyQt5]
 (https://www.qt.io/qt-for-python) and packed up by [fbs (free edition)](https:/
 /build-system.fman.io/). * The localization (l10n) and internationalization
 (i18n) of Rickrack is based on [Google Translate](https://translate.google.cn/
 ) and [Microsoft Translator](https://cn.bing.com/translator), deployed on
 [POEditor](https://poeditor.com/join/project?hash=kBeQjfxCES). * The code
 repository is deposited on [Github](https://github.com/eigenmiao/Rickrack) and
 [Gitee](https://gitee.com/eigenmiao/Rickrack).
```

### Comparing `Rickrack-2.7.25/setup.py` & `Rickrack-2.7.26/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """
 
 from setuptools import setup
 
 
 setup(
     name="Rickrack",
-    version="2.7.25",
+    version="2.7.26",
     author="Eigenmiao",
     author_email="eigenmiao@outlook.com",
     description="Generate harmonious colors freely.",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://eigenmiao.github.io/rickrack/",
     classifiers=[
```

