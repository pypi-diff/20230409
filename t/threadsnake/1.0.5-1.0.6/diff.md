# Comparing `tmp/threadsnake-1.0.5.tar.gz` & `tmp/threadsnake-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threadsnake-1.0.5.tar", last modified: Sat Apr  8 13:22:34 2023, max compression
+gzip compressed data, was "threadsnake-1.0.6.tar", last modified: Sun Apr  9 13:45:15 2023, max compression
```

## Comparing `threadsnake-1.0.5.tar` & `threadsnake-1.0.6.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-08 13:22:34.000744 threadsnake-1.0.5/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2023-04-07 19:56:48.000000 threadsnake-1.0.5/LICENSE
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       37 2023-04-07 21:41:56.000000 threadsnake-1.0.5/MANIFEST.in
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      860 2023-04-08 13:22:34.000744 threadsnake-1.0.5/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       86 2023-04-07 21:41:56.000000 threadsnake-1.0.5/README.MD
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2023-04-07 19:56:48.000000 threadsnake-1.0.5/pyproject.toml
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2023-04-08 13:22:34.000744 threadsnake-1.0.5/setup.cfg
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1152 2023-04-08 03:17:13.000000 threadsnake-1.0.5/setup.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-08 13:22:33.956744 threadsnake-1.0.5/src/
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-08 13:22:33.972744 threadsnake-1.0.5/src/threadsnake/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/__init__.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-08 13:22:33.976744 threadsnake-1.0.5/src/threadsnake/html/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/html/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      595 2023-04-08 13:22:26.000000 threadsnake-1.0.5/src/threadsnake/html/tools.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-08 13:22:33.976744 threadsnake-1.0.5/src/threadsnake/http/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2407 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/application.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-08 13:22:33.992744 threadsnake-1.0.5/src/threadsnake/http/core/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/core/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2847 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/core/common.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1059 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/core/constants.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4060 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/core/httprequest.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     5898 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/core/httpresponse.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2186 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/core/httpserver.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     3112 2023-04-08 12:09:56.000000 threadsnake-1.0.5/src/threadsnake/http/core/server.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1272 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/core/session.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-08 13:22:33.992744 threadsnake-1.0.5/src/threadsnake/http/core/values/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       79 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/core/values/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      404 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/core/values/contenttypes.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2203 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/core/values/responsecodes.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-08 13:22:34.000744 threadsnake-1.0.5/src/threadsnake/http/middlewares/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/middlewares/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      370 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/middlewares/app.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1626 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/middlewares/authorization.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1379 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/middlewares/bodyparser.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      334 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/middlewares/cors.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1332 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/middlewares/defaultheaders.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      679 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/middlewares/jsonbodyparser.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4038 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/middlewares/multipartformdataparser.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1970 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/middlewares/requests.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2186 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/middlewares/session.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1451 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/middlewares/static.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      467 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/middlewares/timemeassure.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4916 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/router.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-08 13:22:34.000744 threadsnake-1.0.5/src/threadsnake/http/tools/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/tools/__init__.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1202 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/tools/common.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4248 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/tools/routing.py
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1342 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/http/types.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-08 13:22:34.000744 threadsnake-1.0.5/src/threadsnake/turbo/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      199 2023-04-07 19:56:48.000000 threadsnake-1.0.5/src/threadsnake/turbo/__init__.py
-drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-08 13:22:33.972744 threadsnake-1.0.5/src/threadsnake.egg-info/
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      860 2023-04-08 13:22:33.000000 threadsnake-1.0.5/src/threadsnake.egg-info/PKG-INFO
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1609 2023-04-08 13:22:33.000000 threadsnake-1.0.5/src/threadsnake.egg-info/SOURCES.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2023-04-08 13:22:33.000000 threadsnake-1.0.5/src/threadsnake.egg-info/dependency_links.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       12 2023-04-08 13:22:33.000000 threadsnake-1.0.5/src/threadsnake.egg-info/top_level.txt
--rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        5 2023-04-08 13:22:26.000000 threadsnake-1.0.5/version.txt
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 13:45:15.582886 threadsnake-1.0.6/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)    35148 2023-04-07 19:56:48.000000 threadsnake-1.0.6/LICENSE
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       37 2023-04-07 21:41:56.000000 threadsnake-1.0.6/MANIFEST.in
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      860 2023-04-09 13:45:15.582886 threadsnake-1.0.6/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       86 2023-04-07 21:41:56.000000 threadsnake-1.0.6/README.MD
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       84 2023-04-07 19:56:48.000000 threadsnake-1.0.6/pyproject.toml
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       38 2023-04-09 13:45:15.582886 threadsnake-1.0.6/setup.cfg
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1152 2023-04-08 03:17:13.000000 threadsnake-1.0.6/setup.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 13:45:15.574886 threadsnake-1.0.6/src/
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 13:45:15.574886 threadsnake-1.0.6/src/threadsnake/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/__init__.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 13:45:15.578886 threadsnake-1.0.6/src/threadsnake/html/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/html/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      595 2023-04-08 13:22:26.000000 threadsnake-1.0.6/src/threadsnake/html/tools.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 13:45:15.578886 threadsnake-1.0.6/src/threadsnake/http/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2407 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/application.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 13:45:15.578886 threadsnake-1.0.6/src/threadsnake/http/core/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/core/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2847 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/core/common.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1059 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/core/constants.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4060 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/core/httprequest.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     5898 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/core/httpresponse.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2186 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/core/httpserver.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     3112 2023-04-08 12:09:56.000000 threadsnake-1.0.6/src/threadsnake/http/core/server.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1272 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/core/session.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 13:45:15.578886 threadsnake-1.0.6/src/threadsnake/http/core/values/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       79 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/core/values/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      404 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/core/values/contenttypes.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2203 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/core/values/responsecodes.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 13:45:15.582886 threadsnake-1.0.6/src/threadsnake/http/middlewares/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/middlewares/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      370 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/middlewares/app.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1626 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/middlewares/authorization.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1379 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/middlewares/bodyparser.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      334 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/middlewares/cors.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1332 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/middlewares/defaultheaders.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      679 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/middlewares/jsonbodyparser.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4038 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/middlewares/multipartformdataparser.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1970 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/middlewares/requests.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2186 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/middlewares/session.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1451 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/middlewares/static.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      467 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/middlewares/timemeassure.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     4916 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/router.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 13:45:15.582886 threadsnake-1.0.6/src/threadsnake/http/tools/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/tools/__init__.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1202 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/tools/common.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     2919 2023-04-09 13:45:07.000000 threadsnake-1.0.6/src/threadsnake/http/tools/routing.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1342 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/http/types.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 13:45:15.582886 threadsnake-1.0.6/src/threadsnake/turbo/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      199 2023-04-07 19:56:48.000000 threadsnake-1.0.6/src/threadsnake/turbo/__init__.py
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 13:45:15.578886 threadsnake-1.0.6/src/threadsnake.egg-info/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)      860 2023-04-09 13:45:15.000000 threadsnake-1.0.6/src/threadsnake.egg-info/PKG-INFO
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)     1635 2023-04-09 13:45:15.000000 threadsnake-1.0.6/src/threadsnake.egg-info/SOURCES.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        1 2023-04-09 13:45:15.000000 threadsnake-1.0.6/src/threadsnake.egg-info/dependency_links.txt
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       12 2023-04-09 13:45:15.000000 threadsnake-1.0.6/src/threadsnake.egg-info/top_level.txt
+drwxr-xr-x   0 actions-runner  (1000) actions-runner  (1000)        0 2023-04-09 13:45:15.582886 threadsnake-1.0.6/tests/
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)       35 2023-04-09 13:45:07.000000 threadsnake-1.0.6/tests/test_get_routing.py
+-rw-r--r--   0 actions-runner  (1000) actions-runner  (1000)        5 2023-04-09 13:45:07.000000 threadsnake-1.0.6/version.txt
```

### Comparing `threadsnake-1.0.5/LICENSE` & `threadsnake-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/PKG-INFO` & `threadsnake-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threadsnake
-Version: 1.0.5
+Version: 1.0.6
 Summary: A tiny experimental server-side express-like library
 Home-page: https://github.com/LostSavannah/threadsnake
 Author: Erick Fernando Mora Ramirez
 Author-email: erickfernandomoraramirez@gmail.com
 Project-URL: Bug Tracker, https://dev.moradev.dev/threadsnake/issues
 Project-URL: Documentation, https://dev.moradev.dev/threadsnake/documentation
 Project-URL: Examples, https://dev.moradev.dev/threadsnake/examples
```

### Comparing `threadsnake-1.0.5/setup.py` & `threadsnake-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake/html/tools.py` & `threadsnake-1.0.6/src/threadsnake/html/tools.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake/http/application.py` & `threadsnake-1.0.6/src/threadsnake/http/application.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake/http/core/common.py` & `threadsnake-1.0.6/src/threadsnake/http/core/common.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake/http/core/constants.py` & `threadsnake-1.0.6/src/threadsnake/http/core/constants.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake/http/core/httprequest.py` & `threadsnake-1.0.6/src/threadsnake/http/core/httprequest.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake/http/core/httpresponse.py` & `threadsnake-1.0.6/src/threadsnake/http/core/httpresponse.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake/http/core/httpserver.py` & `threadsnake-1.0.6/src/threadsnake/http/core/httpserver.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake/http/core/server.py` & `threadsnake-1.0.6/src/threadsnake/http/core/server.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake/http/core/session.py` & `threadsnake-1.0.6/src/threadsnake/http/core/session.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake/http/core/values/responsecodes.py` & `threadsnake-1.0.6/src/threadsnake/http/core/values/responsecodes.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake/http/middlewares/authorization.py` & `threadsnake-1.0.6/src/threadsnake/http/middlewares/authorization.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake/http/middlewares/bodyparser.py` & `threadsnake-1.0.6/src/threadsnake/http/middlewares/bodyparser.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake/http/middlewares/defaultheaders.py` & `threadsnake-1.0.6/src/threadsnake/http/middlewares/defaultheaders.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake/http/middlewares/jsonbodyparser.py` & `threadsnake-1.0.6/src/threadsnake/http/middlewares/jsonbodyparser.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake/http/middlewares/multipartformdataparser.py` & `threadsnake-1.0.6/src/threadsnake/http/middlewares/multipartformdataparser.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake/http/middlewares/requests.py` & `threadsnake-1.0.6/src/threadsnake/http/middlewares/requests.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake/http/middlewares/session.py` & `threadsnake-1.0.6/src/threadsnake/http/middlewares/session.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake/http/middlewares/static.py` & `threadsnake-1.0.6/src/threadsnake/http/middlewares/static.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake/http/router.py` & `threadsnake-1.0.6/src/threadsnake/http/router.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake/http/tools/common.py` & `threadsnake-1.0.6/src/threadsnake/http/tools/common.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake/http/types.py` & `threadsnake-1.0.6/src/threadsnake/http/types.py`

 * *Files identical despite different names*

### Comparing `threadsnake-1.0.5/src/threadsnake.egg-info/PKG-INFO` & `threadsnake-1.0.6/src/threadsnake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threadsnake
-Version: 1.0.5
+Version: 1.0.6
 Summary: A tiny experimental server-side express-like library
 Home-page: https://github.com/LostSavannah/threadsnake
 Author: Erick Fernando Mora Ramirez
 Author-email: erickfernandomoraramirez@gmail.com
 Project-URL: Bug Tracker, https://dev.moradev.dev/threadsnake/issues
 Project-URL: Documentation, https://dev.moradev.dev/threadsnake/documentation
 Project-URL: Examples, https://dev.moradev.dev/threadsnake/examples
```

### Comparing `threadsnake-1.0.5/src/threadsnake.egg-info/SOURCES.txt` & `threadsnake-1.0.6/src/threadsnake.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -37,8 +37,9 @@
 src/threadsnake/http/middlewares/requests.py
 src/threadsnake/http/middlewares/session.py
 src/threadsnake/http/middlewares/static.py
 src/threadsnake/http/middlewares/timemeassure.py
 src/threadsnake/http/tools/__init__.py
 src/threadsnake/http/tools/common.py
 src/threadsnake/http/tools/routing.py
-src/threadsnake/turbo/__init__.py
+src/threadsnake/turbo/__init__.py
+tests/test_get_routing.py
```

