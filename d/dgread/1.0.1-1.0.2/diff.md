# Comparing `tmp/dgread-1.0.1.tar.gz` & `tmp/dgread-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dgread-1.0.1.tar", last modified: Sun Apr  9 15:16:30 2023, max compression
+gzip compressed data, was "dgread-1.0.2.tar", last modified: Sun Apr  9 15:31:53 2023, max compression
```

## Comparing `dgread-1.0.1.tar` & `dgread-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,34 @@
-drwxr-xr-x   0 sheinb     (501) staff       (20)        0 2023-04-09 15:16:30.000000 dgread-1.0.1/
--rw-r--r--   0 sheinb     (501) staff       (20)     1311 2023-04-09 15:12:42.000000 dgread-1.0.1/LICENSE-lz4
--rw-r--r--   0 sheinb     (501) staff       (20)       76 2023-04-09 15:16:30.000000 dgread-1.0.1/PKG-INFO
--rw-r--r--   0 sheinb     (501) staff       (20)      210 2023-04-09 15:16:26.000000 dgread-1.0.1/README.md
--rw-r--r--   0 sheinb     (501) staff       (20)    26839 2023-04-08 15:21:35.000000 dgread-1.0.1/df.c
--rwxr-xr-x   0 sheinb     (501) staff       (20)   108069 2023-04-08 15:21:35.000000 dgread-1.0.1/dfutils.c
--rwxr-xr-x   0 sheinb     (501) staff       (20)    10680 2023-04-08 15:21:35.000000 dgread-1.0.1/dgread.c
-drwxr-xr-x   0 sheinb     (501) staff       (20)        0 2023-04-09 15:16:30.000000 dgread-1.0.1/dgread.egg-info/
--rwxr-xr-x   0 sheinb     (501) staff       (20)       76 2023-04-09 15:16:30.000000 dgread-1.0.1/dgread.egg-info/PKG-INFO
--rwxr-xr-x   0 sheinb     (501) staff       (20)      234 2023-04-09 15:16:30.000000 dgread-1.0.1/dgread.egg-info/SOURCES.txt
--rwxr-xr-x   0 sheinb     (501) staff       (20)        1 2023-04-09 15:16:30.000000 dgread-1.0.1/dgread.egg-info/dependency_links.txt
--rwxr-xr-x   0 sheinb     (501) staff       (20)        7 2023-04-09 15:16:30.000000 dgread-1.0.1/dgread.egg-info/top_level.txt
--rw-r--r--   0 sheinb     (501) staff       (20)    59097 2023-04-08 15:21:35.000000 dgread-1.0.1/dynio.c
--rwxr-xr-x   0 sheinb     (501) staff       (20)     1892 2023-04-08 15:21:35.000000 dgread-1.0.1/flip.c
--rwxr-xr-x   0 sheinb     (501) staff       (20)   114204 2023-04-09 15:12:20.000000 dgread-1.0.1/lz4.c
--rwxr-xr-x   0 sheinb     (501) staff       (20)    88996 2023-04-09 15:12:20.000000 dgread-1.0.1/lz4frame.c
--rwxr-xr-x   0 sheinb     (501) staff       (20)    70760 2023-04-09 15:12:20.000000 dgread-1.0.1/lz4hc.c
--rwxr-xr-x   0 sheinb     (501) staff       (20)     4816 2023-04-08 15:21:35.000000 dgread-1.0.1/lz4utils.c
--rw-r--r--   0 sheinb     (501) staff       (20)       38 2023-04-09 15:16:30.000000 dgread-1.0.1/setup.cfg
--rwxr-xr-x   0 sheinb     (501) staff       (20)      475 2023-04-08 15:37:38.000000 dgread-1.0.1/setup.py
--rwxr-xr-x   0 sheinb     (501) staff       (20)    34045 2023-04-09 15:12:20.000000 dgread-1.0.1/xxhash.c
+drwxr-xr-x   0 sheinb     (501) staff       (20)        0 2023-04-09 15:31:53.601278 dgread-1.0.2/
+-rw-r--r--   0 sheinb     (501) staff       (20)     1311 2023-04-09 15:12:42.000000 dgread-1.0.2/LICENSE-lz4
+-rw-r--r--   0 sheinb     (501) staff       (20)       11 2023-04-09 15:29:41.000000 dgread-1.0.2/MANIFEST.in
+-rw-r--r--   0 sheinb     (501) staff       (20)       76 2023-04-09 15:31:53.600972 dgread-1.0.2/PKG-INFO
+-rw-r--r--   0 sheinb     (501) staff       (20)      210 2023-04-09 15:16:26.000000 dgread-1.0.2/README.md
+-rw-r--r--   0 sheinb     (501) staff       (20)    26839 2023-04-08 15:21:35.000000 dgread-1.0.2/df.c
+-rw-r--r--   0 sheinb     (501) staff       (20)    40343 2023-04-08 15:21:35.000000 dgread-1.0.2/df.h
+-rwxr-xr-x   0 sheinb     (501) staff       (20)   108069 2023-04-08 15:21:35.000000 dgread-1.0.2/dfutils.c
+-rwxr-xr-x   0 sheinb     (501) staff       (20)    10680 2023-04-08 15:21:35.000000 dgread-1.0.2/dgread.c
+drwxr-xr-x   0 sheinb     (501) staff       (20)        0 2023-04-09 15:31:53.600498 dgread-1.0.2/dgread.egg-info/
+-rwxr-xr-x   0 sheinb     (501) staff       (20)       76 2023-04-09 15:31:53.000000 dgread-1.0.2/dgread.egg-info/PKG-INFO
+-rwxr-xr-x   0 sheinb     (501) staff       (20)      353 2023-04-09 15:31:53.000000 dgread-1.0.2/dgread.egg-info/SOURCES.txt
+-rwxr-xr-x   0 sheinb     (501) staff       (20)        1 2023-04-09 15:31:53.000000 dgread-1.0.2/dgread.egg-info/dependency_links.txt
+-rwxr-xr-x   0 sheinb     (501) staff       (20)        7 2023-04-09 15:31:53.000000 dgread-1.0.2/dgread.egg-info/top_level.txt
+-rw-r--r--   0 sheinb     (501) staff       (20)    59097 2023-04-08 15:21:35.000000 dgread-1.0.2/dynio.c
+-rw-r--r--   0 sheinb     (501) staff       (20)     3623 2023-04-08 15:21:35.000000 dgread-1.0.2/dynio.h
+-rwxr-xr-x   0 sheinb     (501) staff       (20)     1892 2023-04-08 15:21:35.000000 dgread-1.0.2/flip.c
+-rwxr-xr-x   0 sheinb     (501) staff       (20)   114204 2023-04-09 15:12:20.000000 dgread-1.0.2/lz4.c
+-rwxr-xr-x   0 sheinb     (501) staff       (20)    44421 2023-04-09 15:12:20.000000 dgread-1.0.2/lz4.h
+-rw-r--r--   0 sheinb     (501) staff       (20)     3304 2023-04-09 15:12:20.000000 dgread-1.0.2/lz4file.h
+-rwxr-xr-x   0 sheinb     (501) staff       (20)    88996 2023-04-09 15:12:20.000000 dgread-1.0.2/lz4frame.c
+-rwxr-xr-x   0 sheinb     (501) staff       (20)    33741 2023-04-09 15:12:20.000000 dgread-1.0.2/lz4frame.h
+-rwxr-xr-x   0 sheinb     (501) staff       (20)     2044 2023-04-09 15:12:20.000000 dgread-1.0.2/lz4frame_static.h
+-rwxr-xr-x   0 sheinb     (501) staff       (20)    70760 2023-04-09 15:12:20.000000 dgread-1.0.2/lz4hc.c
+-rwxr-xr-x   0 sheinb     (501) staff       (20)    20179 2023-04-09 15:12:20.000000 dgread-1.0.2/lz4hc.h
+-rwxr-xr-x   0 sheinb     (501) staff       (20)    13986 2023-04-08 15:21:35.000000 dgread-1.0.2/lz4opt.h
+-rwxr-xr-x   0 sheinb     (501) staff       (20)     4816 2023-04-08 15:21:35.000000 dgread-1.0.2/lz4utils.c
+-rw-r--r--   0 sheinb     (501) staff       (20)       38 2023-04-09 15:31:53.601380 dgread-1.0.2/setup.cfg
+-rwxr-xr-x   0 sheinb     (501) staff       (20)      494 2023-04-09 15:31:38.000000 dgread-1.0.2/setup.py
+-rwxr-xr-x   0 sheinb     (501) staff       (20)     3065 2023-04-08 15:21:35.000000 dgread-1.0.2/utilc.h
+-rwxr-xr-x   0 sheinb     (501) staff       (20)    34045 2023-04-09 15:12:20.000000 dgread-1.0.2/xxhash.c
+-rwxr-xr-x   0 sheinb     (501) staff       (20)    13466 2023-04-09 15:12:20.000000 dgread-1.0.2/xxhash.h
+-rwxr-xr-x   0 sheinb     (501) staff       (20)    15508 2023-04-08 15:21:35.000000 dgread-1.0.2/zconf.h
+-rwxr-xr-x   0 sheinb     (501) staff       (20)    87883 2023-04-08 15:21:35.000000 dgread-1.0.2/zlib.h
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dgread-1.0.1/LICENSE-lz4` & `dgread-1.0.2/LICENSE-lz4`

 * *Files identical despite different names*

### Comparing `dgread-1.0.1/df.c` & `dgread-1.0.2/df.c`

 * *Files identical despite different names*

### Comparing `dgread-1.0.1/dfutils.c` & `dgread-1.0.2/dfutils.c`

 * *Files identical despite different names*

### Comparing `dgread-1.0.1/dgread.c` & `dgread-1.0.2/dgread.c`

 * *Files identical despite different names*

### Comparing `dgread-1.0.1/dynio.c` & `dgread-1.0.2/dynio.c`

 * *Files identical despite different names*

### Comparing `dgread-1.0.1/flip.c` & `dgread-1.0.2/flip.c`

 * *Files identical despite different names*

### Comparing `dgread-1.0.1/lz4.c` & `dgread-1.0.2/lz4.c`

 * *Files identical despite different names*

### Comparing `dgread-1.0.1/lz4frame.c` & `dgread-1.0.2/lz4frame.c`

 * *Files identical despite different names*

### Comparing `dgread-1.0.1/lz4hc.c` & `dgread-1.0.2/lz4hc.c`

 * *Files identical despite different names*

### Comparing `dgread-1.0.1/lz4utils.c` & `dgread-1.0.2/lz4utils.c`

 * *Files identical despite different names*

### Comparing `dgread-1.0.1/xxhash.c` & `dgread-1.0.2/xxhash.c`

 * *Files identical despite different names*

