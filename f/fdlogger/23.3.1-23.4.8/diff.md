# Comparing `tmp/fdlogger-23.3.1.tar.gz` & `tmp/fdlogger-23.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdlogger-23.3.1.tar", last modified: Wed Mar  1 19:41:23 2023, max compression
+gzip compressed data, was "fdlogger-23.4.8.tar", last modified: Sun Apr  9 01:09:01 2023, max compression
```

## Comparing `fdlogger-23.3.1.tar` & `fdlogger-23.4.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-03-01 19:41:23.532233 fdlogger-23.3.1/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-07-24 04:24:05.000000 fdlogger-23.3.1/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20723 2023-03-01 19:41:23.530233 fdlogger-23.3.1/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19934 2023-02-03 16:14:23.000000 fdlogger-23.3.1/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-03-01 19:41:23.484235 fdlogger-23.3.1/fdlogger/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-01 14:55:26.000000 fdlogger-23.3.1/fdlogger/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   105316 2023-03-01 19:35:22.000000 fdlogger-23.3.1/fdlogger/__main__.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-03-01 19:41:23.507234 fdlogger-23.3.1/fdlogger/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-02-01 14:55:26.000000 fdlogger-23.3.1/fdlogger/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   331983 2023-02-01 14:55:26.000000 fdlogger-23.3.1/fdlogger/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2972 2023-02-01 14:55:26.000000 fdlogger-23.3.1/fdlogger/data/arrl_sect.dat
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      482 2022-07-24 04:24:05.000000 fdlogger-23.3.1/fdlogger/data/cwmacros_fd.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10325 2023-02-01 18:15:34.000000 fdlogger-23.3.1/fdlogger/data/dialog.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      592 2022-07-24 04:24:05.000000 fdlogger-23.3.1/fdlogger/data/fd_preferences.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      213 2023-02-01 14:59:00.000000 fdlogger-23.3.1/fdlogger/data/k6gte-fieldday.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   104172 2023-02-02 21:16:39.000000 fdlogger-23.3.1/fdlogger/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30785 2023-02-02 20:14:22.000000 fdlogger-23.3.1/fdlogger/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3812 2023-02-01 18:15:34.000000 fdlogger-23.3.1/fdlogger/data/startup.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-03-01 19:41:23.516234 fdlogger-23.3.1/fdlogger/icon/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      626 2023-02-01 14:55:26.000000 fdlogger-23.3.1/fdlogger/icon/cloud_green.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      641 2023-02-01 14:55:26.000000 fdlogger-23.3.1/fdlogger/icon/cloud_grey.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      482 2023-02-01 14:55:26.000000 fdlogger-23.3.1/fdlogger/icon/cloud_red.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      605 2023-02-01 14:55:26.000000 fdlogger-23.3.1/fdlogger/icon/gear16x16.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2876 2023-02-01 14:55:26.000000 fdlogger-23.3.1/fdlogger/icon/k6gte-fdlogger.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    96313 2023-02-19 21:29:22.000000 fdlogger-23.3.1/fdlogger/icon/logo.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5972 2023-02-01 14:55:26.000000 fdlogger-23.3.1/fdlogger/icon/radio.svg
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1234 2023-02-01 14:55:26.000000 fdlogger-23.3.1/fdlogger/icon/radio_green.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1258 2023-02-01 14:55:26.000000 fdlogger-23.3.1/fdlogger/icon/radio_grey.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      957 2023-02-01 14:55:26.000000 fdlogger-23.3.1/fdlogger/icon/radio_red.png
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-03-01 19:41:23.527233 fdlogger-23.3.1/fdlogger/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-01 14:55:26.000000 fdlogger-23.3.1/fdlogger/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10234 2023-02-02 20:57:22.000000 fdlogger-23.3.1/fdlogger/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1661 2023-02-02 20:57:35.000000 fdlogger-23.3.1/fdlogger/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13592 2023-02-02 20:58:22.000000 fdlogger-23.3.1/fdlogger/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14064 2023-02-03 16:08:03.000000 fdlogger-23.3.1/fdlogger/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4626 2023-02-02 20:59:29.000000 fdlogger-23.3.1/fdlogger/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6676 2023-03-01 19:13:45.000000 fdlogger-23.3.1/fdlogger/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-03-01 19:37:44.000000 fdlogger-23.3.1/fdlogger/lib/version.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1289 2023-02-02 20:14:22.000000 fdlogger-23.3.1/fdlogger/lib/versiontest.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-03-01 19:41:23.495234 fdlogger-23.3.1/fdlogger.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20723 2023-03-01 19:41:23.000000 fdlogger-23.3.1/fdlogger.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1170 2023-03-01 19:41:23.000000 fdlogger-23.3.1/fdlogger.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-03-01 19:41:23.000000 fdlogger-23.3.1/fdlogger.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-03-01 19:41:23.000000 fdlogger-23.3.1/fdlogger.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       35 2023-03-01 19:41:23.000000 fdlogger-23.3.1/fdlogger.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-03-01 19:41:23.000000 fdlogger-23.3.1/fdlogger.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1180 2023-03-01 19:38:02.000000 fdlogger-23.3.1/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-03-01 19:41:23.532233 fdlogger-23.3.1/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-03-01 19:41:23.529234 fdlogger-23.3.1/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2714 2022-09-14 17:33:52.000000 fdlogger-23.3.1/testing/inject_multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      862 2022-07-24 04:24:05.000000 fdlogger-23.3.1/testing/inject_udp.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)     1051 2023-03-01 19:35:50.000000 fdlogger-23.3.1/testing/multicast_listener.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    10948 2023-03-01 19:35:42.000000 fdlogger-23.3.1/testing/simulant.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-04-09 01:09:01.304266 fdlogger-23.4.8/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-07-24 04:24:05.000000 fdlogger-23.4.8/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20764 2023-04-09 01:09:01.303266 fdlogger-23.4.8/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19975 2023-04-09 01:07:05.000000 fdlogger-23.4.8/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-04-09 01:09:01.284265 fdlogger-23.4.8/fdlogger/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-01 14:55:26.000000 fdlogger-23.4.8/fdlogger/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   105316 2023-04-09 01:04:57.000000 fdlogger-23.4.8/fdlogger/__main__.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-04-09 01:09:01.293266 fdlogger-23.4.8/fdlogger/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-02-01 14:55:26.000000 fdlogger-23.4.8/fdlogger/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   331983 2023-02-01 14:55:26.000000 fdlogger-23.4.8/fdlogger/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2972 2023-02-01 14:55:26.000000 fdlogger-23.4.8/fdlogger/data/arrl_sect.dat
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      482 2022-07-24 04:24:05.000000 fdlogger-23.4.8/fdlogger/data/cwmacros_fd.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10325 2023-02-01 18:15:34.000000 fdlogger-23.4.8/fdlogger/data/dialog.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      592 2022-07-24 04:24:05.000000 fdlogger-23.4.8/fdlogger/data/fd_preferences.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      213 2023-02-01 14:59:00.000000 fdlogger-23.4.8/fdlogger/data/k6gte-fieldday.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   104172 2023-02-02 21:16:39.000000 fdlogger-23.4.8/fdlogger/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30785 2023-02-02 20:14:22.000000 fdlogger-23.4.8/fdlogger/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3812 2023-02-01 18:15:34.000000 fdlogger-23.4.8/fdlogger/data/startup.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-04-09 01:09:01.297266 fdlogger-23.4.8/fdlogger/icon/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      626 2023-02-01 14:55:26.000000 fdlogger-23.4.8/fdlogger/icon/cloud_green.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      641 2023-02-01 14:55:26.000000 fdlogger-23.4.8/fdlogger/icon/cloud_grey.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      482 2023-02-01 14:55:26.000000 fdlogger-23.4.8/fdlogger/icon/cloud_red.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      605 2023-02-01 14:55:26.000000 fdlogger-23.4.8/fdlogger/icon/gear16x16.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2876 2023-02-01 14:55:26.000000 fdlogger-23.4.8/fdlogger/icon/k6gte-fdlogger.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    96313 2023-02-19 21:29:22.000000 fdlogger-23.4.8/fdlogger/icon/logo.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5972 2023-02-01 14:55:26.000000 fdlogger-23.4.8/fdlogger/icon/radio.svg
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1234 2023-02-01 14:55:26.000000 fdlogger-23.4.8/fdlogger/icon/radio_green.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1258 2023-02-01 14:55:26.000000 fdlogger-23.4.8/fdlogger/icon/radio_grey.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      957 2023-02-01 14:55:26.000000 fdlogger-23.4.8/fdlogger/icon/radio_red.png
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-04-09 01:09:01.301266 fdlogger-23.4.8/fdlogger/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-01 14:55:26.000000 fdlogger-23.4.8/fdlogger/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10234 2023-02-02 20:57:22.000000 fdlogger-23.4.8/fdlogger/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1661 2023-02-02 20:57:35.000000 fdlogger-23.4.8/fdlogger/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13592 2023-02-02 20:58:22.000000 fdlogger-23.4.8/fdlogger/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14064 2023-02-03 16:08:03.000000 fdlogger-23.4.8/fdlogger/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4626 2023-02-02 20:59:29.000000 fdlogger-23.4.8/fdlogger/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6707 2023-04-08 23:33:07.000000 fdlogger-23.4.8/fdlogger/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-04-09 01:06:09.000000 fdlogger-23.4.8/fdlogger/lib/version.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1289 2023-02-02 20:14:22.000000 fdlogger-23.4.8/fdlogger/lib/versiontest.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-04-09 01:09:01.287265 fdlogger-23.4.8/fdlogger.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20764 2023-04-09 01:09:01.000000 fdlogger-23.4.8/fdlogger.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1170 2023-04-09 01:09:01.000000 fdlogger-23.4.8/fdlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-04-09 01:09:01.000000 fdlogger-23.4.8/fdlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2023-04-09 01:09:01.000000 fdlogger-23.4.8/fdlogger.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       35 2023-04-09 01:09:01.000000 fdlogger-23.4.8/fdlogger.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-04-09 01:09:01.000000 fdlogger-23.4.8/fdlogger.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1180 2023-04-09 01:05:58.000000 fdlogger-23.4.8/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-04-09 01:09:01.304266 fdlogger-23.4.8/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-04-09 01:09:01.302266 fdlogger-23.4.8/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2714 2022-09-14 17:33:52.000000 fdlogger-23.4.8/testing/inject_multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      862 2022-07-24 04:24:05.000000 fdlogger-23.4.8/testing/inject_udp.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)     1051 2023-03-01 19:35:50.000000 fdlogger-23.4.8/testing/multicast_listener.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    10948 2023-03-01 19:35:42.000000 fdlogger-23.4.8/testing/simulant.py
```

### Comparing `fdlogger-23.3.1/LICENSE` & `fdlogger-23.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/PKG-INFO` & `fdlogger-23.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdlogger
-Version: 23.3.1
+Version: 23.4.8
 Summary: ARRL Field Day logger GUI
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/FieldDayLogger
 Project-URL: Bug Tracker, https://github.com/mbridak/FieldDayLogger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -92,14 +92,15 @@
 Just search for the two places in the code 'FT8' is used and Bob's your dads
 brother.
 
 **WB8ERJ's blog writeup** [Mike's Tech Blog WB8ERJ](https://mikestechblog.com/field-day-logging-software-for-the-raspberry-pi/)
 
 ## Recent Changes
 
+- [23.4.8] Fixed crash on setting setup.
 - [23.2.3] Fixed crash when qrz or hamqth was used. Fixed crash when not debugging. Contact lookup now shows in infoline. Reduced font size in the group chat window. Improved debug logging.
 - [23.2.2] Added N1MM status packets. fdserver program moved into it's own repo/PyPi package.
 - [23.2.1] Made interface resizable.
 - [23.1.30] Repackaged for PyPi pip installation
 
 ## Wheres the data
```

### Comparing `fdlogger-23.3.1/README.md` & `fdlogger-23.4.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 Just search for the two places in the code 'FT8' is used and Bob's your dads
 brother.
 
 **WB8ERJ's blog writeup** [Mike's Tech Blog WB8ERJ](https://mikestechblog.com/field-day-logging-software-for-the-raspberry-pi/)
 
 ## Recent Changes
 
+- [23.4.8] Fixed crash on setting setup.
 - [23.2.3] Fixed crash when qrz or hamqth was used. Fixed crash when not debugging. Contact lookup now shows in infoline. Reduced font size in the group chat window. Improved debug logging.
 - [23.2.2] Added N1MM status packets. fdserver program moved into it's own repo/PyPi package.
 - [23.2.1] Made interface resizable.
 - [23.1.30] Repackaged for PyPi pip installation
 
 ## Wheres the data
```

### Comparing `fdlogger-23.3.1/fdlogger/__main__.py` & `fdlogger-23.4.8/fdlogger/__main__.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/data/JetBrainsMono-Regular.ttf` & `fdlogger-23.4.8/fdlogger/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/data/MASTER.SCP` & `fdlogger-23.4.8/fdlogger/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/data/arrl_sect.dat` & `fdlogger-23.4.8/fdlogger/data/arrl_sect.dat`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/data/dialog.ui` & `fdlogger-23.4.8/fdlogger/data/dialog.ui`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/data/fd_preferences.json` & `fdlogger-23.4.8/fdlogger/data/fd_preferences.json`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/data/main.ui` & `fdlogger-23.4.8/fdlogger/data/main.ui`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/data/settings.ui` & `fdlogger-23.4.8/fdlogger/data/settings.ui`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/data/startup.ui` & `fdlogger-23.4.8/fdlogger/data/startup.ui`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/icon/cloud_green.png` & `fdlogger-23.4.8/fdlogger/icon/cloud_green.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/icon/cloud_grey.png` & `fdlogger-23.4.8/fdlogger/icon/cloud_grey.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/icon/gear16x16.png` & `fdlogger-23.4.8/fdlogger/icon/gear16x16.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/icon/k6gte-fdlogger.png` & `fdlogger-23.4.8/fdlogger/icon/k6gte-fdlogger.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/icon/logo.png` & `fdlogger-23.4.8/fdlogger/icon/logo.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/icon/radio.svg` & `fdlogger-23.4.8/fdlogger/icon/radio.svg`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/icon/radio_green.png` & `fdlogger-23.4.8/fdlogger/icon/radio_green.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/icon/radio_grey.png` & `fdlogger-23.4.8/fdlogger/icon/radio_grey.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/icon/radio_red.png` & `fdlogger-23.4.8/fdlogger/icon/radio_red.png`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/lib/cat_interface.py` & `fdlogger-23.4.8/fdlogger/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/lib/cwinterface.py` & `fdlogger-23.4.8/fdlogger/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/lib/database.py` & `fdlogger-23.4.8/fdlogger/lib/database.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/lib/lookup.py` & `fdlogger-23.4.8/fdlogger/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/lib/n1mm.py` & `fdlogger-23.4.8/fdlogger/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger/lib/settings.py` & `fdlogger-23.4.8/fdlogger/lib/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,17 @@
             )
             self.n1mm_operator.setText(str(self.preference.get("n1mm_operator", "")))
             self.n1mm_ip.setText(str(self.preference.get("n1mm_ip", "")))
             self.n1mm_radioport.setText(str(self.preference.get("n1mm_radioport", "")))
             self.n1mm_contactport.setText(
                 str(self.preference.get("n1mm_contactport", ""))
             )
-            self.n1mm_lookupport.setText(str(self.preferenceget("n1mm_lookupport", "")))
+            self.n1mm_lookupport.setText(
+                str(self.preference.get("n1mm_lookupport", ""))
+            )
             self.n1mm_scoreport.setText(str(self.preference.get("n1mm_scoreport", "")))
 
     def save_changes(self):
         """
         Write preferences to json file.
         """
```

### Comparing `fdlogger-23.3.1/fdlogger/lib/versiontest.py` & `fdlogger-23.4.8/fdlogger/lib/versiontest.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/fdlogger.egg-info/PKG-INFO` & `fdlogger-23.4.8/fdlogger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdlogger
-Version: 23.3.1
+Version: 23.4.8
 Summary: ARRL Field Day logger GUI
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/FieldDayLogger
 Project-URL: Bug Tracker, https://github.com/mbridak/FieldDayLogger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -92,14 +92,15 @@
 Just search for the two places in the code 'FT8' is used and Bob's your dads
 brother.
 
 **WB8ERJ's blog writeup** [Mike's Tech Blog WB8ERJ](https://mikestechblog.com/field-day-logging-software-for-the-raspberry-pi/)
 
 ## Recent Changes
 
+- [23.4.8] Fixed crash on setting setup.
 - [23.2.3] Fixed crash when qrz or hamqth was used. Fixed crash when not debugging. Contact lookup now shows in infoline. Reduced font size in the group chat window. Improved debug logging.
 - [23.2.2] Added N1MM status packets. fdserver program moved into it's own repo/PyPi package.
 - [23.2.1] Made interface resizable.
 - [23.1.30] Repackaged for PyPi pip installation
 
 ## Wheres the data
```

### Comparing `fdlogger-23.3.1/fdlogger.egg-info/SOURCES.txt` & `fdlogger-23.4.8/fdlogger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/pyproject.toml` & `fdlogger-23.4.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fdlogger" 
-version = "23.3.1"
+version = "23.4.8"
 description = "ARRL Field Day logger GUI"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

### Comparing `fdlogger-23.3.1/testing/inject_multicast.py` & `fdlogger-23.4.8/testing/inject_multicast.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/testing/inject_udp.py` & `fdlogger-23.4.8/testing/inject_udp.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/testing/multicast_listener.py` & `fdlogger-23.4.8/testing/multicast_listener.py`

 * *Files identical despite different names*

### Comparing `fdlogger-23.3.1/testing/simulant.py` & `fdlogger-23.4.8/testing/simulant.py`

 * *Files identical despite different names*

