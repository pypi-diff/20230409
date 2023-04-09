# Comparing `tmp/ossapi-3.1.8.tar.gz` & `tmp/ossapi-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ossapi-3.1.8.tar", last modified: Fri Apr  7 18:52:38 2023, max compression
+gzip compressed data, was "ossapi-3.1.9.tar", last modified: Sun Apr  9 00:25:59 2023, max compression
```

## Comparing `ossapi-3.1.8.tar` & `ossapi-3.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-04-07 18:52:38.609646 ossapi-3.1.8/
--rw-r--r--   0 tybug      (501) staff       (20)    34523 2023-01-30 05:20:33.000000 ossapi-3.1.8/LICENSE
--rw-r--r--   0 tybug      (501) staff       (20)    10020 2023-04-07 18:52:38.609433 ossapi-3.1.8/PKG-INFO
--rw-r--r--   0 tybug      (501) staff       (20)     9513 2023-03-28 20:31:37.000000 ossapi-3.1.8/README.md
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-04-07 18:52:38.607068 ossapi-3.1.8/ossapi/
--rw-r--r--   0 tybug      (501) staff       (20)     3864 2023-03-09 02:19:38.000000 ossapi-3.1.8/ossapi/__init__.py
--rw-r--r--   0 tybug      (501) staff       (20)      925 2023-03-31 23:04:14.000000 ossapi-3.1.8/ossapi/encoder.py
--rw-r--r--   0 tybug      (501) staff       (20)    16948 2023-04-06 05:02:02.000000 ossapi-3.1.8/ossapi/enums.py
--rw-r--r--   0 tybug      (501) staff       (20)    11982 2023-01-31 22:30:17.000000 ossapi-3.1.8/ossapi/mod.py
--rw-r--r--   0 tybug      (501) staff       (20)    36025 2023-03-09 05:37:37.000000 ossapi-3.1.8/ossapi/models.py
--rw-r--r--   0 tybug      (501) staff       (20)    14955 2023-02-01 05:09:38.000000 ossapi-3.1.8/ossapi/ossapi.py
--rw-r--r--   0 tybug      (501) staff       (20)    84208 2023-04-07 18:52:33.000000 ossapi-3.1.8/ossapi/ossapiv2.py
--rw-r--r--   0 tybug      (501) staff       (20)    89252 2023-04-07 18:52:33.000000 ossapi-3.1.8/ossapi/ossapiv2_async.py
--rw-r--r--   0 tybug      (501) staff       (20)     2639 2023-03-08 17:51:25.000000 ossapi-3.1.8/ossapi/replay.py
--rw-r--r--   0 tybug      (501) staff       (20)     8707 2023-01-30 00:39:41.000000 ossapi-3.1.8/ossapi/utils.py
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-04-07 18:52:38.607949 ossapi-3.1.8/ossapi.egg-info/
--rw-r--r--   0 tybug      (501) staff       (20)    10020 2023-04-07 18:52:38.000000 ossapi-3.1.8/ossapi.egg-info/PKG-INFO
--rw-r--r--   0 tybug      (501) staff       (20)      460 2023-04-07 18:52:38.000000 ossapi-3.1.8/ossapi.egg-info/SOURCES.txt
--rw-r--r--   0 tybug      (501) staff       (20)        1 2023-04-07 18:52:38.000000 ossapi-3.1.8/ossapi.egg-info/dependency_links.txt
--rw-r--r--   0 tybug      (501) staff       (20)       71 2023-04-07 18:52:38.000000 ossapi-3.1.8/ossapi.egg-info/requires.txt
--rw-r--r--   0 tybug      (501) staff       (20)        7 2023-04-07 18:52:38.000000 ossapi-3.1.8/ossapi.egg-info/top_level.txt
--rw-r--r--   0 tybug      (501) staff       (20)      644 2023-04-07 18:52:11.000000 ossapi-3.1.8/pyproject.toml
--rw-r--r--   0 tybug      (501) staff       (20)       38 2023-04-07 18:52:38.609695 ossapi-3.1.8/setup.cfg
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-04-07 18:52:38.609130 ossapi-3.1.8/tests/
--rw-r--r--   0 tybug      (501) staff       (20)     3082 2023-04-07 18:52:33.000000 ossapi-3.1.8/tests/__init__.py
--rw-r--r--   0 tybug      (501) staff       (20)      523 2023-01-28 21:17:50.000000 ossapi-3.1.8/tests/test_cursor.py
--rw-r--r--   0 tybug      (501) staff       (20)     9694 2023-03-09 05:36:41.000000 ossapi-3.1.8/tests/test_endpoints.py
--rw-r--r--   0 tybug      (501) staff       (20)     4040 2023-04-07 18:52:33.000000 ossapi-3.1.8/tests/test_models.py
--rw-r--r--   0 tybug      (501) staff       (20)     1137 2023-01-28 21:17:50.000000 ossapi-3.1.8/tests/test_v1.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-04-09 00:25:59.765352 ossapi-3.1.9/
+-rw-r--r--   0 tybug      (501) staff       (20)    34523 2023-01-30 05:20:33.000000 ossapi-3.1.9/LICENSE
+-rw-r--r--   0 tybug      (501) staff       (20)    10020 2023-04-09 00:25:59.765113 ossapi-3.1.9/PKG-INFO
+-rw-r--r--   0 tybug      (501) staff       (20)     9513 2023-03-28 20:31:37.000000 ossapi-3.1.9/README.md
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-04-09 00:25:59.761620 ossapi-3.1.9/ossapi/
+-rw-r--r--   0 tybug      (501) staff       (20)     3864 2023-03-09 02:19:38.000000 ossapi-3.1.9/ossapi/__init__.py
+-rw-r--r--   0 tybug      (501) staff       (20)      925 2023-03-31 23:04:14.000000 ossapi-3.1.9/ossapi/encoder.py
+-rw-r--r--   0 tybug      (501) staff       (20)    16948 2023-04-06 05:02:02.000000 ossapi-3.1.9/ossapi/enums.py
+-rw-r--r--   0 tybug      (501) staff       (20)    11982 2023-01-31 22:30:17.000000 ossapi-3.1.9/ossapi/mod.py
+-rw-r--r--   0 tybug      (501) staff       (20)    36025 2023-03-09 05:37:37.000000 ossapi-3.1.9/ossapi/models.py
+-rw-r--r--   0 tybug      (501) staff       (20)    14955 2023-02-01 05:09:38.000000 ossapi-3.1.9/ossapi/ossapi.py
+-rw-r--r--   0 tybug      (501) staff       (20)    84207 2023-04-09 00:25:54.000000 ossapi-3.1.9/ossapi/ossapiv2.py
+-rw-r--r--   0 tybug      (501) staff       (20)    89585 2023-04-09 00:25:54.000000 ossapi-3.1.9/ossapi/ossapiv2_async.py
+-rw-r--r--   0 tybug      (501) staff       (20)     2639 2023-03-08 17:51:25.000000 ossapi-3.1.9/ossapi/replay.py
+-rw-r--r--   0 tybug      (501) staff       (20)     8707 2023-01-30 00:39:41.000000 ossapi-3.1.9/ossapi/utils.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-04-09 00:25:59.762825 ossapi-3.1.9/ossapi.egg-info/
+-rw-r--r--   0 tybug      (501) staff       (20)    10020 2023-04-09 00:25:59.000000 ossapi-3.1.9/ossapi.egg-info/PKG-INFO
+-rw-r--r--   0 tybug      (501) staff       (20)      460 2023-04-09 00:25:59.000000 ossapi-3.1.9/ossapi.egg-info/SOURCES.txt
+-rw-r--r--   0 tybug      (501) staff       (20)        1 2023-04-09 00:25:59.000000 ossapi-3.1.9/ossapi.egg-info/dependency_links.txt
+-rw-r--r--   0 tybug      (501) staff       (20)       71 2023-04-09 00:25:59.000000 ossapi-3.1.9/ossapi.egg-info/requires.txt
+-rw-r--r--   0 tybug      (501) staff       (20)        7 2023-04-09 00:25:59.000000 ossapi-3.1.9/ossapi.egg-info/top_level.txt
+-rw-r--r--   0 tybug      (501) staff       (20)      644 2023-04-09 00:25:40.000000 ossapi-3.1.9/pyproject.toml
+-rw-r--r--   0 tybug      (501) staff       (20)       38 2023-04-09 00:25:59.765426 ossapi-3.1.9/setup.cfg
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2023-04-09 00:25:59.764727 ossapi-3.1.9/tests/
+-rw-r--r--   0 tybug      (501) staff       (20)     3082 2023-04-09 00:25:54.000000 ossapi-3.1.9/tests/__init__.py
+-rw-r--r--   0 tybug      (501) staff       (20)      523 2023-01-28 21:17:50.000000 ossapi-3.1.9/tests/test_cursor.py
+-rw-r--r--   0 tybug      (501) staff       (20)     9694 2023-03-09 05:36:41.000000 ossapi-3.1.9/tests/test_endpoints.py
+-rw-r--r--   0 tybug      (501) staff       (20)     4040 2023-04-09 00:25:54.000000 ossapi-3.1.9/tests/test_models.py
+-rw-r--r--   0 tybug      (501) staff       (20)     1137 2023-01-28 21:17:50.000000 ossapi-3.1.9/tests/test_v1.py
```

### Comparing `ossapi-3.1.8/LICENSE` & `ossapi-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.8/PKG-INFO` & `ossapi-3.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ossapi
-Version: 3.1.8
+Version: 3.1.9
 Summary: Complete python wrapper for osu! api v2 and v1.
 Author-email: Liam DeVoe <orionldevoe@gmail.com>
 Project-URL: Homepage, https://github.com/circleguard/ossapi
 Keywords: osu!,wrapper,api,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `ossapi-3.1.8/README.md` & `ossapi-3.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.8/ossapi/__init__.py` & `ossapi-3.1.9/ossapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.8/ossapi/encoder.py` & `ossapi-3.1.9/ossapi/encoder.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.8/ossapi/enums.py` & `ossapi-3.1.9/ossapi/enums.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.8/ossapi/mod.py` & `ossapi-3.1.9/ossapi/mod.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.8/ossapi/models.py` & `ossapi-3.1.9/ossapi/models.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.8/ossapi/ossapi.py` & `ossapi-3.1.9/ossapi/ossapi.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.8/ossapi/ossapiv2.py` & `ossapi-3.1.9/ossapi/ossapiv2.py`

 * *Files 0% similar despite different names*

```diff
@@ -946,15 +946,15 @@
             The md5 hash of the beatmap.
         filename
             The filename of the beatmap.
 
         Notes
         -----
         Combines the
-        `Get Beatmap <https://osu.ppy.sh/docs/index.html#get-beatmapL>`_ and
+        `Get Beatmap <https://osu.ppy.sh/docs/index.html#get-beatmap>`_ and
         `Lookup Beatmap <https://osu.ppy.sh/docs/index.html#lookup-beatmap>`_
         endpoints.
         """
         if not (beatmap_id or checksum or filename):
             raise ValueError("at least one of beatmap_id, checksum, or "
                 "filename must be passed")
         params = {"checksum": checksum, "filename": filename, "id": beatmap_id}
```

### Comparing `ossapi-3.1.8/ossapi/ossapiv2_async.py` & `ossapi-3.1.9/ossapi/ossapiv2_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -1041,15 +1041,15 @@
             The md5 hash of the beatmap.
         filename
             The filename of the beatmap.
 
         Notes
         -----
         Combines the
-        `Get Beatmap <https://osu.ppy.sh/docs/index.html#get-beatmapL>`_ and
+        `Get Beatmap <https://osu.ppy.sh/docs/index.html#get-beatmap>`_ and
         `Lookup Beatmap <https://osu.ppy.sh/docs/index.html#lookup-beatmap>`_
         endpoints.
         """
         if not (beatmap_id or checksum or filename):
             raise ValueError("at least one of beatmap_id, checksum, or "
                 "filename must be passed")
         params = {"checksum": checksum, "filename": filename, "id": beatmap_id}
@@ -2176,32 +2176,42 @@
 
         Notes
         -----
         Implements the `Download Score
         <https://osu.ppy.sh/docs/index.html#scoresmodescoredownload>`__
         endpoint.
         """
+        from aiohttp import ClientSession, ContentTypeError
+
         url = f"{self.BASE_URL}/scores/{mode.value}/{score_id}/download"
-        r = await self.session.request_async("GET", url)
+
+        aiohttp_session = ClientSession()
+        r = await self.session.request_async("GET", url,
+            session=aiohttp_session)
 
         # if the response above succeeded, it will return a raw string
         # instead of json. If it didn't succeed, it will return json with an
         # error.
-        # So always try parsing as json to check if there's an error. If parsin
+        # So always try parsing as json to check if there's an error. If parsing
         # fails, just assume the request succeeded and move on.
+        # TODO we probably want to be checking headers here instead.
+        # Should be x-osu-replay for valid response.
         try:
-            json_ = r.json()
+            json_ = await r.json()
             self._check_response(json_, url)
-        except json.JSONDecodeError:
+        except ContentTypeError:
             pass
 
+        content = await r.read()
+        await aiohttp_session.close()
+
         if raw:
-            return r.content
+            return content
 
-        replay = osrparse.Replay.from_string(r.content)
+        replay = osrparse.Replay.from_string(content)
         return Replay(replay, self)
 
 
     # seasonal backgrounds
     # --------------------
 
     @request(scope=None, category="seasonal backgrounds")
```

### Comparing `ossapi-3.1.8/ossapi/replay.py` & `ossapi-3.1.9/ossapi/replay.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.8/ossapi/utils.py` & `ossapi-3.1.9/ossapi/utils.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.8/ossapi.egg-info/PKG-INFO` & `ossapi-3.1.9/ossapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ossapi
-Version: 3.1.8
+Version: 3.1.9
 Summary: Complete python wrapper for osu! api v2 and v1.
 Author-email: Liam DeVoe <orionldevoe@gmail.com>
 Project-URL: Homepage, https://github.com/circleguard/ossapi
 Keywords: osu!,wrapper,api,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `ossapi-3.1.8/pyproject.toml` & `ossapi-3.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ossapi"
-version = "3.1.8"
+version = "3.1.9"
 description = "Complete python wrapper for osu! api v2 and v1."
 readme = "README.md"
 keywords = ["osu!", "wrapper", "api", "python"]
 authors = [
   {name = "Liam DeVoe", email = "orionldevoe@gmail.com" }
 ]
 classifiers = [
```

### Comparing `ossapi-3.1.8/tests/__init__.py` & `ossapi-3.1.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.8/tests/test_cursor.py` & `ossapi-3.1.9/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.8/tests/test_endpoints.py` & `ossapi-3.1.9/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.8/tests/test_models.py` & `ossapi-3.1.9/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ossapi-3.1.8/tests/test_v1.py` & `ossapi-3.1.9/tests/test_v1.py`

 * *Files identical despite different names*

