# Comparing `tmp/k-amino.py-1.0.8.tar.gz` & `tmp/k-amino.py-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k-amino.py-1.0.8.tar", last modified: Fri Mar 17 22:22:40 2023, max compression
+gzip compressed data, was "k-amino.py-1.1.0.tar", last modified: Sun Apr  9 01:21:22 2023, max compression
```

## Comparing `k-amino.py-1.0.8.tar` & `k-amino.py-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-03-17 22:22:40.109278 k-amino.py-1.0.8/
--rw-rw-rw-   0        0        0      586 2023-03-10 16:12:29.000000 k-amino.py-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     2157 2023-03-17 22:22:40.110282 k-amino.py-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1596 2023-03-17 20:55:37.000000 k-amino.py-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-17 22:22:40.065271 k-amino.py-1.0.8/k_amino/
--rw-rw-rw-   0        0        0      628 2023-03-17 20:55:37.000000 k-amino.py-1.0.8/k_amino/__init__.py
--rw-rw-rw-   0        0        0     3749 2023-03-17 22:19:00.000000 k-amino.py-1.0.8/k_amino/acm.py
--rw-rw-rw-   0        0        0     2058 2023-03-17 20:55:37.000000 k-amino.py-1.0.8/k_amino/bot.py
--rw-rw-rw-   0        0        0    30337 2023-03-17 22:22:07.000000 k-amino.py-1.0.8/k_amino/client.py
-drwxrwxrwx   0        0        0        0 2023-03-17 22:22:40.106283 k-amino.py-1.0.8/k_amino/lib/
--rw-rw-rw-   0        0        0       95 2023-03-17 20:55:37.000000 k-amino.py-1.0.8/k_amino/lib/__init__.py
--rw-rw-rw-   0        0        0     8314 2023-03-17 20:55:37.000000 k-amino.py-1.0.8/k_amino/lib/exception.py
--rw-rw-rw-   0        0        0     1986 2023-03-17 20:55:37.000000 k-amino.py-1.0.8/k_amino/lib/headers.py
--rw-rw-rw-   0        0        0   198102 2023-03-17 20:55:37.000000 k-amino.py-1.0.8/k_amino/lib/objects.py
--rw-rw-rw-   0        0        0     2422 2023-03-17 20:55:37.000000 k-amino.py-1.0.8/k_amino/lib/sessions.py
--rw-rw-rw-   0        0        0      771 2023-03-17 20:55:37.000000 k-amino.py-1.0.8/k_amino/lib/util.py
--rw-rw-rw-   0        0        0    45167 2023-03-17 20:55:37.000000 k-amino.py-1.0.8/k_amino/local.py
--rw-rw-rw-   0        0        0    23193 2023-03-17 20:55:37.000000 k-amino.py-1.0.8/k_amino/sockets.py
-drwxrwxrwx   0        0        0        0 2023-03-17 22:22:40.086263 k-amino.py-1.0.8/k_amino.py.egg-info/
--rw-rw-rw-   0        0        0     2157 2023-03-17 22:22:39.000000 k-amino.py-1.0.8/k_amino.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2023-03-17 22:22:39.000000 k-amino.py-1.0.8/k_amino.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-17 22:22:39.000000 k-amino.py-1.0.8/k_amino.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-03-17 22:22:39.000000 k-amino.py-1.0.8/k_amino.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-17 22:22:39.000000 k-amino.py-1.0.8/k_amino.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-17 22:22:40.114287 k-amino.py-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1377 2023-03-11 05:05:25.000000 k-amino.py-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 01:21:22.345925 k-amino.py-1.1.0/
+-rw-rw-rw-   0        0        0      586 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2143 2023-04-09 01:21:22.346931 k-amino.py-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1596 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 01:21:22.243178 k-amino.py-1.1.0/k_amino/
+-rw-rw-rw-   0        0        0      872 2023-04-09 01:09:36.000000 k-amino.py-1.1.0/k_amino/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-09 01:21:22.278179 k-amino.py-1.1.0/k_amino/k_async/
+-rw-rw-rw-   0        0        0      122 2023-04-09 01:08:06.000000 k-amino.py-1.1.0/k_amino/k_async/__init__.py
+-rw-rw-rw-   0        0        0     3922 2023-04-07 02:03:55.000000 k-amino.py-1.1.0/k_amino/k_async/acm.py
+-rw-rw-rw-   0        0        0     1950 2023-04-07 03:16:23.000000 k-amino.py-1.1.0/k_amino/k_async/bot.py
+-rw-rw-rw-   0        0        0    31693 2023-04-07 03:34:54.000000 k-amino.py-1.1.0/k_amino/k_async/client.py
+-rw-rw-rw-   0        0        0    46342 2023-04-07 02:21:35.000000 k-amino.py-1.1.0/k_amino/k_async/local.py
+-rw-rw-rw-   0        0        0    24649 2023-04-07 03:42:28.000000 k-amino.py-1.1.0/k_amino/k_async/sockets.py
+drwxrwxrwx   0        0        0        0 2023-04-09 01:21:22.295180 k-amino.py-1.1.0/k_amino/k_sync/
+-rw-rw-rw-   0        0        0      102 2023-04-09 01:08:25.000000 k-amino.py-1.1.0/k_amino/k_sync/__init__.py
+-rw-rw-rw-   0        0        0     3751 2023-04-07 01:34:38.000000 k-amino.py-1.1.0/k_amino/k_sync/acm.py
+-rw-rw-rw-   0        0        0     1912 2023-04-09 01:12:28.000000 k-amino.py-1.1.0/k_amino/k_sync/bot.py
+-rw-rw-rw-   0        0        0    30339 2023-04-07 01:34:43.000000 k-amino.py-1.1.0/k_amino/k_sync/client.py
+-rw-rw-rw-   0        0        0    45169 2023-04-07 01:37:06.000000 k-amino.py-1.1.0/k_amino/k_sync/local.py
+-rw-rw-rw-   0        0        0    23210 2023-04-09 01:13:33.000000 k-amino.py-1.1.0/k_amino/k_sync/sockets.py
+drwxrwxrwx   0        0        0        0 2023-04-09 01:21:22.311192 k-amino.py-1.1.0/k_amino/lib/
+-rw-rw-rw-   0        0        0       95 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_amino/lib/__init__.py
+-rw-rw-rw-   0        0        0     2803 2023-04-07 05:28:51.000000 k-amino.py-1.1.0/k_amino/lib/async_sessions.py
+-rw-rw-rw-   0        0        0     8314 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_amino/lib/exception.py
+-rw-rw-rw-   0        0        0     1986 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_amino/lib/headers.py
+-rw-rw-rw-   0        0        0   198102 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_amino/lib/objects.py
+-rw-rw-rw-   0        0        0     2422 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_amino/lib/sessions.py
+-rw-rw-rw-   0        0        0     1244 2023-04-09 01:09:13.000000 k-amino.py-1.1.0/k_amino/lib/util.py
+drwxrwxrwx   0        0        0        0 2023-04-09 01:21:22.264180 k-amino.py-1.1.0/k_amino.py.egg-info/
+-rw-rw-rw-   0        0        0     2143 2023-04-09 01:21:21.000000 k-amino.py-1.1.0/k_amino.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      926 2023-04-09 01:21:22.000000 k-amino.py-1.1.0/k_amino.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 01:21:21.000000 k-amino.py-1.1.0/k_amino.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2023-04-09 01:21:21.000000 k-amino.py-1.1.0/k_amino.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-09 01:21:21.000000 k-amino.py-1.1.0/k_amino.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 01:21:22.328926 k-amino.py-1.1.0/k_asyncOld/
+-rw-rw-rw-   0        0        0       79 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_asyncOld/__init__.py
+-rw-rw-rw-   0        0        0     5940 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_asyncOld/acm.py
+-rw-rw-rw-   0        0        0    40417 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_asyncOld/client.py
+drwxrwxrwx   0        0        0        0 2023-04-09 01:21:22.342913 k-amino.py-1.1.0/k_asyncOld/lib/
+-rw-rw-rw-   0        0        0       95 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_asyncOld/lib/__init__.py
+-rw-rw-rw-   0        0        0     8314 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_asyncOld/lib/exception.py
+-rw-rw-rw-   0        0        0     1631 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_asyncOld/lib/headers.py
+-rw-rw-rw-   0        0        0   198118 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_asyncOld/lib/objects.py
+-rw-rw-rw-   0        0        0      768 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_asyncOld/lib/util.py
+-rw-rw-rw-   0        0        0    55364 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_asyncOld/local.py
+-rw-rw-rw-   0        0        0    24930 2023-03-17 22:23:53.000000 k-amino.py-1.1.0/k_asyncOld/sockets.py
+-rw-rw-rw-   0        0        0       42 2023-04-09 01:21:22.350917 k-amino.py-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1363 2023-04-07 01:13:01.000000 k-amino.py-1.1.0/setup.py
```

### Comparing `k-amino.py-1.0.8/LICENSE` & `k-amino.py-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.0.8/PKG-INFO` & `k-amino.py-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: k-amino.py
-Version: 1.0.8
+Version: 1.1.0
 Summary: Amino Bots with python!
 Home-page: https://github.com/kwel999/KAmino
 Download-URL: https://github.com/kwel999/KAmino/archive/refs/heads/main.zip
-Author: KWEL, ThePhoenix78
+Author: KWEL
 Author-email: itskwel999@gmail.com
 License: Apache
 Keywords: api,python,python3,python3.x,KWEL,kwel999,kwel.py,Amino,kamino,kamino pyK-Amino,kamino,kamino,kamino-bot,kamino-bots,kamino-bot,ndc,narvii.apps,aminoapps,kamino-py,kamino,kamino-bot,narvii
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## k_amino
```

### Comparing `k-amino.py-1.0.8/README.md` & `k-amino.py-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.0.8/k_amino/acm.py` & `k-amino.py-1.1.0/k_amino/k_sync/acm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from time import time as timestamp
 
-from .lib.objects import *
-from .lib.sessions import Session
+from ..lib.objects import *
+from ..lib.sessions import Session
 
 
 class Acm(Session):
     def __init__(self, comId: str, proxies: dict = None):
         self.comId = comId
         self.proxies = proxies
```

### Comparing `k-amino.py-1.0.8/k_amino/bot.py` & `k-amino.py-1.1.0/k_amino/k_sync/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 from easy_events import Events, Parameters
 
 from .local import SubClient
-from .acm import Acm
 
 
 class Bot(Events):
     def __init__(self, prefix: str = "!"):
-        try:
-            Events.__init__(self, prefix=prefix, str_only=True, first_parameter_object=True, default_event=False)
-        except Exception:
-            Events.__init__(self, prefix=prefix, str_only=True, first_parameter_object=True)
+        Events.__init__(self, prefix=prefix, str_only=True, first_parameter_object=True, default_event=False)
 
         # to make @client.command()
         self.command = self.add_event
 
     def build_parameters(self, obj_data):
-        data = Parameters(data=obj_data.message.content, prefix=self.prefix)
+        data = Parameters(data=obj_data.message.content, prefix=self.prefix, str_only=True)
 
         for k, v in obj_data.__dict__.items():
             setattr(data, k, v)
 
         for k, v in obj_data.message.__dict__.items():
             if k != "json":
                 setattr(data, k, v)
```

### Comparing `k-amino.py-1.0.8/k_amino/client.py` & `k-amino.py-1.1.0/k_amino/k_sync/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 from base64 import b64encode
 from binascii import hexlify
 from time import time as timestamp
 from typing import BinaryIO, Union
 from uuid import UUID
 
-from .lib.objects import *
-from .lib.sessions import Session
+from ..lib.objects import *
+from ..lib.sessions import Session
 from .sockets import Wss
 
 
 class Client(Wss, Session):
     def __init__(self, deviceId: str = None, proxies: dict = None, trace: bool = False, bot: bool = False):
         self.trace = trace
         self.proxies = proxies
```

### Comparing `k-amino.py-1.0.8/k_amino/lib/exception.py` & `k-amino.py-1.1.0/k_amino/lib/exception.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.0.8/k_amino/lib/headers.py` & `k-amino.py-1.1.0/k_amino/lib/headers.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.0.8/k_amino/lib/objects.py` & `k-amino.py-1.1.0/k_amino/lib/objects.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.0.8/k_amino/lib/sessions.py` & `k-amino.py-1.1.0/k_amino/lib/sessions.py`

 * *Files identical despite different names*

### Comparing `k-amino.py-1.0.8/k_amino/lib/util.py` & `k-amino.py-1.1.0/k_asyncOld/lib/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import base64
 import hashlib
 import hmac
 from uuid import uuid4
 
 # tapjoy = "https://ads.tapdaq.com/v4/analytics/reward"
+api = "https://service.narvii.com/api/v1{}".format
 webApi = "https://aminoapps.com/api{}".format
-api = "https://service.aminoapps.com/api/v1{}".format
 
 
 def generateSig(data: str):
     return base64.b64encode(
         bytes.fromhex("19") + hmac.new(bytes.fromhex("dfa5ed192dda6e88a12fe12130dc6206b1251e44"),
         data.encode(),
         hashlib.sha1).digest()
```

### Comparing `k-amino.py-1.0.8/k_amino/local.py` & `k-amino.py-1.1.0/k_amino/k_sync/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from base64 import b64encode
 from binascii import hexlify
 from time import time as timestamp
 from time import timezone as timezones
 from typing import Union, BinaryIO
 from uuid import UUID
 
-from .lib.objects import *
-from .lib.sessions import Session
+from ..lib.objects import *
+from ..lib.sessions import Session
 from .acm import Acm
 
 
 class SubClient(Acm, Session):
     def __init__(self, comId: str, proxies: dict = None, acm: bool = False):
         self.proxies = proxies
         self.comId = comId
```

### Comparing `k-amino.py-1.0.8/k_amino/sockets.py` & `k-amino.py-1.1.0/k_amino/k_sync/sockets.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import time as timer
 from sys import _getframe as getframe
 from typing import Union
 
 import ujson as json
 import websocket
 
-from .lib import *
-from .lib.objects import *
+from ..lib import *
+from ..lib.objects import *
 from .bot import Bot
 
 
 class Callbacks(Bot):
     def __init__(self, is_bot: bool = False, prefix: str = "!"):
         Bot.__init__(self, prefix=prefix)
 
@@ -129,15 +129,15 @@
     def setCall(self, name, data):
         self.call(name, Event(data["o"]).Event)
 
     def on_text_message(self, data):
         if self.is_bot:
             new_data = Event(data["o"]).Event
             new_data = self.build_parameters(new_data)
-            self.trigger(new_data)
+            self.trigger(new_data, str_only=True)
 
         self.setCall(getframe(0).f_code.co_name, data)
 
     def on_member_set_you_host(self, data): self.call(getframe(0).f_code.co_name, Payload(data["o"]).Payload)
     def on_member_remove_you_cohost(self, data): self.call(getframe(0).f_code.co_name, Payload(data["o"]).Payload)
     def on_member_set_you_cohost(self, data): self.call(getframe(0).f_code.co_name, Payload(data["o"]).Payload)
```

### Comparing `k-amino.py-1.0.8/k_amino.py.egg-info/PKG-INFO` & `k-amino.py-1.1.0/k_amino.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: k-amino.py
-Version: 1.0.8
+Version: 1.1.0
 Summary: Amino Bots with python!
 Home-page: https://github.com/kwel999/KAmino
 Download-URL: https://github.com/kwel999/KAmino/archive/refs/heads/main.zip
-Author: KWEL, ThePhoenix78
+Author: KWEL
 Author-email: itskwel999@gmail.com
 License: Apache
 Keywords: api,python,python3,python3.x,KWEL,kwel999,kwel.py,Amino,kamino,kamino pyK-Amino,kamino,kamino,kamino-bot,kamino-bots,kamino-bot,ndc,narvii.apps,aminoapps,kamino-py,kamino,kamino-bot,narvii
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## k_amino
```

### Comparing `k-amino.py-1.0.8/setup.py` & `k-amino.py-1.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     name="k-amino.py",
     version=__version__,
     url="https://github.com/kwel999/KAmino",
     download_url="https://github.com/kwel999/KAmino/archive/refs/heads/main.zip",
     description="Amino Bots with python!",
     long_description=README,
     long_description_content_type="text/markdown",
-    author="KWEL, ThePhoenix78",
+    author="KWEL",
     author_email="itskwel999@gmail.com",
     license="Apache",
     keywords=[
         "api",
         "python",
         "python3",
         "python3.x",
@@ -44,14 +44,14 @@
     include_package_data=True,
     install_requires=[
         "JSON_minify",
         "setuptools",
         "aiohttp",
         "websocket-client==1.3.1",
         "websockets",
-        "requests",
         "ujson",
-        "easy-events>=2.6.2"
+        "requests",
+        "easy-events==2.8.2"
     ],
     setup_requires=["wheel"],
     packages=find_packages(),
 )
```

