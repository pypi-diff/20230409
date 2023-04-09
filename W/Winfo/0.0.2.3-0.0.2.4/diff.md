# Comparing `tmp/Winfo-0.0.2.3.tar.gz` & `tmp/Winfo-0.0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Winfo-0.0.2.3.tar", last modified: Sat Apr  8 17:59:16 2023, max compression
+gzip compressed data, was "Winfo-0.0.2.4.tar", last modified: Sun Apr  9 17:08:28 2023, max compression
```

## Comparing `Winfo-0.0.2.3.tar` & `Winfo-0.0.2.4.tar`

### file list

```diff
@@ -1,13 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 17:59:16.832026 Winfo-0.0.2.3/
--rw-rw-rw-   0        0        0     1156 2023-04-07 10:35:15.000000 Winfo-0.0.2.3/LICENSE
--rw-rw-rw-   0        0        0     5360 2023-04-08 17:59:16.831026 Winfo-0.0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     4912 2023-04-08 17:58:30.000000 Winfo-0.0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 17:59:16.811397 Winfo-0.0.2.3/Winfo/
--rw-rw-rw-   0        0        0     8482 2023-04-08 16:41:27.000000 Winfo-0.0.2.3/Winfo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-08 17:59:16.830030 Winfo-0.0.2.3/Winfo.egg-info/
--rw-rw-rw-   0        0        0     5360 2023-04-08 17:59:16.000000 Winfo-0.0.2.3/Winfo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2023-04-08 17:59:16.000000 Winfo-0.0.2.3/Winfo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 17:59:16.000000 Winfo-0.0.2.3/Winfo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-08 17:59:16.000000 Winfo-0.0.2.3/Winfo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 17:59:16.832026 Winfo-0.0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      677 2023-04-08 16:24:31.000000 Winfo-0.0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 17:08:28.142839 Winfo-0.0.2.4/
+-rw-rw-rw-   0        0        0     1156 2023-04-07 10:35:15.000000 Winfo-0.0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     5360 2023-04-09 17:08:28.141837 Winfo-0.0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4912 2023-04-08 21:41:44.000000 Winfo-0.0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 17:08:28.110823 Winfo-0.0.2.4/Winfo/
+-rw-rw-rw-   0        0        0     2647 2023-04-09 17:02:04.000000 Winfo-0.0.2.4/Winfo/__init__.py
+-rw-rw-rw-   0        0        0     1300 2023-04-09 16:56:37.000000 Winfo-0.0.2.4/Winfo/cpu.py
+-rw-rw-rw-   0        0        0      967 2023-04-09 16:58:02.000000 Winfo-0.0.2.4/Winfo/disk.py
+-rw-rw-rw-   0        0        0      680 2023-04-09 16:58:55.000000 Winfo-0.0.2.4/Winfo/ethernet.py
+-rw-rw-rw-   0        0        0      522 2023-04-09 16:57:11.000000 Winfo-0.0.2.4/Winfo/gpu.py
+-rw-rw-rw-   0        0        0      961 2023-04-09 16:57:42.000000 Winfo-0.0.2.4/Winfo/memory.py
+-rw-rw-rw-   0        0        0      479 2023-04-09 16:59:58.000000 Winfo-0.0.2.4/Winfo/motherboard.py
+-rw-rw-rw-   0        0        0     1110 2023-04-09 16:55:44.000000 Winfo-0.0.2.4/Winfo/software.py
+drwxrwxrwx   0        0        0        0 2023-04-09 17:08:28.140839 Winfo-0.0.2.4/Winfo.egg-info/
+-rw-rw-rw-   0        0        0     5360 2023-04-09 17:08:27.000000 Winfo-0.0.2.4/Winfo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-04-09 17:08:28.000000 Winfo-0.0.2.4/Winfo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 17:08:27.000000 Winfo-0.0.2.4/Winfo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-09 17:08:27.000000 Winfo-0.0.2.4/Winfo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 17:08:28.142839 Winfo-0.0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      677 2023-04-08 18:00:26.000000 Winfo-0.0.2.4/setup.py
```

### Comparing `Winfo-0.0.2.3/LICENSE` & `Winfo-0.0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.2.3/PKG-INFO` & `Winfo-0.0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Winfo
-Version: 0.0.2.3
+Version: 0.0.2.4
 Summary: Get information about your windows system
 Author: BLUEAMETHYST Studios
 Keywords: python,windows,util,information,system
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `Winfo-0.0.2.3/README.md` & `Winfo-0.0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `Winfo-0.0.2.3/Winfo.egg-info/PKG-INFO` & `Winfo-0.0.2.4/Winfo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Winfo
-Version: 0.0.2.3
+Version: 0.0.2.4
 Summary: Get information about your windows system
 Author: BLUEAMETHYST Studios
 Keywords: python,windows,util,information,system
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `Winfo-0.0.2.3/setup.py` & `Winfo-0.0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     readme = f.read()
     f.close()
     
 setup(
     name="Winfo",
-    version="0.0.2.3",
+    version="0.0.2.4",
     author="BLUEAMETHYST Studios",
     description="Get information about your windows system",
     long_description_content_type="text/markdown",
     long_description=readme,
     packages=find_packages(),
     keywords=['python', 'windows', 'util', 'information', 'system'],
     classifiers=[
```

