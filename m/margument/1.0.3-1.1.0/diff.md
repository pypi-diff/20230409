# Comparing `tmp/margument-1.0.3.tar.gz` & `tmp/margument-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "margument-1.0.3.tar", last modified: Mon Mar 27 19:06:48 2023, max compression
+gzip compressed data, was "margument-1.1.0.tar", last modified: Sun Apr  9 11:48:54 2023, max compression
```

## Comparing `margument-1.0.3.tar` & `margument-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:06:48.123295 margument-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-03-27 19:06:33.000000 margument-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-27 19:06:48.123295 margument-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-27 19:06:33.000000 margument-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:06:48.123295 margument-1.0.3/margument/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 19:06:33.000000 margument-1.0.3/margument/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-03-27 19:06:33.000000 margument-1.0.3/margument/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-03-27 19:06:33.000000 margument-1.0.3/margument/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-27 19:06:33.000000 margument-1.0.3/margument/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-27 19:06:33.000000 margument-1.0.3/margument/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-27 19:06:33.000000 margument-1.0.3/margument/non_repeatable_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-27 19:06:33.000000 margument-1.0.3/margument/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-03-27 19:06:33.000000 margument-1.0.3/margument/reflection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-03-27 19:06:33.000000 margument-1.0.3/margument/repeatable_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-03-27 19:06:33.000000 margument-1.0.3/margument/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-27 19:06:33.000000 margument-1.0.3/margument/settings_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:06:48.123295 margument-1.0.3/margument/version/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 19:06:33.000000 margument-1.0.3/margument/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-27 19:06:33.000000 margument-1.0.3/margument/version/progsettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-27 19:06:33.000000 margument-1.0.3/margument/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:06:48.123295 margument-1.0.3/margument.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-27 19:06:48.000000 margument-1.0.3/margument.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-03-27 19:06:48.000000 margument-1.0.3/margument.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 19:06:48.000000 margument-1.0.3/margument.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-27 19:06:48.000000 margument-1.0.3/margument.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-27 19:06:48.000000 margument-1.0.3/margument.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 19:06:48.123295 margument-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-03-27 19:06:33.000000 margument-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:48:54.397095 margument-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-09 11:48:39.000000 margument-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-09 11:48:54.397095 margument-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-04-09 11:48:39.000000 margument-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:48:54.397095 margument-1.1.0/margument/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 11:48:39.000000 margument-1.1.0/margument/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-09 11:48:39.000000 margument-1.1.0/margument/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-09 11:48:39.000000 margument-1.1.0/margument/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-09 11:48:39.000000 margument-1.1.0/margument/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-09 11:48:39.000000 margument-1.1.0/margument/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-09 11:48:39.000000 margument-1.1.0/margument/non_repeatable_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-09 11:48:39.000000 margument-1.1.0/margument/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-09 11:48:39.000000 margument-1.1.0/margument/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-09 11:48:39.000000 margument-1.1.0/margument/repeatable_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-09 11:48:39.000000 margument-1.1.0/margument/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-09 11:48:39.000000 margument-1.1.0/margument/settings_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:48:54.397095 margument-1.1.0/margument/version/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 11:48:39.000000 margument-1.1.0/margument/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-09 11:48:39.000000 margument-1.1.0/margument/version/progsettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-09 11:48:39.000000 margument-1.1.0/margument/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:48:54.397095 margument-1.1.0/margument.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-09 11:48:54.000000 margument-1.1.0/margument.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-09 11:48:54.000000 margument-1.1.0/margument.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 11:48:54.000000 margument-1.1.0/margument.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-09 11:48:54.000000 margument-1.1.0/margument.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 11:48:54.000000 margument-1.1.0/margument.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 11:48:54.397095 margument-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-09 11:48:39.000000 margument-1.1.0/setup.py
```

### Comparing `margument-1.0.3/LICENSE` & `margument-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `margument-1.0.3/margument/file.py` & `margument-1.1.0/margument/file.py`

 * *Files identical despite different names*

### Comparing `margument-1.0.3/margument/non_repeatable_settings.py` & `margument-1.1.0/margument/non_repeatable_settings.py`

 * *Files identical despite different names*

### Comparing `margument-1.0.3/margument/repeatable_settings.py` & `margument-1.1.0/margument/repeatable_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,31 @@
+from margument.log import throw
 from margument.options import Options
 from margument.reflection import convert_to_dict
 from margument.settings import Settings
 from margument.yaml import write_yaml
 
 
 class RepeatableSettings(Settings):
     __main_arg = {'name': '', 'value': ''}
 
     def __init__(self, path, program_arguments=None, options=Options()):
         super().__init__(path, program_arguments, options)
 
     def __process_main_arg(self):
+        main_arg_exists = False
         for arg in self.program_arguments.to_list():
             if arg.is_main:
+                main_arg_exists = True
                 self.__main_arg['name'] = arg.name
                 break
 
+        if not main_arg_exists:
+            throw("No main argument defined.")
+
         if self.__main_arg['name'] in self.user_arguments:
             self.__main_arg['value'] = getattr(self.user_arguments, self.__main_arg['name'])
 
     def set(self):
         self.__process_main_arg()
 
         user_arguments_dict = convert_to_dict(self.user_arguments)
```

### Comparing `margument-1.0.3/margument/settings.py` & `margument-1.1.0/margument/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os.path
 
 from margument.options import Options
 from margument.file import File
 from margument.yaml import read_yaml
 from margument.log import show
-from margument.reflection import convert_to_dict
+
 
 class Settings:
 
     def __init__(self, path, program_arguments=None, options=Options()):
         self.file = File(path)
         self.program_arguments = program_arguments
         self.settings_from_file = {}
```

### Comparing `margument-1.0.3/margument/settings_processor.py` & `margument-1.1.0/margument/settings_processor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 from margument.log import throw
 
 
 class SettingsProcessor:
     def __init__(self, settings, args_parser):
+        """
+        :param settings: A list of settings to be processed.
+        :param args_parser: the instance from argsparse.ArgumentParser() previously created
+        """
         self.settings = settings
         self.args_parser = args_parser
 
     def run(self):
-
+        """
+        This method will iterate through all the given settings and will process each one according to their specifications.
+        :return: A dictionary of all settings given each containing a list of all parsed configurations from the user and/or the external file .
+        """
         for setting in self.settings:
             setting.program_arguments.add_arguments(self.args_parser)
 
         user_arguments = None
         try:
             user_arguments = self.args_parser.parse_args()
         except AssertionError:
```

### Comparing `margument-1.0.3/margument.egg-info/SOURCES.txt` & `margument-1.1.0/margument.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `margument-1.0.3/setup.py` & `margument-1.1.0/setup.py`

 * *Files identical despite different names*

