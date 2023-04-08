# Comparing `tmp/nonebot-plugin-SDGPT-0.0.7.tar.gz` & `tmp/nonebot-plugin-SDGPT-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-SDGPT-0.0.7.tar", last modified: Sat Apr  8 23:14:09 2023, max compression
+gzip compressed data, was "nonebot-plugin-SDGPT-0.0.8.tar", last modified: Sat Apr  8 23:50:00 2023, max compression
```

## Comparing `nonebot-plugin-SDGPT-0.0.7.tar` & `nonebot-plugin-SDGPT-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 23:14:09.694280 nonebot-plugin-SDGPT-0.0.7/
--rw-rw-rw-   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot-plugin-SDGPT-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      364 2023-04-08 23:14:09.693280 nonebot-plugin-SDGPT-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      147 2023-04-08 20:35:51.000000 nonebot-plugin-SDGPT-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 23:14:09.681269 nonebot-plugin-SDGPT-0.0.7/nonebot_plugin_SDGPT/
--rw-rw-rw-   0        0        0     3522 2023-04-08 19:41:45.000000 nonebot-plugin-SDGPT-0.0.7/nonebot_plugin_SDGPT/__init__.py
--rw-rw-rw-   0        0        0     8905 2023-04-08 20:30:32.000000 nonebot-plugin-SDGPT-0.0.7/nonebot_plugin_SDGPT/bot.py
-drwxrwxrwx   0        0        0        0 2023-04-08 23:14:09.691278 nonebot-plugin-SDGPT-0.0.7/nonebot_plugin_SDGPT.egg-info/
--rw-rw-rw-   0        0        0      364 2023-04-08 23:14:09.000000 nonebot-plugin-SDGPT-0.0.7/nonebot_plugin_SDGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-04-08 23:14:09.000000 nonebot-plugin-SDGPT-0.0.7/nonebot_plugin_SDGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 23:14:09.000000 nonebot-plugin-SDGPT-0.0.7/nonebot_plugin_SDGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2023-04-08 23:14:09.000000 nonebot-plugin-SDGPT-0.0.7/nonebot_plugin_SDGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-08 23:14:09.000000 nonebot-plugin-SDGPT-0.0.7/nonebot_plugin_SDGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 23:14:09.694280 nonebot-plugin-SDGPT-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      853 2023-04-08 23:12:36.000000 nonebot-plugin-SDGPT-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 23:50:00.604003 nonebot-plugin-SDGPT-0.0.8/
+-rw-rw-rw-   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot-plugin-SDGPT-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      210 2023-04-08 23:50:00.603002 nonebot-plugin-SDGPT-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2023-04-08 20:35:51.000000 nonebot-plugin-SDGPT-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-08 23:50:00.590991 nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT/
+-rw-rw-rw-   0        0        0     3550 2023-04-08 23:48:23.000000 nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT/__init__.py
+-rw-rw-rw-   0        0        0     8862 2023-04-08 23:40:51.000000 nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT/bot.py
+drwxrwxrwx   0        0        0        0 2023-04-08 23:50:00.601000 nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT.egg-info/
+-rw-rw-rw-   0        0        0      210 2023-04-08 23:50:00.000000 nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-04-08 23:50:00.000000 nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 23:50:00.000000 nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2023-04-08 23:50:00.000000 nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-08 23:50:00.000000 nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-08 23:50:00.604003 nonebot-plugin-SDGPT-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      663 2023-04-08 23:49:51.000000 nonebot-plugin-SDGPT-0.0.8/setup.py
```

### Comparing `nonebot-plugin-SDGPT-0.0.7/LICENSE` & `nonebot-plugin-SDGPT-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-SDGPT-0.0.7/nonebot_plugin_SDGPT/__init__.py` & `nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from nonebot import get_driver
+from nonebot import get_driver, require
 
 
 from .bot import info,error,warn
 from nonebot.plugin import on_command , on_message , on
 from nonebot.adapters.onebot.v11 import Bot, MessageSegment
 from nonebot.adapters import Message
 from nonebot.plugin import PluginMetadata
-from nonebot_plugin_guild_patch import GuildMessageEvent
+
 from nonebot.adapters.onebot.v11.event import GroupMessageEvent
 from nonebot.params import CommandArg
 from nonebot.rule import to_me
 from .bot import Chat,Bing,text2image,startup,Chat_api
 
 from dotenv import dotenv_values, load_dotenv
 config =dotenv_values(".cfg")
@@ -18,15 +18,15 @@
 __plugin_meta__ = PluginMetadata(
     name="ChatBot",
     description="ChatBot for NoneBot : 链接 ChatGPT / Bing / Stable-Diffusion",
     usage="ChatGPT Bing聊天, gpt解析自然语言转Stable-Diffusion生成图像",
     extra={},
 )
 
-
+GuildMessageEvent = require('nonebot_plugin_guild_patch').GuildMessageEvent
 
 driver = get_driver()
 
 @driver.on_startup
 async def do_something():
     global Presets
     global botList
```

### Comparing `nonebot-plugin-SDGPT-0.0.7/nonebot_plugin_SDGPT/bot.py` & `nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import glob
 from io import BytesIO
 import json
 import os
 import sys
 import time
 import re
-from nonebot import get_driver
+
 from nonebot.log import logger_id
-from nonebot.log import default_format, default_filter
+from nonebot.log import  default_filter
 
 from nonebot import logger
 import webuiapi
 from revChatGPT.V1 import Chatbot as chatGPT
 from revChatGPT.V3 import Chatbot as chatGPT_api
 from EdgeGPT import Chatbot as bing
 logger.remove(logger_id)
@@ -196,15 +196,15 @@
             with open(cfg_['cookies_file_path'], 'r') as f: # type: ignore
                 cookies = json.load(f)
                 suc('Config','配置文件 有效')
         else:raise Exception()
         cfg.update(cfg_)
     except:
         err('Config','配置文件 config.cfg 未配置')
-        raise Exception('配置文件 config.cfg 未配置')
+        # raise Exception('配置文件 config.cfg 未配置')
 
 
     botList  = []
 
     info('Presets Load','开始加载预设')
     Presets = {}
     for file_path in glob.glob(os.path.join(cfg['presets_dir'], '*.txt')):
```

