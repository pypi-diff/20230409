# Comparing `tmp/cron-converter-1.0.1.tar.gz` & `tmp/cron-converter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cron-converter-1.0.1.tar", last modified: Wed Jul 20 21:59:10 2022, max compression
+gzip compressed data, was "cron-converter-1.0.2.tar", last modified: Sun Apr  9 21:36:06 2023, max compression
```

## Comparing `cron-converter-1.0.1.tar` & `cron-converter-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2022-07-20 21:59:10.266837 cron-converter-1.0.1/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1177 2022-07-20 21:56:20.000000 cron-converter-1.0.1/LICENSE
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7458 2022-07-20 21:59:10.266837 cron-converter-1.0.1/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     6681 2022-07-16 09:49:15.000000 cron-converter-1.0.1/README.md
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2022-07-20 21:59:10.262838 cron-converter-1.0.1/cron_converter/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       23 2022-07-16 09:49:15.000000 cron-converter-1.0.1/cron_converter/__init__.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     4376 2022-07-16 09:49:15.000000 cron-converter-1.0.1/cron_converter/cron.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2022-07-20 21:59:10.266837 cron-converter-1.0.1/cron_converter/sub_modules/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)    14926 2022-07-20 21:58:44.000000 cron-converter-1.0.1/cron_converter/sub_modules/part.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     8853 2022-07-16 09:49:15.000000 cron-converter-1.0.1/cron_converter/sub_modules/seeker.py
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      483 2022-07-16 09:49:15.000000 cron-converter-1.0.1/cron_converter/sub_modules/units.py
-drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2022-07-20 21:59:10.262838 cron-converter-1.0.1/cron_converter.egg-info/
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     7458 2022-07-20 21:59:10.000000 cron-converter-1.0.1/cron_converter.egg-info/PKG-INFO
--rw-rw-r--   0 andrea    (1000) andrea    (1000)      383 2022-07-20 21:59:10.000000 cron-converter-1.0.1/cron_converter.egg-info/SOURCES.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)        1 2022-07-20 21:59:10.000000 cron-converter-1.0.1/cron_converter.egg-info/dependency_links.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       33 2022-07-20 21:59:10.000000 cron-converter-1.0.1/cron_converter.egg-info/requires.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       42 2022-07-20 21:59:10.000000 cron-converter-1.0.1/cron_converter.egg-info/top_level.txt
--rw-rw-r--   0 andrea    (1000) andrea    (1000)       38 2022-07-20 21:59:10.266837 cron-converter-1.0.1/setup.cfg
--rw-rw-r--   0 andrea    (1000) andrea    (1000)     1074 2022-07-20 21:53:54.000000 cron-converter-1.0.1/setup.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-09 21:36:06.820160 cron-converter-1.0.2/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1177 2023-04-09 20:40:39.000000 cron-converter-1.0.2/LICENSE
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     7438 2023-04-09 21:36:06.820160 cron-converter-1.0.2/PKG-INFO
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     6681 2023-04-09 21:08:32.000000 cron-converter-1.0.2/README.md
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-09 21:36:06.816160 cron-converter-1.0.2/cron_converter/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       23 2023-04-09 20:40:39.000000 cron-converter-1.0.2/cron_converter/__init__.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     4376 2023-04-09 20:40:39.000000 cron-converter-1.0.2/cron_converter/cron.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-09 21:36:06.820160 cron-converter-1.0.2/cron_converter/sub_modules/
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)    14926 2023-04-09 20:40:39.000000 cron-converter-1.0.2/cron_converter/sub_modules/part.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     8994 2023-04-09 21:08:32.000000 cron-converter-1.0.2/cron_converter/sub_modules/seeker.py
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)      483 2023-04-09 20:40:39.000000 cron-converter-1.0.2/cron_converter/sub_modules/units.py
+drwxrwxr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-09 21:36:06.820160 cron-converter-1.0.2/cron_converter.egg-info/
+-rwxr-xr-x   0 andrea    (1000) andrea    (1000)     7438 2023-04-09 21:36:06.000000 cron-converter-1.0.2/cron_converter.egg-info/PKG-INFO
+-rwxr-xr-x   0 andrea    (1000) andrea    (1000)      383 2023-04-09 21:36:06.000000 cron-converter-1.0.2/cron_converter.egg-info/SOURCES.txt
+-rwxr-xr-x   0 andrea    (1000) andrea    (1000)        1 2023-04-09 21:36:06.000000 cron-converter-1.0.2/cron_converter.egg-info/dependency_links.txt
+-rwxr-xr-x   0 andrea    (1000) andrea    (1000)       33 2023-04-09 21:36:06.000000 cron-converter-1.0.2/cron_converter.egg-info/requires.txt
+-rwxr-xr-x   0 andrea    (1000) andrea    (1000)       42 2023-04-09 21:36:06.000000 cron-converter-1.0.2/cron_converter.egg-info/top_level.txt
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)       38 2023-04-09 21:36:06.820160 cron-converter-1.0.2/setup.cfg
+-rw-rw-r--   0 andrea    (1000) andrea    (1000)     1074 2023-04-09 21:27:07.000000 cron-converter-1.0.2/setup.py
```

### Comparing `cron-converter-1.0.1/LICENSE` & `cron-converter-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cron-converter-1.0.1/PKG-INFO` & `cron-converter-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: cron-converter
-Version: 1.0.1
+Version: 1.0.2
 Summary: Cron string parser and scheduler for Python
 Home-page: https://github.com/Sonic0/cron-converter
 Author: Andrea Salvatori
 Author-email: andrea.salvatori92@gmail.com
 License: MIT License
 Keywords: cron
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -88,18 +87,18 @@
 # Prints: '0 1 1 5 */2'
 print(cron_instance.to_string())
 ```
 
 ### Constructor options
 Possible options:
 - output_weekday_names: false (default)
-- output_month_mames: false (default)
+- output_month_names: false (default)
 - output_hashes: false (default)
 
-#### output_weekday_names and output_month_mames
+#### output_weekday_names and output_month_names
 ```python
 cron_instance = Cron(None, {
   'output_weekday_names': True,
   'output_month_names': True
 })
 cron_instance.from_string('*/5 9-17/2 * 1-3 1-5')
 # Prints: '*/5 9-17/2 * JAN-MAR MON-FRI'
@@ -240,9 +239,7 @@
 This repo is part of a projects group, called _Cron-Converter_.
 Its related repositories:
 
 - [local-crontab](https://github.com/Sonic0/local-crontab)
 - [local-crontab-ansible-filter](https://github.com/Sonic0/local-crontab-ansible-filter)
 - [local-crontab-serverless-infrastructure](https://github.com/Sonic0/local-crontab-serverless-infrastructure)
 - [local-crontab-web-converter](https://github.com/Sonic0/local-crontab-web-converter)
-
-
```

### Comparing `cron-converter-1.0.1/README.md` & `cron-converter-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -66,18 +66,18 @@
 # Prints: '0 1 1 5 */2'
 print(cron_instance.to_string())
 ```
 
 ### Constructor options
 Possible options:
 - output_weekday_names: false (default)
-- output_month_mames: false (default)
+- output_month_names: false (default)
 - output_hashes: false (default)
 
-#### output_weekday_names and output_month_mames
+#### output_weekday_names and output_month_names
 ```python
 cron_instance = Cron(None, {
   'output_weekday_names': True,
   'output_month_names': True
 })
 cron_instance.from_string('*/5 9-17/2 * 1-3 1-5')
 # Prints: '*/5 9-17/2 * JAN-MAR MON-FRI'
```

### Comparing `cron-converter-1.0.1/cron_converter/cron.py` & `cron-converter-1.0.2/cron_converter/cron.py`

 * *Files identical despite different names*

### Comparing `cron-converter-1.0.1/cron_converter/sub_modules/part.py` & `cron-converter-1.0.2/cron_converter/sub_modules/part.py`

 * *Files identical despite different names*

### Comparing `cron-converter-1.0.1/cron_converter/sub_modules/seeker.py` & `cron-converter-1.0.2/cron_converter/sub_modules/seeker.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,21 @@
 
 from typing import TYPE_CHECKING, List, Literal
 
 if TYPE_CHECKING:
     from cron import Cron
     from sub_modules.part import Part
 
-weekdays = {'Sun': 0, 'Mon': 1, 'Tue': 2, 'Wed': 3, 'Thu': 4, 'Fri': 5, 'Sat': 6}  # en_US weekdays
 
+"""Converts ISO weekday numbers to cron weekday numbers.
+    ISO weekday numbers are Monday (1) to Sunday (7)
+    Cron weekday numbers are Sunday (0) to Saturday (6).
+"""
+def iso_to_cron_weekday(iso_weekday):
+    return iso_weekday % 7
 
 class Seeker:
     """Create an instance of Seeker. Seeker objects search for execution times of a cron schedule.
     Args:
         cron (object): Cron object
         start_date (datetime): The start date for the schedule iterator, with or without timezone.
         timezone_str (str): The timezone to make an timezone aware datetime as response.
@@ -127,15 +132,15 @@
         operation (Literal['add', 'subtract']): The function to call on date: 'add' or 'subtract'.
     Returns:
         (boolean): Whether the month of the date was changed.
     """
     def _shift_day(self, cron_day_part: 'Part', cron_weekday_part: 'Part', operation: Literal['add', 'subtract']) -> bool:
         current_month = self.date.month
         while self.date.day not in cron_day_part.to_list() or \
-                weekdays.get(self.date.strftime("%a")) not in cron_weekday_part.to_list():
+                iso_to_cron_weekday(self.date.isoweekday()) not in cron_weekday_part.to_list():
             if operation == 'add':
                 self.date = self.date + timedelta(days=+1)
                 self.date = self.date.replace(hour=0, minute=0, second=0)
             else:
                 self.date = self.date + timedelta(days=-1)
                 self.date = self.date.replace(hour=23, minute=59, second=59)
             if current_month != self.date.month:
```

### Comparing `cron-converter-1.0.1/cron_converter.egg-info/PKG-INFO` & `cron-converter-1.0.2/cron_converter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: cron-converter
-Version: 1.0.1
+Version: 1.0.2
 Summary: Cron string parser and scheduler for Python
 Home-page: https://github.com/Sonic0/cron-converter
 Author: Andrea Salvatori
 Author-email: andrea.salvatori92@gmail.com
 License: MIT License
 Keywords: cron
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -88,18 +87,18 @@
 # Prints: '0 1 1 5 */2'
 print(cron_instance.to_string())
 ```
 
 ### Constructor options
 Possible options:
 - output_weekday_names: false (default)
-- output_month_mames: false (default)
+- output_month_names: false (default)
 - output_hashes: false (default)
 
-#### output_weekday_names and output_month_mames
+#### output_weekday_names and output_month_names
 ```python
 cron_instance = Cron(None, {
   'output_weekday_names': True,
   'output_month_names': True
 })
 cron_instance.from_string('*/5 9-17/2 * 1-3 1-5')
 # Prints: '*/5 9-17/2 * JAN-MAR MON-FRI'
@@ -240,9 +239,7 @@
 This repo is part of a projects group, called _Cron-Converter_.
 Its related repositories:
 
 - [local-crontab](https://github.com/Sonic0/local-crontab)
 - [local-crontab-ansible-filter](https://github.com/Sonic0/local-crontab-ansible-filter)
 - [local-crontab-serverless-infrastructure](https://github.com/Sonic0/local-crontab-serverless-infrastructure)
 - [local-crontab-web-converter](https://github.com/Sonic0/local-crontab-web-converter)
-
-
```

### Comparing `cron-converter-1.0.1/setup.py` & `cron-converter-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cron-converter',
-    version='1.0.1',
+    version='1.0.2',
     license='MIT License',
     description='Cron string parser and scheduler for Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Andrea Salvatori',
     author_email='andrea.salvatori92@gmail.com',
     url='https://github.com/Sonic0/cron-converter',
```

