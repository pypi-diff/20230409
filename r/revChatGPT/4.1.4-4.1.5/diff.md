# Comparing `tmp/revChatGPT-4.1.4.tar.gz` & `tmp/revChatGPT-4.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-4.1.4.tar", last modified: Sat Apr  8 03:10:46 2023, max compression
+gzip compressed data, was "revChatGPT-4.1.5.tar", last modified: Sun Apr  9 14:43:36 2023, max compression
```

## Comparing `revChatGPT-4.1.4.tar` & `revChatGPT-4.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 03:10:46.958106 revChatGPT-4.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-08 03:10:12.000000 revChatGPT-4.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-04-08 03:10:46.958106 revChatGPT-4.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-04-08 03:10:46.000000 revChatGPT-4.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-08 03:10:46.962106 revChatGPT-4.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-08 03:10:12.000000 revChatGPT-4.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 03:10:46.958106 revChatGPT-4.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 03:10:46.958106 revChatGPT-4.1.4/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    34583 2023-04-08 03:10:12.000000 revChatGPT-4.1.4/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-04-08 03:10:12.000000 revChatGPT-4.1.4/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-08 03:10:12.000000 revChatGPT-4.1.4/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-08 03:10:12.000000 revChatGPT-4.1.4/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 03:10:46.958106 revChatGPT-4.1.4/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-08 03:10:12.000000 revChatGPT-4.1.4/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-08 03:10:12.000000 revChatGPT-4.1.4/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-08 03:10:12.000000 revChatGPT-4.1.4/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 03:10:46.958106 revChatGPT-4.1.4/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-04-08 03:10:46.000000 revChatGPT-4.1.4/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-08 03:10:46.000000 revChatGPT-4.1.4/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 03:10:46.000000 revChatGPT-4.1.4/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-08 03:10:46.000000 revChatGPT-4.1.4/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-08 03:10:46.000000 revChatGPT-4.1.4/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:43:36.665821 revChatGPT-4.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-09 14:43:07.000000 revChatGPT-4.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-04-09 14:43:36.665821 revChatGPT-4.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-04-09 14:43:36.000000 revChatGPT-4.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-09 14:43:36.665821 revChatGPT-4.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-09 14:43:07.000000 revChatGPT-4.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:43:36.661821 revChatGPT-4.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:43:36.665821 revChatGPT-4.1.5/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    34475 2023-04-09 14:43:07.000000 revChatGPT-4.1.5/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22942 2023-04-09 14:43:07.000000 revChatGPT-4.1.5/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-09 14:43:07.000000 revChatGPT-4.1.5/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-09 14:43:07.000000 revChatGPT-4.1.5/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:43:36.665821 revChatGPT-4.1.5/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-09 14:43:07.000000 revChatGPT-4.1.5/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-09 14:43:07.000000 revChatGPT-4.1.5/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-09 14:43:07.000000 revChatGPT-4.1.5/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:43:36.665821 revChatGPT-4.1.5/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-04-09 14:43:36.000000 revChatGPT-4.1.5/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-09 14:43:36.000000 revChatGPT-4.1.5/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:43:36.000000 revChatGPT-4.1.5/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-09 14:43:36.000000 revChatGPT-4.1.5/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 14:43:36.000000 revChatGPT-4.1.5/src/revChatGPT.egg-info/top_level.txt
```

### Comparing `revChatGPT-4.1.4/LICENSE` & `revChatGPT-4.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.4/PKG-INFO` & `revChatGPT-4.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 4.1.4
+Version: 4.1.5
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-4.1.4/README.md` & `revChatGPT-4.1.5/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.4/setup.py` & `revChatGPT-4.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="4.1.4",
+    version="4.1.5",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-4.1.4/src/revChatGPT/V1.py` & `revChatGPT-4.1.5/src/revChatGPT/V1.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 """
 from __future__ import annotations
 
 import base64
 import contextlib
 import json
 import logging
-import os
-import os.path as osp
 import time
 import uuid
 from functools import wraps
 from os import environ
 from os import getenv
 from typing import NoReturn
 
 import requests
+from pathlib import Path
 from httpx import AsyncClient
 from OpenAIAuth import Authenticator
 from OpenAIAuth import Error as AuthError
 
 from . import typings as t
 from .utils import create_completer
 from .utils import create_session
@@ -45,31 +44,25 @@
     """
 
     def decorator(func):
         wraps(func)
 
         def wrapper(*args, **kwargs):
             log.debug(
-                "Entering %s with args %s and kwargs %s",
-                func.__name__,
-                args,
-                kwargs,
+                f"Entering {func.__name__} with args {args} and kwargs {kwargs}",
             )
             start = time.time()
             out = func(*args, **kwargs)
             end = time.time()
             if is_timed:
                 log.debug(
-                    "Exiting %s with return value %s. Took %s seconds.",
-                    func.__name__,
-                    out,
-                    end - start,
+                    f"Exiting {func.__name__} with return value {out}. Took {end - start} seconds.",
                 )
             else:
-                log.debug("Exiting %s with return value %s", func.__name__, out)
+                log.debug(f"Exiting {func.__name__} with return value {out}")
 
             return out
 
         return wrapper
 
     return decorator
 
@@ -112,22 +105,22 @@
             session_client (_type_, optional): _description_. Defaults to None.
 
         Raises:
             Exception: _description_
         """
         user_home = getenv("HOME")
         if user_home is None:
-            self.cache_path = osp.join(os.getcwd(), ".chatgpt_cache.json")
+            self.cache_path = Path(Path().cwd(), ".chatgpt_cache.json")
         else:
             # mkdir ~/.config/revChatGPT
-            if not osp.exists(osp.join(user_home, ".config")):
-                os.mkdir(osp.join(user_home, ".config"))
-            if not osp.exists(osp.join(user_home, ".config", "revChatGPT")):
-                os.mkdir(osp.join(user_home, ".config", "revChatGPT"))
-            self.cache_path = osp.join(user_home, ".config", "revChatGPT", "cache.json")
+            if not Path(user_home, ".config").exists():
+                Path(user_home, ".config").mkdir()
+            if not Path(user_home, ".config", "revChatGPT").exists():
+                Path(user_home, ".config", "revChatGPT").mkdir()
+            self.cache_path = Path(user_home, ".config", "revChatGPT", "cache.json")
 
         self.config = config
         self.session = session_client() if session_client else requests.Session()
         try:
             cached_access_token = self.__get_cached_access_token(
                 self.config.get("email", None),
             )
@@ -298,16 +291,16 @@
 
         Args:
             info (dict): cache info, current format
             {
                 "access_tokens":{"someone@example.com": 'this account's access token', }
             }
         """
-        dirname = osp.dirname(self.cache_path) or "."
-        os.makedirs(dirname, exist_ok=True)
+        dirname = self.cache_path.home() or Path(".")
+        dirname.mkdir(parents=True, exist_ok=True)
         json.dump(info, open(self.cache_path, "w", encoding="utf-8"), indent=4)
 
     @logger(is_timed=False)
     def __read_cache(self):
         try:
             cached = json.load(open(self.cache_path, encoding="utf-8"))
         except (FileNotFoundError, json.decoder.JSONDecodeError):
@@ -385,41 +378,37 @@
             log.debug("Updating to new conversation by setting parent_id to None")
             self.parent_id = None
 
         conversation_id = conversation_id or self.conversation_id
         parent_id = parent_id or self.parent_id
         if conversation_id is None and parent_id is None:
             parent_id = str(uuid.uuid4())
-            log.debug("New conversation, setting parent_id to new UUID4: %s", parent_id)
+            log.debug(f"New conversation, setting parent_id to new UUID4: {parent_id}")
 
         if conversation_id is not None and parent_id is None:
             if conversation_id not in self.conversation_mapping:
                 if self.lazy_loading:
                     log.debug(
-                        "Conversation ID %s not found in conversation mapping, try to get conversation history for the given ID",
-                        conversation_id,
+                        f"Conversation ID {conversation_id} not found in conversation mapping, try to get conversation history for the given ID",
                     )
                     with contextlib.suppress(Exception):
                         history = self.get_msg_history(conversation_id)
                         self.conversation_mapping[conversation_id] = history[
                             "current_node"
                         ]
                 else:
                     log.debug(
-                        "Conversation ID %s not found in conversation mapping, mapping conversations",
-                        conversation_id,
+                        f"Conversation ID {conversation_id} not found in conversation mapping, mapping conversations",
                     )
 
                     self.__map_conversations()
 
             if conversation_id in self.conversation_mapping:
                 log.debug(
-                    "Conversation ID %s found in conversation mapping, setting parent_id to %s",
-                    conversation_id,
-                    self.conversation_mapping[conversation_id],
+                    f"Conversation ID {conversation_id} found in conversation mapping, setting parent_id to {self.conversation_mapping[conversation_id]}",
                 )
                 parent_id = self.conversation_mapping[conversation_id]
             else:  # invalid conversation_id provided, treat as a new conversation
                 conversation_id = None
                 parent_id = str(uuid.uuid4())
         data = {
             "action": "next",
@@ -456,15 +445,15 @@
         )
         self.__check_response(response)
         done: bool = False
         for line in response.iter_lines():
             # remove b' and ' at the beginning and end and ignore case
             line = str(line)[2:-1]
             if line.lower() == "internal server error":
-                log.error("Internal Server Error: %s", line)
+                log.error(f"Internal Server Error: {line}")
                 error = t.Error(
                     source="ask",
                     message="Internal Server Error",
                     code=t.ErrorType.SERVER_ERROR,
                 )
                 raise error
             if not line or line is None:
@@ -516,17 +505,17 @@
                 continue
             conversation_id = line["conversation_id"]
             parent_id = line["message"]["id"]
             try:
                 model = line["message"]["metadata"]["model_slug"]
             except KeyError:
                 model = None
-            log.debug("Received message: %s", message)
-            log.debug("Received conversation_id: %s", conversation_id)
-            log.debug("Received parent_id: %s", parent_id)
+            log.debug(f"Received message: {message}")
+            log.debug(f"Received conversation_id: {conversation_id}")
+            log.debug(f"Received parent_id: {parent_id}")
             yield {
                 "message": message.strip("\n"),
                 "conversation_id": conversation_id,
                 "parent_id": parent_id,
                 "model": model,
             }
         if not done:
@@ -877,21 +866,23 @@
 
 
 @logger(is_timed=False)
 def configure() -> dict:
     """
     Looks for a config file in the following locations:
     """
-    config_files = ["config.json"]
+    config_files: list[Path] = [Path("config.json")]
     if xdg_config_home := getenv("XDG_CONFIG_HOME"):
-        config_files.append(f"{xdg_config_home}/revChatGPT/config.json")
+        config_files.append(Path(xdg_config_home, "revChatGPT/config.json"))
     if user_home := getenv("HOME"):
-        config_files.append(f"{user_home}/.config/revChatGPT/config.json")
+        config_files.append(Path(user_home, ".config/revChatGPT/config.json"))
+    if windows_home := getenv("HOMEPATH"):
+        config_files.append(f"{windows_home}/.config/revChatGPT/config.json")
 
-    if config_file := next((f for f in config_files if osp.exists(f)), None):
+    if config_file := next((f for f in config_files if f.exists()), None):
         with open(config_file, encoding="utf-8") as f:
             config = json.load(f)
     else:
         print("No config file found.")
         raise FileNotFoundError("No config file found.")
     return config
```

### Comparing `revChatGPT-4.1.4/src/revChatGPT/V3.py` & `revChatGPT-4.1.5/src/revChatGPT/V3.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 A simple wrapper for the official ChatGPT API
 """
 import argparse
 import json
 import os
 import sys
 from importlib.resources import path
+from pathlib import Path
 from typing import AsyncGenerator
 from typing import NoReturn
 
 import httpx
 import requests
 import tiktoken
 
@@ -604,15 +605,15 @@
             top_p=args.top_p,
             reply_count=args.reply_count,
             engine=args.model,
         )
     # Check if internet is enabled
     if args.enable_internet:
         config = path("revChatGPT", "config").__str__()
-        chatbot.load(os.path.join(config, "enable_internet.json"), "conversation")
+        chatbot.load(Path(config, "enable_internet.json"), "conversation")
 
     session = create_session()
     completer = create_completer(
         [
             "!help",
             "!exit",
             "!reset",
```

### Comparing `revChatGPT-4.1.4/src/revChatGPT/__init__.py` & `revChatGPT-4.1.5/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.4/src/revChatGPT/__main__.py` & `revChatGPT-4.1.5/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.4/src/revChatGPT/config/enable_internet.json` & `revChatGPT-4.1.5/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.4/src/revChatGPT/typings.py` & `revChatGPT-4.1.5/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.4/src/revChatGPT/utils.py` & `revChatGPT-4.1.5/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.1.4/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-4.1.5/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 4.1.4
+Version: 4.1.5
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

