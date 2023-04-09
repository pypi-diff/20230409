# Comparing `tmp/chat_agent-0.1.6.5.tar.gz` & `tmp/chat_agent-0.1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_agent-0.1.6.5.tar", last modified: Sat Apr  8 16:52:22 2023, max compression
+gzip compressed data, was "chat_agent-0.1.6.6.tar", last modified: Sun Apr  9 12:27:34 2023, max compression
```

## Comparing `chat_agent-0.1.6.5.tar` & `chat_agent-0.1.6.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.451400 chat_agent-0.1.6.5/
--rw-r--r--   0 alex       (501) staff       (20)       48 2023-03-20 19:07:00.000000 chat_agent-0.1.6.5/MANIFEST.in
--rw-r--r--   0 alex       (501) staff       (20)      263 2023-04-08 16:52:22.451130 chat_agent-0.1.6.5/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     1696 2023-04-08 16:48:02.000000 chat_agent-0.1.6.5/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.444129 chat_agent-0.1.6.5/chat_agent/
--rw-r--r--   0 alex       (501) staff       (20)     2755 2023-04-08 16:47:51.000000 chat_agent-0.1.6.5/chat_agent/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     2881 2023-04-03 16:26:46.000000 chat_agent-0.1.6.5/chat_agent/app.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.445245 chat_agent-0.1.6.5/chat_agent/base/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-04-07 05:27:54.000000 chat_agent-0.1.6.5/chat_agent/base/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     3843 2023-04-08 16:45:47.000000 chat_agent-0.1.6.5/chat_agent/base/base_websocket.py
--rw-r--r--   0 alex       (501) staff       (20)      223 2023-04-07 11:50:22.000000 chat_agent-0.1.6.5/chat_agent/base/singleton.py
--rw-r--r--   0 alex       (501) staff       (20)     1536 2023-04-08 05:26:59.000000 chat_agent-0.1.6.5/chat_agent/base_websocket_app.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.445901 chat_agent-0.1.6.5/chat_agent/cache/
--rw-r--r--   0 alex       (501) staff       (20)      252 2023-03-24 01:24:01.000000 chat_agent-0.1.6.5/chat_agent/cache/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      818 2023-03-24 01:39:51.000000 chat_agent-0.1.6.5/chat_agent/cache/cache_helper.py
--rw-r--r--   0 alex       (501) staff       (20)     2147 2023-03-31 01:41:44.000000 chat_agent-0.1.6.5/chat_agent/cert.pem
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.446466 chat_agent-0.1.6.5/chat_agent/client/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-04-05 02:46:32.000000 chat_agent-0.1.6.5/chat_agent/client/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1055 2023-04-08 16:50:23.000000 chat_agent-0.1.6.5/chat_agent/client/base_web_socket_client.py
--rw-r--r--   0 alex       (501) staff       (20)      670 2023-04-07 05:26:50.000000 chat_agent-0.1.6.5/chat_agent/client/web_socket_client.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.446696 chat_agent-0.1.6.5/chat_agent/config/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-03-20 17:04:34.000000 chat_agent-0.1.6.5/chat_agent/config/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      605 2023-04-08 16:45:47.000000 chat_agent-0.1.6.5/chat_agent/config/config_helper.py
--rw-r--r--   0 alex       (501) staff       (20)     1150 2023-03-31 01:41:44.000000 chat_agent-0.1.6.5/chat_agent/favicon.ico
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.447154 chat_agent-0.1.6.5/chat_agent/handler/
--rw-r--r--   0 alex       (501) staff       (20)     1048 2023-03-20 18:00:41.000000 chat_agent-0.1.6.5/chat_agent/handler/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     4356 2023-04-05 05:33:47.000000 chat_agent-0.1.6.5/chat_agent/handler/openai_handler.py
--rw-r--r--   0 alex       (501) staff       (20)     3272 2023-03-31 01:41:44.000000 chat_agent-0.1.6.5/chat_agent/key.pem
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.447507 chat_agent-0.1.6.5/chat_agent/logger/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-03-23 13:54:55.000000 chat_agent-0.1.6.5/chat_agent/logger/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     1433 2023-03-23 16:59:21.000000 chat_agent-0.1.6.5/chat_agent/logger/logger_helper.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.448115 chat_agent-0.1.6.5/chat_agent/static/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.449063 chat_agent-0.1.6.5/chat_agent/static/icon/
--rw-r--r--   0 alex       (501) staff       (20)    38340 2023-03-20 17:04:34.000000 chat_agent-0.1.6.5/chat_agent/static/icon/openai.png
--rw-r--r--   0 alex       (501) staff       (20)    23807 2023-03-20 17:04:34.000000 chat_agent-0.1.6.5/chat_agent/static/icon/whale.png
--rw-r--r--   0 alex       (501) staff       (20)     7336 2023-03-24 18:00:26.000000 chat_agent-0.1.6.5/chat_agent/static/index.html
--rw-r--r--   0 alex       (501) staff       (20)     8308 2023-04-05 17:43:03.000000 chat_agent-0.1.6.5/chat_agent/static/websocket_index.html
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.449283 chat_agent-0.1.6.5/chat_agent/test/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-04-07 05:51:34.000000 chat_agent-0.1.6.5/chat_agent/test/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.450927 chat_agent-0.1.6.5/chat_agent/util/
--rw-r--r--   0 alex       (501) staff       (20)        0 2023-03-23 14:25:57.000000 chat_agent-0.1.6.5/chat_agent/util/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      909 2023-04-08 05:17:18.000000 chat_agent-0.1.6.5/chat_agent/util/context.py
--rw-r--r--   0 alex       (501) staff       (20)       75 2023-03-23 16:56:11.000000 chat_agent-0.1.6.5/chat_agent/util/file.py
--rw-r--r--   0 alex       (501) staff       (20)      345 2023-03-23 16:08:29.000000 chat_agent-0.1.6.5/chat_agent/util/random.py
--rw-r--r--   0 alex       (501) staff       (20)      124 2023-03-24 01:09:14.000000 chat_agent-0.1.6.5/chat_agent/util/time.py
--rw-r--r--   0 alex       (501) staff       (20)      731 2023-03-31 01:41:44.000000 chat_agent-0.1.6.5/chat_agent/util/timeout.py
--rw-r--r--   0 alex       (501) staff       (20)     2956 2023-04-07 05:26:50.000000 chat_agent-0.1.6.5/chat_agent/websocket_app.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-08 16:52:22.444766 chat_agent-0.1.6.5/chat_agent.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)      263 2023-04-08 16:52:22.000000 chat_agent-0.1.6.5/chat_agent.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     1146 2023-04-08 16:52:22.000000 chat_agent-0.1.6.5/chat_agent.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-04-08 16:52:22.000000 chat_agent-0.1.6.5/chat_agent.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)      269 2023-04-08 16:52:22.000000 chat_agent-0.1.6.5/chat_agent.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       11 2023-04-08 16:52:22.000000 chat_agent-0.1.6.5/chat_agent.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2023-04-08 16:52:22.451448 chat_agent-0.1.6.5/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)      874 2023-04-08 16:47:51.000000 chat_agent-0.1.6.5/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.365045 chat_agent-0.1.6.6/
+-rw-r--r--   0 alex       (501) staff       (20)       48 2023-03-20 19:07:00.000000 chat_agent-0.1.6.6/MANIFEST.in
+-rw-r--r--   0 alex       (501) staff       (20)      263 2023-04-09 12:27:34.364852 chat_agent-0.1.6.6/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     1696 2023-04-09 12:27:15.000000 chat_agent-0.1.6.6/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.356353 chat_agent-0.1.6.6/chat_agent/
+-rw-r--r--   0 alex       (501) staff       (20)     2755 2023-04-08 16:47:51.000000 chat_agent-0.1.6.6/chat_agent/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     2893 2023-04-09 12:26:53.000000 chat_agent-0.1.6.6/chat_agent/app.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.357775 chat_agent-0.1.6.6/chat_agent/base/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-04-07 05:27:54.000000 chat_agent-0.1.6.6/chat_agent/base/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     3843 2023-04-08 16:45:47.000000 chat_agent-0.1.6.6/chat_agent/base/base_websocket.py
+-rw-r--r--   0 alex       (501) staff       (20)      223 2023-04-07 11:50:22.000000 chat_agent-0.1.6.6/chat_agent/base/singleton.py
+-rw-r--r--   0 alex       (501) staff       (20)     1550 2023-04-09 12:24:16.000000 chat_agent-0.1.6.6/chat_agent/base_websocket_app.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.358792 chat_agent-0.1.6.6/chat_agent/cache/
+-rw-r--r--   0 alex       (501) staff       (20)      252 2023-03-24 01:24:01.000000 chat_agent-0.1.6.6/chat_agent/cache/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      818 2023-03-24 01:39:51.000000 chat_agent-0.1.6.6/chat_agent/cache/cache_helper.py
+-rw-r--r--   0 alex       (501) staff       (20)     2147 2023-03-31 01:41:44.000000 chat_agent-0.1.6.6/chat_agent/cert.pem
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.359523 chat_agent-0.1.6.6/chat_agent/client/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-04-05 02:46:32.000000 chat_agent-0.1.6.6/chat_agent/client/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1055 2023-04-08 16:55:38.000000 chat_agent-0.1.6.6/chat_agent/client/base_web_socket_client.py
+-rw-r--r--   0 alex       (501) staff       (20)      670 2023-04-07 05:26:50.000000 chat_agent-0.1.6.6/chat_agent/client/web_socket_client.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.359905 chat_agent-0.1.6.6/chat_agent/config/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-03-20 17:04:34.000000 chat_agent-0.1.6.6/chat_agent/config/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      605 2023-04-08 16:45:47.000000 chat_agent-0.1.6.6/chat_agent/config/config_helper.py
+-rw-r--r--   0 alex       (501) staff       (20)     1150 2023-03-31 01:41:44.000000 chat_agent-0.1.6.6/chat_agent/favicon.ico
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.360381 chat_agent-0.1.6.6/chat_agent/handler/
+-rw-r--r--   0 alex       (501) staff       (20)     1048 2023-03-20 18:00:41.000000 chat_agent-0.1.6.6/chat_agent/handler/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     4368 2023-04-09 12:26:53.000000 chat_agent-0.1.6.6/chat_agent/handler/openai_handler.py
+-rw-r--r--   0 alex       (501) staff       (20)     3272 2023-03-31 01:41:44.000000 chat_agent-0.1.6.6/chat_agent/key.pem
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.360745 chat_agent-0.1.6.6/chat_agent/logger/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-03-23 13:54:55.000000 chat_agent-0.1.6.6/chat_agent/logger/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     1433 2023-03-23 16:59:21.000000 chat_agent-0.1.6.6/chat_agent/logger/logger_helper.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.361513 chat_agent-0.1.6.6/chat_agent/static/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.362399 chat_agent-0.1.6.6/chat_agent/static/icon/
+-rw-r--r--   0 alex       (501) staff       (20)    38340 2023-03-20 17:04:34.000000 chat_agent-0.1.6.6/chat_agent/static/icon/openai.png
+-rw-r--r--   0 alex       (501) staff       (20)    23807 2023-03-20 17:04:34.000000 chat_agent-0.1.6.6/chat_agent/static/icon/whale.png
+-rw-r--r--   0 alex       (501) staff       (20)     7336 2023-03-24 18:00:26.000000 chat_agent-0.1.6.6/chat_agent/static/index.html
+-rw-r--r--   0 alex       (501) staff       (20)     8308 2023-04-05 17:43:03.000000 chat_agent-0.1.6.6/chat_agent/static/websocket_index.html
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.362594 chat_agent-0.1.6.6/chat_agent/test/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-04-07 05:51:34.000000 chat_agent-0.1.6.6/chat_agent/test/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.364551 chat_agent-0.1.6.6/chat_agent/util/
+-rw-r--r--   0 alex       (501) staff       (20)        0 2023-03-23 14:25:57.000000 chat_agent-0.1.6.6/chat_agent/util/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)      909 2023-04-08 05:17:18.000000 chat_agent-0.1.6.6/chat_agent/util/context.py
+-rw-r--r--   0 alex       (501) staff       (20)       75 2023-03-23 16:56:11.000000 chat_agent-0.1.6.6/chat_agent/util/file.py
+-rw-r--r--   0 alex       (501) staff       (20)      345 2023-03-23 16:08:29.000000 chat_agent-0.1.6.6/chat_agent/util/random.py
+-rw-r--r--   0 alex       (501) staff       (20)      124 2023-03-24 01:09:14.000000 chat_agent-0.1.6.6/chat_agent/util/time.py
+-rw-r--r--   0 alex       (501) staff       (20)      731 2023-03-31 01:41:44.000000 chat_agent-0.1.6.6/chat_agent/util/timeout.py
+-rw-r--r--   0 alex       (501) staff       (20)     2964 2023-04-09 12:26:53.000000 chat_agent-0.1.6.6/chat_agent/websocket_app.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 12:27:34.357231 chat_agent-0.1.6.6/chat_agent.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)      263 2023-04-09 12:27:34.000000 chat_agent-0.1.6.6/chat_agent.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     1146 2023-04-09 12:27:34.000000 chat_agent-0.1.6.6/chat_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-04-09 12:27:34.000000 chat_agent-0.1.6.6/chat_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)      269 2023-04-09 12:27:34.000000 chat_agent-0.1.6.6/chat_agent.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       11 2023-04-09 12:27:34.000000 chat_agent-0.1.6.6/chat_agent.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)       38 2023-04-09 12:27:34.365099 chat_agent-0.1.6.6/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)      874 2023-04-09 12:27:08.000000 chat_agent-0.1.6.6/setup.py
```

### Comparing `chat_agent-0.1.6.5/README.md` & `chat_agent-0.1.6.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # 简单的OpenAI chatGPT代理
 
 ### 安装
 ```
 使用pip安装最新版本，指定到官方pypi源
-pip install chat-agent==0.1.6.5 -i https://pypi.org/simple/
+pip install chat-agent==0.1.6.6 -i https://pypi.org/simple/
 ```
 
 ### 环境变量配置项：
 ```
 必配：
 OPENAI_ORGANIZATION_KEY: openai对应的组织id
 OPENAI_API_KEY: openai分配的api key
```

### Comparing `chat_agent-0.1.6.5/chat_agent/__init__.py` & `chat_agent-0.1.6.6/chat_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.5/chat_agent/app.py` & `chat_agent-0.1.6.6/chat_agent/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 CORS(app)
 
 logger = get_logger('app')
 
 
 @app.route('/')
 def index():
-    sid = get_thread_context()['sid']
-    ip = get_thread_context()['remote_ip']
+    sid = get_thread_context().get('sid')
+    ip = get_thread_context().get('remote_ip')
     logger.debug('new guest, sid: {} ip: {}'.format(sid, ip))
     return send_from_directory(app.static_folder, 'index.html')
 
 
 @app.route('/chat')
 @timeout_decorator(CHAT_AGENT_TIMEOUT)
 def chat():
@@ -48,15 +48,15 @@
 
 
 @app.before_request
 def before():
     if 'sid' not in session:
         sid = random.get_random_md5()
         session['sid'] = sid
-    sid = session['sid']
+    sid = session.get('sid')
     get_thread_context()['sid'] = sid
     get_thread_context()['remote_ip'] = request.remote_addr
 
 
 @socketio.on('websock_chat')
 def websock_chat():
     try:
```

### Comparing `chat_agent-0.1.6.5/chat_agent/base/base_websocket.py` & `chat_agent-0.1.6.6/chat_agent/base/base_websocket.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.5/chat_agent/base_websocket_app.py` & `chat_agent-0.1.6.6/chat_agent/base_websocket_app.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,29 +19,29 @@
     context['sid'] = sid
     context['remote_ip'] = get_remote_ip()
     logger.info('客户端已连接, sid: {} ip: {}'.format(sid, get_remote_ip()))
 
 
 @server.on('disconnect')
 def handle_disconnect():
-    sid = get_thread_context()['sid']
+    sid = get_thread_context().get('sid')
     logger.info('客户端已断开连接, sid: {}'.format(sid))
     set_thread_context(None)
 
 
 @server.on('websocket_chat')
 def websock_chat(data):
     context = get_thread_context()
     request_msg = json.loads(data)
-    if 'sid' in request_msg:
-        context['sid'] = request_msg['sid']
+    if request_msg.get('sid'):
+        context['sid'] = request_msg.get('sid')
     else:
         sid = random.get_random_md5()
         context['sid'] = sid
-    for response_message in send_chat_message_with_socket_steam_response(msg=request_msg['data'], chat_log=None):
+    for response_message in send_chat_message_with_socket_steam_response(msg=request_msg.get('data'), chat_log=None):
         send_message('websocket_chat', response_message)
 
 
 def start_socket_agent():
     server.start(CHAT_AGENT_HOST, CHAT_AGENT_WEBSOCKET_PORT)
```

### Comparing `chat_agent-0.1.6.5/chat_agent/cache/cache_helper.py` & `chat_agent-0.1.6.6/chat_agent/cache/cache_helper.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.5/chat_agent/cert.pem` & `chat_agent-0.1.6.6/chat_agent/cert.pem`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.5/chat_agent/client/base_web_socket_client.py` & `chat_agent-0.1.6.6/chat_agent/client/base_web_socket_client.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.5/chat_agent/client/web_socket_client.py` & `chat_agent-0.1.6.6/chat_agent/client/web_socket_client.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.5/chat_agent/config/config_helper.py` & `chat_agent-0.1.6.6/chat_agent/config/config_helper.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.5/chat_agent/favicon.ico` & `chat_agent-0.1.6.6/chat_agent/favicon.ico`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.5/chat_agent/handler/__init__.py` & `chat_agent-0.1.6.6/chat_agent/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.5/chat_agent/handler/openai_handler.py` & `chat_agent-0.1.6.6/chat_agent/handler/openai_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         return num_tokens
     else:
         raise NotImplementedError(f"""num_tokens_from_messages() is not presently implemented for model {model}.
   See https://github.com/openai/openai-python/blob/main/chatml.md for information on how messages are converted to tokens.""")
 
 
 def get_valid_chat_log(chat_log: []):
-    sid = get_thread_context()['sid']
+    sid = get_thread_context().get('sid')
     valid_context_chat_log = []
     for chat in chat_log:
         if 'user' == chat['role']:
             valid_context_chat_log.append(chat)
         elif 'system' == chat['role']:
             valid_context_chat_log.append(chat)
     temp_messages = valid_context_chat_log[-CHAT_ROUND:]
@@ -48,15 +48,15 @@
         else:
             logger.debug('sid: {} current token count: {}'.format(sid, token_count))
             break
     return temp_messages
 
 
 def send_chat_message_with_steam_response(msg: str, chat_log: [] = None):
-    sid = get_thread_context()['sid']
+    sid = get_thread_context().get('sid')
     ip = get_thread_context()['remote_ip']
     logger.debug('receive msg, sid: {} ip: {} msg: {}'.format(sid, ip, msg))
     is_need_cache = False
     if not chat_log:
         chat_log = get_cache(CHAT_LOG, sid=sid)
         is_need_cache = True
     cur_msg = {'role': 'user', 'content': msg}
@@ -95,15 +95,15 @@
     except Exception as e:
         logger.error('send message has exception, msg: ' + e)
 
 
 def send_chat_message_with_socket_steam_response(msg: str, chat_log: [] = None):
     msg_id = random.get_random_md5()
     index = 0
-    sid = get_thread_context()['sid']
+    sid = get_thread_context().get('sid')
     for response in send_chat_message_with_steam_response(msg=msg, chat_log=chat_log):
         response_msg = {
             'sid': sid,
             'msg_id': msg_id,
             'index': index,
             'data': response,
             'end': False
```

### Comparing `chat_agent-0.1.6.5/chat_agent/key.pem` & `chat_agent-0.1.6.6/chat_agent/key.pem`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.5/chat_agent/logger/logger_helper.py` & `chat_agent-0.1.6.6/chat_agent/logger/logger_helper.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.5/chat_agent/static/icon/openai.png` & `chat_agent-0.1.6.6/chat_agent/static/icon/openai.png`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.5/chat_agent/static/icon/whale.png` & `chat_agent-0.1.6.6/chat_agent/static/icon/whale.png`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.5/chat_agent/static/index.html` & `chat_agent-0.1.6.6/chat_agent/static/index.html`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.5/chat_agent/static/websocket_index.html` & `chat_agent-0.1.6.6/chat_agent/static/websocket_index.html`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.5/chat_agent/util/context.py` & `chat_agent-0.1.6.6/chat_agent/util/context.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.5/chat_agent/util/timeout.py` & `chat_agent-0.1.6.6/chat_agent/util/timeout.py`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.5/chat_agent/websocket_app.py` & `chat_agent-0.1.6.6/chat_agent/websocket_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 CORS(app)
 
 logger = get_logger('websocket_app')
 
 
 @app.route('/')
 def index():
-    sid = get_thread_context()['sid']
+    sid = get_thread_context().get('sid')
     ip = get_thread_context()['remote_ip']
     logger.debug('new guest, sid: {} ip: {}'.format(sid, ip))
     return send_from_directory(app.static_folder, 'websocket_index.html')
 
 
 @app.route('/.<path:hidden_path>')
 def ssl_check(hidden_path):
@@ -54,15 +54,15 @@
     get_thread_context()['sid'] = sid
     get_thread_context()['remote_ip'] = request.remote_addr
     logger.info('客户端已连接, sid: {} ip: {}'.format(sid, request.remote_addr))
 
 
 @socketio.on('disconnect')
 def handle_disconnect():
-    sid = get_thread_context()['sid']
+    sid = get_thread_context().get('sid')
     logger.info('客户端已断开连接, sid: {}'.format(sid))
     set_thread_context(None)
 
 
 @socketio.on('websocket_chat')
 def websock_chat(msg):
     request_msg = json.loads(msg)
```

### Comparing `chat_agent-0.1.6.5/chat_agent.egg-info/SOURCES.txt` & `chat_agent-0.1.6.6/chat_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chat_agent-0.1.6.5/setup.py` & `chat_agent-0.1.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chat_agent",
-    version="0.1.6.5",
+    version="0.1.6.6",
     packages=find_packages(),
     zip_sage=False,
     include_package_data=True,
     install_requires=[
         'setuptools~=63.4.1',
         'flask~=2.2.2',
         'flask_cors~=3.0.10',
```

