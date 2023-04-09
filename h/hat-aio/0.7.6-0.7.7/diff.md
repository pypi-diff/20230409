# Comparing `tmp/hat_aio-0.7.6-cp38.cp39.cp310.cp311-none-any.whl.zip` & `tmp/hat_aio-0.7.7-cp38.cp39.cp310.cp311-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 14712 bytes, number of entries: 12
+Zip file size: 14779 bytes, number of entries: 12
 -rw-r--r--  2.0 unx     1225 b- defN 23-Mar-23 19:16 hat/aio/__init__.py
 -rw-r--r--  2.0 unx     2761 b- defN 23-Mar-23 19:15 hat/aio/executor.py
--rw-r--r--  2.0 unx     6776 b- defN 23-Mar-23 19:09 hat/aio/group.py
--rw-r--r--  2.0 unx     9130 b- defN 23-Mar-23 14:48 hat/aio/misc.py
--rw-r--r--  2.0 unx     6230 b- defN 23-Mar-23 14:45 hat/aio/queue.py
--rw-r--r--  2.0 unx     1780 b- defN 23-Mar-23 14:50 hat/aio/wait.py
--rw-r--r--  2.0 unx    11358 b- defN 23-Mar-23 19:22 hat_aio-0.7.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     1794 b- defN 23-Mar-23 19:22 hat_aio-0.7.6.dist-info/METADATA
--rw-r--r--  2.0 unx      152 b- defN 23-Mar-23 19:22 hat_aio-0.7.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Mar-23 19:22 hat_aio-0.7.6.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-23 19:22 hat_aio-0.7.6.dist-info/zip-safe
--rw-rw-r--  2.0 unx      915 b- defN 23-Mar-23 19:22 hat_aio-0.7.6.dist-info/RECORD
-12 files, 42126 bytes uncompressed, 13196 bytes compressed:  68.7%
+-rw-r--r--  2.0 unx     6903 b- defN 23-Apr-09 18:24 hat/aio/group.py
+-rw-r--r--  2.0 unx     9360 b- defN 23-Apr-09 18:39 hat/aio/misc.py
+-rw-r--r--  2.0 unx     6172 b- defN 23-Apr-09 19:06 hat/aio/queue.py
+-rw-r--r--  2.0 unx     1836 b- defN 23-Apr-09 18:48 hat/aio/wait.py
+-rw-r--r--  2.0 unx    11358 b- defN 23-Apr-09 19:09 hat_aio-0.7.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1794 b- defN 23-Apr-09 19:09 hat_aio-0.7.7.dist-info/METADATA
+-rw-r--r--  2.0 unx      152 b- defN 23-Apr-09 19:09 hat_aio-0.7.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Apr-09 19:09 hat_aio-0.7.7.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-09 19:09 hat_aio-0.7.7.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      915 b- defN 23-Apr-09 19:09 hat_aio-0.7.7.dist-info/RECORD
+12 files, 42481 bytes uncompressed, 13263 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: hat/aio/queue.py
 Comment: 
 
 Filename: hat/aio/wait.py
 Comment: 
 
-Filename: hat_aio-0.7.6.dist-info/LICENSE
+Filename: hat_aio-0.7.7.dist-info/LICENSE
 Comment: 
 
-Filename: hat_aio-0.7.6.dist-info/METADATA
+Filename: hat_aio-0.7.7.dist-info/METADATA
 Comment: 
 
-Filename: hat_aio-0.7.6.dist-info/WHEEL
+Filename: hat_aio-0.7.7.dist-info/WHEEL
 Comment: 
 
-Filename: hat_aio-0.7.6.dist-info/top_level.txt
+Filename: hat_aio-0.7.7.dist-info/top_level.txt
 Comment: 
 
-Filename: hat_aio-0.7.6.dist-info/zip-safe
+Filename: hat_aio-0.7.7.dist-info/zip-safe
 Comment: 
 
-Filename: hat_aio-0.7.6.dist-info/RECORD
+Filename: hat_aio-0.7.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hat/aio/group.py

```diff
@@ -51,14 +51,18 @@
         self.async_group.close()
 
     async def async_close(self):
         """Close resource and wait until closed is ``True``."""
         await self.async_group.async_close()
 
 
+class GroupClosedError(Exception):
+    """Group closed exception"""
+
+
 class Group(Resource):
     """Group of asyncio Tasks.
 
     Group enables creation and management of related asyncio Tasks. The
     Group ensures uninterrupted execution of Tasks and Task completion upon
     Group closing.
 
@@ -74,17 +78,16 @@
 
     def __init__(self,
                  log_exceptions: bool = True,
                  *,
                  loop: typing.Optional[asyncio.AbstractEventLoop] = None):
         self._log_exceptions = log_exceptions
         self._loop = loop or asyncio.get_running_loop()
-        self._closing = asyncio.Future(loop=loop)
-        self._closed = asyncio.Future(loop=loop)
-        self._canceled = False
+        self._closing = self._loop.create_future()
+        self._closed = self._loop.create_future()
         self._tasks = set()
         self._parent = None
         self._children = set()
 
     @property
     def async_group(self):
         """Async group"""
@@ -122,40 +125,46 @@
         Closing of a subgroup has no effect on the parent Group.
 
         If `log_exceptions` is ``None``, subgroup inherits `log_exceptions`
         from its parent.
 
         """
         if self._closing.done():
-            raise Exception('group not open')
+            raise GroupClosedError("can't create subgroup of closed group")
 
         child = Group(
             log_exceptions=(self._log_exceptions if log_exceptions is None
                             else log_exceptions),
             loop=self._loop)
         child._parent = self
         self._children.add(child)
         return child
 
     def wrap(self,
-             future: asyncio.Future
+             obj: typing.Awaitable
              ) -> asyncio.Task:
-        """Wrap the Future into a Task and schedule its execution. Return the
-        Task object.
+        """Wrap the awaitable object into a Task and schedule its execution.
+        Return the Task object.
 
         Resulting task is shielded and can be canceled only with
         `Group.async_close`.
 
         """
         if self._closing.done():
-            raise Exception('group not open')
+            raise GroupClosedError("can't wrap object in closed group")
+
+        if asyncio.iscoroutine(obj):
+            task = self._loop.create_task(obj)
+
+        else:
+            task = asyncio.ensure_future(obj, loop=self._loop)
 
-        task = asyncio.ensure_future(future, loop=self._loop)
         self._tasks.add(task)
         task.add_done_callback(self._on_task_done)
+
         return asyncio.shield(task)
 
     def spawn(self,
               fn: typing.Callable[..., typing.Awaitable],
               *args, **kwargs
               ) -> asyncio.Task:
         """Wrap the result of a `fn` into a Task and schedule its execution.
@@ -163,45 +172,43 @@
 
         Function `fn` is called with provided `args` and `kwargs`.
         Resulting Task is shielded and can be canceled only with
         `Group.async_close`.
 
         """
         if self._closing.done():
-            raise Exception('group not open')
+            raise GroupClosedError("can't spawn task in closed group")
 
         future = fn(*args, **kwargs)
         return self.wrap(future)
 
     def close(self):
         """Schedule Group closing.
 
         Closing Future is set immediately. All subgroups are closed, and all
         running tasks are canceled. Once closing of all subgroups
         and execution of all tasks is completed, closed Future is set.
 
         """
-        for child in list(self._children):
-            child.close()
-
-        if not self._canceled:
-            self._canceled = True
-            for task in self._tasks:
-                self._loop.call_soon(task.cancel)
-
         if self._closing.done():
             return
+
         self._closing.set_result(True)
 
+        for child in list(self._children):
+            child.close()
+
+        for task in self._tasks:
+            self._loop.call_soon(task.cancel)
+
         futures = [*self._tasks,
                    *(child._closed for child in self._children)]
         if futures:
-            waiting_future = asyncio.ensure_future(
-                asyncio.wait(futures), loop=self._loop)
-            waiting_future.add_done_callback(lambda _: self._on_closed())
+            waiting_task = self._loop.create_task(asyncio.wait(futures))
+            waiting_task.add_done_callback(lambda _: self._on_closed())
 
         else:
             self._on_closed()
 
     async def async_close(self):
         """Close Group and wait until closed is ``True``."""
         self.close()
@@ -213,17 +220,20 @@
     async def __aexit__(self, *args):
         await self.async_close()
 
     def _on_closed(self):
         if self._parent is not None:
             self._parent._children.remove(self)
             self._parent = None
+
         self._closed.set_result(True)
 
     def _on_task_done(self, task):
         self._tasks.remove(task)
+
         if task.cancelled():
             return
+
         e = task.exception()
         if e and self._log_exceptions:
             mlog.error('unhandled exception in async group: %s', e, exc_info=e)
             warnings.warn('unhandled exception in async group')
```

## hat/aio/misc.py

```diff
@@ -38,52 +38,65 @@
         assert await first(async_range(3), lambda x: x > 2) is None
         assert await first(async_range(3), lambda x: x > 2, 123) == 123
 
     """
     async for i in xs:
         if fn(i):
             return i
+
     return default
 
 
-async def uncancellable(f: asyncio.Future,
+async def uncancellable(obj: typing.Awaitable,
                         raise_cancel: bool = True
                         ) -> typing.Any:
-    """Uncancellable execution of a Future.
+    """Uncancellable execution of a awaitable object.
 
-    Future is shielded and its execution cannot be interrupted.
+    Object is scheduled as task, shielded and its execution cannot be
+    interrupted.
 
-    If `raise_cancel` is `True` and the Future gets canceled,
+    If `raise_cancel` is `True` and the object gets canceled,
     `asyncio.CancelledError` is reraised after the Future finishes.
 
     Warning:
         If `raise_cancel` is `False`, this method suppresses
         `asyncio.CancelledError` and stops its propagation. Use with
         caution.
 
     Args:
-        f: future
+        obj: awaitable object
         raise_cancel: raise CancelledError flag
 
     Returns:
-        future's result
+        object execution result
 
     """
     exception = None
-    task = asyncio.ensure_future(f)
+    loop = asyncio.get_running_loop()
+
+    if asyncio.iscoroutine(obj):
+        task = loop.create_task(obj)
+
+    else:
+        task = asyncio.ensure_future(obj, loop=loop)
+
     while not task.done():
         try:
             await asyncio.shield(task)
+
         except asyncio.CancelledError as e:
             if raise_cancel:
                 exception = e
+
         except Exception:
             pass
+
     if exception:
         raise exception
+
     return task.result()
 
 
 # TODO: AsyncCallable rewrite needed
 class _AsyncCallableType(type(typing.Callable), _root=True):
 
     def __init__(self):
@@ -137,16 +150,18 @@
 
         assert 'f1' == await hat.aio.call(f1, 'f1')
         assert 'f2' == await hat.aio.call(f2, 'f2')
         assert 'f3' == await hat.aio.call(f3, 'f3')
 
     """
     result = fn(*args, **kwargs)
+
     if inspect.isawaitable(result):
         result = await result
+
     return result
 
 
 async def call_on_cancel(fn: AsyncCallable, *args, **kwargs) -> typing.Any:
     """Call a function or a coroutine when canceled.
 
     When canceled, `fn` is called with `args` and `kwargs` by using
@@ -167,15 +182,16 @@
         group.spawn(call_on_cancel, f.set_result, 123)
         assert not f.done()
         await group.async_close()
         assert f.result() == 123
 
     """
     with contextlib.suppress(asyncio.CancelledError):
-        await asyncio.Future()
+        await asyncio.get_running_loop().create_future()
+
     return await call(fn, *args, *kwargs)
 
 
 async def call_on_done(f: typing.Awaitable,
                        fn: AsyncCallable,
                        *args, **kwargs
                        ) -> typing.Any:
@@ -207,14 +223,15 @@
         f.set_result(None)
         await group.wait_closed()
         assert group.is_closed
 
     """
     with contextlib.suppress(Exception):
         await f
+
     return await call(fn, *args, *kwargs)
 
 
 def init_asyncio(policy: typing.Optional[asyncio.AbstractEventLoopPolicy] = None):  # NOQA
     """Initialize asyncio.
 
     Sets event loop policy (if ``None``, instance of
```

## hat/aio/queue.py

```diff
@@ -44,184 +44,212 @@
         asyncio.ensure_future(producer())
         result = await consumer()
         assert result == 6
 
     """
 
     def __init__(self,
-                 maxsize: int = 0, *,
-                 loop: typing.Optional[asyncio.AbstractEventLoop] = None):
+                 maxsize: int = 0):
         self._maxsize = maxsize
-        self._loop = loop
         self._queue = collections.deque()
         self._getters = collections.deque()
         self._putters = collections.deque()
-        self._closed = asyncio.Future(loop=loop)
+        self._closed = False
 
     def __aiter__(self):
         return self
 
     async def __anext__(self):
         try:
             return await self.get()
+
         except QueueClosedError:
             raise StopAsyncIteration
 
     def __str__(self):
         return (f'<{type(self).__name__}'
-                f' _closed={self._closed.done()} '
+                f' _closed={self._closed} '
                 f' _queue={list(self._queue)}>')
 
     def __len__(self):
         return len(self._queue)
 
     @property
     def maxsize(self) -> int:
         """Maximum number of items in the queue."""
         return self._maxsize
 
     @property
     def is_closed(self) -> bool:
         """Is queue closed."""
-        return self._closed.done()
+        return self._closed
 
     def empty(self) -> bool:
         """``True`` if queue is empty, ``False`` otherwise."""
         return not self._queue
 
     def full(self) -> bool:
         """``True`` if queue is full, ``False`` otherwise."""
-        return (len(self._queue) >= self._maxsize if self._maxsize > 0
-                else False)
+        if self._maxsize > 0:
+            return len(self._queue) >= self._maxsize
+
+        return False
 
     def qsize(self) -> int:
         """Number of items currently in the queue."""
         return len(self._queue)
 
     def close(self):
         """Close the queue."""
-        if self._closed.done():
+        if self._closed:
             return
-        self._closed.set_result(True)
+
+        self._closed = True
         self._wakeup_all(self._putters)
         self._wakeup_next(self._getters)
 
     def get_nowait(self) -> typing.Any:
         """Return an item if one is immediately available, else raise
         `QueueEmptyError`.
 
         Raises:
             QueueEmptyError
 
         """
         if self.empty():
             raise QueueEmptyError()
+
         item = self._queue.popleft()
         self._wakeup_next(self._putters)
         return item
 
     def put_nowait(self, item: typing.Any):
         """Put an item into the queue without blocking.
 
         If no free slot is immediately available, raise `QueueFullError`.
 
         Raises:
             QueueFullError
 
         """
-        if self._closed.done():
+        if self._closed:
             raise QueueClosedError()
+
         if self.full():
             raise QueueFullError()
+
         self._queue.append(item)
         self._wakeup_next(self._getters)
 
     async def get(self) -> typing.Any:
         """Remove and return an item from the queue.
 
         If queue is empty, wait until an item is available.
 
         Raises:
             QueueClosedError
 
         """
+        loop = asyncio.get_running_loop()
+
         while self.empty():
-            if self._closed.done():
+            if self._closed:
                 self._wakeup_all(self._getters)
                 raise QueueClosedError()
-            getter = asyncio.Future()
+
+            getter = loop.create_future()
             self._getters.append(getter)
+
             try:
                 await getter
+
             except BaseException:
                 getter.cancel()
+
                 with contextlib.suppress(ValueError):
                     self._getters.remove(getter)
+
                 if not getter.cancelled():
-                    if not self.empty() or self._closed.done():
+                    if not self.empty() or self._closed:
                         self._wakeup_next(self._getters)
+
                 raise
+
         return self.get_nowait()
 
     async def put(self, item: typing.Any):
         """Put an item into the queue.
 
         If the queue is full, wait until a free slot is available before adding
         the item.
 
         Raises:
             QueueClosedError
 
         """
-        while not self._closed.done() and self.full():
-            putter = asyncio.Future()
+        loop = asyncio.get_running_loop()
+
+        while not self._closed and self.full():
+            putter = loop.create_future()
             self._putters.append(putter)
+
             try:
                 await putter
+
             except BaseException:
                 putter.cancel()
+
                 with contextlib.suppress(ValueError):
                     self._putters.remove(putter)
+
                 if not self.full() and not putter.cancelled():
                     self._wakeup_next(self._putters)
+
                 raise
+
         return self.put_nowait(item)
 
     async def get_until_empty(self) -> typing.Any:
         """Empty the queue and return the last item.
 
         If queue is empty, wait until at least one item is available.
 
         Raises:
             QueueClosedError
 
         """
         item = await self.get()
+
         while not self.empty():
             item = self.get_nowait()
+
         return item
 
     def get_nowait_until_empty(self) -> typing.Any:
         """Empty the queue and return the last item if at least one
         item is immediately available, else raise `QueueEmptyError`.
 
         Raises:
             QueueEmptyError
 
         """
         item = self.get_nowait()
+
         while not self.empty():
             item = self.get_nowait()
+
         return item
 
     def _wakeup_next(self, waiters):
         while waiters:
             waiter = waiters.popleft()
+
             if not waiter.done():
                 waiter.set_result(None)
                 break
 
     def _wakeup_all(self, waiters):
         while waiters:
             waiter = waiters.popleft()
+
             if not waiter.done():
                 waiter.set_result(None)
```

## hat/aio/wait.py

```diff
@@ -5,63 +5,66 @@
 from hat.aio.misc import call_on_done, uncancellable
 
 
 class CancelledWithResultError(asyncio.CancelledError):
     """CancelledError with associated result or exception"""
 
     def __init__(self,
-                 result: typing.Any,
+                 result: typing.Optional[typing.Any],
                  exception: typing.Optional[BaseException]):
         super().__init__()
         self.__result = result
         self.__exception = exception
 
     @property
-    def result(self) -> typing.Any:
+    def result(self) -> typing.Optional[typing.Any]:
         """Result"""
         return self.__result
 
     @property
     def exception(self) -> typing.Optional[BaseException]:
         return self.__exception
 
 
-async def wait_for(f: typing.Awaitable,
+async def wait_for(obj: typing.Awaitable,
                    timeout: float
                    ) -> typing.Any:
-    """"Wait for the single Future or coroutine to complete, with timeout.
+    """"Wait for the awaitable object to complete, with timeout.
 
     Implementation `asyncio.wait_for` that ensure propagation of
     CancelledError.
 
-    If task is cancelled with future's result available, instead of
+    If task is cancelled with objects's result available, instead of
     returning result, this implementation raises `CancelledWithResultError`.
 
     """
     group = Group(log_exceptions=False)
     group.spawn(call_on_done, asyncio.sleep(timeout), group.close)
 
-    f = group.wrap(f)
-    group.spawn(call_on_done, asyncio.shield(f), group.close)
+    task = group.wrap(obj)
+    group.spawn(call_on_done, asyncio.shield(task), group.close)
 
     exc = None
 
     try:
         await group.wait_closing()
+
     except asyncio.CancelledError as e:
         exc = e
 
     try:
         await uncancellable(group.async_close())
+
     except asyncio.CancelledError as e:
         exc = e
 
     if exc:
-        if f.cancelled():
+        if task.cancelled():
             raise exc
-        result = None if f.exception() else f.result()
-        raise CancelledWithResultError(result, f.exception()) from exc
 
-    if f.cancelled():
+        result = None if task.exception() else task.result()
+        raise CancelledWithResultError(result, task.exception()) from exc
+
+    if task.cancelled():
         raise asyncio.TimeoutError()
 
-    return f.result()
+    return task.result()
```

## Comparing `hat_aio-0.7.6.dist-info/LICENSE` & `hat_aio-0.7.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hat_aio-0.7.6.dist-info/METADATA` & `hat_aio-0.7.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hat-aio
-Version: 0.7.6
+Version: 0.7.7
 Summary: Hat async utility library
 Home-page: https://github.com/hat-open/hat-aio
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
```

