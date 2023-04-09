# Comparing `tmp/Medical_media_sridhar-0.1.2.tar.gz` & `tmp/Medical_media_sridhar-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Medical_media_sridhar-0.1.2.tar", last modified: Sun Apr  9 03:02:57 2023, max compression
+gzip compressed data, was "Medical_media_sridhar-0.1.3.tar", last modified: Sun Apr  9 03:06:21 2023, max compression
```

## Comparing `Medical_media_sridhar-0.1.2.tar` & `Medical_media_sridhar-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-09 03:02:57.647934 Medical_media_sridhar-0.1.2/
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-09 03:02:57.647934 Medical_media_sridhar-0.1.2/Medical_media_sridhar.egg-info/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1432 2023-04-09 03:02:57.000000 Medical_media_sridhar-0.1.2/Medical_media_sridhar.egg-info/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      422 2023-04-09 03:02:57.000000 Medical_media_sridhar-0.1.2/Medical_media_sridhar.egg-info/SOURCES.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-04-09 03:02:57.000000 Medical_media_sridhar-0.1.2/Medical_media_sridhar.egg-info/dependency_links.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       50 2023-04-09 03:02:57.000000 Medical_media_sridhar-0.1.2/Medical_media_sridhar.egg-info/entry_points.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        5 2023-04-09 03:02:57.000000 Medical_media_sridhar-0.1.2/Medical_media_sridhar.egg-info/top_level.txt
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1432 2023-04-09 03:02:57.647934 Medical_media_sridhar-0.1.2/PKG-INFO
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1093 2023-04-09 03:00:11.000000 Medical_media_sridhar-0.1.2/README.md
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-09 03:02:57.647934 Medical_media_sridhar-0.1.2/main/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       22 2023-04-04 14:25:19.000000 Medical_media_sridhar-0.1.2/main/__init__.py
-drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-09 03:02:57.647934 Medical_media_sridhar-0.1.2/main/lib/
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1091 2023-04-02 10:16:52.000000 Medical_media_sridhar-0.1.2/main/lib/Argument.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1180 2023-04-02 11:41:06.000000 Medical_media_sridhar-0.1.2/main/lib/Command_help.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      862 2023-04-04 14:28:05.000000 Medical_media_sridhar-0.1.2/main/lib/Help.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1992 2023-04-04 14:33:04.000000 Medical_media_sridhar-0.1.2/main/lib/Validation_command.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     6664 2023-04-02 11:41:47.000000 Medical_media_sridhar-0.1.2/main/lib/Validation_funtion.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       37 2023-04-01 17:10:53.000000 Medical_media_sridhar-0.1.2/main/lib/__init__.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      890 2023-04-04 14:28:50.000000 Medical_media_sridhar-0.1.2/main/main.py
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-09 03:02:57.647934 Medical_media_sridhar-0.1.2/setup.cfg
--rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      653 2023-04-09 03:02:35.000000 Medical_media_sridhar-0.1.2/setup.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-09 03:06:21.478791 Medical_media_sridhar-0.1.3/
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-09 03:06:21.458791 Medical_media_sridhar-0.1.3/Medical_media_sridhar.egg-info/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1432 2023-04-09 03:06:21.000000 Medical_media_sridhar-0.1.3/Medical_media_sridhar.egg-info/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      422 2023-04-09 03:06:21.000000 Medical_media_sridhar-0.1.3/Medical_media_sridhar.egg-info/SOURCES.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        1 2023-04-09 03:06:21.000000 Medical_media_sridhar-0.1.3/Medical_media_sridhar.egg-info/dependency_links.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       50 2023-04-09 03:06:21.000000 Medical_media_sridhar-0.1.3/Medical_media_sridhar.egg-info/entry_points.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        5 2023-04-09 03:06:21.000000 Medical_media_sridhar-0.1.3/Medical_media_sridhar.egg-info/top_level.txt
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1432 2023-04-09 03:06:21.478791 Medical_media_sridhar-0.1.3/PKG-INFO
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1093 2023-04-09 03:00:11.000000 Medical_media_sridhar-0.1.3/README.md
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-09 03:06:21.474791 Medical_media_sridhar-0.1.3/main/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       22 2023-04-04 14:25:19.000000 Medical_media_sridhar-0.1.3/main/__init__.py
+drwxrwxr-x   0 sridhard.21cse  (1000) sridhard.21cse  (1000)        0 2023-04-09 03:06:21.478791 Medical_media_sridhar-0.1.3/main/lib/
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1091 2023-04-02 10:16:52.000000 Medical_media_sridhar-0.1.3/main/lib/Argument.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1180 2023-04-02 11:41:06.000000 Medical_media_sridhar-0.1.3/main/lib/Command_help.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      862 2023-04-04 14:28:05.000000 Medical_media_sridhar-0.1.3/main/lib/Help.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     1992 2023-04-04 14:33:04.000000 Medical_media_sridhar-0.1.3/main/lib/Validation_command.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)     6664 2023-04-02 11:41:47.000000 Medical_media_sridhar-0.1.3/main/lib/Validation_funtion.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       37 2023-04-01 17:10:53.000000 Medical_media_sridhar-0.1.3/main/lib/__init__.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      890 2023-04-04 14:28:50.000000 Medical_media_sridhar-0.1.3/main/main.py
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)       38 2023-04-09 03:06:21.478791 Medical_media_sridhar-0.1.3/setup.cfg
+-rw-rw-r--   0 sridhard.21cse  (1000) sridhard.21cse  (1000)      653 2023-04-09 03:06:01.000000 Medical_media_sridhar-0.1.3/setup.py
```

### Comparing `Medical_media_sridhar-0.1.2/Medical_media_sridhar.egg-info/PKG-INFO` & `Medical_media_sridhar-0.1.3/Medical_media_sridhar.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Medical-media-sridhar
-Version: 0.1.2
-Summary: Medical_media is like a Health Condition checking tool
+Version: 0.1.3
+Summary: Medical_media gives the status of our Health Condition
 Home-page: https://git.selfmade.ninja/SRIDHARDSCV/bmi_calculater_python_project
 Author: Sridhar
 Author-email: dcsvsridhar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: Medical-media-sridhar Version: 0.1.2 Summary:
-Medical_media is like a Health Condition checking tool Home-page: https://
+Metadata-Version: 2.1 Name: Medical-media-sridhar Version: 0.1.3 Summary:
+Medical_media gives the status of our Health Condition Home-page: https://
 git.selfmade.ninja/SRIDHARDSCV/bmi_calculater_python_project Author: Sridhar
 Author-email: dcsvsridhar@gmail.com License: UNKNOWN Platform: UNKNOWN
 Description-Content-Type: text/markdown ## Uname_sridhar is a wrapper of uname
 Linux Command #### Prerequisites On Ubuntu/Debian: ``` sudo apt install update
 sudo apt install upgrade ``` #### Usage To get the status about BMI,Blood
 Pressure and Heart Beat Rate Health Condition. ``` Medical_media [Option..] ```
 To get the BMI status ``` Medical_media bmi -weight=[Weight] -height=[Height]
```

### Comparing `Medical_media_sridhar-0.1.2/PKG-INFO` & `Medical_media_sridhar-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Medical_media_sridhar
-Version: 0.1.2
-Summary: Medical_media is like a Health Condition checking tool
+Version: 0.1.3
+Summary: Medical_media gives the status of our Health Condition
 Home-page: https://git.selfmade.ninja/SRIDHARDSCV/bmi_calculater_python_project
 Author: Sridhar
 Author-email: dcsvsridhar@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: Medical_media_sridhar Version: 0.1.2 Summary:
-Medical_media is like a Health Condition checking tool Home-page: https://
+Metadata-Version: 2.1 Name: Medical_media_sridhar Version: 0.1.3 Summary:
+Medical_media gives the status of our Health Condition Home-page: https://
 git.selfmade.ninja/SRIDHARDSCV/bmi_calculater_python_project Author: Sridhar
 Author-email: dcsvsridhar@gmail.com License: UNKNOWN Platform: UNKNOWN
 Description-Content-Type: text/markdown ## Uname_sridhar is a wrapper of uname
 Linux Command #### Prerequisites On Ubuntu/Debian: ``` sudo apt install update
 sudo apt install upgrade ``` #### Usage To get the status about BMI,Blood
 Pressure and Heart Beat Rate Health Condition. ``` Medical_media [Option..] ```
 To get the BMI status ``` Medical_media bmi -weight=[Weight] -height=[Height]
```

### Comparing `Medical_media_sridhar-0.1.2/README.md` & `Medical_media_sridhar-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `Medical_media_sridhar-0.1.2/main/lib/Argument.py` & `Medical_media_sridhar-0.1.3/main/lib/Argument.py`

 * *Files identical despite different names*

### Comparing `Medical_media_sridhar-0.1.2/main/lib/Command_help.py` & `Medical_media_sridhar-0.1.3/main/lib/Command_help.py`

 * *Files identical despite different names*

### Comparing `Medical_media_sridhar-0.1.2/main/lib/Help.py` & `Medical_media_sridhar-0.1.3/main/lib/Help.py`

 * *Files identical despite different names*

### Comparing `Medical_media_sridhar-0.1.2/main/lib/Validation_command.py` & `Medical_media_sridhar-0.1.3/main/lib/Validation_command.py`

 * *Files identical despite different names*

### Comparing `Medical_media_sridhar-0.1.2/main/lib/Validation_funtion.py` & `Medical_media_sridhar-0.1.3/main/lib/Validation_funtion.py`

 * *Files identical despite different names*

### Comparing `Medical_media_sridhar-0.1.2/main/main.py` & `Medical_media_sridhar-0.1.3/main/main.py`

 * *Files identical despite different names*

### Comparing `Medical_media_sridhar-0.1.2/setup.py` & `Medical_media_sridhar-0.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import os
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='Medical_media_sridhar',
-    version='0.1.2',
+    version='0.1.3',
     author='Sridhar',
     author_email='dcsvsridhar@gmail.com',
-    description='Medical_media is like a Health Condition checking tool',
+    description='Medical_media gives the status of our Health Condition',
     packages=find_packages(),
     url='https://git.selfmade.ninja/SRIDHARDSCV/bmi_calculater_python_project',
     long_description=long_description,
     long_description_content_type='text/markdown',
     entry_points={
         'console_scripts': [
             'Medical_media=main.main:main',
```

