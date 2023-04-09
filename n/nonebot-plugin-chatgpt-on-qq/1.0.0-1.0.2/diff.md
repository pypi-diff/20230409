# Comparing `tmp/nonebot-plugin-chatgpt-on-qq-1.0.0.tar.gz` & `tmp/nonebot-plugin-chatgpt-on-qq-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-1.0.0.tar", last modified: Sat Apr  8 19:16:16 2023, max compression
+gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-1.0.2.tar", last modified: Sun Apr  9 16:02:18 2023, max compression
```

## Comparing `nonebot-plugin-chatgpt-on-qq-1.0.0.tar` & `nonebot-plugin-chatgpt-on-qq-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 19:16:16.534462 nonebot-plugin-chatgpt-on-qq-1.0.0/
--rw-rw-rw-   0        0        0      769 2023-04-08 19:16:16.532461 nonebot-plugin-chatgpt-on-qq-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-08 19:16:16.517738 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq/
--rw-rw-rw-   0        0        0    12548 2023-03-22 09:12:42.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq/__init__.py
--rw-rw-rw-   0        0        0     3819 2023-04-08 19:14:06.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq/chatGPT.py
--rw-rw-rw-   0        0        0      423 2023-04-08 19:14:06.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq/config.py
--rw-rw-rw-   0        0        0     7253 2023-04-08 19:14:06.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq/conversation.py
--rw-rw-rw-   0        0        0      502 2023-03-07 16:08:33.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq/custom_errors.py
--rw-rw-rw-   0        0        0     1969 2023-03-15 12:15:37.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq/main.py
-drwxrwxrwx   0        0        0        0 2023-04-08 19:16:16.528967 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq.egg-info/
--rw-rw-rw-   0        0        0      769 2023-04-08 19:16:16.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2023-04-08 19:16:16.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 19:16:16.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-04-08 19:16:16.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-04-08 19:16:16.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 19:16:16.534462 nonebot-plugin-chatgpt-on-qq-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-04-08 19:15:49.000000 nonebot-plugin-chatgpt-on-qq-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:02:18.884490 nonebot-plugin-chatgpt-on-qq-1.0.2/
+-rw-rw-rw-   0        0        0      769 2023-04-09 16:02:18.880487 nonebot-plugin-chatgpt-on-qq-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-09 16:02:18.850300 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq/
+-rw-rw-rw-   0        0        0    12538 2023-04-09 15:34:37.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq/__init__.py
+-rw-rw-rw-   0        0        0     3660 2023-04-09 15:33:24.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq/chatGPT.py
+-rw-rw-rw-   0        0        0      416 2023-04-08 19:05:12.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq/config.py
+-rw-rw-rw-   0        0        0     4351 2023-04-08 19:05:35.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq/conversation.py
+-rw-rw-rw-   0        0        0      502 2023-03-07 16:08:33.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq/custom_errors.py
+-rw-rw-rw-   0        0        0     5422 2023-04-09 15:59:04.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq/loadpresets.py
+drwxrwxrwx   0        0        0        0 2023-04-09 16:02:18.876493 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq.egg-info/
+-rw-rw-rw-   0        0        0      769 2023-04-09 16:02:18.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2023-04-09 16:02:18.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 16:02:18.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-04-09 16:02:18.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-04-09 16:02:18.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 16:02:18.884490 nonebot-plugin-chatgpt-on-qq-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-04-09 16:01:36.000000 nonebot-plugin-chatgpt-on-qq-1.0.2/setup.py
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.0.0/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 1.0.0
+Version: 1.0.2
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq/__init__.py` & `nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 import json
 import re
 
-from typing import Dict, List
-
 from nonebot import get_driver
 from nonebot.adapters.onebot.v11 import (Bot,
                                          Event,
                                          GroupMessageEvent, PrivateMessageEvent)
 from nonebot.log import logger
 from nonebot.plugin import on_regex, on_fullmatch
 from nonebot.params import ArgPlainText
 
-from .conversation import Conversation, GroupPanel
+from .conversation import Conversation, GroupPanel,listpresets
 from .custom_errors import NoApiKeyError
+
 Chat = on_regex(r"^/talk\s+.+")  # 聊天
 CallMenu = on_fullmatch("/chat")  # 呼出菜单
 ShowList = on_regex(r"^/chat\s+list\s*$")  # 展示群聊天列表
 Join = on_regex(r"^/chat\s+join\s+\d+")  # 加入对话
 Delete = on_regex(r"^/chat\s+delete\s+\d+")  # 删除对话
 Dump = on_regex(r"^/chat\s+dump$")  # 导出json
-CreateConversationWithPrompt = on_regex(
-    r"^/chat\s+create\s+.+$")  # 利用自定义prompt创建对话
-CreateConversationWithTemplate = on_regex(r"^/chat\s+create$")  # 利用模板创建对话
-CreateConversationWithJson = on_regex(r"^/chat\s+json$")  # 利用json创建对话
+CreateConversationWithPrompt = on_regex(r"^/chat\s+create\s+.+$")# 利用自定义prompt创建对话
+CreateConversationWithTemplate = on_regex(r"^/chat\s+create$")# 利用模板创建对话
+CreateConversationWithJson = on_regex(r"^/chat\s+json$")# 利用json创建对话
 
-groupPanels: Dict[int,GroupPanel] = {}
-privateConversations: Dict[int, Conversation] = {}
+groupPanels: dict[int:GroupPanel] = {}
+privateConversations: dict[int, Conversation] = {}
 
 
 @Dump.handle()
 async def _(event: Event):
     userId = event.get_user_id()
     if isinstance(event, GroupMessageEvent):
         groupId = event.group_id
@@ -57,35 +55,35 @@
         else:  # 获取GroupPanel
             groupPanel = groupPanels.get(groupId)
         if not groupPanel.userInConversation.get(userId):
             await Chat.finish("你还没有加入一个对话!请用/chat create命令来创建对话!", at_sender=True)
         else:  # 获取用户当前加入的对话
             userConversation: Conversation = groupPanel.userInConversation.get(
                 userId)
-        try:
-            answer = await userConversation.ask(userInput)
-            await userConversation.GroupAutoSave(groupId)
-        except Exception as e:
-            answer = "获取gpt回答失败,访问请求速度过快或是网络波动orz\n若反复出现,可尝试使用/chat delete 序号 命令来删除该对话并重新创建"
-            logger.error(str(e))
+        # try:
+        answer = await userConversation.ask(userInput)
+        await userConversation.GroupAutoSave(groupId)
+        # except Exception as e:
+        #     answer = "获取gpt回答失败,访问请求速度过快或是网络波动orz\n若反复出现,可尝试使用/chat delete 序号 命令来删除该对话并重新创建"
+        #     logger.error(str(e))
         await Chat.finish(answer, at_sender=True)
     if isinstance(event, PrivateMessageEvent):
         userId = event.get_user_id()
         if not privateConversations.get(userId):
             await Chat.finish("尚未创建过对话!请用/chat create命令来创建对话!")
         else:
             userConversation: Conversation = privateConversations.get(userId)
-            try:
-                answer = await userConversation.ask(userInput)
-                await Chat.send(answer)
-                await userConversation.PrivateAutoSave()
-            except Exception as e:
-                answer = "test获取gpt回答失败,访问请求速度过快或是网络波动orz\n若反复出现,可尝试使用/chat delete 序号 命令来删除该对话并重新创建"
-                logger.error(str(e))
-                await Chat.finish(answer, at_sender=True)
+            # try:
+            answer = await userConversation.ask(userInput)
+            await Chat.send(answer)
+            await userConversation.PrivateAutoSave()
+            # except Exception as e:
+            #     answer="test获取gpt回答失败,访问请求速度过快或是网络波动orz\n若反复出现,可尝试使用/chat delete 序号 命令来删除该对话并重新创建"
+            #     logger.error(str(e))
+            #     await Chat.finish(answer,at_sender=True)
 
 
 @Join.handle()
 async def _(event: Event):
     msg = event.get_plaintext()
     msg = re.sub(r"^/chat\s+join\s+", '', msg)
     id = int(msg)
@@ -106,20 +104,20 @@
 @CallMenu.handle()
 async def _(bot: Bot, event: Event):
     menu: str = (
         "太长不看版:\n"
         + "先用/chat create命令,选择模板来创建对话,随后/talk 内容 来对话\n\n"
         + "/chat :获取菜单\n"
         + "/chat create :利用模板创建一个对话并加入\n"
-        + "/talk <内容> :在当前的对话进行聊天"
+        + "/talk <内容> :在当前的对话进行聊天\n"
         + "/chat list :获得当前已创建的对话列表\n"
         + "/chat join 序号(指/chat list中的序号) :参与list中的某个对话\n"
         + "/chat create (prompt) :自定义prompt来创建一个新的对话\n"
         + "/chat delete 序号(指/chat list中的序号) :删除list中的某个对话\n"
-        + "/chat dump :导出当前对话的历史记录json"
+        + "/chat dump :导出当前对话的历史记录json\n"
     )
     await CallMenu.finish(menu, at_sender=True)
 
 
 @Delete.handle()
 async def _(event: Event):
     msg = event.get_plaintext()
@@ -128,17 +126,17 @@
     if isinstance(event, GroupMessageEvent):
         groupPanel = groupPanels.get(event.group_id)
         if not groupPanel:
             await Join.finish("本群尚未创建过对话!", at_sender=True)
         if id < 1 or id > len(groupPanel.conversations):
             await Join.finish("序号超出!", at_sender=True)
         userId = event.get_user_id()
-        if groupPanel.conversations[id-1].owner.id == userId or userId in groupPanel.conversations[id-1].admin:
+        if groupPanel.conversations[id-1].owner.id == userId:
             conver = groupPanel.conversations[id-1]
-            jointUser: List[int] = []
+            jointUser: list[int] = []
             for user, conversation in groupPanel.userInConversation.items():
                 if conver == conversation:
                     jointUser.append(user)
             for user in jointUser:
                 groupPanel.userInConversation.pop(user)
 
             groupPanel.conversations.pop(id-1)
@@ -197,17 +195,16 @@
                 await CreateConversationWithPrompt.finish(f"用户{str(userID)}创建成功")
     else:  # 若prompt全为空
         await CreateConversationWithPrompt.finish("输入prompt不能为空格!")
 
 
 @CreateConversationWithTemplate.handle()
 async def CreateConversation(event: Event):
-    await CreateConversationWithTemplate.send("请选择模板:\n" +
-                                              "1.普通ChatGPT\n" +
-                                              "2.猫娘\n", at_sender=True)
+    ans=listpresets()
+    await CreateConversationWithTemplate.send(ans, at_sender=True)
 
 # 暂时完成
 
 
 @CreateConversationWithTemplate.got(key="template")
 async def Create(event: Event, id: str = ArgPlainText("template")):
     ifGroup = True
@@ -219,27 +216,29 @@
     if not id.isdigit():
         await CreateConversationWithTemplate.reject("输入ID无效!")
     newConversation = None
     try:
         newConversation = Conversation.CreateWithTemplate(id, userId)
     except NoApiKeyError:
         await CreateConversationWithTemplate.finish("请机器人管理员在设置中添加APIKEY！")
-    except Exception as e:
-        logger.error(str(e))
-    if int(id) == 1:
-        if newConversation is not None:
-            await CreateConversationWithTemplate.send("创建普通模板成功!", at_sender=True)
-    elif int(id) == 2:
-        if newConversation is not None:
-            await CreateConversationWithTemplate.send("创建猫娘模板成功!", at_sender=True)
-    elif int(id) == 3:
-        if newConversation is not None:
-            await CreateConversationWithTemplate.send("创建诺拉模板成功!", at_sender=True)
-    else:
-        await CreateConversationWithTemplate.finish("不存在该序号!")
+    if newConversation is not None:
+        await CreateConversationWithTemplate.send(f"创建{newConversation.name}模板成功!",at_sender=True)
+    else :
+        await CreateConversationWithTemplate.finish("输入ID无效!")
+    # if int(id) == 1:
+    #     if newConversation is not None:
+    #         await CreateConversationWithTemplate.send("创建普通模板成功!", at_sender=True)
+    # elif int(id) == 2:
+    #     if newConversation is not None:
+    #         await CreateConversationWithTemplate.send("创建猫娘模板成功!", at_sender=True)
+    # elif int(id) == 3:
+    #     if newConversation is not None:
+    #         await CreateConversationWithTemplate.send("创建诺拉模板成功!", at_sender=True)
+    # else:
+    #     await CreateConversationWithTemplate.finish("不存在该序号!")
     if ifGroup:
         if not groupPanels.get(event.group_id):
             groupPanels[event.group_id] = GroupPanel()
         groupPanels[event.group_id].userInConversation[userId] = newConversation
         groupPanels[event.group_id].conversations.append(newConversation)
     else:
         privateConversations[userId] = newConversation
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq/chatGPT.py` & `nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq/chatGPT.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,117 +1,107 @@
 import openai
 # import tiktoken
 import json
 from nonebot.log import logger
 from nonebot import get_driver
 
-from typing import Dict, List
-
 from .config import Config
-from .custom_errors import OverMaxTokenLengthError, NoResponseError, NoApiKeyError
+from .custom_errors import OverMaxTokenLengthError, NoResponseError,NoApiKeyError
 
 plugin_config = Config.parse_obj(get_driver().config.dict())
 
 # ENCODER = tiktoken.get_encoding("gpt2")
 MAX_TOKEN = 4000
-
-if plugin_config.model_name:
-    MODEL = plugin_config.model_name
-else:
-    MODEL = "gpt-3.5-turbo"
-
-if plugin_config.temperature:
-    TEMPERATURE = plugin_config.temperature
-else:
-    TEMPERATURE = 0.5
+MODEL = "gpt-3.5-turbo"
 
 
 class PromptManager:
     def __init__(self,  basic_prompt, history_max: int) -> None:
-        self.history: List[Dict[str, str]] = basic_prompt
+        self.history: list[dict[str:str]] = basic_prompt
         self.history_max = history_max
-        self.basic_len = len(basic_prompt)
-        self.count = 0
+        self.basic_len=len(basic_prompt)
+        self.count=0
 
     # def check_token_length(self, dicts) -> int:
     #     msgs: str = ""
     #     for dict in dicts:
     #         msgs += (dict["content"])+(dict["role"])+":::\n\n\n" #人工补正
     #     # print("预估长度："+str(len(ENCODER.encode(msgs))))
     #     return len(ENCODER.encode(msgs))
 
     def construct_prompt(
             self,
             new_prompt: str,
-    ) -> List[Dict[str, str]]:
+    ) -> list[dict[str:str]]:
         self.history.append({"role": "user", "content": new_prompt})
-        # if (len(self.history)-self.basic_len > self.history_max+1):
+        #if (len(self.history)-self.basic_len > self.history_max+1):
         while len(self.history)-self.basic_len > self.history_max+1:
             self.history.pop(self.basic_len)
+            logger.info(f"{len(self.history)-self.basic_len}  {self.history_max}")
         return self.history
 
     def add_to_history(self, completion):
         role = completion["choices"][0]["message"]["role"]
         content = completion["choices"][0]["message"]["content"]
         self.history.append({"role": role, "content": content})
-
     def dumpJsonStr(self):
-        self.count = self.count+1
+        self.count=self.count+1
         try:
-            jsonStr = json.dumps(self.history, ensure_ascii=False)
+            jsonStr=json.dumps(self.history,ensure_ascii=False)
         except UnicodeEncodeError:
-            jsonStr = json.dumps(self.history, ensure_ascii=True)
+            jsonStr=json.dumps(self.history,ensure_ascii=True)
         return jsonStr
+        
+
 
 
 class ChatGPTBot:
-    def __init__(self, api_key: str, basic_prompt, history_max: int) -> None:
-        if api_key:
+    def __init__(self, api_key: str, basic_prompt,history_max:int) -> None:
+        if api_key != "NoKey":
             openai.api_key = api_key
         else:
             raise NoApiKeyError("未设置ApiKey")
-        self.prompt_manager = PromptManager(
-            basic_prompt=basic_prompt, history_max=history_max)
-        self.talk_count = 0
+        self.prompt_manager = PromptManager(basic_prompt=basic_prompt,history_max=history_max)
+        self.talk_count=0
 
     async def ask(
         self,
         user_input: str,
-        temperature: float = TEMPERATURE
-    ) -> Dict:
+        temperature: float = 0.5,
+    ) -> dict:
 
         try:
             completion = await self._get_completion(user_input, temperature)
             await self._process_completion(completion=completion)
             return completion["choices"][0]["message"]["content"]
         except:
             self.prompt_manager.history.pop()
             raise ConnectionError
+        
 
     async def _get_completion(
             self,
             user_input: str,
-            temperature: float = TEMPERATURE
+            temperature: float = 0.5
     ):
 
         return await openai.ChatCompletion.acreate(
             model=MODEL,
             messages=self.prompt_manager.construct_prompt(user_input),
             temperature=temperature,
             max_tokens=1000
         )
 
     async def _process_completion(
         self,
-        completion: Dict
+        completion: dict
     ):
         if completion.get("choices") is None:
             raise NoResponseError("未返回任何choices")
         if (len(completion["choices"]) == 0):
             raise NoResponseError("返回的choices长度为0")
         if completion["choices"][0].get("message") is None:
             raise NoResponseError("未返回任何文本!")
 
         self.prompt_manager.add_to_history(completion)
-
     def dumpJsonStr(self):
         return self.prompt_manager.dumpJsonStr()
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 1.0.0
+Version: 1.0.2
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.0.0/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt` & `nonebot-plugin-chatgpt-on-qq-1.0.2/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 README.rst
 setup.py
 nonebot_plugin_chatgpt_on_qq/__init__.py
 nonebot_plugin_chatgpt_on_qq/chatGPT.py
 nonebot_plugin_chatgpt_on_qq/config.py
 nonebot_plugin_chatgpt_on_qq/conversation.py
 nonebot_plugin_chatgpt_on_qq/custom_errors.py
-nonebot_plugin_chatgpt_on_qq/main.py
+nonebot_plugin_chatgpt_on_qq/loadpresets.py
 nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
 nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
 nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
 nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
 nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.0.0/setup.py` & `nonebot-plugin-chatgpt-on-qq-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding:utf-8
 
 from setuptools import find_packages, setup
 
 setup(
     name='nonebot-plugin-chatgpt-on-qq',
-    version='1.0.0',
+    version='1.0.2',
     description='具有多对话功能的chatGPT聊天插件',
     long_description=open('README.rst').read(),
     author='颜曦',
     author_email='424504326@qq.com',
     maintainer='颜曦',
     maintainer_email='424504326@qq.com',
     packages=find_packages(),
```

