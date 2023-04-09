# Comparing `tmp/pyC8-0.9.6.tar.gz` & `tmp/pyC8-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyC8-0.9.6.tar", last modified: Mon Oct 29 17:52:04 2018, max compression
+gzip compressed data, was "pyC8-1.0.0.tar", last modified: Sun Apr  9 10:08:34 2023, max compression
```

## Comparing `pyC8-0.9.6.tar` & `pyC8-1.0.0.tar`

### file list

```diff
@@ -1,34 +1,52 @@
-drwxrwxr-x   0 velotio   (1000) velotio   (1000)        0 2018-10-29 17:52:04.000000 pyC8-0.9.6/
--rw-rw-r--   0 velotio   (1000) velotio   (1000)       39 2018-10-29 17:50:49.000000 pyC8-0.9.6/MANIFEST.in
--rw-rw-r--   0 velotio   (1000) velotio   (1000)     9654 2018-10-29 17:50:49.000000 pyC8-0.9.6/README.md
-drwxrwxr-x   0 velotio   (1000) velotio   (1000)        0 2018-10-29 17:52:04.000000 pyC8-0.9.6/c8/
--rw-rw-r--   0 velotio   (1000) velotio   (1000)    15821 2018-10-29 17:50:49.000000 pyC8-0.9.6/c8/c8ql.py
--rw-rw-r--   0 velotio   (1000) velotio   (1000)      133 2018-10-29 17:50:49.000000 pyC8-0.9.6/c8/__init__.py
--rw-rw-r--   0 velotio   (1000) velotio   (1000)     1989 2018-10-29 17:50:49.000000 pyC8-0.9.6/c8/utils.py
--rw-rw-r--   0 velotio   (1000) velotio   (1000)    14142 2018-10-29 17:50:49.000000 pyC8-0.9.6/c8/executor.py
--rw-rw-r--   0 velotio   (1000) velotio   (1000)    38278 2018-10-29 17:50:49.000000 pyC8-0.9.6/c8/stream_collection.py
--rw-rw-r--   0 velotio   (1000) velotio   (1000)     2622 2018-10-29 17:50:49.000000 pyC8-0.9.6/c8/api.py
--rw-rw-r--   0 velotio   (1000) velotio   (1000)     9457 2018-10-29 17:50:49.000000 pyC8-0.9.6/c8/job.py
--rw-rw-r--   0 velotio   (1000) velotio   (1000)    64353 2018-10-29 17:50:49.000000 pyC8-0.9.6/c8/database.py
--rw-rw-r--   0 velotio   (1000) velotio   (1000)    23745 2018-10-29 17:50:49.000000 pyC8-0.9.6/c8/tenant.py
--rw-rw-r--   0 velotio   (1000) velotio   (1000)     4032 2018-10-29 17:50:49.000000 pyC8-0.9.6/c8/request.py
--rw-rw-r--   0 velotio   (1000) velotio   (1000)     1560 2018-10-29 17:50:49.000000 pyC8-0.9.6/c8/constants.py
--rw-rw-r--   0 velotio   (1000) velotio   (1000)     7734 2018-10-29 17:50:49.000000 pyC8-0.9.6/c8/connection.py
--rw-rw-r--   0 velotio   (1000) velotio   (1000)    12781 2018-10-29 17:50:49.000000 pyC8-0.9.6/c8/exceptions.py
--rw-rw-r--   0 velotio   (1000) velotio   (1000)   103002 2018-10-29 17:50:49.000000 pyC8-0.9.6/c8/collection.py
--rw-rw-r--   0 velotio   (1000) velotio   (1000)       22 2018-10-29 17:50:49.000000 pyC8-0.9.6/c8/version.py
--rw-rw-r--   0 velotio   (1000) velotio   (1000)     2699 2018-10-29 17:50:49.000000 pyC8-0.9.6/c8/http.py
--rw-rw-r--   0 velotio   (1000) velotio   (1000)     2684 2018-10-29 17:50:49.000000 pyC8-0.9.6/c8/response.py
--rw-rw-r--   0 velotio   (1000) velotio   (1000)     4889 2018-10-29 17:50:49.000000 pyC8-0.9.6/c8/client.py
--rw-rw-r--   0 velotio   (1000) velotio   (1000)     8289 2018-10-29 17:50:49.000000 pyC8-0.9.6/c8/cursor.py
--rw-rw-r--   0 velotio   (1000) velotio   (1000)    34106 2018-10-29 17:50:49.000000 pyC8-0.9.6/c8/graph.py
--rw-rw-r--   0 velotio   (1000) velotio   (1000)     1010 2018-10-29 17:50:49.000000 pyC8-0.9.6/setup.py
--rw-rw-r--   0 velotio   (1000) velotio   (1000)       67 2018-10-29 17:52:04.000000 pyC8-0.9.6/setup.cfg
--rw-rw-r--   0 velotio   (1000) velotio   (1000)    12563 2018-10-29 17:52:04.000000 pyC8-0.9.6/PKG-INFO
-drwxrwxr-x   0 velotio   (1000) velotio   (1000)        0 2018-10-29 17:52:04.000000 pyC8-0.9.6/pyC8.egg-info/
--rw-rw-r--   0 velotio   (1000) velotio   (1000)       34 2018-10-29 17:52:03.000000 pyC8-0.9.6/pyC8.egg-info/requires.txt
--rw-rw-r--   0 velotio   (1000) velotio   (1000)        3 2018-10-29 17:52:03.000000 pyC8-0.9.6/pyC8.egg-info/top_level.txt
--rw-rw-r--   0 velotio   (1000) velotio   (1000)      471 2018-10-29 17:52:03.000000 pyC8-0.9.6/pyC8.egg-info/SOURCES.txt
--rw-rw-r--   0 velotio   (1000) velotio   (1000)        1 2018-10-29 17:52:03.000000 pyC8-0.9.6/pyC8.egg-info/dependency_links.txt
--rw-rw-r--   0 velotio   (1000) velotio   (1000)    12563 2018-10-29 17:52:03.000000 pyC8-0.9.6/pyC8.egg-info/PKG-INFO
--rw-rw-r--   0 velotio   (1000) velotio   (1000)    11357 2018-10-29 17:50:49.000000 pyC8-0.9.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:08:34.730556 pyC8-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 10:08:26.000000 pyC8-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-09 10:08:26.000000 pyC8-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-09 10:08:34.730556 pyC8-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-04-09 10:08:26.000000 pyC8-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:08:34.730556 pyC8-1.0.0/c8/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20267 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/apikeys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:08:34.730556 pyC8-1.0.0/c8/billing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/billing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/billing/billing_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/billing/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/c8ql.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114125 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87300 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8845 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20472 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54622 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/fabric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:08:34.730556 pyC8-1.0.0/c8/function/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/function/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/function/function_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27951 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9954 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/keyvalue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:08:34.730556 pyC8-1.0.0/c8/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/redis/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118971 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/redis/redis_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/redis/redis_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/stream_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24998 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/stream_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37091 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 10:08:26.000000 pyC8-1.0.0/c8/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 10:08:34.730556 pyC8-1.0.0/pyC8.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-09 10:08:34.000000 pyC8-1.0.0/pyC8.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-09 10:08:34.000000 pyC8-1.0.0/pyC8.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 10:08:34.000000 pyC8-1.0.0/pyC8.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-09 10:08:34.000000 pyC8-1.0.0/pyC8.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-09 10:08:34.000000 pyC8-1.0.0/pyC8.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-09 10:08:26.000000 pyC8-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-09 10:08:34.734556 pyC8-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-09 10:08:26.000000 pyC8-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyC8-0.9.6/c8/c8ql.py` & `pyC8-1.0.0/c8/c8ql.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from __future__ import absolute_import, unicode_literals
 
 from json import dumps
 
-__all__ = ['C8QL', 'C8QLQueryCache']
-
 from c8.api import APIWrapper
 from c8.cursor import Cursor
 from c8.exceptions import (
-    C8QLQueryExplainError,
-    C8QLQueryValidateError,
-    C8QLQueryExecuteError,
-    C8QLQueryListError,
+    C8QLGetAllBatchesError,
     C8QLQueryClearError,
+    C8QLQueryExecuteError,
+    C8QLQueryExplainError,
     C8QLQueryKillError,
-    C8QLFunctionCreateError,
-    C8QLFunctionDeleteError,
-    C8QLFunctionListError,
+    C8QLQueryListError,
+    C8QLQueryValidateError,
 )
 from c8.request import Request
+from c8.utils import clean_doc
+
+__all__ = ["C8QL"]
 
 
 class C8QL(APIWrapper):
     """C8QL (C8Db Query Language) API wrapper.
 
     :param connection: HTTP connection.
     :type connection: c8.connection.Connection
@@ -29,40 +28,42 @@
     :type executor: c8.executor.Executor
     """
 
     def __init__(self, connection, executor):
         super(C8QL, self).__init__(connection, executor)
 
     def __repr__(self):
-        return '<C8QL in {}>'.format(self._conn.db_name)
+        return "<C8QL in {}>".format(self._conn.fabric_name)
 
     # noinspection PyMethodMayBeStatic
     def _format_queries(self, body):
         """Format the list of queries.
 
         :param body: Response body.
         :type body: dict
         :return: Formatted body.
         :rtype: dict
         """
         for query in body:
-            if 'bindVars' in query:
-                query['bind_vars'] = query.pop('bindVars')
-            if 'runTime' in query:
-                query['runtime'] = query.pop('runTime')
+            if "bindVars" in query:
+                query["bind_vars"] = query.pop("bindVars")
+            if "runTime" in query:
+                query["runtime"] = query.pop("runTime")
         return body
 
     @property
     def cache(self):
         """Return the query cache API wrapper.
 
         :return: Query cache API wrapper.
         :rtype: c8.c8ql.C8QLQueryCache
         """
-        return C8QLQueryCache(self._conn, self._executor)
+        # TODO: Implement C8QLQueryCache
+        # return C8QLQueryCache(self._conn, self._executor)
+        pass
 
     def explain(self, query, all_plans=False, max_plans=None, opt_rules=None):
         """Inspect the query and return its metadata without executing it.
 
         :param query: Query to inspect.
         :type query: str | unicode
         :param all_plans: If set to True, all possible execution plans are
@@ -73,114 +74,100 @@
         :type max_plans: int
         :param opt_rules: List of optimizer rules.
         :type opt_rules: list
         :return: Execution plan, or plans if **all_plans** was set to True.
         :rtype: dict | list
         :raise c8.exceptions.C8QLQueryExplainError: If explain fails.
         """
-        options = {'allPlans': all_plans}
+        options = {"allPlans": all_plans}
         if max_plans is not None:
-            options['maxNumberOfPlans'] = max_plans
+            options["maxNumberOfPlans"] = max_plans
         if opt_rules is not None:
-            options['optimizer'] = {'rules': opt_rules}
+            options["optimizer"] = {"rules": opt_rules}
 
         request = Request(
-            method='post',
-            endpoint='/_api/explain',
-            data={'query': query, 'options': options}
+            method="post",
+            endpoint="/query/explain",
+            data={"query": query, "options": options},
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise C8QLQueryExplainError(resp, request)
-            if 'plan' in resp.body:
-                return resp.body['plan']
+            if "plan" in resp.body:
+                return resp.body["plan"]
             else:
-                return resp.body['plans']
+                return resp.body["plans"]
 
         return self._execute(request, response_handler)
 
     def validate(self, query):
         """Parse and validate the query without executing it.
 
         :param query: Query to validate.
         :type query: str | unicode
         :return: Query details.
         :rtype: dict
         :raise c8.exceptions.C8QLQueryValidateError: If validation fails.
         """
-        request = Request(
-            method='post',
-            endpoint='/_api/query',
-            data={'query': query}
-        )
+        request = Request(method="post", endpoint="/query", data={"query": query})
 
         def response_handler(resp):
             if not resp.is_success:
                 raise C8QLQueryValidateError(resp, request)
             body = resp.body
-            body.pop('code', None)
-            body.pop('error', None)
-            if 'bindVars' in body:
-                body['bind_vars'] = body.pop('bindVars')
+            body.pop("code", None)
+            body.pop("error", None)
+            if "bindVars" in body:
+                body["bind_vars"] = body.pop("bindVars")
             return body
 
         return self._execute(request, response_handler)
 
-    def execute(self,
-                query,
-                count=False,
-                batch_size=None,
-                ttl=None,
-                bind_vars=None,
-                full_count=None,
-                max_plans=None,
-                optimizer_rules=None,
-                cache=None,
-                memory_limit=0,
-                fail_on_warning=None,
-                profile=None,
-                max_transaction_size=None,
-                max_warning_count=None,
-                intermediate_commit_count=None,
-                intermediate_commit_size=None,
-                satellite_sync_wait=None,
-                read_collections=None,
-                write_collections=None):
+    def execute(
+        self,
+        query,
+        count=False,
+        batch_size=None,
+        ttl=None,
+        bind_vars=None,
+        full_count=None,
+        optimizer_rules=None,
+        fail_on_warning=None,
+        profile=None,
+        max_transaction_size=None,
+        max_warning_count=None,
+        intermediate_commit_count=None,
+        intermediate_commit_size=None,
+        skip_inaccessible_collections=None,
+        stream=None,
+        sql=False,
+    ):
         """Execute the query and return the result cursor.
 
         :param query: Query to execute.
         :type query: str | unicode
         :param count: If set to True, the total document count is included in
             the result cursor.
         :type count: bool
         :param batch_size: Number of documents fetched by the cursor in one
-            round trip.
+            round trip
         :type batch_size: int
         :param ttl: Server side time-to-live for the cursor in seconds.
         :type ttl: int
         :param bind_vars: Bind variables for the query.
         :type bind_vars: dict
         :param full_count: This parameter applies only to queries with LIMIT
             clauses. If set to True, the number of matched documents before
             the last LIMIT clause executed is included in teh cursor. This is
             similar to MySQL SQL_CALC_FOUND_ROWS hint. Using this disables a
             few LIMIT optimizations and may lead to a longer query execution.
         :type full_count: bool
-        :param max_plans: Max number of plans the optimizer generates.
-        :type max_plans: int
         :param optimizer_rules: List of optimizer rules.
         :type optimizer_rules: [str | unicode]
-        :param cache: If set to True, the query cache is used. The operation
-            mode of the query cache must be set to "on" or "demand".
-        :type cache: bool
-        :param memory_limit: Max amount of memory the query is allowed to use
-            in bytes. If the query goes over the limit, it fails with error
-            "resource limit exceeded". Value 0 indicates no limit.
-        :type memory_limit: int
         :param fail_on_warning: If set to True, the query throws an exception
             instead of producing a warning. This parameter can be used during
             development to catch issues early. If set to False, warnings are
             returned with the query result. There is a server configuration
             option "--query.fail-on-warning" for setting the default value for
             this behaviour so it does not need to be set per-query.
         :type fail_on_warning: bool
@@ -196,101 +183,95 @@
             which an intermediate commit is performed automatically. Applies
             only to RocksDB storage engine.
         :type intermediate_commit_count: int
         :param intermediate_commit_size: Max size of operations in bytes after
             which an intermediate commit is performed automatically. Applies
             only to RocksDB storage engine.
         :type intermediate_commit_size: int
-        :param satellite_sync_wait: Number of seconds in which the server must
-            synchronize the satellite collections involved in the query. When
-            the threshold is reached, the query is stopped. Applies only to
-            enterprise version of C8Db.
-        :type satellite_sync_wait: int | float
-        :param read_collections: Names of collections read during query
-            execution. Required for :doc:`transactions <transaction>`.
-        :type read_collections: [str | unicode]
-        :param write_collections: Names of collections written to during query
-            execution. Required for :doc:`transactions <transaction>`.
-        :type write_collections: [str | unicode]
+        :param skip_inaccessible_collections: C8QL queries (especially graph
+            traversals) treat collections to which a user has no access rights
+            as if these collections were empty. Instead of returning a forbidden
+            access error, your query runs normally.
+        :type skip_inaccessible_collections: bool
+        :param stream: Specify *true* and the query runs as a **stream**.
+            The query result is not stored on server, but calculated on the fly.
+        :type stream: bool
+        :param sql: Specify *true* and write sql query.
+        :type sql: bool
         :return: Result cursor.
         :rtype: c8.cursor.Cursor
         :raise c8.exceptions.C8QLQueryExecuteError: If execute fails.
         """
-        data = {'query': query, 'count': count}
+        data = {"query": query, "count": count}
         if batch_size is not None:
-            data['batchSize'] = batch_size
+            data["batchSize"] = batch_size
         if ttl is not None:
-            data['ttl'] = ttl
+            data["ttl"] = ttl
         if bind_vars is not None:
-            data['bindVars'] = bind_vars
-        if cache is not None:
-            data['cache'] = cache
-        if memory_limit is not None:
-            data['memoryLimit'] = memory_limit
+            data["bindVars"] = bind_vars
 
         options = {}
         if full_count is not None:
-            options['fullCount'] = full_count
-        if max_plans is not None:
-            options['maxNumberOfPlans'] = max_plans
+            options["fullCount"] = full_count
         if optimizer_rules is not None:
-            options['optimizer'] = {'rules': optimizer_rules}
+            options["optimizer"] = {"rules": optimizer_rules}
         if fail_on_warning is not None:
-            options['failOnWarning'] = fail_on_warning
+            options["failOnWarning"] = fail_on_warning
         if profile is not None:
-            options['profile'] = profile
+            options["profile"] = profile
         if max_transaction_size is not None:
-            options['maxTransactionSize'] = max_transaction_size
+            options["maxTransactionSize"] = max_transaction_size
         if max_warning_count is not None:
-            options['maxWarningCount'] = max_warning_count
+            options["maxWarningCount"] = max_warning_count
         if intermediate_commit_count is not None:
-            options['intermediateCommitCount'] = intermediate_commit_count
+            options["intermediateCommitCount"] = intermediate_commit_count
         if intermediate_commit_size is not None:
-            options['intermediateCommitSize'] = intermediate_commit_size
-        if satellite_sync_wait is not None:
-            options['satelliteSyncWait'] = satellite_sync_wait
+            options["intermediateCommitSize"] = intermediate_commit_size
+        if skip_inaccessible_collections is not None:
+            options["skipInaccessibleCollections"] = skip_inaccessible_collections
+        if stream is not None:
+            options["stream"] = stream
         if options:
-            data['options'] = options
+            data["options"] = options
         data.update(options)
 
-        command = 'db._query({}, {}, {}).toArray()'.format(
-            dumps(query),
-            dumps(bind_vars),
-            dumps(data),
-        ) if self._is_transaction else None
-
-        request = Request(
-            method='post',
-            endpoint='/_api/cursor',
-            data=data,
-            command=command,
-            read=read_collections,
-            write=write_collections
+        command = (
+            "db._query({}, {}, {}).toArray()".format(
+                dumps(query),
+                dumps(bind_vars),
+                dumps(data),
+            )
+            if self._is_transaction
+            else None
         )
 
+        if sql:
+            end_point = "/cursor/sql"
+        else:
+            end_point = "/cursor"
+
+        request = Request(method="post", endpoint=end_point, data=data, command=command)
+
         def response_handler(resp):
             if not resp.is_success:
                 raise C8QLQueryExecuteError(resp, request)
             return Cursor(self._conn, resp.body)
 
         return self._execute(request, response_handler)
 
     def kill(self, query_id):
         """Kill a running query.
 
         :param query_id: Query ID.
         :type query_id: str | unicode
         :return: True if kill request was sent successfully.
         :rtype: bool
-        :raise c8.exceptions.C8QLQueryKillError: If the send fails.
+        :raise c8.exceptions.C8QLQueryKillError: If send fails.
         """
-        request = Request(
-            method='delete',
-            endpoint='/_api/query/{}'.format(query_id)
-        )
+        request = Request(method="delete", endpoint="/query/{}".format(query_id))
 
         def response_handler(resp):
             if not resp.is_success:
                 raise C8QLQueryKillError(resp, request)
             return True
 
         return self._execute(request, response_handler)
@@ -298,18 +279,15 @@
     def queries(self):
         """Return the currently running C8QL queries.
 
         :return: Running C8QL queries.
         :rtype: [dict]
         :raise c8.exceptions.C8QLQueryListError: If retrieval fails.
         """
-        request = Request(
-            method='get',
-            endpoint='/_api/query/current'
-        )
+        request = Request(method="get", endpoint="/query/current")
 
         def response_handler(resp):
             if not resp.is_success:
                 raise C8QLQueryListError(resp, request)
             return self._format_queries(resp.body)
 
         return self._execute(request, response_handler)
@@ -317,18 +295,15 @@
     def slow_queries(self):
         """Return a list of all slow C8QL queries.
 
         :return: Slow C8QL queries.
         :rtype: [dict]
         :raise c8.exceptions.C8QLQueryListError: If retrieval fails.
         """
-        request = Request(
-            method='get',
-            endpoint='/_api/query/slow'
-        )
+        request = Request(method="get", endpoint="/query/slow")
 
         def response_handler(resp):
             if not resp.is_success:
                 raise C8QLQueryListError(resp, request)
             return self._format_queries(resp.body)
 
         return self._execute(request, response_handler)
@@ -336,97 +311,73 @@
     def clear_slow_queries(self):
         """Clear slow C8QL queries.
 
         :return: True if slow queries were cleared successfully.
         :rtype: bool
         :raise c8.exceptions.C8QLQueryClearError: If operation fails.
         """
-        request = Request(
-            method='delete',
-            endpoint='/_api/query/slow'
-        )
+        request = Request(method="delete", endpoint="/query/slow")
 
         def response_handler(resp):
             if not resp.is_success:
                 raise C8QLQueryClearError(resp, request)
             return True
 
         return self._execute(request, response_handler)
 
-    def functions(self):
-        """List the C8QL functions defined in the database.
-
-        :return: Mapping of C8QL function names to their javascript code.
+    def export_data_query(self, query, bind_vars):
+        """Run the query and return list of result documents. Query cannot contain
+         the following keywords: INSERT, UPDATE, REPLACE, REMOVE and UPSERT.
+
+        :param query: C8QL query to execute
+        :type query: str
+        :param bind_vars: C8QL supports the usage of bind parameters, thus allowing to
+         separate the query text from literal values used in the query.
+        :type bind_vars: dict
+        :returns: Documents in the collection according to the query logic.
         :rtype: dict
-        :raise c8.exceptions.C8QLFunctionListError: If retrieval fails.
+        :raise c8.exceptions.C8QLQueryExecuteError: If export fails.
         """
-        request = Request(
-            method='get',
-            endpoint='/_api/c8qlfunction'
-        )
+        data = {"query": query}
+        if bind_vars is not None:
+            data["bindVars"] = bind_vars
+        request = Request(method="POST", endpoint="/export", data=data)
 
         def response_handler(resp):
             if not resp.is_success:
-                raise C8QLFunctionListError(resp, request)
-            body = resp.body or {}
-            return {func['name']: func['code'] for func in map(dict, body)}
+                raise C8QLQueryExecuteError(resp, request)
+            return resp.body
 
         return self._execute(request, response_handler)
 
-    def create_function(self, name, code):
-        """Create a new C8QL function.
-
-        :param name: C8QL function name.
-        :type name: str | unicode
-        :param code: Function definition in Javascript.
-        :type code: str | unicode
-        :return: True if C8QL function was created successfully.
-        :rtype: bool
-        :raise c8.exceptions.C8QLFunctionCreateError: If create fails.
-        """
-        request = Request(
-            method='post',
-            endpoint='/_api/c8qlfunction',
-            data={'name': name, 'code': code}
-        )
-
-        def response_handler(resp):
-            if not resp.is_success:
-                raise C8QLFunctionCreateError(resp, request)
-            return True
+    def get_all_batches(self, query, bind_vars=None, batch_size=1000):
+        """Returns all batches for a query. It should only be used for Read operations. Query cannot contain
+         the following keywords: INSERT, UPDATE, REPLACE, REMOVE and UPSERT.
 
-        return self._execute(request, response_handler)
+         Note: Please make sure there is more than enough memory available on your system (RAM + Swap(if swap is enabled))
+         to be able fetch total size of the documents to be returned. This will help avoid any Out-Of-Memory problems.
 
-    def delete_function(self, name, group=False, ignore_missing=False):
-        """Delete a C8QL function.
+        :param query: Query to execute
+        :type query: str
+        :param bind_vars: Bind variables for the query.
+        :type bind_vars: dict
+        :param batch_size: Batch size is a configurable number. Results are retieved by continuously
+            calling the next batch of cursor of size batch_size
+        :type batch_size: int
+        :returns: Documents, or None if not found.
+        :rtype: dict | None
+        :raise c8.exceptions.C8QLQueryExecuteError: If retrieval fails.
+        """
+        write_ops = ["INSERT", "UPDATE", "REPLACE", "REMOVE", "UPSERT"]
+        if any(ele in query.upper() for ele in write_ops):
+            raise C8QLGetAllBatchesError(
+                "Write operations provided in the query. Only read operations can be provided"
+            )
 
-        :param name: C8QL function name.
-        :type name: str | unicode
-        :param group: If set to True, value of parameter **name** is treated
-            as a namespace prefix, and all functions in the namespace are
-            deleted. If set to False, the value of **name** must be a fully
-            qualified function name including any namespaces.
-        :type group: bool
-        :param ignore_missing: Do not raise an exception on missing function.
-        :type ignore_missing: bool
-        :return: True if C8QL function was deleted successfully, False if
-            function was not found and **ignore_missing** was set to True.
-        :rtype: bool
-        :raise c8.exceptions.C8QLFunctionDeleteError: If delete fails.
-        """
-        request = Request(
-            method='delete',
-            endpoint='/_api/c8qlfunction/{}'.format(name),
-            params={'group': group}
+        cursor = self.execute(
+            query=query, bind_vars=bind_vars, batch_size=batch_size, stream=True
         )
+        while cursor.has_more():
+            cursor.fetch()
 
-        def response_handler(resp):
-            if resp.error_code == 1582 and ignore_missing:
-                return False
-            if not resp.is_success:
-                raise C8QLFunctionDeleteError(resp, request)
-            return True
-
-        return self._execute(request, response_handler)
-
-
-
+        result = clean_doc(cursor.batch())
+        return result
```

### Comparing `pyC8-0.9.6/c8/api.py` & `pyC8-1.0.0/c8/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,41 @@
-from __future__ import absolute_import, unicode_literals
-
-__all__ = ['APIWrapper']
+__all__ = ["APIWrapper"]
 
 
 class APIWrapper(object):
     """Base class for API wrappers.
 
     :param connection: HTTP connection.
     :type connection: c8.connection.Connection
     :param executor: API executor.
     :type executor: c8.executor.Executor
     """
 
     def __init__(self, connection, executor):
         self._conn = connection
         self._executor = executor
-        self._is_transaction = self.context == 'transaction'
+        self._is_transaction = self.context == "transaction"
 
     @property
     def tenant_name(self):
         """Return the name of the current tenant.
 
         :return: tenant name.
         :rtype: str | unicode
         """
         return self._conn.tenant_name
 
     @property
-    def db_name(self):
-        """Return the name of the current database.
+    def fabric_name(self):
+        """Return the name of the current fabric.
 
-        :return: Database name.
+        :return: Fabric name.
         :rtype: str | unicode
         """
-        return self._conn.db_name
+        return self._conn.fabric_name
 
     @property
     def stream_name(self):
         """Return the name of the current stream.
 
         :return: Stream name.
         :rtype: str | unicode
@@ -59,23 +57,14 @@
 
         :return: topic persistence.
         :rtype: bool
         """
         return self._conn.topic_persistence
 
     @property
-    def fn_name(self):
-        """Return the name of the current function.
-
-        :return: Database name.
-        :rtype: str | unicode
-        """
-        return self._conn.fn_name
-
-    @property
     def username(self):
         """Return the username.
 
         :returns: Username.
         :rtype: str | unicode
         """
         return self._conn.username
@@ -86,18 +75,20 @@
 
         :return: API execution context. Possible values are "default", "async",
             "batch" and "transaction".
         :rtype: str | unicode
         """
         return self._executor.context
 
-    def _execute(self, request, response_handler):
+    def _execute(self, request, response_handler, custom_prefix=None):
         """Execute an API per execution context.
 
         :param request: HTTP request.
         :type request: c8.request.Request
         :param response_handler: HTTP response handler.
         :type response_handler: callable
         :return: API execution result.
         :rtype: str | unicode | bool | int | list | dict
         """
-        return self._executor.execute(request, response_handler)
+        return self._executor.execute(
+            request, response_handler, custom_prefix=custom_prefix
+        )
```

### Comparing `pyC8-0.9.6/c8/job.py` & `pyC8-1.0.0/c8/job.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import absolute_import, unicode_literals
 
 from uuid import uuid4
 
 from c8.exceptions import (
     AsyncJobCancelError,
-    AsyncJobStatusError,
-    AsyncJobResultError,
     AsyncJobClearError,
+    AsyncJobResultError,
+    AsyncJobStatusError,
     BatchJobResultError,
-    TransactionJobResultError,
 )
 from c8.request import Request
 
 
 class Job(object):  # pragma: no cover
     """Base class for API execution jobs.
 
@@ -53,23 +52,23 @@
     :type connection: c8.connection.Connection
     :param job_id: Async job ID.
     :type job_id: str | unicode
     :param response_handler: HTTP response handler.
     :type response_handler: callable
     """
 
-    __slots__ = ['_conn', '_id', '_response_handler']
+    __slots__ = ["_conn", "_id", "_response_handler"]
 
     def __init__(self, connection, job_id, response_handler):
         self._conn = connection
         self._id = job_id
         self._response_handler = response_handler
 
     def __repr__(self):
-        return '<AsyncJob {}>'.format(self._id)
+        return "<AsyncJob {}>".format(self._id)
 
     @property
     def id(self):
         """Return the async job ID.
 
         :return: Async job ID.
         :rtype: str | unicode
@@ -85,25 +84,22 @@
 
         :return: Async job status. Possible values are "pending" (job is still
             in queue), "done" (job finished or raised an error), or "cancelled"
             (job was cancelled before completion).
         :rtype: str | unicode
         :raise c8.exceptions.AsyncJobStatusError: If retrieval fails.
         """
-        request = Request(
-            method='get',
-            endpoint='/_api/job/{}'.format(self._id)
-        )
+        request = Request(method="get", endpoint="/job/{}".format(self._id))
         resp = self._conn.send_request(request)
         if resp.status_code == 204:
-            return 'pending'
+            return "pending"
         elif resp.is_success:
-            return 'done'
+            return "done"
         elif resp.error_code == 404:
-            error_message = 'job {} not found'.format(self._id)
+            error_message = "job {} not found".format(self._id)
             raise AsyncJobStatusError(resp, request, error_message)
         else:
             raise AsyncJobStatusError(resp, request)
 
     def result(self):
         """Return the async job result from server.
 
@@ -113,27 +109,24 @@
         queries for result will fail.
 
         :return: Async job result.
         :rtype: str | unicode | bool | int | list | dict
         :raise c8.exceptions.C8Error: If the job raised an exception.
         :raise c8.exceptions.AsyncJobResultError: If retrieval fails.
         """
-        request = Request(
-            method='put',
-            endpoint='/_api/job/{}'.format(self._id)
-        )
+        request = Request(method="put", endpoint="/job/{}".format(self._id))
         resp = self._conn.send_request(request)
         headers = resp.headers
-        if 'X-C8-Async-Id' in headers or 'x-c8-async-id' in headers:
+        if "X-C8-Async-Id" in headers or "x-c8-async-id" in headers:
             return self._response_handler(resp)
         if resp.status_code == 204:
-            error_message = 'job {} not done'.format(self._id)
+            error_message = "job {} not done".format(self._id)
             raise AsyncJobResultError(resp, request, error_message)
         elif resp.error_code == 404:
-            error_message = 'job {} not found'.format(self._id)
+            error_message = "job {} not found".format(self._id)
             raise AsyncJobResultError(resp, request, error_message)
         else:
             raise AsyncJobResultError(resp, request)
 
     def cancel(self, ignore_missing=False):
         """Cancel the async job.
 
@@ -142,72 +135,66 @@
         :param ignore_missing: Do not raise an exception on missing job.
         :type ignore_missing: bool
         :return: True if job was cancelled successfully, False if the job
             was not found but **ignore_missing** was set to True.
         :rtype: bool
         :raise c8.exceptions.AsyncJobCancelError: If cancel fails.
         """
-        request = Request(
-            method='put',
-            endpoint='/_api/job/{}/cancel'.format(self._id)
-        )
+        request = Request(method="put", endpoint="/job/{}/cancel".format(self._id))
         resp = self._conn.send_request(request)
         if resp.status_code == 200:
             return True
         elif resp.error_code == 404:
             if ignore_missing:
                 return False
-            error_message = 'job {} not found'.format(self._id)
+            error_message = "job {} not found".format(self._id)
             raise AsyncJobCancelError(resp, request, error_message)
         else:
             raise AsyncJobCancelError(resp, request)
 
     def clear(self, ignore_missing=False):
         """Delete the job result from the server.
 
         :param ignore_missing: Do not raise an exception on missing job.
         :type ignore_missing: bool
         :return: True if result was deleted successfully, False if the job
             was not found but **ignore_missing** was set to True.
         :rtype: bool
         :raise c8.exceptions.AsyncJobClearError: If delete fails.
         """
-        request = Request(
-            method='delete',
-            endpoint='/_api/job/{}'.format(self._id)
-        )
+        request = Request(method="delete", endpoint="/job/{}".format(self._id))
         resp = self._conn.send_request(request)
         if resp.is_success:
             return True
         elif resp.error_code == 404:
             if ignore_missing:
                 return False
-            error_message = 'job {} not found'.format(self._id)
+            error_message = "job {} not found".format(self._id)
             raise AsyncJobClearError(resp, request, error_message)
         else:
             raise AsyncJobClearError(resp, request)
 
 
 class BatchJob(Job):
     """Job for tracking and retrieving result of batch execution.
 
     :param response_handler: HTTP response handler.
     :type response_handler: callable
     """
 
-    __slots__ = ['_id', '_status', '_response', '_response_handler']
+    __slots__ = ["_id", "_status", "_response", "_response_handler"]
 
     def __init__(self, response_handler):
         self._id = uuid4().hex
-        self._status = 'pending'
+        self._status = "pending"
         self._response = None
         self._response_handler = response_handler
 
     def __repr__(self):
-        return '<BatchJob {}>'.format(self._id)
+        return "<BatchJob {}>".format(self._id)
 
     @property
     def id(self):
         """Return the batch job ID.
 
         :return: Batch job ID.
         :rtype: str | unicode
@@ -231,62 +218,10 @@
 
         :return: Batch job result.
         :rtype: str | unicode | bool | int | list | dict
         :raise c8.exceptions.C8Error: If the job raised an exception.
         :raise c8.exceptions.BatchJobResultError: If job result is not
             available (i.e. batch is not committed yet).
         """
-        if self._status == 'pending':
-            raise BatchJobResultError('result not available yet')
-        return self._response_handler(self._response)
-
-
-class TransactionJob(Job):
-    """Transaction API execution job.
-
-    :param response_handler: HTTP response handler.
-    :type response_handler: callable
-    """
-
-    __slots__ = ['_id', '_status', '_response', '_response_handler']
-
-    def __init__(self, response_handler):
-        self._id = uuid4().hex
-        self._status = 'pending'
-        self._response = None
-        self._response_handler = response_handler
-
-    def __repr__(self):
-        return '<TransactionJob {}>'.format(self._id)
-
-    @property
-    def id(self):
-        """Return the transaction job ID.
-
-        :return: Transaction job ID.
-        :rtype: str | unicode
-        """
-        return self._id
-
-    def status(self):
-        """Return the transaction job status.
-
-        :return: Transaction job status. Possible values are "pending" (job is
-            waiting for transaction to be committed, or transaction failed and
-            job is orphaned), or "done" (transaction was committed and job is
-            updated with the result).
-        :rtype: str | unicode
-        """
-        return self._status
-
-    def result(self):
-        """Return the transaction job result.
-
-        :return: Transaction job result.
-        :rtype: str | unicode | bool | int | list | dict
-        :raise c8.exceptions.C8Error: If the job raised an exception.
-        :raise c8.exceptions.TransactionJobResultError: If job result is
-            not available (i.e. transaction is not committed yet or failed).
-        """
-        if self._status == 'pending':
-            raise TransactionJobResultError('result not available yet')
+        if self._status == "pending":
+            raise BatchJobResultError("result not available yet")
         return self._response_handler(self._response)
```

### Comparing `pyC8-0.9.6/c8/database.py` & `pyC8-1.0.0/c8/fabric.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,590 +1,656 @@
 from __future__ import absolute_import, unicode_literals
 
-from c8.utils import get_col_name
+import base64
 import json
+import random
 
-__all__ = [
-    'StandardDatabase',
-    'AsyncDatabase',
-    'BatchDatabase',
-    'TransactionDatabase'
-]
-
-from datetime import datetime
+import websocket
 
+from c8 import constants
 from c8.api import APIWrapper
+from c8.apikeys import APIKeys
 from c8.c8ql import C8QL
-from c8 import constants
-from c8.executor import (
-    DefaultExecutor,
-    AsyncExecutor,
-    BatchExecutor,
-    TransactionExecutor,
-)
 from c8.collection import StandardCollection
-from c8.stream_collection import StreamCollection
 from c8.exceptions import (
-    AsyncJobClearError,
-    AsyncJobListError,
     CollectionCreateError,
     CollectionDeleteError,
+    CollectionFindError,
     CollectionListError,
-    DatabaseDeleteError,
-    DatabaseCreateError,
-    DatabaseListError,
-    DatabasePropertiesError,
-    GraphListError,
+    CollectionPropertiesError,
+    EventCreateError,
+    EventGetError,
+    FabricCreateError,
+    FabricDeleteError,
+    FabricGetMetadataError,
+    FabricListError,
+    FabricPropertiesError,
+    FabricSetMetadataError,
+    FabricUpdateMetadataError,
+    GetAPIKeys,
+    GetDcDetailError,
+    GetDcListError,
+    GetLocalDcError,
     GraphCreateError,
     GraphDeleteError,
+    GraphListError,
+    RestqlCreateError,
+    RestqlCursorError,
+    RestqlDeleteError,
+    RestqlExecuteError,
+    RestqlImportError,
+    RestqlListError,
+    RestqlUpdateError,
+    RestqlValidationError,
     ServerConnectionError,
-    ServerDetailsError,
     ServerVersionError,
-    TransactionExecuteError,
-    TenantDcListError,
+    SpotRegionAssignError,
+    SpotRegionUpdateError,
+    StreamAppGetSampleError,
+    StreamCommunicationError,
+    StreamConnectionError,
+    StreamCreateError,
+    StreamDeleteError,
+    StreamListError,
+    StreamPermissionError,
 )
-from c8 import exceptions as ex
-
+from c8.executor import AsyncExecutor, BatchExecutor, DefaultExecutor
 from c8.graph import Graph
+from c8.keyvalue import KV
 from c8.request import Request
-import json
-import random
-import pulsar
-from urllib.parse import urlparse
+from c8.search import Search
+from c8.stream_apps import StreamApps
+from c8.stream_collection import StreamCollection
 
-def printdata(event):
-    """Prints the event.
+__all__ = [
+    "StandardFabric",
+    "AsyncFabric",
+    "BatchFabric",
+]
+ENDPOINT = "/streams"
 
-    :param event: real-time update.
-    :type event: str | unicode
-    """
-    print(event)
 
-class Database(APIWrapper):
-    """Base class for Database API wrappers.
+def raise_timeout(signum, frame):
+    raise TimeoutError
+
+
+class Fabric(APIWrapper):
+    """Base class for Fabric API wrappers.
 
     :param connection: HTTP connection.
     :type connection: c8.connection.Connection
     :param executor: API executor.
     :type executor: c8.executor.Executor
     """
 
+    def enum(**enums):
+        return type("Enum", (), enums)
+
+    SPOT_CREATION_TYPES = enum(
+        AUTOMATIC="automatic", NONE="none", SPOT_REGION="spot_region"
+    )
+
     def __init__(self, connection, executor):
-        self.url=connection.url
-        self.stream_port=connection.stream_port
-        self.pulsar_client=None
-        super(Database, self).__init__(connection, executor)
+        self.url = connection.url
+        self.header = connection.headers
+        self.stream_port = constants.STREAM_PORT
+        super(Fabric, self).__init__(connection, executor)
 
     def __getitem__(self, name):
         """Return the collection API wrapper.
 
         :param name: Collection name.
         :type name: str | unicode
-        :return: Collection API wrapper.
+        :returns: Collection API wrapper.
         :rtype: c8.collection.StandardCollection
         """
         return self.collection(name)
 
-    def _get_col_by_doc(self, document):
-        """Return the collection of the given document.
-
-        :param document: Document ID or body with "_id" field.
-        :type document: str | unicode | dict
-        :return: Collection API wrapper.
-        :rtype: c8.collection.StandardCollection
-        :raise c8.exceptions.DocumentParseError: On malformed document.
-        """
-        return self.collection(get_col_name(document))
-
     @property
     def name(self):
-        """Return database name.
+        """Return fabric name.
 
-        :return: Database name.
+        :returns: Fabric name.
         :rtype: str | unicode
         """
-        return self.db_name
+        return self.fabric_name
 
     @property
     def c8ql(self):
         """Return C8QL (C8Db Query Language) API wrapper.
 
-        :return: C8QL API wrapper.
+        :returns: C8QL API wrapper.
         :rtype: c8.c8ql.C8QL
         """
         return C8QL(self._conn, self._executor)
 
-    def on_change(self, collection, callback=printdata):
+    @property
+    def key_value(self):
+        """Return KV (Key Value) API wrapper.
+
+        :returns: KV API wrapper.
+        :rtype: c8.keyvalue.KV
+        """
+        return KV(self._conn, self._executor)
+
+    def on_change(self, collection, callback, timeout=60):
         """Execute given input function on receiving a change.
 
+        :param collection: Collection name(s) regex to listen for
+        :type collection: str
+        :param timeout: timeout value
+        :type timeout: int
         :param callback: Function to execute on a change
         :type callback: function
-        :param collections: Collection name or Collection names regex to listen for
-        :type collections: str
         """
-        if not collection: 
-            raise ValueError('You must specify a collection on which to watch for realtime data!')
+        if not callback:
+            raise ValueError("You must specify a callback function")
 
-        namespace = constants.STREAM_LOCAL_NS_PREFIX + self.tenant_name + '.' + self.db_name
-        if self.tenant_name == "_mm":
-            namespace = constants.STREAM_LOCAL_NS_PREFIX + self.db_name
-
-        topic = "non-persistent://" + self.tenant_name + "/" + namespace + "/" + collection
-        subscription_name = self.tenant_name + "-" + self.db_name + "-subscription-" + str(random.randint(1, 1000))
-        print("pyC8 Realtime: Subscribing to topic: "+ topic + " on Subscription name: "+subscription_name)
-    
-        if self.pulsar_client:
-            print("pyC8 Realtime: Initialized C8Streams connection to "+ self.url + ":" + str(self.stream_port))
-        else:
-            dcl_local = self.dclist_local()
-            self.pulsar_client = pulsar.Client('pulsar://' + constants.PLUSAR_URL_PREFIX + dcl_local['tags']['url'] + ":" + str(self.stream_port)) 
-        
-        consumer = self.pulsar_client.subscribe(topic, subscription_name)
+        if not collection:
+            raise ValueError(
+                "You must specify a collection on which realtime "
+                "data is to be watched!"
+            )
+
+        namespace = constants.STREAM_LOCAL_NS_PREFIX + self.fabric_name
+
+        subscription_name = "%s-%s-subscription-%s" % (
+            self.tenant_name,
+            self.fabric_name,
+            str(random.randint(1, 1000)),
+        )
+
+        url = self.url.split("//")[1].split(":")[0]
+
+        topic = "wss://{}/_ws/ws/v2/consumer/persistent/{}/{}/{}/{}".format(
+            url, self.tenant_name, namespace, collection, subscription_name
+        )
+
+        ws = websocket.create_connection(topic, header=self.header, timeout=timeout)
 
         try:
-            print("pyC8 Realtime: Begin monitoring realtime updates for "+topic)
+            # "pyC8 Realtime: Begin monitoring realtime updates for " + topic
             while True:
-                msg = consumer.receive()
-                data = msg.data().decode('utf-8')
-                jdata = json.loads(data)
-                #self.consumer.acknowledge(msg)
-                callback(jdata)
+                msg = json.loads(ws.recv())
+                data = base64.b64decode(msg["payload"])
+                ws.send(json.dumps({"messageId": msg["messageId"]}))
+                callback(data)
+        except websocket.WebSocketTimeoutException:
+            pass
+        except Exception as e:
+            raise Exception(e)
         finally:
-            self.pulsar_client.close()
+            ws.close()
 
     def properties(self):
-        """Return database properties.
+        """Return fabric properties.
 
-        :return: Database properties.
+        :returns: Fabric properties.
         :rtype: dict
-        :raise c8.exceptions.DatabasePropertiesError: If retrieval fails.
+        :raise c8.exceptions.FabricPropertiesError: If retrieval fails.
         """
         request = Request(
-            method='get',
-            endpoint='/_api/database/current',
+            method="get",
+            endpoint="/database/current",
         )
 
         def response_handler(resp):
             if not resp.is_success:
-                raise DatabasePropertiesError(resp, request)
-            result = resp.body['result']
-            result['system'] = result.pop('isSystem')
+                raise FabricPropertiesError(resp, request)
+            result = resp.body["result"]
+            result["system"] = result.pop("isSystem")
             return result
 
         return self._execute(request, response_handler)
 
-    def execute_transaction(self,
-                            command,
-                            params=None,
-                            read=None,
-                            write=None,
-                            sync=None,
-                            timeout=None,
-                            max_size=None,
-                            allow_implicit=None,
-                            intermediate_commit_count=None,
-                            intermediate_commit_size=None):
-        """Execute raw Javascript command in transaction.
-
-        :param command: Javascript command to execute.
-        :type command: str | unicode
-        :param read: Names of collections read during transaction. If parameter
-            **allow_implicit** is set to True, any undeclared read collections
-            are loaded lazily.
-        :type read: [str | unicode]
-        :param write: Names of collections written to during transaction.
-            Transaction fails on undeclared write collections.
-        :type write: [str | unicode]
-        :param params: Optional parameters passed into the Javascript command.
-        :type params: dict
-        :param sync: Block until operation is synchronized to disk.
-        :type sync: bool
-        :param timeout: Timeout for waiting on collection locks. If set to 0,
-            C8Db server waits indefinitely. If not set, system default
-            value is used.
-        :type timeout: int
-        :param max_size: Max transaction size limit in bytes. Applies only
-            to RocksDB storage engine.
-        :type max_size: int
-        :param allow_implicit: If set to True, undeclared read collections are
-            loaded lazily. If set to False, transaction fails on any undeclared
-            collections.
-        :type allow_implicit: bool
-        :param intermediate_commit_count: Max number of operations after which
-            an intermediate commit is performed automatically. Applies only to
-            RocksDB storage engine.
-        :type intermediate_commit_count: int
-        :param intermediate_commit_size: Max size of operations in bytes after
-            which an intermediate commit is performed automatically. Applies
-            only to RocksDB storage engine.
-        :type intermediate_commit_size: int
-        :return: Return value of **command**.
-        :rtype: str | unicode
-        :raise c8.exceptions.TransactionExecuteError: If execution fails.
+    def update_spot_region(self, tenant, fabric, new_dc):
+        """Updates spot primary region for the geo-fabric
+
+        :param tenant: tenant name
+        :type tenant: str
+        :param fabric: fabric name
+        :type fabric: str
+        :param new_dc: New spot region
+        :type new_dc: str
+        :returns: True if request successful,false otherwise
+        :rtype: bool
+        :raise c8.exceptions.SpotRegionUpdateError: If updation fails.
         """
-        collections = {'allowImplicit': allow_implicit}
-        if read is not None:
-            collections['read'] = read
-        if write is not None:
-            collections['write'] = write
-
-        data = {'action': command}
-        if collections:
-            data['collections'] = collections
-        if params is not None:
-            data['params'] = params
-        if timeout is not None:
-            data['lockTimeout'] = timeout
-        if sync is not None:
-            data['waitForSync'] = sync
-        if max_size is not None:
-            data['maxTransactionSize'] = max_size
-        if intermediate_commit_count is not None:
-            data['intermediateCommitCount'] = intermediate_commit_count
-        if intermediate_commit_size is not None:
-            data['intermediateCommitSize'] = intermediate_commit_size
 
         request = Request(
-            method='post',
-            endpoint='/_api/transaction',
-            data=data
+            method="put", endpoint="/_fabric/{}/database/{}".format(fabric, new_dc)
         )
 
         def response_handler(resp):
             if not resp.is_success:
-                raise TransactionExecuteError(resp, request)
-            return resp.body.get('result')
+                raise SpotRegionUpdateError(resp, request)
+            return True
 
         return self._execute(request, response_handler)
 
-    def version(self):
-        """Return C8Db server version.
-
-        :return: Server version.
-        :rtype: str | unicode
-        :raise c8.exceptions.ServerVersionError: If retrieval fails.
-        """
-        request = Request(
-            method='get',
-            endpoint='/_admin/version',
-            params={'details': False}
-        )
+    def fabrics_detail(self):
+        request = Request(method="get", endpoint="/database/user")
 
         def response_handler(resp):
             if not resp.is_success:
-                raise ServerVersionError(resp, request)
-            return resp.body['version']
+                raise FabricListError(resp, request)
+            return [
+                {"name": col["name"], "options": col["options"]}
+                for col in map(dict, resp.body["result"])
+            ]
 
         return self._execute(request, response_handler)
 
-    def details(self):
-        """Return C8Db server details.
+    def version(self):
+        """Return C8Db server version.
 
-        :return: Server details.
-        :rtype: dict
-        :raise c8.exceptions.ServerDetailsError: If retrieval fails.
+        :returns: Server version.
+        :rtype: str | unicode
+        :raise c8.exceptions.ServerVersionError: If retrieval fails.
         """
-        request = Request(
-            method='get',
-            endpoint='/_api/version',
-            params={'details': True}
-        )
+        request = Request(method="get", endpoint="/version", params={"details": False})
 
         def response_handler(resp):
             if not resp.is_success:
-                raise ServerDetailsError(resp, request)
-            return resp.body['details']
+                raise ServerVersionError(resp, request)
+            return resp.body["version"]
 
         return self._execute(request, response_handler)
 
     def ping(self):
         """Ping the C8Db server by sending a test request.
 
-        :return: Response code from server.
+        :returns: Response code from server.
         :rtype: int
         :raise c8.exceptions.ServerConnectionError: If ping fails.
         """
         request = Request(
-            method='get',
-            endpoint='/_api/collection',
+            method="get",
+            endpoint="/collection",
         )
 
         def response_handler(resp):
             code = resp.status_code
             if code in {401, 403}:
-                raise ServerConnectionError('bad username and/or password')
+                raise ServerConnectionError("bad username and/or password")
             if not resp.is_success:
-                raise ServerConnectionError(
-                    resp.error_message or 'bad server response')
+                raise ServerConnectionError(resp.error_message or "bad server response")
             return code
 
         return self._execute(request, response_handler)
 
     #########################
     # Datacenter Management #
     #########################
 
-    def dclist(self):
-        """Return the list of Datacenters
+    def dclist(self, detail=False):
+        """Return the list of names of Datacenters
 
-        :return: DC List.
+        :param detail: detail list of DCs if set to true else only DC names
+        :type: boolean
+        :returns: DC List.
         :rtype: [str | unicode ]
-        :raise c8.exceptions.TenantListError: If retrieval fails.
+        :raise c8.exceptions.GetDcListError: If retrieval fails.
         """
+        properties = self.properties()
+        if not detail:
+            return properties["options"]["dcList"].split(",")
+
+        tenant_name = properties["options"]["tenant"]
+
         request = Request(
-            method='get',
-            endpoint='/_api/datacenter/all'
+            method="get", endpoint="/datacenter/_tenant/{}".format(tenant_name)
         )
 
         def response_handler(resp):
-            #print("dclist() : Response body: " + str(resp.body))
             if not resp.is_success:
-                raise TenantDcListError(resp, request)
-            dc_list = []
-            for dc in resp.body:
-                dc_list.append(dc['name'])
+                raise GetDcListError(resp, request)
+            dc_list = resp.body[0]["dcInfo"]
+            for dc in dc_list:
+                if dc["name"] not in properties["options"]["dcList"]:
+                    dc_list.remove(dc)
             return dc_list
 
-        return self._execute(request, response_handler)
+        return self._execute(request, response_handler, custom_prefix="")
+
+    def localdc(self, detail=True):
+        """Fetch data for a local/regional the data center
+
+        :param detail: Details of local DC if set to true else only DC name.
+        :type: boolean
+        :returns: Local DC details.
+        :rtype: str | dict
+        :raise c8.exceptions.GetLocalDcError: If retrieval fails.
+        """
+        request = Request(method="get", endpoint="/datacenter/local")
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise GetLocalDcError(resp, request)
+            if detail:
+                return resp.body
+            return resp.body["name"]
+
+        return self._execute(request, response_handler, custom_prefix="")
+
+    def get_dc_detail(self, dc):
+        """Fetch data for data center, identified by dc-name
+
+        :param dc: DC name
+        :type: str
+        :returns: DC details.
+        :rtype: dict
+        :raise c8.exceptions.GetDcDetailError: If retrieval fails.
+        """
+        request = Request(method="get", endpoint="/datacenter/{}".format(dc))
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise GetDcDetailError(resp, request)
+            return resp.body
+
+        return self._execute(request, response_handler, custom_prefix="")
 
-    def dclist_local(self):
-        """Return the list of local Datacenters
+    def dclist_all(self):
+        """Fetch data about all the data centers
 
-        :return: DC List.
+        :returns: DC List.
         :rtype: [str | unicode ]
-        :raise c8.exceptions.TenantListError: If retrieval fails.
+        :raise c8.exceptions.GetDcListError: If retrieval fails.
         """
-        request = Request(
-            method='get',
-            endpoint='/_api/datacenter/local'
-        )
+
+        request = Request(method="get", endpoint="/datacenter/all")
 
         def response_handler(resp):
-            #print("dclist() : Response body: " + str(resp.body))
             if not resp.is_success:
-                raise TenantDcListError(resp, request)
+                raise GetDcListError(resp, request)
             return resp.body
 
-        return self._execute(request, response_handler)
+        return self._execute(request, response_handler, custom_prefix="")
+
+    def assign_dc_spot(self, dc, spot_region=False):
+        """Assigns spot region of a fed
+
+        :param dc: dc name
+        :type dc: str
+        :param spot_region: If True, makes the region a spot region
+        :type spot_region: bool
+        :returns: True if request successful, False otherwise
+        :rtype: bool
+        :raise c8.exceptions.SpotRegionAssignError: If assignment fails.
+        """
+        data = json.dumps(spot_region)
+        request = Request(method="put", endpoint="/datacenter/{}/{}".format(dc, data))
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise SpotRegionAssignError(resp, request)
+            return True
 
+        return self._execute(request, response_handler, custom_prefix="")
 
     #######################
-    # Database Management #
+    # Fabric Management #
     #######################
 
-    def databases(self):
-        """Return the names all databases.
+    def fabrics(self):
+        """Return the names all fabrics.
 
-        :return: Database names.
+        :returns: Fabric names.
         :rtype: [str | unicode]
-        :raise c8.exceptions.DatabaseListError: If retrieval fails.
+        :raise c8.exceptions.FabricListError: If retrieval fails.
         """
-        request = Request(
-            method='get',
-            endpoint='/_api/database'
-        )
+        request = Request(method="get", endpoint="/database")
 
         def response_handler(resp):
             if not resp.is_success:
-                raise DatabaseListError(resp, request)
-            return resp.body['result']
+                raise FabricListError(resp, request)
+            return resp.body["result"]
 
         return self._execute(request, response_handler)
 
-    def has_database(self, name):
-        """Check if a database exists.
+    def has_fabric(self, name):
+        """Check if a fabric exists.
 
-        :param name: Database name.
+        :param name: Fabric name.
         :type name: str | unicode
-        :return: True if database exists, False otherwise.
+        :returns: True if fabric exists, False otherwise.
         :rtype: bool
         """
-        return name in self.databases()
+        return name in self.fabrics()
 
-    def create_database(self, name, users=None, dclist=None, realtime=False):
-        """Create a new database.
+    def create_fabric(
+        self,
+        name,
+        spot_dc=None,
+        users=None,
+        dclist=None,
+        spot_creation_type=SPOT_CREATION_TYPES.AUTOMATIC,
+    ):
+        """Create a new fabric.
 
-        :param name: Database name.
+        :param name: Fabric name.
         :type name: str | unicode
-        :param users: List of users with access to the new database, where each
-            user is a dictionary with fields "username", "password", "active"
-            and "extra" (see below for example). If not set, only the admin and
-            current user are granted access.
-        :type users: [dict]
-        :param dclist : list of strings of datacenters
+        :param spot_creation_type: Specifying the mode of creating geo-fabric.
+                                   If you use AUTOMATIC, a random spot region
+                                   will be assigned by the system. If you
+                                   specify NONE, a geo-fabric is created
+                                   without the spot properties. If you specify
+                                   SPOT_REGION,pass the corresponding spot
+                                   region in the spot_dc parameter.
+        :type name: Enum containing spot region creation types
+        :param name: Spot Region name, if spot_creation_type is set to
+                     SPOT_REGION
+        :type name: str
+        :param users: List of users with access to the new fabric
+        :type users: [str | unicode]
+        :param dclist: list of strings of datacenters
         :type dclist: [str | unicode]
-        :param realtime: Whether or not the DB is realtime-enabled.
-        :type realtime: bool
-        :return: True if database was created successfully.
+        :returns: True if fabric was created successfully.
         :rtype: bool
-        :raise c8.exceptions.DatabaseCreateError: If create fails.
-
-        Here is an example entry for parameter **users**:
-
-        .. code-block:: python
-
-            {
-                'username': 'john',
-                'password': 'password',
-                'active': True,
-                'extra': {'Department': 'IT'}
-            }
+        :raise c8.exceptions.FabricCreateError: If create fails.
         """
-        data = {'name': name}
+        data = {"name": name}
         if users is not None:
-            data['users'] = [{
-                'username': user['username'],
-                'passwd': user['password'],
-                'active': user.get('active', True),
-                'extra': user.get('extra', {})
-            } for user in users]
+            data["users"] = users
 
         options = {}
-        options['realTime'] = realtime
-
+        dcl = ""
         if dclist:
-            # Process dclist param (type list) to build up comma-separated string of DCs
-            dcl = ''
+            # Process dclist param (type list) to build up comma-separated
+            # string of DCs
             for dc in dclist:
                 if len(dcl) > 0:
-                    dcl += ','
+                    dcl += ","
                 dcl += dc
-            options['dcList'] = dcl
+        options["dcList"] = dcl
 
-        data['options'] = options
+        if spot_creation_type == self.SPOT_CREATION_TYPES.NONE:
+            options["spotDc"] = ""
+        elif spot_creation_type == self.SPOT_CREATION_TYPES.SPOT_REGION and spot_dc:
+            options["spotDc"] = spot_dc
 
-        request = Request(
-            method='post',
-            endpoint='/_api/database',
-            data=data
-        )
+        data["options"] = options
+
+        request = Request(method="post", endpoint="/database", data=data)
 
         def response_handler(resp):
             if not resp.is_success:
-                raise DatabaseCreateError(resp, request)
+                raise FabricCreateError(resp, request)
             return True
 
         return self._execute(request, response_handler)
 
-    def delete_database(self, name, ignore_missing=False):
-        """Delete the database.
+    def get_fabric_metadata(self):
+        """Fetch information about a GeoFabric.
 
-        :param name: Database name.
+        :returns: Fabric information.
+        :rtype: dict
+        :raise c8.exceptions.FabricGetMetadataError: If retrieval fails.
+        """
+        request = Request(method="get", endpoint="/database/metadata")
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise FabricGetMetadataError(resp, request)
+            return resp.body["result"]
+
+        return self._execute(request, response_handler)
+
+    def set_fabric_metadata(self, metadata):
+        """Set the GeoFabric Metadata.
+
+        :param metadata: Fabric metadata.
+        :type metadata: dict
+        :returns: True if metadata was set successfully.
+        :rtype: bool
+        :raise c8.exceptions.FabricSetMetadataError: If set fails.
+        """
+
+        data = {"metadata": metadata}
+        request = Request(method="put", endpoint="/database/metadata", data=data)
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise FabricSetMetadataError(resp, request)
+            return resp.body["result"]
+
+        return self._execute(request, response_handler)
+
+    def update_fabric_metadata(self, metadata):
+        """Modfiy the GeoFabric metadata.
+
+        :param metadata: Fabric metadata.
+        :type metadata: dict
+        :returns: True if metadata was set successfully.
+        :rtype: bool
+        :raise c8.exceptions.FabricUpdateMetadataError: If update fails.
+        """
+        data = {"metadata": metadata}
+        request = Request(method="patch", endpoint="/database/metadata", data=data)
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise FabricUpdateMetadataError(resp, request)
+            return resp.body["result"]
+
+        return self._execute(request, response_handler)
+
+    def delete_fabric(self, name, ignore_missing=False):
+        """Delete the fabric.
+
+        :param name: Fabric name.
         :type name: str | unicode
-        :param ignore_missing: Do not raise an exception on missing database.
+        :param ignore_missing: Do not raise an exception on missing fabric.
         :type ignore_missing: bool
-        :return: True if database was deleted successfully, False if database
+        :returns: True if fabric was deleted successfully, False if fabric
             was not found and **ignore_missing** was set to True.
         :rtype: bool
-        :raise c8.exceptions.DatabaseDeleteError: If delete fails.
+        :raise c8.exceptions.FabricDeleteError: If delete fails.
         """
-        request = Request(
-            method='delete',
-            endpoint='/_api/database/{}'.format(name)
-        )
+        request = Request(method="delete", endpoint="/database/{}".format(name))
 
         def response_handler(resp):
             if resp.error_code == 1228 and ignore_missing:
                 return False
             if not resp.is_success:
-                raise DatabaseDeleteError(resp, request)
-            return resp.body['result']
+                raise FabricDeleteError(resp, request)
+            return resp.body["result"]
 
         return self._execute(request, response_handler)
 
     #########################
     # Collection Management #
     #########################
 
     def collection(self, name):
         """Return the standard collection API wrapper.
 
         :param name: Collection name.
         :type name: str | unicode
-        :return: Standard collection API wrapper.
+        :returns: Standard collection API wrapper.
         :rtype: c8.collection.StandardCollection
         """
-        return StandardCollection(self._conn, self._executor, name)
+        if self.has_collection(name):
+            return StandardCollection(self._conn, self._executor, name)
+        else:
+            raise CollectionFindError("Collection not found")
 
     def has_collection(self, name):
-        """Check if collection exists in the database.
+        """Check if collection exists in the fabric.
 
         :param name: Collection name.
         :type name: str | unicode
-        :return: True if collection exists, False otherwise.
+        :returns: True if collection exists, False otherwise.
         :rtype: bool
         """
-        return any(col['name'] == name for col in self.collections())
+        return any(col["name"] == name for col in self.collections())
 
-    def collections(self):
-        """Return the collections in the database.
+    def collections(self, collectionModel=None):
+        """Return the collections in the fabric.
 
-        :return: Collections in the database and their details.
+        :returns: Collections in the fabric and their details.
         :rtype: [dict]
         :raise c8.exceptions.CollectionListError: If retrieval fails.
         """
-        request = Request(
-            method='get',
-            endpoint='/_api/collection'
-        )
+        request = Request(method="get", endpoint="/collection")
 
         def response_handler(resp):
             if not resp.is_success:
                 raise CollectionListError(resp, request)
-            return [{
-                'id': col['id'],
-                'name': col['name'],
-                'system': col['isSystem'],
-                'type': StandardCollection.types[col['type']],
-                'status': StandardCollection.statuses[col['status']],
-            } for col in map(dict, resp.body['result'])]
+            if collectionModel is not None:
+                docs = [
+                    col
+                    for col in map(dict, resp.body["result"])
+                    if col["collectionModel"] == collectionModel
+                ]
+            else:
+                docs = [col for col in map(dict, resp.body["result"])]
+            return [
+                {
+                    "id": col["id"],
+                    "name": col["name"],
+                    "system": col["isSystem"],
+                    "isSpot": col["isSpot"],
+                    "type": StandardCollection.types[col["type"]],
+                    "status": StandardCollection.statuses[col["status"]],
+                    "collectionModel": col["collectionModel"],
+                }
+                for col in docs
+            ]
 
         return self._execute(request, response_handler)
 
-    def create_collection(self,
-                          name,
-                          sync=False,
-                          compact=True,
-                          system=False,
-                          journal_size=None,
-                          edge=False,
-                          volatile=False,
-                          user_keys=True,
-                          key_increment=None,
-                          key_offset=None,
-                          key_generator='traditional',
-                          shard_fields=None,
-                          shard_count=None,
-                          index_bucket_count=None,
-                          replication_factor=None,
-                          shard_like=None,
-                          sync_replication=None,
-                          enforce_replication_factor=None):
+    def create_collection(
+        self,
+        name,
+        sync=False,
+        edge=False,
+        user_keys=True,
+        key_increment=None,
+        key_offset=None,
+        key_generator="traditional",
+        shard_fields=None,
+        index_bucket_count=None,
+        sync_replication=None,
+        enforce_replication_factor=None,
+        spot_collection=False,
+        local_collection=False,
+        is_system=False,
+        stream=False,
+    ):
         """Create a new collection.
 
         :param name: Collection name.
         :type name: str | unicode
         :param sync: If set to True, document operations via the collection
             will block until synchronized to disk by default.
         :type sync: bool
-        :param compact: If set to True, the collection is compacted. Applies
-            only to MMFiles storage engine.
-        :type compact: bool
-        :param system: If set to True, a system collection is created. The
-            collection name must have leading underscore "_" character.
-        :type system: bool
-        :param journal_size: Max size of the journal in bytes.
-        :type journal_size: int
         :param edge: If set to True, an edge collection is created.
         :type edge: bool
-        :param volatile: If set to True, collection data is kept in-memory only
-            and not made persistent. Unloading the collection will cause the
-            collection data to be discarded. Stopping or re-starting the server
-            will also cause full loss of data.
-        :type volatile: bool
         :param key_generator: Used for generating document keys. Allowed values
             are "traditional" or "autoincrement".
         :type key_generator: str | unicode
         :param user_keys: If set to True, users are allowed to supply document
             keys. If set to False, the key generator is solely responsible for
             supplying the key values.
         :type user_keys: bool
@@ -592,118 +658,133 @@
             **key_generator** is set to "autoincrement".
         :type key_increment: int
         :param key_offset: Key offset value. Applies only when value of
             **key_generator** is set to "autoincrement".
         :type key_offset: int
         :param shard_fields: Field(s) used to determine the target shard.
         :type shard_fields: [str | unicode]
-        :param shard_count: Number of shards to create.
-        :type shard_count: int
         :param index_bucket_count: Number of buckets into which indexes using
             hash tables are split. The default is 16, and this number has to be
             a power of 2 and less than or equal to 1024. For large collections,
             one should increase this to avoid long pauses when the hash table
             has to be initially built or re-sized, since buckets are re-sized
             individually and can be initially built in parallel. For instance,
             64 may be a sensible value for 100 million documents.
         :type index_bucket_count: int
-        :param replication_factor: Number of copies of each shard on different
-            servers in a cluster. Allowed values are 1 (only one copy is kept
-            and no synchronous replication), and n (n-1 replicas are kept and
-            any two copies are replicated across servers synchronously, meaning
-            every write to the master is copied to all slaves before operation
-            is reported successful).
-        :type replication_factor: int
-        :param shard_like: Name of prototype collection whose sharding
-            specifics are imitated. Prototype collections cannot be dropped
-            before imitating collections. Applies to enterprise version of
-            C8Db only.
-        :type shard_like: str | unicode
         :param sync_replication: If set to True, server reports success only
             when collection is created in all replicas. You can set this to
             False for faster server response, and if full replication is not a
             concern.
         :type sync_replication: bool
         :param enforce_replication_factor: Check if there are enough replicas
             available at creation time, or halt the operation.
         :type enforce_replication_factor: bool
-        :return: Standard collection API wrapper.
+        :param spot_collection: If True, it is a spot collection
+        :type spot_collection: bool
+        :param is_system: If True, able to create system collections
+        :type is_system: bool
+        :param stream: If True, create a local stream for collection.
+        :type stream: bool
+        :returns: Standard collection API wrapper.
         :rtype: c8.collection.StandardCollection
         :raise c8.exceptions.CollectionCreateError: If create fails.
         """
-        key_options = {'type': key_generator, 'allowUserKeys': user_keys}
+        key_options = {"type": key_generator, "allowUserKeys": user_keys}
         if key_increment is not None:
-            key_options['increment'] = key_increment
+            key_options["increment"] = key_increment
         if key_offset is not None:
-            key_options['offset'] = key_offset
+            key_options["offset"] = key_offset
+        if spot_collection and local_collection:
+            return "Collection can either be spot or local"
+        else:
+            data = {
+                "name": name,
+                "waitForSync": sync,
+                "keyOptions": key_options,
+                "type": 3 if edge else 2,
+                "isSpot": spot_collection,
+                "isLocal": local_collection,
+                "isSystem": is_system,
+                "stream": stream,
+            }
 
-        data = {
-            'name': name,
-            'waitForSync': sync,
-            'doCompact': compact,
-            'isSystem': system,
-            'isVolatile': volatile,
-            'keyOptions': key_options,
-            'type': 3 if edge else 2
-        }
-        if journal_size is not None:
-            data['journalSize'] = journal_size
-        if shard_count is not None:
-            data['numberOfShards'] = shard_count
         if shard_fields is not None:
-            data['shardKeys'] = shard_fields
+            data["shardKeys"] = shard_fields
         if index_bucket_count is not None:
-            data['indexBuckets'] = index_bucket_count
-        if replication_factor is not None:
-            data['replicationFactor'] = replication_factor
-        if shard_like is not None:
-            data['distributeShardsLike'] = shard_like
+            data["indexBuckets"] = index_bucket_count
 
         params = {}
         if sync_replication is not None:
-            params['waitForSyncReplication'] = sync_replication
+            params["waitForSyncReplication"] = sync_replication
         if enforce_replication_factor is not None:
-            params['enforceReplicationFactor'] = enforce_replication_factor
+            params["enforceReplicationFactor"] = enforce_replication_factor
 
         request = Request(
-            method='post',
-            endpoint='/_api/collection',
-            params=params,
-            data=data
+            method="post", endpoint="/collection", params=params, data=data
         )
 
         def response_handler(resp):
             if resp.is_success:
                 return self.collection(name)
             raise CollectionCreateError(resp, request)
 
         return self._execute(request, response_handler)
 
+    def update_collection_properties(
+        self, collection_name, has_stream=None, wait_for_sync=None
+    ):
+        """Changes the properties of a collection.
+           Note: except for waitForSync and hasStream, collection properties cannot be changed once a collection is created.
+        :param collection_name: Collection name.
+        :type collection_name: str | unicode
+        :param has_stream: True if creating a live collection stream.
+        :type has_stream: bool
+        :param wait_for_sync: True if all data must be synced to storage before operation returns.
+        :type wait_for_sync: bool
+        """
+
+        data = {}
+        if has_stream is not None:
+            data["hasStream"] = has_stream
+        if wait_for_sync is not None:
+            data["waitForSync"] = wait_for_sync
+
+        request = Request(
+            method="put",
+            endpoint="/collection/{}/properties".format(collection_name),
+            data=data,
+        )
+
+        def response_handler(resp):
+            if resp.is_success:
+                return resp.body
+            raise CollectionPropertiesError(resp, request)
+
+        return self._execute(request, response_handler)
+
     def delete_collection(self, name, ignore_missing=False, system=None):
         """Delete the collection.
 
         :param name: Collection name.
         :type name: str | unicode
         :param ignore_missing: Do not raise an exception on missing collection.
         :type ignore_missing: bool
         :param system: Whether the collection is a system collection.
         :type system: bool
-        :return: True if collection was deleted successfully, False if
+        :returns: True if collection was deleted successfully, False if
             collection was not found and **ignore_missing** was set to True.
         :rtype: bool
         :raise c8.exceptions.CollectionDeleteError: If delete fails.
         """
         params = {}
         if system is not None:
-            params['isSystem'] = system
+            params["isSystem"] = system
 
         request = Request(
-            method='delete',
-            endpoint='/_api/collection/{}'.format(name),
-            params=params
+            method="delete", endpoint="/collection/{}".format(name), params=params
         )
 
         def response_handler(resp):
             if resp.error_code == 1203 and ignore_missing:
                 return False
             if not resp.is_success:
                 raise CollectionDeleteError(resp, request)
@@ -716,976 +797,824 @@
     ####################
 
     def graph(self, name):
         """Return the graph API wrapper.
 
         :param name: Graph name.
         :type name: str | unicode
-        :return: Graph API wrapper.
+        :returns: Graph API wrapper.
         :rtype: c8.graph.Graph
         """
         return Graph(self._conn, self._executor, name)
 
     def has_graph(self, name):
-        """Check if a graph exists in the database.
+        """Check if a graph exists in the fabric.
 
         :param name: Graph name.
         :type name: str | unicode
-        :return: True if graph exists, False otherwise.
+        :returns: True if graph exists, False otherwise.
         :rtype: bool
         """
         for graph in self.graphs():
-            if graph['name'] == name:
+            if graph["name"] == name:
                 return True
         return False
 
     def graphs(self):
-        """List all graphs in the database.
+        """List all graphs in the fabric.
 
-        :return: Graphs in the database.
+        :returns: Graphs in the fabric.
         :rtype: [dict]
         :raise c8.exceptions.GraphListError: If retrieval fails.
         """
-        request = Request(method='get', endpoint='/_api/graph')
+        request = Request(method="get", endpoint="/graph")
 
         def response_handler(resp):
             if not resp.is_success:
                 raise GraphListError(resp, request)
             return [
                 {
-                    'id': body['_id'],
-                    'name': body['_key'],
-                    'revision': body['_rev'],
-                    'orphan_collections': body['orphanCollections'],
-                    'edge_definitions': [
+                    "id": body["_id"],
+                    "name": body["_key"],
+                    "revision": body["_rev"],
+                    "orphan_collections": body["orphanCollections"],
+                    "edge_definitions": [
                         {
-                            'edge_collection': definition['collection'],
-                            'from_vertex_collections': definition['from'],
-                            'to_vertex_collections': definition['to'],
+                            "edge_collection": definition["collection"],
+                            "from_vertex_collections": definition["from"],
+                            "to_vertex_collections": definition["to"],
                         }
-                        for definition in body['edgeDefinitions']
+                        for definition in body["edgeDefinitions"]
                     ],
-                    'shard_count': body.get('numberOfShards'),
-                    'replication_factor': body.get('replicationFactor')
-                } for body in resp.body['graphs']
+                    "shard_count": body.get("numberOfShards"),
+                    "replication_factor": body.get("replicationFactor"),
+                }
+                for body in resp.body["graphs"]
             ]
 
         return self._execute(request, response_handler)
 
-    def create_graph(self,
-                     name,
-                     edge_definitions=None,
-                     orphan_collections=None,
-                     smart=None,
-                     smart_field=None,
-                     shard_count=None):
+    def create_graph(
+        self, name, edge_definitions=None, orphan_collections=None, shard_count=None
+    ):
         """Create a new graph.
 
         :param name: Graph name.
         :type name: str | unicode
         :param edge_definitions: List of edge definitions, where each edge
             definition entry is a dictionary with fields "edge_collection",
             "from_vertex_collections" and "to_vertex_collections" (see below
             for example).
         :type edge_definitions: [dict]
         :param orphan_collections: Names of additional vertex collections that
             are not in edge definitions.
         :type orphan_collections: [str | unicode]
-        :param smart: If set to True, sharding is enabled (see parameter
-            **smart_field** below). Applies only to enterprise version of
-            C8Db.
-        :type smart: bool
-        :param smart_field: Document field used to shard the vertices of the
-            graph. To use this, parameter **smart** must be set to True and
-            every vertex in the graph must have the smart field. Applies only
-            to enterprise version of C8Db.
-        :type smart_field: str | unicode
         :param shard_count: Number of shards used for every collection in the
             graph. To use this, parameter **smart** must be set to True and
             every vertex in the graph must have the smart field. This number
             cannot be modified later once set. Applies only to enterprise
             version of C8Db.
         :type shard_count: int
-        :return: Graph API wrapper.
+        :returns: Graph API wrapper.
         :rtype: c8.graph.Graph
         :raise c8.exceptions.GraphCreateError: If create fails.
 
         Here is an example entry for parameter **edge_definitions**:
 
         .. code-block:: python
 
             {
                 'edge_collection': 'teach',
                 'from_vertex_collections': ['teachers'],
                 'to_vertex_collections': ['lectures']
             }
         """
-        data = {'name': name}
+        data = {"name": name}
         if edge_definitions is not None:
-            data['edgeDefinitions'] = [{
-                'collection': definition['edge_collection'],
-                'from': definition['from_vertex_collections'],
-                'to': definition['to_vertex_collections']
-            } for definition in edge_definitions]
+            data["edgeDefinitions"] = [
+                {
+                    "collection": definition["edge_collection"],
+                    "from": definition["from_vertex_collections"],
+                    "to": definition["to_vertex_collections"],
+                }
+                for definition in edge_definitions
+            ]
         if orphan_collections is not None:
-            data['orphanCollections'] = orphan_collections
-        if smart is not None:  # pragma: no cover
-            data['isSmart'] = smart
-        if smart_field is not None:  # pragma: no cover
-            data['smartGraphAttribute'] = smart_field
+            data["orphanCollections"] = orphan_collections
         if shard_count is not None:  # pragma: no cover
-            data['numberOfShards'] = shard_count
+            data["numberOfShards"] = shard_count
 
-        request = Request(
-            method='post',
-            endpoint='/_api/graph',
-            data=data
-        )
+        request = Request(method="post", endpoint="/graph", data=data)
 
         def response_handler(resp):
             if resp.is_success:
                 return Graph(self._conn, self._executor, name)
             raise GraphCreateError(resp, request)
 
         return self._execute(request, response_handler)
 
     def delete_graph(self, name, ignore_missing=False, drop_collections=None):
-        """Drop the graph of the given name from the database.
+        """Drop the graph of the given name from the fabric.
 
         :param name: Graph name.
         :type name: str | unicode
         :param ignore_missing: Do not raise an exception on missing graph.
         :type ignore_missing: bool
         :param drop_collections: Drop the collections of the graph also. This
             is only if they are not in use by other graphs.
         :type drop_collections: bool
-        :return: True if graph was deleted successfully, False if graph was not
+        :returns: True if graph was deleted successfully, False if graph was not
             found and **ignore_missing** was set to True.
         :rtype: bool
         :raise c8.exceptions.GraphDeleteError: If delete fails.
         """
         params = {}
         if drop_collections is not None:
-            params['dropCollections'] = drop_collections
+            params["dropCollections"] = drop_collections
 
         request = Request(
-            method='delete',
-            endpoint='/_api/graph/{}'.format(name),
-            params=params
+            method="delete", endpoint="/graph/{}".format(name), params=params
         )
 
         def response_handler(resp):
             if resp.error_code == 1924 and ignore_missing:
                 return False
             if not resp.is_success:
                 raise GraphDeleteError(resp, request)
             return True
 
         return self._execute(request, response_handler)
 
-    #######################
-    # Document Management #
-    #######################
-
-    def has_document(self, document, rev=None, check_rev=True):
-        """Check if a document exists.
+    ########################
+    # Async Job Management #
+    ########################
 
-        :param document: Document ID or body with "_id" field.
-        :type document: str | unicode | dict
-        :param rev: Expected document revision. Overrides value of "_rev" field
-            in **document** if present.
-        :type rev: str | unicode
-        :param check_rev: If set to True, revision of **document** (if given)
-            is compared against the revision of target document.
-        :type check_rev: bool
-        :return: True if document exists, False otherwise.
-        :rtype: bool
-        :raise c8.exceptions.DocumentInError: If check fails.
-        :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
-        """
-        return self._get_col_by_doc(document).has(
-            document=document,
-            rev=rev,
-            check_rev=check_rev
-        )
+    # Pratik: APIs not supported in documentation. Waiting for verification
+    # def async_jobs(self, status, count=None):
+    #     """Return IDs of async jobs with given status.
+    #
+    #     :param status: Job status (e.g. "pending", "done").
+    #     :type status: str | unicode
+    #     :param count: Max number of job IDs to return.
+    #     :type count: int
+    #     :returns: List of job IDs.
+    #     :rtype: [str | unicode]
+    #     :raise c8.exceptions.AsyncJobListError: If retrieval fails.
+    #     """
+    #     params = {}
+    #     if count is not None:
+    #         params['count'] = count
+    #
+    #     request = Request(
+    #         method='get',
+    #         endpoint='/job/{}'.format(status),
+    #         params=params
+    #     )
+    #
+    #     def response_handler(resp):
+    #         if resp.is_success:
+    #             return resp.body
+    #         raise AsyncJobListError(resp, request)
+    #
+    #     return self._execute(request, response_handler)
+    #
+    # def clear_async_jobs(self, threshold=None):
+    #     """Clear async job results from the server.
+    #
+    #     Async jobs that are still queued or running are not stopped.
+    #
+    #     :param threshold: If specified, only the job results created prior to
+    #         the threshold (a unix timestamp) are deleted. Otherwise, all job
+    #         results are deleted.
+    #     :type threshold: int
+    #     :returns: True if job results were cleared successfully.
+    #     :rtype: bool
+    #     :raise c8.exceptions.AsyncJobClearError: If operation fails.
+    #     """
+    #     if threshold is None:
+    #         url = '/job/all'
+    #         params = None
+    #     else:
+    #         url = '/job/expired'
+    #         params = {'stamp': threshold}
+    #
+    #     request = Request(
+    #         method='delete',
+    #         endpoint=url,
+    #         params=params
+    #     )
+    #
+    #     def response_handler(resp):
+    #         if resp.is_success:
+    #             return True
+    #         raise AsyncJobClearError(resp, request)
+    #
+    #     return self._execute(request, response_handler)
 
-    def document(self, document, rev=None, check_rev=True):
-        """Return a document.
+    ########################
+    # Streams Management   #
+    ########################
 
-        :param document: Document ID or body with "_id" field.
-        :type document: str | unicode | dict
-        :param rev: Expected document revision. Overrides the value of "_rev"
-            field in **document** if present.
-        :type rev: str | unicode
-        :param check_rev: If set to True, revision of **document** (if given)
-            is compared against the revision of target document.
-        :type check_rev: bool
-        :return: Document, or None if not found.
-        :rtype: dict | None
-        :raise c8.exceptions.DocumentGetError: If retrieval fails.
-        :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
-        """
-        return self._get_col_by_doc(document).get(
-            document=document,
-            rev=rev,
-            check_rev=check_rev
-        )
+    def stream(self, operation_timeout_seconds=30):
+        """Return the stream collection API wrapper.
 
-    def insert_document(self,
-                        collection,
-                        document,
-                        return_new=False,
-                        sync=None,
-                        silent=False):
-        """Insert a new document.
-
-        :param collection: Collection name.
-        :type collection: str | unicode
-        :param document: Document to insert. If it contains the "_key" or "_id"
-            field, the value is used as the key of the new document (otherwise
-            it is auto-generated). Any "_rev" field is ignored.
-        :type document: dict
-        :param return_new: Include body of the new document in the returned
-            metadata. Ignored if parameter **silent** is set to True.
-        :type return_new: bool
-        :param sync: Block until operation is synchronized to disk.
-        :type sync: bool
-        :param silent: If set to True, no document metadata is returned. This
-            can be used to save resources.
-        :type silent: bool
-        :return: Document metadata (e.g. document key, revision) or True if
-            parameter **silent** was set to True.
-        :rtype: bool | dict
-        :raise c8.exceptions.DocumentInsertError: If insert fails.
-        """
-        return self.collection(collection).insert(
-            document=document,
-            return_new=return_new,
-            sync=sync,
-            silent=silent
+        :returns: stream collection API wrapper.
+        :rtype: c8.stream_collection.StreamCollection
+        """
+        return StreamCollection(
+            self,
+            self._conn,
+            self._executor,
+            self.url,
+            self.stream_port,
+            operation_timeout_seconds,
         )
 
-    def update_document(self,
-                        document,
-                        check_rev=True,
-                        merge=True,
-                        keep_none=True,
-                        return_new=False,
-                        return_old=False,
-                        sync=None,
-                        silent=False):
-        """Update a document.
-
-        :param document: Partial or full document with the updated values. It
-            must contain the "_id" field.
-        :type document: dict
-        :param check_rev: If set to True, revision of **document** (if given)
-            is compared against the revision of target document.
-        :type check_rev: bool
-        :param merge: If set to True, sub-dictionaries are merged instead of
-            the new one overwriting the old one.
-        :type merge: bool
-        :param keep_none: If set to True, fields with value None are retained
-            in the document. Otherwise, they are removed completely.
-        :type keep_none: bool
-        :param return_new: Include body of the new document in the result.
-        :type return_new: bool
-        :param return_old: Include body of the old document in the result.
-        :type return_old: bool
-        :param sync: Block until operation is synchronized to disk.
-        :type sync: bool
-        :param silent: If set to True, no document metadata is returned. This
-            can be used to save resources.
-        :type silent: bool
-        :return: Document metadata (e.g. document key, revision) or True if
-            parameter **silent** was set to True.
-        :rtype: bool | dict
-        :raise c8.exceptions.DocumentUpdateError: If update fails.
-        :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
-        """
-        return self._get_col_by_doc(document).update(
-            document=document,
-            check_rev=check_rev,
-            merge=merge,
-            keep_none=keep_none,
-            return_new=return_new,
-            return_old=return_old,
-            sync=sync,
-            silent=silent
-        )
+    def streams(self, local=None):
+        """Get list of all streams under given fabric
 
-    def replace_document(self,
-                         document,
-                         check_rev=True,
-                         return_new=False,
-                         return_old=False,
-                         sync=None,
-                         silent=False):
-        """Replace a document.
-
-        :param document: New document to replace the old one with. It must
-            contain the "_id" field. Edge document must also have "_from" and
-            "_to" fields.
-        :type document: dict
-        :param check_rev: If set to True, revision of **document** (if given)
-            is compared against the revision of target document.
-        :type check_rev: bool
-        :param return_new: Include body of the new document in the result.
-        :type return_new: bool
-        :param return_old: Include body of the old document in the result.
-        :type return_old: bool
-        :param sync: Block until operation is synchronized to disk.
-        :type sync: bool
-        :param silent: If set to True, no document metadata is returned. This
-            can be used to save resources.
-        :type silent: bool
-        :return: Document metadata (e.g. document key, revision) or True if
-            parameter **silent** was set to True.
-        :rtype: bool | dict
-        :raise c8.exceptions.DocumentReplaceError: If replace fails.
-        :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
-        """
-        return self._get_col_by_doc(document).replace(
-            document=document,
-            check_rev=check_rev,
-            return_new=return_new,
-            return_old=return_old,
-            sync=sync,
-            silent=silent
-        )
+        :returns: List of streams under given fabric.
+        :rtype: json
+        :raise c8.exceptions.StreamListError: If retrieving streams fails.
+        """
+        if local is False:
+            url_endpoint = "/streams?global=true"
 
-    def delete_document(self,
-                        document,
-                        rev=None,
-                        check_rev=True,
-                        ignore_missing=False,
-                        return_old=False,
-                        sync=None,
-                        silent=False):
-        """Delete a document.
-
-        :param document: Document ID, key or body. Document body must contain
-            the "_id" field.
-        :type document: str | unicode | dict
-        :param rev: Expected document revision. Overrides the value of "_rev"
-            field in **document** if present.
-        :type rev: str | unicode
-        :param check_rev: If set to True, revision of **document** (if given)
-            is compared against the revision of target document.
-        :type check_rev: bool
-        :param ignore_missing: Do not raise an exception on missing document.
-            This parameter has no effect in transactions where an exception is
-            always raised on failures.
-        :type ignore_missing: bool
-        :param return_old: Include body of the old document in the result.
-        :type return_old: bool
-        :param sync: Block until operation is synchronized to disk.
-        :type sync: bool
-        :param silent: If set to True, no document metadata is returned. This
-            can be used to save resources.
-        :type silent: bool
-        :return: Document metadata (e.g. document key, revision), or True if
-            parameter **silent** was set to True, or False if document was not
-            found and **ignore_missing** was set to True (does not apply in
-            transactions).
-        :rtype: bool | dict
-        :raise c8.exceptions.DocumentDeleteError: If delete fails.
-        :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
-        """
-        return self._get_col_by_doc(document).delete(
-            document=document,
-            rev=rev,
-            check_rev=check_rev,
-            ignore_missing=ignore_missing,
-            return_old=return_old,
-            sync=sync,
-            silent=silent
-        )
+        elif local is True:
+            url_endpoint = "/streams?global=false"
 
+        elif local is None:
+            url_endpoint = "/streams"
 
-    ###################
-    # User Management #
-    ###################
-    # See tenant.py
+        request = Request(method="get", endpoint=url_endpoint)
 
-    #########################
-    # Permission Management #
-    #########################
-    # See tenant.py
+        def response_handler(resp):
+            code = resp.status_code
+            if resp.is_success:
+                return [
+                    {
+                        "name": col["topic"],
+                        "topic": col["topic"],
+                        "local": col["local"],
+                        "db": col["db"],
+                        "tenant": col["tenant"],
+                        "type": StreamCollection.types[col["type"]],
+                        "status": "terminated"
+                        if "terminated" in col
+                        else "active",  # noqa
+                    }
+                    for col in map(dict, resp.body["result"])
+                ]
+            elif code == 403:
+                raise StreamPermissionError(resp, request)
+            raise StreamListError(resp, request)
 
+        return self._execute(request, response_handler)
 
-    ########################
-    # Async Job Management #
-    ########################
+    def has_stream(self, stream, isCollectionStream=False, local=False):
+        """Check if the list of streams has a stream with the given name.
 
-    def async_jobs(self, status, count=None):
-        """Return IDs of async jobs with given status.
+        :param stream: The name of the stream for which to check in the list
+                       of all streams.
+        :type stream: str | unicode
+        :returns: True=stream found; False=stream not found.
+        :rtype: bool
+        """
+        if isCollectionStream is False:
+            if local is False and "c8globals" not in stream:
+                stream = "c8globals." + stream
+            elif local is True and "c8locals" not in stream:
+                stream = "c8locals." + stream
+        return any(mystream["name"] == stream for mystream in self.streams(local=local))
 
-        :param status: Job status (e.g. "pending", "done").
-        :type status: str | unicode
-        :param count: Max number of job IDs to return.
-        :type count: int
-        :return: List of job IDs.
-        :rtype: [str | unicode]
-        :raise c8.exceptions.AsyncJobListError: If retrieval fails.
+    def create_stream(self, stream, local=False):
         """
-        params = {}
-        if count is not None:
-            params['count'] = count
+        Create the stream under the given fabric
 
-        request = Request(
-            method='get',
-            endpoint='/_api/job/{}'.format(status),
-            params=params
-        )
+        :param stream: name of stream
+        :param local: Operate on a local stream instead of a global one.
+        :returns: 200, OK if operation successful
+        :raise: c8.exceptions.StreamCreateError: If creating streams fails.
+        """
+        if local is True:
+            endpoint = "{}/{}?global=False".format(ENDPOINT, stream)
+        elif local is False:
+            endpoint = "{}/{}?global=True".format(ENDPOINT, stream)
+
+        request = Request(method="post", endpoint=endpoint)
 
         def response_handler(resp):
+            code = resp.status_code
             if resp.is_success:
-                return resp.body
-            raise AsyncJobListError(resp, request)
+                return resp.body["result"]
+            elif code == 502:
+                raise StreamCommunicationError(resp, request)
+            raise StreamCreateError(resp, request)
 
         return self._execute(request, response_handler)
 
-    def clear_async_jobs(self, threshold=None):
-        """Clear async job results from the server.
-
-        Async jobs that are still queued or running are not stopped.
+    def delete_stream(self, stream, force=False):
+        """
+        Delete the streams under the given fabric
 
-        :param threshold: If specified, only the job results created prior to
-            the threshold (a unix timestamp) are deleted. Otherwise, all job
-            results are deleted.
-        :type threshold: int
-        :return: True if job results were cleared successfully.
-        :rtype: bool
-        :raise c8.exceptions.AsyncJobClearError: If operation fails.
+        :param stream: name of stream
+        :param force:
+        :returns: 200, OK if operation successful
+        :raise: c8.exceptions.StreamDeleteError: If deleting streams fails.
         """
-        if threshold is None:
-            url = '/_api/job/all'
-            params = None
-        else:
-            url = '/_api/job/expired'
-            params = {'stamp': threshold}
+        endpoint = f"{ENDPOINT}/{stream}"
+        if force:
+            endpoint = endpoint + "?force=true"
 
-        request = Request(
-            method='delete',
-            endpoint=url,
-            params=params
-        )
+        request = Request(method="delete", endpoint=endpoint)
 
         def response_handler(resp):
+            code = resp.status_code
             if resp.is_success:
                 return True
-            raise AsyncJobClearError(resp, request)
+            elif code == 403:
+                raise StreamPermissionError(resp, request)
+            elif code == 412:
+                raise StreamDeleteError(resp, request)
+            raise StreamConnectionError(resp, request)
 
         return self._execute(request, response_handler)
 
-    ########################
-    # Streams Management   #
-    ########################
+    #####################
+    # Restql Management #
+    #####################
 
-    def stream(self, operation_timeout_seconds=30):
-        """Return the stream collection API wrapper.
+    def save_restql(self, data):
+        """Save restql by name.
 
-        :return: stream collection API wrapper.
-        :rtype: c8.stream_collection.StreamCollection
+        :param data: data to be used for restql POST API
+        :type data: dict
+        :returns: Results of restql API
+        :rtype: dict
+        :raise c8.exceptions.RestqlCreateError: if restql operation failed
         """
-        return StreamCollection(self, self._conn, self._executor, self.url, self.stream_port, operation_timeout_seconds)
 
-    def streams(self):
-        """Get list of all streams under given database
+        query_name = data["query"]["name"]
+        if " " in query_name:
+            raise RestqlValidationError("White Spaces not allowed in Query " "Name")
 
-        :return: List of streams under given database.
-        :rtype: json
-        :raise c8.exceptions.StreamListError: If retrieving streams fails.
-        """
-        url_endpoint = '/streams'
+        request = Request(method="post", endpoint="/restql", data=data)
 
-        request = Request(
-            method='get',
-            endpoint=url_endpoint
-        )
-        
         def response_handler(resp):
-            code = resp.status_code
-            if resp.is_success:
-                # NOTE: server API returns stream name as field 'topic' - we provide both here for user convenience
-                return [{
-                    'name': col['topic'],
-                    'topic': col['topic'],
-                    'local': col['local'],
-                    'db': col['db'],
-                    'tenant': col['tenant'],
-                    'type': StreamCollection.types[col['type']],
-                    'status': 'terminated' if 'terminated' in col else 'active',
-                } for col in map(dict, resp.body['result'])]
-            elif code == 403:
-                raise ex.StreamPermissionError(resp, request)
-            raise ex.StreamConnectionError(resp, request)
-        
-        return self._execute(request, response_handler)
- 
-    def persistent_streams(self, local=False):
-        """Get list of all streams under given database
+            if not resp.is_success:
+                raise RestqlCreateError(resp, request)
+            return resp.body["result"]
 
-        :param local: Operate on a local stream instead of a global one. Default value: false
-        :return: List of streams under given database.
-        :rtype: json
-        :raise c8.exceptions.StreamListError: If retrieving streams fails.
+        return self._execute(request, response_handler)
+
+    def import_restql(self, queries, details=False):
+        """Import custom queries.
+
+        :param queries: queries to be imported
+        :type queries: [dict]
+        :param details: Whether to include details
+        :type details: bool
+        :returns: Results of importing restql
+        :rtype: dict
+        :raise c8.exceptions.RestqlImportError: if restql operation failed
         """
-        url_endpoint = '/streams/persistent?local={}'.format(local)
 
-        request = Request(
-            method='get',
-            endpoint=url_endpoint
-        )
+        data = {"queries": queries, "details": details}
+
+        request = Request(method="post", endpoint="/restql/import", data=data)
 
         def response_handler(resp):
-            code = resp.status_code
-            if resp.is_success:
-                # NOTE: server API returns stream name as field 'topic' - we provide both here for user convenience
-                return [{
-                    'name': col['topic'],
-                    'topic': col['topic'],
-                    'local': col['local'],
-                    'db': col['db'],
-                    'tenant': col['tenant'],
-                    'type': StreamCollection.types[col['type']],
-                    'status': 'terminated' if 'terminated' in col else 'active',
-                } for col in map(dict, resp.body['result'])]
-            elif code == 403:
-                raise ex.StreamPermissionError(resp, request)
-            raise ex.StreamConnectionError(resp, request)
+            if not resp.is_success:
+                raise RestqlImportError(resp, request)
+            return resp.body["result"]
 
         return self._execute(request, response_handler)
 
+    def execute_restql(self, name, data=None):
+        """Execute restql by name.
 
-    def nonpersistent_streams(self, local=False):
-        """Get list of all streams under given database
-
-        :param persistent: persistent flag (if it is set to True, the API deletes persistent stream.
-        If it is set to False, API deletes non-persistent stream)
-        :param local: Operate on a local stream instead of a global one. Default value: false
-        :return: List of streams under given database.
-        :rtype: json
-        :raise c8.exceptions.StreamListError: If retrieving streams fails.
+        :param name: restql name
+        :type name: str | unicode
+        :param data: restql data (optional)
+        :type data: dict
+        :returns: Results of execute restql
+        :rtype: dict
+        :raise c8.exceptions.RestqlExecuteError: if restql execution failed
         """
-        url_endpoint = '/streams/non-persistent?local={}'.format(local)
+
+        if data is None or not ("bindVars" in data or "batchSize" in data):
+            data = {}
 
         request = Request(
-            method='get',
-            endpoint=url_endpoint
+            method="post", data=data, endpoint="/restql/execute/{}".format(name)
         )
 
         def response_handler(resp):
-            code = resp.status_code
-            if resp.is_success:
-                # NOTE: server API returns stream name as field 'topic' - we provide both here for user convenience
-                return [{
-                    'name': col['topic'],
-                    'topic': col['topic'],
-                    'local': col['local'],
-                    'db': col['db'],
-                    'tenant': col['tenant'],
-                    'type': StreamCollection.types[col['type']],
-                    'status': 'terminated' if 'terminated' in col else 'active',
-                } for col in map(dict, resp.body['result'])]
-                    
-            elif code == 403:
-                raise ex.StreamPermissionError(resp, request)
-            raise ex.StreamConnectionError(resp, request)
+            if not resp.is_success:
+                raise RestqlExecuteError(resp, request)
+            return resp.body
 
         return self._execute(request, response_handler)
 
+    def read_next_batch_restql(self, id):
+        """Read next batch from query worker cursor.
 
-    def has_stream(self, stream):
-        """ Check if the list of streams has a stream with the given name.
+        :param id: the cursor-identifier
+        :type id: int
+        :returns: Results of execute restql
+        :rtype: dict
+        :raise c8.exceptions.RestqlCursorError: if fetch next batch failed
+        """
 
-        :param stream: The name of the stream for which to check in the list of all streams. 
-        :type stream: str | unicode
-        :return: True=stream found; False=stream not found.
-        :rtype: bool
+        request = Request(method="put", endpoint="/restql/fetch/{}".format(id))
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise RestqlCursorError(resp, request)
+            return resp.body
+
+        return self._execute(request, response_handler)
+
+    def get_all_restql(self):
+        """Get all restql associated for user.
+
+        :returns: Details of all restql
+        :rtype: list
+        :raise c8.exceptions.RestqlListError: if getting restql failed
         """
-        return any(mystream['name'] == stream for mystream in self.streams())
 
+        request = Request(method="get", endpoint="/restql/user")
 
-    def has_persistent_stream(self, stream, local=False):
-        """ Check if the list of persistent streams has a stream with the given name
-        and local setting.
+        def response_handler(resp):
+            if not resp.is_success:
+                raise RestqlListError(resp, request)
+            return resp.body["result"]
 
-        :param stream: The name of the stream for which to check in the list of persistent streams.
-        :type stream: str | unicode
-        :param local: if True, operate on a local stream instead of a global one. Default value: false
-        :type local: bool
-        :return: True=stream found; False=stream not found.
+        return self._execute(request, response_handler)
+
+    def update_restql(self, name, data):
+        """Update restql by name.
+
+        :param name: name of restql
+        :type name: str | unicode
+        :param data: restql data
+        :type data: dict
+        :returns: True if restql is updated
         :rtype: bool
+        :raise c8.exceptions.RestqlUpdateError: if query update failed
         """
-        return any(mystream['name'] == stream for mystream in self.persistent_streams(local))
-        
+        request = Request(method="put", data=data, endpoint="/restql/" + name)
 
-    def has_nonpersistent_stream(self, stream, local=False):
-        """ Check if the list of nonpersistent streams has a stream with the given name
-        and local setting.
+        def response_handler(resp):
+            if not resp.is_success:
+                raise RestqlUpdateError(resp, request)
+            return True
 
-        :param stream: The name of the stream for which to check in the list of nonpersistent streams 
-        :type stream: str | unicode
-        :param local: if True, operate on a local stream instead of a global one. Default value: false
-        :type local: bool
-        :return: True=stream found; False=stream not found.
+        return self._execute(request, response_handler)
+
+    def delete_restql(self, name):
+        """Delete restql by name.
+
+        :param name: restql name
+        :type name: str | unicode
+        :returns: True if restql is deleted
         :rtype: bool
+        :raise c8.exceptions.RestqlDeleteError: if restql deletion failed
         """
-        return any(mystream['name'] == stream for mystream in self.nonpersistent_streams(local))
+        request = Request(method="delete", endpoint="/restql/" + name)
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise RestqlDeleteError(resp, request)
+            return True
+
+        return self._execute(request, response_handler)
+
+    ########################
+    # Events #
+    ########################
 
+    def create_event(self, payload):
+        """Create an event.
 
-    def create_stream(self, stream, persistent=True, local=False):
+        :param payload: Payload to create event
+        :type payload: dict
+        :returns:  Dictionary containing the event id
+        :rtype: dict
+        :raise c8.exceptions.EventCreateError: if event creation failed
+
+        Here is an example entry for parameter **payload**:
+
+        .. code-block:: python
+
+            {
+            "action": "string",
+            "attributes": {},
+            "description": "string",
+            "details": "string",
+            "entityName": "string",
+            "entityType": "string",
+            "status": "string"
+            }
         """
-        Create the stream under the given database
-        :param stream: name of stream
-        :param persistent: persistent flag (if it is set to True, the API creates persistent stream.
-        If it is set to False, API creates non-persistent stream)
-        :param local: Operate on a local stream instead of a global one. Default value: false
-        :return: 200, OK if operation successful
-        :raise: c8.exceptions.StreamDeleteError: If creating streams fails.
+        request = Request(method="post", endpoint="/events", data=payload)
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise EventCreateError(resp, request)
+            return resp.body
+
+        return self._execute(request, response_handler)
+
+    def delete_event(self, eventIds):
+        """Delete an event/s.
+
+        :param eventIds: The event id for which you want to fetch the event details
+        :type eventId: list of strings(event Ids)
+        :returns: List containig all the information of existing events
+        :rtype: list
+        :raise c8.exceptions.EventDeleteError: if event creation failed
+
         """
-        if persistent:
-            url_endpoint = '/streams/' + 'persistent/stream/{}?local={}'.format(stream, local)
-        else:
-            url_endpoint = '/streams/' + 'non-persistent/stream/{}?local={}'.format(stream, local)
-        request = Request(
-            method='post',
-            endpoint=url_endpoint
-        )
+        data = json.dumps((eventIds))
+
+        request = Request(method="delete", endpoint="/events", data=data)
 
         def response_handler(resp):
-            code = resp.status_code
-            if resp.is_success:
-                return resp.body['result']
-            elif code == 502:
-                raise ex.StreamCommunicationError(resp, request)
+            if not resp.is_success:
+                raise EventGetError(resp, request)
+            return True
+
+        return self._execute(request, response_handler)
+
+    def get_all_events(self):
+        """Create an event.
 
-            raise ex.StreamCreateError(resp, request)
+        :returns: List containig all the information of existing events
+        :rtype: list
+        :raise c8.exceptions.EventGetError: if event creation failed
+
+        """
+        request = Request(method="get", endpoint="/events/tenant")
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise EventGetError(resp, request)
+            return resp.body
 
         return self._execute(request, response_handler)
 
-    def delete_stream(self, stream, persistent=True, force=False, local=False):
+    def get_event_by_Id(self, eventId):
+        """Create an event.
+
+        :param eventId: The event id for which you want to fetch the event details
+        :returns: List containig all the information of existing events
+        :rtype: list
+        :raise c8.exceptions.EventGetError: if event creation failed
+
         """
-        Delete the streams under the given database
-        :param stream: name of stream
-        :param persistent: persistent flag (if it is set to True, the API deletes persistent stream.
-        If it is set to False, API deletes non-persistent stream)
-        :param force:
-        :param local: Operate on a local stream instead of a global one. Default value: false
-        :return: 200, OK if operation successful
-        :raise: c8.exceptions.StreamDeleteError: If deleting streams fails.
+        request = Request(method="get", endpoint="/events/" + str(eventId))
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise EventGetError(resp, request)
+            return resp.body
+
+        return self._execute(request, response_handler)
+
+    ########################
+    # Stream Apps #
+    ########################
+
+    def stream_app(self, name):
+        return StreamApps(self._conn, self._executor, name)
+
+    def validate_stream_app(self, data):
+        """validates a stream app by given data
+
+        :param data: stream app defination string
         """
-        # KARTIK : 20181002 : Stream delete not supported. 
-        # We still have some issues to work through for stream deletion on the
-        # pulsar side. So for v0.9.0 we only support terminate, and that too 
-        # only for persistent streams.
-        if not persistent:
-            print("WARNING: Delete not yet implemented for nonpersistent streams. Returning 204. Stream will not be deleted.")
-            # 204 = No Content
-            return 204 
-
-        # Persistent stream, let's terminate it instead.
-        print("WARNING: Delete not yet implemented for persistent streams, calling terminate instead.")
-        return self.terminate_stream(stream=stream, persistent=persistent, local=local)
-
-        ######## HEY HEY DO THE ZOMBIE STOMP ########
-        # KARTIK : 20181002 : Stream delete not supported. 
-        # TODO : When stream delete is implemented, enable below code and 
-        # remove the above code.
-        # Below code is dead code for the moment, until delete stream is 
-        # implemented on the server side. Consider it to be "#if 0"-ed out :-)
-        # (why, yes indeed, that was a C reference)
-        #if force and persistent:
-        #    url_endpoint = '/streams/persistent/stream/{}?force=true&local={}'.format(stream, local)
-        #elif force and not persistent:
-        #    url_endpoint = '/streams/non-persistent/stream/{}?force=true&local={}'.format(stream, local)
-        #elif not force and persistent:
-        #    url_endpoint = '/streams/persistent/stream/{}?local={}'.format(stream, local)
-        #elif not force and not persistent:
-        #    url_endpoint = '/streams/non-persistent/stream/{}?local={}'.format(stream, local)
-        #
-        #request = Request(
-        #    method='delete',
-        #    endpoint=url_endpoint
-        #)
-        #
-        #def response_handler(resp):
-        #    code = resp.status_code
-        #    if resp.is_success:
-        #        return resp.body['result']
-        #    elif code == 403:
-        #        raise ex.StreamPermissionError(resp, request)
-        #    elif code == 412:
-        #        raise ex.StreamDeleteError(resp, request)
-        #    raise ex.StreamConnectionError(resp, request)
-        #
-        #return self._execute(request, response_handler)
+        body = {"definition": data}
+        req = Request(
+            method="post", endpoint="/streamapps/validate", data=json.dumps(body)
+        )
+
+        def response_handler(resp):
+            if resp.is_success is True:
+                return True
+            return False
+
+        return self._execute(req, response_handler)
+
+    def retrieve_stream_app(self):
+        """retrieves all the stream apps of a fabric"""
+        req = Request(
+            method="get",
+            endpoint="/streamapps",
+        )
+
+        def response_handler(resp):
+            if resp.is_success is True:
+                return resp.body
+            return False
+
+        return self._execute(req, response_handler)
+
+    def get_samples_stream_app(self):
+        """gets samples for stream apps"""
+        req = Request(
+            method="get",
+            endpoint="/streamapps/samples",
+        )
+
+        def response_handler(resp):
+            if resp.is_success is not True:
+                raise StreamAppGetSampleError(resp, req)
+            return resp.body["streamAppSample"]
+
+        return self._execute(req, response_handler)
 
-    def terminate_stream(self, stream, persistent=True, local=False):
+    def create_stream_app(self, data, dclist=[]):
+        """Creates a stream application by given data
+
+        :param data: stream app definition
+        :param dclist: regions where stream app has to be deployed
         """
-        Terminate a stream. A stream that is terminated will not accept any more messages to be published and will let consumer to drain existing messages in backlog
-        :param stream: name of stream
-        :param persistent: persistent flag (if it is set to True, the API deletes persistent stream.
-        If it is set to False, API deletes non-persistent stream)
-        :param local: Operate on a local stream instead of a global one. Default value: false
-        :return: 200, OK if operation successful
-        :raise: c8.exceptions.StreamPermissionError: Dont have permission.
+        # create request body
+        req_body = {"definition": data, "regions": dclist}
+        # create request
+        req = Request(method="post", endpoint="/streamapps", data=json.dumps(req_body))
+
+        # create response handler
+
+        def response_handler(resp):
+            if resp.is_success is True:
+                return True
+            return False
+
+        # call api
+        return self._execute(req, response_handler)
+
+    ########################
+    # APIKeys #
+    ########################
+
+    def api_keys(self, keyid):
+        """Return the API keys API wrapper.
+
+        :param keyid: API Key id
+        :type kaeyid: string | unicode
+        :returns: API keys API wrapper.
+        :rtype: c8.stream_collection.StreamCollection
         """
-        if persistent:
-            url_endpoint = '/streams/persistent/stream/{}/terminate?local={}'.format(stream, local)
-        else:
-            # url_endpoint = '/streams/non-persistent/stream/{}/terminate?local={}'.format(stream, local)
-            # KARTIK : 20181002 : terminate not supported for nonpersistent
-            # streams. Just return 204 = No Content
-            print("WARNING: Nonpersistent streams cannot be terminated. Returning 204.")
-            return 204
+        return APIKeys(self._conn, self._executor, keyid)
+
+    def list_all_api_keys(self):
+        """List the API keys.
 
+        :returns:list.
+        :raise c8.exceptions.GetAPIKeys: If request fails
+        """
         request = Request(
-            method='post',
-            endpoint=url_endpoint
+            method="get",
+            endpoint="/key",
         )
 
+        # create response handler
+
         def response_handler(resp):
-            code = resp.status_code
-            if resp.is_success:
-                return resp.body['result']
-            elif code == 403:
-                raise ex.StreamPermissionError(resp, request)
-            raise ex.StreamConnectionError(resp, request)
+            if not resp.is_success:
+                raise GetAPIKeys(resp, request)
+            else:
+                return resp.body["result"]
 
-        return self._execute(request, response_handler)
+        return self._execute(request, response_handler, custom_prefix="/_api")
+
+    ##############################
+    # Search, View and Analyzers #
+    ##############################
+    def search(self):
+        """Returns the Search APIWrapper
+        :returns: Search API Wrapper
+        :rtype: c8.search.Search
+        """
+        return Search(self._conn, self._executor)
 
 
-class StandardDatabase(Database):
-    """Standard database API wrapper.
+class StandardFabric(Fabric):
+    """Standard fabric API wrapper.
 
     :param connection: HTTP connection.
     :type connection: c8.connection.Connection
     """
 
     def __init__(self, connection):
-        super(StandardDatabase, self).__init__(
-            connection=connection,
-            executor=DefaultExecutor(connection)
+        super(StandardFabric, self).__init__(
+            connection=connection, executor=DefaultExecutor(connection)
         )
 
     def __repr__(self):
-        return '<StandardDatabase {}>'.format(self.name)
+        return "<StandardFabric {}>".format(self.name)
 
     def begin_async_execution(self, return_result=True):
         """Begin async execution.
 
         :param return_result: If set to True, API executions return instances
             of :class:`c8.job.AsyncJob`, which you can use to retrieve
             results from server once available. If set to False, API executions
             return None and no results are stored on server.
         :type return_result: bool
-        :return: Database API wrapper built specifically for async execution.
-        :rtype: c8.database.AsyncDatabase
+        :returns: Fabric API wrapper built specifically for async execution.
+        :rtype: c8.fabric.AsyncFabric
         """
-        return AsyncDatabase(self._conn, return_result)
+        return AsyncFabric(self._conn, return_result)
 
     def begin_batch_execution(self, return_result=True):
         """Begin batch execution.
 
         :param return_result: If set to True, API executions return instances
             of :class:`c8.job.BatchJob` that are populated with results on
             commit. If set to False, API executions return None and no results
             are tracked client-side.
         :type return_result: bool
-        :return: Database API wrapper built specifically for batch execution.
-        :rtype: c8.database.BatchDatabase
+        :returns: Fabric API wrapper built specifically for batch execution.
+        :rtype: c8.fabric.BatchFabric
         """
-        return BatchDatabase(self._conn, return_result)
+        return BatchFabric(self._conn, return_result)
 
-    def begin_transaction(self,
-                          return_result=True,
-                          timeout=None,
-                          sync=None,
-                          read=None,
-                          write=None):
-        """Begin transaction.
-
-        :param return_result: If set to True, API executions return instances
-            of :class:`c8.job.TransactionJob` that are populated with
-            results on commit. If set to False, API executions return None and
-            no results are tracked client-side.
-        :type return_result: bool
-        :param read: Names of collections read during transaction. If not
-            specified, they are added automatically as jobs are queued.
-        :type read: [str | unicode]
-        :param write: Names of collections written to during transaction.
-            If not specified, they are added automatically as jobs are queued.
-        :type write: [str | unicode]
-        :param timeout: Timeout for waiting on collection locks. If set to 0,
-            C8Db server waits indefinitely. If not set, system default
-            value is used.
-        :type timeout: int
-        :param sync: Block until the transaction is synchronized to disk.
-        :type sync: bool
-        :return: Database API wrapper built specifically for transactions.
-        :rtype: c8.database.TransactionDatabase
-        """
-        return TransactionDatabase(
-            connection=self._conn,
-            return_result=return_result,
-            read=read,
-            write=write,
-            timeout=timeout,
-            sync=sync
-        )
 
+class AsyncFabric(Fabric):
+    """Fabric API wrapper tailored specifically for async execution.
 
-class AsyncDatabase(Database):
-    """Database API wrapper tailored specifically for async execution.
-
-    See :func:`c8.database.StandardDatabase.begin_async_execution`.
+    See :func:`c8.fabric.StandardFabric.begin_async_execution`.
 
     :param connection: HTTP connection.
     :type connection: c8.connection.Connection
     :param return_result: If set to True, API executions return instances of
         :class:`c8.job.AsyncJob`, which you can use to retrieve results
         from server once available. If set to False, API executions return None
         and no results are stored on server.
     :type return_result: bool
     """
 
     def __init__(self, connection, return_result):
-        super(AsyncDatabase, self).__init__(
-            connection=connection,
-            executor=AsyncExecutor(connection, return_result)
+        super(AsyncFabric, self).__init__(
+            connection=connection, executor=AsyncExecutor(connection, return_result)
         )
 
     def __repr__(self):
-        return '<AsyncDatabase {}>'.format(self.name)
+        return "<AsyncFabric {}>".format(self.name)
 
 
-class BatchDatabase(Database):
-    """Database API wrapper tailored specifically for batch execution.
+class BatchFabric(Fabric):
+    """Fabric API wrapper tailored specifically for batch execution.
 
-    See :func:`c8.database.StandardDatabase.begin_batch_execution`.
+    See :func:`c8.fabric.StandardFabric.begin_batch_execution`.
 
     :param connection: HTTP connection.
     :type connection: c8.connection.Connection
     :param return_result: If set to True, API executions return instances of
         :class:`c8.job.BatchJob` that are populated with results on commit.
         If set to False, API executions return None and no results are tracked
         client-side.
     :type return_result: bool
     """
 
     def __init__(self, connection, return_result):
-        super(BatchDatabase, self).__init__(
-            connection=connection,
-            executor=BatchExecutor(connection, return_result)
+        super(BatchFabric, self).__init__(
+            connection=connection, executor=BatchExecutor(connection, return_result)
         )
 
     def __repr__(self):
-        return '<BatchDatabase {}>'.format(self.name)
+        return "<BatchFabric {}>".format(self.name)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exception, *_):
         if exception is None:
             self._executor.commit()
 
     def queued_jobs(self):
         """Return the queued batch jobs.
 
-        :return: Queued batch jobs or None if **return_result** parameter was
+        :returns: Queued batch jobs or None if **return_result** parameter was
             set to False during initialization.
         :rtype: [c8.job.BatchJob] | None
         """
         return self._executor.jobs
 
     def commit(self):
         """Execute the queued requests in a single batch API request.
 
         If **return_result** parameter was set to True during initialization,
         :class:`c8.job.BatchJob` instances are populated with results.
 
-        :return: Batch jobs, or None if **return_result** parameter was set to
+        :returns: Batch jobs, or None if **return_result** parameter was set to
             False during initialization.
         :rtype: [c8.job.BatchJob] | None
         :raise c8.exceptions.BatchStateError: If batch state is invalid
             (e.g. batch was already committed or the response size did not
             match expected).
         :raise c8.exceptions.BatchExecuteError: If commit fails.
         """
         return self._executor.commit()
-
-
-class TransactionDatabase(Database):
-    """Database API wrapper tailored specifically for transactions.
-
-    See :func:`c8.database.StandardDatabase.begin_transaction`.
-
-    :param connection: HTTP connection.
-    :type connection: c8.connection.Connection
-    :param return_result: If set to True, API executions return instances of
-        :class:`c8.job.TransactionJob` that are populated with results on
-        commit. If set to False, API executions return None and no results are
-        tracked client-side.
-    :type return_result: bool
-    :param read: Names of collections read during transaction.
-    :type read: [str | unicode]
-    :param write: Names of collections written to during transaction.
-    :type write: [str | unicode]
-    :param timeout: Timeout for waiting on collection locks. If set to 0, the
-        C8Db server waits indefinitely. If not set, system default value
-        is used.
-    :type timeout: int
-    :param sync: Block until operation is synchronized to disk.
-    :type sync: bool
-    """
-
-    def __init__(self, connection, return_result, read, write, timeout, sync):
-        super(TransactionDatabase, self).__init__(
-            connection=connection,
-            executor=TransactionExecutor(
-                connection=connection,
-                return_result=return_result,
-                read=read,
-                write=write,
-                timeout=timeout,
-                sync=sync
-            )
-        )
-
-    def __repr__(self):
-        return '<TransactionDatabase {}>'.format(self.name)
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exception, *_):
-        if exception is None:
-            self._executor.commit()
-
-    def queued_jobs(self):
-        """Return the queued transaction jobs.
-
-        :return: Queued transaction jobs, or None if **return_result** was set
-            to False during initialization.
-        :rtype: [c8.job.TransactionJob] | None
-        """
-        return self._executor.jobs
-
-    def commit(self):
-        """Execute the queued requests in a single transaction API request.
-
-        If **return_result** parameter was set to True during initialization,
-        :class:`c8.job.TransactionJob` instances are populated with
-        results.
-
-        :return: Transaction jobs, or None if **return_result** parameter was
-            set to False during initialization.
-        :rtype: [c8.job.TransactionJob] | None
-        :raise c8.exceptions.TransactionStateError: If the transaction was
-            already committed.
-        :raise c8.exceptions.TransactionExecuteError: If commit fails.
-        """
-        return self._executor.commit()
-
```

### Comparing `pyC8-0.9.6/c8/tenant.py` & `pyC8-1.0.0/c8/tenant.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,742 +1,1074 @@
 from __future__ import absolute_import, unicode_literals
 
-from c8.utils import get_col_name
-
-__all__ = ['Tenant']
-
-from datetime import datetime
+import json
 
 from c8.api import APIWrapper
-from c8.request import Request
-from c8.executor import (
-    DefaultExecutor,
-)
-
 from c8.exceptions import (
-    TenantDeleteError,
+    BillingAccessLevel,
+    ClearBillingAccessLevel,
+    ClearCollectionAccessLevel,
+    ClearDataBaseAccessLevel,
+    ClearStreamAccessLevel,
+    CollectionAccessLevel,
+    DataBaseError,
+    GetAttributes,
+    GetDataBaseAccessLevel,
+    ListStreams,
+    PermissionListError,
+    RemoveAllAttributes,
+    RemoveAttribute,
+    SetBillingAccessLevel,
+    SetCollectionAccessLevel,
+    SetDataBaseAccessLevel,
+    SetStreamAccessLevel,
+    SpotRegionAssignError,
+    StreamAccessLevel,
     TenantCreateError,
-    TenantListError,
     TenantDcListError,
+    TenantDeleteError,
+    TenantDetailsError,
+    TenantListError,
     TenantUpdateError,
-    DatabaseListError,
-    DatabaseCreateError,
-    DatabaseDeleteError,
-    PermissionListError,
-    PermissionGetError,
-    PermissionResetError,
-    PermissionUpdateError,
+    UpdateAttributes,
     UserCreateError,
     UserDeleteError,
     UserGetError,
     UserListError,
-    UserReplaceError,
     UserUpdateError,
 )
+from c8.executor import DefaultExecutor
+from c8.fabric import StandardFabric
+from c8.request import Request
 
+__all__ = ["Tenant"]
 
 
 class Tenant(APIWrapper):
     """Base class for Tenant API wrappers.
 
     :param connection: HTTP connection.
     :type connection: c8.connection.Connection
     :param executor: API executor.
     :type executor: c8.executor.Executor
     """
 
     def __init__(self, connection):
-        self._auth_tok = ""
-        super(Tenant, self).__init__(connection, executor=DefaultExecutor(connection))
 
+        super(Tenant, self).__init__(connection, executor=DefaultExecutor(connection))
+        # self.get_auth_token_from_server()
 
     @property
     def name(self):
         """Return tenant name.
 
-        :return: tenant name.
+        :returns: tenant name.
         :rtype: str | unicode
         """
         return self.tenant_name
 
-
     def get_auth_token_from_server(self):
+
         """
         Returns the JWT auth token which can be used in subsequent requests
         The login for the auth token is done using the username and password
         for the current tenant object.
         """
         # Do an auth login. We need to rewrite the connection's standard URL
         # prefix because the /_open/auth call does not expect anything past
         # the '_tenant/{tenantname}' part of the URL. So we rewrite it here
         # temporarily to do the auth call, then set it back
         oldconnprefix = self._conn.url_prefix
-        proto = oldconnprefix.split('//')[0]
-        rema = oldconnprefix.split('//')[1].split('/')[0]
+        proto = oldconnprefix.split("//")[0]
+        rema = oldconnprefix.split("//")[1].split("/")[0]
 
         # We set the temp URL prefix here for the auth call. It is restored
         # below
-        self._conn.set_url_prefix(proto+'//'+rema+'/_database/_tenant/'+self.tenant_name)
-        data = {"tenant":self.tenant_name}
-        data['username'] = self._conn.username
-        data['password'] = self._conn._auth[1]
-        request = Request(
-            method='post',
-            endpoint='/_open/auth',
-            data=data
-        )
+        self._conn.set_url_prefix(proto + "//" + rema)
+        data = {"tenant": self.tenant_name}
+        data["email"] = self._conn._email
+        data["password"] = self._conn._password
+        request = Request(method="post", endpoint="/_open/auth", data=data)
 
         def response_handler(resp):
             if not resp.is_success:
-                raise TenantListError
-            if 'jwt' not in resp.body:
-                raise TenantListError
-            return resp.body['jwt']
+                raise "Authentication Error"
+            if "jwt" not in resp.body:
+                raise "Failed to fetch jwt"
+            return resp.body["jwt"]
 
         tok = self._execute(request, response_handler)
-        # NOTE : Set tok as _self.auth_tok so other functions can pass self._auth.tok
-        # to the request object as the Request.auth_tok field. See request.py
-        self._auth_tok = tok
-
-        # Print the auth token
-        #print("TENANT INIT: "+self.tenant_name+" : Token: "+tok)
+        # NOTE : Set tok as _self.auth_tok so other functions can pass
+        # self._auth.tok to the request object as the Request.auth_tok field.
+        self._conn._auth_token = tok
 
         # Set the connection object's url prefix back to what it was.
         self._conn.set_url_prefix(oldconnprefix)
 
-
     @property
     def auth_token(self):
         """Return the stored JWT auth token for this tenant & user, if stored.
         This will be stored after calling get_auth_token_from_server() above.
 
-        :return: JWT auth token stored for this tenant user
+        :returns: JWT auth token stored for this tenant user
         :rtype: str | unicode
         """
-        return self._auth_tok
+        return self._conn._auth_token
 
+    def useFabric(self, fabric_name):
+        conn = self._conn
+        conn.set_fabric_name(fabric_name)
+        url_prefix = "{}/_fabric/{}/_api".format(conn.url, conn.fabric_name)
+        conn.set_url_prefix(url_prefix)
+        fabric = StandardFabric(conn)
+        return fabric
 
     #######################
     # Tenant Management #
     #######################
 
     def tenants(self):
         """Return the names all tenants.
 
-        :return: Tenant names.
+        :returns: Tenant names.
         :rtype: [str | unicode]
         :raise c8.exceptions.TenantListError: If retrieval fails.
         """
+        self.auth_token
         request = Request(
-            method='get',
-            endpoint='/_api/tenants'
+            method="get",
+            endpoint="/_api/tenants",
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise TenantListError(resp, request)
-            #print("tenants() : Response body: " + str(resp.body))
             retval = []
-            for item in resp.body['result']:
-                retval.append(item['tenant'])
+            for item in resp.body["result"]:
+                retval.append(item["tenant"])
             return retval
 
-        return self._execute(request, response_handler)
+        return self._execute(request, response_handler, custom_prefix="")
 
     def has_tenant(self, name):
         """Check if a tenant exists.
 
         :param name: Tenant name.
         :type name: str | unicode
-        :return: True if tenant exists, False otherwise.
+        :returns: True if tenant exists, False otherwise.
         :rtype: bool
         """
         return name in self.tenants()
 
-    def create_tenant(self, name, passwd='', extra={}):
+    def create_tenant(
+        self,
+        email,
+        display_name=None,
+        passwd="",
+        plan=None,
+        attribution=None,
+        dclist=[],
+        metadata={},
+        contact={},
+    ):
         """Create a new tenant.
-        :param name: Tenant name.
-        :type name: str | unicode
-        :param passwd: What I presume is the tenant admin user password.
-        :param extra: Extra config info.
-        :type extra: [dict]
-        :return: True if tenant was created successfully.
-        :rtype: bool
+
+        :param email: Tenant email address.
+        :type email: str | unicode
+        :param display_name: Tenant display name.
+        :type display_name: str | unicode
+        :param passwd: Tenant password to be set.
+        :type passwd: str
+        :param plan: Tenant plan to be set (example: FREE, METERED, ENTERPRISE).
+        :type plan: str | unicode
+        :param attribution: Tenant attribution (example: Macrometa, Cox-Edge).
+        :type attribution: str | unicode
+        :param dclist: comma separated list of region where the tenant will be
+                       created. If no value passed tenant will be created
+                       globally.
+        :type dclist: list
+        :param metadata: Metadata info.
+        :type metadata: dict
+        :param contact: Contact info.
+        :type contact: dict
+        :returns: Created tenant details if creation was successful
+        :rtype: dict
         :raise c8.exceptions.TenantCreateError: If create fails.
+        """
+        data = {}
+        if display_name is not None:
+            data["displayName"] = display_name
+        data["email"] = email
+        data["passwd"] = passwd
+        if plan is not None:
+            data["plan"] = plan.upper()
+        if attribution is not None:
+            data["attribution"] = attribution
+        data["metadata"] = metadata
+        data["contact"] = contact
+        if dclist != "":
+            data["dcList"] = dclist
 
-        Here is an example entry for parameter **users**:
+        request = Request(method="post", endpoint="/_api/tenant", data=data)
 
-        .. code-block:: python
+        def response_handler(resp):
+            if not resp.is_success:
+                raise TenantCreateError(resp, request)
+            return resp.body
 
-            {
-                'username': 'john',
-                'password': 'password',
-                'active': True,
-                'extra': {'Department': 'IT'}
-            }
+        return self._execute(request, response_handler, custom_prefix="")
+
+    def update_tenant(
+        self, name, active=True, status="active", display_name=None, metadata=None
+    ):
+        """Update an existing tenant.
+
+        :param name: Tenant name.
+        :type name: str | unicode
+        :param active: Whether the tenant is active or not.
+        :type active: bool
+        :param status: The current status of the tenant.
+        :type status: str | unicode
+        :param display_name: Display name of the tenant
+        :type display_name: str | unicode
+        :param metadata: Metadata info.
+        :type metadata: [dict]
+        :returns: True if the update was successful else False.
+        :rtype: bool
+        :raise c8.exceptions.TenantUpdateError: If update fails.
         """
-        data = {'name': name}
-        data['passwd'] = passwd
-        data['extra'] = extra
+        data = {}
+        data["active"] = active
+        data["status"] = status
+        if display_name is not None:
+            data["displayName"] = display_name
+        if metadata is not None:
+            data["metadata"] = metadata
 
         request = Request(
-            method='post',
-            endpoint='/_api/tenant',
-            data=data
+            method="patch",
+            endpoint="/_api/tenant/{tenantname}".format(tenantname=name),
+            data=data,
         )
 
         def response_handler(resp):
             if not resp.is_success:
-                raise TenantCreateError(resp, request)
+                raise TenantUpdateError(resp, request)
             return True
 
-        return self._execute(request, response_handler)
-    
-    def update_tenant(self, name, passwd='', extra={}):
-        """Update a existing tenant.
-        :param name: Tenant name.
-        :type name: str | unicode
-        :param passwd: What I presume is the tenant admin user password.
-        :param extra: Extra config info.
-        :type extra: [dict]
-        :return: True if tenant was created successfully.
-        :rtype: bool
-        :raise c8.exceptions.TenantCreateError: If create fails.
-
-        Here is an example entry for parameter **users**:
+        return self._execute(request, response_handler, custom_prefix="")
 
-        .. code-block:: python
+    def get_tenant_details(self, name):
+        """Get the details of the tenant.
 
-            {
-                'username': 'john',
-                'password': 'password',
-                'active': True,
-                'extra': {'Department': 'IT'}
-            }
+        :param name: Tenant name.
+        :type name: str | unicode
+        :returns: Tenant Details
+        :rtype: dict
+        :raise c8.exceptions.TenantDetailsError: If retrieval of details fails.
         """
-        data = {'name': name}
-        data['passwd'] = passwd
-        data['extra'] = extra
-
         request = Request(
-            method='patch',
-            endpoint='/_api/tenant/{tenantname}'.format(tenantname=name),
-            data=data
+            method="get", endpoint="/_api/tenant/{tenantname}".format(tenantname=name)
         )
 
         def response_handler(resp):
             if not resp.is_success:
-                raise TenantUpdateError(resp, request)
-            return True
+                raise TenantDetailsError(resp, request)
+            return resp.body["result"]
 
-        return self._execute(request, response_handler)
+        return self._execute(request, response_handler, custom_prefix="")
 
     def delete_tenant(self, name, ignore_missing=False):
         """Delete the tenant.
+
         :param name: Tenant name.
         :type name: str | unicode
         :param ignore_missing: Do not raise an exception on missing tenant.
         :type ignore_missing: bool
-        :return: True if tenant was deleted successfully, False if tenant
+        :returns: True if tenant was deleted successfully, False if tenant
             was not found and **ignore_missing** was set to True.
         :rtype: bool
         :raise c8.exceptions.TenantDeleteError: If delete fails.
         """
         request = Request(
-            method='delete',
-            endpoint='/_api/tenant/{tenantname}'.format(tenantname=name)
+            method="delete",
+            endpoint="/_api/tenant/{tenantname}".format(tenantname=name),
         )
 
         def response_handler(resp):
-            #print("DELETE TENANT: RESP BODY IS: "+str(resp.body)) # TODO REMOVE FROM PRODUCTION
             if resp.error_code == 1228 and ignore_missing:
                 return False
             if not resp.is_success:
                 raise TenantDeleteError(resp, request)
-            return resp.body['result']
+            return resp.body["result"]
 
-        return self._execute(request, response_handler)
+        return self._execute(request, response_handler, custom_prefix="")
 
+    def dclist(self, detail=False):
+        """Return the list of names of Datacenters
 
-    def dclist(self):
-        """Return the list of Datacenters
-
-        :return: DC List.
+        :param detail: detail list of DCs if set to true else only DC names
+        :type: boolean
+        :returns: DC List.
         :rtype: [str | unicode ]
         :raise c8.exceptions.TenantListError: If retrieval fails.
         """
-        request = Request(
-            method='get',
-            endpoint='/_api/datacenter/all'
-        )
+        request = Request(method="get", endpoint="/datacenter/_tenant/%s" % self.name)
 
         def response_handler(resp):
-            #print("dclist() : Response body: " + str(resp.body))
             if not resp.is_success:
                 raise TenantDcListError(resp, request)
+            if detail:
+                return resp.body[0]["dcInfo"]
             dc_list = []
-            for dc in resp.body:
-                dc_list.append(dc['name'])
+            for dc in resp.body[0]["dcInfo"]:
+                dc_list.append(dc["name"])
             return dc_list
 
-        return self._execute(request, response_handler)
+        return self._execute(request, response_handler, custom_prefix="")
 
-    def dclist_local(self):
+    def localdc(self, detail=True):
         """Return the list of local Datacenters
 
-        :return: DC List.
-        :rtype: [str | unicode ]
+        :param detail: detail list of DCs if set to true else only DC names
+        :type detail: boolean
+        :returns: DC List.
+        :rtype: [str | dict ]
         :raise c8.exceptions.TenantListError: If retrieval fails.
         """
-        request = Request(
-            method='get',
-            endpoint='/_api/datacenter/local'
-        )
+        request = Request(method="get", endpoint="/datacenter/local")
 
         def response_handler(resp):
-            #print("dclist() : Response body: " + str(resp.body))
             if not resp.is_success:
                 raise TenantDcListError(resp, request)
-            return resp.body
-
-        return self._execute(request, response_handler)
-
-    #######################
-    # Database Management #
-    #######################
-
-    def databases(self):
-        """Return the names all databases.
-
-        :return: Database names.
-        :rtype: [str | unicode]
-        :raise c8.exceptions.DatabaseListError: If retrieval fails.
-        """
-        request = Request(
-            method='get',
-            endpoint='/_api/database'
-        )
-
-        def response_handler(resp):
-            if not resp.is_success:
-                raise DatabaseListError(resp, request)
-            return resp.body['result']
-
-        return self._execute(request, response_handler)
-
-    def has_database(self, name):
-        """Check if a database exists.
-
-        :param name: Database name.
-        :type name: str | unicode
-        :return: True if database exists, False otherwise.
-        :rtype: bool
-        """
-        return name in self.databases()
-
-    def create_database(self, name, users=None, dclist=None, realtime=False):
-        """Create a new database.
-
-        :param name: Database name.
-        :type name: str | unicode
-        :param users: List of users with access to the new database, where each
-            user is a dictionary with fields "username", "password", "active"
-            and "extra" (see below for example). If not set, only the admin and
-            current user are granted access.
-        :type users: [dict]
-        :param dclist : list of strings of datacenters
-        :type dclist: [str | unicode]
-        :param realtime: Whether or not the DB is realtime-enabled.
-        :type realtime: bool
-        :return: True if database was created successfully.
+            if detail:
+                return resp.body
+            return resp.body["name"]
+
+        return self._execute(request, response_handler, custom_prefix="")
+
+    def assign_dc_spot(self, dc, spot_region=False):
+        """Assigns spot region of a fed
+
+        :param dc: dc name
+        :type dc: str
+        :param spot_region: If True, makes the region a spot region
+        :type spot_region: bool
+        :returns: True if request successful, False otherwise
         :rtype: bool
-        :raise c8.exceptions.DatabaseCreateError: If create fails.
-
-        Here is an example entry for parameter **users**:
-
-        .. code-block:: python
-
-            {
-                'username': 'john',
-                'password': 'password',
-                'active': True,
-                'extra': {'Department': 'IT'}
-            }
+        :raise c8.exceptions.SpotRegionAssignError: If assignment fails.
         """
-        data = {'name': name}
-        if users is not None:
-            data['users'] = [{
-                'username': user['username'],
-                'passwd': user['password'],
-                'active': user.get('active', True),
-                'extra': user.get('extra', {})
-            } for user in users]
-
-        options = {}
-        options['realTime'] = realtime
-
-        if dclist:
-            # Process dclist param (type list) to build up comma-separated string of DCs
-            dcl = ''
-            for dc in dclist:
-                if len(dcl) > 0:
-                    dcl += ','
-                dcl += dc
-            options['dcList'] = dcl
-
-        data['options'] = options
-
-        request = Request(
-            method='post',
-            endpoint='/_api/database',
-            data=data
-        )
+        data = json.dumps(spot_region)
+        request = Request(method="put", endpoint="/datacenter/{}/{}".format(dc, data))
 
         def response_handler(resp):
             if not resp.is_success:
-                raise DatabaseCreateError(resp, request)
+                raise SpotRegionAssignError(resp, request)
             return True
 
-        return self._execute(request, response_handler)
-
-    def delete_database(self, name, ignore_missing=False):
-        """Delete the database.
-
-        :param name: Database name.
-        :type name: str | unicode
-        :param ignore_missing: Do not raise an exception on missing database.
-        :type ignore_missing: bool
-        :return: True if database was deleted successfully, False if database
-            was not found and **ignore_missing** was set to True.
-        :rtype: bool
-        :raise c8.exceptions.DatabaseDeleteError: If delete fails.
-        """
-        request = Request(
-            method='delete',
-            endpoint='/_api/database/{}'.format(name)
-        )
-
-        def response_handler(resp):
-            if resp.error_code == 1228 and ignore_missing:
-                return False
-            if not resp.is_success:
-                raise DatabaseDeleteError(resp, request)
-            return resp.body['result']
-
-        return self._execute(request, response_handler)
+        return self._execute(request, response_handler, custom_prefix="")
 
     ###################
     # User Management #
     ###################
 
     def has_user(self, username):
         """Check if user exists.
 
         :param username: Username.
         :type username: str | unicode
-        :return: True if user exists, False otherwise.
+        :returns: True if user exists, False otherwise.
         :rtype: bool
         """
-        return any(user['username'] == username for user in self.users())
+        return any(user["username"] == username for user in self.users())
 
     def users(self):
         """Return all user details.
 
-        :return: List of user details.
+        :returns: List of user details.
         :rtype: [dict]
         :raise c8.exceptions.UserListError: If retrieval fails.
         """
-        request = Request(
-            method='get',
-            endpoint='/_admin/user'
-        )
+        request = Request(method="get", endpoint="/user")
 
         def response_handler(resp):
             if not resp.is_success:
                 raise UserListError(resp, request)
-            return [{
-                'username': record['user'],
-                'active': record['active'],
-                'extra': record['extra'],
-            } for record in resp.body['result']]
+            return [
+                {
+                    "display_name": record["displayName"],
+                    "email": record["email"],
+                    "username": record["user"],
+                    "active": record["active"],
+                    "extra": record["extra"],
+                }
+                for record in resp.body["result"]
+            ]
 
-        return self._execute(request, response_handler)
+        return self._execute(request, response_handler, custom_prefix="/_api")
 
     def user(self, username):
         """Return user details.
 
         :param username: Username.
         :type username: str | unicode
-        :return: User details.
+        :returns: User details.
         :rtype: dict
         :raise c8.exceptions.UserGetError: If retrieval fails.
         """
-        request = Request(
-            method='get',
-            endpoint='/_admin/user/{}'.format(username)
-        )
+        request = Request(method="get", endpoint="/user/{}".format(username))
 
         def response_handler(resp):
-            #print("TENANT USER DETAILS RESP BODY: "+str(resp.body))
             if not resp.is_success:
                 raise UserGetError(resp, request)
             return {
-                'username': resp.body['user'],
-                'active': resp.body['active'],
-                'extra': resp.body['extra']
+                "display_name": resp.body["displayName"],
+                "email": resp.body["email"],
+                "username": resp.body["user"],
+                "active": resp.body["active"],
+                "extra": resp.body["extra"],
             }
 
-        return self._execute(request, response_handler)
+        return self._execute(request, response_handler, custom_prefix="/_api")
 
-    def create_user(self, username, password, active=True, extra=None):
+    def create_user(self, email, password, display_name=None, active=True, extra=None):
         """Create a new user.
 
-        :param username: Username.
-        :type username: str | unicode
-        :param password: Password.
+        :param email: Email address of the user.
+        :type email: str | unicode
+        :param password: Password to be set for the user.
         :type password: str | unicode
+        :param display_name: Display name for the user.
+        :type display_name: str | unicode
         :param active: True if user is active, False otherwise.
         :type active: bool
         :param extra: Additional data for the user.
         :type extra: dict
-        :return: New user details.
+        :returns: New user details.
         :rtype: dict
         :raise c8.exceptions.UserCreateError: If create fails.
         """
-        data = {'user': username, 'passwd': password, 'active': active}
+        data = {"email": email, "passwd": password, "active": active}
+        if display_name is not None:
+            data["displayName"] = display_name
         if extra is not None:
-            data['extra'] = extra
+            data["extra"] = extra
 
-        request = Request(
-            method='post',
-            endpoint='/_admin/user',
-            data=data
-        )
+        request = Request(method="post", endpoint="/user", data=data)
 
         def response_handler(resp):
             if not resp.is_success:
                 raise UserCreateError(resp, request)
             return {
-                'username': resp.body['user'],
-                'active': resp.body['active'],
-                'extra': resp.body['extra'],
+                "display_name": resp.body["displayName"],
+                "email": resp.body["email"],
+                "username": resp.body["user"],
+                "active": resp.body["active"],
+                "extra": resp.body["extra"],
+                "tenant": resp.body["tenant"],
             }
 
-        return self._execute(request, response_handler)
+        return self._execute(request, response_handler, custom_prefix="/_api")
 
-    def update_user(self, username, password=None, active=None, extra=None):
+    def update_user(
+        self,
+        username,
+        password=None,
+        display_name=None,
+        email=None,
+        is_verified=None,
+        active=None,
+        extra=None,
+    ):
         """Update a user.
 
         :param username: Username.
         :type username: str | unicode
         :param password: New password.
         :type password: str | unicode
+        :param display_name: New display name for the user.
+        :type display_name: str | unicode
+        :param email: New email for the user.
+        :type email: str | unicode
+        :param is_verified: Whether the email is verified or not.
+        :type is_verified: bool
         :param active: Whether the user is active.
         :type active: bool
         :param extra: Additional data for the user.
         :type extra: dict
-        :return: New user details.
+        :returns: New user details.
         :rtype: dict
         :raise c8.exceptions.UserUpdateError: If update fails.
         """
         data = {}
         if password is not None:
-            data['passwd'] = password
+            data["passwd"] = password
+        if display_name is not None:
+            data["displayName"] = display_name
+        if email is not None and is_verified is not None:
+            new_email = {"email": email, "isVerified": is_verified}
+            data["newEmail"] = new_email
         if active is not None:
-            data['active'] = active
+            data["active"] = active
         if extra is not None:
-            data['extra'] = extra
+            data["extra"] = extra
 
         request = Request(
-            method='patch',
-            endpoint='/_admin/user/{user}'.format(user=username),
-            data=data
+            method="patch", endpoint="/user/{user}".format(user=username), data=data
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise UserUpdateError(resp, request)
             return {
-                'username': resp.body['user'],
-                'active': resp.body['active'],
-                'extra': resp.body['extra'],
+                "display_name": resp.body["displayName"],
+                "email": resp.body["email"],
+                "username": resp.body["user"],
+                "active": resp.body["active"],
+                "extra": resp.body["extra"],
             }
 
-        return self._execute(request, response_handler)
-
-    def replace_user(self, username, password, active=None, extra=None):
-        """Replace a user.
-
-        :param username: Username.
-        :type username: str | unicode
-        :param password: New password.
-        :type password: str | unicode
-        :param active: Whether the user is active.
-        :type active: bool
-        :param extra: Additional data for the user.
-        :type extra: dict
-        :return: New user details.
-        :rtype: dict
-        :raise c8.exceptions.UserReplaceError: If replace fails.
-        """
-        data = {'user': username, 'passwd': password}
-        if active is not None:
-            data['active'] = active
-        if extra is not None:
-            data['extra'] = extra
-
-        request = Request(
-            method='put',
-            endpoint='/_admin/user/{user}'.format(user=username),
-            data=data
-        )
-
-        def response_handler(resp):
-            if resp.is_success:
-                return {
-                    'username': resp.body['user'],
-                    'active': resp.body['active'],
-                    'extra': resp.body['extra'],
-                }
-            raise UserReplaceError(resp, request)
-
-        return self._execute(request, response_handler)
+        return self._execute(request, response_handler, custom_prefix="/_api")
 
     def delete_user(self, username, ignore_missing=False):
         """Delete a user.
 
         :param username: Username.
         :type username: str | unicode
         :param ignore_missing: Do not raise an exception on missing user.
         :type ignore_missing: bool
-        :return: True if user was deleted successfully, False if user was not
+        :returns: True if user was deleted successfully, False if user was not
             found and **ignore_missing** was set to True.
         :rtype: bool
         :raise c8.exceptions.UserDeleteError: If delete fails.
         """
         request = Request(
-            method='delete',
-            endpoint='/_admin/user/{user}'.format(user=username)
+            method="delete", endpoint="/user/{user}".format(user=username)
         )
 
         def response_handler(resp):
             if resp.is_success:
                 return True
             elif resp.status_code == 404 and ignore_missing:
                 return False
             raise UserDeleteError(resp, request)
 
-        return self._execute(request, response_handler)
+        return self._execute(request, response_handler, custom_prefix="/_api")
 
-    #########################
-    # Permission Management #
-    #########################
-
-    def permissions(self, username):
-        """Return user permissions for all databases and collections.
+    def list_accessible_databases_user(self, username, full=False):
+        """Lists accessible databases for a user.
 
         :param username: Username.
         :type username: str | unicode
-        :return: User permissions for all databases and collections.
-        :rtype: dict
-        :raise: c8.exceptions.PermissionListError: If retrieval fails.
+        :param full: Return the full set of access levels for all databases
+                and all collections if set to true.
+        :type full: bool
+        :returns: Object containing database details
+        :rtype: list | object
+        :raise c8.exceptions.DataBaseError: If request fails.
         """
         request = Request(
-            method='get',
-            endpoint='/_admin/user/{}/database'.format(username),
-            params={'full': True}
+            method="get", endpoint="/user/{}/database?full={}".format(username, full)
         )
 
         def response_handler(resp):
             if resp.is_success:
-                return resp.body['result']
-            raise PermissionListError(resp, request)
+                return resp.body["result"]
+            raise DataBaseError(resp, request)
 
-        return self._execute(request, response_handler)
+        return self._execute(request, response_handler, custom_prefix="/_api")
 
-    def permission(self, username, database, collection=None):
-        """Return user permission for a specific database or collection.
+    def get_database_access_level_user(self, username, databasename=""):
+        """Fetch the access level for a specific database.
 
         :param username: Username.
         :type username: str | unicode
-        :param database: database name.
-        :type database: str | unicode
-        :param collection: Collection name.
-        :type collection: str | unicode
-        :return: Permission for given database or collection.
-        :rtype: str | unicode
-        :raise: c8.exceptions.PermissionGetError: If retrieval fails.
+        :param databasename: Database name.
+        :type databasename: str | unicode
+        :returns: Access Details
+        :rtype: string
+        :raise c8.exceptions.GetDataBaseAccessLevel: If request fails.
         """
-        endpoint = '/_admin/user/{}/database/{}'.format(username, database)
-        if collection is not None:
-            endpoint += '/' + collection
-        request = Request(method='get', endpoint=endpoint)
+        request = Request(
+            method="get", endpoint="/user/{}/database/{}".format(username, databasename)
+        )
 
         def response_handler(resp):
-            if not resp.is_success:
-                raise PermissionGetError(resp, request)
-            return resp.body['result']
+            if resp.is_success:
+                return resp.body["result"]
+            raise GetDataBaseAccessLevel(resp, request)
 
-        return self._execute(request, response_handler)
+        return self._execute(request, response_handler, custom_prefix="/_api")
 
-    def update_permission(self,
-                          username,
-                          permission,
-                          database,
-                          collection=None):
-        """Update user permission for a specific database or collection.
+    def remove_database_access_level_user(self, username, databasename=""):
+        """Clear the access level for the specific database of user.
+        As consequence the default database access level is used.
 
         :param username: Username.
         :type username: str | unicode
-        :param database: database name.
-        :type database: str | unicode
-        :param collection: Collection name.
-        :type collection: str | unicode
-        :param permission: Allowed values are "rw" (read and write), "ro"
-            (read only) or "none" (no access).
-        :type permission: str | unicode
-        :return: True if access was granted successfully.
-        :rtype: bool
-        :raise c8.exceptions.PermissionUpdateError: If update fails.
+        :param databasename: Database name.
+        :type databasename: str | unicode
+        :returns: Object containing database details
+        :rtype: object
+        :raise c8.exceptions.ClearDataBaseAccessLevel: If request fails.
         """
-        endpoint = '/_admin/user/{}/database/{}'.format(username, database)
-        if collection is not None:
-            endpoint += '/' + collection
-
         request = Request(
-            method='put',
-            endpoint=endpoint,
-            data={'grant': permission}
+            method="delete",
+            endpoint="/user/{}/database/{}".format(username, databasename),
         )
 
         def response_handler(resp):
             if resp.is_success:
                 return True
-            raise PermissionUpdateError(resp, request)
+            raise ClearDataBaseAccessLevel(resp, request)
 
-        return self._execute(request, response_handler)
+        return self._execute(request, response_handler, custom_prefix="/_api")
 
-    def reset_permission(self, username, database, collection=None):
-        """Reset user permission for a specific database or collection.
+    def set_database_access_level_user(self, username, databasename="", grant="ro"):
+        """Set the access levels for the specific database of user.
 
         :param username: Username.
         :type username: str | unicode
-        :param database: database name.
-        :type database: str | unicode
-        :param collection: Collection name.
-        :type collection: str | unicode
-        :return: True if permission was reset successfully.
-        :rtype: bool
-        :raise c8.exceptions.PermissionRestError: If reset fails.
+        :param databasename: Database name.
+        :type databasename: str | unicode
+        :param grant: Grant accesslevel.
+                    Use "rw" to set the database access level to Administrate .
+                    Use "ro" to set the database access level to Access.
+                    Use "none" to set the database access level to No access.
+        :type grant: string
+        :returns: Object containing database details
+        :rtype: object
+        :raise c8.exceptions.SetDataBaseAccessLevel: If request fails.
+        """
+        request = Request(
+            method="put",
+            endpoint="/user/{}/database/{}".format(username, databasename),
+            data={"grant": grant},
+        )
+
+        def response_handler(resp):
+            if resp.is_success:
+                return resp.body
+            raise SetDataBaseAccessLevel(resp, request)
+
+        return self._execute(request, response_handler, custom_prefix="/_api")
+
+    def list_accessible_collections_user(
+        self, username, databasename="_system", full=False
+    ):
+        """Fetch the collection access level for a specific collection in a database.
+
+        :param username: Name of the user
+        :type username: string
+        :param databasename: Name of the database
+        :type databasename: string
+        :param full: Return the full set of access levels for all collections.
+        :type full: boolean
+        :returns: Fetch the list of collections access level for a specific user.
+        :rtype: string
+        :raise c8.exceptions.CollectionAccessLevel: If request fails.
+        """
+        request = Request(
+            method="get",
+            endpoint="/user/{}/database/{}/collection?full={}".format(
+                username, databasename, full
+            ),
+        )
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise CollectionAccessLevel(resp, request)
+            else:
+                return resp.body["result"]
+
+        return self._execute(request, response_handler, custom_prefix="/_api")
+
+    def get_collection_access_level_user(
+        self, username, collection_name, databasename="_system"
+    ):
+        """Fetch the collection access level for a specific collection in a database.
+
+        :param collection_name: Name of the collection
+        :type collection_name: string
+        :param databasename: Name of the database
+        :type databasename: string
+        :returns: AccessLevel of a db.
+        :rtype: string
+        :raise c8.exceptions.CollectionAccessLevel: If request fails.
+        """
+        request = Request(
+            method="get",
+            endpoint="/user/{}/database/{}/collection/{}".format(
+                username, databasename, collection_name
+            ),
+        )
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise CollectionAccessLevel(resp, request)
+            else:
+                return resp.body["result"]
+
+        return self._execute(request, response_handler, custom_prefix="/_api")
+
+    def set_collection_access_level_user(
+        self, username, collection_name, databasename="_system", grant="ro"
+    ):
+
+        """Set the collection access level for a specific collection in a database.
+
+        :param collection_name: Name of the collection
+        :type collection_name: string
+        :param databasename: Name of the database
+        :type databasename: string
+        :param grant: Use "rw" to set the database access level to Administrate .
+                      Use "ro" to set the database access level to Access.
+                      Use "none" to set the database access level to No access.
+        :type grant: string
+        :returns: Accesslevel of a particular db.
+        :rtype: Object
+        :raise c8.exceptions.SetCollectionAccessLevel: If request fails.
+        """
+        request = Request(
+            method="put",
+            endpoint="/user/{}/database/{}/collection/{}".format(
+                username, databasename, collection_name
+            ),
+            data={"grant": grant},
+        )
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise SetCollectionAccessLevel(resp, request)
+            else:
+                return resp.body
+
+        return self._execute(request, response_handler, custom_prefix="/_api")
+
+    def clear_collection_access_level_user(
+        self, username, collection_name, databasename="_system"
+    ):
+
+        """Clear the collection access level for a specific collection in a database.
+
+        :param collection_name: Name of the collection
+        :type collection_name: string
+        :param databasename: Name of the database
+        :type databasename: string
+        :returns: True if operation successful.
+        :rtype: booleaan
+        :raise c8.exceptions.ClearCollectionAccessLevel: If request fails.
+        """
+        request = Request(
+            method="delete",
+            endpoint="/user/{}/database/{}/collection/{}".format(
+                username, databasename, collection_name
+            ),
+        )
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise ClearCollectionAccessLevel(resp, request)
+            else:
+                if resp.body["error"] is False:
+                    return True
+                elif resp.body["error"] is True:
+                    return False
+
+        return self._execute(request, response_handler, custom_prefix="/_api")
+
+    def list_accessible_streams_user(
+        self, username, databasename="_system", full=False
+    ):
+        """Fetch the list of streams available to the specified user.
+
+        :param databasename: Name of the database
+        :type databasename: string
+        :param full: Return the full set of access levels for all streams.
+        :type full: boolean
+        :returns: List of available databases.
+        :rtype: list
+        :raise c8.exceptions.ListStreams: If request fails.
+        """
+        request = Request(
+            method="get",
+            endpoint="/user/{}/database/{}/stream?full={}".format(
+                username, databasename, full
+            ),
+        )
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise ListStreams(resp, request)
+            else:
+                return resp.body["result"]
+
+        return self._execute(request, response_handler, custom_prefix="/_api")
+
+    def get_stream_access_level_user(
+        self, username, streamname, databasename="_system"
+    ):
+        """Fetch the database access level for a specific stream.
+
+        :param streamname: Name of the stream
+        :type streamname: string
+        :param databasename: Name of the database
+        :type databasename: string
+        :returns: AccessLevel of a db.
+        :rtype: string
+        :raise c8.exceptions.StreamAccessLevel: If request fails.
+        """
+
+        request = Request(
+            method="get",
+            endpoint="/user/{}/database/{}/stream/{}".format(
+                username, databasename, streamname
+            ),
+        )
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise StreamAccessLevel(resp, request)
+            else:
+                return resp.body["result"]
+
+        return self._execute(request, response_handler, custom_prefix="/_api")
+
+    def set_stream_access_level_user(
+        self, username, streamname, databasename="_system", grant="ro"
+    ):
+
+        """Set the database access level for a specific stream.
+
+        :param streamname: Name of the stream
+        :type streamname: string
+        :param databasename: Name of the database
+        :type databasename: string
+        :param grant: Use "rw" to set the database access level to Administrate .
+                      Use "ro" to set the database access level to Access.
+                      Use "none" to set the database access level to No access.
+        :type grant: string
+        :returns: Accesslevel of a particular db.
+        :rtype: Object
+        :raise c8.exceptions.SetStreamAccessLevel: If request fails.
+        """
+
+        request = Request(
+            method="put",
+            endpoint="/user/{}/database/{}/stream/{}".format(
+                username, databasename, streamname
+            ),
+            data={"grant": grant},
+        )
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise SetStreamAccessLevel(resp, request)
+            else:
+                return resp.body
+
+        return self._execute(request, response_handler, custom_prefix="/_api")
+
+    def clear_stream_access_level_user(
+        self, username, streamname, databasename="_system"
+    ):
+
+        """Clear the database access level for a specific stream.
+
+        :param streamname: Name of the stream
+        :type streamname: string
+        :param databasename: Name of the database
+        :type databasename: string
+        :returns: True if operation successful.
+        :rtype: booleaan
+        :raise c8.exceptions.ClearStreamAccessLevel: If request fails.
+        """
+
+        request = Request(
+            method="delete",
+            endpoint="/user/{}/database/{}/stream/{}".format(
+                username, databasename, streamname
+            ),
+        )
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise ClearStreamAccessLevel(resp, request)
+            else:
+                if resp.body["error"] is False:
+                    return True
+                elif resp.body["error"] is True:
+                    return False
+
+        return self._execute(request, response_handler, custom_prefix="/_api")
+
+    def get_billing_access_level_user(self, username):
+        """Fetch the billing access level.
+
+        :returns: AccessLevel of billing.
+        :rtype: string
+        :raise c8.exceptions.BillingAccessLevel: If request fails.
+        """
+        request = Request(method="get", endpoint="/user/{}/billing".format(username))
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise BillingAccessLevel(resp, request)
+            else:
+                return resp.body["result"]
+
+        return self._execute(request, response_handler, custom_prefix="/_api")
+
+    def set_billing_access_level_user(self, username, grant="ro"):
+
+        """Set the billing access level for user.
+
+        :param grant: Use "rw" to set the database access level to Administrate .
+                      Use "ro" to set the database access level to Access.
+                      Use "none" to set the database access level to No access.
+        :type grant: string
+        :returns: Billing Accesslevel of a particular user.
+        :rtype: Object
+        :raise c8.exceptions.SetBillingAccessLevel: If request fails.
+        """
+        request = Request(
+            method="put",
+            endpoint="/user/{}/billing".format(username),
+            data={"grant": grant},
+        )
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise SetBillingAccessLevel(resp, request)
+            else:
+                return resp.body
+
+        return self._execute(request, response_handler, custom_prefix="/_api")
+
+    def clear_billing_access_level_user(self, username):
+
+        """Clear the billing access level.
+
+        :returns: True if operation successful.
+        :rtype: booleaan
+        :raise c8.exceptions.ClearBillingAccessLevel: If request fails.
+        """
+        request = Request(method="delete", endpoint="/user/{}/billing".format(username))
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise ClearBillingAccessLevel(resp, request)
+            else:
+                return resp.body
+
+        return self._execute(request, response_handler, custom_prefix="/_api")
+
+    def get_attributes_user(self, username):
+
+        """Fetch the list of attributes for the specified user.
+
+        :returns: All attributes for the specified user.
+        :rtype: dict
+        :raise c8.exceptions.GetAttributes: If request fails.
+        """
+        request = Request(method="get", endpoint="/user/{}/attributes".format(username))
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise GetAttributes(resp, request)
+            else:
+                return resp.body
+
+        return self._execute(request, response_handler, custom_prefix="/_api")
+
+    def update_attributes_user(self, username, attributes):
+
+        """Update the list of attributes for the specified user.
+
+        :param attributes: The key-value pairs of attributes with values that needs to be updated.
+        :type attributes: dict
+        :returns: The updated attributes.
+        :rtype: Object
+        :raise c8.exceptions.UpdateAttributes: If request fails.
+        """
+        request = Request(
+            method="put",
+            endpoint="/user/{}/attributes".format(username),
+            data=attributes,
+        )
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise UpdateAttributes(resp, request)
+            else:
+                return resp.body
+
+        return self._execute(request, response_handler, custom_prefix="/_api")
+
+    def remove_all_attributes_user(self, username):
+
+        """Remove all attributes of the specified user.
+
+        :returns: True if operation successful.
+        :returns: All attributes for the specified user.
+        :rtype: dict
+        """
+        request = Request(
+            method="delete", endpoint="/user/{}/attributes/truncate".format(username)
+        )
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise RemoveAllAttributes(resp, request)
+            else:
+                return resp.body
+
+        return self._execute(request, response_handler, custom_prefix="/_api")
+
+    def remove_attribute_user(self, username, attributeid):
+
+        """Remove the specified attribute for the specified user.
+
+        :param attributeid: Name of the attribute
+        :type attributeid: string
+        :returns: All attributes for the specified user.
+        :rtype: dict
+        :raise c8.exceptions.RemoveAttribute: If request fails.
         """
-        endpoint = '/_admin/user/{}/database/{}'.format(username, database)
-        if collection is not None:
-            endpoint += '/' + collection
+        request = Request(
+            method="delete",
+            endpoint="/user/{}/attributes/{}".format(username, attributeid),
+        )
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise RemoveAttribute(resp, request)
+            else:
+                return resp.body
+
+        return self._execute(request, response_handler, custom_prefix="/_api")
+
+    #########################
+    # Permission Management #
+    #########################
+
+    def permissions(self, username):
+        """Return user permissions for all fabrics and collections.
 
-        request = Request(method='delete', endpoint=endpoint)
+        :param username: Username.
+        :type username: str | unicode
+        :returns: User permissions for all fabrics and collections.
+        :rtype: dict
+        :raise: c8.exceptions.PermissionListError: If retrieval fails.
+        """
+        request = Request(
+            method="get",
+            endpoint="/user/{}/database".format(username),
+            params={"full": True},
+        )
 
         def response_handler(resp):
             if resp.is_success:
-                return True
-            raise PermissionResetError(resp, request)
+                return resp.body["result"]
+            raise PermissionListError(resp, request)
 
-        return self._execute(request, response_handler)
+        return self._execute(request, response_handler, custom_prefix="/_api")
```

### Comparing `pyC8-0.9.6/c8/request.py` & `pyC8-1.0.0/c8/request.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from __future__ import absolute_import, unicode_literals
 
-__all__ = ['Request']
-
 import json
+import warnings
 
 from six import moves, string_types
 
-# KARTIK : Disable the insecure HTTPS cert warnings 
-# WARNING : POTENTIAL SECURITY HAZARD! We should remove this after we get a
-# properly signed certificate for C8.
-import warnings
+__all__ = ["Request"]
+
 warnings.filterwarnings("ignore")
 
 
 class Request(object):
     """HTTP request.
 
     :param method: HTTP method in lowercase (e.g. "post").
@@ -48,44 +45,47 @@
     :ivar read: Names of collections read during transaction.
     :vartype read: str | unicode | [str | unicode] | None
     :ivar write: Names of collections written to during transaction.
     :vartype write: str | unicode | [str | unicode] | None
     """
 
     __slots__ = (
-        'method',
-        'endpoint',
-        'headers',
-        'params',
-        'data',
-        'command',
-        'read',
-        'write'
+        "method",
+        "endpoint",
+        "headers",
+        "params",
+        "data",
+        "command",
+        "read",
+        "write",
     )
 
-    def __init__(self,
-                 method,
-                 endpoint,
-                 auth_tok=None,
-                 headers=None,
-                 params=None,
-                 data=None,
-                 command=None,
-                 read=None,
-                 write=None):
+    def __init__(
+        self,
+        method,
+        endpoint,
+        auth_tok=None,
+        headers=None,
+        params=None,
+        data=None,
+        command=None,
+        read=None,
+        write=None,
+    ):
         self.method = method
         self.endpoint = endpoint
         self.headers = headers or {}
 
         # Insert default headers.
-        self.headers['content-type'] = 'application/json'
-        self.headers['charset'] = 'utf-8'
-        if auth_tok:
-            self.headers['Authorization'] = 'bearer '+auth_tok
+        if "content-type" not in self.headers:
+            self.headers["content-type"] = "application/json"
+        self.headers["charset"] = "utf-8"
 
+        if auth_tok:
+            self.headers["Authorization"] = "bearer " + auth_tok
 
         # Sanitize URL params.
         if params is not None:
             for key, val in params.items():
                 if isinstance(val, bool):
                     params[key] = int(val)
         self.params = params
@@ -99,30 +99,28 @@
             self.data = json.dumps(data)
 
         # Set the transaction metadata.
         self.command = command
         self.read = read
         self.write = write
 
-
-    def set_auth_token_in_header(auth_tok):
-        """ Set the Authorization header with the specified JWT auth token.
+    def set_auth_token_in_header(self, auth_tok):
+        """Set the Authorization header with the specified JWT auth token.
 
         :param auth_tok: JWT Autentication to use in this request
         :type auth_tok: str | unicode
         """
         if auth_tok:
-            self.headers['Authorization'] = 'bearer '+auth_tok
-
+            self.headers["Authorization"] = "bearer " + auth_tok
 
     def __str__(self):
         """Return the request details in string form."""
         path = self.endpoint
         if self.params is not None:
-            path += '?' + moves.urllib.parse.urlencode(self.params)
-        request_strings = ['{} {} HTTP/1.1'.format(self.method, path)]
+            path += "?" + moves.urllib.parse.urlencode(self.params)
+        request_strings = ["{} {} HTTP/1.1".format(self.method, path)]
         if self.headers is not None:
             for key, value in sorted(self.headers.items()):
-                request_strings.append('{}: {}'.format(key, value))
+                request_strings.append("{}: {}".format(key, value))
         if self.data is not None:
-            request_strings.append('\r\n{}'.format(self.data))
-        return '\r\n'.join(request_strings)
+            request_strings.append("\r\n{}".format(self.data))
+        return "\r\n".join(request_strings)
```

### Comparing `pyC8-0.9.6/c8/constants.py` & `pyC8-1.0.0/c8/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,25 +9,24 @@
 #  CHANGELOG:                                                                 #
 #      2018-07-23 : Initial cut                                               #
 #                                                                             #
 #                                                                             #
 ###############################################################################
 
 
-### C8DB Defaults
-TENANT_DEFAULT = "_mm"
-DB_DEFAULT = "_system"
+# C8DB Defaults
+TENANT_DEFAULT = "mytenant"
+FABRIC_DEFAULT = "_system"
 USER_DEFAULT = "root"
-DB_PORT = "30005"
+FABRIC_PORT = "30005"
 
-### TODO : Streams defaults
-STREAM_PORT = "30002"
+# Streams defaults
+STREAM_PORT = "6650"
 STREAM_GLOBAL_NS_PREFIX = "c8global."
 STREAM_LOCAL_NS_PREFIX = "c8local."
-PLUSAR_URL_PREFIX = "c8."
-STREAMNAME_GLOBAL_SYSTEM_DEFAULT = STREAM_GLOBAL_NS_PREFIX+"_system"
-STREAMNAME_LOCAL_SYSTEM_DEFAULT = STREAM_LOCAL_NS_PREFIX+"_system"
+STREAMNAME_GLOBAL_SYSTEM_DEFAULT = STREAM_GLOBAL_NS_PREFIX + "_system"
+STREAMNAME_LOCAL_SYSTEM_DEFAULT = STREAM_LOCAL_NS_PREFIX + "_system"
 
-### TODO : Functions defaults
+# TODO : Functions defaults
 
 if __name__ == "__main__":
-    print('This file is only meant to be used as an import module')
+    print("This file is only meant to be used as an import module")  # noqa: T201
```

### Comparing `pyC8-0.9.6/c8/connection.py` & `pyC8-1.0.0/c8/connection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,134 @@
 from __future__ import absolute_import, unicode_literals
 
-from c8.http import DefaultHTTPClient
+import json
+
+import requests
 
 import c8.constants as constants
+from c8.exceptions import (
+    C8AuthenticationError,
+    C8TenantNotFoundError,
+    C8TokenNotFoundError,
+)
+from c8.http import DefaultHTTPClient
 
-__all__ = ['Connection']
+__all__ = ["Connection"]
 
-### TODO : Functions API
 
 class Connection(object):
     """HTTP connection to specific C8 tenant.
 
     :param url: C8Db base URL.
     :type url: str | unicode
-    :param db: Database name.
-    :type db: str | unicode
+    :param fabric: Fabric name.
+    :type fabric: str | unicode
     :param username: Username.
     :type username: str | unicode
     :param password: Password.
     :type password: str | unicode
     :param http_client: User-defined HTTP client.
     :type http_client: c8.http.HTTPClient
-    :param is_db: Whether this a DB or streams call. Anything other than streams is a DB call.
-    :type is_db: bool
+    :param is_fabric: Whether this a DB or streams call.
+                      Anything other than streams is a DB call.
+    :type is_fabric: bool
     """
 
-    def __init__(self, url, tenantname, db_or_stream_name, username, password, http_client, is_db=True):
-        self.url=url
+    def __init__(self, url, email, password, token, apikey, http_client):
+        self.url = url
         self._tenant_name = ""
-        self._db_name = ""
-        self._stream_name = ""
-        self._username = username
+        self._fabric_name = constants.FABRIC_DEFAULT
+        self._email = email
+        self._password = password
         self._http_client = http_client or DefaultHTTPClient()
+        self._token = token
+        self._apikey = apikey
+        self._header = ""
+
+        if self._token is not None:
+            self._auth_token = self._token
+
+        if self._apikey is not None:
+            self._auth_token = self._apikey
+
+        if self._email != "" and password != "":
+            body = self._get_auth_token()
+            self._auth_token = body.get("jwt")
+            self._tenant_name = body.get("tenant")
+            self._header = {"Authorization": "Bearer " + self._auth_token}
+
+        if self._tenant_name == "" and self._token is not None:
+            headers = {"Authorization": "Bearer " + self._auth_token}
+            self._header = headers
+
+            tenurl = self.url + "/_api/user"
+            response = requests.get(url=tenurl, headers=headers)
+            if response.status_code == 200:
+                body = json.loads(response.text)
+                self._tenant_name = body["result"][0]["tenant"]
+
+        if self._tenant_name == "" and self._apikey is not None:
+            headers = {"Authorization": "apikey " + self._auth_token}
+            self._header = headers
+            tenurl = self.url + "/_api/user"
+            response = requests.get(url=tenurl, headers=headers)
+            if response.status_code == 200:
+                body = json.loads(response.text)
+                self._tenant_name = body["result"][0]["tenant"]
 
-        # Multitenancy
-        # TODO : Streams permissions?
-        if not tenantname or self._tenant_name.isspace():
-            self._tenant_name = constants.TENANT_DEFAULT 
-        else:
-            self._tenant_name=tenantname
+        self._url_prefix = "{}/_fabric/{}/_api".format(url, self._fabric_name)
 
-        # Set the auth credentials depending on tenant name
-        if self._tenant_name == '_mm':
-            self._auth = (username, password)
-        else:
-            self._auth = (self._tenant_name+'.'+username, password)
+        # TODO : Handle the functions side of things
 
-        # Construct the URL prefix in the required format.
-        # E.g. C8DB Connections: GET /_db/_tenant/{tenant-name}/_database/{db_name}/_admin/user/{user}/database/
-        # E.g C8Streams Conns..:  /_streams/_tenant/<tenant-name>/_stream/<stream-name>/topics
-        if(is_db):
-            # Handle the DB side of things
-            if not db_or_stream_name:
-                self._db_name = constants.DB_DEFAULT
+    def _get_auth_token(self, email=None, password=None, tenant=None, username=None):
+        data = {}
+        if password is not None:
+            data.update({"password": password})
+            if email is not None:
+                data.update({"email": email})
+            elif tenant is not None and username is not None:
+                data.update({"tenant": tenant, "username": username})
             else:
-                self._db_name = db_or_stream_name
-
-            # self._url_prefix = '{}/_db/{}'.format(url, self._db_name) # ORIG CODE
-            #self._url_prefix = '{}/_db/tenant/{}/_database/{}'.format(url, self._tenant_name, self._db_name)
-            self._url_prefix = '{}/_database/_tenant/{}/_db/{}'.format(url, self._tenant_name, self._db_name )
-
+                raise C8AuthenticationError(
+                    "Failed to Authenticate the C8DB user, Error: Invalid JSON"
+                )
         else:
-            # Handle the streams side of things
-            if not db_or_stream_name:
-                self._stream_name = constants.STREAMNAME_GLOBAL_SYSTEM_DEFAULT
-            else:
-                self._stream_name = db_or_stream_name
+            data = {"email": self._email, "password": self._password}
 
-            self._url_prefix = '{}/_streams/tenant/{}'.format(url, self._tenant_name, self._stream_name)
-
-        # TODO : Handle the functions side of things
+        data = json.dumps(data)
+        url = self.url + "/_open/auth"
+        response = requests.post(url, data=data)
+
+        if response.status_code == 200:
+            body = json.loads(response.text)
+            tenant = body.get("tenant")
+            token = body.get("jwt")
+            if not tenant:
+                raise C8TenantNotFoundError(
+                    "Failed to get Tenant Name for URL: {} and Email: {}".format(
+                        self.url, self._email
+                    )
+                )
+            if not token:
+                raise C8TokenNotFoundError(
+                    "Failed to get Authentication Token for URL: {} Tenant: {} and Email: {}".format(
+                        self.url, self.tenant_name, self._email
+                    )
+                )
+        else:
+            raise C8AuthenticationError(
+                "Failed to Authenticate the C8DB user for URL: {} and Email: {}. Error: {}".format(
+                    self.url, self._email, response.text
+                )
+            )
+        return body
 
+    @property
+    def headers(self):
+        return self._header
 
     @property
     def url_prefix(self):
         """Return the C8 URL prefix (base URL + tenant name).
 
         :returns: C8 URL prefix.
         :rtype: str | unicode
@@ -96,153 +150,126 @@
 
         :returns: tenant name.
         :rtype: str | unicode
         """
         return self._tenant_name
 
     @property
-    def db_name(self):
+    def fabric_name(self):
         """Return the DB name if it was called from the DB class
 
         :returns:  DB name.
         :rtype: str | unicode
         """
-        return self._db_name
+        return self._fabric_name
 
-    @property
-    def stream_name(self):
-        """Return the Stream name if it was called from the Stream class
-
-        :returns: Stream name.
-        :rtype: str | unicode
-        """
-        return self._stream_name
+    def set_fabric_name(self, new_fabric_name):
+        self._fabric_name = new_fabric_name
 
     def set_url_prefix(self, new_prefix):
         """
         Set the URL prefix to the new prefix,
         returns (old_prefix,new_prefix) so it can be tracked.
         """
-        old_prefix = self._url_prefix
         self._url_prefix = new_prefix
-        return old_prefix,self._url_prefix
+        # return old_prefix, self._url_prefix
 
-    def send_request(self, request):
+    def send_request(self, request, custom_prefix=None):
         """Send an HTTP request to C8 server.
 
         :param request: HTTP request.
         :type request: c8.request.Request
+        :param custom_prefix: Custom url-path value
+        :type custom_prefix: str
         :return: HTTP response.
         :rtype: c8.response.Response
         """
-        # Below line is a debug to show what the full request URL is. Useful in testing multitenancy API calls
-        #print("KARTIK : CONN OBJECT : send_request called with URL: '"+self._url_prefix + request.endpoint+"'")
+        # Below line is a debug to show what the full request URL is.
+        # Useful in testing multitenancy API calls
+        # if '_tenant' in request.endpoint and '_fabric' in request.endpoint:
+        if "/_fabric" in request.endpoint:
+            find_url = self._url_prefix.find("/_fabric")
+            url = self._url_prefix[0:find_url]
+            final_url = url + request.endpoint
+        else:
+            if custom_prefix is not None:
+                final_url = self.url + custom_prefix + request.endpoint
+            else:
+                final_url = self._url_prefix + request.endpoint
+
+        headers = request.headers
+
+        if self._token is not None:
+            headers["Authorization"] = "bearer " + self._auth_token
+
+        elif self._apikey is not None:
+            headers["Authorization"] = "apikey " + self._auth_token
+
+        elif self._token is None and self._apikey is None:
+            headers["Authorization"] = "bearer " + self._auth_token
+
+        self._header = headers
         return self._http_client.send_request(
             method=request.method,
-            url=self._url_prefix + request.endpoint,
+            url=final_url,
             params=request.params,
             data=request.data,
-            headers=request.headers,
-            auth=self._auth,
+            headers=headers,
         )
 
+
 class TenantConnection(Connection):
     """Tenant Connection wrapper.
 
     :param connection: HTTP connection.
     :type connection: c8.connection.Connection
     """
 
-    def __init__(self, url, tenant, db, username, password, http_client):
-        super(TenantConnection, self).__init__(url, tenant, db, username, password, http_client, is_db=True)
-        self._fqdb_name = tenant+"."+db
+    def __init__(self, url, email, password, token, apikey, http_client):
+        super(TenantConnection, self).__init__(
+            url=url,
+            email=email,
+            password=password,
+            token=token,
+            apikey=apikey,
+            http_client=http_client,
+        )
+        self._fqfabric_name = self._tenant_name + "." + self._fabric_name
 
     def __repr__(self):
-        return '<TenantConnection {}>'.format(self._fqdb_name)
+        return "<TenantConnection {}>".format(self._fqfabric_name)
 
     @property
-    def fqdb_name(self):
-        """Return the fully qualified (i.e with tenant) database name.
+    def fqfabric_name(self):
+        """Return the fully qualified (i.e with tenant) fabric name.
 
         :returns: Tenant name.
         :rtype: str | unicode
         """
-        return self._fqdb_name
-
-
-class DatabaseConnection(Connection):
-    """Database Connection wrapper.
-
-    :param connection: HTTP connection.
-    :type connection: c8.connection.Connection
-    """
-
-    def __init__(self, url, stream_port, tenant, db, username, password, http_client):
-        super(DatabaseConnection, self).__init__(url, tenant, db, username, password, http_client, is_db=True)
-        self._db_name = db
-        self.stream_port = stream_port
-    def __repr__(self):
-        return '<DatabaseConnection {}>'.format(self._db_name)
-
-    @property
-    def db_name(self):
-        """Return the database name.
-
-        :returns: Database name.
-        :rtype: str | unicode
-        """
-        return self._db_name
-
-class StreamConnection(Connection):
-    """Stream Connection wrapper.
+        return self._fqfabric_name
 
-    :param connection: HTTP connection.
-    :type connection: c8.connection.Connection
-    """
-
-    def __init__(self, url, tenant, stream, username, password, http_client):
-        super(StreamConnection, self).__init__(url, tenant, stream, username, password, http_client, is_db=False)
-        self._stream_name = stream
-
-    def __repr__(self):
-        return '<StreamConnection {}>'.format(self._stream_name)
-
-    @property
-    def stream_name(self):
-        """Return the stream name.
-
-        :returns: Stream name.
-        :rtype: str | unicode
-        """
-        return self._stream_name
-
-
-class RealtimeConnection(Connection):
-    """
-    Realtime connection wrapper.
-
-    :param connection: HTTP connection.
-    :type connection: c8.connection.Connection
-    """
-    # TODO : Topic persistence settings
-
-    def __init__(self, url, tenant, db, username, password, http_client, topic):
-        super(RealtimeConnection, self).__init__(url, tenant, db, username, password, http_client, is_db=False)
-        self._topic_name = topic
-        self._realtime_url = url
-        # super's _url_prefix is useless in this case so override it here
-        self._url_prefix = url
-
-
-    def __repr__(self):
-        return '<RealtimeConnection tenant={}, db={}, topic={}>'.format(self._tenant_name, self._db_name, self._topic_name)
-
-    @property
-    def topic_name(self):
-        return self._topic_name
-
-    @property
-    def realtime_url(self):
-        return self._realtime_url
 
+# class FabricConnection(Connection):
+#     """Fabric Connection wrapper.
 
-# TODO : class FunctionConnection(Connection)
+#     :param connection: HTTP connection.
+#     :type connection: c8.connection.Connection
+#     """
+
+#     def __init__(self, url, stream_port, tenant, fabric, email, password,
+#                  http_client):
+#         super(FabricConnection, self).__init__(url, tenant, fabric, email,
+#                                                password, http_client, True)
+#         self._fabric_name = fabric
+#         self.stream_port = stream_port
+
+#     def __repr__(self):
+#         return '<FabricConnection {}>'.format(self._fabric_name)
+
+#     @property
+#     def fabric_name(self):
+#         """Return the fabric name.
+
+#         :returns: Fabric name.
+#         :rtype: str | unicode
+#         """
+#         return self._fabric_name
```

### Comparing `pyC8-0.9.6/c8/collection.py` & `pyC8-1.0.0/c8/collection.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 from __future__ import absolute_import, unicode_literals
 
-__all__ = ['StandardCollection', 'VertexCollection', 'EdgeCollection']
-
-from numbers import Number
-
 from json import dumps
+from numbers import Number
 
 from c8.api import APIWrapper
 from c8.cursor import Cursor
 from c8.exceptions import (
-    CollectionRenameError,
+    CollectionImportFromFileError,
+    CollectionPropertiesError,
     CollectionTruncateError,
     DocumentCountError,
-    DocumentInError,
     DocumentDeleteError,
     DocumentGetError,
-    DocumentKeysError,
-    DocumentIDsError,
+    DocumentInError,
     DocumentInsertError,
     DocumentParseError,
     DocumentReplaceError,
     DocumentRevisionError,
     DocumentUpdateError,
     EdgeListError,
+    GetIndexError,
     IndexCreateError,
     IndexDeleteError,
     IndexListError,
 )
 from c8.request import Request
 from c8.response import Response
 from c8.utils import (
+    csv_reader,
     get_doc_id,
+    get_documents_from_file,
+    group_csv_key_values,
     is_none_or_int,
     is_none_or_str,
+    json_reader,
 )
 
+__all__ = ["StandardCollection", "VertexCollection", "EdgeCollection"]
+
 
 class Collection(APIWrapper):
     """Base class for collection API wrappers.
 
     :param connection: HTTP connection.
     :type connection: c8.connection.Connection
     :param executor: API executor.
     :type executor: c8.executor.Executor
     :param name: Collection name.
     :type name: str | unicode
     """
 
-    types = {
-        2: 'document',
-        3: 'edge'
-    }
+    types = {2: "document", 3: "edge"}
 
     statuses = {
-        1: 'new',
-        2: 'unloaded',
-        3: 'loaded',
-        4: 'unloading',
-        5: 'deleted',
-        6: 'loading'
+        1: "new",
+        2: "unloaded",
+        3: "loaded",
+        4: "unloading",
+        5: "deleted",
+        6: "loading",
     }
 
     def __init__(self, connection, executor, name):
         super(Collection, self).__init__(connection, executor)
         self._name = name
-        self._id_prefix = name + '/'
+        self._id_prefix = name + "/"
 
     def __iter__(self):
         return self.all()
 
     def __len__(self):
         return self.count()
 
@@ -76,272 +76,285 @@
         return self.has(document, check_rev=False)
 
     def _get_status_text(self, code):  # pragma: no cover
         """Return the collection status text.
 
         :param code: Collection status code.
         :type code: int
-        :return: Collection status text or None if code is None.
+        :returns: Collection status text or None if code is None.
         :rtype: str | unicode
         """
         return None if code is None else self.statuses[code]
 
     def _format_properties(self, body):  # pragma: no cover
         """Format the collection properties.
 
         :param body: Response body.
         :type body: dict
-        :return: Formatted body.
+        :returns: Formatted body.
         :rtype: dict
         """
-        body.pop('code', None)
-        body.pop('error', None)
+        body.pop("code", None)
+        body.pop("error", None)
 
-        if 'name' not in body:
-            body['name'] = self.name
-        if 'isSystem' in body:
-            body['system'] = body.pop('isSystem')
-        if 'type' in body:
-            body['edge'] = body.pop('type') == 3
-        if 'waitForSync' in body:
-            body['sync'] = body.pop('waitForSync')
-        if 'statusString' in body:
-            body['status'] = body.pop('statusString')
-        elif 'status' in body:
-            body['status'] = self._get_status_text(body['status'])
-        if 'globallyUniqueId' in body:
-            body['global_id'] = body.pop('globallyUniqueId')
-        if 'objectId' in body:
-            body['id'] = body.pop('objectId')
-        if 'cacheEnabled' in body:
-            body['cache'] = body.pop('cacheEnabled')
-        if 'doCompact' in body:
-            body['compact'] = body.pop('doCompact')
-        if 'isVolatile' in body:
-            body['volatile'] = body.pop('isVolatile')
-        if 'shardKeys' in body:
-            body['shard_fields'] = body.pop('shardKeys')
-        if 'replicationFactor' in body:
-            body['replication_factor'] = body.pop('replicationFactor')
-        if 'isSmart' in body:
-            body['smart'] = body.pop('isSmart')
-        if 'indexBuckets' in body:
-            body['index_bucket_count'] = body.pop('indexBuckets')
-        if 'journalSize' in body:
-            body['journal_size'] = body.pop('journalSize')
-        if 'numberOfShards' in body:
-            body['shard_count'] = body.pop('numberOfShards')
-
-        key_options = body.pop('keyOptions', {})
-        if 'type' in key_options:
-            body['key_generator'] = key_options['type']
-        if 'increment' in key_options:
-            body['key_increment'] = key_options['increment']
-        if 'offset' in key_options:
-            body['key_offset'] = key_options['offset']
-        if 'allowUserKeys' in key_options:
-            body['user_keys'] = key_options['allowUserKeys']
-        if 'lastValue' in key_options:
-            body['key_last_value'] = key_options['lastValue']
+        if "name" not in body:
+            body["name"] = self.name
+        if "isSystem" in body:
+            body["system"] = body.pop("isSystem")
+        if "type" in body:
+            body["edge"] = body.pop("type") == 3
+        if "waitForSync" in body:
+            body["sync"] = body.pop("waitForSync")
+        if "statusString" in body:
+            body["status"] = body.pop("statusString")
+        elif "status" in body:
+            body["status"] = self._get_status_text(body["status"])
+        if "globallyUniqueId" in body:
+            body["global_id"] = body.pop("globallyUniqueId")
+        if "objectId" in body:
+            body["id"] = body.pop("objectId")
+        if "cacheEnabled" in body:
+            body["cache"] = body.pop("cacheEnabled")
+        if "doCompact" in body:
+            body["compact"] = body.pop("doCompact")
+        if "isVolatile" in body:
+            body["volatile"] = body.pop("isVolatile")
+        if "shardKeys" in body:
+            body["shard_fields"] = body.pop("shardKeys")
+        if "replicationFactor" in body:
+            body["replication_factor"] = body.pop("replicationFactor")
+        if "isSmart" in body:
+            body["smart"] = body.pop("isSmart")
+        if "indexBuckets" in body:
+            body["index_bucket_count"] = body.pop("indexBuckets")
+        if "journalSize" in body:
+            body["journal_size"] = body.pop("journalSize")
+        if "numberOfShards" in body:
+            body["shard_count"] = body.pop("numberOfShards")
+
+        key_options = body.pop("keyOptions", {})
+        if "type" in key_options:
+            body["key_generator"] = key_options["type"]
+        if "increment" in key_options:
+            body["key_increment"] = key_options["increment"]
+        if "offset" in key_options:
+            body["key_offset"] = key_options["offset"]
+        if "allowUserKeys" in key_options:
+            body["user_keys"] = key_options["allowUserKeys"]
+        if "lastValue" in key_options:
+            body["key_last_value"] = key_options["lastValue"]
         return body
 
     def _validate_id(self, doc_id):
         """Check the collection name in the document ID.
 
         :param doc_id: Document ID.
         :type doc_id: str | unicode
-        :return: Verified document ID.
+        :returns: Verified document ID.
         :rtype: str | unicode
         :raise c8.exceptions.DocumentParseError: On bad collection name.
         """
         if not doc_id.startswith(self._id_prefix):
             raise DocumentParseError(
-                'bad collection name in document ID "{}"'.format(doc_id))
+                'bad collection name in document ID "{}"'.format(doc_id)
+            )
         return doc_id
 
     def _extract_id(self, body):
         """Extract the document ID from document body.
 
         :param body: Document body.
         :type body: dict
-        :return: Document ID.
+        :returns: Document ID.
         :rtype: str | unicode
         :raise c8.exceptions.DocumentParseError: On missing ID and key.
         """
         try:
-            if '_id' in body:
-                return self._validate_id(body['_id'])
+            if "_id" in body:
+                return self._validate_id(body["_id"])
             else:
-                return self._id_prefix + body['_key']
+                return self._id_prefix + body["_key"]
         except KeyError:
             raise DocumentParseError('field "_key" or "_id" required')
 
     def _prep_from_body(self, document, check_rev):
         """Prepare document ID and request headers.
 
         :param document: Document body.
         :type document: dict
         :param check_rev: Whether to check the revision.
         :type check_rev: bool
-        :return: Document ID and request headers.
+        :returns: Document ID and request headers.
         :rtype: (str | unicode, dict)
         """
         doc_id = self._extract_id(document)
-        if not check_rev or '_rev' not in document:
+        if not check_rev or "_rev" not in document:
             return doc_id, {}
-        return doc_id, {'If-Match': document['_rev']}
+        return doc_id, {"If-Match": document["_rev"]}
 
     def _prep_from_doc(self, document, rev, check_rev):
         """Prepare document ID, body and request headers.
 
         :param document: Document ID, key or body.
         :type document: str | unicode | dict
         :param rev: Document revision or None.
         :type rev: str | unicode | None
         :param check_rev: Whether to check the revision.
         :type check_rev: bool
-        :return: Document ID, body and request headers.
+        :returns: Document ID, body and request headers.
         :rtype: (str | unicode, str | unicode | body, dict)
         """
         if isinstance(document, dict):
             doc_id = self._extract_id(document)
-            rev = rev or document.get('_rev')
+            rev = rev or document.get("_rev")
 
             if not check_rev or rev is None:
                 return doc_id, doc_id, {}
             elif self._is_transaction:
                 body = document.copy()
-                body['_rev'] = rev
-                return doc_id, body, {'If-Match': rev}
+                body["_rev"] = rev
+                return doc_id, body, {"If-Match": rev}
             else:
-                return doc_id, doc_id, {'If-Match': rev}
+                return doc_id, doc_id, {"If-Match": rev}
         else:
-            if '/' in document:
+            if "/" in document:
                 doc_id = self._validate_id(document)
             else:
                 doc_id = self._id_prefix + document
 
             if not check_rev or rev is None:
                 return doc_id, doc_id, {}
             elif self._is_transaction:
-                body = {'_id': doc_id, '_rev': rev}
-                return doc_id, body, {'If-Match': rev}
+                body = {"_id": doc_id, "_rev": rev}
+                return doc_id, body, {"If-Match": rev}
             else:
-                return doc_id, doc_id, {'If-Match': rev}
+                return doc_id, doc_id, {"If-Match": rev}
 
     def _ensure_key_in_body(self, body):
         """Return the document body with "_key" field populated.
 
         :param body: Document body.
         :type body: dict
-        :return: Document body with "_key" field.
+        :returns: Document body with "_key" field.
         :rtype: dict
         :raise c8.exceptions.DocumentParseError: On missing ID and key.
         """
-        if '_key' in body:
+        if "_key" in body:
             return body
-        elif '_id' in body:
-            doc_id = self._validate_id(body['_id'])
+        elif "_id" in body:
+            doc_id = self._validate_id(body["_id"])
             body = body.copy()
-            body['_key'] = doc_id[len(self._id_prefix):]
+            body["_key"] = doc_id[len(self._id_prefix) :]  # noqa: E203
             return body
         raise DocumentParseError('field "_key" or "_id" required')
 
     def _ensure_key_from_id(self, body):
         """Return the body with "_key" field if it has "_id" field.
 
         :param body: Document body.
         :type body: dict
-        :return: Document body with "_key" field if it has "_id" field.
+        :returns: Document body with "_key" field if it has "_id" field.
         :rtype: dict
         """
-        if '_id' in body and '_key' not in body:
-            doc_id = self._validate_id(body['_id'])
+        if not isinstance(body, dict):
+            raise DocumentParseError("Document is not a dict")
+        if "_id" in body and "_key" not in body:
+            doc_id = self._validate_id(body["_id"])
             body = body.copy()
-            body['_key'] = doc_id[len(self._id_prefix):]
+            body["_key"] = doc_id[len(self._id_prefix) :]  # noqa: E203
         return body
 
     @property
     def name(self):
         """Return collection name.
 
-        :return: Collection name.
+        :returns: Collection name.
         :rtype: str | unicode
         """
         return self._name
 
-    def rename(self, new_name):
-        """Rename the collection.
+    def get_collection_information(self):
+        """Fetch the information about collection.
 
-        Renames may not be reflected immediately in async execution, batch
-        execution or transactions. It is recommended to initialize new API
-        wrappers after a rename.
-
-        :param new_name: New collection name.
-        :type new_name: str | unicode
-        :return: True if collection was renamed successfully.
-        :rtype: bool
-        :raise c8.exceptions.CollectionRenameError: If rename fails.
+        :returns: information about collection as  searchEnabled, globallyUniqueId,
+        isSystem, waitForSync, hasStream, isLocal, isSpot,collectionModel, type, id.
+        :rtype: dict
         """
         request = Request(
-            method='put',
-            endpoint='/_api/collection/{}/rename'.format(self.name),
-            data={'name': new_name}
+            method="get",
+            endpoint="/collection/{}".format(self.name),
         )
 
         def response_handler(resp):
-            if not resp.is_success:
-                raise CollectionRenameError(resp, request)
-            self._name = new_name
-            self._id_prefix = new_name + '/'
-            return True
+            if resp.is_success:
+                return resp.body
+            raise CollectionPropertiesError(resp, request)
+
+        return self._execute(request, response_handler)
+
+    def collection_figures(self):
+        """Returns an object containing statistics about a collection.
+
+        :returns: statistics related with cache, index, document size, key options
+        :rtype: dict
+        """
+
+        request = Request(
+            method="get",
+            endpoint="/collection/{}/figures".format(self.name),
+        )
+
+        def response_handler(resp):
+            if resp.is_success:
+                return resp.body
+            raise CollectionPropertiesError(resp, request)
 
         return self._execute(request, response_handler)
 
     def truncate(self):
         """Delete all documents in the collection.
 
-        :return: True if collection was truncated successfully.
+        :returns: True if collection was truncated successfully.
         :rtype: dict
         :raise c8.exceptions.CollectionTruncateError: If operation fails.
         """
         request = Request(
-            method='put',
-            endpoint='/_api/collection/{}/truncate'.format(self.name),
-            command='db.{}.truncate()'.format(self.name),
-            write=self.name
+            method="put",
+            endpoint="/collection/{}/truncate".format(self.name),
+            command="db.{}.truncate()".format(self.name),
+            write=self.name,
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise CollectionTruncateError(resp, request)
             return True
 
         return self._execute(request, response_handler)
 
     def count(self):
         """Return the total document count.
 
-        :return: Total document count.
+        :returns: Total document count.
         :rtype: int
         :raise c8.exceptions.DocumentCountError: If retrieval fails.
         """
         request = Request(
-            method='get',
-            endpoint='/_api/collection/{}/count'.format(self.name),
-            command='db.{}.count()'.format(self.name),
-            read=self.name
+            method="get",
+            endpoint="/collection/{}/count".format(self.name),
+            command="db.{}.count()".format(self.name),
+            read=self.name,
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise DocumentCountError(resp, request)
             if self._is_transaction:
                 return resp.body
-            return resp.body['count']
+            return resp.body["count"]
 
         return self._execute(request, response_handler)
 
     def has(self, document, rev=None, check_rev=True):
         """Check if a document exists in the collection.
 
         :param document: Document ID, key or body. Document body must contain
@@ -349,239 +362,75 @@
         :type document: str | unicode | dict
         :param rev: Expected document revision. Overrides value of "_rev" field
             in **document** if present.
         :type rev: str | unicode
         :param check_rev: If set to True, revision of **document** (if given)
             is compared against the revision of target document.
         :type check_rev: bool
-        :return: True if document exists, False otherwise.
+        :returns: True if document exists, False otherwise.
         :rtype: bool
         :raise c8.exceptions.DocumentInError: If check fails.
         :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
         """
         handle, body, headers = self._prep_from_doc(document, rev, check_rev)
 
-        command = 'db.{}.exists({})'.format(
-            self.name,
-            dumps(body)
-        ) if self._is_transaction else None
+        command = (
+            "db.{}.exists({})".format(self.name, dumps(body))
+            if self._is_transaction
+            else None
+        )
 
         request = Request(
-            method='get',
-            endpoint='/_api/document/{}'.format(handle),
+            method="get",
+            endpoint="/document/{}".format(handle),
             headers=headers,
             command=command,
-            read=self.name
+            read=self.name,
         )
 
         def response_handler(resp):
             if resp.error_code == 1202:
                 return False
             if resp.status_code == 412:
                 raise DocumentRevisionError(resp, request)
             if not resp.is_success:
                 raise DocumentInError(resp, request)
             return bool(resp.body)
 
         return self._execute(request, response_handler)
 
-    def ids(self):
-        """Return the IDs of all documents in the collection.
-
-        :return: Document ID cursor.
-        :rtype: c8.cursor.Cursor
-        :raise c8.exceptions.DocumentIDsError: If retrieval fails.
-        """
-        request = Request(
-            method='put',
-            endpoint='/_api/simple/all-keys',
-            data={'collection': self.name, 'type': 'id'},
-            command='db.{}.toArray().map(d => d._id)'.format(self.name),
-            read=self.name
-        )
-
-        def response_handler(resp):
-            if not resp.is_success:
-                raise DocumentIDsError(resp, request)
-            return Cursor(self._conn, resp.body)
-
-        return self._execute(request, response_handler)
-
-    def keys(self):
-        """Return the keys of all documents in the collection.
-
-        :return: Document key cursor.
-        :rtype: c8.cursor.Cursor
-        :raise c8.exceptions.DocumentKeysError: If retrieval fails.
-        """
-        request = Request(
-            method='put',
-            endpoint='/_api/simple/all-keys',
-            data={'collection': self.name, 'type': 'key'},
-            command='db.{}.toArray().map(d => d._key)'.format(self.name),
-            read=self.name
-        )
+    def export(self, offset=None, limit=None, order=None):
+        """Export all documents in the collection.
 
-        def response_handler(resp):
-            if not resp.is_success:
-                raise DocumentKeysError(resp, request)
-            return Cursor(self._conn, resp.body)
-
-        return self._execute(request, response_handler)
-
-    def all(self, skip=None, limit=None):
-        """Return all documents in the collection.
-
-        :param skip: Number of documents to skip.
-        :type skip: int
-        :param limit: Max number of documents returned.
+        :param offset: This option can be used to simulate paging.
+        :type offset: int
+        :param limit: This option can be used to simulate paging. Limits the result. Maximum: 1000.
         :type limit: int
-        :return: Document cursor.
-        :rtype: c8.cursor.Cursor
-        :raise c8.exceptions.DocumentGetError: If retrieval fails.
-        """
-        assert is_none_or_int(skip), 'skip must be a non-negative int'
-        assert is_none_or_int(limit), 'limit must be a non-negative int'
-
-        data = {'collection': self.name}
-        if skip is not None:
-            data['skip'] = skip
-        if limit is not None:
-            data['limit'] = limit
-
-        command = 'db.{}.all(){}{}.toArray()'.format(
-            self.name,
-            '' if skip is None else '.skip({})'.format(skip),
-            '' if limit is None else '.limit({})'.format(limit),
-        ) if self._is_transaction else None
-
-        request = Request(
-            method='put',
-            endpoint='/_api/simple/all',
-            data=data,
-            command=command,
-            read=self.name
-        )
-
-        def response_handler(resp):
-            # TODO workaround for a bug in C8Db
-            if self._is_transaction and limit == 0:
-                return Cursor(self._conn, [])
-            if not resp.is_success:
-                raise DocumentGetError(resp, request)
-            return Cursor(self._conn, resp.body)
-
-        return self._execute(request, response_handler)
-
-    def export(self,
-               limit=None,
-               count=False,
-               batch_size=None,
-               flush=False,
-               flush_wait=None,
-               ttl=None,
-               filter_fields=None,
-               filter_type='include'):  # pragma: no cover
-        """Export all documents in the collection using a server cursor.
-
-        :param flush: If set to True, flush the write-ahead log prior to the
-            export. If set to False, documents in the write-ahead log during
-            the export are not included in the result.
-        :type flush: bool
-        :param flush_wait: Max wait time in seconds for write-ahead log flush.
-        :type flush_wait: int
-        :param count: Include the document count in the server cursor.
-        :type count: bool
-        :param batch_size: Max number of documents in the batch fetched by
-            the cursor in one round trip.
-        :type batch_size: int
-        :param limit: Max number of documents fetched by the cursor.
-        :type limit: int
-        :param ttl: Time-to-live for the cursor on the server.
-        :type ttl: int
-        :param filter_fields: Document fields to filter with.
-        :type filter_fields: [str | unicode]
-        :param filter_type: Allowed values are "include" or "exclude".
-        :type filter_type: str | unicode
-        :return: Document cursor.
-        :rtype: c8.cursor.Cursor
+        :param order: Sorts the result in specified order. Allowed values are "asc" or "desc".
+        :type order: str | unicode
+        :returns: Documents in the collection.
+        :rtype: dict
         :raise c8.exceptions.DocumentGetError: If export fails.
         """
-        data = {'count': count, 'flush': flush}
-        if flush_wait is not None:
-            data['flushWait'] = flush_wait
-        if batch_size is not None:
-            data['batchSize'] = batch_size
+        data = {}
+        if offset is not None:
+            data["offset"] = offset
         if limit is not None:
-            data['limit'] = limit
-        if ttl is not None:
-            data['ttl'] = ttl
-        if filter_fields is not None:
-            data['restrict'] = {
-                'fields': filter_fields,
-                'type': filter_type
-            }
-        request = Request(
-            method='post',
-            endpoint='/_api/export',
-            params={'collection': self.name},
-            data=data
-        )
-
-        def response_handler(resp):
-            if not resp.is_success:
-                raise DocumentGetError(resp, request)
-            return Cursor(self._conn, resp.body, 'export')
-
-        return self._execute(request, response_handler)
-
-    def find(self, filters, skip=None, limit=None):
-        """Return all documents that match the given filters.
-
-        :param filters: Document filters.
-        :type filters: dict
-        :param skip: Number of documents to skip.
-        :type skip: int
-        :param limit: Max number of documents returned.
-        :type limit: int
-        :return: Document cursor.
-        :rtype: c8.cursor.Cursor
-        :raise c8.exceptions.DocumentGetError: If retrieval fails.
-        """
-        assert isinstance(filters, dict), 'filters must be a dict'
-        assert is_none_or_int(skip), 'skip must be a non-negative int'
-        assert is_none_or_int(limit), 'limit must be a non-negative int'
-
-        data = {
-            'collection': self.name,
-            'example': filters,
-            'skip': skip,
-        }
-        if limit is not None:
-            data['limit'] = limit
-
-        command = 'db.{}.byExample({}){}{}.toArray()'.format(
-            self.name,
-            dumps(filters),
-            '' if skip is None else '.skip({})'.format(skip),
-            '' if limit is None else '.limit({})'.format(limit),
-        ) if self._is_transaction else None
+            data["limit"] = limit
+        if order == "asc" or order == "desc":
+            data["order"] = order
 
         request = Request(
-            method='put',
-            endpoint='/_api/simple/by-example',
-            data=data,
-            command=command,
-            read=self.name
+            method="get", endpoint="/export/{}".format(self.name), params=data
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise DocumentGetError(resp, request)
-            return Cursor(self._conn, resp.body)
+            return resp.body["result"]
 
         return self._execute(request, response_handler)
 
     def find_near(self, latitude, longitude, limit=None):
         """Return documents near a given coordinate.
 
         Documents returned are sorted according to distance, with the nearest
@@ -595,66 +444,59 @@
         :type longitude: int | float
         :param limit: Max number of documents returned.
         :type limit: int
         :returns: Document cursor.
         :rtype: c8.cursor.Cursor
         :raises c8.exceptions.DocumentGetError: If retrieval fails.
         """
-        assert isinstance(latitude, Number), 'latitude must be a number'
-        assert isinstance(longitude, Number), 'longitude must be a number'
-        assert is_none_or_int(limit), 'limit must be a non-negative int'
+        assert isinstance(latitude, Number), "latitude must be a number"
+        assert isinstance(longitude, Number), "longitude must be a number"
+        assert is_none_or_int(limit), "limit must be a non-negative int"
 
         query = """
         FOR doc IN NEAR(@collection, @latitude, @longitude{})
             RETURN doc
-        """.format('' if limit is None else ', @limit ')
+        """.format(
+            "" if limit is None else ", @limit "
+        )
 
         bind_vars = {
-            'collection': self._name,
-            'latitude': latitude,
-            'longitude': longitude
+            "collection": self._name,
+            "latitude": latitude,
+            "longitude": longitude,
         }
         if limit is not None:
-            bind_vars['limit'] = limit
+            bind_vars["limit"] = limit
 
         if not self._is_transaction:
-            command = 'db.{}.near({},{}){}.toArray()'.format(
+            command = "db.{}.near({},{}){}.toArray()".format(
                 self.name,
                 latitude,
                 longitude,
-                '' if limit is None else '.limit({})'.format(limit),
+                "" if limit is None else ".limit({})".format(limit),
             )
         else:
             command = None
 
         request = Request(
-            method='post',
-            endpoint='/_api/cursor',
-            data={
-                'query': query,
-                'bindVars': bind_vars,
-                'count': True
-            },
+            method="post",
+            endpoint="/cursor",
+            data={"query": query, "bindVars": bind_vars, "count": True},
             command=command,
-            read=self.name
+            read=self.name,
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise DocumentGetError(resp, request)
             return Cursor(self._conn, resp.body)
 
         return self._execute(request, response_handler)
 
-    def find_in_range(self,
-                      field,
-                      lower,
-                      upper,
-                      skip=None,
-                      limit=None):
+    def find_in_range(self, field, lower, upper, skip=None, limit=None):
         """Return documents within a given range in a random order.
 
         A skiplist index must be defined in the collection to use this method.
 
         :param field: Document field name.
         :type field: str | unicode
         :param lower: Lower bound (inclusive).
@@ -665,52 +507,52 @@
         :type skip: int
         :param limit: Max number of documents returned.
         :type limit: int
         :returns: Document cursor.
         :rtype: c8.cursor.Cursor
         :raises c8.exceptions.DocumentGetError: If retrieval fails.
         """
-        assert is_none_or_int(skip), 'skip must be a non-negative int'
-        assert is_none_or_int(limit), 'limit must be a non-negative int'
+        assert is_none_or_int(skip), "skip must be a non-negative int"
+        assert is_none_or_int(limit), "limit must be a non-negative int"
 
         bind_vars = {
-            '@collection': self._name,
-            'field': field,
-            'lower': lower,
-            'upper': upper,
-            'skip': 0 if skip is None else skip,
-            'limit': 2147483647 if limit is None else limit,  # 2 ^ 31 - 1
+            "@collection": self._name,
+            "field": field,
+            "lower": lower,
+            "upper": upper,
+            "skip": 0 if skip is None else skip,
+            "limit": 2147483647 if limit is None else limit,  # 2 ^ 31 - 1
         }
 
         query = """
         FOR doc IN @@collection
             FILTER doc.@field >= @lower && doc.@field < @upper
             LIMIT @skip, @limit
             RETURN doc
         """
 
-        command = 'db.{}.range({},{},{}){}{}.toArray()'.format(
-            self.name,
-            dumps(field),
-            dumps(lower),
-            dumps(upper),
-            '' if skip is None else '.skip({})'.format(skip),
-            '' if limit is None else '.limit({})'.format(limit),
-        ) if self._is_transaction else None
-
-        request = Request(
-            method='post',
-            endpoint='/_api/cursor',
-            data={
-                'query': query,
-                'bindVars': bind_vars,
-                'count': True
-            },
+        command = (
+            "db.{}.range({},{},{}){}{}.toArray()".format(
+                self.name,
+                dumps(field),
+                dumps(lower),
+                dumps(upper),
+                "" if skip is None else ".skip({})".format(skip),
+                "" if limit is None else ".limit({})".format(limit),
+            )
+            if self._is_transaction
+            else None
+        )
+
+        request = Request(
+            method="post",
+            endpoint="/cursor",
+            data={"query": query, "bindVars": bind_vars, "count": True},
             command=command,
-            read=self.name
+            read=self.name,
         )
 
         def response_handler(resp):
             # TODO workaround for a bug in C8Db
             if self._is_transaction and limit == 0:
                 return Cursor(self._conn, [])
             if not resp.is_success:
@@ -733,125 +575,49 @@
         :param distance_field: Document field used to indicate the distance to
             the given coordinate. This parameter is ignored in transactions.
         :type distance_field: str | unicode
         :returns: Document cursor.
         :rtype: c8.cursor.Cursor
         :raises c8.exceptions.DocumentGetError: If retrieval fails.
         """
-        assert isinstance(latitude, Number), 'latitude must be a number'
-        assert isinstance(longitude, Number), 'longitude must be a number'
-        assert isinstance(radius, Number), 'radius must be a number'
-        assert is_none_or_str(distance_field), 'distance_field must be a str'
+        assert isinstance(latitude, Number), "latitude must be a number"
+        assert isinstance(longitude, Number), "longitude must be a number"
+        assert isinstance(radius, Number), "radius must be a number"
+        assert is_none_or_str(distance_field), "distance_field must be a str"
 
         query = """
         FOR doc IN WITHIN(@@collection, @latitude, @longitude, @radius{})
             RETURN doc
-        """.format('' if distance_field is None else ', @distance')
+        """.format(
+            "" if distance_field is None else ", @distance"
+        )
 
         bind_vars = {
-            '@collection': self._name,
-            'latitude': latitude,
-            'longitude': longitude,
-            'radius': radius
+            "@collection": self._name,
+            "latitude": latitude,
+            "longitude": longitude,
+            "radius": radius,
         }
         if distance_field is not None:
-            bind_vars['distance'] = distance_field
+            bind_vars["distance"] = distance_field
 
-        command = 'db.{}.within({},{},{}).toArray()'.format(
-            self.name,
-            latitude,
-            longitude,
-            radius
-        ) if self._is_transaction else None
-
-        request = Request(
-            method='post',
-            endpoint='/_api/cursor',
-            data={
-                'query': query,
-                'bindVars': bind_vars,
-                'count': True
-            },
-            command=command,
-            read=self.name
+        command = (
+            "db.{}.within({},{},{}).toArray()".format(
+                self.name, latitude, longitude, radius
+            )
+            if self._is_transaction
+            else None
         )
 
-        def response_handler(resp):
-            if not resp.is_success:
-                raise DocumentGetError(resp, request)
-            return Cursor(self._conn, resp.body)
-
-        return self._execute(request, response_handler)
-
-    def find_in_box(self,
-                    latitude1,
-                    longitude1,
-                    latitude2,
-                    longitude2,
-                    skip=None,
-                    limit=None,
-                    index=None):
-        """Return all documents in an rectangular area.
-
-        :param latitude1: First latitude.
-        :type latitude1: int | float
-        :param longitude1: First longitude.
-        :type longitude1: int | float
-        :param latitude2: Second latitude.
-        :type latitude2: int | float
-        :param longitude2: Second longitude
-        :type longitude2: int | float
-        :param skip: Number of documents to skip.
-        :type skip: int
-        :param limit: Max number of documents returned.
-        :type limit: int
-        :param index: ID of the geo index to use (without the collection
-            prefix). This parameter is ignored in transactions.
-        :type index: str | unicode
-        :returns: Document cursor.
-        :rtype: c8.cursor.Cursor
-        :raises c8.exceptions.DocumentGetError: If retrieval fails.
-        """
-        assert isinstance(latitude1, Number), 'latitude1 must be a number'
-        assert isinstance(longitude1, Number), 'longitude1 must be a number'
-        assert isinstance(latitude2, Number), 'latitude2 must be a number'
-        assert isinstance(longitude2, Number), 'longitude2 must be a number'
-        assert is_none_or_int(skip), 'skip must be a non-negative int'
-        assert is_none_or_int(limit), 'limit must be a non-negative int'
-
-        data = {
-            'collection': self._name,
-            'latitude1': latitude1,
-            'longitude1': longitude1,
-            'latitude2': latitude2,
-            'longitude2': longitude2,
-        }
-        if skip is not None:
-            data['skip'] = skip
-        if limit is not None:
-            data['limit'] = limit
-        if index is not None:
-            data['geo'] = self._name + '/' + index
-
-        command = 'db.{}.withinRectangle({},{},{},{}){}{}.toArray()'.format(
-            self.name,
-            latitude1,
-            longitude1,
-            latitude2,
-            longitude2,
-            '' if skip is None else '.skip({})'.format(skip),
-            '' if limit is None else '.limit({})'.format(limit),
-        ) if self._is_transaction else None
-
         request = Request(
-            method='put',
-            endpoint='/_api/simple/within-rectangle',
-            data=data,
+            method="post",
+            endpoint="/cursor",
+            data={"query": query, "bindVars": bind_vars, "count": True},
             command=command,
-            read=self.name
+            read=self.name,
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise DocumentGetError(resp, request)
             return Cursor(self._conn, resp.body)
 
@@ -866,332 +632,306 @@
         :type query: str | unicode
         :param limit: Max number of documents returned.
         :type limit: int
         :returns: Document cursor.
         :rtype: c8.cursor.Cursor
         :raises c8.exceptions.DocumentGetError: If retrieval fails.
         """
-        assert is_none_or_int(limit), 'limit must be a non-negative int'
+        assert is_none_or_int(limit), "limit must be a non-negative int"
 
         bind_vars = {
-            'collection': self._name,
-            'field': field,
-            'query': query,
+            "collection": self._name,
+            "field": field,
+            "query": query,
         }
         if limit is not None:
-            bind_vars['limit'] = limit
+            bind_vars["limit"] = limit
 
         c8ql = """
         FOR doc IN FULLTEXT(@collection, @field, @query{})
             RETURN doc
-        """.format('' if limit is None else ', @limit')
+        """.format(
+            "" if limit is None else ", @limit"
+        )
 
-        command = 'db.{}.fulltext({},{}){}.toArray()'.format(
-            self.name,
-            dumps(field),
-            dumps(query),
-            '' if limit is None else '.limit({})'.format(limit),
-        ) if self._is_transaction else None
+        command = (
+            "db.{}.fulltext({},{}){}.toArray()".format(
+                self.name,
+                dumps(field),
+                dumps(query),
+                "" if limit is None else ".limit({})".format(limit),
+            )
+            if self._is_transaction
+            else None
+        )
 
         request = Request(
-            method='post',
-            endpoint='/_api/cursor',
-            data={'query': c8ql, 'bindVars': bind_vars, 'count': True},
+            method="post",
+            endpoint="/cursor",
+            data={"query": c8ql, "bindVars": bind_vars, "count": True},
             command=command,
-            read=self.name
+            read=self.name,
         )
 
         def response_handler(resp):
             # TODO workaround for a bug in C8Db
             if self._is_transaction and limit == 0:
                 return Cursor(self._conn, [])
             if not resp.is_success:
                 raise DocumentGetError(resp, request)
             return Cursor(self._conn, resp.body)
 
         return self._execute(request, response_handler)
 
-    def get_many(self, documents):
-        """Return multiple documents ignoring any missing ones.
-
-        :param documents: List of document keys, IDs or bodies. Document bodies
-            must contain the "_id" or "_key" fields.
-        :type documents: [str | unicode | dict]
-        :return: Documents. Missing ones are not included.
-        :rtype: [dict]
-        :raise c8.exceptions.DocumentGetError: If retrieval fails.
-        """
-        handles = [
-            self._extract_id(doc) if isinstance(doc, dict) else doc
-            for doc in documents
-        ]
-
-        command = 'db.{}.document({})'.format(
-            self.name,
-            dumps(handles)
-        ) if self._is_transaction else None
-
-        request = Request(
-            method='put',
-            endpoint='/_api/simple/lookup-by-keys',
-            data={'collection': self.name, 'keys': handles},
-            command=command,
-            read=self.name
-        )
-
-        def response_handler(resp):
-            if not resp.is_success:
-                raise DocumentGetError(resp, request)
-            if self._is_transaction:
-                docs = resp.body
-            else:
-                docs = resp.body['documents']
-            return [doc for doc in docs if '_id' in doc]
-
-        return self._execute(request, response_handler)
-
-    def random(self):
-        """Return a random document from the collection.
-
-        :return: A random document.
-        :rtype: dict
-        :raise c8.exceptions.DocumentGetError: If retrieval fails.
-        """
-        request = Request(
-            method='put',
-            endpoint='/_api/simple/any',
-            data={'collection': self.name},
-            command='db.{}.any()'.format(self.name),
-            read=self.name
-        )
-
-        def response_handler(resp):
-            if not resp.is_success:
-                raise DocumentGetError(resp, request)
-            if self._is_transaction:
-                return resp.body
-            return resp.body['document']
-
-        return self._execute(request, response_handler)
-
     ####################
     # Index Management #
     ####################
 
     def indexes(self):
         """Return the collection indexes.
 
-        :return: Collection indexes.
+        :returns: Collection indexes.
         :rtype: [dict]
         :raise c8.exceptions.IndexListError: If retrieval fails.
         """
         request = Request(
-            method='get',
-            endpoint='/_api/index',
-            params={'collection': self.name},
-            command='db.{}.getIndexes()'.format(self.name),
-            read=self.name
+            method="get",
+            endpoint="/index",
+            params={"collection": self.name},
+            command="db.{}.getIndexes()".format(self.name),
+            read=self.name,
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise IndexListError(resp, request)
             if self._is_transaction:
                 result = resp.body
             else:
-                result = resp.body['indexes']
+                result = resp.body["indexes"]
 
             indexes = []
             for index in result:
-                index['id'] = index['id'].split('/', 1)[-1]
-                if 'minLength' in index:
-                    index['min_length'] = index.pop('minLength')
-                if 'geoJson' in index:
-                    index['geo_json'] = index.pop('geoJson')
-                if 'ignoreNull' in index:
-                    index['ignore_none'] = index.pop('ignoreNull')
-                if 'selectivityEstimate' in index:
-                    index['selectivity'] = index.pop('selectivityEstimate')
+                index["id"] = index["id"].split("/", 1)[-1]
+                if "minLength" in index:
+                    index["min_length"] = index.pop("minLength")
+                if "geoJson" in index:
+                    index["geo_json"] = index.pop("geoJson")
+                if "ignoreNull" in index:
+                    index["ignore_none"] = index.pop("ignoreNull")
+                if "selectivityEstimate" in index:
+                    index["selectivity"] = index.pop("selectivityEstimate")
                 indexes.append(index)
             return indexes
 
         return self._execute(request, response_handler)
 
-    def _add_index(self, data):
+    def get_index(self, index_name):
+        request = Request(
+            method="get", endpoint="/index/{}/{}".format(self.name, index_name)
+        )
+
+        def response_handler(resp):
+            if not resp.is_success:
+                raise GetIndexError
+            else:
+                return resp.body
+
+        return self._execute(request, response_handler)
+
+    def add_index(self, data):
         """Helper method for creating a new index.
 
         :param data: Index data.
         :type data: dict
-        :return: New index details.
+        :returns: New index details.
         :rtype: dict
         :raise c8.exceptions.IndexCreateError: If create fails.
         """
         request = Request(
-            method='post',
-            endpoint='/_api/index',
+            method="post",
+            endpoint="/index",
             data=data,
-            params={'collection': self.name}
+            params={"collection": self.name},
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise IndexCreateError(resp, request)
             details = resp.body
-            details['id'] = details['id'].split('/', 1)[1]
-            details.pop('error', None)
-            details.pop('code', None)
-            if 'minLength' in details:
-                details['min_length'] = details.pop('minLength')
-            if 'geoJson' in details:
-                details['geo_json'] = details.pop('geoJson')
-            if 'ignoreNull' in details:
-                details['ignore_none'] = details.pop('ignoreNull')
-            if 'selectivityEstimate' in details:
-                details['selectivity'] = details.pop('selectivityEstimate')
-            if 'isNewlyCreated' in details:
-                details['new'] = details.pop('isNewlyCreated')
+            details["id"] = details["id"].split("/", 1)[1]
+            details.pop("error", None)
+            details.pop("code", None)
+            if "minLength" in details:
+                details["min_length"] = details.pop("minLength")
+            if "geoJson" in details:
+                details["geo_json"] = details.pop("geoJson")
+            if "ignoreNull" in details:
+                details["ignore_none"] = details.pop("ignoreNull")
+            if "selectivityEstimate" in details:
+                details["selectivity"] = details.pop("selectivityEstimate")
+            if "isNewlyCreated" in details:
+                details["new"] = details.pop("isNewlyCreated")
             return details
 
         return self._execute(request, response_handler)
 
-    def add_hash_index(self,
-                       fields,
-                       unique=None,
-                       sparse=None,
-                       deduplicate=None):
+    def add_hash_index(self, fields, unique=None, sparse=None, deduplicate=None):
         """Create a new hash index.
 
         :param fields: Document fields to index.
         :type fields: [str | unicode]
         :param unique: Whether the index is unique.
         :type unique: bool
         :param sparse: If set to True, documents with None in the field
             are also indexed. If set to False, they are skipped.
         :type sparse: bool
         :param deduplicate: If set to True, inserting duplicate index values
             from the same document triggers unique constraint errors.
         :type deduplicate: bool
-        :return: New index details.
+        :returns: New index details.
         :rtype: dict
         :raise c8.exceptions.IndexCreateError: If create fails.
         """
-        data = {'type': 'hash', 'fields': fields}
+        data = {"type": "hash", "fields": fields}
         if unique is not None:
-            data['unique'] = unique
+            data["unique"] = unique
         if sparse is not None:
-            data['sparse'] = sparse
+            data["sparse"] = sparse
         if deduplicate is not None:
-            data['deduplicate'] = deduplicate
-        return self._add_index(data)
+            data["deduplicate"] = deduplicate
+        return self.add_index(data)
 
-    def add_skiplist_index(self,
-                           fields,
-                           unique=None,
-                           sparse=None,
-                           deduplicate=None):
+    def add_skiplist_index(self, fields, unique=None, sparse=None, deduplicate=None):
         """Create a new skiplist index.
 
         :param fields: Document fields to index.
         :type fields: [str | unicode]
         :param unique: Whether the index is unique.
         :type unique: bool
         :param sparse: If set to True, documents with None in the field
             are also indexed. If set to False, they are skipped.
         :type sparse: bool
         :param deduplicate: If set to True, inserting duplicate index values
             from the same document triggers unique constraint errors.
         :type deduplicate: bool
-        :return: New index details.
+        :returns: New index details.
         :rtype: dict
         :raise c8.exceptions.IndexCreateError: If create fails.
         """
-        data = {'type': 'skiplist', 'fields': fields}
+        data = {"type": "skiplist", "fields": fields}
         if unique is not None:
-            data['unique'] = unique
+            data["unique"] = unique
         if sparse is not None:
-            data['sparse'] = sparse
+            data["sparse"] = sparse
         if deduplicate is not None:
-            data['deduplicate'] = deduplicate
-        return self._add_index(data)
+            data["deduplicate"] = deduplicate
+        return self.add_index(data)
 
     def add_geo_index(self, fields, ordered=None):
         """Create a new geo-spatial index.
 
         :param fields: A single document field or a list of document fields. If
             a single field is given, the field must have values that are lists
             with at least two floats. Documents with missing fields or invalid
             values are excluded.
         :type fields: str | unicode | list
         :param ordered: Whether the order is longitude, then latitude.
         :type ordered: bool
-        :return: New index details.
+        :returns: New index details.
         :rtype: dict
         :raise c8.exceptions.IndexCreateError: If create fails.
         """
-        data = {'type': 'geo', 'fields': fields}
+        data = {"type": "geo", "fields": fields}
         if ordered is not None:
-            data['geoJson'] = ordered
-        return self._add_index(data)
+            data["geoJson"] = ordered
+        return self.add_index(data)
 
     def add_fulltext_index(self, fields, min_length=None):
         """Create a new fulltext index.
 
         :param fields: Document fields to index.
         :type fields: [str | unicode]
         :param min_length: Minimum number of characters to index.
         :type min_length: int
-        :return: New index details.
+        :returns: New index details.
         :rtype: dict
         :raise c8.exceptions.IndexCreateError: If create fails.
         """
-        data = {'type': 'fulltext', 'fields': fields}
+        data = {"type": "fulltext", "fields": fields}
         if min_length is not None:
-            data['minLength'] = min_length
-        return self._add_index(data)
+            data["minLength"] = min_length
+        return self.add_index(data)
 
-    def add_persistent_index(self, fields, unique=None, sparse=None):
+    def add_persistent_index(self, fields, unique=None, sparse=None, deduplicate=None):
         """Create a new persistent index.
 
         Unique persistent indexes on non-sharded keys are not supported in a
         cluster.
 
         :param fields: Document fields to index.
         :type fields: [str | unicode]
         :param unique: Whether the index is unique.
         :type unique: bool
         :param sparse: Exclude documents that do not contain at least one of
             the indexed fields, or documents that have a value of None in any
             of the indexed fields.
         :type sparse: bool
-        :return: New index details.
+        :param deduplicate: If set to True, inserting duplicate index values
+            from the same document triggers unique constraint errors.
+        :type deduplicate: bool
+        :returns: New index details.
         :rtype: dict
         :raise c8.exceptions.IndexCreateError: If create fails.
         """
-        data = {'type': 'persistent', 'fields': fields}
+        data = {"type": "persistent", "fields": fields}
         if unique is not None:
-            data['unique'] = unique
+            data["unique"] = unique
         if sparse is not None:
-            data['sparse'] = sparse
-        return self._add_index(data)
+            data["sparse"] = sparse
+        if deduplicate is not None:
+            data["deduplicate"] = deduplicate
+        return self.add_index(data)
+
+    def add_ttl_index(self, fields, expireAfter=0, inBackground=False):
+        """Create a new ttl index.
 
-    def delete_index(self, index_id, ignore_missing=False):
+        :param fields: Document fields to index.
+        :type fields: [str | unicode]
+        :param expireAfter:  The time (in seconds) after
+            a document's creation after which the documents count as "expired".
+        :type expireAfter: int
+        :param inBackground: Expire Documents in Background.
+        :type inBackground: bool
+        :returns: New index details.
+        :rtype: dict
+        :raise c8.exceptions.IndexCreateError: If create fails.
+        """
+        data = {
+            "type": "ttl",
+            "fields": fields,
+            "expireAfter": expireAfter,
+            "inBackground": inBackground,
+        }
+        return self.add_index(data)
+
+    def delete_index(self, index_name, ignore_missing=False):
         """Delete an index.
 
-        :param index_id: Index ID.
-        :type index_id: str | unicode
+        :param index_name: Index name.
+        :type index_name: str | unicode
         :param ignore_missing: Do not raise an exception on missing index.
         :type ignore_missing: bool
-        :return: True if index was deleted successfully, False if index was
+        :returns: True if index was deleted successfully, False if index was
             not found and **ignore_missing** was set to True.
         :rtype: bool
         :raise c8.exceptions.IndexDeleteError: If delete fails.
         """
         request = Request(
-            method='delete',
-            endpoint='/_api/index/{}/{}'.format(self.name, index_id)
+            method="delete", endpoint="/index/{}/{}".format(self.name, index_name)
         )
 
         def response_handler(resp):
             if resp.error_code == 1212 and ignore_missing:
                 return False
             if not resp.is_success:
                 raise IndexDeleteError(resp, request)
@@ -1211,15 +951,15 @@
     :type name: str | unicode
     """
 
     def __init__(self, connection, executor, name):
         super(StandardCollection, self).__init__(connection, executor, name)
 
     def __repr__(self):
-        return '<StandardCollection {}>'.format(self.name)
+        return "<StandardCollection {}>".format(self.name)
 
     def __getitem__(self, key):
         return self.get(key)
 
     def get(self, document, rev=None, check_rev=True):
         """Return a document.
 
@@ -1228,45 +968,80 @@
         :type document: str | unicode | dict
         :param rev: Expected document revision. Overrides the value of "_rev"
             field in **document** if present.
         :type rev: str | unicode
         :param check_rev: If set to True, revision of **document** (if given)
             is compared against the revision of target document.
         :type check_rev: bool
-        :return: Document, or None if not found.
+        :returns: Document, or None if not found.
         :rtype: dict | None
         :raise c8.exceptions.DocumentGetError: If retrieval fails.
         :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
         """
         handle, body, headers = self._prep_from_doc(document, rev, check_rev)
 
-        command = 'db.{}.exists({}) || undefined'.format(
-            self.name,
-            dumps(body)
-        ) if self._is_transaction else None
+        command = (
+            "db.{}.exists({}) || undefined".format(self.name, dumps(body))
+            if self._is_transaction
+            else None
+        )
 
         request = Request(
-            method='get',
-            endpoint='/_api/document/{}'.format(handle),
+            method="get",
+            endpoint="/document/{}".format(handle),
             headers=headers,
             command=command,
-            read=self.name
+            read=self.name,
         )
 
         def response_handler(resp):
             if resp.error_code == 1202:
                 return None
             if resp.status_code == 412:
                 raise DocumentRevisionError(resp, request)
             if not resp.is_success:
                 raise DocumentGetError(resp, request)
             return resp.body
 
         return self._execute(request, response_handler)
 
+    def insert_from_file(self, filepath, return_new=False, sync=None, silent=False):
+        """Insert a documents from csv file.
+        :param filepath: CSV or JSON file path which contains documents
+        :type filepath: str
+        :param return_new: Include body of the new document in the returned
+            metadata. Ignored if parameter **silent** is set to True.
+        :type return_new: bool
+        :param sync: Block until operation is synchronized to disk.
+        :type sync: bool
+        :param silent: If set to True, no document metadata is returned. This
+            can be used to save resources.
+        :type silent: bool
+        :returns: Document metadata (e.g. document key, revision) or True if
+            parameter **silent** was set to True.
+        :rtype: bool | dict
+        :raise c8.exceptions.DocumentInsertError: If insert fails.
+        """
+        result = []
+        if filepath.endswith(".csv"):
+            data = csv_reader(filepath)
+            data_dict = group_csv_key_values(data)
+            documents, index = get_documents_from_file(data_dict, 0)
+            resp = self.insert_many(documents, return_new, sync, silent)
+            result.append(resp)
+            return result
+
+        elif filepath.endswith(".json"):
+            documents = json_reader(filepath)
+            resp = self.insert_many(documents, return_new, sync, silent)
+            result.append(resp)
+            return result
+        else:
+            raise CollectionImportFromFileError("Invalid file")
+
     def insert(self, document, return_new=False, sync=None, silent=False):
         """Insert a new document.
 
         :param document: Document to insert. If it contains the "_key" or "_id"
             field, the value is used as the key of the new document (otherwise
             it is auto-generated). Any "_rev" field is ignored.
         :type document: dict
@@ -1274,52 +1049,49 @@
             metadata. Ignored if parameter **silent** is set to True.
         :type return_new: bool
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool
         :param silent: If set to True, no document metadata is returned. This
             can be used to save resources.
         :type silent: bool
-        :return: Document metadata (e.g. document key, revision) or True if
+        :returns: Document metadata (e.g. document key, revision) or True if
             parameter **silent** was set to True.
         :rtype: bool | dict
         :raise c8.exceptions.DocumentInsertError: If insert fails.
         """
+
         document = self._ensure_key_from_id(document)
 
-        params = {'returnNew': return_new, 'silent': silent}
+        params = {"returnNew": return_new, "silent": silent}
         if sync is not None:
-            params['waitForSync'] = sync
+            params["waitForSync"] = sync
 
-        command = 'db.{}.insert({},{})'.format(
-            self.name,
-            dumps(document),
-            dumps(params)
-        ) if self._is_transaction else None
+        command = (
+            "db.{}.insert({},{})".format(self.name, dumps(document), dumps(params))
+            if self._is_transaction
+            else None
+        )
 
         request = Request(
-            method='post',
-            endpoint='/_api/document/{}'.format(self.name),
+            method="post",
+            endpoint="/document/{}".format(self.name),
             data=document,
             params=params,
             command=command,
-            write=self.name
+            write=self.name,
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise DocumentInsertError(resp, request)
             return True if silent else resp.body
 
         return self._execute(request, response_handler)
 
-    def insert_many(self,
-                    documents,
-                    return_new=False,
-                    sync=None,
-                    silent=False):
+    def insert_many(self, documents, return_new=False, sync=None, silent=False):
         """Insert multiple documents.
 
         If inserting a document fails, the exception object is placed in the
         result list instead of document metadata.
 
         :param documents: List of new documents to insert. If they contain the
             "_key" or "_id" fields, the values are used as the keys of the new
@@ -1329,74 +1101,76 @@
             metadata. Ignored if parameter **silent** is set to True
         :type return_new: bool
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool
         :param silent: If set to True, no document metadata is returned. This
             can be used to save resources.
         :type silent: bool
-        :return: List of document metadata (e.g. document keys, revisions) and
+        :returns: List of document metadata (e.g. document keys, revisions) and
             any exception, or True if parameter **silent** was set to True.
         :rtype: [dict | C8Error] | bool
         :raise c8.exceptions.DocumentInsertError: If insert fails.
         """
         documents = [self._ensure_key_from_id(doc) for doc in documents]
 
-        params = {'returnNew': return_new, 'silent': silent}
+        params = {"returnNew": return_new, "silent": silent}
         if sync is not None:
-            params['waitForSync'] = sync
+            params["waitForSync"] = sync
 
-        command = 'db.{}.insert({},{})'.format(
-            self.name,
-            dumps(documents),
-            dumps(params)
-        ) if self._is_transaction else None
+        command = (
+            "db.{}.insert({},{})".format(self.name, dumps(documents), dumps(params))
+            if self._is_transaction
+            else None
+        )
 
         request = Request(
-            method='post',
-            endpoint='/_api/document/{}'.format(self.name),
+            method="post",
+            endpoint="/document/{}".format(self.name),
             data=documents,
             params=params,
             command=command,
-            write=self.name
+            write=self.name,
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise DocumentInsertError(resp, request)
             if silent is True:
                 return True
 
             results = []
             for result in resp.body:
-                if '_id' in result:
+                if "_id" in result:
                     results.append(result)
                 else:
                     sub_resp = Response(
                         method=resp.method,
                         url=resp.url,
                         headers=resp.headers,
                         status_code=resp.status_code,
                         status_text=resp.status_text,
-                        raw_body=result
+                        raw_body=result,
                     )
                     results.append(DocumentInsertError(sub_resp, request))
 
             return results
 
         return self._execute(request, response_handler)
 
-    def update(self,
-               document,
-               check_rev=True,
-               merge=True,
-               keep_none=True,
-               return_new=False,
-               return_old=False,
-               sync=None,
-               silent=False):
+    def update(
+        self,
+        document,
+        check_rev=True,
+        merge=True,
+        keep_none=True,
+        return_new=False,
+        return_old=False,
+        sync=None,
+        silent=False,
+    ):
         """Update a document.
 
         :param document: Partial or full document with the updated values. It
             must contain the "_id" or "_key" field.
         :type document: dict
         :param check_rev: If set to True, revision of **document** (if given)
             is compared against the revision of target document.
@@ -1412,70 +1186,72 @@
         :param return_old: Include body of the old document in the result.
         :type return_old: bool
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool
         :param silent: If set to True, no document metadata is returned. This
             can be used to save resources.
         :type silent: bool
-        :return: Document metadata (e.g. document key, revision) or True if
+        :returns: Document metadata (e.g. document key, revision) or True if
             parameter **silent** was set to True.
         :rtype: bool | dict
         :raise c8.exceptions.DocumentUpdateError: If update fails.
         :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
         """
         params = {
-            'keepNull': keep_none,
-            'mergeObjects': merge,
-            'returnNew': return_new,
-            'returnOld': return_old,
-            'ignoreRevs': not check_rev,
-            'overwrite': not check_rev,
-            'silent': silent
+            "keepNull": keep_none,
+            "mergeObjects": merge,
+            "returnNew": return_new,
+            "returnOld": return_old,
+            "ignoreRevs": not check_rev,
+            "overwrite": not check_rev,
+            "silent": silent,
         }
         if sync is not None:
-            params['waitForSync'] = sync
+            params["waitForSync"] = sync
 
-        command = 'db.{col}.update({doc},{doc},{opts})'.format(
-            col=self.name,
-            doc=dumps(document),
-            opts=dumps(params)
-        ) if self._is_transaction else None
+        command = (
+            "db.{col}.update({doc},{doc},{opts})".format(
+                col=self.name, doc=dumps(document), opts=dumps(params)
+            )
+            if self._is_transaction
+            else None
+        )
 
         request = Request(
-            method='patch',
-            endpoint='/_api/document/{}'.format(
-                self._extract_id(document)
-            ),
+            method="patch",
+            endpoint="/document/{}".format(self._extract_id(document)),
             data=document,
             params=params,
             command=command,
-            write=self.name
+            write=self.name,
         )
 
         def response_handler(resp):
             if resp.status_code == 412:
                 raise DocumentRevisionError(resp, request)
             elif not resp.is_success:
                 raise DocumentUpdateError(resp, request)
             if silent is True:
                 return True
-            resp.body['_old_rev'] = resp.body.pop('_oldRev')
+            resp.body["_old_rev"] = resp.body.pop("_oldRev")
             return resp.body
 
         return self._execute(request, response_handler)
 
-    def update_many(self,
-                    documents,
-                    check_rev=True,
-                    merge=True,
-                    keep_none=True,
-                    return_new=False,
-                    return_old=False,
-                    sync=None,
-                    silent=False):
+    def update_many(
+        self,
+        documents,
+        check_rev=True,
+        merge=True,
+        keep_none=True,
+        return_new=False,
+        return_old=False,
+        sync=None,
+        silent=False,
+    ):
         """Update multiple documents.
 
         If updating a document fails, the exception object is placed in the
         result list instead of document metadata.
 
         :param documents: Partial or full documents with the updated values.
             They must contain the "_id" or "_key" fields.
@@ -1494,148 +1270,87 @@
         :param return_old: Include bodies of the old documents in the result.
         :type return_old: bool
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool
         :param silent: If set to True, no document metadata is returned. This
             can be used to save resources.
         :type silent: bool
-        :return: List of document metadata (e.g. document keys, revisions) and
+        :returns: List of document metadata (e.g. document keys, revisions) and
             any exceptions, or True if parameter **silent** was set to True.
         :rtype: [dict | C8Error] | bool
         :raise c8.exceptions.DocumentUpdateError: If update fails.
         """
         params = {
-            'keepNull': keep_none,
-            'mergeObjects': merge,
-            'returnNew': return_new,
-            'returnOld': return_old,
-            'ignoreRevs': not check_rev,
-            'overwrite': not check_rev,
-            'silent': silent
+            "keepNull": keep_none,
+            "mergeObjects": merge,
+            "returnNew": return_new,
+            "returnOld": return_old,
+            "ignoreRevs": not check_rev,
+            "overwrite": not check_rev,
+            "silent": silent,
         }
         if sync is not None:
-            params['waitForSync'] = sync
+            params["waitForSync"] = sync
 
         documents = [self._ensure_key_in_body(doc) for doc in documents]
-        command = 'db.{col}.update({docs},{docs},{opts})'.format(
-            col=self.name,
-            docs=dumps(documents),
-            opts=dumps(params)
-        ) if self._is_transaction else None
+        command = (
+            "db.{col}.update({docs},{docs},{opts})".format(
+                col=self.name, docs=dumps(documents), opts=dumps(params)
+            )
+            if self._is_transaction
+            else None
+        )
 
         request = Request(
-            method='patch',
-            endpoint='/_api/document/{}'.format(self.name),
+            method="patch",
+            endpoint="/document/{}".format(self.name),
             data=documents,
             params=params,
             command=command,
-            write=self.name
+            write=self.name,
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise DocumentUpdateError(resp, request)
             if silent is True:
                 return True
 
             results = []
             for result in resp.body:
-                if '_id' not in result:
+                if "_id" not in result:
                     sub_resp = Response(
-                        method='patch',
+                        method="patch",
                         url=resp.url,
                         headers=resp.headers,
                         status_code=resp.status_code,
                         status_text=resp.status_text,
                         raw_body=result,
                     )
-                    if result['errorNum'] == 1200:
+                    if result["errorNum"] == 1200:
                         result = DocumentRevisionError(sub_resp, request)
                     else:
                         result = DocumentUpdateError(sub_resp, request)
                 else:
-                    result['_old_rev'] = result.pop('_oldRev')
+                    result["_old_rev"] = result.pop("_oldRev")
                 results.append(result)
 
             return results
 
         return self._execute(request, response_handler)
 
-    def update_match(self,
-                     filters,
-                     body,
-                     limit=None,
-                     keep_none=True,
-                     sync=None,
-                     merge=True):
-        """Update matching documents.
-
-        :param filters: Document filters.
-        :type filters: dict
-        :param body: Full or partial document body with the updates.
-        :type body: dict
-        :param limit: Max number of documents to update. If the limit is lower
-            than the number of matched documents, random documents are
-            chosen. This parameter is not supported on sharded collections.
-        :type limit: int
-        :param keep_none: If set to True, fields with value None are retained
-            in the document. Otherwise, they are removed completely.
-        :type keep_none: bool
-        :param sync: Block until operation is synchronized to disk.
-        :type sync: bool
-        :param merge: If set to True, sub-dictionaries are merged instead of
-            the new ones overwriting the old ones.
-        :type merge: bool
-        :return: Number of documents updated.
-        :rtype: int
-        :raise c8.exceptions.DocumentUpdateError: If update fails.
-        """
-        data = {
-            'collection': self.name,
-            'example': filters,
-            'newValue': body,
-            'keepNull': keep_none,
-            'mergeObjects': merge
-        }
-        if limit is not None:
-            data['limit'] = limit
-        if sync is not None:
-            data['waitForSync'] = sync
-
-        command = 'db.{}.updateByExample({},{},{})'.format(
-            self.name,
-            dumps(filters),
-            dumps(body),
-            dumps(data)
-        ) if self._is_transaction else None
-
-        request = Request(
-            method='put',
-            endpoint='/_api/simple/update-by-example',
-            data=data,
-            command=command,
-            write=self.name
-        )
-
-        def response_handler(resp):
-            if not resp.is_success:
-                raise DocumentUpdateError(resp, request)
-            if self._is_transaction:
-                return resp.body
-            return resp.body['updated']
-
-        return self._execute(request, response_handler)
-
-    def replace(self,
-                document,
-                check_rev=True,
-                return_new=False,
-                return_old=False,
-                sync=None,
-                silent=False):
+    def replace(
+        self,
+        document,
+        check_rev=True,
+        return_new=False,
+        return_old=False,
+        sync=None,
+        silent=False,
+    ):
         """Replace a document.
 
         :param document: New document to replace the old one with. It must
             contain the "_id" or "_key" field. Edge document must also have
             "_from" and "_to" fields.
         :type document: dict
         :param check_rev: If set to True, revision of **document** (if given)
@@ -1646,66 +1361,68 @@
         :param return_old: Include body of the old document in the result.
         :type return_old: bool
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool
         :param silent: If set to True, no document metadata is returned. This
             can be used to save resources.
         :type silent: bool
-        :return: Document metadata (e.g. document key, revision) or True if
+        :returns: Document metadata (e.g. document key, revision) or True if
             parameter **silent** was set to True.
         :rtype: bool | dict
         :raise c8.exceptions.DocumentReplaceError: If replace fails.
         :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
         """
         params = {
-            'returnNew': return_new,
-            'returnOld': return_old,
-            'ignoreRevs': not check_rev,
-            'overwrite': not check_rev,
-            'silent': silent
+            "returnNew": return_new,
+            "returnOld": return_old,
+            "ignoreRevs": not check_rev,
+            "overwrite": not check_rev,
+            "silent": silent,
         }
         if sync is not None:
-            params['waitForSync'] = sync
+            params["waitForSync"] = sync
 
-        command = 'db.{col}.replace({doc},{doc},{opts})'.format(
-            col=self.name,
-            doc=dumps(document),
-            opts=dumps(params)
-        ) if self._is_transaction else None
+        command = (
+            "db.{col}.replace({doc},{doc},{opts})".format(
+                col=self.name, doc=dumps(document), opts=dumps(params)
+            )
+            if self._is_transaction
+            else None
+        )
 
         request = Request(
-            method='put',
-            endpoint='/_api/document/{}'.format(
-                self._extract_id(document)
-            ),
+            method="put",
+            endpoint="/document/{}".format(self._extract_id(document)),
             params=params,
             data=document,
             command=command,
-            write=self.name
+            write=self.name,
         )
 
         def response_handler(resp):
             if resp.status_code == 412:
                 raise DocumentRevisionError(resp, request)
             if not resp.is_success:
                 raise DocumentReplaceError(resp, request)
             if silent is True:
                 return True
-            resp.body['_old_rev'] = resp.body.pop('_oldRev')
+            resp.body["_old_rev"] = resp.body.pop("_oldRev")
             return resp.body
 
         return self._execute(request, response_handler)
 
-    def replace_many(self,
-                     documents,
-                     check_rev=True,
-                     return_new=False,
-                     return_old=False,
-                     sync=None,
-                     silent=False):
+    def replace_many(
+        self,
+        documents,
+        check_rev=True,
+        return_new=False,
+        return_old=False,
+        sync=None,
+        silent=False,
+    ):
         """Replace multiple documents.
 
         If replacing a document fails, the exception object is placed in the
         result list instead of document metadata.
 
         :param documents: New documents to replace the old ones with. They must
             contain the "_id" or "_key" fields. Edge documents must also have
@@ -1719,132 +1436,86 @@
         :param return_old: Include bodies of the old documents in the result.
         :type return_old: bool
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool
         :param silent: If set to True, no document metadata is returned. This
             can be used to save resources.
         :type silent: bool
-        :return: List of document metadata (e.g. document keys, revisions) and
+        :returns: List of document metadata (e.g. document keys, revisions) and
             any exceptions, or True if parameter **silent** was set to True.
         :rtype: [dict | C8Error] | bool
         :raise c8.exceptions.DocumentReplaceError: If replace fails.
         """
         params = {
-            'returnNew': return_new,
-            'returnOld': return_old,
-            'ignoreRevs': not check_rev,
-            'overwrite': not check_rev,
-            'silent': silent
+            "returnNew": return_new,
+            "returnOld": return_old,
+            "ignoreRevs": not check_rev,
+            "overwrite": not check_rev,
+            "silent": silent,
         }
         if sync is not None:
-            params['waitForSync'] = sync
+            params["waitForSync"] = sync
 
         documents = [self._ensure_key_in_body(doc) for doc in documents]
-        command = 'db.{col}.replace({docs},{docs},{opts})'.format(
-            col=self.name,
-            docs=dumps(documents),
-            opts=dumps(params)
-        ) if self._is_transaction else None
+        command = (
+            "db.{col}.replace({docs},{docs},{opts})".format(
+                col=self.name, docs=dumps(documents), opts=dumps(params)
+            )
+            if self._is_transaction
+            else None
+        )
 
         request = Request(
-            method='put',
-            endpoint='/_api/document/{}'.format(self.name),
+            method="put",
+            endpoint="/document/{}".format(self.name),
             params=params,
             data=documents,
             command=command,
-            write=self.name
+            write=self.name,
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise DocumentReplaceError(resp, request)
             if silent is True:
                 return True
 
             results = []
             for result in resp.body:
-                if '_id' not in result:
+                if "_id" not in result:
                     sub_resp = Response(
                         method=resp.method,
                         url=resp.url,
                         headers=resp.headers,
                         status_code=resp.status_code,
                         status_text=resp.status_text,
-                        raw_body=result
+                        raw_body=result,
                     )
-                    if result['errorNum'] == 1200:
+                    if result["errorNum"] == 1200:
                         result = DocumentRevisionError(sub_resp, request)
                     else:
                         result = DocumentReplaceError(sub_resp, request)
                 else:
-                    result['_old_rev'] = result.pop('_oldRev')
+                    result["_old_rev"] = result.pop("_oldRev")
                 results.append(result)
 
             return results
 
         return self._execute(request, response_handler)
 
-    def replace_match(self, filters, body, limit=None, sync=None):
-        """Replace matching documents.
-
-        :param filters: Document filters.
-        :type filters: dict
-        :param body: New document body.
-        :type body: dict
-        :param limit: Max number of documents to replace. If the limit is lower
-            than the number of matched documents, random documents are chosen.
-        :type limit: int
-        :param sync: Block until operation is synchronized to disk.
-        :type sync: bool
-        :return: Number of documents replaced.
-        :rtype: int
-        :raise c8.exceptions.DocumentReplaceError: If replace fails.
-        """
-        data = {
-            'collection': self.name,
-            'example': filters,
-            'newValue': body
-        }
-        if limit is not None:
-            data['limit'] = limit
-        if sync is not None:
-            data['waitForSync'] = sync
-
-        command = 'db.{}.replaceByExample({},{},{})'.format(
-            self.name,
-            dumps(filters),
-            dumps(body),
-            dumps(data)
-        ) if self._is_transaction else None
-
-        request = Request(
-            method='put',
-            endpoint='/_api/simple/replace-by-example',
-            data=data,
-            command=command,
-            write=self.name
-        )
-
-        def response_handler(resp):
-            if not resp.is_success:
-                raise DocumentReplaceError(resp, request)
-            if self._is_transaction:
-                return resp.body
-            return resp.body['replaced']
-
-        return self._execute(request, response_handler)
-
-    def delete(self,
-               document,
-               rev=None,
-               check_rev=True,
-               ignore_missing=False,
-               return_old=False,
-               sync=None,
-               silent=False):
+    def delete(
+        self,
+        document,
+        rev=None,
+        check_rev=True,
+        ignore_missing=False,
+        return_old=False,
+        sync=None,
+        silent=False,
+    ):
         """Delete a document.
 
         :param document: Document ID, key or body. Document body must contain
             the "_id" or "_key" field.
         :type document: str | unicode | dict
         :param rev: Expected document revision. Overrides the value of "_rev"
             field in **document** if present.
@@ -1859,65 +1530,62 @@
         :param return_old: Include body of the old document in the result.
         :type return_old: bool
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool
         :param silent: If set to True, no document metadata is returned. This
             can be used to save resources.
         :type silent: bool
-        :return: Document metadata (e.g. document key, revision), or True if
+        :returns: Document metadata (e.g. document key, revision), or True if
             parameter **silent** was set to True, or False if document was not
             found and **ignore_missing** was set to True (does not apply in
             transactions).
         :rtype: bool | dict
         :raise c8.exceptions.DocumentDeleteError: If delete fails.
         :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
         """
         handle, body, headers = self._prep_from_doc(document, rev, check_rev)
 
         params = {
-            'returnOld': return_old,
-            'ignoreRevs': not check_rev,
-            'overwrite': not check_rev,
-            'silent': silent
+            "returnOld": return_old,
+            "ignoreRevs": not check_rev,
+            "overwrite": not check_rev,
+            "silent": silent,
         }
         if sync is not None:
-            params['waitForSync'] = sync
+            params["waitForSync"] = sync
 
-        command = 'db.{}.remove({},{})'.format(
-            self.name,
-            dumps(body),
-            dumps(params)
-        ) if self._is_transaction else None
+        command = (
+            "db.{}.remove({},{})".format(self.name, dumps(body), dumps(params))
+            if self._is_transaction
+            else None
+        )
 
         request = Request(
-            method='delete',
-            endpoint='/_api/document/{}'.format(handle),
+            method="delete",
+            endpoint="/document/{}".format(handle),
             params=params,
             headers=headers,
             command=command,
-            write=self.name
+            write=self.name,
         )
 
         def response_handler(resp):
             if resp.error_code == 1202 and ignore_missing:
                 return False
             if resp.status_code == 412:
                 raise DocumentRevisionError(resp, request)
             if not resp.is_success:
                 raise DocumentDeleteError(resp, request)
             return True if silent else resp.body
 
         return self._execute(request, response_handler)
 
-    def delete_many(self,
-                    documents,
-                    return_old=False,
-                    check_rev=True,
-                    sync=None,
-                    silent=False):
+    def delete_many(
+        self, documents, return_old=False, check_rev=True, sync=None, silent=False
+    ):
         """Delete multiple documents.
 
         If deleting a document fails, the exception object is placed in the
         result list instead of document metadata.
 
         :param documents: Document IDs, keys or bodies. Document bodies must
             contain the "_id" or "_key" fields.
@@ -1928,197 +1596,112 @@
             are compared against the revisions of target documents.
         :type check_rev: bool
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool
         :param silent: If set to True, no document metadata is returned. This
             can be used to save resources.
         :type silent: bool
-        :return: List of document metadata (e.g. document keys, revisions) and
+        :returns: List of document metadata (e.g. document keys, revisions) and
             any exceptions, or True if parameter **silent** was set to True.
         :rtype: [dict | C8Error] | bool
         :raise c8.exceptions.DocumentDeleteError: If delete fails.
         """
         params = {
-            'returnOld': return_old,
-            'ignoreRevs': not check_rev,
-            'overwrite': not check_rev,
-            'silent': silent
+            "returnOld": return_old,
+            "ignoreRevs": not check_rev,
+            "overwrite": not check_rev,
+            "silent": silent,
         }
         if sync is not None:
-            params['waitForSync'] = sync
+            params["waitForSync"] = sync
 
         documents = [
             self._ensure_key_in_body(doc) if isinstance(doc, dict) else doc
             for doc in documents
         ]
-        command = 'db.{}.remove({},{})'.format(
-            self.name,
-            dumps(documents),
-            dumps(params)
-        ) if self._is_transaction else None
+        command = (
+            "db.{}.remove({},{})".format(self.name, dumps(documents), dumps(params))
+            if self._is_transaction
+            else None
+        )
 
         request = Request(
-            method='delete',
-            endpoint='/_api/document/{}'.format(self.name),
+            method="delete",
+            endpoint="/document/{}".format(self.name),
             params=params,
             data=documents,
             command=command,
-            write=self.name
+            write=self.name,
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise DocumentDeleteError(resp, request)
             if silent is True:
                 return True
 
             results = []
             for result in resp.body:
-                if '_id' not in result:
+                if "_id" not in result:
                     sub_resp = Response(
                         method=resp.method,
                         url=resp.url,
                         headers=resp.headers,
                         status_code=resp.status_code,
                         status_text=resp.status_text,
-                        raw_body=result
+                        raw_body=result,
                     )
-                    if result['errorNum'] == 1200:
+                    if result["errorNum"] == 1200:
                         result = DocumentRevisionError(sub_resp, request)
                     else:
                         result = DocumentDeleteError(sub_resp, request)
                 results.append(result)
 
             return results
 
         return self._execute(request, response_handler)
 
-    def delete_match(self, filters, limit=None, sync=None):
-        """Delete matching documents.
-
-        :param filters: Document filters.
-        :type filters: dict
-        :param limit: Max number of documents to delete. If the limit is lower
-            than the number of matched documents, random documents are chosen.
-        :type limit: int
-        :param sync: Block until operation is synchronized to disk.
-        :type sync: bool
-        :return: Number of documents deleted.
-        :rtype: dict
-        :raise c8.exceptions.DocumentDeleteError: If delete fails.
-        """
-        data = {'collection': self.name, 'example': filters}
-        if sync is not None:
-            data['waitForSync'] = sync
-        if limit is not None and limit != 0:
-            data['limit'] = limit
-
-        command = 'db.{}.removeByExample({},{})'.format(
-            self.name,
-            dumps(filters),
-            dumps(data)
-        ) if self._is_transaction else None
-
-        request = Request(
-            method='put',
-            endpoint='/_api/simple/remove-by-example',
-            data=data,
-            command=command,
-            write=self.name
-        )
-
-        def response_handler(resp):
-            if not resp.is_success:
-                raise DocumentDeleteError(resp, request)
-            if self._is_transaction:
-                return resp.body
-            return resp.body['deleted']
-
-        return self._execute(request, response_handler)
-
-    def import_bulk(self,
-                    documents,
-                    halt_on_error=True,
-                    details=True,
-                    from_prefix=None,
-                    to_prefix=None,
-                    overwrite=None,
-                    on_duplicate=None,
-                    sync=None):
+    def import_bulk(self, documents, details=True, primaryKey=None, replace=False):
         """Insert multiple documents into the collection.
 
         This is faster than :func:`c8.collection.Collection.insert_many`
         but does not return as much information.
 
         :param documents: List of new documents to insert. If they contain the
             "_key" or "_id" fields, the values are used as the keys of the new
             documents (auto-generated otherwise). Any "_rev" field is ignored.
         :type documents: [dict]
-        :param halt_on_error: Halt the entire import on an error.
-        :type halt_on_error: bool
         :param details: If set to True, the returned result will include an
             additional list of detailed error messages.
         :type details: bool
-        :param from_prefix: String prefix prepended to the value of "_from"
-            field in each edge document inserted. For example, prefix "foo"
-            prepended to "_from": "bar" will result in "_from": "foo/bar".
-            Applies only to edge collections.
-        :type from_prefix: str | unicode
-        :param to_prefix: String prefix prepended to the value of "_to" field
-            in edge document inserted. For example, prefix "foo" prepended to
-            "_to": "bar" will result in "_to": "foo/bar". Applies only to edge
-            collections.
-        :type to_prefix: str | unicode
-        :param overwrite: If set to True, all existing documents are removed
-            prior to the import. Indexes are still preserved.
-        :type overwrite: bool
-        :param on_duplicate: Action to take on unique key constraint violations
-            (for documents with "_key" fields). Allowed values are "error" (do
-            not import the new documents and count them as errors), "update"
-            (update the existing documents while preserving any fields missing
-            in the new ones), "replace" (replace the existing documents with
-            new ones), and  "ignore" (do not import the new documents and count
-            them as ignored, as opposed to counting them as errors). Options
-            "update" and "replace" may fail on secondary unique key constraint
-            violations.
-        :type on_duplicate: str | unicode
-        :param sync: Block until operation is synchronized to disk.
-        :type sync: bool
-        :return: Result of the bulk import.
+        :param primaryKey: If not None then uses this field as the primary key for
+            the documents to be inserted.
+        :type primaryKey: str | unicode
+        :param replace: Action to take on unique key constraint violations
+            (for documents with "_key" fields). A bool "replace" if set to true replaces
+            the existing documents with new ones else it won't replace the documents and
+            count it as "error".
+        :type replace: bool
+        :returns: Result of the bulk import.
         :rtype: dict
         :raise c8.exceptions.DocumentInsertError: If import fails.
         """
+        data = {}
         documents = [self._ensure_key_from_id(doc) for doc in documents]
+        data["data"] = documents
 
-        params = {
-            'type': 'array',
-            'collection': self.name,
-            'complete': halt_on_error,
-            'details': details,
-        }
-        if halt_on_error is not None:
-            params['complete'] = halt_on_error
         if details is not None:
-            params['details'] = details
-        if from_prefix is not None:
-            params['fromPrefix'] = from_prefix
-        if to_prefix is not None:
-            params['toPrefix'] = to_prefix
-        if overwrite is not None:
-            params['overwrite'] = overwrite
-        if on_duplicate is not None:
-            params['onDuplicate'] = on_duplicate
-        if sync is not None:
-            params['waitForSync'] = sync
+            data["details"] = details
+        if primaryKey is not None:
+            data["primaryKey"] = primaryKey
+        if replace is not None:
+            data["replace"] = replace
 
         request = Request(
-            method='post',
-            endpoint='/_api/import',
-            data=documents,
-            params=params
+            method="post", endpoint="/import/{}".format(self.name), data=data
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise DocumentInsertError(resp, request)
             return resp.body
 
@@ -2139,24 +1722,24 @@
     """
 
     def __init__(self, connection, executor, graph, name):
         super(VertexCollection, self).__init__(connection, executor, name)
         self._graph = graph
 
     def __repr__(self):
-        return '<VertexCollection {}>'.format(self.name)
+        return "<VertexCollection {}>".format(self.name)
 
     def __getitem__(self, key):
         return self.get(key)
 
     @property
     def graph(self):
         """Return the graph name.
 
-        :return: Graph name.
+        :returns: Graph name.
         :rtype: str | unicode
         """
         return self._graph
 
     def get(self, vertex, rev=None, check_rev=True):
         """Return a vertex document.
 
@@ -2165,47 +1748,45 @@
         :type vertex: str | unicode | dict
         :param rev: Expected document revision. Overrides the value of "_rev"
             field in **vertex** if present.
         :type rev: str | unicode
         :param check_rev: If set to True, revision of **vertex** (if given) is
             compared against the revision of target vertex document.
         :type check_rev: bool
-        :return: Vertex document or None if not found.
+        :returns: Vertex document or None if not found.
         :rtype: dict | None
         :raise c8.exceptions.DocumentGetError: If retrieval fails.
         :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
         """
         handle, body, headers = self._prep_from_doc(vertex, rev, check_rev)
 
-        command = 'gm._graph("{}").{}.document({})'.format(
-            self.graph,
-            self.name,
-            dumps(body)
-        ) if self._is_transaction else None
+        command = (
+            'gm._graph("{}").{}.document({})'.format(self.graph, self.name, dumps(body))
+            if self._is_transaction
+            else None
+        )
 
         request = Request(
-            method='get',
-            endpoint='/_api/graph/{}/vertex/{}'.format(
-                self._graph, handle
-            ),
+            method="get",
+            endpoint="/graph/{}/vertex/{}".format(self._graph, handle),
             headers=headers,
             command=command,
-            read=self.name
+            read=self.name,
         )
 
         def response_handler(resp):
             if resp.error_code == 1202:
                 return None
             if resp.status_code == 412:
                 raise DocumentRevisionError(resp, request)
             if not resp.is_success:
                 raise DocumentGetError(resp, request)
             if self._is_transaction:
                 return resp.body
-            return resp.body['vertex']
+            return resp.body["vertex"]
 
         return self._execute(request, response_handler)
 
     def insert(self, vertex, sync=None, silent=False):
         """Insert a new vertex document.
 
         :param vertex: New vertex document to insert. If it has "_key" or "_id"
@@ -2213,60 +1794,54 @@
             auto-generated). Any "_rev" field is ignored.
         :type vertex: dict
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool
         :param silent: If set to True, no document metadata is returned. This
             can be used to save resources.
         :type silent: bool
-        :return: Document metadata (e.g. document key, revision) or True if
+        :returns: Document metadata (e.g. document key, revision) or True if
             parameter **silent** was set to True.
         :rtype: bool | dict
         :raise c8.exceptions.DocumentInsertError: If insert fails.
         """
         vertex = self._ensure_key_from_id(vertex)
 
-        params = {'silent': silent}
+        params = {"silent": silent}
         if sync is not None:
-            params['waitForSync'] = sync
+            params["waitForSync"] = sync
 
-        command = 'gm._graph("{}").{}.save({},{})'.format(
-            self.graph,
-            self.name,
-            dumps(vertex),
-            dumps(params)
-        ) if self._is_transaction else None
+        command = (
+            'gm._graph("{}").{}.save({},{})'.format(
+                self.graph, self.name, dumps(vertex), dumps(params)
+            )
+            if self._is_transaction
+            else None
+        )
 
         request = Request(
-            method='post',
-            endpoint='/_api/graph/{}/vertex/{}'.format(
-                self._graph, self.name
-            ),
+            method="post",
+            endpoint="/graph/{}/vertex/{}".format(self._graph, self.name),
             data=vertex,
             params=params,
             command=command,
-            write=self.name
+            write=self.name,
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise DocumentInsertError(resp, request)
             if silent is True:
                 return True
             if self._is_transaction:
                 return resp.body
-            return resp.body['vertex']
+            return resp.body["vertex"]
 
         return self._execute(request, response_handler)
 
-    def update(self,
-               vertex,
-               check_rev=True,
-               keep_none=True,
-               sync=None,
-               silent=False):
+    def update(self, vertex, check_rev=True, keep_none=True, sync=None, silent=False):
         """Update a vertex document.
 
         :param vertex: Partial or full vertex document with updated values. It
             must contain the "_key" or "_id" field.
         :type vertex: dict
         :param check_rev: If set to True, revision of **vertex** (if given) is
             compared against the revision of target vertex document.
@@ -2275,62 +1850,56 @@
             in the document. If set to False, they are removed completely.
         :type keep_none: bool
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool
         :param silent: If set to True, no document metadata is returned. This
             can be used to save resources.
         :type silent: bool
-        :return: Document metadata (e.g. document key, revision) or True if
+        :returns: Document metadata (e.g. document key, revision) or True if
             parameter **silent** was set to True.
         :rtype: bool | dict
         :raise c8.exceptions.DocumentUpdateError: If update fails.
         :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
         """
         vertex_id, headers = self._prep_from_body(vertex, check_rev)
 
-        params = {
-            'keepNull': keep_none,
-            'overwrite': not check_rev,
-            'silent': silent
-        }
+        params = {"keepNull": keep_none, "overwrite": not check_rev, "silent": silent}
         if sync is not None:
-            params['waitForSync'] = sync
+            params["waitForSync"] = sync
 
-        command = 'gm._graph("{}").{}.update("{}",{},{})'.format(
-            self.graph,
-            self.name,
-            vertex_id,
-            dumps(vertex),
-            dumps(params)
-        ) if self._is_transaction else None
+        command = (
+            'gm._graph("{}").{}.update("{}",{},{})'.format(
+                self.graph, self.name, vertex_id, dumps(vertex), dumps(params)
+            )
+            if self._is_transaction
+            else None
+        )
 
         request = Request(
-            method='patch',
-            endpoint='/_api/graph/{}/vertex/{}'.format(
-                self._graph, vertex_id
-            ),
+            method="patch",
+            endpoint="/graph/{}/vertex/{}".format(self._graph, vertex_id),
             headers=headers,
             params=params,
             data=vertex,
             command=command,
-            write=self.name
+            write=self.name,
         )
 
         def response_handler(resp):
             if resp.status_code == 412:
                 raise DocumentRevisionError(resp, request)
             elif not resp.is_success:
                 raise DocumentUpdateError(resp, request)
             if silent is True:
                 return True
             if self._is_transaction:
                 result = resp.body
             else:
-                result = resp.body['vertex']
-            result['_old_rev'] = result.pop('_oldRev')
+                result = resp.body["vertex"]
+            result["_old_rev"] = result.pop("_oldRev")
             return result
 
         return self._execute(request, response_handler)
 
     def replace(self, vertex, check_rev=True, sync=None, silent=False):
         """Replace a vertex document.
 
@@ -2341,68 +1910,61 @@
             compared against the revision of target vertex document.
         :type check_rev: bool
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool
         :param silent: If set to True, no document metadata is returned. This
             can be used to save resources.
         :type silent: bool
-        :return: Document metadata (e.g. document key, revision) or True if
+        :returns: Document metadata (e.g. document key, revision) or True if
             parameter **silent** was set to True.
         :rtype: bool | dict
         :raise c8.exceptions.DocumentReplaceError: If replace fails.
         :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
         """
         vertex_id, headers = self._prep_from_body(vertex, check_rev)
 
-        params = {'silent': silent}
+        params = {"silent": silent}
         if sync is not None:
-            params['waitForSync'] = sync
+            params["waitForSync"] = sync
 
-        command = 'gm._graph("{}").{}.replace("{}",{},{})'.format(
-            self.graph,
-            self.name,
-            vertex_id,
-            dumps(vertex),
-            dumps(params)
-        ) if self._is_transaction else None
+        command = (
+            'gm._graph("{}").{}.replace("{}",{},{})'.format(
+                self.graph, self.name, vertex_id, dumps(vertex), dumps(params)
+            )
+            if self._is_transaction
+            else None
+        )
 
         request = Request(
-            method='put',
-            endpoint='/_api/graph/{}/vertex/{}'.format(
-                self._graph, vertex_id
-            ),
+            method="put",
+            endpoint="/graph/{}/vertex/{}".format(self._graph, vertex_id),
             headers=headers,
             params=params,
             data=vertex,
             command=command,
-            write=self.name
+            write=self.name,
         )
 
         def response_handler(resp):
             if resp.status_code == 412:
                 raise DocumentRevisionError(resp, request)
             elif not resp.is_success:
                 raise DocumentReplaceError(resp, request)
             if silent is True:
                 return True
             if self._is_transaction:
                 result = resp.body
             else:
-                result = resp.body['vertex']
-            result['_old_rev'] = result.pop('_oldRev')
+                result = resp.body["vertex"]
+            result["_old_rev"] = result.pop("_oldRev")
             return result
 
         return self._execute(request, response_handler)
 
-    def delete(self,
-               vertex,
-               rev=None,
-               check_rev=True,
-               ignore_missing=False,
-               sync=None):
+    def delete(self, vertex, rev=None, check_rev=True, ignore_missing=False, sync=None):
         """Delete a vertex document.
 
         :param vertex: Vertex document ID, key or body. Document body must
             contain the "_id" or "_key" field.
         :type vertex: str | unicode | dict
         :param rev: Expected document revision. Overrides the value of "_rev"
             field in **vertex** if present.
@@ -2412,40 +1974,39 @@
         :type check_rev: bool
         :param ignore_missing: Do not raise an exception on missing document.
             This parameter has no effect in transactions where an exception is
             always raised on failures.
         :type ignore_missing: bool
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool
-        :return: True if vertex was deleted successfully, False if vertex was
+        :returns: True if vertex was deleted successfully, False if vertex was
             not found and **ignore_missing** was set to True (does not apply in
             transactions).
         :rtype: bool
         :raise c8.exceptions.DocumentDeleteError: If delete fails.
         :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
         """
         handle, _, headers = self._prep_from_doc(vertex, rev, check_rev)
 
-        params = {} if sync is None else {'waitForSync': sync}
-        command = 'gm._graph("{}").{}.remove("{}",{})'.format(
-            self.graph,
-            self.name,
-            handle,
-            dumps(params)
-        ) if self._is_transaction else None
+        params = {} if sync is None else {"waitForSync": sync}
+        command = (
+            'gm._graph("{}").{}.remove("{}",{})'.format(
+                self.graph, self.name, handle, dumps(params)
+            )
+            if self._is_transaction
+            else None
+        )
 
         request = Request(
-            method='delete',
-            endpoint='/_api/graph/{}/vertex/{}'.format(
-                self._graph, handle
-            ),
+            method="delete",
+            endpoint="/graph/{}/vertex/{}".format(self._graph, handle),
             params=params,
             headers=headers,
             command=command,
-            write=self.name
+            write=self.name,
         )
 
         def response_handler(resp):
             if resp.error_code == 1202 and ignore_missing:
                 return False
             if resp.status_code == 412:
                 raise DocumentRevisionError(resp, request)
@@ -2470,24 +2031,24 @@
     """
 
     def __init__(self, connection, executor, graph, name):
         super(EdgeCollection, self).__init__(connection, executor, name)
         self._graph = graph
 
     def __repr__(self):
-        return '<EdgeCollection {}>'.format(self.name)
+        return "<EdgeCollection {}>".format(self.name)
 
     def __getitem__(self, key):
         return self.get(key)
 
     @property
     def graph(self):
         """Return the graph name.
 
-        :return: Graph name.
+        :returns: Graph name.
         :rtype: str | unicode
         """
         return self._graph
 
     def get(self, edge, rev=None, check_rev=True):
         """Return an edge document.
 
@@ -2496,47 +2057,45 @@
         :type edge: str | unicode | dict
         :param rev: Expected document revision. Overrides the value of "_rev"
             field in **edge** if present.
         :type rev: str | unicode
         :param check_rev: If set to True, revision of **edge** (if given) is
             compared against the revision of target edge document.
         :type check_rev: bool
-        :return: Edge document or None if not found.
+        :returns: Edge document or None if not found.
         :rtype: dict | None
         :raise c8.exceptions.DocumentGetError: If retrieval fails.
         :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
         """
         handle, body, headers = self._prep_from_doc(edge, rev, check_rev)
 
-        command = 'gm._graph("{}").{}.document({})'.format(
-            self.graph,
-            self.name,
-            dumps(body)
-        ) if self._is_transaction else None
+        command = (
+            'gm._graph("{}").{}.document({})'.format(self.graph, self.name, dumps(body))
+            if self._is_transaction
+            else None
+        )
 
         request = Request(
-            method='get',
-            endpoint='/_api/graph/{}/edge/{}'.format(
-                self._graph, handle
-            ),
+            method="get",
+            endpoint="/graph/{}/edge/{}".format(self._graph, handle),
             headers=headers,
             command=command,
-            read=self.name
+            read=self.name,
         )
 
         def response_handler(resp):
             if resp.error_code == 1202:
                 return None
             if resp.status_code == 412:
                 raise DocumentRevisionError(resp, request)
             if not resp.is_success:
                 raise DocumentGetError(resp, request)
             if self._is_transaction:
                 return resp.body
-            return resp.body['edge']
+            return resp.body["edge"]
 
         return self._execute(request, response_handler)
 
     def insert(self, edge, sync=None, silent=False):
         """Insert a new edge document.
 
         :param edge: New edge document to insert. It must contain "_from" and
@@ -2545,62 +2104,59 @@
             Any "_rev" field is ignored.
         :type edge: dict
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool
         :param silent: If set to True, no document metadata is returned. This
             can be used to save resources.
         :type silent: bool
-        :return: Document metadata (e.g. document key, revision) or True if
+        :returns: Document metadata (e.g. document key, revision) or True if
             parameter **silent** was set to True.
         :rtype: bool | dict
         :raise c8.exceptions.DocumentInsertError: If insert fails.
         """
         edge = self._ensure_key_from_id(edge)
 
-        params = {'silent': silent}
+        params = {"silent": silent}
         if sync is not None:
-            params['waitForSync'] = sync
+            params["waitForSync"] = sync
+
+        command = (
+            'gm._graph("{}").{}.save("{}","{}",{},{})'.format(
+                self.graph,
+                self.name,
+                edge["_from"],
+                edge["_to"],
+                dumps(edge),
+                dumps(params),
+            )
+            if self._is_transaction
+            else None
+        )
 
-        command = 'gm._graph("{}").{}.save("{}","{}",{},{})'.format(
-            self.graph,
-            self.name,
-            edge['_from'],
-            edge['_to'],
-            dumps(edge),
-            dumps(params)
-        ) if self._is_transaction else None
-
-        request = Request(
-            method='post',
-            endpoint='/_api/graph/{}/edge/{}'.format(
-                self._graph, self.name
-            ),
+        request = Request(
+            method="post",
+            endpoint="/graph/{}/edge/{}".format(self._graph, self.name),
             data=edge,
             params=params,
             command=command,
-            write=self.name
+            write=self.name,
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise DocumentInsertError(resp, request)
             if silent is True:
                 return True
             if self._is_transaction:
                 return resp.body
-            return resp.body['edge']
+            return resp.body["edge"]
 
         return self._execute(request, response_handler)
 
-    def update(self,
-               edge,
-               check_rev=True,
-               keep_none=True,
-               sync=None,
-               silent=False):
+    def update(self, edge, check_rev=True, keep_none=True, sync=None, silent=False):
         """Update an edge document.
 
         :param edge: Partial or full edge document with updated values. It must
             contain the "_key" or "_id" field.
         :type edge: dict
         :param check_rev: If set to True, revision of **edge** (if given) is
             compared against the revision of target edge document.
@@ -2609,62 +2165,56 @@
             in the document. If set to False, they are removed completely.
         :type keep_none: bool
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool
         :param silent: If set to True, no document metadata is returned. This
             can be used to save resources.
         :type silent: bool
-        :return: Document metadata (e.g. document key, revision) or True if
+        :returns: Document metadata (e.g. document key, revision) or True if
             parameter **silent** was set to True.
         :rtype: bool | dict
         :raise c8.exceptions.DocumentUpdateError: If update fails.
         :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
         """
         edge_id, headers = self._prep_from_body(edge, check_rev)
 
-        params = {
-            'keepNull': keep_none,
-            'overwrite': not check_rev,
-            'silent': silent
-        }
+        params = {"keepNull": keep_none, "overwrite": not check_rev, "silent": silent}
         if sync is not None:
-            params['waitForSync'] = sync
+            params["waitForSync"] = sync
 
-        command = 'gm._graph("{}").{}.update("{}",{},{})'.format(
-            self.graph,
-            self.name,
-            edge_id,
-            dumps(edge),
-            dumps(params)
-        ) if self._is_transaction else None
+        command = (
+            'gm._graph("{}").{}.update("{}",{},{})'.format(
+                self.graph, self.name, edge_id, dumps(edge), dumps(params)
+            )
+            if self._is_transaction
+            else None
+        )
 
         request = Request(
-            method='patch',
-            endpoint='/_api/graph/{}/edge/{}'.format(
-                self._graph, edge_id
-            ),
+            method="patch",
+            endpoint="/graph/{}/edge/{}".format(self._graph, edge_id),
             headers=headers,
             params=params,
             data=edge,
             command=command,
-            write=self.name
+            write=self.name,
         )
 
         def response_handler(resp):
             if resp.status_code == 412:
                 raise DocumentRevisionError(resp, request)
             if not resp.is_success:
                 raise DocumentUpdateError(resp, request)
             if silent is True:
                 return True
             if self._is_transaction:
                 result = resp.body
             else:
-                result = resp.body['edge']
-            result['_old_rev'] = result.pop('_oldRev')
+                result = resp.body["edge"]
+            result["_old_rev"] = result.pop("_oldRev")
             return result
 
         return self._execute(request, response_handler)
 
     def replace(self, edge, check_rev=True, sync=None, silent=False):
         """Replace an edge document.
 
@@ -2676,68 +2226,61 @@
             compared against the revision of target edge document.
         :type check_rev: bool
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool
         :param silent: If set to True, no document metadata is returned. This
             can be used to save resources.
         :type silent: bool
-        :return: Document metadata (e.g. document key, revision) or True if
+        :returns: Document metadata (e.g. document key, revision) or True if
             parameter **silent** was set to True.
         :rtype: bool | dict
         :raise c8.exceptions.DocumentReplaceError: If replace fails.
         :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
         """
         edge_id, headers = self._prep_from_body(edge, check_rev)
 
-        params = {'silent': silent}
+        params = {"silent": silent}
         if sync is not None:
-            params['waitForSync'] = sync
+            params["waitForSync"] = sync
 
-        command = 'gm._graph("{}").{}.replace("{}",{},{})'.format(
-            self.graph,
-            self.name,
-            edge_id,
-            dumps(edge),
-            dumps(params)
-        ) if self._is_transaction else None
+        command = (
+            'gm._graph("{}").{}.replace("{}",{},{})'.format(
+                self.graph, self.name, edge_id, dumps(edge), dumps(params)
+            )
+            if self._is_transaction
+            else None
+        )
 
         request = Request(
-            method='put',
-            endpoint='/_api/graph/{}/edge/{}'.format(
-                self._graph, edge_id
-            ),
+            method="put",
+            endpoint="/graph/{}/edge/{}".format(self._graph, edge_id),
             headers=headers,
             params=params,
             data=edge,
             command=command,
-            write=self.name
+            write=self.name,
         )
 
         def response_handler(resp):
             if resp.status_code == 412:
                 raise DocumentRevisionError(resp, request)
             if not resp.is_success:
                 raise DocumentReplaceError(resp, request)
             if silent is True:
                 return True
             if self._is_transaction:
                 result = resp.body
             else:
-                result = resp.body['edge']
-            result['_old_rev'] = result.pop('_oldRev')
+                result = resp.body["edge"]
+            result["_old_rev"] = result.pop("_oldRev")
             return result
 
         return self._execute(request, response_handler)
 
-    def delete(self,
-               edge,
-               rev=None,
-               check_rev=True,
-               ignore_missing=False,
-               sync=None):
+    def delete(self, edge, rev=None, check_rev=True, ignore_missing=False, sync=None):
         """Delete an edge document.
 
         :param edge: Edge document ID, key or body. Document body must contain
             the "_id" or "_key" field.
         :type edge: str | unicode | dict
         :param rev: Expected document revision. Overrides the value of "_rev"
             field in **edge** if present.
@@ -2747,40 +2290,39 @@
         :type check_rev: bool
         :param ignore_missing: Do not raise an exception on missing document.
             This parameter has no effect in transactions where an exception is
             always raised on failures.
         :type ignore_missing: bool
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool
-        :return: True if edge was deleted successfully, False if edge was not
+        :returns: True if edge was deleted successfully, False if edge was not
             found and **ignore_missing** was set to True (does not  apply in
             transactions).
         :rtype: bool
         :raise c8.exceptions.DocumentDeleteError: If delete fails.
         :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
         """
         handle, _, headers = self._prep_from_doc(edge, rev, check_rev)
 
-        params = {} if sync is None else {'waitForSync': sync}
-        command = 'gm._graph("{}").{}.remove("{}",{})'.format(
-            self.graph,
-            self.name,
-            handle,
-            dumps(params)
-        ) if self._is_transaction else None
+        params = {} if sync is None else {"waitForSync": sync}
+        command = (
+            'gm._graph("{}").{}.remove("{}",{})'.format(
+                self.graph, self.name, handle, dumps(params)
+            )
+            if self._is_transaction
+            else None
+        )
 
         request = Request(
-            method='delete',
-            endpoint='/_api/graph/{}/edge/{}'.format(
-                self._graph, handle
-            ),
+            method="delete",
+            endpoint="/graph/{}/edge/{}".format(self._graph, handle),
             params=params,
             headers=headers,
             command=command,
-            write=self.name
+            write=self.name,
         )
 
         def response_handler(resp):
             if resp.error_code == 1202 and ignore_missing:
                 return False
             if resp.status_code == 412:
                 raise DocumentRevisionError(resp, request)
@@ -2802,55 +2344,50 @@
             (otherwise it is auto-generated).
         :type data: dict
         :param sync: Block until operation is synchronized to disk.
         :type sync: bool
         :param silent: If set to True, no document metadata is returned. This
             can be used to save resources.
         :type silent: bool
-        :return: Document metadata (e.g. document key, revision) or True if
+        :returns: Document metadata (e.g. document key, revision) or True if
             parameter **silent** was set to True.
         :rtype: bool | dict
         :raise c8.exceptions.DocumentInsertError: If insert fails.
         """
-        edge = {
-            '_from': get_doc_id(from_vertex),
-            '_to': get_doc_id(to_vertex)
-        }
+        edge = {"_from": get_doc_id(from_vertex), "_to": get_doc_id(to_vertex)}
         if data is not None:
             edge.update(self._ensure_key_from_id(data))
         return self.insert(edge, sync=sync, silent=silent)
 
     def edges(self, vertex, direction=None):
         """Return the edge documents coming in and/or out of the vertex.
 
         :param vertex: Vertex document ID or body with "_id" field.
         :type vertex: str | unicode | dict
         :param direction: The direction of the edges. Allowed values are "in"
             and "out". If not set, edges in both directions are returned.
         :type direction: str | unicode
-        :return: List of edges
+        :returns: List of edges
         :rtype: dict
         :raise c8.exceptions.EdgeListError: If retrieval fails.
         """
-        params = {'vertex': get_doc_id(vertex)}
+        params = {"vertex": get_doc_id(vertex)}
         if direction is not None:
-            params['direction'] = direction
+            params["direction"] = direction
 
         request = Request(
-            method='get',
-            endpoint='/_api/edges/{}'.format(self.name),
-            params=params
+            method="get", endpoint="/edges/{}".format(self.name), params=params
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise EdgeListError(resp, request)
-            stats = resp.body['stats']
+            stats = resp.body["stats"]
             return {
-                'edges': resp.body['edges'],
-                'stats': {
-                    'filtered': stats['filtered'],
-                    'scanned_index': stats['scannedIndex'],
-                }
+                "edges": resp.body["edges"],
+                "stats": {
+                    "filtered": stats["filtered"],
+                    "scanned_index": stats["scannedIndex"],
+                },
             }
 
         return self._execute(request, response_handler)
```

### Comparing `pyC8-0.9.6/c8/response.py` & `pyC8-1.0.0/c8/response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import absolute_import, unicode_literals
 
-__all__ = ['Response']
-
 import json
 
+__all__ = ["Response"]
+
 
 class Response(object):
     """HTTP response.
 
     :param method: HTTP method in lowercase (e.g. "post").
     :type method: str | unicode
     :param url: API URL.
@@ -40,33 +40,27 @@
     :ivar error_message: Error message from C8Db server.
     :vartype error_message: str | unicode
     :ivar is_success: True if response status code was 2XX.
     :vartype is_success: bool
     """
 
     __slots__ = (
-        'method',
-        'url',
-        'headers',
-        'status_code',
-        'status_text',
-        'body',
-        'raw_body',
-        'error_code',
-        'error_message',
-        'is_success',
+        "method",
+        "url",
+        "headers",
+        "status_code",
+        "status_text",
+        "body",
+        "raw_body",
+        "error_code",
+        "error_message",
+        "is_success",
     )
 
-    def __init__(self,
-                 method,
-                 url,
-                 headers,
-                 status_code,
-                 status_text,
-                 raw_body):
+    def __init__(self, method, url, headers, status_code, status_text, raw_body):
         self.method = method.lower()
         self.url = url
         self.headers = headers
         self.status_code = status_code
         self.status_text = status_text
         self.raw_body = raw_body
 
@@ -74,15 +68,15 @@
         try:
             self.body = json.loads(raw_body)
         except (ValueError, TypeError):
             self.body = raw_body
 
         # Extract error code and message.
         if isinstance(self.body, dict):
-            self.error_code = self.body.get('errorNum')
-            self.error_message = self.body.get('errorMessage')
+            self.error_code = self.body.get("errorNum")
+            self.error_message = self.body.get("errorMessage")
         else:
             self.error_code = None
             self.error_message = None
 
         http_ok = 200 <= status_code < 300
         self.is_success = http_ok and self.error_code is None
```

### Comparing `pyC8-0.9.6/c8/cursor.py` & `pyC8-1.0.0/c8/cursor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import absolute_import, unicode_literals
 
-__all__ = ['Cursor']
-
 from collections import deque
 
 from c8.exceptions import (
-    CursorNextError,
     CursorCloseError,
+    CursorEmptyError,
+    CursorNextError,
     CursorStateError,
-    CursorEmptyError
 )
 from c8.request import Request
 
+__all__ = ["Cursor"]
+
 
 class Cursor(object):
     """Cursor API wrapper.
 
     Cursors fetch query results from C8Db server in batches. Cursor objects
     are *stateful* as they store the fetched items in-memory. They must not be
     shared across threads without proper locking mechanism.
@@ -29,27 +29,27 @@
     :param init_data: Cursor initialization data.
     :type init_data: dict | list
     :param cursor_type: Cursor type ("cursor" or "export").
     :type cursor_type: str | unicode
     """
 
     __slots__ = [
-        '_conn',
-        '_type',
-        '_id',
-        '_count',
-        '_cached',
-        '_profile',
-        '_warnings',
-        '_has_more',
-        '_batch',
-        '_count'
+        "_conn",
+        "_type",
+        "_id",
+        "_count",
+        "_cached",
+        "_profile",
+        "_warnings",
+        "_has_more",
+        "_batch",
+        "_count",
     ]
 
-    def __init__(self, connection, init_data, cursor_type='cursor'):
+    def __init__(self, connection, init_data, cursor_type="cursor"):
         self._conn = connection
         self._type = cursor_type
         self._batch = deque()
         self._id = None
         self._count = None
         self._cached = None
         self._profile = None
@@ -78,50 +78,50 @@
     def __len__(self):
         return self._count
 
     def __exit__(self, *_):
         self.close(ignore_missing=True)
 
     def __repr__(self):
-        return '<Cursor {}>'.format(self._id) if self._id else '<Cursor>'
+        return "<Cursor {}>".format(self._id) if self._id else "<Cursor>"
 
     def _update(self, data):
         """Update the cursor using data from C8Db server.
 
         :param data: Cursor data from C8Db server (e.g. results).
         :type data: dict
         """
         result = {}
 
-        if 'id' in data:
-            self._id = data['id']
-            result['id'] = data['id']
-        if 'count' in data:
-            self._count = data['count']
-            result['count'] = data['count']
-        if 'cached' in data:
-            self._cached = data['cached']
-            result['cached'] = data['cached']
-
-        self._has_more = data['hasMore']
-        result['has_more'] = data['hasMore']
-
-        self._batch.extend(data['result'])
-        result['batch'] = data['result']
-
-        if 'extra' in data:
-            extra = data['extra']
-
-            if 'profile' in extra:
-                self._profile = extra['profile']
-                result['profile'] = extra['profile']
-
-            if 'warnings' in extra:
-                self._warnings = extra['warnings']
-                result['warnings'] = extra['warnings']
+        if "id" in data:
+            self._id = data["id"]
+            result["id"] = data["id"]
+        if "count" in data:
+            self._count = data["count"]
+            result["count"] = data["count"]
+        if "cached" in data:
+            self._cached = data["cached"]
+            result["cached"] = data["cached"]
+
+        self._has_more = data["hasMore"]
+        result["has_more"] = data["hasMore"]
+
+        self._batch.extend(data["result"])
+        result["batch"] = data["result"]
+
+        if "extra" in data:
+            extra = data["extra"]
+
+            if "profile" in extra:
+                self._profile = extra["profile"]
+                result["profile"] = extra["profile"]
+
+            if "warnings" in extra:
+                self._warnings = extra["warnings"]
+                result["warnings"] = extra["warnings"]
 
         return result
 
     @property
     def id(self):
         """Return the cursor ID.
 
@@ -223,31 +223,28 @@
         batch from server.
 
         :return: Next item in current batch.
         :rtype: str | unicode | bool | int | list | dict
         :raise c8.exceptions.CursorEmptyError: If current batch is empty.
         """
         if len(self._batch) == 0:
-            raise CursorEmptyError('current batch is empty')
+            raise CursorEmptyError("current batch is empty")
         return self._batch.popleft()
 
     def fetch(self):
         """Fetch the next batch from server and update the cursor.
 
         :return: New batch details.
         :rtype: dict
         :raise c8.exceptions.CursorNextError: If batch retrieval fails.
         :raise c8.exceptions.CursorStateError: If cursor ID is not set.
         """
         if self._id is None:
-            raise CursorStateError('cursor ID not set')
-        request = Request(
-            method='put',
-            endpoint='/_api/{}/{}'.format(self._type, self._id)
-        )
+            raise CursorStateError("cursor ID not set")
+        request = Request(method="put", endpoint="/cursor/{}".format(self._id))
         resp = self._conn.send_request(request)
 
         if not resp.is_success:
             raise CursorNextError(resp, request)
         return self._update(resp.body)
 
     def close(self, ignore_missing=False):
@@ -261,17 +258,14 @@
             smaller than the batch size, or in transactions).
         :rtype: bool | None
         :raise c8.exceptions.CursorCloseError: If operation fails.
         :raise c8.exceptions.CursorStateError: If cursor ID is not set.
         """
         if self._id is None:
             return None
-        request = Request(
-            method='delete',
-            endpoint='/_api/{}/{}'.format(self._type, self._id)
-        )
+        request = Request(method="delete", endpoint="/cursor/{}".format(self._id))
         resp = self._conn.send_request(request)
         if resp.is_success:
             return True
         if resp.status_code == 404 and ignore_missing:
             return False
         raise CursorCloseError(resp, request)
```

### Comparing `pyC8-0.9.6/c8/graph.py` & `pyC8-1.0.0/c8/graph.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from __future__ import absolute_import, unicode_literals
 
-__all__ = ['Graph']
-
 from c8.api import APIWrapper
-from c8.collection import EdgeCollection
-from c8.collection import VertexCollection
+from c8.collection import EdgeCollection, VertexCollection
 from c8.exceptions import (
-    EdgeDefinitionListError,
     EdgeDefinitionCreateError,
     EdgeDefinitionDeleteError,
+    EdgeDefinitionListError,
     EdgeDefinitionReplaceError,
     GraphPropertiesError,
-    GraphTraverseError,
-    VertexCollectionListError,
     VertexCollectionCreateError,
     VertexCollectionDeleteError,
+    VertexCollectionListError,
 )
 from c8.request import Request
-from c8.utils import get_col_name, get_doc_id
+from c8.utils import get_col_name
+
+__all__ = ["Graph"]
 
 
 class Graph(APIWrapper):
     """Graph API wrapper.
 
     :param executor: API executor.
     :type executor: c8.executor.Executor
@@ -30,15 +28,15 @@
     """
 
     def __init__(self, connection, executor, name):
         super(Graph, self).__init__(connection, executor)
         self._name = name
 
     def __repr__(self):
-        return '<Graph {}>'.format(self._name)
+        return "<Graph {}>".format(self._name)
 
     def _get_col_by_vertex(self, vertex):
         """Return the vertex collection for the given vertex document.
 
         :param vertex: Vertex document ID or body with "_id" field.
         :type vertex: str | unicode | dict
         :return: Vertex collection API wrapper.
@@ -68,45 +66,42 @@
     def properties(self):
         """Return graph properties.
 
         :return: Graph properties.
         :rtype: dict
         :raise c8.exceptions.GraphPropertiesError: If retrieval fails.
         """
-        request = Request(
-            method='get',
-            endpoint='/_api/graph/{}'.format(self._name)
-        )
+        request = Request(method="get", endpoint="/graph/{}".format(self._name))
 
         def response_handler(resp):
             if not resp.is_success:
                 raise GraphPropertiesError(resp, request)
-            body = resp.body['graph']
+            body = resp.body["graph"]
             properties = {
-                'id': body['_id'],
-                'name': body['name'],
-                'revision': body['_rev'],
-                'orphan_collections': body['orphanCollections'],
-                'edge_definitions': [
+                "id": body["_id"],
+                "name": body["name"],
+                "revision": body["_rev"],
+                "orphan_collections": body["orphanCollections"],
+                "edge_definitions": [
                     {
-                        'edge_collection': edge_definition['collection'],
-                        'from_vertex_collections': edge_definition['from'],
-                        'to_vertex_collections': edge_definition['to'],
+                        "edge_collection": edge_definition["collection"],
+                        "from_vertex_collections": edge_definition["from"],
+                        "to_vertex_collections": edge_definition["to"],
                     }
-                    for edge_definition in body['edgeDefinitions']
-                ]
+                    for edge_definition in body["edgeDefinitions"]
+                ],
             }
-            if 'isSmart' in body:
-                properties['smart'] = body['isSmart']
-            if 'smartGraphAttribute' in body:
-                properties['smart_field'] = body['smartGraphAttribute']
-            if 'numberOfShards' in body:
-                properties['shard_count'] = body['numberOfShards']
-            if 'replicationFactor' in body:
-                properties['replication_factor'] = body['replicationFactor']
+            if "isSmart" in body:
+                properties["smart"] = body["isSmart"]
+            if "smartGraphAttribute" in body:
+                properties["smart_field"] = body["smartGraphAttribute"]
+            if "numberOfShards" in body:
+                properties["shard_count"] = body["numberOfShards"]
+            if "replicationFactor" in body:
+                properties["replication_factor"] = body["replicationFactor"]
             return properties
 
         return self._execute(request, response_handler)
 
     ################################
     # Vertex Collection Management #
     ################################
@@ -125,22 +120,22 @@
         """Return vertex collections in the graph that are not orphaned.
 
         :return: Names of vertex collections that are not orphaned.
         :rtype: [str | unicode]
         :raise c8.exceptions.VertexCollectionListError: If retrieval fails.
         """
         request = Request(
-            method='get',
-            endpoint='/_api/graph/{}/vertex'.format(self._name),
+            method="get",
+            endpoint="/graph/{}/vertex".format(self._name),
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise VertexCollectionListError(resp, request)
-            return sorted(set(resp.body['collections']))
+            return sorted(set(resp.body["collections"]))
 
         return self._execute(request, response_handler)
 
     def vertex_collection(self, name):
         """Return the vertex collection API wrapper.
 
         :param name: Vertex collection name.
@@ -156,17 +151,17 @@
         :param name: Vertex collection name.
         :type name: str | unicode
         :return: Vertex collection API wrapper.
         :rtype: c8.collection.VertexCollection
         :raise c8.exceptions.VertexCollectionCreateError: If create fails.
         """
         request = Request(
-            method='post',
-            endpoint='/_api/graph/{}/vertex'.format(self._name),
-            data={'collection': name}
+            method="post",
+            endpoint="/graph/{}/vertex".format(self._name),
+            data={"collection": name},
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise VertexCollectionCreateError(resp, request)
             return self.vertex_collection(name)
 
@@ -174,24 +169,24 @@
 
     def delete_vertex_collection(self, name, purge=False):
         """Remove a vertex collection from the graph.
 
         :param name: Vertex collection name.
         :type name: str | unicode
         :param purge: If set to True, the vertex collection is not just deleted
-            from the graph but also from the database completely.
+            from the graph but also from the fabric completely.
         :type purge: bool
         :return: True if vertex collection was deleted successfully.
         :rtype: bool
         :raise c8.exceptions.VertexCollectionDeleteError: If delete fails.
         """
         request = Request(
-            method='delete',
-            endpoint='/_api/graph/{}/vertex/{}'.format(self._name, name),
-            params={'dropCollection': purge}
+            method="delete",
+            endpoint="/graph/{}/vertex/{}".format(self._name, name),
+            params={"dropCollection": purge},
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise VertexCollectionDeleteError(resp, request)
             return True
 
@@ -206,15 +201,15 @@
 
         :param name: Edge collection name.
         :type name: str | unicode
         :return: True if edge definition exists, False otherwise.
         :rtype: bool
         """
         return any(
-            definition['edge_collection'] == name
+            definition["edge_collection"] == name
             for definition in self.edge_definitions()
         )
 
     def has_edge_collection(self, name):
         """Check if the graph has the given edge collection.
 
         :param name: Edge collection name.
@@ -238,22 +233,21 @@
         """Return the edge definitions of the graph.
 
         :return: Edge definitions of the graph.
         :rtype: [dict]
         :raise c8.exceptions.EdgeDefinitionListError: If retrieval fails.
         """
         try:
-            return self.properties()['edge_definitions']
+            return self.properties()["edge_definitions"]
         except GraphPropertiesError as err:
             raise EdgeDefinitionListError(err.response, err.request)
 
-    def create_edge_definition(self,
-                               edge_collection,
-                               from_vertex_collections,
-                               to_vertex_collections):
+    def create_edge_definition(
+        self, edge_collection, from_vertex_collections, to_vertex_collections
+    ):
         """Create a new edge definition.
 
         An edge definition consists of an edge collection, "from" vertex
         collection(s) and "to" vertex collection(s). Here is an example entry:
 
         .. code-block:: python
 
@@ -270,56 +264,53 @@
         :param to_vertex_collections: Names of "to" vertex collections.
         :type to_vertex_collections: [str | unicode]
         :return: Edge collection API wrapper.
         :rtype: c8.collection.EdgeCollection
         :raise c8.exceptions.EdgeDefinitionCreateError: If create fails.
         """
         request = Request(
-            method='post',
-            endpoint='/_api/graph/{}/edge'.format(self._name),
+            method="post",
+            endpoint="/graph/{}/edge".format(self._name),
             data={
-                'collection': edge_collection,
-                'from': from_vertex_collections,
-                'to': to_vertex_collections
-            }
+                "collection": edge_collection,
+                "from": from_vertex_collections,
+                "to": to_vertex_collections,
+            },
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise EdgeDefinitionCreateError(resp, request)
             return self.edge_collection(edge_collection)
 
         return self._execute(request, response_handler)
 
-    def replace_edge_definition(self,
-                                edge_collection,
-                                from_vertex_collections,
-                                to_vertex_collections):
+    def replace_edge_definition(
+        self, edge_collection, from_vertex_collections, to_vertex_collections
+    ):
         """Replace an edge definition.
 
         :param edge_collection: Edge collection name.
         :type edge_collection: str | unicode
         :param from_vertex_collections: Names of "from" vertex collections.
         :type from_vertex_collections: [str | unicode]
         :param to_vertex_collections: Names of "to" vertex collections.
         :type to_vertex_collections: [str | unicode]
         :return: True if edge definition was replaced successfully.
         :rtype: bool
         :raise c8.exceptions.EdgeDefinitionReplaceError: If replace fails.
         """
         request = Request(
-            method='put',
-            endpoint='/_api/graph/{}/edge/{}'.format(
-                self._name, edge_collection
-            ),
+            method="put",
+            endpoint="/graph/{}/edge/{}".format(self._name, edge_collection),
             data={
-                'collection': edge_collection,
-                'from': from_vertex_collections,
-                'to': to_vertex_collections
-            }
+                "collection": edge_collection,
+                "from": from_vertex_collections,
+                "to": to_vertex_collections,
+            },
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise EdgeDefinitionReplaceError(resp, request)
             return self.edge_collection(edge_collection)
 
@@ -328,154 +319,33 @@
     def delete_edge_definition(self, name, purge=False):
         """Delete an edge definition from the graph.
 
         :param name: Edge collection name.
         :type name: str | unicode
         :param purge: If set to True, the edge definition is not just removed
             from the graph but the edge collection is also deleted completely
-            from the database.
+            from the fabric.
         :type purge: bool
         :return: True if edge definition was deleted successfully.
         :rtype: bool
         :raise c8.exceptions.EdgeDefinitionDeleteError: If delete fails.
         """
         request = Request(
-            method='delete',
-            endpoint='/_api/graph/{}/edge/{}'.format(self._name, name),
-            params={'dropCollection': purge}
+            method="delete",
+            endpoint="/graph/{}/edge/{}".format(self._name, name),
+            params={"dropCollection": purge},
         )
 
         def response_handler(resp):
             if not resp.is_success:
                 raise EdgeDefinitionDeleteError(resp, request)
             return True
 
         return self._execute(request, response_handler)
 
-    ###################
-    # Graph Functions #
-    ###################
-
-    def traverse(self,
-                 start_vertex,
-                 direction='outbound',
-                 item_order='forward',
-                 strategy=None,
-                 order=None,
-                 edge_uniqueness=None,
-                 vertex_uniqueness=None,
-                 max_iter=None,
-                 min_depth=None,
-                 max_depth=None,
-                 init_func=None,
-                 sort_func=None,
-                 filter_func=None,
-                 visitor_func=None,
-                 expander_func=None):
-        """Traverse the graph and return the visited vertices and edges.
-
-        :param start_vertex: Start vertex document ID or body with "_id" field.
-        :type start_vertex: str | unicode | dict
-        :param direction: Traversal direction. Allowed values are "outbound"
-            (default), "inbound" and "any".
-        :type direction: str | unicode
-        :param item_order: Item iteration order. Allowed values are "forward"
-            (default) and "backward".
-        :type item_order: str | unicode
-        :param strategy: Traversal strategy. Allowed values are "depthfirst"
-            and "breadthfirst".
-        :type strategy: str | unicode
-        :param order: Traversal order. Allowed values are "preorder",
-            "postorder", and "preorder-expander".
-        :type order: str | unicode
-        :param vertex_uniqueness: Uniqueness for visited vertices. Allowed
-            values are "global", "path" or "none".
-        :type vertex_uniqueness: str | unicode
-        :param edge_uniqueness: Uniqueness for visited edges. Allowed values
-            are "global", "path" or "none".
-        :type edge_uniqueness: str | unicode
-        :param min_depth: Minimum depth of the nodes to visit.
-        :type min_depth: int
-        :param max_depth: Maximum depth of the nodes to visit.
-        :type max_depth: int
-        :param max_iter: If set, halt the traversal after the given number of
-            iterations. This parameter can be used to prevent endless loops in
-            cyclic graphs.
-        :type max_iter: int
-        :param init_func: Initialization function in Javascript with signature
-            ``(config, result) -> void``. This function is used to initialize
-            values in the result.
-        :type init_func: str | unicode
-        :param sort_func: Sorting function in Javascript with signature
-            ``(left, right) -> integer``, which returns ``-1`` if ``left <
-            right``, ``+1`` if ``left > right`` and ``0`` if ``left == right``.
-        :type sort_func: str | unicode
-        :param filter_func: Filter function in Javascript with signature
-            ``(config, vertex, path) -> mixed``, where ``mixed`` can have one
-            of the following values (or an array with multiple): "exclude" (do
-            not visit the vertex), "prune" (do not follow the edges of the
-            vertex), or "undefined" (visit the vertex and follow its edges).
-        :type filter_func: str | unicode
-        :param visitor_func: Visitor function in Javascript with signature
-            ``(config, result, vertex, path, connected) -> void``. The return
-            value is ignored, ``result`` is modified by reference, and
-            ``connected`` is populated only when parameter **order** is set to
-            "preorder-expander".
-        :type visitor_func: str | unicode
-        :param expander_func: Expander function in Javascript with signature
-            ``(config, vertex, path) -> mixed``. The function must return an
-            array of connections for ``vertex``. Each connection is an object
-            with attributes "edge" and "vertex".
-        :type expander_func: str | unicode
-        :return: Visited edges and vertices.
-        :rtype: dict
-        :raise c8.exceptions.GraphTraverseError: If traversal fails.
-        """
-        if strategy is not None:
-            if strategy.lower() == 'dfs':
-                strategy = 'depthfirst'
-            elif strategy.lower() == 'bfs':
-                strategy = 'breadthfirst'
-
-        uniqueness = {}
-        if vertex_uniqueness is not None:
-            uniqueness['vertices'] = vertex_uniqueness
-        if edge_uniqueness is not None:
-            uniqueness['edges'] = edge_uniqueness
-
-        data = {
-            'startVertex': get_doc_id(start_vertex),
-            'graphName': self._name,
-            'direction': direction,
-            'strategy': strategy,
-            'order': order,
-            'itemOrder': item_order,
-            'uniqueness': uniqueness or None,
-            'maxIterations': max_iter,
-            'minDepth': min_depth,
-            'maxDepth': max_depth,
-            'init': init_func,
-            'filter': filter_func,
-            'visitor': visitor_func,
-            'sort': sort_func,
-            'expander': expander_func
-        }
-        request = Request(
-            method='post',
-            endpoint='/_api/traversal',
-            data={k: v for k, v in data.items() if v is not None}
-        )
-
-        def response_handler(resp):
-            if not resp.is_success:
-                raise GraphTraverseError(resp, request)
-            return resp.body['result']['visited']
-
-        return self._execute(request, response_handler)
-
     #####################
     # Vertex Management #
     #####################
 
     def has_vertex(self, vertex, rev=None, check_rev=True):
         """Check if the given vertex document exists in the graph.
 
@@ -529,20 +399,17 @@
         :return: Document metadata (e.g. document key, revision) or True if
             parameter **silent** was set to True.
         :rtype: bool | dict
         :raise c8.exceptions.DocumentInsertError: If insert fails.
         """
         return self.vertex_collection(collection).insert(vertex, sync, silent)
 
-    def update_vertex(self,
-                      vertex,
-                      check_rev=True,
-                      keep_none=True,
-                      sync=None,
-                      silent=False):
+    def update_vertex(
+        self, vertex, check_rev=True, keep_none=True, sync=None, silent=False
+    ):
         """Update a vertex document.
 
         :param vertex: Partial or full vertex document with updated values. It
             must contain the "_id" field.
         :type vertex: dict
         :param check_rev: If set to True, revision of **vertex** (if given) is
             compared against the revision of target vertex document.
@@ -562,15 +429,15 @@
         :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
         """
         return self._get_col_by_vertex(vertex).update(
             vertex=vertex,
             check_rev=check_rev,
             keep_none=keep_none,
             sync=sync,
-            silent=silent
+            silent=silent,
         )
 
     def replace_vertex(self, vertex, check_rev=True, sync=None, silent=False):
         """Replace a vertex document.
 
         :param vertex: New vertex document to replace the old one with. It must
             contain the "_id" field.
@@ -586,26 +453,20 @@
         :return: Document metadata (e.g. document key, revision) or True if
             parameter **silent** was set to True.
         :rtype: bool | dict
         :raise c8.exceptions.DocumentReplaceError: If replace fails.
         :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
         """
         return self._get_col_by_vertex(vertex).replace(
-            vertex=vertex,
-            check_rev=check_rev,
-            sync=sync,
-            silent=silent
+            vertex=vertex, check_rev=check_rev, sync=sync, silent=silent
         )
 
-    def delete_vertex(self,
-                      vertex,
-                      rev=None,
-                      check_rev=True,
-                      ignore_missing=False,
-                      sync=None):
+    def delete_vertex(
+        self, vertex, rev=None, check_rev=True, ignore_missing=False, sync=None
+    ):
         """Delete a vertex document.
 
         :param vertex: Vertex document ID or body with "_id" field.
         :type vertex: str | unicode | dict
         :param rev: Expected document revision. Overrides the value of "_rev"
             field in **vertex** if present.
         :type rev: str | unicode
@@ -626,15 +487,15 @@
         :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
         """
         return self._get_col_by_vertex(vertex).delete(
             vertex=vertex,
             rev=rev,
             check_rev=check_rev,
             ignore_missing=ignore_missing,
-            sync=sync
+            sync=sync,
         )
 
     ###################
     # Edge Management #
     ###################
 
     def has_edge(self, edge, rev=None, check_rev=True):
@@ -691,20 +552,17 @@
         :return: Document metadata (e.g. document key, revision) or True if
             parameter **silent** was set to True.
         :rtype: bool | dict
         :raise c8.exceptions.DocumentInsertError: If insert fails.
         """
         return self.edge_collection(collection).insert(edge, sync, silent)
 
-    def update_edge(self,
-                    edge,
-                    check_rev=True,
-                    keep_none=True,
-                    sync=None,
-                    silent=False):
+    def update_edge(
+        self, edge, check_rev=True, keep_none=True, sync=None, silent=False
+    ):
         """Update an edge document.
 
         :param edge: Partial or full edge document with updated values. It must
             contain the "_id" field.
         :type edge: dict
         :param check_rev: If set to True, revision of **edge** (if given) is
             compared against the revision of target edge document.
@@ -724,15 +582,15 @@
         :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
         """
         return self._get_col_by_edge(edge).update(
             edge=edge,
             check_rev=check_rev,
             keep_none=keep_none,
             sync=sync,
-            silent=silent
+            silent=silent,
         )
 
     def replace_edge(self, edge, check_rev=True, sync=None, silent=False):
         """Replace an edge document.
 
         :param edge: New edge document to replace the old one with. It must
             contain the "_id" field. It must also contain the "_from" and "_to"
@@ -749,26 +607,20 @@
         :return: Document metadata (e.g. document key, revision) or True if
             parameter **silent** was set to True.
         :rtype: bool | dict
         :raise c8.exceptions.DocumentReplaceError: If replace fails.
         :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
         """
         return self._get_col_by_edge(edge).replace(
-            edge=edge,
-            check_rev=check_rev,
-            sync=sync,
-            silent=silent
+            edge=edge, check_rev=check_rev, sync=sync, silent=silent
         )
 
-    def delete_edge(self,
-                    edge,
-                    rev=None,
-                    check_rev=True,
-                    ignore_missing=False,
-                    sync=None):
+    def delete_edge(
+        self, edge, rev=None, check_rev=True, ignore_missing=False, sync=None
+    ):
         """Delete an edge document.
 
         :param edge: Edge document ID or body with "_id" field.
         :type edge: str | unicode | dict
         :param rev: Expected document revision. Overrides the value of "_rev"
             field in **edge** if present.
         :type rev: str | unicode
@@ -789,24 +641,20 @@
         :raise c8.exceptions.DocumentRevisionError: If revisions mismatch.
         """
         return self._get_col_by_edge(edge).delete(
             edge=edge,
             rev=rev,
             check_rev=check_rev,
             ignore_missing=ignore_missing,
-            sync=sync
+            sync=sync,
         )
 
-    def link(self,
-             collection,
-             from_vertex,
-             to_vertex,
-             data=None,
-             sync=None,
-             silent=False):
+    def link(
+        self, collection, from_vertex, to_vertex, data=None, sync=None, silent=False
+    ):
         """Insert a new edge document linking the given vertices.
 
         :param collection: Edge collection name.
         :type collection: str | unicode
         :param from_vertex: "From" vertex document ID or body with "_id" field.
         :type from_vertex: str | unicode | dict
         :param to_vertex: "To" vertex document ID or body with "_id" field.
@@ -826,15 +674,15 @@
         :raise c8.exceptions.DocumentInsertError: If insert fails.
         """
         return self.edge_collection(collection).link(
             from_vertex=from_vertex,
             to_vertex=to_vertex,
             data=data,
             sync=sync,
-            silent=silent
+            silent=silent,
         )
 
     def edges(self, collection, vertex, direction=None):
         """Return the edge documents coming in and/or out of given vertex.
 
         :param collection: Edge collection name.
         :type collection: str | unicode
```

### Comparing `pyC8-0.9.6/LICENSE` & `pyC8-1.0.0/LICENSE`

 * *Files identical despite different names*

