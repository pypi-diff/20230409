# Comparing `tmp/hds-stats-0.1.1.tar.gz` & `tmp/hds-stats-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hds-stats-0.1.1.tar", last modified: Sun Apr  9 07:59:40 2023, max compression
+gzip compressed data, was "hds-stats-0.1.2.tar", last modified: Sun Apr  9 20:12:35 2023, max compression
```

## Comparing `hds-stats-0.1.1.tar` & `hds-stats-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-09 07:59:40.276522 hds-stats-0.1.1/
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.1.1/LICENSE
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-04-09 07:59:40.276242 hds-stats-0.1.1/PKG-INFO
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.1.1/README.md
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     7055 2023-04-09 07:18:03.000000 hds-stats-0.1.1/hds_plot.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    17278 2023-04-09 07:52:15.000000 hds-stats-0.1.1/hds_stat.py
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-09 07:59:40.275800 hds-stats-0.1.1/hds_stats.egg-info/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-04-09 07:59:40.000000 hds-stats-0.1.1/hds_stats.egg-info/PKG-INFO
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      229 2023-04-09 07:59:40.000000 hds-stats-0.1.1/hds_stats.egg-info/SOURCES.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-04-09 07:59:40.000000 hds-stats-0.1.1/hds_stats.egg-info/dependency_links.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       63 2023-04-09 07:59:40.000000 hds-stats-0.1.1/hds_stats.egg-info/requires.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       18 2023-04-09 07:59:40.000000 hds-stats-0.1.1/hds_stats.egg-info/top_level.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.1.1/pyproject.toml
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-04-09 07:59:40.276619 hds-stats-0.1.1/setup.cfg
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     1164 2023-04-09 07:59:04.000000 hds-stats-0.1.1/setup.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-09 20:12:35.559670 hds-stats-0.1.2/
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.1.2/LICENSE
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-04-09 20:12:35.559426 hds-stats-0.1.2/PKG-INFO
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.1.2/README.md
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-09 20:12:35.558107 hds-stats-0.1.2/hds_stats.egg-info/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-04-09 20:12:35.000000 hds-stats-0.1.2/hds_stats.egg-info/PKG-INFO
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      245 2023-04-09 20:12:35.000000 hds-stats-0.1.2/hds_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-04-09 20:12:35.000000 hds-stats-0.1.2/hds_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       63 2023-04-09 20:12:35.000000 hds-stats-0.1.2/hds_stats.egg-info/requires.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       14 2023-04-09 20:12:35.000000 hds-stats-0.1.2/hds_stats.egg-info/top_level.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.1.2/pyproject.toml
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-04-09 20:12:35.559758 hds-stats-0.1.2/setup.cfg
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     1171 2023-04-09 20:10:04.000000 hds-stats-0.1.2/setup.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-09 20:12:35.558978 hds-stats-0.1.2/src/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       26 2023-04-09 20:04:38.000000 hds-stats-0.1.2/src/__init__.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     7055 2023-04-09 07:18:03.000000 hds-stats-0.1.2/src/plot.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    17278 2023-04-09 07:52:15.000000 hds-stats-0.1.2/src/stat.py
```

### Comparing `hds-stats-0.1.1/LICENSE` & `hds-stats-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hds-stats-0.1.1/PKG-INFO` & `hds-stats-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.1.1
+Version: 0.1.2
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.1.1/hds_plot.py` & `hds-stats-0.1.2/src/plot.py`

 * *Files identical despite different names*

### Comparing `hds-stats-0.1.1/hds_stat.py` & `hds-stats-0.1.2/src/stat.py`

 * *Files identical despite different names*

### Comparing `hds-stats-0.1.1/hds_stats.egg-info/PKG-INFO` & `hds-stats-0.1.2/hds_stats.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.1.1
+Version: 0.1.2
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.1.1/setup.py` & `hds-stats-0.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 from setuptools import setup
 from setuptools import find_packages
 
-with open(file = "README.md", mode = "r", encoding = "utf-8") as file:
+with open(file = 'README.md', mode = 'r', encoding = 'utf-8') as file:
     long_description = file.read()
 
 setup(
-    name = "hds-stats",
-    
-    version = "0.1.1",
-    
-    author = "HelloDataScience",
-    
-    author_email = "hellodatasciencekorea@gmail.com",
-    
-    description = "Useful functions for Statistics and Machine Learning",
+    name = 'hds-stats',
+    version = '0.1.2',
+    author = 'HelloDataScience',
+    author_email = 'hellodatasciencekorea@gmail.com',
     
+    description = 'Useful functions for Statistics and Machine Learning',
     long_description = long_description,
+    long_description_content_type = 'text/markdown',
     
-    long_description_content_type = "text/markdown",
-    
-    url = "https://github.com/HelloDataScience/hds-stats",
-    
-    license = "MIT",
-    
-    py_modules = ['hds_plot', 'hds_stat'],
-    
+    url = 'https://github.com/HelloDataScience/hds-stats',
     project_urls = {
-        "Bug Tracker": "https://github.com/HelloDataScience/hds-stats/issues",
+        'Bug Tracker': 'https://github.com/HelloDataScience/hds-stats/issues',
     },
-    
+    license = 'MIT',
     classifiers = [
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
+        'Programming Language :: Python :: 3',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
     ],
     
-    python_requires = ">=3.6",
-    
+    python_requires = '>=3.6',
     packages = find_packages(),
-    
-    install_requires = ['numpy', 'pandas', 'scipy', 'seaborn', 'matplotlib', 'statsmodels', 'scikit-learn'],
-    
-    # package_dir = {"": "src"},
+    package_dir = {'hds_stats': 'src'},
+    py_modules = ['plot', 'stat'],
+    install_requires = [
+        'numpy', 
+        'pandas', 
+        'scipy', 
+        'seaborn', 
+        'matplotlib', 
+        'statsmodels', 
+        'scikit-learn'
+    ],
 )
```

