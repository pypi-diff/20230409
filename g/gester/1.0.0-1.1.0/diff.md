# Comparing `tmp/gester-1.0.0.tar.gz` & `tmp/gester-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E:\dev\projects\gest\dist\.tmp-3dfjw8d0\gester-1.0.0.tar", last modified: Sun Apr  9 08:44:54 2023, max compression
+gzip compressed data, was "E:\dev\projects\gest\dist\.tmp-_fotl_yn\gester-1.1.0.tar", last modified: Sun Apr  9 09:41:33 2023, max compression
```

## Comparing `gester-1.0.0.tar` & `gester-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 08:44:54.930287 gester-1.0.0/
--rw-rw-rw-   0        0        0     1361 2023-04-08 06:55:38.000000 gester-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2808 2023-04-09 08:44:54.930287 gester-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       57 2023-04-09 07:55:46.000000 gester-1.0.0/README.md
--rw-rw-rw-   0        0        0     1206 2023-04-09 08:42:30.000000 gester-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-09 08:44:54.945887 gester-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-09 08:44:54.852287 gester-1.0.0/src/
--rw-rw-rw-   0        0        0       23 2023-04-09 07:22:30.000000 gester-1.0.0/src/__init__.py
--rw-rw-rw-   0        0        0     6348 2023-04-09 07:21:22.000000 gester-1.0.0/src/gest.py
-drwxrwxrwx   0        0        0        0 2023-04-09 08:44:54.914687 gester-1.0.0/src/gester.egg-info/
--rw-rw-rw-   0        0        0     2808 2023-04-09 08:44:54.000000 gester-1.0.0/src/gester.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-04-09 08:44:54.000000 gester-1.0.0/src/gester.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 08:44:54.000000 gester-1.0.0/src/gester.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-09 08:44:54.000000 gester-1.0.0/src/gester.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-04-09 08:44:54.000000 gester-1.0.0/src/gester.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 09:41:33.602823 gester-1.1.0/
+-rw-rw-rw-   0        0        0     1361 2023-04-08 06:55:38.000000 gester-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2808 2023-04-09 09:41:33.602823 gester-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       57 2023-04-09 07:55:46.000000 gester-1.1.0/README.md
+-rw-rw-rw-   0        0        0     1211 2023-04-09 09:06:50.000000 gester-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-09 09:41:33.602823 gester-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-09 09:41:33.509223 gester-1.1.0/src/
+-rw-rw-rw-   0        0        0       23 2023-04-09 07:22:30.000000 gester-1.1.0/src/__init__.py
+-rw-rw-rw-   0        0        0     6407 2023-04-09 09:31:16.000000 gester-1.1.0/src/gest.py
+drwxrwxrwx   0        0        0        0 2023-04-09 09:41:33.571623 gester-1.1.0/src/gester.egg-info/
+-rw-rw-rw-   0        0        0     2808 2023-04-09 09:41:33.000000 gester-1.1.0/src/gester.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-04-09 09:41:33.000000 gester-1.1.0/src/gester.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 09:41:33.000000 gester-1.1.0/src/gester.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-09 09:41:33.000000 gester-1.1.0/src/gester.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-04-09 09:41:33.000000 gester-1.1.0/src/gester.egg-info/top_level.txt
```

### Comparing `gester-1.0.0/LICENSE` & `gester-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gester-1.0.0/PKG-INFO` & `gester-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gester
-Version: 1.0.0
+Version: 1.1.0
 Summary: A game engine for console based text game
 Author-email: etcetra7n <greeknio@gmail.com>
 License: Boost Software License - Version 1.0 - August 17th, 2003
         
         Permission is hereby granted, free of charge, to any person or organization
         obtaining a copy of the software and accompanying documentation covered by
         this license (the "Software") to use, reproduce, display, distribute,
```

### Comparing `gester-1.0.0/pyproject.toml` & `gester-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gester"
-version = "1.0.0"
+version = "1.1.0"
 description = "A game engine for console based text game"
 readme = "README.md"
 keywords = ["games", "game development", "game engine", "console"]
 license = {file = "LICENSE"}
 authors = [
     {name = "etcetra7n", email = "greeknio@gmail.com"}
 ]
@@ -24,12 +24,12 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)",
     "Operating System :: OS Independent",
 ]
 
 [project.scripts]
-gest = "gest"
+gest = "gest:main"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/etcetra7n/gest/issues"
 repository = "https://github.com/etcetra7n/gest"
```

### Comparing `gester-1.0.0/src/gest.py` & `gester-1.1.0/src/gest.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,25 +3,23 @@
 from os.path import isfile, abspath
 import re
 #from keyboard import is_pressed
 import pickle
 import colorama
 from colorama import Fore
 
-in_game_vars = {}
-gsav_file = None
-
 def init_in_game_vars(gest_file):
     in_game_vars['gest_file'] = abspath(gest_file)
     in_game_vars['line_index'] = 0
     gsav_file = re.search(r'^(.+?)\.gest$', abspath(gest_file))
     in_game_vars['gsav_file'] = gsav_file.group(1) + '.gsav'
     return
 
 def save():
+    gsav_file.seek(0)
     pickle.dump(in_game_vars, gsav_file)
 
 def trim(str):
     begin = 0
     end = len(str)
     for i, c in enumerate(str):
         if(c != ' '):
@@ -86,33 +84,33 @@
                 if(command == 'input'):
                     '''
                     INPUT COMMAND
                     Syntax:
                         [input: var] some text
                     for example:
                         [input: name] Enter your name:
-                        
+
                     The name will be stored in the varible 'name' which
                     can be accessed by `{name}`
                     '''
                     txtout(prompt + ' ')
                     in_game_vars[var] = input()
                     line_index += 1
                     continue
-                
+
                 elif(command == 'yes_or_no'):
                     '''
                     YES_OR_NO COMMAND
                     Syntax:
                         [yes_or_no: var] some question
                     for example:
                         [yes_or_no: p] Are you ready to proceed
                     while playing the above example yould be displayed
                     as:
-                        Are you ready to proceed (y/n): 
+                        Are you ready to proceed (y/n):
                     '''
                     txtout(prompt + ' (y/n): ')
                     inp = input()
                     if inp == 'y':
                         in_game_vars[var] = 'yes'
                     elif inp == 'n':
                         in_game_vars[var] = 'no'
@@ -165,31 +163,38 @@
             if re.match(r'[ ]*\[[ ]*abort[ ]*\]', line):
                 break
 
             txtout(trim(line))
             line_index += 1
     save()
 
-if __name__=='__main__':
+def main():
+    global in_game_vars
+    global gsav_file
+    in_game_vars = {}
+    gsav_file = None
     if len(argv)<2:
         print(Fore.RED + "\nError:" + Fore.RESET + " Argument not provided")
         exit()
     file = argv[1]
     if not(isfile(file)):
         print(Fore.RED + "\nError:" + Fore.RESET + " This file cannot be located")
     try:
         if(file.endswith('.gest')):
-            init_in_game_vars(argv[1])
+            init_in_game_vars(file)
             gsav_file = open(in_game_vars['gsav_file'], 'wb')
             play()
             gsav_file.close()
         elif(file.endswith('.gsav')):
             with open(file, 'rb') as sf:
                 in_game_vars = pickle.load(sf)
             gsav_file = open(in_game_vars['gsav_file'], 'wb')
             play()
             gsav_file.close()
         else:
             print(Fore.RED + "\nError:" + Fore.RESET + " Unrecognized file type. \
 Only .gest and .gsav file extentions are supported")
     except KeyboardInterrupt:
         exit() #exit the game in case the user press `ctrl+C` which raises a KeyboardInterrupt
+
+if __name__=='__main__':
+    main()
```

### Comparing `gester-1.0.0/src/gester.egg-info/PKG-INFO` & `gester-1.1.0/src/gester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gester
-Version: 1.0.0
+Version: 1.1.0
 Summary: A game engine for console based text game
 Author-email: etcetra7n <greeknio@gmail.com>
 License: Boost Software License - Version 1.0 - August 17th, 2003
         
         Permission is hereby granted, free of charge, to any person or organization
         obtaining a copy of the software and accompanying documentation covered by
         this license (the "Software") to use, reproduce, display, distribute,
```

