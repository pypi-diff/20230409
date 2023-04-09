# Comparing `tmp/ChatGPTWeb-0.0.4.tar.gz` & `tmp/ChatGPTWeb-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatGPTWeb-0.0.4.tar", last modified: Sat Apr  8 10:20:31 2023, max compression
+gzip compressed data, was "ChatGPTWeb-0.0.5.tar", last modified: Sun Apr  9 14:17:40 2023, max compression
```

## Comparing `ChatGPTWeb-0.0.4.tar` & `ChatGPTWeb-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 10:20:31.798356 ChatGPTWeb-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-04-08 10:20:31.789357 ChatGPTWeb-0.0.4/ChatGPTWeb/
--rw-rw-rw-   0        0        0    13828 2023-04-08 10:06:41.000000 ChatGPTWeb-0.0.4/ChatGPTWeb/ChatGPTWeb.py
--rw-rw-rw-   0        0        0       56 2023-04-08 08:59:30.000000 ChatGPTWeb-0.0.4/ChatGPTWeb/__init__.py
--rw-rw-rw-   0        0        0     1551 2023-04-08 10:18:52.000000 ChatGPTWeb-0.0.4/ChatGPTWeb/__main__.py
--rw-rw-rw-   0        0        0     4692 2023-04-07 13:14:27.000000 ChatGPTWeb-0.0.4/ChatGPTWeb/config.py
-drwxrwxrwx   0        0        0        0 2023-04-08 10:20:31.797356 ChatGPTWeb-0.0.4/ChatGPTWeb.egg-info/
--rw-rw-rw-   0        0        0     3011 2023-04-08 10:20:31.000000 ChatGPTWeb-0.0.4/ChatGPTWeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-04-08 10:20:31.000000 ChatGPTWeb-0.0.4/ChatGPTWeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 10:20:31.000000 ChatGPTWeb-0.0.4/ChatGPTWeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-08 10:20:31.000000 ChatGPTWeb-0.0.4/ChatGPTWeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-08 10:20:31.000000 ChatGPTWeb-0.0.4/ChatGPTWeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-04-07 06:03:43.000000 ChatGPTWeb-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3011 2023-04-08 10:20:31.798356 ChatGPTWeb-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2656 2023-04-08 10:18:57.000000 ChatGPTWeb-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-08 10:20:31.799356 ChatGPTWeb-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      748 2023-04-08 08:39:15.000000 ChatGPTWeb-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 14:17:40.260396 ChatGPTWeb-0.0.5/
+drwxrwxrwx   0        0        0        0 2023-04-09 14:17:40.253449 ChatGPTWeb-0.0.5/ChatGPTWeb/
+-rw-rw-rw-   0        0        0    15098 2023-04-09 14:04:38.000000 ChatGPTWeb-0.0.5/ChatGPTWeb/ChatGPTWeb.py
+-rw-rw-rw-   0        0        0       56 2023-04-08 08:59:30.000000 ChatGPTWeb-0.0.5/ChatGPTWeb/__init__.py
+-rw-rw-rw-   0        0        0     1551 2023-04-08 10:18:52.000000 ChatGPTWeb-0.0.5/ChatGPTWeb/__main__.py
+-rw-rw-rw-   0        0        0     6195 2023-04-09 14:04:00.000000 ChatGPTWeb-0.0.5/ChatGPTWeb/config.py
+drwxrwxrwx   0        0        0        0 2023-04-09 14:17:40.258397 ChatGPTWeb-0.0.5/ChatGPTWeb.egg-info/
+-rw-rw-rw-   0        0        0     3466 2023-04-09 14:17:40.000000 ChatGPTWeb-0.0.5/ChatGPTWeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-04-09 14:17:40.000000 ChatGPTWeb-0.0.5/ChatGPTWeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 14:17:40.000000 ChatGPTWeb-0.0.5/ChatGPTWeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-09 14:17:40.000000 ChatGPTWeb-0.0.5/ChatGPTWeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-09 14:17:40.000000 ChatGPTWeb-0.0.5/ChatGPTWeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-04-07 06:03:43.000000 ChatGPTWeb-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3466 2023-04-09 14:17:40.260396 ChatGPTWeb-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3111 2023-04-09 14:17:16.000000 ChatGPTWeb-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-09 14:17:40.260396 ChatGPTWeb-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      748 2023-04-09 14:16:59.000000 ChatGPTWeb-0.0.5/setup.py
```

### Comparing `ChatGPTWeb-0.0.4/ChatGPTWeb/ChatGPTWeb.py` & `ChatGPTWeb-0.0.5/ChatGPTWeb/ChatGPTWeb.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import json
 from playwright.async_api import async_playwright, Route, Request
 import asyncio
 import typing
 import threading
-from config import *
+from .config import *
 import logging
 import re
 from pathlib import Path
 
 class chatgpt():
     def __init__(self,
                  proxy: typing.Optional[ProxySettings] = None,
                  session_token: str = "",
-                 chat_file: Path = Path()/"data"/"chat_history",
-                 personality: str = "",
+                 chat_file: Path = Path()/"data"/"chat_history"/"conversation",
+                 personality: Optional[Personality] = Personality([{"name":"cat","value":"you are a cat now."}]),
                  log_status: bool = True,
                  plugin: bool = False) -> None:
         '''
         proxy : your proxy for openai | 你用于访问openai的代理
         session_token : your session_token | 你的session_token
         chat_file : save the chat history file path | 保存聊天文件的路径，默认 data/chat_history/..  
-        personality : init personality | 初始化人格
+        personality : init personality | 初始化人格 [{"name":"人格名","value":"预设内容"},{"name":"personality name","value":"personality value"},....]
         log_status : start log? | 开启日志输出吗
         plugin : is a Nonebot bot? | 作为Nonebot 插件实现
         '''
         self.data = MsgData()
         self.status = False
         self.join = False
         self.proxy = proxy
@@ -131,14 +131,15 @@
             self.access_token = access_token
             self.status = True
             self.join = True
             
         if self.plugin:
             from nonebot.log import logger
             self.logger = logger
+        self.personality.read_data()
         threading.Thread(target=self.tmp(loop)).start()
             
     def tmp(self,loop):
         asyncio.run_coroutine_threadsafe(self.__alive__(),loop)
 
                 
     def markdown_to_text(self,markdown_string):
@@ -165,39 +166,43 @@
             if "cookie" in request.headers:
                 self.header["Cookie"] = request.headers["cookie"]
             if "user-agent" in request.headers:
                 self.header["User-Agent"] = request.headers["user-agent"]
             await route.continue_(method="POST",headers=self.header,post_data=msg_data.post_data)
             
         await self.page.route("**/backend-api/conversation",route_handle) # type: ignore
-        
-        async with self.page.expect_response("https://chat.openai.com/backend-api/conversation") as response_info:
-            try:
-                self.logger.debug(f"send:{msg_data.msg_send}")
-                await self.page.goto(url_chatgpt)
-            except:
-                pass
-        resp = await response_info.value
-        stream_text = await resp.text()
-        stream_lines = stream_text.splitlines()
-        for x in stream_lines:
+        try:
+            async with self.page.expect_response("https://chat.openai.com/backend-api/conversation",timeout=600000) as response_info:
+                try:
+                    self.logger.debug(f"send:{msg_data.msg_send}")
+                    await self.page.goto(url_chatgpt,timeout=600000)
+                except:
+                    pass
+            resp = await response_info.value
+            stream_text = await resp.text()
+            stream_lines = stream_text.splitlines()
             for x in stream_lines:
-                if "finish_details" in x:
-                    msg = json.loads(x[6:])
-                    msg_data.msg_recv = self.markdown_to_text(msg["message"]["content"]["parts"][0]) 
-                    msg_data.conversation_id = msg["conversation_id"]
-                    msg_data.next_msg_id = msg["message"]["id"]
-                    msg_data.status = True
-                    msg_data.msg_type = "old_session"
-        if stream_lines:
-            self.logger.debug(f"recive:{msg_data.msg_recv}")
-            await self.save_chat(msg_data)
-        else:
-            msg_data.msg_recv = str(resp.status)
-        return msg_data
+                for x in stream_lines:
+                    if "finish_details" in x:
+                        msg = json.loads(x[6:])
+                        msg_data.msg_recv = self.markdown_to_text(msg["message"]["content"]["parts"][0]) 
+                        msg_data.conversation_id = msg["conversation_id"]
+                        msg_data.next_msg_id = msg["message"]["id"]
+                        msg_data.status = True
+                        msg_data.msg_type = "old_session"
+            if stream_lines:
+                self.logger.debug(f"recive:{msg_data.msg_recv}")
+                await self.save_chat(msg_data)
+            else:
+                msg_data.msg_recv = str(resp.status)
+            return msg_data
+        except:
+            msg_data.msg_recv = "error"
+            self.join = True
+            return msg_data
         
 
     async def save_chat(self,msg_data: MsgData):
         '''save chat file
         保存聊天文件'''
         path = self.chat_file/msg_data.conversation_id
         path.touch()
@@ -319,21 +324,41 @@
         else:
             msg_data.msg_recv = "back error"
             return msg_data
             
     async def init_personality(self,msg_data: MsgData):
         '''init_personality
         初始化人格'''
-        msg_data.msg_send = self.personality
+        msg_data.msg_send = self.personality.get_value_by_name(msg_data.msg_send)
         msg_data.conversation_id = ""
         msg_data.p_msg_id = ""
         msg_data.msg_type = "new_session"
         return await self.continue_chat(msg_data)
     
     async def back_init_personality(self,msg_data: MsgData):
         '''
         back the init_personality time
         回到初始化人格之后'''
         msg_data.msg_send = "1"
         msg_data.msg_type = "back_loop"
         return await self.back_chat_from_input(msg_data)
     
+    async def add_personality(self,personality: dict):
+        '''
+        personality = {"name":"cat1","value":"you are a cat now1."}
+        
+        add personality,please input json just like this.
+        添加人格 ,请传像这样的json数据
+        '''
+        self.personality.add_dict_to_list(personality)
+        self.personality.flush_data()
+        
+    async def show_personality_list(self):
+        '''show_personality_list 
+        展示人格列表'''
+        return self.personality.show_name()
+    
+    async def del_personality(self,name: str):
+        '''del_personality by name
+        删除人格根据名字'''
+        self.personality.del_data_by_name(name)
+        return self.personality.show_name()
```

### Comparing `ChatGPTWeb-0.0.4/ChatGPTWeb/__main__.py` & `ChatGPTWeb-0.0.5/ChatGPTWeb/__main__.py`

 * *Files identical despite different names*

### Comparing `ChatGPTWeb-0.0.4/ChatGPTWeb/config.py` & `ChatGPTWeb-0.0.5/ChatGPTWeb/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,67 @@
 import typing
 import uuid
 import json
 import logging
-from typing import TypedDict,Optional,Literal
+from typing import TypedDict,Optional,Literal,List,Dict
 
 url_session = "https://chat.openai.com/api/auth/session"
 url_chatgpt = "https://chat.openai.com:443/backend-api/conversation"
 
-formator = logging.Formatter(fmt = "%(asctime)s %(filename)s %(levelname)s %(message)s",
-                                         datefmt="%Y/%m/%d %X")
+formator = logging.Formatter(fmt = "%(asctime)s %(filename)s %(levelname)s %(message)s",datefmt="%Y/%m/%d %X")
+
+
+class Personality:
+    def __init__(self, init_list: List[Dict[str, str]]):
+        self.init_list = []
+        init_list += self.read_data()
+        for item in init_list:
+            if str(item) not in [str(x) for x in self.init_list]:
+                self.init_list.append(item)
+       
+    
+    def show_name(self):
+        name = [f"{index+1}. {x.get('name')}" for index,x in enumerate(self.init_list)]
+        return '\n'.join(name)
+    
+    
+    def get_value_by_name(self, name: str):
+        return next((x.get("value") for x in self.init_list if x.get("name") == name), None)
+    
+    def add_dict_to_list(self, new_dict: dict):
+        self.init_list.append(new_dict)
+        
+    def save_data(self):
+        tmp = '\n'.join([json.dumps(x) for x in self.init_list])
+        try:
+            with open("data/chat_history/personality","w") as f:
+                f.write(tmp)
+        except:
+            pass
+            
+    def read_data(self):
+        try:
+            with open("data/chat_history/personality","r") as f:
+                init_list = [json.loads(x) for x in f.read().split("\n")]
+        except:
+            init_list = []
+        return init_list
+                
+    def flush_data(self):
+        self.save_data()
+        self.read_data()
+        
+    def del_data_by_name(self,name:str):
+        for item in self.init_list:
+            if item.get('name') == name:
+                self.init_list.remove(item)
+        self.save_data()
+        return 
+
+
 class SetCookieParam(TypedDict, total=False):
     name: str
     value: str
     url: Optional[str]
     domain: Optional[str]
     path: Optional[str]
     expires: Optional[float]
```

### Comparing `ChatGPTWeb-0.0.4/ChatGPTWeb.egg-info/PKG-INFO` & `ChatGPTWeb-0.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,87 @@
-Metadata-Version: 2.1
-Name: ChatGPTWeb
-Version: 0.0.4
-Summary: a ChatGPT API,no web ui
-Home-page: https://github.com/nek0us/ChatGPT
-Author: nek0us
-Author-email: nekouss@gmail.com
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ChatGPT
-a ChatGPT api,no web ui
+ChatGPT api,not openai api,no web ui
 
 一个不怎么使用网页的ChatGPT api
 [![PyPi](https://img.shields.io/pypi/v/ChatGPTWeb.svg)](https://pypi.python.org/pypi/ChatGPTWeb)
 
+# 待填坑
+-   [x] 网页api对话构成
+-   [x] 多人格预设与切换
+-   [x] 聊天记录存储与导出
+-   [x] 自定义人设
+-   [x] 重置聊天或回到某一时刻
+-   [ ] 多账号并发
+-   [ ] GPT4
+-   [ ] 代码过于混乱等优化
+-   [ ] 抽空完善readme
+
+
 # 安装/Install
 Ubuntu & Windows
 
 ```bash
 pip install ChatGPTWeb
 
 sudo playwright install-deps
 
 playwright install firefox
 ```
 
 
 ### MsgData() 数据类型
 ```bash 
+from ChatGPTWeb.config import MsgData
+
 class MsgData(): 
     status: bool = False,
     msg_type: typing.Optional[typing.Literal["old_session","back_loop","new_session"]] = "new_session",
     msg_send: str = "hi",
     # your msg 
     msg_recv: str = "",
     # gpt's msg
     conversation_id: str = "",
     p_msg_id: str = "",
     # p_msg_id : the message's parent_message_id in this conversation id / 这个会话里某条消息的 parent_message_id
     next_msg_id: str = "",
     post_data: str = ""
 
-
-from ChatGPTWeb.config import MsgData
-data:MsgData = MsgData(conversation_id=c_id,p_msg_id=p_id)
-```
 # 使用/Used
 just simple to use
 
 简单使用
 
 ### copy __main__.py or this code to start / 复制 __main__.py 或者以下code来开始
 ```bash
 from ChatGPTWeb.ChatGPTWeb import chatgpt
-from ChatGPTWeb.config import MsgData
+from ChatGPTWeb.config import Personality
 import asyncio
 import aioconsole
 
 session_token=""
-person = "hello,my name is 'pig'."
-chat = chatgpt(session_token=session_token,personality=person,log_status=False)
+
+personality_definition = Personality(
+    [
+        {
+            "name":"猪咪",
+            'value':'咩~ '
+            },
+        {
+            "name":"cat",
+            "value":"you are a cat"
+        }
+        ])
+
+chat = chatgpt(session_token=session_token,log_status=False,personality=personality_definition)
 
 async def main():
     
     c_id = await aioconsole.ainput("your conversation_id if you have:")
     p_id = await aioconsole.ainput("your parent_message_id if you have:")
-    data:MsgData = MsgData(conversation_id=c_id,p_msg_id=p_id)
+    chat.data.conversation_id,chat.data.p_msg_id = c_id,p_id
     while 1:
         print("\n------------------------------")
         data.msg_send = await aioconsole.ainput("input：")
         print("------------------------------\n")
         if data.msg_send == "quit":
             break
         elif data.msg_send == "re":
```

### Comparing `ChatGPTWeb-0.0.4/LICENSE` & `ChatGPTWeb-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatGPTWeb-0.0.4/PKG-INFO` & `ChatGPTWeb-0.0.5/ChatGPTWeb.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,99 @@
 Metadata-Version: 2.1
 Name: ChatGPTWeb
-Version: 0.0.4
+Version: 0.0.5
 Summary: a ChatGPT API,no web ui
 Home-page: https://github.com/nek0us/ChatGPT
 Author: nek0us
 Author-email: nekouss@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ChatGPT
-a ChatGPT api,no web ui
+ChatGPT api,not openai api,no web ui
 
 一个不怎么使用网页的ChatGPT api
 [![PyPi](https://img.shields.io/pypi/v/ChatGPTWeb.svg)](https://pypi.python.org/pypi/ChatGPTWeb)
 
+# 待填坑
+-   [x] 网页api对话构成
+-   [x] 多人格预设与切换
+-   [x] 聊天记录存储与导出
+-   [x] 自定义人设
+-   [x] 重置聊天或回到某一时刻
+-   [ ] 多账号并发
+-   [ ] GPT4
+-   [ ] 代码过于混乱等优化
+-   [ ] 抽空完善readme
+
+
 # 安装/Install
 Ubuntu & Windows
 
 ```bash
 pip install ChatGPTWeb
 
 sudo playwright install-deps
 
 playwright install firefox
 ```
 
 
 ### MsgData() 数据类型
 ```bash 
+from ChatGPTWeb.config import MsgData
+
 class MsgData(): 
     status: bool = False,
     msg_type: typing.Optional[typing.Literal["old_session","back_loop","new_session"]] = "new_session",
     msg_send: str = "hi",
     # your msg 
     msg_recv: str = "",
     # gpt's msg
     conversation_id: str = "",
     p_msg_id: str = "",
     # p_msg_id : the message's parent_message_id in this conversation id / 这个会话里某条消息的 parent_message_id
     next_msg_id: str = "",
     post_data: str = ""
 
-
-from ChatGPTWeb.config import MsgData
-data:MsgData = MsgData(conversation_id=c_id,p_msg_id=p_id)
-```
 # 使用/Used
 just simple to use
 
 简单使用
 
 ### copy __main__.py or this code to start / 复制 __main__.py 或者以下code来开始
 ```bash
 from ChatGPTWeb.ChatGPTWeb import chatgpt
-from ChatGPTWeb.config import MsgData
+from ChatGPTWeb.config import Personality
 import asyncio
 import aioconsole
 
 session_token=""
-person = "hello,my name is 'pig'."
-chat = chatgpt(session_token=session_token,personality=person,log_status=False)
+
+personality_definition = Personality(
+    [
+        {
+            "name":"猪咪",
+            'value':'咩~ '
+            },
+        {
+            "name":"cat",
+            "value":"you are a cat"
+        }
+        ])
+
+chat = chatgpt(session_token=session_token,log_status=False,personality=personality_definition)
 
 async def main():
     
     c_id = await aioconsole.ainput("your conversation_id if you have:")
     p_id = await aioconsole.ainput("your parent_message_id if you have:")
-    data:MsgData = MsgData(conversation_id=c_id,p_msg_id=p_id)
+    chat.data.conversation_id,chat.data.p_msg_id = c_id,p_id
     while 1:
         print("\n------------------------------")
         data.msg_send = await aioconsole.ainput("input：")
         print("------------------------------\n")
         if data.msg_send == "quit":
             break
         elif data.msg_send == "re":
```

### Comparing `ChatGPTWeb-0.0.4/setup.py` & `ChatGPTWeb-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r",encoding="utf8") as readme_file:
     readme = readme_file.read()
 
 requirements = ["playwright","aioconsole"] # 这里填依赖包信息
 
 setup(
     name="ChatGPTWeb",
-    version="0.0.4",
+    version="0.0.5",
     author="nek0us",
     author_email="nekouss@gmail.com",
     description="a ChatGPT API,no web ui",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/nek0us/ChatGPT",
     packages=find_packages(),
```

