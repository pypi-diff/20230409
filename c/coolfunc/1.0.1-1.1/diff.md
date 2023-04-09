# Comparing `tmp/coolfunc-1.0.1.tar.gz` & `tmp/coolfunc-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolfunc-1.0.1.tar", last modified: Sat Apr  8 18:36:23 2023, max compression
+gzip compressed data, was "coolfunc-1.1.tar", last modified: Sun Apr  9 16:20:20 2023, max compression
```

## Comparing `coolfunc-1.0.1.tar` & `coolfunc-1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.559068 coolfunc-1.0.1/LICENSE
--rw-r--r--   0        0        0      119 2023-03-26 12:11:14.648893 coolfunc-1.0.1/README.md
--rw-r--r--   0        0        0       40 2023-03-05 13:34:26.457361 coolfunc-1.0.1/coolfunc/__init__.py
--rw-r--r--   0        0        0     1694 2023-03-05 13:23:09.230912 coolfunc-1.0.1/coolfunc/_coolfunc.py
--rw-r--r--   0        0        0      460 2023-04-08 18:34:43.091346 coolfunc-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 coolfunc-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.559068 coolfunc-1.1/LICENSE
+-rw-r--r--   0        0        0      119 2023-03-26 12:11:14.648893 coolfunc-1.1/README.md
+-rw-r--r--   0        0        0       24 2023-04-09 15:53:46.667418 coolfunc-1.1/coolfunc/__init__.py
+-rw-r--r--   0        0        0     1995 2023-04-09 16:14:05.921381 coolfunc-1.1/coolfunc/_coolfunc.py
+-rw-r--r--   0        0        0      458 2023-04-09 16:13:15.581546 coolfunc-1.1/pyproject.toml
+-rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 coolfunc-1.1/PKG-INFO
```

### Comparing `coolfunc-1.0.1/LICENSE` & `coolfunc-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coolfunc-1.0.1/coolfunc/_coolfunc.py` & `coolfunc-1.1/coolfunc/_coolfunc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,66 @@
 '''
 Copyright [2023] [许灿标]
 license: Apache License, Version 2.0
 email: lcctoor@outlook.com
 '''
 
-from vtype import SysEmpty
+import numpy as _np
+from pathlib import Path as _Path
+from vtype import SysEmpty as _SysEmpty
 
 # 以下模块允许被其它模块导入
 from json import dumps as jsonDumps
 from json import loads as jsonLoads
 from pickle import dumps as pickleDumps
 from pickle import loads as pickleLoads
-from pathlib import Path as libpath
 from os.path import abspath
 
 
 def jsonChinese(data): return jsonDumps(data, ensure_ascii=False)
 
 # 三元表达式
 def ternary(tv, obj, fv): return tv if obj else fv
 
-def setDir(path):
-    return libpath(path).mkdir(parents=True, exist_ok=True)
-def setParentDir(path):
-    return libpath(path).parent.mkdir(parents=True, exist_ok=True)
+def check_dir(path):
+    return _Path(path).mkdir(parents=True, exist_ok=True)
+def check_parent_dir(path):
+    return _Path(path).parent.mkdir(parents=True, exist_ok=True)
 
-def readJson(fpath, default=SysEmpty, mode=3):
+def readJson(fpath, default=_SysEmpty, mode=3):
     '''
     mode:
         等于1时: 文件不存在时返回default
         等于2时: 文件内容解析错误时返回default
         等于3时: 无论哪种错误, 都返回default
     '''
     try:
-        return jsonLoads(libpath(fpath).read_text('utf8'))
+        return jsonLoads(_Path(fpath).read_text('utf8'))
     except BaseException as e:
-        if default is not SysEmpty:
+        if default is not _SysEmpty:
             if mode == 3: return default
             if mode == 1 and type(e) is FileNotFoundError: return default
         raise
 
 def writeJson(fpath, data, ensure_ascii=False):
-    fpath = libpath(fpath)
+    fpath = _Path(fpath)
     data = jsonDumps(data, ensure_ascii=ensure_ascii)
     try:
         return fpath.write_text(data, 'utf8')
     except FileNotFoundError:
         fpath.parent.mkdir(parents=True, exist_ok=True)
         return fpath.write_text(data, 'utf8')
 
-def rePathClash(path):
-    # 解决命名冲突
-    while libpath(path).exists():
+def repairPathClash(path):
+    ''' 解决命名冲突 '''
+    while _Path(path).exists():
         path += '_'
-    return path
+    return path
+
+def uniform_put(total, siteCount):
+    ''' 均匀放球 '''
+    baseCount, r = divmod(total, siteCount)
+    sites = [baseCount] * siteCount
+    if r:
+        for x in _np.linspace(0, siteCount-1, r):
+            sites[round(x)] += 1
+    return sites
```

