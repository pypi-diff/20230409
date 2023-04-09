# Comparing `tmp/pytheus-0.0.4.tar.gz` & `tmp/pytheus-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytheus-0.0.4.tar", last modified: Fri Dec  9 01:00:49 2022, max compression
+gzip compressed data, was "pytheus-0.0.5.tar", last modified: Sun Apr  9 01:13:41 2023, max compression
```

## Comparing `pytheus-0.0.4.tar` & `pytheus-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2022-12-09 01:00:49.317318 pytheus-0.0.4/
--rw-r--r--   0 llandy     (501) staff       (20)    11357 2022-12-08 15:38:03.000000 pytheus-0.0.4/LICENSE
--rw-r--r--   0 llandy     (501) staff       (20)     9416 2022-12-09 01:00:49.317132 pytheus-0.0.4/PKG-INFO
--rw-r--r--   0 llandy     (501) staff       (20)     9036 2022-12-09 00:50:24.000000 pytheus-0.0.4/README.md
--rw-r--r--   0 llandy     (501) staff       (20)      437 2022-12-09 00:59:59.000000 pytheus-0.0.4/pyproject.toml
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2022-12-09 01:00:49.315355 pytheus-0.0.4/pytheus/
--rw-r--r--   0 llandy     (501) staff       (20)       58 2022-08-17 14:31:41.000000 pytheus-0.0.4/pytheus/__init__.py
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2022-12-09 01:00:49.316841 pytheus-0.0.4/pytheus/backends/
--rw-r--r--   0 llandy     (501) staff       (20)       60 2022-12-05 15:34:16.000000 pytheus-0.0.4/pytheus/backends/__init__.py
--rw-r--r--   0 llandy     (501) staff       (20)     4762 2022-12-07 16:28:04.000000 pytheus-0.0.4/pytheus/backends/base.py
--rw-r--r--   0 llandy     (501) staff       (20)     2879 2022-12-08 21:27:29.000000 pytheus-0.0.4/pytheus/backends/redis.py
--rw-r--r--   0 llandy     (501) staff       (20)      352 2022-12-07 13:57:38.000000 pytheus-0.0.4/pytheus/exceptions.py
--rw-r--r--   0 llandy     (501) staff       (20)     2043 2022-12-08 11:29:08.000000 pytheus-0.0.4/pytheus/exposition.py
--rw-r--r--   0 llandy     (501) staff       (20)    16875 2022-12-09 00:45:21.000000 pytheus-0.0.4/pytheus/metrics.py
--rw-r--r--   0 llandy     (501) staff       (20)     2037 2022-12-08 11:37:34.000000 pytheus-0.0.4/pytheus/registry.py
-drwxr-xr-x   0 llandy     (501) staff       (20)        0 2022-12-09 01:00:49.316144 pytheus-0.0.4/pytheus.egg-info/
--rw-r--r--   0 llandy     (501) staff       (20)     9416 2022-12-09 01:00:49.000000 pytheus-0.0.4/pytheus.egg-info/PKG-INFO
--rw-r--r--   0 llandy     (501) staff       (20)      378 2022-12-09 01:00:49.000000 pytheus-0.0.4/pytheus.egg-info/SOURCES.txt
--rw-r--r--   0 llandy     (501) staff       (20)        1 2022-12-09 01:00:49.000000 pytheus-0.0.4/pytheus.egg-info/dependency_links.txt
--rw-r--r--   0 llandy     (501) staff       (20)       44 2022-12-09 01:00:49.000000 pytheus-0.0.4/pytheus.egg-info/requires.txt
--rw-r--r--   0 llandy     (501) staff       (20)        8 2022-12-09 01:00:49.000000 pytheus-0.0.4/pytheus.egg-info/top_level.txt
--rw-r--r--   0 llandy     (501) staff       (20)       38 2022-12-09 01:00:49.317354 pytheus-0.0.4/setup.cfg
--rw-r--r--   0 llandy     (501) staff       (20)       38 2022-07-09 16:35:46.000000 pytheus-0.0.4/setup.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-09 01:13:41.662736 pytheus-0.0.5/
+-rw-r--r--   0 llandy     (501) staff       (20)    11357 2022-12-08 15:38:03.000000 pytheus-0.0.5/LICENSE
+-rw-r--r--   0 llandy     (501) staff       (20)    12214 2023-04-09 01:13:41.662497 pytheus-0.0.5/PKG-INFO
+-rw-r--r--   0 llandy     (501) staff       (20)    11813 2023-04-09 00:43:25.000000 pytheus-0.0.5/README.md
+-rw-r--r--   0 llandy     (501) staff       (20)     1037 2023-04-09 01:11:17.000000 pytheus-0.0.5/pyproject.toml
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-09 01:13:41.659371 pytheus-0.0.5/pytheus/
+-rw-r--r--   0 llandy     (501) staff       (20)       58 2022-08-17 14:31:41.000000 pytheus-0.0.5/pytheus/__init__.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-09 01:13:41.661125 pytheus-0.0.5/pytheus/backends/
+-rw-r--r--   0 llandy     (501) staff       (20)       60 2022-12-05 15:34:16.000000 pytheus-0.0.5/pytheus/backends/__init__.py
+-rw-r--r--   0 llandy     (501) staff       (20)     4148 2023-04-04 00:38:41.000000 pytheus-0.0.5/pytheus/backends/base.py
+-rw-r--r--   0 llandy     (501) staff       (20)     3142 2023-04-04 00:38:41.000000 pytheus-0.0.5/pytheus/backends/redis.py
+-rw-r--r--   0 llandy     (501) staff       (20)      352 2022-12-07 13:57:38.000000 pytheus-0.0.5/pytheus/exceptions.py
+-rw-r--r--   0 llandy     (501) staff       (20)     2058 2023-04-02 20:13:46.000000 pytheus-0.0.5/pytheus/exposition.py
+-rw-r--r--   0 llandy     (501) staff       (20)    17904 2023-04-08 18:15:41.000000 pytheus-0.0.5/pytheus/metrics.py
+-rw-r--r--   0 llandy     (501) staff       (20)     3051 2023-04-03 00:08:23.000000 pytheus-0.0.5/pytheus/registry.py
+-rw-r--r--   0 llandy     (501) staff       (20)      173 2023-04-01 23:52:48.000000 pytheus-0.0.5/pytheus/utils.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-09 01:13:41.660329 pytheus-0.0.5/pytheus.egg-info/
+-rw-r--r--   0 llandy     (501) staff       (20)    12214 2023-04-09 01:13:41.000000 pytheus-0.0.5/pytheus.egg-info/PKG-INFO
+-rw-r--r--   0 llandy     (501) staff       (20)      465 2023-04-09 01:13:41.000000 pytheus-0.0.5/pytheus.egg-info/SOURCES.txt
+-rw-r--r--   0 llandy     (501) staff       (20)        1 2023-04-09 01:13:41.000000 pytheus-0.0.5/pytheus.egg-info/dependency_links.txt
+-rw-r--r--   0 llandy     (501) staff       (20)      164 2023-04-09 01:13:41.000000 pytheus-0.0.5/pytheus.egg-info/requires.txt
+-rw-r--r--   0 llandy     (501) staff       (20)        8 2023-04-09 01:13:41.000000 pytheus-0.0.5/pytheus.egg-info/top_level.txt
+-rw-r--r--   0 llandy     (501) staff       (20)       38 2023-04-09 01:13:41.662786 pytheus-0.0.5/setup.cfg
+-rw-r--r--   0 llandy     (501) staff       (20)       38 2022-07-09 16:35:46.000000 pytheus-0.0.5/setup.py
+drwxr-xr-x   0 llandy     (501) staff       (20)        0 2023-04-09 01:13:41.662047 pytheus-0.0.5/tests/
+-rw-r--r--   0 llandy     (501) staff       (20)     5852 2023-03-30 23:54:35.000000 pytheus-0.0.5/tests/test_exposition.py
+-rw-r--r--   0 llandy     (501) staff       (20)    21760 2023-04-03 00:00:50.000000 pytheus-0.0.5/tests/test_metrics.py
+-rw-r--r--   0 llandy     (501) staff       (20)     2892 2023-04-01 00:46:20.000000 pytheus-0.0.5/tests/test_registry.py
```

### Comparing `pytheus-0.0.4/LICENSE` & `pytheus-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytheus-0.0.4/PKG-INFO` & `pytheus-0.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,59 @@
-Metadata-Version: 2.1
-Name: pytheus
-Version: 0.0.4
-Summary: playing with metrics
-Author-email: Llandy Riveron Del Risco <llandy3d@gmail.com>
-Project-URL: repository, https://github.com/Llandy3d/pytheus
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: redis
-License-File: LICENSE
-
 <img src="https://user-images.githubusercontent.com/16627175/185823115-b33905c3-f389-40e1-b830-2197889a936a.png" height="400">
 
 # pytheus
 
 playing with metrics
 
 ---
 
-Experimenting with a different way of creating prometheus metrics in python:
-- support for default labels value ✅
-- partial labels value (built in an incremental way) ✅
-- multiple multiprocess support:
-  - mmap file based (wip ⚠️)
-  - redis backend ✅
-- customizable registry support ✅
-- registry prefix support ✅
+pytheus is a modern python library for collecting [prometheus](https://prometheus.io/docs/introduction/overview/) metrics built with multiprocessing in mind.
+
+Some of the features are:
+
+  - multiple multiprocess support:
+    - redis backend ✅
+    - bring your own ✅
+  - support for default labels value ✅
+  - partial labels value (built in an incremental way) ✅
+  - customizable registry support ✅
+  - registry prefix support ✅
+
+---
+## Philosophy
+
+Simply put is to let you work with metrics the way you want.
+
+Be extremely flexible, allow for customization from the user for anything they might want to do without having to resort to hacks and most importantly offer the same api for single & multi process scenarios, the switch should be as easy as loading a different backend without having to change anything in the code.
+
+- What you see is what you get.
+- No differences between `singleprocess` & `multiprocess`, the only change is loading a different backend and everything will work out of the box.
+- High flexibility with an high degree of `labels` control and customization.
+
+---
+## Requirements
+
+- Python 3.10+
+- redis >= 4.0.0 (**optional**: for multiprocessing)
+
+---
+
+**Architecture**
+
+A small piece of the architecture is described in the [ARCHITECTURE.md file](ARCHITECTURE.md)
 
 ---
 
 **Install**
 
 ```
 pip install pytheus
 ```
 
-Optionally if you want to use the Redis backend you will need the redis library:
+Optionally if you want to use the Redis backend (for multiprocess support) you will need the redis library:
 ```python
 pip install redis
 # or
 pip install pytheus[redis]
 ```
 
 ---
@@ -124,24 +137,26 @@
 histogram = Histogram('page_visits_latency_seconds', 'used for testing')
 
 # this is the endpoint that prometheus will use to scrape the metrics
 @app.route('/metrics')
 def metrics():
     return generate_metrics()
 
+# track time with the context manager
 @app.route('/')
 def home():
     with histogram.time():
         return 'hello world!'
 
+# you can also track time with the decorator shortcut
 @app.route('/slow')
+@histogram
 def slow():
-    with histogram.time():
-        time.sleep(3)
-        return 'hello world! from slow!'
+    time.sleep(3)
+    return 'hello world! from slow!'
 
 app.run(host='0.0.0.0', port=8080)
 ```
 
 and if you have prometheus installed configure it to scrape on localhost:8080 or you can still use the included `docker-compose.yml` file.
 
 ---
@@ -162,15 +177,15 @@
 
 # increase by x
 counter.inc(7)
 
 # it is possible to count exceptions
 with counter.count_exceptions():
     raise ValueError  # increases counter by 1
-    
+
 # you can specify which exceptions to watch for
 with counter.count_exceptions((IndexError, ValueError)):
     raise ValueError. # increases counter by 1
 
 # it is possible to use the counter as a decorator as a shortcut to count exceptions
 @counter
 def test():
@@ -207,15 +222,15 @@
 
 # set to current unix timestamp
 gauge.set_to_current_time()
 
 # it is possible to track progress so that when entered increases the value by 1, and when exited decreases it
 with gauge.track_inprogress():
     do_something()
-    
+
 # you can also time a piece of code, will set the duration in seconds to value when exited
 with gauge.time():
     do_something()
 
 # tracking time can also be done as a decorator
 @gauge
 def do_something():
@@ -236,25 +251,46 @@
 # note: the +Inf bucket will be added automatically, this is float('inf') in python
 
 # create a histogram specifying buckets
 histogram = Histogram(name="my_histogram", description="My description", buckets=(0.2, 1, 3))
 
 # observe a value
 histogram.observe(0.4)
-    
+
 # you can also time a piece of code, will set the duration in seconds to value when exited
 with histogram.time():
     do_something()
 
 # tracking time can also be done as a decorator
 @histogram
 def do_something():
     ...
 ```
 
+## Custom Collectors
+
+It is possible to use a custom collector in cases you can't directly instrument the code.
+You will need to inherit from `CustomCollector` and define the `collect` method.
+Also be sure to disable the automatic registering of a newly created metric into the default registry.
+
+```python
+from pytheus.metrics import Counter, CustomCollector
+from pytheus.registry import REGISTRY
+
+class MyCustomCollector(CustomCollector):
+    def collect():
+        counter = Counter('name', 'desc', registry=None)  # note that we are disabling automatic registering
+        counter.inc()
+        yield counter
+
+REGISTRY.register(MyCustomCollector())
+```
+
+Note: if one of the yield metrics have a name already registered with the registry you are trying to register to, the custom collector will be ignored.
+
 
 ## How to use different backends
 
 Things work out of the box, using the SingleProcessBackend:
 
 ```python
 from pytheus.metrics import Counter
@@ -269,15 +305,15 @@
 print(counter._metric_value_backend.config)
 # {}
 ```
 
 You can define environment configuration to have different defaults, using two environment variables:
 
 ```bash
-export PYTHEUS_BACKEND_CLASS="pytheus.backends.MultipleProcessFileBackend"
+export PYTHEUS_BACKEND_CLASS="pytheus.backends.MultiProcessFileBackend"
 export PYTHEUS_BACKEND_CONFIG="./config.json"
 ```
 
 Now, create the config file, `./config.json`:
 
 ```json
 {
@@ -292,29 +328,29 @@
 
 counter = Counter(
     name="my_metric",
     description="My description",
     required_labels=["label_a", "label_b"],
 )
 print(counter._metric_value_backend.__class__)
-# <class 'pytheus.backends.MultipleProcessFileBackend'>
+# <class 'pytheus.backends.MultiProcessFileBackend'>
 print(counter._metric_value_backend.config)
 # {'pytheus_file_directory': "./"}
 ```
 
 You can also pass the values directly in Python, which would take precedence over the environment
 setup we have just described:
 
 ```python
 
 from pytheus.metrics import Counter
-from pytheus.backends import MultipleProcessRedisBackend, load_backend
+from pytheus.backends import MultiProcessRedisBackend, load_backend
 
 load_backend(
-    backend_class=MultipleProcessRedisBackend,
+    backend_class=MultiProcessRedisBackend,
     backend_config={
       "host": "127.0.0.1",
       "port":  6379
     }
 )
 # Notice that if you simply call load_backend(), it would reload config from the environment.
 
@@ -323,11 +359,52 @@
 
 counter = Counter(
     name="my_metric",
     description="My description",
     required_labels=["label_a", "label_b"],
 )
 print(counter._metric_value_backend.__class__)
-# <class 'pytheus.backends.MultipleProcessRedisBackend'>
+# <class 'pytheus.backends.MultiProcessRedisBackend'>
 print(counter._metric_value_backend.config)
 # {'host': '127.0.0.1', 'port': 6379}
 ```
+
+## Create your own Backend
+
+### Custom Backend
+
+You can create your own backend by implementing a class that fulfills the `Backend` protocol.
+
+```python
+class Backend(Protocol):
+    def __init__(
+        self,
+        config: BackendConfig,
+        metric: "_Metric",
+        histogram_bucket: str | None = None,
+    ) -> None:
+        ...
+
+    def inc(self, value: float) -> None:
+        ...
+
+    def dec(self, value: float) -> None:
+        ...
+
+    def set(self, value: float) -> None:
+        ...
+
+    def get(self) -> float:
+        ...
+```
+
+### Initialization hook
+
+It's possible that you want to initialize your custom backed or there are one time steps that you want to happen on import.
+
+To achieve that you can use the class method hook called `_initialize` that accepts a `BackendConfig` parameter.
+
+```python
+@classmethod
+def _initialize(cls, config: "BackendConfig") -> None:
+    # initialization steps
+```
```

### Comparing `pytheus-0.0.4/README.md` & `pytheus-0.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,73 @@
+Metadata-Version: 2.1
+Name: pytheus
+Version: 0.0.5
+Summary: playing with metrics
+Author-email: Llandy Riveron Del Risco <llandy3d@gmail.com>
+Project-URL: repository, https://github.com/Llandy3d/pytheus
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: redis
+Provides-Extra: docs
+License-File: LICENSE
+
 <img src="https://user-images.githubusercontent.com/16627175/185823115-b33905c3-f389-40e1-b830-2197889a936a.png" height="400">
 
 # pytheus
 
 playing with metrics
 
 ---
 
-Experimenting with a different way of creating prometheus metrics in python:
-- support for default labels value ✅
-- partial labels value (built in an incremental way) ✅
-- multiple multiprocess support:
-  - mmap file based (wip ⚠️)
-  - redis backend ✅
-- customizable registry support ✅
-- registry prefix support ✅
+pytheus is a modern python library for collecting [prometheus](https://prometheus.io/docs/introduction/overview/) metrics built with multiprocessing in mind.
+
+Some of the features are:
+
+  - multiple multiprocess support:
+    - redis backend ✅
+    - bring your own ✅
+  - support for default labels value ✅
+  - partial labels value (built in an incremental way) ✅
+  - customizable registry support ✅
+  - registry prefix support ✅
+
+---
+## Philosophy
+
+Simply put is to let you work with metrics the way you want.
+
+Be extremely flexible, allow for customization from the user for anything they might want to do without having to resort to hacks and most importantly offer the same api for single & multi process scenarios, the switch should be as easy as loading a different backend without having to change anything in the code.
+
+- What you see is what you get.
+- No differences between `singleprocess` & `multiprocess`, the only change is loading a different backend and everything will work out of the box.
+- High flexibility with an high degree of `labels` control and customization.
+
+---
+## Requirements
+
+- Python 3.10+
+- redis >= 4.0.0 (**optional**: for multiprocessing)
+
+---
+
+**Architecture**
+
+A small piece of the architecture is described in the [ARCHITECTURE.md file](ARCHITECTURE.md)
 
 ---
 
 **Install**
 
 ```
 pip install pytheus
 ```
 
-Optionally if you want to use the Redis backend you will need the redis library:
+Optionally if you want to use the Redis backend (for multiprocess support) you will need the redis library:
 ```python
 pip install redis
 # or
 pip install pytheus[redis]
 ```
 
 ---
@@ -111,24 +151,26 @@
 histogram = Histogram('page_visits_latency_seconds', 'used for testing')
 
 # this is the endpoint that prometheus will use to scrape the metrics
 @app.route('/metrics')
 def metrics():
     return generate_metrics()
 
+# track time with the context manager
 @app.route('/')
 def home():
     with histogram.time():
         return 'hello world!'
 
+# you can also track time with the decorator shortcut
 @app.route('/slow')
+@histogram
 def slow():
-    with histogram.time():
-        time.sleep(3)
-        return 'hello world! from slow!'
+    time.sleep(3)
+    return 'hello world! from slow!'
 
 app.run(host='0.0.0.0', port=8080)
 ```
 
 and if you have prometheus installed configure it to scrape on localhost:8080 or you can still use the included `docker-compose.yml` file.
 
 ---
@@ -149,15 +191,15 @@
 
 # increase by x
 counter.inc(7)
 
 # it is possible to count exceptions
 with counter.count_exceptions():
     raise ValueError  # increases counter by 1
-    
+
 # you can specify which exceptions to watch for
 with counter.count_exceptions((IndexError, ValueError)):
     raise ValueError. # increases counter by 1
 
 # it is possible to use the counter as a decorator as a shortcut to count exceptions
 @counter
 def test():
@@ -194,15 +236,15 @@
 
 # set to current unix timestamp
 gauge.set_to_current_time()
 
 # it is possible to track progress so that when entered increases the value by 1, and when exited decreases it
 with gauge.track_inprogress():
     do_something()
-    
+
 # you can also time a piece of code, will set the duration in seconds to value when exited
 with gauge.time():
     do_something()
 
 # tracking time can also be done as a decorator
 @gauge
 def do_something():
@@ -223,25 +265,46 @@
 # note: the +Inf bucket will be added automatically, this is float('inf') in python
 
 # create a histogram specifying buckets
 histogram = Histogram(name="my_histogram", description="My description", buckets=(0.2, 1, 3))
 
 # observe a value
 histogram.observe(0.4)
-    
+
 # you can also time a piece of code, will set the duration in seconds to value when exited
 with histogram.time():
     do_something()
 
 # tracking time can also be done as a decorator
 @histogram
 def do_something():
     ...
 ```
 
+## Custom Collectors
+
+It is possible to use a custom collector in cases you can't directly instrument the code.
+You will need to inherit from `CustomCollector` and define the `collect` method.
+Also be sure to disable the automatic registering of a newly created metric into the default registry.
+
+```python
+from pytheus.metrics import Counter, CustomCollector
+from pytheus.registry import REGISTRY
+
+class MyCustomCollector(CustomCollector):
+    def collect():
+        counter = Counter('name', 'desc', registry=None)  # note that we are disabling automatic registering
+        counter.inc()
+        yield counter
+
+REGISTRY.register(MyCustomCollector())
+```
+
+Note: if one of the yield metrics have a name already registered with the registry you are trying to register to, the custom collector will be ignored.
+
 
 ## How to use different backends
 
 Things work out of the box, using the SingleProcessBackend:
 
 ```python
 from pytheus.metrics import Counter
@@ -256,15 +319,15 @@
 print(counter._metric_value_backend.config)
 # {}
 ```
 
 You can define environment configuration to have different defaults, using two environment variables:
 
 ```bash
-export PYTHEUS_BACKEND_CLASS="pytheus.backends.MultipleProcessFileBackend"
+export PYTHEUS_BACKEND_CLASS="pytheus.backends.MultiProcessFileBackend"
 export PYTHEUS_BACKEND_CONFIG="./config.json"
 ```
 
 Now, create the config file, `./config.json`:
 
 ```json
 {
@@ -279,29 +342,29 @@
 
 counter = Counter(
     name="my_metric",
     description="My description",
     required_labels=["label_a", "label_b"],
 )
 print(counter._metric_value_backend.__class__)
-# <class 'pytheus.backends.MultipleProcessFileBackend'>
+# <class 'pytheus.backends.MultiProcessFileBackend'>
 print(counter._metric_value_backend.config)
 # {'pytheus_file_directory': "./"}
 ```
 
 You can also pass the values directly in Python, which would take precedence over the environment
 setup we have just described:
 
 ```python
 
 from pytheus.metrics import Counter
-from pytheus.backends import MultipleProcessRedisBackend, load_backend
+from pytheus.backends import MultiProcessRedisBackend, load_backend
 
 load_backend(
-    backend_class=MultipleProcessRedisBackend,
+    backend_class=MultiProcessRedisBackend,
     backend_config={
       "host": "127.0.0.1",
       "port":  6379
     }
 )
 # Notice that if you simply call load_backend(), it would reload config from the environment.
 
@@ -310,11 +373,52 @@
 
 counter = Counter(
     name="my_metric",
     description="My description",
     required_labels=["label_a", "label_b"],
 )
 print(counter._metric_value_backend.__class__)
-# <class 'pytheus.backends.MultipleProcessRedisBackend'>
+# <class 'pytheus.backends.MultiProcessRedisBackend'>
 print(counter._metric_value_backend.config)
 # {'host': '127.0.0.1', 'port': 6379}
 ```
+
+## Create your own Backend
+
+### Custom Backend
+
+You can create your own backend by implementing a class that fulfills the `Backend` protocol.
+
+```python
+class Backend(Protocol):
+    def __init__(
+        self,
+        config: BackendConfig,
+        metric: "_Metric",
+        histogram_bucket: str | None = None,
+    ) -> None:
+        ...
+
+    def inc(self, value: float) -> None:
+        ...
+
+    def dec(self, value: float) -> None:
+        ...
+
+    def set(self, value: float) -> None:
+        ...
+
+    def get(self) -> float:
+        ...
+```
+
+### Initialization hook
+
+It's possible that you want to initialize your custom backed or there are one time steps that you want to happen on import.
+
+To achieve that you can use the class method hook called `_initialize` that accepts a `BackendConfig` parameter.
+
+```python
+@classmethod
+def _initialize(cls, config: "BackendConfig") -> None:
+    # initialization steps
+```
```

### Comparing `pytheus-0.0.4/pytheus/backends/redis.py` & `pytheus-0.0.5/pytheus/backends/redis.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,91 @@
-import redis
-
 from typing import TYPE_CHECKING
 
-from pytheus.backends.base import Backend, BackendConfig
-
+import redis
 
 if TYPE_CHECKING:
-    from pytheus.metrics import _Metric, Histogram
+    from pytheus.backends.base import BackendConfig
+    from pytheus.metrics import _Metric
+
 
+EXPIRE_KEY_TIME = 3600  # 1 hour
 
-class MultipleProcessRedisBackend(Backend):
+
+class MultiProcessRedisBackend:
     """
     Provides a multi-process backend that uses Redis.
     Single dimension metrics will be stored as list (ex. Counter) while labelled
     metrics will be stored in an hash.
     Currently is very naive, and there is a lot of room for improvement.
     (ex. maybe store all dimensions in the same hash and be smart on retrieving everything...)
-    Note: currently not expiring keys
     """
 
-    CONNECTION_POOL: redis.Redis = None
+    CONNECTION_POOL: redis.Redis | None = None
 
     def __init__(
         self,
-        config: BackendConfig,
-        metric: '_Metric',
-        histogram_bucket: float = None
+        config: "BackendConfig",
+        metric: "_Metric",
+        histogram_bucket: str | None = None,
     ) -> None:
-        super().__init__(config, metric)
-        self._key_name = self.metric._collector.name
+        self._key_name = metric._collector.name
         self._labels_hash = None
         self._histogram_bucket = histogram_bucket
 
         # keys for histograms are of type `myhisto:2.5`
         if histogram_bucket:
-            self._key_name = f'{self._key_name}:{histogram_bucket}'
+            self._key_name = f"{self._key_name}:{histogram_bucket}"
 
         # default labels
         joint_labels = None
-        if self.metric._collector._default_labels_count:
-            joint_labels = self.metric._collector._default_labels.copy()
-            if self.metric._labels:
-                joint_labels.update(self.metric._labels)
+        if metric._collector._default_labels_count:
+            joint_labels = metric._collector._default_labels.copy()  # type: ignore
+            if metric._labels:
+                joint_labels.update(metric._labels)
 
         if joint_labels:
-            self._labels_hash = '-'.join(sorted(joint_labels.values()))
-        elif self.metric._labels:
-            self._labels_hash = '-'.join(sorted(self.metric._labels.values()))
-
-        if self.CONNECTION_POOL is None:
-            MultipleProcessRedisBackend.CONNECTION_POOL = redis.Redis(
-                **config,
-                decode_responses=True,
-            )
-
-    def is_valid_config(self, config: BackendConfig) -> bool:
-        return True  # TODO
+            self._labels_hash = "-".join(sorted(joint_labels.values()))
+        elif metric._labels:
+            self._labels_hash = "-".join(sorted(metric._labels.values()))
+
+    @classmethod
+    def _initialize(cls, config: "BackendConfig") -> None:
+        cls.CONNECTION_POOL = redis.Redis(
+            **config,
+            decode_responses=True,
+        )
+        cls.CONNECTION_POOL.ping()
 
     def inc(self, value: float) -> None:
+        assert self.CONNECTION_POOL is not None
         if self._labels_hash:
             self.CONNECTION_POOL.hincrbyfloat(self._key_name, self._labels_hash, value)
         else:
             self.CONNECTION_POOL.incrbyfloat(self._key_name, value)
 
+        self.CONNECTION_POOL.expire(self._key_name, EXPIRE_KEY_TIME)
+
     def dec(self, value: float) -> None:
+        assert self.CONNECTION_POOL is not None
         if self._labels_hash:
             self.CONNECTION_POOL.hincrbyfloat(self._key_name, self._labels_hash, -value)
         else:
             self.CONNECTION_POOL.incrbyfloat(self._key_name, -value)
 
+        self.CONNECTION_POOL.expire(self._key_name, EXPIRE_KEY_TIME)
+
     def set(self, value: float) -> None:
+        assert self.CONNECTION_POOL is not None
         if self._labels_hash:
             self.CONNECTION_POOL.hset(self._key_name, self._labels_hash, value)
         else:
             self.CONNECTION_POOL.set(self._key_name, value)
 
+        self.CONNECTION_POOL.expire(self._key_name, EXPIRE_KEY_TIME)
+
     def get(self) -> float:
+        assert self.CONNECTION_POOL is not None
         if self._labels_hash:
             value = self.CONNECTION_POOL.hget(self._key_name, self._labels_hash)
         else:
             value = self.CONNECTION_POOL.get(self._key_name)
         return float(value) if value else 0.0
```

### Comparing `pytheus-0.0.4/pytheus/exposition.py` & `pytheus-0.0.5/pytheus/exposition.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,54 +10,53 @@
 
 
 def generate_metrics(registry: Registry = REGISTRY) -> str:
     """
     Returns the metrics from the registry in prometheus text format
     """
     lines = (
-        generate_from_collector(collector, registry.prefix)
-        for collector in registry.collect()
+        generate_from_collector(collector, registry.prefix) for collector in registry.collect()
     )
     output = LINE_SEPARATOR.join(lines)
     output += "\n"
     return output
 
 
 def format_labels(labels: Labels | None) -> str:
     if not labels:
-        return ''
+        return ""
     label_str = (f'{name}="{value}"' for name, value in labels.items())
     return f"{{{LABEL_SEPARATOR.join(label_str)}}}"
 
 
-def generate_from_collector(collector: Collector, prefix: str = None) -> str:
+def generate_from_collector(collector: Collector, prefix: str | None = None) -> str:
     """
     Returns the metrics from a given collector in prometheus text format
     """
-    metric_name = f'{prefix}_{collector.name}' if prefix else collector.name
+    metric_name = f"{prefix}_{collector.name}" if prefix else collector.name
     help_text = f"# HELP {metric_name} {collector.description}"
     type_text = f"# TYPE {metric_name} {collector.type_}"
     output = [help_text, type_text]
 
     for sample in collector.collect():
         label_str = format_labels(sample.labels)
         metric = f"{metric_name}{sample.suffix}{label_str} {sample.value}"
         output.append(metric)
     return LINE_SEPARATOR.join(output)
 
 
 def make_wsgi_app(registry: Registry = REGISTRY) -> Callable:
     """Create a WSGI app which serves the metrics from a registry."""
 
-    def prometheus_app(environ, start_response):
-        status = '200 OK'
-        if environ['PATH_INFO'] == '/favicon.ico':
+    def prometheus_app(environ, start_response):  # type: ignore
+        status = "200 OK"
+        if environ["PATH_INFO"] == "/favicon.ico":
             # Serve empty response for browsers
-            headers = [('', '')]
-            output = ''
+            headers = [("", "")]
+            output = ""
         else:
             output = generate_metrics(registry)
-            headers = [('Content-Type', PROMETHEUS_CONTENT_TYPE)]
+            headers = [("Content-Type", PROMETHEUS_CONTENT_TYPE)]
         start_response(status, headers)
         return [output.encode()]
 
     return prometheus_app
```

### Comparing `pytheus-0.0.4/pytheus/metrics.py` & `pytheus-0.0.5/pytheus/metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,158 +1,170 @@
 import functools
 import itertools
 import re
 import time
-
 from collections.abc import Generator
 from contextlib import contextmanager
 from dataclasses import dataclass
-from typing import Sequence, Iterator, Callable
+from typing import Callable, Iterable, Sequence
 
 from pytheus.backends import get_backend
 from pytheus.exceptions import (
-    UnobservableMetricException,
-    LabelValidationException,
     BucketException,
+    LabelValidationException,
+    UnobservableMetricException,
 )
-from pytheus.registry import REGISTRY, Registry
-
+from pytheus.registry import REGISTRY, Collector, Registry
+from pytheus.utils import MetricType
 
 Labels = dict[str, str]
 
 
-metric_name_re = re.compile(r'[a-zA-Z_:][a-zA-Z0-9_:]*')
-label_name_re = re.compile(r'[a-zA-Z_][a-zA-Z0-9_]*')
+metric_name_re = re.compile(r"[a-zA-Z_:][a-zA-Z0-9_:]*")
+label_name_re = re.compile(r"[a-zA-Z_][a-zA-Z0-9_]*")
 
 
 @dataclass
 class Sample:
     suffix: str
     labels: dict[str, str] | None
     value: float
 
 
+class CustomCollector(Collector):
+    """
+    Inheriting from this protocol is the current way to create a custom collector.
+    The property `name` will return the lowercased class name so that it can be
+    tracked in a registry.
+    Not particularly liking this solution but for now it should suffice due to
+    the current structure.
+    """
+
+    @property
+    def name(self) -> str:
+        return str.lower(self.__class__.__name__)
+
+    # overriding the Collector protocol it requires to be writeable so we have this dummy setter
+    @name.setter
+    def name(self, value: str) -> None:
+        pass
+
+
 class _MetricCollector:
     """
     #TODO
-
     _labeled_metrics contains all observable metrics when required_labels is set.
     """
 
     def __init__(
         self,
         name: str,
         description: str,
-        metric: '_Metric',
+        metric: "_Metric",
         required_labels: Sequence[str] | None = None,
         default_labels: Labels | None = None,
-        registry: Registry = REGISTRY
+        registry: Registry | None = REGISTRY,
     ) -> None:
         if metric_name_re.fullmatch(name) is None:
-            raise ValueError(f'Invalid metric name: {name}')
+            raise ValueError(f"Invalid metric name: {name}")
 
         if required_labels:
             is_histogram = isinstance(metric, Histogram)
             self._validate_required_labels(required_labels, is_histogram)
 
         self._required_labels = set(required_labels) if required_labels else None
 
         if default_labels:
             self._validate_labels(default_labels)
 
         self.name = name
         self.description = description
+        self.type_ = metric.type_
         self._default_labels = default_labels
         self._default_labels_count = len(default_labels) if default_labels else 0
         self._metric = metric
         self._labeled_metrics: dict[tuple[str, ...], _Metric] = {}
-        registry.register(self)
+        self._registry = registry
 
-    @property
-    def type_(self) -> str:
-        # TODO check maybe a proper MetricTypes should to be defined
-        return str.lower(self._metric.__class__.__name__)
+        if registry:
+            registry.register(self)
 
-    def _validate_required_labels(self, labels: Sequence[str], is_histogram: bool = False):
+    def _validate_required_labels(self, labels: Sequence[str], is_histogram: bool = False) -> None:
         """
         Validates label names according to the regex.
         Labels starting with `__` are reserved for internal use by Prometheus.
         """
         for label in labels:
-            if label.startswith('__') or label_name_re.fullmatch(label) is None:
-                raise LabelValidationException(f'Invalid label name: {label}')
-            if is_histogram and label == 'le':
-                raise LabelValidationException(f'Invalid label name for Histogram: {label}')
+            if label.startswith("__") or label_name_re.fullmatch(label) is None:
+                raise LabelValidationException(f"Invalid label name: {label}")
+            if is_histogram and label == "le":
+                raise LabelValidationException(f"Invalid label name for Histogram: {label}")
 
-    def _validate_labels(self, labels: Labels):
+    def _validate_labels(self, labels: Labels) -> None:
         """
         Validates labels.
         If no `required_labels` is set raises an error.
         `labels` will be also validated to be a subset of `required_labels`.
         """
         if not self._required_labels:
-            raise LabelValidationException('trying to use labels while required_labels is None')
+            raise LabelValidationException("trying to use labels while required_labels is None")
 
         labels_set = set(labels.keys())
         if not labels_set.issubset(self._required_labels):
             raise LabelValidationException(
-                'labels different than required_labels: '
-                f'{labels_set} != {self._required_labels}'
+                "labels different than required_labels: " f"{labels_set} != {self._required_labels}"
             )
 
-    def collect(self) -> Iterator[Sample]:
+    def collect(self) -> Iterable[Sample]:
         """
         Collects Samples for the metric.
         """
+        labeled_metrics: Iterable[Sample]
         if self._required_labels:
-            labeled_metrics = (metric.collect() for metric in self._labeled_metrics.values())
-            if isinstance(self._metric, Histogram):
-                # as histograms collect returns an iterator, we flatten it
-                labeled_metrics = (sample for metric in labeled_metrics for sample in metric)
+            labeled_metrics = (
+                sample for metric in self._labeled_metrics.values() for sample in metric.collect()
+            )
             if self._default_labels and self._metric._can_observe:
-                # NOTE: a lot of these checks or duplication could be removed if all collect()
-                # would return an Iterator
-                if isinstance(self._metric, Histogram):
-                    labeled_metrics = itertools.chain(labeled_metrics, self._metric.collect())
-                else:
-                    labeled_metrics = itertools.chain(labeled_metrics, (self._metric.collect(),))
+                labeled_metrics = itertools.chain(labeled_metrics, self._metric.collect())
             return labeled_metrics
         else:
-            # histograms return already an iterator of Samples
-            if isinstance(self._metric, Histogram):
-                return self._metric.collect()
-            else:
-                return iter((self._metric.collect(),))
+            return self._metric.collect()
 
 
 class _Metric:
+    type_: MetricType = MetricType.UNTYPED
+
     def __init__(
         self,
         name: str,
         description: str,
         required_labels: Sequence[str] | None = None,
         labels: Labels | None = None,
         default_labels: Labels | None = None,
+        registry: Registry | None = REGISTRY,
         collector: _MetricCollector | None = None,
     ) -> None:
-        self._name = name
-        self._description = description
+        self.name = name
+        self.description = description
         self._labels = labels
+        self._registry = registry
         self._metric_value_backend = None
         self._collector = (
             collector
             if collector
-            else _MetricCollector(name, description, self, required_labels, default_labels)
+            else _MetricCollector(
+                name, description, self, required_labels, default_labels, registry
+            )
         )
         self._can_observe = self._check_can_observe()
 
         if not collector and labels:
             raise LabelValidationException(
-                'Setting labels when creating a metric is not allowed. '
-                'You might be looking for default_labels.'
+                "Setting labels when creating a metric is not allowed. "
+                "You might be looking for default_labels."
             )
 
         if self._can_observe and not isinstance(self, Histogram):
             self._metric_value_backend = get_backend(self)
 
     def _check_can_observe(self) -> bool:
         if not self._collector._required_labels:
@@ -181,15 +193,15 @@
         return True
 
     def _raise_if_cannot_observe(self) -> None:
         """Raise if the metric cannot be observed, for example if labels values are missing."""
         if not self._can_observe:
             raise UnobservableMetricException
 
-    def labels(self, labels_: Labels) -> '_Metric':
+    def labels(self, labels_: Labels) -> "_Metric":
         """
         If no labels is passed to the call returns itself.
         If there are already present labels, they will be updated with the passed labels_ and if
         it's not observable will just return the new child instance. Otherwise it will also add
         the instance to the labeled_metrics on the collector.
         """
         # if not labels_ or self._collector._required_labels is None:
@@ -206,79 +218,82 @@
         if self._collector._default_labels:
             default_labels = self._collector._default_labels.copy()
             default_labels.update(labels_)
             labels_count = len(default_labels)
         else:
             labels_count = len(labels_)
 
+        assert self._collector._required_labels is not None
         if labels_count != len(self._collector._required_labels):
             # does not add to collector
             return self.__class__(
-                self._name,
-                self._description,
+                self.name,
+                self.description,
                 collector=self._collector,
-                labels=labels_
+                labels=labels_,
+                registry=self._registry,
             )
 
         # add to collector
         sorted_label_values = tuple(v for _, v in sorted(labels_.items()))
         if sorted_label_values in self._collector._labeled_metrics:
             metric = self._collector._labeled_metrics[sorted_label_values]
         else:
             metric = self.__class__(
-                self._name,
-                self._description,
+                self.name,
+                self.description,
                 collector=self._collector,
-                labels=labels_
+                labels=labels_,
+                registry=self._registry,
             )
             self._collector._labeled_metrics[sorted_label_values] = metric
         return metric
 
-    def collect(self) -> Sample:
+    def collect(self) -> Iterable[Sample]:
         raise NotImplementedError
 
     def _get_sample(self) -> Sample:
         """Get a Sample for testing. Each metric type will need to define its own."""
         self._raise_if_cannot_observe()
-        sample = Sample('', self._labels, 0)
+        sample = Sample("", self._labels, 0)
         return self._add_default_labels_to_sample(sample)
 
     def _add_default_labels_to_sample(self, sample: Sample) -> Sample:
         """Adds default labels if available to a sample."""
         if self._collector._default_labels_count:
-            joint_labels = self._collector._default_labels.copy()
+            joint_labels = self._collector._default_labels.copy()  # type: ignore
             if sample.labels:
                 joint_labels.update(sample.labels)
             sample.labels = joint_labels
 
         return sample
 
     def __repr__(self) -> str:
-        return f'{self.__class__.__qualname__}({self._collector.name})'
+        return f"{self.__class__.__qualname__}({self._collector.name})"
 
 
 class Counter(_Metric):
+    type_: MetricType = MetricType.COUNTER
 
     def inc(self, value: float = 1.0) -> None:
         """
         Increments the value by the given amount.
         By default it will be 1.
         value must be >= 0.
         """
         self._raise_if_cannot_observe()
         if value < 0:
-            raise ValueError(f'Counter increase value ({value}) must be >= 0')
+            raise ValueError(f"Counter increase value ({value}) must be >= 0")
 
+        assert self._metric_value_backend is not None
         self._metric_value_backend.inc(value)
 
-    # TODO: consider adding decorator support
     @contextmanager
     def count_exceptions(
-        self,
-        exceptions: type[Exception] | tuple[Exception] | None = None
+        self, exceptions: type[Exception] | tuple[Exception] | None = None
     ) -> Generator[None, None, None]:
         """
         Will count and reraise raised exceptions.
         It is possibly to specify which exceptions to track.
         """
         self._raise_if_cannot_observe()
         if exceptions is None:
@@ -288,212 +303,230 @@
             yield
         except exceptions:  # type: ignore
             self.inc()
             raise
 
     def __call__(
         self,
-        func: Callable = None,
+        func: Callable | None = None,
         exceptions: type[Exception] | tuple[Exception] | None = None,
-    ):
+    ) -> Callable:
         """
         When called acts as a decorator counting exceptions raised.
         """
         if func is None:
             return functools.partial(self.__call__, exceptions=exceptions)
 
         @functools.wraps(func)
-        def wrapper(*args, **kwargs):
+        def wrapper(*args, **kwargs):  # type: ignore
             with self.count_exceptions(exceptions):
                 return func(*args, **kwargs)
+
         return wrapper
 
-    def collect(self) -> Sample:
+    def collect(self) -> Iterable[Sample]:
         self._raise_if_cannot_observe()
-        sample = Sample('', self._labels, self._metric_value_backend.get())
-        return self._add_default_labels_to_sample(sample)
+        assert self._metric_value_backend is not None
+        sample = Sample("", self._labels, self._metric_value_backend.get())
+        return (self._add_default_labels_to_sample(sample),)
 
 
 class Gauge(_Metric):
+    type_: MetricType = MetricType.GAUGE
 
     def inc(self, value: float = 1.0) -> None:
         """
         Increments the value by the given amount.
         By default it will be 1.
         """
         self._raise_if_cannot_observe()
+        assert self._metric_value_backend is not None
         self._metric_value_backend.inc(value)
 
     def dec(self, value: float = 1.0) -> None:
         """
         Decrements the value by the given amount.
         By default it will be 1.
         """
         self._raise_if_cannot_observe()
+        assert self._metric_value_backend is not None
         self._metric_value_backend.dec(value)
 
     def set(self, value: float) -> None:
         """
         Set the value to the given amount.
         """
         self._raise_if_cannot_observe()
+        assert self._metric_value_backend is not None
         self._metric_value_backend.set(value)
 
     def set_to_current_time(self) -> None:
         """Set the value to the current unix timestamp."""
         self._raise_if_cannot_observe()
+        assert self._metric_value_backend is not None
         self._metric_value_backend.set(time.time())
 
     @contextmanager
     def track_inprogress(self) -> Generator[None, None, None]:
         """
         Will increase the gauge value when entered and decrease it when exited.
         """
         self._raise_if_cannot_observe()
         self.inc()
         yield
         self.dec()
 
     # TODO: this could be configured to allow the decoration to be used
     # with track_inprogress giving more flexibility.
-    def __call__(self, func: Callable):
+    def __call__(self, func: Callable) -> Callable:
         """
         When called acts as a decorator tracking the time taken by
         the wrapped function.
         """
+
         @functools.wraps(func)
-        def wrapper(*args, **kwargs):
+        def wrapper(*args, **kwargs):  # type: ignore
             with self.time():
                 return func(*args, **kwargs)
+
         return wrapper
 
     @contextmanager
     def time(self) -> Generator[None, None, None]:
         """
         Times the duration inside of it and sets the value.
         """
         self._raise_if_cannot_observe()
         start = time.perf_counter()
         yield
         self.set(time.perf_counter() - start)
 
-    def collect(self) -> Sample:
+    def collect(self) -> Iterable[Sample]:
         self._raise_if_cannot_observe()
-        sample = Sample('', self._labels, self._metric_value_backend.get())
-        return self._add_default_labels_to_sample(sample)
+        assert self._metric_value_backend is not None
+        sample = Sample("", self._labels, self._metric_value_backend.get())
+        return (self._add_default_labels_to_sample(sample),)
 
 
 class Histogram(_Metric):
+    type_: MetricType = MetricType.HISTOGRAM
     # Default buckets are tailored to broadly measure the response time (in seconds) of a network
     # service. Most likely you will be required to define buckets customized to your use case.
-    # Valus taken from the golang/rust client.
-    DEFAULT_BUCKETS = (.005, .01, .025, .05, .1, .25, .5, 1, 2.5, 5, 10)
+    # Values taken from the golang/rust client.
+    DEFAULT_BUCKETS = (0.005, 0.01, 0.025, 0.05, 0.1, 0.25, 0.5, 1, 2.5, 5, 10)
 
     def __init__(
         self,
         name: str,
         description: str,
         required_labels: Sequence[str] | None = None,
         labels: Labels | None = None,
         default_labels: Labels | None = None,
+        registry: Registry | None = REGISTRY,
         collector: _MetricCollector | None = None,
         buckets: Sequence[float] = DEFAULT_BUCKETS,
     ) -> None:
         super().__init__(
             name,
             description,
             required_labels,
             labels,
             default_labels,
+            registry,
             collector,
         )
 
         # buckets
 
         # if buckets is None or an empty sequence default buckets will be used
         if not buckets:
             buckets = list(self.DEFAULT_BUCKETS)
         else:
             buckets = list(buckets)
 
         sorted_buckets = sorted(buckets)
         if buckets != sorted_buckets:
             raise BucketException(
-                f'buckets values are not in sorted order. {buckets} != {sorted_buckets}'
+                f"buckets values are not in sorted order. {buckets} != {sorted_buckets}"
             )
 
         # +inf is required so we always add it
-        if buckets[-1] != float('inf'):
-            buckets.append(float('inf'))
+        if buckets[-1] != float("inf"):
+            buckets.append(float("inf"))
 
         self._upper_bounds = buckets
 
         # create bucket values
         self._buckets = None
         self._sum = None
         self._count = None
         if self._can_observe:
             self._buckets = []
 
             # this will be added just to the default name on the redis backend but it is
             # fine for now as it's the only one. Might require a more robust way in the future.
-            self._sum = get_backend(self, histogram_bucket='sum')
-            self._count = get_backend(self, histogram_bucket='count')
-            # NOTE: yap might make more sente to rename it
+            self._sum = get_backend(self, histogram_bucket="sum")
+            self._count = get_backend(self, histogram_bucket="count")
 
             for bucket in self._upper_bounds:
-                self._buckets.append(get_backend(self, histogram_bucket=bucket))
+                self._buckets.append(get_backend(self, histogram_bucket=str(bucket)))
 
     def observe(self, value: float) -> None:
         """
         Observe the given value.
         Value can be negative, in that case the rate function will be less useful so
         it's better to consider using two histograms for positive and negative values.
         """
         self._raise_if_cannot_observe()
+        assert self._sum is not None
         self._sum.inc(value)
 
         for i, bound in enumerate(self._upper_bounds):
             if value <= bound:
                 self._buckets[i].inc(1)
 
+        assert self._count is not None
         self._count.inc(1)
 
     @contextmanager
     def time(self) -> Generator[None, None, None]:
         """
         Times the duration inside of it and sets the value.
         """
         self._raise_if_cannot_observe()
         start = time.perf_counter()
         yield
         self.observe(time.perf_counter() - start)
 
-    def __call__(self, func: Callable):
+    def __call__(self, func: Callable) -> Callable:
         """
         When called acts as a decorator tracking the time taken by
         the wrapped function.
         """
+
         @functools.wraps(func)
-        def wrapper(*args, **kwargs):
+        def wrapper(*args, **kwargs):  # type: ignore
             with self.time():
                 return func(*args, **kwargs)
+
         return wrapper
 
-    def collect(self) -> Iterator[Sample]:
+    def collect(self) -> Iterable[Sample]:
         self._raise_if_cannot_observe()
         samples = []
         for i, bound in enumerate(self._upper_bounds):
             bucket_labels = self._labels.copy() if self._labels else {}
-            bucket_labels['le'] = bound
-            sample = Sample('_bucket', bucket_labels, self._buckets[i].get())
+            bucket_labels["le"] = str(bound)
+            sample = Sample("_bucket", bucket_labels, self._buckets[i].get())
             samples.append(sample)
 
-        samples.append(Sample('_sum', self._labels, self._sum.get()))
-        samples.append(Sample('_count', self._labels, self._count.get()))
+        assert self._sum is not None
+        assert self._count is not None
+        samples.append(Sample("_sum", self._labels, self._sum.get()))
+        samples.append(Sample("_count", self._labels, self._count.get()))
 
         return (self._add_default_labels_to_sample(sample) for sample in samples)
 
 
 # maybe just go with the typing alias
 @dataclass
 class Label:
```

### Comparing `pytheus-0.0.4/pytheus/registry.py` & `pytheus-0.0.5/pytheus/registry.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,65 +1,83 @@
 from logging import getLogger
 from threading import Lock
-from typing import Iterable, Optional, Protocol
+from typing import Iterable, Protocol
+
+from pytheus.utils import MetricType
 
 logger = getLogger(__name__)
 
 
 class Collector(Protocol):
     name: str
     description: str
+    type_: MetricType
 
     def collect(self) -> Iterable:
         ...
 
-    @property
-    def type_(self) -> str:
-        ...
-
 
 class Registry(Protocol):
     prefix: str | None
 
-    def register(self, collector: Collector):
+    def register(self, collector: Collector) -> None:
         ...
 
-    def unregister(self, collector: Collector):
+    def unregister(self, collector: Collector) -> None:
         ...
 
     def collect(self) -> Iterable:
         ...
 
 
 class CollectorRegistry:
-    def __init__(self, prefix: str = None) -> None:
+    def __init__(self, prefix: str | None = None) -> None:
         self._lock = Lock()
         self.prefix = prefix
         self._collectors: dict[str, Collector] = {}
 
     def register(self, collector: Collector) -> None:
         with self._lock:
             if collector.name in self._collectors:
-                logger.warning(f"collector with name '{collector.name}' already registred")
+                logger.warning(
+                    f"collector with name '{collector.name}' already registered."
+                    " Keeping previous entry"
+                )
                 return
+            # if it has not this field it's a custom collector, I do not like this approach but
+            # let's get it working
+            if not hasattr(collector, "type_"):
+                for _collector in collector.collect():
+                    if _collector.name in self._collectors:
+                        logger.warning(
+                            f"CustomCollector: {collector.name} - collector with name"
+                            f" '{_collector.name}' already registered. Ignoring custom collector"
+                        )
+                        return
+
+            # NOTE: in case the user is adding directly a metric to the registry
+            # we need to add the _MetricCollector to the registry. There might be a better way
+            # to d this but it should work for now.
+            if hasattr(collector, "_collector"):
+                collector = collector._collector
             self._collectors[collector.name] = collector
 
     def unregister(self, collector: Collector) -> None:
         with self._lock:
             if collector.name not in self._collectors:
                 logger.warning(f"no collector found with name '{collector.name}'")
                 return
             del self._collectors[collector.name]
 
     def collect(self) -> Iterable[Collector]:
         yield from self._collectors.values()
 
 
 class CollectorRegistryProxy:
-    def __init__(self, registry: Registry = None) -> None:
+    def __init__(self, registry: Registry | None = None) -> None:
         self._registry = registry or CollectorRegistry()
         self.prefix = self._registry.prefix
 
     def set_registry(self, registry: Registry) -> None:
         self._registry = registry
         self.prefix = self._registry.prefix
```

### Comparing `pytheus-0.0.4/pytheus.egg-info/PKG-INFO` & `pytheus-0.0.5/pytheus.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,73 @@
 Metadata-Version: 2.1
 Name: pytheus
-Version: 0.0.4
+Version: 0.0.5
 Summary: playing with metrics
 Author-email: Llandy Riveron Del Risco <llandy3d@gmail.com>
 Project-URL: repository, https://github.com/Llandy3d/pytheus
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: redis
+Provides-Extra: docs
 License-File: LICENSE
 
 <img src="https://user-images.githubusercontent.com/16627175/185823115-b33905c3-f389-40e1-b830-2197889a936a.png" height="400">
 
 # pytheus
 
 playing with metrics
 
 ---
 
-Experimenting with a different way of creating prometheus metrics in python:
-- support for default labels value ✅
-- partial labels value (built in an incremental way) ✅
-- multiple multiprocess support:
-  - mmap file based (wip ⚠️)
-  - redis backend ✅
-- customizable registry support ✅
-- registry prefix support ✅
+pytheus is a modern python library for collecting [prometheus](https://prometheus.io/docs/introduction/overview/) metrics built with multiprocessing in mind.
+
+Some of the features are:
+
+  - multiple multiprocess support:
+    - redis backend ✅
+    - bring your own ✅
+  - support for default labels value ✅
+  - partial labels value (built in an incremental way) ✅
+  - customizable registry support ✅
+  - registry prefix support ✅
+
+---
+## Philosophy
+
+Simply put is to let you work with metrics the way you want.
+
+Be extremely flexible, allow for customization from the user for anything they might want to do without having to resort to hacks and most importantly offer the same api for single & multi process scenarios, the switch should be as easy as loading a different backend without having to change anything in the code.
+
+- What you see is what you get.
+- No differences between `singleprocess` & `multiprocess`, the only change is loading a different backend and everything will work out of the box.
+- High flexibility with an high degree of `labels` control and customization.
+
+---
+## Requirements
+
+- Python 3.10+
+- redis >= 4.0.0 (**optional**: for multiprocessing)
+
+---
+
+**Architecture**
+
+A small piece of the architecture is described in the [ARCHITECTURE.md file](ARCHITECTURE.md)
 
 ---
 
 **Install**
 
 ```
 pip install pytheus
 ```
 
-Optionally if you want to use the Redis backend you will need the redis library:
+Optionally if you want to use the Redis backend (for multiprocess support) you will need the redis library:
 ```python
 pip install redis
 # or
 pip install pytheus[redis]
 ```
 
 ---
@@ -124,24 +151,26 @@
 histogram = Histogram('page_visits_latency_seconds', 'used for testing')
 
 # this is the endpoint that prometheus will use to scrape the metrics
 @app.route('/metrics')
 def metrics():
     return generate_metrics()
 
+# track time with the context manager
 @app.route('/')
 def home():
     with histogram.time():
         return 'hello world!'
 
+# you can also track time with the decorator shortcut
 @app.route('/slow')
+@histogram
 def slow():
-    with histogram.time():
-        time.sleep(3)
-        return 'hello world! from slow!'
+    time.sleep(3)
+    return 'hello world! from slow!'
 
 app.run(host='0.0.0.0', port=8080)
 ```
 
 and if you have prometheus installed configure it to scrape on localhost:8080 or you can still use the included `docker-compose.yml` file.
 
 ---
@@ -162,15 +191,15 @@
 
 # increase by x
 counter.inc(7)
 
 # it is possible to count exceptions
 with counter.count_exceptions():
     raise ValueError  # increases counter by 1
-    
+
 # you can specify which exceptions to watch for
 with counter.count_exceptions((IndexError, ValueError)):
     raise ValueError. # increases counter by 1
 
 # it is possible to use the counter as a decorator as a shortcut to count exceptions
 @counter
 def test():
@@ -207,15 +236,15 @@
 
 # set to current unix timestamp
 gauge.set_to_current_time()
 
 # it is possible to track progress so that when entered increases the value by 1, and when exited decreases it
 with gauge.track_inprogress():
     do_something()
-    
+
 # you can also time a piece of code, will set the duration in seconds to value when exited
 with gauge.time():
     do_something()
 
 # tracking time can also be done as a decorator
 @gauge
 def do_something():
@@ -236,25 +265,46 @@
 # note: the +Inf bucket will be added automatically, this is float('inf') in python
 
 # create a histogram specifying buckets
 histogram = Histogram(name="my_histogram", description="My description", buckets=(0.2, 1, 3))
 
 # observe a value
 histogram.observe(0.4)
-    
+
 # you can also time a piece of code, will set the duration in seconds to value when exited
 with histogram.time():
     do_something()
 
 # tracking time can also be done as a decorator
 @histogram
 def do_something():
     ...
 ```
 
+## Custom Collectors
+
+It is possible to use a custom collector in cases you can't directly instrument the code.
+You will need to inherit from `CustomCollector` and define the `collect` method.
+Also be sure to disable the automatic registering of a newly created metric into the default registry.
+
+```python
+from pytheus.metrics import Counter, CustomCollector
+from pytheus.registry import REGISTRY
+
+class MyCustomCollector(CustomCollector):
+    def collect():
+        counter = Counter('name', 'desc', registry=None)  # note that we are disabling automatic registering
+        counter.inc()
+        yield counter
+
+REGISTRY.register(MyCustomCollector())
+```
+
+Note: if one of the yield metrics have a name already registered with the registry you are trying to register to, the custom collector will be ignored.
+
 
 ## How to use different backends
 
 Things work out of the box, using the SingleProcessBackend:
 
 ```python
 from pytheus.metrics import Counter
@@ -269,15 +319,15 @@
 print(counter._metric_value_backend.config)
 # {}
 ```
 
 You can define environment configuration to have different defaults, using two environment variables:
 
 ```bash
-export PYTHEUS_BACKEND_CLASS="pytheus.backends.MultipleProcessFileBackend"
+export PYTHEUS_BACKEND_CLASS="pytheus.backends.MultiProcessFileBackend"
 export PYTHEUS_BACKEND_CONFIG="./config.json"
 ```
 
 Now, create the config file, `./config.json`:
 
 ```json
 {
@@ -292,29 +342,29 @@
 
 counter = Counter(
     name="my_metric",
     description="My description",
     required_labels=["label_a", "label_b"],
 )
 print(counter._metric_value_backend.__class__)
-# <class 'pytheus.backends.MultipleProcessFileBackend'>
+# <class 'pytheus.backends.MultiProcessFileBackend'>
 print(counter._metric_value_backend.config)
 # {'pytheus_file_directory': "./"}
 ```
 
 You can also pass the values directly in Python, which would take precedence over the environment
 setup we have just described:
 
 ```python
 
 from pytheus.metrics import Counter
-from pytheus.backends import MultipleProcessRedisBackend, load_backend
+from pytheus.backends import MultiProcessRedisBackend, load_backend
 
 load_backend(
-    backend_class=MultipleProcessRedisBackend,
+    backend_class=MultiProcessRedisBackend,
     backend_config={
       "host": "127.0.0.1",
       "port":  6379
     }
 )
 # Notice that if you simply call load_backend(), it would reload config from the environment.
 
@@ -323,11 +373,52 @@
 
 counter = Counter(
     name="my_metric",
     description="My description",
     required_labels=["label_a", "label_b"],
 )
 print(counter._metric_value_backend.__class__)
-# <class 'pytheus.backends.MultipleProcessRedisBackend'>
+# <class 'pytheus.backends.MultiProcessRedisBackend'>
 print(counter._metric_value_backend.config)
 # {'host': '127.0.0.1', 'port': 6379}
 ```
+
+## Create your own Backend
+
+### Custom Backend
+
+You can create your own backend by implementing a class that fulfills the `Backend` protocol.
+
+```python
+class Backend(Protocol):
+    def __init__(
+        self,
+        config: BackendConfig,
+        metric: "_Metric",
+        histogram_bucket: str | None = None,
+    ) -> None:
+        ...
+
+    def inc(self, value: float) -> None:
+        ...
+
+    def dec(self, value: float) -> None:
+        ...
+
+    def set(self, value: float) -> None:
+        ...
+
+    def get(self) -> float:
+        ...
+```
+
+### Initialization hook
+
+It's possible that you want to initialize your custom backed or there are one time steps that you want to happen on import.
+
+To achieve that you can use the class method hook called `_initialize` that accepts a `BackendConfig` parameter.
+
+```python
+@classmethod
+def _initialize(cls, config: "BackendConfig") -> None:
+    # initialization steps
+```
```

