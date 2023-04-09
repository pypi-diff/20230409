# Comparing `tmp/utran-1.0.2-py3-none-any.whl.zip` & `tmp/utran-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 32653 bytes, number of entries: 23
--rw-rw-rw-  2.0 fat      119 b- defN 23-Apr-08 13:11 utran/__init__.py
+Zip file size: 33949 bytes, number of entries: 23
+-rw-rw-rw-  2.0 fat      119 b- defN 23-Apr-09 15:51 utran/__init__.py
 -rw-rw-rw-  2.0 fat       56 b- defN 23-Mar-29 06:22 utran/__main__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-29 13:25 utran/application.py
 -rw-rw-rw-  2.0 fat     9798 b- defN 23-Apr-07 11:51 utran/handler.py
 -rw-rw-rw-  2.0 fat      540 b- defN 23-Apr-02 16:36 utran/log.py
 -rw-rw-rw-  2.0 fat    15004 b- defN 23-Apr-06 07:10 utran/object.py
 -rw-rw-rw-  2.0 fat    17630 b- defN 23-Apr-08 12:38 utran/register.py
 -rw-rw-rw-  2.0 fat     1318 b- defN 23-Apr-04 18:39 utran/runner.py
 -rw-rw-rw-  2.0 fat     5937 b- defN 23-Apr-05 16:38 utran/utils.py
 -rw-rw-rw-  2.0 fat       86 b- defN 23-Apr-04 18:45 utran/client/__init__.py
--rw-rw-rw-  2.0 fat    21867 b- defN 23-Apr-08 07:16 utran/client/baseclient.py
--rw-rw-rw-  2.0 fat     9244 b- defN 23-Apr-08 07:46 utran/client/client.py
+-rw-rw-rw-  2.0 fat    23021 b- defN 23-Apr-09 14:34 utran/client/baseclient.py
+-rw-rw-rw-  2.0 fat    13091 b- defN 23-Apr-09 15:44 utran/client/client.py
 -rw-rw-rw-  2.0 fat     1828 b- defN 23-Apr-06 17:14 utran/client/que.py
 -rw-rw-rw-  2.0 fat      163 b- defN 23-Mar-29 16:26 utran/server/__init__.py
 -rw-rw-rw-  2.0 fat     2668 b- defN 23-Apr-07 11:49 utran/server/baseServer.py
 -rw-rw-rw-  2.0 fat     4897 b- defN 23-Apr-07 11:49 utran/server/rpcServer.py
 -rw-rw-rw-  2.0 fat     5522 b- defN 23-Apr-05 17:27 utran/server/server.py
 -rw-rw-rw-  2.0 fat     5631 b- defN 23-Apr-07 11:48 utran/server/webserver.py
--rw-rw-rw-  2.0 fat     1062 b- defN 23-Apr-08 13:18 utran-1.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      403 b- defN 23-Apr-08 13:18 utran-1.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-08 13:18 utran-1.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-08 13:18 utran-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1749 b- defN 23-Apr-08 13:18 utran-1.0.2.dist-info/RECORD
-23 files, 105620 bytes uncompressed, 29873 bytes compressed:  71.7%
+-rw-rw-rw-  2.0 fat     1062 b- defN 23-Apr-09 15:53 utran-1.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      403 b- defN 23-Apr-09 15:53 utran-1.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-09 15:53 utran-1.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-09 15:53 utran-1.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1750 b- defN 23-Apr-09 15:53 utran-1.0.3.dist-info/RECORD
+23 files, 110622 bytes uncompressed, 31169 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -48,23 +48,23 @@
 
 Filename: utran/server/server.py
 Comment: 
 
 Filename: utran/server/webserver.py
 Comment: 
 
-Filename: utran-1.0.2.dist-info/LICENSE
+Filename: utran-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: utran-1.0.2.dist-info/METADATA
+Filename: utran-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: utran-1.0.2.dist-info/WHEEL
+Filename: utran-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: utran-1.0.2.dist-info/top_level.txt
+Filename: utran-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: utran-1.0.2.dist-info/RECORD
+Filename: utran-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## utran/__init__.py

```diff
@@ -1,5 +1,5 @@
 from utran.runner import run
 from utran.server import Server
 from utran.client import Client
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
```

## utran/client/baseclient.py

```diff
@@ -159,69 +159,91 @@
         self._reconnectNum:int = reconnectNum                           # 断线重连的次数
         self._serveHost:str = host                                      # 服务器host 
         self._servePort:int = port                                      # 服务器端口号
         self._reconnectingEvent:asyncio.Event = asyncio.Event()         # 用于等待重连
         self._reconnectingEvent.set()               # 默认关闭等待
         self._lastReconectTime:float = None                             # 最后一次重连时间
         self._main_task:asyncio.Task = None
-        self._main:callable = None
+        self._main:Union[Future,Coroutine,Callable] = None
         self._ignore = ignore                                           # 是否忽略远程调用异常
         self._isRuning = False                                          # 是否运行中
         self._curSendTask:asyncio.Task = None
 
-    async def start(self,main:Union[Future,asyncio.Task,Coroutine,Callable]=None,uri:str=None,host:str=None,port:int=None):
+    async def start(self,main:Union[Future,Coroutine,Callable]=None,uri:str=None,host:str=None,port:int=None,runforever:bool=False):
         """# 启动连接
         存在订阅的话题时，程序会一直等待话题的推送，无订阅话题时程序在执行完入口函数`main`后自动退出
-        Args:
-            uri: 服务器地址
-            main:入口函数，这是一个协程对象或Future对象
+        Args:            
+            main:入口函数，这是一个可等待对象，它可以是协程函数、协程对象或Future对象,
+            uri: 服务器地址 例：`utran://127.0.0.1:8081`
+            host: 不使用uri时可以直接指定服务器的host和port
+            port: 不使用uri时可以直接指定服务器的host和port
+            runforever: 是否一直运行,默认入口函数执行完毕且无任何订阅时会自动退出
         """
-        main = main or self._main
-        assert main,ValueError('No entry function or method was specified')
+        self._main = main or self._main
         self._serveHost = host or self._serveHost
         self._servePort = port or self._servePort
         if uri:
             self._serveHost,self._servePort = parse_utran_uri(uri)
         
         assert self._serveHost and self._servePort,ValueError('Specify the correct host and port.')
 
         self._reader, self._writer = await asyncio.open_connection(self._serveHost, self._servePort)
+        logger.debug(f"启动连接，{self._serveHost}:{self._servePort}")
         self._receive_task = asyncio.create_task(self.__receive())  
         self._heartbeatTimer = self._heartbeatTimer or HeartBeatTimer(self._ping,self._ping_timeout,self._heartbeatFreq,self._serverTimeout)
         self._exitEvent.clear()
 
         self._isRuning = True
-        if asyncio.iscoroutine(main):
-            # 同步单次调用模式
-            try:
-                result = await main
-            finally:
-                self._receive_task.cancel()
-                self._isRuning = False
-                await self._close()            
-            return result
 
-        elif asyncio.iscoroutinefunction(main):
-            # 异步服务模式
-            self._main_task = asyncio.create_task(main())
-            try:
-                await self._main_task
-                if self._topics_handler: logger.info('主函数执行完毕,持续等待订阅推送..')
-                if not self._topics_handler:
-                    await self.exit()
+        result = None
+        try:
+            if self._main:
+                if asyncio.iscoroutine(self._main) or asyncio.isfuture(self._main):
+                    # 同步单次调用模式
+                    self._main_task = asyncio.create_task(main)
+                    result = await self._main_task
+                elif asyncio.iscoroutinefunction(self._main):
+                    # 异步服务模式
+                    self._main_task = asyncio.create_task(self._main())
+                    result = await self._main_task
                 else:
+                    raise ValueError(f'The "{type(self._main)}" cannot be an entry object ,must be coroutinefunction,Coroutine or Future')        
+                logger.debug('主函数执行完毕.')
+
+            if runforever:
+                # __enter__进入
+                await self._exitEvent.wait()
+            else:
+                if self._topics_handler:
+                    logger.debug('持续等待订阅推送..')
                     self._heartbeatTimer.alive()
-                    await self._exitEvent.wait()                
-            finally:
-                await self.exit()
-        else:
+                    await self._exitEvent.wait()
+                else:
+                    logger.debug('无订阅,程序即将退出')
+
+        finally:
             await self.exit()
-            raise ValueError(f'The entry object "main" must be coroutinefunction,Coroutine or Future,Task')
+            return result
+    
 
+    def hasSubscribe(self,returnTopics:bool=True)->Union[tuple,bool]:
+        """# 是否有订阅话题
+        Args:
+            returnTopics: 是否返回已订阅的话题
         
+        Returns:
+            当returnTopics为True时返回值为tuple，否则返回 bool值            
+        """
+        if returnTopics:
+            return tuple(self._topics_handler.keys())
+        if self._topics_handler:
+            return True
+        else:
+            return False
+
 
     def __call__(self, *args: any, **opts: any) -> callable:
         """# 指定入口函数，可以使用装饰器方式指定入口函数
         opts 选项参数暂时未设置功能，待开发..
         """
         if len(args)==0:
             return partial(self.__call__,**opts)
@@ -234,16 +256,14 @@
     async def _ping(self):
         """向服务器发送ping"""
         try:
             await self._send(None,heartbeat=True)
         except ConnectionResetError as e:
             logger.error('发送PING时服务器错误，'+str(e))
 
-            
-
 
     async def _ping_timeout(self):
         """服务器响应超时，该方法会被执行"""
         logger.error("服务器响应超时，启动断线重连..")
         self._reconnectTask = asyncio.create_task(self._reconnecting())
 
 
@@ -251,16 +271,15 @@
         """断线重连"""
         n = self._reconnectNum
         logger.error(f"开始尝试重连,将在{self._reconnectNum}次后停止...")
         self._reconnectingEvent.clear()
         while n>0:
             if n<=12:logger.error(f"剩余{n}次重连..")
             await self._close()
-            try:
-                self._receive_task.cancel()
+            try:                
                 self._reader, self._writer = await asyncio.open_connection(self._serveHost, self._servePort)
                 logger.success(f"重连成功")
                 self._lastReconectTime = time.time()
                 if self._curSendTask and not self._curSendTask.done():
                     self._curSendTask.cancel()
                     self._curSendTask = None
 
@@ -342,21 +361,24 @@
         Returns:
             {'allTopics': ['topic1'], 'unSubTopics': ['topic2']}   
 
         |allTopics|unSubTopics|
         |---------|-----------|
         |所有已订阅的话题 `list`|本次取消订阅的话题 `list`|
         """
-        [self._topics_handler.pop(t) for t in topic if t in self._topics_handler]              
-
+        if topic:
+            [self._topics_handler.pop(t) for t in topic if t in self._topics_handler]              
 
         msg = dict(requestType=UtType.UNSUBSCRIBE.value,topics=topic)
         request:UtRequest = create_UtRequest(msg)
         res = await self._send(request,timeout=timeout,ignore=ignore)
-        if not self._topics_handler:logger.warning('已无任何订阅.')
+        if not self._topics_handler:
+            logger.debug('已无任何订阅,程序即将退出..')
+            self._exitEvent.set()
+
         return res
         
 
     async def call(self,
                    methodName:str,
                    args:list=tuple(),
                    dicts:dict=dict(),
@@ -498,29 +520,30 @@
             await callback(msg,topic)                
         else:
             callback(msg,topic)
 
 
     async def _close(self):
         """# 关闭连接"""
+        self._receive_task.cancel()
+        self._heartbeatTimer.stop()
+
         if self._writer is not None:
             try:            
                 self._writer.write(b'')
                 await self._writer.drain()
             except ConnectionResetError as e:
                 pass
             self._writer.close()
 
-        self._heartbeatTimer.stop()
         self._reader = None
         self._writer = None
 
+
     async def exit(self):
         """# 退出程序
         调用退出时，并不会立即退出，需要等run方法中指定的`main`入口函数执行完毕才会退出。
         """
-        self._topics_handler = None
-        self._receive_task.cancel()
         self._isRuning = False
+        self._topics_handler = None        
         await self._close()
         self._exitEvent.set()
-
```

## utran/client/client.py

```diff
@@ -1,12 +1,16 @@
 import asyncio
+from asyncio import Future
 from functools import partial
-from typing import Coroutine, Union
+import threading
+import time
+from typing import Callable, Coroutine, Union
 from utran.client.baseclient import BaseClient
 from utran.utils import parse_utran_uri
+import inspect
 
 class ExeProxy:
     """远程执行代理"""
     __slots__ = ('_accessProxy_',)
     def __init__(self,accessProxy:'AccessProxy'):
         self._accessProxy_ = accessProxy
 
@@ -19,53 +23,58 @@
         """# 执行远程函数
 
         Returns:
             返回值 (dict): 当选项标记为multicall时: `client.call(multicall=True).add(1,2)`         
             返回值 (asyncio.Task): 当baseclient已经运行时，`client.call.add(1,2)` 返回Task。可使用await拿到调用结果，例: `await client.call.add(1,2)`
             返回值 (any): 当baseclient未运行时，`client.call.add(1,2)`返回最终的调用结果
         """
-        f:Union[Coroutine,dict] = self._accessProxy_._bsclient_.call(methodName=self._accessProxy_._temp_name_,args=args,dicts=dicts,**self._accessProxy_._temp_opts_)
-        if self._accessProxy_._bsclient_._isRuning:
+        f:Union[Coroutine,dict] = self._accessProxy_._client_._bsclient.call(methodName=self._accessProxy_._temp_name_,args=args,dicts=dicts,**self._accessProxy_._temp_opts_)
+        
+        if self._accessProxy_._client_._enterLoop:
+            # self._accessProxy_._client_._enterLoop.run_until_complete
+            futrue = asyncio.run_coroutine_threadsafe(f,self._accessProxy_._client_._enterLoop)
+            return futrue.result()
+
+        if self._accessProxy_._client_._bsclient._isRuning:
             # f is coroutine
             return asyncio.create_task(f)
         else: 
             if self._accessProxy_._temp_opts_.get('multicall'):
                 # f is dict
                 return f
             else:
                 # f is coroutine
                 loop = asyncio.get_event_loop()
-                res = loop.run_until_complete(self._accessProxy_._bsclient_.start(main=f))
+                res = loop.run_until_complete(self._accessProxy_._client_._bsclient.start(main=f))
                 return res
 
-
 class AccessProxy:
     """访问代理"""
-    __slots__ = ('_temp_opts_','_temp_name_','_bsclient_','_exeProxy_')
-    def __init__(self,bsclient:BaseClient):
+    __slots__ = ('_temp_opts_','_temp_name_','_client_','_exeProxy_')
+    def __init__(self,client:'Client'):
         self._temp_opts_ = dict()
         self._temp_name_:str = ''
-        self._bsclient_ = bsclient
+        self._client_ = client
         self._exeProxy_ = ExeProxy(self)
 
     def __getattr__(self, methodName):
         self._temp_name_ = methodName
         return self._exeProxy_
 
     def __call__(self,*,timeout:int=None,encrypt:bool=None, ignore:bool=None,multicall:bool=False):
         """# 设置调用选项
         Args:
             timeout: 本地等待响应超时，抛出TimeoutError错误（单位：秒） ，默认为为client实例化的值
             encrypt: 是否加密， 默认为为client实例化的值
             ignore: 是否忽略远程执行结果的错误，忽略错误则值用None填充，默认为为client实例化的值
             multicall: 是否标记为合并调用
         """
-        self._temp_opts_ = dict(timeout= self._bsclient_._localTimeout if timeout==None else timeout,
-                          encrypt= self._bsclient_._encrypt if timeout==None else encrypt,
-                          ignore = self._bsclient_._ignore if ignore==None else ignore,
+        self._temp_opts_ = dict(timeout= self._client_._localTimeout if timeout==None else timeout,
+                          encrypt= self._client_._encrypt if timeout==None else encrypt,
+                          ignore = self._client_._ignore if ignore==None else ignore,
                           multicall = multicall)
         return self
 
 
 class Client:
     """# 客户端
     支持代理调用
@@ -73,15 +82,15 @@
         heartbeatFreq: 心跳频率
         serverTimeout: 服务器心跳响应超时时间，用于判断是否断线，超过此值会进行重连 (单位:秒)
         localTimeout: 本地调用超时 (单位:秒)
         reconnectNum: 断线重连的次数
         ignore: 是否忽略远程调用异常
         encrypt: 是否加密传输
     """
-    __slots__ = ('_localTimeout','_ignore','_encrypt','_heartbeatFreq','_serverTimeout','_reconnectNum','_bsclient','_proxy','_serveHost','_servePort')
+    __slots__ = ('_localTimeout','_ignore','_encrypt','_heartbeatFreq','_serverTimeout','_reconnectNum','_bsclient','_proxy','_serveHost','_servePort','_enterLoop','_thread')
     def __init__(self,
                  *,
                  host:str=None,
                  port:int=None,
                  uri:str = None,
                  heartbeatFreq:int=2,
                  serverTimeout:int=2,
@@ -97,66 +106,131 @@
         self._serverTimeout:int = serverTimeout                         # 服务器响应超时时间 （单位：秒）
         self._reconnectNum:int = reconnectNum                           # 断线重连的次数
 
         self._serveHost:str = host                                      # 服务器host 
         self._servePort:int = port                                      # 服务器端口号
         self._bsclient:BaseClient = None
 
+        self._enterLoop:asyncio.AbstractEventLoop = None                # 使用__enter__时创建的loop
+
         if uri:
             self._serveHost,self._servePort = parse_utran_uri(uri)
 
-        
 
-    def __call__(self, *args: any,**opts: any) -> callable:
-        """指定入口函数，可以使用装饰器方式指定入口函数"""
-        self._bsclient:BaseClient = self._bsclient or BaseClient(heartbeatFreq=self._heartbeatFreq,
-                                                                serverTimeout=self._serverTimeout,
-                                                                reconnectNum=self._reconnectNum,
-                                                                encrypt=self._encrypt,
-                                                                host=self._serveHost,
-                                                                port=self._servePort)
+        self._bsclient:BaseClient = BaseClient(heartbeatFreq=self._heartbeatFreq,
+                                                serverTimeout=self._serverTimeout,
+                                                reconnectNum=self._reconnectNum,
+                                                encrypt=self._encrypt,
+                                                host=self._serveHost,
+                                                port=self._servePort)
+        self._proxy = AccessProxy(self)
 
-        return self._bsclient(*args,**opts)
-    
 
-    async def start(self,main:Union[asyncio.Future,Coroutine]=None,uri:str=None,host:str=None,port:int=None):
+    def __call__(self, *args: any,**opts: any) -> callable:
+        """指定入口函数，可以使用装饰器方式指定入口函数"""
+        if len(args)==0:
+            return partial(self.__call__,**opts)
+        
+        if inspect.iscoroutinefunction(args[0]):
+            asyncio.run(self._bsclient.start(main=args[0](),host=self._serveHost,port=self._servePort))
+  
+        elif inspect.isfunction(args[0]) or inspect.ismethod(args[0]):
+            self.__enter__()
+            try:
+                args[0]()
+            finally:
+                while True:
+                    if not self._bsclient._isRuning:
+                        break
+                    if not self._bsclient.hasSubscribe(returnTopics=False):
+                        _ = asyncio.run_coroutine_threadsafe(self._bsclient.exit(),self._enterLoop)
+                        _.result()
+                        break
+                    time.sleep(1)
+
+                self.__exit__(None,None,None)
+
+
+    async def start(self,main:Union[Future,Coroutine,Callable]=None,uri:str=None,host:str=None,port:int=None,runforever:bool=False):
+        """# 启动连接
+        存在订阅的话题时，程序会一直等待话题的推送，无订阅话题时程序在执行完入口函数`main`后自动退出
+        Args:            
+            main:入口函数，它是一个可等待对象，可以是协程函数、协程对象或Future对象。为指定时默认为
+            uri: 服务器地址 例：`utran://127.0.0.1:8081`
+            host: 不使用uri时可以直接指定服务器的host和port
+            port: 不使用uri时可以直接指定服务器的host和port
+            runforever: 是否一直运行,默认入口函数执行完毕且无任何订阅时会自动退出
+        """
         host = host or self._serveHost
         port = port or self._servePort
-                # 基础客户端
-        self._bsclient:BaseClient = self._bsclient or BaseClient(heartbeatFreq=self._heartbeatFreq,
-                                                                serverTimeout=self._serverTimeout,
-                                                                reconnectNum=self._reconnectNum,
-                                                                encrypt=self._encrypt,
-                                                                host=self._serveHost,
-                                                                port=self._servePort)
-
-        self._proxy = AccessProxy(self._bsclient)
-        await self._bsclient.start(main=main,uri=uri,host=host,port=port)
+        # 基础客户端
+        
+        await self._bsclient.start(main=main,uri=uri,host=host,port=port,runforever=runforever)
 
 
-    @property
-    def subscribe(self)->BaseClient.subscribe:
-        """订阅
-        异步方法
+    def subscribe(self,
+                topic:Union[str,tuple[str]],
+                callback:callable,
+                *,
+                timeout:int=None,
+                ignore:bool=None)->Union[Coroutine,dict]:
+        """# 订阅话题
+        支持同步和异步的调用，
+        存在订阅的话题时，程序会一直等待话题的推送，无订阅话题时程序在执行完入口函数`main`后自动退出
+        
+        Args:
+            topic: 话题
+            callback: 回调函数，有两个参数 msg,topic。支持异步和同步回调函数, 
+            timeout: 本地等待响应超时，抛出TimeoutError错误（单位：秒）
+            ignore: 是否忽略远程执行结果的错误，忽略错误则值用None填充
+        
         Returns:
-            返回订阅方法
+            {'allTopics': ['topic1','topic2'], 'subTopics': ['topic2']}
+        
+        |allTopics|subTopics|
+        |---------|-----------|
+        |所有已订阅的话题 `list`|本次订阅的话题 `list`|
         """
-        return self._bsclient.subscribe
+        coro = self._bsclient.subscribe(topic=topic,callback=callback,timeout=timeout,ignore=ignore)
+        if self._enterLoop:
+            futrue = asyncio.run_coroutine_threadsafe(coro,self._enterLoop)
+            return futrue.result()
+
+        else:
+            return coro
     
 
-    @property
-    def unsubscribe(self)->BaseClient.unsubscribe:
-        """订阅
-        异步方法
+    def unsubscribe(self,
+                    *topic:str,
+                    timeout:int=None,
+                    ignore:bool=None)->Union[Coroutine,dict]:
+        """# 取消订阅话题
+        支持同步和异步的调用，
+        存在订阅的话题时，程序会一直等待话题的推送，无订阅话题时程序在执行完入口函数`main`后自动退出
+        Args:
+            topic: 话题
+            timeout: 本地等待响应超时，抛出TimeoutError错误（单位：秒）
+            ignore: 是否忽略远程执行结果的错误，忽略错误则值用None填充
+
         Returns:
-            返回取消订阅方法
+            {'allTopics': ['topic1'], 'unSubTopics': ['topic2']}   
+
+        |allTopics|unSubTopics|
+        |---------|-----------|
+        |所有已订阅的话题 `list`|本次取消订阅的话题 `list`|
         """
-        return self._bsclient.unsubscribe
+        coro = self._bsclient.unsubscribe(*topic,timeout=timeout,ignore=ignore)
+        if self._enterLoop:
+            futrue = asyncio.run_coroutine_threadsafe(coro,self._enterLoop)
+            return futrue.result()
+        else:
+            return coro
     
 
+
     def multicall(self,*calls:Coroutine,encrypt:bool = False,timeout:int=None,ignore:bool=None)->list:
         """# 合并多次调用远程方法或函数
         支持同步和异步的调用，
                 同步调用方式会：1自动建立连接 -- 2任务执行完毕 --3自动关闭连接，适用于未建立连接时使用。
                 异步调用方式会：1使用现有的连接-- 2任务执行完毕。适用于已建立连接时。
         Args:
             *calls: 需要远程调用协程对象
@@ -171,28 +245,59 @@
         if self._bsclient._isRuning:
             return f
         else:
             _loop = asyncio.get_event_loop()
             return _loop.run_until_complete(self._bsclient.start(main=f))
 
 
+    def exit(self):
+        """# 退出程序
+        支持同步和异步的调用，
+        """
+        coro = self._bsclient.exit()
+        if self._enterLoop:
+            futrue = asyncio.run_coroutine_threadsafe(coro,self._enterLoop)
+            return futrue.result()
+        else:
+            return coro
+        
+
     @property
     def call(self)->AccessProxy:
         """远程调用
         支持同步和异步的调用，
                 同步调用方式会：1自动建立连接 -- 2任务执行完毕 --3自动关闭连接，适用于未建立连接时使用。
                 异步调用方式会：1使用现有的连接-- 2任务执行完毕。适用于已建立连接时。
 
         Returns:
             返回远程调用的代理类
         """
-        if self._bsclient is None or  not self._bsclient._isRuning:
-            self._bsclient:BaseClient = BaseClient(heartbeatFreq=self._heartbeatFreq,
-                                                    serverTimeout=self._serverTimeout,
-                                                    reconnectNum=self._reconnectNum,
-                                                    encrypt=self._encrypt,
-                                                    host=self._serveHost,
-                                                    port=self._servePort)
-            self._proxy = AccessProxy(self._bsclient)
-
+        
         return self._proxy
-        
+    
+
+    def __enter__(self):        
+        self._enterLoop = asyncio.new_event_loop()
+        def worker(loop:asyncio.AbstractEventLoop):
+            loop.run_until_complete(self._bsclient.start(runforever=True))
+
+        self._thread = threading.Thread(target=worker, args=(self._enterLoop,))
+        self._thread.start()
+
+        while True:
+            if self._bsclient._isRuning:
+                break
+            time.sleep(0.1)
+        return self
+    
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        try:
+            if exc_type:
+                raise exc_type(exc_value)
+        finally:
+            self._thread.join()
+            self._enterLoop.close()
+            self._enterLoop = None
+
+
+
```

## Comparing `utran-1.0.2.dist-info/LICENSE` & `utran-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `utran-1.0.2.dist-info/RECORD` & `utran-1.0.3.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-utran/__init__.py,sha256=62nxXSq83ooYcZp92ZWA7HHgxlpp6P_dP4ojqQ1vmzM,119
+utran/__init__.py,sha256=IIerGgJq-dAT_yDcqzA-EaoGgeRE1Fply3RErD174u8,119
 utran/__main__.py,sha256=iJDh2-BPQSCB63Vdx_oTisjzUZHGfG1yGBz2T-EUusY,56
 utran/application.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 utran/handler.py,sha256=ua0pmYJhZeCtJ-uZYvHQGOwwyVFbwkWkjTaQHxphE7c,9798
 utran/log.py,sha256=yV3OegWgMX4rzzJcBnBzvX5sqh4WFgFDKFTvNUAzPzo,540
 utran/object.py,sha256=_DfgGmDnm5vwPapevBX5pwExQapoccLV-ABQTgOiwhM,15004
 utran/register.py,sha256=ltbef-Xj3taLr__6CUAt7af3AXVPjr5U_OQ-Xwd3xMw,17630
 utran/runner.py,sha256=MRyK9lwkcGCgQSJhZtcm7scvrPhry1jiNyDDSxNKiN0,1318
 utran/utils.py,sha256=hfcFvn2Yl0uwn1w8wnFe7FjCqkJxFsCZnngyiu8OMWM,5937
 utran/client/__init__.py,sha256=Kav3KmWiPhdMDjV7poRDaAM_XxBqbngvrH9nVaQd5fk,86
-utran/client/baseclient.py,sha256=QjFfaAF1DFMVmljNCb01veM6eA79v7NHjV92-CHT0IY,21867
-utran/client/client.py,sha256=qZf7TpEVMqum7hSJsfRwuZdQNQprFfjtsVXliufg3mg,9244
+utran/client/baseclient.py,sha256=pEo23TMAk1TwirbjB3zTdkiKDDPpoCJ9TJvc6r4BvdI,23021
+utran/client/client.py,sha256=pcryOVwmJb76WvHHkri_2oC493oZOU0UagJ5py4krN4,13091
 utran/client/que.py,sha256=cgUmJ3Pz_1j3B0LnC4gx8PGqLC__c4f20qQuQXuLt0A,1828
 utran/server/__init__.py,sha256=S-DRV8KWrwO_4yM3vJWEkDfcJCyjwSlSHaDDk8UGl_Q,163
 utran/server/baseServer.py,sha256=URBy6NkEnXotpgI9atdcuhPecC9EasYjJQ7hLcokYu0,2668
 utran/server/rpcServer.py,sha256=rc9ht889j3nSrBh5A0zqBalVsjdcO9957gWCI0biwNE,4897
 utran/server/server.py,sha256=HQgDNLcvM2fvzMGI_it2z5MKyAU0kzE1WfPf9iOl-Y8,5522
 utran/server/webserver.py,sha256=0xMQ65cyKJxlOkYNk2N-NtwKE7VDObU4n2MRHw4PFb8,5631
-utran-1.0.2.dist-info/LICENSE,sha256=7HB3vUUZ3KdogFm8d92SgQCXP7uuE2kNYWGajh3eo4Y,1062
-utran-1.0.2.dist-info/METADATA,sha256=5P427XV2gl0HbRJ7lrpJzNaSjopWqnvT8KnZp4u__Fg,403
-utran-1.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-utran-1.0.2.dist-info/top_level.txt,sha256=kcB7HqGkubiQlKanIo6oNBlCUQJOy5zc_HSvHiaoOA8,6
-utran-1.0.2.dist-info/RECORD,,
+utran-1.0.3.dist-info/LICENSE,sha256=7HB3vUUZ3KdogFm8d92SgQCXP7uuE2kNYWGajh3eo4Y,1062
+utran-1.0.3.dist-info/METADATA,sha256=THzhKMKbk9aHfzHbrOx6Or4u2tKc2RT_UKLbdDWHaow,403
+utran-1.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+utran-1.0.3.dist-info/top_level.txt,sha256=kcB7HqGkubiQlKanIo6oNBlCUQJOy5zc_HSvHiaoOA8,6
+utran-1.0.3.dist-info/RECORD,,
```

