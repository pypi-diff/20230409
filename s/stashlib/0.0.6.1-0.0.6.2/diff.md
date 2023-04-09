# Comparing `tmp/stashlib-0.0.6.1.tar.gz` & `tmp/stashlib-0.0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stashlib-0.0.6.1.tar", last modified: Wed Apr  5 03:33:38 2023, max compression
+gzip compressed data, was "stashlib-0.0.6.2.tar", last modified: Sun Apr  9 09:29:13 2023, max compression
```

## Comparing `stashlib-0.0.6.1.tar` & `stashlib-0.0.6.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 03:33:38.841868 stashlib-0.0.6.1/
--rw-rw-rw-   0        0        0     1104 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/LICENSE
--rw-rw-rw-   0        0        0      988 2023-04-05 03:33:38.841868 stashlib-0.0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/README.md
--rw-rw-rw-   0        0        0     1135 2023-04-05 03:33:38.842885 stashlib-0.0.6.1/setup.cfg
--rw-rw-rw-   0        0        0       85 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-05 03:33:38.770111 stashlib-0.0.6.1/stash/
--rw-rw-rw-   0        0        0     2728 2023-04-05 03:01:37.000000 stashlib-0.0.6.1/stash/__init__.py
--rw-rw-rw-   0        0        0     5467 2023-04-05 03:32:01.000000 stashlib-0.0.6.1/stash/_helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-05 03:33:38.793859 stashlib-0.0.6.1/stash/codecs/
--rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/codecs/__init__.py
--rw-rw-rw-   0        0        0      265 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/codecs/brotli.py
--rw-rw-rw-   0        0        0      255 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/codecs/bzip2.py
--rw-rw-rw-   0        0        0      197 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/codecs/codec.py
--rw-rw-rw-   0        0        0      257 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/codecs/gzip.py
--rw-rw-rw-   0        0        0      271 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/codecs/lz4.py
--rw-rw-rw-   0        0        0      253 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/codecs/lzf.py
--rw-rw-rw-   0        0        0      335 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/codecs/lzma.py
--rw-rw-rw-   0        0        0      253 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/codecs/lzo.py
--rw-rw-rw-   0        0        0      173 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/codecs/passthru.py
--rw-rw-rw-   0        0        0      265 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/codecs/snappy.py
--rw-rw-rw-   0        0        0      214 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/codecs/zlib.py
--rw-rw-rw-   0        0        0      303 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/codecs/zopfli.py
--rw-rw-rw-   0        0        0      274 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/codecs/zstd.py
--rw-rw-rw-   0        0        0      395 2023-04-05 03:32:56.000000 stashlib-0.0.6.1/stash/consts.py
--rw-rw-rw-   0        0        0      383 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/defaults.py
--rw-rw-rw-   0        0        0     1781 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/manager.py
--rw-rw-rw-   0        0        0     1395 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/options.py
-drwxrwxrwx   0        0        0        0 2023-04-05 03:33:38.810744 stashlib-0.0.6.1/stash/serializers/
--rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/serializers/__init__.py
--rw-rw-rw-   0        0        0      294 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/serializers/bson.py
--rw-rw-rw-   0        0        0      291 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/serializers/cbor.py
--rw-rw-rw-   0        0        0      248 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/serializers/default.py
--rw-rw-rw-   0        0        0      290 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/serializers/json.py
--rw-rw-rw-   0        0        0      296 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/serializers/msgpack.py
--rw-rw-rw-   0        0        0      294 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/serializers/orjson.py
--rw-rw-rw-   0        0        0      300 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/serializers/rapidjson.py
--rw-rw-rw-   0        0        0      203 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/serializers/serializer.py
--rw-rw-rw-   0        0        0      302 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/serializers/simplejson.py
--rw-rw-rw-   0        0        0      296 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/serializers/ujson.py
-drwxrwxrwx   0        0        0        0 2023-04-05 03:33:38.828724 stashlib-0.0.6.1/stash/storages/
--rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/storages/__init__.py
--rw-rw-rw-   0        0        0     1144 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/storages/dbm_.py
--rw-rw-rw-   0        0        0     3657 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/storages/filesystem.py
--rw-rw-rw-   0        0        0      411 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/storages/leveldb.py
--rw-rw-rw-   0        0        0     1758 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/storages/lmdb.py
--rw-rw-rw-   0        0        0     1243 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/storages/lsmdb.py
--rw-rw-rw-   0        0        0      672 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/storages/memory.py
--rw-rw-rw-   0        0        0     1347 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/storages/mongodb.py
--rw-rw-rw-   0        0        0      416 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/storages/null.py
--rw-rw-rw-   0        0        0     1252 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/storages/redis.py
--rw-rw-rw-   0        0        0      672 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/storages/storage.py
-drwxrwxrwx   0        0        0        0 2023-04-05 03:33:38.832724 stashlib-0.0.6.1/stash/utils/
--rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/utils/__init__.py
--rw-rw-rw-   0        0        0     1489 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/utils/checksum.py
--rw-rw-rw-   0        0        0     1993 2023-04-05 02:46:31.000000 stashlib-0.0.6.1/stash/utils/nested_path.py
-drwxrwxrwx   0        0        0        0 2023-04-05 03:33:38.840721 stashlib-0.0.6.1/stashlib.egg-info/
--rw-rw-rw-   0        0        0      988 2023-04-05 03:33:38.000000 stashlib-0.0.6.1/stashlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1242 2023-04-05 03:33:38.000000 stashlib-0.0.6.1/stashlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 03:33:38.000000 stashlib-0.0.6.1/stashlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-05 03:33:38.000000 stashlib-0.0.6.1/stashlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-09 09:29:13.469732 stashlib-0.0.6.2/
+-rw-rw-rw-   0        0        0     1104 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/LICENSE
+-rw-rw-rw-   0        0        0      988 2023-04-09 09:29:13.470732 stashlib-0.0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/README.md
+-rw-rw-rw-   0        0        0     1135 2023-04-09 09:29:13.471731 stashlib-0.0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0       85 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-09 09:29:13.395624 stashlib-0.0.6.2/stash/
+-rw-rw-rw-   0        0        0     2728 2023-04-05 03:01:37.000000 stashlib-0.0.6.2/stash/__init__.py
+-rw-rw-rw-   0        0        0     6422 2023-04-09 09:26:26.000000 stashlib-0.0.6.2/stash/_helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-09 09:29:13.420745 stashlib-0.0.6.2/stash/codecs/
+-rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/__init__.py
+-rw-rw-rw-   0        0        0      265 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/brotli.py
+-rw-rw-rw-   0        0        0      255 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/bzip2.py
+-rw-rw-rw-   0        0        0      197 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/codec.py
+-rw-rw-rw-   0        0        0      257 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/gzip.py
+-rw-rw-rw-   0        0        0      271 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/lz4.py
+-rw-rw-rw-   0        0        0      253 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/lzf.py
+-rw-rw-rw-   0        0        0      335 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/lzma.py
+-rw-rw-rw-   0        0        0      253 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/lzo.py
+-rw-rw-rw-   0        0        0      173 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/passthru.py
+-rw-rw-rw-   0        0        0      265 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/snappy.py
+-rw-rw-rw-   0        0        0      214 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/zlib.py
+-rw-rw-rw-   0        0        0      303 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/zopfli.py
+-rw-rw-rw-   0        0        0      274 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/codecs/zstd.py
+-rw-rw-rw-   0        0        0      395 2023-04-09 09:27:23.000000 stashlib-0.0.6.2/stash/consts.py
+-rw-rw-rw-   0        0        0      383 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/defaults.py
+-rw-rw-rw-   0        0        0     1781 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/manager.py
+-rw-rw-rw-   0        0        0     1395 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/options.py
+drwxrwxrwx   0        0        0        0 2023-04-09 09:29:13.439762 stashlib-0.0.6.2/stash/serializers/
+-rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/__init__.py
+-rw-rw-rw-   0        0        0      294 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/bson.py
+-rw-rw-rw-   0        0        0      291 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/cbor.py
+-rw-rw-rw-   0        0        0      248 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/default.py
+-rw-rw-rw-   0        0        0      290 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/json.py
+-rw-rw-rw-   0        0        0      296 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/msgpack.py
+-rw-rw-rw-   0        0        0      294 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/orjson.py
+-rw-rw-rw-   0        0        0      300 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/rapidjson.py
+-rw-rw-rw-   0        0        0      203 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/serializer.py
+-rw-rw-rw-   0        0        0      302 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/simplejson.py
+-rw-rw-rw-   0        0        0      296 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/serializers/ujson.py
+drwxrwxrwx   0        0        0        0 2023-04-09 09:29:13.456751 stashlib-0.0.6.2/stash/storages/
+-rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/__init__.py
+-rw-rw-rw-   0        0        0     1144 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/dbm_.py
+-rw-rw-rw-   0        0        0     3657 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/filesystem.py
+-rw-rw-rw-   0        0        0      411 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/leveldb.py
+-rw-rw-rw-   0        0        0     1758 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/lmdb.py
+-rw-rw-rw-   0        0        0     1243 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/lsmdb.py
+-rw-rw-rw-   0        0        0      672 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/memory.py
+-rw-rw-rw-   0        0        0     1347 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/mongodb.py
+-rw-rw-rw-   0        0        0      416 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/null.py
+-rw-rw-rw-   0        0        0     1252 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/redis.py
+-rw-rw-rw-   0        0        0      672 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/storages/storage.py
+drwxrwxrwx   0        0        0        0 2023-04-09 09:29:13.461735 stashlib-0.0.6.2/stash/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/utils/__init__.py
+-rw-rw-rw-   0        0        0     1489 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/utils/checksum.py
+-rw-rw-rw-   0        0        0     1993 2023-04-05 02:46:31.000000 stashlib-0.0.6.2/stash/utils/nested_path.py
+drwxrwxrwx   0        0        0        0 2023-04-09 09:29:13.467733 stashlib-0.0.6.2/stashlib.egg-info/
+-rw-rw-rw-   0        0        0      988 2023-04-09 09:29:13.000000 stashlib-0.0.6.2/stashlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1242 2023-04-09 09:29:13.000000 stashlib-0.0.6.2/stashlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-09 09:29:13.000000 stashlib-0.0.6.2/stashlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-09 09:29:13.000000 stashlib-0.0.6.2/stashlib.egg-info/top_level.txt
```

### Comparing `stashlib-0.0.6.1/LICENSE` & `stashlib-0.0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.1/PKG-INFO` & `stashlib-0.0.6.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashlib
-Version: 0.0.6.1
+Version: 0.0.6.2
 Summary: stash is an extensible and lightweight cache library for python
 Home-page: https://github.com/masroore/stash.py
 Author: Masroor Ehsan
 Author-email: masroore@gmail.com
 License: MIT
 Keywords: cache caching
 Platform: any
```

### Comparing `stashlib-0.0.6.1/setup.cfg` & `stashlib-0.0.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.1/stash/__init__.py` & `stashlib-0.0.6.2/stash/__init__.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.1/stash/_helpers.py` & `stashlib-0.0.6.2/stash/_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,20 @@
 
 def get_fs_zstd_stash(options: StashOptions) -> StashManager:
     from .codecs.zstd import ZstdCodec
 
     return _init_fs_cache(ZstdCodec(), options=options)
 
 
+def get_fs_lzma_stash(options: StashOptions) -> StashManager:
+    from .codecs.lzma import LzmaCodec
+
+    return _init_fs_cache(LzmaCodec(), options=options)
+
+
 def get_mongo_zlib_stash(options: StashOptions) -> StashManager:
     from .codecs.zlib import ZlibCodec
     from .storages.mongodb import MongoDbStorage
 
     storage = MongoDbStorage(options=options)
     return _init_cache(storage, ZlibCodec(), options=options)
 
@@ -47,23 +53,31 @@
     from .codecs.brotli import BrotliCodec
     from .storages.lmdb import LmdbStorage
 
     storage = LmdbStorage(options=options)
     return _init_cache(storage, BrotliCodec(), options=options)
 
 
+def get_lmdb_lzma_stash(options: StashOptions) -> StashManager:
+    from .codecs.lzma import LzmaCodec
+    from .storages.lmdb import LmdbStorage
+
+    storage = LmdbStorage(options=options)
+    return _init_cache(storage, LzmaCodec(), options=options)
+
+
 def get_lmdb_stash(options: StashOptions) -> StashManager:
     from .codecs.passthru import PassthruCodec
     from .storages.lmdb import LmdbStorage
 
     storage = LmdbStorage(options=options)
     return _init_cache(storage, PassthruCodec(), options=options)
 
 
-def get_lmdb_zl_stash(options: StashOptions) -> StashManager:
+def get_lmdb_zlib_stash(options: StashOptions) -> StashManager:
     from .codecs.zlib import ZlibCodec
     from .storages.lmdb import LmdbStorage
 
     storage = LmdbStorage(options=options)
     return _init_cache(storage, ZlibCodec(), options=options)
 
 
@@ -109,14 +123,22 @@
     from .codecs.brotli import BrotliCodec
     from .storages.dbm_ import DbmStorage
 
     storage = DbmStorage(options=options)
     return _init_cache(storage, BrotliCodec(), options=options)
 
 
+def get_dbm_lzma_stash(options: StashOptions) -> StashManager:
+    from .codecs.lzma import LzmaCodec
+    from .storages.dbm_ import DbmStorage
+
+    storage = DbmStorage(options=options)
+    return _init_cache(storage, LzmaCodec(), options=options)
+
+
 def get_dbm_stash(options: StashOptions) -> StashManager:
     from .storages.dbm_ import DbmStorage
     from .codecs.passthru import PassthruCodec
 
     storage = DbmStorage(options=options)
     return _init_cache(storage, codec=PassthruCodec(), options=options)
 
@@ -133,14 +155,22 @@
     from .codecs.zstd import ZstdCodec
     from .storages.lsmdb import LsmDbStorage
 
     storage = LsmDbStorage(options=options)
     return _init_cache(storage, ZstdCodec(), options=options)
 
 
+def get_lsmdb_lzma_stash(options: StashOptions) -> StashManager:
+    from .codecs.lzma import LzmaCodec
+    from .storages.lsmdb import LsmDbStorage
+
+    storage = LsmDbStorage(options=options)
+    return _init_cache(storage, LzmaCodec(), options=options)
+
+
 def get_lsmdb_zlib_stash(options: StashOptions) -> StashManager:
     from .codecs.zlib import ZlibCodec
     from .storages.lsmdb import LsmDbStorage
 
     storage = LsmDbStorage(options=options)
     return _init_cache(storage, ZlibCodec(), options=options)
```

### Comparing `stashlib-0.0.6.1/stash/manager.py` & `stashlib-0.0.6.2/stash/manager.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.1/stash/options.py` & `stashlib-0.0.6.2/stash/options.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.1/stash/storages/dbm_.py` & `stashlib-0.0.6.2/stash/storages/dbm_.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.1/stash/storages/filesystem.py` & `stashlib-0.0.6.2/stash/storages/filesystem.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.1/stash/storages/lmdb.py` & `stashlib-0.0.6.2/stash/storages/lmdb.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.1/stash/storages/lsmdb.py` & `stashlib-0.0.6.2/stash/storages/lsmdb.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.1/stash/storages/memory.py` & `stashlib-0.0.6.2/stash/storages/memory.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.1/stash/storages/mongodb.py` & `stashlib-0.0.6.2/stash/storages/mongodb.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.1/stash/storages/redis.py` & `stashlib-0.0.6.2/stash/storages/redis.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.1/stash/storages/storage.py` & `stashlib-0.0.6.2/stash/storages/storage.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.1/stash/utils/checksum.py` & `stashlib-0.0.6.2/stash/utils/checksum.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.1/stash/utils/nested_path.py` & `stashlib-0.0.6.2/stash/utils/nested_path.py`

 * *Files identical despite different names*

### Comparing `stashlib-0.0.6.1/stashlib.egg-info/PKG-INFO` & `stashlib-0.0.6.2/stashlib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashlib
-Version: 0.0.6.1
+Version: 0.0.6.2
 Summary: stash is an extensible and lightweight cache library for python
 Home-page: https://github.com/masroore/stash.py
 Author: Masroor Ehsan
 Author-email: masroore@gmail.com
 License: MIT
 Keywords: cache caching
 Platform: any
```

### Comparing `stashlib-0.0.6.1/stashlib.egg-info/SOURCES.txt` & `stashlib-0.0.6.2/stashlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

