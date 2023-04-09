# Comparing `tmp/canvasdl-1.4.8.tar.gz` & `tmp/canvasdl-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canvasdl-1.4.8.tar", last modified: Thu Feb 23 17:01:25 2023, max compression
+gzip compressed data, was "canvasdl-1.4.9.tar", last modified: Thu Feb 23 17:23:33 2023, max compression
```

## Comparing `canvasdl-1.4.8.tar` & `canvasdl-1.4.9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:01:25.725299 canvasdl-1.4.8/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1069 2023-02-23 16:28:33.000000 canvasdl-1.4.8/LICENSE
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2178 2023-02-23 17:01:25.725299 canvasdl-1.4.8/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1827 2023-02-23 16:28:33.000000 canvasdl-1.4.8/README.md
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:01:25.717299 canvasdl-1.4.8/canvasdl/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       76 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/__init__.py
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:01:25.717299 canvasdl-1.4.8/canvasdl/asset_types/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      195 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/asset_types/__init__.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2673 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/asset_types/assignment.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      846 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/asset_types/base.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     4625 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/asset_types/canvas.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1043 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/asset_types/course.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1781 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/asset_types/edstem.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      436 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/asset_types/gradescope.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1749 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/asset_types/piazza.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      634 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/asset_types/section.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     3001 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/asset_types/streams.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1976 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/asset_types/video.py
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:01:25.713299 canvasdl-1.4.8/canvasdl/assets/
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:01:25.717299 canvasdl-1.4.8/canvasdl/assets/templates/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      262 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/assets/templates/announ.css
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:01:25.721299 canvasdl-1.4.8/canvasdl/checkers/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      222 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/checkers/__init__.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1474 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/checkers/announ.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2867 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/checkers/base.py
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:01:25.721299 canvasdl-1.4.8/canvasdl/checkers/canvas/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      156 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/checkers/canvas/__init__.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1122 2023-02-23 16:59:02.000000 canvasdl-1.4.8/canvasdl/checkers/canvas/announ.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      395 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/checkers/canvas/assignment.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      233 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/checkers/canvas/base.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1554 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/checkers/canvas/files.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1582 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/checkers/canvas/tab.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     3576 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/checkers/canvas/videos.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      476 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/checkers/drive.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2998 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/checkers/edstem.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1476 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/checkers/gradescope.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1051 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/checkers/piazza.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     5284 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/checkers/website.py
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:01:25.721299 canvasdl-1.4.8/canvasdl/core/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       27 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/core/__init__.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      207 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/core/checkservice.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      112 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/core/client.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      282 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/core/courseinfo.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     4260 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/core/coursemaker.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      221 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/core/main.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      601 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/core/starter.py
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:01:25.721299 canvasdl-1.4.8/canvasdl/ui/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        0 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/ui/__init__.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2606 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/ui/downloadprogress.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     3625 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/ui/popup.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      398 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/ui/progressbar.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2007 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/ui/progressmanager.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      132 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/ui/silentpopup.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1378 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/ui/userinterface.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      869 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/ui/widget.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2117 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/ui/widgetui.py
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:01:25.725299 canvasdl-1.4.8/canvasdl/utils/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       98 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/utils/__init__.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      577 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/utils/announcements.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      419 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/utils/argparser.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1216 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/utils/calendar.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      877 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/utils/config.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1947 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/utils/configchecker.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     3010 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/utils/configmaker.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      730 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/utils/path.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      424 2023-02-23 16:28:33.000000 canvasdl-1.4.8/canvasdl/utils/time.py
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:01:25.717299 canvasdl-1.4.8/canvasdl.egg-info/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2178 2023-02-23 17:01:25.000000 canvasdl-1.4.8/canvasdl.egg-info/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1779 2023-02-23 17:01:25.000000 canvasdl-1.4.8/canvasdl.egg-info/SOURCES.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        1 2023-02-23 17:01:25.000000 canvasdl-1.4.8/canvasdl.egg-info/dependency_links.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       91 2023-02-23 17:01:25.000000 canvasdl-1.4.8/canvasdl.egg-info/entry_points.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      335 2023-02-23 17:01:25.000000 canvasdl-1.4.8/canvasdl.egg-info/requires.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        9 2023-02-23 17:01:25.000000 canvasdl-1.4.8/canvasdl.egg-info/top_level.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       79 2023-02-23 17:01:25.725299 canvasdl-1.4.8/setup.cfg
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1057 2023-02-23 17:00:24.000000 canvasdl-1.4.8/setup.py
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:23:33.580270 canvasdl-1.4.9/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1069 2023-02-23 16:28:33.000000 canvasdl-1.4.9/LICENSE
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2458 2023-02-23 17:23:33.580270 canvasdl-1.4.9/PKG-INFO
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2107 2023-02-23 17:21:09.000000 canvasdl-1.4.9/README.md
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:23:33.568270 canvasdl-1.4.9/canvasdl/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       76 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/__init__.py
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:23:33.572270 canvasdl-1.4.9/canvasdl/asset_types/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      195 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/asset_types/__init__.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2673 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/asset_types/assignment.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      846 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/asset_types/base.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     4625 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/asset_types/canvas.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1043 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/asset_types/course.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1781 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/asset_types/edstem.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      436 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/asset_types/gradescope.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1749 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/asset_types/piazza.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      634 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/asset_types/section.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     3001 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/asset_types/streams.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1976 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/asset_types/video.py
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:23:33.564270 canvasdl-1.4.9/canvasdl/assets/
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:23:33.572270 canvasdl-1.4.9/canvasdl/assets/templates/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      262 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/assets/templates/announ.css
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:23:33.572270 canvasdl-1.4.9/canvasdl/checkers/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      222 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/checkers/__init__.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1474 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/checkers/announ.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2867 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/checkers/base.py
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:23:33.572270 canvasdl-1.4.9/canvasdl/checkers/canvas/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      156 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/checkers/canvas/__init__.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1122 2023-02-23 16:59:02.000000 canvasdl-1.4.9/canvasdl/checkers/canvas/announ.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      395 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/checkers/canvas/assignment.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      233 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/checkers/canvas/base.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1554 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/checkers/canvas/files.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1582 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/checkers/canvas/tab.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     3576 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/checkers/canvas/videos.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      476 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/checkers/drive.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2998 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/checkers/edstem.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1476 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/checkers/gradescope.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1051 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/checkers/piazza.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     5284 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/checkers/website.py
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:23:33.576270 canvasdl-1.4.9/canvasdl/core/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       27 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/core/__init__.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      207 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/core/checkservice.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      112 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/core/client.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      282 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/core/courseinfo.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     4260 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/core/coursemaker.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      221 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/core/main.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      601 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/core/starter.py
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:23:33.576270 canvasdl-1.4.9/canvasdl/ui/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        0 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/ui/__init__.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2606 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/ui/downloadprogress.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     3625 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/ui/popup.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      398 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/ui/progressbar.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2007 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/ui/progressmanager.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      132 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/ui/silentpopup.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1378 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/ui/userinterface.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      869 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/ui/widget.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2117 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/ui/widgetui.py
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:23:33.580270 canvasdl-1.4.9/canvasdl/utils/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       98 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/utils/__init__.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      577 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/utils/announcements.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      419 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/utils/argparser.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1216 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/utils/calendar.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      877 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/utils/config.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1947 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/utils/configchecker.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     3010 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/utils/configmaker.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      730 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/utils/path.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      424 2023-02-23 16:28:33.000000 canvasdl-1.4.9/canvasdl/utils/time.py
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-02-23 17:23:33.568270 canvasdl-1.4.9/canvasdl.egg-info/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2458 2023-02-23 17:23:33.000000 canvasdl-1.4.9/canvasdl.egg-info/PKG-INFO
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1779 2023-02-23 17:23:33.000000 canvasdl-1.4.9/canvasdl.egg-info/SOURCES.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        1 2023-02-23 17:23:33.000000 canvasdl-1.4.9/canvasdl.egg-info/dependency_links.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       91 2023-02-23 17:23:33.000000 canvasdl-1.4.9/canvasdl.egg-info/entry_points.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      335 2023-02-23 17:23:33.000000 canvasdl-1.4.9/canvasdl.egg-info/requires.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        9 2023-02-23 17:23:33.000000 canvasdl-1.4.9/canvasdl.egg-info/top_level.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       79 2023-02-23 17:23:33.580270 canvasdl-1.4.9/setup.cfg
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1057 2023-02-23 17:23:16.000000 canvasdl-1.4.9/setup.py
```

### Comparing `canvasdl-1.4.8/LICENSE` & `canvasdl-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/PKG-INFO` & `canvasdl-1.4.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: canvasdl
-Version: 1.4.8
+Version: 1.4.9
 Summary: course content synchronizer
 Home-page: https://github.com/quintenroets/canvasdl
-Download-URL: https://github.com/quintenroets/canvasdl/archive/refs/tags/v1.4.8.tar.gz
+Download-URL: https://github.com/quintenroets/canvasdl/archive/refs/tags/v1.4.9.tar.gz
 Author: Quinten Roets
 Author-email: quinten.roets@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Canvasdl
 
@@ -62,7 +62,11 @@
    - pip install PyQt6
 
 ## Usage
 Run command to synchronize all content and check for updates
 ```shell
 canvasdl
 ```
+
+## Quickstart
+To quickly experiment with the package you can run the [quickstart](https://github.com/quintenroets/canvasdl/blob/main/examples/quickstart.ipynb) in Google Collab.
+The downloaded content will be available in the folder /root/Documents in the Google Collab session.
```

### Comparing `canvasdl-1.4.8/README.md` & `canvasdl-1.4.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -51,7 +51,11 @@
    - pip install PyQt6
 
 ## Usage
 Run command to synchronize all content and check for updates
 ```shell
 canvasdl
 ```
+
+## Quickstart
+To quickly experiment with the package you can run the [quickstart](https://github.com/quintenroets/canvasdl/blob/main/examples/quickstart.ipynb) in Google Collab.
+The downloaded content will be available in the folder /root/Documents in the Google Collab session.
```

### Comparing `canvasdl-1.4.8/canvasdl/asset_types/assignment.py` & `canvasdl-1.4.9/canvasdl/asset_types/assignment.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/asset_types/base.py` & `canvasdl-1.4.9/canvasdl/asset_types/base.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/asset_types/canvas.py` & `canvasdl-1.4.9/canvasdl/asset_types/canvas.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/asset_types/course.py` & `canvasdl-1.4.9/canvasdl/asset_types/course.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/asset_types/edstem.py` & `canvasdl-1.4.9/canvasdl/asset_types/edstem.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/asset_types/piazza.py` & `canvasdl-1.4.9/canvasdl/asset_types/piazza.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/asset_types/section.py` & `canvasdl-1.4.9/canvasdl/asset_types/section.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/asset_types/streams.py` & `canvasdl-1.4.9/canvasdl/asset_types/streams.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/asset_types/video.py` & `canvasdl-1.4.9/canvasdl/asset_types/video.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/checkers/announ.py` & `canvasdl-1.4.9/canvasdl/checkers/announ.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/checkers/base.py` & `canvasdl-1.4.9/canvasdl/checkers/base.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/checkers/canvas/announ.py` & `canvasdl-1.4.9/canvasdl/checkers/canvas/announ.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/checkers/canvas/files.py` & `canvasdl-1.4.9/canvasdl/checkers/canvas/files.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/checkers/canvas/tab.py` & `canvasdl-1.4.9/canvasdl/checkers/canvas/tab.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/checkers/canvas/videos.py` & `canvasdl-1.4.9/canvasdl/checkers/canvas/videos.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/checkers/edstem.py` & `canvasdl-1.4.9/canvasdl/checkers/edstem.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/checkers/gradescope.py` & `canvasdl-1.4.9/canvasdl/checkers/gradescope.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/checkers/piazza.py` & `canvasdl-1.4.9/canvasdl/checkers/piazza.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/checkers/website.py` & `canvasdl-1.4.9/canvasdl/checkers/website.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/core/coursemaker.py` & `canvasdl-1.4.9/canvasdl/core/coursemaker.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/core/starter.py` & `canvasdl-1.4.9/canvasdl/core/starter.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/ui/downloadprogress.py` & `canvasdl-1.4.9/canvasdl/ui/downloadprogress.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/ui/popup.py` & `canvasdl-1.4.9/canvasdl/ui/popup.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/ui/progressmanager.py` & `canvasdl-1.4.9/canvasdl/ui/progressmanager.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/ui/userinterface.py` & `canvasdl-1.4.9/canvasdl/ui/userinterface.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/ui/widget.py` & `canvasdl-1.4.9/canvasdl/ui/widget.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/ui/widgetui.py` & `canvasdl-1.4.9/canvasdl/ui/widgetui.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/utils/announcements.py` & `canvasdl-1.4.9/canvasdl/utils/announcements.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/utils/calendar.py` & `canvasdl-1.4.9/canvasdl/utils/calendar.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/utils/config.py` & `canvasdl-1.4.9/canvasdl/utils/config.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/utils/configchecker.py` & `canvasdl-1.4.9/canvasdl/utils/configchecker.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/utils/configmaker.py` & `canvasdl-1.4.9/canvasdl/utils/configmaker.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl/utils/path.py` & `canvasdl-1.4.9/canvasdl/utils/path.py`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/canvasdl.egg-info/PKG-INFO` & `canvasdl-1.4.9/canvasdl.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: canvasdl
-Version: 1.4.8
+Version: 1.4.9
 Summary: course content synchronizer
 Home-page: https://github.com/quintenroets/canvasdl
-Download-URL: https://github.com/quintenroets/canvasdl/archive/refs/tags/v1.4.8.tar.gz
+Download-URL: https://github.com/quintenroets/canvasdl/archive/refs/tags/v1.4.9.tar.gz
 Author: Quinten Roets
 Author-email: quinten.roets@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Canvasdl
 
@@ -62,7 +62,11 @@
    - pip install PyQt6
 
 ## Usage
 Run command to synchronize all content and check for updates
 ```shell
 canvasdl
 ```
+
+## Quickstart
+To quickly experiment with the package you can run the [quickstart](https://github.com/quintenroets/canvasdl/blob/main/examples/quickstart.ipynb) in Google Collab.
+The downloaded content will be available in the folder /root/Documents in the Google Collab session.
```

### Comparing `canvasdl-1.4.8/canvasdl.egg-info/SOURCES.txt` & `canvasdl-1.4.9/canvasdl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `canvasdl-1.4.8/setup.py` & `canvasdl-1.4.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 NAME = "canvasdl"
-version = "1.4.8"
+version = "1.4.9"
 
 
 def read(filename):
     try:
         with open(filename) as fp:
             content = fp.readlines()
     except FileNotFoundError:
```

