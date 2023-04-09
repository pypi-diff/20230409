# Comparing `tmp/lupin-danquin-0.0.1.dev0.tar.gz` & `tmp/lupin-danquin-0.0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lupin-danquin-0.0.1.dev0.tar", last modified: Sun Apr  9 16:10:49 2023, max compression
+gzip compressed data, was "lupin-danquin-0.0.1.dev1.tar", last modified: Sun Apr  9 16:23:48 2023, max compression
```

## Comparing `lupin-danquin-0.0.1.dev0.tar` & `lupin-danquin-0.0.1.dev1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 16:10:49.436698 lupin-danquin-0.0.1.dev0/
--rw-rw-rw-   0        0        0     1093 2023-04-09 16:08:01.000000 lupin-danquin-0.0.1.dev0/LICENCE
--rw-rw-rw-   0        0        0      535 2023-04-09 16:10:49.436698 lupin-danquin-0.0.1.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     1214 2023-04-09 16:03:59.000000 lupin-danquin-0.0.1.dev0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 16:10:49.412677 lupin-danquin-0.0.1.dev0/lupin_danquin/
--rw-rw-rw-   0        0        0       28 2023-04-09 16:10:49.000000 lupin-danquin-0.0.1.dev0/lupin_danquin/__init__.py
--rw-rw-rw-   0        0        0      825 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev0/lupin_danquin/check_coding_rules.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:10:49.433696 lupin-danquin-0.0.1.dev0/lupin_danquin/core/
--rw-rw-rw-   0        0        0        0 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev0/lupin_danquin/core/__init__.py
--rw-rw-rw-   0        0        0     4561 2023-04-07 13:23:10.000000 lupin-danquin-0.0.1.dev0/lupin_danquin/core/application.py
--rw-rw-rw-   0        0        0      538 2023-04-09 15:14:35.000000 lupin-danquin-0.0.1.dev0/lupin_danquin/core/external_resources.py
--rw-rw-rw-   0        0        0     1797 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev0/lupin_danquin/core/global_variable.py
--rw-rw-rw-   0        0        0       23 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev0/lupin_danquin/core/line_ended.py
--rw-rw-rw-   0        0        0     1173 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev0/lupin_danquin/core/local_variable.py
--rw-rw-rw-   0        0        0     1448 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev0/lupin_danquin/core/parameter.py
--rw-rw-rw-   0        0        0     4619 2023-04-09 15:14:46.000000 lupin-danquin-0.0.1.dev0/lupin_danquin/core/program.py
--rw-rw-rw-   0        0        0      356 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev0/lupin_danquin/core/rules.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:10:49.434695 lupin-danquin-0.0.1.dev0/lupin_danquin/core/tools/
--rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev0/lupin_danquin/core/tools/__init__.py
--rw-rw-rw-   0        0        0      961 2023-04-09 15:57:16.000000 lupin-danquin-0.0.1.dev0/lupin_danquin/core/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:10:49.435695 lupin-danquin-0.0.1.dev0/lupin_danquin/core/val3_doc_generator/
--rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev0/lupin_danquin/core/val3_doc_generator/__init__.py
--rw-rw-rw-   0        0        0     1363 2023-04-09 15:14:35.000000 lupin-danquin-0.0.1.dev0/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py
--rw-rw-rw-   0        0        0     1461 2023-04-09 15:14:35.000000 lupin-danquin-0.0.1.dev0/lupin_danquin/documentation_extraction.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:10:49.425696 lupin-danquin-0.0.1.dev0/lupin_danquin.egg-info/
--rw-rw-rw-   0        0        0      535 2023-04-09 16:10:49.000000 lupin-danquin-0.0.1.dev0/lupin_danquin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      845 2023-04-09 16:10:49.000000 lupin-danquin-0.0.1.dev0/lupin_danquin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 16:10:49.000000 lupin-danquin-0.0.1.dev0/lupin_danquin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-09 15:55:39.000000 lupin-danquin-0.0.1.dev0/lupin_danquin.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       89 2023-04-09 16:10:49.000000 lupin-danquin-0.0.1.dev0/lupin_danquin.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-09 16:10:49.000000 lupin-danquin-0.0.1.dev0/lupin_danquin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      773 2023-04-09 16:10:49.441202 lupin-danquin-0.0.1.dev0/setup.cfg
--rw-rw-rw-   0        0        0      172 2023-04-09 15:52:50.000000 lupin-danquin-0.0.1.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:48.352696 lupin-danquin-0.0.1.dev1/
+-rw-rw-rw-   0        0        0     1093 2023-04-09 16:08:01.000000 lupin-danquin-0.0.1.dev1/LICENCE
+-rw-rw-rw-   0        0        0      573 2023-04-09 16:23:48.352696 lupin-danquin-0.0.1.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     1010 2023-04-09 16:15:47.000000 lupin-danquin-0.0.1.dev1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:48.327161 lupin-danquin-0.0.1.dev1/lupin_danquin/
+-rw-rw-rw-   0        0        0       28 2023-04-09 16:23:48.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/__init__.py
+-rw-rw-rw-   0        0        0      825 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/check_coding_rules.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:48.348185 lupin-danquin-0.0.1.dev1/lupin_danquin/core/
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/__init__.py
+-rw-rw-rw-   0        0        0     4561 2023-04-07 13:23:10.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/application.py
+-rw-rw-rw-   0        0        0      538 2023-04-09 15:14:35.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/external_resources.py
+-rw-rw-rw-   0        0        0     1797 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/global_variable.py
+-rw-rw-rw-   0        0        0       23 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/line_ended.py
+-rw-rw-rw-   0        0        0     1173 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/local_variable.py
+-rw-rw-rw-   0        0        0     1448 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/parameter.py
+-rw-rw-rw-   0        0        0     4619 2023-04-09 15:14:46.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/program.py
+-rw-rw-rw-   0        0        0      356 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/rules.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:48.349757 lupin-danquin-0.0.1.dev1/lupin_danquin/core/tools/
+-rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/tools/__init__.py
+-rw-rw-rw-   0        0        0      961 2023-04-09 15:57:16.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:48.351699 lupin-danquin-0.0.1.dev1/lupin_danquin/core/val3_doc_generator/
+-rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/val3_doc_generator/__init__.py
+-rw-rw-rw-   0        0        0     1363 2023-04-09 15:14:35.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py
+-rw-rw-rw-   0        0        0     1461 2023-04-09 15:14:35.000000 lupin-danquin-0.0.1.dev1/lupin_danquin/documentation_extraction.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:23:48.341183 lupin-danquin-0.0.1.dev1/lupin_danquin.egg-info/
+-rw-rw-rw-   0        0        0      573 2023-04-09 16:23:48.000000 lupin-danquin-0.0.1.dev1/lupin_danquin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      845 2023-04-09 16:23:48.000000 lupin-danquin-0.0.1.dev1/lupin_danquin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 16:23:48.000000 lupin-danquin-0.0.1.dev1/lupin_danquin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-09 15:55:39.000000 lupin-danquin-0.0.1.dev1/lupin_danquin.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       89 2023-04-09 16:23:48.000000 lupin-danquin-0.0.1.dev1/lupin_danquin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-09 16:23:48.000000 lupin-danquin-0.0.1.dev1/lupin_danquin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      828 2023-04-09 16:23:48.353696 lupin-danquin-0.0.1.dev1/setup.cfg
+-rw-rw-rw-   0        0        0      172 2023-04-09 15:52:50.000000 lupin-danquin-0.0.1.dev1/setup.py
```

### Comparing `lupin-danquin-0.0.1.dev0/LICENCE` & `lupin-danquin-0.0.1.dev1/LICENCE`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev0/PKG-INFO` & `lupin-danquin-0.0.1.dev1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: lupin-danquin
-Version: 0.0.1.dev0
-Summary: Testing - Documentation VAL3 from Code
+Version: 0.0.1.dev1
+Summary: Testing - Documentation
 License: MIT License
 Keywords: documentation,testing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Documentation
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Provides-Extra: test
 License-File: LICENCE
+
+Test VAL3 code and generate documentation from it
```

### Comparing `lupin-danquin-0.0.1.dev0/README.md` & `lupin-danquin-0.0.1.dev1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Documentation extraction
 
 ## Purpose
 
 "documentation_extraction.py" Python script allow to create SDD documentation from source code.
 
-The goal is to replace the hand written wiki page accessible here: https://gitlab.com/lupindental/arsene/robotics/production/lupin.robot.staubli/-/wikis/Software-Detailed-Design-Robot-Application-unit
-
 ## Run it
 
 1. Go to current directory.
 2. Execute
 > python documentation_extraction.py
 3. Result is available in "./val3_documentation.md"
```

### Comparing `lupin-danquin-0.0.1.dev0/lupin_danquin/check_coding_rules.py` & `lupin-danquin-0.0.1.dev1/lupin_danquin/check_coding_rules.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev0/lupin_danquin/core/application.py` & `lupin-danquin-0.0.1.dev1/lupin_danquin/core/application.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev0/lupin_danquin/core/external_resources.py` & `lupin-danquin-0.0.1.dev1/lupin_danquin/core/external_resources.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev0/lupin_danquin/core/global_variable.py` & `lupin-danquin-0.0.1.dev1/lupin_danquin/core/global_variable.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev0/lupin_danquin/core/local_variable.py` & `lupin-danquin-0.0.1.dev1/lupin_danquin/core/local_variable.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev0/lupin_danquin/core/parameter.py` & `lupin-danquin-0.0.1.dev1/lupin_danquin/core/parameter.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev0/lupin_danquin/core/program.py` & `lupin-danquin-0.0.1.dev1/lupin_danquin/core/program.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev0/lupin_danquin/core/tools/utils.py` & `lupin-danquin-0.0.1.dev1/lupin_danquin/core/tools/utils.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev0/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py` & `lupin-danquin-0.0.1.dev1/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev0/lupin_danquin/documentation_extraction.py` & `lupin-danquin-0.0.1.dev1/lupin_danquin/documentation_extraction.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev0/lupin_danquin.egg-info/PKG-INFO` & `lupin-danquin-0.0.1.dev1/lupin_danquin.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: lupin-danquin
-Version: 0.0.1.dev0
-Summary: Testing - Documentation VAL3 from Code
+Version: 0.0.1.dev1
+Summary: Testing - Documentation
 License: MIT License
 Keywords: documentation,testing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Documentation
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Provides-Extra: test
 License-File: LICENCE
+
+Test VAL3 code and generate documentation from it
```

### Comparing `lupin-danquin-0.0.1.dev0/lupin_danquin.egg-info/SOURCES.txt` & `lupin-danquin-0.0.1.dev1/lupin_danquin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev0/setup.cfg` & `lupin-danquin-0.0.1.dev1/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 7570 696e 2d64 616e 7175 696e   = lupin-danquin
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 302e  ..version = 0.0.
-00000030: 312e 6465 7630 0d0a 6465 7363 7269 7074  1.dev0..descript
+00000030: 312e 6465 7631 0d0a 6465 7363 7269 7074  1.dev1..descript
 00000040: 696f 6e20 3d20 5465 7374 696e 6720 2d20  ion = Testing - 
-00000050: 446f 6375 6d65 6e74 6174 696f 6e20 5641  Documentation VA
-00000060: 4c33 2066 726f 6d20 436f 6465 0d0a 6b65  L3 from Code..ke
-00000070: 7977 6f72 6473 203d 2064 6f63 756d 656e  ywords = documen
-00000080: 7461 7469 6f6e 2c20 7465 7374 696e 670d  tation, testing.
-00000090: 0a6c 6963 656e 7365 203d 204d 4954 204c  .license = MIT L
-000000a0: 6963 656e 7365 0d0a 636c 6173 7369 6669  icense..classifi
-000000b0: 6572 7320 3d20 0d0a 0944 6576 656c 6f70  ers = ...Develop
-000000c0: 6d65 6e74 2053 7461 7475 7320 3a3a 2033  ment Status :: 3
-000000d0: 202d 2041 6c70 6861 0d0a 0949 6e74 656e   - Alpha...Inten
-000000e0: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
-000000f0: 496e 666f 726d 6174 696f 6e20 5465 6368  Information Tech
-00000100: 6e6f 6c6f 6779 0d0a 0954 6f70 6963 203a  nology...Topic :
-00000110: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
-00000120: 6f70 6d65 6e74 203a 3a20 5465 7374 696e  opment :: Testin
-00000130: 670d 0a09 546f 7069 6320 3a3a 2044 6f63  g...Topic :: Doc
-00000140: 756d 656e 7461 7469 6f6e 0d0a 0950 726f  umentation...Pro
-00000150: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000160: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000170: 2e31 300d 0a09 4c69 6365 6e73 6520 3a3a  .10...License ::
-00000180: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-00000190: 204d 4954 204c 6963 656e 7365 0d0a 0d0a   MIT License....
-000001a0: 5b6f 7074 696f 6e73 5d0d 0a7a 6970 5f73  [options]..zip_s
-000001b0: 6166 6520 3d20 4661 6c73 650d 0a69 6e63  afe = False..inc
-000001c0: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
-000001d0: 6120 3d20 5472 7565 0d0a 7061 636b 6167  a = True..packag
-000001e0: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
-000001f0: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-00000200: 332e 3130 0d0a 696e 7374 616c 6c5f 7265  3.10..install_re
-00000210: 7175 6972 6573 203d 200d 0a09 7479 7065  quires = ...type
-00000220: 725b 616c 6c5d 3d3d 302e 372e 300d 0a09  r[all]==0.7.0...
-00000230: 7079 7468 6f6e 2d64 6f74 656e 763d 3d31  python-dotenv==1
-00000240: 2e30 2e30 0d0a 094a 696e 6a61 323d 3d33  .0.0...Jinja2==3
-00000250: 2e31 2e32 0d0a 0d0a 5b6f 7074 696f 6e73  .1.2....[options
-00000260: 2e65 7874 7261 735f 7265 7175 6972 655d  .extras_require]
-00000270: 0d0a 7465 7374 203d 200d 0a09 7079 7465  ..test = ...pyte
-00000280: 7374 3d3d 372e 322e 320d 0a09 666c 616b  st==7.2.2...flak
-00000290: 6538 3d3d 362e 302e 300d 0a0d 0a5b 6f70  e8==6.0.0....[op
-000002a0: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-000002b0: 696e 645d 0d0a 6578 636c 7564 6520 3d20  ind]..exclude = 
-000002c0: 0d0a 096c 7570 696e 5f64 616e 7175 696e  ...lupin_danquin
-000002d0: 2e74 6573 7473 2a0d 0a0d 0a5b 6567 675f  .tests*....[egg_
-000002e0: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-000002f0: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-00000300: 300d 0a0d 0a                             0....
+00000050: 446f 6375 6d65 6e74 6174 696f 6e0d 0a6c  Documentation..l
+00000060: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
+00000070: 3d20 5465 7374 2056 414c 3320 636f 6465  = Test VAL3 code
+00000080: 2061 6e64 2067 656e 6572 6174 6520 646f   and generate do
+00000090: 6375 6d65 6e74 6174 696f 6e20 6672 6f6d  cumentation from
+000000a0: 2069 740d 0a6b 6579 776f 7264 7320 3d20   it..keywords = 
+000000b0: 646f 6375 6d65 6e74 6174 696f 6e2c 2074  documentation, t
+000000c0: 6573 7469 6e67 0d0a 6c69 6365 6e73 6520  esting..license 
+000000d0: 3d20 4d49 5420 4c69 6365 6e73 650d 0a63  = MIT License..c
+000000e0: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
+000000f0: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
+00000100: 7573 203a 3a20 3320 2d20 416c 7068 610d  us :: 3 - Alpha.
+00000110: 0a09 496e 7465 6e64 6564 2041 7564 6965  ..Intended Audie
+00000120: 6e63 6520 3a3a 2049 6e66 6f72 6d61 7469  nce :: Informati
+00000130: 6f6e 2054 6563 686e 6f6c 6f67 790d 0a09  on Technology...
+00000140: 546f 7069 6320 3a3a 2053 6f66 7477 6172  Topic :: Softwar
+00000150: 6520 4465 7665 6c6f 706d 656e 7420 3a3a  e Development ::
+00000160: 2054 6573 7469 6e67 0d0a 0954 6f70 6963   Testing...Topic
+00000170: 203a 3a20 446f 6375 6d65 6e74 6174 696f   :: Documentatio
+00000180: 6e0d 0a09 5072 6f67 7261 6d6d 696e 6720  n...Programming 
+00000190: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000001a0: 6f6e 203a 3a20 332e 3130 0d0a 094c 6963  on :: 3.10...Lic
+000001b0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+000001c0: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
+000001d0: 6e73 650d 0a0d 0a5b 6f70 7469 6f6e 735d  nse....[options]
+000001e0: 0d0a 7a69 705f 7361 6665 203d 2046 616c  ..zip_safe = Fal
+000001f0: 7365 0d0a 696e 636c 7564 655f 7061 636b  se..include_pack
+00000200: 6167 655f 6461 7461 203d 2054 7275 650d  age_data = True.
+00000210: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
+00000220: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
+00000230: 6573 203d 203e 3d33 2e31 300d 0a69 6e73  es = >=3.10..ins
+00000240: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
+00000250: 0d0a 0974 7970 6572 5b61 6c6c 5d3d 3d30  ...typer[all]==0
+00000260: 2e37 2e30 0d0a 0970 7974 686f 6e2d 646f  .7.0...python-do
+00000270: 7465 6e76 3d3d 312e 302e 300d 0a09 4a69  tenv==1.0.0...Ji
+00000280: 6e6a 6132 3d3d 332e 312e 320d 0a0d 0a5b  nja2==3.1.2....[
+00000290: 6f70 7469 6f6e 732e 6578 7472 6173 5f72  options.extras_r
+000002a0: 6571 7569 7265 5d0d 0a74 6573 7420 3d20  equire]..test = 
+000002b0: 0d0a 0970 7974 6573 743d 3d37 2e32 2e32  ...pytest==7.2.2
+000002c0: 0d0a 0966 6c61 6b65 383d 3d36 2e30 2e30  ...flake8==6.0.0
+000002d0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
+000002e0: 6b61 6765 732e 6669 6e64 5d0d 0a65 7863  kages.find]..exc
+000002f0: 6c75 6465 203d 200d 0a09 6c75 7069 6e5f  lude = ...lupin_
+00000300: 6461 6e71 7569 6e2e 7465 7374 732a 0d0a  danquin.tests*..
+00000310: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+00000320: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+00000330: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

