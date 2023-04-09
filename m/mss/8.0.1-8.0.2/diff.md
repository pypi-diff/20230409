# Comparing `tmp/mss-8.0.1.tar.gz` & `tmp/mss-8.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mss-8.0.1.tar", last modified: Sun Apr  9 18:34:05 2023, max compression
+gzip compressed data, was "mss-8.0.2.tar", last modified: Sun Apr  9 22:01:04 2023, max compression
```

## Comparing `mss-8.0.1.tar` & `mss-8.0.2.tar`

### file list

```diff
@@ -1,46 +1,75 @@
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 18:34:05.044221 mss-8.0.1/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1093 2023-01-01 09:58:18.000000 mss-8.0.1/LICENSE
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       88 2021-08-03 16:40:06.000000 mss-8.0.1/MANIFEST.in
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3578 2023-04-09 18:34:05.044221 mss-8.0.1/PKG-INFO
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2199 2023-04-09 16:24:40.000000 mss-8.0.1/README.rst
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 18:34:05.040220 mss-8.0.1/mss/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      940 2023-04-09 17:27:28.000000 mss-8.0.1/mss/__init__.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2690 2023-04-09 17:52:33.000000 mss-8.0.1/mss/__main__.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     8565 2023-04-09 18:12:06.000000 mss-8.0.1/mss/base.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     7513 2023-04-09 18:10:22.000000 mss-8.0.1/mss/darwin.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      368 2023-04-09 16:24:40.000000 mss-8.0.1/mss/exception.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      911 2023-01-01 09:57:58.000000 mss-8.0.1/mss/factory.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    14900 2023-04-09 16:31:22.000000 mss-8.0.1/mss/linux.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      416 2023-01-01 09:57:58.000000 mss-8.0.1/mss/models.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3859 2023-04-09 16:24:40.000000 mss-8.0.1/mss/screenshot.py
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 18:34:05.044221 mss-8.0.1/mss/tests/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1566 2023-01-01 09:57:58.000000 mss-8.0.1/mss/tests/bench_bgra2rgb.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1327 2023-01-01 09:57:58.000000 mss-8.0.1/mss/tests/bench_general.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1382 2023-04-08 11:57:14.000000 mss-8.0.1/mss/tests/conftest.py
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 18:34:05.044221 mss-8.0.1/mss/tests/res/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)  3145728 2021-08-03 16:40:06.000000 mss-8.0.1/mss/tests/res/monitor-1024x768.raw
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      501 2023-01-01 09:57:58.000000 mss-8.0.1/mss/tests/test_bgra_to_rgb.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      573 2023-04-08 11:57:14.000000 mss-8.0.1/mss/tests/test_cls_image.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      863 2023-04-08 11:57:14.000000 mss-8.0.1/mss/tests/test_find_monitors.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1777 2023-04-08 11:57:14.000000 mss-8.0.1/mss/tests/test_get_pixels.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     5383 2023-04-09 16:24:40.000000 mss-8.0.1/mss/tests/test_gnu_linux.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     6336 2023-04-09 18:04:49.000000 mss-8.0.1/mss/tests/test_implementation.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1242 2023-04-09 16:24:40.000000 mss-8.0.1/mss/tests/test_issue_220.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3530 2023-04-08 11:57:14.000000 mss-8.0.1/mss/tests/test_leaks.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1719 2023-01-01 09:57:58.000000 mss-8.0.1/mss/tests/test_macos.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2242 2023-04-08 11:57:14.000000 mss-8.0.1/mss/tests/test_save.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      666 2023-04-08 11:57:14.000000 mss-8.0.1/mss/tests/test_setup.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2475 2023-04-08 11:57:14.000000 mss-8.0.1/mss/tests/test_third_party.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1969 2023-04-08 11:57:14.000000 mss-8.0.1/mss/tests/test_tools.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1866 2023-01-01 09:57:58.000000 mss-8.0.1/mss/tests/test_windows.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1928 2023-04-09 16:24:40.000000 mss-8.0.1/mss/tools.py
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     9290 2023-04-09 18:10:25.000000 mss-8.0.1/mss/windows.py
-drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 18:34:05.040220 mss-8.0.1/mss.egg-info/
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3578 2023-04-09 18:34:05.000000 mss-8.0.1/mss.egg-info/PKG-INFO
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      871 2023-04-09 18:34:05.000000 mss-8.0.1/mss.egg-info/SOURCES.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        1 2023-04-09 18:34:05.000000 mss-8.0.1/mss.egg-info/dependency_links.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       42 2023-04-09 18:34:05.000000 mss-8.0.1/mss.egg-info/entry_points.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        1 2023-04-08 11:57:57.000000 mss-8.0.1/mss.egg-info/not-zip-safe
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        4 2023-04-09 18:34:05.000000 mss-8.0.1/mss.egg-info/top_level.txt
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1865 2023-04-09 18:34:05.048221 mss-8.0.1/setup.cfg
--rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       39 2021-08-03 16:40:06.000000 mss-8.0.1/setup.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 22:01:04.133612 mss-8.0.2/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1093 2023-04-05 04:26:59.000000 mss-8.0.2/LICENSE
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       88 2022-10-27 01:33:30.000000 mss-8.0.2/MANIFEST.in
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3578 2023-04-09 22:01:04.133612 mss-8.0.2/PKG-INFO
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2199 2023-04-08 22:53:33.000000 mss-8.0.2/README.rst
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 22:01:04.129612 mss-8.0.2/docs/
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 22:01:04.129612 mss-8.0.2/docs/source/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2417 2023-04-09 20:16:52.000000 mss-8.0.2/docs/source/conf.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 22:01:04.129612 mss-8.0.2/docs/source/examples/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      550 2022-10-27 02:45:16.000000 mss-8.0.2/docs/source/examples/callback.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      729 2022-10-27 03:01:57.000000 mss-8.0.2/docs/source/examples/custom_cls_image.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1356 2022-10-27 02:44:18.000000 mss-8.0.2/docs/source/examples/fps.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1113 2022-10-27 02:47:31.000000 mss-8.0.2/docs/source/examples/fps_multiprocessing.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      751 2022-10-27 02:46:10.000000 mss-8.0.2/docs/source/examples/from_pil_tuple.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      240 2022-10-27 02:08:04.000000 mss-8.0.2/docs/source/examples/linux_display_keyword.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      885 2022-10-27 02:08:14.000000 mss-8.0.2/docs/source/examples/opencv_numpy.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      526 2022-10-27 02:08:22.000000 mss-8.0.2/docs/source/examples/part_of_screen.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      792 2022-10-27 02:08:18.000000 mss-8.0.2/docs/source/examples/part_of_screen_monitor_2.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      712 2022-10-27 02:08:45.000000 mss-8.0.2/docs/source/examples/pil.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      755 2022-10-27 02:08:36.000000 mss-8.0.2/docs/source/examples/pil_pixels.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 22:01:04.133612 mss-8.0.2/mss/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      940 2023-04-09 20:16:52.000000 mss-8.0.2/mss/__init__.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2659 2023-04-09 20:52:13.000000 mss-8.0.2/mss/__main__.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     8565 2023-04-09 20:16:52.000000 mss-8.0.2/mss/base.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     7513 2023-04-08 22:53:33.000000 mss-8.0.2/mss/darwin.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      368 2023-04-09 12:48:59.000000 mss-8.0.2/mss/exception.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      911 2023-04-08 14:16:44.000000 mss-8.0.2/mss/factory.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    14900 2023-04-09 21:49:42.000000 mss-8.0.2/mss/linux.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      416 2022-10-27 02:52:39.000000 mss-8.0.2/mss/models.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3859 2023-04-08 22:53:33.000000 mss-8.0.2/mss/screenshot.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 22:01:04.133612 mss-8.0.2/mss/tests/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1566 2022-10-27 02:10:59.000000 mss-8.0.2/mss/tests/bench_bgra2rgb.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1327 2022-10-27 02:11:02.000000 mss-8.0.2/mss/tests/bench_general.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1577 2023-04-09 21:56:53.000000 mss-8.0.2/mss/tests/conftest.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 22:01:04.133612 mss-8.0.2/mss/tests/res/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)    37834 2023-04-09 21:56:53.000000 mss-8.0.2/mss/tests/res/monitor-1024x768.raw.zip
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      501 2023-04-09 21:29:44.000000 mss-8.0.2/mss/tests/test_bgra_to_rgb.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      573 2023-04-08 07:06:47.000000 mss-8.0.2/mss/tests/test_cls_image.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      863 2023-04-08 07:06:47.000000 mss-8.0.2/mss/tests/test_find_monitors.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1777 2023-04-08 07:06:47.000000 mss-8.0.2/mss/tests/test_get_pixels.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     5383 2023-04-09 12:48:59.000000 mss-8.0.2/mss/tests/test_gnu_linux.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     6602 2023-04-09 20:52:13.000000 mss-8.0.2/mss/tests/test_implementation.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1521 2023-04-09 21:56:55.000000 mss-8.0.2/mss/tests/test_issue_220.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3530 2023-04-08 07:06:47.000000 mss-8.0.2/mss/tests/test_leaks.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1719 2022-10-27 02:12:18.000000 mss-8.0.2/mss/tests/test_macos.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2242 2023-04-08 07:06:47.000000 mss-8.0.2/mss/tests/test_save.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)      666 2023-04-05 14:07:14.000000 mss-8.0.2/mss/tests/test_setup.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     2475 2023-04-08 07:06:47.000000 mss-8.0.2/mss/tests/test_third_party.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1969 2023-04-08 07:06:47.000000 mss-8.0.2/mss/tests/test_tools.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1866 2022-10-27 02:12:50.000000 mss-8.0.2/mss/tests/test_windows.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1928 2023-04-08 22:53:33.000000 mss-8.0.2/mss/tools.py
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     9290 2023-04-09 21:08:05.000000 mss-8.0.2/mss/windows.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 22:01:04.133612 mss-8.0.2/mss.egg-info/
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     3578 2023-04-09 22:01:04.000000 mss-8.0.2/mss.egg-info/PKG-INFO
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1583 2023-04-09 22:01:04.000000 mss-8.0.2/mss.egg-info/SOURCES.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        1 2023-04-09 22:01:04.000000 mss-8.0.2/mss.egg-info/dependency_links.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       42 2023-04-09 22:01:04.000000 mss-8.0.2/mss.egg-info/entry_points.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        1 2023-04-08 05:42:35.000000 mss-8.0.2/mss.egg-info/not-zip-safe
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)        4 2023-04-09 22:01:04.000000 mss-8.0.2/mss.egg-info/top_level.txt
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)     1904 2023-04-09 22:01:04.133612 mss-8.0.2/setup.cfg
+-rw-r--r--   0 tiger-222  (1000) tiger-222  (1000)       39 2022-10-27 01:33:30.000000 mss-8.0.2/setup.py
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 22:01:04.129612 mss-8.0.2/venv/
+drwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)        0 2023-04-09 22:01:04.133612 mss-8.0.2/venv/bin/
+-rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)      627 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2html.py
+-rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)      749 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2html4.py
+-rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)     1094 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2html5.py
+-rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)      826 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2latex.py
+-rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)      649 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2man.py
+-rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)      815 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2odt.py
+-rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)     1753 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)      634 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)      670 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2s5.py
+-rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)      906 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)      635 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rst2xml.py
+-rwxr-xr-x   0 tiger-222  (1000) tiger-222  (1000)      703 2023-04-05 10:03:07.000000 mss-8.0.2/venv/bin/rstpep2html.py
```

### Comparing `mss-8.0.1/LICENSE` & `mss-8.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/PKG-INFO` & `mss-8.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mss
-Version: 8.0.1
+Version: 8.0.2
 Summary: An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 Home-page: https://github.com/BoboTiG/python-mss
 Author: Mickaël 'Tiger-222' Schoentgen
 Author-email: contact@tiger-222.fr
 License: MIT
 Project-URL: Documentation, https://python-mss.readthedocs.io
 Project-URL: Source, https://github.com/BoboTiG/python-mss
```

### Comparing `mss-8.0.1/README.rst` & `mss-8.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/mss/__init__.py` & `mss-8.0.2/mss/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 You can always get the latest version of this module at:
     https://github.com/BoboTiG/python-mss
 If that URL should fail, try contacting the author.
 """
 from .exception import ScreenShotError
 from .factory import mss
 
-__version__ = "8.0.1"
+__version__ = "8.0.2"
 __author__ = "Mickaël 'Tiger-222' Schoentgen"
 __copyright__ = """
 Copyright (c) 2013-2023, Mickaël 'Tiger-222' Schoentgen
 
 Permission to use, copy, modify, and distribute this software and its
 documentation for any purpose and without fee or royalty is hereby
 granted, provided that the above copyright notice appear in all copies
```

### Comparing `mss-8.0.1/mss/__main__.py` & `mss-8.0.2/mss/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """
 This is part of the MSS Python's module.
 Source: https://github.com/BoboTiG/python-mss
 """
 import os.path
 from argparse import ArgumentParser
-from typing import List
 
 from . import __version__
 from .exception import ScreenShotError
 from .factory import mss
 from .tools import to_png
 
 
-def main(args: List[str], /) -> int:
+def main(*args: str) -> int:
     """Main logic."""
 
     cli_args = ArgumentParser()
     cli_args.add_argument(
         "-c",
         "--coordinates",
         default="",
@@ -79,8 +78,8 @@
             return 1
         raise
 
 
 if __name__ == "__main__":  # pragma: nocover
     import sys
 
-    sys.exit(main(sys.argv[1:]))
+    sys.exit(main(*sys.argv[1:]))
```

### Comparing `mss-8.0.1/mss/base.py` & `mss-8.0.2/mss/base.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/mss/darwin.py` & `mss-8.0.2/mss/darwin.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/mss/factory.py` & `mss-8.0.2/mss/factory.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/mss/linux.py` & `mss-8.0.2/mss/linux.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/mss/screenshot.py` & `mss-8.0.2/mss/screenshot.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/mss/tests/bench_bgra2rgb.py` & `mss-8.0.2/mss/tests/bench_bgra2rgb.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/mss/tests/bench_general.py` & `mss-8.0.2/mss/tests/bench_general.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/mss/tests/conftest.py` & `mss-8.0.2/mss/tests/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 This is part of the MSS Python's module.
 Source: https://github.com/BoboTiG/python-mss
 """
 import glob
 import os
+from hashlib import md5
 from pathlib import Path
+from zipfile import ZipFile
 
 import pytest
 
 from mss import mss
 
 
 @pytest.fixture(autouse=True)
@@ -38,16 +40,20 @@
 @pytest.fixture(scope="module", autouse=True)
 def before_tests(request):
     request.addfinalizer(purge_files)
 
 
 @pytest.fixture(scope="session")
 def raw() -> bytes:
-    file = Path(__file__).parent / "res" / "monitor-1024x768.raw"
-    return file.read_bytes()
+    file = Path(__file__).parent / "res" / "monitor-1024x768.raw.zip"
+    with ZipFile(file) as fh:
+        data = fh.read(file.with_suffix("").name)
+
+    assert md5(data).hexdigest() == "125696266e2a8f5240f6bc17e4df98c6"
+    return data
 
 
 @pytest.fixture(scope="session")
 def pixel_ratio() -> int:
     """Get the pixel, used to adapt test checks."""
     # Grab a 1x1 screenshot
     region = {"top": 0, "left": 0, "width": 1, "height": 1}
```

### Comparing `mss-8.0.1/mss/tests/test_cls_image.py` & `mss-8.0.2/mss/tests/test_cls_image.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/mss/tests/test_find_monitors.py` & `mss-8.0.2/mss/tests/test_find_monitors.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/mss/tests/test_get_pixels.py` & `mss-8.0.2/mss/tests/test_get_pixels.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/mss/tests/test_gnu_linux.py` & `mss-8.0.2/mss/tests/test_gnu_linux.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/mss/tests/test_implementation.py` & `mss-8.0.2/mss/tests/test_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,24 @@
     from datetime import datetime
 
     from mss.__main__ import main as entry_point
 
     def main(*args: str, ret: int = 0) -> None:
         if with_cursor:
             args = args + ("--with-cursor",)
-        assert entry_point(args) == ret
+        assert entry_point(*args) == ret
+
+    # No arguments
+    main()
+    out, _ = capsys.readouterr()
+    for mon, line in enumerate(out.splitlines(), 1):
+        filename = f"monitor-{mon}.png"
+        assert line.endswith(filename)
+        assert os.path.isfile(filename)
+        os.remove(filename)
 
     for opt in ("-m", "--monitor"):
         main(opt, "1")
         out, _ = capsys.readouterr()
         assert out.endswith("monitor-1.png\n")
         assert os.path.isfile("monitor-1.png")
         os.remove("monitor-1.png")
@@ -143,15 +152,15 @@
 @pytest.mark.parametrize("quiet", [False, True])
 def test_entry_point_error(quiet: bool, capsys):
     from mss.__main__ import main as entry_point
 
     def main(*args: str) -> int:
         if quiet:
             args = args + ("--quiet",)
-        return entry_point(args)
+        return entry_point(*args)
 
     if quiet:
         assert main() == 1
         out, err = capsys.readouterr()
         assert not out
         assert not err
     else:
```

### Comparing `mss-8.0.1/mss/tests/test_issue_220.py` & `mss-8.0.2/mss/tests/test_issue_220.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 """
 This is part of the MSS Python's module.
 Source: https://github.com/BoboTiG/python-mss
 """
+import platform
+
 import pytest
 
 import mss
 
 tkinter = pytest.importorskip("tkinter")
 
+if platform.system().lower() == "darwin" and platform.python_implementation() == "PyPy":
+    # [macOS] PyPy 7.3.11 [Python 3.9.16] fails on GitHub:
+    #     RuntimeError: tk.h version (8.5) doesn't match libtk.a version (8.6)
+    pytestmark = pytest.mark.skip
+
 
 @pytest.fixture
 def root() -> tkinter.Tk:
     master = tkinter.Tk()
     try:
         yield master
     finally:
```

### Comparing `mss-8.0.1/mss/tests/test_leaks.py` & `mss-8.0.2/mss/tests/test_leaks.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/mss/tests/test_macos.py` & `mss-8.0.2/mss/tests/test_macos.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/mss/tests/test_save.py` & `mss-8.0.2/mss/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/mss/tests/test_setup.py` & `mss-8.0.2/mss/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/mss/tests/test_third_party.py` & `mss-8.0.2/mss/tests/test_third_party.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/mss/tests/test_tools.py` & `mss-8.0.2/mss/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/mss/tests/test_windows.py` & `mss-8.0.2/mss/tests/test_windows.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/mss/tools.py` & `mss-8.0.2/mss/tools.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/mss/windows.py` & `mss-8.0.2/mss/windows.py`

 * *Files identical despite different names*

### Comparing `mss-8.0.1/mss.egg-info/PKG-INFO` & `mss-8.0.2/mss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mss
-Version: 8.0.1
+Version: 8.0.2
 Summary: An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 Home-page: https://github.com/BoboTiG/python-mss
 Author: Mickaël 'Tiger-222' Schoentgen
 Author-email: contact@tiger-222.fr
 License: MIT
 Project-URL: Documentation, https://python-mss.readthedocs.io
 Project-URL: Source, https://github.com/BoboTiG/python-mss
```

### Comparing `mss-8.0.1/setup.cfg` & `mss-8.0.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mss
-version = 8.0.1
+version = 8.0.2
 author = Mickaël 'Tiger-222' Schoentgen
 author_email = contact@tiger-222.fr
 description = An ultra fast cross-platform multiple screenshots module in pure python using ctypes.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/BoboTiG/python-mss
 home_page = https://pypi.org/project/mss/
@@ -31,18 +31,22 @@
 	Programming Language :: Python :: 3.11
 	Topic :: Multimedia :: Graphics :: Capture :: Screen Capture
 	Topic :: Software Development :: Libraries
 
 [options]
 zip_safe = False
 include_package_data = True
-packages_dir = mss
-packages = find:
+packages = find_namespace:
 python_requires = >=3.8
 
+[options.packages.find]
+include = 
+	mss
+	mss.*
+
 [options.entry_points]
 console_scripts = 
 	mss = mss.__main__:main
 
 [coverage:run]
 omit = 
 	mss/tests/*
```

