# Comparing `tmp/zoinks-0.0.5.tar.gz` & `tmp/zoinks-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoinks-0.0.5.tar", last modified: Tue Jan  4 15:16:37 2022, max compression
+gzip compressed data, was "zoinks-0.0.6.tar", last modified: Sun Apr  9 18:03:05 2023, max compression
```

## Comparing `zoinks-0.0.5.tar` & `zoinks-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2022-01-04 15:16:37.531158 zoinks-0.0.5/
--rw-r--r--   0 mhucka     (511) staff       (20)     1617 2022-01-03 15:11:06.000000 zoinks-0.0.5/LICENSE
--rw-r--r--   0 mhucka     (511) staff       (20)     4250 2022-01-04 15:16:37.531315 zoinks-0.0.5/PKG-INFO
--rw-r--r--   0 mhucka     (511) staff       (20)     3418 2022-01-04 15:15:36.000000 zoinks-0.0.5/README.md
--rw-r--r--   0 mhucka     (511) staff       (20)      957 2022-01-04 15:16:37.532009 zoinks-0.0.5/setup.cfg
--rw-r--r--   0 mhucka     (511) staff       (20)      885 2022-01-03 15:12:35.000000 zoinks-0.0.5/setup.py
-drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2022-01-04 15:16:37.528479 zoinks-0.0.5/zoinks/
--rw-r--r--   0 mhucka     (511) staff       (20)     1493 2022-01-04 15:15:07.000000 zoinks-0.0.5/zoinks/__init__.py
--rw-r--r--   0 mhucka     (511) staff       (20)    10951 2022-01-03 19:57:40.000000 zoinks-0.0.5/zoinks/__main__.py
--rw-r--r--   0 mhucka     (511) staff       (20)     1013 2022-01-03 16:10:18.000000 zoinks-0.0.5/zoinks/exceptions.py
--rw-r--r--   0 mhucka     (511) staff       (20)     1394 2022-01-03 15:22:00.000000 zoinks-0.0.5/zoinks/exit_codes.py
-drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2022-01-04 15:16:37.530884 zoinks-0.0.5/zoinks.egg-info/
--rw-r--r--   0 mhucka     (511) staff       (20)     4250 2022-01-04 15:16:37.000000 zoinks-0.0.5/zoinks.egg-info/PKG-INFO
--rw-r--r--   0 mhucka     (511) staff       (20)      327 2022-01-04 15:16:37.000000 zoinks-0.0.5/zoinks.egg-info/SOURCES.txt
--rw-r--r--   0 mhucka     (511) staff       (20)        1 2022-01-04 15:16:37.000000 zoinks-0.0.5/zoinks.egg-info/dependency_links.txt
--rw-r--r--   0 mhucka     (511) staff       (20)       65 2022-01-04 15:16:37.000000 zoinks-0.0.5/zoinks.egg-info/entry_points.txt
--rw-r--r--   0 mhucka     (511) staff       (20)        1 2022-01-04 15:16:37.000000 zoinks-0.0.5/zoinks.egg-info/not-zip-safe
--rw-r--r--   0 mhucka     (511) staff       (20)      141 2022-01-04 15:16:37.000000 zoinks-0.0.5/zoinks.egg-info/requires.txt
--rw-r--r--   0 mhucka     (511) staff       (20)        7 2022-01-04 15:16:37.000000 zoinks-0.0.5/zoinks.egg-info/top_level.txt
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-09 18:03:05.841721 zoinks-0.0.6/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1622 2023-04-09 17:58:40.000000 zoinks-0.0.6/LICENSE
+-rw-r--r--   0 mhucka     (503) staff       (20)     4241 2023-04-09 18:03:05.841784 zoinks-0.0.6/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)     3429 2023-04-09 17:59:09.000000 zoinks-0.0.6/README.md
+-rw-r--r--   0 mhucka     (503) staff       (20)      957 2023-04-09 18:03:05.842151 zoinks-0.0.6/setup.cfg
+-rw-r--r--   0 mhucka     (503) staff       (20)      885 2022-01-03 15:12:35.000000 zoinks-0.0.6/setup.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-09 18:03:05.840563 zoinks-0.0.6/zoinks/
+-rw-r--r--   0 mhucka     (503) staff       (20)     1493 2023-04-09 18:01:32.000000 zoinks-0.0.6/zoinks/__init__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)    15045 2022-11-13 17:22:14.000000 zoinks-0.0.6/zoinks/__main__.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1013 2022-01-03 16:10:18.000000 zoinks-0.0.6/zoinks/exceptions.py
+-rw-r--r--   0 mhucka     (503) staff       (20)     1394 2022-01-03 15:22:00.000000 zoinks-0.0.6/zoinks/exit_codes.py
+drwxr-xr-x   0 mhucka     (503) staff       (20)        0 2023-04-09 18:03:05.841610 zoinks-0.0.6/zoinks.egg-info/
+-rw-r--r--   0 mhucka     (503) staff       (20)     4241 2023-04-09 18:03:05.000000 zoinks-0.0.6/zoinks.egg-info/PKG-INFO
+-rw-r--r--   0 mhucka     (503) staff       (20)      327 2023-04-09 18:03:05.000000 zoinks-0.0.6/zoinks.egg-info/SOURCES.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-09 18:03:05.000000 zoinks-0.0.6/zoinks.egg-info/dependency_links.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)       64 2023-04-09 18:03:05.000000 zoinks-0.0.6/zoinks.egg-info/entry_points.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        1 2023-04-09 18:03:05.000000 zoinks-0.0.6/zoinks.egg-info/not-zip-safe
+-rw-r--r--   0 mhucka     (503) staff       (20)      129 2023-04-09 18:03:05.000000 zoinks-0.0.6/zoinks.egg-info/requires.txt
+-rw-r--r--   0 mhucka     (503) staff       (20)        7 2023-04-09 18:03:05.000000 zoinks-0.0.6/zoinks.egg-info/top_level.txt
```

### Comparing `zoinks-0.0.5/LICENSE` & `zoinks-0.0.6/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022 by Michael Hucka and the California Institute of
+Copyright (c) 2022-2023 by Michael Hucka and the California Institute of
 Technology (Pasadena, California, USA).  All rights not granted herein
 are expressly reserved by the copyright holders.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice,
```

### Comparing `zoinks-0.0.5/PKG-INFO` & `zoinks-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: zoinks
-Version: 0.0.5
+Version: 0.0.6
 Summary: Zoinks: a command-line utility to retrieve Zotero record values
 Home-page: https://github.com/mhucka/zoinks
 Author: Mike Hucka
 Author-email: mhucka@caltech.edu
 License: BSD 3-clause license
 Project-URL: Source Code, https://github.com/mhucka/zoinks
 Project-URL: Bug Tracker, https://github.com/mhucka/zoinks/issues
 Keywords: Python,applications
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
@@ -82,18 +81,16 @@
 
 I would be happy to receive your help and participation if you are interested.  Everyone is asked to read and respect the [code of conduct](CONDUCT.md) when participating in this project.  Development generally takes place on the `development` branch.
 
 
 License
 -------
 
-This software is Copyright (C) 2022, by Michael Hucka and the California Institute of Technology (Pasadena, California, USA).  This software is freely distributed under a 3-clause BSD type license.  Please see the [LICENSE](LICENSE) file for more information.
+This software is Copyright (C) 2022&ndash;2023, by Michael Hucka and the California Institute of Technology (Pasadena, California, USA).  This software is freely distributed under a 3-clause BSD type license.  Please see the [LICENSE](LICENSE) file for more information.
 
 
 Acknowledgments
 ---------------
 
 This work is a personal project developed by the author, using computing facilities and other resources of the [California Institute of Technology Library](https://www.library.caltech.edu).
 
 The [vector artwork](https://thenounproject.com/term/surprise/2696259/) of a surprised person, used as the icon for this repository, was created by [Adrien Coquet](https://thenounproject.com/coquet_adrien/) from the Noun Project.  It is licensed under the Creative Commons [CC-BY 3.0](https://creativecommons.org/licenses/by/3.0/) license.
-
-
```

### Comparing `zoinks-0.0.5/README.md` & `zoinks-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 I would be happy to receive your help and participation if you are interested.  Everyone is asked to read and respect the [code of conduct](CONDUCT.md) when participating in this project.  Development generally takes place on the `development` branch.
 
 
 License
 -------
 
-This software is Copyright (C) 2022, by Michael Hucka and the California Institute of Technology (Pasadena, California, USA).  This software is freely distributed under a 3-clause BSD type license.  Please see the [LICENSE](LICENSE) file for more information.
+This software is Copyright (C) 2022&ndash;2023, by Michael Hucka and the California Institute of Technology (Pasadena, California, USA).  This software is freely distributed under a 3-clause BSD type license.  Please see the [LICENSE](LICENSE) file for more information.
 
 
 Acknowledgments
 ---------------
 
 This work is a personal project developed by the author, using computing facilities and other resources of the [California Institute of Technology Library](https://www.library.caltech.edu).
```

### Comparing `zoinks-0.0.5/setup.cfg` & `zoinks-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = zoinks
-version = 0.0.5
+version = 0.0.6
 description = Zoinks: a command-line utility to retrieve Zotero record values
 author = Mike Hucka
 author_email = mhucka@caltech.edu
 license = BSD 3-clause license
 license_files = LICENSE
 url = https://github.com/mhucka/zoinks
 project_urls =
```

### Comparing `zoinks-0.0.5/setup.py` & `zoinks-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `zoinks-0.0.5/zoinks/__init__.py` & `zoinks-0.0.6/zoinks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Package metadata ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 #
 #  ╭────────────────────── Notice ── Notice ── Notice ─────────────────────╮
 #  |    The following values are automatically updated at every release    |
 #  |    by the Makefile. Manual changes to these values will be lost.      |
 #  ╰────────────────────── Notice ── Notice ── Notice ─────────────────────╯
 
-__version__     = '0.0.5'
+__version__     = '0.0.6'
 __description__ = 'Zoinks: a command-line utility to retrieve Zotero record values'
 __url__         = 'https://github.com/mhucka/zoinks'
 __author__      = 'Mike Hucka'
 __email__       = 'mhucka@caltech.edu'
 __license__     = 'BSD 3-clause license'
```

### Comparing `zoinks-0.0.5/zoinks/exceptions.py` & `zoinks-0.0.6/zoinks/exceptions.py`

 * *Files identical despite different names*

### Comparing `zoinks-0.0.5/zoinks/exit_codes.py` & `zoinks-0.0.6/zoinks/exit_codes.py`

 * *Files identical despite different names*

### Comparing `zoinks-0.0.5/zoinks.egg-info/PKG-INFO` & `zoinks-0.0.6/zoinks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: zoinks
-Version: 0.0.5
+Version: 0.0.6
 Summary: Zoinks: a command-line utility to retrieve Zotero record values
 Home-page: https://github.com/mhucka/zoinks
 Author: Mike Hucka
 Author-email: mhucka@caltech.edu
 License: BSD 3-clause license
 Project-URL: Source Code, https://github.com/mhucka/zoinks
 Project-URL: Bug Tracker, https://github.com/mhucka/zoinks/issues
 Keywords: Python,applications
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
@@ -82,18 +81,16 @@
 
 I would be happy to receive your help and participation if you are interested.  Everyone is asked to read and respect the [code of conduct](CONDUCT.md) when participating in this project.  Development generally takes place on the `development` branch.
 
 
 License
 -------
 
-This software is Copyright (C) 2022, by Michael Hucka and the California Institute of Technology (Pasadena, California, USA).  This software is freely distributed under a 3-clause BSD type license.  Please see the [LICENSE](LICENSE) file for more information.
+This software is Copyright (C) 2022&ndash;2023, by Michael Hucka and the California Institute of Technology (Pasadena, California, USA).  This software is freely distributed under a 3-clause BSD type license.  Please see the [LICENSE](LICENSE) file for more information.
 
 
 Acknowledgments
 ---------------
 
 This work is a personal project developed by the author, using computing facilities and other resources of the [California Institute of Technology Library](https://www.library.caltech.edu).
 
 The [vector artwork](https://thenounproject.com/term/surprise/2696259/) of a surprised person, used as the icon for this repository, was created by [Adrien Coquet](https://thenounproject.com/coquet_adrien/) from the Noun Project.  It is licensed under the Creative Commons [CC-BY 3.0](https://creativecommons.org/licenses/by/3.0/) license.
-
-
```

