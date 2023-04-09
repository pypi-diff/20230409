# Comparing `tmp/fastapi_mvc_framework-1.1.2.tar.gz` & `tmp/fastapi_mvc_framework-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_mvc_framework-1.1.2.tar", last modified: Sat Apr  8 11:42:14 2023, max compression
+gzip compressed data, was "fastapi_mvc_framework-1.1.3.tar", last modified: Sun Apr  9 06:40:46 2023, max compression
```

## Comparing `fastapi_mvc_framework-1.1.2.tar` & `fastapi_mvc_framework-1.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 11:42:14.440612 fastapi_mvc_framework-1.1.2/
--rw-rw-rw-   0        0        0     4888 2023-04-08 11:42:14.438617 fastapi_mvc_framework-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3420 2023-04-08 11:41:32.000000 fastapi_mvc_framework-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-08 11:42:14.430637 fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/
--rw-rw-rw-   0        0        0      251 2023-04-06 06:00:47.000000 fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/__init__.py
--rw-rw-rw-   0        0        0      931 2023-04-07 07:39:59.000000 fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/_utils.py
--rw-rw-rw-   0        0        0     9964 2023-04-08 11:25:23.000000 fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/auth.py
--rw-rw-rw-   0        0        0     8826 2023-04-08 11:33:08.000000 fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/base_controller.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/cbv.py
--rw-rw-rw-   0        0        0     2996 2023-04-07 10:55:51.000000 fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/config.py
--rw-rw-rw-   0        0        0     3897 2023-04-06 12:09:13.000000 fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/controller.py
--rw-rw-rw-   0        0        0    12975 2023-04-08 09:48:48.000000 fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/controller_utils.py
--rw-rw-rw-   0        0        0    10474 2023-04-08 11:27:35.000000 fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/core.py
--rw-rw-rw-   0        0        0     5507 2023-04-07 11:35:06.000000 fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/midware_casbin.py
--rw-rw-rw-   0        0        0     9185 2023-04-08 05:46:03.000000 fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/midware_session.py
--rw-rw-rw-   0        0        0     1597 2023-04-06 04:58:51.000000 fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/view.py
-drwxrwxrwx   0        0        0        0 2023-04-08 11:42:14.437619 fastapi_mvc_framework-1.1.2/fastapi_mvc_framework.egg-info/
--rw-rw-rw-   0        0        0     4888 2023-04-08 11:42:14.000000 fastapi_mvc_framework-1.1.2/fastapi_mvc_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      648 2023-04-08 11:42:14.000000 fastapi_mvc_framework-1.1.2/fastapi_mvc_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 11:42:14.000000 fastapi_mvc_framework-1.1.2/fastapi_mvc_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-08 11:42:14.000000 fastapi_mvc_framework-1.1.2/fastapi_mvc_framework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-08 11:42:14.440612 fastapi_mvc_framework-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      721 2023-04-08 11:41:55.000000 fastapi_mvc_framework-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:40:46.442270 fastapi_mvc_framework-1.1.3/
+-rw-rw-rw-   0        0        0     6265 2023-04-09 06:40:46.441272 fastapi_mvc_framework-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4421 2023-04-09 06:40:13.000000 fastapi_mvc_framework-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-09 06:40:46.433295 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/
+-rw-rw-rw-   0        0        0      251 2023-04-06 06:00:47.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/__init__.py
+-rw-rw-rw-   0        0        0      931 2023-04-07 07:39:59.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/_utils.py
+-rw-rw-rw-   0        0        0     9943 2023-04-09 05:56:58.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/auth.py
+-rw-rw-rw-   0        0        0     8826 2023-04-08 11:33:08.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/base_controller.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/cbv.py
+-rw-rw-rw-   0        0        0     2996 2023-04-07 10:55:51.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/config.py
+-rw-rw-rw-   0        0        0     3733 2023-04-09 05:46:23.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/controller.py
+-rw-rw-rw-   0        0        0    12971 2023-04-09 05:48:57.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/controller_utils.py
+-rw-rw-rw-   0        0        0    10468 2023-04-09 05:50:46.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/core.py
+-rw-rw-rw-   0        0        0     5507 2023-04-07 11:35:06.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/midware_casbin.py
+-rw-rw-rw-   0        0        0     9185 2023-04-08 05:46:03.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/midware_session.py
+-rw-rw-rw-   0        0        0     1597 2023-04-06 04:58:51.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/view.py
+drwxrwxrwx   0        0        0        0 2023-04-09 06:40:46.440276 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework.egg-info/
+-rw-rw-rw-   0        0        0     6265 2023-04-09 06:40:46.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      648 2023-04-09 06:40:46.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 06:40:46.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-09 06:40:46.000000 fastapi_mvc_framework-1.1.3/fastapi_mvc_framework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-09 06:40:46.442270 fastapi_mvc_framework-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      721 2023-04-09 06:40:34.000000 fastapi_mvc_framework-1.1.3/setup.py
```

### Comparing `fastapi_mvc_framework-1.1.2/PKG-INFO` & `fastapi_mvc_framework-1.1.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,136 +1,169 @@
-Metadata-Version: 2.1
-Name: fastapi_mvc_framework
-Version: 1.1.2
-Summary: Simple and elegant use of FastApi in MVC mode
-Home-page: https://github.com/smjkzsl/fastapi_framework
-Author: Bruce chou
-Author-email: smjkzsl@gmail.com
-License: UNKNOWN
-Description: # fastapi_framework
-        A mvc framework used FastApi
-        Simple and elegant use of FastApi in MVC mode
-        
-        usage:
-        
-        
-        ```python
-        
-        from fastapi_mvc_framework import api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect
-        import requests,openai,json
-        from typing import Dict
-        from fastapi_mvc_framework import Form
+# fastapi_framework
+A mvc framework used FastApi
+Simple and elegant use of FastApi in MVC mode
+
+usage:
+
+
+```python
+
+from fastapi_mvc_framework import api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect
+import requests,openai,json
+from typing import Dict
+from fastapi_mvc_framework import Form
+ 
+application._public_auth_url = '/user/login'
+application._user_auth_url = '/user/login'
+
+@api_router(auth='public')
+class TestController(BaseController):
+    # _auth_url = '/user/login'
+    
+    @api.get("/user/login")
+    def login(self):
+        """:title Login""" 
+        
+        redirect = self.params['redirect'] if 'redirect' in self.params else '/'
+       
+        return self.view() 
+    @api.get("/user/logout")
+    def logout(self):
+        return self._user_logout()
+    
+    @api.post("/test/verity_user")
+    async def verity_user(self): 
+        form = self.params
+        username = form['username']
+        password = form['password']
+        redirect = form['redirect']
+        if username and password:
+            #do veritied
+            if username in ['bruce','alice'] and password:
+                return self._verity_successed(username,redirect)
+            else:
+                return self._verity_error() 
+        return self._verity_error()
+    
+    @api.get("/" )
+    def home(self,request:Request): 
+        '''
+        :title Home
+        '''
+        c = self.session.get('home',1)
+        c = c+1 
+        # #setting cookies   
+        # self.response.set_cookie('a',c) 
+        self.cookies["a"] = c
+        if c>10:
+            del self.cookies["a"]
+            c = 0
+        self.session['home'] = c
+        text = "Hello World! I'm in FastapiMvcFramework"
+        routers_map = application.routers_map
+        routers = application.routes
          
-        application._public_auth_url = '/user/login'
-        application._user_auth_url = '/user/login'
-        
-        @api_router(auth='public')
-        class TestController(BaseController):
-            # _auth_url = '/user/login'
-            
-            @api.get("/user/login")
-            def login(self):
-                """:title Login""" 
-                
-                redirect = self.params['redirect'] if 'redirect' in self.params else '/'
-               
-                return self.view() 
-            @api.get("/user/logout")
-            def logout(self):
-                return self._user_logout()
-            
-            @api.post("/test/verity_user")
-            async def verity_user(self): 
-                form = self.params
-                username = form['username']
-                password = form['password']
-                redirect = form['redirect']
-                if username and password:
-                    #do veritied
-                    if username in ['bruce','alice'] and password:
-                        return self._verity_successed(username,redirect)
-                    else:
-                        return self._verity_error() 
-                return self._verity_error()
-            
-            @api.get("/" )
-            def home(self,request:Request): 
-                '''
-                :title Home
-                '''
-                c = self.session.get('home',1)
-                c = c+1 
-                # #setting cookies   
-                # self.response.set_cookie('a',c) 
-                self.cookies["a"] = c
-                if c>10:
-                    del self.cookies["a"]
-                    c = 0
-                self.session['home'] = c
-                text = "Hello World! I'm in FastapiMvcFramework"
-                routers_map = application.routers_map
-                routers = application.routes
-                 
-                return self.view()
-            @api.get("/xml",auth='user')
-            def get_legacy_data(self):
-                """:title XML(Protected)"""
-        
-                data = """<?xml version="1.0"?>
-                <shampoo>
-                <Header>
-                    Apply shampoo here.
-                </Header>
-                <Body>
-                    You'll have to use soap here.
-                </Body>
-                </shampoo>
-                """
-                return self.view(content=data,media_type="application/xml")
-                 
-        
-             
-            @api.get("/chatgpt")
-            def chatgpt(self):
-                """
-                :title Chat
-                """
-                return self.view()
-        
-        
+        return self.view()
+    @api.get("/xml",auth='user')
+    def get_legacy_data(self):
+        """:title XML(Protected)"""
+
+        data = """<?xml version="1.0"?>
+        <shampoo>
+        <Header>
+            Apply shampoo here.
+        </Header>
+        <Body>
+            You'll have to use soap here.
+        </Body>
+        </shampoo>
+        """
+        return self.view(content=data,media_type="application/xml")
          
-        
-        ```
-        
-        home.html:
-        
-        ```html
-        <body>
-            <header>
-                <h1>My Website</h1>
-            </header>
-            <nav>
-                {% for item in routers_map %} {% if 'GET' in routers_map[item]['methods'] %}
-                <a href="{{routers_map[item]['path']}}">{{routers_map[item]['doc'] and routers_map[item]['doc']['title'] or item}}</a> {% endif %} {% endfor %}
-        
-                <a href="#">About</a>
-                <a href="#">Contact</a> {% if request.session['user'] %}
-                <a href="/user/logout"><b>{{request.session['user']['username']}}</b> Logout</a> {% endif %}
-            </nav>
-            <section>
-                <h2>Welcome to my website</h2>
-                <p>This is an example of a responsive design that works well on both desktop and mobile devices.</p>
-                <p>here is the `text` variable in class method:{{text}}</p>
-                <p style="color:red"><b>{{flash}}</b></p>
-            </section>
-            <footer>
-                <p>&copy; 2023 My Website</p>
-            </footer>
-        </body>
-        ```
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+
+     
+    @api.get("/chatgpt")
+    def chatgpt(self):
+        """
+        :title Chat
+        """
+        return self.view()
+
+
+ 
+
+```
+
+home.html:
+
+```html
+<body>
+    <header>
+        <h1>My Website</h1>
+    </header>
+    <nav>
+        {% for item in routers_map %} {% if 'GET' in routers_map[item]['methods'] %}
+        <a href="{{routers_map[item]['path']}}">{{routers_map[item]['doc'] and routers_map[item]['doc']['title'] or item}}</a> {% endif %} {% endfor %}
+
+        <a href="#">About</a>
+        <a href="#">Contact</a> {% if request.session['user'] %}
+        <a href="/user/logout"><b>{{request.session['user']['username']}}</b> Logout</a> {% endif %}
+    </nav>
+    <section>
+        <h2>Welcome to my website</h2>
+        <p>This is an example of a responsive design that works well on both desktop and mobile devices.</p>
+        <p>here is the `text` variable in class method:{{text}}</p>
+        <p style="color:red"><b>{{flash}}</b></p>
+    </section>
+    <footer>
+        <p>&copy; 2023 My Website</p>
+    </footer>
+</body>
+```
+
+your project directory structrue:
+```
++---app
+|   |   __init__.py
+|   |
+|   +---controllers
+|   |   |   test_controller.py
+|   |   |   __init__.py
+|   |   |
+|   +---views
+|   |   +---abc(controller name defined in app/controllers/test_controller.py)
+|   |   |   \---2.0
+|   |   |           css.css
+|   |   |           home.html
+|   |   |
+|   |   +---test 
+|   |   |       chatgpt.css
+|   |   |       chatgpt.html
+|   |   |       chatgpt.js
+|   |   |       home.html
+|   |   |       home.js
+|   |   |       login.html
+|   |   |
+|   |   \---ws 
+|   |           ws_home.html
+├─app1
+│  ├─controllers
+│  │  └─...
+│  ├─views
+│  │  ├─test1
+│  │  │  └─v1.0
+│  │  └─test2
++---configs
+|       cache.yaml
+|       casbin-adapter.csv
+|       casbin-model.conf
+|       database.yaml
+|       general.yaml
+|       session.yaml
++---public
+|       error_404.html
+|       error_500.html
+|       js.js
+└─sessions
+ 
+
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,13 +1,9 @@
-Metadata-Version: 2.1 Name: fastapi_mvc_framework Version: 1.1.2 Summary:
-Simple and elegant use of FastApi in MVC mode Home-page: https://github.com/
-smjkzsl/fastapi_framework Author: Bruce chou Author-email: smjkzsl@gmail.com
-License: UNKNOWN Description: # fastapi_framework A mvc framework used FastApi
-Simple and elegant use of FastApi in MVC mode usage: ```python from
-fastapi_mvc_framework import
+# fastapi_framework A mvc framework used FastApi Simple and elegant use of
+FastApi in MVC mode usage: ```python from fastapi_mvc_framework import
 api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect
 import requests,openai,json from typing import Dict from fastapi_mvc_framework
 import Form application._public_auth_url = '/user/login'
 application._user_auth_url = '/user/login' @api_router(auth='public') class
 TestController(BaseController): # _auth_url = '/user/login' @api.get("/user/
 login") def login(self): """:title Login""" redirect = self.params['redirect']
 if 'redirect' in self.params else '/' return self.view() @api.get("/user/
@@ -36,11 +32,17 @@
 ***** Welcome to my website *****
 This is an example of a responsive design that works well on both desktop and
 mobile devices.
 here is the `text` variable in class method:{{text}}
 {{flash}}
 
 © 2023 My Website
-``` Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
-markdown
+``` your project directory structrue: ``` +---app | | __init__.py | | | +---
+controllers | | | test_controller.py | | | __init__.py | | | | +---views | | +-
+--abc(controller name defined in app/controllers/test_controller.py) | | | \---
+2.0 | | | css.css | | | home.html | | | | | +---test | | | chatgpt.css | | |
+chatgpt.html | | | chatgpt.js | | | home.html | | | home.js | | | login.html |
+| | | | \---ws | | ws_home.html ââapp1 â ââcontrollers â â
+ââ... â ââviews â â ââtest1 â â â ââv1.0 â â
+ââtest2 +---configs | cache.yaml | casbin-adapter.csv | casbin-model.conf |
+database.yaml | general.yaml | session.yaml +---public | error_404.html |
+error_500.html | js.js ââsessions ```
```

### Comparing `fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/_utils.py` & `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/auth.py` & `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,28 +16,31 @@
 import jwt
 from datetime import datetime, timedelta
 from typing import Optional, Tuple, Union,Dict
 from ._utils import iJSONEncoder,is_datetime_format
 _session_name:str = ""
 class AuthenticationBackend_(AuthenticationBackend):
     def create_access_token(self,**kwargs):
-        raise NotImplementedError
+        raise NotImplementedError()
     def clear_userinfo(self,request:Request):
-        raise NotImplementedError
+        raise NotImplementedError()
     pass
 class CasbinAuth:
     def __init__(self,enforcer:Enforcer,session_name="user") -> None:
         global _session_name
         self.enforcer = enforcer
         self.__session_name = _session_name = session_name
         pass
     def _auth(self,request:Request,username:str):
         path = request.url.path
         method = request.method   
-        user = request.user.display_name if request.user.is_authenticated else 'anonymous'
+        if username:
+            user = username
+        else:
+            user = request.user.display_name if request.user.is_authenticated else 'anonymous'
 
         return self.enforcer.enforce(user, path, method)
     def __get_token_from_header(self, authorization: str, prefix: str) -> str:
         """Parses the Authorization header and returns only the token"""
         try:
             scheme, token = authorization.split()
         except ValueError as e:
@@ -87,27 +90,27 @@
         return "","",None
     
 class BasicAuth(AuthenticationBackend_):
     def __init__(self,**kwargs) -> None:
         super().__init__()
      
     
-    async def authenticate(self, request:Request,response,**kwargs):
+    async def authenticate(self, request:Request, **kwargs):
         username,password,_ = _casbin_auth.get_user_from_request(request=request)
         if not username:
             return False,None
         user = SimpleUser(username)
         request.scope['user'] = user
         auth_type:str = kwargs.get("auth_type")
         if not auth_type or auth_type.lower()=='public': 
             return True,  user
         result = _casbin_auth._auth(request=request,username=username)
         return result, user
 
-        return AuthCredentials(["authenticated"]), SimpleUser(username)
+         
     def clear_userinfo(self,request:Request):
         global _session_name
         del request.session[_session_name] 
         
     def create_access_token(self,  username,**kwargs):
         global _session_name
         request:Request = kwargs['request'] if 'request' in kwargs else None
@@ -144,15 +147,15 @@
         self.prefix = prefix
         self.username_field = username_field
         self.audience = audience
         self.options = options or dict()
     
      
     
-    async def authenticate(self, request,response,**kwargs) -> Union[None, Tuple[AuthCredentials, BaseUser]]:
+    async def authenticate(self, request,**kwargs) -> Union[None, Tuple[AuthCredentials, BaseUser]]:
         auth_type:str = kwargs.get("auth_type")
 
         args = {'username_field':self.username_field, 'key':self.secret_key, 'algorithms': self.algorithm , 'audience':self.audience ,
                                             'options':self.options }
         userobj,token,payload = _casbin_auth.get_user_from_request(request=request,
                                                                  prefix=self.prefix, 
                                                                  is_jwt=True,**args)
@@ -214,16 +217,16 @@
     cfg = config.get("auth")
     model_file = cfg.get("auth_model",'./configs/casbin-model.conf')    
     if not adapter:
         adapter_file = cfg.get("auth_adapter",'./configs/casbin-adapter.csv') 
         adapter = FileAdapter(adapter_file)   
     enforcer = casbin.Enforcer(model_file, adapter)
     _casbin_auth = CasbinAuth(enforcer=enforcer,session_name=__session_name)
-    authObj = backend(**kwagrs)
-    return authObj
+     
+    return backend(**kwagrs)
     app.add_middleware(CasbinMiddleware, enforcer=enforcer)
     app.add_middleware(AuthenticationMiddleware, backend=backend(**kwagrs))
 
 def reload_adapter(app:FastAPI,adapter:Adapter=None):
     cfg = config.get("auth")
     model_file = cfg.get("auth_model",'./configs/casbin-model.conf')    
     if not adapter:
```

### Comparing `fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/base_controller.py` & `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/base_controller.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/cbv.py` & `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/cbv.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/config.py` & `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/config.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/controller.py` & `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,19 +72,15 @@
     setattr(GeneratedController, TEMPLATE_PATH_KEY, template_path_prefix)
     setattr(GeneratedController, VER_KEY, version)
 
     return GeneratedController
 
 
 class controller:
-    @staticmethod
-    def login(path,*args,**kwargs):  
-        kwargs['__auth_url__']=path
-        return  _route_method(path,method='get',*args,**kwargs)
-         
+     
         
     """ """
     @staticmethod
     def http(path,methods=['GET'],*args,**kwargs):
         return _route_method(path,method=methods,*args,**kwargs)
     @staticmethod
     def get(path: str, *args, **kwargs):
```

### Comparing `fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/controller_utils.py` & `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/controller_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,15 +299,15 @@
         async def decorator(  *args, **kwargs):
             # 获取当前方法的名称
             # method_name = inspect.currentframe().f_code.co_name
             # # 获取当前方法的对象
             # method_obj = inspect.currentframe().f_back.f_locals.get(method_name)
             # print("当前方法名称为：", method_name)
             # print("当前方法对象为：", method_obj)
-            auth_type:str = getattr(func,'__auth__') 
+            auth_type:str = getattr(func,AUTH_KEY) 
             has_request = kwargs.get("__has_request__")
             has_response = kwargs.get("__has_response__")
             module = inspect.getmodule(func)
             cls = getattr(module, func.__qualname__.split('.<locals>', 1)[0].rsplit('.', 1)[0])
             
             #it's not instanced yet
             #instance = cls.__dict__.get('__wrapped__', None).__self__ #or cls.__dict__.get('__objclass__', None)(obj)
@@ -354,15 +354,15 @@
         setattr(decorator, ARGS_KEY, args)
         if '__auth_url__' in mwargs: 
             setattr(func,'__auth_url__',mwargs['__auth_url__'])
             del mwargs['__auth_url__']
 
         if not 'auth' in mwargs:
             mwargs["auth"] = 'public'
-        setattr(func,"__auth__",mwargs['auth'])
+        setattr(func,AUTH_KEY,mwargs['auth'])
         del mwargs['auth']
         setattr(decorator, KWARGS_KEY, mwargs)
         # setattr(decorator,'__doc__',getattr(func,'__doc__'))
         setattr(decorator, "__signature__", inspect.signature(func))
         return decorator
     return wrapper
```

### Comparing `fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/core.py` & `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
                      Response,
                      WebSocket,
                      WebSocketDisconnect, 
                      Cookie,
                      status as StateCodes)
  
 from .controller import create_controller,controller as api,   register_controllers_to_app 
-from .controller_utils import  TEMPLATE_PATH_KEY, VER_KEY,get_docs  
+from .controller_utils import  TEMPLATE_PATH_KEY,AUTH_KEY, VER_KEY,get_docs  
 from .config import config,ROOT_PATH,_log
 from fastapi.staticfiles import StaticFiles
 from fastapi.responses import RedirectResponse,JSONResponse,ORJSONResponse
 from . import midware
 from . import auth
 
 
@@ -52,16 +52,16 @@
     if not casbin_adapter:
         raise f"Not support {__type_casbin_adapter} ,Adapter config error in auth.casbin_adapter"
     
     auth_class = auth._auth_types[auth_type] if auth_type in auth._auth_types else None
     if not auth_class:
         raise f"{auth_type} auth type not support"
     __adapter_uri = config.get("auth").get("adapter_uri",'./configs/casbin-adapter.csv') 
-    __auth_key = config.get("auth").get(f"{auth_type}_key","")
-    kwargs = {'secret_key':__auth_key} 
+    secret_key = config.get("auth").get(f"{auth_type}_key","")
+    kwargs = {'secret_key':secret_key} 
     return auth.init(app=app, backend = auth_class,**kwargs)
 
 
 def api_router(path:str="", version:str="",**allargs):  
     '''
     :param path :special path format ,ex. '/{controller}/{version}'
     :param version :str like 'v1.0' ,'2.0'..
@@ -136,15 +136,15 @@
             @classmethod
             async def _auth__(cls,request:Request,response:Response,**kwargs):
                 '''called by .controller_util.py->route_method'''
                 if not hasattr(application,'authObj'):
                     return True,None
                 auth_type = kwargs['auth_type'] 
                 kwargs['session'] = request.session # cls._session
-                ret,user = await application.authObj.authenticate(request,response,**kwargs)
+                ret,user = await application.authObj.authenticate(request,**kwargs)
                 def add_redirect_param(url: str, redirect_url: str) -> str:
                     if "?" in url:
                         return url + "&redirect=" + redirect_url
                     else:
                         return url + "?redirect=" + redirect_url
                 accept_header = request.headers.get("Accept")
                 
@@ -162,15 +162,15 @@
                         _auth_url = add_redirect_param(_auth_url,str(request.url))
                         return RedirectResponse(_auth_url,status_code=StateCodes.HTTP_303_SEE_OTHER),None
                     else:  
                         return RedirectResponse('/',status_code=StateCodes.HTTP_303_SEE_OTHER),None
                 else:
                     return ret,user
 
-        setattr(puppetController,"__auth__",allargs['auth'])         
+        setattr(puppetController,AUTH_KEY,allargs['auth'])         
         setattr(puppetController,"__name__",targetController.__name__)  
         setattr(puppetController,"__controller_name__",targetController.__name__.lower().replace("controller",""))  
         
         setattr(puppetController,"__version__",version)  
         setattr(puppetController,"__location__",relative_path)  
         setattr(puppetController,"__appdir__",app_dir)  
 
@@ -204,15 +204,15 @@
     all_routers_map = {}
     for ctrl in __all_controller__:
         all_routers.append(register_controllers_to_app(__app, ctrl))
     for router in all_routers:
         for r in router.routes:
             funcname = str(r.endpoint).split('<function ')[1].split(" at ")[0] 
             end_point_abs = get_wrapped_endpoint(r.endpoint)
-            auth_type = getattr(end_point_abs,'__auth__') if hasattr(end_point_abs,'__auth__') else 'None'
+            auth_type = getattr(end_point_abs,AUTH_KEY) if hasattr(end_point_abs,AUTH_KEY) else 'None'
             doc_map =  get_docs(r.description) if hasattr(r,'description') else {}
             if hasattr(r,'methods'):
                 methods = r.methods
             else:
                 methods = r.name
             if isDebug:  
                 _log.debug('{:20}-->{:50}-->{}'.format(str(methods),r.path,funcname) )
```

### Comparing `fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/midware.py` & `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/midware.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/midware_casbin.py` & `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/midware_session.py` & `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/midware_session.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.2/fastapi_mvc_framework/view.py` & `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework/view.py`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.2/fastapi_mvc_framework.egg-info/PKG-INFO` & `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-mvc-framework
-Version: 1.1.2
+Version: 1.1.3
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/fastapi_framework
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: UNKNOWN
 Description: # fastapi_framework
         A mvc framework used FastApi
@@ -124,13 +124,60 @@
             </section>
             <footer>
                 <p>&copy; 2023 My Website</p>
             </footer>
         </body>
         ```
         
+        your project directory structrue:
+        ```
+        +---app
+        |   |   __init__.py
+        |   |
+        |   +---controllers
+        |   |   |   test_controller.py
+        |   |   |   __init__.py
+        |   |   |
+        |   +---views
+        |   |   +---abc(controller name defined in app/controllers/test_controller.py)
+        |   |   |   \---2.0
+        |   |   |           css.css
+        |   |   |           home.html
+        |   |   |
+        |   |   +---test 
+        |   |   |       chatgpt.css
+        |   |   |       chatgpt.html
+        |   |   |       chatgpt.js
+        |   |   |       home.html
+        |   |   |       home.js
+        |   |   |       login.html
+        |   |   |
+        |   |   \---ws 
+        |   |           ws_home.html
+        ├─app1
+        │  ├─controllers
+        │  │  └─...
+        │  ├─views
+        │  │  ├─test1
+        │  │  │  └─v1.0
+        │  │  └─test2
+        +---configs
+        |       cache.yaml
+        |       casbin-adapter.csv
+        |       casbin-model.conf
+        |       database.yaml
+        |       general.yaml
+        |       session.yaml
+        +---public
+        |       error_404.html
+        |       error_500.html
+        |       js.js
+        └─sessions
+         
+        
+        ```
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-mvc-framework Version: 1.1.2 Summary:
+Metadata-Version: 2.1 Name: fastapi-mvc-framework Version: 1.1.3 Summary:
 Simple and elegant use of FastApi in MVC mode Home-page: https://github.com/
 smjkzsl/fastapi_framework Author: Bruce chou Author-email: smjkzsl@gmail.com
 License: UNKNOWN Description: # fastapi_framework A mvc framework used FastApi
 Simple and elegant use of FastApi in MVC mode usage: ```python from
 fastapi_mvc_framework import
 api_router,api,Request,Response,BaseController,application,WebSocket,WebSocketDisconnect
 import requests,openai,json from typing import Dict from fastapi_mvc_framework
@@ -36,11 +36,20 @@
 ***** Welcome to my website *****
 This is an example of a responsive design that works well on both desktop and
 mobile devices.
 here is the `text` variable in class method:{{text}}
 {{flash}}
 
 © 2023 My Website
-``` Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
-markdown
+``` your project directory structrue: ``` +---app | | __init__.py | | | +---
+controllers | | | test_controller.py | | | __init__.py | | | | +---views | | +-
+--abc(controller name defined in app/controllers/test_controller.py) | | | \---
+2.0 | | | css.css | | | home.html | | | | | +---test | | | chatgpt.css | | |
+chatgpt.html | | | chatgpt.js | | | home.html | | | home.js | | | login.html |
+| | | | \---ws | | ws_home.html ââapp1 â ââcontrollers â â
+ââ... â ââviews â â ââtest1 â â â ââv1.0 â â
+ââtest2 +---configs | cache.yaml | casbin-adapter.csv | casbin-model.conf |
+database.yaml | general.yaml | session.yaml +---public | error_404.html |
+error_500.html | js.js ââsessions ``` Platform: UNKNOWN Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

### Comparing `fastapi_mvc_framework-1.1.2/fastapi_mvc_framework.egg-info/SOURCES.txt` & `fastapi_mvc_framework-1.1.3/fastapi_mvc_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi_mvc_framework-1.1.2/setup.py` & `fastapi_mvc_framework-1.1.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name='fastapi_mvc_framework',
-    version='1.1.2',
+    version='1.1.3',
     author='Bruce chou',
     author_email='smjkzsl@gmail.com',
     description='Simple and elegant use of FastApi in MVC mode',
     long_description=long_description,
     long_description_content_type="text/markdown",
     
     url='https://github.com/smjkzsl/fastapi_framework',
```

