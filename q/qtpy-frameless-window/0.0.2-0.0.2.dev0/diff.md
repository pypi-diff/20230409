# Comparing `tmp/QtPy-Frameless-Window-0.0.2.tar.gz` & `tmp/QtPy-Frameless-Window-0.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QtPy-Frameless-Window-0.0.2.tar", last modified: Sun Apr  9 15:46:34 2023, max compression
+gzip compressed data, was "QtPy-Frameless-Window-0.0.2.dev0.tar", last modified: Sun Apr  9 15:41:51 2023, max compression
```

## Comparing `QtPy-Frameless-Window-0.0.2.tar` & `QtPy-Frameless-Window-0.0.2.dev0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35823 2023-04-09 13:19:55.238828 QtPy-Frameless-Window-0.0.2/LICENSE
--rw-r--r--   0        0        0      868 2023-04-09 15:46:10.751484 QtPy-Frameless-Window-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1811 2023-04-09 15:30:40.737482 QtPy-Frameless-Window-0.0.2/qtframelesswindow/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 13:19:55.243556 QtPy-Frameless-Window-0.0.2/qtframelesswindow/_rc/__init__.py
--rw-r--r--   0        0        0     2726 2023-04-09 13:19:55.243556 QtPy-Frameless-Window-0.0.2/qtframelesswindow/_rc/resource.py
--rw-r--r--   0        0        0      135 2023-04-09 13:19:55.244615 QtPy-Frameless-Window-0.0.2/qtframelesswindow/_rc/resource.qrc
--rw-r--r--   0        0        0     1471 2023-04-09 13:19:55.244615 QtPy-Frameless-Window-0.0.2/qtframelesswindow/_rc/resource_rc.py
--rw-r--r--   0        0        0      270 2023-04-09 13:19:55.245818 QtPy-Frameless-Window-0.0.2/qtframelesswindow/_rc/title_bar/close.svg
--rw-r--r--   0        0        0     3107 2023-04-09 15:30:12.853686 QtPy-Frameless-Window-0.0.2/qtframelesswindow/linux/__init__.py
--rw-r--r--   0        0        0     2920 2023-04-09 15:30:12.854739 QtPy-Frameless-Window-0.0.2/qtframelesswindow/linux/window_effect.py
--rw-r--r--   0        0        0     3013 2023-04-09 15:30:12.856021 QtPy-Frameless-Window-0.0.2/qtframelesswindow/mac/__init__.py
--rw-r--r--   0        0        0     4093 2023-04-09 15:30:12.856021 QtPy-Frameless-Window-0.0.2/qtframelesswindow/mac/window_effect.py
--rw-r--r--   0        0        0     4981 2023-04-09 13:19:55.250827 QtPy-Frameless-Window-0.0.2/qtframelesswindow/titlebar/__init__.py
--rw-r--r--   0        0        0     9024 2023-04-09 13:19:55.250827 QtPy-Frameless-Window-0.0.2/qtframelesswindow/titlebar/title_bar_buttons.py
--rw-r--r--   0        0        0      885 2023-04-09 13:19:55.251827 QtPy-Frameless-Window-0.0.2/qtframelesswindow/utils/__init__.py
--rw-r--r--   0        0        0      457 2023-04-09 15:31:56.716491 QtPy-Frameless-Window-0.0.2/qtframelesswindow/utils/api_differ.py
--rw-r--r--   0        0        0     5296 2023-04-09 15:30:12.857623 QtPy-Frameless-Window-0.0.2/qtframelesswindow/utils/linux_utils.py
--rw-r--r--   0        0        0     1848 2023-04-09 15:30:12.858697 QtPy-Frameless-Window-0.0.2/qtframelesswindow/utils/mac_utils.py
--rw-r--r--   0        0        0     7814 2023-04-09 13:19:55.254337 QtPy-Frameless-Window-0.0.2/qtframelesswindow/utils/win32_utils.py
--rw-r--r--   0        0        0     8675 2023-04-09 15:30:12.858697 QtPy-Frameless-Window-0.0.2/qtframelesswindow/windows/__init__.py
--rw-r--r--   0        0        0     4261 2023-04-09 13:19:55.256379 QtPy-Frameless-Window-0.0.2/qtframelesswindow/windows/c_structures.py
--rw-r--r--   0        0        0     8977 2023-04-09 13:19:55.256379 QtPy-Frameless-Window-0.0.2/qtframelesswindow/windows/window_effect.py
--rw-r--r--   0        0        0     1858 2023-04-09 15:38:49.563994 QtPy-Frameless-Window-0.0.2/README.md
--rw-r--r--   0        0        0     2323 1970-01-01 00:00:00.000000 QtPy-Frameless-Window-0.0.2/PKG-INFO
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

### Comparing `QtPy-Frameless-Window-0.0.2/LICENSE` & `QtPy-Frameless-Window-0.0.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2/pyproject.toml` & `QtPy-Frameless-Window-0.0.2.dev0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 description = "A cross-platform frameless window based on QtPy."
 keywords = [
     "pyqt frameless",
 ]
 name = "QtPy-Frameless-Window"
 readme = "README.md"
 requires-python = ">=3.6"
-version = "0.0.2"
+version = "0.0.2-dev"
 
 [project.license]
 text = "GPLv3"
 
 [project.urls]
 Homepage = "https://github.com/TaoChenyue/QtPy-Frameless-Window.git"
```

### Comparing `QtPy-Frameless-Window-0.0.2/qtframelesswindow/__init__.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2/qtframelesswindow/_rc/resource.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/_rc/resource.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2/qtframelesswindow/_rc/resource_rc.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/_rc/resource_rc.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2/qtframelesswindow/linux/__init__.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/linux/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2/qtframelesswindow/linux/window_effect.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/linux/window_effect.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2/qtframelesswindow/mac/__init__.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/mac/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2/qtframelesswindow/mac/window_effect.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/mac/window_effect.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2/qtframelesswindow/titlebar/__init__.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/titlebar/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2/qtframelesswindow/titlebar/title_bar_buttons.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/titlebar/title_bar_buttons.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2/qtframelesswindow/utils/__init__.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2/qtframelesswindow/utils/linux_utils.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/utils/linux_utils.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2/qtframelesswindow/utils/mac_utils.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/utils/mac_utils.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2/qtframelesswindow/utils/win32_utils.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/utils/win32_utils.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2/qtframelesswindow/windows/__init__.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2/qtframelesswindow/windows/c_structures.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/windows/c_structures.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2/qtframelesswindow/windows/window_effect.py` & `QtPy-Frameless-Window-0.0.2.dev0/qtframelesswindow/windows/window_effect.py`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2/README.md` & `QtPy-Frameless-Window-0.0.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `QtPy-Frameless-Window-0.0.2/PKG-INFO` & `QtPy-Frameless-Window-0.0.2.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QtPy-Frameless-Window
-Version: 0.0.2
+Version: 0.0.2-dev
 Summary: A cross-platform frameless window based on QtPy.
 License: GPLv3
 Keywords: pyqt frameless
 Author-email: TaoChenyue <3038816978@qq.com>
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

