# Comparing `tmp/dequeai-0.686.tar.gz` & `tmp/dequeai-0.688.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.686.tar", last modified: Fri Apr  7 19:00:13 2023, max compression
+gzip compressed data, was "dequeai-0.688.tar", last modified: Sun Apr  9 14:07:43 2023, max compression
```

## Comparing `dequeai-0.686.tar` & `dequeai-0.688.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:00:13.598715 dequeai-0.686/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-07 19:00:13.598715 dequeai-0.686/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:00:13.598715 dequeai-0.686/dequeai/
--rw-r--r--   0 root         (0) root         (0)      260 2023-04-07 18:40:49.000000 dequeai-0.686/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15374 2023-03-27 20:38:54.000000 dequeai-0.686/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.686/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      489 2022-05-12 21:04:59.000000 dequeai-0.686/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      538 2023-04-07 18:51:21.000000 dequeai-0.686/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    19333 2023-04-07 18:59:51.000000 dequeai-0.686/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.686/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.686/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.686/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.686/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 19:00:13.598715 dequeai-0.686/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-07 19:00:13.000000 dequeai-0.686/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-07 19:00:13.000000 dequeai-0.686/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 19:00:13.000000 dequeai-0.686/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-04-07 19:00:13.000000 dequeai-0.686/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-07 19:00:13.000000 dequeai-0.686/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-07 19:00:13.598715 dequeai-0.686/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      479 2023-04-07 19:00:00.000000 dequeai-0.686/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 14:07:43.621577 dequeai-0.688/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-09 14:07:43.621577 dequeai-0.688/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 14:07:43.621577 dequeai-0.688/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-04-08 20:25:27.000000 dequeai-0.688/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15374 2023-03-27 20:38:54.000000 dequeai-0.688/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.688/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      489 2022-05-12 21:04:59.000000 dequeai-0.688/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      613 2023-04-09 13:53:50.000000 dequeai-0.688/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    20399 2023-04-09 14:07:06.000000 dequeai-0.688/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.688/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.688/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.688/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.688/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 14:07:43.621577 dequeai-0.688/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-09 14:07:43.000000 dequeai-0.688/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-09 14:07:43.000000 dequeai-0.688/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 14:07:43.000000 dequeai-0.688/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-04-09 14:07:43.000000 dequeai-0.688/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-09 14:07:43.000000 dequeai-0.688/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 14:07:43.621577 dequeai-0.688/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      479 2023-04-09 14:07:22.000000 dequeai-0.688/setup.py
```

### Comparing `dequeai-0.686/dequeai/datatypes.py` & `dequeai-0.688/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.686/dequeai/dequeai_run.py` & `dequeai-0.688/dequeai/dequeai_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -287,14 +287,27 @@
         p = multiprocessing.Process(target=self._log_task, args=(full_data, self._run_meta_data))
         p.start()
         #self._send_data_to_redis(step=self._step, data=full_data)
         os.environ['step']=str(self._step)
         if commit:
             self._step += 1
 
+    def log_hyperparams(self, hyperparams):
+        self._validate_hyperparams(hyperparams=hyperparams)
+        full_data = {"hyperparams": hyperparams}
+        full_data.update(
+            {"user_name": self.user_name, "run_id": self._run_id, "workload_type": self._workload_type,
+             "workload_id": self._workload_id, "submission_id": self._submission_id,
+             "project_name": self._project_name, "deque_log_time": datetime.datetime.now()})
+
+        resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/experiment/hyperparams/create/",
+                             json=full_data)
+        res = resp.json()
+        print(res)
+
     def _log_task(self, data, run_meta_data):
         pickled_data = pickle.dumps(data)
         self._rest.post_binary(url=TRACKING_ENDPOINT, data=pickled_data)
 
     def log_artifact(self, artifact_type, path):
         if self._run_meta_data is None:
             raise ValueError("Run not initialized. Please call init first")
@@ -455,25 +468,35 @@
                                    Image, Plot] or type(value) in types.__builtins__.values():
                     pass
                 else:
                     raise ValueError(
                         "Invalid type in dictionary. Allowed values include builtin types and Deque data types " + str(
                             type(value)) + " " + str(value.__class__.__module__))
 
+    def _validate_hyperparams(self, hyperparams):
+        for key, value in hyperparams.items():
+
+            if type(value) in types.__builtins__.values():
+                pass
+            else:
+                raise ValueError(
+                    "Invalid type in hyperparam dict. Allowed values include builtin types " + str(
+                        type(value)) + " " + str(value.__class__.__module__))
+
     def _send_upstream(self):
         self._rest.post(url=AGENT_API_SERVICE_URL + "/fex/python/track/", json=self._history)
         self._history = dict()
 
     def _authenticate(self):
         return True
 
 
 if __name__ == "__main__":
     deque = Run()
-    deque.validate_data({"train": {"accuracy": "1.3", "loss": "2.2"}})
+    deque._validate_hyperparams({"train": {"accuracy": "1.3", "loss": "2.2"}})
     #deque.log_artifact_task(artifact_type=RESOURCES, path="//dequeapp.egg-info",
        #                     run_meta_data=None)
     # deque.init(user_name="riju@deque.app", project_name="awesome-dude")
     # for i in range(100):
     # deque.log(data={"train": {"accuracy": i, "loss": i - 100}, "image": deque.im})
 
     # deque.log(data={"image":deque.im})
```

### Comparing `dequeai-0.686/dequeai/parsing_service.py` & `dequeai-0.688/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.686/dequeai/rest_connect.py` & `dequeai-0.688/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.686/dequeai/util.py` & `dequeai-0.688/dequeai/util.py`

 * *Files identical despite different names*

