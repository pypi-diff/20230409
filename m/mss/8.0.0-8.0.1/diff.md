# Comparing `tmp/mss-8.0.0.tar.gz` & `tmp/mss-8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mss-8.0.0.tar", last modified: Sun Apr  9 17:14:33 2023, max compression
+gzip compressed data, was "mss-8.0.1.tar", last modified: Sun Apr  9 18:34:05 2023, max compression
```

## Comparing `mss-8.0.0.tar` & `mss-8.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 17:14:33.609279 mss-8.0.0/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1093 2023-01-01 09:58:18.000000 mss-8.0.0/LICENSE
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       88 2021-08-03 16:40:06.000000 mss-8.0.0/MANIFEST.in
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3578 2023-04-09 17:14:33.609279 mss-8.0.0/PKG-INFO
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2199 2023-04-09 16:24:40.000000 mss-8.0.0/README.rst
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 17:14:33.601280 mss-8.0.0/mss/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      940 2023-04-08 11:57:14.000000 mss-8.0.0/mss/__init__.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2646 2023-04-09 16:40:38.000000 mss-8.0.0/mss/__main__.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     8606 2023-04-09 16:24:40.000000 mss-8.0.0/mss/base.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     7513 2023-04-09 16:24:40.000000 mss-8.0.0/mss/darwin.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      368 2023-04-09 16:24:40.000000 mss-8.0.0/mss/exception.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      911 2023-01-01 09:57:58.000000 mss-8.0.0/mss/factory.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    14900 2023-04-09 16:31:22.000000 mss-8.0.0/mss/linux.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      416 2023-01-01 09:57:58.000000 mss-8.0.0/mss/models.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3859 2023-04-09 16:24:40.000000 mss-8.0.0/mss/screenshot.py
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 17:14:33.605280 mss-8.0.0/mss/tests/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1566 2023-01-01 09:57:58.000000 mss-8.0.0/mss/tests/bench_bgra2rgb.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1327 2023-01-01 09:57:58.000000 mss-8.0.0/mss/tests/bench_general.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1382 2023-04-08 11:57:14.000000 mss-8.0.0/mss/tests/conftest.py
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 17:14:33.605280 mss-8.0.0/mss/tests/res/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)  3145728 2021-08-03 16:40:06.000000 mss-8.0.0/mss/tests/res/monitor-1024x768.raw
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      501 2023-01-01 09:57:58.000000 mss-8.0.0/mss/tests/test_bgra_to_rgb.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      573 2023-04-08 11:57:14.000000 mss-8.0.0/mss/tests/test_cls_image.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      863 2023-04-08 11:57:14.000000 mss-8.0.0/mss/tests/test_find_monitors.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1777 2023-04-08 11:57:14.000000 mss-8.0.0/mss/tests/test_get_pixels.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     5383 2023-04-09 16:24:40.000000 mss-8.0.0/mss/tests/test_gnu_linux.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     5505 2023-04-08 11:57:14.000000 mss-8.0.0/mss/tests/test_implementation.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1242 2023-04-09 16:24:40.000000 mss-8.0.0/mss/tests/test_issue_220.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3530 2023-04-08 11:57:14.000000 mss-8.0.0/mss/tests/test_leaks.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1719 2023-01-01 09:57:58.000000 mss-8.0.0/mss/tests/test_macos.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2242 2023-04-08 11:57:14.000000 mss-8.0.0/mss/tests/test_save.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      666 2023-04-08 11:57:14.000000 mss-8.0.0/mss/tests/test_setup.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2475 2023-04-08 11:57:14.000000 mss-8.0.0/mss/tests/test_third_party.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1969 2023-04-08 11:57:14.000000 mss-8.0.0/mss/tests/test_tools.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1866 2023-01-01 09:57:58.000000 mss-8.0.0/mss/tests/test_windows.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1928 2023-04-09 16:24:40.000000 mss-8.0.0/mss/tools.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     9290 2023-04-09 16:24:40.000000 mss-8.0.0/mss/windows.py
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 17:14:33.605280 mss-8.0.0/mss.egg-info/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3578 2023-04-09 17:14:33.000000 mss-8.0.0/mss.egg-info/PKG-INFO
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      871 2023-04-09 17:14:33.000000 mss-8.0.0/mss.egg-info/SOURCES.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        1 2023-04-09 17:14:33.000000 mss-8.0.0/mss.egg-info/dependency_links.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       42 2023-04-09 17:14:33.000000 mss-8.0.0/mss.egg-info/entry_points.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        1 2023-04-08 11:57:57.000000 mss-8.0.0/mss.egg-info/not-zip-safe
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        4 2023-04-09 17:14:33.000000 mss-8.0.0/mss.egg-info/top_level.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1865 2023-04-09 17:14:33.609279 mss-8.0.0/setup.cfg
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       39 2021-08-03 16:40:06.000000 mss-8.0.0/setup.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 18:34:05.044221 mss-8.0.1/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1093 2023-01-01 09:58:18.000000 mss-8.0.1/LICENSE
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       88 2021-08-03 16:40:06.000000 mss-8.0.1/MANIFEST.in
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3578 2023-04-09 18:34:05.044221 mss-8.0.1/PKG-INFO
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2199 2023-04-09 16:24:40.000000 mss-8.0.1/README.rst
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 18:34:05.040220 mss-8.0.1/mss/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      940 2023-04-09 17:27:28.000000 mss-8.0.1/mss/__init__.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2690 2023-04-09 17:52:33.000000 mss-8.0.1/mss/__main__.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     8565 2023-04-09 18:12:06.000000 mss-8.0.1/mss/base.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     7513 2023-04-09 18:10:22.000000 mss-8.0.1/mss/darwin.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      368 2023-04-09 16:24:40.000000 mss-8.0.1/mss/exception.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      911 2023-01-01 09:57:58.000000 mss-8.0.1/mss/factory.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    14900 2023-04-09 16:31:22.000000 mss-8.0.1/mss/linux.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      416 2023-01-01 09:57:58.000000 mss-8.0.1/mss/models.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3859 2023-04-09 16:24:40.000000 mss-8.0.1/mss/screenshot.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 18:34:05.044221 mss-8.0.1/mss/tests/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1566 2023-01-01 09:57:58.000000 mss-8.0.1/mss/tests/bench_bgra2rgb.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1327 2023-01-01 09:57:58.000000 mss-8.0.1/mss/tests/bench_general.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1382 2023-04-08 11:57:14.000000 mss-8.0.1/mss/tests/conftest.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 18:34:05.044221 mss-8.0.1/mss/tests/res/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)  3145728 2021-08-03 16:40:06.000000 mss-8.0.1/mss/tests/res/monitor-1024x768.raw
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      501 2023-01-01 09:57:58.000000 mss-8.0.1/mss/tests/test_bgra_to_rgb.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      573 2023-04-08 11:57:14.000000 mss-8.0.1/mss/tests/test_cls_image.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      863 2023-04-08 11:57:14.000000 mss-8.0.1/mss/tests/test_find_monitors.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1777 2023-04-08 11:57:14.000000 mss-8.0.1/mss/tests/test_get_pixels.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     5383 2023-04-09 16:24:40.000000 mss-8.0.1/mss/tests/test_gnu_linux.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     6336 2023-04-09 18:04:49.000000 mss-8.0.1/mss/tests/test_implementation.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1242 2023-04-09 16:24:40.000000 mss-8.0.1/mss/tests/test_issue_220.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3530 2023-04-08 11:57:14.000000 mss-8.0.1/mss/tests/test_leaks.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1719 2023-01-01 09:57:58.000000 mss-8.0.1/mss/tests/test_macos.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2242 2023-04-08 11:57:14.000000 mss-8.0.1/mss/tests/test_save.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      666 2023-04-08 11:57:14.000000 mss-8.0.1/mss/tests/test_setup.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2475 2023-04-08 11:57:14.000000 mss-8.0.1/mss/tests/test_third_party.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1969 2023-04-08 11:57:14.000000 mss-8.0.1/mss/tests/test_tools.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1866 2023-01-01 09:57:58.000000 mss-8.0.1/mss/tests/test_windows.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1928 2023-04-09 16:24:40.000000 mss-8.0.1/mss/tools.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     9290 2023-04-09 18:10:25.000000 mss-8.0.1/mss/windows.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 18:34:05.040220 mss-8.0.1/mss.egg-info/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3578 2023-04-09 18:34:05.000000 mss-8.0.1/mss.egg-info/PKG-INFO
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      871 2023-04-09 18:34:05.000000 mss-8.0.1/mss.egg-info/SOURCES.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        1 2023-04-09 18:34:05.000000 mss-8.0.1/mss.egg-info/dependency_links.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       42 2023-04-09 18:34:05.000000 mss-8.0.1/mss.egg-info/entry_points.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        1 2023-04-08 11:57:57.000000 mss-8.0.1/mss.egg-info/not-zip-safe
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        4 2023-04-09 18:34:05.000000 mss-8.0.1/mss.egg-info/top_level.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1865 2023-04-09 18:34:05.048221 mss-8.0.1/setup.cfg
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       39 2021-08-03 16:40:06.000000 mss-8.0.1/setup.py
```

### Comparing `mss-8.0.0/LICENSE` & `mss-8.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/PKG-INFO` & `mss-8.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mss
-Version: 8.0.0
+Version: 8.0.1
 Summary: An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 Home-page: https://github.com/BoboTiG/python-mss
 Author: Mickaël 'Tiger-222' Schoentgen
 Author-email: contact@tiger-222.fr
 License: MIT
 Project-URL: Documentation, https://python-mss.readthedocs.io
 Project-URL: Source, https://github.com/BoboTiG/python-mss
```

### Comparing `mss-8.0.0/README.rst` & `mss-8.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/__init__.py` & `mss-8.0.1/mss/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 You can always get the latest version of this module at:
     https://github.com/BoboTiG/python-mss
 If that URL should fail, try contacting the author.
 """
 from .exception import ScreenShotError
 from .factory import mss
 
-__version__ = "8.0.0"
+__version__ = "8.0.1"
 __author__ = "Mickaël 'Tiger-222' Schoentgen"
 __copyright__ = """
 Copyright (c) 2013-2023, Mickaël 'Tiger-222' Schoentgen
 
 Permission to use, copy, modify, and distribute this software and its
 documentation for any purpose and without fee or royalty is hereby
 granted, provided that the above copyright notice appear in all copies
```

### Comparing `mss-8.0.0/mss/__main__.py` & `mss-8.0.1/mss/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,16 @@
                     print(os.path.realpath(output))
             else:
                 for file_name in sct.save(**kwargs):
                     if not options.quiet:
                         print(os.path.realpath(file_name))
             return 0
     except ScreenShotError:
-        return 1
+        if options.quiet:
+            return 1
+        raise
 
 
 if __name__ == "__main__":  # pragma: nocover
     import sys
 
     sys.exit(main(sys.argv[1:]))
```

### Comparing `mss-8.0.0/mss/base.py` & `mss-8.0.1/mss/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,16 @@
                 "top": monitor[1],
                 "width": monitor[2] - monitor[0],
                 "height": monitor[3] - monitor[1],
             }
 
         with lock:
             screenshot = self._grab_impl(monitor)
-            if self.with_cursor:
-                cursor = self._cursor_impl()
-                screenshot = self._merge(screenshot, cursor)  # type: ignore[arg-type]
+            if self.with_cursor and (cursor := self._cursor_impl()):
+                return self._merge(screenshot, cursor)
             return screenshot
 
     @property
     def monitors(self) -> Monitors:
         """
         Get positions of all monitors.
         If the monitor has rotation, you have to deal with it
```

### Comparing `mss-8.0.0/mss/darwin.py` & `mss-8.0.1/mss/darwin.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/factory.py` & `mss-8.0.1/mss/factory.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/linux.py` & `mss-8.0.1/mss/linux.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/screenshot.py` & `mss-8.0.1/mss/screenshot.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/tests/bench_bgra2rgb.py` & `mss-8.0.1/mss/tests/bench_bgra2rgb.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/tests/bench_general.py` & `mss-8.0.1/mss/tests/bench_general.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/tests/conftest.py` & `mss-8.0.1/mss/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/tests/res/monitor-1024x768.raw` & `mss-8.0.1/mss/tests/res/monitor-1024x768.raw`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/tests/test_cls_image.py` & `mss-8.0.1/mss/tests/test_cls_image.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/tests/test_find_monitors.py` & `mss-8.0.1/mss/tests/test_find_monitors.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/tests/test_get_pixels.py` & `mss-8.0.1/mss/tests/test_get_pixels.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/tests/test_gnu_linux.py` & `mss-8.0.1/mss/tests/test_gnu_linux.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/tests/test_implementation.py` & `mss-8.0.1/mss/tests/test_implementation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This is part of the MSS Python's module.
 Source: https://github.com/BoboTiG/python-mss
 """
 import os
 import os.path
 import platform
+from unittest.mock import patch
 
 import pytest
 
 import mss.tools
 from mss import mss
 from mss.base import MSSBase
 from mss.exception import ScreenShotError
@@ -73,69 +74,95 @@
         mss()
     monkeypatch.undo()
 
     error = exc.value.args[0]
     assert error == "System 'chuck norris' not (yet?) implemented."
 
 
-def test_entry_point(capsys):
+@pytest.mark.parametrize("with_cursor", [False, True])
+def test_entry_point(with_cursor: bool, capsys):
     from datetime import datetime
 
-    from mss.__main__ import main
+    from mss.__main__ import main as entry_point
+
+    def main(*args: str, ret: int = 0) -> None:
+        if with_cursor:
+            args = args + ("--with-cursor",)
+        assert entry_point(args) == ret
 
     for opt in ("-m", "--monitor"):
-        main([opt, "1"])
+        main(opt, "1")
         out, _ = capsys.readouterr()
         assert out.endswith("monitor-1.png\n")
         assert os.path.isfile("monitor-1.png")
         os.remove("monitor-1.png")
 
-    for opt in zip(("-m 1", "--monitor=1"), ("-q", "--quiet")):
-        main(opt)
+    for opt in zip(["-m 1", "--monitor=1"], ["-q", "--quiet"]):
+        main(*opt)
         out, _ = capsys.readouterr()
         assert not out
         assert os.path.isfile("monitor-1.png")
         os.remove("monitor-1.png")
 
-    fmt = "sct-{width}x{height}.png"
+    fmt = "sct-{mon}-{width}x{height}.png"
     for opt in ("-o", "--out"):
-        main([opt, fmt])
+        main(opt, fmt)
         out, _ = capsys.readouterr()
         with mss(display=os.getenv("DISPLAY")) as sct:
-            for monitor, line in zip(sct.monitors[1:], out.splitlines()):
-                filename = fmt.format(**monitor)
+            for mon, (monitor, line) in enumerate(zip(sct.monitors[1:], out.splitlines()), 1):
+                filename = fmt.format(mon=mon, **monitor)
                 assert line.endswith(filename)
                 assert os.path.isfile(filename)
                 os.remove(filename)
 
     fmt = "sct_{mon}-{date:%Y-%m-%d}.png"
     for opt in ("-o", "--out"):
-        main(["-m 1", opt, fmt])
+        main("-m 1", opt, fmt)
         filename = fmt.format(mon=1, date=datetime.now())
         out, _ = capsys.readouterr()
         assert out.endswith(filename + "\n")
         assert os.path.isfile(filename)
         os.remove(filename)
 
     coordinates = "2,12,40,67"
     filename = "sct-2x12_40x67.png"
     for opt in ("-c", "--coordinates"):
-        main([opt, coordinates])
+        main(opt, coordinates)
         out, _ = capsys.readouterr()
         assert out.endswith(filename + "\n")
         assert os.path.isfile(filename)
         os.remove(filename)
 
     coordinates = "2,12,40"
     for opt in ("-c", "--coordinates"):
-        main([opt, coordinates])
+        main(opt, coordinates, ret=2)
         out, _ = capsys.readouterr()
         assert out == "Coordinates syntax: top, left, width, height\n"
 
 
+@patch("mss.base.MSSBase.monitors", new=[])
+@pytest.mark.parametrize("quiet", [False, True])
+def test_entry_point_error(quiet: bool, capsys):
+    from mss.__main__ import main as entry_point
+
+    def main(*args: str) -> int:
+        if quiet:
+            args = args + ("--quiet",)
+        return entry_point(args)
+
+    if quiet:
+        assert main() == 1
+        out, err = capsys.readouterr()
+        assert not out
+        assert not err
+    else:
+        with pytest.raises(ScreenShotError):
+            main()
+
+
 def test_grab_with_tuple(pixel_ratio):
     left = 100
     top = 100
     right = 500
     lower = 500
     width = right - left  # 400px width
     height = lower - top  # 400px height
```

### Comparing `mss-8.0.0/mss/tests/test_issue_220.py` & `mss-8.0.1/mss/tests/test_issue_220.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/tests/test_leaks.py` & `mss-8.0.1/mss/tests/test_leaks.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/tests/test_macos.py` & `mss-8.0.1/mss/tests/test_macos.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/tests/test_save.py` & `mss-8.0.1/mss/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/tests/test_setup.py` & `mss-8.0.1/mss/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/tests/test_third_party.py` & `mss-8.0.1/mss/tests/test_third_party.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/tests/test_tools.py` & `mss-8.0.1/mss/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/tests/test_windows.py` & `mss-8.0.1/mss/tests/test_windows.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/tools.py` & `mss-8.0.1/mss/tools.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss/windows.py` & `mss-8.0.1/mss/windows.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/mss.egg-info/PKG-INFO` & `mss-8.0.1/mss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mss
-Version: 8.0.0
+Version: 8.0.1
 Summary: An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 Home-page: https://github.com/BoboTiG/python-mss
 Author: Mickaël 'Tiger-222' Schoentgen
 Author-email: contact@tiger-222.fr
 License: MIT
 Project-URL: Documentation, https://python-mss.readthedocs.io
 Project-URL: Source, https://github.com/BoboTiG/python-mss
```

### Comparing `mss-8.0.0/mss.egg-info/SOURCES.txt` & `mss-8.0.1/mss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mss-8.0.0/setup.cfg` & `mss-8.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mss
-version = 8.0.0
+version = 8.0.1
 author = Mickaël 'Tiger-222' Schoentgen
 author_email = contact@tiger-222.fr
 description = An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/BoboTiG/python-mss
 home_page = https://pypi.org/project/mss/
```

