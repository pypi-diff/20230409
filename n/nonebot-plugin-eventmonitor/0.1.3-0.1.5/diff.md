# Comparing `tmp/nonebot_plugin_eventmonitor-0.1.3.tar.gz` & `tmp/nonebot_plugin_eventmonitor-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_eventmonitor-0.1.3.tar", last modified: Fri Mar 31 12:09:10 2023, max compression
+gzip compressed data, was "nonebot_plugin_eventmonitor-0.1.5.tar", last modified: Sun Apr  9 06:13:09 2023, max compression
```

## Comparing `nonebot_plugin_eventmonitor-0.1.3.tar` & `nonebot_plugin_eventmonitor-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 12:09:10.884256 nonebot_plugin_eventmonitor-0.1.3/
--rw-rw-rw-   0        0        0    35149 2023-01-29 04:13:58.000000 nonebot_plugin_eventmonitor-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     3998 2023-03-31 12:09:10.880244 nonebot_plugin_eventmonitor-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3367 2023-03-31 12:02:55.000000 nonebot_plugin_eventmonitor-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-31 12:09:10.821261 nonebot_plugin_eventmonitor-0.1.3/nonebot_plugin_eventmonitor/
--rw-rw-rw-   0        0        0     4437 2023-03-26 13:14:45.000000 nonebot_plugin_eventmonitor-0.1.3/nonebot_plugin_eventmonitor/__init__.py
--rw-rw-rw-   0        0        0     1850 2023-03-26 12:19:28.000000 nonebot_plugin_eventmonitor-0.1.3/nonebot_plugin_eventmonitor/admin.py
--rw-rw-rw-   0        0        0     1276 2023-03-31 11:58:23.000000 nonebot_plugin_eventmonitor-0.1.3/nonebot_plugin_eventmonitor/honour.py
--rw-rw-rw-   0        0        0     2208 2023-03-26 13:16:28.000000 nonebot_plugin_eventmonitor-0.1.3/nonebot_plugin_eventmonitor/stamp.py
-drwxrwxrwx   0        0        0        0 2023-03-31 12:09:10.868261 nonebot_plugin_eventmonitor-0.1.3/nonebot_plugin_eventmonitor.egg-info/
--rw-rw-rw-   0        0        0     3998 2023-03-31 12:09:10.000000 nonebot_plugin_eventmonitor-0.1.3/nonebot_plugin_eventmonitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2023-03-31 12:09:10.000000 nonebot_plugin_eventmonitor-0.1.3/nonebot_plugin_eventmonitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 12:09:10.000000 nonebot_plugin_eventmonitor-0.1.3/nonebot_plugin_eventmonitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-03-31 12:09:10.000000 nonebot_plugin_eventmonitor-0.1.3/nonebot_plugin_eventmonitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-03-31 12:09:10.000000 nonebot_plugin_eventmonitor-0.1.3/nonebot_plugin_eventmonitor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-31 12:09:10.884256 nonebot_plugin_eventmonitor-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      993 2023-03-31 12:08:42.000000 nonebot_plugin_eventmonitor-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:13:09.467748 nonebot_plugin_eventmonitor-0.1.5/
+-rw-rw-rw-   0        0        0    35149 2023-01-29 04:13:58.000000 nonebot_plugin_eventmonitor-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1293 2023-04-09 06:13:09.467748 nonebot_plugin_eventmonitor-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      662 2023-04-09 06:12:53.000000 nonebot_plugin_eventmonitor-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 06:13:09.420829 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor/
+-rw-rw-rw-   0        0        0     4627 2023-04-09 06:00:28.000000 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor/__init__.py
+-rw-rw-rw-   0        0        0     1882 2023-04-09 05:58:13.000000 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor/admin.py
+-rw-rw-rw-   0        0        0     1086 2023-04-09 05:58:40.000000 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor/honour.py
+-rw-rw-rw-   0        0        0     1995 2023-04-09 05:58:48.000000 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor/stamp.py
+-rw-rw-rw-   0        0        0      386 2023-04-09 05:58:55.000000 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:13:09.467748 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor.egg-info/
+-rw-rw-rw-   0        0        0     1293 2023-04-09 06:13:08.000000 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2023-04-09 06:13:09.000000 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 06:13:08.000000 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-09 06:13:08.000000 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-04-09 06:13:08.000000 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 06:13:09.467748 nonebot_plugin_eventmonitor-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      993 2023-04-09 06:11:30.000000 nonebot_plugin_eventmonitor-0.1.5/setup.py
```

### Comparing `nonebot_plugin_eventmonitor-0.1.3/LICENSE` & `nonebot_plugin_eventmonitor-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_eventmonitor-0.1.3/nonebot_plugin_eventmonitor/admin.py` & `nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor/admin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 from datetime import datetime
-from .honour import bot_qq, super_qq
+from .utils import superusers
 
 
-
-def admin_changer(sub_type, user_id):
+async def admin_changer(sub_type, user_id, bot_qq) : 
     admin_msg = ""
+
     if sub_type == "set":
-        if user_id == bot_qq:
-            admin_msg = f"我也是管理啦，你们要小心喵~"
-        else:
-            admin_msg = f"🚔 管理员变动\n恭喜[CQ:at,qq={user_id}]喜提本群管理喵~"
+        admin_msg = (
+            "我也是管理啦，你们要小心喵~"
+            if user_id == bot_qq
+            else f"🚔 管理员变动\n恭喜[CQ:at,qq={user_id}]喜提本群管理喵~"
+        )
     elif sub_type == "unset":
-        if user_id == bot_qq:
-            admin_msg = f"呜呜，别下咱管理呀QwQ，喵呜~"
-        else:
-            admin_msg = f"🚔 管理员变动\n[CQ:at,qq={user_id}]痛失本群管理喵~"
+        admin_msg = (
+            "呜呜，别下咱管理呀QwQ，喵呜~"
+            if user_id == bot_qq
+            else f"🚔 管理员变动\n[CQ:at,qq={user_id}]痛失本群管理喵~"
+        )
     return admin_msg
 
 
-def del_user_bye(add_time, group_id, user_id):
-    global groups_all, del_user_msg
+async def del_user_bye(add_time, user_id):
+    global del_user_msg
     del_time = datetime.fromtimestamp(add_time)
-    if user_id in super_qq:
+    if user_id in superusers:
         del_user_msg = f"⌈{del_time}⌋\n@{user_id}恭送主人离开喵~"
+        print(superusers)
     else:
         del_user_msg = f"✈️ 成员变动⌈{del_time}⌋\nQQ号为：{user_id}的小可爱退群喵~" \
                        f"[CQ:image,file=https://q4.qlogo.cn/headimg_dl?dst_uin={user_id}&spec=640]"
         return del_user_msg
 
 
-def add_user_wecome(add_time, group_id, user_id):
+async def add_user_wecome(add_time, user_id, bot_qq):
     global groups_all, add_user_msg
     add_time = datetime.fromtimestamp(add_time)
     if user_id == bot_qq:
         add_user_msg = f"本喵被邀进入贵群喵~\n" \
                        f"火速上个管理喵~"
-    elif user_id in super_qq:
+    elif user_id in superusers:
         add_user_msg = f"✨ 成员变动 ✨\n@{user_id}[CQ:at,qq={user_id}]欢迎主人进群喵~[CQ:face,id=175]"
     else:
         add_user_msg = f"✨ 成员变动 ✨\n欢迎[CQ:at,qq={user_id}]的加入喵~\n加入时间：⌈{add_time}⌋，请在群内积极发言喵~" \
                        f"[CQ:image,file=https://q4.qlogo.cn/headimg_dl?dst_uin={user_id}&spec=640]"
     return add_user_msg
```

### Comparing `nonebot_plugin_eventmonitor-0.1.3/nonebot_plugin_eventmonitor/honour.py` & `nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor/honour.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,29 @@
-import nonebot
-from nonebot.permission import SUPERUSER
+from .utils import superusers
 
-try:
-    bot_qq = nonebot.get_driver().config.bot_qq
-except:
-    bot_qq = "寄"
-
-try:
-    super_qq = nonebot.get_driver().config.superusers
-except:
-    super_qq = "寄"
-
-
-
-def monitor_rongyu(honor_type, user_id):
+async def monitor_rongyu(honor_type, user_id, bot_qq):  
     rely = ""
 
-    if honor_type == "talkative":
+    if honor_type == "emotion":
         if user_id == bot_qq:
-            rely = f"你们又不行了，本喵喜提龙王🐲~"
-        elif user_id == super_qq:
-            rely = f"[CQ:at,qq={user_id}]恭喜主人荣获龙王🐲标识喵~"
+            pass
+        elif user_id != superusers:
+            rely = f"[CQ:at,qq={user_id}]恭喜主人荣获快乐源泉🤣标识喵~"
         else:
-            rely = f"恭喜[CQ:at,qq={user_id}]荣获龙王🐲标识喵~"
-
+            rely = f"恭喜[CQ:at,qq={user_id}]荣获快乐源泉🤣标识喵~"
     elif honor_type == "performer":
         if user_id == bot_qq:
             pass
-        elif user_id == super_qq:
+        elif user_id != superusers:
             rely = f"[CQ:at,qq={user_id}]恭喜主人荣获群聊之火🔥标识喵~"
         else:
             rely = f"恭喜[CQ:at,qq={user_id}]荣获群聊之火🔥标识喵~"
 
-    elif honor_type == "emotion":
+    elif honor_type == "talkative":
         if user_id == bot_qq:
-            pass
-        elif user_id == super_qq:
-            rely = f"[CQ:at,qq={user_id}]恭喜主人荣获快乐源泉🤣标识喵~"
+            rely = "你们又不行了，本喵喜提龙王🐲~"
+        elif user_id != superusers:
+            rely = f"[CQ:at,qq={user_id}]恭喜主人荣获龙王🐲标识喵~"
         else:
-            rely = f"恭喜[CQ:at,qq={user_id}]荣获快乐源泉🤣标识喵~"
+            rely = f"恭喜[CQ:at,qq={user_id}]荣获龙王🐲标识喵~"
+
     return rely
```

### Comparing `nonebot_plugin_eventmonitor-0.1.3/nonebot_plugin_eventmonitor/stamp.py` & `nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor/stamp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,57 @@
 import random
-import nonebot
+from .utils import nickname
 
-
-try:
-    bot_name = nonebot.get_driver().config.bot_name
-except:
-    bot_name = "寄"
-
-chuo_CD_dir = {}
-
-try:
-    chuo_cd = nonebot.get_driver().config.chuo_cd
-except:
-    chuo_cd = 0
     
-def chuo_send_msg():
+async def chuo_send_msg():
     rand_num = random.randint(0, len(chuo_msg) - 1)
     return chuo_msg[rand_num]
 
 
 chuo_msg = [
-    f"别戳了，{bot_name}怕疼QwQ",
-    f"呜呜，再戳{bot_name}脸都要肿了",
-    f"戳坏了{bot_name}，你赔得起吗？",
-    f"再戳{bot_name}，我要叫我主人了",
-    f"别老戳{bot_name}了，您歇会吧~",
-    f"再戳{bot_name}，咬你了嗷~",
-    f"想好了再戳，(*-`ω´-)✄",
-    f"喂，110吗，有人老戳我",
-    f"嗷呜嗷呜...恶龙咆哮┗|｀O′|┛",
-    f"有事恁叫我，别天天一个劲戳戳戳！",
-    f"再戳我让你变成女人，嘿嘿",
-    f"不要戳我了 >_<",
-    f"不要这样子啦(*/ω＼*)",
-    f"不要再戳了(害怕ing)",
-    f"还戳，哼(つд⊂)（生气）",
-    f"再戳，小心我顺着网线找你.",
-    f"咱要型气了o(>﹏<)o",
-    f"嘿嘿，好舒服呀(bushi)",
-    f"乖，好了好了，别戳了~",
-    f"我爪巴爪巴，球球别再戳了",
-    f"别再戳我了，行🐎？！",
-    f"啊呜，你有什么事吗？",
-    f"lsp你再戳？",
-    f"连个可爱美少女都要戳的肥宅真恶心啊。",
-    f"你再戳！",
-    f"？再戳试试？",
-    f"别戳了别戳了再戳就坏了555",
-    f"我爪巴爪巴，球球别再戳了",
-    f"你戳你🐎呢？！",
-    f"请不要戳{bot_name} >_<",
-    f"放手啦，不给戳QAQ",
-    f"喂(#`O′) 戳{bot_name}干嘛！",
-    f"戳坏了，赔钱！",
-    f"戳坏了",
-    f"嗯……不可以……啦……不要乱戳",
-    f"那...那里...那里不能戳...绝对...",
-    f"(。´・ω・)ん?",
-    f"有事恁叫我，别天天一个劲戳戳戳！",
-    f"欸很烦欸！你戳🔨呢",
-    f"再戳一下试试？",
-    f"正在关闭对您的所有服务...关闭成功",
-    f"啊呜，太舒服刚刚竟然睡着了。什么事？",
-    f"正在定位您的真实地址...定位成功。轰炸机已起飞"
+    f"别戳了，{nickname}怕疼QwQ",
+    f"呜呜，再戳{nickname}脸都要肿了",
+    f"戳坏了{nickname}，你赔得起吗？",
+    f"再戳{nickname}，我要叫我主人了",
+    f"别老戳{nickname}了，您歇会吧~",
+    f"再戳{nickname}，咬你了嗷~",
+    f"请不要戳{nickname} >_<",
+    f"喂(#`O′) 戳{nickname}干嘛！",
+    "想好了再戳，(*-`ω´-)✄",
+    "喂，110吗，有人老戳我",
+    "嗷呜嗷呜...恶龙咆哮┗|｀O′|┛",
+    "有事恁叫我，别天天一个劲戳戳戳！",
+    "再戳我让你变成女人，嘿嘿",
+    "不要戳我了 >_<",
+    "不要这样子啦(*/ω＼*)",
+    "不要再戳了(害怕ing)",
+    "还戳，哼(つд⊂)（生气）",
+    "再戳，小心我顺着网线找你.",
+    "咱要型气了o(>﹏<)o",
+    "嘿嘿，好舒服呀(bushi)",
+    "乖，好了好了，别戳了~",
+    "我爪巴爪巴，球球别再戳了",
+    "别再戳我了，行🐎？！",
+    "啊呜，你有什么事吗？",
+    "lsp你再戳？",
+    "连个可爱美少女都要戳的肥宅真恶心啊。",
+    "你再戳！",
+    "？再戳试试？",
+    "别戳了别戳了再戳就坏了555",
+    "我爪巴爪巴，球球别再戳了",
+    "你戳你🐎呢？！",
+    "放手啦，不给戳QAQ",
+    "戳坏了，赔钱！",
+    "戳坏了",
+    "嗯……不可以……啦……不要乱戳",
+    "那...那里...那里不能戳...绝对...",
+    "(。´・ω・)ん?",
+    "有事恁叫我，别天天一个劲戳戳戳！",
+    "欸很烦欸！你戳🔨呢",
+    "再戳一下试试？",
+    "正在关闭对您的所有服务...关闭成功",
+    "啊呜，太舒服刚刚竟然睡着了。什么事？",
+    "正在定位您的真实地址...定位成功。轰炸机已起飞"
 ]
```

### Comparing `nonebot_plugin_eventmonitor-0.1.3/setup.py` & `nonebot_plugin_eventmonitor-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot_plugin_eventmonitor",
-    version="0.1.3",
+    version="0.1.5",
     author="schwarzwald",
     description="监控群事件的插件，支持戳一戳，成员变动，群荣誉，运气王变化等提示",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Reversedeer/nonebot_plugin_eventmonitor",
     project_urls={
         "Bug Tracker": "https://github.com/Reversedeer/nonebot_plugin_eventmonitor/issues",
```

