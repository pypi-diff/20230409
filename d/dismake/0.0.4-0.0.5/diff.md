# Comparing `tmp/dismake-0.0.4.tar.gz` & `tmp/dismake-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dismake-0.0.4.tar", last modified: Fri Mar 17 14:54:01 2023, max compression
+gzip compressed data, was "dist/dismake-0.0.5.tar", last modified: Sun Apr  9 15:55:20 2023, max compression
```

## Comparing `dismake-0.0.4.tar` & `dismake-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,40 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-03-17 14:54:01.615442 dismake-0.0.4/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      519 2023-03-17 14:54:01.615442 dismake-0.0.4/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       10 2023-03-17 14:37:30.000000 dismake-0.0.4/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-03-17 14:54:01.611442 dismake-0.0.4/dismake/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      114 2023-03-17 14:37:30.000000 dismake-0.0.4/dismake/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      310 2023-03-17 14:46:02.000000 dismake-0.0.4/dismake/_types.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2330 2023-03-17 14:37:30.000000 dismake-0.0.4/dismake/api.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-03-17 14:54:01.611442 dismake-0.0.4/dismake/app_commands/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       23 2023-03-17 14:37:30.000000 dismake-0.0.4/dismake/app_commands/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     9270 2023-03-17 14:47:57.000000 dismake-0.0.4/dismake/app_commands/command.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      865 2023-03-17 14:37:30.000000 dismake-0.0.4/dismake/asset.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     8062 2023-03-17 14:42:34.000000 dismake-0.0.4/dismake/client.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1464 2023-03-17 14:37:30.000000 dismake-0.0.4/dismake/enums.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     7858 2023-03-17 14:47:20.000000 dismake-0.0.4/dismake/interaction.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-03-17 14:54:01.615442 dismake-0.0.4/dismake/models/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       76 2023-03-17 14:37:30.000000 dismake-0.0.4/dismake/models/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1371 2023-03-17 14:48:19.000000 dismake-0.0.4/dismake/models/application_command.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2643 2023-03-17 14:37:30.000000 dismake-0.0.4/dismake/models/embed.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-03-17 14:37:30.000000 dismake-0.0.4/dismake/models/guild.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2174 2023-03-17 14:48:38.000000 dismake-0.0.4/dismake/models/user.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      852 2023-03-17 14:37:30.000000 dismake-0.0.4/dismake/params.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-03-17 14:54:01.615442 dismake-0.0.4/dismake/types/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      155 2023-03-17 14:37:30.000000 dismake-0.0.4/dismake/types/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      163 2023-03-17 14:49:03.000000 dismake-0.0.4/dismake/types/snowflake.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      613 2023-03-17 14:46:03.000000 dismake-0.0.4/dismake/utils.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-03-17 14:54:01.611442 dismake-0.0.4/dismake.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      519 2023-03-17 14:54:01.000000 dismake-0.0.4/dismake.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      589 2023-03-17 14:54:01.000000 dismake-0.0.4/dismake.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-03-17 14:54:01.000000 dismake-0.0.4/dismake.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       43 2023-03-17 14:54:01.000000 dismake-0.0.4/dismake.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        8 2023-03-17 14:54:01.000000 dismake-0.0.4/dismake.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-03-17 14:54:01.615442 dismake-0.0.4/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      871 2023-03-17 14:53:00.000000 dismake-0.0.4/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-09 15:55:20.081338 dismake-0.0.5/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      519 2023-04-09 15:55:20.081338 dismake-0.0.5/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       10 2023-04-02 02:37:00.000000 dismake-0.0.5/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-09 15:55:20.081338 dismake-0.0.5/dismake/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      137 2023-04-09 04:35:20.000000 dismake-0.0.5/dismake/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      310 2023-04-02 02:37:00.000000 dismake-0.0.5/dismake/_types.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      865 2023-04-02 02:37:00.000000 dismake-0.0.5/dismake/asset.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3938 2023-04-09 15:36:25.000000 dismake-0.0.5/dismake/client.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-09 15:55:20.081338 dismake-0.0.5/dismake/commands/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       46 2023-04-09 04:35:20.000000 dismake-0.0.5/dismake/commands/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5323 2023-04-09 15:38:37.000000 dismake-0.0.5/dismake/commands/command.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5192 2023-04-09 13:51:10.000000 dismake-0.0.5/dismake/commands/context.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3160 2023-04-08 19:27:21.000000 dismake-0.0.5/dismake/enums.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      573 2023-04-09 14:49:21.000000 dismake-0.0.5/dismake/errors.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5632 2023-04-09 15:32:55.000000 dismake-0.0.5/dismake/handler.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2347 2023-04-09 04:34:38.000000 dismake-0.0.5/dismake/http.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2150 2023-04-09 13:02:53.000000 dismake-0.0.5/dismake/interaction.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-09 15:55:20.081338 dismake-0.0.5/dismake/models/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       76 2023-04-02 02:37:00.000000 dismake-0.0.5/dismake/models/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1389 2023-04-04 12:31:54.000000 dismake-0.0.5/dismake/models/application_command.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-09 15:55:20.081338 dismake-0.0.5/dismake/models/channels/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       20 2023-04-08 19:27:21.000000 dismake-0.0.5/dismake/models/channels/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      158 2023-04-08 19:27:21.000000 dismake-0.0.5/dismake/models/channels/base.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1161 2023-04-08 19:27:21.000000 dismake-0.0.5/dismake/models/channels/text.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2643 2023-04-02 02:37:00.000000 dismake-0.0.5/dismake/models/embed.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2760 2023-04-02 02:37:00.000000 dismake-0.0.5/dismake/models/guild.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2142 2023-04-02 04:02:12.000000 dismake-0.0.5/dismake/models/user.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      852 2023-04-02 02:37:00.000000 dismake-0.0.5/dismake/params.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-09 15:55:20.081338 dismake-0.0.5/dismake/types/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      155 2023-04-02 02:37:00.000000 dismake-0.0.5/dismake/types/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      163 2023-04-02 02:37:00.000000 dismake-0.0.5/dismake/types/snowflake.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      613 2023-04-02 02:37:00.000000 dismake-0.0.5/dismake/utils.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-04-09 15:55:20.081338 dismake-0.0.5/dismake.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      519 2023-04-09 15:55:20.000000 dismake-0.0.5/dismake.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      747 2023-04-09 15:55:20.000000 dismake-0.0.5/dismake.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-04-09 15:55:20.000000 dismake-0.0.5/dismake.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       43 2023-04-09 15:55:20.000000 dismake-0.0.5/dismake.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        8 2023-04-09 15:55:20.000000 dismake-0.0.5/dismake.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-04-09 15:55:20.081338 dismake-0.0.5/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      871 2023-04-09 15:52:59.000000 dismake-0.0.5/setup.py
```

### Comparing `dismake-0.0.4/PKG-INFO` & `dismake-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dismake
-Version: 0.0.4
+Version: 0.0.5
 Summary: None
 Home-page: https://github.com/PranoyMajumdar/dismake
 Author: Pranoy Majumdar
 Author-email: officialpranoy2@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/PranoyMajumdar/dismake
 Description: # Dismake
```

### Comparing `dismake-0.0.4/dismake/api.py` & `dismake-0.0.5/dismake/http.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
-from typing import Optional
+from typing import List, Optional
 from httpx import AsyncClient, Response
 
 from .models import User
 from .models import ApplicationCommand
-from .app_commands import SlashCommand
+from .commands import SlashCommand
 
-__all__ = ("API",)
 
+__all__ = ("HttpClient",)
 
-class API:
+
+class HttpClient:
     def __init__(
         self,
         *,
         token: str,
         client_id: int,
     ) -> None:
         self.token = token
@@ -49,15 +50,15 @@
         _json = res.json()
         if not _json:
             return
 
         return [ApplicationCommand(**command) for command in _json]
 
     async def bulk_override_commands(
-        self, commands: list[SlashCommand], guild_id: Optional[int] = None
+        self, commands: List[SlashCommand], guild_id: Optional[int] = None
     ) -> Response:
         return await self.client.request(
             method="PUT",
             url=f"/applications/{self.client_id}/commands",
             json=[command.to_dict() for command in commands],
             headers=self.headers,
         )
```

### Comparing `dismake-0.0.4/dismake/asset.py` & `dismake-0.0.5/dismake/asset.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.4/dismake/models/application_command.py` & `dismake-0.0.5/dismake/models/application_command.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pydantic import BaseModel
-from typing import Optional, Union
+from typing import Dict, List, Optional, Union
 from ..types import SnowFlake
 
 
 __all__ = (
     "ApplicationCommandChoice",
     "ApplicationCommandOption",
     "ApplicationCommand",
@@ -18,31 +18,31 @@
 class ApplicationCommandOption(BaseModel):
     type: int
     name: str
     name_localizations: Optional[dict[str, str]]
     description: Optional[str] = "No description provided"
     description_localizations: Optional[dict[str, str]]
     required: Optional[bool] = False
-    choices: Optional[list[ApplicationCommandChoice]]
-    options: Optional[list["ApplicationCommandOption"]]
-    channel_types: Optional[list[str]]
+    choices: Optional[List[ApplicationCommandChoice]]
+    options: Optional[List["ApplicationCommandOption"]]
+    channel_types: Optional[List[str]]
     min_value: Optional[int]
     max_value: Optional[int]
     min_length: Optional[int]
     max_length: Optional[int]
     autocomplete: Optional[bool]
 
 
 class ApplicationCommand(BaseModel):
     id: SnowFlake
     type: int = 1
     application_id: SnowFlake
-    guild_id: Optional[int]
+    guild_id: Optional[SnowFlake]
     name: str
-    name_localizations: Optional[dict[str, str]]
+    name_localizations: Optional[Dict[str, str]]
     description: Optional[str] = "No description provided"
-    description_localizations: Optional[dict[str, str]]
-    options: Optional[list[ApplicationCommandOption]]
+    description_localizations: Optional[Dict[str, str]]
+    options: Optional[List[ApplicationCommandOption]]
     default_member_permissions: Optional[str]
     dm_permission: Optional[bool] = True
     nsfw: Optional[bool] = False
     version: int
```

### Comparing `dismake-0.0.4/dismake/models/embed.py` & `dismake-0.0.5/dismake/models/embed.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.4/dismake/models/user.py` & `dismake-0.0.5/dismake/models/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     1 << 22: "ACTIVE_DEVELOPER",
 }
 
 
 class User(BaseModel):
     id: int
     username: str
-    display_name: Optional[str]
     discriminator: str
     avatar: Optional[str]
     avatar_decoration: Optional[str]
     bot: Optional[bool]
     bio: Optional[str]
     system: Optional[bool]
     mfa_enabled: Optional[bool]
```

### Comparing `dismake-0.0.4/dismake/params.py` & `dismake-0.0.5/dismake/params.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.4/dismake/utils.py` & `dismake-0.0.5/dismake/utils.py`

 * *Files identical despite different names*

### Comparing `dismake-0.0.4/dismake.egg-info/PKG-INFO` & `dismake-0.0.5/dismake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dismake
-Version: 0.0.4
+Version: 0.0.5
 Summary: None
 Home-page: https://github.com/PranoyMajumdar/dismake
 Author: Pranoy Majumdar
 Author-email: officialpranoy2@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/PranoyMajumdar/dismake
 Description: # Dismake
```

### Comparing `dismake-0.0.4/dismake.egg-info/SOURCES.txt` & `dismake-0.0.5/dismake.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 README.md
 setup.py
 dismake/__init__.py
 dismake/_types.py
-dismake/api.py
 dismake/asset.py
 dismake/client.py
 dismake/enums.py
+dismake/errors.py
+dismake/handler.py
+dismake/http.py
 dismake/interaction.py
 dismake/params.py
 dismake/utils.py
 dismake.egg-info/PKG-INFO
 dismake.egg-info/SOURCES.txt
 dismake.egg-info/dependency_links.txt
 dismake.egg-info/requires.txt
 dismake.egg-info/top_level.txt
-dismake/app_commands/__init__.py
-dismake/app_commands/command.py
+dismake/commands/__init__.py
+dismake/commands/command.py
+dismake/commands/context.py
 dismake/models/__init__.py
 dismake/models/application_command.py
 dismake/models/embed.py
 dismake/models/guild.py
 dismake/models/user.py
+dismake/models/channels/__init__.py
+dismake/models/channels/base.py
+dismake/models/channels/text.py
 dismake/types/__init__.py
 dismake/types/snowflake.py
```

### Comparing `dismake-0.0.4/setup.py` & `dismake-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as file:
     long_description = file.read()
 setup(
     name="dismake",
-    version="0.0.4",
+    version="0.0.5",
     author="Pranoy Majumdar",
     author_email="officialpranoy2@gmail.com",
     description="None",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PranoyMajumdar/dismake",
     project_urls={"Homepage": "https://github.com/PranoyMajumdar/dismake"},
```

