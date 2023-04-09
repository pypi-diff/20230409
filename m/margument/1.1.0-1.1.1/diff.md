# Comparing `tmp/margument-1.1.0.tar.gz` & `tmp/margument-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "margument-1.1.0.tar", last modified: Sun Apr  9 11:48:54 2023, max compression
+gzip compressed data, was "margument-1.1.1.tar", last modified: Sun Apr  9 11:58:01 2023, max compression
```

## Comparing `margument-1.1.0.tar` & `margument-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:48:54.397095 margument-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-09 11:48:39.000000 margument-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-09 11:48:54.397095 margument-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-04-09 11:48:39.000000 margument-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:48:54.397095 margument-1.1.0/margument/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 11:48:39.000000 margument-1.1.0/margument/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-09 11:48:39.000000 margument-1.1.0/margument/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-09 11:48:39.000000 margument-1.1.0/margument/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-09 11:48:39.000000 margument-1.1.0/margument/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-09 11:48:39.000000 margument-1.1.0/margument/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-09 11:48:39.000000 margument-1.1.0/margument/non_repeatable_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-09 11:48:39.000000 margument-1.1.0/margument/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-09 11:48:39.000000 margument-1.1.0/margument/reflection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-09 11:48:39.000000 margument-1.1.0/margument/repeatable_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-09 11:48:39.000000 margument-1.1.0/margument/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-09 11:48:39.000000 margument-1.1.0/margument/settings_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:48:54.397095 margument-1.1.0/margument/version/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 11:48:39.000000 margument-1.1.0/margument/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-09 11:48:39.000000 margument-1.1.0/margument/version/progsettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-09 11:48:39.000000 margument-1.1.0/margument/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:48:54.397095 margument-1.1.0/margument.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-09 11:48:54.000000 margument-1.1.0/margument.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-09 11:48:54.000000 margument-1.1.0/margument.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 11:48:54.000000 margument-1.1.0/margument.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-09 11:48:54.000000 margument-1.1.0/margument.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 11:48:54.000000 margument-1.1.0/margument.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 11:48:54.397095 margument-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-09 11:48:39.000000 margument-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:58:01.110774 margument-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-09 11:57:46.000000 margument-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-09 11:58:01.110774 margument-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-04-09 11:57:46.000000 margument-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:58:01.110774 margument-1.1.1/margument/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 11:57:46.000000 margument-1.1.1/margument/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-09 11:57:46.000000 margument-1.1.1/margument/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-09 11:57:46.000000 margument-1.1.1/margument/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-09 11:57:46.000000 margument-1.1.1/margument/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-09 11:57:46.000000 margument-1.1.1/margument/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-09 11:57:46.000000 margument-1.1.1/margument/non_repeatable_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-09 11:57:46.000000 margument-1.1.1/margument/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-09 11:57:46.000000 margument-1.1.1/margument/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-09 11:57:46.000000 margument-1.1.1/margument/repeatable_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-09 11:57:46.000000 margument-1.1.1/margument/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-09 11:57:46.000000 margument-1.1.1/margument/settings_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:58:01.110774 margument-1.1.1/margument/version/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 11:57:46.000000 margument-1.1.1/margument/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-09 11:57:46.000000 margument-1.1.1/margument/version/progsettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-09 11:57:46.000000 margument-1.1.1/margument/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 11:58:01.110774 margument-1.1.1/margument.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-09 11:58:01.000000 margument-1.1.1/margument.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-09 11:58:01.000000 margument-1.1.1/margument.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 11:58:01.000000 margument-1.1.1/margument.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-09 11:58:01.000000 margument-1.1.1/margument.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-09 11:58:01.000000 margument-1.1.1/margument.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 11:58:01.114774 margument-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-09 11:57:46.000000 margument-1.1.1/setup.py
```

### Comparing `margument-1.1.0/LICENSE` & `margument-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `margument-1.1.0/PKG-INFO` & `margument-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: margument
-Version: 1.1.0
+Version: 1.1.1
 Summary: python library to manage configurations from program arguments including doing commands and saving configurations in a yaml file.
 Home-page: https://github.com/zaytiri/settings-manager
 Author: zaytiri
 Project-URL: GitHub, https://github.com/zaytiri/settings-manager
 Project-URL: Changelog, https://github.com/zaytiri/settings-manager/blob/main/CHANGELOG.md
 Keywords: manager,configurations,settings,arguments,argparse,yaml,save
 Classifier: Environment :: Console
```

### Comparing `margument-1.1.0/README.md` & `margument-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `margument-1.1.0/margument/argument.py` & `margument-1.1.1/margument/argument.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,29 +7,28 @@
                  help_message='',
                  metavar='',
                  default='None',
                  to_save=False,
                  is_main=False,
                  command=None,
                  command_args=None,
-                 choices=None,
+                 choices=None):
         """
         :param name: the name of the argument, ex: alias (must be the same as full_name)
         :param abbreviation_name: the abbreviation name for the argument, ex: -a (see argsparse documentation https://docs.python.org/3/library/argparse.html#name-or-flags)
         :param full_name: the full name of the argument, ex: --alias (must be the same as name) (see argsparse documentation https://docs.python.org/3/library/argparse.html#name-or-flags)
         :param value: the value of the argument provided posteriorly by the user.
         :param help_message: the help message for the argument (see argsparse documentation https://docs.python.org/3/library/argparse.html#help)
         :param metavar: the metavar for the argument (see argsparse documentation https://docs.python.org/3/library/argparse.html#metavar)
         :param default: the default value for the argument
         :param to_save: a boolean defining if this argument should be saved in the yaml file.
         :param is_main: a boolean defining if this argument is a main argument. There must be 1 if to use on RepeatableSettings class
         :param command: the method that this argument should call when it's present on the arguments parsed and provided by the user.
         :param command_args: all the arguments the previous method needs to have. If more than one argument, please wrap them in (), ex: (arg1, arg2)
-        :param choices: a list of choices required by the argument (see argsparse documentation
-        https://docs.python.org/3/library/argparse.html#choices)
+        :param choices: a list of choices required by the argument (see argsparse documentation https://docs.python.org/3/library/argparse.html#choices)
         """
         self.name = name
         self.abbreviation_name = abbreviation_name
         self.full_name = full_name
         self.value = value
         self.help_message = help_message
         self.metavar = metavar
@@ -50,15 +49,15 @@
             help_message=argument.help_message,
             metavar=argument.metavar,
             default=argument.default,
             to_save=argument.to_save,
             is_main=argument.is_main,
             command=argument.command,
             command_args=argument.command_args,
-            choices=argument.choices,
+            choices=argument.choices)
 
     def set_value(self, value):
         self.value = value
 
     def set_command(self, command):
         self.command = command
```

### Comparing `margument-1.1.0/margument/arguments.py` & `margument-1.1.1/margument/arguments.py`

 * *Files identical despite different names*

### Comparing `margument-1.1.0/margument/file.py` & `margument-1.1.1/margument/file.py`

 * *Files identical despite different names*

### Comparing `margument-1.1.0/margument/non_repeatable_settings.py` & `margument-1.1.1/margument/non_repeatable_settings.py`

 * *Files identical despite different names*

### Comparing `margument-1.1.0/margument/options.py` & `margument-1.1.1/margument/options.py`

 * *Files identical despite different names*

### Comparing `margument-1.1.0/margument/repeatable_settings.py` & `margument-1.1.1/margument/repeatable_settings.py`

 * *Files identical despite different names*

### Comparing `margument-1.1.0/margument/settings.py` & `margument-1.1.1/margument/settings.py`

 * *Files identical despite different names*

### Comparing `margument-1.1.0/margument/settings_processor.py` & `margument-1.1.1/margument/settings_processor.py`

 * *Files identical despite different names*

### Comparing `margument-1.1.0/margument.egg-info/PKG-INFO` & `margument-1.1.1/margument.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: margument
-Version: 1.1.0
+Version: 1.1.1
 Summary: python library to manage configurations from program arguments including doing commands and saving configurations in a yaml file.
 Home-page: https://github.com/zaytiri/settings-manager
 Author: zaytiri
 Project-URL: GitHub, https://github.com/zaytiri/settings-manager
 Project-URL: Changelog, https://github.com/zaytiri/settings-manager/blob/main/CHANGELOG.md
 Keywords: manager,configurations,settings,arguments,argparse,yaml,save
 Classifier: Environment :: Console
```

### Comparing `margument-1.1.0/margument.egg-info/SOURCES.txt` & `margument-1.1.1/margument.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `margument-1.1.0/setup.py` & `margument-1.1.1/setup.py`

 * *Files identical despite different names*

