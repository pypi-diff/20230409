# Comparing `tmp/taskgen-0.3.7.1.tar.gz` & `tmp/taskgen-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskgen-0.3.7.1.tar", last modified: Sun Mar 12 16:35:32 2023, max compression
+gzip compressed data, was "taskgen-0.3.8.tar", last modified: Sun Apr  9 20:55:28 2023, max compression
```

## Comparing `taskgen-0.3.7.1.tar` & `taskgen-0.3.8.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxr-xr-x   0 artyomzolotarevskiy   (501) staff       (20)        0 2023-03-12 16:35:32.191263 taskgen-0.3.7.1/
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     2634 2023-03-12 16:35:32.191107 taskgen-0.3.7.1/PKG-INFO
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     2108 2023-02-25 14:50:29.000000 taskgen-0.3.7.1/README.md
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)       38 2023-03-12 16:35:32.191308 taskgen-0.3.7.1/setup.cfg
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     1295 2023-03-12 16:22:41.000000 taskgen-0.3.7.1/setup.py
-drwxr-xr-x   0 artyomzolotarevskiy   (501) staff       (20)        0 2023-03-12 16:35:32.190055 taskgen-0.3.7.1/taskgen/
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     2115 2023-03-12 16:22:36.000000 taskgen-0.3.7.1/taskgen/__init__.py
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)    67936 2023-03-12 16:24:39.000000 taskgen-0.3.7.1/taskgen/generator.py
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     7462 2023-03-07 01:11:23.000000 taskgen-0.3.7.1/taskgen/html2pdf.py
-drwxr-xr-x   0 artyomzolotarevskiy   (501) staff       (20)        0 2023-03-12 16:35:32.190922 taskgen-0.3.7.1/taskgen.egg-info/
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     2634 2023-03-12 16:35:32.000000 taskgen-0.3.7.1/taskgen.egg-info/PKG-INFO
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)      233 2023-03-12 16:35:32.000000 taskgen-0.3.7.1/taskgen.egg-info/SOURCES.txt
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)        1 2023-03-12 16:35:32.000000 taskgen-0.3.7.1/taskgen.egg-info/dependency_links.txt
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)      175 2023-03-12 16:35:32.000000 taskgen-0.3.7.1/taskgen.egg-info/requires.txt
--rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)        8 2023-03-12 16:35:32.000000 taskgen-0.3.7.1/taskgen.egg-info/top_level.txt
+drwxr-xr-x   0 artyomzolotarevskiy   (501) staff       (20)        0 2023-04-09 20:55:28.221231 taskgen-0.3.8/
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     2632 2023-04-09 20:55:28.221047 taskgen-0.3.8/PKG-INFO
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     2108 2023-02-25 14:50:29.000000 taskgen-0.3.8/README.md
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)       38 2023-04-09 20:55:28.221284 taskgen-0.3.8/setup.cfg
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     1293 2023-04-08 21:48:53.000000 taskgen-0.3.8/setup.py
+drwxr-xr-x   0 artyomzolotarevskiy   (501) staff       (20)        0 2023-04-09 20:55:28.219773 taskgen-0.3.8/taskgen/
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     2390 2023-04-08 21:51:45.000000 taskgen-0.3.8/taskgen/__init__.py
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     2128 2023-04-08 21:46:42.000000 taskgen-0.3.8/taskgen/config.py
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)    16514 2023-04-09 20:53:57.000000 taskgen-0.3.8/taskgen/converters.py
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)    14818 2023-04-09 20:25:40.000000 taskgen-0.3.8/taskgen/functions.py
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)    10426 2023-04-09 17:48:01.000000 taskgen-0.3.8/taskgen/html.py
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)    21693 2023-04-09 15:32:02.000000 taskgen-0.3.8/taskgen/main.py
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     8654 2023-04-08 21:41:31.000000 taskgen-0.3.8/taskgen/moodle.py
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     1633 2023-04-08 21:41:38.000000 taskgen-0.3.8/taskgen/stats.py
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     7072 2023-04-09 20:27:26.000000 taskgen-0.3.8/taskgen/tex.py
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)      323 2023-04-09 20:20:45.000000 taskgen-0.3.8/taskgen/variable_types.py
+drwxr-xr-x   0 artyomzolotarevskiy   (501) staff       (20)        0 2023-04-09 20:55:28.220836 taskgen-0.3.8/taskgen.egg-info/
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)     2632 2023-04-09 20:55:28.000000 taskgen-0.3.8/taskgen.egg-info/PKG-INFO
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)      361 2023-04-09 20:55:28.000000 taskgen-0.3.8/taskgen.egg-info/SOURCES.txt
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)        1 2023-04-09 20:55:28.000000 taskgen-0.3.8/taskgen.egg-info/dependency_links.txt
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)      175 2023-04-09 20:55:28.000000 taskgen-0.3.8/taskgen.egg-info/requires.txt
+-rw-r--r--   0 artyomzolotarevskiy   (501) staff       (20)        8 2023-04-09 20:55:28.000000 taskgen-0.3.8/taskgen.egg-info/top_level.txt
```

### Comparing `taskgen-0.3.7.1/PKG-INFO` & `taskgen-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskgen
-Version: 0.3.7.1
+Version: 0.3.8
 Summary: Ядро генератора банка задач на базе MiKTeX и Jupyter Notebook
 Home-page: https://github.com/artyom-zolotarevskiy/taskgen-core
 Author: Артём Золотаревский
 Author-email: artyom@zolotarevskiy.ru
 Project-URL: Bug Tracker, https://github.com/artyom-zolotarevskiy/taskgen-core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `taskgen-0.3.7.1/README.md` & `taskgen-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `taskgen-0.3.7.1/setup.py` & `taskgen-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         line
         for line in lineiter
         if line and not line.startswith("#") and not line.startswith("git+")
     ]
 
 
 setup(name='taskgen',
-      version='0.3.7.1',
+      version='0.3.8',
       author='Артём Золотаревский',
       author_email='artyom@zolotarevskiy.ru',
       description='Ядро генератора банка задач на базе MiKTeX и Jupyter Notebook',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/artyom-zolotarevskiy/taskgen-core',
       project_urls={
```

### Comparing `taskgen-0.3.7.1/taskgen/__init__.py` & `taskgen-0.3.8/taskgen/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,20 +20,27 @@
 Связь с автором: artyom@zolotarevskiy.ru
 
 Благодарности
 -------
 Отдельная благодарность научному руководителю, Павлу Евгеньевичу Рябову,
 за постановку задачи и постоянное внимание к работе.
 '''
-from taskgen.generator import *
-from taskgen.html2pdf import *
+from taskgen.config import *
+from taskgen.functions import *
+from taskgen.converters import *
+from taskgen.stats import *
+from taskgen.tex import *
+from taskgen.html import *
+from taskgen.moodle import *
+from taskgen.variable_types import *
+from taskgen.main import *
 
 format = "%(asctime)s: %(message)s"
 logging.basicConfig(format=format, level=logging.INFO, datefmt="%H:%M:%S")
 
 __title__ = 'artyom-zolotarevskiy'
-__version__ = '0.3.7.1'
+__version__ = '0.3.8'
 __url__ = 'https://github.com/artyom-zolotarevskiy/taskgen-core'
 __author__ = 'Артём Золотаревский'
 __author_email__ = 'artyom@zolotarevskiy.ru'
 
-__all__ = ["generator", "html2pdf"]
+__all__ = ["config", "functions", "converters", "stats", "tex", "html", "moodle", "variable_types", "main"]
```

### Comparing `taskgen-0.3.7.1/taskgen.egg-info/PKG-INFO` & `taskgen-0.3.8/taskgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskgen
-Version: 0.3.7.1
+Version: 0.3.8
 Summary: Ядро генератора банка задач на базе MiKTeX и Jupyter Notebook
 Home-page: https://github.com/artyom-zolotarevskiy/taskgen-core
 Author: Артём Золотаревский
 Author-email: artyom@zolotarevskiy.ru
 Project-URL: Bug Tracker, https://github.com/artyom-zolotarevskiy/taskgen-core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

