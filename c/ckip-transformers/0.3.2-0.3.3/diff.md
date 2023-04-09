# Comparing `tmp/ckip-transformers-0.3.2.tar.gz` & `tmp/ckip-transformers-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckip-transformers-0.3.2.tar", last modified: Wed Aug 10 06:01:17 2022, max compression
+gzip compressed data, was "ckip-transformers-0.3.3.tar", last modified: Sun Apr  9 05:38:25 2023, max compression
```

## Comparing `ckip-transformers-0.3.2.tar` & `ckip-transformers-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 emfo       (501) staff       (20)        0 2022-08-10 06:01:17.627994 ckip-transformers-0.3.2/
--rw-r--r--   0 emfo       (501) staff       (20)    35149 2021-02-01 06:02:22.000000 ckip-transformers-0.3.2/LICENSE
--rw-r--r--   0 emfo       (501) staff       (20)       26 2021-02-01 06:53:21.000000 ckip-transformers-0.3.2/MANIFEST.in
--rw-r--r--   0 emfo       (501) staff       (20)    25418 2022-08-10 06:01:17.628322 ckip-transformers-0.3.2/PKG-INFO
--rw-r--r--   0 emfo       (501) staff       (20)    24484 2022-08-10 06:00:50.000000 ckip-transformers-0.3.2/README.rst
-drwxr-xr-x   0 emfo       (501) staff       (20)        0 2022-08-10 06:01:17.624657 ckip-transformers-0.3.2/ckip_transformers/
--rw-r--r--   0 emfo       (501) staff       (20)      403 2022-08-10 06:00:50.000000 ckip-transformers-0.3.2/ckip_transformers/__init__.py
-drwxr-xr-x   0 emfo       (501) staff       (20)        0 2022-08-10 06:01:17.627683 ckip-transformers-0.3.2/ckip_transformers/nlp/
--rw-r--r--   0 emfo       (501) staff       (20)      298 2022-06-26 08:53:50.000000 ckip-transformers-0.3.2/ckip_transformers/nlp/__init__.py
--rw-r--r--   0 emfo       (501) staff       (20)    12388 2022-08-10 06:00:50.000000 ckip-transformers-0.3.2/ckip_transformers/nlp/driver.py
--rw-r--r--   0 emfo       (501) staff       (20)     9457 2022-08-10 06:00:50.000000 ckip-transformers-0.3.2/ckip_transformers/nlp/util.py
-drwxr-xr-x   0 emfo       (501) staff       (20)        0 2022-08-10 06:01:17.626472 ckip-transformers-0.3.2/ckip_transformers.egg-info/
--rw-r--r--   0 emfo       (501) staff       (20)    25418 2022-08-10 06:01:17.000000 ckip-transformers-0.3.2/ckip_transformers.egg-info/PKG-INFO
--rw-r--r--   0 emfo       (501) staff       (20)      394 2022-08-10 06:01:17.000000 ckip-transformers-0.3.2/ckip_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 emfo       (501) staff       (20)        1 2022-08-10 06:01:17.000000 ckip-transformers-0.3.2/ckip_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 emfo       (501) staff       (20)       44 2022-08-10 06:01:17.000000 ckip-transformers-0.3.2/ckip_transformers.egg-info/requires.txt
--rw-r--r--   0 emfo       (501) staff       (20)       18 2022-08-10 06:01:17.000000 ckip-transformers-0.3.2/ckip_transformers.egg-info/top_level.txt
--rw-r--r--   0 emfo       (501) staff       (20)       57 2021-06-16 06:01:27.000000 ckip-transformers-0.3.2/pyproject.toml
--rw-r--r--   0 emfo       (501) staff       (20)       80 2022-08-10 06:01:17.628730 ckip-transformers-0.3.2/setup.cfg
--rw-r--r--   0 emfo       (501) staff       (20)     1944 2022-06-26 08:53:50.000000 ckip-transformers-0.3.2/setup.py
+drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 05:38:25.973787 ckip-transformers-0.3.3/
+-rw-r--r--   0 emfo       (501) staff       (20)    35149 2021-02-01 06:02:22.000000 ckip-transformers-0.3.3/LICENSE
+-rw-r--r--   0 emfo       (501) staff       (20)       26 2021-02-01 06:53:21.000000 ckip-transformers-0.3.3/MANIFEST.in
+-rw-r--r--   0 emfo       (501) staff       (20)    25418 2023-04-09 05:38:25.973934 ckip-transformers-0.3.3/PKG-INFO
+-rw-r--r--   0 emfo       (501) staff       (20)    24484 2023-04-09 05:37:58.000000 ckip-transformers-0.3.3/README.rst
+drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 05:38:25.972128 ckip-transformers-0.3.3/ckip_transformers/
+-rw-r--r--   0 emfo       (501) staff       (20)      403 2023-04-09 05:37:58.000000 ckip-transformers-0.3.3/ckip_transformers/__init__.py
+drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 05:38:25.973636 ckip-transformers-0.3.3/ckip_transformers/nlp/
+-rw-r--r--   0 emfo       (501) staff       (20)      298 2023-04-09 05:37:58.000000 ckip-transformers-0.3.3/ckip_transformers/nlp/__init__.py
+-rw-r--r--   0 emfo       (501) staff       (20)    12460 2023-04-09 05:37:58.000000 ckip-transformers-0.3.3/ckip_transformers/nlp/driver.py
+-rw-r--r--   0 emfo       (501) staff       (20)     9620 2023-04-09 05:37:58.000000 ckip-transformers-0.3.3/ckip_transformers/nlp/util.py
+drwxr-xr-x   0 emfo       (501) staff       (20)        0 2023-04-09 05:38:25.973055 ckip-transformers-0.3.3/ckip_transformers.egg-info/
+-rw-r--r--   0 emfo       (501) staff       (20)    25418 2023-04-09 05:38:25.000000 ckip-transformers-0.3.3/ckip_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 emfo       (501) staff       (20)      394 2023-04-09 05:38:25.000000 ckip-transformers-0.3.3/ckip_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 emfo       (501) staff       (20)        1 2023-04-09 05:38:25.000000 ckip-transformers-0.3.3/ckip_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 emfo       (501) staff       (20)       44 2023-04-09 05:38:25.000000 ckip-transformers-0.3.3/ckip_transformers.egg-info/requires.txt
+-rw-r--r--   0 emfo       (501) staff       (20)       18 2023-04-09 05:38:25.000000 ckip-transformers-0.3.3/ckip_transformers.egg-info/top_level.txt
+-rw-r--r--   0 emfo       (501) staff       (20)       57 2021-06-16 06:01:27.000000 ckip-transformers-0.3.3/pyproject.toml
+-rw-r--r--   0 emfo       (501) staff       (20)       80 2023-04-09 05:38:25.974388 ckip-transformers-0.3.3/setup.cfg
+-rw-r--r--   0 emfo       (501) staff       (20)     1944 2023-04-09 05:37:58.000000 ckip-transformers-0.3.3/setup.py
```

### Comparing `ckip-transformers-0.3.2/LICENSE` & `ckip-transformers-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ckip-transformers-0.3.2/PKG-INFO` & `ckip-transformers-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ckip-transformers
-Version: 0.3.2
+Version: 0.3.3
 Summary: CKIP Transformers
 Home-page: https://ckip-transformers.readthedocs.io
 Author: Mu Yang
 Author-email: emfomy@gmail.com
 License: GPL-3.0
-Download-URL: https://ckip-transformers.readthedocs.io/tarball/0.3.2
+Download-URL: https://ckip-transformers.readthedocs.io/tarball/0.3.3
 Platform: linux_x86_64
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -493,13 +493,13 @@
 | † 我們重新訓練／測試我們的 BERT 模型於跟 CkipTagger 相同的資料集。
 
 License
 -------
 
 |GPL-3.0|
 
-Copyright (c) 2021 `CKIP Lab <https://ckip.iis.sinica.edu.tw>`__ under the `GPL-3.0 License <https://www.gnu.org/licenses/gpl-3.0.html>`__.
+Copyright (c) 2023 `CKIP Lab <https://ckip.iis.sinica.edu.tw>`__ under the `GPL-3.0 License <https://www.gnu.org/licenses/gpl-3.0.html>`__.
 
 .. |GPL-3.0| image:: https://www.gnu.org/graphics/gplv3-with-text-136x68.png
    :target: https://www.gnu.org/licenses/gpl-3.0.html
```

### Comparing `ckip-transformers-0.3.2/README.rst` & `ckip-transformers-0.3.3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -468,11 +468,11 @@
 | † 我們重新訓練／測試我們的 BERT 模型於跟 CkipTagger 相同的資料集。
 
 License
 -------
 
 |GPL-3.0|
 
-Copyright (c) 2021 `CKIP Lab <https://ckip.iis.sinica.edu.tw>`__ under the `GPL-3.0 License <https://www.gnu.org/licenses/gpl-3.0.html>`__.
+Copyright (c) 2023 `CKIP Lab <https://ckip.iis.sinica.edu.tw>`__ under the `GPL-3.0 License <https://www.gnu.org/licenses/gpl-3.0.html>`__.
 
 .. |GPL-3.0| image:: https://www.gnu.org/graphics/gplv3-with-text-136x68.png
    :target: https://www.gnu.org/licenses/gpl-3.0.html
```

### Comparing `ckip-transformers-0.3.2/ckip_transformers/nlp/driver.py` & `ckip-transformers-0.3.3/ckip_transformers/nlp/driver.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 """
 This module implements the CKIP Transformers NLP drivers.
 """
 
 __author__ = "Mu Yang <http://muyang.pro>"
-__copyright__ = "2021 CKIP Lab"
+__copyright__ = "2023 CKIP Lab"
 __license__ = "GPL-3.0"
 
 from typing import (
     List,
 )
 
 import numpy as np
@@ -73,16 +73,16 @@
                 The size of mini-batch.
             max_length : ``int``, *optional*
                 The maximum length of the sentence,
                 must not longer then the maximum sequence length for this model (i.e. ``tokenizer.model_max_length``).
             show_progress : ``int``, *optional*, defaults to True
                 Show progress bar.
             pin_memory : ``bool``, *optional*, defaults to True
-                Pin memory in order to accelerate the speed of data transfer to the GPU. This option is
-                incompatible with multiprocessing.
+                Pin memory in order to accelerate the speed of data transfer to the GPU. This option is incompatible with
+                multiprocessing. Disabled on CPU device.
 
         Returns
         -------
             ``List[List[str]]``
                 A list of list of words (``str``).
         """
 
@@ -173,16 +173,16 @@
                 The size of mini-batch.
             max_length : ``int``, *optional*
                 The maximum length of the sentence,
                 must not longer then the maximum sequence length for this model (i.e. ``tokenizer.model_max_length``).
             show_progress : ``int``, *optional*, defaults to True
                 Show progress bar.
             pin_memory : ``bool``, *optional*, defaults to True
-                Pin memory in order to accelerate the speed of data transfer to the GPU. This option is
-                incompatible with multiprocessing.
+                Pin memory in order to accelerate the speed of data transfer to the GPU. This option is incompatible with
+                multiprocessing. Disabled on CPU device.
 
         Returns
         -------
             ``List[List[str]]``
                 A list of list of POS tags (``str``).
         """
 
@@ -263,16 +263,16 @@
                 The size of mini-batch.
             max_length : ``int``, *optional*
                 The maximum length of the sentence,
                 must not longer then the maximum sequence length for this model (i.e. ``tokenizer.model_max_length``).
             show_progress : ``int``, *optional*, defaults to True
                 Show progress bar.
             pin_memory : ``bool``, *optional*, defaults to True
-                Pin memory in order to accelerate the speed of data transfer to the GPU. This option is
-                incompatible with multiprocessing.
+                Pin memory in order to accelerate the speed of data transfer to the GPU. This option is incompatible with
+                multiprocessing. Disabled on CPU device.
 
         Returns
         -------
             ``List[List[NerToken]]``
                 A list of list of entities (:class:`~.util.NerToken`).
         """
```

### Comparing `ckip-transformers-0.3.2/ckip_transformers/nlp/util.py` & `ckip-transformers-0.3.3/ckip_transformers/nlp/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding:utf-8 -*-
 
 """
 This module implements the utilities for CKIP Transformers NLP drivers.
 """
 
 __author__ = "Mu Yang <http://muyang.pro>"
-__copyright__ = "2021 CKIP Lab"
+__copyright__ = "2023 CKIP Lab"
 __license__ = "GPL-3.0"
 
 
 from abc import (
     ABCMeta,
     abstractmethod,
 )
@@ -119,18 +119,22 @@
                 The size of mini-batch.
             max_length : ``int``, *optional*
                 The maximum length of the sentence,
                 must not longer then the maximum sequence length for this model (i.e. ``tokenizer.model_max_length``).
             show_progress : ``bool``, *optional*, defaults to True
                 Show progress bar.
             pin_memory : ``bool``, *optional*, defaults to True
-                Pin memory in order to accelerate the speed of data transfer to the GPU. This option is
-                incompatible with multiprocessing.
+                Pin memory in order to accelerate the speed of data transfer to the GPU. This option is incompatible with
+                multiprocessing. Disabled on CPU device.
         """
+        # Disable pin memory on CPU device
+        if self.device.type == "cpu":
+            pin_memory = False
 
+        # Check max length
         model_max_length = self.tokenizer.model_max_length - 2  # Add [CLS] and [SEP]
         if max_length:
             assert max_length < model_max_length, (
                 "Sequence length is longer than the maximum sequence length for this model "
                 f"({max_length} > {model_max_length})."
             )
         else:
```

### Comparing `ckip-transformers-0.3.2/ckip_transformers.egg-info/PKG-INFO` & `ckip-transformers-0.3.3/ckip_transformers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ckip-transformers
-Version: 0.3.2
+Version: 0.3.3
 Summary: CKIP Transformers
 Home-page: https://ckip-transformers.readthedocs.io
 Author: Mu Yang
 Author-email: emfomy@gmail.com
 License: GPL-3.0
-Download-URL: https://ckip-transformers.readthedocs.io/tarball/0.3.2
+Download-URL: https://ckip-transformers.readthedocs.io/tarball/0.3.3
 Platform: linux_x86_64
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -493,13 +493,13 @@
 | † 我們重新訓練／測試我們的 BERT 模型於跟 CkipTagger 相同的資料集。
 
 License
 -------
 
 |GPL-3.0|
 
-Copyright (c) 2021 `CKIP Lab <https://ckip.iis.sinica.edu.tw>`__ under the `GPL-3.0 License <https://www.gnu.org/licenses/gpl-3.0.html>`__.
+Copyright (c) 2023 `CKIP Lab <https://ckip.iis.sinica.edu.tw>`__ under the `GPL-3.0 License <https://www.gnu.org/licenses/gpl-3.0.html>`__.
 
 .. |GPL-3.0| image:: https://www.gnu.org/graphics/gplv3-with-text-136x68.png
    :target: https://www.gnu.org/licenses/gpl-3.0.html
```

### Comparing `ckip-transformers-0.3.2/setup.py` & `ckip-transformers-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 
 __author__ = "Mu Yang <http://muyang.pro>"
-__copyright__ = "2021 CKIP Lab"
+__copyright__ = "2023 CKIP Lab"
 __license__ = "GPL-3.0"
 
 from setuptools import setup, find_namespace_packages
 import ckip_transformers as about
 
 ################################################################################
```

