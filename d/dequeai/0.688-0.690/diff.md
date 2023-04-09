# Comparing `tmp/dequeai-0.688.tar.gz` & `tmp/dequeai-0.690.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.688.tar", last modified: Sun Apr  9 14:07:43 2023, max compression
+gzip compressed data, was "dequeai-0.690.tar", last modified: Sun Apr  9 14:33:58 2023, max compression
```

## Comparing `dequeai-0.688.tar` & `dequeai-0.690.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 14:07:43.621577 dequeai-0.688/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-09 14:07:43.621577 dequeai-0.688/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 14:07:43.621577 dequeai-0.688/dequeai/
--rw-r--r--   0 root         (0) root         (0)      295 2023-04-08 20:25:27.000000 dequeai-0.688/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15374 2023-03-27 20:38:54.000000 dequeai-0.688/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.688/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      489 2022-05-12 21:04:59.000000 dequeai-0.688/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      613 2023-04-09 13:53:50.000000 dequeai-0.688/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    20399 2023-04-09 14:07:06.000000 dequeai-0.688/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.688/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.688/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.688/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.688/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 14:07:43.621577 dequeai-0.688/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      316 2023-04-09 14:07:43.000000 dequeai-0.688/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-09 14:07:43.000000 dequeai-0.688/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 14:07:43.000000 dequeai-0.688/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-04-09 14:07:43.000000 dequeai-0.688/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-09 14:07:43.000000 dequeai-0.688/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 14:07:43.621577 dequeai-0.688/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      479 2023-04-09 14:07:22.000000 dequeai-0.688/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 14:33:58.403685 dequeai-0.690/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-09 14:33:58.403685 dequeai-0.690/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 14:33:58.403685 dequeai-0.690/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-04-08 20:25:27.000000 dequeai-0.690/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15374 2023-03-27 20:38:54.000000 dequeai-0.690/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.690/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      489 2022-05-12 21:04:59.000000 dequeai-0.690/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      613 2023-04-09 13:53:50.000000 dequeai-0.690/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    20399 2023-04-09 14:33:12.000000 dequeai-0.690/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.690/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.690/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.690/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.690/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-09 14:33:58.403685 dequeai-0.690/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-04-09 14:33:57.000000 dequeai-0.690/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-09 14:33:58.000000 dequeai-0.690/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-09 14:33:57.000000 dequeai-0.690/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-04-09 14:33:58.000000 dequeai-0.690/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-09 14:33:58.000000 dequeai-0.690/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-09 14:33:58.403685 dequeai-0.690/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      479 2023-04-09 14:33:46.000000 dequeai-0.690/setup.py
```

### Comparing `dequeai-0.688/dequeai/datatypes.py` & `dequeai-0.690/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.688/dequeai/dequeai.py` & `dequeai-0.690/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.688/dequeai/dequeai_run.py` & `dequeai-0.690/dequeai/dequeai_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,20 +288,20 @@
         p.start()
         #self._send_data_to_redis(step=self._step, data=full_data)
         os.environ['step']=str(self._step)
         if commit:
             self._step += 1
 
     def log_hyperparams(self, hyperparams):
-        self._validate_hyperparams(hyperparams=hyperparams)
+        #self._validate_hyperparams(hyperparams=hyperparams)
         full_data = {"hyperparams": hyperparams}
         full_data.update(
             {"user_name": self.user_name, "run_id": self._run_id, "workload_type": self._workload_type,
              "workload_id": self._workload_id, "submission_id": self._submission_id,
-             "project_name": self._project_name, "deque_log_time": datetime.datetime.now()})
+             "project_name": self._project_name,"create_datetime":datetime.datetime.now()})
 
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/experiment/hyperparams/create/",
                              json=full_data)
         res = resp.json()
         print(res)
 
     def _log_task(self, data, run_meta_data):
```

### Comparing `dequeai-0.688/dequeai/parsing_service.py` & `dequeai-0.690/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.688/dequeai/rest_connect.py` & `dequeai-0.690/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.688/dequeai/util.py` & `dequeai-0.690/dequeai/util.py`

 * *Files identical despite different names*

