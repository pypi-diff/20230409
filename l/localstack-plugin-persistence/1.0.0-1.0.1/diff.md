# Comparing `tmp/localstack-plugin-persistence-1.0.0.tar.gz` & `tmp/localstack-plugin-persistence-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-plugin-persistence-1.0.0.tar", last modified: Thu Mar 30 10:41:57 2023, max compression
+gzip compressed data, was "localstack-plugin-persistence-1.0.1.tar", last modified: Sat Apr  8 23:37:33 2023, max compression
```

## Comparing `localstack-plugin-persistence-1.0.0.tar` & `localstack-plugin-persistence-1.0.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-03-30 10:41:57.510800 localstack-plugin-persistence-1.0.0/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2023-03-30 10:41:57.510800 localstack-plugin-persistence-1.0.0/PKG-INFO
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-03-30 10:41:57.510800 localstack-plugin-persistence-1.0.0/localstack_persistence/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      175 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/constants.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-03-30 10:41:57.510800 localstack-plugin-persistence-1.0.0/localstack_persistence/pickling/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/pickling/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      372 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/pickling/__plugins__.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-03-30 10:41:57.510800 localstack-plugin-persistence-1.0.0/localstack_persistence/pickling/reducers/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      533 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/pickling/reducers/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1008 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/pickling/reducers/cryptography.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-03-30 10:41:57.510800 localstack-plugin-persistence-1.0.0/localstack_persistence/pickling/reducers/services/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/pickling/reducers/services/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      391 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/pickling/reducers/services/acm.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1105 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/pickling/reducers/stdlib.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-03-30 10:41:57.510800 localstack-plugin-persistence-1.0.0/localstack_persistence/pods/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/pods/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      333 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/pods/__plugins__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1754 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/pods/endpoints.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3155 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/pods/load.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2038 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/pods/manager.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1638 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/pods/save.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-03-30 10:41:57.510800 localstack-plugin-persistence-1.0.0/localstack_persistence/reset/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/reset/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      337 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/reset/__plugins__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      766 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/reset/endpoints.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2478 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/reset/reset.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-03-30 10:41:57.510800 localstack-plugin-persistence-1.0.0/localstack_persistence/snapshot/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/snapshot/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3343 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/snapshot/__plugins__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1030 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/snapshot/api.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      580 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/snapshot/endpoints.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1640 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/snapshot/load.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6270 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/snapshot/manager.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1361 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/snapshot/save.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      584 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_persistence/utils.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-03-30 10:41:57.510800 localstack-plugin-persistence-1.0.0/localstack_plugin_persistence.egg-info/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_plugin_persistence.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1626 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_plugin_persistence.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_plugin_persistence.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      925 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_plugin_persistence.egg-info/entry_points.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_plugin_persistence.egg-info/not-zip-safe
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      940 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_plugin_persistence.egg-info/plux.json
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      277 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_plugin_persistence.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       23 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/localstack_plugin_persistence.egg-info/top_level.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      571 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/pyproject.toml
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      843 2023-03-30 10:41:57.510800 localstack-plugin-persistence-1.0.0/setup.cfg
--rwxrwxr-x   0 thomas    (1000) thomas    (1000)       60 2023-03-30 10:41:57.000000 localstack-plugin-persistence-1.0.0/setup.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-04-08 23:37:33.320562 localstack-plugin-persistence-1.0.1/
+-rw-r--r--   0 giograno   (501) staff       (20)      331 2023-04-08 23:37:33.320622 localstack-plugin-persistence-1.0.1/PKG-INFO
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-04-08 23:37:33.315797 localstack-plugin-persistence-1.0.1/localstack_persistence/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      175 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/constants.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-04-08 23:37:33.316074 localstack-plugin-persistence-1.0.1/localstack_persistence/pickling/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/pickling/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      372 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/pickling/__plugins__.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-04-08 23:37:33.316537 localstack-plugin-persistence-1.0.1/localstack_persistence/pickling/reducers/
+-rw-r--r--   0 giograno   (501) staff       (20)      533 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/pickling/reducers/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1514 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/pickling/reducers/cryptography.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-04-08 23:37:33.316821 localstack-plugin-persistence-1.0.1/localstack_persistence/pickling/reducers/services/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/pickling/reducers/services/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      391 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/pickling/reducers/services/acm.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1105 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/pickling/reducers/stdlib.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-04-08 23:37:33.317670 localstack-plugin-persistence-1.0.1/localstack_persistence/pods/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/pods/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      333 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/pods/__plugins__.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1754 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/pods/endpoints.py
+-rw-r--r--   0 giograno   (501) staff       (20)     3155 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/pods/load.py
+-rw-r--r--   0 giograno   (501) staff       (20)     2038 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/pods/manager.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1638 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/pods/save.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-04-08 23:37:33.318239 localstack-plugin-persistence-1.0.1/localstack_persistence/reset/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/reset/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      337 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/reset/__plugins__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      766 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/reset/endpoints.py
+-rw-r--r--   0 giograno   (501) staff       (20)     2478 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/reset/reset.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-04-08 23:37:33.319244 localstack-plugin-persistence-1.0.1/localstack_persistence/snapshot/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/snapshot/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)     3410 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/snapshot/__plugins__.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1030 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/snapshot/api.py
+-rw-r--r--   0 giograno   (501) staff       (20)      580 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/snapshot/endpoints.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1640 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/snapshot/load.py
+-rw-r--r--   0 giograno   (501) staff       (20)     6973 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/snapshot/manager.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1361 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/snapshot/save.py
+-rw-r--r--   0 giograno   (501) staff       (20)      584 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_persistence/utils.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-04-08 23:37:33.320432 localstack-plugin-persistence-1.0.1/localstack_plugin_persistence.egg-info/
+-rw-r--r--   0 giograno   (501) staff       (20)      331 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_plugin_persistence.egg-info/PKG-INFO
+-rw-r--r--   0 giograno   (501) staff       (20)     1626 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_plugin_persistence.egg-info/SOURCES.txt
+-rw-r--r--   0 giograno   (501) staff       (20)        1 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_plugin_persistence.egg-info/dependency_links.txt
+-rw-r--r--   0 giograno   (501) staff       (20)      925 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_plugin_persistence.egg-info/entry_points.txt
+-rw-r--r--   0 giograno   (501) staff       (20)        1 2023-04-08 23:37:32.000000 localstack-plugin-persistence-1.0.1/localstack_plugin_persistence.egg-info/not-zip-safe
+-rw-r--r--   0 giograno   (501) staff       (20)      940 2023-04-08 23:37:32.000000 localstack-plugin-persistence-1.0.1/localstack_plugin_persistence.egg-info/plux.json
+-rw-r--r--   0 giograno   (501) staff       (20)      277 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_plugin_persistence.egg-info/requires.txt
+-rw-r--r--   0 giograno   (501) staff       (20)       23 2023-04-08 23:37:33.000000 localstack-plugin-persistence-1.0.1/localstack_plugin_persistence.egg-info/top_level.txt
+-rw-r--r--   0 giograno   (501) staff       (20)      571 2023-04-08 23:37:32.000000 localstack-plugin-persistence-1.0.1/pyproject.toml
+-rw-r--r--   0 giograno   (501) staff       (20)      843 2023-04-08 23:37:33.320926 localstack-plugin-persistence-1.0.1/setup.cfg
+-rwxr-xr-x   0 giograno   (501) staff       (20)       60 2023-04-08 23:37:32.000000 localstack-plugin-persistence-1.0.1/setup.py
```

### Comparing `localstack-plugin-persistence-1.0.0/localstack_persistence/pickling/reducers/__init__.py` & `localstack-plugin-persistence-1.0.1/localstack_persistence/pickling/reducers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.0/localstack_persistence/pickling/reducers/stdlib.py` & `localstack-plugin-persistence-1.0.1/localstack_persistence/pickling/reducers/stdlib.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.0/localstack_persistence/pods/endpoints.py` & `localstack-plugin-persistence-1.0.1/localstack_persistence/pods/endpoints.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.0/localstack_persistence/pods/load.py` & `localstack-plugin-persistence-1.0.1/localstack_persistence/pods/load.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.0/localstack_persistence/pods/manager.py` & `localstack-plugin-persistence-1.0.1/localstack_persistence/pods/manager.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.0/localstack_persistence/pods/save.py` & `localstack-plugin-persistence-1.0.1/localstack_persistence/pods/save.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.0/localstack_persistence/reset/endpoints.py` & `localstack-plugin-persistence-1.0.1/localstack_persistence/reset/endpoints.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.0/localstack_persistence/reset/reset.py` & `localstack-plugin-persistence-1.0.1/localstack_persistence/reset/reset.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.0/localstack_persistence/snapshot/__plugins__.py` & `localstack-plugin-persistence-1.0.1/localstack_persistence/snapshot/__plugins__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import logging,os
 from localstack import config
 from localstack.aws.handlers import serve_custom_service_request_handlers
 from localstack.runtime import hooks,shutdown
 from localstack.utils.objects import singleton_factory
 from .api import LoadStrategy,SaveStrategy
 LOG=logging.getLogger(__name__)
+DEFAULT_SAVE_STRATEGY=SaveStrategy.SCHEDULED
 def is_persistence_activated():return config.PERSISTENCE and'LOCALSTACK_API_KEY'in os.environ
 @singleton_factory
 def get_save_strategy():
 	try:
 		if config.SNAPSHOT_SAVE_STRATEGY:return SaveStrategy(config.SNAPSHOT_SAVE_STRATEGY)
-	except ValueError as A:LOG.warning('Invalid save strategy, falling back to on_shutdown: %s',A)
-	return SaveStrategy.ON_REQUEST
+	except ValueError as A:LOG.warning('Invalid save strategy, falling back to %s: %s',DEFAULT_SAVE_STRATEGY,A)
+	return DEFAULT_SAVE_STRATEGY
 @singleton_factory
 def get_load_strategy():
 	try:
 		if config.SNAPSHOT_LOAD_STRATEGY:return LoadStrategy(config.SNAPSHOT_LOAD_STRATEGY)
 	except ValueError as A:LOG.warning('Invalid load strategy, falling back to on_startup: %s',A)
 	return LoadStrategy.ON_REQUEST
 @singleton_factory
@@ -32,14 +33,14 @@
 		case _:LOG.warning('Unknown load strategy %s',A)
 @hooks.on_infra_ready(should_load=is_persistence_activated(),priority=-10)
 def do_run_state_load_all():
 	A=get_load_strategy()
 	if A==LoadStrategy.ON_STARTUP:LOG.info('restoring state of all services');get_service_state_manager().load_all()
 @hooks.on_infra_start(should_load=is_persistence_activated())
 def register_state_save_strategy():
-	from localstack.aws.handlers import run_custom_response_handlers as G,serve_custom_service_request_handlers as C;from .api import SaveStrategy as A;from .manager import SaveOnRequestHandler as H,SaveStateScheduler as I;D=get_save_strategy();E=get_service_state_manager()
-	match D:
-		case A.ON_SHUTDOWN:LOG.info('registering ON_SHUTDOWN save strategy');shutdown.SHUTDOWN_HANDLERS.register(E.save_all)
-		case A.ON_REQUEST:LOG.info('registering ON_REQUEST save strategy');F=H(get_service_state_manager());C.append(F.on_request);G.append(F.on_response)
-		case A.SCHEDULED:LOG.info('registering SCHEDULED save strategy');B=I(E,period=15);shutdown.SHUTDOWN_HANDLERS.register(B.close);C.append(B.on_request_mark_service);B.start()
+	from localstack.aws.handlers import run_custom_response_handlers as C,serve_custom_service_request_handlers as D;from .api import SaveStrategy as A;from .manager import SaveOnRequestHandler as H,SaveStateScheduler as I;E=get_save_strategy();F=get_service_state_manager()
+	match E:
+		case A.ON_SHUTDOWN:LOG.info('registering ON_SHUTDOWN save strategy');shutdown.SHUTDOWN_HANDLERS.register(F.save_all)
+		case A.ON_REQUEST:LOG.info('registering ON_REQUEST save strategy');G=H(get_service_state_manager());D.append(G.on_request);C.append(G.on_response)
+		case A.SCHEDULED:LOG.info('registering SCHEDULED save strategy');B=I(F,period=15);shutdown.SHUTDOWN_HANDLERS.register(B.close);D.append(B.on_request);C.append(B.on_response);B.start()
 		case A.MANUAL:LOG.info('registering MANUAL save strategy (call /_localstack/state endpoints to save state)')
-		case _:LOG.warning('Unknown save strategy %s',D)
+		case _:LOG.warning('Unknown save strategy %s',E)
```

### Comparing `localstack-plugin-persistence-1.0.0/localstack_persistence/snapshot/api.py` & `localstack-plugin-persistence-1.0.1/localstack_persistence/snapshot/api.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.0/localstack_persistence/snapshot/endpoints.py` & `localstack-plugin-persistence-1.0.1/localstack_persistence/snapshot/endpoints.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.0/localstack_persistence/snapshot/load.py` & `localstack-plugin-persistence-1.0.1/localstack_persistence/snapshot/load.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.0/localstack_persistence/snapshot/manager.py` & `localstack-plugin-persistence-1.0.1/localstack_persistence/snapshot/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+_B=True
 _A=False
 import logging,os.path,threading,time
 from typing import Dict,Set
 from localstack.aws.api import RequestContext
 from localstack.services.plugins import ServiceManager
 from localstack.state import StateVisitor
 from localstack.state.snapshot import SnapshotPersistencePlugin
 from localstack.utils.functions import call_safe
 from localstack.utils.json import FileMappedDocument
 from localstack.utils.scheduler import Scheduler
 from localstack.utils.sync import SynchronizedDefaultDict
 from plugin import PluginManager
+from readerwriterlock import rwlock
 from localstack_persistence import constants
 from ..utils import DefaultPrioritySorter,ServiceSorter
 from .load import LoadSnapshotVisitor
 from .save import SaveSnapshotVisitor
 LOG=logging.getLogger(__name__)
 class SnapshotManager:
 	'\n    This implements the glue for making the simple disk-based persistence strategy work. It instantiates\n    the correct visitors, uses a ``ServiceManager`` to locate service plugins, and makes sure\n    ``StateLifecycleHook``s are invoked appropriately.\n    ';service_manager:0;data_dir:0;persistence_plugin_manager:0;service_sorter:0
@@ -60,49 +62,59 @@
 		if A in B._restored:return
 		if not B._locks[A].acquire(timeout=10):LOG.debug('skipping state load, service %s may still be loading state %s ',A);return
 		try:
 			if A in B._restored:return
 			try:B.state_manager.load(A)
 			finally:B._restored.add(A)
 		finally:B._locks[A].release()
+def _should_save_request(context):
+	'\n    This method determines whether a particular AWS request should trigger a state save.\n    :param context: the request context\n    :return:\n    ';A=context
+	if getattr(A,'_skip_snapshot_save',_A):return _A
+	if not A.service:return _A
+	if A.request.method not in['POST','PUT','PATCH','DELETE']:return _A
+	if A.operation:
+		B=A.operation.name
+		if B.startswith('List')or B.startswith('Get')or B.startswith('Describe'):return _A
+	elif A.service.service_name=='s3':return _A
+	return _B
 class SaveOnRequestHandler:
 	'\n    Facilitates the "ON_REQUEST" save strategy.\n    ';state_manager:0
 	def __init__(A,state_manager):A.state_manager=state_manager;A._locks=SynchronizedDefaultDict(threading.RLock)
-	def _should_save(C,context):
+	def on_request(C,_chain,context,_response):
 		A=context
-		if getattr(A,'_skip_snapshot_save',_A):return _A
-		if not A.service:return _A
-		if A.request.method not in['POST','PUT','PATCH','DELETE']:return _A
-		if A.operation:
-			B=A.operation.name
-			if B.startswith('List')or B.startswith('Get')or B.startswith('Describe'):return _A
-		elif A.service.service_name=='s3':return _A
-		return True
-	def on_request(B,_chain,context,_response):
-		A=context
-		if not B._should_save(A):return
-		C=A.service.service_name
-		if not B._locks[C].acquire(timeout=5):LOG.debug('skipping state save, service %s may still be saving state',C);A._skip_snapshot_save=True
+		if not _should_save_request(A):return
+		B=A.service.service_name
+		if not C._locks[B].acquire(timeout=5):LOG.debug('skipping state save, service %s may still be saving state',B);A._skip_snapshot_save=_B
 		else:A._skip_snapshot_save=_A
 	def on_response(A,_chain,context,_response):
 		B=context
-		if not A._should_save(B):return
+		if not _should_save_request(B):return
 		C=B.service.service_name;D=A._locks[C]
 		try:A.state_manager.save(C)
 		finally:D.release()
 class SaveStateScheduler:
 	'\n    Saves the state on a regular basis, and facilitates the "SCHEDULED" save strategy (a compromise between\n    ON_REQUEST and ON_SHUTDOWN).\n\n    It also exposes a Handler that should be added to the handler chain, which schedules services similar\n    to the SaveOnRequestHandler.\n    ';state_manager:0;period:0
-	def __init__(A,state_manager,period=30):A.state_manager=state_manager;A.scheduler=Scheduler();A.period=period;A._dirty_markers=set();A._marker_lock=threading.Lock()
-	def start(A):threading.Thread(target=A.scheduler.run,daemon=True).start();A.scheduler.schedule(A._do_save,period=A.period)
+	def __init__(A,state_manager,period=30):A.state_manager=state_manager;A.scheduler=Scheduler();A.period=period;A._dirty_markers=set();A._marker_lock=threading.Lock();A._save_lock=rwlock.RWLockWrite()
+	def start(A):threading.Thread(target=A.scheduler.run,daemon=_B).start();A.scheduler.schedule(A._do_save,period=A.period)
 	def schedule_for_save(A,service):
 		'\n        Schedule the given service into the next save cycle. Call this when you think the state of a\n        service may have changed and should be flushed to disk.\n\n        :param service: the service to be stored\n        '
 		with A._marker_lock:A._dirty_markers.add(service)
 	def _do_save(A):
 		'\n        Internal routine to perform save calls through the StateManager.\n        ';C=time.perf_counter()
-		with A._marker_lock:B=list(A._dirty_markers);A._dirty_markers.clear()
-		for D in B:A.state_manager.save(D)
-		if B:LOG.info('Service state saved to disk in %.2f seconds',time.perf_counter()-C)
+		with A._marker_lock:
+			B=list(A._dirty_markers);A._dirty_markers.clear()
+			if not B:return
+		with A._save_lock.gen_wlock():
+			LOG.debug('Saving snapshot for services %s',B)
+			for D in B:A.state_manager.save(D)
+		LOG.info('Saving snapshot to disk took %.2f seconds',time.perf_counter()-C)
 	def close(A):A.scheduler.close();A._do_save()
-	def on_request_mark_service(B,_chain,context,_response):
+	def on_request(B,_chain,context,_response):
+		A=context
+		if not _should_save_request(A):return
+		B.schedule_for_save(A.service.service_name);A._snapshot_save_rlock=B._save_lock.gen_rlock()
+		if not A._snapshot_save_rlock.acquire(timeout=10):LOG.warning('waiting on snapshot save timed out, this can cause data corruption');A._skip_snapshot_save=_B
+		else:A._skip_snapshot_save=_A
+	def on_response(B,_chain,context,_response):
 		A=context
-		if A.service is None:return
-		B.schedule_for_save(A.service.service_name)
+		if not _should_save_request(A):return
+		A._snapshot_save_rlock.release()
```

### Comparing `localstack-plugin-persistence-1.0.0/localstack_persistence/snapshot/save.py` & `localstack-plugin-persistence-1.0.1/localstack_persistence/snapshot/save.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.0/localstack_persistence/utils.py` & `localstack-plugin-persistence-1.0.1/localstack_persistence/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.0/localstack_plugin_persistence.egg-info/SOURCES.txt` & `localstack-plugin-persistence-1.0.1/localstack_plugin_persistence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.0/localstack_plugin_persistence.egg-info/entry_points.txt` & `localstack-plugin-persistence-1.0.1/localstack_plugin_persistence.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.0/localstack_plugin_persistence.egg-info/plux.json` & `localstack-plugin-persistence-1.0.1/localstack_plugin_persistence.egg-info/plux.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8888888888888888%*

 * *Differences: {"'localstack.hooks.on_infra_start'": '{insert: [(0, '*

 * *                                      "'register_reset_state_resource=localstack_persistence.reset.__plugins__:register_reset_state_resource'), "*

 * *                                      '(1, '*

 * *                                      "'register_public_cloudpods_endpoints=localstack_persistence.pods.__plugins__:register_public_cloudpods_endpoints'), "*

 * *                                      '(2, '*

 * *                                      "'register_pickle_patches_ […]*

```diff
@@ -1,16 +1,16 @@
 {
     "localstack.hooks.on_infra_ready": [
         "do_run_state_load_all=localstack_persistence.snapshot.__plugins__:do_run_state_load_all"
     ],
     "localstack.hooks.on_infra_start": [
+        "register_reset_state_resource=localstack_persistence.reset.__plugins__:register_reset_state_resource",
+        "register_public_cloudpods_endpoints=localstack_persistence.pods.__plugins__:register_public_cloudpods_endpoints",
+        "register_pickle_patches_runtime=localstack_persistence.pickling.__plugins__:register_pickle_patches_runtime",
         "register_state_load_strategy=localstack_persistence.snapshot.__plugins__:register_state_load_strategy",
         "register_state_resource=localstack_persistence.snapshot.__plugins__:register_state_resource",
-        "register_state_save_strategy=localstack_persistence.snapshot.__plugins__:register_state_save_strategy",
-        "register_pickle_patches_runtime=localstack_persistence.pickling.__plugins__:register_pickle_patches_runtime",
-        "register_reset_state_resource=localstack_persistence.reset.__plugins__:register_reset_state_resource",
-        "register_public_cloudpods_endpoints=localstack_persistence.pods.__plugins__:register_public_cloudpods_endpoints"
+        "register_state_save_strategy=localstack_persistence.snapshot.__plugins__:register_state_save_strategy"
     ],
     "localstack.hooks.prepare_host": [
         "register_pickle_patches_host=localstack_persistence.pickling.__plugins__:register_pickle_patches_host"
     ]
 }
```

### Comparing `localstack-plugin-persistence-1.0.0/pyproject.toml` & `localstack-plugin-persistence-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.0/setup.cfg` & `localstack-plugin-persistence-1.0.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [metadata]
 name = localstack-plugin-persistence
-version = 1.0.0
+version = 1.0.1
 url = https://github.com/localstack/localstack-plugin-persistence
 author = LocalStack Contributors
 author_email = info@localstack.cloud
 description = plugin containing persistence code
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 
 [options]
 zip_safe = False
 packages = find:
 install_requires = 
-	localstack-core>=1.4.1.dev
+	localstack-core>=2.0.0.dev
 	moto-ext
 
 [options.extras_require]
 dev = 
 	black>=22.1
 	coverage[toml]>=5.0.0
 	flake8-black>=0.3.6
 	flake8-isort>=6.0.0
 	flake8-quotes>=3.3.2
 	flake8>=6.0.0
 	isort>=5.10
-	localstack-core[runtime]>=1.4.1.dev
+	localstack-core[runtime]>=2.0.0.dev
 	plux>=1.3.1
 	pyproject-flake8>=6.0.0.post1
 	pytest>=7.0
 	python-minifier>=2.8.0
 
 [options.packages.find]
 exclude =
```

