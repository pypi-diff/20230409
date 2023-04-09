# Comparing `tmp/transmission_rpc-4.1.5.tar.gz` & `tmp/transmission_rpc-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transmission_rpc-4.1.5.tar", max compression
+gzip compressed data, was "transmission_rpc-4.2.0.tar", max compression
```

## Comparing `transmission_rpc-4.1.5.tar` & `transmission_rpc-4.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1127 2023-04-05 06:53:17.050727 transmission_rpc-4.1.5/LICENSE
--rw-r--r--   0        0        0     1630 2023-04-05 06:53:17.050727 transmission_rpc-4.1.5/README.md
--rw-r--r--   0        0        0     3147 2023-04-05 06:53:17.050727 transmission_rpc-4.1.5/pyproject.toml
--rw-r--r--   0        0        0     1982 2023-04-05 06:53:17.050727 transmission_rpc-4.1.5/transmission_rpc/__init__.py
--rw-r--r--   0        0        0    44572 2023-04-05 06:53:17.050727 transmission_rpc-4.1.5/transmission_rpc/client.py
--rw-r--r--   0        0        0    11051 2023-04-05 06:53:17.050727 transmission_rpc-4.1.5/transmission_rpc/constants.py
--rw-r--r--   0        0        0     1124 2023-04-05 06:53:17.050727 transmission_rpc-4.1.5/transmission_rpc/error.py
--rw-r--r--   0        0        0    12990 2023-04-05 06:53:17.050727 transmission_rpc-4.1.5/transmission_rpc/session.py
--rw-r--r--   0        0        0    23663 2023-04-05 06:53:17.050727 transmission_rpc-4.1.5/transmission_rpc/torrent.py
--rw-r--r--   0        0        0     1497 2023-04-05 06:53:17.050727 transmission_rpc-4.1.5/transmission_rpc/types.py
--rw-r--r--   0        0        0     2669 2023-04-05 06:53:17.050727 transmission_rpc-4.1.5/transmission_rpc/utils.py
--rw-r--r--   0        0        0     3016 1970-01-01 00:00:00.000000 transmission_rpc-4.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1127 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/LICENSE
+-rw-r--r--   0        0        0     1630 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/README.md
+-rw-r--r--   0        0        0     3147 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1982 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/transmission_rpc/__init__.py
+-rw-r--r--   0        0        0    45188 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/transmission_rpc/client.py
+-rw-r--r--   0        0        0    11051 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/transmission_rpc/constants.py
+-rw-r--r--   0        0        0     1639 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/transmission_rpc/error.py
+-rw-r--r--   0        0        0    12990 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/transmission_rpc/session.py
+-rw-r--r--   0        0        0    23663 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/transmission_rpc/torrent.py
+-rw-r--r--   0        0        0     1497 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/transmission_rpc/types.py
+-rw-r--r--   0        0        0     2669 2023-04-09 09:37:20.250403 transmission_rpc-4.2.0/transmission_rpc/utils.py
+-rw-r--r--   0        0        0     3016 1970-01-01 00:00:00.000000 transmission_rpc-4.2.0/PKG-INFO
```

### Comparing `transmission_rpc-4.1.5/LICENSE` & `transmission_rpc-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.1.5/README.md` & `transmission_rpc-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.1.5/pyproject.toml` & `transmission_rpc-4.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "transmission-rpc"
-version = "4.1.5"
+version = "4.2.0"
 description = "Python module that implements the Transmission bittorent client JSON-RPC protocol"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'README.md'
 repository = 'https://github.com/Trim21/transmission-rpc'
 license = 'MIT'
 packages = [{ include = 'transmission_rpc' }]
 keywords = ['transmission', 'rpc']
```

### Comparing `transmission_rpc-4.1.5/transmission_rpc/__init__.py` & `transmission_rpc-4.2.0/transmission_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.1.5/transmission_rpc/client.py` & `transmission_rpc-4.2.0/transmission_rpc/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,22 +225,36 @@
 
         try:
             data: ResponseData = json.loads(http_data)
         except ValueError as error:
             self.logger.error("Error: %s", str(error))
             self.logger.error('Request: "%s"', query)
             self.logger.error('HTTP data: "%s"', http_data)
-            raise TransmissionError("failed to parse response as json") from error
+            raise TransmissionError(
+                "failed to parse response as json", method=method, argument=arguments, rawResponse=http_data
+            ) from error
 
         self.logger.debug(json.dumps(data, indent=2))
         if "result" not in data:
-            raise TransmissionError("Query failed, response data missing without result.")
+            raise TransmissionError(
+                "Query failed, response data missing without result.",
+                method=method,
+                argument=arguments,
+                response=data,
+                rawResponse=http_data,
+            )
 
         if data["result"] != "success":
-            raise TransmissionError(f'Query failed with result "{data["result"]}".')
+            raise TransmissionError(
+                f'Query failed with result "{data["result"]}".',
+                method=method,
+                argument=arguments,
+                response=data,
+                rawResponse=http_data,
+            )
 
         res = data["arguments"]
 
         results = {}
         if method == RpcMethod.TorrentGet:
             return res
         elif method == RpcMethod.TorrentAdd:
@@ -248,15 +262,21 @@
             if "torrent-added" in res:
                 item = res["torrent-added"]
             elif "torrent-duplicate" in res:
                 item = res["torrent-duplicate"]
             if item:
                 results[item["id"]] = Torrent(fields=item)
             else:
-                raise TransmissionError("Invalid torrent-add response.")
+                raise TransmissionError(
+                    "Invalid torrent-add response.",
+                    method=method,
+                    argument=arguments,
+                    response=data,
+                    rawResponse=http_data,
+                )
         elif method == RpcMethod.SessionGet:
             self.raw_session.update(res)
         elif method == RpcMethod.SessionStats:
             # older versions of T has the return data in "session-stats"
             if "session-stats" in res:
                 return res["session-stats"]
             else:
```

### Comparing `transmission_rpc-4.1.5/transmission_rpc/constants.py` & `transmission_rpc-4.2.0/transmission_rpc/constants.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.1.5/transmission_rpc/session.py` & `transmission_rpc-4.2.0/transmission_rpc/session.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.1.5/transmission_rpc/torrent.py` & `transmission_rpc-4.2.0/transmission_rpc/torrent.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.1.5/transmission_rpc/types.py` & `transmission_rpc-4.2.0/transmission_rpc/types.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.1.5/transmission_rpc/utils.py` & `transmission_rpc-4.2.0/transmission_rpc/utils.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.1.5/PKG-INFO` & `transmission_rpc-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transmission-rpc
-Version: 4.1.5
+Version: 4.2.0
 Summary: Python module that implements the Transmission bittorent client JSON-RPC protocol
 Home-page: https://github.com/Trim21/transmission-rpc
 License: MIT
 Keywords: transmission,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.7,<4.0
```

