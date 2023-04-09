# Comparing `tmp/nonebot-plugin-SDGPT-0.0.8.tar.gz` & `tmp/nonebot-plugin-SDGPT-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-SDGPT-0.0.8.tar", last modified: Sat Apr  8 23:50:00 2023, max compression
+gzip compressed data, was "nonebot-plugin-SDGPT-0.0.9.tar", last modified: Sun Apr  9 00:36:06 2023, max compression
```

## Comparing `nonebot-plugin-SDGPT-0.0.8.tar` & `nonebot-plugin-SDGPT-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 23:50:00.604003 nonebot-plugin-SDGPT-0.0.8/
--rw-rw-rw-   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot-plugin-SDGPT-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      210 2023-04-08 23:50:00.603002 nonebot-plugin-SDGPT-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      147 2023-04-08 20:35:51.000000 nonebot-plugin-SDGPT-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 23:50:00.590991 nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT/
--rw-rw-rw-   0        0        0     3550 2023-04-08 23:48:23.000000 nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT/__init__.py
--rw-rw-rw-   0        0        0     8862 2023-04-08 23:40:51.000000 nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT/bot.py
-drwxrwxrwx   0        0        0        0 2023-04-08 23:50:00.601000 nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT.egg-info/
--rw-rw-rw-   0        0        0      210 2023-04-08 23:50:00.000000 nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-04-08 23:50:00.000000 nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 23:50:00.000000 nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2023-04-08 23:50:00.000000 nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-08 23:50:00.000000 nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 23:50:00.604003 nonebot-plugin-SDGPT-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      663 2023-04-08 23:49:51.000000 nonebot-plugin-SDGPT-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 00:36:06.534931 nonebot-plugin-SDGPT-0.0.9/
+-rw-rw-rw-   0        0        0     1062 2023-04-08 20:16:38.000000 nonebot-plugin-SDGPT-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      210 2023-04-09 00:36:06.534931 nonebot-plugin-SDGPT-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      699 2023-04-09 00:32:22.000000 nonebot-plugin-SDGPT-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 00:36:06.524923 nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT/
+-rw-rw-rw-   0        0        0     3550 2023-04-08 23:48:23.000000 nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT/__init__.py
+-rw-rw-rw-   0        0        0     9400 2023-04-09 00:35:17.000000 nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT/bot.py
+drwxrwxrwx   0        0        0        0 2023-04-09 00:36:06.532930 nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT.egg-info/
+-rw-rw-rw-   0        0        0      210 2023-04-09 00:36:06.000000 nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-04-09 00:36:06.000000 nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 00:36:06.000000 nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2023-04-09 00:36:06.000000 nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-09 00:36:06.000000 nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 00:36:06.535933 nonebot-plugin-SDGPT-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      663 2023-04-09 00:35:06.000000 nonebot-plugin-SDGPT-0.0.9/setup.py
```

### Comparing `nonebot-plugin-SDGPT-0.0.8/LICENSE` & `nonebot-plugin-SDGPT-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT/__init__.py` & `nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-SDGPT-0.0.8/nonebot_plugin_SDGPT/bot.py` & `nonebot-plugin-SDGPT-0.0.9/nonebot_plugin_SDGPT/bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,14 +141,15 @@
     if mode ==2:
         return text.replace(r'.*\.AIP','')
 
 async def text2image(func,prompt):
     ip = cfg['text2img_proxy'].split(':')
     info('Stable-Diffusion','开始询问 api'+cfg['text2img_proxy'])
     api = webuiapi.WebUIApi(host=ip[0], port=ip[1]) # type: ignore
+    
     result1 = api.txt2img(
         prompt=prompt,
         negative_prompt=cfg['text2img_negative_prompt'],
         steps=cfg['text2img_step'],
     )
     image = result1.image
     success('Stable-Diffusion','返回图片')
@@ -161,33 +162,37 @@
     global bingbot
     global chatbot
     global chatbot_api
     global botList 
     if not os.path.exists('./config.cfg'):
         with open('config.cfg', 'w',encoding='utf-8') as f:
             text = """
-text2img_step=27
-text2img_negative_prompt="(worst quality, low quality:1.4),NSFW,r18"
-text2img_proxy='127.0.0.1:7860'
-
-presets_dir='./presets'
-Chat_stream_waitTime=2
-Chat_stream_endStr=('？','。','?','\\n')
-defaultAI='chatGPT'
+# "#"后面的为注释
 
-chatGPT # ChatGPT 配置:
-access_token=""
+Stable-Diffusion # Stable-Diffusion 配置:
+text2img_step=27 # 文生图 渲染步数
+text2img_negative_prompt="(worst quality, low quality:1.4),NSFW,r18" #文生图 固定负面提示词
+text2img_proxy='127.0.0.1:7860' #Stable-Diffusion api地址 (SD内配置 --server-name 127.0.0.1 --port 7860 --api)
+
+chat # 聊天 api 通用设置:
+presets_dir='./presets' # 预设文件夹
+Chat_stream_waitTime=2 # 频道内 分条发送间隔 (秒)
+Chat_stream_endStr=('？','。','?','\n') # 频道内 分条发送分割依据
+defaultAI='chatGPT' # 默认 AI
+
+chatGPT # ChatGPT 配置 (网页):
+access_token="" # access_token  获取:https://chat.openai.com/api/auth/session
 
 chatGPT_api # ChatGPT api 配置:
-api_key=""
+api_key="" # api_key 获取:https://platform.openai.com/account/api-keys
 model="gpt-3.5-turbo"
 
 bing # Bing api 配置:
-cookies_file_path="./cookies.json"
-            """
+cookies_file_path="./cookies.json" # 设置:https://github.com/thx114/SDGPT/wiki/bing-cookies
+"""
             f.write(text)
 
 
     cfg_ =dotenv_values("config.cfg")
 
     try : 
         if len(cfg_['access_token']) >0:suc('Config','配置文件 有效') # type: ignore
```

### Comparing `nonebot-plugin-SDGPT-0.0.8/setup.py` & `nonebot-plugin-SDGPT-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 
 
 setuptools.setup(
     name="nonebot-plugin-SDGPT",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.0.8",  # 程序版本
+    version="0.0.9",  # 程序版本
     author="F_thx",  # 项目作者
     author_email="thx1140093097@gmail.com",  # 作者邮件
     url="https://github.com/thx114/SDGPT",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
     license="MIT Licence",
     install_requires=[
         'nonebot2',
```

