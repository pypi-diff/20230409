# Comparing `tmp/freeplot-0.3.0.tar.gz` & `tmp/freeplot-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeplot-0.3.0.tar", last modified: Sat Feb 25 07:42:25 2023, max compression
+gzip compressed data, was "freeplot-0.3.1.tar", last modified: Sun Apr  9 12:09:27 2023, max compression
```

## Comparing `freeplot-0.3.0.tar` & `freeplot-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-02-25 07:42:25.689582 freeplot-0.3.0/
--rw-rw-rw-   0        0        0     1085 2022-09-19 12:06:04.000000 freeplot-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     7420 2023-02-25 07:42:25.689582 freeplot-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     6937 2023-01-01 10:56:12.000000 freeplot-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-25 07:42:25.670416 freeplot-0.3.0/freeplot/
--rw-rw-rw-   0        0        0       51 2023-02-25 07:41:33.000000 freeplot-0.3.0/freeplot/__init__.py
--rw-rw-rw-   0        0        0    17958 2023-02-17 05:04:04.000000 freeplot-0.3.0/freeplot/base.py
--rw-rw-rw-   0        0        0     3682 2023-02-17 05:04:08.000000 freeplot-0.3.0/freeplot/config.py
--rw-rw-rw-   0        0        0    23929 2023-02-21 12:02:26.000000 freeplot-0.3.0/freeplot/unit.py
--rw-rw-rw-   0        0        0     2303 2023-02-17 05:04:16.000000 freeplot-0.3.0/freeplot/utils.py
--rw-rw-rw-   0        0        0     6226 2022-09-19 12:06:04.000000 freeplot-0.3.0/freeplot/zoo.py
-drwxrwxrwx   0        0        0        0 2023-02-25 07:42:25.687586 freeplot-0.3.0/freeplot.egg-info/
--rw-rw-rw-   0        0        0     7420 2023-02-25 07:42:25.000000 freeplot-0.3.0/freeplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-02-25 07:42:25.000000 freeplot-0.3.0/freeplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-25 07:42:25.000000 freeplot-0.3.0/freeplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-02-25 07:42:25.000000 freeplot-0.3.0/freeplot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-02-25 07:42:25.000000 freeplot-0.3.0/freeplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-25 07:42:25.689582 freeplot-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1101 2023-02-21 12:03:09.000000 freeplot-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 12:09:27.919465 freeplot-0.3.1/
+-rw-rw-rw-   0        0        0     1085 2022-09-19 12:06:04.000000 freeplot-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     7420 2023-04-09 12:09:27.918464 freeplot-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6937 2023-01-01 10:56:12.000000 freeplot-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 12:09:27.894497 freeplot-0.3.1/freeplot/
+-rw-rw-rw-   0        0        0       51 2023-04-09 12:08:20.000000 freeplot-0.3.1/freeplot/__init__.py
+-rw-rw-rw-   0        0        0    17958 2023-02-17 05:04:04.000000 freeplot-0.3.1/freeplot/base.py
+-rw-rw-rw-   0        0        0     3682 2023-02-17 05:04:08.000000 freeplot-0.3.1/freeplot/config.py
+-rw-rw-rw-   0        0        0    23929 2023-02-21 12:02:26.000000 freeplot-0.3.1/freeplot/unit.py
+-rw-rw-rw-   0        0        0     2303 2023-02-17 05:04:16.000000 freeplot-0.3.1/freeplot/utils.py
+-rw-rw-rw-   0        0        0     6226 2022-09-19 12:06:04.000000 freeplot-0.3.1/freeplot/zoo.py
+drwxrwxrwx   0        0        0        0 2023-04-09 12:09:27.918464 freeplot-0.3.1/freeplot.egg-info/
+-rw-rw-rw-   0        0        0     7420 2023-04-09 12:09:27.000000 freeplot-0.3.1/freeplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-04-09 12:09:27.000000 freeplot-0.3.1/freeplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 12:09:27.000000 freeplot-0.3.1/freeplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-04-09 12:09:27.000000 freeplot-0.3.1/freeplot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-09 12:09:27.000000 freeplot-0.3.1/freeplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 12:09:27.919465 freeplot-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1101 2023-04-09 12:08:12.000000 freeplot-0.3.1/setup.py
```

### Comparing `freeplot-0.3.0/LICENSE` & `freeplot-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `freeplot-0.3.0/PKG-INFO` & `freeplot-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeplot
-Version: 0.3.0
+Version: 0.3.1
 Summary: a Python data visualization library based on matplotlib
 Home-page: https://github.com/MTandHJ/freeplot
 Author: MTandHJ
 Author-email: congxueric@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `freeplot-0.3.0/README.md` & `freeplot-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `freeplot-0.3.0/freeplot/base.py` & `freeplot-0.3.1/freeplot/base.py`

 * *Files identical despite different names*

### Comparing `freeplot-0.3.0/freeplot/config.py` & `freeplot-0.3.1/freeplot/config.py`

 * *Files identical despite different names*

### Comparing `freeplot-0.3.0/freeplot/unit.py` & `freeplot-0.3.1/freeplot/unit.py`

 * *Files identical despite different names*

### Comparing `freeplot-0.3.0/freeplot/utils.py` & `freeplot-0.3.1/freeplot/utils.py`

 * *Files identical despite different names*

### Comparing `freeplot-0.3.0/freeplot/zoo.py` & `freeplot-0.3.1/freeplot/zoo.py`

 * *Files identical despite different names*

### Comparing `freeplot-0.3.0/freeplot.egg-info/PKG-INFO` & `freeplot-0.3.1/freeplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeplot
-Version: 0.3.0
+Version: 0.3.1
 Summary: a Python data visualization library based on matplotlib
 Home-page: https://github.com/MTandHJ/freeplot
 Author: MTandHJ
 Author-email: congxueric@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `freeplot-0.3.0/setup.py` & `freeplot-0.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 requires = [
     'numpy>=1.18.1',
     'pandas>=1.0.1',
     'scipy>=1.4.1',
     'scikit-learn>=0.23.2',
     'matplotlib>=3.1.3',
     'seaborn>=0.10.0',
-    'SciencePlots==1.0.5'
+    'SciencePlots==1.0.9'
 ]
 
 def get_property(prop, project):
     result = re.search(r'{}\s*=\s*[\'"]([^\'"]*)[\'"]'.format(prop), open(project + '/__init__.py').read())
     return result.group(1)
 
 setuptools.setup(
```

