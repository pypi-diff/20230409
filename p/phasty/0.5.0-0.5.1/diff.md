# Comparing `tmp/phasty-0.5.0.tar.gz` & `tmp/phasty-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phasty-0.5.0.tar", last modified: Sat Mar  4 15:29:44 2023, max compression
+gzip compressed data, was "phasty-0.5.1.tar", last modified: Sun Apr  9 11:11:56 2023, max compression
```

## Comparing `phasty-0.5.0.tar` & `phasty-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-04 15:29:44.658212 phasty-0.5.0/
--rw-rw-rw-   0        0        0     1517 2022-08-07 15:41:55.000000 phasty-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     2822 2023-03-04 15:29:44.659210 phasty-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     2175 2023-02-02 08:39:22.000000 phasty-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-04 15:29:44.601219 phasty-0.5.0/phasty/
--rw-rw-rw-   0        0        0      105 2023-03-04 12:03:07.000000 phasty-0.5.0/phasty/__init__.py
--rw-rw-rw-   0        0        0     1333 2023-03-04 13:18:48.000000 phasty-0.5.0/phasty/parser.py
--rw-rw-rw-   0        0        0     2454 2023-03-04 12:52:32.000000 phasty-0.5.0/phasty/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-03-04 15:29:44.646211 phasty-0.5.0/phasty.egg-info/
--rw-rw-rw-   0        0        0     2822 2023-03-04 15:29:44.000000 phasty-0.5.0/phasty.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-03-04 15:29:44.000000 phasty-0.5.0/phasty.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-04 15:29:44.000000 phasty-0.5.0/phasty.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      141 2023-03-04 15:29:44.000000 phasty-0.5.0/phasty.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-04 15:29:44.000000 phasty-0.5.0/phasty.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      112 2022-08-09 08:57:59.000000 phasty-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0      868 2023-03-04 15:29:44.662210 phasty-0.5.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-04 15:29:44.655215 phasty-0.5.0/tests/
--rw-rw-rw-   0        0        0      250 2023-02-02 11:04:32.000000 phasty-0.5.0/tests/test_parser.py
--rw-rw-rw-   0        0        0      900 2022-09-06 08:21:36.000000 phasty-0.5.0/tests/test_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-09 11:11:56.270657 phasty-0.5.1/
+-rw-rw-rw-   0        0        0     1517 2022-08-07 15:41:55.000000 phasty-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0     2787 2023-04-09 11:11:56.271657 phasty-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2140 2023-04-09 11:10:39.000000 phasty-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 11:11:56.240656 phasty-0.5.1/phasty/
+-rw-rw-rw-   0        0        0      105 2023-04-09 11:10:39.000000 phasty-0.5.1/phasty/__init__.py
+-rw-rw-rw-   0        0        0     1333 2023-04-09 11:08:27.000000 phasty-0.5.1/phasty/parser.py
+-rw-rw-rw-   0        0        0     2454 2023-04-09 11:08:27.000000 phasty-0.5.1/phasty/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-09 11:11:56.258653 phasty-0.5.1/phasty.egg-info/
+-rw-rw-rw-   0        0        0     2787 2023-04-09 11:11:56.000000 phasty-0.5.1/phasty.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-04-09 11:11:56.000000 phasty-0.5.1/phasty.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 11:11:56.000000 phasty-0.5.1/phasty.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      166 2023-04-09 11:11:56.000000 phasty-0.5.1/phasty.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-09 11:11:56.000000 phasty-0.5.1/phasty.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      112 2022-08-09 08:57:59.000000 phasty-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0      895 2023-04-09 11:11:56.279673 phasty-0.5.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-09 11:11:56.268654 phasty-0.5.1/tests/
+-rw-rw-rw-   0        0        0      250 2023-04-09 11:08:27.000000 phasty-0.5.1/tests/test_parser.py
+-rw-rw-rw-   0        0        0      900 2023-04-09 11:08:27.000000 phasty-0.5.1/tests/test_wrapper.py
```

### Comparing `phasty-0.5.0/LICENSE` & `phasty-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phasty-0.5.0/PKG-INFO` & `phasty-0.5.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phasty
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Python interface for PHAST (phylogenetic analysis with space/time models).
 Home-page: https://github.com/yuanx749/phasty
 Author: Xiao Yuan
 Author-email: yuanx749@gmail.com
 License: BSD 3-Clause License
 Keywords: phylogenetics
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE
 
 # phasty
 
 [![PyPI version](https://badge.fury.io/py/phasty.svg)](https://badge.fury.io/py/phasty)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/7baee8cdd9784bfdbdfc5840260426b5)](https://www.codacy.com/gh/yuanx749/phasty/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=yuanx749/phasty&amp;utm_campaign=Badge_Grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/319819871685432882de8aa62c58fec0)](https://app.codacy.com/gh/yuanx749/phasty/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![codecov](https://codecov.io/gh/yuanx749/phasty/branch/main/graph/badge.svg?token=NT7LUW1ECF)](https://codecov.io/gh/yuanx749/phasty)
 
 A Python interface for PHAST (phylogenetic analysis with space/time models).
 
 ## Description
 
 [PHAST](http://compgen.cshl.edu/phast/) is a package consisting of command-line programs for comparative genomics. It supports several nucleotide substitution models. This package phasty provides Python wrappers for some major programs so that it is easier to integrate them into complicated workflows. It can also parse some files from plain text to more computer-friendly forms to help downstream analysis.
```

### Comparing `phasty-0.5.0/README.md` & `phasty-0.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # phasty
 
 [![PyPI version](https://badge.fury.io/py/phasty.svg)](https://badge.fury.io/py/phasty)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/7baee8cdd9784bfdbdfc5840260426b5)](https://www.codacy.com/gh/yuanx749/phasty/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=yuanx749/phasty&amp;utm_campaign=Badge_Grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/319819871685432882de8aa62c58fec0)](https://app.codacy.com/gh/yuanx749/phasty/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![codecov](https://codecov.io/gh/yuanx749/phasty/branch/main/graph/badge.svg?token=NT7LUW1ECF)](https://codecov.io/gh/yuanx749/phasty)
 
 A Python interface for PHAST (phylogenetic analysis with space/time models).
 
 ## Description
 
 [PHAST](http://compgen.cshl.edu/phast/) is a package consisting of command-line programs for comparative genomics. It supports several nucleotide substitution models. This package phasty provides Python wrappers for some major programs so that it is easier to integrate them into complicated workflows. It can also parse some files from plain text to more computer-friendly forms to help downstream analysis.
```

### Comparing `phasty-0.5.0/phasty/parser.py` & `phasty-0.5.1/phasty/parser.py`

 * *Files identical despite different names*

### Comparing `phasty-0.5.0/phasty/wrapper.py` & `phasty-0.5.1/phasty/wrapper.py`

 * *Files identical despite different names*

### Comparing `phasty-0.5.0/phasty.egg-info/PKG-INFO` & `phasty-0.5.1/phasty.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phasty
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Python interface for PHAST (phylogenetic analysis with space/time models).
 Home-page: https://github.com/yuanx749/phasty
 Author: Xiao Yuan
 Author-email: yuanx749@gmail.com
 License: BSD 3-Clause License
 Keywords: phylogenetics
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE
 
 # phasty
 
 [![PyPI version](https://badge.fury.io/py/phasty.svg)](https://badge.fury.io/py/phasty)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/7baee8cdd9784bfdbdfc5840260426b5)](https://www.codacy.com/gh/yuanx749/phasty/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=yuanx749/phasty&amp;utm_campaign=Badge_Grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/319819871685432882de8aa62c58fec0)](https://app.codacy.com/gh/yuanx749/phasty/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![codecov](https://codecov.io/gh/yuanx749/phasty/branch/main/graph/badge.svg?token=NT7LUW1ECF)](https://codecov.io/gh/yuanx749/phasty)
 
 A Python interface for PHAST (phylogenetic analysis with space/time models).
 
 ## Description
 
 [PHAST](http://compgen.cshl.edu/phast/) is a package consisting of command-line programs for comparative genomics. It supports several nucleotide substitution models. This package phasty provides Python wrappers for some major programs so that it is easier to integrate them into complicated workflows. It can also parse some files from plain text to more computer-friendly forms to help downstream analysis.
```

### Comparing `phasty-0.5.0/setup.cfg` & `phasty-0.5.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -37,19 +37,20 @@
 00000240: 6e75 6d70 790d 0a70 7974 686f 6e5f 7265  numpy..python_re
 00000250: 7175 6972 6573 203d 203e 3d33 2e38 0d0a  quires = >=3.8..
 00000260: 0d0a 5b6f 7074 696f 6e73 2e65 7874 7261  ..[options.extra
 00000270: 735f 7265 7175 6972 655d 0d0a 6465 7620  s_require]..dev 
 00000280: 3d20 0d0a 0970 7265 2d63 6f6d 6d69 740d  = ...pre-commit.
 00000290: 0a09 626c 6163 6b3d 3d32 322e 332e 300d  ..black==22.3.0.
 000002a0: 0a09 666c 616b 6538 3d3d 342e 302e 310d  ..flake8==4.0.1.
-000002b0: 0a09 6973 6f72 743d 3d35 2e31 322e 310d  ..isort==5.12.1.
+000002b0: 0a09 6973 6f72 743d 3d35 2e31 322e 300d  ..isort==5.12.0.
 000002c0: 0a09 7079 7465 7374 0d0a 0970 7974 6573  ..pytest...pytes
 000002d0: 742d 636f 760d 0a64 6f63 203d 200d 0a09  t-cov..doc = ...
 000002e0: 7370 6869 6e78 3d3d 352e 332e 300d 0a09  sphinx==5.3.0...
 000002f0: 6675 726f 3d3d 3230 3232 2e31 322e 370d  furo==2022.12.7.
 00000300: 0a09 6d79 7374 2d70 6172 7365 723d 3d30  ..myst-parser==0
-00000310: 2e31 382e 310d 0a0d 0a5b 666c 616b 6538  .18.1....[flake8
-00000320: 5d0d 0a69 676e 6f72 6520 3d20 4634 3033  ]..ignore = F403
-00000330: 2c20 4634 3031 0d0a 0d0a 5b65 6767 5f69  , F401....[egg_i
-00000340: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-00000350: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-00000360: 0d0a 0d0a                                ....
+00000310: 2e31 382e 310d 0a09 7370 6869 6e78 2d63  .18.1...sphinx-c
+00000320: 6f70 7962 7574 746f 6e3d 3d30 2e35 2e31  opybutton==0.5.1
+00000330: 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a 6967  ....[flake8]..ig
+00000340: 6e6f 7265 203d 2046 3430 332c 2046 3430  nore = F403, F40
+00000350: 310d 0a0d 0a5b 6567 675f 696e 666f 5d0d  1....[egg_info].
+00000360: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+00000370: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

### Comparing `phasty-0.5.0/tests/test_wrapper.py` & `phasty-0.5.1/tests/test_wrapper.py`

 * *Files identical despite different names*

