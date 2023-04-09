# Comparing `tmp/nonebot_plugin_l4d2_server-0.4.5.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.4.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.4.6.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.4.5.tar` & `nonebot_plugin_l4d2_server-0.4.6.tar`

### file list

```diff
@@ -1,49 +1,48 @@
--rw-r--r--   0        0        0    35823 2023-01-11 11:22:12.357251 nonebot_plugin_l4d2_server-0.4.5/LICENSE
--rw-r--r--   0        0        0    16826 2023-04-09 05:48:47.180567 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0     8027 2023-04-08 18:50:15.782345 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/command.py
--rw-r--r--   0        0        0     4965 2023-04-08 18:09:47.583660 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/config.py
--rw-r--r--   0        0        0   158357 2023-01-08 15:05:11.765786 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-03-24 06:27:47.516852 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2022-11-27 13:06:53.317128 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1666 2023-03-06 09:04:41.376881 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-03-03 03:43:40.240633 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2150 2023-02-23 00:58:59.231306 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     5829 2023-03-01 12:23:49.342774 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/help - 副本.html
--rw-r--r--   0        0        0     6206 2023-03-05 16:25:01.648005 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6417 2023-02-27 15:03:03.981712 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1595 2023-03-02 15:28:44.743644 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     7874 2023-02-11 08:42:33.584146 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0     9067 2023-04-08 18:51:30.036612 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1661 2023-03-25 04:40:02.232501 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3085 2023-03-05 15:25:37.373454 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1702 2023-03-05 15:52:53.906753 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      376 2023-03-06 08:23:02.068422 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3332 2023-02-26 09:03:45.382934 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      485 2023-01-14 18:23:43.868353 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0     3308 2023-02-26 09:03:47.639393 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1316 2023-01-20 07:16:17.336574 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4197 2023-03-28 03:12:43.717423 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     4128 2023-03-18 17:22:46.673151 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4097 2023-02-11 08:44:48.430294 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1070 2023-02-06 23:05:41.006175 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0      968 2023-01-14 18:06:13.728698 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3882 2023-04-08 18:51:00.452792 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1427 2023-02-04 03:31:45.112442 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     3520 2023-04-08 12:57:15.592761 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1141 2023-04-08 18:08:59.052656 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0      741 2023-03-25 17:41:59.756270 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    10656 2023-04-08 15:58:37.818041 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1676 2023-02-19 10:27:01.909990 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0     1160 2023-02-17 18:42:54.854831 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1409 2023-03-02 15:06:19.826864 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     3397 2023-04-08 18:51:42.656361 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_web/config.py
--rw-r--r--   0        0        0     6336 2023-04-08 18:49:08.823312 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    10799 2023-04-08 18:36:09.768036 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1678 2023-02-26 09:29:05.903725 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/message.py
--rw-r--r--   0        0        0     1025 2023-03-05 15:52:53.333459 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/seach.py
--rw-r--r--   0        0        0     2166 2023-04-08 18:49:42.643806 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/txt_to_img.py
--rw-r--r--   0        0        0     8297 2023-04-09 05:43:10.168248 nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/utils.py
--rw-r--r--   0        0        0     1505 2023-04-09 05:47:40.005077 nonebot_plugin_l4d2_server-0.4.5/pyproject.toml
--rw-r--r--   0        0        0    10903 2023-04-09 05:48:40.831608 nonebot_plugin_l4d2_server-0.4.5/README.md
--rw-r--r--   0        0        0    12712 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.5/setup.py
--rw-r--r--   0        0        0    12573 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-01-11 11:22:12.357251 nonebot_plugin_l4d2_server-0.4.6/LICENSE
+-rw-r--r--   0        0        0    16832 2023-04-09 16:02:28.698025 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0     8027 2023-04-08 18:50:15.782345 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/command.py
+-rw-r--r--   0        0        0     4966 2023-04-09 16:00:29.769094 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/config.py
+-rw-r--r--   0        0        0   158357 2023-01-08 15:05:11.765786 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-03-24 06:27:47.516852 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2022-11-27 13:06:53.317128 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1650 2023-04-09 15:09:05.585642 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-03-03 03:43:40.240633 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2150 2023-02-23 00:58:59.231306 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6190 2023-04-09 15:09:04.151919 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6401 2023-04-09 15:09:04.937399 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1571 2023-04-09 15:08:29.280432 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     7874 2023-02-11 08:42:33.584146 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0     9067 2023-04-08 18:51:30.036612 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1661 2023-03-25 04:40:02.232501 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3085 2023-03-05 15:25:37.373454 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1702 2023-03-05 15:52:53.906753 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      376 2023-03-06 08:23:02.068422 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3332 2023-02-26 09:03:45.382934 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      485 2023-01-14 18:23:43.868353 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0     3308 2023-02-26 09:03:47.639393 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1316 2023-01-20 07:16:17.336574 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4197 2023-03-28 03:12:43.717423 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     4128 2023-03-18 17:22:46.673151 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4097 2023-02-11 08:44:48.430294 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1070 2023-02-06 23:05:41.006175 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0      968 2023-01-14 18:06:13.728698 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3882 2023-04-08 18:51:00.452792 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1427 2023-02-04 03:31:45.112442 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     3520 2023-04-08 12:57:15.592761 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1124 2023-04-09 15:06:02.337793 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0      741 2023-03-25 17:41:59.756270 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    10845 2023-04-09 15:59:41.750644 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1676 2023-02-19 10:27:01.909990 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0     1160 2023-02-17 18:42:54.854831 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1409 2023-03-02 15:06:19.826864 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     3397 2023-04-08 18:51:42.656361 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_web/config.py
+-rw-r--r--   0        0        0     6336 2023-04-08 18:49:08.823312 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    10799 2023-04-08 18:36:09.768036 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1678 2023-02-26 09:29:05.903725 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/message.py
+-rw-r--r--   0        0        0     1025 2023-03-05 15:52:53.333459 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/seach.py
+-rw-r--r--   0        0        0     2166 2023-04-08 18:49:42.643806 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/txt_to_img.py
+-rw-r--r--   0        0        0     8297 2023-04-09 05:43:10.168248 nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/utils.py
+-rw-r--r--   0        0        0     1505 2023-04-09 16:02:33.334787 nonebot_plugin_l4d2_server-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0    11317 2023-04-09 16:03:41.480929 nonebot_plugin_l4d2_server-0.4.6/README.md
+-rw-r--r--   0        0        0    13126 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.6/setup.py
+-rw-r--r--   0        0        0    12982 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.6/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.4.5/LICENSE` & `nonebot_plugin_l4d2_server-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     from .l4d2_web import web,webUI
 else:
     pass
 
 driver = get_driver()
 
 
-__version__ = "0.4.5"
+__version__ = "0.4.6"
 __plugin_meta__ = PluginMetadata(
     name="求生之路小助手",
     description='群内对有关求生之路的查询和操作',
     usage='求生服务器操作指令',
     extra={
         "version": __version__,
         "author": "Agnes4m <Z735803792@163.com>",
@@ -416,15 +416,15 @@
     await matcher.finish(mode_txt_to_img(mes,msg))
     
 @search_api.handle()
 async def _(matcher:Matcher,state:T_State,event:GroupMessageEvent,args:Message = CommandArg()):
     msg:str = args.extract_plain_text()
     # if msg.startswith('代码'):
         # 建图代码返回三方图信息
-    data = seach_map(msg,l4_qq,l4_key)
+    data = await seach_map(msg,l4_qq,l4_key)
     # else:
     if type(data) == str:
         await matcher.finish(data)
     else:
         state['maps'] = data
         await matcher.send(await map_dict_to_str(data))
```

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/command.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/command.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/config.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,169 +143,169 @@
 000008e0: 6967 2e6c 345f 7461 670d 0a65 7863 6570  ig.l4_tag..excep
 000008f0: 743a 0d0a 2020 2020 6c34 5f74 6167 203d  t:..    l4_tag =
 00000900: 204e 6f6e 650d 0a0d 0a74 7279 3a0d 0a20   None....try:.. 
 00000910: 2020 206c 345f 7765 623a 626f 6f6c 203d     l4_web:bool =
 00000920: 2064 7269 7665 722e 636f 6e66 6967 2e6c   driver.config.l
 00000930: 345f 7765 620d 0a65 7863 6570 743a 0d0a  4_web..except:..
 00000940: 2020 2020 6c34 5f77 6562 3a62 6f6f 6c20      l4_web:bool 
-00000950: 3d20 5472 7565 0d0a 2020 2020 0d0a 2320  = True..    ..# 
-00000960: e5bc bae5 88b6 e8bd ac6c 6973 740d 0a69  .........list..i
-00000970: 6620 7479 7065 286c 345f 7461 6729 203d  f type(l4_tag) =
-00000980: 3d20 7374 7220 6f72 206c 6973 743a 0d0a  = str or list:..
-00000990: 2020 2020 6c34 5f6c 6973 7420 3d20 5b6c      l4_list = [l
-000009a0: 345f 6669 6c65 2c20 6c34 5f73 7465 616d  4_file, l4_steam
-000009b0: 6964 2c20 6c34 5f68 6f73 742c 206c 345f  id, l4_host, l4_
-000009c0: 706f 7274 2c20 6c34 5f72 636f 6e2c 206c  port, l4_rcon, l
-000009d0: 345f 6d61 7374 6572 2c6c 345f 7461 675d  4_master,l4_tag]
-000009e0: 0d0a 2020 2020 6c34 5f6c 6973 7420 3d20  ..    l4_list = 
-000009f0: 5b61 7374 2e6c 6974 6572 616c 5f65 7661  [ast.literal_eva
-00000a00: 6c28 6929 2069 6620 6973 696e 7374 616e  l(i) if isinstan
-00000a10: 6365 2869 2c20 7374 7229 2065 6c73 6520  ce(i, str) else 
-00000a20: 6920 666f 7220 6920 696e 206c 345f 6c69  i for i in l4_li
-00000a30: 7374 5d0d 0a20 2020 206c 345f 6669 6c65  st]..    l4_file
-00000a40: 2c20 6c34 5f73 7465 616d 6964 2c20 6c34  , l4_steamid, l4
-00000a50: 5f68 6f73 742c 206c 345f 706f 7274 2c20  _host, l4_port, 
-00000a60: 6c34 5f72 636f 6e2c 206c 345f 6d61 7374  l4_rcon, l4_mast
-00000a70: 6572 2c20 6c34 5f74 6167 3d20 6c34 5f6c  er, l4_tag= l4_l
-00000a80: 6973 740d 0a65 6c73 653a 0d0a 2020 2020  ist..else:..    
-00000a90: 6c34 5f6c 6973 7420 3d20 5b6c 345f 6669  l4_list = [l4_fi
-00000aa0: 6c65 2c20 6c34 5f73 7465 616d 6964 2c20  le, l4_steamid, 
-00000ab0: 6c34 5f68 6f73 742c 206c 345f 706f 7274  l4_host, l4_port
-00000ac0: 2c20 6c34 5f72 636f 6e2c 206c 345f 6d61  , l4_rcon, l4_ma
-00000ad0: 7374 6572 5d0d 0a20 2020 206c 345f 6c69  ster]..    l4_li
-00000ae0: 7374 203d 205b 6173 742e 6c69 7465 7261  st = [ast.litera
-00000af0: 6c5f 6576 616c 2869 2920 6966 2069 7369  l_eval(i) if isi
-00000b00: 6e73 7461 6e63 6528 692c 2073 7472 2920  nstance(i, str) 
-00000b10: 656c 7365 2069 2066 6f72 2069 2069 6e20  else i for i in 
-00000b20: 6c34 5f6c 6973 745d 0d0a 2020 2020 6c34  l4_list]..    l4
-00000b30: 5f66 696c 652c 206c 345f 7374 6561 6d69  _file, l4_steami
-00000b40: 642c 206c 345f 686f 7374 2c20 6c34 5f70  d, l4_host, l4_p
-00000b50: 6f72 742c 206c 345f 7263 6f6e 2c20 6c34  ort, l4_rcon, l4
-00000b60: 5f6d 6173 7465 723d 206c 345f 6c69 7374  _master= l4_list
-00000b70: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00000b80: 2020 2020 2020 0d0a 2727 270d 0ae5 9cb0        ..'''.....
-00000b90: e59b bee8 b7af e5be 840d 0a27 2727 0d0a  ...........'''..
-00000ba0: 7670 6b5f 7061 7468 203d 2022 6c65 6674  vpk_path = "left
-00000bb0: 3464 6561 6432 2f61 6464 6f6e 7322 0d0a  4dead2/addons"..
-00000bc0: 2320 6d61 705f 7061 7468 203d 2050 6174  # map_path = Pat
-00000bd0: 6828 6c34 5f66 696c 655b 4348 4543 4b5f  h(l4_file[CHECK_
-00000be0: 4649 4c45 5d2c 7670 6b5f 7061 7468 290d  FILE],vpk_path).
-00000bf0: 0a23 206c 345f 6669 6c65 5f6f 6e65 203d  .# l4_file_one =
-00000c00: 206c 345f 6669 6c65 5b43 4845 434b 5f46   l4_file[CHECK_F
-00000c10: 494c 455d 0d0a 2320 6c34 5f68 6f73 745f  ILE]..# l4_host_
-00000c20: 6f6e 6520 3d20 6c34 5f68 6f73 745b 4348  one = l4_host[CH
-00000c30: 4543 4b5f 4649 4c45 5d0d 0a23 206c 345f  ECK_FILE]..# l4_
-00000c40: 706f 7274 5f6f 6e65 203d 2069 6e74 286c  port_one = int(l
-00000c50: 345f 706f 7274 5b43 4845 434b 5f46 494c  4_port[CHECK_FIL
-00000c60: 455d 290d 0a23 206c 345f 7263 6f6e 5f6f  E])..# l4_rcon_o
-00000c70: 6e65 203d 206c 345f 7263 6f6e 5b43 4845  ne = l4_rcon[CHE
-00000c80: 434b 5f46 494c 455d 0d0a 2320 6465 6620  CK_FILE]..# def 
-00000c90: 6c6f 6164 5f63 6f6e 6669 6728 293a 0d0a  load_config():..
-00000ca0: 2320 2020 2020 2320 e696 87e4 bbb6 e8b7  #     # ........
-00000cb0: afe5 be84 0d0a 2320 2020 2020 676c 6f62  ......#     glob
-00000cc0: 616c 206d 6170 5f70 6174 682c 6c34 5f66  al map_path,l4_f
-00000cd0: 696c 655f 6f6e 652c 6c34 5f68 6f73 745f  ile_one,l4_host_
-00000ce0: 6f6e 652c 6c34 5f70 6f72 745f 6f6e 652c  one,l4_port_one,
-00000cf0: 6c34 5f72 636f 6e5f 6f6e 650d 0a23 2020  l4_rcon_one..#  
-00000d00: 2020 206d 6170 5f70 6174 6820 3d20 5061     map_path = Pa
-00000d10: 7468 286c 345f 6669 6c65 5b43 4845 434b  th(l4_file[CHECK
-00000d20: 5f46 494c 455d 2c76 706b 5f70 6174 6829  _FILE],vpk_path)
-00000d30: 0d0a 2320 2020 2020 6c34 5f66 696c 655f  ..#     l4_file_
-00000d40: 6f6e 6520 3d20 6c34 5f66 696c 655b 4348  one = l4_file[CH
-00000d50: 4543 4b5f 4649 4c45 5d0d 0a23 2020 2020  ECK_FILE]..#    
-00000d60: 206c 345f 686f 7374 5f6f 6e65 203d 206c   l4_host_one = l
-00000d70: 345f 686f 7374 5b43 4845 434b 5f46 494c  4_host[CHECK_FIL
-00000d80: 455d 0d0a 2320 2020 2020 6c34 5f70 6f72  E]..#     l4_por
-00000d90: 745f 6f6e 6520 3d20 696e 7428 6c34 5f70  t_one = int(l4_p
-00000da0: 6f72 745b 4348 4543 4b5f 4649 4c45 5d29  ort[CHECK_FILE])
-00000db0: 0d0a 2320 2020 2020 6c34 5f72 636f 6e5f  ..#     l4_rcon_
-00000dc0: 6f6e 6520 3d20 6c34 5f72 636f 6e5b 4348  one = l4_rcon[CH
-00000dd0: 4543 4b5f 4649 4c45 5d0d 0a0d 0a0d 0a50  ECK_FILE]......P
-00000de0: 4c41 5945 5253 4441 5441 203d 2050 6174  LAYERSDATA = Pat
-00000df0: 6828 2920 2f20 2264 6174 612f 4c34 4432  h() / "data/L4D2
-00000e00: 2f69 6d61 6765 2f70 6c61 7965 7273 220d  /image/players".
-00000e10: 0a22 2222 e794 a8e6 88b7 e695 b0e6 8dae  ."""............
-00000e20: e8b7 afe5 be84 2222 220d 0a54 4558 545f  ......"""..TEXT_
-00000e30: 5041 5448 203d 2050 6174 6828 5f5f 6669  PATH = Path(__fi
-00000e40: 6c65 5f5f 292e 7061 7265 6e74 202f 2027  le__).parent / '
-00000e50: 6461 7461 2f4c 3444 322f 696d 6167 6527  data/L4D2/image'
-00000e60: 0d0a 2222 22e5 9bbe e789 87e5 ad98 e582  .."""...........
-00000e70: a8e8 b7af e5be 8422 2222 0d0a 5445 5854  ......."""..TEXT
-00000e80: 5f58 5041 5448 203d 2050 6174 6828 2920  _XPATH = Path() 
-00000e90: 2f20 2764 6174 612f 4c34 4432 2f69 6d61  / 'data/L4D2/ima
-00000ea0: 6765 270d 0a22 2222 e586 85e7 bdae e59b  ge'.."""........
-00000eb0: bee7 8987 e8b7 afe5 be84 2222 220d 0a0d  .........."""...
-00000ec0: 0a0d 0a0d 0a50 4c41 5945 5253 4441 5441  .....PLAYERSDATA
-00000ed0: 203d 2050 6174 6828 2920 2f20 2264 6174   = Path() / "dat
-00000ee0: 612f 4c34 4432 2f73 716c 220d 0a22 2222  a/L4D2/sql".."""
-00000ef0: e695 b0e6 8dae e5ba 93e8 b7af e5be 8422  ..............."
-00000f00: 2222 0d0a 4441 5441 5351 4c49 5445 203d  ""..DATASQLITE =
-00000f10: 2050 6174 6828 292e 7061 7265 6e74 202f   Path().parent /
-00000f20: 2022 6461 7461 2f4c 3444 322f 7371 6c2f   "data/L4D2/sql/
-00000f30: 4c34 4432 2e64 6222 0d0a 2222 22e6 95b0  L4D2.db".."""...
-00000f40: e68d aee5 ba93 efbc 8122 2222 2020 0d0a  ........."""  ..
-00000f50: 0d0a 7461 626c 655f 6461 7461 203d 205b  ..table_data = [
-00000f60: 224c 3464 325f 706c 6179 6572 7322 2c22  "L4d2_players","
-00000f70: 4c34 4432 5f73 6572 7665 7222 5d0d 0a22  L4D2_server"].."
-00000f80: 2222 e695 b0e6 8dae e5ba 93e8 a1a8 2222  ""............""
-00000f90: 220d 0a4c 3464 325f 706c 6179 6572 735f  "..L4d2_players_
-00000fa0: 7461 6720 3d20 5b27 7171 272c 2027 6e69  tag = ['qq', 'ni
-00000fb0: 636b 6e61 6d65 272c 2027 7374 6561 6d69  ckname', 'steami
-00000fc0: 6427 5d0d 0a22 2222 e695 b0e6 8dae e5ba  d'].."""........
-00000fd0: 93e8 a1a8 3122 2222 0d0a 4c34 6432 5f73  ....1"""..L4d2_s
-00000fe0: 6572 7665 725f 7461 6720 3d20 5b27 6964  erver_tag = ['id
-00000ff0: 272c 2771 7167 726f 7570 272c 2027 686f  ','qqgroup', 'ho
-00001000: 7374 272c 2027 706f 7274 272c 2027 7263  st', 'port', 'rc
-00001010: 6f6e 275d 0d0a 2222 22e6 95b0 e68d aee5  on']..""".......
-00001020: ba93 e8a1 a832 2222 220d 0a4c 3464 325f  .....2"""..L4d2_
-00001030: 494e 5445 4745 5220 3d20 5b27 6964 272c  INTEGER = ['id',
-00001040: 2771 7127 2c27 7171 6772 6f75 7027 2c27  'qq','qqgroup','
-00001050: 706f 7274 275d 0d0a 2222 2249 4e49 5445  port'].."""INITE
-00001060: 4745 52e7 9a84 e8a1 a8e5 a4b4 2222 220d  GER.........""".
-00001070: 0a4c 3464 325f 5445 5854 203d 205b 276e  .L4d2_TEXT = ['n
-00001080: 6963 6b6e 616d 6527 2c27 7374 6561 6d69  ickname','steami
-00001090: 6427 2c27 686f 7374 272c 2772 636f 6e27  d','host','rcon'
-000010a0: 2c27 7061 7468 275d 0d0a 2222 2254 4558  ,'path'].."""TEX
-000010b0: 54e7 9a84 e8a1 a8e5 a4b4 2222 220d 0a4c  T........."""..L
-000010c0: 3464 325f 424f 4f4c 4541 4e20 3d20 5b27  4d2_BOOLEAN = ['
-000010d0: 7573 6527 5d0d 0a22 2222 424f 4f4c 4541  use'].."""BOOLEA
-000010e0: 4ee7 9a84 e8a1 a8e5 a4b4 2222 220d 0a0d  N........."""...
-000010f0: 0a74 6162 6c65 735f 636f 6c75 6d6e 7320  .tables_columns 
-00001100: 3d20 7b0d 0a20 2020 2074 6162 6c65 5f64  = {..    table_d
-00001110: 6174 615b 305d 3a4c 3464 325f 706c 6179  ata[0]:L4d2_play
-00001120: 6572 735f 7461 672c 0d0a 2020 2020 7461  ers_tag,..    ta
-00001130: 626c 655f 6461 7461 5b31 5d3a 4c34 6432  ble_data[1]:L4d2
-00001140: 5f73 6572 7665 725f 7461 670d 0a7d 0d0a  _server_tag..}..
-00001150: 0d0a 2320 e6b1 82e7 949f 616e 6e65 e69c  ..# ......anne..
-00001160: 8de5 8aa1 e599 a80d 0a61 6e6e 655f 7572  .........anne_ur
-00001170: 6c20 3d20 2268 7474 7073 3a2f 2f73 6572  l = "https://ser
-00001180: 7665 722e 7472 7967 656b 2e63 6f6d 2f22  ver.trygek.com/"
-00001190: 0d0a 0d0a 6761 6d65 6d6f 6465 5f6c 6973  ....gamemode_lis
-000011a0: 7420 3d20 5b0d 0a20 2020 2027 e688 98e5  t = [..    '....
-000011b0: bdb9 272c 0d0a 2020 2020 27e5 a49a e789  ..',..    '.....
-000011c0: b927 2c0d 0a20 2020 2027 e586 99e4 b893  .',..    '......
-000011d0: 272c 0d0a 2020 2020 2761 6e6e 6527 2c0d  ',..    'anne',.
-000011e0: 0a20 2020 2027 e88d afe6 8a97 272c 0d0a  .    '......',..
-000011f0: 2020 2020 27e5 8c85 e68a 9727 2c0d 0a20      '......',.. 
-00001200: 2020 2027 e7bb 9de5 a283 272c 0d0a 2020     '......',..  
-00001210: 2020 27e6 adbb e4b8 9327 2c0d 0a20 2020    '......',..   
-00001220: 2027 6173 7427 2c0d 0a20 2020 2027 e6b8   'ast',..    '..
-00001230: 85e9 8193 e5a4 ab27 2c0d 0a5d 0d0a 0d0a  .......',..]....
-00001240: 2320 e7b3 bbe7 bb9f 0d0a 6966 2070 6c61  # ........if pla
-00001250: 7466 6f72 6d2e 7379 7374 656d 2829 203d  tform.system() =
-00001260: 3d20 2757 696e 646f 7773 273a 0d0a 2020  = 'Windows':..  
-00001270: 2020 7379 7374 656d 733a 7374 7220 3d20    systems:str = 
-00001280: 2777 696e 270d 0a65 6c69 6620 706c 6174  'win'..elif plat
-00001290: 666f 726d 2e73 7973 7465 6d28 2920 3d3d  form.system() ==
-000012a0: 2027 4c69 6e75 7827 3a0d 0a20 2020 2073   'Linux':..    s
-000012b0: 7973 7465 6d73 3a73 7472 203d 2027 6c69  ystems:str = 'li
-000012c0: 6e75 7827 0d0a 656c 7365 3a0d 0a20 2020  nux'..else:..   
-000012d0: 2073 7973 7465 6d73 3a73 7472 203d 2027   systems:str = '
-000012e0: 6f74 6865 7273 270d 0a41 4e4e 455f 4950  others'..ANNE_IP
-000012f0: 203d 207b 7d0d 0a0d 0a74 7279 3a0d 0a20   = {}....try:.. 
-00001300: 2020 206f 732e 7265 6d6f 7665 2850 6174     os.remove(Pat
-00001310: 6828 292e 7061 7265 6e74 2e6a 6f69 6e70  h().parent.joinp
-00001320: 6174 6828 2764 6174 612f 4c34 4432 2f6c  ath('data/L4D2/l
-00001330: 3464 322e 796d 6c27 2929 0d0a 6578 6365  4d2.yml'))..exce
-00001340: 7074 3a0d 0a20 2020 2070 6173 730d 0a20  pt:..    pass.. 
-00001350: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00001360: 2020 2020 20                                  
+00000950: 3d20 4661 6c73 650d 0a20 2020 200d 0a23  = False..    ..#
+00000960: 20e5 bcba e588 b6e8 bdac 6c69 7374 0d0a   .........list..
+00000970: 6966 2074 7970 6528 6c34 5f74 6167 2920  if type(l4_tag) 
+00000980: 3d3d 2073 7472 206f 7220 6c69 7374 3a0d  == str or list:.
+00000990: 0a20 2020 206c 345f 6c69 7374 203d 205b  .    l4_list = [
+000009a0: 6c34 5f66 696c 652c 206c 345f 7374 6561  l4_file, l4_stea
+000009b0: 6d69 642c 206c 345f 686f 7374 2c20 6c34  mid, l4_host, l4
+000009c0: 5f70 6f72 742c 206c 345f 7263 6f6e 2c20  _port, l4_rcon, 
+000009d0: 6c34 5f6d 6173 7465 722c 6c34 5f74 6167  l4_master,l4_tag
+000009e0: 5d0d 0a20 2020 206c 345f 6c69 7374 203d  ]..    l4_list =
+000009f0: 205b 6173 742e 6c69 7465 7261 6c5f 6576   [ast.literal_ev
+00000a00: 616c 2869 2920 6966 2069 7369 6e73 7461  al(i) if isinsta
+00000a10: 6e63 6528 692c 2073 7472 2920 656c 7365  nce(i, str) else
+00000a20: 2069 2066 6f72 2069 2069 6e20 6c34 5f6c   i for i in l4_l
+00000a30: 6973 745d 0d0a 2020 2020 6c34 5f66 696c  ist]..    l4_fil
+00000a40: 652c 206c 345f 7374 6561 6d69 642c 206c  e, l4_steamid, l
+00000a50: 345f 686f 7374 2c20 6c34 5f70 6f72 742c  4_host, l4_port,
+00000a60: 206c 345f 7263 6f6e 2c20 6c34 5f6d 6173   l4_rcon, l4_mas
+00000a70: 7465 722c 206c 345f 7461 673d 206c 345f  ter, l4_tag= l4_
+00000a80: 6c69 7374 0d0a 656c 7365 3a0d 0a20 2020  list..else:..   
+00000a90: 206c 345f 6c69 7374 203d 205b 6c34 5f66   l4_list = [l4_f
+00000aa0: 696c 652c 206c 345f 7374 6561 6d69 642c  ile, l4_steamid,
+00000ab0: 206c 345f 686f 7374 2c20 6c34 5f70 6f72   l4_host, l4_por
+00000ac0: 742c 206c 345f 7263 6f6e 2c20 6c34 5f6d  t, l4_rcon, l4_m
+00000ad0: 6173 7465 725d 0d0a 2020 2020 6c34 5f6c  aster]..    l4_l
+00000ae0: 6973 7420 3d20 5b61 7374 2e6c 6974 6572  ist = [ast.liter
+00000af0: 616c 5f65 7661 6c28 6929 2069 6620 6973  al_eval(i) if is
+00000b00: 696e 7374 616e 6365 2869 2c20 7374 7229  instance(i, str)
+00000b10: 2065 6c73 6520 6920 666f 7220 6920 696e   else i for i in
+00000b20: 206c 345f 6c69 7374 5d0d 0a20 2020 206c   l4_list]..    l
+00000b30: 345f 6669 6c65 2c20 6c34 5f73 7465 616d  4_file, l4_steam
+00000b40: 6964 2c20 6c34 5f68 6f73 742c 206c 345f  id, l4_host, l4_
+00000b50: 706f 7274 2c20 6c34 5f72 636f 6e2c 206c  port, l4_rcon, l
+00000b60: 345f 6d61 7374 6572 3d20 6c34 5f6c 6973  4_master= l4_lis
+00000b70: 7420 2020 2020 2020 2020 2020 200d 0a20  t            .. 
+00000b80: 2020 2020 2020 200d 0a27 2727 0d0a e59c         ..'''....
+00000b90: b0e5 9bbe e8b7 afe5 be84 0d0a 2727 270d  ............'''.
+00000ba0: 0a76 706b 5f70 6174 6820 3d20 226c 6566  .vpk_path = "lef
+00000bb0: 7434 6465 6164 322f 6164 646f 6e73 220d  t4dead2/addons".
+00000bc0: 0a23 206d 6170 5f70 6174 6820 3d20 5061  .# map_path = Pa
+00000bd0: 7468 286c 345f 6669 6c65 5b43 4845 434b  th(l4_file[CHECK
+00000be0: 5f46 494c 455d 2c76 706b 5f70 6174 6829  _FILE],vpk_path)
+00000bf0: 0d0a 2320 6c34 5f66 696c 655f 6f6e 6520  ..# l4_file_one 
+00000c00: 3d20 6c34 5f66 696c 655b 4348 4543 4b5f  = l4_file[CHECK_
+00000c10: 4649 4c45 5d0d 0a23 206c 345f 686f 7374  FILE]..# l4_host
+00000c20: 5f6f 6e65 203d 206c 345f 686f 7374 5b43  _one = l4_host[C
+00000c30: 4845 434b 5f46 494c 455d 0d0a 2320 6c34  HECK_FILE]..# l4
+00000c40: 5f70 6f72 745f 6f6e 6520 3d20 696e 7428  _port_one = int(
+00000c50: 6c34 5f70 6f72 745b 4348 4543 4b5f 4649  l4_port[CHECK_FI
+00000c60: 4c45 5d29 0d0a 2320 6c34 5f72 636f 6e5f  LE])..# l4_rcon_
+00000c70: 6f6e 6520 3d20 6c34 5f72 636f 6e5b 4348  one = l4_rcon[CH
+00000c80: 4543 4b5f 4649 4c45 5d0d 0a23 2064 6566  ECK_FILE]..# def
+00000c90: 206c 6f61 645f 636f 6e66 6967 2829 3a0d   load_config():.
+00000ca0: 0a23 2020 2020 2023 20e6 9687 e4bb b6e8  .#     # .......
+00000cb0: b7af e5be 840d 0a23 2020 2020 2067 6c6f  .......#     glo
+00000cc0: 6261 6c20 6d61 705f 7061 7468 2c6c 345f  bal map_path,l4_
+00000cd0: 6669 6c65 5f6f 6e65 2c6c 345f 686f 7374  file_one,l4_host
+00000ce0: 5f6f 6e65 2c6c 345f 706f 7274 5f6f 6e65  _one,l4_port_one
+00000cf0: 2c6c 345f 7263 6f6e 5f6f 6e65 0d0a 2320  ,l4_rcon_one..# 
+00000d00: 2020 2020 6d61 705f 7061 7468 203d 2050      map_path = P
+00000d10: 6174 6828 6c34 5f66 696c 655b 4348 4543  ath(l4_file[CHEC
+00000d20: 4b5f 4649 4c45 5d2c 7670 6b5f 7061 7468  K_FILE],vpk_path
+00000d30: 290d 0a23 2020 2020 206c 345f 6669 6c65  )..#     l4_file
+00000d40: 5f6f 6e65 203d 206c 345f 6669 6c65 5b43  _one = l4_file[C
+00000d50: 4845 434b 5f46 494c 455d 0d0a 2320 2020  HECK_FILE]..#   
+00000d60: 2020 6c34 5f68 6f73 745f 6f6e 6520 3d20    l4_host_one = 
+00000d70: 6c34 5f68 6f73 745b 4348 4543 4b5f 4649  l4_host[CHECK_FI
+00000d80: 4c45 5d0d 0a23 2020 2020 206c 345f 706f  LE]..#     l4_po
+00000d90: 7274 5f6f 6e65 203d 2069 6e74 286c 345f  rt_one = int(l4_
+00000da0: 706f 7274 5b43 4845 434b 5f46 494c 455d  port[CHECK_FILE]
+00000db0: 290d 0a23 2020 2020 206c 345f 7263 6f6e  )..#     l4_rcon
+00000dc0: 5f6f 6e65 203d 206c 345f 7263 6f6e 5b43  _one = l4_rcon[C
+00000dd0: 4845 434b 5f46 494c 455d 0d0a 0d0a 0d0a  HECK_FILE]......
+00000de0: 504c 4159 4552 5344 4154 4120 3d20 5061  PLAYERSDATA = Pa
+00000df0: 7468 2829 202f 2022 6461 7461 2f4c 3444  th() / "data/L4D
+00000e00: 322f 696d 6167 652f 706c 6179 6572 7322  2/image/players"
+00000e10: 0d0a 2222 22e7 94a8 e688 b7e6 95b0 e68d  .."""...........
+00000e20: aee8 b7af e5be 8422 2222 0d0a 5445 5854  ......."""..TEXT
+00000e30: 5f50 4154 4820 3d20 5061 7468 285f 5f66  _PATH = Path(__f
+00000e40: 696c 655f 5f29 2e70 6172 656e 7420 2f20  ile__).parent / 
+00000e50: 2764 6174 612f 4c34 4432 2f69 6d61 6765  'data/L4D2/image
+00000e60: 270d 0a22 2222 e59b bee7 8987 e5ad 98e5  '.."""..........
+00000e70: 82a8 e8b7 afe5 be84 2222 220d 0a54 4558  ........"""..TEX
+00000e80: 545f 5850 4154 4820 3d20 5061 7468 2829  T_XPATH = Path()
+00000e90: 202f 2027 6461 7461 2f4c 3444 322f 696d   / 'data/L4D2/im
+00000ea0: 6167 6527 0d0a 2222 22e5 8685 e7bd aee5  age'..""".......
+00000eb0: 9bbe e789 87e8 b7af e5be 8422 2222 0d0a  ..........."""..
+00000ec0: 0d0a 0d0a 0d0a 504c 4159 4552 5344 4154  ......PLAYERSDAT
+00000ed0: 4120 3d20 5061 7468 2829 202f 2022 6461  A = Path() / "da
+00000ee0: 7461 2f4c 3444 322f 7371 6c22 0d0a 2222  ta/L4D2/sql"..""
+00000ef0: 22e6 95b0 e68d aee5 ba93 e8b7 afe5 be84  "...............
+00000f00: 2222 220d 0a44 4154 4153 514c 4954 4520  """..DATASQLITE 
+00000f10: 3d20 5061 7468 2829 2e70 6172 656e 7420  = Path().parent 
+00000f20: 2f20 2264 6174 612f 4c34 4432 2f73 716c  / "data/L4D2/sql
+00000f30: 2f4c 3444 322e 6462 220d 0a22 2222 e695  /L4D2.db".."""..
+00000f40: b0e6 8dae e5ba 93ef bc81 2222 2220 200d  .........."""  .
+00000f50: 0a0d 0a74 6162 6c65 5f64 6174 6120 3d20  ...table_data = 
+00000f60: 5b22 4c34 6432 5f70 6c61 7965 7273 222c  ["L4d2_players",
+00000f70: 224c 3444 325f 7365 7276 6572 225d 0d0a  "L4D2_server"]..
+00000f80: 2222 22e6 95b0 e68d aee5 ba93 e8a1 a822  """............"
+00000f90: 2222 0d0a 4c34 6432 5f70 6c61 7965 7273  ""..L4d2_players
+00000fa0: 5f74 6167 203d 205b 2771 7127 2c20 276e  _tag = ['qq', 'n
+00000fb0: 6963 6b6e 616d 6527 2c20 2773 7465 616d  ickname', 'steam
+00000fc0: 6964 275d 0d0a 2222 22e6 95b0 e68d aee5  id']..""".......
+00000fd0: ba93 e8a1 a831 2222 220d 0a4c 3464 325f  .....1"""..L4d2_
+00000fe0: 7365 7276 6572 5f74 6167 203d 205b 2769  server_tag = ['i
+00000ff0: 6427 2c27 7171 6772 6f75 7027 2c20 2768  d','qqgroup', 'h
+00001000: 6f73 7427 2c20 2770 6f72 7427 2c20 2772  ost', 'port', 'r
+00001010: 636f 6e27 5d0d 0a22 2222 e695 b0e6 8dae  con'].."""......
+00001020: e5ba 93e8 a1a8 3222 2222 0d0a 4c34 6432  ......2"""..L4d2
+00001030: 5f49 4e54 4547 4552 203d 205b 2769 6427  _INTEGER = ['id'
+00001040: 2c27 7171 272c 2771 7167 726f 7570 272c  ,'qq','qqgroup',
+00001050: 2770 6f72 7427 5d0d 0a22 2222 494e 4954  'port'].."""INIT
+00001060: 4547 4552 e79a 84e8 a1a8 e5a4 b422 2222  EGER........."""
+00001070: 0d0a 4c34 6432 5f54 4558 5420 3d20 5b27  ..L4d2_TEXT = ['
+00001080: 6e69 636b 6e61 6d65 272c 2773 7465 616d  nickname','steam
+00001090: 6964 272c 2768 6f73 7427 2c27 7263 6f6e  id','host','rcon
+000010a0: 272c 2770 6174 6827 5d0d 0a22 2222 5445  ','path'].."""TE
+000010b0: 5854 e79a 84e8 a1a8 e5a4 b422 2222 0d0a  XT........."""..
+000010c0: 4c34 6432 5f42 4f4f 4c45 414e 203d 205b  L4d2_BOOLEAN = [
+000010d0: 2775 7365 275d 0d0a 2222 2242 4f4f 4c45  'use'].."""BOOLE
+000010e0: 414e e79a 84e8 a1a8 e5a4 b422 2222 0d0a  AN........."""..
+000010f0: 0d0a 7461 626c 6573 5f63 6f6c 756d 6e73  ..tables_columns
+00001100: 203d 207b 0d0a 2020 2020 7461 626c 655f   = {..    table_
+00001110: 6461 7461 5b30 5d3a 4c34 6432 5f70 6c61  data[0]:L4d2_pla
+00001120: 7965 7273 5f74 6167 2c0d 0a20 2020 2074  yers_tag,..    t
+00001130: 6162 6c65 5f64 6174 615b 315d 3a4c 3464  able_data[1]:L4d
+00001140: 325f 7365 7276 6572 5f74 6167 0d0a 7d0d  2_server_tag..}.
+00001150: 0a0d 0a23 20e6 b182 e794 9f61 6e6e 65e6  ...# ......anne.
+00001160: 9c8d e58a a1e5 99a8 0d0a 616e 6e65 5f75  ..........anne_u
+00001170: 726c 203d 2022 6874 7470 733a 2f2f 7365  rl = "https://se
+00001180: 7276 6572 2e74 7279 6765 6b2e 636f 6d2f  rver.trygek.com/
+00001190: 220d 0a0d 0a67 616d 656d 6f64 655f 6c69  "....gamemode_li
+000011a0: 7374 203d 205b 0d0a 2020 2020 27e6 8898  st = [..    '...
+000011b0: e5bd b927 2c0d 0a20 2020 2027 e5a4 9ae7  ...',..    '....
+000011c0: 89b9 272c 0d0a 2020 2020 27e5 8699 e4b8  ..',..    '.....
+000011d0: 9327 2c0d 0a20 2020 2027 616e 6e65 272c  .',..    'anne',
+000011e0: 0d0a 2020 2020 27e8 8daf e68a 9727 2c0d  ..    '......',.
+000011f0: 0a20 2020 2027 e58c 85e6 8a97 272c 0d0a  .    '......',..
+00001200: 2020 2020 27e7 bb9d e5a2 8327 2c0d 0a20      '......',.. 
+00001210: 2020 2027 e6ad bbe4 b893 272c 0d0a 2020     '......',..  
+00001220: 2020 2761 7374 272c 0d0a 2020 2020 27e6    'ast',..    '.
+00001230: b885 e981 93e5 a4ab 272c 0d0a 5d0d 0a0d  ........',..]...
+00001240: 0a23 20e7 b3bb e7bb 9f0d 0a69 6620 706c  .# ........if pl
+00001250: 6174 666f 726d 2e73 7973 7465 6d28 2920  atform.system() 
+00001260: 3d3d 2027 5769 6e64 6f77 7327 3a0d 0a20  == 'Windows':.. 
+00001270: 2020 2073 7973 7465 6d73 3a73 7472 203d     systems:str =
+00001280: 2027 7769 6e27 0d0a 656c 6966 2070 6c61   'win'..elif pla
+00001290: 7466 6f72 6d2e 7379 7374 656d 2829 203d  tform.system() =
+000012a0: 3d20 274c 696e 7578 273a 0d0a 2020 2020  = 'Linux':..    
+000012b0: 7379 7374 656d 733a 7374 7220 3d20 276c  systems:str = 'l
+000012c0: 696e 7578 270d 0a65 6c73 653a 0d0a 2020  inux'..else:..  
+000012d0: 2020 7379 7374 656d 733a 7374 7220 3d20    systems:str = 
+000012e0: 276f 7468 6572 7327 0d0a 414e 4e45 5f49  'others'..ANNE_I
+000012f0: 5020 3d20 7b7d 0d0a 0d0a 7472 793a 0d0a  P = {}....try:..
+00001300: 2020 2020 6f73 2e72 656d 6f76 6528 5061      os.remove(Pa
+00001310: 7468 2829 2e70 6172 656e 742e 6a6f 696e  th().parent.join
+00001320: 7061 7468 2827 6461 7461 2f4c 3444 322f  path('data/L4D2/
+00001330: 6c34 6432 2e79 6d6c 2729 290d 0a65 7863  l4d2.yml'))..exc
+00001340: 6570 743a 0d0a 2020 2020 7061 7373 0d0a  ept:..    pass..
+00001350: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00001360: 2020 2020 2020
```

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files 1% similar despite different names*

```diff
@@ -49,12 +49,12 @@
 		</tbody>
 	</table>
 </div>
 <font color="yellow">
 {% endfor %}
 <h5><center>©爱丽数码</center></br>
 	<center>
-		github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server
+		github.com/Agnes4m/nonebot_plugin_l4d2_server
 	</center>
 </h5>
 </font>
 </body>
```

#### html2text {}

```diff
@@ -12,8 +12,8 @@
                   {item.point_min}}
                   ç&emsp;&emsp;å¤´ | { ç  å¤´  ç | {{item.out}}
                   {item.shut}}
                   æ¸¸ç©æ¬¡æ° | { æ  æ´  å³ | {
                   {item.playtimes}}            {item.last_one}}
 {% endfor %}
                                 Â©ç±ä¸½æ°ç 
-         github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server
+                 github.com/Agnes4m/nonebot_plugin_l4d2_server
```

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/help - 副本.html` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,123 +1,121 @@
 <html>
   <head>
-<style>
-  body {
-    margin: 0px;
-    zoom: 150%;
-    background-color: #F7D04B;
-  }
-  .image {
-    display: flex;
-    flex-direction: column;
-    overflow: scroll;
-    width: max-content;
-    padding: 20px;
-  }
-  .head {
-    display: flex;
-    flex-direction: row;
-    align-items: center;
-    justify-content: space-between;
-    background-color: #F5D76E;
-    padding-left: 20px;
-    padding-right: 20px;
-    padding-top: 10px;
-    padding-bottom: 10px;
-    border: 2px solid;
-    border-radius: 50px;
-    border-color: #F1C40F;
-    font-size: 16px;
-    margin-bottom: 20px;
-  }
+    <style>
+      body {
+        margin: 0px;
+        zoom: 150%;
+      }
+      .image {
+        display: flex;
+        flex-direction: column;
+        overflow: scroll;
+        width: max-content;
+        padding: 20px;
+      }
+      .head {
+        display: flex;
+        flex-direction: row;
+        align-items: center;
+        justify-content: space-between;
+        background-color: #f5f6f7;
+        padding-left: 20px;
+        padding-right: 20px;
+        padding-top: 10px;
+        padding-bottom: 10px;
+        border: 2px solid;
+        border-radius: 50px;
+        border-color: #e5e7eb;
+        font-size: 16px;
+        margin-bottom: 20px;
+      }
 
-  .plugins {
-    display: grid;
-    grid-template-columns: auto auto auto;
-    row-gap: 20px;
-    column-gap: 20px;
-    margin-bottom: 20px;
-  }
-  .plugin {
-    display: flex;
-    padding: 5px;
-    border: 1px solid;
-    border-radius: 5px;
-    border-color: #F1C40F;
-    box-shadow: 0px 2px 6px 1px rgba(0, 0, 0, 0.2);
-    background-color: #F7D04B;
-  }
-  .plugin_meta {
-    display: flex;
-    flex-direction: column;
-    padding: 5px;
-    width: 250px;
-    justify-content: space-between;
-  }
-  .plugin_name {
-    font-size: 20px;
-    color: #F1C40F;
-  }
-  .plugin_description {
-    font-size: 15px;
-    color: gray;
-    margin-top: 5px;
-    margin-bottom: 5px;
-  }
-  .plugin_meta_line1 {
-    display: flex;
-    flex-direction: row;
-    align-items: center;
-    justify-content: space-between;
-  }
-  .plugin_meta_line3 {
-    display: flex;
-    flex-direction: row;
-    align-items: center;
-  }
-  .package_name_label {
-    background-image: url(./fingerprint.svg);
-    width: 13px;
-    height: 13px;
-    margin-right: 8px;
-  }
-  .package_name {
-    font-size: 13px;
-    color: gray;
-  }
-  .switch {
-    position: relative;
-    display: inline-block;
-    width: 40px;
-    height: 24px;
-  }
-  .slider {
-    position: absolute;
-    cursor: pointer;
-    top: 0;
-    left: 0;
-    right: 0;
-    bottom: 0;
-    background-color: #ccc;
-  }
-  .slider:before {
-    position: absolute;
-    content: "";
-    height: 16px;
-    width: 16px;
-    left: 4px;
-    bottom: 4px;
-    background-color: white;
-  }
-  .switch input {
-    display: none;
-  }
-  .switch input:checked + .slider {
-    background-color: rgba(86, 40, 238, 0.5);
-  }
+      .plugins {
+        display: grid;
+        grid-template-columns: auto auto auto;
+        row-gap: 20px;
+        column-gap: 20px;
+		margin-bottom: 20px;
+      }
+      .plugin {
+        display: flex;
+        padding: 5px;
+        border: 1px solid;
+        border-radius: 5px;
+        border-color: #e5e7eb;
+        box-shadow: 0px 2px 6px 1px rgba(0, 0, 0, 0.2);
+        background-color: #f5f6f7;
+      }
+      .plugin_meta {
+        display: flex;
+        flex-direction: column;
+        padding: 5px;
+        width: 250px;
+        justify-content: space-between;
+      }
+      .plugin_name {
+        font-size: 20px;
+      }
+      .plugin_description {
+        font-size: 15px;
+        color: gray;
+        margin-top: 5px;
+        margin-bottom: 5px;
+      }
+      .plugin_meta_line1 {
+        display: flex;
+        flex-direction: row;
+        align-items: center;
+        justify-content: space-between;
+      }
+      .plugin_meta_line3 {
+        display: flex;
+        flex-direction: row;
+        align-items: center;
+      }
+      .package_name_label {
+        background-image: url(./fingerprint.svg);
+        width: 13px;
+        height: 13px;
+        margin-right: 8px;
+      }
+      .package_name {
+        font-size: 13px;
+        color: gray;
+      }
+      .switch {
+        position: relative;
+        display: inline-block;
+        width: 40px;
+        height: 24px;
+      }
+      .slider {
+        position: absolute;
+        cursor: pointer;
+        top: 0;
+        left: 0;
+        right: 0;
+        bottom: 0;
+        background-color: #ccc;
+      }
+      .slider:before {
+        position: absolute;
+        content: "";
+        height: 16px;
+        width: 16px;
+        left: 4px;
+        bottom: 4px;
+        background-color: white;
+      }
+      .switch input {
+        display: none;
+      }
+      .switch input:checked + .slider {
+        background-color: rgba(86, 40, 238, 0.5);
+      }
       .switch input:checked + .slider:before {
         -webkit-transform: translateX(16px);
         -ms-transform: translateX(16px);
         transform: translateX(16px);
       }
       .slider.round {
         border-radius: 24px;
@@ -218,15 +216,15 @@
             </div>
           </div>
         </div>
         {% endfor %}
       </div>
 	  <div class="head">
       <span><b>©爱丽数码</b></span>
-      <span>https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server</span>
+      <span>github.com/Agnes4m/nonebot_plugin_l4d2_server</span>
       </div>
     </div>
 </html>
   </body>
```

#### html2text {}

```diff
@@ -4,9 +4,8 @@
 
 % if plugin.enabled %} checked {% endif %} />
 {{ plugin.map_ }}
 {% for Player in plugin.Players %} {{ Player }}
 {% endfor %}
 {{ plugin.max_players }}
 {% endfor %}
-Â©ç±ä¸½æ°ç  https://github.com/Umamusume-Agnes-Digital/
-nonebot_plugin_l4d2_server
+Â©ç±ä¸½æ°ç  github.com/Agnes4m/nonebot_plugin_l4d2_server
```

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 <html>
   <head>
     <style>
       body {
         margin: 0px;
         zoom: 150%;
+        background-color: #0D1117;
       }
       .image {
         display: flex;
         flex-direction: column;
         overflow: scroll;
         width: max-content;
         padding: 20px;
       }
       .head {
         display: flex;
         flex-direction: row;
         align-items: center;
         justify-content: space-between;
-        background-color: #f5f6f7;
+        background-color: #161B22;
         padding-left: 20px;
         padding-right: 20px;
         padding-top: 10px;
         padding-bottom: 10px;
         border: 2px solid;
         border-radius: 50px;
-        border-color: #e5e7eb;
+        border-color: #1a1a1a;
         font-size: 16px;
         margin-bottom: 20px;
       }
 
       .plugins {
         display: grid;
         grid-template-columns: auto auto auto;
@@ -37,17 +38,17 @@
 		margin-bottom: 20px;
       }
       .plugin {
         display: flex;
         padding: 5px;
         border: 1px solid;
         border-radius: 5px;
-        border-color: #e5e7eb;
+        border-color: #161B22;
         box-shadow: 0px 2px 6px 1px rgba(0, 0, 0, 0.2);
-        background-color: #f5f6f7;
+        background-color: #1a1a1a;
       }
       .plugin_meta {
         display: flex;
         flex-direction: column;
         padding: 5px;
         width: 250px;
         justify-content: space-between;
@@ -106,15 +107,15 @@
         bottom: 4px;
         background-color: white;
       }
       .switch input {
         display: none;
       }
       .switch input:checked + .slider {
-        background-color: rgba(86, 40, 238, 0.5);
+        background-color: rgba(46, 160, 67);
       }
       .switch input:checked + .slider:before {
         -webkit-transform: translateX(16px);
         -ms-transform: translateX(16px);
         transform: translateX(16px);
       }
       .slider.round {
@@ -182,49 +183,49 @@
         visibility: inherit;
       }
     </style>
   </head>
   <body>
     <div class="image">
       <div class="head">
-        <span><b>已加载服务器</b></span>
-        <span>发送 “<b>服务器昵称/序号</b>” 查看详情</span>
+        <span><b><font color="Silver">已加载服务器</font></b></span>
+        <span><font color="Silver">发送“<b>服务器昵称/序号</b>”查看详情</font></span>
       </div>
       <div class="plugins">
         {% for plugin in plugins %}
         <div class="plugin">
           <div class="plugin_meta">
             <div class="plugin_meta_line1">
-              <div class="plugin_name">{{ plugin.number }}:{{ plugin.name }}</div>
+              <div class="plugin_name"><font color="DeepSkyBlue">{{ plugin.number }}:{{ plugin.name }}</font></div>
               <div class="plugin_status">
                 <label class="switch">
                   <input class="checkbox" type="checkbox" {% if plugin.enabled %} checked {% endif %} />
                   <span class="slider round {% if plugin.locked %} locked {% endif %}">
                     <span class="lock {% if plugin.locked %} locked {% endif %}"></span>
                   </span>
                 </label>
               </div>
             </div>
             <div class="plugin_meta_line2">
-				<font color="blue">{{ plugin.map_ }}</font><br>
+				<font color="LightSkyBlue">{{ plugin.map_ }}</font><br>
                 {% for Player in plugin.Players %}
-                    <font color="green">{{ Player }}</font><br>
+                    <font color="LightGray">{{ Player }}</font><br>
                 {% endfor %}
             </div>
             <div class="plugin_meta_line3">
               <div class="package_name_label"></div>
-              <div class="package_name">{{ plugin.max_players }}</div>
+              <div class="package_name"><font color="LightGray">{{ plugin.max_players }}</font></div>
             </div>
           </div>
         </div>
         {% endfor %}
       </div>
 	  <div class="head">
-      <span><b>©爱丽数码</b></span>
-      <span>github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server</span>
+      <span><b><font color="Silver">©爱丽数码</font></b></span>
+      <span><font color="Silver">github*Agnes4m</font></span>
       </div>
     </div>
-</html>
   </body>
+</html>
+  
 
-
-
+/*暗黑风格-ArcPav*/
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
-å·²å è½½æå¡å¨ åé âæå¡å¨æµç§°/åºå·â æ¥çè¯¦æ
+å·²å è½½æå¡å¨ åéâæå¡å¨æµç§°/åºå·âæ¥çè¯¦æ
 {% for plugin in plugins %}
 {{ plugin.number }}:{{ plugin.name }}
 
 % if plugin.enabled %} checked {% endif %} />
 {{ plugin.map_ }}
 {% for Player in plugin.Players %} {{ Player }}
 {% endfor %}
 {{ plugin.max_players }}
 {% endfor %}
-Â©ç±ä¸½æ°ç  github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server
+Â©ç±ä¸½æ°ç  github*Agnes4m
+/*æé»é£æ ¼-ArcPav*/
```

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files 19% similar despite different names*

```diff
@@ -38,12 +38,12 @@
                 {% endif %}
             {% endfor %}
         </tr>
     {% endfor %}
 </table>
 <h5><center>©爱丽数码</center></br>
 	<center>
-		https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server
+		github.com/Agnes4m/nonebot_plugin_l4d2_server
 	</center>
 </h5>
 </div>
 </html>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
 {{ data[j].number }}
 {{ data[j].name }}
 {{ data[j].ip }}
 {{ data[j].map_ }}
 {% for Player in data[j].Players %} {{ Player }}
 {% endfor %} {{ data[j].max_players }}{{data[j].ping}}
                                 Â©ç±ä¸½æ°ç 
-     https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server
+                 github.com/Agnes4m/nonebot_plugin_l4d2_server
```

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,13 @@
     elif mode == 'first':
         ip_tag:list = file.json()
         return ip_tag
         
 
 async def map_dict_to_str(data:List[dict]):
     msg = ""
-    print(data)
     for key,value in data[0].items():
         if key == "url":
             continue
         msg += f"{key}:{value}\n"
     return msg
```

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,16 +64,17 @@
                 number, qqgroup, host, port = i
             finally:
                 # 将异步任务添加到任务列表中
                 tasks.append(asyncio.create_task(process_message(number, host, port, msg_list,qqgroup)))
         # 等待所有异步任务完成
         await asyncio.gather(*tasks)
         # 对msg_list按照number顺序排序
-        msg_list = sorted(msg_list, key=lambda x: x['number'])
+        msg_list.sort(key=lambda x: x['number'])
         result = {'msg_list': msg_list}
+
     else:
         result = {}
     return result
 
 
 async def qq_ip_queries_pic(msg: list):
     result = await qq_ip_querie(msg)
@@ -91,15 +92,18 @@
         msg2 = await player_queries_anne_dict(host, port)
         msg1 = await queries_dict(host, port)
         msg1.update({'Players':msg2,'number':number,})
         if qqgroup:
             msg1.update({'tag':qqgroup})
         msg_list.append(msg1)
     except errors:
-        pass  # 忽略异常，继续下一次循环
+        # 空白字典
+        null_dict = {key: 'null' for key in ['name', 'map_', 'players', 'max_players', 'rank_players', 'ping']}
+        null_dict.update({'number':number,'ip':f'{host}:{port}','Players':[]})
+        msg_list.append(null_dict)  
 
 
     
 async def get_tan_jian(msg:List[tuple],mode:int):
     """获取anne列表抽一个"""
     msg_list = []
     random.shuffle(msg)
```

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_web/config.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_web/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/message.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/seach.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/txt_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/nonebot_plugin_l4d2_server/utils.py` & `nonebot_plugin_l4d2_server-0.4.6/nonebot_plugin_l4d2_server/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.5/pyproject.toml` & `nonebot_plugin_l4d2_server-0.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.4.5"
+version = "0.4.6"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_l4d2_server-0.4.5/README.md` & `nonebot_plugin_l4d2_server-0.4.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -32,21 +32,20 @@
     <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">
 </div>
 
 
 ## 快速使用（env示例）
     # 复制到env文件里，没有默认就是下列值，如需修改安装下面env设置
     # 所有的多选，用逗号隔开
-    l4_master = ['1145149191']
-    l4_file = ['/home/ubuntu/l4d2/coop']
-    l4_host = ['127.0.0.1']
-    l4_port = ['20715']
-    l4_rcon = ['1145149191810']
-    l4_font = 'simsun.ttc'
-    l4_only = True
+    l4_master = ['1145149191']            # 允许上传地图的qq号
+    l4_file = ['/home/ubuntu/l4d2/coop']  # 本地服务器路径
+    l4_host = ['127.0.0.1']               # 服务器ip（建议内网，公网也可以）
+    l4_port = ['20715']                   # 服务器端口
+    l4_rcon = ['1145149191810']           # 服务器rcon密码，如果没有可以列空str对象元素
+    l4_font = 'simsun.ttc'                # 服务器字体
 
 
 ## 新文档（暂未完成）
 
 [点击这里](https://Agnes4m.github.io/l4d2)
 
 <h2 id="gn">主要功能</h2>
@@ -92,30 +91,36 @@
 
 <h2 id="ty">🌐 默认服务器</h2>
 目前 **已授权** 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主
 
 | 指令 | 服务器 | op | 数量 |
 |:-----:|:----:|:----:|:----:|
 | 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 3
-| 云 | anne电信服云服 | 东 | 25
-| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15
-| 橘 | 橘希实香的小窝 | 橘希实香 | 13
-| 竹 | 竹烨 | 竹烨oО柠檬茶 | 9
+| 云 | anne电信服云服 | 东 | 27
+| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 14
+| 橘 | 橘希实香的小窝 | 橘希实香 | 14
+| 竹 | 竹烨 | 竹烨oО柠檬茶 | 6
 | 音理 | 星空列车与白的旅行 | 音理 | 3
 | 尤 | 尤尤 | 晓音 | 3
 | 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3
 | 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 1
 | Air | Air | Air | 15
+| 3ks | 为人民服务 | DK | 14
 
 
 ## 🔖 更新日志
 
 <details>
 <summary>展开/收起</summary>
 
+### 0.4.6--2022.4.9
+
+ - 显示无效服
+ - 优化服务器排序算法（list.sort()天下第一）
+ - 默认关闭web端
 
 ### 0.4.5--2022.4.9
 
 - 修bug（恼）
 
 ### 0.4.2--2022.4.9
```

#### html2text {}

```diff
@@ -3,18 +3,22 @@
    # nonebot_plugin_l4d2_server _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
                 ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
 
 [GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
                                    [NoneBot]
 ## å¿«éä½¿ç¨ï¼envç¤ºä¾ï¼ #
 å¤å¶å°envæä»¶éï¼æ²¡æé»è®¤å°±æ¯ä¸åå¼ï¼å¦éä¿®æ¹å®è£ä¸é¢envè®¾ç½®
-# ææçå¤éï¼ç¨éå·éå¼ l4_master = ['1145149191'] l4_file = ['/
-home/ubuntu/l4d2/coop'] l4_host = ['127.0.0.1'] l4_port = ['20715'] l4_rcon =
-['1145149191810'] l4_font = 'simsun.ttc' l4_only = True ##
-æ°ææ¡£ï¼ææªå®æï¼ [ç¹å»è¿é](https://Agnes4m.github.io/l4d2)
+# ææçå¤éï¼ç¨éå·éå¼ l4_master = ['1145149191'] #
+åè®¸ä¸ä¼ å°å¾çqqå· l4_file = ['/home/ubuntu/l4d2/coop'] #
+æ¬å°æå¡å¨è·¯å¾ l4_host = ['127.0.0.1'] #
+æå¡å¨ipï¼å»ºè®®åç½ï¼å¬ç½ä¹å¯ä»¥ï¼ l4_port = ['20715'] #
+æå¡å¨ç«¯å£ l4_rcon = ['1145149191810'] #
+æå¡å¨rconå¯ç ï¼å¦ææ²¡æå¯ä»¥åç©ºstrå¯¹è±¡åç´  l4_font =
+'simsun.ttc' # æå¡å¨å­ä½ ## æ°ææ¡£ï¼ææªå®æï¼ [ç¹å»è¿é]
+(https://Agnes4m.github.io/l4d2)
 ***** ä¸»è¦åè½ *****
 - æ±çæå¡å¨-æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶ -
 åæå·¥åä¸è½½åå·æ¼å¶ä½ - [æ±ççµä¿¡æanne](https://github.com/
 fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/l4d_stats/
 ranking/index.php)
 ***** å¦ä½è·åkey *****
@@ -31,22 +35,24 @@
 æ°å¢ä¸ä¸ªjsonæä»¶ï¼æ ¼å¼å¦ä¸,æä»¶åä¸éè¦ååºçæä»¤ä¸è´
 { "åå": [ { "id": 1, "version": "æå½¹", "ip": "43.248.188.17:27031" } ] }
 ***** ð é»è®¤æå¡å¨ *****
 ç®å **å·²ææ**
 çæå¡å¨æ¥è¯¢ï¼å¦æéè¦å å¥èªå·±çipå¯ä»¥è¿qqç¾¤ç§èç¾¤ä¸» |
 æä»¤ | æå¡å¨ | op | æ°é | |:-----:|:----:|:----:|:----:| | æ°ç  |
 ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 3 | äº | anneçµä¿¡æäºæ | ä¸ |
-25 | åå | ååçå°çª | æè«å¤§é­ç | 15 | æ© |
-æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 13 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ |
-9 | é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³ |
+27 | åå | ååçå°çª | æè«å¤§é­ç | 14 | æ© |
+æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 14 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ |
+6 | é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³ |
 3 | é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3 | ææ |
 ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿ | å¤æå°æ | 1 | Air | Air | Air | 15
-## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.4.5--2022.4.9 - ä¿®bugï¼æ¼ï¼ ###
-0.4.2--2022.4.9 - ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug - å¯ç¨webç«¯ -
-webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½® ### 0.4.1--2022.3 -
+| 3ks | ä¸ºäººæ°æå¡ | DK | 14 ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ###
+0.4.6--2022.4.9 - æ¾ç¤ºæ ææ - ä¼åæå¡å¨æåºç®æ³ï¼list.sort
+()å¤©ä¸ç¬¬ä¸ï¼ - é»è®¤å³é­webç«¯ ### 0.4.5--2022.4.9 - ä¿®bugï¼æ¼ï¼
+### 0.4.2--2022.4.9 - ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug - å¯ç¨webç«¯
+- webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½® ### 0.4.1--2022.3 -
 ä¿®å¤raråç¼©åå½åéè¯¯ - æ´æ°äºtagçåæ°è¯»åæ¹å¼ -
 ç¡®å®äºä¼ æä»¶ç§èæ¯ç¾¤èå¿«é - ä¿®å¤äºçµä¿¡æè®¡ç®éè¯¯ ###
 0.4.0--2022.3.27 - æ°å¢webæ§å¶å° - ä¿®å¤ä¼ å¾è¶æ¶åæ°éè¯¯ -
 éåæ±çipè·åæ¹æ³ ~ æ°æ®åºè¦æ ~ - éåææ¡£ -
 ä¸ååç½®ipï¼æ¯ç«ipv4é½æ´é²å¤ªå±é©äºï¼ ### 0.3.7--2022.3 -
 æ°å¢ä¸æ¹ä¸è½½ç½ç - ä¿®å¤windowsä¸ä¼ ä¸´æ¶æä»¶éè¯¯ -
 ä¼åæ¥ææµç¨ - ä¼åanneæéæºåè½ ### 0.3.6--2022.3.10 -
```

### Comparing `nonebot_plugin_l4d2_server-0.4.5/setup.py` & `nonebot_plugin_l4d2_server-0.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,17 @@
  'rarfile>=4.0,<5.0',
  'rcon>=2.1.0,<3.0.0',
  'ruamel.yaml>=0.17.21,<0.18.0',
  'srctools>=2.3.9,<3.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-l4d2-server',
-    'version': '0.4.5',
+    'version': '0.4.6',
     'description': 'L4D2 server related operations plugin for NoneBot2',
-    'long_description': '<div align="center">\n  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_l4d2_server\n_✨Nonebot & Left 4 Dead 2 server操作✨_\n<div align = "center">\n        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3" target="_blank">文档</a> &nbsp; · &nbsp;\n        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3#zl" target="_blank">指令列表</a> &nbsp; · &nbsp;\n        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/BUG%E5%8F%8D%E9%A6%88">常见问题</a>\n</div><br>\n<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/stargazers">\n        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_l4d2_server" alt="stars">\n</a>\n<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/issues">\n        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_l4d2_server" alt="issues">\n</a>\n<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">\n        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n        <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n    <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">\n</a>\n    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n    <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">\n</div>\n\n\n## 快速使用（env示例）\n    # 复制到env文件里，没有默认就是下列值，如需修改安装下面env设置\n    # 所有的多选，用逗号隔开\n    l4_master = [\'1145149191\']\n    l4_file = [\'/home/ubuntu/l4d2/coop\']\n    l4_host = [\'127.0.0.1\']\n    l4_port = [\'20715\']\n    l4_rcon = [\'1145149191810\']\n    l4_font = \'simsun.ttc\'\n    l4_only = True\n\n\n## 新文档（暂未完成）\n\n[点击这里](https://Agnes4m.github.io/l4d2)\n\n<h2 id="gn">主要功能</h2>\n\n- 求生服务器-本地多路径操作（传地图）\n- 批量查询指定ip服务器状态和玩家\n- 创意工坊下载和喷漆制作\n- [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)\n\n\n<h2 id="gn">如何获取key</h2>\n\n为了使得ip不被滥用，我采取这种方式管理。\n\n这并不影响正常使用，如果不需要可以忽略\n\n[点击这里加群](https://jq.qq.com/?_wv=1027&k=HdjoCcAe)并在群内发送“申请求生key”\n如果你只查询自己的服务器ip则可以忽略如下，并且更改env设置：\n\n        l4_tag = [\'呆呆\',\'橘\']      # 这里是内置可以查询的服的list对象\n        l4_key = \'qwertyuiopasdfg\'  # 这里是获取的key，是13个字符组成的字符串\n\n\n\n## 🚑  提交自己的服务器？\n\n**本项目原旨在方便自己查询管理服务器，如果你希望提供了ip**\n\n**那么我只能尽可能保证您的ip不会泄漏，如果无法承担风险则请勿提供ip**\n\n\n新增一个json文件，格式如下,文件名与需要响应的指令一致\n\n        {\n        "呆呆": [\n                {\n                "id": 1,\n                "version": "战役",\n                "ip": "43.248.188.17:27031"\n                }\n        ]\n        }\n\n<h2 id="ty">🌐 默认服务器</h2>\n目前 **已授权** 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主\n\n| 指令 | 服务器 | op | 数量 |\n|:-----:|:----:|:----:|:----:|\n| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 3\n| 云 | anne电信服云服 | 东 | 25\n| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15\n| 橘 | 橘希实香的小窝 | 橘希实香 | 13\n| 竹 | 竹烨 | 竹烨oО柠檬茶 | 9\n| 音理 | 星空列车与白的旅行 | 音理 | 3\n| 尤 | 尤尤 | 晓音 | 3\n| 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3\n| 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 1\n| Air | Air | Air | 15\n\n\n## 🔖 更新日志\n\n<details>\n<summary>展开/收起</summary>\n\n\n### 0.4.5--2022.4.9\n\n- 修bug（恼）\n\n### 0.4.2--2022.4.9\n\n - 修复响应开头匹配出现的重大bug\n - 启用web端\n - web使用yaml管理，未来可能删除env配置\n\n### 0.4.1--2022.3\n\n - 修复rar压缩包命名错误\n - 更新了tag的参数读取方式\n - 确定了传文件私聊比群聊快速\n - 修复了电信服计算错误\n\n### 0.4.0--2022.3.27\n\n - 新增web控制台\n - 修复传图超时参数错误\n - 重写求生ip获取方法 ~ 数据库苦手 ~\n - 重写文档\n - 不再内置ip（毕竟ipv4都暴露太危险了）\n\n### 0.3.7--2022.3\n\n - 新增三方下载网盘\n - 修复windows上传临时文件错误\n - 优化查服流程\n - 优化anne服随机功能\n\n### 0.3.6--2022.3.10\n\n - 暂时关闭web端，后续修改\n - 优化图片显示\n - 修复了海量bug\n - 新增三方图查询\n\n### 0.3.5--2022.3.6\n\n - 新增ping查询（在ip里包括）\n - 新增api查询（未完成）\n - 修复了电信服查询绑定名字无法查询的错误\n - 新增了救援率的显示\n - 新增web端（未完成）\n\n### 0.3.4--2022.3.1\n\n - 新增本地插件smx查询\n - 增加了三个内置群服\n - 修改了图片的UI,变好看了\n - 删减了部分图片和字体，使得轻量化\n - 修复了海量bug\n - 修复了python3.8中typing错误\n\n### 0.3.3--2022.2.26\n\n - 重写协议，使用a2s库，同时解决win端不同报错无法输出\n - 重~抄~写服务器查询UI,解决了不好看的问题\n - 从win测试，解决了一些win特有的bug\n - 重写服务器查询~还得是json~\n - 内置服务器查询系统，可以通过[服务器简称]+[number]/[模式]来访问\n - 新增批量查询服务器，不带参数则返回图片\n\n### 0.3.1--2022.2.22\n\n - 修复了路径识别为str对象的错误\n - 修复了初始化找不到文件的错误\n - 修复了路径拼接错误\n - 在win端成功测试，修复压缩包bug\n - 新增开关协程异步env设置\n - 测试rcon建立通讯\n - 实现切换路径查看地图和使用rcon指令\n\n### 0.3.0--2022.2.18\n\n - 修改了新的env配置，使得支持本地多服务器操作\n - 彻底解决了压缩包解压linux端的问题\n - 解决了win端默认gbk解码的错误\n - 解决rcon指令字体报错\n\n### 0.2.5--2022.2.10\n\n - 修复了依赖不足的bug\n - 更新了电信服战绩个人图片UI\n - 更新了批量服务器查看的UI\n - 修改了传文件为协程异步\n - 优化了部分rcon指令\n - ~tnd7z怎么不去死啊~使用pyunpack库解压7z\n\n### 0.2.4--2022.2.8\n\n - 使用poetry修复了pip安装文件缺失的bug\n\n### 0.2.3--2022.2.7\n\n - 新增坐牢和开牢\n - 修改了获取资源为异步协程却阻碍其他指令的bug\n - 新增json统计部分已知服务器（未来应该独立成库持续更新，如果把您的非公开服记录请联系我删除）\n - 喷剂制作开摆了，推测需要c/c++环境\n - 修改抽取文案\n - 新增查询服务器状态时返回connect ip\n - 修复了服务器查询无响应的时候，因为报错无回复信息的bug\n - 个人信息重置测试代码，下个版本更新\n - 新增求生更新添加和删除\n\n### 0.2.2--2022.2.1\n\n - 新增探监\n - 新增喷漆制作\n - 修复了魔改服务器导致解包错误的bug（就是直接忽略了）\n - 修改了部分对话响应\n\n### 0.2.1--2022.1.25\n\n - 新增电信服获取（东哥的肯定）\n - 优化图片UI \n - 新增云服快捷查询\n - 修复了因为没用玩家，导致的服务器状态查询错误\n - 新增电信服ip爬取（仅仅作为单次更新ip列表）\n\n### 0.2.0--2022.1.21\n\n - 新增创意工坊查询\n - 优化查询图片UI\n - 新增创意工坊文件下载\n - 修复了因为电信服官网前端修改导致查询失败的BUG\n\n### 0.1.7--2022.1.19\n\n - 新增群ip订阅，批量查询\n - 新增图片显示ip状态\n - 修复了因为玩家名字特殊字符导致的utf-8解码错误\n - 更新自己的第三方库VSQ==0.0.6\n\n### 0.1.6--2022.1.15\n\n - 新增ip查询服务器提供玩家数量和名字\n - 增加协程函数修复因为加载顺序导致的错误\n - 更新自己的第三方库VSQ==0.0.4\n\n### 0.1.5--2022.1.15\n\n- 新增服务器控制台指令，新增依赖rcon\n- 重新了数据库，不再使用json而是使用sql3\n- 改写了求生anne信息显示方式：如果单个数据以图片显示，如果多个数据以文字显示\n\n### 0.1.4--2022.1.9\n\n- 新增求生anne详情（看排名）\n- 所有的请求改为httpx\n- 更新了anne信息图片\n- 可选使用模拟谷歌浏览器来获取anne更多数据（~有点屎了，希望大佬救救~)\n\n### 0.1.3--2022.1.7\n\n- 新增绑定昵称和steamid\n- 新增可以艾特人查询anne成绩\n- 新增解绑信息\n\n### 0.1.2--2022.1.6\n\n- 新增支持图片输出\n- 新增查询anne服数据\n\n### 0.1.1--2022.1.5\n\n- 新增删除地图\n- 新增地图改名\n- 新增支持图片输出\n\n### 0.1.0--2022.1.4\n\n- 集中修复了Bug\n\n### 0.0.9--2022.1.4\n\n- 新增上传地图后，检测对比回复新地图名字\n- 修复中文名乱码问题\n\n### 0.0.8--2022.1.4\n\n- 支持vpk格式地图\n- 支持查看所有vpk格式文件\n\n### 0.0.6--2022.1.3\n\n- 修复了7z压缩包的方式，优化代码\n\n### 0.0.1--2022.1.3\n\n- 插件初次发布，可私聊添加地图\n\n</details>\n\n## 🙈 其他\n\n+ 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr\n+ 如果本插件对你有帮助，不要忘了点个Star~\n+ 本项目仅供学习使用，请勿用于商业用途\n+ [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)\n        \n\n<h2 id="ty">🌐 感谢</h2>\n\n- [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian) - 数据库的写法来自于他\n- [自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)(已弃用)\n- [@MeetWq](https://github.com/MeetWq) - 非常热心解答nonebot2相关的写法\n  - [可爱小Q](https://github.com/MeetWq/mybot) - 服务器图片写法参考小Q帮助\n- [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat) - web控制台的写法来自于他\n- [gsuid](https://github.com/KimigaiiWuyi/GenshinUID) - readme和wiki的格式参考\n- 呆呆 - 提供三方地图的详细数据\n',
+    'long_description': '<div align="center">\n  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_l4d2_server\n_✨Nonebot & Left 4 Dead 2 server操作✨_\n<div align = "center">\n        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3" target="_blank">文档</a> &nbsp; · &nbsp;\n        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3#zl" target="_blank">指令列表</a> &nbsp; · &nbsp;\n        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/BUG%E5%8F%8D%E9%A6%88">常见问题</a>\n</div><br>\n<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/stargazers">\n        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_l4d2_server" alt="stars">\n</a>\n<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/issues">\n        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_l4d2_server" alt="issues">\n</a>\n<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">\n        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n        <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n    <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">\n</a>\n    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n    <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">\n</div>\n\n\n## 快速使用（env示例）\n    # 复制到env文件里，没有默认就是下列值，如需修改安装下面env设置\n    # 所有的多选，用逗号隔开\n    l4_master = [\'1145149191\']            # 允许上传地图的qq号\n    l4_file = [\'/home/ubuntu/l4d2/coop\']  # 本地服务器路径\n    l4_host = [\'127.0.0.1\']               # 服务器ip（建议内网，公网也可以）\n    l4_port = [\'20715\']                   # 服务器端口\n    l4_rcon = [\'1145149191810\']           # 服务器rcon密码，如果没有可以列空str对象元素\n    l4_font = \'simsun.ttc\'                # 服务器字体\n\n\n## 新文档（暂未完成）\n\n[点击这里](https://Agnes4m.github.io/l4d2)\n\n<h2 id="gn">主要功能</h2>\n\n- 求生服务器-本地多路径操作（传地图）\n- 批量查询指定ip服务器状态和玩家\n- 创意工坊下载和喷漆制作\n- [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)\n\n\n<h2 id="gn">如何获取key</h2>\n\n为了使得ip不被滥用，我采取这种方式管理。\n\n这并不影响正常使用，如果不需要可以忽略\n\n[点击这里加群](https://jq.qq.com/?_wv=1027&k=HdjoCcAe)并在群内发送“申请求生key”\n如果你只查询自己的服务器ip则可以忽略如下，并且更改env设置：\n\n        l4_tag = [\'呆呆\',\'橘\']      # 这里是内置可以查询的服的list对象\n        l4_key = \'qwertyuiopasdfg\'  # 这里是获取的key，是13个字符组成的字符串\n\n\n\n## 🚑  提交自己的服务器？\n\n**本项目原旨在方便自己查询管理服务器，如果你希望提供了ip**\n\n**那么我只能尽可能保证您的ip不会泄漏，如果无法承担风险则请勿提供ip**\n\n\n新增一个json文件，格式如下,文件名与需要响应的指令一致\n\n        {\n        "呆呆": [\n                {\n                "id": 1,\n                "version": "战役",\n                "ip": "43.248.188.17:27031"\n                }\n        ]\n        }\n\n<h2 id="ty">🌐 默认服务器</h2>\n目前 **已授权** 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主\n\n| 指令 | 服务器 | op | 数量 |\n|:-----:|:----:|:----:|:----:|\n| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 3\n| 云 | anne电信服云服 | 东 | 27\n| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 14\n| 橘 | 橘希实香的小窝 | 橘希实香 | 14\n| 竹 | 竹烨 | 竹烨oО柠檬茶 | 6\n| 音理 | 星空列车与白的旅行 | 音理 | 3\n| 尤 | 尤尤 | 晓音 | 3\n| 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3\n| 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 1\n| Air | Air | Air | 15\n| 3ks | 为人民服务 | DK | 14\n\n\n## 🔖 更新日志\n\n<details>\n<summary>展开/收起</summary>\n\n### 0.4.6--2022.4.9\n\n - 显示无效服\n - 优化服务器排序算法（list.sort()天下第一）\n - 默认关闭web端\n\n### 0.4.5--2022.4.9\n\n- 修bug（恼）\n\n### 0.4.2--2022.4.9\n\n - 修复响应开头匹配出现的重大bug\n - 启用web端\n - web使用yaml管理，未来可能删除env配置\n\n### 0.4.1--2022.3\n\n - 修复rar压缩包命名错误\n - 更新了tag的参数读取方式\n - 确定了传文件私聊比群聊快速\n - 修复了电信服计算错误\n\n### 0.4.0--2022.3.27\n\n - 新增web控制台\n - 修复传图超时参数错误\n - 重写求生ip获取方法 ~ 数据库苦手 ~\n - 重写文档\n - 不再内置ip（毕竟ipv4都暴露太危险了）\n\n### 0.3.7--2022.3\n\n - 新增三方下载网盘\n - 修复windows上传临时文件错误\n - 优化查服流程\n - 优化anne服随机功能\n\n### 0.3.6--2022.3.10\n\n - 暂时关闭web端，后续修改\n - 优化图片显示\n - 修复了海量bug\n - 新增三方图查询\n\n### 0.3.5--2022.3.6\n\n - 新增ping查询（在ip里包括）\n - 新增api查询（未完成）\n - 修复了电信服查询绑定名字无法查询的错误\n - 新增了救援率的显示\n - 新增web端（未完成）\n\n### 0.3.4--2022.3.1\n\n - 新增本地插件smx查询\n - 增加了三个内置群服\n - 修改了图片的UI,变好看了\n - 删减了部分图片和字体，使得轻量化\n - 修复了海量bug\n - 修复了python3.8中typing错误\n\n### 0.3.3--2022.2.26\n\n - 重写协议，使用a2s库，同时解决win端不同报错无法输出\n - 重~抄~写服务器查询UI,解决了不好看的问题\n - 从win测试，解决了一些win特有的bug\n - 重写服务器查询~还得是json~\n - 内置服务器查询系统，可以通过[服务器简称]+[number]/[模式]来访问\n - 新增批量查询服务器，不带参数则返回图片\n\n### 0.3.1--2022.2.22\n\n - 修复了路径识别为str对象的错误\n - 修复了初始化找不到文件的错误\n - 修复了路径拼接错误\n - 在win端成功测试，修复压缩包bug\n - 新增开关协程异步env设置\n - 测试rcon建立通讯\n - 实现切换路径查看地图和使用rcon指令\n\n### 0.3.0--2022.2.18\n\n - 修改了新的env配置，使得支持本地多服务器操作\n - 彻底解决了压缩包解压linux端的问题\n - 解决了win端默认gbk解码的错误\n - 解决rcon指令字体报错\n\n### 0.2.5--2022.2.10\n\n - 修复了依赖不足的bug\n - 更新了电信服战绩个人图片UI\n - 更新了批量服务器查看的UI\n - 修改了传文件为协程异步\n - 优化了部分rcon指令\n - ~tnd7z怎么不去死啊~使用pyunpack库解压7z\n\n### 0.2.4--2022.2.8\n\n - 使用poetry修复了pip安装文件缺失的bug\n\n### 0.2.3--2022.2.7\n\n - 新增坐牢和开牢\n - 修改了获取资源为异步协程却阻碍其他指令的bug\n - 新增json统计部分已知服务器（未来应该独立成库持续更新，如果把您的非公开服记录请联系我删除）\n - 喷剂制作开摆了，推测需要c/c++环境\n - 修改抽取文案\n - 新增查询服务器状态时返回connect ip\n - 修复了服务器查询无响应的时候，因为报错无回复信息的bug\n - 个人信息重置测试代码，下个版本更新\n - 新增求生更新添加和删除\n\n### 0.2.2--2022.2.1\n\n - 新增探监\n - 新增喷漆制作\n - 修复了魔改服务器导致解包错误的bug（就是直接忽略了）\n - 修改了部分对话响应\n\n### 0.2.1--2022.1.25\n\n - 新增电信服获取（东哥的肯定）\n - 优化图片UI \n - 新增云服快捷查询\n - 修复了因为没用玩家，导致的服务器状态查询错误\n - 新增电信服ip爬取（仅仅作为单次更新ip列表）\n\n### 0.2.0--2022.1.21\n\n - 新增创意工坊查询\n - 优化查询图片UI\n - 新增创意工坊文件下载\n - 修复了因为电信服官网前端修改导致查询失败的BUG\n\n### 0.1.7--2022.1.19\n\n - 新增群ip订阅，批量查询\n - 新增图片显示ip状态\n - 修复了因为玩家名字特殊字符导致的utf-8解码错误\n - 更新自己的第三方库VSQ==0.0.6\n\n### 0.1.6--2022.1.15\n\n - 新增ip查询服务器提供玩家数量和名字\n - 增加协程函数修复因为加载顺序导致的错误\n - 更新自己的第三方库VSQ==0.0.4\n\n### 0.1.5--2022.1.15\n\n- 新增服务器控制台指令，新增依赖rcon\n- 重新了数据库，不再使用json而是使用sql3\n- 改写了求生anne信息显示方式：如果单个数据以图片显示，如果多个数据以文字显示\n\n### 0.1.4--2022.1.9\n\n- 新增求生anne详情（看排名）\n- 所有的请求改为httpx\n- 更新了anne信息图片\n- 可选使用模拟谷歌浏览器来获取anne更多数据（~有点屎了，希望大佬救救~)\n\n### 0.1.3--2022.1.7\n\n- 新增绑定昵称和steamid\n- 新增可以艾特人查询anne成绩\n- 新增解绑信息\n\n### 0.1.2--2022.1.6\n\n- 新增支持图片输出\n- 新增查询anne服数据\n\n### 0.1.1--2022.1.5\n\n- 新增删除地图\n- 新增地图改名\n- 新增支持图片输出\n\n### 0.1.0--2022.1.4\n\n- 集中修复了Bug\n\n### 0.0.9--2022.1.4\n\n- 新增上传地图后，检测对比回复新地图名字\n- 修复中文名乱码问题\n\n### 0.0.8--2022.1.4\n\n- 支持vpk格式地图\n- 支持查看所有vpk格式文件\n\n### 0.0.6--2022.1.3\n\n- 修复了7z压缩包的方式，优化代码\n\n### 0.0.1--2022.1.3\n\n- 插件初次发布，可私聊添加地图\n\n</details>\n\n## 🙈 其他\n\n+ 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr\n+ 如果本插件对你有帮助，不要忘了点个Star~\n+ 本项目仅供学习使用，请勿用于商业用途\n+ [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)\n        \n\n<h2 id="ty">🌐 感谢</h2>\n\n- [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian) - 数据库的写法来自于他\n- [自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)(已弃用)\n- [@MeetWq](https://github.com/MeetWq) - 非常热心解答nonebot2相关的写法\n  - [可爱小Q](https://github.com/MeetWq/mybot) - 服务器图片写法参考小Q帮助\n- [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat) - web控制台的写法来自于他\n- [gsuid](https://github.com/KimigaiiWuyi/GenshinUID) - readme和wiki的格式参考\n- 呆呆 - 提供三方地图的详细数据\n',
     'author': 'Agnes_Digital',
     'author_email': 'Z735803792@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Agnes4m/nonebot_plugin_l4d2_server',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -12,34 +12,37 @@
 'jinja2>=3.0.0', 'nonebot-adapter-onebot>=2.1.5', 'nonebot2>=2.0.0rc4,<3.0.0',
 'nonebot_plugin_apscheduler>=0.2.0,<0.3.0',
 'nonebot_plugin_htmlrender>=0.2.0.1,<0.3.0.0', 'nonebot_plugin_txt2img>=0.3.0',
 'pandas>=1.5.2', 'patool>=1.12,<2.0', 'pillow>=9.3.0,<10.0.0', 'python-
 a2s>=1.3.0,<2.0.0', 'python-jose>=3.3.0,<4.0.0', 'pyunpack>=0.3.0,<0.4.0',
 'rarfile>=4.0,<5.0', 'rcon>=2.1.0,<3.0.0', 'ruamel.yaml>=0.17.21,<0.18.0',
 'srctools>=2.3.9,<3.0.0'] setup_kwargs = { 'name': 'nonebot-plugin-l4d2-
-server', 'version': '0.4.5', 'description': 'L4D2 server related operations
+server', 'version': '0.4.6', 'description': 'L4D2 server related operations
 plugin for NoneBot2', 'long_description': '
                            \n [AgnesDigitalLogo]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n
          \n\n# nonebot_plugin_l4d2_server\n_â¨Nonebot & Left 4 Dead 2
                               serveræä½â¨_\n
             \n ææ¡£   Â·  \n æä»¤åè¡¨   Â·  \n å¸¸è§é®é¢\n
 
     \n\n_[GitHub_stars]\n\n\n_[GitHub_issues]\n\n\n_[QQ_Chat_Group]\n\n\n_
             [pypi]\n\n\n_[pypi_download]\n\n [python]\n [NoneBot]\n
 \n\n\n## å¿«éä½¿ç¨ï¼envç¤ºä¾ï¼\n #
 å¤å¶å°envæä»¶éï¼æ²¡æé»è®¤å°±æ¯ä¸åå¼ï¼å¦éä¿®æ¹å®è£ä¸é¢envè®¾ç½®\n
-# ææçå¤éï¼ç¨éå·éå¼\n l4_master = [\'1145149191\']\n l4_file =
-[\'/home/ubuntu/l4d2/coop\']\n l4_host = [\'127.0.0.1\']\n l4_port =
-[\'20715\']\n l4_rcon = [\'1145149191810\']\n l4_font = \'simsun.ttc\'\n
-l4_only = True\n\n\n## æ°ææ¡£ï¼ææªå®æï¼\n\n[ç¹å»è¿é](https://
-Agnes4m.github.io/l4d2)\n\n
+# ææçå¤éï¼ç¨éå·éå¼\n l4_master = [\'1145149191\'] #
+åè®¸ä¸ä¼ å°å¾çqqå·\n l4_file = [\'/home/ubuntu/l4d2/coop\'] #
+æ¬å°æå¡å¨è·¯å¾\n l4_host = [\'127.0.0.1\'] #
+æå¡å¨ipï¼å»ºè®®åç½ï¼å¬ç½ä¹å¯ä»¥ï¼\n l4_port = [\'20715\'] #
+æå¡å¨ç«¯å£\n l4_rcon = [\'1145149191810\'] #
+æå¡å¨rconå¯ç ï¼å¦ææ²¡æå¯ä»¥åç©ºstrå¯¹è±¡åç´ \n l4_font =
+\'simsun.ttc\' # æå¡å¨å­ä½\n\n\n## æ°ææ¡£ï¼ææªå®æï¼\n\n
+[ç¹å»è¿é](https://Agnes4m.github.io/l4d2)\n\n
 ***** ä¸»è¦åè½ *****
 \n\n- æ±çæå¡å¨-æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼\n-
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶\n-
 åæå·¥åä¸è½½åå·æ¼å¶ä½\n- [æ±ççµä¿¡æanne](https://github.com/
 fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/l4d_stats/
 ranking/index.php)\n\n\n
 ***** å¦ä½è·åkey *****
@@ -53,22 +56,24 @@
 {\n "åå": [\n {\n "id": 1,\n "version": "æå½¹",\n "ip": "43.248.188.17:
 27031"\n }\n ]\n }\n\n
 ***** ð é»è®¤æå¡å¨ *****
 \nç®å **å·²ææ**
 çæå¡å¨æ¥è¯¢ï¼å¦æéè¦å å¥èªå·±çipå¯ä»¥è¿qqç¾¤ç§èç¾¤ä¸»\n\n|
 æä»¤ | æå¡å¨ | op | æ°é |\n|:-----:|:----:|:----:|:----:|\n| æ°ç  |
 ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 3\n| äº | anneçµä¿¡æäºæ | ä¸
-| 25\n| åå | ååçå°çª | æè«å¤§é­ç | 15\n| æ© |
-æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 13\n| ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶
-| 9\n| é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3\n| å°¤ | å°¤å°¤ |
+| 27\n| åå | ååçå°çª | æè«å¤§é­ç | 14\n| æ© |
+æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 14\n| ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶
+| 6\n| é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3\n| å°¤ | å°¤å°¤ |
 æé³ | 3\n| é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3\n| ææ |
 ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿ | å¤æå°æ | 1\n| Air | Air | Air |
-15\n\n\n## ð æ´æ°æ¥å¿\n\n\nå±å¼/æ¶èµ·\n\n\n### 0.4.5--2022.4.9\n\n-
-ä¿®bugï¼æ¼ï¼\n\n### 0.4.2--2022.4.9\n\n -
-ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug\n - å¯ç¨webç«¯\n -
+15\n| 3ks | ä¸ºäººæ°æå¡ | DK | 14\n\n\n## ð æ´æ°æ¥å¿\n\n\nå±å¼/
+æ¶èµ·\n\n### 0.4.6--2022.4.9\n\n - æ¾ç¤ºæ ææ\n -
+ä¼åæå¡å¨æåºç®æ³ï¼list.sort()å¤©ä¸ç¬¬ä¸ï¼\n -
+é»è®¤å³é­webç«¯\n\n### 0.4.5--2022.4.9\n\n- ä¿®bugï¼æ¼ï¼\n\n### 0.4.2--
+2022.4.9\n\n - ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug\n - å¯ç¨webç«¯\n -
 webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½®\n\n### 0.4.1--2022.3\n\n -
 ä¿®å¤raråç¼©åå½åéè¯¯\n - æ´æ°äºtagçåæ°è¯»åæ¹å¼\n -
 ç¡®å®äºä¼ æä»¶ç§èæ¯ç¾¤èå¿«é\n -
 ä¿®å¤äºçµä¿¡æè®¡ç®éè¯¯\n\n### 0.4.0--2022.3.27\n\n -
 æ°å¢webæ§å¶å°\n - ä¿®å¤ä¼ å¾è¶æ¶åæ°éè¯¯\n -
 éåæ±çipè·åæ¹æ³ ~ æ°æ®åºè¦æ ~\n - éåææ¡£\n -
 ä¸ååç½®ipï¼æ¯ç«ipv4é½æ´é²å¤ªå±é©äºï¼\n\n### 0.3.7--2022.3\n\n -
```

### Comparing `nonebot_plugin_l4d2_server-0.4.5/PKG-INFO` & `nonebot_plugin_l4d2_server-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.4.5
+Version: 0.4.6
 Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -79,21 +79,20 @@
     <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">
 </div>
 
 
 ## 快速使用（env示例）
     # 复制到env文件里，没有默认就是下列值，如需修改安装下面env设置
     # 所有的多选，用逗号隔开
-    l4_master = ['1145149191']
-    l4_file = ['/home/ubuntu/l4d2/coop']
-    l4_host = ['127.0.0.1']
-    l4_port = ['20715']
-    l4_rcon = ['1145149191810']
-    l4_font = 'simsun.ttc'
-    l4_only = True
+    l4_master = ['1145149191']            # 允许上传地图的qq号
+    l4_file = ['/home/ubuntu/l4d2/coop']  # 本地服务器路径
+    l4_host = ['127.0.0.1']               # 服务器ip（建议内网，公网也可以）
+    l4_port = ['20715']                   # 服务器端口
+    l4_rcon = ['1145149191810']           # 服务器rcon密码，如果没有可以列空str对象元素
+    l4_font = 'simsun.ttc'                # 服务器字体
 
 
 ## 新文档（暂未完成）
 
 [点击这里](https://Agnes4m.github.io/l4d2)
 
 <h2 id="gn">主要功能</h2>
@@ -139,30 +138,36 @@
 
 <h2 id="ty">🌐 默认服务器</h2>
 目前 **已授权** 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主
 
 | 指令 | 服务器 | op | 数量 |
 |:-----:|:----:|:----:|:----:|
 | 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 3
-| 云 | anne电信服云服 | 东 | 25
-| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15
-| 橘 | 橘希实香的小窝 | 橘希实香 | 13
-| 竹 | 竹烨 | 竹烨oО柠檬茶 | 9
+| 云 | anne电信服云服 | 东 | 27
+| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 14
+| 橘 | 橘希实香的小窝 | 橘希实香 | 14
+| 竹 | 竹烨 | 竹烨oО柠檬茶 | 6
 | 音理 | 星空列车与白的旅行 | 音理 | 3
 | 尤 | 尤尤 | 晓音 | 3
 | 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3
 | 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 1
 | Air | Air | Air | 15
+| 3ks | 为人民服务 | DK | 14
 
 
 ## 🔖 更新日志
 
 <details>
 <summary>展开/收起</summary>
 
+### 0.4.6--2022.4.9
+
+ - 显示无效服
+ - 优化服务器排序算法（list.sort()天下第一）
+ - 默认关闭web端
 
 ### 0.4.5--2022.4.9
 
 - 修bug（恼）
 
 ### 0.4.2--2022.4.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.4.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.4.6 Summary:
 L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
 Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
@@ -30,18 +30,22 @@
    # nonebot_plugin_l4d2_server _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
                 ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
 
 [GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
                                    [NoneBot]
 ## å¿«éä½¿ç¨ï¼envç¤ºä¾ï¼ #
 å¤å¶å°envæä»¶éï¼æ²¡æé»è®¤å°±æ¯ä¸åå¼ï¼å¦éä¿®æ¹å®è£ä¸é¢envè®¾ç½®
-# ææçå¤éï¼ç¨éå·éå¼ l4_master = ['1145149191'] l4_file = ['/
-home/ubuntu/l4d2/coop'] l4_host = ['127.0.0.1'] l4_port = ['20715'] l4_rcon =
-['1145149191810'] l4_font = 'simsun.ttc' l4_only = True ##
-æ°ææ¡£ï¼ææªå®æï¼ [ç¹å»è¿é](https://Agnes4m.github.io/l4d2)
+# ææçå¤éï¼ç¨éå·éå¼ l4_master = ['1145149191'] #
+åè®¸ä¸ä¼ å°å¾çqqå· l4_file = ['/home/ubuntu/l4d2/coop'] #
+æ¬å°æå¡å¨è·¯å¾ l4_host = ['127.0.0.1'] #
+æå¡å¨ipï¼å»ºè®®åç½ï¼å¬ç½ä¹å¯ä»¥ï¼ l4_port = ['20715'] #
+æå¡å¨ç«¯å£ l4_rcon = ['1145149191810'] #
+æå¡å¨rconå¯ç ï¼å¦ææ²¡æå¯ä»¥åç©ºstrå¯¹è±¡åç´  l4_font =
+'simsun.ttc' # æå¡å¨å­ä½ ## æ°ææ¡£ï¼ææªå®æï¼ [ç¹å»è¿é]
+(https://Agnes4m.github.io/l4d2)
 ***** ä¸»è¦åè½ *****
 - æ±çæå¡å¨-æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶ -
 åæå·¥åä¸è½½åå·æ¼å¶ä½ - [æ±ççµä¿¡æanne](https://github.com/
 fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/l4d_stats/
 ranking/index.php)
 ***** å¦ä½è·åkey *****
@@ -58,22 +62,24 @@
 æ°å¢ä¸ä¸ªjsonæä»¶ï¼æ ¼å¼å¦ä¸,æä»¶åä¸éè¦ååºçæä»¤ä¸è´
 { "åå": [ { "id": 1, "version": "æå½¹", "ip": "43.248.188.17:27031" } ] }
 ***** ð é»è®¤æå¡å¨ *****
 ç®å **å·²ææ**
 çæå¡å¨æ¥è¯¢ï¼å¦æéè¦å å¥èªå·±çipå¯ä»¥è¿qqç¾¤ç§èç¾¤ä¸» |
 æä»¤ | æå¡å¨ | op | æ°é | |:-----:|:----:|:----:|:----:| | æ°ç  |
 ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 3 | äº | anneçµä¿¡æäºæ | ä¸ |
-25 | åå | ååçå°çª | æè«å¤§é­ç | 15 | æ© |
-æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 13 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ |
-9 | é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³ |
+27 | åå | ååçå°çª | æè«å¤§é­ç | 14 | æ© |
+æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 14 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ |
+6 | é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³ |
 3 | é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3 | ææ |
 ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿ | å¤æå°æ | 1 | Air | Air | Air | 15
-## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.4.5--2022.4.9 - ä¿®bugï¼æ¼ï¼ ###
-0.4.2--2022.4.9 - ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug - å¯ç¨webç«¯ -
-webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½® ### 0.4.1--2022.3 -
+| 3ks | ä¸ºäººæ°æå¡ | DK | 14 ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ###
+0.4.6--2022.4.9 - æ¾ç¤ºæ ææ - ä¼åæå¡å¨æåºç®æ³ï¼list.sort
+()å¤©ä¸ç¬¬ä¸ï¼ - é»è®¤å³é­webç«¯ ### 0.4.5--2022.4.9 - ä¿®bugï¼æ¼ï¼
+### 0.4.2--2022.4.9 - ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug - å¯ç¨webç«¯
+- webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½® ### 0.4.1--2022.3 -
 ä¿®å¤raråç¼©åå½åéè¯¯ - æ´æ°äºtagçåæ°è¯»åæ¹å¼ -
 ç¡®å®äºä¼ æä»¶ç§èæ¯ç¾¤èå¿«é - ä¿®å¤äºçµä¿¡æè®¡ç®éè¯¯ ###
 0.4.0--2022.3.27 - æ°å¢webæ§å¶å° - ä¿®å¤ä¼ å¾è¶æ¶åæ°éè¯¯ -
 éåæ±çipè·åæ¹æ³ ~ æ°æ®åºè¦æ ~ - éåææ¡£ -
 ä¸ååç½®ipï¼æ¯ç«ipv4é½æ´é²å¤ªå±é©äºï¼ ### 0.3.7--2022.3 -
 æ°å¢ä¸æ¹ä¸è½½ç½ç - ä¿®å¤windowsä¸ä¼ ä¸´æ¶æä»¶éè¯¯ -
 ä¼åæ¥ææµç¨ - ä¼åanneæéæºåè½ ### 0.3.6--2022.3.10 -
```

