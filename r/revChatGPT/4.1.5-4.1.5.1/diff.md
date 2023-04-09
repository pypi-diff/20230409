# Comparing `tmp/revChatGPT-4.1.5.tar.gz` & `tmp/revChatGPT-4.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-4.1.5.tar", last modified: Sun Apr  9 14:43:36 2023, max compression
+gzip compressed data, was "revChatGPT-4.1.5.1.tar", last modified: Sun Apr  9 16:38:42 2023, max compression
```

## Comparing `revChatGPT-4.1.5.tar` & `revChatGPT-4.1.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:43:36.665821 revChatGPT-4.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-09 14:43:07.000000 revChatGPT-4.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-04-09 14:43:36.665821 revChatGPT-4.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-04-09 14:43:36.000000 revChatGPT-4.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-09 14:43:36.665821 revChatGPT-4.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-09 14:43:07.000000 revChatGPT-4.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:43:36.661821 revChatGPT-4.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:43:36.665821 revChatGPT-4.1.5/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    34475 2023-04-09 14:43:07.000000 revChatGPT-4.1.5/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    22942 2023-04-09 14:43:07.000000 revChatGPT-4.1.5/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-09 14:43:07.000000 revChatGPT-4.1.5/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-09 14:43:07.000000 revChatGPT-4.1.5/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:43:36.665821 revChatGPT-4.1.5/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-09 14:43:07.000000 revChatGPT-4.1.5/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-09 14:43:07.000000 revChatGPT-4.1.5/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-09 14:43:07.000000 revChatGPT-4.1.5/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:43:36.665821 revChatGPT-4.1.5/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-04-09 14:43:36.000000 revChatGPT-4.1.5/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-09 14:43:36.000000 revChatGPT-4.1.5/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:43:36.000000 revChatGPT-4.1.5/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-09 14:43:36.000000 revChatGPT-4.1.5/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 14:43:36.000000 revChatGPT-4.1.5/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:38:42.160083 revChatGPT-4.1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-09 16:38:05.000000 revChatGPT-4.1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-04-09 16:38:42.160083 revChatGPT-4.1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-04-09 16:38:41.000000 revChatGPT-4.1.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-09 16:38:42.160083 revChatGPT-4.1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-09 16:38:05.000000 revChatGPT-4.1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:38:42.152083 revChatGPT-4.1.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:38:42.156083 revChatGPT-4.1.5.1/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    34481 2023-04-09 16:38:05.000000 revChatGPT-4.1.5.1/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22942 2023-04-09 16:38:05.000000 revChatGPT-4.1.5.1/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-09 16:38:05.000000 revChatGPT-4.1.5.1/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-09 16:38:05.000000 revChatGPT-4.1.5.1/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:38:42.160083 revChatGPT-4.1.5.1/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-09 16:38:05.000000 revChatGPT-4.1.5.1/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-09 16:38:05.000000 revChatGPT-4.1.5.1/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-09 16:38:05.000000 revChatGPT-4.1.5.1/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 16:38:42.160083 revChatGPT-4.1.5.1/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-04-09 16:38:42.000000 revChatGPT-4.1.5.1/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-09 16:38:42.000000 revChatGPT-4.1.5.1/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 16:38:42.000000 revChatGPT-4.1.5.1/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-09 16:38:42.000000 revChatGPT-4.1.5.1/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 16:38:42.000000 revChatGPT-4.1.5.1/src/revChatGPT.egg-info/top_level.txt
```

### Comparing `revChatGPT-4.1.5/LICENSE` & `revChatGPT-4.1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.5/PKG-INFO` & `revChatGPT-4.1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 4.1.5
+Version: 4.1.5.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-4.1.5/README.md` & `revChatGPT-4.1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.5/setup.py` & `revChatGPT-4.1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="4.1.5",
+    version="4.1.5.1",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-4.1.5/src/revChatGPT/V1.py` & `revChatGPT-4.1.5.1/src/revChatGPT/V1.py`

 * *Files 0% similar despite different names*

```diff
@@ -872,15 +872,15 @@
     """
     config_files: list[Path] = [Path("config.json")]
     if xdg_config_home := getenv("XDG_CONFIG_HOME"):
         config_files.append(Path(xdg_config_home, "revChatGPT/config.json"))
     if user_home := getenv("HOME"):
         config_files.append(Path(user_home, ".config/revChatGPT/config.json"))
     if windows_home := getenv("HOMEPATH"):
-        config_files.append(f"{windows_home}/.config/revChatGPT/config.json")
+        config_files.append(Path(f"{windows_home}/.config/revChatGPT/config.json"))
 
     if config_file := next((f for f in config_files if f.exists()), None):
         with open(config_file, encoding="utf-8") as f:
             config = json.load(f)
     else:
         print("No config file found.")
         raise FileNotFoundError("No config file found.")
```

### Comparing `revChatGPT-4.1.5/src/revChatGPT/V3.py` & `revChatGPT-4.1.5.1/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.5/src/revChatGPT/__init__.py` & `revChatGPT-4.1.5.1/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.5/src/revChatGPT/__main__.py` & `revChatGPT-4.1.5.1/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.5/src/revChatGPT/config/enable_internet.json` & `revChatGPT-4.1.5.1/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.5/src/revChatGPT/typings.py` & `revChatGPT-4.1.5.1/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.5/src/revChatGPT/utils.py` & `revChatGPT-4.1.5.1/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.5/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-4.1.5.1/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 4.1.5
+Version: 4.1.5.1
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

