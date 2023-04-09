# Comparing `tmp/random-ip-generator-0.1.2.tar.gz` & `tmp/random-ip-generator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "random-ip-generator-0.1.2.tar", last modified: Sun Mar 26 05:37:50 2023, max compression
+gzip compressed data, was "random-ip-generator-0.1.3.tar", last modified: Sun Apr  9 17:34:12 2023, max compression
```

## Comparing `random-ip-generator-0.1.2.tar` & `random-ip-generator-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 edde746    (501) staff       (20)        0 2023-03-26 05:37:50.217603 random-ip-generator-0.1.2/
--rw-r--r--   0 edde746    (501) staff       (20)    35149 2023-03-26 05:35:49.000000 random-ip-generator-0.1.2/LICENSE
--rw-r--r--   0 edde746    (501) staff       (20)     1265 2023-03-26 05:37:50.217350 random-ip-generator-0.1.2/PKG-INFO
--rw-r--r--   0 edde746    (501) staff       (20)      952 2023-03-26 05:35:49.000000 random-ip-generator-0.1.2/README.md
-drwxr-xr-x   0 edde746    (501) staff       (20)        0 2023-03-26 05:37:50.215512 random-ip-generator-0.1.2/random_ip_generator/
--rw-r--r--   0 edde746    (501) staff       (20)       40 2023-03-26 05:15:33.000000 random-ip-generator-0.1.2/random_ip_generator/__init__.py
--rw-r--r--   0 edde746    (501) staff       (20)      770 2023-03-26 05:13:51.000000 random-ip-generator-0.1.2/random_ip_generator/main.py
-drwxr-xr-x   0 edde746    (501) staff       (20)        0 2023-03-26 05:37:50.217028 random-ip-generator-0.1.2/random_ip_generator.egg-info/
--rw-r--r--   0 edde746    (501) staff       (20)     1265 2023-03-26 05:37:50.000000 random-ip-generator-0.1.2/random_ip_generator.egg-info/PKG-INFO
--rw-r--r--   0 edde746    (501) staff       (20)      346 2023-03-26 05:37:50.000000 random-ip-generator-0.1.2/random_ip_generator.egg-info/SOURCES.txt
--rw-r--r--   0 edde746    (501) staff       (20)        1 2023-03-26 05:37:50.000000 random-ip-generator-0.1.2/random_ip_generator.egg-info/dependency_links.txt
--rw-r--r--   0 edde746    (501) staff       (20)       71 2023-03-26 05:37:50.000000 random-ip-generator-0.1.2/random_ip_generator.egg-info/entry_points.txt
--rw-r--r--   0 edde746    (501) staff       (20)       10 2023-03-26 05:37:50.000000 random-ip-generator-0.1.2/random_ip_generator.egg-info/requires.txt
--rw-r--r--   0 edde746    (501) staff       (20)       20 2023-03-26 05:37:50.000000 random-ip-generator-0.1.2/random_ip_generator.egg-info/top_level.txt
--rw-r--r--   0 edde746    (501) staff       (20)       38 2023-03-26 05:37:50.217669 random-ip-generator-0.1.2/setup.cfg
--rw-r--r--   0 edde746    (501) staff       (20)      662 2023-03-26 05:36:24.000000 random-ip-generator-0.1.2/setup.py
+drwxr-xr-x   0 edde746    (501) staff       (20)        0 2023-04-09 17:34:12.033083 random-ip-generator-0.1.3/
+-rw-r--r--   0 edde746    (501) staff       (20)    35149 2023-03-26 05:35:49.000000 random-ip-generator-0.1.3/LICENSE
+-rw-r--r--   0 edde746    (501) staff       (20)       52 2023-04-09 17:30:30.000000 random-ip-generator-0.1.3/MANIFEST.in
+-rw-r--r--   0 edde746    (501) staff       (20)     1265 2023-04-09 17:34:12.032783 random-ip-generator-0.1.3/PKG-INFO
+-rw-r--r--   0 edde746    (501) staff       (20)      952 2023-03-26 05:38:43.000000 random-ip-generator-0.1.3/README.md
+drwxr-xr-x   0 edde746    (501) staff       (20)        0 2023-04-09 17:34:12.031494 random-ip-generator-0.1.3/random_ip_generator/
+-rwxr-xr-x   0 edde746    (501) staff       (20) 10797986 2023-03-26 04:48:53.000000 random-ip-generator-0.1.3/random_ip_generator/IP2LOCATION-LITE-DB1.CSV
+-rw-r--r--   0 edde746    (501) staff       (20)       40 2023-03-26 05:15:33.000000 random-ip-generator-0.1.3/random_ip_generator/__init__.py
+-rw-r--r--   0 edde746    (501) staff       (20)      848 2023-04-09 17:32:58.000000 random-ip-generator-0.1.3/random_ip_generator/main.py
+drwxr-xr-x   0 edde746    (501) staff       (20)        0 2023-04-09 17:34:12.032579 random-ip-generator-0.1.3/random_ip_generator.egg-info/
+-rw-r--r--   0 edde746    (501) staff       (20)     1265 2023-04-09 17:34:11.000000 random-ip-generator-0.1.3/random_ip_generator.egg-info/PKG-INFO
+-rw-r--r--   0 edde746    (501) staff       (20)      403 2023-04-09 17:34:11.000000 random-ip-generator-0.1.3/random_ip_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 edde746    (501) staff       (20)        1 2023-04-09 17:34:11.000000 random-ip-generator-0.1.3/random_ip_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 edde746    (501) staff       (20)       71 2023-04-09 17:34:11.000000 random-ip-generator-0.1.3/random_ip_generator.egg-info/entry_points.txt
+-rw-r--r--   0 edde746    (501) staff       (20)       10 2023-04-09 17:34:11.000000 random-ip-generator-0.1.3/random_ip_generator.egg-info/requires.txt
+-rw-r--r--   0 edde746    (501) staff       (20)       20 2023-04-09 17:34:11.000000 random-ip-generator-0.1.3/random_ip_generator.egg-info/top_level.txt
+-rw-r--r--   0 edde746    (501) staff       (20)       38 2023-04-09 17:34:12.033136 random-ip-generator-0.1.3/setup.cfg
+-rw-r--r--   0 edde746    (501) staff       (20)      693 2023-04-09 17:31:20.000000 random-ip-generator-0.1.3/setup.py
```

### Comparing `random-ip-generator-0.1.2/LICENSE` & `random-ip-generator-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `random-ip-generator-0.1.2/PKG-INFO` & `random-ip-generator-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: random-ip-generator
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to generate random IP addresses for a given country code
 Home-page: https://github.com/edde746/random-ip-generator
 Author: edde746
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `random-ip-generator-0.1.2/README.md` & `random-ip-generator-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `random-ip-generator-0.1.2/random_ip_generator.egg-info/PKG-INFO` & `random-ip-generator-0.1.3/random_ip_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: random-ip-generator
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to generate random IP addresses for a given country code
 Home-page: https://github.com/edde746/random-ip-generator
 Author: edde746
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `random-ip-generator-0.1.2/setup.py` & `random-ip-generator-0.1.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="random-ip-generator",
-    version="0.1.2",
+    version="0.1.3",
     author="edde746",
     description="A package to generate random IP addresses for a given country code",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/edde746/random-ip-generator",
     packages=find_packages(),
+    include_package_data=True,
     install_requires=[
         "ipaddress",
     ],
     entry_points={
         "console_scripts": [
             "random-ip-generator=random_ip_generator.main:main",
         ],
```

