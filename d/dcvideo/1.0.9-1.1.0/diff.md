# Comparing `tmp/dcvideo-1.0.9.tar.gz` & `tmp/dcvideo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcvideo-1.0.9.tar", last modified: Sun Apr  2 08:11:47 2023, max compression
+gzip compressed data, was "dcvideo-1.1.0.tar", last modified: Sun Apr  9 16:30:11 2023, max compression
```

## Comparing `dcvideo-1.0.9.tar` & `dcvideo-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 netfere    (501) staff       (20)        0 2023-04-02 08:11:47.721564 dcvideo-1.0.9/
--rw-r--r--   0 netfere    (501) staff       (20)      223 2023-04-02 08:11:47.721287 dcvideo-1.0.9/PKG-INFO
-drwxr-xr-x   0 netfere    (501) staff       (20)        0 2023-04-02 08:11:47.718493 dcvideo-1.0.9/dcvideo/
--rw-r--r--   0 netfere    (501) staff       (20)        0 2023-04-02 06:57:57.000000 dcvideo-1.0.9/dcvideo/__init__.py
--rw-r--r--   0 netfere    (501) staff       (20)     3744 2023-04-02 08:11:25.000000 dcvideo-1.0.9/dcvideo/config.py
--rw-r--r--   0 netfere    (501) staff       (20)     6163 2023-04-02 07:24:52.000000 dcvideo-1.0.9/dcvideo/export.py
--rw-r--r--   0 netfere    (501) staff       (20)     5379 2023-04-02 07:23:40.000000 dcvideo-1.0.9/dcvideo/message.py
--rw-r--r--   0 netfere    (501) staff       (20)      894 2023-04-02 03:47:14.000000 dcvideo-1.0.9/dcvideo/object.py
--rw-r--r--   0 netfere    (501) staff       (20)    11472 2023-04-02 07:24:37.000000 dcvideo-1.0.9/dcvideo/publish.py
--rw-r--r--   0 netfere    (501) staff       (20)      304 2023-04-02 07:23:43.000000 dcvideo-1.0.9/dcvideo/result.py
--rw-r--r--   0 netfere    (501) staff       (20)     4606 2023-04-02 07:24:15.000000 dcvideo-1.0.9/dcvideo/utils.py
--rw-r--r--   0 netfere    (501) staff       (20)     2683 2023-04-02 05:52:29.000000 dcvideo-1.0.9/dcvideo/web.py
--rw-r--r--   0 netfere    (501) staff       (20)    10085 2023-04-02 07:23:46.000000 dcvideo-1.0.9/dcvideo/youban.py
-drwxr-xr-x   0 netfere    (501) staff       (20)        0 2023-04-02 08:11:47.720899 dcvideo-1.0.9/dcvideo.egg-info/
--rw-r--r--   0 netfere    (501) staff       (20)      223 2023-04-02 08:11:47.000000 dcvideo-1.0.9/dcvideo.egg-info/PKG-INFO
--rw-r--r--   0 netfere    (501) staff       (20)      376 2023-04-02 08:11:47.000000 dcvideo-1.0.9/dcvideo.egg-info/SOURCES.txt
--rw-r--r--   0 netfere    (501) staff       (20)        1 2023-04-02 08:11:47.000000 dcvideo-1.0.9/dcvideo.egg-info/dependency_links.txt
--rw-r--r--   0 netfere    (501) staff       (20)      113 2023-04-02 08:11:47.000000 dcvideo-1.0.9/dcvideo.egg-info/entry_points.txt
--rw-r--r--   0 netfere    (501) staff       (20)      122 2023-04-02 08:11:47.000000 dcvideo-1.0.9/dcvideo.egg-info/requires.txt
--rw-r--r--   0 netfere    (501) staff       (20)        8 2023-04-02 08:11:47.000000 dcvideo-1.0.9/dcvideo.egg-info/top_level.txt
--rw-r--r--   0 netfere    (501) staff       (20)       38 2023-04-02 08:11:47.721673 dcvideo-1.0.9/setup.cfg
--rw-r--r--   0 netfere    (501) staff       (20)      813 2023-04-02 07:50:13.000000 dcvideo-1.0.9/setup.py
+drwxr-xr-x   0 netfere    (501) staff       (20)        0 2023-04-09 16:30:11.753178 dcvideo-1.1.0/
+-rw-r--r--   0 netfere    (501) staff       (20)      223 2023-04-09 16:30:11.752936 dcvideo-1.1.0/PKG-INFO
+drwxr-xr-x   0 netfere    (501) staff       (20)        0 2023-04-09 16:30:11.750910 dcvideo-1.1.0/dcvideo/
+-rw-r--r--   0 netfere    (501) staff       (20)        0 2023-04-02 06:57:57.000000 dcvideo-1.1.0/dcvideo/__init__.py
+-rw-r--r--   0 netfere    (501) staff       (20)     5380 2023-04-02 08:30:31.000000 dcvideo-1.1.0/dcvideo/_message.py
+-rw-r--r--   0 netfere    (501) staff       (20)      894 2023-04-02 03:47:14.000000 dcvideo-1.1.0/dcvideo/_object.py
+-rw-r--r--   0 netfere    (501) staff       (20)      305 2023-04-02 08:30:31.000000 dcvideo-1.1.0/dcvideo/_result.py
+-rw-r--r--   0 netfere    (501) staff       (20)    10210 2023-04-02 16:15:46.000000 dcvideo-1.1.0/dcvideo/_youban.py
+-rw-r--r--   0 netfere    (501) staff       (20)     3886 2023-04-09 16:30:01.000000 dcvideo-1.1.0/dcvideo/config.py
+-rw-r--r--   0 netfere    (501) staff       (20)     6165 2023-04-02 08:30:31.000000 dcvideo-1.1.0/dcvideo/export.py
+-rw-r--r--   0 netfere    (501) staff       (20)    11475 2023-04-02 08:30:31.000000 dcvideo-1.1.0/dcvideo/publish.py
+-rw-r--r--   0 netfere    (501) staff       (20)     4607 2023-04-02 08:30:31.000000 dcvideo-1.1.0/dcvideo/utils.py
+-rw-r--r--   0 netfere    (501) staff       (20)     2536 2023-04-02 12:01:59.000000 dcvideo-1.1.0/dcvideo/web.py
+drwxr-xr-x   0 netfere    (501) staff       (20)        0 2023-04-09 16:30:11.752578 dcvideo-1.1.0/dcvideo.egg-info/
+-rw-r--r--   0 netfere    (501) staff       (20)      223 2023-04-09 16:30:11.000000 dcvideo-1.1.0/dcvideo.egg-info/PKG-INFO
+-rw-r--r--   0 netfere    (501) staff       (20)      380 2023-04-09 16:30:11.000000 dcvideo-1.1.0/dcvideo.egg-info/SOURCES.txt
+-rw-r--r--   0 netfere    (501) staff       (20)        1 2023-04-09 16:30:11.000000 dcvideo-1.1.0/dcvideo.egg-info/dependency_links.txt
+-rw-r--r--   0 netfere    (501) staff       (20)      113 2023-04-09 16:30:11.000000 dcvideo-1.1.0/dcvideo.egg-info/entry_points.txt
+-rw-r--r--   0 netfere    (501) staff       (20)      122 2023-04-09 16:30:11.000000 dcvideo-1.1.0/dcvideo.egg-info/requires.txt
+-rw-r--r--   0 netfere    (501) staff       (20)        8 2023-04-09 16:30:11.000000 dcvideo-1.1.0/dcvideo.egg-info/top_level.txt
+-rw-r--r--   0 netfere    (501) staff       (20)       38 2023-04-09 16:30:11.753270 dcvideo-1.1.0/setup.cfg
+-rw-r--r--   0 netfere    (501) staff       (20)      813 2023-04-02 07:50:13.000000 dcvideo-1.1.0/setup.py
```

### Comparing `dcvideo-1.0.9/dcvideo/config.py` & `dcvideo-1.1.0/dcvideo/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import re
 from tkinter import filedialog
 from .utils import port_is_used,get_host_ip
 
 filepath = os.path.join(os.path.dirname(__file__), 'config.ini')
 config = configparser.ConfigParser()
-VERSION = '1.0.9'
+VERSION = '1.1.0'
 HOST = 'https://www.shortvideo.work'
 
 def save_config(section,key,value):
     config.read(filepath)
     if not config.has_section(section):
         config.add_section(section)
     config.set(section, key, value)
@@ -27,14 +27,19 @@
 
     if not config.has_section('server'):
         config.add_section("server")
         config.set("server", "host", HOST)
         config.write(open(filepath, "w"))
 
     version = config.get('video', 'version', fallback=VERSION)
+    if version!=VERSION:
+        version = VERSION
+        config.set('video', 'version', VERSION)
+        config.write(open(filepath, "w"))
+
     host = config.get('server', 'host', fallback=HOST)
     appid = config.get('server', 'appid', fallback='')
     appsecret = config.get('server', 'appsecret', fallback='')
 
     while not appid:
         value = input('请输入appid：')
         if value:
```

### Comparing `dcvideo-1.0.9/dcvideo/export.py` & `dcvideo-1.1.0/dcvideo/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import os
 import signal
 import sys
 
 import requests
 
 from .config import read, read_workdir, save_config
-from .message import ExportMessage
-from .result import Result
+from ._message import ExportMessage
+from ._result import Result
 from .utils import download, md5_value, sign_dict, ymd
 
 log = logging.getLogger(__name__)
 
 class Export:
     def __init__(self, version: str, host: str, workdir: str, appid: str, appsecret: str) -> None:
         self.do_action = ''
```

### Comparing `dcvideo-1.0.9/dcvideo/message.py` & `dcvideo-1.1.0/dcvideo/_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import math
-from .object import Object
+from ._object import Object
 from typing import Any, List, Union
 
 
 class VideoValue(Object):
     def __init__(self, title: str, category: str, tag: List[str], source: int, activity: Union[int, None], **kwargs) -> None:
         self.title = title
         self.category = category
```

### Comparing `dcvideo-1.0.9/dcvideo/object.py` & `dcvideo-1.1.0/dcvideo/_object.py`

 * *Files identical despite different names*

### Comparing `dcvideo-1.0.9/dcvideo/publish.py` & `dcvideo-1.1.0/dcvideo/publish.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import os
 import signal
 import sys
 
 import requests
 
 from .config import read, read_workdir, save_config
-from .message import Message
-from .result import Result
-from .youban import Youban
+from ._message import Message
+from ._result import Result
+from ._youban import Youban
 from .utils import download, md5_value, sign_dict, to_cos
 
 log = logging.getLogger(__name__)
 
 
 class Publish:
     do_action: str
```

### Comparing `dcvideo-1.0.9/dcvideo/utils.py` & `dcvideo-1.1.0/dcvideo/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from contextlib import closing
 from typing import Callable
 
 import requests
 from qcloud_cos import CosConfig, CosS3Client
 from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
 
-from .result import Result
+from ._result import Result
 
 
 def ymd():
     return datetime.datetime.now().strftime('%Y%m%d')
 
 
 def sign_dict(data, secret):
```

### Comparing `dcvideo-1.0.9/dcvideo/web.py` & `dcvideo-1.1.0/dcvideo/web.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 from flask import Flask, request, jsonify, send_from_directory
 from flask_cors import cross_origin, CORS
 import os
 import datetime
 import argparse
-from .config import read_web,save_config
+from .config import read_web, save_config
 
-BASE_URL = ''  # f'http://{get_host_ip()}:8019'
-
-# 获取当前文件所在目录的绝对路径
-BASE_DIR = os.path.abspath(os.path.dirname(__file__))
-
-
-UPLOAD_PATH = ''  # os.path.join(BASE_DIR, 'static')
+BASE_URL = ''
 
 app = Flask(__name__)
 CORS(app)
 
 
 @app.route('/ping')
 @cross_origin(origins='*')
@@ -45,50 +39,50 @@
 
     isVideo = f.mimetype.startswith('video/mp4')
     isImage = f.mimetype.startswith('image/')
     if not isVideo and not isImage:
         return jsonify({'success': False, 'msg': '必须上传mp4或图片文件'})
 
     save_dir = os.path.join(
-        UPLOAD_PATH, datetime.date.today().strftime('%Y%m%d'))
+        app.static_folder, datetime.date.today().strftime('%Y%m%d'))
     # 如果目录不存在则创建
     if not os.path.exists(save_dir):
         os.makedirs(save_dir)
 
     # 保存文件
     save_path = os.path.join(save_dir, key)
     f.save(save_path)
-    url_path = save_path.replace(BASE_DIR, '')
+    url_path = save_path.replace(app.static_folder, '').replace('\\', '/')
     # 返回文件路径
-    return jsonify({'success': True, 'msg': BASE_URL+url_path})
+    return jsonify({'success': True, 'msg': f"{BASE_URL}/static{url_path}"})
 
 
 def run(host: str, port: int, workdir: str):
-    global BASE_URL, UPLOAD_PATH
+    global BASE_URL
     BASE_URL = f'http://{host}:{port}'
-    UPLOAD_PATH = workdir
+    app.static_folder = workdir
     app.run(host=host, port=port, threaded=True)
 
 
 def main():
-    
+
     version, host, port, workdir = read_web()
     if not port or not workdir:
         return
     parser = argparse.ArgumentParser()
     parser.add_argument('-port', type=int, default=0)
     parser.add_argument('-dir', type=str, default='')
 
     args = parser.parse_args()
-    if args.port and args.port!=port:
+    if args.port and args.port != port:
         port = args.port
-        save_config('web','port',port)
+        save_config('web', 'port', port)
 
-    if args.dir and args.dir!=workdir:
+    if args.dir and args.dir != workdir:
         if not os.path.exists(args.dir):
             print(f'{args.dir}目录不存在')
             return
         workdir = args.dir
-        save_config('web','workdir',workdir)
+        save_config('web', 'workdir', workdir)
 
     print(f'\n\n《八戒来了之上传服务 - {version}》\nhost：{host}:{port}\n工作目录：{workdir}\n')
     run(host, port, workdir)
```

### Comparing `dcvideo-1.0.9/dcvideo/youban.py` & `dcvideo-1.1.0/dcvideo/_youban.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 from typing import List
 
 import requests
 from fake_useragent import UserAgent
 from requests.cookies import RequestsCookieJar
 
-from .message import Account
-from .object import Object
-from .result import Result
+from ._message import Account
+from ._object import Object
+from ._result import Result
 
 # https://gist.github.com/kazqvaizer/4cebebe5db654a414132809f9f88067b
 
 
 def multipartify(data, parent_key=None, formatter: callable = None) -> dict:
     if formatter is None:
         def formatter(v): return (None, v)  # Multipart representation of value
@@ -128,24 +128,27 @@
         self.cookies = None
         self.xsrfToken = ''
 
     async def api_get_token(self, module: str):
         """
             module = upload_video | upload_cover
         """
-        url = f'https://{self.platform}.xiaozhuyouban.com/video/publish/uploadtoken?app_id={self.account.app_id}&app_token={self.account.app_token}&module={module}'
-        response = requests.get(url)
-        if response.status_code == 200:
-            data = response.json()
-            if data.get('code') == 0 and data.get('data') and data['data'].get('cos'):
-                return Result(True, data=data['data'].get('cos'))
+        try:
+            url = f'https://{self.platform}.xiaozhuyouban.com/video/publish/uploadtoken?app_id={self.account.app_id}&app_token={self.account.app_token}&module={module}'
+            response = requests.get(url)
+            if response.status_code == 200:
+                data = response.json()
+                if data.get('code') == 0 and data.get('data') and data['data'].get('cos'):
+                    return Result(True, data=data['data'].get('cos'))
+                else:
+                    return Result(msg=data.get('message') or '获取上传token失败')
             else:
-                return Result(msg=data.get('message') or '获取上传token失败')
-        else:
-            return Result(msg='获取上传token失败')
+                return Result(msg='获取上传token失败')
+        except Exception as e:
+            return Result(msg=str(e))
 
     async def api_submit(self,payload: dict):
         data = VideoPayload(**payload).get_data('api',self.platform)
         data['app_id'] = self.account.app_id
         data['app_token'] = self.account.app_token
         
         headers = {'Content-Type': 'application/json'}
```

### Comparing `dcvideo-1.0.9/setup.py` & `dcvideo-1.1.0/setup.py`

 * *Files identical despite different names*

