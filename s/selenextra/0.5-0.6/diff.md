# Comparing `tmp/selenextra-0.5.tar.gz` & `tmp/selenextra-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenextra-0.5.tar", last modified: Sun Apr  9 06:37:08 2023, max compression
+gzip compressed data, was "selenextra-0.6.tar", last modified: Sun Apr  9 06:42:18 2023, max compression
```

## Comparing `selenextra-0.5.tar` & `selenextra-0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 06:37:08.002355 selenextra-0.5/
--rw-rw-rw-   0        0        0    35823 2023-04-09 06:25:50.000000 selenextra-0.5/LICENSE
--rw-rw-rw-   0        0        0      625 2023-04-09 06:37:08.002355 selenextra-0.5/PKG-INFO
--rw-rw-rw-   0        0        0       93 2023-04-09 06:25:50.000000 selenextra-0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 06:37:07.991385 selenextra-0.5/selenextra/
--rw-rw-rw-   0        0        0     4472 2023-04-09 06:36:28.000000 selenextra-0.5/selenextra/__init__.py
--rw-rw-rw-   0        0        0       46 2023-04-09 06:25:50.000000 selenextra-0.5/selenextra/exceptions.py
--rw-rw-rw-   0        0        0     1239 2023-04-09 06:25:50.000000 selenextra-0.5/selenextra/patcher.py
--rw-rw-rw-   0        0        0     5149 2023-04-09 06:25:50.000000 selenextra-0.5/selenextra/typer.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:37:08.001359 selenextra-0.5/selenextra.egg-info/
--rw-rw-rw-   0        0        0      625 2023-04-09 06:37:07.000000 selenextra-0.5/selenextra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-04-09 06:37:07.000000 selenextra-0.5/selenextra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 06:37:07.000000 selenextra-0.5/selenextra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-09 06:37:07.000000 selenextra-0.5/selenextra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-09 06:37:07.000000 selenextra-0.5/selenextra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 06:37:08.003353 selenextra-0.5/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-04-09 06:36:34.000000 selenextra-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:42:18.878799 selenextra-0.6/
+-rw-rw-rw-   0        0        0    35823 2023-04-09 06:25:50.000000 selenextra-0.6/LICENSE
+-rw-rw-rw-   0        0        0      625 2023-04-09 06:42:18.877801 selenextra-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       93 2023-04-09 06:25:50.000000 selenextra-0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 06:42:18.869823 selenextra-0.6/selenextra/
+-rw-rw-rw-   0        0        0     4561 2023-04-09 06:41:48.000000 selenextra-0.6/selenextra/__init__.py
+-rw-rw-rw-   0        0        0       46 2023-04-09 06:25:50.000000 selenextra-0.6/selenextra/exceptions.py
+-rw-rw-rw-   0        0        0     1239 2023-04-09 06:25:50.000000 selenextra-0.6/selenextra/patcher.py
+-rw-rw-rw-   0        0        0     5149 2023-04-09 06:25:50.000000 selenextra-0.6/selenextra/typer.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:42:18.876804 selenextra-0.6/selenextra.egg-info/
+-rw-rw-rw-   0        0        0      625 2023-04-09 06:42:18.000000 selenextra-0.6/selenextra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-04-09 06:42:18.000000 selenextra-0.6/selenextra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 06:42:18.000000 selenextra-0.6/selenextra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-09 06:42:18.000000 selenextra-0.6/selenextra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-09 06:42:18.000000 selenextra-0.6/selenextra.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 06:42:18.878799 selenextra-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      798 2023-04-09 06:41:56.000000 selenextra-0.6/setup.py
```

### Comparing `selenextra-0.5/LICENSE` & `selenextra-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `selenextra-0.5/PKG-INFO` & `selenextra-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 0.5
+Version: 0.6
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `selenextra-0.5/selenextra/__init__.py` & `selenextra-0.6/selenextra/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,18 @@
         raise TimeoutException(
             'Could not find the requested item within the specified timeout')
 
     def remove_executable(self) -> None:
         if self.can_delete_executable:
             os.remove(self.custom_patcher.executable_path)
 
+    def quit(self) -> None:
+        super().quit()
+        self.remove_executable()
+
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
         super().__exit__(exc_type, exc_val, exc_tb)
         self.remove_executable()
 
     def __del__(self) -> None:
         super().__del__()
         self.remove_executable()
```

### Comparing `selenextra-0.5/selenextra/patcher.py` & `selenextra-0.6/selenextra/patcher.py`

 * *Files identical despite different names*

### Comparing `selenextra-0.5/selenextra/typer.py` & `selenextra-0.6/selenextra/typer.py`

 * *Files identical despite different names*

### Comparing `selenextra-0.5/selenextra.egg-info/PKG-INFO` & `selenextra-0.6/selenextra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: selenextra
-Version: 0.5
+Version: 0.6
 Summary: Bringing additional features to Selenium
 Home-page: https://github.com/nguyenvantat1182002/SeleneXtra
 Author: Tat Nguyen Van
 Author-email: nguyenvantat1182002@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `selenextra-0.5/setup.py` & `selenextra-0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='selenextra',
-    version='0.5',
+    version='0.6',
     description='Bringing additional features to Selenium',
     author='Tat Nguyen Van',
     author_email='nguyenvantat1182002@gmail.com',
     url='https://github.com/nguyenvantat1182002/SeleneXtra',
     packages=find_packages(),
     install_requires=[
         'scipy',
```

