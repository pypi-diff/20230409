# Comparing `tmp/QtPy-Frameless-Window-0.0.1.tar.gz` & `tmp/QtPy-Frameless-Window-0.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QtPy-Frameless-Window-0.0.1.tar", last modified: Sun Apr  9 14:05:32 2023, max compression
+gzip compressed data, was "QtPy-Frameless-Window-0.0.2.dev0.tar", last modified: Sun Apr  9 15:41:51 2023, max compression
```

## Comparing `QtPy-Frameless-Window-0.0.1.tar` & `QtPy-Frameless-Window-0.0.2.dev0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35823 2023-04-09 13:19:55.238828 QtPy-Frameless-Window-0.0.1/LICENSE
--rw-r--r--   0        0        0     1027 2023-04-09 14:04:05.976016 QtPy-Frameless-Window-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1801 2023-04-09 13:19:55.242550 QtPy-Frameless-Window-0.0.1/qtframelesswindow/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 13:19:55.243556 QtPy-Frameless-Window-0.0.1/qtframelesswindow/_rc/__init__.py
--rw-r--r--   0        0        0     2726 2023-04-09 13:19:55.243556 QtPy-Frameless-Window-0.0.1/qtframelesswindow/_rc/resource.py
--rw-r--r--   0        0        0      135 2023-04-09 13:19:55.244615 QtPy-Frameless-Window-0.0.1/qtframelesswindow/_rc/resource.qrc
--rw-r--r--   0        0        0     1471 2023-04-09 13:19:55.244615 QtPy-Frameless-Window-0.0.1/qtframelesswindow/_rc/resource_rc.py
--rw-r--r--   0        0        0      270 2023-04-09 13:19:55.245818 QtPy-Frameless-Window-0.0.1/qtframelesswindow/_rc/title_bar/close.svg
--rw-r--r--   0        0        0     3107 2023-04-09 13:19:55.247833 QtPy-Frameless-Window-0.0.1/qtframelesswindow/linux/__init__.py
--rw-r--r--   0        0        0     2920 2023-04-09 13:19:55.247833 QtPy-Frameless-Window-0.0.1/qtframelesswindow/linux/window_effect.py
--rw-r--r--   0        0        0     3013 2023-04-09 13:19:55.248829 QtPy-Frameless-Window-0.0.1/qtframelesswindow/mac/__init__.py
--rw-r--r--   0        0        0     4093 2023-04-09 13:19:55.249828 QtPy-Frameless-Window-0.0.1/qtframelesswindow/mac/window_effect.py
--rw-r--r--   0        0        0     4981 2023-04-09 13:19:55.250827 QtPy-Frameless-Window-0.0.1/qtframelesswindow/titlebar/__init__.py
--rw-r--r--   0        0        0     9024 2023-04-09 13:19:55.250827 QtPy-Frameless-Window-0.0.1/qtframelesswindow/titlebar/title_bar_buttons.py
--rw-r--r--   0        0        0      885 2023-04-09 13:19:55.251827 QtPy-Frameless-Window-0.0.1/qtframelesswindow/utils/__init__.py
--rw-r--r--   0        0        0      533 2023-04-09 13:19:55.252830 QtPy-Frameless-Window-0.0.1/qtframelesswindow/utils/api_differ.py
--rw-r--r--   0        0        0     5296 2023-04-09 13:19:55.252830 QtPy-Frameless-Window-0.0.1/qtframelesswindow/utils/linux_utils.py
--rw-r--r--   0        0        0     1848 2023-04-09 13:19:55.254337 QtPy-Frameless-Window-0.0.1/qtframelesswindow/utils/mac_utils.py
--rw-r--r--   0        0        0     7814 2023-04-09 13:19:55.254337 QtPy-Frameless-Window-0.0.1/qtframelesswindow/utils/win32_utils.py
--rw-r--r--   0        0        0     8675 2023-04-09 13:19:55.255349 QtPy-Frameless-Window-0.0.1/qtframelesswindow/windows/__init__.py
--rw-r--r--   0        0        0     4261 2023-04-09 13:19:55.256379 QtPy-Frameless-Window-0.0.1/qtframelesswindow/windows/c_structures.py
--rw-r--r--   0        0        0     8977 2023-04-09 13:19:55.256379 QtPy-Frameless-Window-0.0.1/qtframelesswindow/windows/window_effect.py
--rw-r--r--   0        0        0     1467 2023-04-09 14:03:15.339643 QtPy-Frameless-Window-0.0.1/README.md
--rw-r--r--   0        0        0     1937 1970-01-01 00:00:00.000000 QtPy-Frameless-Window-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-04-09 13:19:55.238828 QtPy-Frameless-Window-0.0.2.dev0/LICENSE
+-rw-r--r--   0        0        0      872 2023-04-09 15:39:35.842902 QtPy-Frameless-Window-0.0.2.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1811 2023-04-09 15:30:40.737482 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-09 13:19:55.243556 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/_rc/__init__.py
+-rw-r--r--   0        0        0     2726 2023-04-09 13:19:55.243556 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/_rc/resource.py
+-rw-r--r--   0        0        0      135 2023-04-09 13:19:55.244615 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/_rc/resource.qrc
+-rw-r--r--   0        0        0     1471 2023-04-09 13:19:55.244615 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/_rc/resource_rc.py
+-rw-r--r--   0        0        0      270 2023-04-09 13:19:55.245818 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/_rc/title_bar/close.svg
+-rw-r--r--   0        0        0     3107 2023-04-09 15:30:12.853686 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/linux/__init__.py
+-rw-r--r--   0        0        0     2920 2023-04-09 15:30:12.854739 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/linux/window_effect.py
+-rw-r--r--   0        0        0     3013 2023-04-09 15:30:12.856021 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/mac/__init__.py
+-rw-r--r--   0        0        0     4093 2023-04-09 15:30:12.856021 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/mac/window_effect.py
+-rw-r--r--   0        0        0     4981 2023-04-09 13:19:55.250827 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/titlebar/__init__.py
+-rw-r--r--   0        0        0     9024 2023-04-09 13:19:55.250827 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/titlebar/title_bar_buttons.py
+-rw-r--r--   0        0        0      885 2023-04-09 13:19:55.251827 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/utils/__init__.py
+-rw-r--r--   0        0        0      457 2023-04-09 15:31:56.716491 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/utils/api_differ.py
+-rw-r--r--   0        0        0     5296 2023-04-09 15:30:12.857623 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/utils/linux_utils.py
+-rw-r--r--   0        0        0     1848 2023-04-09 15:30:12.858697 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/utils/mac_utils.py
+-rw-r--r--   0        0        0     7814 2023-04-09 13:19:55.254337 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/utils/win32_utils.py
+-rw-r--r--   0        0        0     8675 2023-04-09 15:30:12.858697 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/windows/__init__.py
+-rw-r--r--   0        0        0     4261 2023-04-09 13:19:55.256379 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/windows/c_structures.py
+-rw-r--r--   0        0        0     8977 2023-04-09 13:19:55.256379 QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/windows/window_effect.py
+-rw-r--r--   0        0        0     1858 2023-04-09 15:38:49.563994 QtPy-Frameless-Window-0.0.2.dev0/README.md
+-rw-r--r--   0        0        0     2327 1970-01-01 00:00:00.000000 QtPy-Frameless-Window-0.0.2.dev0/PKG-INFO
```

### Comparing `QtPy-Frameless-Window-0.0.1/LICENSE` & `QtPy-Frameless-Window-0.0.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.1/pyproject.toml` & `QtPy-Frameless-Window-0.0.2.dev0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,8 @@
-[[tool.pdm.autoexport]]
-filename = "requirements.txt"
-groups = [
-    "default",
-]
-without_hashes = true
-
-[[tool.pdm.autoexport]]
-filename = "setup.py"
-format = "setuppy"
+[tool.pdm]
 
 [project]
 authors = [
     { name = "TaoChenyue", email = "3038816978@qq.com" },
 ]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -28,15 +19,15 @@
 description = "A cross-platform frameless window based on QtPy."
 keywords = [
     "pyqt frameless",
 ]
 name = "QtPy-Frameless-Window"
 readme = "README.md"
 requires-python = ">=3.6"
-version = "0.0.1"
+version = "0.0.2-dev"
 
 [project.license]
 text = "GPLv3"
 
 [project.urls]
 Homepage = "https://github.com/TaoChenyue/QtPy-Frameless-Window.git"
```

### Comparing `QtPy-Frameless-Window-0.0.1/qtframelesswindow/__init__.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 def set_qt_api(api:str=None,parse:bool=False):
     if parse:
         parser = argparse.ArgumentParser(description='Set Qt API')
         parser.add_argument('--api', type=str)
         args = parser.parse_args()
         if args.api is not None:
             api=args.api
+        return args
     if api is None:
         api="pyqt5"
     os.environ["QT_API"]=api
-    return args
+    
 set_qt_api(parse=True)
 
 from .titlebar import TitleBar, TitleBarButton, SvgTitleBarButton, StandardTitleBar
 from qtpy.QtWidgets import QDialog,QMainWindow
 import sys
 if sys.platform == "win32":
     from .windows import AcrylicWindow
```

### Comparing `QtPy-Frameless-Window-0.0.1/qtframelesswindow/_rc/resource.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.1/qtframelesswindow/_rc/resource_rc.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/_rc/resource_rc.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.1/qtframelesswindow/linux/__init__.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.1/qtframelesswindow/linux/window_effect.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/linux/window_effect.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.1/qtframelesswindow/mac/__init__.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.1/qtframelesswindow/mac/window_effect.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/mac/window_effect.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.1/qtframelesswindow/titlebar/__init__.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.1/qtframelesswindow/titlebar/title_bar_buttons.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.1/qtframelesswindow/utils/__init__.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.1/qtframelesswindow/utils/linux_utils.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.1/qtframelesswindow/utils/mac_utils.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.1/qtframelesswindow/utils/win32_utils.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.1/qtframelesswindow/windows/__init__.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.1/qtframelesswindow/windows/c_structures.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.1/qtframelesswindow/windows/window_effect.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/windows/window_effect.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.1/README.md` & `QtPy-Frameless-Window-0.0.2.dev0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-<div align=center>
+<div align="center">
 
 # QtPy-Frameless-Window
 
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
+[![Downloads](https://static.pepy.tech/badge/qtpy-frameless-window)](https://pepy.tech/project/qtpy-frameless-window)
+![GitHub](https://img.shields.io/github/license/TaoChenyue/Qtpy-Frameless-Window?style=plastic)
 
 A cross-platform frameless window based on QtPy.
 
 </div>
 
 This repo is based on *QtPy* and [PyQt-Frameless-Window](https://github.com/zhiyiYo/PyQt-Frameless-Window). Due to library in diffrent *PyQt-Frameless-Window* branches cannot exist in one virtual environment, I created this repository by adding *QtPy* dependence and modifying some modules. This repo will keep up with *PyQt-Frameless-Window*.
 
@@ -47,9 +49,12 @@
 
 
 if __name__ == "__main__":
     app = QApplication([])
     demo = Window()
     demo.show()
     app.exec_()
+```
 
-```
+## FQ
+Q: Why acrylic window response slowly when dragging its edge on Windows platform?
+A: Reference to https://www.cnblogs.com/zhiyiYo/p/14659981.html, change settings.
```

### Comparing `QtPy-Frameless-Window-0.0.1/PKG-INFO` & `QtPy-Frameless-Window-0.0.2.dev0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: QtPy-Frameless-Window
-Version: 0.0.1
+Version: 0.0.2-dev
 Summary: A cross-platform frameless window based on QtPy.
 License: GPLv3
 Keywords: pyqt frameless
 Author-email: TaoChenyue <3038816978@qq.com>
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/TaoChenyue/QtPy-Frameless-Window.git
 Description-Content-Type: text/markdown
 
-<div align=center>
+<div align="center">
 
 # QtPy-Frameless-Window
 
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
+[![Downloads](https://static.pepy.tech/badge/qtpy-frameless-window)](https://pepy.tech/project/qtpy-frameless-window)
+![GitHub](https://img.shields.io/github/license/TaoChenyue/Qtpy-Frameless-Window?style=plastic)
 
 A cross-platform frameless window based on QtPy.
 
 </div>
 
 This repo is based on *QtPy* and [PyQt-Frameless-Window](https://github.com/zhiyiYo/PyQt-Frameless-Window). Due to library in diffrent *PyQt-Frameless-Window* branches cannot exist in one virtual environment, I created this repository by adding *QtPy* dependence and modifying some modules. This repo will keep up with *PyQt-Frameless-Window*.
 
@@ -61,9 +63,12 @@
 
 
 if __name__ == "__main__":
     app = QApplication([])
     demo = Window()
     demo.show()
     app.exec_()
-
 ```
+
+## FQ
+Q: Why acrylic window response slowly when dragging its edge on Windows platform?
+A: Reference to https://www.cnblogs.com/zhiyiYo/p/14659981.html, change settings.
```

