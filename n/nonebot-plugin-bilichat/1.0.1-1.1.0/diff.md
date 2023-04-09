# Comparing `tmp/nonebot_plugin_bilichat-1.0.1.tar.gz` & `tmp/nonebot_plugin_bilichat-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-1.0.1.tar", last modified: Sat Apr  8 11:25:51 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-1.1.0.tar", last modified: Sun Apr  9 10:45:51 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-1.0.1.tar` & `nonebot_plugin_bilichat-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    34523 2023-04-08 11:25:42.981399 nonebot_plugin_bilichat-1.0.1/LICENSE
--rw-r--r--   0        0        0     5642 2023-04-08 11:25:42.981399 nonebot_plugin_bilichat-1.0.1/README.md
--rw-r--r--   0        0        0     6258 2023-04-08 11:25:42.989399 nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     3376 2023-04-08 11:25:42.989399 nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-04-08 11:25:42.989399 nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6286 2023-04-08 11:25:42.989399 nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4606 2023-04-08 11:25:42.989399 nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      927 2023-04-08 11:25:42.989399 nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     4430 2023-04-08 11:25:42.989399 nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     9008 2023-04-08 11:25:42.989399 nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3838 2023-04-08 11:25:42.989399 nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      288 2023-04-08 11:25:42.989399 nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1867 2023-04-08 11:25:42.989399 nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     3677 2023-04-08 11:25:42.989399 nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0     2910 2023-04-08 11:25:42.989399 nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0      864 2023-04-08 11:25:42.989399 nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0       93 2023-04-08 11:25:42.989399 nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      148 2023-04-08 11:25:42.989399 nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      259 2023-04-08 11:25:42.989399 nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0     2326 2023-04-08 11:25:42.989399 nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/summary/content_summarise.py
--rw-r--r--   0        0        0     4472 2023-04-08 11:25:42.989399 nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     1794 2023-04-08 11:25:42.989399 nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1098 2023-04-08 11:25:51.429412 nonebot_plugin_bilichat-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6462 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-09 10:45:43.254714 nonebot_plugin_bilichat-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5965 2023-04-09 10:45:43.258714 nonebot_plugin_bilichat-1.1.0/README.md
+-rw-r--r--   0        0        0     8383 2023-04-09 10:45:43.262714 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4125 2023-04-09 10:45:43.262714 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-04-09 10:45:43.262714 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4592 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      927 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     4408 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3800 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      289 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     3678 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0     2854 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0      866 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0       93 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      148 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0     2212 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/summary/content_summarise.py
+-rw-r--r--   0        0        0     4388 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     1764 2023-04-09 10:45:43.266713 nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1098 2023-04-09 10:45:51.690604 nonebot_plugin_bilichat-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6785 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-1.0.1/LICENSE` & `nonebot_plugin_bilichat-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.0.1/README.md` & `nonebot_plugin_bilichat-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -109,28 +109,30 @@
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的配置, 配置均为**非必须项**
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| bilichat_block              | bool      | False              | 是否拦截事件(防止其他插件二次解析) |
-| bilichat_enable_private     | bool      | True               | 是否允许响应私聊 |
-| bilichat_enable_v12_channel | bool      | True               | 是否允许响应频道消息(ob12专属) |
-| bilichat_enable_unkown_src  | bool      | False              | 是否允许响应未知来源的消息 |
-| bilichat_whitelist          | list[str] | []                 | **响应**的群聊(频道)名单, 会覆盖黑名单 |
-| bilichat_blacklist          | list[str] | []                 | **不响应**的群聊(频道)名单 |
-| bilichat_dynamic_font       | str       | None               | 视频信息及词云图片使用的字体 |
-| bilichat_cd_time            | int       | 120                | 对同一视频的响应冷却时间(防止刷屏) |
-| bilichat_use_bcut_asr       | bool      | True               | 是否在**没有字幕时**调用必剪接口生成字幕 |
-| bilichat_word_cloud         | bool      | True               | 是否开启词云功能 |
-| bilichat_openai_token       | str       | None               | openai的apikey, 若留空则禁用AI总结 |
-| bilichat_openai_proxy       | str       | None               | 访问openai使用的代理地址 |
-| bilichat_openai_model       | str       | gpt-3.5-turbo-0301 | 使用的语言模型名称 |
-| bilichat_openai_token_limit | int       | 3500               | 请求的文本量上限, 计算方式可参考[tiktoken](https://github.com/openai/tiktoken) |
+| bilichat_block              | bool      | False                | 是否拦截事件(防止其他插件二次解析) |
+| bilichat_enable_private     | bool      | True                 | 是否允许响应私聊 |
+| bilichat_enable_v12_channel | bool      | True                 | 是否允许响应频道消息(ob12专属) |
+| bilichat_enable_unkown_src  | bool      | False                | 是否允许响应未知来源的消息 |
+| bilichat_whitelist          | list[str] | []                   | **响应**的群聊(频道)名单, 会覆盖黑名单 |
+| bilichat_blacklist          | list[str] | []                   | **不响应**的群聊(频道)名单 |
+| bilichat_dynamic_font       | str       | None                 | 视频信息及词云图片使用的字体 |
+| bilichat_cd_time            | int       | 120                  | 对同一视频的响应冷却时间(防止刷屏) |
+| bilichat_forword_msg        | set[str]  | ()                   | 对什么类型的消息开启合并转发(ob11专属),包含 `info`、`wordcloud`、`summary` 三个可选项 |
+| nickname                    | set[str]  | ("awesome-nonebot",) | 合并转发中,bot的昵称(取第一个值) |
+| bilichat_use_bcut_asr       | bool      | True                 | 是否在**没有字幕时**调用必剪接口生成字幕 |
+| bilichat_word_cloud         | bool      | True                 | 是否开启词云功能 |
+| bilichat_openai_token       | str       | None                 | openai的apikey, 若留空则禁用AI总结 |
+| bilichat_openai_proxy       | str       | None                 | 访问openai使用的代理地址 |
+| bilichat_openai_model       | str       | gpt-3.5-turbo-0301   | 使用的语言模型名称 |
+| bilichat_openai_token_limit | int       | 3500                 | 请求的文本量上限, 计算方式可参考[tiktoken](https://github.com/openai/tiktoken) |
 
 ## 🎉 使用
 
 直接发送视频(专栏)链接即可
 
 ### 指令表
```

#### html2text {}

```diff
@@ -35,15 +35,19 @@
 æ¯å¦åè®¸ååºç§è | | bilichat_enable_v12_channel | bool | True |
 æ¯å¦åè®¸ååºé¢éæ¶æ¯(ob12ä¸å±) | | bilichat_enable_unkown_src |
 bool | False | æ¯å¦åè®¸ååºæªç¥æ¥æºçæ¶æ¯ | | bilichat_whitelist |
 list[str] | [] | **ååº**çç¾¤è(é¢é)åå, ä¼è¦çé»åå | |
 bilichat_blacklist | list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
 bilichat_dynamic_font | str | None | è§é¢ä¿¡æ¯åè¯äºå¾çä½¿ç¨çå­ä½
 | | bilichat_cd_time | int | 120 | å¯¹åä¸è§é¢çååºå·å´æ¶é´
-(é²æ­¢å·å±) | | bilichat_use_bcut_asr | bool | True |
+(é²æ­¢å·å±) | | bilichat_forword_msg | set[str] | () |
+å¯¹ä»ä¹ç±»åçæ¶æ¯å¼å¯åå¹¶è½¬å(ob11ä¸å±),åå«
+`info`ã`wordcloud`ã`summary` ä¸ä¸ªå¯éé¡¹ | | nickname | set[str] |
+("awesome-nonebot",) | åå¹¶è½¬åä¸­,botçæµç§°(åç¬¬ä¸ä¸ªå¼) | |
+bilichat_use_bcut_asr | bool | True |
 æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | |
 bilichat_word_cloud | bool | True | æ¯å¦å¼å¯è¯äºåè½ | |
 bilichat_openai_token | str | None | openaiçapikey,
 è¥çç©ºåç¦ç¨AIæ»ç» | | bilichat_openai_proxy | str | None |
 è®¿é®openaiä½¿ç¨çä»£çå°å | | bilichat_openai_model | str | gpt-3.5-
 turbo-0301 | ä½¿ç¨çè¯­è¨æ¨¡ååç§° | | bilichat_openai_token_limit | int
 | 3500 | è¯·æ±çææ¬éä¸é, è®¡ç®æ¹å¼å¯åè[tiktoken](https://
```

### Comparing `nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import re
 from typing import Union
 
+from nonebot.adapters.onebot.v11 import Bot as V11_Bot
 from nonebot.adapters.onebot.v11 import GroupMessageEvent as V11_GME
+from nonebot.adapters.onebot.v11 import Message as V11_Message
 from nonebot.adapters.onebot.v11 import MessageEvent as V11_ME
 from nonebot.adapters.onebot.v11 import MessageSegment as V11_MS
 from nonebot.adapters.onebot.v11 import PrivateMessageEvent as V11_PME
 from nonebot.adapters.onebot.v12 import Bot as V12_Bot
 from nonebot.adapters.onebot.v12 import ChannelMessageEvent as V12_CME
 from nonebot.adapters.onebot.v12 import GroupMessageEvent as V12_GME
 from nonebot.adapters.onebot.v12 import MessageEvent as V12_ME
 from nonebot.adapters.onebot.v12 import MessageSegment as V12_MS
 from nonebot.adapters.onebot.v12 import PrivateMessageEvent as V12_PME
 from nonebot.consts import REGEX_GROUP, REGEX_STR
+from nonebot.exception import FinishedException
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.plugin import PluginMetadata, on_regex
 from nonebot.rule import Rule
 from nonebot.typing import T_State
 
 from .config import __version__, plugin_config
@@ -30,15 +33,15 @@
     from .wordcloud.wordcloud import wordcloud
 
 __plugin_meta__ = PluginMetadata(
     name="nonebot-plugin-bilichat",
     description="一个通过 OpenAI 来对b站视频进行总结插件",
     usage="直接发送视频链接即可",
     extra={
-        "author": "djkcyl",
+        "author": "djkcyl & Well404",
         "version": __version__,
         "priority": 1,
     },
 )
 
 
 async def _bili_check(event: Union[V11_ME, V12_ME], state: T_State):
@@ -79,78 +82,134 @@
 
 @b23.handle()
 async def get_bili_number_b23(state: T_State):
     if matched := re.search(r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})", await b23_extract(state[REGEX_GROUP])):  # type: ignore
         state["bili_number"] = matched.group()
 
 
+async def forword_msg_v11(bot: V11_Bot, event: V11_ME, forword_list: V11_Message):
+    msgs = [
+        {"type": "node", "data": {"name": plugin_config.nickname[0], "uin": bot.self_id, "content": msg}}
+        for msg in forword_list
+    ]
+    if isinstance(event, V11_GME):
+        await bot.send_group_forward_msg(id=str(event.group_id), messages=msgs)
+    else:
+        await bot.send_private_forward_msg(id=str(event.user_id), messages=msgs)
+    raise FinishedException
+
+
 @bili.handle()
 @b23.handle()
-async def video_info_v11(event: V11_ME, state: T_State, matcher: Matcher):
+async def video_info_v11(bot: V11_Bot, event: V11_ME, state: T_State, matcher: Matcher):
+    forword_list = []
     # basic info
     msg, img, info = await get_video_basic(state["bili_number"], state["_uid_"])
     if not msg or not info:
         await matcher.finish()
     reply = V11_MS.reply(event.message_id)
     if not img:
         await matcher.finish(reply + msg)
     image = V11_MS.image(img)
-    msgid = (await matcher.send(reply + image + msg))["message_id"]
-    # furtuer fuctions
-    if plugin_config.bilichat_openai_token or plugin_config.bilichat_word_cloud:
+    if "info" in plugin_config.bilichat_forword_msg:
+        forword_list.append(reply + image + msg)
+        reply = ""
+    else:
+        msgid = (await matcher.send(reply + image + msg))["message_id"]
         reply = V11_MS.reply(msgid)
-        try:
-            cache = await get_video_cache(info)
-        except AbortError as e:
-            logger.exception(e)
-            await matcher.finish(reply + "视频字幕获取失败: " + str(e))  # type: ignore
-        except Exception as e:
-            capture_exception()
-            logger.exception(e)
-            await matcher.finish(reply + "未知错误: " + str(e))  # type: ignore
+
+    # furtuer fuctions
+    if not plugin_config.bilichat_openai_token and not plugin_config.bilichat_word_cloud:
+        raise FinishedException
+
+    # get video cache
+    try:
+        cache = await get_video_cache(info)
+    except AbortError as e:
+        logger.exception(e)
+        if "info" in plugin_config.bilichat_forword_msg:
+            forword_list.append(f"视频字幕获取失败: {str(e)}")
+            await forword_msg_v11(bot, event, forword_list)
+        else:
+            await matcher.finish(f"{reply}视频字幕获取失败: {str(e)}")
+    except Exception as e:
+        capture_exception()
+        logger.exception(e)
+        if "info" in plugin_config.bilichat_forword_msg:
+            forword_list.append(f"未知错误: {e}")
+            await forword_msg_v11(bot, event, forword_list)
+        else:
+            await matcher.finish(f"{reply}未知错误: {e}")  # type: ignore
+
+    if image := await wordcloud(cache=cache, cid=str(info["cid"])):
         if plugin_config.bilichat_word_cloud:
-            if image := await wordcloud(cache=cache, cid=str(info["cid"])):
-                await matcher.send(reply + V11_MS.image(image))  # type: ignore
+            if "wordcloud" in plugin_config.bilichat_forword_msg:
+                forword_list.append(V11_MS.image(image))
             else:
-                await matcher.finish(reply + "视频无有效字幕")
+                await matcher.send(reply + V11_MS.image(image))  # type: ignore
+    elif plugin_config.bilichat_word_cloud:
+        if "wordcloud" in plugin_config.bilichat_forword_msg:
+            forword_list.append("视频无有效字幕")
+            await forword_msg_v11(bot, event, forword_list)
+        else:
+            await matcher.finish(f"{reply}视频无有效字幕")
+
+    if summary := await openai_summarization(cache=cache, cid=str(info["cid"])):
         if plugin_config.bilichat_openai_token:
-            await matcher.send(reply + await openai_summarization(cache=cache, cid=str(info["cid"])))  # type: ignore
+            if "summary" in plugin_config.bilichat_forword_msg:
+                forword_list.append(summary)
+            else:
+                await matcher.send(reply + summary)  # type: ignore
+    elif plugin_config.bilichat_openai_token:
+        if "summary" in plugin_config.bilichat_forword_msg:
+            forword_list.append("视频无有效字幕")
+            await forword_msg_v11(bot, event, forword_list)
+        else:
+            await matcher.finish(f"{reply}视频无有效字幕")
+
+    if forword_list:
+        await forword_msg_v11(bot, event, forword_list)
 
 
 @bili.handle()
 @b23.handle()
 async def video_info_v12(bot: V12_Bot, event: V12_ME, state: T_State, matcher: Matcher):
     # basic info
     msg, img, info = await get_video_basic(state["bili_number"], state["_uid_"])
     if not msg:
         await matcher.finish()
     reply = V12_MS.reply(message_id=event.message_id, user_id=event.get_user_id())
     if not img:
         await matcher.finish(reply + msg)
-    fileid = await bot.upload_file(
-        type="data", name=f"{state['bili_number']}.jpg", data=img
-    )
+    fileid = await bot.upload_file(type="data", name=f"{state['bili_number']}.jpg", data=img)
     image = V12_MS.image(file_id=fileid["file_id"])
     msgid = (await matcher.send(reply + image + msg))["message_id"]
+
     # furtuer fuctions
-    if plugin_config.bilichat_openai_token or plugin_config.bilichat_word_cloud:
-        reply = V12_MS.reply(message_id=msgid, user_id=bot.self_id)
-        try:
-            cache = await get_video_cache(info)  # type: ignore
-        except AbortError as e:
-            logger.exception(e)
-            await matcher.finish(reply + "视频字幕获取失败: " + str(e))  # type: ignore
-        except Exception as e:
-            capture_exception()
-            logger.exception(e)
-            await matcher.finish(reply + "未知错误: " + str(e))  # type: ignore
-        if plugin_config.bilichat_word_cloud:
-            if image := await wordcloud(cache=cache, cid=str(info["cid"])):  # type: ignore
-                fileid = await bot.upload_file(
-                    type="data", name=f"{state['bili_number']}_wc.jpg", data=image
-                )  # type: ignore
-                await matcher.send(reply + V12_MS.image(file_id=fileid["file_id"]))
-            else:
-                await matcher.finish(reply + "视频无有效字幕")
+    if not (plugin_config.bilichat_openai_token or plugin_config.bilichat_word_cloud):
+        raise FinishedException
 
-        if plugin_config.bilichat_openai_token:
-            await matcher.send(reply + await openai_summarization(cache=cache, cid=str(info["cid"])))  # type: ignore
+    reply = V12_MS.reply(message_id=msgid, user_id=bot.self_id)
+    try:
+        cache = await get_video_cache(info)  # type: ignore
+    except AbortError as e:
+        logger.exception(e)
+        await matcher.finish(f"{reply}视频字幕获取失败: {str(e)}")
+    except Exception as e:
+        capture_exception()
+        logger.exception(e)
+        await matcher.finish(f"{reply}未知错误: {str(e)}")
+
+    if plugin_config.bilichat_word_cloud:
+        if image := await wordcloud(cache=cache, cid=str(info["cid"])):
+            fileid = await bot.upload_file(
+                type="data", name=f"{state['bili_number']}_wc.jpg", data=image
+            )  # type: ignore
+            await matcher.send(reply + V12_MS.image(file_id=fileid["file_id"]))
+        else:
+            await matcher.finish(f"{reply}视频无有效字幕")
+
+    if plugin_config.bilichat_openai_token:
+        if summary := await openai_summarization(cache=cache, cid=str(info["cid"])):
+            await matcher.send(reply + summary)  # type: ignore
+        else:
+            await matcher.finish(f"{reply}视频无有效字幕")
```

### Comparing `nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import importlib.util
 import sys
-from typing import Literal, Optional, Sequence, Union
+from typing import Literal, Optional, Sequence, Union, Set
 
 from nonebot import get_driver
 from nonebot.log import logger
 from pydantic import BaseModel, validator
 
 # get package version
 if sys.version_info < (3, 10):
@@ -24,37 +24,53 @@
     bilichat_enable_private: bool = True
     bilichat_enable_v12_channel: bool = True
     bilichat_enable_unkown_src: bool = False
     bilichat_whitelist: Sequence[str] = []
     bilichat_blacklist: Sequence[str] = []
     bilichat_dynamic_font: Optional[str]
     bilichat_cd_time: int = 120
+    bilichat_forword_msg: Sequence[str] = {}  # ("info", "wordcloud", "summary")
+    nickname: Sequence[str] = ["awesome-nonebot"]
 
     # both WC and AI
     bilichat_use_bcut_asr: bool = True
 
     # Word Cloud
     bilichat_word_cloud: bool = True
 
     # AI Summary
     bilichat_openai_token: Optional[str]
     bilichat_openai_proxy: Optional[str]
-    bilichat_openai_model: Literal[
-        "gpt-3.5-turbo-0301", "gpt-4-0314", "gpt-4-32k-0314"
-    ] = "gpt-3.5-turbo-0301"
+    bilichat_openai_model: Literal["gpt-3.5-turbo-0301", "gpt-4-0314", "gpt-4-32k-0314"] = "gpt-3.5-turbo-0301"
     bilichat_openai_token_limit: int = 3500
 
+    @validator("bilichat_forword_msg")
+    def check_adapter_can_send_forword_msg(cls, v):
+        if not v:
+            return
+        drivers = get_driver()._adapters.keys()
+        if "OneBot V12" in drivers:
+            logger.warning(
+                "Forword_msg is not implemented by OneBot V12, events of OneBot V12 will not be sent as forword_msg!"
+            )
+        if "OneBot V11" in drivers:
+            logger.warning(
+                "Using forward_msg may cause serious risk control restrictions, please enable this feature with caution!"
+            )
+
+    @validator("nickname")
+    def check_nickname(cls, v):
+        return list(v) or ["awesome-nonebot"]
+
     @validator("bilichat_openai_proxy")
     def check_openai_proxy(cls, v, values):
         if values["bilichat_openai_token"] is None:
             return v
         if v is None:
-            logger.warning(
-                "you have enabled openai summary without a proxy, this may cause request failure."
-            )
+            logger.warning("you have enabled openai summary without a proxy, this may cause request failure.")
         return v
 
     @validator("bilichat_openai_token_limit")
     def check_token_limit(cls, v, values):
         if values["bilichat_openai_token"] is None:
             return v
         if not isinstance(v, int):
@@ -79,17 +95,15 @@
         else:
             raise RuntimeError(
                 "Package(s) of fuction openai summary not installed, use **nb plugin install nonebot-plugin-bilichat[openai]** to install required dependencies"
             )
 
     @validator("bilichat_word_cloud", always=True)
     def check_pypackage_wordcloud(cls, v):
-        if (
-            importlib.util.find_spec("wordcloud") and importlib.util.find_spec("jieba")
-        ) or not v:
+        if (importlib.util.find_spec("wordcloud") and importlib.util.find_spec("jieba")) or not v:
             return v
         else:
             raise RuntimeError(
                 "Package(s) of fuction wordcloud not installed, use **nb plugin install nonebot-plugin-bilichat[wordcloud]** to install required dependencies"
             )
 
     def verify_permission(self, uid: Union[str, int]):
```

### Comparing `nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,18 @@
     ResourceCreateRspSchema,
     ResultRspSchema,
     TaskCreateRspSchema,
 )
 
 __version__ = "0.0.2"
 
-API_REQ_UPLOAD = (
-    "https://member.bilibili.com/x/bcut/rubick-interface/resource/create"  # 申请上传
-)
+API_REQ_UPLOAD = "https://member.bilibili.com/x/bcut/rubick-interface/resource/create"  # 申请上传
 API_COMMIT_UPLOAD = "https://member.bilibili.com/x/bcut/rubick-interface/resource/create/complete"  # 提交上传
 API_CREATE_TASK = "https://member.bilibili.com/x/bcut/rubick-interface/task"  # 创建任务
-API_QUERY_RESULT = (
-    "https://member.bilibili.com/x/bcut/rubick-interface/task/result"  # 查询结果
-)
+API_QUERY_RESULT = "https://member.bilibili.com/x/bcut/rubick-interface/task/result"  # 查询结果
 
 SUPPORT_SOUND_FORMAT = Literal["flac", "aac", "m4a", "mp3", "wav"]
 
 
 class APIError(Exception):
     "接口调用错误"
 
@@ -154,29 +150,25 @@
             raise APIError(code, resp["message"])
         resp_data = ResourceCompleteRspSchema.parse_obj(resp["data"])
         self.__download_url = resp_data.download_url
         logger.debug("commit complete")
 
     async def create_task(self) -> str:
         "开始创建转换任务"
-        resp = await self.session.post(
-            API_CREATE_TASK, json={"resource": self.__download_url, "model_id": "7"}
-        )
+        resp = await self.session.post(API_CREATE_TASK, json={"resource": self.__download_url, "model_id": "7"})
         resp.raise_for_status()
         resp = resp.json()
         if code := resp["code"]:
             raise APIError(code, resp["message"])
         resp_data = TaskCreateRspSchema.parse_obj(resp["data"])
         self.task_id = resp_data.task_id
         logger.info(f"Conversion task created: {self.task_id}")
         return self.task_id
 
     async def result(self, task_id: Optional[str] = None) -> ResultRspSchema:
         "查询转换结果"
-        resp = await self.session.get(
-            API_QUERY_RESULT, params={"model_id": 7, "task_id": task_id or self.task_id}
-        )
+        resp = await self.session.get(API_QUERY_RESULT, params={"model_id": 7, "task_id": task_id or self.task_id})
         resp.raise_for_status()
         resp = resp.json()
         if code := resp["code"]:
             raise APIError(code, resp["message"])
         return ResultRspSchema.parse_obj(resp["data"])
```

### Comparing `nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,17 +128,15 @@
     resp = await grpc_get_followed_dynamics(auth=Bili_Auth)
     exclude_list = [
         DynamicType.ad,
         DynamicType.live,
         DynamicType.live_rcmd,
         DynamicType.banner,
     ]
-    dynamic_list = [
-        dyn for dyn in resp.dynamic_list.list if dyn.card_type not in exclude_list
-    ]
+    dynamic_list = [dyn for dyn in resp.dynamic_list.list if dyn.card_type not in exclude_list]
     dynamic_list.reverse()
     return dynamic_list
 
 
 @grpc_request
 async def grpc_get_dynamic_details(dynamic_ids: str, **kwargs) -> DynDetailsReply:
     stub = DynamicStub(kwargs.pop("_channel"))
```

### Comparing `nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files 5% similar despite different names*

```diff
@@ -104,17 +104,15 @@
                     content=await get_subtitle(int(info["aid"]), int(info["cid"])),
                     jieba=None,
                     openai=None,
                 )
             },
         )
     elif str(info["cid"]) not in cache.episodes.keys():
-        logger.debug(
-            f'cache of av{info["aid"]} exists, but cid{info["cid"]} not found, appending cache'
-        )
+        logger.debug(f'cache of av{info["aid"]} exists, but cid{info["cid"]} not found, appending cache')
         cache.episodes[str(info["cid"])] = Episode(
             title=None,
             content=await get_subtitle(int(info["aid"]), int(info["cid"])),
             jieba=None,
             openai=None,
         )
     else:
```

### Comparing `nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 
 font_semibold = str(get_font_sync("sarasa-mono-sc-semibold.ttf"))
 font_bold = str(get_font_sync("sarasa-mono-sc-bold.ttf"))
 font_vanfont = str(get_font_sync("vanfont.ttf"))
 
 
 async def binfo_image_create(video_view: ViewReply, b23_url: str):
-    video_info = (
-        video_view.activity_season if video_view.activity_season.arc.aid else video_view
-    )
+    video_info = video_view.activity_season if video_view.activity_season.arc.aid else video_view
 
     client = hc
     client.headers.update(
         {
             "User-Agent": (
                 "Mozilla/5.0 (Windows NT 10.0; Win64; x64)"
                 "AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.149 Safari/537.36"
@@ -156,19 +154,15 @@
             up_level = "\uE6D0"
             level_color = (255, 108, 0)
         else:
             up_level = "\uE6D1"
             level_color = (255, 0, 0)
 
         # 头像
-        face_url = (
-            up_data["card"]["face"]
-            if up_data
-            else "https://i0.hdslb.com/bfs/face/member/noface.jpg"
-        )
+        face_url = up_data["card"]["face"] if up_data else "https://i0.hdslb.com/bfs/face/member/noface.jpg"
         face_req = await client.get(face_url)
         if face_req.status_code == 404:
             face_req = await client.get(f"{face_url}@160w_160h_1c_1s.webp")
         face_get = face_req.content
         face_bio = BytesIO(face_get)
         face = Image.open(face_bio)
         face.convert("RGB")
@@ -177,21 +171,17 @@
         # 名字
         draw.text(
             (160, 25 + (i * 120)),
             up_data["card"]["name"] if up_data else f"账号已注销（{uid}）",
             name_color or "black",
             name_font,
         )
-        name_size_x, _ = name_font.getsize(
-            up_data["card"]["name"] if up_data else f"账号已注销（{uid} "
-        )
+        name_size_x, _ = name_font.getsize(up_data["card"]["name"] if up_data else f"账号已注销（{uid} ")
         # 等级
-        draw.text(
-            (160 + name_size_x + 10, 16 + (i * 120)), up_level, level_color, icon_font
-        )
+        draw.text((160 + name_size_x + 10, 16 + (i * 120)), up_level, level_color, icon_font)
         # 身份
         up_title_size_x, up_title_size_y = up_title_font.getsize(up_title)
         draw.rectangle(
             (
                 60,
                 10 + (i * 120),
                 73 + up_title_size_x,
```

### Comparing `nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,17 @@
     logger.debug(f"Loading font: {font}")
     url = URL(font)
     if url.is_absolute():
         if font_path.joinpath(url.name).exists():
             logger.debug(f"Font {url.name} found in local")
             return font_path.joinpath(url.name)
         else:
-            logger.warning(f"font {font} does not exist, this will take several seconds to minutes to download fonts depend on your network.")
+            logger.warning(
+                f"font {font} does not exist, this will take several seconds to minutes to download fonts depend on your network."
+            )
             async with httpx.AsyncClient() as client:
                 resp = await client.get(font)
                 if resp.status_code != 200:
                     raise ConnectionError(f"Font {font} failed to download")
                 font_path.joinpath(url.name).write_bytes(resp.content)
                 return font_path.joinpath(url.name)
     else:
@@ -70,33 +72,29 @@
     if lock_file.read_text() != font_url:
         logger.warning("font file does not exist. Trying to download")
         font_file = BytesIO()
         with httpx.stream("GET", font_url) as r:
             for chunk in r.iter_bytes():
                 font_file.write(chunk)
         with ZipFile(font_file) as z:
-            fonts = [
-                i for i in z.filelist if str(i.filename).startswith("bbot_fonts/font/")
-            ]
+            fonts = [i for i in z.filelist if str(i.filename).startswith("bbot_fonts/font/")]
             for font in fonts:
                 file_name = Path(font.filename).name
                 local_file = font_path.joinpath(file_name)
                 if not local_file.exists():
                     logger.debug(local_file)
                     local_file.write_bytes(z.read(font))
 
         lock_file.write_text(font_url)
 
     if plugin_config.bilichat_dynamic_font:
         if plugin_config.bilichat_dynamic_font.startswith("http"):
             custom_font = URL(plugin_config.bilichat_dynamic_font)
             if not custom_font.is_absolute():
-                raise ValueError(
-                    f"The custom font {plugin_config.bilichat_dynamic_font} is not a valid URL!"
-                )
+                raise ValueError(f"The custom font {plugin_config.bilichat_dynamic_font} is not a valid URL!")
             if custom_font.name != URL(DEFUALT_DYNAMIC_FONT).name:
                 logger.debug(get_font_sync(plugin_config.bilichat_dynamic_font))
         else:
             custom_font = font_path.joinpath(plugin_config.bilichat_dynamic_font)
             if not custom_font.exists():
                 raise FileNotFoundError(
                     f"The custom font {plugin_config.bilichat_dynamic_font} does not exist, please put the font file in {font_path.absolute()} folder!"
```

### Comparing `nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/strings.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         i += 1
         if next_str == "":
             break
         elif next_str[0] == "\n":
             next_str = next_str[1:]
         elif s == "\n":
             str_list.append(next_str[: i - 1])
-            next_str = next_str[i - 1:]
+            next_str = next_str[i - 1 :]
             si = 0
             i = 0
             continue
         if si > cut:
             try:
                 if next_str[i] in punc:
                     i += 1
```

### Comparing `nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from loguru import logger
 
 from ..config import plugin_config
 from ..model.bcut_asr import ResultStateEnum
 from ..model.exception import AbortError
 from .bcut_asr import BcutASR
 from .bilibili_request import get_player, grpc_get_playview, hc
-from ..optional import capture_exception # type: ignore
+from ..optional import capture_exception  # type: ignore
 
 
 async def get_subtitle_url(aid: int, cid: int) -> Optional[str]:
     video_player = await get_player(aid, cid)
     subtitles_raw: List[Dict] = video_player["subtitle"]["subtitles"]
     logger.debug(subtitles_raw)
```

### Comparing `nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files 12% similar despite different names*

```diff
@@ -55,24 +55,19 @@
 
     def to_txt(self) -> str:
         "转成txt格式字幕 (无时间标记)"
         return "\n".join(seg.transcript for seg in self.utterances)
 
     def to_srt(self) -> str:
         "转成srt格式字幕"
-        return "\n".join(
-            f"{n}\n{seg.to_srt_ts()}\n{seg.transcript}\n"
-            for n, seg in enumerate(self.utterances, 1)
-        )
+        return "\n".join(f"{n}\n{seg.to_srt_ts()}\n{seg.transcript}\n" for n, seg in enumerate(self.utterances, 1))
 
     def to_lrc(self) -> str:
         "转成lrc格式字幕"
-        return "\n".join(
-            f"{seg.to_lrc_ts()}{seg.transcript}" for seg in self.utterances
-        )
+        return "\n".join(f"{seg.to_lrc_ts()}{seg.transcript}" for seg in self.utterances)
 
     def to_ass(self) -> str:
         ...
 
 
 class ResourceCreateRspSchema(BaseModel):
     "上传申请响应"
```

### Comparing `nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/model/cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,13 +20,13 @@
         cache = cls(id=id, title=title, episodes=episodes)
         cache.save()
         return cache
 
     @classmethod
     def get(cls, id: Union[str, int]):
         f = cache_dir.joinpath(f"{id}.json")
-        return cls.parse_file(f,encoding="utf-8") if f.exists() else None
+        return cls.parse_file(f, encoding="utf-8") if f.exists() else None
 
     def save(self):
         cache_dir.touch(0o755)
         f = cache_dir.joinpath(f"{self.id}.json")
-        f.write_text(self.json(ensure_ascii=False),encoding="utf-8")
+        f.write_text(self.json(ensure_ascii=False), encoding="utf-8")
```

### Comparing `nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/summary/content_summarise.py` & `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/summary/content_summarise.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,31 +27,25 @@
 async def openai_summarization(cache: Cache, cid: str = "0"):
     try:
         logger.info(f"Generation summary of Video(Column) {cache.id}")
         if not cache.episodes[cid] or not cache.episodes[cid].content:
             return "视频无有效字幕"
         elif not cache.episodes[cid].openai:
             if cache.id[:2].lower() in ["bv", "av"]:
-                ai_summary = await subtitle_summarise(
-                    cache.title, cache.episodes[cid].content
-                )
+                ai_summary = await subtitle_summarise(cache.title, cache.episodes[cid].content)
             elif cache.id[:2].lower() == "cv":
-                ai_summary = await column_summarise(
-                    cache.title, cache.episodes[cid].content[0]
-                )
+                ai_summary = await column_summarise(cache.title, cache.episodes[cid].content[0])
             else:
                 raise ValueError(f"Illegal Video(Column) types {cache.id}")
 
             if ai_summary.summary:
                 cache.episodes[cid].openai = ai_summary.summary
                 cache.save()
             else:
-                logger.warning(
-                    f"Video(Column) {cache.id} summary failure: {ai_summary.raw}"
-                )
+                logger.warning(f"Video(Column) {cache.id} summary failure: {ai_summary.raw}")
                 return None
         return cache.episodes[cid].openai or "视频无法总结"  # TODO: add image type output
     except AbortError as e:
         logger.exception(f"Video(Column) {cache.id} summary aborted: {e}")
         return f"视频(专栏) {cache.id} 总结中止: {e}"
     except Exception as e:
         capture_exception()
```

### Comparing `nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/summary/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 from loguru import logger
 
 from ..config import plugin_config
 from ..model.openai import AISummary
 
 if plugin_config.bilichat_openai_token:
     logger.info("Loading OpenAI Token enc model")
-    tiktoken_enc = asyncio.run(
-        tiktoken_async.encoding_for_model(plugin_config.bilichat_openai_model)
-    )
+    tiktoken_enc = asyncio.run(tiktoken_async.encoding_for_model(plugin_config.bilichat_openai_model))
     logger.success(f"Enc model {tiktoken_enc.name} load successfully")
 
 
 def get_user_prompt(title: str, transcript: str) -> List[Dict[str, str]]:
     title = title.replace("\n", " ").strip() if title else ""
     transcript = transcript.replace("\n", " ").strip() if transcript else ""
     language = "Chinese"
@@ -29,17 +27,15 @@
         "starting with a short highlight, each bullet point is at least 15 words. "
         "Choose an appropriate emoji for each bullet point. "
         "Use the video above: {{Title}} {{Transcript}}."
         "If you think that the content in the transcript is meaningless, "
         "Or if there is very little content that cannot be well summarized, "
         "then you can simply output the two words 'no meaning'. Remember, not to output anything else."
     )
-    return get_full_prompt(
-        f'Title: "{title}"\nTranscript: "{transcript}"', sys_prompt, language
-    )
+    return get_full_prompt(f'Title: "{title}"\nTranscript: "{transcript}"', sys_prompt, language)
 
 
 def count_tokens(prompts: List[Dict[str, str]]):
     """根据内容计算 token 数"""
 
     if plugin_config.bilichat_openai_model == "gpt-3.5-turbo-0301":
         tokens_per_message = 4
@@ -57,26 +53,22 @@
             num_tokens += len(tiktoken_enc.encode(value))
             if key == "name":
                 num_tokens += tokens_per_name
     num_tokens += 3
     return num_tokens
 
 
-def get_small_size_transcripts(
-    text_data: List[str], token_limit: int = plugin_config.bilichat_openai_token_limit
-):
+def get_small_size_transcripts(text_data: List[str], token_limit: int = plugin_config.bilichat_openai_token_limit):
     unique_texts = list(OrderedDict.fromkeys(text_data))
     while count_tokens(get_user_prompt("", " ".join(unique_texts))) > token_limit:
         unique_texts.pop(random.randint(0, len(unique_texts) - 1))
     return " ".join(unique_texts)
 
 
-def get_full_prompt(
-    prompt: str, system: Optional[str] = None, language: Optional[str] = None
-):
+def get_full_prompt(prompt: str, system: Optional[str] = None, language: Optional[str] = None):
     plist: List[Dict[str, str]] = []
     if system:
         plist.append({"role": "system", "content": system})
     plist.append({"role": "user", "content": prompt})
     if language:
         plist.extend(
             (
@@ -109,14 +101,10 @@
             json={
                 "model": model,
                 "messages": prompt_message,
             },
         )
         if req.status_code != 200:
             return AISummary(error=True, message=req.text, raw=req.json())
-        logger.info(
-            f"[OpenAI] Response:\n{req.json()['choices'][0]['message']['content']}"
-        )
+        logger.info(f"[OpenAI] Response:\n{req.json()['choices'][0]['message']['content']}")
         logger.info(f"[OpenAI] Response token usage: {req.json()['usage']}")
-        return AISummary(
-            summary=req.json()["choices"][0]["message"]["content"], raw=req.json()
-        )
+        return AISummary(summary=req.json()["choices"][0]["message"]["content"], raw=req.json())
```

### Comparing `nonebot_plugin_bilichat-1.0.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-1.1.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 import asyncio
 from io import BytesIO
 from typing import Dict
 
 from jieba.analyse.tfidf import TFIDF
-from wordcloud import WordCloud
 from nonebot.log import logger
+from wordcloud import WordCloud
 
+from ..lib.fonts_provider import get_font
 from ..model.cache import Cache
 from ..model.exception import AbortError
 from ..optional import capture_exception
-from ..lib.fonts_provider import get_font
 
 tfidf = TFIDF()
 
 
 async def wordcloud(cache: Cache, cid: str = "0"):
     try:
         logger.info(f"Generation wordcloud of Video(Column) {cache.id}")
         if not cache.episodes[cid] or not cache.episodes[cid].content:
             return None
         elif not cache.episodes[cid].jieba:
             loop = asyncio.get_running_loop()
-            cache.episodes[cid].jieba = await loop.run_in_executor(
-                None, get_frequencies, cache.episodes[cid].content
-            )
+            cache.episodes[cid].jieba = await loop.run_in_executor(None, get_frequencies, cache.episodes[cid].content)
             cache.save()
         return await get_worldcloud_image(cache.episodes[cid].jieba)
     except AbortError as e:
         logger.exception(f"Video(Column) {cache.id} wordcloud generation aborted: {e}")
         return None
     except Exception as e:
         capture_exception()
```

### Comparing `nonebot_plugin_bilichat-1.0.1/pyproject.toml` & `nonebot_plugin_bilichat-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "1.0.1"
+version = "1.1.0"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "httpx>=0.23.3",
```

### Comparing `nonebot_plugin_bilichat-1.0.1/PKG-INFO` & `nonebot_plugin_bilichat-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 1.0.1
+Version: 1.1.0
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx>=0.23.3
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
@@ -132,28 +132,30 @@
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的配置, 配置均为**非必须项**
 
 | 配置项 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|
-| bilichat_block              | bool      | False              | 是否拦截事件(防止其他插件二次解析) |
-| bilichat_enable_private     | bool      | True               | 是否允许响应私聊 |
-| bilichat_enable_v12_channel | bool      | True               | 是否允许响应频道消息(ob12专属) |
-| bilichat_enable_unkown_src  | bool      | False              | 是否允许响应未知来源的消息 |
-| bilichat_whitelist          | list[str] | []                 | **响应**的群聊(频道)名单, 会覆盖黑名单 |
-| bilichat_blacklist          | list[str] | []                 | **不响应**的群聊(频道)名单 |
-| bilichat_dynamic_font       | str       | None               | 视频信息及词云图片使用的字体 |
-| bilichat_cd_time            | int       | 120                | 对同一视频的响应冷却时间(防止刷屏) |
-| bilichat_use_bcut_asr       | bool      | True               | 是否在**没有字幕时**调用必剪接口生成字幕 |
-| bilichat_word_cloud         | bool      | True               | 是否开启词云功能 |
-| bilichat_openai_token       | str       | None               | openai的apikey, 若留空则禁用AI总结 |
-| bilichat_openai_proxy       | str       | None               | 访问openai使用的代理地址 |
-| bilichat_openai_model       | str       | gpt-3.5-turbo-0301 | 使用的语言模型名称 |
-| bilichat_openai_token_limit | int       | 3500               | 请求的文本量上限, 计算方式可参考[tiktoken](https://github.com/openai/tiktoken) |
+| bilichat_block              | bool      | False                | 是否拦截事件(防止其他插件二次解析) |
+| bilichat_enable_private     | bool      | True                 | 是否允许响应私聊 |
+| bilichat_enable_v12_channel | bool      | True                 | 是否允许响应频道消息(ob12专属) |
+| bilichat_enable_unkown_src  | bool      | False                | 是否允许响应未知来源的消息 |
+| bilichat_whitelist          | list[str] | []                   | **响应**的群聊(频道)名单, 会覆盖黑名单 |
+| bilichat_blacklist          | list[str] | []                   | **不响应**的群聊(频道)名单 |
+| bilichat_dynamic_font       | str       | None                 | 视频信息及词云图片使用的字体 |
+| bilichat_cd_time            | int       | 120                  | 对同一视频的响应冷却时间(防止刷屏) |
+| bilichat_forword_msg        | set[str]  | ()                   | 对什么类型的消息开启合并转发(ob11专属),包含 `info`、`wordcloud`、`summary` 三个可选项 |
+| nickname                    | set[str]  | ("awesome-nonebot",) | 合并转发中,bot的昵称(取第一个值) |
+| bilichat_use_bcut_asr       | bool      | True                 | 是否在**没有字幕时**调用必剪接口生成字幕 |
+| bilichat_word_cloud         | bool      | True                 | 是否开启词云功能 |
+| bilichat_openai_token       | str       | None                 | openai的apikey, 若留空则禁用AI总结 |
+| bilichat_openai_proxy       | str       | None                 | 访问openai使用的代理地址 |
+| bilichat_openai_model       | str       | gpt-3.5-turbo-0301   | 使用的语言模型名称 |
+| bilichat_openai_token_limit | int       | 3500                 | 请求的文本量上限, 计算方式可参考[tiktoken](https://github.com/openai/tiktoken) |
 
 ## 🎉 使用
 
 直接发送视频(专栏)链接即可
 
 ### 指令表
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.1.0 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx>=0.23.3 Requires-Dist: bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-
 plugin-localstore>=0.4.1 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-
 Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra" Requires-Dist:
@@ -47,15 +47,19 @@
 æ¯å¦åè®¸ååºç§è | | bilichat_enable_v12_channel | bool | True |
 æ¯å¦åè®¸ååºé¢éæ¶æ¯(ob12ä¸å±) | | bilichat_enable_unkown_src |
 bool | False | æ¯å¦åè®¸ååºæªç¥æ¥æºçæ¶æ¯ | | bilichat_whitelist |
 list[str] | [] | **ååº**çç¾¤è(é¢é)åå, ä¼è¦çé»åå | |
 bilichat_blacklist | list[str] | [] | **ä¸ååº**çç¾¤è(é¢é)åå | |
 bilichat_dynamic_font | str | None | è§é¢ä¿¡æ¯åè¯äºå¾çä½¿ç¨çå­ä½
 | | bilichat_cd_time | int | 120 | å¯¹åä¸è§é¢çååºå·å´æ¶é´
-(é²æ­¢å·å±) | | bilichat_use_bcut_asr | bool | True |
+(é²æ­¢å·å±) | | bilichat_forword_msg | set[str] | () |
+å¯¹ä»ä¹ç±»åçæ¶æ¯å¼å¯åå¹¶è½¬å(ob11ä¸å±),åå«
+`info`ã`wordcloud`ã`summary` ä¸ä¸ªå¯éé¡¹ | | nickname | set[str] |
+("awesome-nonebot",) | åå¹¶è½¬åä¸­,botçæµç§°(åç¬¬ä¸ä¸ªå¼) | |
+bilichat_use_bcut_asr | bool | True |
 æ¯å¦å¨**æ²¡æå­å¹æ¶**è°ç¨å¿åªæ¥å£çæå­å¹ | |
 bilichat_word_cloud | bool | True | æ¯å¦å¼å¯è¯äºåè½ | |
 bilichat_openai_token | str | None | openaiçapikey,
 è¥çç©ºåç¦ç¨AIæ»ç» | | bilichat_openai_proxy | str | None |
 è®¿é®openaiä½¿ç¨çä»£çå°å | | bilichat_openai_model | str | gpt-3.5-
 turbo-0301 | ä½¿ç¨çè¯­è¨æ¨¡ååç§° | | bilichat_openai_token_limit | int
 | 3500 | è¯·æ±çææ¬éä¸é, è®¡ç®æ¹å¼å¯åè[tiktoken](https://
```

