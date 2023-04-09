# Comparing `tmp/dauth-0.0.1.tar.gz` & `tmp/dauth-0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dauth-0.0.1.tar", last modified: Sun Apr  9 21:29:36 2023, max compression
+gzip compressed data, was "dauth-0.0.dev2.tar", last modified: Sun Apr  9 21:38:51 2023, max compression
```

## Comparing `dauth-0.0.1.tar` & `dauth-0.0.dev2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 vvelikovich (161766200) 593637566        0 2023-04-09 21:29:36.680897 dauth-0.0.1/
--rw-r--r--   0 vvelikovich (161766200) 593637566       97 2023-04-09 21:29:36.680780 dauth-0.0.1/PKG-INFO
--rw-r--r--   0 vvelikovich (161766200) 593637566     1477 2023-04-09 21:29:17.000000 dauth-0.0.1/README.md
--rw-r--r--   0 vvelikovich (161766200) 593637566       38 2023-04-09 21:29:36.680929 dauth-0.0.1/setup.cfg
--rw-r--r--   0 vvelikovich (161766200) 593637566      353 2023-04-09 21:01:40.000000 dauth-0.0.1/setup.py
-drwxr-xr-x   0 vvelikovich (161766200) 593637566        0 2023-04-09 21:29:36.679573 dauth-0.0.1/src/
-drwxr-xr-x   0 vvelikovich (161766200) 593637566        0 2023-04-09 21:29:36.680123 dauth-0.0.1/src/dauth/
--rw-r--r--   0 vvelikovich (161766200) 593637566      149 2023-04-09 20:57:55.000000 dauth-0.0.1/src/dauth/__init__.py
--rw-r--r--   0 vvelikovich (161766200) 593637566      601 2023-04-09 21:17:50.000000 dauth-0.0.1/src/dauth/auth.py
-drwxr-xr-x   0 vvelikovich (161766200) 593637566        0 2023-04-09 21:29:36.680634 dauth-0.0.1/src/dauth.egg-info/
--rw-r--r--   0 vvelikovich (161766200) 593637566       97 2023-04-09 21:29:36.000000 dauth-0.0.1/src/dauth.egg-info/PKG-INFO
--rw-r--r--   0 vvelikovich (161766200) 593637566      190 2023-04-09 21:29:36.000000 dauth-0.0.1/src/dauth.egg-info/SOURCES.txt
--rw-r--r--   0 vvelikovich (161766200) 593637566        1 2023-04-09 21:29:36.000000 dauth-0.0.1/src/dauth.egg-info/dependency_links.txt
--rw-r--r--   0 vvelikovich (161766200) 593637566        6 2023-04-09 21:29:36.000000 dauth-0.0.1/src/dauth.egg-info/top_level.txt
+drwxr-xr-x   0 vvelikovich (161766200) 593637566        0 2023-04-09 21:38:51.023845 dauth-0.0.dev2/
+-rw-r--r--   0 vvelikovich (161766200) 593637566     1628 2023-04-09 21:38:51.023713 dauth-0.0.dev2/PKG-INFO
+-rw-r--r--   0 vvelikovich (161766200) 593637566     1487 2023-04-09 21:37:25.000000 dauth-0.0.dev2/README.md
+-rw-r--r--   0 vvelikovich (161766200) 593637566       38 2023-04-09 21:38:51.023882 dauth-0.0.dev2/setup.cfg
+-rw-r--r--   0 vvelikovich (161766200) 593637566      576 2023-04-09 21:37:09.000000 dauth-0.0.dev2/setup.py
+drwxr-xr-x   0 vvelikovich (161766200) 593637566        0 2023-04-09 21:38:51.022276 dauth-0.0.dev2/src/
+drwxr-xr-x   0 vvelikovich (161766200) 593637566        0 2023-04-09 21:38:51.022981 dauth-0.0.dev2/src/dauth/
+-rw-r--r--   0 vvelikovich (161766200) 593637566      149 2023-04-09 20:57:55.000000 dauth-0.0.dev2/src/dauth/__init__.py
+-rw-r--r--   0 vvelikovich (161766200) 593637566      601 2023-04-09 21:17:50.000000 dauth-0.0.dev2/src/dauth/auth.py
+drwxr-xr-x   0 vvelikovich (161766200) 593637566        0 2023-04-09 21:38:51.023556 dauth-0.0.dev2/src/dauth.egg-info/
+-rw-r--r--   0 vvelikovich (161766200) 593637566     1628 2023-04-09 21:38:50.000000 dauth-0.0.dev2/src/dauth.egg-info/PKG-INFO
+-rw-r--r--   0 vvelikovich (161766200) 593637566      190 2023-04-09 21:38:51.000000 dauth-0.0.dev2/src/dauth.egg-info/SOURCES.txt
+-rw-r--r--   0 vvelikovich (161766200) 593637566        1 2023-04-09 21:38:50.000000 dauth-0.0.dev2/src/dauth.egg-info/dependency_links.txt
+-rw-r--r--   0 vvelikovich (161766200) 593637566        6 2023-04-09 21:38:50.000000 dauth-0.0.dev2/src/dauth.egg-info/top_level.txt
```

### Comparing `dauth-0.0.1/README.md` & `dauth-0.0.dev2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 - - `item_id` __(by default '*')__ is providing by FastAPI decorator `@app.get(/test/{item_id})`
 - - `method` is argument of `Policy()`
 
 ---
 ## Examples
 Simple usage
 ```python
-from fastapi import Depends
+from fastapi import FastAPI, Depends
 from dauth import auth
 
 app = FastAPI()
 
 def is_admin(subject, resource_type, item_id, method):
     if 'admin' not in subject.scopes:
         raise auth.DENY
@@ -53,8 +53,8 @@
 @app.get("/test")
 # function get_user_auth returns User's object
 def test(user = Depends(auth.Policy(get_user_auth, 'test', 'get', is_admin))):
     return {"message":"Good"}
 ```
 
 ---
-Developed by [DenVilk](https://github.com/denvilk)
+Developed by [DenVilk](https://github.com/denvilk)
```

### Comparing `dauth-0.0.1/src/dauth/auth.py` & `dauth-0.0.dev2/src/dauth/auth.py`

 * *Files identical despite different names*

