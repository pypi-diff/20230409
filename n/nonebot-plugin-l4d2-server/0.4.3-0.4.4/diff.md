# Comparing `tmp/nonebot_plugin_l4d2_server-0.4.3.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.4.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.4.4.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.4.3.tar` & `nonebot_plugin_l4d2_server-0.4.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0    35823 2023-01-11 11:22:12.357251 nonebot_plugin_l4d2_server-0.4.3/LICENSE
--rw-r--r--   0        0        0    16800 2023-04-08 18:52:51.706045 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0     8027 2023-04-08 18:50:15.782345 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/command.py
--rw-r--r--   0        0        0     4965 2023-04-08 18:09:47.583660 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/config.py
--rw-r--r--   0        0        0   158357 2023-01-08 15:05:11.765786 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-03-24 06:27:47.516852 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2022-11-27 13:06:53.317128 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1666 2023-03-06 09:04:41.376881 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-03-03 03:43:40.240633 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2150 2023-02-23 00:58:59.231306 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     5829 2023-03-01 12:23:49.342774 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help - 副本.html
--rw-r--r--   0        0        0     6206 2023-03-05 16:25:01.648005 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6417 2023-02-27 15:03:03.981712 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1595 2023-03-02 15:28:44.743644 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     7874 2023-02-11 08:42:33.584146 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0     9067 2023-04-08 18:51:30.036612 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1661 2023-03-25 04:40:02.232501 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3085 2023-03-05 15:25:37.373454 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1702 2023-03-05 15:52:53.906753 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      376 2023-03-06 08:23:02.068422 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3332 2023-02-26 09:03:45.382934 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      485 2023-01-14 18:23:43.868353 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0     3308 2023-02-26 09:03:47.639393 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1316 2023-01-20 07:16:17.336574 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4197 2023-03-28 03:12:43.717423 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     4128 2023-03-18 17:22:46.673151 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4097 2023-02-11 08:44:48.430294 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1070 2023-02-06 23:05:41.006175 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0      968 2023-01-14 18:06:13.728698 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3882 2023-04-08 18:51:00.452792 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1427 2023-02-04 03:31:45.112442 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     3520 2023-04-08 12:57:15.592761 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1141 2023-04-08 18:08:59.052656 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0      741 2023-03-25 17:41:59.756270 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    10656 2023-04-08 15:58:37.818041 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1676 2023-02-19 10:27:01.909990 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0     1160 2023-02-17 18:42:54.854831 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1409 2023-03-02 15:06:19.826864 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     3397 2023-04-08 18:51:42.656361 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_web/config.py
--rw-r--r--   0        0        0     6336 2023-04-08 18:49:08.823312 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    10799 2023-04-08 18:36:09.768036 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1678 2023-02-26 09:29:05.903725 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/message.py
--rw-r--r--   0        0        0     1025 2023-03-05 15:52:53.333459 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/seach.py
--rw-r--r--   0        0        0     2166 2023-04-08 18:49:42.643806 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/txt_to_img.py
--rw-r--r--   0        0        0     8189 2023-04-08 18:49:44.109038 nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/utils.py
--rw-r--r--   0        0        0     1513 2023-04-08 18:52:45.819534 nonebot_plugin_l4d2_server-0.4.3/pyproject.toml
--rw-r--r--   0        0        0    11067 2023-04-08 18:35:22.067066 nonebot_plugin_l4d2_server-0.4.3/README.md
--rw-r--r--   0        0        0    12862 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.3/setup.py
--rw-r--r--   0        0        0    12779 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-01-11 11:22:12.357251 nonebot_plugin_l4d2_server-0.4.4/LICENSE
+-rw-r--r--   0        0        0    16815 2023-04-09 05:13:35.513024 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0     8027 2023-04-08 18:50:15.782345 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/command.py
+-rw-r--r--   0        0        0     4965 2023-04-08 18:09:47.583660 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/config.py
+-rw-r--r--   0        0        0   158357 2023-01-08 15:05:11.765786 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-03-24 06:27:47.516852 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2022-11-27 13:06:53.317128 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1666 2023-03-06 09:04:41.376881 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-03-03 03:43:40.240633 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2150 2023-02-23 00:58:59.231306 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     5829 2023-03-01 12:23:49.342774 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help - 副本.html
+-rw-r--r--   0        0        0     6206 2023-03-05 16:25:01.648005 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6417 2023-02-27 15:03:03.981712 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1595 2023-03-02 15:28:44.743644 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     7874 2023-02-11 08:42:33.584146 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0     9067 2023-04-08 18:51:30.036612 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1661 2023-03-25 04:40:02.232501 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3085 2023-03-05 15:25:37.373454 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1702 2023-03-05 15:52:53.906753 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      376 2023-03-06 08:23:02.068422 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3332 2023-02-26 09:03:45.382934 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      485 2023-01-14 18:23:43.868353 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0     3308 2023-02-26 09:03:47.639393 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1316 2023-01-20 07:16:17.336574 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4197 2023-03-28 03:12:43.717423 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     4128 2023-03-18 17:22:46.673151 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4097 2023-02-11 08:44:48.430294 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1070 2023-02-06 23:05:41.006175 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0      968 2023-01-14 18:06:13.728698 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3882 2023-04-08 18:51:00.452792 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1427 2023-02-04 03:31:45.112442 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     3520 2023-04-08 12:57:15.592761 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1141 2023-04-08 18:08:59.052656 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0      741 2023-03-25 17:41:59.756270 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    10656 2023-04-08 15:58:37.818041 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1676 2023-02-19 10:27:01.909990 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0     1160 2023-02-17 18:42:54.854831 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1409 2023-03-02 15:06:19.826864 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     3397 2023-04-08 18:51:42.656361 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_web/config.py
+-rw-r--r--   0        0        0     6336 2023-04-08 18:49:08.823312 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    10799 2023-04-08 18:36:09.768036 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1678 2023-02-26 09:29:05.903725 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/message.py
+-rw-r--r--   0        0        0     1025 2023-03-05 15:52:53.333459 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/seach.py
+-rw-r--r--   0        0        0     2166 2023-04-08 18:49:42.643806 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/txt_to_img.py
+-rw-r--r--   0        0        0     8189 2023-04-08 18:49:44.109038 nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/utils.py
+-rw-r--r--   0        0        0     1505 2023-04-09 05:14:40.703997 nonebot_plugin_l4d2_server-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0    10903 2023-04-09 05:15:08.471487 nonebot_plugin_l4d2_server-0.4.4/README.md
+-rw-r--r--   0        0        0    12712 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.4/setup.py
+-rw-r--r--   0        0        0    12573 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.4/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.4.3/LICENSE` & `nonebot_plugin_l4d2_server-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,28 +35,30 @@
 from .l4d2_queries.ohter import load_josn
 from .l4d2_queries.qqgroup import write_json
 from .l4d2_file import updown_l4d2_vpk,all_zip_to_one
 
 from .txt_to_img import mode_txt_to_img
 # from .l4d2_server import RCONClient
 scheduler = require("nonebot_plugin_apscheduler").scheduler
-
-from .l4d2_web import web,webUI
+if l4_web:
+    from .l4d2_web import web,webUI
+else:
+    pass
 
 driver = get_driver()
 
 
 __version__ = "0.4.3"
 __plugin_meta__ = PluginMetadata(
     name="求生之路小助手",
     description='群内对有关求生之路的查询和操作',
     usage='求生服务器操作指令',
     extra={
         "version": __version__,
-        "author": "Umamusume-Agnes-Digital <Z735803792@163.com>",
+        "author": "Agnes4m <Z735803792@163.com>",
     },
 )
 
 
 """相当于启动就检查数据库"""
```

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/command.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/command.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/config.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help - 副本.html` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help - 副本.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_web/config.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_web/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/message.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/seach.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/txt_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/nonebot_plugin_l4d2_server/utils.py` & `nonebot_plugin_l4d2_server-0.4.4/nonebot_plugin_l4d2_server/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.3/pyproject.toml` & `nonebot_plugin_l4d2_server-0.4.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.4.3"
+version = "0.4.4"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
-homepage = "https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server"
-repository = "https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server"
+homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
+repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -18,16 +18,16 @@
     "Operating System :: OS Independent",
 ]
 include = [
     "LICENSE","README.md"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-nonebot2 = "^2.0.0rc3"
+python = "^3.9"
+nonebot2 = "^2.0.0rc4"
 nonebot-adapter-onebot = ">=2.1.5"
 nonebot_plugin_htmlrender = "^0.2.0.1"
 nonebot_plugin_txt2img = ">=0.3.0"
 nonebot_plugin_apscheduler = "^0.2.0"
 asyncio = ">=3.4.3"
 jinja2 = ">=3.0.0"
 srctools="^2.3.9"
@@ -40,11 +40,12 @@
 "ruamel.yaml" = "^0.17.21"
 rarfile = "^4.0"
 patool = "^1.12"
 python-a2s = "^1.3.0"
 amis-python = "^1.0.6"
 jieba = "^0.42.1"
 pandas = ">=1.5.2"
+python-jose = "^3.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_l4d2_server-0.4.3/README.md` & `nonebot_plugin_l4d2_server-0.4.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <div align="center">
-  <img src="https://raw.githubusercontent.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
+  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
   <br>
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot_plugin_l4d2_server
 _✨Nonebot & Left 4 Dead 2 server操作✨_
 <div align = "center">
-        <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3" target="_blank">文档</a> &nbsp; · &nbsp;
-        <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3#zl" target="_blank">指令列表</a> &nbsp; · &nbsp;
-        <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/wiki/BUG%E5%8F%8D%E9%A6%88">常见问题</a>
+        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3" target="_blank">文档</a> &nbsp; · &nbsp;
+        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3#zl" target="_blank">指令列表</a> &nbsp; · &nbsp;
+        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/BUG%E5%8F%8D%E9%A6%88">常见问题</a>
 </div><br>
-<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/stargazers">
-        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server" alt="stars">
+<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/stargazers">
+        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_l4d2_server" alt="stars">
 </a>
-<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/issues">
-        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server" alt="issues">
+<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/issues">
+        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_l4d2_server" alt="issues">
 </a>
 <a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">
         <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">
         <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">
 </a>
@@ -43,15 +43,15 @@
     l4_rcon = ['1145149191810']
     l4_font = 'simsun.ttc'
     l4_only = True
 
 
 ## 新文档（暂未完成）
 
-[点击这里](https://umamusume-agnes-digital.github.io/l4d2)
+[点击这里](https://Agnes4m.github.io/l4d2)
 
 <h2 id="gn">主要功能</h2>
 
 - 求生服务器-本地多路径操作（传地图）
 - 批量查询指定ip服务器状态和玩家
 - 创意工坊下载和喷漆制作
 - [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)
@@ -109,14 +109,18 @@
 
 ## 🔖 更新日志
 
 <details>
 <summary>展开/收起</summary>
 
 
+### 0.4.4--2022.4.9
+
+- 修bug（恼）
+
 ### 0.4.2--2022.4.9
 
  - 修复响应开头匹配出现的重大bug
  - 启用web端
  - web使用yaml管理，未来可能删除env配置
 
 ### 0.4.1--2022.3
@@ -306,19 +310,19 @@
 </details>
 
 ## 🙈 其他
 
 + 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr
 + 如果本插件对你有帮助，不要忘了点个Star~
 + 本项目仅供学习使用，请勿用于商业用途
-+ [GPL-3.0 License](https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Umamusume-Agnes-Digital](https://github.com/Umamusume-Agnes-Digital)
++ [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
         
 
 <h2 id="ty">🌐 感谢</h2>
 
 - [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian) - 数据库的写法来自于他
-- [自己写的求生之路查询库](https://github.com/Umamusume-Agnes-Digital/VSQ)(已弃用)
+- [自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)(已弃用)
 - [@MeetWq](https://github.com/MeetWq) - 非常热心解答nonebot2相关的写法
   - [可爱小Q](https://github.com/MeetWq/mybot) - 服务器图片写法参考小Q帮助
 - [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat) - web控制台的写法来自于他
 - [gsuid](https://github.com/KimigaiiWuyi/GenshinUID) - readme和wiki的格式参考
 - 呆呆 - 提供三方地图的详细数据
```

#### html2text {}

```diff
@@ -6,16 +6,15 @@
 [GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
                                    [NoneBot]
 ## å¿«éä½¿ç¨ï¼envç¤ºä¾ï¼ #
 å¤å¶å°envæä»¶éï¼æ²¡æé»è®¤å°±æ¯ä¸åå¼ï¼å¦éä¿®æ¹å®è£ä¸é¢envè®¾ç½®
 # ææçå¤éï¼ç¨éå·éå¼ l4_master = ['1145149191'] l4_file = ['/
 home/ubuntu/l4d2/coop'] l4_host = ['127.0.0.1'] l4_port = ['20715'] l4_rcon =
 ['1145149191810'] l4_font = 'simsun.ttc' l4_only = True ##
-æ°ææ¡£ï¼ææªå®æï¼ [ç¹å»è¿é](https://umamusume-agnes-
-digital.github.io/l4d2)
+æ°ææ¡£ï¼ææªå®æï¼ [ç¹å»è¿é](https://Agnes4m.github.io/l4d2)
 ***** ä¸»è¦åè½ *****
 - æ±çæå¡å¨-æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶ -
 åæå·¥åä¸è½½åå·æ¼å¶ä½ - [æ±ççµä¿¡æanne](https://github.com/
 fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/l4d_stats/
 ranking/index.php)
 ***** å¦ä½è·åkey *****
@@ -37,16 +36,16 @@
 æä»¤ | æå¡å¨ | op | æ°é | |:-----:|:----:|:----:|:----:| | æ°ç  |
 ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 3 | äº | anneçµä¿¡æäºæ | ä¸ |
 25 | åå | ååçå°çª | æè«å¤§é­ç | 15 | æ© |
 æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 13 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ |
 9 | é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³ |
 3 | é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3 | ææ |
 ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿ | å¤æå°æ | 1 | Air | Air | Air | 15
-## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.4.2--2022.4.9 -
-ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug - å¯ç¨webç«¯ -
+## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.4.4--2022.4.9 - ä¿®bugï¼æ¼ï¼ ###
+0.4.2--2022.4.9 - ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug - å¯ç¨webç«¯ -
 webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½® ### 0.4.1--2022.3 -
 ä¿®å¤raråç¼©åå½åéè¯¯ - æ´æ°äºtagçåæ°è¯»åæ¹å¼ -
 ç¡®å®äºä¼ æä»¶ç§èæ¯ç¾¤èå¿«é - ä¿®å¤äºçµä¿¡æè®¡ç®éè¯¯ ###
 0.4.0--2022.3.27 - æ°å¢webæ§å¶å° - ä¿®å¤ä¼ å¾è¶æ¶åæ°éè¯¯ -
 éåæ±çipè·åæ¹æ³ ~ æ°æ®åºè¦æ ~ - éåææ¡£ -
 ä¸ååç½®ipï¼æ¯ç«ipv4é½æ´é²å¤ªå±é©äºï¼ ### 0.3.7--2022.3 -
 æ°å¢ä¸æ¹ä¸è½½ç½ç - ä¿®å¤windowsä¸ä¼ ä¸´æ¶æä»¶éè¯¯ -
@@ -118,20 +117,19 @@
 ä¿®å¤ä¸­æåä¹±ç é®é¢ ### 0.0.8--2022.1.4 - æ¯ævpkæ ¼å¼å°å¾ -
 æ¯ææ¥çæævpkæ ¼å¼æä»¶ ### 0.0.6--2022.1.3 -
 ä¿®å¤äº7zåç¼©åçæ¹å¼ï¼ä¼åä»£ç  ### 0.0.1--2022.1.3 -
 æä»¶åæ¬¡åå¸ï¼å¯ç§èæ·»å å°å¾  ## ð å¶ä» +
 æ¬äººææ¯å¾å·®ï¼å¦ææ¨æåç°BUGæèæ´å¥½çå»ºè®®ï¼æ¬¢è¿æIssue
 & Pr + å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ +
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é + [GPL-3.0 License]
-(https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/blob/
-main/LICENSE) Â©[@Umamusume-Agnes-Digital](https://github.com/Umamusume-Agnes-
-Digital)
+(https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) Â©
+[@Agnes4m](https://github.com/Agnes4m)
 ***** ð æè°¢ *****
 - [ä¿®ä»](https://github.com/s52047qwas/nonebot_plugin_xiuxian) -
 æ°æ®åºçåæ³æ¥èªäºä» - [èªå·±åçæ±çä¹è·¯æ¥è¯¢åº](https://
-github.com/Umamusume-Agnes-Digital/VSQ)(å·²å¼ç¨) - [@MeetWq](https://
-github.com/MeetWq) - éå¸¸ç­å¿è§£ç­nonebot2ç¸å³çåæ³ - [å¯ç±å°Q]
-(https://github.com/MeetWq/mybot) - æå¡å¨å¾çåæ³åèå°Qå¸®å© -
-[ç¾¤èå­¦ä¹ ](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat)
-- webæ§å¶å°çåæ³æ¥èªäºä» - [gsuid](https://github.com/KimigaiiWuyi/
+github.com/Agnes4m/VSQ)(å·²å¼ç¨) - [@MeetWq](https://github.com/MeetWq) -
+éå¸¸ç­å¿è§£ç­nonebot2ç¸å³çåæ³ - [å¯ç±å°Q](https://github.com/
+MeetWq/mybot) - æå¡å¨å¾çåæ³åèå°Qå¸®å© - [ç¾¤èå­¦ä¹ ](https://
+github.com/CMHopeSunshine/nonebot-plugin-learning-chat) -
+webæ§å¶å°çåæ³æ¥èªäºä» - [gsuid](https://github.com/KimigaiiWuyi/
 GenshinUID) - readmeåwikiçæ ¼å¼åè - åå -
 æä¾ä¸æ¹å°å¾çè¯¦ç»æ°æ®
```

### Comparing `nonebot_plugin_l4d2_server-0.4.3/setup.py` & `nonebot_plugin_l4d2_server-0.4.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,39 +22,40 @@
  'amis-python>=1.0.6,<2.0.0',
  'asyncio>=3.4.3',
  'beautifulsoup4>=4.8.0',
  'httpx>=0.23.3,<0.24.0',
  'jieba>=0.42.1,<0.43.0',
  'jinja2>=3.0.0',
  'nonebot-adapter-onebot>=2.1.5',
- 'nonebot2>=2.0.0rc3,<3.0.0',
+ 'nonebot2>=2.0.0rc4,<3.0.0',
  'nonebot_plugin_apscheduler>=0.2.0,<0.3.0',
  'nonebot_plugin_htmlrender>=0.2.0.1,<0.3.0.0',
  'nonebot_plugin_txt2img>=0.3.0',
  'pandas>=1.5.2',
  'patool>=1.12,<2.0',
  'pillow>=9.3.0,<10.0.0',
  'python-a2s>=1.3.0,<2.0.0',
+ 'python-jose>=3.3.0,<4.0.0',
  'pyunpack>=0.3.0,<0.4.0',
  'rarfile>=4.0,<5.0',
  'rcon>=2.1.0,<3.0.0',
  'ruamel.yaml>=0.17.21,<0.18.0',
  'srctools>=2.3.9,<3.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-l4d2-server',
-    'version': '0.4.3',
+    'version': '0.4.4',
     'description': 'L4D2 server related operations plugin for NoneBot2',
-    'long_description': '<div align="center">\n  <img src="https://raw.githubusercontent.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_l4d2_server\n_✨Nonebot & Left 4 Dead 2 server操作✨_\n<div align = "center">\n        <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3" target="_blank">文档</a> &nbsp; · &nbsp;\n        <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3#zl" target="_blank">指令列表</a> &nbsp; · &nbsp;\n        <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/wiki/BUG%E5%8F%8D%E9%A6%88">常见问题</a>\n</div><br>\n<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/stargazers">\n        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server" alt="stars">\n</a>\n<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/issues">\n        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server" alt="issues">\n</a>\n<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">\n        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n        <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n    <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">\n</a>\n    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n    <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">\n</div>\n\n\n## 快速使用（env示例）\n    # 复制到env文件里，没有默认就是下列值，如需修改安装下面env设置\n    # 所有的多选，用逗号隔开\n    l4_master = [\'1145149191\']\n    l4_file = [\'/home/ubuntu/l4d2/coop\']\n    l4_host = [\'127.0.0.1\']\n    l4_port = [\'20715\']\n    l4_rcon = [\'1145149191810\']\n    l4_font = \'simsun.ttc\'\n    l4_only = True\n\n\n## 新文档（暂未完成）\n\n[点击这里](https://umamusume-agnes-digital.github.io/l4d2)\n\n<h2 id="gn">主要功能</h2>\n\n- 求生服务器-本地多路径操作（传地图）\n- 批量查询指定ip服务器状态和玩家\n- 创意工坊下载和喷漆制作\n- [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)\n\n\n<h2 id="gn">如何获取key</h2>\n\n为了使得ip不被滥用，我采取这种方式管理。\n\n这并不影响正常使用，如果不需要可以忽略\n\n[点击这里加群](https://jq.qq.com/?_wv=1027&k=HdjoCcAe)并在群内发送“申请求生key”\n如果你只查询自己的服务器ip则可以忽略如下，并且更改env设置：\n\n        l4_tag = [\'呆呆\',\'橘\']      # 这里是内置可以查询的服的list对象\n        l4_key = \'qwertyuiopasdfg\'  # 这里是获取的key，是13个字符组成的字符串\n\n\n\n## 🚑  提交自己的服务器？\n\n**本项目原旨在方便自己查询管理服务器，如果你希望提供了ip**\n\n**那么我只能尽可能保证您的ip不会泄漏，如果无法承担风险则请勿提供ip**\n\n\n新增一个json文件，格式如下,文件名与需要响应的指令一致\n\n        {\n        "呆呆": [\n                {\n                "id": 1,\n                "version": "战役",\n                "ip": "43.248.188.17:27031"\n                }\n        ]\n        }\n\n<h2 id="ty">🌐 默认服务器</h2>\n目前 **已授权** 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主\n\n| 指令 | 服务器 | op | 数量 |\n|:-----:|:----:|:----:|:----:|\n| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 3\n| 云 | anne电信服云服 | 东 | 25\n| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15\n| 橘 | 橘希实香的小窝 | 橘希实香 | 13\n| 竹 | 竹烨 | 竹烨oО柠檬茶 | 9\n| 音理 | 星空列车与白的旅行 | 音理 | 3\n| 尤 | 尤尤 | 晓音 | 3\n| 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3\n| 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 1\n| Air | Air | Air | 15\n\n\n## 🔖 更新日志\n\n<details>\n<summary>展开/收起</summary>\n\n\n### 0.4.2--2022.4.9\n\n - 修复响应开头匹配出现的重大bug\n - 启用web端\n - web使用yaml管理，未来可能删除env配置\n\n### 0.4.1--2022.3\n\n - 修复rar压缩包命名错误\n - 更新了tag的参数读取方式\n - 确定了传文件私聊比群聊快速\n - 修复了电信服计算错误\n\n### 0.4.0--2022.3.27\n\n - 新增web控制台\n - 修复传图超时参数错误\n - 重写求生ip获取方法 ~ 数据库苦手 ~\n - 重写文档\n - 不再内置ip（毕竟ipv4都暴露太危险了）\n\n### 0.3.7--2022.3\n\n - 新增三方下载网盘\n - 修复windows上传临时文件错误\n - 优化查服流程\n - 优化anne服随机功能\n\n### 0.3.6--2022.3.10\n\n - 暂时关闭web端，后续修改\n - 优化图片显示\n - 修复了海量bug\n - 新增三方图查询\n\n### 0.3.5--2022.3.6\n\n - 新增ping查询（在ip里包括）\n - 新增api查询（未完成）\n - 修复了电信服查询绑定名字无法查询的错误\n - 新增了救援率的显示\n - 新增web端（未完成）\n\n### 0.3.4--2022.3.1\n\n - 新增本地插件smx查询\n - 增加了三个内置群服\n - 修改了图片的UI,变好看了\n - 删减了部分图片和字体，使得轻量化\n - 修复了海量bug\n - 修复了python3.8中typing错误\n\n### 0.3.3--2022.2.26\n\n - 重写协议，使用a2s库，同时解决win端不同报错无法输出\n - 重~抄~写服务器查询UI,解决了不好看的问题\n - 从win测试，解决了一些win特有的bug\n - 重写服务器查询~还得是json~\n - 内置服务器查询系统，可以通过[服务器简称]+[number]/[模式]来访问\n - 新增批量查询服务器，不带参数则返回图片\n\n### 0.3.1--2022.2.22\n\n - 修复了路径识别为str对象的错误\n - 修复了初始化找不到文件的错误\n - 修复了路径拼接错误\n - 在win端成功测试，修复压缩包bug\n - 新增开关协程异步env设置\n - 测试rcon建立通讯\n - 实现切换路径查看地图和使用rcon指令\n\n### 0.3.0--2022.2.18\n\n - 修改了新的env配置，使得支持本地多服务器操作\n - 彻底解决了压缩包解压linux端的问题\n - 解决了win端默认gbk解码的错误\n - 解决rcon指令字体报错\n\n### 0.2.5--2022.2.10\n\n - 修复了依赖不足的bug\n - 更新了电信服战绩个人图片UI\n - 更新了批量服务器查看的UI\n - 修改了传文件为协程异步\n - 优化了部分rcon指令\n - ~tnd7z怎么不去死啊~使用pyunpack库解压7z\n\n### 0.2.4--2022.2.8\n\n - 使用poetry修复了pip安装文件缺失的bug\n\n### 0.2.3--2022.2.7\n\n - 新增坐牢和开牢\n - 修改了获取资源为异步协程却阻碍其他指令的bug\n - 新增json统计部分已知服务器（未来应该独立成库持续更新，如果把您的非公开服记录请联系我删除）\n - 喷剂制作开摆了，推测需要c/c++环境\n - 修改抽取文案\n - 新增查询服务器状态时返回connect ip\n - 修复了服务器查询无响应的时候，因为报错无回复信息的bug\n - 个人信息重置测试代码，下个版本更新\n - 新增求生更新添加和删除\n\n### 0.2.2--2022.2.1\n\n - 新增探监\n - 新增喷漆制作\n - 修复了魔改服务器导致解包错误的bug（就是直接忽略了）\n - 修改了部分对话响应\n\n### 0.2.1--2022.1.25\n\n - 新增电信服获取（东哥的肯定）\n - 优化图片UI \n - 新增云服快捷查询\n - 修复了因为没用玩家，导致的服务器状态查询错误\n - 新增电信服ip爬取（仅仅作为单次更新ip列表）\n\n### 0.2.0--2022.1.21\n\n - 新增创意工坊查询\n - 优化查询图片UI\n - 新增创意工坊文件下载\n - 修复了因为电信服官网前端修改导致查询失败的BUG\n\n### 0.1.7--2022.1.19\n\n - 新增群ip订阅，批量查询\n - 新增图片显示ip状态\n - 修复了因为玩家名字特殊字符导致的utf-8解码错误\n - 更新自己的第三方库VSQ==0.0.6\n\n### 0.1.6--2022.1.15\n\n - 新增ip查询服务器提供玩家数量和名字\n - 增加协程函数修复因为加载顺序导致的错误\n - 更新自己的第三方库VSQ==0.0.4\n\n### 0.1.5--2022.1.15\n\n- 新增服务器控制台指令，新增依赖rcon\n- 重新了数据库，不再使用json而是使用sql3\n- 改写了求生anne信息显示方式：如果单个数据以图片显示，如果多个数据以文字显示\n\n### 0.1.4--2022.1.9\n\n- 新增求生anne详情（看排名）\n- 所有的请求改为httpx\n- 更新了anne信息图片\n- 可选使用模拟谷歌浏览器来获取anne更多数据（~有点屎了，希望大佬救救~)\n\n### 0.1.3--2022.1.7\n\n- 新增绑定昵称和steamid\n- 新增可以艾特人查询anne成绩\n- 新增解绑信息\n\n### 0.1.2--2022.1.6\n\n- 新增支持图片输出\n- 新增查询anne服数据\n\n### 0.1.1--2022.1.5\n\n- 新增删除地图\n- 新增地图改名\n- 新增支持图片输出\n\n### 0.1.0--2022.1.4\n\n- 集中修复了Bug\n\n### 0.0.9--2022.1.4\n\n- 新增上传地图后，检测对比回复新地图名字\n- 修复中文名乱码问题\n\n### 0.0.8--2022.1.4\n\n- 支持vpk格式地图\n- 支持查看所有vpk格式文件\n\n### 0.0.6--2022.1.3\n\n- 修复了7z压缩包的方式，优化代码\n\n### 0.0.1--2022.1.3\n\n- 插件初次发布，可私聊添加地图\n\n</details>\n\n## 🙈 其他\n\n+ 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr\n+ 如果本插件对你有帮助，不要忘了点个Star~\n+ 本项目仅供学习使用，请勿用于商业用途\n+ [GPL-3.0 License](https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Umamusume-Agnes-Digital](https://github.com/Umamusume-Agnes-Digital)\n        \n\n<h2 id="ty">🌐 感谢</h2>\n\n- [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian) - 数据库的写法来自于他\n- [自己写的求生之路查询库](https://github.com/Umamusume-Agnes-Digital/VSQ)(已弃用)\n- [@MeetWq](https://github.com/MeetWq) - 非常热心解答nonebot2相关的写法\n  - [可爱小Q](https://github.com/MeetWq/mybot) - 服务器图片写法参考小Q帮助\n- [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat) - web控制台的写法来自于他\n- [gsuid](https://github.com/KimigaiiWuyi/GenshinUID) - readme和wiki的格式参考\n- 呆呆 - 提供三方地图的详细数据\n',
+    'long_description': '<div align="center">\n  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_l4d2_server\n_✨Nonebot & Left 4 Dead 2 server操作✨_\n<div align = "center">\n        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3" target="_blank">文档</a> &nbsp; · &nbsp;\n        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3#zl" target="_blank">指令列表</a> &nbsp; · &nbsp;\n        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/BUG%E5%8F%8D%E9%A6%88">常见问题</a>\n</div><br>\n<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/stargazers">\n        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_l4d2_server" alt="stars">\n</a>\n<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/issues">\n        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_l4d2_server" alt="issues">\n</a>\n<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">\n        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n        <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n    <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">\n</a>\n    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n    <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">\n</div>\n\n\n## 快速使用（env示例）\n    # 复制到env文件里，没有默认就是下列值，如需修改安装下面env设置\n    # 所有的多选，用逗号隔开\n    l4_master = [\'1145149191\']\n    l4_file = [\'/home/ubuntu/l4d2/coop\']\n    l4_host = [\'127.0.0.1\']\n    l4_port = [\'20715\']\n    l4_rcon = [\'1145149191810\']\n    l4_font = \'simsun.ttc\'\n    l4_only = True\n\n\n## 新文档（暂未完成）\n\n[点击这里](https://Agnes4m.github.io/l4d2)\n\n<h2 id="gn">主要功能</h2>\n\n- 求生服务器-本地多路径操作（传地图）\n- 批量查询指定ip服务器状态和玩家\n- 创意工坊下载和喷漆制作\n- [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)\n\n\n<h2 id="gn">如何获取key</h2>\n\n为了使得ip不被滥用，我采取这种方式管理。\n\n这并不影响正常使用，如果不需要可以忽略\n\n[点击这里加群](https://jq.qq.com/?_wv=1027&k=HdjoCcAe)并在群内发送“申请求生key”\n如果你只查询自己的服务器ip则可以忽略如下，并且更改env设置：\n\n        l4_tag = [\'呆呆\',\'橘\']      # 这里是内置可以查询的服的list对象\n        l4_key = \'qwertyuiopasdfg\'  # 这里是获取的key，是13个字符组成的字符串\n\n\n\n## 🚑  提交自己的服务器？\n\n**本项目原旨在方便自己查询管理服务器，如果你希望提供了ip**\n\n**那么我只能尽可能保证您的ip不会泄漏，如果无法承担风险则请勿提供ip**\n\n\n新增一个json文件，格式如下,文件名与需要响应的指令一致\n\n        {\n        "呆呆": [\n                {\n                "id": 1,\n                "version": "战役",\n                "ip": "43.248.188.17:27031"\n                }\n        ]\n        }\n\n<h2 id="ty">🌐 默认服务器</h2>\n目前 **已授权** 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主\n\n| 指令 | 服务器 | op | 数量 |\n|:-----:|:----:|:----:|:----:|\n| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 3\n| 云 | anne电信服云服 | 东 | 25\n| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15\n| 橘 | 橘希实香的小窝 | 橘希实香 | 13\n| 竹 | 竹烨 | 竹烨oО柠檬茶 | 9\n| 音理 | 星空列车与白的旅行 | 音理 | 3\n| 尤 | 尤尤 | 晓音 | 3\n| 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3\n| 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 1\n| Air | Air | Air | 15\n\n\n## 🔖 更新日志\n\n<details>\n<summary>展开/收起</summary>\n\n\n### 0.4.4--2022.4.9\n\n- 修bug（恼）\n\n### 0.4.2--2022.4.9\n\n - 修复响应开头匹配出现的重大bug\n - 启用web端\n - web使用yaml管理，未来可能删除env配置\n\n### 0.4.1--2022.3\n\n - 修复rar压缩包命名错误\n - 更新了tag的参数读取方式\n - 确定了传文件私聊比群聊快速\n - 修复了电信服计算错误\n\n### 0.4.0--2022.3.27\n\n - 新增web控制台\n - 修复传图超时参数错误\n - 重写求生ip获取方法 ~ 数据库苦手 ~\n - 重写文档\n - 不再内置ip（毕竟ipv4都暴露太危险了）\n\n### 0.3.7--2022.3\n\n - 新增三方下载网盘\n - 修复windows上传临时文件错误\n - 优化查服流程\n - 优化anne服随机功能\n\n### 0.3.6--2022.3.10\n\n - 暂时关闭web端，后续修改\n - 优化图片显示\n - 修复了海量bug\n - 新增三方图查询\n\n### 0.3.5--2022.3.6\n\n - 新增ping查询（在ip里包括）\n - 新增api查询（未完成）\n - 修复了电信服查询绑定名字无法查询的错误\n - 新增了救援率的显示\n - 新增web端（未完成）\n\n### 0.3.4--2022.3.1\n\n - 新增本地插件smx查询\n - 增加了三个内置群服\n - 修改了图片的UI,变好看了\n - 删减了部分图片和字体，使得轻量化\n - 修复了海量bug\n - 修复了python3.8中typing错误\n\n### 0.3.3--2022.2.26\n\n - 重写协议，使用a2s库，同时解决win端不同报错无法输出\n - 重~抄~写服务器查询UI,解决了不好看的问题\n - 从win测试，解决了一些win特有的bug\n - 重写服务器查询~还得是json~\n - 内置服务器查询系统，可以通过[服务器简称]+[number]/[模式]来访问\n - 新增批量查询服务器，不带参数则返回图片\n\n### 0.3.1--2022.2.22\n\n - 修复了路径识别为str对象的错误\n - 修复了初始化找不到文件的错误\n - 修复了路径拼接错误\n - 在win端成功测试，修复压缩包bug\n - 新增开关协程异步env设置\n - 测试rcon建立通讯\n - 实现切换路径查看地图和使用rcon指令\n\n### 0.3.0--2022.2.18\n\n - 修改了新的env配置，使得支持本地多服务器操作\n - 彻底解决了压缩包解压linux端的问题\n - 解决了win端默认gbk解码的错误\n - 解决rcon指令字体报错\n\n### 0.2.5--2022.2.10\n\n - 修复了依赖不足的bug\n - 更新了电信服战绩个人图片UI\n - 更新了批量服务器查看的UI\n - 修改了传文件为协程异步\n - 优化了部分rcon指令\n - ~tnd7z怎么不去死啊~使用pyunpack库解压7z\n\n### 0.2.4--2022.2.8\n\n - 使用poetry修复了pip安装文件缺失的bug\n\n### 0.2.3--2022.2.7\n\n - 新增坐牢和开牢\n - 修改了获取资源为异步协程却阻碍其他指令的bug\n - 新增json统计部分已知服务器（未来应该独立成库持续更新，如果把您的非公开服记录请联系我删除）\n - 喷剂制作开摆了，推测需要c/c++环境\n - 修改抽取文案\n - 新增查询服务器状态时返回connect ip\n - 修复了服务器查询无响应的时候，因为报错无回复信息的bug\n - 个人信息重置测试代码，下个版本更新\n - 新增求生更新添加和删除\n\n### 0.2.2--2022.2.1\n\n - 新增探监\n - 新增喷漆制作\n - 修复了魔改服务器导致解包错误的bug（就是直接忽略了）\n - 修改了部分对话响应\n\n### 0.2.1--2022.1.25\n\n - 新增电信服获取（东哥的肯定）\n - 优化图片UI \n - 新增云服快捷查询\n - 修复了因为没用玩家，导致的服务器状态查询错误\n - 新增电信服ip爬取（仅仅作为单次更新ip列表）\n\n### 0.2.0--2022.1.21\n\n - 新增创意工坊查询\n - 优化查询图片UI\n - 新增创意工坊文件下载\n - 修复了因为电信服官网前端修改导致查询失败的BUG\n\n### 0.1.7--2022.1.19\n\n - 新增群ip订阅，批量查询\n - 新增图片显示ip状态\n - 修复了因为玩家名字特殊字符导致的utf-8解码错误\n - 更新自己的第三方库VSQ==0.0.6\n\n### 0.1.6--2022.1.15\n\n - 新增ip查询服务器提供玩家数量和名字\n - 增加协程函数修复因为加载顺序导致的错误\n - 更新自己的第三方库VSQ==0.0.4\n\n### 0.1.5--2022.1.15\n\n- 新增服务器控制台指令，新增依赖rcon\n- 重新了数据库，不再使用json而是使用sql3\n- 改写了求生anne信息显示方式：如果单个数据以图片显示，如果多个数据以文字显示\n\n### 0.1.4--2022.1.9\n\n- 新增求生anne详情（看排名）\n- 所有的请求改为httpx\n- 更新了anne信息图片\n- 可选使用模拟谷歌浏览器来获取anne更多数据（~有点屎了，希望大佬救救~)\n\n### 0.1.3--2022.1.7\n\n- 新增绑定昵称和steamid\n- 新增可以艾特人查询anne成绩\n- 新增解绑信息\n\n### 0.1.2--2022.1.6\n\n- 新增支持图片输出\n- 新增查询anne服数据\n\n### 0.1.1--2022.1.5\n\n- 新增删除地图\n- 新增地图改名\n- 新增支持图片输出\n\n### 0.1.0--2022.1.4\n\n- 集中修复了Bug\n\n### 0.0.9--2022.1.4\n\n- 新增上传地图后，检测对比回复新地图名字\n- 修复中文名乱码问题\n\n### 0.0.8--2022.1.4\n\n- 支持vpk格式地图\n- 支持查看所有vpk格式文件\n\n### 0.0.6--2022.1.3\n\n- 修复了7z压缩包的方式，优化代码\n\n### 0.0.1--2022.1.3\n\n- 插件初次发布，可私聊添加地图\n\n</details>\n\n## 🙈 其他\n\n+ 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr\n+ 如果本插件对你有帮助，不要忘了点个Star~\n+ 本项目仅供学习使用，请勿用于商业用途\n+ [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)\n        \n\n<h2 id="ty">🌐 感谢</h2>\n\n- [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian) - 数据库的写法来自于他\n- [自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)(已弃用)\n- [@MeetWq](https://github.com/MeetWq) - 非常热心解答nonebot2相关的写法\n  - [可爱小Q](https://github.com/MeetWq/mybot) - 服务器图片写法参考小Q帮助\n- [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat) - web控制台的写法来自于他\n- [gsuid](https://github.com/KimigaiiWuyi/GenshinUID) - readme和wiki的格式参考\n- 呆呆 - 提供三方地图的详细数据\n',
     'author': 'Agnes_Digital',
     'author_email': 'Z735803792@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server',
+    'url': 'https://github.com/Agnes4m/nonebot_plugin_l4d2_server',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -5,23 +5,23 @@
 'nonebot_plugin_l4d2_server.l4d2_queries',
 'nonebot_plugin_l4d2_server.l4d2_server',
 'nonebot_plugin_l4d2_server.l4d2_web'] package_data = \ {'': ['*'],
 'nonebot_plugin_l4d2_server': ['data/L4D2/image/head/*', 'data/L4D2/image/
 header/*', 'data/L4D2/image/template/*']} install_requires = \
 ['aiohttp>=3.8.3,<4.0.0', 'amis-python>=1.0.6,<2.0.0', 'asyncio>=3.4.3',
 'beautifulsoup4>=4.8.0', 'httpx>=0.23.3,<0.24.0', 'jieba>=0.42.1,<0.43.0',
-'jinja2>=3.0.0', 'nonebot-adapter-onebot>=2.1.5', 'nonebot2>=2.0.0rc3,<3.0.0',
+'jinja2>=3.0.0', 'nonebot-adapter-onebot>=2.1.5', 'nonebot2>=2.0.0rc4,<3.0.0',
 'nonebot_plugin_apscheduler>=0.2.0,<0.3.0',
 'nonebot_plugin_htmlrender>=0.2.0.1,<0.3.0.0', 'nonebot_plugin_txt2img>=0.3.0',
 'pandas>=1.5.2', 'patool>=1.12,<2.0', 'pillow>=9.3.0,<10.0.0', 'python-
-a2s>=1.3.0,<2.0.0', 'pyunpack>=0.3.0,<0.4.0', 'rarfile>=4.0,<5.0',
-'rcon>=2.1.0,<3.0.0', 'ruamel.yaml>=0.17.21,<0.18.0', 'srctools>=2.3.9,<3.0.0']
-setup_kwargs = { 'name': 'nonebot-plugin-l4d2-server', 'version': '0.4.3',
-'description': 'L4D2 server related operations plugin for NoneBot2',
-'long_description': '
+a2s>=1.3.0,<2.0.0', 'python-jose>=3.3.0,<4.0.0', 'pyunpack>=0.3.0,<0.4.0',
+'rarfile>=4.0,<5.0', 'rcon>=2.1.0,<3.0.0', 'ruamel.yaml>=0.17.21,<0.18.0',
+'srctools>=2.3.9,<3.0.0'] setup_kwargs = { 'name': 'nonebot-plugin-l4d2-
+server', 'version': '0.4.4', 'description': 'L4D2 server related operations
+plugin for NoneBot2', 'long_description': '
                            \n [AgnesDigitalLogo]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n
          \n\n# nonebot_plugin_l4d2_server\n_â¨Nonebot & Left 4 Dead 2
                               serveræä½â¨_\n
@@ -31,15 +31,15 @@
             [pypi]\n\n\n_[pypi_download]\n\n [python]\n [NoneBot]\n
 \n\n\n## å¿«éä½¿ç¨ï¼envç¤ºä¾ï¼\n #
 å¤å¶å°envæä»¶éï¼æ²¡æé»è®¤å°±æ¯ä¸åå¼ï¼å¦éä¿®æ¹å®è£ä¸é¢envè®¾ç½®\n
 # ææçå¤éï¼ç¨éå·éå¼\n l4_master = [\'1145149191\']\n l4_file =
 [\'/home/ubuntu/l4d2/coop\']\n l4_host = [\'127.0.0.1\']\n l4_port =
 [\'20715\']\n l4_rcon = [\'1145149191810\']\n l4_font = \'simsun.ttc\'\n
 l4_only = True\n\n\n## æ°ææ¡£ï¼ææªå®æï¼\n\n[ç¹å»è¿é](https://
-umamusume-agnes-digital.github.io/l4d2)\n\n
+Agnes4m.github.io/l4d2)\n\n
 ***** ä¸»è¦åè½ *****
 \n\n- æ±çæå¡å¨-æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼\n-
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶\n-
 åæå·¥åä¸è½½åå·æ¼å¶ä½\n- [æ±ççµä¿¡æanne](https://github.com/
 fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/l4d_stats/
 ranking/index.php)\n\n\n
 ***** å¦ä½è·åkey *****
@@ -58,15 +58,16 @@
 æä»¤ | æå¡å¨ | op | æ°é |\n|:-----:|:----:|:----:|:----:|\n| æ°ç  |
 ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 3\n| äº | anneçµä¿¡æäºæ | ä¸
 | 25\n| åå | ååçå°çª | æè«å¤§é­ç | 15\n| æ© |
 æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 13\n| ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶
 | 9\n| é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3\n| å°¤ | å°¤å°¤ |
 æé³ | 3\n| é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3\n| ææ |
 ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿ | å¤æå°æ | 1\n| Air | Air | Air |
-15\n\n\n## ð æ´æ°æ¥å¿\n\n\nå±å¼/æ¶èµ·\n\n\n### 0.4.2--2022.4.9\n\n -
+15\n\n\n## ð æ´æ°æ¥å¿\n\n\nå±å¼/æ¶èµ·\n\n\n### 0.4.4--2022.4.9\n\n-
+ä¿®bugï¼æ¼ï¼\n\n### 0.4.2--2022.4.9\n\n -
 ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug\n - å¯ç¨webç«¯\n -
 webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½®\n\n### 0.4.1--2022.3\n\n -
 ä¿®å¤raråç¼©åå½åéè¯¯\n - æ´æ°äºtagçåæ°è¯»åæ¹å¼\n -
 ç¡®å®äºä¼ æä»¶ç§èæ¯ç¾¤èå¿«é\n -
 ä¿®å¤äºçµä¿¡æè®¡ç®éè¯¯\n\n### 0.4.0--2022.3.27\n\n -
 æ°å¢webæ§å¶å°\n - ä¿®å¤ä¼ å¾è¶æ¶åæ°éè¯¯\n -
 éåæ±çipè·åæ¹æ³ ~ æ°æ®åºè¦æ ~\n - éåææ¡£\n -
@@ -145,25 +146,23 @@
 æ¯ævpkæ ¼å¼å°å¾\n- æ¯ææ¥çæævpkæ ¼å¼æä»¶\n\n### 0.0.6--
 2022.1.3\n\n- ä¿®å¤äº7zåç¼©åçæ¹å¼ï¼ä¼åä»£ç \n\n### 0.0.1--
 2022.1.3\n\n- æä»¶åæ¬¡åå¸ï¼å¯ç§èæ·»å å°å¾\n\n\n\n## ð
 å¶ä»\n\n+
 æ¬äººææ¯å¾å·®ï¼å¦ææ¨æåç°BUGæèæ´å¥½çå»ºè®®ï¼æ¬¢è¿æIssue
 & Pr\n+ å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~\n+
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é\n+ [GPL-3.0 License]
-(https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/blob/
-main/LICENSE) Â©[@Umamusume-Agnes-Digital](https://github.com/Umamusume-Agnes-
-Digital)\n \n\n
+(https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) Â©
+[@Agnes4m](https://github.com/Agnes4m)\n \n\n
 ***** ð æè°¢ *****
 \n\n- [ä¿®ä»](https://github.com/s52047qwas/nonebot_plugin_xiuxian) -
 æ°æ®åºçåæ³æ¥èªäºä»\n- [èªå·±åçæ±çä¹è·¯æ¥è¯¢åº](https://
-github.com/Umamusume-Agnes-Digital/VSQ)(å·²å¼ç¨)\n- [@MeetWq](https://
-github.com/MeetWq) - éå¸¸ç­å¿è§£ç­nonebot2ç¸å³çåæ³\n - [å¯ç±å°Q]
-(https://github.com/MeetWq/mybot) - æå¡å¨å¾çåæ³åèå°Qå¸®å©\n-
-[ç¾¤èå­¦ä¹ ](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat)
-- webæ§å¶å°çåæ³æ¥èªäºä»\n- [gsuid](https://github.com/KimigaiiWuyi/
+github.com/Agnes4m/VSQ)(å·²å¼ç¨)\n- [@MeetWq](https://github.com/MeetWq) -
+éå¸¸ç­å¿è§£ç­nonebot2ç¸å³çåæ³\n - [å¯ç±å°Q](https://github.com/
+MeetWq/mybot) - æå¡å¨å¾çåæ³åèå°Qå¸®å©\n- [ç¾¤èå­¦ä¹ ](https:/
+/github.com/CMHopeSunshine/nonebot-plugin-learning-chat) -
+webæ§å¶å°çåæ³æ¥èªäºä»\n- [gsuid](https://github.com/KimigaiiWuyi/
 GenshinUID) - readmeåwikiçæ ¼å¼åè\n- åå -
 æä¾ä¸æ¹å°å¾çè¯¦ç»æ°æ®\n', 'author': 'Agnes_Digital',
 'author_email': 'Z735803792@163.com', 'maintainer': 'None', 'maintainer_email':
-'None', 'url': 'https://github.com/Umamusume-Agnes-Digital/
-nonebot_plugin_l4d2_server', 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'python_requires':
-'>=3.8,<4.0', } setup(**setup_kwargs)
+'None', 'url': 'https://github.com/Agnes4m/nonebot_plugin_l4d2_server',
+'packages': packages, 'package_data': package_data, 'install_requires':
+install_requires, 'python_requires': '>=3.9,<4.0', } setup(**setup_kwargs)
```

### Comparing `nonebot_plugin_l4d2_server-0.4.3/PKG-INFO` & `nonebot_plugin_l4d2_server-0.4.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.4.3
+Version: 0.4.4
 Summary: L4D2 server related operations plugin for NoneBot2
-Home-page: https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server
+Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -25,50 +24,51 @@
 Requires-Dist: amis-python (>=1.0.6,<2.0.0)
 Requires-Dist: asyncio (>=3.4.3)
 Requires-Dist: beautifulsoup4 (>=4.8.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: jieba (>=0.42.1,<0.43.0)
 Requires-Dist: jinja2 (>=3.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.5)
-Requires-Dist: nonebot2 (>=2.0.0rc3,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
 Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: nonebot_plugin_htmlrender (>=0.2.0.1,<0.3.0.0)
 Requires-Dist: nonebot_plugin_txt2img (>=0.3.0)
 Requires-Dist: pandas (>=1.5.2)
 Requires-Dist: patool (>=1.12,<2.0)
 Requires-Dist: pillow (>=9.3.0,<10.0.0)
 Requires-Dist: python-a2s (>=1.3.0,<2.0.0)
+Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Requires-Dist: pyunpack (>=0.3.0,<0.4.0)
 Requires-Dist: rarfile (>=4.0,<5.0)
 Requires-Dist: rcon (>=2.1.0,<3.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: srctools (>=2.3.9,<3.0.0)
-Project-URL: Repository, https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server
+Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 Description-Content-Type: text/markdown
 
 <div align="center">
-  <img src="https://raw.githubusercontent.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
+  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
   <br>
   <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
 # nonebot_plugin_l4d2_server
 _✨Nonebot & Left 4 Dead 2 server操作✨_
 <div align = "center">
-        <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3" target="_blank">文档</a> &nbsp; · &nbsp;
-        <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3#zl" target="_blank">指令列表</a> &nbsp; · &nbsp;
-        <a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/wiki/BUG%E5%8F%8D%E9%A6%88">常见问题</a>
+        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3" target="_blank">文档</a> &nbsp; · &nbsp;
+        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/%E6%96%87%E6%A1%A3#zl" target="_blank">指令列表</a> &nbsp; · &nbsp;
+        <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/wiki/BUG%E5%8F%8D%E9%A6%88">常见问题</a>
 </div><br>
-<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/stargazers">
-        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server" alt="stars">
+<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/stargazers">
+        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_l4d2_server" alt="stars">
 </a>
-<a href="https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/issues">
-        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server" alt="issues">
+<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/issues">
+        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_l4d2_server" alt="issues">
 </a>
 <a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">
         <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">
         <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">
 </a>
@@ -90,15 +90,15 @@
     l4_rcon = ['1145149191810']
     l4_font = 'simsun.ttc'
     l4_only = True
 
 
 ## 新文档（暂未完成）
 
-[点击这里](https://umamusume-agnes-digital.github.io/l4d2)
+[点击这里](https://Agnes4m.github.io/l4d2)
 
 <h2 id="gn">主要功能</h2>
 
 - 求生服务器-本地多路径操作（传地图）
 - 批量查询指定ip服务器状态和玩家
 - 创意工坊下载和喷漆制作
 - [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)
@@ -156,14 +156,18 @@
 
 ## 🔖 更新日志
 
 <details>
 <summary>展开/收起</summary>
 
 
+### 0.4.4--2022.4.9
+
+- 修bug（恼）
+
 ### 0.4.2--2022.4.9
 
  - 修复响应开头匹配出现的重大bug
  - 启用web端
  - web使用yaml管理，未来可能删除env配置
 
 ### 0.4.1--2022.3
@@ -353,20 +357,20 @@
 </details>
 
 ## 🙈 其他
 
 + 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr
 + 如果本插件对你有帮助，不要忘了点个Star~
 + 本项目仅供学习使用，请勿用于商业用途
-+ [GPL-3.0 License](https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Umamusume-Agnes-Digital](https://github.com/Umamusume-Agnes-Digital)
++ [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
         
 
 <h2 id="ty">🌐 感谢</h2>
 
 - [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian) - 数据库的写法来自于他
-- [自己写的求生之路查询库](https://github.com/Umamusume-Agnes-Digital/VSQ)(已弃用)
+- [自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)(已弃用)
 - [@MeetWq](https://github.com/MeetWq) - 非常热心解答nonebot2相关的写法
   - [可爱小Q](https://github.com/MeetWq/mybot) - 服务器图片写法参考小Q帮助
 - [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat) - web控制台的写法来自于他
 - [gsuid](https://github.com/KimigaiiWuyi/GenshinUID) - readme和wiki的格式参考
 - 呆呆 - 提供三方地图的详细数据
```

#### html2text {}

```diff
@@ -1,48 +1,47 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.4.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.4.4 Summary:
 L4D2 server related operations plugin for NoneBot2 Home-page: https://
-github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server License: GPLv3
-Keywords: steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
-Z735803792@163.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
+github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
+steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
+Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Requires-Dist: aiohttp (>=3.8.3,<4.0.0) Requires-
-Dist: amis-python (>=1.0.6,<2.0.0) Requires-Dist: asyncio (>=3.4.3) Requires-
-Dist: beautifulsoup4 (>=4.8.0) Requires-Dist: httpx (>=0.23.3,<0.24.0)
-Requires-Dist: jieba (>=0.42.1,<0.43.0) Requires-Dist: jinja2 (>=3.0.0)
-Requires-Dist: nonebot-adapter-onebot (>=2.1.5) Requires-Dist: nonebot2
-(>=2.0.0rc3,<3.0.0) Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
-Requires-Dist: nonebot_plugin_htmlrender (>=0.2.0.1,<0.3.0.0) Requires-Dist:
-nonebot_plugin_txt2img (>=0.3.0) Requires-Dist: pandas (>=1.5.2) Requires-Dist:
-patool (>=1.12,<2.0) Requires-Dist: pillow (>=9.3.0,<10.0.0) Requires-Dist:
-python-a2s (>=1.3.0,<2.0.0) Requires-Dist: pyunpack (>=0.3.0,<0.4.0) Requires-
-Dist: rarfile (>=4.0,<5.0) Requires-Dist: rcon (>=2.1.0,<3.0.0) Requires-Dist:
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Requires-Dist: aiohttp
+(>=3.8.3,<4.0.0) Requires-Dist: amis-python (>=1.0.6,<2.0.0) Requires-Dist:
+asyncio (>=3.4.3) Requires-Dist: beautifulsoup4 (>=4.8.0) Requires-Dist: httpx
+(>=0.23.3,<0.24.0) Requires-Dist: jieba (>=0.42.1,<0.43.0) Requires-Dist:
+jinja2 (>=3.0.0) Requires-Dist: nonebot-adapter-onebot (>=2.1.5) Requires-Dist:
+nonebot2 (>=2.0.0rc4,<3.0.0) Requires-Dist: nonebot_plugin_apscheduler
+(>=0.2.0,<0.3.0) Requires-Dist: nonebot_plugin_htmlrender (>=0.2.0.1,<0.3.0.0)
+Requires-Dist: nonebot_plugin_txt2img (>=0.3.0) Requires-Dist: pandas (>=1.5.2)
+Requires-Dist: patool (>=1.12,<2.0) Requires-Dist: pillow (>=9.3.0,<10.0.0)
+Requires-Dist: python-a2s (>=1.3.0,<2.0.0) Requires-Dist: python-jose
+(>=3.3.0,<4.0.0) Requires-Dist: pyunpack (>=0.3.0,<0.4.0) Requires-Dist:
+rarfile (>=4.0,<5.0) Requires-Dist: rcon (>=2.1.0,<3.0.0) Requires-Dist:
 ruamel.yaml (>=0.17.21,<0.18.0) Requires-Dist: srctools (>=2.3.9,<3.0.0)
-Project-URL: Repository, https://github.com/Umamusume-Agnes-Digital/
-nonebot_plugin_l4d2_server Description-Content-Type: text/markdown
+Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_l4d2_server
+Description-Content-Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
    # nonebot_plugin_l4d2_server _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
                 ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
 
 [GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
                                    [NoneBot]
 ## å¿«éä½¿ç¨ï¼envç¤ºä¾ï¼ #
 å¤å¶å°envæä»¶éï¼æ²¡æé»è®¤å°±æ¯ä¸åå¼ï¼å¦éä¿®æ¹å®è£ä¸é¢envè®¾ç½®
 # ææçå¤éï¼ç¨éå·éå¼ l4_master = ['1145149191'] l4_file = ['/
 home/ubuntu/l4d2/coop'] l4_host = ['127.0.0.1'] l4_port = ['20715'] l4_rcon =
 ['1145149191810'] l4_font = 'simsun.ttc' l4_only = True ##
-æ°ææ¡£ï¼ææªå®æï¼ [ç¹å»è¿é](https://umamusume-agnes-
-digital.github.io/l4d2)
+æ°ææ¡£ï¼ææªå®æï¼ [ç¹å»è¿é](https://Agnes4m.github.io/l4d2)
 ***** ä¸»è¦åè½ *****
 - æ±çæå¡å¨-æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
 æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶ -
 åæå·¥åä¸è½½åå·æ¼å¶ä½ - [æ±ççµä¿¡æanne](https://github.com/
 fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/l4d_stats/
 ranking/index.php)
 ***** å¦ä½è·åkey *****
@@ -64,16 +63,16 @@
 æä»¤ | æå¡å¨ | op | æ°é | |:-----:|:----:|:----:|:----:| | æ°ç  |
 ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 3 | äº | anneçµä¿¡æäºæ | ä¸ |
 25 | åå | ååçå°çª | æè«å¤§é­ç | 15 | æ© |
 æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 13 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ |
 9 | é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³ |
 3 | é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3 | ææ |
 ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿ | å¤æå°æ | 1 | Air | Air | Air | 15
-## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.4.2--2022.4.9 -
-ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug - å¯ç¨webç«¯ -
+## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.4.4--2022.4.9 - ä¿®bugï¼æ¼ï¼ ###
+0.4.2--2022.4.9 - ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug - å¯ç¨webç«¯ -
 webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½® ### 0.4.1--2022.3 -
 ä¿®å¤raråç¼©åå½åéè¯¯ - æ´æ°äºtagçåæ°è¯»åæ¹å¼ -
 ç¡®å®äºä¼ æä»¶ç§èæ¯ç¾¤èå¿«é - ä¿®å¤äºçµä¿¡æè®¡ç®éè¯¯ ###
 0.4.0--2022.3.27 - æ°å¢webæ§å¶å° - ä¿®å¤ä¼ å¾è¶æ¶åæ°éè¯¯ -
 éåæ±çipè·åæ¹æ³ ~ æ°æ®åºè¦æ ~ - éåææ¡£ -
 ä¸ååç½®ipï¼æ¯ç«ipv4é½æ´é²å¤ªå±é©äºï¼ ### 0.3.7--2022.3 -
 æ°å¢ä¸æ¹ä¸è½½ç½ç - ä¿®å¤windowsä¸ä¼ ä¸´æ¶æä»¶éè¯¯ -
@@ -145,20 +144,19 @@
 ä¿®å¤ä¸­æåä¹±ç é®é¢ ### 0.0.8--2022.1.4 - æ¯ævpkæ ¼å¼å°å¾ -
 æ¯ææ¥çæævpkæ ¼å¼æä»¶ ### 0.0.6--2022.1.3 -
 ä¿®å¤äº7zåç¼©åçæ¹å¼ï¼ä¼åä»£ç  ### 0.0.1--2022.1.3 -
 æä»¶åæ¬¡åå¸ï¼å¯ç§èæ·»å å°å¾  ## ð å¶ä» +
 æ¬äººææ¯å¾å·®ï¼å¦ææ¨æåç°BUGæèæ´å¥½çå»ºè®®ï¼æ¬¢è¿æIssue
 & Pr + å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ +
 æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é + [GPL-3.0 License]
-(https://github.com/Umamusume-Agnes-Digital/nonebot_plugin_l4d2_server/blob/
-main/LICENSE) Â©[@Umamusume-Agnes-Digital](https://github.com/Umamusume-Agnes-
-Digital)
+(https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) Â©
+[@Agnes4m](https://github.com/Agnes4m)
 ***** ð æè°¢ *****
 - [ä¿®ä»](https://github.com/s52047qwas/nonebot_plugin_xiuxian) -
 æ°æ®åºçåæ³æ¥èªäºä» - [èªå·±åçæ±çä¹è·¯æ¥è¯¢åº](https://
-github.com/Umamusume-Agnes-Digital/VSQ)(å·²å¼ç¨) - [@MeetWq](https://
-github.com/MeetWq) - éå¸¸ç­å¿è§£ç­nonebot2ç¸å³çåæ³ - [å¯ç±å°Q]
-(https://github.com/MeetWq/mybot) - æå¡å¨å¾çåæ³åèå°Qå¸®å© -
-[ç¾¤èå­¦ä¹ ](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat)
-- webæ§å¶å°çåæ³æ¥èªäºä» - [gsuid](https://github.com/KimigaiiWuyi/
+github.com/Agnes4m/VSQ)(å·²å¼ç¨) - [@MeetWq](https://github.com/MeetWq) -
+éå¸¸ç­å¿è§£ç­nonebot2ç¸å³çåæ³ - [å¯ç±å°Q](https://github.com/
+MeetWq/mybot) - æå¡å¨å¾çåæ³åèå°Qå¸®å© - [ç¾¤èå­¦ä¹ ](https://
+github.com/CMHopeSunshine/nonebot-plugin-learning-chat) -
+webæ§å¶å°çåæ³æ¥èªäºä» - [gsuid](https://github.com/KimigaiiWuyi/
 GenshinUID) - readmeåwikiçæ ¼å¼åè - åå -
 æä¾ä¸æ¹å°å¾çè¯¦ç»æ°æ®
```

