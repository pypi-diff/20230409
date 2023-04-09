# Comparing `tmp/tornado-6.2b2.tar.gz` & `tmp/tornado-6.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tornado-6.2b2.tar", last modified: Fri Jun 17 20:41:49 2022, max compression
+gzip compressed data, was "tornado-6.3b1.tar", last modified: Sun Apr  9 20:54:13 2023, max compression
```

## Comparing `tornado-6.2b2.tar` & `tornado-6.3b1.tar`

### file list

```diff
@@ -1,278 +1,277 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.795465 tornado-6.2b2/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-06-17 20:41:47.000000 tornado-6.2b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-06-17 20:41:47.000000 tornado-6.2b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2540 2022-06-17 20:41:49.795465 tornado-6.2b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1604 2022-06-17 20:41:47.000000 tornado-6.2b2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.767462 tornado-6.2b2/demos/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.771463 tornado-6.2b2/demos/blog/
--rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/blog/README
--rwxr-xr-x   0 runner    (1001) docker     (121)    10501 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/blog/blog.py
--rw-r--r--   0 runner    (1001) docker     (121)     1354 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/blog/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.771463 tornado-6.2b2/demos/blog/static/
--rw-r--r--   0 runner    (1001) docker     (121)     2130 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/blog/static/blog.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.771463 tornado-6.2b2/demos/blog/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/blog/templates/archive.html
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/blog/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (121)     1549 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/blog/templates/compose.html
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/blog/templates/create_author.html
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/blog/templates/entry.html
--rw-r--r--   0 runner    (1001) docker     (121)     1345 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/blog/templates/feed.xml
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/blog/templates/home.html
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/blog/templates/login.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.771463 tornado-6.2b2/demos/blog/templates/modules/
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/blog/templates/modules/entry.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.771463 tornado-6.2b2/demos/chat/
--rwxr-xr-x   0 runner    (1001) docker     (121)     4167 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/chat/chatdemo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.771463 tornado-6.2b2/demos/chat/static/
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/chat/static/chat.css
--rw-r--r--   0 runner    (1001) docker     (121)     4033 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/chat/static/chat.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.775463 tornado-6.2b2/demos/chat/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/chat/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/chat/templates/message.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.775463 tornado-6.2b2/demos/facebook/
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/facebook/README
--rwxr-xr-x   0 runner    (1001) docker     (121)     4241 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/facebook/facebook.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.775463 tornado-6.2b2/demos/facebook/static/
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/facebook/static/facebook.css
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/facebook/static/facebook.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.775463 tornado-6.2b2/demos/facebook/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.775463 tornado-6.2b2/demos/facebook/templates/modules/
--rw-r--r--   0 runner    (1001) docker     (121)      766 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/facebook/templates/modules/post.html
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/facebook/templates/stream.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.775463 tornado-6.2b2/demos/file_upload/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1566 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/file_upload/file_receiver.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3429 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/file_upload/file_uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.775463 tornado-6.2b2/demos/helloworld/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1208 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/helloworld/helloworld.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.775463 tornado-6.2b2/demos/s3server/
--rw-r--r--   0 runner    (1001) docker     (121)    10016 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/s3server/s3server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.775463 tornado-6.2b2/demos/tcpecho/
--rwxr-xr-x   0 runner    (1001) docker     (121)      696 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/tcpecho/client.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1118 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/tcpecho/server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.775463 tornado-6.2b2/demos/twitter/
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/twitter/home.html
--rwxr-xr-x   0 runner    (1001) docker     (121)     3477 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/twitter/twitterdemo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.775463 tornado-6.2b2/demos/websocket/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3087 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/websocket/chatdemo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.775463 tornado-6.2b2/demos/websocket/static/
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/websocket/static/chat.css
--rw-r--r--   0 runner    (1001) docker     (121)     2013 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/websocket/static/chat.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.775463 tornado-6.2b2/demos/websocket/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/websocket/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/websocket/templates/message.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.775463 tornado-6.2b2/demos/webspider/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2705 2022-06-17 20:41:47.000000 tornado-6.2b2/demos/webspider/webspider.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.779464 tornado-6.2b2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      812 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/asyncio.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/auth.rst
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/autoreload.rst
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/caresresolver.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/concurrent.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4081 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/coroutine.rst
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/escape.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3783 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/gen.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.779464 tornado-6.2b2/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (121)     4648 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/guide/async.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10975 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/guide/coroutines.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/guide/intro.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1317 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/guide/queues.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10932 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/guide/running.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12739 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/guide/security.rst
--rw-r--r--   0 runner    (1001) docker     (121)    14257 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/guide/structure.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12557 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/guide/templates.rst
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/guide.rst
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/http.rst
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/http1connection.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/httpclient.rst
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/httpserver.rst
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/httputil.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5649 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/integration.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1263 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/ioloop.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/iostream.rst
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/locale.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/locks.rst
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/log.rst
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/netutil.rst
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/networking.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/options.rst
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/process.rst
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/queues.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.783464 tornado-6.2b2/docs/releases/
--rw-r--r--   0 runner    (1001) docker     (121)     2667 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v1.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v1.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2693 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v1.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)      873 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v1.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5743 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v1.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)      753 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v1.2.1.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2702 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v2.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7576 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v2.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v2.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5583 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v2.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v2.2.1.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5077 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v2.3.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2885 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v2.4.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v2.4.1.rst
--rw-r--r--   0 runner    (1001) docker     (121)    21093 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v3.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v3.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v3.0.2.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10631 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v3.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v3.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7267 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v3.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v3.2.1.rst
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v3.2.2.rst
--rw-r--r--   0 runner    (1001) docker     (121)    14923 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v4.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)      861 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v4.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v4.0.2.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7851 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v4.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8800 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v4.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v4.2.1.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6985 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v4.3.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2638 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v4.4.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v4.4.1.rst
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v4.4.2.rst
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v4.4.3.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7147 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v4.5.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v4.5.1.rst
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v4.5.2.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v4.5.3.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13114 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v5.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v5.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v5.0.2.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7840 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v5.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)      390 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v5.1.1.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5573 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v6.0.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v6.0.1.rst
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v6.0.2.rst
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v6.0.3.rst
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v6.0.4.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3691 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v6.1.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4716 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases/v6.2.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/releases.rst
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/requirements.in
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/routing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/tcpclient.rst
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/tcpserver.rst
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/template.rst
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7101 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/tornado.png
--rw-r--r--   0 runner    (1001) docker     (121)     2253 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/twisted.rst
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/util.rst
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (121)    14108 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/web.rst
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/webframework.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/websocket.rst
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-06-17 20:41:47.000000 tornado-6.2b2/docs/wsgi.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-06-17 20:41:47.000000 tornado-6.2b2/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (121)      511 2022-06-17 20:41:47.000000 tornado-6.2b2/runtests.sh
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-06-17 20:41:49.795465 tornado-6.2b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4108 2022-06-17 20:41:47.000000 tornado-6.2b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.787464 tornado-6.2b2/tornado/
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4627 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/_locale_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    45955 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)    13585 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (121)     8154 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (121)    24660 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/curl_httpclient.py
--rw-r--r--   0 runner    (1001) docker     (121)    13267 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/escape.py
--rw-r--r--   0 runner    (1001) docker     (121)    31168 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/gen.py
--rw-r--r--   0 runner    (1001) docker     (121)    36191 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/http1connection.py
--rw-r--r--   0 runner    (1001) docker     (121)    31919 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/httpclient.py
--rw-r--r--   0 runner    (1001) docker     (121)    16126 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/httpserver.py
--rw-r--r--   0 runner    (1001) docker     (121)    36001 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/httputil.py
--rw-r--r--   0 runner    (1001) docker     (121)    36271 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/ioloop.py
--rw-r--r--   0 runner    (1001) docker     (121)    66422 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/iostream.py
--rw-r--r--   0 runner    (1001) docker     (121)    20895 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/locale.py
--rw-r--r--   0 runner    (1001) docker     (121)    17356 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/locks.py
--rw-r--r--   0 runner    (1001) docker     (121)    12549 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/log.py
--rw-r--r--   0 runner    (1001) docker     (121)    25289 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/netutil.py
--rw-r--r--   0 runner    (1001) docker     (121)    26203 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/options.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.791465 tornado-6.2b2/tornado/platform/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25806 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/platform/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)     3465 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/platform/caresresolver.py
--rw-r--r--   0 runner    (1001) docker     (121)     5624 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/platform/twisted.py
--rw-r--r--   0 runner    (1001) docker     (121)    12789 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/process.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    12478 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/queues.py
--rw-r--r--   0 runner    (1001) docker     (121)    25082 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/routing.py
--rw-r--r--   0 runner    (1001) docker     (121)    27784 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/simple_httpclient.py
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/speedups.c
--rw-r--r--   0 runner    (1001) docker     (121)    12076 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/tcpclient.py
--rw-r--r--   0 runner    (1001) docker     (121)    15354 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/tcpserver.py
--rw-r--r--   0 runner    (1001) docker     (121)    37793 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.795465 tornado-6.2b2/tornado/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7714 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/asyncio_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    23437 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/auth_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3948 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/autoreload_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     6049 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/concurrent_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.795465 tornado-6.2b2/tornado/test/csv_translations/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/csv_translations/fr_FR.csv
--rw-r--r--   0 runner    (1001) docker     (121)     4303 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/curl_httpclient_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    12372 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/escape_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    33838 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/gen_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.767462 tornado-6.2b2/tornado/test/gettext_translations/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.767462 tornado-6.2b2/tornado/test/gettext_translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.795465 tornado-6.2b2/tornado/test/gettext_translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/gettext_translations/fr_FR/LC_MESSAGES/tornado_test.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/gettext_translations/fr_FR/LC_MESSAGES/tornado_test.po
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/http1connection_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    34745 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/httpclient_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    47090 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/httpserver_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    19053 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/httputil_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2074 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/import_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    28041 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/ioloop_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    47311 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/iostream_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     5756 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/locale_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    17010 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/locks_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     9480 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/log_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7959 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/netutil_test.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/options_test.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    11767 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/options_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/options_test_types.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/options_test_types_str.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    11308 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/process_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    13981 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/queues_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/resolve_test_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     8827 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/routing_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     8348 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/runtests.py
--rw-r--r--   0 runner    (1001) docker     (121)    31109 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/simple_httpclient_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.795465 tornado-6.2b2/tornado/test/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.795465 tornado-6.2b2/tornado/test/static/dir/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/static/dir/index.html
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/static/robots.txt
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/static/sample.xml
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/static/sample.xml.bz2
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/static/sample.xml.gz
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/static_foo.txt
--rw-r--r--   0 runner    (1001) docker     (121)    16787 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/tcpclient_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     7720 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/tcpserver_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    18668 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/template_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.795465 tornado-6.2b2/tornado/test/templates/
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/templates/utf8.html
--rw-r--r--   0 runner    (1001) docker     (121)     1224 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/test.crt
--rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/test.key
--rw-r--r--   0 runner    (1001) docker     (121)    11228 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/testing_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1732 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/twisted_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3654 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     9781 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/util_test.py
--rw-r--r--   0 runner    (1001) docker     (121)   117196 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/web_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    28211 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/websocket_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/test/wsgi_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    34043 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/testing.py
--rw-r--r--   0 runner    (1001) docker     (121)    16249 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/util.py
--rw-r--r--   0 runner    (1001) docker     (121)   138994 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/web.py
--rw-r--r--   0 runner    (1001) docker     (121)    61220 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/websocket.py
--rw-r--r--   0 runner    (1001) docker     (121)     7970 2022-06-17 20:41:47.000000 tornado-6.2b2/tornado/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-17 20:41:49.791465 tornado-6.2b2/tornado.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2540 2022-06-17 20:41:49.000000 tornado-6.2b2/tornado.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5967 2022-06-17 20:41:49.000000 tornado-6.2b2/tornado.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-17 20:41:49.000000 tornado-6.2b2/tornado.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-17 20:41:49.000000 tornado-6.2b2/tornado.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.769427 tornado-6.3b1/
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-04-09 20:54:12.000000 tornado-6.3b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-04-09 20:54:12.000000 tornado-6.3b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-04-09 20:54:13.769427 tornado-6.3b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1599 2023-04-09 20:54:12.000000 tornado-6.3b1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.737425 tornado-6.3b1/demos/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/blog/
+-rw-r--r--   0 runner    (1001) docker     (122)     2106 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/README
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10383 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/blog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1354 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/blog/static/
+-rw-r--r--   0 runner    (1001) docker     (122)     2130 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/static/blog.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/blog/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      673 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/templates/archive.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1028 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1549 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/templates/compose.html
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/templates/create_author.html
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/templates/entry.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1345 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/templates/feed.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/templates/home.html
+-rw-r--r--   0 runner    (1001) docker     (122)      342 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/templates/login.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/blog/templates/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/blog/templates/modules/entry.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/chat/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4120 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/chat/chatdemo.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/chat/static/
+-rw-r--r--   0 runner    (1001) docker     (122)      989 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/chat/static/chat.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4033 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/chat/static/chat.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/chat/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/chat/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/chat/templates/message.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/facebook/
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/facebook/README
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4146 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/facebook/facebook.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/facebook/static/
+-rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/facebook/static/facebook.css
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/facebook/static/facebook.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/facebook/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/facebook/templates/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/facebook/templates/modules/post.html
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/facebook/templates/stream.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/file_upload/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1562 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/file_upload/file_receiver.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3429 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/file_upload/file_uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/helloworld/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1155 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/helloworld/helloworld.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/s3server/
+-rw-r--r--   0 runner    (1001) docker     (122)    10014 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/s3server/s3server.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/tcpecho/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      696 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/tcpecho/client.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1118 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/tcpecho/server.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/twitter/
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/twitter/home.html
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3477 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/twitter/twitterdemo.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/websocket/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3013 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/websocket/chatdemo.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/websocket/static/
+-rw-r--r--   0 runner    (1001) docker     (122)      989 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/websocket/static/chat.css
+-rw-r--r--   0 runner    (1001) docker     (122)     2013 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/websocket/static/chat.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/websocket/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/websocket/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/websocket/templates/message.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.741426 tornado-6.3b1/demos/webspider/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2705 2023-04-09 20:54:12.000000 tornado-6.3b1/demos/webspider/webspider.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.745426 tornado-6.3b1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/asyncio.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/auth.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/autoreload.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      968 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/caresresolver.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1206 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/concurrent.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4119 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/coroutine.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      912 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/escape.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (122)     1047 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/gen.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.745426 tornado-6.3b1/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/guide/async.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10975 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/guide/coroutines.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1409 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/guide/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/guide/queues.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10932 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/guide/running.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    12712 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/guide/security.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    14248 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/guide/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    12553 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/guide/templates.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/guide.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/http.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/http1connection.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/httpclient.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      910 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/httpserver.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/httputil.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5644 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/integration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1263 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/ioloop.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/iostream.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/locale.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/locks.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/log.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/netutil.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/networking.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1036 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/options.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/process.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      523 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/queues.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.753426 tornado-6.3b1/docs/releases/
+-rw-r--r--   0 runner    (1001) docker     (122)     2667 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v1.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v1.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2693 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v1.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      873 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v1.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5743 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v1.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v1.2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2702 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v2.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7576 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v2.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v2.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5583 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v2.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v2.2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5077 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v2.3.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2885 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v2.4.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v2.4.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    21093 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v3.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1019 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v3.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v3.0.2.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10631 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v3.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      348 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v3.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7267 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v3.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v3.2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      920 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v3.2.2.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    14923 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      824 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.0.2.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7851 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8800 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.2.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6985 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.3.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2638 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.4.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      248 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.4.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      755 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.4.2.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.4.3.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7147 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.5.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.5.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.5.2.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v4.5.3.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    13114 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v5.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      279 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v5.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v5.0.2.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7840 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v5.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v5.1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5573 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v6.0.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      202 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v6.0.1.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v6.0.2.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v6.0.3.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v6.0.4.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3691 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v6.1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5100 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v6.2.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4223 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases/v6.3.0.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/releases.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/routing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/tcpclient.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      171 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/tcpserver.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      546 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/template.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      690 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7101 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/tornado.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2253 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/twisted.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      619 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/util.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    15055 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/web.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/webframework.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/websocket.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-04-09 20:54:12.000000 tornado-6.3b1/docs/wsgi.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-04-09 20:54:12.000000 tornado-6.3b1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (122)      511 2023-04-09 20:54:12.000000 tornado-6.3b1/runtests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-09 20:54:13.769427 tornado-6.3b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4077 2023-04-09 20:54:12.000000 tornado-6.3b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.753426 tornado-6.3b1/tornado/
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4503 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/_locale_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46806 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13585 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24660 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/curl_httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13266 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/escape.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31447 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/gen.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36191 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/http1connection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31919 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16126 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/httpserver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36001 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/httputil.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35832 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/ioloop.py
+-rw-r--r--   0 runner    (1001) docker     (122)    65497 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/iostream.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20890 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/locale.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17356 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/locks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12549 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25303 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/netutil.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26254 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/options.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.757426 tornado-6.3b1/tornado/platform/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25088 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/platform/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3500 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/platform/caresresolver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5624 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/platform/twisted.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12789 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/process.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    12530 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/queues.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25082 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/routing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27796 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/simple_httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/speedups.c
+-rw-r--r--   0 runner    (1001) docker     (122)    12152 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/tcpclient.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15022 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/tcpserver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37793 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/template.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.765426 tornado-6.3b1/tornado/test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      335 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8345 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/asyncio_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23418 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/auth_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3948 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/autoreload_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6049 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/concurrent_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.765426 tornado-6.3b1/tornado/test/csv_translations/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/csv_translations/fr_FR.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     4303 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/curl_httpclient_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12295 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/escape_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34093 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/gen_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.737425 tornado-6.3b1/tornado/test/gettext_translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.737425 tornado-6.3b1/tornado/test/gettext_translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.765426 tornado-6.3b1/tornado/test/gettext_translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/gettext_translations/fr_FR/LC_MESSAGES/tornado_test.mo
+-rw-r--r--   0 runner    (1001) docker     (122)     1049 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/gettext_translations/fr_FR/LC_MESSAGES/tornado_test.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1964 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/http1connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34788 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/httpclient_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47084 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/httpserver_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19045 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/httputil_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2231 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/import_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27405 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/ioloop_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47311 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/iostream_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5724 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/locale_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17010 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/locks_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9473 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/log_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8334 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/netutil_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/options_test.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)    11932 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/options_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      296 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/options_test_types.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/options_test_types_str.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)    11308 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/process_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13981 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/queues_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      410 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/resolve_test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8827 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/routing_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8348 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31109 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/simple_httpclient_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.769427 tornado-6.3b1/tornado/test/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.769427 tornado-6.3b1/tornado/test/static/dir/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/static/dir/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/static/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/static/sample.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/static/sample.xml.bz2
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/static/sample.xml.gz
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/static_foo.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    16847 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/tcpclient_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7720 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/tcpserver_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18657 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/template_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.769427 tornado-6.3b1/tornado/test/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/templates/utf8.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1224 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/test.crt
+-rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/test.key
+-rw-r--r--   0 runner    (1001) docker     (122)    10317 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/testing_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1732 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/twisted_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3654 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9771 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/util_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)   119034 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/web_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28703 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/websocket_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3918 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/test/wsgi_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33341 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/testing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16249 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)   141587 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/web.py
+-rw-r--r--   0 runner    (1001) docker     (122)    61175 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10817 2023-04-09 20:54:12.000000 tornado-6.3b1/tornado/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-09 20:54:13.757426 tornado-6.3b1/tornado.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-04-09 20:54:13.000000 tornado-6.3b1/tornado.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5949 2023-04-09 20:54:13.000000 tornado-6.3b1/tornado.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-09 20:54:13.000000 tornado-6.3b1/tornado.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-09 20:54:13.000000 tornado-6.3b1/tornado.egg-info/top_level.txt
```

### Comparing `tornado-6.2b2/LICENSE` & `tornado-6.3b1/LICENSE`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/MANIFEST.in` & `tornado-6.3b1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/PKG-INFO` & `tornado-6.3b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: tornado
-Version: 6.2b2
+Version: 6.3b1
 Summary: Tornado is a Python web framework and asynchronous networking library, originally developed at FriendFeed.
 Home-page: http://www.tornadoweb.org/
 Author: Facebook
 Author-email: python-tornado@googlegroups.com
-License: http://www.apache.org/licenses/LICENSE-2.0
+License: Apache-2.0
 Project-URL: Source, https://github.com/tornadoweb/tornado
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >= 3.7
+Requires-Python: >= 3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Tornado Web Server
 ==================
 
 .. image:: https://badges.gitter.im/Join%20Chat.svg
@@ -39,16 +39,15 @@
 ------------
 
 Here is a simple "Hello, world" example web app for Tornado:
 
 .. code-block:: python
 
     import asyncio
-
-    import tornado.web
+    import tornado
 
     class MainHandler(tornado.web.RequestHandler):
         def get(self):
             self.write("Hello, world")
 
     def make_app():
         return tornado.web.Application([
```

### Comparing `tornado-6.2b2/README.rst` & `tornado-6.3b1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 ------------
 
 Here is a simple "Hello, world" example web app for Tornado:
 
 .. code-block:: python
 
     import asyncio
-
-    import tornado.web
+    import tornado
 
     class MainHandler(tornado.web.RequestHandler):
         def get(self):
             self.write("Hello, world")
 
     def make_app():
         return tornado.web.Application([
```

### Comparing `tornado-6.2b2/demos/blog/README` & `tornado-6.3b1/demos/blog/README`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/demos/blog/blog.py` & `tornado-6.3b1/demos/blog/blog.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,20 +17,15 @@
 import aiopg
 import asyncio
 import bcrypt
 import markdown
 import os.path
 import psycopg2
 import re
-import tornado.escape
-import tornado.httpserver
-import tornado.ioloop
-import tornado.locks
-import tornado.options
-import tornado.web
+import tornado
 import unicodedata
 
 from tornado.options import define, options
 
 define("port", default=8888, help="run on the given port", type=int)
 define("db_host", default="127.0.0.1", help="blog database host")
 define("db_port", default=5432, help="blog database port")
@@ -124,15 +119,15 @@
         elif len(results) > 1:
             raise ValueError("Expected 1 result, got %d" % len(results))
         return results[0]
 
     async def prepare(self):
         # get_current_user cannot be a coroutine, so set
         # self.current_user in prepare instead.
-        user_id = self.get_secure_cookie("blogdemo_user")
+        user_id = self.get_signed_cookie("blogdemo_user")
         if user_id:
             self.current_user = await self.queryone(
                 "SELECT * FROM authors WHERE id = %s", int(user_id)
             )
 
     async def any_author_exists(self):
         return bool(await self.query("SELECT * FROM authors LIMIT 1"))
@@ -243,15 +238,15 @@
         author = await self.queryone(
             "INSERT INTO authors (email, name, hashed_password) "
             "VALUES (%s, %s, %s) RETURNING id",
             self.get_argument("email"),
             self.get_argument("name"),
             tornado.escape.to_unicode(hashed_password),
         )
-        self.set_secure_cookie("blogdemo_user", str(author.id))
+        self.set_signed_cookie("blogdemo_user", str(author.id))
         self.redirect(self.get_argument("next", "/"))
 
 
 class AuthLoginHandler(BaseHandler):
     async def get(self):
         # If there are no authors, redirect to the account creation page.
         if not await self.any_author_exists():
@@ -270,15 +265,15 @@
         password_equal = await tornado.ioloop.IOLoop.current().run_in_executor(
             None,
             bcrypt.checkpw,
             tornado.escape.utf8(self.get_argument("password")),
             tornado.escape.utf8(author.hashed_password),
         )
         if password_equal:
-            self.set_secure_cookie("blogdemo_user", str(author.id))
+            self.set_signed_cookie("blogdemo_user", str(author.id))
             self.redirect(self.get_argument("next", "/"))
         else:
             self.render("login.html", error="incorrect password")
 
 
 class AuthLogoutHandler(BaseHandler):
     def get(self):
```

### Comparing `tornado-6.2b2/demos/blog/schema.sql` & `tornado-6.3b1/demos/blog/schema.sql`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/demos/blog/static/blog.css` & `tornado-6.3b1/demos/blog/static/blog.css`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/demos/blog/templates/archive.html` & `tornado-6.3b1/demos/blog/templates/archive.html`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/demos/blog/templates/base.html` & `tornado-6.3b1/demos/blog/templates/base.html`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/demos/blog/templates/compose.html` & `tornado-6.3b1/demos/blog/templates/compose.html`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/demos/blog/templates/feed.xml` & `tornado-6.3b1/demos/blog/templates/feed.xml`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/demos/chat/chatdemo.py` & `tornado-6.3b1/demos/chat/chatdemo.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import asyncio
-import tornado.escape
-import tornado.locks
-import tornado.web
+import tornado
 import os.path
 import uuid
 
 from tornado.options import define, options, parse_command_line
 
 define("port", default=8888, help="run on the given port", type=int)
 define("debug", default=True, help="run in debug mode")
```

### Comparing `tornado-6.2b2/demos/chat/static/chat.css` & `tornado-6.3b1/demos/chat/static/chat.css`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/demos/chat/static/chat.js` & `tornado-6.3b1/demos/chat/static/chat.js`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/demos/chat/templates/index.html` & `tornado-6.3b1/demos/chat/templates/index.html`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/demos/facebook/facebook.py` & `tornado-6.3b1/demos/facebook/facebook.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import asyncio
 import os.path
-import tornado.auth
-import tornado.escape
-import tornado.httpserver
-import tornado.options
-import tornado.web
+import tornado
 
 from tornado.options import define, options
 
 define("port", default=8888, help="run on the given port", type=int)
 define("facebook_api_key", help="your Facebook application API key", type=str)
 define("facebook_secret", help="your Facebook application secret", type=str)
 
@@ -49,15 +45,15 @@
             autoescape=None,
         )
         tornado.web.Application.__init__(self, handlers, **settings)
 
 
 class BaseHandler(tornado.web.RequestHandler):
     def get_current_user(self):
-        user_json = self.get_secure_cookie("fbdemo_user")
+        user_json = self.get_signed_cookie("fbdemo_user")
         if not user_json:
             return None
         return tornado.escape.json_decode(user_json)
 
 
 class MainHandler(BaseHandler, tornado.auth.FacebookGraphMixin):
     @tornado.web.authenticated
@@ -84,15 +80,15 @@
         if self.get_argument("code", False):
             user = await self.get_authenticated_user(
                 redirect_uri=my_url,
                 client_id=self.settings["facebook_api_key"],
                 client_secret=self.settings["facebook_secret"],
                 code=self.get_argument("code"),
             )
-            self.set_secure_cookie("fbdemo_user", tornado.escape.json_encode(user))
+            self.set_signed_cookie("fbdemo_user", tornado.escape.json_encode(user))
             self.redirect(self.get_argument("next", "/"))
             return
         self.authorize_redirect(
             redirect_uri=my_url,
             client_id=self.settings["facebook_api_key"],
             extra_params={"scope": "user_posts"},
         )
```

### Comparing `tornado-6.2b2/demos/facebook/static/facebook.css` & `tornado-6.3b1/demos/facebook/static/facebook.css`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/demos/facebook/templates/modules/post.html` & `tornado-6.3b1/demos/facebook/templates/modules/post.html`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/demos/facebook/templates/stream.html` & `tornado-6.3b1/demos/facebook/templates/stream.html`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/demos/file_upload/file_receiver.py` & `tornado-6.3b1/demos/file_upload/file_receiver.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 See file_uploader.py in this directory for code that uploads files in this format.
 """
 
 import asyncio
 import logging
 from urllib.parse import unquote
 
-import tornado.web
+import tornado
 from tornado import options
 
 
 class POSTHandler(tornado.web.RequestHandler):
     def post(self):
         for field_name, files in self.request.files.items():
             for info in files:
```

### Comparing `tornado-6.2b2/demos/file_upload/file_uploader.py` & `tornado-6.3b1/demos/file_upload/file_uploader.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/demos/helloworld/helloworld.py` & `tornado-6.3b1/demos/helloworld/helloworld.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import asyncio
-import tornado.httpserver
-import tornado.options
-import tornado.web
+import tornado
 
 from tornado.options import define, options
 
 define("port", default=8888, help="run on the given port", type=int)
 
 
 class MainHandler(tornado.web.RequestHandler):
```

### Comparing `tornado-6.2b2/demos/s3server/s3server.py` & `tornado-6.3b1/demos/s3server/s3server.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,16 +142,16 @@
                 }
             )
         self.render_xml({"ListAllMyBucketsResult": {"Buckets": {"Bucket": buckets}}})
 
 
 class BucketHandler(BaseRequestHandler):
     def get(self, bucket_name):
-        prefix = self.get_argument("prefix", u"")
-        marker = self.get_argument("marker", u"")
+        prefix = self.get_argument("prefix", "")
+        marker = self.get_argument("marker", "")
         max_keys = int(self.get_argument("max-keys", 50000))
         path = os.path.abspath(os.path.join(self.application.directory, bucket_name))
         terse = int(self.get_argument("terse", 0))
         if not path.startswith(self.application.directory) or not os.path.isdir(path):
             raise web.HTTPError(404)
         object_names = []
         for root, dirs, files in os.walk(path):
```

### Comparing `tornado-6.2b2/demos/tcpecho/client.py` & `tornado-6.3b1/demos/tcpecho/client.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/demos/tcpecho/server.py` & `tornado-6.3b1/demos/tcpecho/server.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/demos/twitter/twitterdemo.py` & `tornado-6.3b1/demos/twitter/twitterdemo.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 )
 
 
 class BaseHandler(RequestHandler):
     COOKIE_NAME = "twitterdemo_user"
 
     def get_current_user(self):
-        user_json = self.get_secure_cookie(self.COOKIE_NAME)
+        user_json = self.get_signed_cookie(self.COOKIE_NAME)
         if not user_json:
             return None
         return json_decode(user_json)
 
 
 class MainHandler(BaseHandler, TwitterMixin):
     @authenticated
@@ -71,15 +71,15 @@
 
 class LoginHandler(BaseHandler, TwitterMixin):
     @gen.coroutine
     def get(self):
         if self.get_argument("oauth_token", None):
             user = yield self.get_authenticated_user()
             del user["description"]
-            self.set_secure_cookie(self.COOKIE_NAME, json_encode(user))
+            self.set_signed_cookie(self.COOKIE_NAME, json_encode(user))
             self.redirect(self.get_argument("next", "/"))
         else:
             yield self.authorize_redirect(callback_uri=self.request.full_url())
 
 
 class LogoutHandler(BaseHandler):
     def get(self):
```

### Comparing `tornado-6.2b2/demos/websocket/chatdemo.py` & `tornado-6.3b1/demos/websocket/chatdemo.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,15 @@
 """Simplified chat demo for websockets.
 
 Authentication, error handling, etc are left as an exercise for the reader :)
 """
 
 import asyncio
 import logging
-import tornado.escape
-import tornado.options
-import tornado.web
-import tornado.websocket
+import tornado
 import os.path
 import uuid
 
 from tornado.options import define, options
 
 define("port", default=8888, help="run on the given port", type=int)
```

### Comparing `tornado-6.2b2/demos/websocket/static/chat.css` & `tornado-6.3b1/demos/websocket/static/chat.css`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/demos/websocket/static/chat.js` & `tornado-6.3b1/demos/websocket/static/chat.js`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/demos/websocket/templates/index.html` & `tornado-6.3b1/demos/websocket/templates/index.html`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/demos/webspider/webspider.py` & `tornado-6.3b1/demos/webspider/webspider.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     await q.put(base_url)
 
     # Start workers, then wait for the work queue to be empty.
     workers = gen.multi([worker() for _ in range(concurrency)])
     await q.join(timeout=timedelta(seconds=300))
     assert fetching == (fetched | dead)
     print("Done in %d seconds, fetched %s URLs." % (time.time() - start, len(fetched)))
-    print("Unable to fetch %s URLS." % len(dead))
+    print("Unable to fetch %s URLs." % len(dead))
 
     # Signal all the workers to exit.
     for _ in range(concurrency):
         await q.put(None)
     await workers
```

### Comparing `tornado-6.2b2/docs/Makefile` & `tornado-6.3b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/auth.rst` & `tornado-6.3b1/docs/auth.rst`

 * *Files 7% similar despite different names*

```diff
@@ -3,71 +3,69 @@
 00000020: 206c 6f67 696e 2077 6974 6820 4f70 656e   login with Open
 00000030: 4944 2061 6e64 204f 4175 7468 0a3d 3d3d  ID and OAuth.===
 00000040: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00000050: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00000060: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00000070: 3d3d 3d3d 3d3d 3d3d 3d0a 0a2e 2e20 7465  =========.... te
 00000080: 7374 7365 7475 703a 3a0a 0a20 2020 696d  stsetup::..   im
-00000090: 706f 7274 2074 6f72 6e61 646f 2e61 7574  port tornado.aut
-000000a0: 682c 2074 6f72 6e61 646f 2e67 656e 2c20  h, tornado.gen, 
-000000b0: 746f 726e 6164 6f2e 7765 620a 0a2e 2e20  tornado.web.... 
-000000c0: 6175 746f 6d6f 6475 6c65 3a3a 2074 6f72  automodule:: tor
-000000d0: 6e61 646f 2e61 7574 680a 0a20 2020 436f  nado.auth..   Co
-000000e0: 6d6d 6f6e 2070 726f 746f 636f 6c73 0a20  mmon protocols. 
-000000f0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-00000100: 2d2d 0a0a 2020 2054 6865 7365 2063 6c61  --..   These cla
-00000110: 7373 6573 2069 6d70 6c65 6d65 6e74 2074  sses implement t
-00000120: 6865 204f 7065 6e49 4420 616e 6420 4f41  he OpenID and OA
-00000130: 7574 6820 7374 616e 6461 7264 732e 2020  uth standards.  
-00000140: 5468 6579 2077 696c 6c0a 2020 2067 656e  They will.   gen
-00000150: 6572 616c 6c79 206e 6565 6420 746f 2062  erally need to b
-00000160: 6520 7375 6263 6c61 7373 6564 2074 6f20  e subclassed to 
-00000170: 7573 6520 7468 656d 2077 6974 6820 616e  use them with an
-00000180: 7920 7061 7274 6963 756c 6172 2073 6974  y particular sit
-00000190: 652e 0a20 2020 5468 6520 6465 6772 6565  e..   The degree
-000001a0: 206f 6620 6375 7374 6f6d 697a 6174 696f   of customizatio
-000001b0: 6e20 7265 7175 6972 6564 2077 696c 6c20  n required will 
-000001c0: 7661 7279 2c20 6275 7420 696e 206d 6f73  vary, but in mos
-000001d0: 7420 6361 7365 730a 2020 206f 7665 7272  t cases.   overr
-000001e0: 6964 696e 6720 7468 6520 636c 6173 7320  iding the class 
-000001f0: 6174 7472 6962 7574 6573 2028 7768 6963  attributes (whic
-00000200: 6820 6172 6520 6e61 6d65 6420 6265 6769  h are named begi
-00000210: 6e6e 696e 6720 7769 7468 0a20 2020 756e  nning with.   un
-00000220: 6465 7273 636f 7265 7320 666f 7220 6869  derscores for hi
-00000230: 7374 6f72 6963 616c 2072 6561 736f 6e73  storical reasons
-00000240: 2920 7368 6f75 6c64 2062 6520 7375 6666  ) should be suff
-00000250: 6963 6965 6e74 2e0a 0a20 2020 2e2e 2061  icient...   .. a
-00000260: 7574 6f63 6c61 7373 3a3a 204f 7065 6e49  utoclass:: OpenI
-00000270: 644d 6978 696e 0a20 2020 2020 203a 6d65  dMixin.      :me
-00000280: 6d62 6572 733a 0a0a 2020 202e 2e20 6175  mbers:..   .. au
-00000290: 746f 636c 6173 733a 3a20 4f41 7574 684d  toclass:: OAuthM
-000002a0: 6978 696e 0a0a 2020 2020 2020 2e2e 2061  ixin..      .. a
-000002b0: 7574 6f6d 6574 686f 643a 3a20 6175 7468  utomethod:: auth
-000002c0: 6f72 697a 655f 7265 6469 7265 6374 0a20  orize_redirect. 
-000002d0: 2020 2020 202e 2e20 6175 746f 6d65 7468       .. autometh
-000002e0: 6f64 3a3a 2067 6574 5f61 7574 6865 6e74  od:: get_authent
-000002f0: 6963 6174 6564 5f75 7365 720a 2020 2020  icated_user.    
-00000300: 2020 2e2e 2061 7574 6f6d 6574 686f 643a    .. automethod:
-00000310: 3a20 5f6f 6175 7468 5f63 6f6e 7375 6d65  : _oauth_consume
-00000320: 725f 746f 6b65 6e0a 2020 2020 2020 2e2e  r_token.      ..
-00000330: 2061 7574 6f6d 6574 686f 643a 3a20 5f6f   automethod:: _o
-00000340: 6175 7468 5f67 6574 5f75 7365 725f 6675  auth_get_user_fu
-00000350: 7475 7265 0a20 2020 2020 202e 2e20 6175  ture.      .. au
-00000360: 746f 6d65 7468 6f64 3a3a 2067 6574 5f61  tomethod:: get_a
-00000370: 7574 685f 6874 7470 5f63 6c69 656e 740a  uth_http_client.
-00000380: 0a20 2020 2e2e 2061 7574 6f63 6c61 7373  .   .. autoclass
-00000390: 3a3a 204f 4175 7468 324d 6978 696e 0a20  :: OAuth2Mixin. 
-000003a0: 2020 2020 203a 6d65 6d62 6572 733a 0a0a       :members:..
-000003b0: 2020 2047 6f6f 676c 650a 2020 202d 2d2d     Google.   ---
-000003c0: 2d2d 2d0a 0a20 2020 2e2e 2061 7574 6f63  ---..   .. autoc
-000003d0: 6c61 7373 3a3a 2047 6f6f 676c 654f 4175  lass:: GoogleOAu
-000003e0: 7468 324d 6978 696e 0a20 2020 2020 203a  th2Mixin.      :
-000003f0: 6d65 6d62 6572 733a 0a0a 2020 2046 6163  members:..   Fac
-00000400: 6562 6f6f 6b0a 2020 202d 2d2d 2d2d 2d2d  ebook.   -------
-00000410: 2d0a 0a20 2020 2e2e 2061 7574 6f63 6c61  -..   .. autocla
-00000420: 7373 3a3a 2046 6163 6562 6f6f 6b47 7261  ss:: FacebookGra
-00000430: 7068 4d69 7869 6e0a 2020 2020 2020 3a6d  phMixin.      :m
-00000440: 656d 6265 7273 3a0a 0a20 2020 5477 6974  embers:..   Twit
-00000450: 7465 720a 2020 202d 2d2d 2d2d 2d2d 0a0a  ter.   -------..
-00000460: 2020 202e 2e20 6175 746f 636c 6173 733a     .. autoclass:
-00000470: 3a20 5477 6974 7465 724d 6978 696e 0a20  : TwitterMixin. 
-00000480: 2020 2020 203a 6d65 6d62 6572 733a 0a         :members:.
+00000090: 706f 7274 2074 6f72 6e61 646f 0a0a 2e2e  port tornado....
+000000a0: 2061 7574 6f6d 6f64 756c 653a 3a20 746f   automodule:: to
+000000b0: 726e 6164 6f2e 6175 7468 0a0a 2020 2043  rnado.auth..   C
+000000c0: 6f6d 6d6f 6e20 7072 6f74 6f63 6f6c 730a  ommon protocols.
+000000d0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+000000e0: 2d2d 2d0a 0a20 2020 5468 6573 6520 636c  ---..   These cl
+000000f0: 6173 7365 7320 696d 706c 656d 656e 7420  asses implement 
+00000100: 7468 6520 4f70 656e 4944 2061 6e64 204f  the OpenID and O
+00000110: 4175 7468 2073 7461 6e64 6172 6473 2e20  Auth standards. 
+00000120: 2054 6865 7920 7769 6c6c 0a20 2020 6765   They will.   ge
+00000130: 6e65 7261 6c6c 7920 6e65 6564 2074 6f20  nerally need to 
+00000140: 6265 2073 7562 636c 6173 7365 6420 746f  be subclassed to
+00000150: 2075 7365 2074 6865 6d20 7769 7468 2061   use them with a
+00000160: 6e79 2070 6172 7469 6375 6c61 7220 7369  ny particular si
+00000170: 7465 2e0a 2020 2054 6865 2064 6567 7265  te..   The degre
+00000180: 6520 6f66 2063 7573 746f 6d69 7a61 7469  e of customizati
+00000190: 6f6e 2072 6571 7569 7265 6420 7769 6c6c  on required will
+000001a0: 2076 6172 792c 2062 7574 2069 6e20 6d6f   vary, but in mo
+000001b0: 7374 2063 6173 6573 0a20 2020 6f76 6572  st cases.   over
+000001c0: 7269 6469 6e67 2074 6865 2063 6c61 7373  riding the class
+000001d0: 2061 7474 7269 6275 7465 7320 2877 6869   attributes (whi
+000001e0: 6368 2061 7265 206e 616d 6564 2062 6567  ch are named beg
+000001f0: 696e 6e69 6e67 2077 6974 680a 2020 2075  inning with.   u
+00000200: 6e64 6572 7363 6f72 6573 2066 6f72 2068  nderscores for h
+00000210: 6973 746f 7269 6361 6c20 7265 6173 6f6e  istorical reason
+00000220: 7329 2073 686f 756c 6420 6265 2073 7566  s) should be suf
+00000230: 6669 6369 656e 742e 0a0a 2020 202e 2e20  ficient...   .. 
+00000240: 6175 746f 636c 6173 733a 3a20 4f70 656e  autoclass:: Open
+00000250: 4964 4d69 7869 6e0a 2020 2020 2020 3a6d  IdMixin.      :m
+00000260: 656d 6265 7273 3a0a 0a20 2020 2e2e 2061  embers:..   .. a
+00000270: 7574 6f63 6c61 7373 3a3a 204f 4175 7468  utoclass:: OAuth
+00000280: 4d69 7869 6e0a 0a20 2020 2020 202e 2e20  Mixin..      .. 
+00000290: 6175 746f 6d65 7468 6f64 3a3a 2061 7574  automethod:: aut
+000002a0: 686f 7269 7a65 5f72 6564 6972 6563 740a  horize_redirect.
+000002b0: 2020 2020 2020 2e2e 2061 7574 6f6d 6574        .. automet
+000002c0: 686f 643a 3a20 6765 745f 6175 7468 656e  hod:: get_authen
+000002d0: 7469 6361 7465 645f 7573 6572 0a20 2020  ticated_user.   
+000002e0: 2020 202e 2e20 6175 746f 6d65 7468 6f64     .. automethod
+000002f0: 3a3a 205f 6f61 7574 685f 636f 6e73 756d  :: _oauth_consum
+00000300: 6572 5f74 6f6b 656e 0a20 2020 2020 202e  er_token.      .
+00000310: 2e20 6175 746f 6d65 7468 6f64 3a3a 205f  . automethod:: _
+00000320: 6f61 7574 685f 6765 745f 7573 6572 5f66  oauth_get_user_f
+00000330: 7574 7572 650a 2020 2020 2020 2e2e 2061  uture.      .. a
+00000340: 7574 6f6d 6574 686f 643a 3a20 6765 745f  utomethod:: get_
+00000350: 6175 7468 5f68 7474 705f 636c 6965 6e74  auth_http_client
+00000360: 0a0a 2020 202e 2e20 6175 746f 636c 6173  ..   .. autoclas
+00000370: 733a 3a20 4f41 7574 6832 4d69 7869 6e0a  s:: OAuth2Mixin.
+00000380: 2020 2020 2020 3a6d 656d 6265 7273 3a0a        :members:.
+00000390: 0a20 2020 476f 6f67 6c65 0a20 2020 2d2d  .   Google.   --
+000003a0: 2d2d 2d2d 0a0a 2020 202e 2e20 6175 746f  ----..   .. auto
+000003b0: 636c 6173 733a 3a20 476f 6f67 6c65 4f41  class:: GoogleOA
+000003c0: 7574 6832 4d69 7869 6e0a 2020 2020 2020  uth2Mixin.      
+000003d0: 3a6d 656d 6265 7273 3a0a 0a20 2020 4661  :members:..   Fa
+000003e0: 6365 626f 6f6b 0a20 2020 2d2d 2d2d 2d2d  cebook.   ------
+000003f0: 2d2d 0a0a 2020 202e 2e20 6175 746f 636c  --..   .. autocl
+00000400: 6173 733a 3a20 4661 6365 626f 6f6b 4772  ass:: FacebookGr
+00000410: 6170 684d 6978 696e 0a20 2020 2020 203a  aphMixin.      :
+00000420: 6d65 6d62 6572 733a 0a0a 2020 2054 7769  members:..   Twi
+00000430: 7474 6572 0a20 2020 2d2d 2d2d 2d2d 2d0a  tter.   -------.
+00000440: 0a20 2020 2e2e 2061 7574 6f63 6c61 7373  .   .. autoclass
+00000450: 3a3a 2054 7769 7474 6572 4d69 7869 6e0a  :: TwitterMixin.
+00000460: 2020 2020 2020 3a6d 656d 6265 7273 3a0a        :members:.
```

### Comparing `tornado-6.2b2/docs/caresresolver.rst` & `tornado-6.3b1/docs/caresresolver.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/concurrent.rst` & `tornado-6.3b1/docs/concurrent.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/conf.py` & `tornado-6.3b1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,15 @@
     "Rule",
     "socket.AddressFamily",
     "tornado.concurrent._T",
     "tornado.gen._T",
     "tornado.ioloop._S",
     "tornado.ioloop._T",
     "tornado.ioloop._Selectable",
+    "tornado.iostream._IOStreamType",
     "tornado.locks._ReleasingContextManager",
     "tornado.queues._T",
     "tornado.options._Mockable",
     "tornado.web._ArgDefaultMarker",
     "tornado.web._HandlerDelegate",
     "tornado.web._RequestHandlerType",
     "_RequestHandlerType",
```

### Comparing `tornado-6.2b2/docs/escape.rst` & `tornado-6.3b1/docs/escape.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/faq.rst` & `tornado-6.3b1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/favicon.ico` & `tornado-6.3b1/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/gen.rst` & `tornado-6.3b1/docs/gen.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/guide/async.rst` & `tornado-6.3b1/docs/guide/async.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/guide/coroutines.rst` & `tornado-6.3b1/docs/guide/coroutines.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/guide/intro.rst` & `tornado-6.3b1/docs/guide/intro.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/guide/queues.rst` & `tornado-6.3b1/docs/guide/queues.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/guide/running.rst` & `tornado-6.3b1/docs/guide/running.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/guide/security.rst` & `tornado-6.3b1/docs/guide/security.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Authentication and security
 ===========================
 
 .. testsetup::
 
-   import tornado.auth
-   import tornado.web
+   import tornado
 
-Cookies and secure cookies
+Cookies and signed cookies
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 You can set cookies in the user's browser with the ``set_cookie``
 method:
 
 .. testcode::
 
@@ -24,16 +23,16 @@
 
 .. testoutput::
    :hide:
 
 Cookies are not secure and can easily be modified by clients.  If you
 need to set cookies to, e.g., identify the currently logged in user,
 you need to sign your cookies to prevent forgery. Tornado supports
-signed cookies with the `~.RequestHandler.set_secure_cookie` and
-`~.RequestHandler.get_secure_cookie` methods. To use these methods,
+signed cookies with the `~.RequestHandler.set_signed_cookie` and
+`~.RequestHandler.get_signed_cookie` methods. To use these methods,
 you need to specify a secret key named ``cookie_secret`` when you
 create your application. You can pass in application settings as
 keyword arguments to your application:
 
 .. testcode::
 
     application = tornado.web.Application([
@@ -42,51 +41,51 @@
 
 .. testoutput::
    :hide:
 
 Signed cookies contain the encoded value of the cookie in addition to a
 timestamp and an `HMAC <http://en.wikipedia.org/wiki/HMAC>`_ signature.
 If the cookie is old or if the signature doesn't match,
-``get_secure_cookie`` will return ``None`` just as if the cookie isn't
+``get_signed_cookie`` will return ``None`` just as if the cookie isn't
 set. The secure version of the example above:
 
 .. testcode::
 
     class MainHandler(tornado.web.RequestHandler):
         def get(self):
-            if not self.get_secure_cookie("mycookie"):
-                self.set_secure_cookie("mycookie", "myvalue")
+            if not self.get_signed_cookie("mycookie"):
+                self.set_signed_cookie("mycookie", "myvalue")
                 self.write("Your cookie was not set yet!")
             else:
                 self.write("Your cookie was set!")
 
 .. testoutput::
    :hide:
 
-Tornado's secure cookies guarantee integrity but not confidentiality.
+Tornado's signed cookies guarantee integrity but not confidentiality.
 That is, the cookie cannot be modified but its contents can be seen by the
 user.  The ``cookie_secret`` is a symmetric key and must be kept secret --
 anyone who obtains the value of this key could produce their own signed
 cookies.
 
-By default, Tornado's secure cookies expire after 30 days.  To change this,
-use the ``expires_days`` keyword argument to ``set_secure_cookie`` *and* the
-``max_age_days`` argument to ``get_secure_cookie``.  These two values are
+By default, Tornado's signed cookies expire after 30 days.  To change this,
+use the ``expires_days`` keyword argument to ``set_signed_cookie`` *and* the
+``max_age_days`` argument to ``get_signed_cookie``.  These two values are
 passed separately so that you may e.g. have a cookie that is valid for 30 days
 for most purposes, but for certain sensitive actions (such as changing billing
 information) you use a smaller ``max_age_days`` when reading the cookie.
 
 Tornado also supports multiple signing keys to enable signing key
 rotation. ``cookie_secret`` then must be a dict with integer key versions
 as keys and the corresponding secrets as values. The currently used
 signing key must then be set as ``key_version`` application setting
 but all other keys in the dict are allowed for cookie signature validation,
 if the correct key version is set in the cookie.
 To implement cookie updates, the current signing key version can be
-queried via `~.RequestHandler.get_secure_cookie_key_version`.
+queried via `~.RequestHandler.get_signed_cookie_key_version`.
 
 .. _user-authentication:
 
 User authentication
 ~~~~~~~~~~~~~~~~~~~
 
 The currently authenticated user is available in every request handler
@@ -100,15 +99,15 @@
 is an example that lets users log into the application simply by
 specifying a nickname, which is then saved in a cookie:
 
 .. testcode::
 
     class BaseHandler(tornado.web.RequestHandler):
         def get_current_user(self):
-            return self.get_secure_cookie("user")
+            return self.get_signed_cookie("user")
 
     class MainHandler(BaseHandler):
         def get(self):
             if not self.current_user:
                 self.redirect("/login")
                 return
             name = tornado.escape.xhtml_escape(self.current_user)
@@ -118,15 +117,15 @@
         def get(self):
             self.write('<html><body><form action="/login" method="post">'
                        'Name: <input type="text" name="name">'
                        '<input type="submit" value="Sign in">'
                        '</form></body></html>')
 
         def post(self):
-            self.set_secure_cookie("user", self.get_argument("name"))
+            self.set_signed_cookie("user", self.get_argument("name"))
             self.redirect("/")
 
     application = tornado.web.Application([
         (r"/", MainHandler),
         (r"/login", LoginHandler),
     ], cookie_secret="__TODO:_GENERATE_YOUR_OWN_RANDOM_VALUE_HERE__")
 
@@ -190,15 +189,15 @@
     class GoogleOAuth2LoginHandler(tornado.web.RequestHandler,
                                    tornado.auth.GoogleOAuth2Mixin):
         async def get(self):
             if self.get_argument('code', False):
                 user = await self.get_authenticated_user(
                     redirect_uri='http://your.site.com/auth/google',
                     code=self.get_argument('code'))
-                # Save the user with e.g. set_secure_cookie
+                # Save the user with e.g. set_signed_cookie
             else:
                 await self.authorize_redirect(
                     redirect_uri='http://your.site.com/auth/google',
                     client_id=self.settings['google_oauth']['key'],
                     scope=['profile', 'email'],
                     response_type='code',
                     extra_params={'approval_prompt': 'auto'})
```

### Comparing `tornado-6.2b2/docs/guide/structure.rst` & `tornado-6.3b1/docs/guide/structure.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 .. currentmodule:: tornado.web
 
 .. testsetup::
 
-   import tornado.web
+   import tornado
 
 Structure of a Tornado web application
 ======================================
 
 A Tornado web application generally consists of one or more
 `.RequestHandler` subclasses, an `.Application` object which
 routes incoming requests to handlers, and a ``main()`` function
 to start the server.
 
 A minimal "hello world" example looks something like this:
 
 .. testcode::
 
     import asyncio
-
-    import tornado.web
+    import tornado
 
     class MainHandler(tornado.web.RequestHandler):
         def get(self):
             self.write("Hello, world")
 
     def make_app():
         return tornado.web.Application([
@@ -173,15 +172,15 @@
 (i.e. a ``multipart/form-data`` Content-Type); if this format was not used
 the raw uploaded data is available in ``self.request.body``.
 By default uploaded files are fully buffered in memory; if you need to
 handle files that are too large to comfortably keep in memory see the
 `.stream_request_body` class decorator.
 
 In the demos directory,
-`file_receiver.py <https://github.com/tornadoweb/tornado/tree/master/demos/file_upload/>`_
+`file_receiver.py <https://github.com/tornadoweb/tornado/tree/stable/demos/file_upload/>`_
 shows both methods of receiving file uploads.
 
 Due to the quirks of the HTML form encoding (e.g. the ambiguity around
 singular versus plural arguments), Tornado does not attempt to unify
 form arguments with other types of input.  In particular, we do not
 parse JSON request bodies.  Applications that wish to use JSON instead
 of form-encoding may override `~.RequestHandler.prepare` to parse their
```

### Comparing `tornado-6.2b2/docs/guide/templates.rst` & `tornado-6.3b1/docs/guide/templates.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Templates and UI
 ================
 
 .. testsetup::
 
-   import tornado.web
+   import tornado
 
 Tornado includes a simple, fast, and flexible templating language.
 This section describes that language as well as related issues
 such as internationalization.
 
 Tornado can also be used with any other Python template language,
 although there is no provision for integrating these systems into
@@ -188,15 +188,15 @@
 locale as a preference, you can override this default locale selection
 by overriding `.RequestHandler.get_user_locale`:
 
 .. testcode::
 
     class BaseHandler(tornado.web.RequestHandler):
         def get_current_user(self):
-            user_id = self.get_secure_cookie("user")
+            user_id = self.get_signed_cookie("user")
             if not user_id: return None
             return self.backend.get_user_by_id(user_id)
 
         def get_user_locale(self):
             if "locale" not in self.current_user.prefs:
                 # Use the Accept-Language header
                 return None
```

### Comparing `tornado-6.2b2/docs/httpclient.rst` & `tornado-6.3b1/docs/httpclient.rst`

 * *Files 2% similar despite different names*

```diff
@@ -109,23 +109,23 @@
 000006c0: 7465 6420 746f 2074 6869 7320 636c 6965  ted to this clie
 000006d0: 6e74 2e0a 0a45 7861 6d70 6c65 2043 6f64  nt...Example Cod
 000006e0: 650a 7e7e 7e7e 7e7e 7e7e 7e7e 7e7e 0a0a  e.~~~~~~~~~~~~..
 000006f0: 2a20 6041 2073 696d 706c 6520 7765 6273  * `A simple webs
 00000700: 7069 6465 7220 3c68 7474 7073 3a2f 2f67  pider <https://g
 00000710: 6974 6875 622e 636f 6d2f 746f 726e 6164  ithub.com/tornad
 00000720: 6f77 6562 2f74 6f72 6e61 646f 2f62 6c6f  oweb/tornado/blo
-00000730: 622f 6d61 7374 6572 2f64 656d 6f73 2f77  b/master/demos/w
+00000730: 622f 7374 6162 6c65 2f64 656d 6f73 2f77  b/stable/demos/w
 00000740: 6562 7370 6964 6572 2f77 6562 7370 6964  ebspider/webspid
 00000750: 6572 2e70 793e 605f 0a20 2073 686f 7773  er.py>`_.  shows
 00000760: 2068 6f77 2074 6f20 6665 7463 6820 5552   how to fetch UR
 00000770: 4c73 2063 6f6e 6375 7272 656e 746c 792e  Ls concurrently.
 00000780: 0a2a 2060 5468 6520 6669 6c65 2075 706c  .* `The file upl
 00000790: 6f61 6465 7220 6465 6d6f 203c 6874 7470  oader demo <http
 000007a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
 000007b0: 6f72 6e61 646f 7765 622f 746f 726e 6164  ornadoweb/tornad
-000007c0: 6f2f 7472 6565 2f6d 6173 7465 722f 6465  o/tree/master/de
+000007c0: 6f2f 7472 6565 2f73 7461 626c 652f 6465  o/tree/stable/de
 000007d0: 6d6f 732f 6669 6c65 5f75 706c 6f61 642f  mos/file_upload/
 000007e0: 3e60 5f0a 2020 7573 6573 2065 6974 6865  >`_.  uses eithe
 000007f0: 7220 4854 5450 2050 4f53 5420 6f72 2048  r HTTP POST or H
 00000800: 5454 5020 5055 5420 746f 2075 706c 6f61  TTP PUT to uploa
 00000810: 6420 6669 6c65 7320 746f 2061 2073 6572  d files to a ser
 00000820: 7665 722e 0a                             ver..
```

### Comparing `tornado-6.2b2/docs/httpserver.rst` & `tornado-6.3b1/docs/httpserver.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/index.rst` & `tornado-6.3b1/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,15 @@
 
 Hello, world
 ------------
 
 Here is a simple "Hello, world" example web app for Tornado::
 
     import asyncio
-
-    import tornado.web
+    import tornado
 
     class MainHandler(tornado.web.RequestHandler):
         def get(self):
             self.write("Hello, world")
 
     def make_app():
         return tornado.web.Application([
@@ -96,15 +95,15 @@
 Tornado is listed in `PyPI <https://pypi.org/project/tornado/>`_ and
 can be installed with ``pip``. Note that the source distribution
 includes demo applications that are not present when Tornado is
 installed in this way, so you may wish to download a copy of the
 source tarball or clone the `git repository
 <https://github.com/tornadoweb/tornado>`_ as well.
 
-**Prerequisites**: Tornado 6.2 requires Python 3.7 or newer. The following
+**Prerequisites**: Tornado 6.3 requires Python 3.8 or newer. The following
 optional packages may be useful:
 
 * `pycurl <http://pycurl.io/>`_ is used by the optional
   ``tornado.curl_httpclient``.  Libcurl version 7.22 or higher is required.
 * `pycares <https://pypi.org/project/pycares/>`_ is an alternative
   non-blocking DNS resolver that can be used when threads are not
   appropriate.
```

### Comparing `tornado-6.2b2/docs/ioloop.rst` & `tornado-6.3b1/docs/ioloop.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/iostream.rst` & `tornado-6.3b1/docs/iostream.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/locks.rst` & `tornado-6.3b1/docs/locks.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/options.rst` & `tornado-6.3b1/docs/options.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/queues.rst` & `tornado-6.3b1/docs/queues.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v1.0.0.rst` & `tornado-6.3b1/docs/releases/v1.0.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v1.1.0.rst` & `tornado-6.3b1/docs/releases/v1.1.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v1.1.1.rst` & `tornado-6.3b1/docs/releases/v1.1.1.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v1.2.0.rst` & `tornado-6.3b1/docs/releases/v1.2.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v1.2.1.rst` & `tornado-6.3b1/docs/releases/v1.2.1.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v2.0.0.rst` & `tornado-6.3b1/docs/releases/v2.0.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v2.1.0.rst` & `tornado-6.3b1/docs/releases/v2.1.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v2.1.1.rst` & `tornado-6.3b1/docs/releases/v2.1.1.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v2.2.0.rst` & `tornado-6.3b1/docs/releases/v2.2.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v2.2.1.rst` & `tornado-6.3b1/docs/releases/v2.2.1.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v2.3.0.rst` & `tornado-6.3b1/docs/releases/v2.3.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v2.4.0.rst` & `tornado-6.3b1/docs/releases/v2.4.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v3.0.0.rst` & `tornado-6.3b1/docs/releases/v3.0.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v3.0.1.rst` & `tornado-6.3b1/docs/releases/v3.0.1.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v3.1.0.rst` & `tornado-6.3b1/docs/releases/v3.1.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v3.2.0.rst` & `tornado-6.3b1/docs/releases/v3.2.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v3.2.1.rst` & `tornado-6.3b1/docs/releases/v3.2.1.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v3.2.2.rst` & `tornado-6.3b1/docs/releases/v3.2.2.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v4.0.0.rst` & `tornado-6.3b1/docs/releases/v4.0.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v4.0.1.rst` & `tornado-6.3b1/docs/releases/v4.0.1.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v4.0.2.rst` & `tornado-6.3b1/docs/releases/v4.0.2.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v4.1.0.rst` & `tornado-6.3b1/docs/releases/v4.1.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v4.2.0.rst` & `tornado-6.3b1/docs/releases/v4.2.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v4.3.0.rst` & `tornado-6.3b1/docs/releases/v4.3.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v4.4.0.rst` & `tornado-6.3b1/docs/releases/v4.4.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v4.4.2.rst` & `tornado-6.3b1/docs/releases/v4.4.2.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v4.5.0.rst` & `tornado-6.3b1/docs/releases/v4.5.0.rst`

 * *Files 1% similar despite different names*

```diff
@@ -174,18 +174,18 @@
   the keys ``compression_level`` and ``mem_level`` to set gzip parameters.
   The default compression level is now 6 instead of 9.
 
 Demos
 ~~~~~
 
 - A new file upload demo is available in the `file_upload
-  <https://github.com/tornadoweb/tornado/tree/master/demos/file_upload>`_
+  <https://github.com/tornadoweb/tornado/tree/stable/demos/file_upload>`_
   directory.
 - A new `.TCPClient` and `.TCPServer` demo is available in the
-  `tcpecho <https://github.com/tornadoweb/tornado/tree/master/demos/tcpecho>`_ directory.
+  `tcpecho <https://github.com/tornadoweb/tornado/tree/stable/demos/tcpecho>`_ directory.
 - Minor updates have been made to several existing demos, including
   updates to more recent versions of jquery.
 
 Credits
 ~~~~~~~
 
 The following people contributed commits to this release:
```

### Comparing `tornado-6.2b2/docs/releases/v4.5.3.rst` & `tornado-6.3b1/docs/releases/v4.5.3.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v5.0.0.rst` & `tornado-6.3b1/docs/releases/v5.0.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v5.0.2.rst` & `tornado-6.3b1/docs/releases/v5.0.2.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v5.1.0.rst` & `tornado-6.3b1/docs/releases/v5.1.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v6.0.0.rst` & `tornado-6.3b1/docs/releases/v6.0.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v6.0.4.rst` & `tornado-6.3b1/docs/releases/v6.0.4.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v6.1.0.rst` & `tornado-6.3b1/docs/releases/v6.1.0.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/releases/v6.2.0.rst` & `tornado-6.3b1/docs/releases/v6.2.0.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 What's new in Tornado 6.2.0
 ===========================
 
-Jun XX, 2022
-------------
+Jul 3, 2022
+-----------
 
 Deprecation notice
 ~~~~~~~~~~~~~~~~~~
 
+- April 2023 update: Python 3.12 reversed some of the changes described below.
+  In Tornado 6.3, `.AsyncTestCase`, `.AsyncHTTPTestCase`, and the behavior
+  of the `.IOLoop` constructor related to the ``make_current`` parameter
+  are no longer deprecated. 
 - Python 3.10 has begun the process of significant changes to the APIs for
   managing the event loop. Calls to methods such as `asyncio.get_event_loop` may
   now raise `DeprecationWarning` if no event loop is running. This has
   significant impact on the patterns for initializing applications, and in
   particular invalidates patterns that have long been the norm in Tornado's
   documentation and actual usage. In the future (with some as-yet-unspecified
   future version of Python), the old APIs will be removed. The new recommended
@@ -36,24 +40,24 @@
 
 General changes
 ~~~~~~~~~~~~~~~
 
 - The minimum supported Python version is now 3.7.
 - Wheels are now published with the Python stable ABI (``abi3``) for
   compatibility across versions of Python.
-- SSL certificate verfication and hostname checks are now enabled by default in
+- SSL certificate verification and hostname checks are now enabled by default in
   more places (primarily in client-side usage of `.SSLIOStream`).
 - Various improvements to type hints throughout the package.
 - CI has moved from Travis and Appveyor to Github Actions.  
 
 `tornado.gen`
 ~~~~~~~~~~~~~
 
 - Fixed a bug in which ``WaitIterator.current_index`` could be incorrect.
-- ``tornado.gen.TimeoutError``` is now an alias for `asyncio.TimeoutError`.
+- ``tornado.gen.TimeoutError`` is now an alias for `asyncio.TimeoutError`.
 
 `tornado.http1connection`
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 - ``max_body_size`` may now be set to zero to disallow a non-empty body.
 - ``Content-Encoding: gzip`` is now recognized case-insensitively.
 
@@ -71,14 +75,16 @@
 - `.PeriodicCallback` now accepts `datetime.timedelta` objects in addition to
   numbers of milliseconds.
 - Avoid logging "Event loop is closed" during shutdown-related race conditions.
 - Tornado no longer calls `logging.basicConfig` when starting an IOLoop; this
   has been unnecessary since Python 3.2 added a logger of last resort.
 - The `.IOLoop` constructor now accepts an ``asyncio_loop`` keyword argument to
   initialize with a specfied asyncio event loop.
+- It is now possible to construct an `.IOLoop` on one thread (with
+  ``make_current=False``) and start it on a different thread.
 
 `tornado.iostream`
 ~~~~~~~~~~~~~~~~~~
 
 - `.SSLIOStream` now supports reading more than 2GB at a time.
 - ``IOStream.write`` now supports typed `memoryview` objects.
 
@@ -117,8 +123,8 @@
 
 `tornado.websocket`
 ~~~~~~~~~~~~~~~~~~~
 
 - `.WebSocketClientConnection.write_message` now accepts `dict` arguments for
   consistency with `.WebSocketHandler.write_message`.
 - `.WebSocketClientConnection.write_message` now raises an exception as
-  documented if the connection is already closed.
+  documented if the connection is already closed.
```

### Comparing `tornado-6.2b2/docs/releases.rst` & `tornado-6.3b1/docs/releases.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Release notes
 =============
 
 .. toctree::
    :maxdepth: 2
 
+   releases/v6.3.0
    releases/v6.2.0
    releases/v6.1.0
    releases/v6.0.4
    releases/v6.0.3
    releases/v6.0.2
    releases/v6.0.1
    releases/v6.0.0
```

### Comparing `tornado-6.2b2/docs/template.rst` & `tornado-6.3b1/docs/template.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/testing.rst` & `tornado-6.3b1/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/tornado.png` & `tornado-6.3b1/docs/tornado.png`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/twisted.rst` & `tornado-6.3b1/docs/twisted.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/util.rst` & `tornado-6.3b1/docs/util.rst`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/docs/web.rst` & `tornado-6.3b1/docs/web.rst`

 * *Files 6% similar despite different names*

```diff
@@ -278,605 +278,664 @@
 00001150: 6574 686f 643a 3a20 5265 7175 6573 7448  ethod:: RequestH
 00001160: 616e 646c 6572 2e63 6c65 6172 5f63 6f6f  andler.clear_coo
 00001170: 6b69 650a 2020 202e 2e20 6175 746f 6d65  kie.   .. autome
 00001180: 7468 6f64 3a3a 2052 6571 7565 7374 4861  thod:: RequestHa
 00001190: 6e64 6c65 722e 636c 6561 725f 616c 6c5f  ndler.clear_all_
 000011a0: 636f 6f6b 6965 730a 2020 202e 2e20 6175  cookies.   .. au
 000011b0: 746f 6d65 7468 6f64 3a3a 2052 6571 7565  tomethod:: Reque
-000011c0: 7374 4861 6e64 6c65 722e 6765 745f 7365  stHandler.get_se
-000011d0: 6375 7265 5f63 6f6f 6b69 650a 2020 202e  cure_cookie.   .
+000011c0: 7374 4861 6e64 6c65 722e 6765 745f 7369  stHandler.get_si
+000011d0: 676e 6564 5f63 6f6f 6b69 650a 2020 202e  gned_cookie.   .
 000011e0: 2e20 6175 746f 6d65 7468 6f64 3a3a 2052  . automethod:: R
 000011f0: 6571 7565 7374 4861 6e64 6c65 722e 6765  equestHandler.ge
-00001200: 745f 7365 6375 7265 5f63 6f6f 6b69 655f  t_secure_cookie_
+00001200: 745f 7369 676e 6564 5f63 6f6f 6b69 655f  t_signed_cookie_
 00001210: 6b65 795f 7665 7273 696f 6e0a 2020 202e  key_version.   .
 00001220: 2e20 6175 746f 6d65 7468 6f64 3a3a 2052  . automethod:: R
 00001230: 6571 7565 7374 4861 6e64 6c65 722e 7365  equestHandler.se
-00001240: 745f 7365 6375 7265 5f63 6f6f 6b69 650a  t_secure_cookie.
-00001250: 2020 202e 2e20 6175 746f 6d65 7468 6f64     .. automethod
-00001260: 3a3a 2052 6571 7565 7374 4861 6e64 6c65  :: RequestHandle
-00001270: 722e 6372 6561 7465 5f73 6967 6e65 645f  r.create_signed_
-00001280: 7661 6c75 650a 2020 202e 2e20 6175 746f  value.   .. auto
-00001290: 6461 7461 3a3a 204d 494e 5f53 5550 504f  data:: MIN_SUPPO
-000012a0: 5254 4544 5f53 4947 4e45 445f 5641 4c55  RTED_SIGNED_VALU
-000012b0: 455f 5645 5253 494f 4e0a 2020 202e 2e20  E_VERSION.   .. 
-000012c0: 6175 746f 6461 7461 3a3a 204d 4158 5f53  autodata:: MAX_S
-000012d0: 5550 504f 5254 4544 5f53 4947 4e45 445f  UPPORTED_SIGNED_
-000012e0: 5641 4c55 455f 5645 5253 494f 4e0a 2020  VALUE_VERSION.  
-000012f0: 202e 2e20 6175 746f 6461 7461 3a3a 2044   .. autodata:: D
-00001300: 4546 4155 4c54 5f53 4947 4e45 445f 5641  EFAULT_SIGNED_VA
-00001310: 4c55 455f 5645 5253 494f 4e0a 2020 202e  LUE_VERSION.   .
-00001320: 2e20 6175 746f 6461 7461 3a3a 2044 4546  . autodata:: DEF
-00001330: 4155 4c54 5f53 4947 4e45 445f 5641 4c55  AULT_SIGNED_VALU
-00001340: 455f 4d49 4e5f 5645 5253 494f 4e0a 0a20  E_MIN_VERSION.. 
-00001350: 2020 4f74 6865 720a 2020 205e 5e5e 5e5e    Other.   ^^^^^
-00001360: 0a0a 2020 202e 2e20 6174 7472 6962 7574  ..   .. attribut
-00001370: 653a 3a20 5265 7175 6573 7448 616e 646c  e:: RequestHandl
-00001380: 6572 2e61 7070 6c69 6361 7469 6f6e 0a0a  er.application..
-00001390: 2020 2020 2020 5468 6520 6041 7070 6c69        The `Appli
-000013a0: 6361 7469 6f6e 6020 6f62 6a65 6374 2073  cation` object s
-000013b0: 6572 7669 6e67 2074 6869 7320 7265 7175  erving this requ
-000013c0: 6573 740a 0a20 2020 2e2e 2061 7574 6f6d  est..   .. autom
-000013d0: 6574 686f 643a 3a20 5265 7175 6573 7448  ethod:: RequestH
-000013e0: 616e 646c 6572 2e63 6865 636b 5f65 7461  andler.check_eta
-000013f0: 675f 6865 6164 6572 0a20 2020 2e2e 2061  g_header.   .. a
-00001400: 7574 6f6d 6574 686f 643a 3a20 5265 7175  utomethod:: Requ
-00001410: 6573 7448 616e 646c 6572 2e63 6865 636b  estHandler.check
-00001420: 5f78 7372 665f 636f 6f6b 6965 0a20 2020  _xsrf_cookie.   
-00001430: 2e2e 2061 7574 6f6d 6574 686f 643a 3a20  .. automethod:: 
-00001440: 5265 7175 6573 7448 616e 646c 6572 2e63  RequestHandler.c
-00001450: 6f6d 7075 7465 5f65 7461 670a 2020 202e  ompute_etag.   .
-00001460: 2e20 6175 746f 6d65 7468 6f64 3a3a 2052  . automethod:: R
-00001470: 6571 7565 7374 4861 6e64 6c65 722e 6372  equestHandler.cr
-00001480: 6561 7465 5f74 656d 706c 6174 655f 6c6f  eate_template_lo
-00001490: 6164 6572 0a20 2020 2e2e 2061 7574 6f61  ader.   .. autoa
-000014a0: 7474 7269 6275 7465 3a3a 2052 6571 7565  ttribute:: Reque
-000014b0: 7374 4861 6e64 6c65 722e 6375 7272 656e  stHandler.curren
-000014c0: 745f 7573 6572 0a20 2020 2e2e 2061 7574  t_user.   .. aut
-000014d0: 6f6d 6574 686f 643a 3a20 5265 7175 6573  omethod:: Reques
-000014e0: 7448 616e 646c 6572 2e64 6574 6163 680a  tHandler.detach.
-000014f0: 2020 202e 2e20 6175 746f 6d65 7468 6f64     .. automethod
-00001500: 3a3a 2052 6571 7565 7374 4861 6e64 6c65  :: RequestHandle
-00001510: 722e 6765 745f 6272 6f77 7365 725f 6c6f  r.get_browser_lo
-00001520: 6361 6c65 0a20 2020 2e2e 2061 7574 6f6d  cale.   .. autom
-00001530: 6574 686f 643a 3a20 5265 7175 6573 7448  ethod:: RequestH
-00001540: 616e 646c 6572 2e67 6574 5f63 7572 7265  andler.get_curre
-00001550: 6e74 5f75 7365 720a 2020 202e 2e20 6175  nt_user.   .. au
-00001560: 746f 6d65 7468 6f64 3a3a 2052 6571 7565  tomethod:: Reque
-00001570: 7374 4861 6e64 6c65 722e 6765 745f 6c6f  stHandler.get_lo
-00001580: 6769 6e5f 7572 6c0a 2020 202e 2e20 6175  gin_url.   .. au
-00001590: 746f 6d65 7468 6f64 3a3a 2052 6571 7565  tomethod:: Reque
-000015a0: 7374 4861 6e64 6c65 722e 6765 745f 7374  stHandler.get_st
-000015b0: 6174 7573 0a20 2020 2e2e 2061 7574 6f6d  atus.   .. autom
-000015c0: 6574 686f 643a 3a20 5265 7175 6573 7448  ethod:: RequestH
-000015d0: 616e 646c 6572 2e67 6574 5f74 656d 706c  andler.get_templ
-000015e0: 6174 655f 7061 7468 0a20 2020 2e2e 2061  ate_path.   .. a
-000015f0: 7574 6f6d 6574 686f 643a 3a20 5265 7175  utomethod:: Requ
-00001600: 6573 7448 616e 646c 6572 2e67 6574 5f75  estHandler.get_u
-00001610: 7365 725f 6c6f 6361 6c65 0a20 2020 2e2e  ser_locale.   ..
-00001620: 2061 7574 6f61 7474 7269 6275 7465 3a3a   autoattribute::
-00001630: 2052 6571 7565 7374 4861 6e64 6c65 722e   RequestHandler.
-00001640: 6c6f 6361 6c65 0a20 2020 2e2e 2061 7574  locale.   .. aut
-00001650: 6f6d 6574 686f 643a 3a20 5265 7175 6573  omethod:: Reques
-00001660: 7448 616e 646c 6572 2e6c 6f67 5f65 7863  tHandler.log_exc
-00001670: 6570 7469 6f6e 0a20 2020 2e2e 2061 7574  eption.   .. aut
-00001680: 6f6d 6574 686f 643a 3a20 5265 7175 6573  omethod:: Reques
-00001690: 7448 616e 646c 6572 2e6f 6e5f 636f 6e6e  tHandler.on_conn
-000016a0: 6563 7469 6f6e 5f63 6c6f 7365 0a20 2020  ection_close.   
-000016b0: 2e2e 2061 7574 6f6d 6574 686f 643a 3a20  .. automethod:: 
-000016c0: 5265 7175 6573 7448 616e 646c 6572 2e72  RequestHandler.r
-000016d0: 6571 7569 7265 5f73 6574 7469 6e67 0a20  equire_setting. 
-000016e0: 2020 2e2e 2061 7574 6f6d 6574 686f 643a    .. automethod:
-000016f0: 3a20 5265 7175 6573 7448 616e 646c 6572  : RequestHandler
-00001700: 2e72 6576 6572 7365 5f75 726c 0a20 2020  .reverse_url.   
-00001710: 2e2e 2061 7574 6f6d 6574 686f 643a 3a20  .. automethod:: 
-00001720: 5265 7175 6573 7448 616e 646c 6572 2e73  RequestHandler.s
-00001730: 6574 5f65 7461 675f 6865 6164 6572 0a20  et_etag_header. 
-00001740: 2020 2e2e 2061 7574 6f61 7474 7269 6275    .. autoattribu
-00001750: 7465 3a3a 2052 6571 7565 7374 4861 6e64  te:: RequestHand
-00001760: 6c65 722e 7365 7474 696e 6773 0a20 2020  ler.settings.   
-00001770: 2e2e 2061 7574 6f6d 6574 686f 643a 3a20  .. automethod:: 
-00001780: 5265 7175 6573 7448 616e 646c 6572 2e73  RequestHandler.s
-00001790: 7461 7469 635f 7572 6c0a 2020 202e 2e20  tatic_url.   .. 
-000017a0: 6175 746f 6d65 7468 6f64 3a3a 2052 6571  automethod:: Req
-000017b0: 7565 7374 4861 6e64 6c65 722e 7873 7266  uestHandler.xsrf
-000017c0: 5f66 6f72 6d5f 6874 6d6c 0a20 2020 2e2e  _form_html.   ..
-000017d0: 2061 7574 6f61 7474 7269 6275 7465 3a3a   autoattribute::
-000017e0: 2052 6571 7565 7374 4861 6e64 6c65 722e   RequestHandler.
-000017f0: 7873 7266 5f74 6f6b 656e 0a0a 0a0a 2020  xsrf_token....  
-00001800: 2041 7070 6c69 6361 7469 6f6e 2063 6f6e   Application con
-00001810: 6669 6775 7261 7469 6f6e 0a20 2020 2d2d  figuration.   --
-00001820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001830: 2d2d 2d2d 2d2d 2d0a 0a20 2020 2e2e 2061  -------..   .. a
-00001840: 7574 6f63 6c61 7373 3a3a 2041 7070 6c69  utoclass:: Appli
-00001850: 6361 7469 6f6e 2868 616e 646c 6572 733a  cation(handlers:
-00001860: 204f 7074 696f 6e61 6c5b 4c69 7374 5b55   Optional[List[U
-00001870: 6e69 6f6e 5b52 756c 652c 2054 7570 6c65  nion[Rule, Tuple
-00001880: 5d5d 5d20 3d20 4e6f 6e65 2c20 6465 6661  ]]] = None, defa
-00001890: 756c 745f 686f 7374 3a20 4f70 7469 6f6e  ult_host: Option
-000018a0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c20  al[str] = None, 
-000018b0: 7472 616e 7366 6f72 6d73 3a20 4f70 7469  transforms: Opti
-000018c0: 6f6e 616c 5b4c 6973 745b 5479 7065 5b4f  onal[List[Type[O
-000018d0: 7574 7075 7454 7261 6e73 666f 726d 5d5d  utputTransform]]
-000018e0: 5d20 3d20 4e6f 6e65 2c20 2a2a 7365 7474  ] = None, **sett
-000018f0: 696e 6773 290a 0a20 2020 2020 202e 2e20  ings)..      .. 
-00001900: 6174 7472 6962 7574 653a 3a20 7365 7474  attribute:: sett
-00001910: 696e 6773 0a0a 2020 2020 2020 2020 2041  ings..         A
-00001920: 6464 6974 696f 6e61 6c20 6b65 7977 6f72  dditional keywor
-00001930: 6420 6172 6775 6d65 6e74 7320 7061 7373  d arguments pass
-00001940: 6564 2074 6f20 7468 6520 636f 6e73 7472  ed to the constr
-00001950: 7563 746f 7220 6172 650a 2020 2020 2020  uctor are.      
-00001960: 2020 2073 6176 6564 2069 6e20 7468 6520     saved in the 
-00001970: 6073 6574 7469 6e67 7360 2064 6963 7469  `settings` dicti
-00001980: 6f6e 6172 792c 2061 6e64 2061 7265 206f  onary, and are o
-00001990: 6674 656e 2072 6566 6572 7265 6420 746f  ften referred to
-000019a0: 0a20 2020 2020 2020 2020 696e 2064 6f63  .         in doc
-000019b0: 756d 656e 7461 7469 6f6e 2061 7320 2261  umentation as "a
-000019c0: 7070 6c69 6361 7469 6f6e 2073 6574 7469  pplication setti
-000019d0: 6e67 7322 2e20 2053 6574 7469 6e67 7320  ngs".  Settings 
-000019e0: 6172 650a 2020 2020 2020 2020 2075 7365  are.         use
-000019f0: 6420 746f 2063 7573 746f 6d69 7a65 2076  d to customize v
-00001a00: 6172 696f 7573 2061 7370 6563 7473 206f  arious aspects o
-00001a10: 6620 546f 726e 6164 6f20 2861 6c74 686f  f Tornado (altho
-00001a20: 7567 6820 696e 0a20 2020 2020 2020 2020  ugh in.         
-00001a30: 736f 6d65 2063 6173 6573 2072 6963 6865  some cases riche
-00001a40: 7220 6375 7374 6f6d 697a 6174 696f 6e20  r customization 
-00001a50: 6973 2070 6f73 7369 626c 6520 6279 206f  is possible by o
-00001a60: 7665 7272 6964 696e 670a 2020 2020 2020  verriding.      
-00001a70: 2020 206d 6574 686f 6473 2069 6e20 6120     methods in a 
-00001a80: 7375 6263 6c61 7373 206f 6620 6052 6571  subclass of `Req
-00001a90: 7565 7374 4861 6e64 6c65 7260 292e 2020  uestHandler`).  
-00001aa0: 536f 6d65 0a20 2020 2020 2020 2020 6170  Some.         ap
-00001ab0: 706c 6963 6174 696f 6e73 2061 6c73 6f20  plications also 
-00001ac0: 6c69 6b65 2074 6f20 7573 6520 7468 6520  like to use the 
-00001ad0: 6073 6574 7469 6e67 7360 2064 6963 7469  `settings` dicti
-00001ae0: 6f6e 6172 7920 6173 2061 0a20 2020 2020  onary as a.     
-00001af0: 2020 2020 7761 7920 746f 206d 616b 6520      way to make 
-00001b00: 6170 706c 6963 6174 696f 6e2d 7370 6563  application-spec
-00001b10: 6966 6963 2073 6574 7469 6e67 7320 6176  ific settings av
-00001b20: 6169 6c61 626c 6520 746f 0a20 2020 2020  ailable to.     
-00001b30: 2020 2020 6861 6e64 6c65 7273 2077 6974      handlers wit
-00001b40: 686f 7574 2075 7369 6e67 2067 6c6f 6261  hout using globa
-00001b50: 6c20 7661 7269 6162 6c65 732e 2020 5365  l variables.  Se
-00001b60: 7474 696e 6773 2075 7365 6420 696e 0a20  ttings used in. 
-00001b70: 2020 2020 2020 2020 546f 726e 6164 6f20          Tornado 
-00001b80: 6172 6520 6465 7363 7269 6265 6420 6265  are described be
-00001b90: 6c6f 772e 0a0a 2020 2020 2020 2020 2047  low...         G
-00001ba0: 656e 6572 616c 2073 6574 7469 6e67 733a  eneral settings:
-00001bb0: 0a0a 2020 2020 2020 2020 202a 2060 6061  ..         * ``a
-00001bc0: 7574 6f72 656c 6f61 6460 603a 2049 6620  utoreload``: If 
-00001bd0: 6060 5472 7565 6060 2c20 7468 6520 7365  ``True``, the se
-00001be0: 7276 6572 2070 726f 6365 7373 2077 696c  rver process wil
-00001bf0: 6c20 7265 7374 6172 740a 2020 2020 2020  l restart.      
-00001c00: 2020 2020 2077 6865 6e20 616e 7920 736f       when any so
-00001c10: 7572 6365 2066 696c 6573 2063 6861 6e67  urce files chang
-00001c20: 652c 2061 7320 6465 7363 7269 6265 6420  e, as described 
-00001c30: 696e 203a 7265 663a 6064 6562 7567 2d6d  in :ref:`debug-m
-00001c40: 6f64 6560 2e0a 2020 2020 2020 2020 2020  ode`..          
-00001c50: 2054 6869 7320 6f70 7469 6f6e 2069 7320   This option is 
-00001c60: 6e65 7720 696e 2054 6f72 6e61 646f 2033  new in Tornado 3
-00001c70: 2e32 3b20 7072 6576 696f 7573 6c79 2074  .2; previously t
-00001c80: 6869 7320 6675 6e63 7469 6f6e 616c 6974  his functionalit
-00001c90: 790a 2020 2020 2020 2020 2020 2077 6173  y.           was
-00001ca0: 2063 6f6e 7472 6f6c 6c65 6420 6279 2074   controlled by t
-00001cb0: 6865 2060 6064 6562 7567 6060 2073 6574  he ``debug`` set
-00001cc0: 7469 6e67 2e0a 2020 2020 2020 2020 202a  ting..         *
-00001cd0: 2060 6064 6562 7567 6060 3a20 5368 6f72   ``debug``: Shor
-00001ce0: 7468 616e 6420 666f 7220 7365 7665 7261  thand for severa
-00001cf0: 6c20 6465 6275 6720 6d6f 6465 2073 6574  l debug mode set
-00001d00: 7469 6e67 732c 0a20 2020 2020 2020 2020  tings,.         
-00001d10: 2020 6465 7363 7269 6265 6420 696e 203a    described in :
-00001d20: 7265 663a 6064 6562 7567 2d6d 6f64 6560  ref:`debug-mode`
-00001d30: 2e20 2053 6574 7469 6e67 2060 6064 6562  .  Setting ``deb
-00001d40: 7567 3d54 7275 6560 6020 6973 0a20 2020  ug=True`` is.   
-00001d50: 2020 2020 2020 2020 6571 7569 7661 6c65          equivale
-00001d60: 6e74 2074 6f20 6060 6175 746f 7265 6c6f  nt to ``autorelo
-00001d70: 6164 3d54 7275 6560 602c 2060 6063 6f6d  ad=True``, ``com
-00001d80: 7069 6c65 645f 7465 6d70 6c61 7465 5f63  piled_template_c
-00001d90: 6163 6865 3d46 616c 7365 6060 2c0a 2020  ache=False``,.  
-00001da0: 2020 2020 2020 2020 2060 6073 7461 7469           ``stati
-00001db0: 635f 6861 7368 5f63 6163 6865 3d46 616c  c_hash_cache=Fal
-00001dc0: 7365 6060 2c20 6060 7365 7276 655f 7472  se``, ``serve_tr
-00001dd0: 6163 6562 6163 6b3d 5472 7565 6060 2e0a  aceback=True``..
-00001de0: 2020 2020 2020 2020 202a 2060 6064 6566           * ``def
-00001df0: 6175 6c74 5f68 616e 646c 6572 5f63 6c61  ault_handler_cla
-00001e00: 7373 6060 2061 6e64 2060 6064 6566 6175  ss`` and ``defau
-00001e10: 6c74 5f68 616e 646c 6572 5f61 7267 7360  lt_handler_args`
-00001e20: 603a 0a20 2020 2020 2020 2020 2020 5468  `:.           Th
-00001e30: 6973 2068 616e 646c 6572 2077 696c 6c20  is handler will 
-00001e40: 6265 2075 7365 6420 6966 206e 6f20 6f74  be used if no ot
-00001e50: 6865 7220 6d61 7463 6820 6973 2066 6f75  her match is fou
-00001e60: 6e64 3b0a 2020 2020 2020 2020 2020 2075  nd;.           u
-00001e70: 7365 2074 6869 7320 746f 2069 6d70 6c65  se this to imple
-00001e80: 6d65 6e74 2063 7573 746f 6d20 3430 3420  ment custom 404 
-00001e90: 7061 6765 7320 286e 6577 2069 6e20 546f  pages (new in To
-00001ea0: 726e 6164 6f20 332e 3229 2e0a 2020 2020  rnado 3.2)..    
-00001eb0: 2020 2020 202a 2060 6063 6f6d 7072 6573       * ``compres
-00001ec0: 735f 7265 7370 6f6e 7365 6060 3a20 4966  s_response``: If
-00001ed0: 2060 6054 7275 6560 602c 2072 6573 706f   ``True``, respo
-00001ee0: 6e73 6573 2069 6e20 7465 7874 7561 6c20  nses in textual 
-00001ef0: 666f 726d 6174 730a 2020 2020 2020 2020  formats.        
-00001f00: 2020 2077 696c 6c20 6265 2063 6f6d 7072     will be compr
-00001f10: 6573 7365 6420 6175 746f 6d61 7469 6361  essed automatica
-00001f20: 6c6c 792e 2020 4e65 7720 696e 2054 6f72  lly.  New in Tor
-00001f30: 6e61 646f 2034 2e30 2e0a 2020 2020 2020  nado 4.0..      
-00001f40: 2020 202a 2060 6067 7a69 7060 603a 2044     * ``gzip``: D
-00001f50: 6570 7265 6361 7465 6420 616c 6961 7320  eprecated alias 
-00001f60: 666f 7220 6060 636f 6d70 7265 7373 5f72  for ``compress_r
-00001f70: 6573 706f 6e73 6560 6020 7369 6e63 650a  esponse`` since.
-00001f80: 2020 2020 2020 2020 2020 2054 6f72 6e61             Torna
-00001f90: 646f 2034 2e30 2e0a 2020 2020 2020 2020  do 4.0..        
-00001fa0: 202a 2060 606c 6f67 5f66 756e 6374 696f   * ``log_functio
-00001fb0: 6e60 603a 2054 6869 7320 6675 6e63 7469  n``: This functi
-00001fc0: 6f6e 2077 696c 6c20 6265 2063 616c 6c65  on will be calle
-00001fd0: 6420 6174 2074 6865 2065 6e64 0a20 2020  d at the end.   
-00001fe0: 2020 2020 2020 2020 6f66 2065 7665 7279          of every
-00001ff0: 2072 6571 7565 7374 2074 6f20 6c6f 6720   request to log 
-00002000: 7468 6520 7265 7375 6c74 2028 7769 7468  the result (with
-00002010: 206f 6e65 2061 7267 756d 656e 742c 2074   one argument, t
-00002020: 6865 0a20 2020 2020 2020 2020 2020 6052  he.           `R
-00002030: 6571 7565 7374 4861 6e64 6c65 7260 206f  equestHandler` o
-00002040: 626a 6563 7429 2e20 2054 6865 2064 6566  bject).  The def
-00002050: 6175 6c74 2069 6d70 6c65 6d65 6e74 6174  ault implementat
-00002060: 696f 6e0a 2020 2020 2020 2020 2020 2077  ion.           w
-00002070: 7269 7465 7320 746f 2074 6865 2060 6c6f  rites to the `lo
-00002080: 6767 696e 6760 206d 6f64 756c 6527 7320  gging` module's 
-00002090: 726f 6f74 206c 6f67 6765 722e 2020 4d61  root logger.  Ma
-000020a0: 7920 616c 736f 2062 650a 2020 2020 2020  y also be.      
-000020b0: 2020 2020 2063 7573 746f 6d69 7a65 6420       customized 
-000020c0: 6279 206f 7665 7272 6964 696e 6720 6041  by overriding `A
-000020d0: 7070 6c69 6361 7469 6f6e 2e6c 6f67 5f72  pplication.log_r
-000020e0: 6571 7565 7374 602e 0a20 2020 2020 2020  equest`..       
-000020f0: 2020 2a20 6060 7365 7276 655f 7472 6163    * ``serve_trac
-00002100: 6562 6163 6b60 603a 2049 6620 6060 5472  eback``: If ``Tr
-00002110: 7565 6060 2c20 7468 6520 6465 6661 756c  ue``, the defaul
-00002120: 7420 6572 726f 7220 7061 6765 0a20 2020  t error page.   
-00002130: 2020 2020 2020 2020 7769 6c6c 2069 6e63          will inc
-00002140: 6c75 6465 2074 6865 2074 7261 6365 6261  lude the traceba
-00002150: 636b 206f 6620 7468 6520 6572 726f 722e  ck of the error.
-00002160: 2020 5468 6973 206f 7074 696f 6e20 6973    This option is
-00002170: 206e 6577 2069 6e0a 2020 2020 2020 2020   new in.        
-00002180: 2020 2054 6f72 6e61 646f 2033 2e32 3b20     Tornado 3.2; 
-00002190: 7072 6576 696f 7573 6c79 2074 6869 7320  previously this 
-000021a0: 6675 6e63 7469 6f6e 616c 6974 7920 7761  functionality wa
-000021b0: 7320 636f 6e74 726f 6c6c 6564 2062 790a  s controlled by.
-000021c0: 2020 2020 2020 2020 2020 2074 6865 2060             the `
-000021d0: 6064 6562 7567 6060 2073 6574 7469 6e67  `debug`` setting
-000021e0: 2e0a 2020 2020 2020 2020 202a 2060 6075  ..         * ``u
-000021f0: 695f 6d6f 6475 6c65 7360 6020 616e 6420  i_modules`` and 
-00002200: 6060 7569 5f6d 6574 686f 6473 6060 3a20  ``ui_methods``: 
-00002210: 4d61 7920 6265 2073 6574 2074 6f20 6120  May be set to a 
-00002220: 6d61 7070 696e 670a 2020 2020 2020 2020  mapping.        
-00002230: 2020 206f 6620 6055 494d 6f64 756c 6560     of `UIModule`
-00002240: 206f 7220 5549 206d 6574 686f 6473 2074   or UI methods t
-00002250: 6f20 6265 206d 6164 6520 6176 6169 6c61  o be made availa
-00002260: 626c 6520 746f 2074 656d 706c 6174 6573  ble to templates
-00002270: 2e0a 2020 2020 2020 2020 2020 204d 6179  ..           May
-00002280: 2062 6520 7365 7420 746f 2061 206d 6f64   be set to a mod
-00002290: 756c 652c 2064 6963 7469 6f6e 6172 792c  ule, dictionary,
-000022a0: 206f 7220 6120 6c69 7374 206f 6620 6d6f   or a list of mo
-000022b0: 6475 6c65 730a 2020 2020 2020 2020 2020  dules.          
-000022c0: 2061 6e64 2f6f 7220 6469 6374 732e 2020   and/or dicts.  
-000022d0: 5365 6520 3a72 6566 3a60 7569 2d6d 6f64  See :ref:`ui-mod
-000022e0: 756c 6573 6020 666f 7220 6d6f 7265 2064  ules` for more d
-000022f0: 6574 6169 6c73 2e0a 2020 2020 2020 2020  etails..        
-00002300: 202a 2060 6077 6562 736f 636b 6574 5f70   * ``websocket_p
-00002310: 696e 675f 696e 7465 7276 616c 6060 3a20  ing_interval``: 
-00002320: 4966 2073 6574 2074 6f20 6120 6e75 6d62  If set to a numb
-00002330: 6572 2c20 616c 6c20 7765 6273 6f63 6b65  er, all websocke
-00002340: 7473 2077 696c 6c0a 2020 2020 2020 2020  ts will.        
-00002350: 2020 2062 6520 7069 6e67 6564 2065 7665     be pinged eve
-00002360: 7279 206e 2073 6563 6f6e 6473 2e20 5468  ry n seconds. Th
-00002370: 6973 2063 616e 2068 656c 7020 6b65 6570  is can help keep
-00002380: 2074 6865 2063 6f6e 6e65 6374 696f 6e20   the connection 
-00002390: 616c 6976 650a 2020 2020 2020 2020 2020  alive.          
-000023a0: 2074 6872 6f75 6768 2063 6572 7461 696e   through certain
-000023b0: 2070 726f 7879 2073 6572 7665 7273 2077   proxy servers w
-000023c0: 6869 6368 2063 6c6f 7365 2069 646c 6520  hich close idle 
-000023d0: 636f 6e6e 6563 7469 6f6e 732c 2061 6e64  connections, and
-000023e0: 2069 740a 2020 2020 2020 2020 2020 2063   it.           c
-000023f0: 616e 2064 6574 6563 7420 6966 2074 6865  an detect if the
-00002400: 2077 6562 736f 636b 6574 2068 6173 2066   websocket has f
-00002410: 6169 6c65 6420 7769 7468 6f75 7420 6265  ailed without be
-00002420: 696e 6720 7072 6f70 6572 6c79 2063 6c6f  ing properly clo
-00002430: 7365 642e 0a20 2020 2020 2020 2020 2a20  sed..         * 
-00002440: 6060 7765 6273 6f63 6b65 745f 7069 6e67  ``websocket_ping
-00002450: 5f74 696d 656f 7574 6060 3a20 4966 2074  _timeout``: If t
-00002460: 6865 2070 696e 6720 696e 7465 7276 616c  he ping interval
-00002470: 2069 7320 7365 742c 2061 6e64 2074 6865   is set, and the
-00002480: 0a20 2020 2020 2020 2020 2020 7365 7276  .           serv
-00002490: 6572 2064 6f65 736e 2774 2072 6563 6569  er doesn't recei
-000024a0: 7665 2061 2027 706f 6e67 2720 696e 2074  ve a 'pong' in t
-000024b0: 6869 7320 6d61 6e79 2073 6563 6f6e 6473  his many seconds
-000024c0: 2c20 6974 2077 696c 6c20 636c 6f73 650a  , it will close.
-000024d0: 2020 2020 2020 2020 2020 2074 6865 2077             the w
-000024e0: 6562 736f 636b 6574 2e20 5468 6520 6465  ebsocket. The de
-000024f0: 6661 756c 7420 6973 2074 6872 6565 2074  fault is three t
-00002500: 696d 6573 2074 6865 2070 696e 6720 696e  imes the ping in
-00002510: 7465 7276 616c 2c20 7769 7468 2061 0a20  terval, with a. 
-00002520: 2020 2020 2020 2020 2020 6d69 6e69 6d75            minimu
-00002530: 6d20 6f66 2033 3020 7365 636f 6e64 732e  m of 30 seconds.
-00002540: 2049 676e 6f72 6564 2069 6620 7468 6520   Ignored if the 
-00002550: 7069 6e67 2069 6e74 6572 7661 6c20 6973  ping interval is
-00002560: 206e 6f74 2073 6574 2e0a 0a20 2020 2020   not set...     
-00002570: 2020 2020 4175 7468 656e 7469 6361 7469      Authenticati
-00002580: 6f6e 2061 6e64 2073 6563 7572 6974 7920  on and security 
-00002590: 7365 7474 696e 6773 3a0a 0a20 2020 2020  settings:..     
-000025a0: 2020 2020 2a20 6060 636f 6f6b 6965 5f73      * ``cookie_s
-000025b0: 6563 7265 7460 603a 2055 7365 6420 6279  ecret``: Used by
-000025c0: 2060 5265 7175 6573 7448 616e 646c 6572   `RequestHandler
-000025d0: 2e67 6574 5f73 6563 7572 655f 636f 6f6b  .get_secure_cook
-000025e0: 6965 600a 2020 2020 2020 2020 2020 2061  ie`.           a
-000025f0: 6e64 2060 2e73 6574 5f73 6563 7572 655f  nd `.set_secure_
-00002600: 636f 6f6b 6965 6020 746f 2073 6967 6e20  cookie` to sign 
-00002610: 636f 6f6b 6965 732e 0a20 2020 2020 2020  cookies..       
-00002620: 2020 2a20 6060 6b65 795f 7665 7273 696f    * ``key_versio
-00002630: 6e60 603a 2055 7365 6420 6279 2072 6571  n``: Used by req
-00002640: 7565 7374 4861 6e64 6c65 7220 602e 7365  uestHandler `.se
-00002650: 745f 7365 6375 7265 5f63 6f6f 6b69 6560  t_secure_cookie`
-00002660: 0a20 2020 2020 2020 2020 2020 746f 2073  .           to s
-00002670: 6967 6e20 636f 6f6b 6965 7320 7769 7468  ign cookies with
-00002680: 2061 2073 7065 6369 6669 6320 6b65 7920   a specific key 
-00002690: 7768 656e 2060 6063 6f6f 6b69 655f 7365  when ``cookie_se
-000026a0: 6372 6574 6060 0a20 2020 2020 2020 2020  cret``.         
-000026b0: 2020 6973 2061 206b 6579 2064 6963 7469    is a key dicti
-000026c0: 6f6e 6172 792e 0a20 2020 2020 2020 2020  onary..         
-000026d0: 2a20 6060 6c6f 6769 6e5f 7572 6c60 603a  * ``login_url``:
-000026e0: 2054 6865 2060 6175 7468 656e 7469 6361   The `authentica
-000026f0: 7465 6460 2064 6563 6f72 6174 6f72 2077  ted` decorator w
-00002700: 696c 6c20 7265 6469 7265 6374 0a20 2020  ill redirect.   
-00002710: 2020 2020 2020 2020 746f 2074 6869 7320          to this 
-00002720: 7572 6c20 6966 2074 6865 2075 7365 7220  url if the user 
-00002730: 6973 206e 6f74 206c 6f67 6765 6420 696e  is not logged in
-00002740: 2e20 2043 616e 2062 6520 6675 7274 6865  .  Can be furthe
-00002750: 720a 2020 2020 2020 2020 2020 2063 7573  r.           cus
-00002760: 746f 6d69 7a65 6420 6279 206f 7665 7272  tomized by overr
-00002770: 6964 696e 6720 6052 6571 7565 7374 4861  iding `RequestHa
-00002780: 6e64 6c65 722e 6765 745f 6c6f 6769 6e5f  ndler.get_login_
-00002790: 7572 6c60 0a20 2020 2020 2020 2020 2a20  url`.         * 
-000027a0: 6060 7873 7266 5f63 6f6f 6b69 6573 6060  ``xsrf_cookies``
-000027b0: 3a20 4966 2060 6054 7275 6560 602c 203a  : If ``True``, :
-000027c0: 7265 663a 6078 7372 6660 2077 696c 6c20  ref:`xsrf` will 
-000027d0: 6265 2065 6e61 626c 6564 2e0a 2020 2020  be enabled..    
-000027e0: 2020 2020 202a 2060 6078 7372 665f 636f       * ``xsrf_co
-000027f0: 6f6b 6965 5f76 6572 7369 6f6e 6060 3a20  okie_version``: 
-00002800: 436f 6e74 726f 6c73 2074 6865 2076 6572  Controls the ver
-00002810: 7369 6f6e 206f 6620 6e65 7720 5853 5246  sion of new XSRF
-00002820: 0a20 2020 2020 2020 2020 2020 636f 6f6b  .           cook
-00002830: 6965 7320 7072 6f64 7563 6564 2062 7920  ies produced by 
-00002840: 7468 6973 2073 6572 7665 722e 2020 5368  this server.  Sh
-00002850: 6f75 6c64 2067 656e 6572 616c 6c79 2062  ould generally b
-00002860: 6520 6c65 6674 0a20 2020 2020 2020 2020  e left.         
-00002870: 2020 6174 2074 6865 2064 6566 6175 6c74    at the default
-00002880: 2028 7768 6963 6820 7769 6c6c 2061 6c77   (which will alw
-00002890: 6179 7320 6265 2074 6865 2068 6967 6865  ays be the highe
-000028a0: 7374 2073 7570 706f 7274 6564 0a20 2020  st supported.   
-000028b0: 2020 2020 2020 2020 7665 7273 696f 6e29          version)
-000028c0: 2c20 6275 7420 6d61 7920 6265 2073 6574  , but may be set
-000028d0: 2074 6f20 6120 6c6f 7765 7220 7661 6c75   to a lower valu
-000028e0: 6520 7465 6d70 6f72 6172 696c 790a 2020  e temporarily.  
-000028f0: 2020 2020 2020 2020 2064 7572 696e 6720           during 
-00002900: 7665 7273 696f 6e20 7472 616e 7369 7469  version transiti
-00002910: 6f6e 732e 2020 4e65 7720 696e 2054 6f72  ons.  New in Tor
-00002920: 6e61 646f 2033 2e32 2e32 2c20 7768 6963  nado 3.2.2, whic
-00002930: 680a 2020 2020 2020 2020 2020 2069 6e74  h.           int
-00002940: 726f 6475 6365 6420 5853 5246 2063 6f6f  roduced XSRF coo
-00002950: 6b69 6520 7665 7273 696f 6e20 322e 0a20  kie version 2.. 
-00002960: 2020 2020 2020 2020 2a20 6060 7873 7266          * ``xsrf
-00002970: 5f63 6f6f 6b69 655f 6b77 6172 6773 6060  _cookie_kwargs``
-00002980: 3a20 4d61 7920 6265 2073 6574 2074 6f20  : May be set to 
-00002990: 6120 6469 6374 696f 6e61 7279 206f 660a  a dictionary of.
-000029a0: 2020 2020 2020 2020 2020 2061 6464 6974             addit
-000029b0: 696f 6e61 6c20 6172 6775 6d65 6e74 7320  ional arguments 
-000029c0: 746f 2062 6520 7061 7373 6564 2074 6f20  to be passed to 
-000029d0: 602e 5265 7175 6573 7448 616e 646c 6572  `.RequestHandler
-000029e0: 2e73 6574 5f63 6f6f 6b69 6560 0a20 2020  .set_cookie`.   
-000029f0: 2020 2020 2020 2020 666f 7220 7468 6520          for the 
-00002a00: 5853 5246 2063 6f6f 6b69 652e 0a20 2020  XSRF cookie..   
-00002a10: 2020 2020 2020 2a20 6060 7477 6974 7465        * ``twitte
-00002a20: 725f 636f 6e73 756d 6572 5f6b 6579 6060  r_consumer_key``
-00002a30: 2c20 6060 7477 6974 7465 725f 636f 6e73  , ``twitter_cons
-00002a40: 756d 6572 5f73 6563 7265 7460 602c 0a20  umer_secret``,. 
-00002a50: 2020 2020 2020 2020 2020 6060 6672 6965            ``frie
-00002a60: 6e64 6665 6564 5f63 6f6e 7375 6d65 725f  ndfeed_consumer_
-00002a70: 6b65 7960 602c 2060 6066 7269 656e 6466  key``, ``friendf
-00002a80: 6565 645f 636f 6e73 756d 6572 5f73 6563  eed_consumer_sec
-00002a90: 7265 7460 602c 0a20 2020 2020 2020 2020  ret``,.         
-00002aa0: 2020 6060 676f 6f67 6c65 5f63 6f6e 7375    ``google_consu
-00002ab0: 6d65 725f 6b65 7960 602c 2060 6067 6f6f  mer_key``, ``goo
-00002ac0: 676c 655f 636f 6e73 756d 6572 5f73 6563  gle_consumer_sec
-00002ad0: 7265 7460 602c 0a20 2020 2020 2020 2020  ret``,.         
-00002ae0: 2020 6060 6661 6365 626f 6f6b 5f61 7069    ``facebook_api
-00002af0: 5f6b 6579 6060 2c20 6060 6661 6365 626f  _key``, ``facebo
-00002b00: 6f6b 5f73 6563 7265 7460 603a 2020 5573  ok_secret``:  Us
-00002b10: 6564 2069 6e20 7468 650a 2020 2020 2020  ed in the.      
-00002b20: 2020 2020 2060 746f 726e 6164 6f2e 6175       `tornado.au
-00002b30: 7468 6020 6d6f 6475 6c65 2074 6f20 6175  th` module to au
-00002b40: 7468 656e 7469 6361 7465 2074 6f20 7661  thenticate to va
-00002b50: 7269 6f75 7320 4150 4973 2e0a 0a20 2020  rious APIs...   
-00002b60: 2020 2020 2020 5465 6d70 6c61 7465 2073        Template s
-00002b70: 6574 7469 6e67 733a 0a0a 2020 2020 2020  ettings:..      
-00002b80: 2020 202a 2060 6061 7574 6f65 7363 6170     * ``autoescap
-00002b90: 6560 603a 2043 6f6e 7472 6f6c 7320 6175  e``: Controls au
-00002ba0: 746f 6d61 7469 6320 6573 6361 7069 6e67  tomatic escaping
-00002bb0: 2066 6f72 2074 656d 706c 6174 6573 2e0a   for templates..
-00002bc0: 2020 2020 2020 2020 2020 204d 6179 2062             May b
-00002bd0: 6520 7365 7420 746f 2060 604e 6f6e 6560  e set to ``None`
-00002be0: 6020 746f 2064 6973 6162 6c65 2065 7363  ` to disable esc
-00002bf0: 6170 696e 672c 206f 7220 746f 2074 6865  aping, or to the
-00002c00: 202a 6e61 6d65 2a0a 2020 2020 2020 2020   *name*.        
-00002c10: 2020 206f 6620 6120 6675 6e63 7469 6f6e     of a function
-00002c20: 2074 6861 7420 616c 6c20 6f75 7470 7574   that all output
-00002c30: 2073 686f 756c 6420 6265 2070 6173 7365   should be passe
-00002c40: 6420 7468 726f 7567 682e 0a20 2020 2020  d through..     
-00002c50: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
-00002c60: 6f20 6060 2278 6874 6d6c 5f65 7363 6170  o ``"xhtml_escap
-00002c70: 6522 6060 2e20 2043 616e 2062 6520 6368  e"``.  Can be ch
-00002c80: 616e 6765 6420 6f6e 2061 2070 6572 2d74  anged on a per-t
-00002c90: 656d 706c 6174 650a 2020 2020 2020 2020  emplate.        
-00002ca0: 2020 2062 6173 6973 2077 6974 6820 7468     basis with th
-00002cb0: 6520 6060 7b25 2061 7574 6f65 7363 6170  e ``{% autoescap
-00002cc0: 6520 257d 6060 2064 6972 6563 7469 7665  e %}`` directive
-00002cd0: 2e0a 2020 2020 2020 2020 202a 2060 6063  ..         * ``c
-00002ce0: 6f6d 7069 6c65 645f 7465 6d70 6c61 7465  ompiled_template
-00002cf0: 5f63 6163 6865 6060 3a20 4465 6661 756c  _cache``: Defaul
-00002d00: 7420 6973 2060 6054 7275 6560 603b 2069  t is ``True``; i
-00002d10: 6620 6060 4661 6c73 6560 600a 2020 2020  f ``False``.    
-00002d20: 2020 2020 2020 2074 656d 706c 6174 6573         templates
-00002d30: 2077 696c 6c20 6265 2072 6563 6f6d 7069   will be recompi
-00002d40: 6c65 6420 6f6e 2065 7665 7279 2072 6571  led on every req
-00002d50: 7565 7374 2e20 2054 6869 7320 6f70 7469  uest.  This opti
-00002d60: 6f6e 0a20 2020 2020 2020 2020 2020 6973  on.           is
-00002d70: 206e 6577 2069 6e20 546f 726e 6164 6f20   new in Tornado 
-00002d80: 332e 323b 2070 7265 7669 6f75 736c 7920  3.2; previously 
-00002d90: 7468 6973 2066 756e 6374 696f 6e61 6c69  this functionali
-00002da0: 7479 2077 6173 2063 6f6e 7472 6f6c 6c65  ty was controlle
-00002db0: 640a 2020 2020 2020 2020 2020 2062 7920  d.           by 
-00002dc0: 7468 6520 6060 6465 6275 6760 6020 7365  the ``debug`` se
-00002dd0: 7474 696e 672e 0a20 2020 2020 2020 2020  tting..         
-00002de0: 2a20 6060 7465 6d70 6c61 7465 5f70 6174  * ``template_pat
-00002df0: 6860 603a 2044 6972 6563 746f 7279 2063  h``: Directory c
-00002e00: 6f6e 7461 696e 696e 6720 7465 6d70 6c61  ontaining templa
-00002e10: 7465 2066 696c 6573 2e20 2043 616e 2062  te files.  Can b
-00002e20: 650a 2020 2020 2020 2020 2020 2066 7572  e.           fur
-00002e30: 7468 6572 2063 7573 746f 6d69 7a65 6420  ther customized 
-00002e40: 6279 206f 7665 7272 6964 696e 6720 6052  by overriding `R
-00002e50: 6571 7565 7374 4861 6e64 6c65 722e 6765  equestHandler.ge
-00002e60: 745f 7465 6d70 6c61 7465 5f70 6174 6860  t_template_path`
-00002e70: 0a20 2020 2020 2020 2020 2a20 6060 7465  .         * ``te
-00002e80: 6d70 6c61 7465 5f6c 6f61 6465 7260 603a  mplate_loader``:
-00002e90: 2041 7373 6967 6e20 746f 2061 6e20 696e   Assign to an in
-00002ea0: 7374 616e 6365 206f 660a 2020 2020 2020  stance of.      
-00002eb0: 2020 2020 2060 746f 726e 6164 6f2e 7465       `tornado.te
-00002ec0: 6d70 6c61 7465 2e42 6173 654c 6f61 6465  mplate.BaseLoade
-00002ed0: 7260 2074 6f20 6375 7374 6f6d 697a 6520  r` to customize 
-00002ee0: 7465 6d70 6c61 7465 206c 6f61 6469 6e67  template loading
-00002ef0: 2e0a 2020 2020 2020 2020 2020 2049 6620  ..           If 
-00002f00: 7468 6973 2073 6574 7469 6e67 2069 7320  this setting is 
-00002f10: 7573 6564 2074 6865 2060 6074 656d 706c  used the ``templ
-00002f20: 6174 655f 7061 7468 6060 2061 6e64 2060  ate_path`` and `
-00002f30: 6061 7574 6f65 7363 6170 6560 600a 2020  `autoescape``.  
-00002f40: 2020 2020 2020 2020 2073 6574 7469 6e67           setting
-00002f50: 7320 6172 6520 6967 6e6f 7265 642e 2020  s are ignored.  
-00002f60: 4361 6e20 6265 2066 7572 7468 6572 2063  Can be further c
-00002f70: 7573 746f 6d69 7a65 6420 6279 206f 7665  ustomized by ove
-00002f80: 7272 6964 696e 670a 2020 2020 2020 2020  rriding.        
-00002f90: 2020 2060 5265 7175 6573 7448 616e 646c     `RequestHandl
-00002fa0: 6572 2e63 7265 6174 655f 7465 6d70 6c61  er.create_templa
-00002fb0: 7465 5f6c 6f61 6465 7260 2e0a 2020 2020  te_loader`..    
-00002fc0: 2020 2020 202a 2060 6074 656d 706c 6174       * ``templat
-00002fd0: 655f 7768 6974 6573 7061 6365 6060 3a20  e_whitespace``: 
-00002fe0: 436f 6e74 726f 6c73 2068 616e 646c 696e  Controls handlin
-00002ff0: 6720 6f66 2077 6869 7465 7370 6163 6520  g of whitespace 
-00003000: 696e 0a20 2020 2020 2020 2020 2020 7465  in.           te
-00003010: 6d70 6c61 7465 733b 2073 6565 2060 746f  mplates; see `to
-00003020: 726e 6164 6f2e 7465 6d70 6c61 7465 2e66  rnado.template.f
-00003030: 696c 7465 725f 7768 6974 6573 7061 6365  ilter_whitespace
-00003040: 6020 666f 7220 616c 6c6f 7765 640a 2020  ` for allowed.  
-00003050: 2020 2020 2020 2020 2076 616c 7565 732e           values.
-00003060: 204e 6577 2069 6e20 546f 726e 6164 6f20   New in Tornado 
-00003070: 342e 332e 0a0a 2020 2020 2020 2020 2053  4.3...         S
-00003080: 7461 7469 6320 6669 6c65 2073 6574 7469  tatic file setti
-00003090: 6e67 733a 0a0a 2020 2020 2020 2020 202a  ngs:..         *
-000030a0: 2060 6073 7461 7469 635f 6861 7368 5f63   ``static_hash_c
-000030b0: 6163 6865 6060 3a20 4465 6661 756c 7420  ache``: Default 
-000030c0: 6973 2060 6054 7275 6560 603b 2069 6620  is ``True``; if 
-000030d0: 6060 4661 6c73 6560 600a 2020 2020 2020  ``False``.      
-000030e0: 2020 2020 2073 7461 7469 6320 7572 6c73       static urls
-000030f0: 2077 696c 6c20 6265 2072 6563 6f6d 7075   will be recompu
-00003100: 7465 6420 6f6e 2065 7665 7279 2072 6571  ted on every req
-00003110: 7565 7374 2e20 2054 6869 7320 6f70 7469  uest.  This opti
-00003120: 6f6e 0a20 2020 2020 2020 2020 2020 6973  on.           is
-00003130: 206e 6577 2069 6e20 546f 726e 6164 6f20   new in Tornado 
-00003140: 332e 323b 2070 7265 7669 6f75 736c 7920  3.2; previously 
-00003150: 7468 6973 2066 756e 6374 696f 6e61 6c69  this functionali
-00003160: 7479 2077 6173 2063 6f6e 7472 6f6c 6c65  ty was controlle
-00003170: 640a 2020 2020 2020 2020 2020 2062 7920  d.           by 
-00003180: 7468 6520 6060 6465 6275 6760 6020 7365  the ``debug`` se
-00003190: 7474 696e 672e 0a20 2020 2020 2020 2020  tting..         
-000031a0: 2a20 6060 7374 6174 6963 5f70 6174 6860  * ``static_path`
-000031b0: 603a 2044 6972 6563 746f 7279 2066 726f  `: Directory fro
-000031c0: 6d20 7768 6963 6820 7374 6174 6963 2066  m which static f
-000031d0: 696c 6573 2077 696c 6c20 6265 0a20 2020  iles will be.   
-000031e0: 2020 2020 2020 2020 7365 7276 6564 2e0a          served..
-000031f0: 2020 2020 2020 2020 202a 2060 6073 7461           * ``sta
-00003200: 7469 635f 7572 6c5f 7072 6566 6978 6060  tic_url_prefix``
-00003210: 3a20 2055 726c 2070 7265 6669 7820 666f  :  Url prefix fo
-00003220: 7220 7374 6174 6963 2066 696c 6573 2c0a  r static files,.
-00003230: 2020 2020 2020 2020 2020 2064 6566 6175             defau
-00003240: 6c74 7320 746f 2060 6022 2f73 7461 7469  lts to ``"/stati
-00003250: 632f 2260 602e 0a20 2020 2020 2020 2020  c/"``..         
-00003260: 2a20 6060 7374 6174 6963 5f68 616e 646c  * ``static_handl
-00003270: 6572 5f63 6c61 7373 6060 2c20 6060 7374  er_class``, ``st
-00003280: 6174 6963 5f68 616e 646c 6572 5f61 7267  atic_handler_arg
-00003290: 7360 603a 204d 6179 2062 6520 7365 7420  s``: May be set 
-000032a0: 746f 0a20 2020 2020 2020 2020 2020 7573  to.           us
-000032b0: 6520 6120 6469 6666 6572 656e 7420 6861  e a different ha
-000032c0: 6e64 6c65 7220 666f 7220 7374 6174 6963  ndler for static
-000032d0: 2066 696c 6573 2069 6e73 7465 6164 206f   files instead o
-000032e0: 6620 7468 6520 6465 6661 756c 740a 2020  f the default.  
-000032f0: 2020 2020 2020 2020 2060 746f 726e 6164           `tornad
-00003300: 6f2e 7765 622e 5374 6174 6963 4669 6c65  o.web.StaticFile
-00003310: 4861 6e64 6c65 7260 2e20 2060 6073 7461  Handler`.  ``sta
-00003320: 7469 635f 6861 6e64 6c65 725f 6172 6773  tic_handler_args
-00003330: 6060 2c20 6966 2073 6574 2c0a 2020 2020  ``, if set,.    
-00003340: 2020 2020 2020 2073 686f 756c 6420 6265         should be
-00003350: 2061 2064 6963 7469 6f6e 6172 7920 6f66   a dictionary of
-00003360: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
-00003370: 7473 2074 6f20 6265 2070 6173 7365 6420  ts to be passed 
-00003380: 746f 2074 6865 0a20 2020 2020 2020 2020  to the.         
-00003390: 2020 6861 6e64 6c65 7227 7320 6060 696e    handler's ``in
-000033a0: 6974 6961 6c69 7a65 6060 206d 6574 686f  itialize`` metho
-000033b0: 642e 0a0a 2020 202e 2e20 6175 746f 6d65  d...   .. autome
-000033c0: 7468 6f64 3a3a 2041 7070 6c69 6361 7469  thod:: Applicati
-000033d0: 6f6e 2e6c 6973 7465 6e0a 2020 202e 2e20  on.listen.   .. 
-000033e0: 6175 746f 6d65 7468 6f64 3a3a 2041 7070  automethod:: App
-000033f0: 6c69 6361 7469 6f6e 2e61 6464 5f68 616e  lication.add_han
-00003400: 646c 6572 7328 6861 6e64 6c65 7273 3a20  dlers(handlers: 
-00003410: 4c69 7374 5b55 6e69 6f6e 5b52 756c 652c  List[Union[Rule,
-00003420: 2054 7570 6c65 5d5d 290a 2020 202e 2e20   Tuple]]).   .. 
-00003430: 6175 746f 6d65 7468 6f64 3a3a 2041 7070  automethod:: App
-00003440: 6c69 6361 7469 6f6e 2e67 6574 5f68 616e  lication.get_han
-00003450: 646c 6572 5f64 656c 6567 6174 650a 2020  dler_delegate.  
-00003460: 202e 2e20 6175 746f 6d65 7468 6f64 3a3a   .. automethod::
-00003470: 2041 7070 6c69 6361 7469 6f6e 2e72 6576   Application.rev
-00003480: 6572 7365 5f75 726c 0a20 2020 2e2e 2061  erse_url.   .. a
-00003490: 7574 6f6d 6574 686f 643a 3a20 4170 706c  utomethod:: Appl
-000034a0: 6963 6174 696f 6e2e 6c6f 675f 7265 7175  ication.log_requ
-000034b0: 6573 740a 0a20 2020 2e2e 2061 7574 6f63  est..   .. autoc
-000034c0: 6c61 7373 3a3a 2055 524c 5370 6563 0a0a  lass:: URLSpec..
-000034d0: 2020 2020 2020 5468 6520 6060 5552 4c53        The ``URLS
-000034e0: 7065 6360 6020 636c 6173 7320 6973 2061  pec`` class is a
-000034f0: 6c73 6f20 6176 6169 6c61 626c 6520 756e  lso available un
-00003500: 6465 7220 7468 6520 6e61 6d65 2060 6074  der the name ``t
-00003510: 6f72 6e61 646f 2e77 6562 2e75 726c 6060  ornado.web.url``
-00003520: 2e0a 0a20 2020 4465 636f 7261 746f 7273  ...   Decorators
-00003530: 0a20 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  .   ----------. 
-00003540: 2020 2e2e 2061 7574 6f66 756e 6374 696f    .. autofunctio
-00003550: 6e3a 3a20 6175 7468 656e 7469 6361 7465  n:: authenticate
-00003560: 640a 2020 202e 2e20 6175 746f 6675 6e63  d.   .. autofunc
-00003570: 7469 6f6e 3a3a 2061 6464 736c 6173 680a  tion:: addslash.
-00003580: 2020 202e 2e20 6175 746f 6675 6e63 7469     .. autofuncti
-00003590: 6f6e 3a3a 2072 656d 6f76 6573 6c61 7368  on:: removeslash
-000035a0: 0a20 2020 2e2e 2061 7574 6f66 756e 6374  .   .. autofunct
-000035b0: 696f 6e3a 3a20 7374 7265 616d 5f72 6571  ion:: stream_req
-000035c0: 7565 7374 5f62 6f64 790a 0a20 2020 4576  uest_body..   Ev
-000035d0: 6572 7974 6869 6e67 2065 6c73 650a 2020  erything else.  
-000035e0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-000035f0: 0a20 2020 2e2e 2061 7574 6f65 7863 6570  .   .. autoexcep
-00003600: 7469 6f6e 3a3a 2048 5454 5045 7272 6f72  tion:: HTTPError
-00003610: 0a20 2020 2e2e 2061 7574 6f65 7863 6570  .   .. autoexcep
-00003620: 7469 6f6e 3a3a 2046 696e 6973 680a 2020  tion:: Finish.  
-00003630: 202e 2e20 6175 746f 6578 6365 7074 696f   .. autoexceptio
-00003640: 6e3a 3a20 4d69 7373 696e 6741 7267 756d  n:: MissingArgum
-00003650: 656e 7445 7272 6f72 0a20 2020 2e2e 2061  entError.   .. a
-00003660: 7574 6f63 6c61 7373 3a3a 2055 494d 6f64  utoclass:: UIMod
-00003670: 756c 650a 2020 2020 2020 3a6d 656d 6265  ule.      :membe
-00003680: 7273 3a0a 0a20 2020 2e2e 2061 7574 6f63  rs:..   .. autoc
-00003690: 6c61 7373 3a3a 2045 7272 6f72 4861 6e64  lass:: ErrorHand
-000036a0: 6c65 720a 2020 202e 2e20 6175 746f 636c  ler.   .. autocl
-000036b0: 6173 733a 3a20 4661 6c6c 6261 636b 4861  ass:: FallbackHa
-000036c0: 6e64 6c65 720a 2020 202e 2e20 6175 746f  ndler.   .. auto
-000036d0: 636c 6173 733a 3a20 5265 6469 7265 6374  class:: Redirect
-000036e0: 4861 6e64 6c65 720a 2020 202e 2e20 6175  Handler.   .. au
-000036f0: 746f 636c 6173 733a 3a20 5374 6174 6963  toclass:: Static
-00003700: 4669 6c65 4861 6e64 6c65 720a 2020 2020  FileHandler.    
-00003710: 2020 3a6d 656d 6265 7273 3a0a              :members:.
+00001240: 745f 7369 676e 6564 5f63 6f6f 6b69 650a  t_signed_cookie.
+00001250: 2020 202e 2e20 6d65 7468 6f64 3a3a 2052     .. method:: R
+00001260: 6571 7565 7374 4861 6e64 6c65 722e 6765  equestHandler.ge
+00001270: 745f 7365 6375 7265 5f63 6f6f 6b69 650a  t_secure_cookie.
+00001280: 0a20 2020 2020 2044 6570 7265 6361 7465  .      Deprecate
+00001290: 6420 616c 6961 7320 666f 7220 6060 6765  d alias for ``ge
+000012a0: 745f 7369 676e 6564 5f63 6f6f 6b69 6560  t_signed_cookie`
+000012b0: 602e 0a0a 2020 2020 2020 2e2e 2064 6570  `...      .. dep
+000012c0: 7265 6361 7465 643a 3a20 362e 330a 0a20  recated:: 6.3.. 
+000012d0: 2020 2e2e 206d 6574 686f 643a 3a20 5265    .. method:: Re
+000012e0: 7175 6573 7448 616e 646c 6572 2e67 6574  questHandler.get
+000012f0: 5f73 6563 7572 655f 636f 6f6b 6965 5f6b  _secure_cookie_k
+00001300: 6579 5f76 6572 7369 6f6e 0a0a 2020 2020  ey_version..    
+00001310: 2020 4465 7072 6563 6174 6564 2061 6c69    Deprecated ali
+00001320: 6173 2066 6f72 2060 6067 6574 5f73 6967  as for ``get_sig
+00001330: 6e65 645f 636f 6f6b 6965 5f6b 6579 5f76  ned_cookie_key_v
+00001340: 6572 7369 6f6e 6060 2e0a 0a20 2020 2020  ersion``...     
+00001350: 202e 2e20 6465 7072 6563 6174 6564 3a3a   .. deprecated::
+00001360: 2036 2e33 0a0a 2020 202e 2e20 6d65 7468   6.3..   .. meth
+00001370: 6f64 3a3a 2052 6571 7565 7374 4861 6e64  od:: RequestHand
+00001380: 6c65 722e 7365 745f 7365 6375 7265 5f63  ler.set_secure_c
+00001390: 6f6f 6b69 650a 0a20 2020 2020 2044 6570  ookie..      Dep
+000013a0: 7265 6361 7465 6420 616c 6961 7320 666f  recated alias fo
+000013b0: 7220 6060 7365 745f 7369 676e 6564 5f63  r ``set_signed_c
+000013c0: 6f6f 6b69 6560 602e 0a0a 2020 2020 2020  ookie``...      
+000013d0: 2e2e 2064 6570 7265 6361 7465 643a 3a20  .. deprecated:: 
+000013e0: 362e 330a 0a20 2020 2e2e 2061 7574 6f6d  6.3..   .. autom
+000013f0: 6574 686f 643a 3a20 5265 7175 6573 7448  ethod:: RequestH
+00001400: 616e 646c 6572 2e63 7265 6174 655f 7369  andler.create_si
+00001410: 676e 6564 5f76 616c 7565 0a20 2020 2e2e  gned_value.   ..
+00001420: 2061 7574 6f64 6174 613a 3a20 4d49 4e5f   autodata:: MIN_
+00001430: 5355 5050 4f52 5445 445f 5349 474e 4544  SUPPORTED_SIGNED
+00001440: 5f56 414c 5545 5f56 4552 5349 4f4e 0a20  _VALUE_VERSION. 
+00001450: 2020 2e2e 2061 7574 6f64 6174 613a 3a20    .. autodata:: 
+00001460: 4d41 585f 5355 5050 4f52 5445 445f 5349  MAX_SUPPORTED_SI
+00001470: 474e 4544 5f56 414c 5545 5f56 4552 5349  GNED_VALUE_VERSI
+00001480: 4f4e 0a20 2020 2e2e 2061 7574 6f64 6174  ON.   .. autodat
+00001490: 613a 3a20 4445 4641 554c 545f 5349 474e  a:: DEFAULT_SIGN
+000014a0: 4544 5f56 414c 5545 5f56 4552 5349 4f4e  ED_VALUE_VERSION
+000014b0: 0a20 2020 2e2e 2061 7574 6f64 6174 613a  .   .. autodata:
+000014c0: 3a20 4445 4641 554c 545f 5349 474e 4544  : DEFAULT_SIGNED
+000014d0: 5f56 414c 5545 5f4d 494e 5f56 4552 5349  _VALUE_MIN_VERSI
+000014e0: 4f4e 0a0a 2020 204f 7468 6572 0a20 2020  ON..   Other.   
+000014f0: 5e5e 5e5e 5e0a 0a20 2020 2e2e 2061 7474  ^^^^^..   .. att
+00001500: 7269 6275 7465 3a3a 2052 6571 7565 7374  ribute:: Request
+00001510: 4861 6e64 6c65 722e 6170 706c 6963 6174  Handler.applicat
+00001520: 696f 6e0a 0a20 2020 2020 2054 6865 2060  ion..      The `
+00001530: 4170 706c 6963 6174 696f 6e60 206f 626a  Application` obj
+00001540: 6563 7420 7365 7276 696e 6720 7468 6973  ect serving this
+00001550: 2072 6571 7565 7374 0a0a 2020 202e 2e20   request..   .. 
+00001560: 6175 746f 6d65 7468 6f64 3a3a 2052 6571  automethod:: Req
+00001570: 7565 7374 4861 6e64 6c65 722e 6368 6563  uestHandler.chec
+00001580: 6b5f 6574 6167 5f68 6561 6465 720a 2020  k_etag_header.  
+00001590: 202e 2e20 6175 746f 6d65 7468 6f64 3a3a   .. automethod::
+000015a0: 2052 6571 7565 7374 4861 6e64 6c65 722e   RequestHandler.
+000015b0: 6368 6563 6b5f 7873 7266 5f63 6f6f 6b69  check_xsrf_cooki
+000015c0: 650a 2020 202e 2e20 6175 746f 6d65 7468  e.   .. autometh
+000015d0: 6f64 3a3a 2052 6571 7565 7374 4861 6e64  od:: RequestHand
+000015e0: 6c65 722e 636f 6d70 7574 655f 6574 6167  ler.compute_etag
+000015f0: 0a20 2020 2e2e 2061 7574 6f6d 6574 686f  .   .. autometho
+00001600: 643a 3a20 5265 7175 6573 7448 616e 646c  d:: RequestHandl
+00001610: 6572 2e63 7265 6174 655f 7465 6d70 6c61  er.create_templa
+00001620: 7465 5f6c 6f61 6465 720a 2020 202e 2e20  te_loader.   .. 
+00001630: 6175 746f 6174 7472 6962 7574 653a 3a20  autoattribute:: 
+00001640: 5265 7175 6573 7448 616e 646c 6572 2e63  RequestHandler.c
+00001650: 7572 7265 6e74 5f75 7365 720a 2020 202e  urrent_user.   .
+00001660: 2e20 6175 746f 6d65 7468 6f64 3a3a 2052  . automethod:: R
+00001670: 6571 7565 7374 4861 6e64 6c65 722e 6465  equestHandler.de
+00001680: 7461 6368 0a20 2020 2e2e 2061 7574 6f6d  tach.   .. autom
+00001690: 6574 686f 643a 3a20 5265 7175 6573 7448  ethod:: RequestH
+000016a0: 616e 646c 6572 2e67 6574 5f62 726f 7773  andler.get_brows
+000016b0: 6572 5f6c 6f63 616c 650a 2020 202e 2e20  er_locale.   .. 
+000016c0: 6175 746f 6d65 7468 6f64 3a3a 2052 6571  automethod:: Req
+000016d0: 7565 7374 4861 6e64 6c65 722e 6765 745f  uestHandler.get_
+000016e0: 6375 7272 656e 745f 7573 6572 0a20 2020  current_user.   
+000016f0: 2e2e 2061 7574 6f6d 6574 686f 643a 3a20  .. automethod:: 
+00001700: 5265 7175 6573 7448 616e 646c 6572 2e67  RequestHandler.g
+00001710: 6574 5f6c 6f67 696e 5f75 726c 0a20 2020  et_login_url.   
+00001720: 2e2e 2061 7574 6f6d 6574 686f 643a 3a20  .. automethod:: 
+00001730: 5265 7175 6573 7448 616e 646c 6572 2e67  RequestHandler.g
+00001740: 6574 5f73 7461 7475 730a 2020 202e 2e20  et_status.   .. 
+00001750: 6175 746f 6d65 7468 6f64 3a3a 2052 6571  automethod:: Req
+00001760: 7565 7374 4861 6e64 6c65 722e 6765 745f  uestHandler.get_
+00001770: 7465 6d70 6c61 7465 5f70 6174 680a 2020  template_path.  
+00001780: 202e 2e20 6175 746f 6d65 7468 6f64 3a3a   .. automethod::
+00001790: 2052 6571 7565 7374 4861 6e64 6c65 722e   RequestHandler.
+000017a0: 6765 745f 7573 6572 5f6c 6f63 616c 650a  get_user_locale.
+000017b0: 2020 202e 2e20 6175 746f 6174 7472 6962     .. autoattrib
+000017c0: 7574 653a 3a20 5265 7175 6573 7448 616e  ute:: RequestHan
+000017d0: 646c 6572 2e6c 6f63 616c 650a 2020 202e  dler.locale.   .
+000017e0: 2e20 6175 746f 6d65 7468 6f64 3a3a 2052  . automethod:: R
+000017f0: 6571 7565 7374 4861 6e64 6c65 722e 6c6f  equestHandler.lo
+00001800: 675f 6578 6365 7074 696f 6e0a 2020 202e  g_exception.   .
+00001810: 2e20 6175 746f 6d65 7468 6f64 3a3a 2052  . automethod:: R
+00001820: 6571 7565 7374 4861 6e64 6c65 722e 6f6e  equestHandler.on
+00001830: 5f63 6f6e 6e65 6374 696f 6e5f 636c 6f73  _connection_clos
+00001840: 650a 2020 202e 2e20 6175 746f 6d65 7468  e.   .. autometh
+00001850: 6f64 3a3a 2052 6571 7565 7374 4861 6e64  od:: RequestHand
+00001860: 6c65 722e 7265 7175 6972 655f 7365 7474  ler.require_sett
+00001870: 696e 670a 2020 202e 2e20 6175 746f 6d65  ing.   .. autome
+00001880: 7468 6f64 3a3a 2052 6571 7565 7374 4861  thod:: RequestHa
+00001890: 6e64 6c65 722e 7265 7665 7273 655f 7572  ndler.reverse_ur
+000018a0: 6c0a 2020 202e 2e20 6175 746f 6d65 7468  l.   .. autometh
+000018b0: 6f64 3a3a 2052 6571 7565 7374 4861 6e64  od:: RequestHand
+000018c0: 6c65 722e 7365 745f 6574 6167 5f68 6561  ler.set_etag_hea
+000018d0: 6465 720a 2020 202e 2e20 6175 746f 6174  der.   .. autoat
+000018e0: 7472 6962 7574 653a 3a20 5265 7175 6573  tribute:: Reques
+000018f0: 7448 616e 646c 6572 2e73 6574 7469 6e67  tHandler.setting
+00001900: 730a 2020 202e 2e20 6175 746f 6d65 7468  s.   .. autometh
+00001910: 6f64 3a3a 2052 6571 7565 7374 4861 6e64  od:: RequestHand
+00001920: 6c65 722e 7374 6174 6963 5f75 726c 0a20  ler.static_url. 
+00001930: 2020 2e2e 2061 7574 6f6d 6574 686f 643a    .. automethod:
+00001940: 3a20 5265 7175 6573 7448 616e 646c 6572  : RequestHandler
+00001950: 2e78 7372 665f 666f 726d 5f68 746d 6c0a  .xsrf_form_html.
+00001960: 2020 202e 2e20 6175 746f 6174 7472 6962     .. autoattrib
+00001970: 7574 653a 3a20 5265 7175 6573 7448 616e  ute:: RequestHan
+00001980: 646c 6572 2e78 7372 665f 746f 6b65 6e0a  dler.xsrf_token.
+00001990: 0a0a 0a20 2020 4170 706c 6963 6174 696f  ...   Applicatio
+000019a0: 6e20 636f 6e66 6967 7572 6174 696f 6e0a  n configuration.
+000019b0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+000019c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2020  ------------..  
+000019d0: 202e 2e20 6175 746f 636c 6173 733a 3a20   .. autoclass:: 
+000019e0: 4170 706c 6963 6174 696f 6e28 6861 6e64  Application(hand
+000019f0: 6c65 7273 3a20 4f70 7469 6f6e 616c 5b4c  lers: Optional[L
+00001a00: 6973 745b 556e 696f 6e5b 5275 6c65 2c20  ist[Union[Rule, 
+00001a10: 5475 706c 655d 5d5d 203d 204e 6f6e 652c  Tuple]]] = None,
+00001a20: 2064 6566 6175 6c74 5f68 6f73 743a 204f   default_host: O
+00001a30: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+00001a40: 6f6e 652c 2074 7261 6e73 666f 726d 733a  one, transforms:
+00001a50: 204f 7074 696f 6e61 6c5b 4c69 7374 5b54   Optional[List[T
+00001a60: 7970 655b 4f75 7470 7574 5472 616e 7366  ype[OutputTransf
+00001a70: 6f72 6d5d 5d5d 203d 204e 6f6e 652c 202a  orm]]] = None, *
+00001a80: 2a73 6574 7469 6e67 7329 0a0a 2020 2020  *settings)..    
+00001a90: 2020 2e2e 2061 7474 7269 6275 7465 3a3a    .. attribute::
+00001aa0: 2073 6574 7469 6e67 730a 0a20 2020 2020   settings..     
+00001ab0: 2020 2020 4164 6469 7469 6f6e 616c 206b      Additional k
+00001ac0: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
+00001ad0: 2070 6173 7365 6420 746f 2074 6865 2063   passed to the c
+00001ae0: 6f6e 7374 7275 6374 6f72 2061 7265 0a20  onstructor are. 
+00001af0: 2020 2020 2020 2020 7361 7665 6420 696e          saved in
+00001b00: 2074 6865 2060 7365 7474 696e 6773 6020   the `settings` 
+00001b10: 6469 6374 696f 6e61 7279 2c20 616e 6420  dictionary, and 
+00001b20: 6172 6520 6f66 7465 6e20 7265 6665 7272  are often referr
+00001b30: 6564 2074 6f0a 2020 2020 2020 2020 2069  ed to.         i
+00001b40: 6e20 646f 6375 6d65 6e74 6174 696f 6e20  n documentation 
+00001b50: 6173 2022 6170 706c 6963 6174 696f 6e20  as "application 
+00001b60: 7365 7474 696e 6773 222e 2020 5365 7474  settings".  Sett
+00001b70: 696e 6773 2061 7265 0a20 2020 2020 2020  ings are.       
+00001b80: 2020 7573 6564 2074 6f20 6375 7374 6f6d    used to custom
+00001b90: 697a 6520 7661 7269 6f75 7320 6173 7065  ize various aspe
+00001ba0: 6374 7320 6f66 2054 6f72 6e61 646f 2028  cts of Tornado (
+00001bb0: 616c 7468 6f75 6768 2069 6e0a 2020 2020  although in.    
+00001bc0: 2020 2020 2073 6f6d 6520 6361 7365 7320       some cases 
+00001bd0: 7269 6368 6572 2063 7573 746f 6d69 7a61  richer customiza
+00001be0: 7469 6f6e 2069 7320 706f 7373 6962 6c65  tion is possible
+00001bf0: 2062 7920 6f76 6572 7269 6469 6e67 0a20   by overriding. 
+00001c00: 2020 2020 2020 2020 6d65 7468 6f64 7320          methods 
+00001c10: 696e 2061 2073 7562 636c 6173 7320 6f66  in a subclass of
+00001c20: 2060 5265 7175 6573 7448 616e 646c 6572   `RequestHandler
+00001c30: 6029 2e20 2053 6f6d 650a 2020 2020 2020  `).  Some.      
+00001c40: 2020 2061 7070 6c69 6361 7469 6f6e 7320     applications 
+00001c50: 616c 736f 206c 696b 6520 746f 2075 7365  also like to use
+00001c60: 2074 6865 2060 7365 7474 696e 6773 6020   the `settings` 
+00001c70: 6469 6374 696f 6e61 7279 2061 7320 610a  dictionary as a.
+00001c80: 2020 2020 2020 2020 2077 6179 2074 6f20           way to 
+00001c90: 6d61 6b65 2061 7070 6c69 6361 7469 6f6e  make application
+00001ca0: 2d73 7065 6369 6669 6320 7365 7474 696e  -specific settin
+00001cb0: 6773 2061 7661 696c 6162 6c65 2074 6f0a  gs available to.
+00001cc0: 2020 2020 2020 2020 2068 616e 646c 6572           handler
+00001cd0: 7320 7769 7468 6f75 7420 7573 696e 6720  s without using 
+00001ce0: 676c 6f62 616c 2076 6172 6961 626c 6573  global variables
+00001cf0: 2e20 2053 6574 7469 6e67 7320 7573 6564  .  Settings used
+00001d00: 2069 6e0a 2020 2020 2020 2020 2054 6f72   in.         Tor
+00001d10: 6e61 646f 2061 7265 2064 6573 6372 6962  nado are describ
+00001d20: 6564 2062 656c 6f77 2e0a 0a20 2020 2020  ed below...     
+00001d30: 2020 2020 4765 6e65 7261 6c20 7365 7474      General sett
+00001d40: 696e 6773 3a0a 0a20 2020 2020 2020 2020  ings:..         
+00001d50: 2a20 6060 6175 746f 7265 6c6f 6164 6060  * ``autoreload``
+00001d60: 3a20 4966 2060 6054 7275 6560 602c 2074  : If ``True``, t
+00001d70: 6865 2073 6572 7665 7220 7072 6f63 6573  he server proces
+00001d80: 7320 7769 6c6c 2072 6573 7461 7274 0a20  s will restart. 
+00001d90: 2020 2020 2020 2020 2020 7768 656e 2061            when a
+00001da0: 6e79 2073 6f75 7263 6520 6669 6c65 7320  ny source files 
+00001db0: 6368 616e 6765 2c20 6173 2064 6573 6372  change, as descr
+00001dc0: 6962 6564 2069 6e20 3a72 6566 3a60 6465  ibed in :ref:`de
+00001dd0: 6275 672d 6d6f 6465 602e 0a20 2020 2020  bug-mode`..     
+00001de0: 2020 2020 2020 5468 6973 206f 7074 696f        This optio
+00001df0: 6e20 6973 206e 6577 2069 6e20 546f 726e  n is new in Torn
+00001e00: 6164 6f20 332e 323b 2070 7265 7669 6f75  ado 3.2; previou
+00001e10: 736c 7920 7468 6973 2066 756e 6374 696f  sly this functio
+00001e20: 6e61 6c69 7479 0a20 2020 2020 2020 2020  nality.         
+00001e30: 2020 7761 7320 636f 6e74 726f 6c6c 6564    was controlled
+00001e40: 2062 7920 7468 6520 6060 6465 6275 6760   by the ``debug`
+00001e50: 6020 7365 7474 696e 672e 0a20 2020 2020  ` setting..     
+00001e60: 2020 2020 2a20 6060 6465 6275 6760 603a      * ``debug``:
+00001e70: 2053 686f 7274 6861 6e64 2066 6f72 2073   Shorthand for s
+00001e80: 6576 6572 616c 2064 6562 7567 206d 6f64  everal debug mod
+00001e90: 6520 7365 7474 696e 6773 2c0a 2020 2020  e settings,.    
+00001ea0: 2020 2020 2020 2064 6573 6372 6962 6564         described
+00001eb0: 2069 6e20 3a72 6566 3a60 6465 6275 672d   in :ref:`debug-
+00001ec0: 6d6f 6465 602e 2020 5365 7474 696e 6720  mode`.  Setting 
+00001ed0: 6060 6465 6275 673d 5472 7565 6060 2069  ``debug=True`` i
+00001ee0: 730a 2020 2020 2020 2020 2020 2065 7175  s.           equ
+00001ef0: 6976 616c 656e 7420 746f 2060 6061 7574  ivalent to ``aut
+00001f00: 6f72 656c 6f61 643d 5472 7565 6060 2c20  oreload=True``, 
+00001f10: 6060 636f 6d70 696c 6564 5f74 656d 706c  ``compiled_templ
+00001f20: 6174 655f 6361 6368 653d 4661 6c73 6560  ate_cache=False`
+00001f30: 602c 0a20 2020 2020 2020 2020 2020 6060  `,.           ``
+00001f40: 7374 6174 6963 5f68 6173 685f 6361 6368  static_hash_cach
+00001f50: 653d 4661 6c73 6560 602c 2060 6073 6572  e=False``, ``ser
+00001f60: 7665 5f74 7261 6365 6261 636b 3d54 7275  ve_traceback=Tru
+00001f70: 6560 602e 0a20 2020 2020 2020 2020 2a20  e``..         * 
+00001f80: 6060 6465 6661 756c 745f 6861 6e64 6c65  ``default_handle
+00001f90: 725f 636c 6173 7360 6020 616e 6420 6060  r_class`` and ``
+00001fa0: 6465 6661 756c 745f 6861 6e64 6c65 725f  default_handler_
+00001fb0: 6172 6773 6060 3a0a 2020 2020 2020 2020  args``:.        
+00001fc0: 2020 2054 6869 7320 6861 6e64 6c65 7220     This handler 
+00001fd0: 7769 6c6c 2062 6520 7573 6564 2069 6620  will be used if 
+00001fe0: 6e6f 206f 7468 6572 206d 6174 6368 2069  no other match i
+00001ff0: 7320 666f 756e 643b 0a20 2020 2020 2020  s found;.       
+00002000: 2020 2020 7573 6520 7468 6973 2074 6f20      use this to 
+00002010: 696d 706c 656d 656e 7420 6375 7374 6f6d  implement custom
+00002020: 2034 3034 2070 6167 6573 2028 6e65 7720   404 pages (new 
+00002030: 696e 2054 6f72 6e61 646f 2033 2e32 292e  in Tornado 3.2).
+00002040: 0a20 2020 2020 2020 2020 2a20 6060 636f  .         * ``co
+00002050: 6d70 7265 7373 5f72 6573 706f 6e73 6560  mpress_response`
+00002060: 603a 2049 6620 6060 5472 7565 6060 2c20  `: If ``True``, 
+00002070: 7265 7370 6f6e 7365 7320 696e 2074 6578  responses in tex
+00002080: 7475 616c 2066 6f72 6d61 7473 0a20 2020  tual formats.   
+00002090: 2020 2020 2020 2020 7769 6c6c 2062 6520          will be 
+000020a0: 636f 6d70 7265 7373 6564 2061 7574 6f6d  compressed autom
+000020b0: 6174 6963 616c 6c79 2e20 204e 6577 2069  atically.  New i
+000020c0: 6e20 546f 726e 6164 6f20 342e 302e 0a20  n Tornado 4.0.. 
+000020d0: 2020 2020 2020 2020 2a20 6060 677a 6970          * ``gzip
+000020e0: 6060 3a20 4465 7072 6563 6174 6564 2061  ``: Deprecated a
+000020f0: 6c69 6173 2066 6f72 2060 6063 6f6d 7072  lias for ``compr
+00002100: 6573 735f 7265 7370 6f6e 7365 6060 2073  ess_response`` s
+00002110: 696e 6365 0a20 2020 2020 2020 2020 2020  ince.           
+00002120: 546f 726e 6164 6f20 342e 302e 0a20 2020  Tornado 4.0..   
+00002130: 2020 2020 2020 2a20 6060 6c6f 675f 6675        * ``log_fu
+00002140: 6e63 7469 6f6e 6060 3a20 5468 6973 2066  nction``: This f
+00002150: 756e 6374 696f 6e20 7769 6c6c 2062 6520  unction will be 
+00002160: 6361 6c6c 6564 2061 7420 7468 6520 656e  called at the en
+00002170: 640a 2020 2020 2020 2020 2020 206f 6620  d.           of 
+00002180: 6576 6572 7920 7265 7175 6573 7420 746f  every request to
+00002190: 206c 6f67 2074 6865 2072 6573 756c 7420   log the result 
+000021a0: 2877 6974 6820 6f6e 6520 6172 6775 6d65  (with one argume
+000021b0: 6e74 2c20 7468 650a 2020 2020 2020 2020  nt, the.        
+000021c0: 2020 2060 5265 7175 6573 7448 616e 646c     `RequestHandl
+000021d0: 6572 6020 6f62 6a65 6374 292e 2020 5468  er` object).  Th
+000021e0: 6520 6465 6661 756c 7420 696d 706c 656d  e default implem
+000021f0: 656e 7461 7469 6f6e 0a20 2020 2020 2020  entation.       
+00002200: 2020 2020 7772 6974 6573 2074 6f20 7468      writes to th
+00002210: 6520 606c 6f67 6769 6e67 6020 6d6f 6475  e `logging` modu
+00002220: 6c65 2773 2072 6f6f 7420 6c6f 6767 6572  le's root logger
+00002230: 2e20 204d 6179 2061 6c73 6f20 6265 0a20  .  May also be. 
+00002240: 2020 2020 2020 2020 2020 6375 7374 6f6d            custom
+00002250: 697a 6564 2062 7920 6f76 6572 7269 6469  ized by overridi
+00002260: 6e67 2060 4170 706c 6963 6174 696f 6e2e  ng `Application.
+00002270: 6c6f 675f 7265 7175 6573 7460 2e0a 2020  log_request`..  
+00002280: 2020 2020 2020 202a 2060 6073 6572 7665         * ``serve
+00002290: 5f74 7261 6365 6261 636b 6060 3a20 4966  _traceback``: If
+000022a0: 2060 6054 7275 6560 602c 2074 6865 2064   ``True``, the d
+000022b0: 6566 6175 6c74 2065 7272 6f72 2070 6167  efault error pag
+000022c0: 650a 2020 2020 2020 2020 2020 2077 696c  e.           wil
+000022d0: 6c20 696e 636c 7564 6520 7468 6520 7472  l include the tr
+000022e0: 6163 6562 6163 6b20 6f66 2074 6865 2065  aceback of the e
+000022f0: 7272 6f72 2e20 2054 6869 7320 6f70 7469  rror.  This opti
+00002300: 6f6e 2069 7320 6e65 7720 696e 0a20 2020  on is new in.   
+00002310: 2020 2020 2020 2020 546f 726e 6164 6f20          Tornado 
+00002320: 332e 323b 2070 7265 7669 6f75 736c 7920  3.2; previously 
+00002330: 7468 6973 2066 756e 6374 696f 6e61 6c69  this functionali
+00002340: 7479 2077 6173 2063 6f6e 7472 6f6c 6c65  ty was controlle
+00002350: 6420 6279 0a20 2020 2020 2020 2020 2020  d by.           
+00002360: 7468 6520 6060 6465 6275 6760 6020 7365  the ``debug`` se
+00002370: 7474 696e 672e 0a20 2020 2020 2020 2020  tting..         
+00002380: 2a20 6060 7569 5f6d 6f64 756c 6573 6060  * ``ui_modules``
+00002390: 2061 6e64 2060 6075 695f 6d65 7468 6f64   and ``ui_method
+000023a0: 7360 603a 204d 6179 2062 6520 7365 7420  s``: May be set 
+000023b0: 746f 2061 206d 6170 7069 6e67 0a20 2020  to a mapping.   
+000023c0: 2020 2020 2020 2020 6f66 2060 5549 4d6f          of `UIMo
+000023d0: 6475 6c65 6020 6f72 2055 4920 6d65 7468  dule` or UI meth
+000023e0: 6f64 7320 746f 2062 6520 6d61 6465 2061  ods to be made a
+000023f0: 7661 696c 6162 6c65 2074 6f20 7465 6d70  vailable to temp
+00002400: 6c61 7465 732e 0a20 2020 2020 2020 2020  lates..         
+00002410: 2020 4d61 7920 6265 2073 6574 2074 6f20    May be set to 
+00002420: 6120 6d6f 6475 6c65 2c20 6469 6374 696f  a module, dictio
+00002430: 6e61 7279 2c20 6f72 2061 206c 6973 7420  nary, or a list 
+00002440: 6f66 206d 6f64 756c 6573 0a20 2020 2020  of modules.     
+00002450: 2020 2020 2020 616e 642f 6f72 2064 6963        and/or dic
+00002460: 7473 2e20 2053 6565 203a 7265 663a 6075  ts.  See :ref:`u
+00002470: 692d 6d6f 6475 6c65 7360 2066 6f72 206d  i-modules` for m
+00002480: 6f72 6520 6465 7461 696c 732e 0a20 2020  ore details..   
+00002490: 2020 2020 2020 2a20 6060 7765 6273 6f63        * ``websoc
+000024a0: 6b65 745f 7069 6e67 5f69 6e74 6572 7661  ket_ping_interva
+000024b0: 6c60 603a 2049 6620 7365 7420 746f 2061  l``: If set to a
+000024c0: 206e 756d 6265 722c 2061 6c6c 2077 6562   number, all web
+000024d0: 736f 636b 6574 7320 7769 6c6c 0a20 2020  sockets will.   
+000024e0: 2020 2020 2020 2020 6265 2070 696e 6765          be pinge
+000024f0: 6420 6576 6572 7920 6e20 7365 636f 6e64  d every n second
+00002500: 732e 2054 6869 7320 6361 6e20 6865 6c70  s. This can help
+00002510: 206b 6565 7020 7468 6520 636f 6e6e 6563   keep the connec
+00002520: 7469 6f6e 2061 6c69 7665 0a20 2020 2020  tion alive.     
+00002530: 2020 2020 2020 7468 726f 7567 6820 6365        through ce
+00002540: 7274 6169 6e20 7072 6f78 7920 7365 7276  rtain proxy serv
+00002550: 6572 7320 7768 6963 6820 636c 6f73 6520  ers which close 
+00002560: 6964 6c65 2063 6f6e 6e65 6374 696f 6e73  idle connections
+00002570: 2c20 616e 6420 6974 0a20 2020 2020 2020  , and it.       
+00002580: 2020 2020 6361 6e20 6465 7465 6374 2069      can detect i
+00002590: 6620 7468 6520 7765 6273 6f63 6b65 7420  f the websocket 
+000025a0: 6861 7320 6661 696c 6564 2077 6974 686f  has failed witho
+000025b0: 7574 2062 6569 6e67 2070 726f 7065 726c  ut being properl
+000025c0: 7920 636c 6f73 6564 2e0a 2020 2020 2020  y closed..      
+000025d0: 2020 202a 2060 6077 6562 736f 636b 6574     * ``websocket
+000025e0: 5f70 696e 675f 7469 6d65 6f75 7460 603a  _ping_timeout``:
+000025f0: 2049 6620 7468 6520 7069 6e67 2069 6e74   If the ping int
+00002600: 6572 7661 6c20 6973 2073 6574 2c20 616e  erval is set, an
+00002610: 6420 7468 650a 2020 2020 2020 2020 2020  d the.          
+00002620: 2073 6572 7665 7220 646f 6573 6e27 7420   server doesn't 
+00002630: 7265 6365 6976 6520 6120 2770 6f6e 6727  receive a 'pong'
+00002640: 2069 6e20 7468 6973 206d 616e 7920 7365   in this many se
+00002650: 636f 6e64 732c 2069 7420 7769 6c6c 2063  conds, it will c
+00002660: 6c6f 7365 0a20 2020 2020 2020 2020 2020  lose.           
+00002670: 7468 6520 7765 6273 6f63 6b65 742e 2054  the websocket. T
+00002680: 6865 2064 6566 6175 6c74 2069 7320 7468  he default is th
+00002690: 7265 6520 7469 6d65 7320 7468 6520 7069  ree times the pi
+000026a0: 6e67 2069 6e74 6572 7661 6c2c 2077 6974  ng interval, wit
+000026b0: 6820 610a 2020 2020 2020 2020 2020 206d  h a.           m
+000026c0: 696e 696d 756d 206f 6620 3330 2073 6563  inimum of 30 sec
+000026d0: 6f6e 6473 2e20 4967 6e6f 7265 6420 6966  onds. Ignored if
+000026e0: 2074 6865 2070 696e 6720 696e 7465 7276   the ping interv
+000026f0: 616c 2069 7320 6e6f 7420 7365 742e 0a0a  al is not set...
+00002700: 2020 2020 2020 2020 2041 7574 6865 6e74           Authent
+00002710: 6963 6174 696f 6e20 616e 6420 7365 6375  ication and secu
+00002720: 7269 7479 2073 6574 7469 6e67 733a 0a0a  rity settings:..
+00002730: 2020 2020 2020 2020 202a 2060 6063 6f6f           * ``coo
+00002740: 6b69 655f 7365 6372 6574 6060 3a20 5573  kie_secret``: Us
+00002750: 6564 2062 7920 6052 6571 7565 7374 4861  ed by `RequestHa
+00002760: 6e64 6c65 722e 6765 745f 7369 676e 6564  ndler.get_signed
+00002770: 5f63 6f6f 6b69 6560 0a20 2020 2020 2020  _cookie`.       
+00002780: 2020 2020 616e 6420 602e 7365 745f 7369      and `.set_si
+00002790: 676e 6564 5f63 6f6f 6b69 6560 2074 6f20  gned_cookie` to 
+000027a0: 7369 676e 2063 6f6f 6b69 6573 2e0a 2020  sign cookies..  
+000027b0: 2020 2020 2020 202a 2060 606b 6579 5f76         * ``key_v
+000027c0: 6572 7369 6f6e 6060 3a20 5573 6564 2062  ersion``: Used b
+000027d0: 7920 7265 7175 6573 7448 616e 646c 6572  y requestHandler
+000027e0: 2060 2e73 6574 5f73 6967 6e65 645f 636f   `.set_signed_co
+000027f0: 6f6b 6965 600a 2020 2020 2020 2020 2020  okie`.          
+00002800: 2074 6f20 7369 676e 2063 6f6f 6b69 6573   to sign cookies
+00002810: 2077 6974 6820 6120 7370 6563 6966 6963   with a specific
+00002820: 206b 6579 2077 6865 6e20 6060 636f 6f6b   key when ``cook
+00002830: 6965 5f73 6563 7265 7460 600a 2020 2020  ie_secret``.    
+00002840: 2020 2020 2020 2069 7320 6120 6b65 7920         is a key 
+00002850: 6469 6374 696f 6e61 7279 2e0a 2020 2020  dictionary..    
+00002860: 2020 2020 202a 2060 606c 6f67 696e 5f75       * ``login_u
+00002870: 726c 6060 3a20 5468 6520 6061 7574 6865  rl``: The `authe
+00002880: 6e74 6963 6174 6564 6020 6465 636f 7261  nticated` decora
+00002890: 746f 7220 7769 6c6c 2072 6564 6972 6563  tor will redirec
+000028a0: 740a 2020 2020 2020 2020 2020 2074 6f20  t.           to 
+000028b0: 7468 6973 2075 726c 2069 6620 7468 6520  this url if the 
+000028c0: 7573 6572 2069 7320 6e6f 7420 6c6f 6767  user is not logg
+000028d0: 6564 2069 6e2e 2020 4361 6e20 6265 2066  ed in.  Can be f
+000028e0: 7572 7468 6572 0a20 2020 2020 2020 2020  urther.         
+000028f0: 2020 6375 7374 6f6d 697a 6564 2062 7920    customized by 
+00002900: 6f76 6572 7269 6469 6e67 2060 5265 7175  overriding `Requ
+00002910: 6573 7448 616e 646c 6572 2e67 6574 5f6c  estHandler.get_l
+00002920: 6f67 696e 5f75 726c 600a 2020 2020 2020  ogin_url`.      
+00002930: 2020 202a 2060 6078 7372 665f 636f 6f6b     * ``xsrf_cook
+00002940: 6965 7360 603a 2049 6620 6060 5472 7565  ies``: If ``True
+00002950: 6060 2c20 3a72 6566 3a60 7873 7266 6020  ``, :ref:`xsrf` 
+00002960: 7769 6c6c 2062 6520 656e 6162 6c65 642e  will be enabled.
+00002970: 0a20 2020 2020 2020 2020 2a20 6060 7873  .         * ``xs
+00002980: 7266 5f63 6f6f 6b69 655f 7665 7273 696f  rf_cookie_versio
+00002990: 6e60 603a 2043 6f6e 7472 6f6c 7320 7468  n``: Controls th
+000029a0: 6520 7665 7273 696f 6e20 6f66 206e 6577  e version of new
+000029b0: 2058 5352 460a 2020 2020 2020 2020 2020   XSRF.          
+000029c0: 2063 6f6f 6b69 6573 2070 726f 6475 6365   cookies produce
+000029d0: 6420 6279 2074 6869 7320 7365 7276 6572  d by this server
+000029e0: 2e20 2053 686f 756c 6420 6765 6e65 7261  .  Should genera
+000029f0: 6c6c 7920 6265 206c 6566 740a 2020 2020  lly be left.    
+00002a00: 2020 2020 2020 2061 7420 7468 6520 6465         at the de
+00002a10: 6661 756c 7420 2877 6869 6368 2077 696c  fault (which wil
+00002a20: 6c20 616c 7761 7973 2062 6520 7468 6520  l always be the 
+00002a30: 6869 6768 6573 7420 7375 7070 6f72 7465  highest supporte
+00002a40: 640a 2020 2020 2020 2020 2020 2076 6572  d.           ver
+00002a50: 7369 6f6e 292c 2062 7574 206d 6179 2062  sion), but may b
+00002a60: 6520 7365 7420 746f 2061 206c 6f77 6572  e set to a lower
+00002a70: 2076 616c 7565 2074 656d 706f 7261 7269   value temporari
+00002a80: 6c79 0a20 2020 2020 2020 2020 2020 6475  ly.           du
+00002a90: 7269 6e67 2076 6572 7369 6f6e 2074 7261  ring version tra
+00002aa0: 6e73 6974 696f 6e73 2e20 204e 6577 2069  nsitions.  New i
+00002ab0: 6e20 546f 726e 6164 6f20 332e 322e 322c  n Tornado 3.2.2,
+00002ac0: 2077 6869 6368 0a20 2020 2020 2020 2020   which.         
+00002ad0: 2020 696e 7472 6f64 7563 6564 2058 5352    introduced XSR
+00002ae0: 4620 636f 6f6b 6965 2076 6572 7369 6f6e  F cookie version
+00002af0: 2032 2e0a 2020 2020 2020 2020 202a 2060   2..         * `
+00002b00: 6078 7372 665f 636f 6f6b 6965 5f6b 7761  `xsrf_cookie_kwa
+00002b10: 7267 7360 603a 204d 6179 2062 6520 7365  rgs``: May be se
+00002b20: 7420 746f 2061 2064 6963 7469 6f6e 6172  t to a dictionar
+00002b30: 7920 6f66 0a20 2020 2020 2020 2020 2020  y of.           
+00002b40: 6164 6469 7469 6f6e 616c 2061 7267 756d  additional argum
+00002b50: 656e 7473 2074 6f20 6265 2070 6173 7365  ents to be passe
+00002b60: 6420 746f 2060 2e52 6571 7565 7374 4861  d to `.RequestHa
+00002b70: 6e64 6c65 722e 7365 745f 636f 6f6b 6965  ndler.set_cookie
+00002b80: 600a 2020 2020 2020 2020 2020 2066 6f72  `.           for
+00002b90: 2074 6865 2058 5352 4620 636f 6f6b 6965   the XSRF cookie
+00002ba0: 2e0a 2020 2020 2020 2020 202a 2060 6078  ..         * ``x
+00002bb0: 7372 665f 636f 6f6b 6965 5f6e 616d 6560  srf_cookie_name`
+00002bc0: 603a 2043 6f6e 7472 6f6c 7320 7468 6520  `: Controls the 
+00002bd0: 6e61 6d65 2075 7365 6420 666f 7220 7468  name used for th
+00002be0: 6520 5853 5246 0a20 2020 2020 2020 2020  e XSRF.         
+00002bf0: 2020 636f 6f6b 6965 2028 6465 6661 756c    cookie (defaul
+00002c00: 7420 6060 5f78 7372 6660 6029 2e20 5468  t ``_xsrf``). Th
+00002c10: 6520 696e 7465 6e64 6564 2075 7365 2069  e intended use i
+00002c20: 7320 746f 2074 616b 650a 2020 2020 2020  s to take.      
+00002c30: 2020 2020 2061 6476 616e 7461 6765 206f       advantage o
+00002c40: 6620 6063 6f6f 6b69 6520 7072 6566 6978  f `cookie prefix
+00002c50: 6573 605f 2e20 4e6f 7465 2074 6861 7420  es`_. Note that 
+00002c60: 636f 6f6b 6965 2070 7265 6669 7865 730a  cookie prefixes.
+00002c70: 2020 2020 2020 2020 2020 2069 6e74 6572             inter
+00002c80: 6163 7420 7769 7468 206f 7468 6572 2063  act with other c
+00002c90: 6f6f 6b69 6520 666c 6167 732c 2073 6f20  ookie flags, so 
+00002ca0: 7468 6579 206d 7573 7420 6265 2063 6f6d  they must be com
+00002cb0: 6269 6e65 640a 2020 2020 2020 2020 2020  bined.          
+00002cc0: 2077 6974 6820 6060 7873 7266 5f63 6f6f   with ``xsrf_coo
+00002cd0: 6b69 655f 6b77 6172 6773 6060 2c20 7375  kie_kwargs``, su
+00002ce0: 6368 2061 730a 2020 2020 2020 2020 2020  ch as.          
+00002cf0: 2060 607b 2278 7372 665f 636f 6f6b 6965   ``{"xsrf_cookie
+00002d00: 5f6e 616d 6522 3a20 225f 5f48 6f73 742d  _name": "__Host-
+00002d10: 7873 7266 222c 2022 7873 7266 5f63 6f6f  xsrf", "xsrf_coo
+00002d20: 6b69 655f 6b77 6172 6773 223a 0a20 2020  kie_kwargs":.   
+00002d30: 2020 2020 2020 2020 7b22 7365 6375 7265          {"secure
+00002d40: 223a 2054 7275 657d 7d60 600a 2020 2020  ": True}}``.    
+00002d50: 2020 2020 202a 2060 6074 7769 7474 6572       * ``twitter
+00002d60: 5f63 6f6e 7375 6d65 725f 6b65 7960 602c  _consumer_key``,
+00002d70: 2060 6074 7769 7474 6572 5f63 6f6e 7375   ``twitter_consu
+00002d80: 6d65 725f 7365 6372 6574 6060 2c0a 2020  mer_secret``,.  
+00002d90: 2020 2020 2020 2020 2060 6066 7269 656e           ``frien
+00002da0: 6466 6565 645f 636f 6e73 756d 6572 5f6b  dfeed_consumer_k
+00002db0: 6579 6060 2c20 6060 6672 6965 6e64 6665  ey``, ``friendfe
+00002dc0: 6564 5f63 6f6e 7375 6d65 725f 7365 6372  ed_consumer_secr
+00002dd0: 6574 6060 2c0a 2020 2020 2020 2020 2020  et``,.          
+00002de0: 2060 6067 6f6f 676c 655f 636f 6e73 756d   ``google_consum
+00002df0: 6572 5f6b 6579 6060 2c20 6060 676f 6f67  er_key``, ``goog
+00002e00: 6c65 5f63 6f6e 7375 6d65 725f 7365 6372  le_consumer_secr
+00002e10: 6574 6060 2c0a 2020 2020 2020 2020 2020  et``,.          
+00002e20: 2060 6066 6163 6562 6f6f 6b5f 6170 695f   ``facebook_api_
+00002e30: 6b65 7960 602c 2060 6066 6163 6562 6f6f  key``, ``faceboo
+00002e40: 6b5f 7365 6372 6574 6060 3a20 2055 7365  k_secret``:  Use
+00002e50: 6420 696e 2074 6865 0a20 2020 2020 2020  d in the.       
+00002e60: 2020 2020 6074 6f72 6e61 646f 2e61 7574      `tornado.aut
+00002e70: 6860 206d 6f64 756c 6520 746f 2061 7574  h` module to aut
+00002e80: 6865 6e74 6963 6174 6520 746f 2076 6172  henticate to var
+00002e90: 696f 7573 2041 5049 732e 0a0a 2020 2020  ious APIs...    
+00002ea0: 2020 2020 202e 2e20 5f63 6f6f 6b69 6520       .. _cookie 
+00002eb0: 7072 6566 6978 6573 3a20 6874 7470 733a  prefixes: https:
+00002ec0: 2f2f 6465 7665 6c6f 7065 722e 6d6f 7a69  //developer.mozi
+00002ed0: 6c6c 612e 6f72 672f 656e 2d55 532f 646f  lla.org/en-US/do
+00002ee0: 6373 2f57 6562 2f48 5454 502f 4865 6164  cs/Web/HTTP/Head
+00002ef0: 6572 732f 5365 742d 436f 6f6b 6965 2363  ers/Set-Cookie#c
+00002f00: 6f6f 6b69 655f 7072 6566 6978 6573 0a0a  ookie_prefixes..
+00002f10: 2020 2020 2020 2020 2054 656d 706c 6174           Templat
+00002f20: 6520 7365 7474 696e 6773 3a0a 0a20 2020  e settings:..   
+00002f30: 2020 2020 2020 2a20 6060 6175 746f 6573        * ``autoes
+00002f40: 6361 7065 6060 3a20 436f 6e74 726f 6c73  cape``: Controls
+00002f50: 2061 7574 6f6d 6174 6963 2065 7363 6170   automatic escap
+00002f60: 696e 6720 666f 7220 7465 6d70 6c61 7465  ing for template
+00002f70: 732e 0a20 2020 2020 2020 2020 2020 4d61  s..           Ma
+00002f80: 7920 6265 2073 6574 2074 6f20 6060 4e6f  y be set to ``No
+00002f90: 6e65 6060 2074 6f20 6469 7361 626c 6520  ne`` to disable 
+00002fa0: 6573 6361 7069 6e67 2c20 6f72 2074 6f20  escaping, or to 
+00002fb0: 7468 6520 2a6e 616d 652a 0a20 2020 2020  the *name*.     
+00002fc0: 2020 2020 2020 6f66 2061 2066 756e 6374        of a funct
+00002fd0: 696f 6e20 7468 6174 2061 6c6c 206f 7574  ion that all out
+00002fe0: 7075 7420 7368 6f75 6c64 2062 6520 7061  put should be pa
+00002ff0: 7373 6564 2074 6872 6f75 6768 2e0a 2020  ssed through..  
+00003000: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
+00003010: 7320 746f 2060 6022 7868 746d 6c5f 6573  s to ``"xhtml_es
+00003020: 6361 7065 2260 602e 2020 4361 6e20 6265  cape"``.  Can be
+00003030: 2063 6861 6e67 6564 206f 6e20 6120 7065   changed on a pe
+00003040: 722d 7465 6d70 6c61 7465 0a20 2020 2020  r-template.     
+00003050: 2020 2020 2020 6261 7369 7320 7769 7468        basis with
+00003060: 2074 6865 2060 607b 2520 6175 746f 6573   the ``{% autoes
+00003070: 6361 7065 2025 7d60 6020 6469 7265 6374  cape %}`` direct
+00003080: 6976 652e 0a20 2020 2020 2020 2020 2a20  ive..         * 
+00003090: 6060 636f 6d70 696c 6564 5f74 656d 706c  ``compiled_templ
+000030a0: 6174 655f 6361 6368 6560 603a 2044 6566  ate_cache``: Def
+000030b0: 6175 6c74 2069 7320 6060 5472 7565 6060  ault is ``True``
+000030c0: 3b20 6966 2060 6046 616c 7365 6060 0a20  ; if ``False``. 
+000030d0: 2020 2020 2020 2020 2020 7465 6d70 6c61            templa
+000030e0: 7465 7320 7769 6c6c 2062 6520 7265 636f  tes will be reco
+000030f0: 6d70 696c 6564 206f 6e20 6576 6572 7920  mpiled on every 
+00003100: 7265 7175 6573 742e 2020 5468 6973 206f  request.  This o
+00003110: 7074 696f 6e0a 2020 2020 2020 2020 2020  ption.          
+00003120: 2069 7320 6e65 7720 696e 2054 6f72 6e61   is new in Torna
+00003130: 646f 2033 2e32 3b20 7072 6576 696f 7573  do 3.2; previous
+00003140: 6c79 2074 6869 7320 6675 6e63 7469 6f6e  ly this function
+00003150: 616c 6974 7920 7761 7320 636f 6e74 726f  ality was contro
+00003160: 6c6c 6564 0a20 2020 2020 2020 2020 2020  lled.           
+00003170: 6279 2074 6865 2060 6064 6562 7567 6060  by the ``debug``
+00003180: 2073 6574 7469 6e67 2e0a 2020 2020 2020   setting..      
+00003190: 2020 202a 2060 6074 656d 706c 6174 655f     * ``template_
+000031a0: 7061 7468 6060 3a20 4469 7265 6374 6f72  path``: Director
+000031b0: 7920 636f 6e74 6169 6e69 6e67 2074 656d  y containing tem
+000031c0: 706c 6174 6520 6669 6c65 732e 2020 4361  plate files.  Ca
+000031d0: 6e20 6265 0a20 2020 2020 2020 2020 2020  n be.           
+000031e0: 6675 7274 6865 7220 6375 7374 6f6d 697a  further customiz
+000031f0: 6564 2062 7920 6f76 6572 7269 6469 6e67  ed by overriding
+00003200: 2060 5265 7175 6573 7448 616e 646c 6572   `RequestHandler
+00003210: 2e67 6574 5f74 656d 706c 6174 655f 7061  .get_template_pa
+00003220: 7468 600a 2020 2020 2020 2020 202a 2060  th`.         * `
+00003230: 6074 656d 706c 6174 655f 6c6f 6164 6572  `template_loader
+00003240: 6060 3a20 4173 7369 676e 2074 6f20 616e  ``: Assign to an
+00003250: 2069 6e73 7461 6e63 6520 6f66 0a20 2020   instance of.   
+00003260: 2020 2020 2020 2020 6074 6f72 6e61 646f          `tornado
+00003270: 2e74 656d 706c 6174 652e 4261 7365 4c6f  .template.BaseLo
+00003280: 6164 6572 6020 746f 2063 7573 746f 6d69  ader` to customi
+00003290: 7a65 2074 656d 706c 6174 6520 6c6f 6164  ze template load
+000032a0: 696e 672e 0a20 2020 2020 2020 2020 2020  ing..           
+000032b0: 4966 2074 6869 7320 7365 7474 696e 6720  If this setting 
+000032c0: 6973 2075 7365 6420 7468 6520 6060 7465  is used the ``te
+000032d0: 6d70 6c61 7465 5f70 6174 6860 6020 616e  mplate_path`` an
+000032e0: 6420 6060 6175 746f 6573 6361 7065 6060  d ``autoescape``
+000032f0: 0a20 2020 2020 2020 2020 2020 7365 7474  .           sett
+00003300: 696e 6773 2061 7265 2069 676e 6f72 6564  ings are ignored
+00003310: 2e20 2043 616e 2062 6520 6675 7274 6865  .  Can be furthe
+00003320: 7220 6375 7374 6f6d 697a 6564 2062 7920  r customized by 
+00003330: 6f76 6572 7269 6469 6e67 0a20 2020 2020  overriding.     
+00003340: 2020 2020 2020 6052 6571 7565 7374 4861        `RequestHa
+00003350: 6e64 6c65 722e 6372 6561 7465 5f74 656d  ndler.create_tem
+00003360: 706c 6174 655f 6c6f 6164 6572 602e 0a20  plate_loader`.. 
+00003370: 2020 2020 2020 2020 2a20 6060 7465 6d70          * ``temp
+00003380: 6c61 7465 5f77 6869 7465 7370 6163 6560  late_whitespace`
+00003390: 603a 2043 6f6e 7472 6f6c 7320 6861 6e64  `: Controls hand
+000033a0: 6c69 6e67 206f 6620 7768 6974 6573 7061  ling of whitespa
+000033b0: 6365 2069 6e0a 2020 2020 2020 2020 2020  ce in.          
+000033c0: 2074 656d 706c 6174 6573 3b20 7365 6520   templates; see 
+000033d0: 6074 6f72 6e61 646f 2e74 656d 706c 6174  `tornado.templat
+000033e0: 652e 6669 6c74 6572 5f77 6869 7465 7370  e.filter_whitesp
+000033f0: 6163 6560 2066 6f72 2061 6c6c 6f77 6564  ace` for allowed
+00003400: 0a20 2020 2020 2020 2020 2020 7661 6c75  .           valu
+00003410: 6573 2e20 4e65 7720 696e 2054 6f72 6e61  es. New in Torna
+00003420: 646f 2034 2e33 2e0a 0a20 2020 2020 2020  do 4.3...       
+00003430: 2020 5374 6174 6963 2066 696c 6520 7365    Static file se
+00003440: 7474 696e 6773 3a0a 0a20 2020 2020 2020  ttings:..       
+00003450: 2020 2a20 6060 7374 6174 6963 5f68 6173    * ``static_has
+00003460: 685f 6361 6368 6560 603a 2044 6566 6175  h_cache``: Defau
+00003470: 6c74 2069 7320 6060 5472 7565 6060 3b20  lt is ``True``; 
+00003480: 6966 2060 6046 616c 7365 6060 0a20 2020  if ``False``.   
+00003490: 2020 2020 2020 2020 7374 6174 6963 2075          static u
+000034a0: 726c 7320 7769 6c6c 2062 6520 7265 636f  rls will be reco
+000034b0: 6d70 7574 6564 206f 6e20 6576 6572 7920  mputed on every 
+000034c0: 7265 7175 6573 742e 2020 5468 6973 206f  request.  This o
+000034d0: 7074 696f 6e0a 2020 2020 2020 2020 2020  ption.          
+000034e0: 2069 7320 6e65 7720 696e 2054 6f72 6e61   is new in Torna
+000034f0: 646f 2033 2e32 3b20 7072 6576 696f 7573  do 3.2; previous
+00003500: 6c79 2074 6869 7320 6675 6e63 7469 6f6e  ly this function
+00003510: 616c 6974 7920 7761 7320 636f 6e74 726f  ality was contro
+00003520: 6c6c 6564 0a20 2020 2020 2020 2020 2020  lled.           
+00003530: 6279 2074 6865 2060 6064 6562 7567 6060  by the ``debug``
+00003540: 2073 6574 7469 6e67 2e0a 2020 2020 2020   setting..      
+00003550: 2020 202a 2060 6073 7461 7469 635f 7061     * ``static_pa
+00003560: 7468 6060 3a20 4469 7265 6374 6f72 7920  th``: Directory 
+00003570: 6672 6f6d 2077 6869 6368 2073 7461 7469  from which stati
+00003580: 6320 6669 6c65 7320 7769 6c6c 2062 650a  c files will be.
+00003590: 2020 2020 2020 2020 2020 2073 6572 7665             serve
+000035a0: 642e 0a20 2020 2020 2020 2020 2a20 6060  d..         * ``
+000035b0: 7374 6174 6963 5f75 726c 5f70 7265 6669  static_url_prefi
+000035c0: 7860 603a 2020 5572 6c20 7072 6566 6978  x``:  Url prefix
+000035d0: 2066 6f72 2073 7461 7469 6320 6669 6c65   for static file
+000035e0: 732c 0a20 2020 2020 2020 2020 2020 6465  s,.           de
+000035f0: 6661 756c 7473 2074 6f20 6060 222f 7374  faults to ``"/st
+00003600: 6174 6963 2f22 6060 2e0a 2020 2020 2020  atic/"``..      
+00003610: 2020 202a 2060 6073 7461 7469 635f 6861     * ``static_ha
+00003620: 6e64 6c65 725f 636c 6173 7360 602c 2060  ndler_class``, `
+00003630: 6073 7461 7469 635f 6861 6e64 6c65 725f  `static_handler_
+00003640: 6172 6773 6060 3a20 4d61 7920 6265 2073  args``: May be s
+00003650: 6574 2074 6f0a 2020 2020 2020 2020 2020  et to.          
+00003660: 2075 7365 2061 2064 6966 6665 7265 6e74   use a different
+00003670: 2068 616e 646c 6572 2066 6f72 2073 7461   handler for sta
+00003680: 7469 6320 6669 6c65 7320 696e 7374 6561  tic files instea
+00003690: 6420 6f66 2074 6865 2064 6566 6175 6c74  d of the default
+000036a0: 0a20 2020 2020 2020 2020 2020 6074 6f72  .           `tor
+000036b0: 6e61 646f 2e77 6562 2e53 7461 7469 6346  nado.web.StaticF
+000036c0: 696c 6548 616e 646c 6572 602e 2020 6060  ileHandler`.  ``
+000036d0: 7374 6174 6963 5f68 616e 646c 6572 5f61  static_handler_a
+000036e0: 7267 7360 602c 2069 6620 7365 742c 0a20  rgs``, if set,. 
+000036f0: 2020 2020 2020 2020 2020 7368 6f75 6c64            should
+00003700: 2062 6520 6120 6469 6374 696f 6e61 7279   be a dictionary
+00003710: 206f 6620 6b65 7977 6f72 6420 6172 6775   of keyword argu
+00003720: 6d65 6e74 7320 746f 2062 6520 7061 7373  ments to be pass
+00003730: 6564 2074 6f20 7468 650a 2020 2020 2020  ed to the.      
+00003740: 2020 2020 2068 616e 646c 6572 2773 2060       handler's `
+00003750: 6069 6e69 7469 616c 697a 6560 6020 6d65  `initialize`` me
+00003760: 7468 6f64 2e0a 0a20 2020 2e2e 2061 7574  thod...   .. aut
+00003770: 6f6d 6574 686f 643a 3a20 4170 706c 6963  omethod:: Applic
+00003780: 6174 696f 6e2e 6c69 7374 656e 0a20 2020  ation.listen.   
+00003790: 2e2e 2061 7574 6f6d 6574 686f 643a 3a20  .. automethod:: 
+000037a0: 4170 706c 6963 6174 696f 6e2e 6164 645f  Application.add_
+000037b0: 6861 6e64 6c65 7273 2868 616e 646c 6572  handlers(handler
+000037c0: 733a 204c 6973 745b 556e 696f 6e5b 5275  s: List[Union[Ru
+000037d0: 6c65 2c20 5475 706c 655d 5d29 0a20 2020  le, Tuple]]).   
+000037e0: 2e2e 2061 7574 6f6d 6574 686f 643a 3a20  .. automethod:: 
+000037f0: 4170 706c 6963 6174 696f 6e2e 6765 745f  Application.get_
+00003800: 6861 6e64 6c65 725f 6465 6c65 6761 7465  handler_delegate
+00003810: 0a20 2020 2e2e 2061 7574 6f6d 6574 686f  .   .. autometho
+00003820: 643a 3a20 4170 706c 6963 6174 696f 6e2e  d:: Application.
+00003830: 7265 7665 7273 655f 7572 6c0a 2020 202e  reverse_url.   .
+00003840: 2e20 6175 746f 6d65 7468 6f64 3a3a 2041  . automethod:: A
+00003850: 7070 6c69 6361 7469 6f6e 2e6c 6f67 5f72  pplication.log_r
+00003860: 6571 7565 7374 0a0a 2020 202e 2e20 6175  equest..   .. au
+00003870: 746f 636c 6173 733a 3a20 5552 4c53 7065  toclass:: URLSpe
+00003880: 630a 0a20 2020 2020 2054 6865 2060 6055  c..      The ``U
+00003890: 524c 5370 6563 6060 2063 6c61 7373 2069  RLSpec`` class i
+000038a0: 7320 616c 736f 2061 7661 696c 6162 6c65  s also available
+000038b0: 2075 6e64 6572 2074 6865 206e 616d 6520   under the name 
+000038c0: 6060 746f 726e 6164 6f2e 7765 622e 7572  ``tornado.web.ur
+000038d0: 6c60 602e 0a0a 2020 2044 6563 6f72 6174  l``...   Decorat
+000038e0: 6f72 730a 2020 202d 2d2d 2d2d 2d2d 2d2d  ors.   ---------
+000038f0: 2d0a 2020 202e 2e20 6175 746f 6675 6e63  -.   .. autofunc
+00003900: 7469 6f6e 3a3a 2061 7574 6865 6e74 6963  tion:: authentic
+00003910: 6174 6564 0a20 2020 2e2e 2061 7574 6f66  ated.   .. autof
+00003920: 756e 6374 696f 6e3a 3a20 6164 6473 6c61  unction:: addsla
+00003930: 7368 0a20 2020 2e2e 2061 7574 6f66 756e  sh.   .. autofun
+00003940: 6374 696f 6e3a 3a20 7265 6d6f 7665 736c  ction:: removesl
+00003950: 6173 680a 2020 202e 2e20 6175 746f 6675  ash.   .. autofu
+00003960: 6e63 7469 6f6e 3a3a 2073 7472 6561 6d5f  nction:: stream_
+00003970: 7265 7175 6573 745f 626f 6479 0a0a 2020  request_body..  
+00003980: 2045 7665 7279 7468 696e 6720 656c 7365   Everything else
+00003990: 0a20 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .   ------------
+000039a0: 2d2d 2d0a 2020 202e 2e20 6175 746f 6578  ---.   .. autoex
+000039b0: 6365 7074 696f 6e3a 3a20 4854 5450 4572  ception:: HTTPEr
+000039c0: 726f 720a 2020 202e 2e20 6175 746f 6578  ror.   .. autoex
+000039d0: 6365 7074 696f 6e3a 3a20 4669 6e69 7368  ception:: Finish
+000039e0: 0a20 2020 2e2e 2061 7574 6f65 7863 6570  .   .. autoexcep
+000039f0: 7469 6f6e 3a3a 204d 6973 7369 6e67 4172  tion:: MissingAr
+00003a00: 6775 6d65 6e74 4572 726f 720a 2020 202e  gumentError.   .
+00003a10: 2e20 6175 746f 636c 6173 733a 3a20 5549  . autoclass:: UI
+00003a20: 4d6f 6475 6c65 0a20 2020 2020 203a 6d65  Module.      :me
+00003a30: 6d62 6572 733a 0a0a 2020 202e 2e20 6175  mbers:..   .. au
+00003a40: 746f 636c 6173 733a 3a20 4572 726f 7248  toclass:: ErrorH
+00003a50: 616e 646c 6572 0a20 2020 2e2e 2061 7574  andler.   .. aut
+00003a60: 6f63 6c61 7373 3a3a 2046 616c 6c62 6163  oclass:: Fallbac
+00003a70: 6b48 616e 646c 6572 0a20 2020 2e2e 2061  kHandler.   .. a
+00003a80: 7574 6f63 6c61 7373 3a3a 2052 6564 6972  utoclass:: Redir
+00003a90: 6563 7448 616e 646c 6572 0a20 2020 2e2e  ectHandler.   ..
+00003aa0: 2061 7574 6f63 6c61 7373 3a3a 2053 7461   autoclass:: Sta
+00003ab0: 7469 6346 696c 6548 616e 646c 6572 0a20  ticFileHandler. 
+00003ac0: 2020 2020 203a 6d65 6d62 6572 733a 0a         :members:.
```

### Comparing `tornado-6.2b2/docs/websocket.rst` & `tornado-6.3b1/docs/websocket.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,72 +4,71 @@
 00000030: 6174 696f 6e20 746f 2074 6865 2062 726f  ation to the bro
 00000040: 7773 6572 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d  wser.===========
 00000050: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00000060: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00000070: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00000080: 3d3d 3d3d 3d3d 3d3d 3d0a 0a2e 2e20 7465  =========.... te
 00000090: 7374 7365 7475 703a 3a0a 0a20 2020 696d  stsetup::..   im
-000000a0: 706f 7274 2074 6f72 6e61 646f 2e77 6562  port tornado.web
-000000b0: 736f 636b 6574 0a0a 2e2e 2061 7574 6f6d  socket.... autom
-000000c0: 6f64 756c 653a 3a20 746f 726e 6164 6f2e  odule:: tornado.
-000000d0: 7765 6273 6f63 6b65 740a 0a20 2020 2e2e  websocket..   ..
-000000e0: 2061 7574 6f63 6c61 7373 3a3a 2057 6562   autoclass:: Web
-000000f0: 536f 636b 6574 4861 6e64 6c65 720a 0a20  SocketHandler.. 
-00000100: 2020 4576 656e 7420 6861 6e64 6c65 7273    Event handlers
-00000110: 0a20 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .   ------------
-00000120: 2d2d 0a0a 2020 202e 2e20 6175 746f 6d65  --..   .. autome
-00000130: 7468 6f64 3a3a 2057 6562 536f 636b 6574  thod:: WebSocket
-00000140: 4861 6e64 6c65 722e 6f70 656e 0a20 2020  Handler.open.   
-00000150: 2e2e 2061 7574 6f6d 6574 686f 643a 3a20  .. automethod:: 
-00000160: 5765 6253 6f63 6b65 7448 616e 646c 6572  WebSocketHandler
-00000170: 2e6f 6e5f 6d65 7373 6167 650a 2020 202e  .on_message.   .
-00000180: 2e20 6175 746f 6d65 7468 6f64 3a3a 2057  . automethod:: W
-00000190: 6562 536f 636b 6574 4861 6e64 6c65 722e  ebSocketHandler.
-000001a0: 6f6e 5f63 6c6f 7365 0a20 2020 2e2e 2061  on_close.   .. a
-000001b0: 7574 6f6d 6574 686f 643a 3a20 5765 6253  utomethod:: WebS
-000001c0: 6f63 6b65 7448 616e 646c 6572 2e73 656c  ocketHandler.sel
-000001d0: 6563 745f 7375 6270 726f 746f 636f 6c0a  ect_subprotocol.
-000001e0: 2020 202e 2e20 6175 746f 6174 7472 6962     .. autoattrib
-000001f0: 7574 653a 3a20 5765 6253 6f63 6b65 7448  ute:: WebSocketH
-00000200: 616e 646c 6572 2e73 656c 6563 7465 645f  andler.selected_
-00000210: 7375 6270 726f 746f 636f 6c0a 2020 202e  subprotocol.   .
-00000220: 2e20 6175 746f 6d65 7468 6f64 3a3a 2057  . automethod:: W
-00000230: 6562 536f 636b 6574 4861 6e64 6c65 722e  ebSocketHandler.
-00000240: 6f6e 5f70 696e 670a 0a20 2020 4f75 7470  on_ping..   Outp
-00000250: 7574 0a20 2020 2d2d 2d2d 2d2d 0a0a 2020  ut.   ------..  
-00000260: 202e 2e20 6175 746f 6d65 7468 6f64 3a3a   .. automethod::
-00000270: 2057 6562 536f 636b 6574 4861 6e64 6c65   WebSocketHandle
-00000280: 722e 7772 6974 655f 6d65 7373 6167 650a  r.write_message.
-00000290: 2020 202e 2e20 6175 746f 6d65 7468 6f64     .. automethod
-000002a0: 3a3a 2057 6562 536f 636b 6574 4861 6e64  :: WebSocketHand
-000002b0: 6c65 722e 636c 6f73 650a 0a20 2020 436f  ler.close..   Co
-000002c0: 6e66 6967 7572 6174 696f 6e0a 2020 202d  nfiguration.   -
-000002d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 2020  ------------..  
-000002e0: 202e 2e20 6175 746f 6d65 7468 6f64 3a3a   .. automethod::
-000002f0: 2057 6562 536f 636b 6574 4861 6e64 6c65   WebSocketHandle
-00000300: 722e 6368 6563 6b5f 6f72 6967 696e 0a20  r.check_origin. 
-00000310: 2020 2e2e 2061 7574 6f6d 6574 686f 643a    .. automethod:
-00000320: 3a20 5765 6253 6f63 6b65 7448 616e 646c  : WebSocketHandl
-00000330: 6572 2e67 6574 5f63 6f6d 7072 6573 7369  er.get_compressi
-00000340: 6f6e 5f6f 7074 696f 6e73 0a20 2020 2e2e  on_options.   ..
-00000350: 2061 7574 6f6d 6574 686f 643a 3a20 5765   automethod:: We
-00000360: 6253 6f63 6b65 7448 616e 646c 6572 2e73  bSocketHandler.s
-00000370: 6574 5f6e 6f64 656c 6179 0a0a 2020 204f  et_nodelay..   O
-00000380: 7468 6572 0a20 2020 2d2d 2d2d 2d0a 0a20  ther.   -----.. 
-00000390: 2020 2e2e 2061 7574 6f6d 6574 686f 643a    .. automethod:
-000003a0: 3a20 5765 6253 6f63 6b65 7448 616e 646c  : WebSocketHandl
-000003b0: 6572 2e70 696e 670a 2020 202e 2e20 6175  er.ping.   .. au
-000003c0: 746f 6d65 7468 6f64 3a3a 2057 6562 536f  tomethod:: WebSo
-000003d0: 636b 6574 4861 6e64 6c65 722e 6f6e 5f70  cketHandler.on_p
-000003e0: 6f6e 670a 2020 202e 2e20 6175 746f 6578  ong.   .. autoex
-000003f0: 6365 7074 696f 6e3a 3a20 5765 6253 6f63  ception:: WebSoc
-00000400: 6b65 7443 6c6f 7365 6445 7272 6f72 0a0a  ketClosedError..
-00000410: 0a20 2020 436c 6965 6e74 2d73 6964 6520  .   Client-side 
-00000420: 7375 7070 6f72 740a 2020 202d 2d2d 2d2d  support.   -----
-00000430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
-00000440: 2020 202e 2e20 6175 746f 6675 6e63 7469     .. autofuncti
-00000450: 6f6e 3a3a 2077 6562 736f 636b 6574 5f63  on:: websocket_c
-00000460: 6f6e 6e65 6374 0a20 2020 2e2e 2061 7574  onnect.   .. aut
-00000470: 6f63 6c61 7373 3a3a 2057 6562 536f 636b  oclass:: WebSock
-00000480: 6574 436c 6965 6e74 436f 6e6e 6563 7469  etClientConnecti
-00000490: 6f6e 0a20 2020 2020 2020 3a6d 656d 6265  on.       :membe
-000004a0: 7273 3a0a                                rs:.
+000000a0: 706f 7274 2074 6f72 6e61 646f 0a0a 2e2e  port tornado....
+000000b0: 2061 7574 6f6d 6f64 756c 653a 3a20 746f   automodule:: to
+000000c0: 726e 6164 6f2e 7765 6273 6f63 6b65 740a  rnado.websocket.
+000000d0: 0a20 2020 2e2e 2061 7574 6f63 6c61 7373  .   .. autoclass
+000000e0: 3a3a 2057 6562 536f 636b 6574 4861 6e64  :: WebSocketHand
+000000f0: 6c65 720a 0a20 2020 4576 656e 7420 6861  ler..   Event ha
+00000100: 6e64 6c65 7273 0a20 2020 2d2d 2d2d 2d2d  ndlers.   ------
+00000110: 2d2d 2d2d 2d2d 2d2d 0a0a 2020 202e 2e20  --------..   .. 
+00000120: 6175 746f 6d65 7468 6f64 3a3a 2057 6562  automethod:: Web
+00000130: 536f 636b 6574 4861 6e64 6c65 722e 6f70  SocketHandler.op
+00000140: 656e 0a20 2020 2e2e 2061 7574 6f6d 6574  en.   .. automet
+00000150: 686f 643a 3a20 5765 6253 6f63 6b65 7448  hod:: WebSocketH
+00000160: 616e 646c 6572 2e6f 6e5f 6d65 7373 6167  andler.on_messag
+00000170: 650a 2020 202e 2e20 6175 746f 6d65 7468  e.   .. autometh
+00000180: 6f64 3a3a 2057 6562 536f 636b 6574 4861  od:: WebSocketHa
+00000190: 6e64 6c65 722e 6f6e 5f63 6c6f 7365 0a20  ndler.on_close. 
+000001a0: 2020 2e2e 2061 7574 6f6d 6574 686f 643a    .. automethod:
+000001b0: 3a20 5765 6253 6f63 6b65 7448 616e 646c  : WebSocketHandl
+000001c0: 6572 2e73 656c 6563 745f 7375 6270 726f  er.select_subpro
+000001d0: 746f 636f 6c0a 2020 202e 2e20 6175 746f  tocol.   .. auto
+000001e0: 6174 7472 6962 7574 653a 3a20 5765 6253  attribute:: WebS
+000001f0: 6f63 6b65 7448 616e 646c 6572 2e73 656c  ocketHandler.sel
+00000200: 6563 7465 645f 7375 6270 726f 746f 636f  ected_subprotoco
+00000210: 6c0a 2020 202e 2e20 6175 746f 6d65 7468  l.   .. autometh
+00000220: 6f64 3a3a 2057 6562 536f 636b 6574 4861  od:: WebSocketHa
+00000230: 6e64 6c65 722e 6f6e 5f70 696e 670a 0a20  ndler.on_ping.. 
+00000240: 2020 4f75 7470 7574 0a20 2020 2d2d 2d2d    Output.   ----
+00000250: 2d2d 0a0a 2020 202e 2e20 6175 746f 6d65  --..   .. autome
+00000260: 7468 6f64 3a3a 2057 6562 536f 636b 6574  thod:: WebSocket
+00000270: 4861 6e64 6c65 722e 7772 6974 655f 6d65  Handler.write_me
+00000280: 7373 6167 650a 2020 202e 2e20 6175 746f  ssage.   .. auto
+00000290: 6d65 7468 6f64 3a3a 2057 6562 536f 636b  method:: WebSock
+000002a0: 6574 4861 6e64 6c65 722e 636c 6f73 650a  etHandler.close.
+000002b0: 0a20 2020 436f 6e66 6967 7572 6174 696f  .   Configuratio
+000002c0: 6e0a 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  n.   -----------
+000002d0: 2d2d 0a0a 2020 202e 2e20 6175 746f 6d65  --..   .. autome
+000002e0: 7468 6f64 3a3a 2057 6562 536f 636b 6574  thod:: WebSocket
+000002f0: 4861 6e64 6c65 722e 6368 6563 6b5f 6f72  Handler.check_or
+00000300: 6967 696e 0a20 2020 2e2e 2061 7574 6f6d  igin.   .. autom
+00000310: 6574 686f 643a 3a20 5765 6253 6f63 6b65  ethod:: WebSocke
+00000320: 7448 616e 646c 6572 2e67 6574 5f63 6f6d  tHandler.get_com
+00000330: 7072 6573 7369 6f6e 5f6f 7074 696f 6e73  pression_options
+00000340: 0a20 2020 2e2e 2061 7574 6f6d 6574 686f  .   .. autometho
+00000350: 643a 3a20 5765 6253 6f63 6b65 7448 616e  d:: WebSocketHan
+00000360: 646c 6572 2e73 6574 5f6e 6f64 656c 6179  dler.set_nodelay
+00000370: 0a0a 2020 204f 7468 6572 0a20 2020 2d2d  ..   Other.   --
+00000380: 2d2d 2d0a 0a20 2020 2e2e 2061 7574 6f6d  ---..   .. autom
+00000390: 6574 686f 643a 3a20 5765 6253 6f63 6b65  ethod:: WebSocke
+000003a0: 7448 616e 646c 6572 2e70 696e 670a 2020  tHandler.ping.  
+000003b0: 202e 2e20 6175 746f 6d65 7468 6f64 3a3a   .. automethod::
+000003c0: 2057 6562 536f 636b 6574 4861 6e64 6c65   WebSocketHandle
+000003d0: 722e 6f6e 5f70 6f6e 670a 2020 202e 2e20  r.on_pong.   .. 
+000003e0: 6175 746f 6578 6365 7074 696f 6e3a 3a20  autoexception:: 
+000003f0: 5765 6253 6f63 6b65 7443 6c6f 7365 6445  WebSocketClosedE
+00000400: 7272 6f72 0a0a 0a20 2020 436c 6965 6e74  rror...   Client
+00000410: 2d73 6964 6520 7375 7070 6f72 740a 2020  -side support.  
+00000420: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00000430: 2d2d 2d2d 0a0a 2020 202e 2e20 6175 746f  ----..   .. auto
+00000440: 6675 6e63 7469 6f6e 3a3a 2077 6562 736f  function:: webso
+00000450: 636b 6574 5f63 6f6e 6e65 6374 0a20 2020  cket_connect.   
+00000460: 2e2e 2061 7574 6f63 6c61 7373 3a3a 2057  .. autoclass:: W
+00000470: 6562 536f 636b 6574 436c 6965 6e74 436f  ebSocketClientCo
+00000480: 6e6e 6563 7469 6f6e 0a20 2020 2020 2020  nnection.       
+00000490: 3a6d 656d 6265 7273 3a0a                 :members:.
```

### Comparing `tornado-6.2b2/pyproject.toml` & `tornado-6.3b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.cibuildwheel]
-build = "cp3[789]* cp310*"
+build = "cp3[89]* cp310* cp311*"
 test-command = "python -m tornado.test"
 
 [tool.cibuildwheel.macos]
 archs = "x86_64 universal2"
 # The arm portion of a universal wheel is a cross-compile and cannot
 # be tested on an x86 host. This must be configured explicitly to silence
 # a warning.
```

### Comparing `tornado-6.2b2/setup.py` & `tornado-6.3b1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,35 +48,35 @@
             sources=["tornado/speedups.c"],
             # Unless the user has specified that the extension is mandatory,
             # fall back to the pure-python implementation on any build failure.
             optional=os.environ.get("TORNADO_EXTENSION") != "1",
             # Use the stable ABI so our wheels are compatible across python
             # versions.
             py_limited_api=True,
-            define_macros=[("Py_LIMITED_API", "0x03070000")],
+            define_macros=[("Py_LIMITED_API", "0x03080000")],
         )
     ]
 
 if wheel is not None:
     # From https://github.com/joerick/python-abi3-package-sample/blob/main/setup.py
     class bdist_wheel_abi3(wheel.bdist_wheel.bdist_wheel):
         def get_tag(self):
             python, abi, plat = super().get_tag()
 
             if python.startswith("cp"):
-                return "cp37", "abi3", plat
+                return "cp38", "abi3", plat
             return python, abi, plat
 
     kwargs["cmdclass"] = {"bdist_wheel": bdist_wheel_abi3}
 
 
 setuptools.setup(
     name="tornado",
     version=version,
-    python_requires=">= 3.7",
+    python_requires=">= 3.8",
     packages=["tornado", "tornado.test", "tornado.platform"],
     package_data={
         # data files need to be listed both here (which determines what gets
         # installed) and in MANIFEST.in (which determines what gets included
         # in the sdist tarball)
         "tornado": ["py.typed"],
         "tornado.test": [
@@ -100,24 +100,24 @@
     },
     author="Facebook",
     author_email="python-tornado@googlegroups.com",
     url="http://www.tornadoweb.org/",
     project_urls={
         "Source": "https://github.com/tornadoweb/tornado",
     },
-    license="http://www.apache.org/licenses/LICENSE-2.0",
+    license="Apache-2.0",
     description=(
         "Tornado is a Python web framework and asynchronous networking library,"
         " originally developed at FriendFeed."
     ),
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
     **kwargs
 )
```

### Comparing `tornado-6.2b2/tornado/_locale_data.py` & `tornado-6.3b1/tornado/_locale_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,70 +11,70 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 """Data used by the tornado.locale module."""
 
 LOCALE_NAMES = {
-    "af_ZA": {"name_en": u"Afrikaans", "name": u"Afrikaans"},
-    "am_ET": {"name_en": u"Amharic", "name": u"አማርኛ"},
-    "ar_AR": {"name_en": u"Arabic", "name": u"العربية"},
-    "bg_BG": {"name_en": u"Bulgarian", "name": u"Български"},
-    "bn_IN": {"name_en": u"Bengali", "name": u"বাংলা"},
-    "bs_BA": {"name_en": u"Bosnian", "name": u"Bosanski"},
-    "ca_ES": {"name_en": u"Catalan", "name": u"Català"},
-    "cs_CZ": {"name_en": u"Czech", "name": u"Čeština"},
-    "cy_GB": {"name_en": u"Welsh", "name": u"Cymraeg"},
-    "da_DK": {"name_en": u"Danish", "name": u"Dansk"},
-    "de_DE": {"name_en": u"German", "name": u"Deutsch"},
-    "el_GR": {"name_en": u"Greek", "name": u"Ελληνικά"},
-    "en_GB": {"name_en": u"English (UK)", "name": u"English (UK)"},
-    "en_US": {"name_en": u"English (US)", "name": u"English (US)"},
-    "es_ES": {"name_en": u"Spanish (Spain)", "name": u"Español (España)"},
-    "es_LA": {"name_en": u"Spanish", "name": u"Español"},
-    "et_EE": {"name_en": u"Estonian", "name": u"Eesti"},
-    "eu_ES": {"name_en": u"Basque", "name": u"Euskara"},
-    "fa_IR": {"name_en": u"Persian", "name": u"فارسی"},
-    "fi_FI": {"name_en": u"Finnish", "name": u"Suomi"},
-    "fr_CA": {"name_en": u"French (Canada)", "name": u"Français (Canada)"},
-    "fr_FR": {"name_en": u"French", "name": u"Français"},
-    "ga_IE": {"name_en": u"Irish", "name": u"Gaeilge"},
-    "gl_ES": {"name_en": u"Galician", "name": u"Galego"},
-    "he_IL": {"name_en": u"Hebrew", "name": u"עברית"},
-    "hi_IN": {"name_en": u"Hindi", "name": u"हिन्दी"},
-    "hr_HR": {"name_en": u"Croatian", "name": u"Hrvatski"},
-    "hu_HU": {"name_en": u"Hungarian", "name": u"Magyar"},
-    "id_ID": {"name_en": u"Indonesian", "name": u"Bahasa Indonesia"},
-    "is_IS": {"name_en": u"Icelandic", "name": u"Íslenska"},
-    "it_IT": {"name_en": u"Italian", "name": u"Italiano"},
-    "ja_JP": {"name_en": u"Japanese", "name": u"日本語"},
-    "ko_KR": {"name_en": u"Korean", "name": u"한국어"},
-    "lt_LT": {"name_en": u"Lithuanian", "name": u"Lietuvių"},
-    "lv_LV": {"name_en": u"Latvian", "name": u"Latviešu"},
-    "mk_MK": {"name_en": u"Macedonian", "name": u"Македонски"},
-    "ml_IN": {"name_en": u"Malayalam", "name": u"മലയാളം"},
-    "ms_MY": {"name_en": u"Malay", "name": u"Bahasa Melayu"},
-    "nb_NO": {"name_en": u"Norwegian (bokmal)", "name": u"Norsk (bokmål)"},
-    "nl_NL": {"name_en": u"Dutch", "name": u"Nederlands"},
-    "nn_NO": {"name_en": u"Norwegian (nynorsk)", "name": u"Norsk (nynorsk)"},
-    "pa_IN": {"name_en": u"Punjabi", "name": u"ਪੰਜਾਬੀ"},
-    "pl_PL": {"name_en": u"Polish", "name": u"Polski"},
-    "pt_BR": {"name_en": u"Portuguese (Brazil)", "name": u"Português (Brasil)"},
-    "pt_PT": {"name_en": u"Portuguese (Portugal)", "name": u"Português (Portugal)"},
-    "ro_RO": {"name_en": u"Romanian", "name": u"Română"},
-    "ru_RU": {"name_en": u"Russian", "name": u"Русский"},
-    "sk_SK": {"name_en": u"Slovak", "name": u"Slovenčina"},
-    "sl_SI": {"name_en": u"Slovenian", "name": u"Slovenščina"},
-    "sq_AL": {"name_en": u"Albanian", "name": u"Shqip"},
-    "sr_RS": {"name_en": u"Serbian", "name": u"Српски"},
-    "sv_SE": {"name_en": u"Swedish", "name": u"Svenska"},
-    "sw_KE": {"name_en": u"Swahili", "name": u"Kiswahili"},
-    "ta_IN": {"name_en": u"Tamil", "name": u"தமிழ்"},
-    "te_IN": {"name_en": u"Telugu", "name": u"తెలుగు"},
-    "th_TH": {"name_en": u"Thai", "name": u"ภาษาไทย"},
-    "tl_PH": {"name_en": u"Filipino", "name": u"Filipino"},
-    "tr_TR": {"name_en": u"Turkish", "name": u"Türkçe"},
-    "uk_UA": {"name_en": u"Ukraini ", "name": u"Українська"},
-    "vi_VN": {"name_en": u"Vietnamese", "name": u"Tiếng Việt"},
-    "zh_CN": {"name_en": u"Chinese (Simplified)", "name": u"中文(简体)"},
-    "zh_TW": {"name_en": u"Chinese (Traditional)", "name": u"中文(繁體)"},
+    "af_ZA": {"name_en": "Afrikaans", "name": "Afrikaans"},
+    "am_ET": {"name_en": "Amharic", "name": "አማርኛ"},
+    "ar_AR": {"name_en": "Arabic", "name": "العربية"},
+    "bg_BG": {"name_en": "Bulgarian", "name": "Български"},
+    "bn_IN": {"name_en": "Bengali", "name": "বাংলা"},
+    "bs_BA": {"name_en": "Bosnian", "name": "Bosanski"},
+    "ca_ES": {"name_en": "Catalan", "name": "Català"},
+    "cs_CZ": {"name_en": "Czech", "name": "Čeština"},
+    "cy_GB": {"name_en": "Welsh", "name": "Cymraeg"},
+    "da_DK": {"name_en": "Danish", "name": "Dansk"},
+    "de_DE": {"name_en": "German", "name": "Deutsch"},
+    "el_GR": {"name_en": "Greek", "name": "Ελληνικά"},
+    "en_GB": {"name_en": "English (UK)", "name": "English (UK)"},
+    "en_US": {"name_en": "English (US)", "name": "English (US)"},
+    "es_ES": {"name_en": "Spanish (Spain)", "name": "Español (España)"},
+    "es_LA": {"name_en": "Spanish", "name": "Español"},
+    "et_EE": {"name_en": "Estonian", "name": "Eesti"},
+    "eu_ES": {"name_en": "Basque", "name": "Euskara"},
+    "fa_IR": {"name_en": "Persian", "name": "فارسی"},
+    "fi_FI": {"name_en": "Finnish", "name": "Suomi"},
+    "fr_CA": {"name_en": "French (Canada)", "name": "Français (Canada)"},
+    "fr_FR": {"name_en": "French", "name": "Français"},
+    "ga_IE": {"name_en": "Irish", "name": "Gaeilge"},
+    "gl_ES": {"name_en": "Galician", "name": "Galego"},
+    "he_IL": {"name_en": "Hebrew", "name": "עברית"},
+    "hi_IN": {"name_en": "Hindi", "name": "हिन्दी"},
+    "hr_HR": {"name_en": "Croatian", "name": "Hrvatski"},
+    "hu_HU": {"name_en": "Hungarian", "name": "Magyar"},
+    "id_ID": {"name_en": "Indonesian", "name": "Bahasa Indonesia"},
+    "is_IS": {"name_en": "Icelandic", "name": "Íslenska"},
+    "it_IT": {"name_en": "Italian", "name": "Italiano"},
+    "ja_JP": {"name_en": "Japanese", "name": "日本語"},
+    "ko_KR": {"name_en": "Korean", "name": "한국어"},
+    "lt_LT": {"name_en": "Lithuanian", "name": "Lietuvių"},
+    "lv_LV": {"name_en": "Latvian", "name": "Latviešu"},
+    "mk_MK": {"name_en": "Macedonian", "name": "Македонски"},
+    "ml_IN": {"name_en": "Malayalam", "name": "മലയാളം"},
+    "ms_MY": {"name_en": "Malay", "name": "Bahasa Melayu"},
+    "nb_NO": {"name_en": "Norwegian (bokmal)", "name": "Norsk (bokmål)"},
+    "nl_NL": {"name_en": "Dutch", "name": "Nederlands"},
+    "nn_NO": {"name_en": "Norwegian (nynorsk)", "name": "Norsk (nynorsk)"},
+    "pa_IN": {"name_en": "Punjabi", "name": "ਪੰਜਾਬੀ"},
+    "pl_PL": {"name_en": "Polish", "name": "Polski"},
+    "pt_BR": {"name_en": "Portuguese (Brazil)", "name": "Português (Brasil)"},
+    "pt_PT": {"name_en": "Portuguese (Portugal)", "name": "Português (Portugal)"},
+    "ro_RO": {"name_en": "Romanian", "name": "Română"},
+    "ru_RU": {"name_en": "Russian", "name": "Русский"},
+    "sk_SK": {"name_en": "Slovak", "name": "Slovenčina"},
+    "sl_SI": {"name_en": "Slovenian", "name": "Slovenščina"},
+    "sq_AL": {"name_en": "Albanian", "name": "Shqip"},
+    "sr_RS": {"name_en": "Serbian", "name": "Српски"},
+    "sv_SE": {"name_en": "Swedish", "name": "Svenska"},
+    "sw_KE": {"name_en": "Swahili", "name": "Kiswahili"},
+    "ta_IN": {"name_en": "Tamil", "name": "தமிழ்"},
+    "te_IN": {"name_en": "Telugu", "name": "తెలుగు"},
+    "th_TH": {"name_en": "Thai", "name": "ภาษาไทย"},
+    "tl_PH": {"name_en": "Filipino", "name": "Filipino"},
+    "tr_TR": {"name_en": "Turkish", "name": "Türkçe"},
+    "uk_UA": {"name_en": "Ukraini ", "name": "Українська"},
+    "vi_VN": {"name_en": "Vietnamese", "name": "Tiếng Việt"},
+    "zh_CN": {"name_en": "Chinese (Simplified)", "name": "中文(简体)"},
+    "zh_TW": {"name_en": "Chinese (Traditional)", "name": "中文(繁體)"},
 }
```

### Comparing `tornado-6.2b2/tornado/auth.py` & `tornado-6.3b1/tornado/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     class GoogleOAuth2LoginHandler(tornado.web.RequestHandler,
                                    tornado.auth.GoogleOAuth2Mixin):
         async def get(self):
             if self.get_argument('code', False):
                 user = await self.get_authenticated_user(
                     redirect_uri='http://your.site.com/auth/google',
                     code=self.get_argument('code'))
-                # Save the user with e.g. set_secure_cookie
+                # Save the user with e.g. set_signed_cookie
             else:
                 self.authorize_redirect(
                     redirect_uri='http://your.site.com/auth/google',
                     client_id=self.settings['google_oauth']['key'],
                     scope=['profile', 'email'],
                     response_type='code',
                     extra_params={'approval_prompt': 'auto'})
@@ -132,15 +132,15 @@
             awaitable object instead.
         """
         handler = cast(RequestHandler, self)
         # Verify the OpenID response via direct request to the OP
         args = dict(
             (k, v[-1]) for k, v in handler.request.arguments.items()
         )  # type: Dict[str, Union[str, bytes]]
-        args["openid.mode"] = u"check_authentication"
+        args["openid.mode"] = "check_authentication"
         url = self._OPENID_ENDPOINT  # type: ignore
         if http_client is None:
             http_client = self.get_auth_http_client()
         resp = await http_client.fetch(
             url, method="POST", body=urllib.parse.urlencode(args)
         )
         return self._on_authentication_verified(resp)
@@ -207,32 +207,32 @@
             raise AuthError("Invalid OpenID response: %r" % response.body)
 
         # Make sure we got back at least an email from attribute exchange
         ax_ns = None
         for key in handler.request.arguments:
             if (
                 key.startswith("openid.ns.")
-                and handler.get_argument(key) == u"http://openid.net/srv/ax/1.0"
+                and handler.get_argument(key) == "http://openid.net/srv/ax/1.0"
             ):
                 ax_ns = key[10:]
                 break
 
         def get_ax_arg(uri: str) -> str:
             if not ax_ns:
-                return u""
+                return ""
             prefix = "openid." + ax_ns + ".type."
             ax_name = None
             for name in handler.request.arguments.keys():
                 if handler.get_argument(name) == uri and name.startswith(prefix):
                     part = name[len(prefix) :]
                     ax_name = "openid." + ax_ns + ".value." + part
                     break
             if not ax_name:
-                return u""
-            return handler.get_argument(ax_name, u"")
+                return ""
+            return handler.get_argument(ax_name, "")
 
         email = get_ax_arg("http://axschema.org/contact/email")
         name = get_ax_arg("http://axschema.org/namePerson")
         first_name = get_ax_arg("http://axschema.org/namePerson/first")
         last_name = get_ax_arg("http://axschema.org/namePerson/last")
         username = get_ax_arg("http://axschema.org/namePerson/friendly")
         locale = get_ax_arg("http://axschema.org/pref/language").lower()
@@ -243,15 +243,15 @@
             name_parts.append(first_name)
         if last_name:
             user["last_name"] = last_name
             name_parts.append(last_name)
         if name:
             user["name"] = name
         elif name_parts:
-            user["name"] = u" ".join(name_parts)
+            user["name"] = " ".join(name_parts)
         elif email:
             user["name"] = email.split("@")[0]
         if email:
             user["email"] = email
         if locale:
             user["locale"] = locale
         if username:
@@ -690,15 +690,15 @@
     .. testcode::
 
         class TwitterLoginHandler(tornado.web.RequestHandler,
                                   tornado.auth.TwitterMixin):
             async def get(self):
                 if self.get_argument("oauth_token", None):
                     user = await self.get_authenticated_user()
-                    # Save the user using e.g. set_secure_cookie()
+                    # Save the user using e.g. set_signed_cookie()
                 else:
                     await self.authorize_redirect()
 
     .. testoutput::
        :hide:
 
     The user object returned by `~OAuthMixin.get_authenticated_user`
@@ -851,16 +851,36 @@
 
     _OAUTH_AUTHORIZE_URL = "https://accounts.google.com/o/oauth2/v2/auth"
     _OAUTH_ACCESS_TOKEN_URL = "https://www.googleapis.com/oauth2/v4/token"
     _OAUTH_USERINFO_URL = "https://www.googleapis.com/oauth2/v1/userinfo"
     _OAUTH_NO_CALLBACKS = False
     _OAUTH_SETTINGS_KEY = "google_oauth"
 
+    def get_google_oauth_settings(self) -> Dict[str, str]:
+        """Return the Google OAuth 2.0 credentials that you created with
+        [Google Cloud
+        Platform](https://console.cloud.google.com/apis/credentials). The dict
+        format is::
+
+            {
+                "key": "your_client_id", "secret": "your_client_secret"
+            }
+
+        If your credentials are stored differently (e.g. in a db) you can
+        override this method for custom provision.
+        """
+        handler = cast(RequestHandler, self)
+        return handler.settings[self._OAUTH_SETTINGS_KEY]
+
     async def get_authenticated_user(
-        self, redirect_uri: str, code: str
+        self,
+        redirect_uri: str,
+        code: str,
+        client_id: Optional[str] = None,
+        client_secret: Optional[str] = None,
     ) -> Dict[str, Any]:
         """Handles the login for the Google user, returning an access token.
 
         The result is a dictionary containing an ``access_token`` field
         ([among others](https://developers.google.com/identity/protocols/OAuth2WebServer#handlingtheresponse)).
         Unlike other ``get_authenticated_user`` methods in this package,
         this method does not return any additional information about the user.
@@ -879,38 +899,44 @@
                         access = await self.get_authenticated_user(
                             redirect_uri='http://your.site.com/auth/google',
                             code=self.get_argument('code'))
                         user = await self.oauth2_request(
                             "https://www.googleapis.com/oauth2/v1/userinfo",
                             access_token=access["access_token"])
                         # Save the user and access token with
-                        # e.g. set_secure_cookie.
+                        # e.g. set_signed_cookie.
                     else:
                         self.authorize_redirect(
                             redirect_uri='http://your.site.com/auth/google',
-                            client_id=self.settings['google_oauth']['key'],
+                            client_id=self.get_google_oauth_settings()['key'],
                             scope=['profile', 'email'],
                             response_type='code',
                             extra_params={'approval_prompt': 'auto'})
 
         .. testoutput::
            :hide:
 
         .. versionchanged:: 6.0
 
            The ``callback`` argument was removed. Use the returned awaitable object instead.
         """  # noqa: E501
-        handler = cast(RequestHandler, self)
+
+        if client_id is None or client_secret is None:
+            settings = self.get_google_oauth_settings()
+            if client_id is None:
+                client_id = settings["key"]
+            if client_secret is None:
+                client_secret = settings["secret"]
         http = self.get_auth_http_client()
         body = urllib.parse.urlencode(
             {
                 "redirect_uri": redirect_uri,
                 "code": code,
-                "client_id": handler.settings[self._OAUTH_SETTINGS_KEY]["key"],
-                "client_secret": handler.settings[self._OAUTH_SETTINGS_KEY]["secret"],
+                "client_id": client_id,
+                "client_secret": client_secret,
                 "grant_type": "authorization_code",
             }
         )
 
         response = await http.fetch(
             self._OAUTH_ACCESS_TOKEN_URL,
             method="POST",
@@ -947,15 +973,15 @@
               async def get(self):
                   if self.get_argument("code", False):
                       user = await self.get_authenticated_user(
                           redirect_uri='/auth/facebookgraph/',
                           client_id=self.settings["facebook_api_key"],
                           client_secret=self.settings["facebook_secret"],
                           code=self.get_argument("code"))
-                      # Save the user with e.g. set_secure_cookie
+                      # Save the user with e.g. set_signed_cookie
                   else:
                       self.authorize_redirect(
                           redirect_uri='/auth/facebookgraph/',
                           client_id=self.settings["facebook_api_key"],
                           extra_params={"scope": "read_stream,offline_access"})
 
         .. testoutput::
```

### Comparing `tornado-6.2b2/tornado/autoreload.py` & `tornado-6.3b1/tornado/autoreload.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/concurrent.py` & `tornado-6.3b1/tornado/concurrent.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/curl_httpclient.py` & `tornado-6.3b1/tornado/curl_httpclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
     HTTPResponse,
     HTTPError,
     AsyncHTTPClient,
     main,
 )
 from tornado.log import app_log
 
-from typing import Dict, Any, Callable, Union, Tuple, Optional
+from typing import Dict, Any, Callable, Union, Optional
 import typing
 
 if typing.TYPE_CHECKING:
-    from typing import Deque  # noqa: F401
+    from typing import Deque, Tuple  # noqa: F401
 
 curl_log = logging.getLogger("tornado.curl_httpclient")
 
 
 class CurlAsyncHTTPClient(AsyncHTTPClient):
     def initialize(  # type: ignore
         self, max_clients: int = 10, defaults: Optional[Dict[str, Any]] = None
```

### Comparing `tornado-6.2b2/tornado/escape.py` & `tornado-6.3b1/tornado/escape.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,15 +364,15 @@
                 if len(url) >= len(before_clip):
                     url = before_clip
                 else:
                     # full url is visible on mouse-over (for those who don't
                     # have a status bar, such as Safari by default)
                     params += ' title="%s"' % href
 
-        return u'<a href="%s"%s>%s</a>' % (href, params, url)
+        return '<a href="%s"%s>%s</a>' % (href, params, url)
 
     # First HTML-escape so that our strings are all safe.
     # The regex is modified to avoid character entites other than &amp; so
     # that we won't pick up &quot;, etc.
     text = _unicode(xhtml_escape(text))
     return _URL_RE.sub(make_link, text)
```

### Comparing `tornado-6.2b2/tornado/gen.py` & `tornado-6.3b1/tornado/gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -739,15 +739,15 @@
         self.ctx_run = ctx_run
         self.gen = gen
         self.result_future = result_future
         self.future = _null_future  # type: Union[None, Future]
         self.running = False
         self.finished = False
         self.io_loop = IOLoop.current()
-        if self.handle_yield(first_yielded):
+        if self.ctx_run(self.handle_yield, first_yielded):
             gen = result_future = first_yielded = None  # type: ignore
             self.ctx_run(self.run)
 
     def run(self) -> None:
         """Starts or resumes the generator, running until it reaches a
         yield point that is not ready.
         """
@@ -759,29 +759,33 @@
                 future = self.future
                 if future is None:
                     raise Exception("No pending future")
                 if not future.done():
                     return
                 self.future = None
                 try:
-                    exc_info = None
-
                     try:
                         value = future.result()
-                    except Exception:
-                        exc_info = sys.exc_info()
-                    future = None
+                    except Exception as e:
+                        # Save the exception for later. It's important that
+                        # gen.throw() not be called inside this try/except block
+                        # because that makes sys.exc_info behave unexpectedly.
+                        exc: Optional[Exception] = e
+                    else:
+                        exc = None
+                    finally:
+                        future = None
 
-                    if exc_info is not None:
+                    if exc is not None:
                         try:
-                            yielded = self.gen.throw(*exc_info)  # type: ignore
+                            yielded = self.gen.throw(exc)
                         finally:
-                            # Break up a reference to itself
-                            # for faster GC on CPython.
-                            exc_info = None
+                            # Break up a circular reference for faster GC on
+                            # CPython.
+                            del exc
                     else:
                         yielded = self.gen.send(value)
 
                 except (StopIteration, Return) as e:
                     self.finished = True
                     self.future = _null_future
                     future_set_result_unless_cancelled(
```

### Comparing `tornado-6.2b2/tornado/http1connection.py` & `tornado-6.3b1/tornado/http1connection.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/httpclient.py` & `tornado-6.3b1/tornado/httpclient.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/httpserver.py` & `tornado-6.3b1/tornado/httpserver.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/httputil.py` & `tornado-6.3b1/tornado/httputil.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/ioloop.py` & `tornado-6.3b1/tornado/ioloop.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     .. testcode::
 
         import asyncio
         import errno
         import functools
         import socket
 
-        import tornado.ioloop
+        import tornado
         from tornado.iostream import IOStream
 
         async def handle_connection(connection, address):
             stream = IOStream(connection)
             message = await stream.read_until_close()
             print("message from client:", message.decode().strip())
 
@@ -119,16 +119,15 @@
     .. testoutput::
        :hide:
 
     Most applications should not attempt to construct an `IOLoop` directly,
     and instead initialize the `asyncio` event loop and use `IOLoop.current()`.
     In some cases, such as in test frameworks when initializing an `IOLoop`
     to be run in a secondary thread, it may be appropriate to construct
-    an `IOLoop` with ``IOLoop(make_current=False)``. Constructing an `IOLoop`
-    without the ``make_current=False`` argument is deprecated since Tornado 6.2.
+    an `IOLoop` with ``IOLoop(make_current=False)``.
 
     In general, an `IOLoop` cannot survive a fork or be shared across processes
     in any way. When multiple processes are being used, each process should
     create its own `IOLoop`, which also implies that any objects which depend on
     the `IOLoop` (such as `.AsyncHTTPClient`) must also be created in the child
     processes. As a guideline, anything that starts processes (including the
     `tornado.process` and `multiprocessing` modules) should do so as early as
@@ -141,20 +140,18 @@
 
     .. versionchanged:: 5.0
 
        Uses the `asyncio` event loop by default. The ``IOLoop.configure`` method
        cannot be used on Python 3 except to redundantly specify the `asyncio`
        event loop.
 
-    .. deprecated:: 6.2
-       It is deprecated to create an event loop that is "current" but not
-       running. This means it is deprecated to pass
-       ``make_current=True`` to the ``IOLoop`` constructor, or to create
-       an ``IOLoop`` while no asyncio event loop is running unless
-       ``make_current=False`` is used.
+    .. versionchanged:: 6.3
+       ``make_current=True`` is now the default when creating an IOLoop -
+       previously the default was to make the event loop current if there wasn't
+       already a current one.
     """
 
     # These constants were originally based on constants from the epoll module.
     NONE = 0
     READ = 0x001
     WRITE = 0x004
     ERROR = 0x018
@@ -259,25 +256,28 @@
 
         .. deprecated:: 6.2
            It is deprecated to call ``IOLoop.current()`` when no `asyncio`
            event loop is running.
         """
         try:
             loop = asyncio.get_event_loop()
-        except (RuntimeError, AssertionError):
+        except RuntimeError:
             if not instance:
                 return None
-            raise
+            # Create a new asyncio event loop for this thread.
+            loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(loop)
+
         try:
             return IOLoop._ioloop_for_asyncio[loop]
         except KeyError:
             if instance:
                 from tornado.platform.asyncio import AsyncIOMainLoop
 
-                current = AsyncIOMainLoop(make_current=True)  # type: Optional[IOLoop]
+                current = AsyncIOMainLoop()  # type: Optional[IOLoop]
             else:
                 current = None
         return current
 
     def make_current(self) -> None:
         """Makes this the `IOLoop` for the current thread.
 
@@ -291,20 +291,25 @@
            An `IOLoop` created while there is no current `IOLoop`
            will automatically become current.
 
         .. versionchanged:: 5.0
            This method also sets the current `asyncio` event loop.
 
         .. deprecated:: 6.2
-           The concept of an event loop that is "current" without
-           currently running is deprecated in asyncio since Python
-           3.10. All related functionality in Tornado is also
-           deprecated. Instead, start the event loop with `asyncio.run`
-           before interacting with it.
+           Setting and clearing the current event loop through Tornado is
+           deprecated. Use ``asyncio.set_event_loop`` instead if you need this.
         """
+        warnings.warn(
+            "make_current is deprecated; start the event loop first",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        self._make_current()
+
+    def _make_current(self) -> None:
         # The asyncio event loops override this method.
         raise NotImplementedError()
 
     @staticmethod
     def clear_current() -> None:
         """Clears the `IOLoop` for the current thread.
 
@@ -340,24 +345,17 @@
 
     @classmethod
     def configurable_default(cls) -> Type[Configurable]:
         from tornado.platform.asyncio import AsyncIOLoop
 
         return AsyncIOLoop
 
-    def initialize(self, make_current: Optional[bool] = None) -> None:
-        if make_current is None:
-            if IOLoop.current(instance=False) is None:
-                self.make_current()
-        elif make_current:
-            current = IOLoop.current(instance=False)
-            # AsyncIO loops can already be current by this point.
-            if current is not None and current is not self:
-                raise RuntimeError("current IOLoop already exists")
-            self.make_current()
+    def initialize(self, make_current: bool = True) -> None:
+        if make_current:
+            self._make_current()
 
     def close(self, all_fds: bool = False) -> None:
         """Closes the `IOLoop`, freeing any resources used.
 
         If ``all_fds`` is true, all file descriptors registered on the
         IOLoop will be closed (not just the ones created by the
         `IOLoop` itself).
```

### Comparing `tornado-6.2b2/tornado/iostream.py` & `tornado-6.3b1/tornado/iostream.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,19 +191,17 @@
                 buffers.popleft()
                 size -= len(b) - pos
                 pos = 0
             elif is_large:
                 pos += size
                 size = 0
             else:
-                # Amortized O(1) shrink for Python 2
                 pos += size
-                if len(b) <= 2 * pos:
-                    del typing.cast(bytearray, b)[:pos]
-                    pos = 0
+                del typing.cast(bytearray, b)[:pos]
+                pos = 0
                 size = 0
 
         assert size == 0
         self._first_pos = pos
 
 
 class BaseIOStream(object):
@@ -250,15 +248,14 @@
         self.max_buffer_size = max_buffer_size or 104857600
         # A chunk size that is too close to max_buffer_size can cause
         # spurious failures.
         self.read_chunk_size = min(read_chunk_size or 65536, self.max_buffer_size // 2)
         self.max_write_buffer_size = max_write_buffer_size
         self.error = None  # type: Optional[BaseException]
         self._read_buffer = bytearray()
-        self._read_buffer_pos = 0
         self._read_buffer_size = 0
         self._user_read_buffer = False
         self._after_user_read_buffer = None  # type: Optional[bytearray]
         self._write_buffer = _StreamBuffer()
         self._total_write_index = 0
         self._total_write_done_index = 0
         self._read_delimiter = None  # type: Optional[bytes]
@@ -447,29 +444,25 @@
         """
         future = self._start_read()
 
         # First copy data already in read buffer
         available_bytes = self._read_buffer_size
         n = len(buf)
         if available_bytes >= n:
-            end = self._read_buffer_pos + n
-            buf[:] = memoryview(self._read_buffer)[self._read_buffer_pos : end]
-            del self._read_buffer[:end]
+            buf[:] = memoryview(self._read_buffer)[:n]
+            del self._read_buffer[:n]
             self._after_user_read_buffer = self._read_buffer
         elif available_bytes > 0:
-            buf[:available_bytes] = memoryview(self._read_buffer)[
-                self._read_buffer_pos :
-            ]
+            buf[:available_bytes] = memoryview(self._read_buffer)[:]
 
         # Set up the supplied buffer as our temporary read buffer.
         # The original (if it had any data remaining) has been
         # saved for later.
         self._user_read_buffer = True
         self._read_buffer = buf
-        self._read_buffer_pos = 0
         self._read_buffer_size = available_bytes
         self._read_bytes = n
         self._read_partial = partial
 
         try:
             self._try_inline_read()
         except:
@@ -812,15 +805,14 @@
         self._read_future = Future()
         return self._read_future
 
     def _finish_read(self, size: int) -> None:
         if self._user_read_buffer:
             self._read_buffer = self._after_user_read_buffer or bytearray()
             self._after_user_read_buffer = None
-            self._read_buffer_pos = 0
             self._read_buffer_size = len(self._read_buffer)
             self._user_read_buffer = False
             result = size  # type: Union[int, bytes]
         else:
             result = self._consume(size)
         if self._read_future is not None:
             future = self._read_future
@@ -925,28 +917,25 @@
             # without collapsing the buffer.  However, since protocols
             # using delimited reads (as opposed to reads of a known
             # length) tend to be "line" oriented, the delimiter is likely
             # to be in the first few chunks.  Merge the buffer gradually
             # since large merges are relatively expensive and get undone in
             # _consume().
             if self._read_buffer:
-                loc = self._read_buffer.find(
-                    self._read_delimiter, self._read_buffer_pos
-                )
+                loc = self._read_buffer.find(self._read_delimiter)
                 if loc != -1:
-                    loc -= self._read_buffer_pos
                     delimiter_len = len(self._read_delimiter)
                     self._check_max_bytes(self._read_delimiter, loc + delimiter_len)
                     return loc + delimiter_len
                 self._check_max_bytes(self._read_delimiter, self._read_buffer_size)
         elif self._read_regex is not None:
             if self._read_buffer:
-                m = self._read_regex.search(self._read_buffer, self._read_buffer_pos)
+                m = self._read_regex.search(self._read_buffer)
                 if m is not None:
-                    loc = m.end() - self._read_buffer_pos
+                    loc = m.end()
                     self._check_max_bytes(self._read_regex, loc)
                     return loc
                 self._check_max_bytes(self._read_regex, self._read_buffer_size)
         return None
 
     def _check_max_bytes(self, delimiter: Union[bytes, Pattern], size: int) -> None:
         if self._read_max_bytes is not None and size > self._read_max_bytes:
@@ -995,27 +984,17 @@
 
     def _consume(self, loc: int) -> bytes:
         # Consume loc bytes from the read buffer and return them
         if loc == 0:
             return b""
         assert loc <= self._read_buffer_size
         # Slice the bytearray buffer into bytes, without intermediate copying
-        b = (
-            memoryview(self._read_buffer)[
-                self._read_buffer_pos : self._read_buffer_pos + loc
-            ]
-        ).tobytes()
-        self._read_buffer_pos += loc
+        b = (memoryview(self._read_buffer)[:loc]).tobytes()
         self._read_buffer_size -= loc
-        # Amortized O(1) shrink
-        # (this heuristic is implemented natively in Python 3.4+
-        #  but is replicated here for Python 2)
-        if self._read_buffer_pos > self._read_buffer_size:
-            del self._read_buffer[: self._read_buffer_pos]
-            self._read_buffer_pos = 0
+        del self._read_buffer[:loc]
         return b
 
     def _check_closed(self) -> None:
         if self.closed():
             raise StreamClosedError(real_error=self.error)
 
     def _maybe_add_error_listener(self) -> None:
@@ -1086,17 +1065,16 @@
     connected before passing it to the `IOStream` or connected with
     `IOStream.connect`.
 
     A very simple (and broken) HTTP client using this class:
 
     .. testcode::
 
-        import tornado.ioloop
-        import tornado.iostream
         import socket
+        import tornado
 
         async def main():
             s = socket.socket(socket.AF_INET, socket.SOCK_STREAM, 0)
             stream = tornado.iostream.IOStream(s)
             await stream.connect(("friendfeed.com", 80))
             await stream.write(b"GET / HTTP/1.0\r\nHost: friendfeed.com\r\n\r\n")
             header_data = await stream.read_until(b"\r\n\r\n")
```

### Comparing `tornado-6.2b2/tornado/locale.py` & `tornado-6.3b1/tornado/locale.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,15 @@
             else:
                 locale = CSVLocale(code, translations)
             cls._cache[code] = locale
         return cls._cache[code]
 
     def __init__(self, code: str) -> None:
         self.code = code
-        self.name = LOCALE_NAMES.get(code, {}).get("name", u"Unknown")
+        self.name = LOCALE_NAMES.get(code, {}).get("name", "Unknown")
         self.rtl = False
         for prefix in ["fa", "ar", "he"]:
             if self.code.startswith(prefix):
                 self.rtl = True
                 break
 
         # Initialize strings for date formatting
@@ -402,15 +402,15 @@
             )
 
         tfhour_clock = self.code not in ("en", "en_US", "zh_CN")
         if tfhour_clock:
             str_time = "%d:%02d" % (local_date.hour, local_date.minute)
         elif self.code == "zh_CN":
             str_time = "%s%d:%02d" % (
-                (u"\u4e0a\u5348", u"\u4e0b\u5348")[local_date.hour >= 12],
+                ("\u4e0a\u5348", "\u4e0b\u5348")[local_date.hour >= 12],
                 local_date.hour % 12 or 12,
                 local_date.minute,
             )
         else:
             str_time = "%d:%02d %s" % (
                 local_date.hour % 12 or 12,
                 local_date.minute,
@@ -454,15 +454,15 @@
         of size 1.
         """
         _ = self.translate
         if len(parts) == 0:
             return ""
         if len(parts) == 1:
             return parts[0]
-        comma = u" \u0648 " if self.code.startswith("fa") else u", "
+        comma = " \u0648 " if self.code.startswith("fa") else ", "
         return _("%(commas)s and %(last)s") % {
             "commas": comma.join(parts[:-1]),
             "last": parts[len(parts) - 1],
         }
 
     def friendly_number(self, value: int) -> str:
         """Returns a comma-separated number for the given integer."""
```

### Comparing `tornado-6.2b2/tornado/locks.py` & `tornado-6.3b1/tornado/locks.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/log.py` & `tornado-6.3b1/tornado/log.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/netutil.py` & `tornado-6.3b1/tornado/netutil.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,18 +40,18 @@
     _server_ssl_defaults.options |= ssl.OP_NO_COMPRESSION
 
 # ThreadedResolver runs getaddrinfo on a thread. If the hostname is unicode,
 # getaddrinfo attempts to import encodings.idna. If this is done at
 # module-import time, the import lock is already held by the main thread,
 # leading to deadlock. Avoid it by caching the idna encoder on the main
 # thread now.
-u"foo".encode("idna")
+"foo".encode("idna")
 
 # For undiagnosed reasons, 'latin1' codec may also need to be preloaded.
-u"foo".encode("latin1")
+"foo".encode("latin1")
 
 # Default backlog used when calling sock.listen()
 _DEFAULT_BACKLOG = 128
 
 
 def bind_sockets(
     port: int,
@@ -111,15 +111,15 @@
         unique_addresses.add(res)
 
         af, socktype, proto, canonname, sockaddr = res
         if (
             sys.platform == "darwin"
             and address == "localhost"
             and af == socket.AF_INET6
-            and sockaddr[3] != 0
+            and sockaddr[3] != 0  # type: ignore
         ):
             # Mac OS X includes a link-local address fe80::1%lo0 in the
             # getaddrinfo results for 'localhost'.  However, the firewall
             # doesn't understand that this is a local address and will
             # prompt for access (often repeatedly, due to an apparent
             # bug in its ability to remember granting access to an
             # application). Skip these addresses.
```

### Comparing `tornado-6.2b2/tornado/options.py` & `tornado-6.3b1/tornado/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 when the modules are loaded.  However, all modules that define options
 must have been imported before the command line is parsed.
 
 Your ``main()`` method can parse the command line or parse a config file with
 either `parse_command_line` or `parse_config_file`::
 
     import myapp.db, myapp.server
-    import tornado.options
+    import tornado
 
     if __name__ == '__main__':
         tornado.options.parse_command_line()
         # or
         tornado.options.parse_config_file("/etc/server.conf")
 
 .. note::
@@ -423,15 +423,17 @@
                     if not isinstance(config[name], (list, str)):
                         raise Error(
                             "Option %r is required to be a list of %s "
                             "or a comma-separated string"
                             % (option.name, option.type.__name__)
                         )
 
-                if type(config[name]) == str and option.type != str:
+                if type(config[name]) == str and (
+                    option.type != str or option.multiple
+                ):
                     option.parse(config[name])
                 else:
                     option.set(config[name])
 
         if final:
             self.run_parse_callbacks()
```

### Comparing `tornado-6.2b2/tornado/platform/asyncio.py` & `tornado-6.3b1/tornado/platform/asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,18 @@
 import sys
 import threading
 import typing
 import warnings
 from tornado.gen import convert_yielded
 from tornado.ioloop import IOLoop, _Selectable
 
-from typing import Any, TypeVar, Awaitable, Callable, Union, Optional, List, Tuple, Dict
+from typing import Any, TypeVar, Awaitable, Callable, Union, Optional, List, Dict
 
 if typing.TYPE_CHECKING:
-    from typing import Set  # noqa: F401
+    from typing import Set, Tuple  # noqa: F401
     from typing_extensions import Protocol
 
     class _HasFileno(Protocol):
         def fileno(self) -> int:
             pass
 
     _FileDescriptorLike = Union[int, _HasFileno]
@@ -70,28 +70,14 @@
         # I've never been able to reproduce locally.
         loop._thread.join()
     _selector_loops.clear()
 
 
 atexit.register(_atexit_callback)
 
-if sys.version_info >= (3, 10):
-
-    def _get_event_loop() -> asyncio.AbstractEventLoop:
-        try:
-            return asyncio.get_running_loop()
-        except RuntimeError:
-            pass
-
-        return asyncio.get_event_loop_policy().get_event_loop()
-
-
-else:
-    from asyncio import get_event_loop as _get_event_loop
-
 
 class BaseAsyncIOLoop(IOLoop):
     def initialize(  # type: ignore
         self, asyncio_loop: asyncio.AbstractEventLoop, **kwargs: Any
     ) -> None:
         # asyncio_loop is always the real underlying IOLoop. This is used in
         # ioloop.py to maintain the asyncio-to-ioloop mappings.
@@ -127,31 +113,22 @@
             if loop.is_closed():
                 try:
                     del IOLoop._ioloop_for_asyncio[loop]
                 except KeyError:
                     pass
 
         # Make sure we don't already have an IOLoop for this asyncio loop
-        if asyncio_loop in IOLoop._ioloop_for_asyncio:
-            existing_loop = IOLoop._ioloop_for_asyncio[asyncio_loop]
+        existing_loop = IOLoop._ioloop_for_asyncio.setdefault(asyncio_loop, self)
+        if existing_loop is not self:
             raise RuntimeError(
                 f"IOLoop {existing_loop} already associated with asyncio loop {asyncio_loop}"
             )
 
-        IOLoop._ioloop_for_asyncio[asyncio_loop] = self
-
-        self._thread_identity = 0
-
         super().initialize(**kwargs)
 
-        def assign_thread_identity() -> None:
-            self._thread_identity = threading.get_ident()
-
-        self.add_callback(assign_thread_identity)
-
     def close(self, all_fds: bool = False) -> None:
         self.closing = True
         for fd in list(self.handlers):
             fileobj, handler_func = self.handlers[fd]
             self.remove_handler(fd)
             if all_fds:
                 self.close_fd(fileobj)
@@ -211,23 +188,15 @@
         del self.handlers[fd]
 
     def _handle_events(self, fd: int, events: int) -> None:
         fileobj, handler_func = self.handlers[fd]
         handler_func(fileobj, events)
 
     def start(self) -> None:
-        try:
-            old_loop = _get_event_loop()
-        except (RuntimeError, AssertionError):
-            old_loop = None  # type: ignore
-        try:
-            asyncio.set_event_loop(self.asyncio_loop)
-            self.asyncio_loop.run_forever()
-        finally:
-            asyncio.set_event_loop(old_loop)
+        self.asyncio_loop.run_forever()
 
     def stop(self) -> None:
         self.asyncio_loop.stop()
 
     def call_at(
         self, when: float, callback: Callable, *args: Any, **kwargs: Any
     ) -> object:
@@ -240,18 +209,22 @@
             functools.partial(callback, *args, **kwargs),
         )
 
     def remove_timeout(self, timeout: object) -> None:
         timeout.cancel()  # type: ignore
 
     def add_callback(self, callback: Callable, *args: Any, **kwargs: Any) -> None:
-        if threading.get_ident() == self._thread_identity:
-            call_soon = self.asyncio_loop.call_soon
-        else:
+        try:
+            if asyncio.get_running_loop() is self.asyncio_loop:
+                call_soon = self.asyncio_loop.call_soon
+            else:
+                call_soon = self.asyncio_loop.call_soon_threadsafe
+        except RuntimeError:
             call_soon = self.asyncio_loop.call_soon_threadsafe
+
         try:
             call_soon(self._run_callback, functools.partial(callback, *args, **kwargs))
         except RuntimeError:
             # "Event loop is closed". Swallow the exception for
             # consistency with PollIOLoop (and logical consistency
             # with the fact that we can't guarantee that an
             # add_callback that completes without error will
@@ -299,15 +272,15 @@
 
        Closing an `AsyncIOMainLoop` now closes the underlying asyncio loop.
     """
 
     def initialize(self, **kwargs: Any) -> None:  # type: ignore
         super().initialize(asyncio.get_event_loop(), **kwargs)
 
-    def make_current(self) -> None:
+    def _make_current(self) -> None:
         # AsyncIOMainLoop already refers to the current asyncio loop so
         # nothing to do here.
         pass
 
 
 class AsyncIOLoop(BaseAsyncIOLoop):
     """``AsyncIOLoop`` is an `.IOLoop` that runs on an ``asyncio`` event loop.
@@ -350,20 +323,15 @@
             raise
 
     def close(self, all_fds: bool = False) -> None:
         if self.is_current:
             self._clear_current()
         super().close(all_fds=all_fds)
 
-    def make_current(self) -> None:
-        warnings.warn(
-            "make_current is deprecated; start the event loop first",
-            DeprecationWarning,
-            stacklevel=2,
-        )
+    def _make_current(self) -> None:
         if not self.is_current:
             try:
                 self.old_asyncio = asyncio.get_event_loop()
             except (RuntimeError, AssertionError):
                 self.old_asyncio = None  # type: ignore
             self.is_current = True
         asyncio.set_event_loop(self.asyncio_loop)
@@ -673,14 +641,22 @@
 
     def add_writer(
         self, fd: "_FileDescriptorLike", callback: Callable[..., None], *args: Any
     ) -> None:
         self._writers[fd] = functools.partial(callback, *args)
         self._wake_selector()
 
-    def remove_reader(self, fd: "_FileDescriptorLike") -> None:
-        del self._readers[fd]
+    def remove_reader(self, fd: "_FileDescriptorLike") -> bool:
+        try:
+            del self._readers[fd]
+        except KeyError:
+            return False
         self._wake_selector()
+        return True
 
-    def remove_writer(self, fd: "_FileDescriptorLike") -> None:
-        del self._writers[fd]
+    def remove_writer(self, fd: "_FileDescriptorLike") -> bool:
+        try:
+            del self._writers[fd]
+        except KeyError:
+            return False
         self._wake_selector()
+        return True
```

### Comparing `tornado-6.2b2/tornado/platform/caresresolver.py` & `tornado-6.3b1/tornado/platform/caresresolver.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,22 +11,23 @@
 if typing.TYPE_CHECKING:
     from typing import Generator, Any, List, Tuple, Dict  # noqa: F401
 
 
 class CaresResolver(Resolver):
     """Name resolver based on the c-ares library.
 
-    This is a non-blocking and non-threaded resolver.  It may not produce
-    the same results as the system resolver, but can be used for non-blocking
+    This is a non-blocking and non-threaded resolver.  It may not produce the
+    same results as the system resolver, but can be used for non-blocking
     resolution when threads cannot be used.
 
-    c-ares fails to resolve some names when ``family`` is ``AF_UNSPEC``,
-    so it is only recommended for use in ``AF_INET`` (i.e. IPv4).  This is
-    the default for ``tornado.simple_httpclient``, but other libraries
-    may default to ``AF_UNSPEC``.
+    ``pycares`` will not return a mix of ``AF_INET`` and ``AF_INET6`` when
+    ``family`` is ``AF_UNSPEC``, so it is only recommended for use in
+    ``AF_INET`` (i.e. IPv4).  This is the default for
+    ``tornado.simple_httpclient``, but other libraries may default to
+    ``AF_UNSPEC``.
 
     .. versionchanged:: 5.0
        The ``io_loop`` argument (deprecated since version 4.1) has been removed.
 
     .. deprecated:: 6.2
        This class is deprecated and will be removed in Tornado 7.0. Use the default
        thread-based resolver instead.
```

### Comparing `tornado-6.2b2/tornado/platform/twisted.py` & `tornado-6.3b1/tornado/platform/twisted.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/process.py` & `tornado-6.3b1/tornado/process.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/queues.py` & `tornado-6.3b1/tornado/queues.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     def _init(self) -> None:
         self._queue = []
 
     def _put(self, item: _T) -> None:
         heapq.heappush(self._queue, item)
 
-    def _get(self) -> _T:
+    def _get(self) -> _T:  # type: ignore[type-var]
         return heapq.heappop(self._queue)
 
 
 class LifoQueue(Queue):
     """A `.Queue` that retrieves the most recently put items first.
 
     .. testcode::
@@ -414,9 +414,9 @@
 
     def _init(self) -> None:
         self._queue = []
 
     def _put(self, item: _T) -> None:
         self._queue.append(item)
 
-    def _get(self) -> _T:
+    def _get(self) -> _T:  # type: ignore[type-var]
         return self._queue.pop()
```

### Comparing `tornado-6.2b2/tornado/routing.py` & `tornado-6.3b1/tornado/routing.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/simple_httpclient.py` & `tornado-6.3b1/tornado/simple_httpclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -543,15 +543,15 @@
 
     def _handle_exception(
         self,
         typ: "Optional[Type[BaseException]]",
         value: Optional[BaseException],
         tb: Optional[TracebackType],
     ) -> bool:
-        if self.final_callback:
+        if self.final_callback is not None:
             self._remove_timeout()
             if isinstance(value, StreamClosedError):
                 if value.real_error is None:
                     value = HTTPStreamClosedError("Stream closed")
                 else:
                     value = value.real_error
             self._run_callback(
```

### Comparing `tornado-6.2b2/tornado/speedups.c` & `tornado-6.3b1/tornado/speedups.c`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/tcpclient.py` & `tornado-6.3b1/tornado/tcpclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,23 +17,27 @@
 """
 
 import functools
 import socket
 import numbers
 import datetime
 import ssl
+import typing
 
 from tornado.concurrent import Future, future_add_done_callback
 from tornado.ioloop import IOLoop
 from tornado.iostream import IOStream
 from tornado import gen
 from tornado.netutil import Resolver
 from tornado.gen import TimeoutError
 
-from typing import Any, Union, Dict, Tuple, List, Callable, Iterator, Optional, Set
+from typing import Any, Union, Dict, Tuple, List, Callable, Iterator, Optional
+
+if typing.TYPE_CHECKING:
+    from typing import Set  # noqa(F401)
 
 _INITIAL_CONNECT_TIMEOUT = 0.3
 
 
 class _Connector(object):
     """A stateless implementation of the "Happy Eyeballs" algorithm.
```

### Comparing `tornado-6.2b2/tornado/tcpserver.py` & `tornado-6.3b1/tornado/tcpserver.py`

 * *Files 4% similar despite different names*

```diff
@@ -242,17 +242,15 @@
            Added the ``reuse_port`` argument.
 
         .. versionchanged:: 6.2
            Added the ``flags`` argument to match `.bind_sockets`.
 
         .. deprecated:: 6.2
            Use either ``listen()`` or ``add_sockets()`` instead of ``bind()``
-           and ``start()``. The ``bind()/start()`` pattern depends on
-           interfaces that have been deprecated in Python 3.10 and will be
-           removed in future versions of Python.
+           and ``start()``.
         """
         sockets = bind_sockets(
             port,
             address=address,
             family=family,
             backlog=backlog,
             flags=flags,
@@ -291,17 +289,15 @@
 
         .. versionchanged:: 6.0
 
            Added ``max_restarts`` argument.
 
         .. deprecated:: 6.2
            Use either ``listen()`` or ``add_sockets()`` instead of ``bind()``
-           and ``start()``. The ``bind()/start()`` pattern depends on
-           interfaces that have been deprecated in Python 3.10 and will be
-           removed in future versions of Python.
+           and ``start()``.
         """
         assert not self._started
         self._started = True
         if num_processes != 1:
             process.fork_processes(num_processes, max_restarts)
         sockets = self._pending_sockets
         self._pending_sockets = []
```

### Comparing `tornado-6.2b2/tornado/template.py` & `tornado-6.3b1/tornado/template.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/test/asyncio_test.py` & `tornado-6.3b1/tornado/test/asyncio_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     to_asyncio_future,
     AnyThreadEventLoopPolicy,
 )
 from tornado.testing import AsyncTestCase, gen_test
 
 
 class AsyncIOLoopTest(AsyncTestCase):
-    def get_new_ioloop(self):
-        io_loop = AsyncIOLoop(make_current=False)
-        return io_loop
+    @property
+    def asyncio_loop(self):
+        return self.io_loop.asyncio_loop  # type: ignore
 
     def test_asyncio_callback(self):
         # Basic test that the asyncio loop is set up correctly.
         async def add_callback():
             asyncio.get_event_loop().call_soon(self.stop)
 
         self.asyncio_loop.run_until_complete(add_callback())
@@ -100,30 +100,33 @@
             self.asyncio_loop.run_until_complete(native_coroutine_with_adapter()),
             42,
         )
         self.assertEqual(
             self.asyncio_loop.run_until_complete(native_coroutine_with_adapter2()),
             42,
         )
-        # I'm not entirely sure why this manual cleanup is necessary but without
-        # it we have at-a-distance failures in ioloop_test.TestIOLoopCurrent.
-        asyncio.set_event_loop(None)
 
 
 class LeakTest(unittest.TestCase):
     def setUp(self):
         # Trigger a cleanup of the mapping so we start with a clean slate.
         AsyncIOLoop(make_current=False).close()
         # If we don't clean up after ourselves other tests may fail on
         # py34.
         self.orig_policy = asyncio.get_event_loop_policy()
         asyncio.set_event_loop_policy(asyncio.DefaultEventLoopPolicy())
 
     def tearDown(self):
-        asyncio.get_event_loop_policy().get_event_loop().close()
+        try:
+            loop = asyncio.get_event_loop_policy().get_event_loop()
+        except Exception:
+            # We may not have a current event loop at this point.
+            pass
+        else:
+            loop.close()
         asyncio.set_event_loop_policy(self.orig_policy)
 
     def test_ioloop_close_leak(self):
         orig_count = len(IOLoop._ioloop_for_asyncio)
         for i in range(10):
             # Create and close an AsyncIOLoop using Tornado interfaces.
             with warnings.catch_warnings():
@@ -169,29 +172,38 @@
             loop = asyncio.get_event_loop()
             loop.close()
             return loop
 
         future = self.executor.submit(get_and_close_event_loop)
         return future.result()
 
-    def run_policy_test(self, accessor, expected_type):
+    def test_asyncio_accessor(self):
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", DeprecationWarning)
             # With the default policy, non-main threads don't get an event
             # loop.
             self.assertRaises(
-                (RuntimeError, AssertionError), self.executor.submit(accessor).result
+                RuntimeError, self.executor.submit(asyncio.get_event_loop).result
             )
             # Set the policy and we can get a loop.
             asyncio.set_event_loop_policy(AnyThreadEventLoopPolicy())
             self.assertIsInstance(
-                self.executor.submit(accessor).result(), expected_type
+                self.executor.submit(asyncio.get_event_loop).result(),
+                asyncio.AbstractEventLoop,
             )
             # Clean up to silence leak warnings. Always use asyncio since
             # IOLoop doesn't (currently) close the underlying loop.
             self.executor.submit(lambda: asyncio.get_event_loop().close()).result()  # type: ignore
 
-    def test_asyncio_accessor(self):
-        self.run_policy_test(asyncio.get_event_loop, asyncio.AbstractEventLoop)
-
     def test_tornado_accessor(self):
-        self.run_policy_test(IOLoop.current, IOLoop)
+        # Tornado's IOLoop.current() API can create a loop for any thread,
+        # regardless of this event loop policy.
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", DeprecationWarning)
+            self.assertIsInstance(self.executor.submit(IOLoop.current).result(), IOLoop)
+            # Clean up to silence leak warnings. Always use asyncio since
+            # IOLoop doesn't (currently) close the underlying loop.
+            self.executor.submit(lambda: asyncio.get_event_loop().close()).result()  # type: ignore
+
+            asyncio.set_event_loop_policy(AnyThreadEventLoopPolicy())
+            self.assertIsInstance(self.executor.submit(IOLoop.current).result(), IOLoop)
+            self.executor.submit(lambda: asyncio.get_event_loop().close()).result()  # type: ignore
```

### Comparing `tornado-6.2b2/tornado/test/auth_test.py` & `tornado-6.3b1/tornado/test/auth_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -498,22 +498,22 @@
             headers={"Cookie": "_oauth_request_token=enhjdg==|MTIzNA=="},
         )
         response.rethrow()
         parsed = json_decode(response.body)
         self.assertEqual(
             parsed,
             {
-                u"access_token": {
-                    u"key": u"hjkl",
-                    u"screen_name": u"foo",
-                    u"secret": u"vbnm",
+                "access_token": {
+                    "key": "hjkl",
+                    "screen_name": "foo",
+                    "secret": "vbnm",
                 },
-                u"name": u"Foo",
-                u"screen_name": u"foo",
-                u"username": u"foo",
+                "name": "Foo",
+                "screen_name": "foo",
+                "username": "foo",
             },
         )
 
     def test_twitter_show_user(self):
         response = self.fetch("/twitter/client/show_user?name=somebody")
         response.rethrow()
         self.assertEqual(
@@ -597,13 +597,13 @@
             },
         )
 
     def test_google_login(self):
         response = self.fetch("/client/login")
         self.assertDictEqual(
             {
-                u"name": u"Foo",
-                u"email": u"foo@example.com",
-                u"access_token": u"fake-access-token",
+                "name": "Foo",
+                "email": "foo@example.com",
+                "access_token": "fake-access-token",
             },
             json_decode(response.body),
         )
```

### Comparing `tornado-6.2b2/tornado/test/autoreload_test.py` & `tornado-6.3b1/tornado/test/autoreload_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/test/concurrent_test.py` & `tornado-6.3b1/tornado/test/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/test/curl_httpclient_test.py` & `tornado-6.3b1/tornado/test/curl_httpclient_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/test/escape_test.py` & `tornado-6.3b1/tornado/test/escape_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-import tornado.escape
+import tornado
 from tornado.escape import (
     utf8,
     xhtml_escape,
     xhtml_unescape,
     url_escape,
     url_unescape,
     to_unicode,
@@ -18,250 +18,250 @@
 from typing import List, Tuple, Union, Dict, Any  # noqa: F401
 
 linkify_tests = [
     # (input, linkify_kwargs, expected_output)
     (
         "hello http://world.com/!",
         {},
-        u'hello <a href="http://world.com/">http://world.com/</a>!',
+        'hello <a href="http://world.com/">http://world.com/</a>!',
     ),
     (
         "hello http://world.com/with?param=true&stuff=yes",
         {},
-        u'hello <a href="http://world.com/with?param=true&amp;stuff=yes">http://world.com/with?param=true&amp;stuff=yes</a>',  # noqa: E501
+        'hello <a href="http://world.com/with?param=true&amp;stuff=yes">http://world.com/with?param=true&amp;stuff=yes</a>',  # noqa: E501
     ),
     # an opened paren followed by many chars killed Gruber's regex
     (
         "http://url.com/w(aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa",
         {},
-        u'<a href="http://url.com/w">http://url.com/w</a>(aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa',  # noqa: E501
+        '<a href="http://url.com/w">http://url.com/w</a>(aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa',  # noqa: E501
     ),
     # as did too many dots at the end
     (
         "http://url.com/withmany.......................................",
         {},
-        u'<a href="http://url.com/withmany">http://url.com/withmany</a>.......................................',  # noqa: E501
+        '<a href="http://url.com/withmany">http://url.com/withmany</a>.......................................',  # noqa: E501
     ),
     (
         "http://url.com/withmany((((((((((((((((((((((((((((((((((a)",
         {},
-        u'<a href="http://url.com/withmany">http://url.com/withmany</a>((((((((((((((((((((((((((((((((((a)',  # noqa: E501
+        '<a href="http://url.com/withmany">http://url.com/withmany</a>((((((((((((((((((((((((((((((((((a)',  # noqa: E501
     ),
     # some examples from http://daringfireball.net/2009/11/liberal_regex_for_matching_urls
     # plus a fex extras (such as multiple parentheses).
     (
         "http://foo.com/blah_blah",
         {},
-        u'<a href="http://foo.com/blah_blah">http://foo.com/blah_blah</a>',
+        '<a href="http://foo.com/blah_blah">http://foo.com/blah_blah</a>',
     ),
     (
         "http://foo.com/blah_blah/",
         {},
-        u'<a href="http://foo.com/blah_blah/">http://foo.com/blah_blah/</a>',
+        '<a href="http://foo.com/blah_blah/">http://foo.com/blah_blah/</a>',
     ),
     (
         "(Something like http://foo.com/blah_blah)",
         {},
-        u'(Something like <a href="http://foo.com/blah_blah">http://foo.com/blah_blah</a>)',
+        '(Something like <a href="http://foo.com/blah_blah">http://foo.com/blah_blah</a>)',
     ),
     (
         "http://foo.com/blah_blah_(wikipedia)",
         {},
-        u'<a href="http://foo.com/blah_blah_(wikipedia)">http://foo.com/blah_blah_(wikipedia)</a>',
+        '<a href="http://foo.com/blah_blah_(wikipedia)">http://foo.com/blah_blah_(wikipedia)</a>',
     ),
     (
         "http://foo.com/blah_(blah)_(wikipedia)_blah",
         {},
-        u'<a href="http://foo.com/blah_(blah)_(wikipedia)_blah">http://foo.com/blah_(blah)_(wikipedia)_blah</a>',  # noqa: E501
+        '<a href="http://foo.com/blah_(blah)_(wikipedia)_blah">http://foo.com/blah_(blah)_(wikipedia)_blah</a>',  # noqa: E501
     ),
     (
         "(Something like http://foo.com/blah_blah_(wikipedia))",
         {},
-        u'(Something like <a href="http://foo.com/blah_blah_(wikipedia)">http://foo.com/blah_blah_(wikipedia)</a>)',  # noqa: E501
+        '(Something like <a href="http://foo.com/blah_blah_(wikipedia)">http://foo.com/blah_blah_(wikipedia)</a>)',  # noqa: E501
     ),
     (
         "http://foo.com/blah_blah.",
         {},
-        u'<a href="http://foo.com/blah_blah">http://foo.com/blah_blah</a>.',
+        '<a href="http://foo.com/blah_blah">http://foo.com/blah_blah</a>.',
     ),
     (
         "http://foo.com/blah_blah/.",
         {},
-        u'<a href="http://foo.com/blah_blah/">http://foo.com/blah_blah/</a>.',
+        '<a href="http://foo.com/blah_blah/">http://foo.com/blah_blah/</a>.',
     ),
     (
         "<http://foo.com/blah_blah>",
         {},
-        u'&lt;<a href="http://foo.com/blah_blah">http://foo.com/blah_blah</a>&gt;',
+        '&lt;<a href="http://foo.com/blah_blah">http://foo.com/blah_blah</a>&gt;',
     ),
     (
         "<http://foo.com/blah_blah/>",
         {},
-        u'&lt;<a href="http://foo.com/blah_blah/">http://foo.com/blah_blah/</a>&gt;',
+        '&lt;<a href="http://foo.com/blah_blah/">http://foo.com/blah_blah/</a>&gt;',
     ),
     (
         "http://foo.com/blah_blah,",
         {},
-        u'<a href="http://foo.com/blah_blah">http://foo.com/blah_blah</a>,',
+        '<a href="http://foo.com/blah_blah">http://foo.com/blah_blah</a>,',
     ),
     (
         "http://www.example.com/wpstyle/?p=364.",
         {},
-        u'<a href="http://www.example.com/wpstyle/?p=364">http://www.example.com/wpstyle/?p=364</a>.',  # noqa: E501
+        '<a href="http://www.example.com/wpstyle/?p=364">http://www.example.com/wpstyle/?p=364</a>.',  # noqa: E501
     ),
     (
         "rdar://1234",
         {"permitted_protocols": ["http", "rdar"]},
-        u'<a href="rdar://1234">rdar://1234</a>',
+        '<a href="rdar://1234">rdar://1234</a>',
     ),
     (
         "rdar:/1234",
         {"permitted_protocols": ["rdar"]},
-        u'<a href="rdar:/1234">rdar:/1234</a>',
+        '<a href="rdar:/1234">rdar:/1234</a>',
     ),
     (
         "http://userid:password@example.com:8080",
         {},
-        u'<a href="http://userid:password@example.com:8080">http://userid:password@example.com:8080</a>',  # noqa: E501
+        '<a href="http://userid:password@example.com:8080">http://userid:password@example.com:8080</a>',  # noqa: E501
     ),
     (
         "http://userid@example.com",
         {},
-        u'<a href="http://userid@example.com">http://userid@example.com</a>',
+        '<a href="http://userid@example.com">http://userid@example.com</a>',
     ),
     (
         "http://userid@example.com:8080",
         {},
-        u'<a href="http://userid@example.com:8080">http://userid@example.com:8080</a>',
+        '<a href="http://userid@example.com:8080">http://userid@example.com:8080</a>',
     ),
     (
         "http://userid:password@example.com",
         {},
-        u'<a href="http://userid:password@example.com">http://userid:password@example.com</a>',
+        '<a href="http://userid:password@example.com">http://userid:password@example.com</a>',
     ),
     (
         "message://%3c330e7f8409726r6a4ba78dkf1fd71420c1bf6ff@mail.gmail.com%3e",
         {"permitted_protocols": ["http", "message"]},
-        u'<a href="message://%3c330e7f8409726r6a4ba78dkf1fd71420c1bf6ff@mail.gmail.com%3e">'
-        u"message://%3c330e7f8409726r6a4ba78dkf1fd71420c1bf6ff@mail.gmail.com%3e</a>",
+        '<a href="message://%3c330e7f8409726r6a4ba78dkf1fd71420c1bf6ff@mail.gmail.com%3e">'
+        "message://%3c330e7f8409726r6a4ba78dkf1fd71420c1bf6ff@mail.gmail.com%3e</a>",
     ),
     (
-        u"http://\u27a1.ws/\u4a39",
+        "http://\u27a1.ws/\u4a39",
         {},
-        u'<a href="http://\u27a1.ws/\u4a39">http://\u27a1.ws/\u4a39</a>',
+        '<a href="http://\u27a1.ws/\u4a39">http://\u27a1.ws/\u4a39</a>',
     ),
     (
         "<tag>http://example.com</tag>",
         {},
-        u'&lt;tag&gt;<a href="http://example.com">http://example.com</a>&lt;/tag&gt;',
+        '&lt;tag&gt;<a href="http://example.com">http://example.com</a>&lt;/tag&gt;',
     ),
     (
         "Just a www.example.com link.",
         {},
-        u'Just a <a href="http://www.example.com">www.example.com</a> link.',
+        'Just a <a href="http://www.example.com">www.example.com</a> link.',
     ),
     (
         "Just a www.example.com link.",
         {"require_protocol": True},
-        u"Just a www.example.com link.",
+        "Just a www.example.com link.",
     ),
     (
         "A http://reallylong.com/link/that/exceedsthelenglimit.html",
         {"require_protocol": True, "shorten": True},
-        u'A <a href="http://reallylong.com/link/that/exceedsthelenglimit.html"'
-        u' title="http://reallylong.com/link/that/exceedsthelenglimit.html">http://reallylong.com/link...</a>',  # noqa: E501
+        'A <a href="http://reallylong.com/link/that/exceedsthelenglimit.html"'
+        ' title="http://reallylong.com/link/that/exceedsthelenglimit.html">http://reallylong.com/link...</a>',  # noqa: E501
     ),
     (
         "A http://reallylongdomainnamethatwillbetoolong.com/hi!",
         {"shorten": True},
-        u'A <a href="http://reallylongdomainnamethatwillbetoolong.com/hi"'
-        u' title="http://reallylongdomainnamethatwillbetoolong.com/hi">http://reallylongdomainnametha...</a>!',  # noqa: E501
+        'A <a href="http://reallylongdomainnamethatwillbetoolong.com/hi"'
+        ' title="http://reallylongdomainnamethatwillbetoolong.com/hi">http://reallylongdomainnametha...</a>!',  # noqa: E501
     ),
     (
         "A file:///passwords.txt and http://web.com link",
         {},
-        u'A file:///passwords.txt and <a href="http://web.com">http://web.com</a> link',
+        'A file:///passwords.txt and <a href="http://web.com">http://web.com</a> link',
     ),
     (
         "A file:///passwords.txt and http://web.com link",
         {"permitted_protocols": ["file"]},
-        u'A <a href="file:///passwords.txt">file:///passwords.txt</a> and http://web.com link',
+        'A <a href="file:///passwords.txt">file:///passwords.txt</a> and http://web.com link',
     ),
     (
         "www.external-link.com",
         {"extra_params": 'rel="nofollow" class="external"'},
-        u'<a href="http://www.external-link.com" rel="nofollow" class="external">www.external-link.com</a>',  # noqa: E501
+        '<a href="http://www.external-link.com" rel="nofollow" class="external">www.external-link.com</a>',  # noqa: E501
     ),
     (
         "www.external-link.com and www.internal-link.com/blogs extra",
         {
             "extra_params": lambda href: 'class="internal"'
             if href.startswith("http://www.internal-link.com")
             else 'rel="nofollow" class="external"'
         },
-        u'<a href="http://www.external-link.com" rel="nofollow" class="external">www.external-link.com</a>'  # noqa: E501
-        u' and <a href="http://www.internal-link.com/blogs" class="internal">www.internal-link.com/blogs</a> extra',  # noqa: E501
+        '<a href="http://www.external-link.com" rel="nofollow" class="external">www.external-link.com</a>'  # noqa: E501
+        ' and <a href="http://www.internal-link.com/blogs" class="internal">www.internal-link.com/blogs</a> extra',  # noqa: E501
     ),
     (
         "www.external-link.com",
         {"extra_params": lambda href: '    rel="nofollow" class="external"  '},
-        u'<a href="http://www.external-link.com" rel="nofollow" class="external">www.external-link.com</a>',  # noqa: E501
+        '<a href="http://www.external-link.com" rel="nofollow" class="external">www.external-link.com</a>',  # noqa: E501
     ),
 ]  # type: List[Tuple[Union[str, bytes], Dict[str, Any], str]]
 
 
 class EscapeTestCase(unittest.TestCase):
     def test_linkify(self):
         for text, kwargs, html in linkify_tests:
             linked = tornado.escape.linkify(text, **kwargs)
             self.assertEqual(linked, html)
 
     def test_xhtml_escape(self):
         tests = [
             ("<foo>", "&lt;foo&gt;"),
-            (u"<foo>", u"&lt;foo&gt;"),
+            ("<foo>", "&lt;foo&gt;"),
             (b"<foo>", b"&lt;foo&gt;"),
             ("<>&\"'", "&lt;&gt;&amp;&quot;&#39;"),
             ("&amp;", "&amp;amp;"),
-            (u"<\u00e9>", u"&lt;\u00e9&gt;"),
+            ("<\u00e9>", "&lt;\u00e9&gt;"),
             (b"<\xc3\xa9>", b"&lt;\xc3\xa9&gt;"),
         ]  # type: List[Tuple[Union[str, bytes], Union[str, bytes]]]
         for unescaped, escaped in tests:
             self.assertEqual(utf8(xhtml_escape(unescaped)), utf8(escaped))
             self.assertEqual(utf8(unescaped), utf8(xhtml_unescape(escaped)))
 
     def test_xhtml_unescape_numeric(self):
         tests = [
             ("foo&#32;bar", "foo bar"),
             ("foo&#x20;bar", "foo bar"),
             ("foo&#X20;bar", "foo bar"),
-            ("foo&#xabc;bar", u"foo\u0abcbar"),
+            ("foo&#xabc;bar", "foo\u0abcbar"),
             ("foo&#xyz;bar", "foo&#xyz;bar"),  # invalid encoding
             ("foo&#;bar", "foo&#;bar"),  # invalid encoding
             ("foo&#x;bar", "foo&#x;bar"),  # invalid encoding
         ]
         for escaped, unescaped in tests:
             self.assertEqual(unescaped, xhtml_unescape(escaped))
 
     def test_url_escape_unicode(self):
         tests = [
             # byte strings are passed through as-is
-            (u"\u00e9".encode("utf8"), "%C3%A9"),
-            (u"\u00e9".encode("latin1"), "%E9"),
+            ("\u00e9".encode("utf8"), "%C3%A9"),
+            ("\u00e9".encode("latin1"), "%E9"),
             # unicode strings become utf8
-            (u"\u00e9", "%C3%A9"),
+            ("\u00e9", "%C3%A9"),
         ]  # type: List[Tuple[Union[str, bytes], str]]
         for unescaped, escaped in tests:
             self.assertEqual(url_escape(unescaped), escaped)
 
     def test_url_unescape_unicode(self):
         tests = [
-            ("%C3%A9", u"\u00e9", "utf8"),
-            ("%C3%A9", u"\u00c3\u00a9", "latin1"),
-            ("%C3%A9", utf8(u"\u00e9"), None),
+            ("%C3%A9", "\u00e9", "utf8"),
+            ("%C3%A9", "\u00c3\u00a9", "latin1"),
+            ("%C3%A9", utf8("\u00e9"), None),
         ]
         for escaped, unescaped, encoding in tests:
             # input strings to url_unescape should only contain ascii
             # characters, but make sure the function accepts both byte
             # and unicode strings.
             self.assertEqual(url_unescape(to_unicode(escaped), encoding), unescaped)
             self.assertEqual(url_unescape(utf8(escaped), encoding), unescaped)
@@ -279,44 +279,44 @@
             url_unescape(escaped, encoding=None, plus=False), utf8(unescaped)
         )
 
     def test_escape_return_types(self):
         # On python2 the escape methods should generally return the same
         # type as their argument
         self.assertEqual(type(xhtml_escape("foo")), str)
-        self.assertEqual(type(xhtml_escape(u"foo")), unicode_type)
+        self.assertEqual(type(xhtml_escape("foo")), unicode_type)
 
     def test_json_decode(self):
         # json_decode accepts both bytes and unicode, but strings it returns
         # are always unicode.
-        self.assertEqual(json_decode(b'"foo"'), u"foo")
-        self.assertEqual(json_decode(u'"foo"'), u"foo")
+        self.assertEqual(json_decode(b'"foo"'), "foo")
+        self.assertEqual(json_decode('"foo"'), "foo")
 
         # Non-ascii bytes are interpreted as utf8
-        self.assertEqual(json_decode(utf8(u'"\u00e9"')), u"\u00e9")
+        self.assertEqual(json_decode(utf8('"\u00e9"')), "\u00e9")
 
     def test_json_encode(self):
         # json deals with strings, not bytes.  On python 2 byte strings will
         # convert automatically if they are utf8; on python 3 byte strings
         # are not allowed.
-        self.assertEqual(json_decode(json_encode(u"\u00e9")), u"\u00e9")
+        self.assertEqual(json_decode(json_encode("\u00e9")), "\u00e9")
         if bytes is str:
-            self.assertEqual(json_decode(json_encode(utf8(u"\u00e9"))), u"\u00e9")
+            self.assertEqual(json_decode(json_encode(utf8("\u00e9"))), "\u00e9")
             self.assertRaises(UnicodeDecodeError, json_encode, b"\xe9")
 
     def test_squeeze(self):
         self.assertEqual(
-            squeeze(u"sequences     of    whitespace   chars"),
-            u"sequences of whitespace chars",
+            squeeze("sequences     of    whitespace   chars"),
+            "sequences of whitespace chars",
         )
 
     def test_recursive_unicode(self):
         tests = {
             "dict": {b"foo": b"bar"},
             "list": [b"foo", b"bar"],
             "tuple": (b"foo", b"bar"),
             "bytes": b"foo",
         }
-        self.assertEqual(recursive_unicode(tests["dict"]), {u"foo": u"bar"})
-        self.assertEqual(recursive_unicode(tests["list"]), [u"foo", u"bar"])
-        self.assertEqual(recursive_unicode(tests["tuple"]), (u"foo", u"bar"))
-        self.assertEqual(recursive_unicode(tests["bytes"]), u"foo")
+        self.assertEqual(recursive_unicode(tests["dict"]), {"foo": "bar"})
+        self.assertEqual(recursive_unicode(tests["list"]), ["foo", "bar"])
+        self.assertEqual(recursive_unicode(tests["tuple"]), ("foo", "bar"))
+        self.assertEqual(recursive_unicode(tests["bytes"]), "foo")
```

### Comparing `tornado-6.2b2/tornado/test/gen_test.py` & `tornado-6.3b1/tornado/test/gen_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1110,10 +1110,20 @@
     def test_reset(self):
         token = ctx_var.set(1)
         yield
         # reset asserts that we are still at the same level of the context tree,
         # so we must make sure that we maintain that property across yield.
         ctx_var.reset(token)
 
+    @gen_test
+    def test_propagate_to_first_yield_with_native_async_function(self):
+        x = 10
+
+        async def native_async_function():
+            self.assertEqual(ctx_var.get(), x)
+
+        ctx_var.set(x)
+        yield native_async_function()
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `tornado-6.2b2/tornado/test/gettext_translations/fr_FR/LC_MESSAGES/tornado_test.mo` & `tornado-6.3b1/tornado/test/gettext_translations/fr_FR/LC_MESSAGES/tornado_test.mo`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/test/gettext_translations/fr_FR/LC_MESSAGES/tornado_test.po` & `tornado-6.3b1/tornado/test/gettext_translations/fr_FR/LC_MESSAGES/tornado_test.po`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/test/http1connection_test.py` & `tornado-6.3b1/tornado/test/http1connection_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import socket
-import typing
+import typing  # noqa(F401)
 
 from tornado.http1connection import HTTP1Connection
 from tornado.httputil import HTTPMessageDelegate
 from tornado.iostream import IOStream
 from tornado.locks import Event
 from tornado.netutil import add_accept_handler
 from tornado.testing import AsyncTestCase, bind_unused_port, gen_test
```

### Comparing `tornado-6.2b2/tornado/test/httpclient_test.py` & `tornado-6.3b1/tornado/test/httpclient_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         self.assertEqual(
             self.fetch("/auth", auth_username="test", auth_password="123£").body,
             b"Basic dGVzdDoxMjPCow==",
         )
 
         # The standard mandates NFC. Give it a decomposed username
         # and ensure it is normalized to composed form.
-        username = unicodedata.normalize("NFD", u"josé")
+        username = unicodedata.normalize("NFD", "josé")
         self.assertEqual(
             self.fetch("/auth", auth_username=username, auth_password="səcrət").body,
             b"Basic am9zw6k6c8mZY3LJmXQ=",
         )
 
     def test_unsupported_auth_mode(self):
         # curl and simple clients handle errors a bit differently; the
@@ -376,15 +376,15 @@
 
     def test_credentials_in_url(self):
         url = self.get_url("/auth").replace("http://", "http://me:secret@")
         response = self.fetch(url)
         self.assertEqual(b"Basic " + base64.b64encode(b"me:secret"), response.body)
 
     def test_body_encoding(self):
-        unicode_body = u"\xe9"
+        unicode_body = "\xe9"
         byte_body = binascii.a2b_hex(b"e9")
 
         # unicode string in body gets converted to utf8
         response = self.fetch(
             "/echopost",
             method="POST",
             body=unicode_body,
@@ -406,15 +406,15 @@
         # Mixing unicode in headers and byte string bodies shouldn't
         # break anything
         response = self.fetch(
             "/echopost",
             method="POST",
             body=byte_body,
             headers={"Content-Type": "application/blah"},
-            user_agent=u"foo",
+            user_agent="foo",
         )
         self.assertEqual(response.headers["Content-Length"], "1")
         self.assertEqual(response.body, byte_body)
 
     def test_types(self):
         response = self.fetch("/hello")
         self.assertEqual(type(response.body), bytes)
@@ -495,15 +495,15 @@
             client.close()
 
     def test_header_types(self):
         # Header values may be passed as character or utf8 byte strings,
         # in a plain dictionary or an HTTPHeaders object.
         # Keys must always be the native str type.
         # All combinations should have the same results on the wire.
-        for value in [u"MyUserAgent", b"MyUserAgent"]:
+        for value in ["MyUserAgent", b"MyUserAgent"]:
             for container in [dict, HTTPHeaders]:
                 headers = container()
                 headers["User-Agent"] = value
                 resp = self.fetch("/user_agent", headers=headers)
                 self.assertEqual(
                     resp.body,
                     b"MyUserAgent",
@@ -547,15 +547,15 @@
     def test_header_encoding(self):
         response = yield self.http_client.fetch(
             self.get_url("/header-encoding"),
             headers={
                 "Foo": "b\xe4r",
             },
         )
-        self.assertEqual(response.body, u"b\xe4r".encode("ISO8859-1"))
+        self.assertEqual(response.body, "b\xe4r".encode("ISO8859-1"))
 
     def test_304_with_content_length(self):
         # According to the spec 304 responses SHOULD NOT include
         # Content-Length or other entity headers, but some servers do it
         # anyway.
         # http://www.w3.org/Protocols/rfc2616/rfc2616-sec10.html#sec10.3.5
         response = self.fetch("/304_with_content_length")
@@ -677,23 +677,24 @@
         response.rethrow()
         self.assertEqual(response.body, b"Put body: hello")
 
     def test_non_ascii_header(self):
         # Non-ascii headers are sent as latin1.
         response = self.fetch("/set_header?k=foo&v=%E9")
         response.rethrow()
-        self.assertEqual(response.headers["Foo"], native_str(u"\u00e9"))
+        self.assertEqual(response.headers["Foo"], native_str("\u00e9"))
 
     def test_response_times(self):
         # A few simple sanity checks of the response time fields to
         # make sure they're using the right basis (between the
         # wall-time and monotonic clocks).
         start_time = time.time()
         response = self.fetch("/hello")
         response.rethrow()
+        assert response.request_time is not None
         self.assertGreaterEqual(response.request_time, 0)
         self.assertLess(response.request_time, 1.0)
         # A very crude check to make sure that start_time is based on
         # wall time and not the monotonic clock.
         assert response.start_time is not None
         self.assertLess(abs(response.start_time - start_time), 1.0)
```

### Comparing `tornado-6.2b2/tornado/test/httpserver_test.py` & `tornado-6.3b1/tornado/test/httpserver_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,31 +277,31 @@
                 b"Content-Type: multipart/form-data; boundary=1234567890",
                 b"X-Header-encoding-test: \xe9",
             ],
             b"\r\n".join(
                 [
                     b"Content-Disposition: form-data; name=argument",
                     b"",
-                    u"\u00e1".encode("utf-8"),
+                    "\u00e1".encode("utf-8"),
                     b"--1234567890",
-                    u'Content-Disposition: form-data; name="files"; filename="\u00f3"'.encode(
+                    'Content-Disposition: form-data; name="files"; filename="\u00f3"'.encode(
                         "utf8"
                     ),
                     b"",
-                    u"\u00fa".encode("utf-8"),
+                    "\u00fa".encode("utf-8"),
                     b"--1234567890--",
                     b"",
                 ]
             ),
         )
         data = json_decode(response)
-        self.assertEqual(u"\u00e9", data["header"])
-        self.assertEqual(u"\u00e1", data["argument"])
-        self.assertEqual(u"\u00f3", data["filename"])
-        self.assertEqual(u"\u00fa", data["filebody"])
+        self.assertEqual("\u00e9", data["header"])
+        self.assertEqual("\u00e1", data["argument"])
+        self.assertEqual("\u00f3", data["filename"])
+        self.assertEqual("\u00fa", data["filebody"])
 
     def test_newlines(self):
         # We support both CRLF and bare LF as line separators.
         for newline in (b"\r\n", b"\n"):
             response = self.raw_fetch([b"GET /hello HTTP/1.0"], b"", newline=newline)
             self.assertEqual(response, b"Hello world")
 
@@ -408,25 +408,25 @@
                 ("/post_gbk", PostEchoGBKHandler),
             ]
         )
 
     def test_query_string_encoding(self):
         response = self.fetch("/echo?foo=%C3%A9")
         data = json_decode(response.body)
-        self.assertEqual(data, {u"foo": [u"\u00e9"]})
+        self.assertEqual(data, {"foo": ["\u00e9"]})
 
     def test_empty_query_string(self):
         response = self.fetch("/echo?foo=&foo=")
         data = json_decode(response.body)
-        self.assertEqual(data, {u"foo": [u"", u""]})
+        self.assertEqual(data, {"foo": ["", ""]})
 
     def test_empty_post_parameters(self):
         response = self.fetch("/echo", method="POST", body="foo=&bar=")
         data = json_decode(response.body)
-        self.assertEqual(data, {u"foo": [u""], u"bar": [u""]})
+        self.assertEqual(data, {"foo": [""], "bar": [""]})
 
     def test_types(self):
         headers = {"Cookie": "foo=bar"}
         response = self.fetch("/typecheck?foo=bar", headers=headers)
         data = json_decode(response.body)
         self.assertEqual(data, {})
 
@@ -528,15 +528,15 @@
 """.replace(
                 b"\n", b"\r\n"
             )
         )
         start_line, headers, response = self.io_loop.run_sync(
             lambda: read_stream_body(self.stream)
         )
-        self.assertEqual(json_decode(response), {u"foo": [u"bar"]})
+        self.assertEqual(json_decode(response), {"foo": ["bar"]})
 
     def test_chunked_request_uppercase(self):
         # As per RFC 2616 section 3.6, "Transfer-Encoding" header's value is
         # case-insensitive.
         self.stream.write(
             b"""\
 POST /echo HTTP/1.1
@@ -552,15 +552,15 @@
 """.replace(
                 b"\n", b"\r\n"
             )
         )
         start_line, headers, response = self.io_loop.run_sync(
             lambda: read_stream_body(self.stream)
         )
-        self.assertEqual(json_decode(response), {u"foo": [u"bar"]})
+        self.assertEqual(json_decode(response), {"foo": ["bar"]})
 
     @gen_test
     def test_invalid_content_length(self):
         with ExpectLog(
             gen_log, ".*Only integer Content-Length is allowed", level=logging.INFO
         ):
             self.stream.write(
@@ -750,15 +750,15 @@
         body = yield self.stream.read_bytes(int(headers["Content-Length"]))
         self.assertEqual(body, b"Hello world")
 
     @gen_test
     def test_unix_socket_bad_request(self):
         # Unix sockets don't have remote addresses so they just return an
         # empty string.
-        with ExpectLog(gen_log, "Malformed HTTP message from"):
+        with ExpectLog(gen_log, "Malformed HTTP message from", level=logging.INFO):
             self.stream.write(b"garbage\r\n\r\n")
             response = yield self.stream.read_until_close()
         self.assertEqual(response, b"HTTP/1.1 400 Bad Request\r\n\r\n")
 
 
 class KeepAliveTest(AsyncHTTPTestCase):
     """Tests various scenarios for HTTP 1.1 keep-alive support.
@@ -987,39 +987,39 @@
             method="POST",
             body=compressed_body,
             headers={"Content-Encoding": "gzip"},
         )
 
     def test_uncompressed(self):
         response = self.fetch("/", method="POST", body="foo=bar")
-        self.assertEqual(json_decode(response.body), {u"foo": [u"bar"]})
+        self.assertEqual(json_decode(response.body), {"foo": ["bar"]})
 
 
 class GzipTest(GzipBaseTest, AsyncHTTPTestCase):
     def get_httpserver_options(self):
         return dict(decompress_request=True)
 
     def test_gzip(self):
         response = self.post_gzip("foo=bar")
-        self.assertEqual(json_decode(response.body), {u"foo": [u"bar"]})
+        self.assertEqual(json_decode(response.body), {"foo": ["bar"]})
 
     def test_gzip_case_insensitive(self):
         # https://datatracker.ietf.org/doc/html/rfc7231#section-3.1.2.1
         bytesio = BytesIO()
         gzip_file = gzip.GzipFile(mode="w", fileobj=bytesio)
         gzip_file.write(utf8("foo=bar"))
         gzip_file.close()
         compressed_body = bytesio.getvalue()
         response = self.fetch(
             "/",
             method="POST",
             body=compressed_body,
             headers={"Content-Encoding": "GZIP"},
         )
-        self.assertEqual(json_decode(response.body), {u"foo": [u"bar"]})
+        self.assertEqual(json_decode(response.body), {"foo": ["bar"]})
 
 
 class GzipUnsupportedTest(GzipBaseTest, AsyncHTTPTestCase):
     def test_gzip_unsupported(self):
         # Gzip support is opt-in; without it the server fails to parse
         # the body (but parsing form bodies is currently just a log message,
         # not a fatal error).
```

### Comparing `tornado-6.2b2/tornado/test/httputil_test.py` & `tornado-6.3b1/tornado/test/httputil_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 Foo
 --1234--""".replace(
             b"\n", b"\r\n"
         )
         args, files = form_data_args()
         parse_multipart_form_data(b"1234", data, args, files)
         file = files["files"][0]
-        self.assertEqual(file["filename"], u"áb.txt")
+        self.assertEqual(file["filename"], "áb.txt")
         self.assertEqual(file["body"], b"Foo")
 
     def test_boundary_starts_and_ends_with_quotes(self):
         data = b"""\
 --1234
 Content-Disposition: form-data; name="files"; filename="ab.txt"
 
@@ -297,21 +297,21 @@
         # Ensure that only \r\n is recognized as a header separator, and not
         # the other newline-like unicode characters.
         # Characters that are likely to be problematic can be found in
         # http://unicode.org/standard/reports/tr13/tr13-5.html
         # and cpython's unicodeobject.c (which defines the implementation
         # of unicode_type.splitlines(), and uses a different list than TR13).
         newlines = [
-            u"\u001b",  # VERTICAL TAB
-            u"\u001c",  # FILE SEPARATOR
-            u"\u001d",  # GROUP SEPARATOR
-            u"\u001e",  # RECORD SEPARATOR
-            u"\u0085",  # NEXT LINE
-            u"\u2028",  # LINE SEPARATOR
-            u"\u2029",  # PARAGRAPH SEPARATOR
+            "\u001b",  # VERTICAL TAB
+            "\u001c",  # FILE SEPARATOR
+            "\u001d",  # GROUP SEPARATOR
+            "\u001e",  # RECORD SEPARATOR
+            "\u0085",  # NEXT LINE
+            "\u2028",  # LINE SEPARATOR
+            "\u2029",  # PARAGRAPH SEPARATOR
         ]
         for newline in newlines:
             # Try the utf8 and latin1 representations of each newline
             for encoding in ["utf8", "latin1"]:
                 try:
                     try:
                         encoded = newline.encode(encoding)
```

### Comparing `tornado-6.2b2/tornado/test/ioloop_test.py` & `tornado-6.3b1/tornado/test/ioloop_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -446,23 +446,14 @@
         self.io_loop = None  # type: typing.Optional[IOLoop]
         IOLoop.clear_current()
 
     def tearDown(self):
         if self.io_loop is not None:
             self.io_loop.close()
 
-    def test_default_current(self):
-        self.io_loop = IOLoop()
-        # The first IOLoop with default arguments is made current.
-        self.assertIs(self.io_loop, IOLoop.current())
-        # A second IOLoop can be created but is not made current.
-        io_loop2 = IOLoop()
-        self.assertIs(self.io_loop, IOLoop.current())
-        io_loop2.close()
-
     def test_non_current(self):
         self.io_loop = IOLoop(make_current=False)
         # The new IOLoop is not initially made current.
         self.assertIsNone(IOLoop.current(instance=False))
         # Starting the IOLoop makes it current, and stopping the loop
         # makes it non-current. This process is repeatable.
         for i in range(3):
@@ -477,19 +468,14 @@
             self.assertIs(self.current_io_loop, self.io_loop)
             # Now that the loop is stopped, it is no longer current.
             self.assertIsNone(IOLoop.current(instance=False))
 
     def test_force_current(self):
         self.io_loop = IOLoop(make_current=True)
         self.assertIs(self.io_loop, IOLoop.current())
-        with self.assertRaises(RuntimeError):
-            # A second make_current=True construction cannot succeed.
-            IOLoop(make_current=True)
-        # current() was not affected by the failed construction.
-        self.assertIs(self.io_loop, IOLoop.current())
 
 
 class TestIOLoopCurrentAsync(AsyncTestCase):
     def setUp(self):
         super().setUp()
         setup_with_context_manager(self, ignore_deprecation())
```

### Comparing `tornado-6.2b2/tornado/test/iostream_test.py` & `tornado-6.3b1/tornado/test/iostream_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/test/locale_test.py` & `tornado-6.3b1/tornado/test/locale_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     def test_csv(self):
         tornado.locale.load_translations(
             os.path.join(os.path.dirname(__file__), "csv_translations")
         )
         locale = tornado.locale.get("fr_FR")
         self.assertTrue(isinstance(locale, tornado.locale.CSVLocale))
-        self.assertEqual(locale.translate("school"), u"\u00e9cole")
+        self.assertEqual(locale.translate("school"), "\u00e9cole")
 
     def test_csv_bom(self):
         with open(
             os.path.join(os.path.dirname(__file__), "csv_translations", "fr_FR.csv"),
             "rb",
         ) as f:
             char_data = to_unicode(f.read())
@@ -49,43 +49,41 @@
             tmpdir = tempfile.mkdtemp()
             try:
                 with open(os.path.join(tmpdir, "fr_FR.csv"), "wb") as f:
                     f.write(char_data.encode(encoding))
                 tornado.locale.load_translations(tmpdir)
                 locale = tornado.locale.get("fr_FR")
                 self.assertIsInstance(locale, tornado.locale.CSVLocale)
-                self.assertEqual(locale.translate("school"), u"\u00e9cole")
+                self.assertEqual(locale.translate("school"), "\u00e9cole")
             finally:
                 shutil.rmtree(tmpdir)
 
     def test_gettext(self):
         tornado.locale.load_gettext_translations(
             os.path.join(os.path.dirname(__file__), "gettext_translations"),
             "tornado_test",
         )
         locale = tornado.locale.get("fr_FR")
         self.assertTrue(isinstance(locale, tornado.locale.GettextLocale))
-        self.assertEqual(locale.translate("school"), u"\u00e9cole")
-        self.assertEqual(locale.pgettext("law", "right"), u"le droit")
-        self.assertEqual(locale.pgettext("good", "right"), u"le bien")
+        self.assertEqual(locale.translate("school"), "\u00e9cole")
+        self.assertEqual(locale.pgettext("law", "right"), "le droit")
+        self.assertEqual(locale.pgettext("good", "right"), "le bien")
+        self.assertEqual(locale.pgettext("organization", "club", "clubs", 1), "le club")
         self.assertEqual(
-            locale.pgettext("organization", "club", "clubs", 1), u"le club"
+            locale.pgettext("organization", "club", "clubs", 2), "les clubs"
         )
-        self.assertEqual(
-            locale.pgettext("organization", "club", "clubs", 2), u"les clubs"
-        )
-        self.assertEqual(locale.pgettext("stick", "club", "clubs", 1), u"le b\xe2ton")
-        self.assertEqual(locale.pgettext("stick", "club", "clubs", 2), u"les b\xe2tons")
+        self.assertEqual(locale.pgettext("stick", "club", "clubs", 1), "le b\xe2ton")
+        self.assertEqual(locale.pgettext("stick", "club", "clubs", 2), "les b\xe2tons")
 
 
 class LocaleDataTest(unittest.TestCase):
     def test_non_ascii_name(self):
         name = tornado.locale.LOCALE_NAMES["es_LA"]["name"]
         self.assertTrue(isinstance(name, unicode_type))
-        self.assertEqual(name, u"Espa\u00f1ol")
+        self.assertEqual(name, "Espa\u00f1ol")
         self.assertEqual(utf8(name), b"Espa\xc3\xb1ol")
 
 
 class EnglishTest(unittest.TestCase):
     def test_format_date(self):
         locale = tornado.locale.get("en_US")
         date = datetime.datetime(2013, 4, 28, 18, 35)
```

### Comparing `tornado-6.2b2/tornado/test/locks_test.py` & `tornado-6.3b1/tornado/test/locks_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/test/log_test.py` & `tornado-6.3b1/tornado/test/log_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,16 @@
 
     def setUp(self):
         self.formatter = LogFormatter(color=False)
         # Fake color support.  We can't guarantee anything about the $TERM
         # variable when the tests are run, so just patch in some values
         # for testing.  (testing with color off fails to expose some potential
         # encoding issues from the control characters)
-        self.formatter._colors = {logging.ERROR: u"\u0001"}
-        self.formatter._normal = u"\u0002"
+        self.formatter._colors = {logging.ERROR: "\u0001"}
+        self.formatter._normal = "\u0002"
         # construct a Logger directly to bypass getLogger's caching
         self.logger = logging.Logger("LogFormatterTest")
         self.logger.propagate = False
         self.tempdir = tempfile.mkdtemp()
         self.filename = os.path.join(self.tempdir, "log.out")
         self.handler = self.make_handler(self.filename)
         self.handler.setFormatter(self.formatter)
@@ -89,48 +89,48 @@
         with ignore_bytes_warning():
             # This will be "\xe9" on python 2 or "b'\xe9'" on python 3
             self.logger.error(b"\xe9")
             self.assertEqual(self.get_output(), utf8(repr(b"\xe9")))
 
     def test_utf8_logging(self):
         with ignore_bytes_warning():
-            self.logger.error(u"\u00e9".encode("utf8"))
+            self.logger.error("\u00e9".encode("utf8"))
         if issubclass(bytes, basestring_type):
             # on python 2, utf8 byte strings (and by extension ascii byte
             # strings) are passed through as-is.
-            self.assertEqual(self.get_output(), utf8(u"\u00e9"))
+            self.assertEqual(self.get_output(), utf8("\u00e9"))
         else:
             # on python 3, byte strings always get repr'd even if
             # they're ascii-only, so this degenerates into another
             # copy of test_bytes_logging.
-            self.assertEqual(self.get_output(), utf8(repr(utf8(u"\u00e9"))))
+            self.assertEqual(self.get_output(), utf8(repr(utf8("\u00e9"))))
 
     def test_bytes_exception_logging(self):
         try:
             raise Exception(b"\xe9")
         except Exception:
             self.logger.exception("caught exception")
         # This will be "Exception: \xe9" on python 2 or
         # "Exception: b'\xe9'" on python 3.
         output = self.get_output()
-        self.assertRegex(output, br"Exception.*\\xe9")
+        self.assertRegex(output, rb"Exception.*\\xe9")
         # The traceback contains newlines, which should not have been escaped.
-        self.assertNotIn(br"\n", output)
+        self.assertNotIn(rb"\n", output)
 
 
 class UnicodeLogFormatterTest(LogFormatterTest):
     def make_handler(self, filename):
         # Adding an explicit encoding configuration allows non-ascii unicode
         # strings in both python 2 and 3, without changing the behavior
         # for byte strings.
         return logging.FileHandler(filename, encoding="utf8")
 
     def test_unicode_logging(self):
-        self.logger.error(u"\u00e9")
-        self.assertEqual(self.get_output(), utf8(u"\u00e9"))
+        self.logger.error("\u00e9")
+        self.assertEqual(self.get_output(), utf8("\u00e9"))
 
 
 class EnablePrettyLoggingTest(unittest.TestCase):
     def setUp(self):
         super().setUp()
         self.options = OptionParser()
         define_logging_options(self.options)
```

### Comparing `tornado-6.2b2/tornado/test/netutil_test.py` & `tornado-6.3b1/tornado/test/netutil_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,22 @@
 
 class _ResolverTestMixin(object):
     resolver = None  # type: typing.Any
 
     @gen_test
     def test_localhost(self: typing.Any):
         addrinfo = yield self.resolver.resolve("localhost", 80, socket.AF_UNSPEC)
-        self.assertIn((socket.AF_INET, ("127.0.0.1", 80)), addrinfo)
+        # Most of the time localhost resolves to either the ipv4 loopback
+        # address alone, or ipv4+ipv6. But some versions of pycares will only
+        # return the ipv6 version, so we have to check for either one alone.
+        self.assertTrue(
+            ((socket.AF_INET, ("127.0.0.1", 80)) in addrinfo)
+            or ((socket.AF_INET6, ("::1", 80)) in addrinfo),
+            f"loopback address not found in {addrinfo}",
+        )
 
 
 # It is impossible to quickly and consistently generate an error in name
 # resolution, so test this case separately, using mocks as needed.
 class _ResolverErrorTestMixin(object):
     resolver = None  # type: typing.Any
```

### Comparing `tornado-6.2b2/tornado/test/options_test.py` & `tornado-6.3b1/tornado/test/options_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,40 +200,43 @@
         options.define("basestring", type=basestring_type)
         options.define("int", type=int)
         options.define("float", type=float)
         options.define("datetime", type=datetime.datetime)
         options.define("timedelta", type=datetime.timedelta)
         options.define("email", type=Email)
         options.define("list-of-int", type=int, multiple=True)
+        options.define("list-of-str", type=str, multiple=True)
         return options
 
     def _check_options_values(self, options):
         self.assertEqual(options.str, "asdf")
         self.assertEqual(options.basestring, "qwer")
         self.assertEqual(options.int, 42)
         self.assertEqual(options.float, 1.5)
         self.assertEqual(options.datetime, datetime.datetime(2013, 4, 28, 5, 16))
         self.assertEqual(options.timedelta, datetime.timedelta(seconds=45))
         self.assertEqual(options.email.value, "tornado@web.com")
         self.assertTrue(isinstance(options.email, Email))
         self.assertEqual(options.list_of_int, [1, 2, 3])
+        self.assertEqual(options.list_of_str, ["a", "b", "c"])
 
     def test_types(self):
         options = self._define_options()
         options.parse_command_line(
             [
                 "main.py",
                 "--str=asdf",
                 "--basestring=qwer",
                 "--int=42",
                 "--float=1.5",
                 "--datetime=2013-04-28 05:16",
                 "--timedelta=45s",
                 "--email=tornado@web.com",
                 "--list-of-int=1,2,3",
+                "--list-of-str=a,b,c",
             ]
         )
         self._check_options_values(options)
 
     def test_types_with_conf_file(self):
         for config_file_name in (
             "options_test_types.cfg",
```

### Comparing `tornado-6.2b2/tornado/test/process_test.py` & `tornado-6.3b1/tornado/test/process_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/test/queues_test.py` & `tornado-6.3b1/tornado/test/queues_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/test/routing_test.py` & `tornado-6.3b1/tornado/test/routing_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/test/runtests.py` & `tornado-6.3b1/tornado/test/runtests.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/test/simple_httpclient_test.py` & `tornado-6.3b1/tornado/test/simple_httpclient_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/test/static/sample.xml` & `tornado-6.3b1/tornado/test/static/sample.xml`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/test/tcpclient_test.py` & `tornado-6.3b1/tornado/test/tcpclient_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,19 @@
         if socket.AF_INET6 not in families:
             self.skipTest("localhost does not resolve to ipv6")
 
     @gen_test
     def do_test_connect(self, family, host, source_ip=None, source_port=None):
         port = self.start_server(family)
         stream = yield self.client.connect(
-            host, port, source_ip=source_ip, source_port=source_port
+            host,
+            port,
+            source_ip=source_ip,
+            source_port=source_port,
+            af=family,
         )
         assert self.server is not None
         server_stream = yield self.server.queue.get()
         with closing(stream):
             stream.write(b"hello")
             data = yield server_stream.read_bytes(5)
             self.assertEqual(data, b"hello")
```

### Comparing `tornado-6.2b2/tornado/test/tcpserver_test.py` & `tornado-6.3b1/tornado/test/tcpserver_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/test/template_test.py` & `tornado-6.3b1/tornado/test/template_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,24 +74,24 @@
         self.assertEqual(Template("{#!").generate(), b"{#")
         self.assertEqual(
             Template("{{ 'expr' }} {{!jquery expr}}").generate(),
             b"expr {{jquery expr}}",
         )
 
     def test_unicode_template(self):
-        template = Template(utf8(u"\u00e9"))
-        self.assertEqual(template.generate(), utf8(u"\u00e9"))
+        template = Template(utf8("\u00e9"))
+        self.assertEqual(template.generate(), utf8("\u00e9"))
 
     def test_unicode_literal_expression(self):
         # Unicode literals should be usable in templates.  Note that this
         # test simulates unicode characters appearing directly in the
         # template file (with utf8 encoding), i.e. \u escapes would not
         # be used in the template file itself.
-        template = Template(utf8(u'{{ "\u00e9" }}'))
-        self.assertEqual(template.generate(), utf8(u"\u00e9"))
+        template = Template(utf8('{{ "\u00e9" }}'))
+        self.assertEqual(template.generate(), utf8("\u00e9"))
 
     def test_custom_namespace(self):
         loader = DictLoader(
             {"test.html": "{{ inc(5) }}"}, namespace={"inc": lambda x: x + 1}
         )
         self.assertEqual(loader.load("test.html").generate(), b"6")
 
@@ -102,23 +102,23 @@
         template = Template(utf8("{% apply upper %}foo{% end %}"))
         self.assertEqual(template.generate(upper=upper), b"FOO")
 
     def test_unicode_apply(self):
         def upper(s):
             return to_unicode(s).upper()
 
-        template = Template(utf8(u"{% apply upper %}foo \u00e9{% end %}"))
-        self.assertEqual(template.generate(upper=upper), utf8(u"FOO \u00c9"))
+        template = Template(utf8("{% apply upper %}foo \u00e9{% end %}"))
+        self.assertEqual(template.generate(upper=upper), utf8("FOO \u00c9"))
 
     def test_bytes_apply(self):
         def upper(s):
             return utf8(to_unicode(s).upper())
 
-        template = Template(utf8(u"{% apply upper %}foo \u00e9{% end %}"))
-        self.assertEqual(template.generate(upper=upper), utf8(u"FOO \u00c9"))
+        template = Template(utf8("{% apply upper %}foo \u00e9{% end %}"))
+        self.assertEqual(template.generate(upper=upper), utf8("FOO \u00c9"))
 
     def test_if(self):
         template = Template(utf8("{% if x > 4 %}yes{% else %}no{% end %}"))
         self.assertEqual(template.generate(x=5), b"yes")
         self.assertEqual(template.generate(x=3), b"no")
 
     def test_if_empty_body(self):
@@ -190,16 +190,16 @@
         # This file has from __future__ import division...
         self.assertEqual(1 / 2, 0.5)
         # ...but the template doesn't
         template = Template("{{ 1 / 2 }}")
         self.assertEqual(template.generate(), "0")
 
     def test_non_ascii_name(self):
-        loader = DictLoader({u"t\u00e9st.html": "hello"})
-        self.assertEqual(loader.load(u"t\u00e9st.html").generate(), b"hello")
+        loader = DictLoader({"t\u00e9st.html": "hello"})
+        self.assertEqual(loader.load("t\u00e9st.html").generate(), b"hello")
 
 
 class StackTraceTest(unittest.TestCase):
     def test_error_line_number_expression(self):
         loader = DictLoader(
             {
                 "test.html": """one
@@ -529,8 +529,8 @@
 class TemplateLoaderTest(unittest.TestCase):
     def setUp(self):
         self.loader = Loader(os.path.join(os.path.dirname(__file__), "templates"))
 
     def test_utf8_in_file(self):
         tmpl = self.loader.load("utf8.html")
         result = tmpl.generate()
-        self.assertEqual(to_unicode(result).strip(), u"H\u00e9llo")
+        self.assertEqual(to_unicode(result).strip(), "H\u00e9llo")
```

### Comparing `tornado-6.2b2/tornado/test/test.crt` & `tornado-6.3b1/tornado/test/test.crt`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/test/test.key` & `tornado-6.3b1/tornado/test/test.key`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/test/testing_test.py` & `tornado-6.3b1/tornado/test/testing_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from tornado import gen, ioloop
 from tornado.httpserver import HTTPServer
 from tornado.locks import Event
-from tornado.test.util import ignore_deprecation
 from tornado.testing import AsyncHTTPTestCase, AsyncTestCase, bind_unused_port, gen_test
 from tornado.web import Application
 import asyncio
 import contextlib
 import inspect
 import gc
 import os
 import platform
+import sys
 import traceback
 import unittest
 import warnings
 
 
 @contextlib.contextmanager
 def set_environ(name, value):
@@ -104,15 +104,15 @@
         path = "/path"
         response = self.fetch(path)
         self.assertEqual(response.request.url, self.get_url(path))
 
     def test_fetch_full_http_url(self):
         # Ensure that self.fetch() recognizes absolute urls and does
         # not transform them into references to our main test server.
-        path = "http://localhost:%d/path" % self.second_port
+        path = "http://127.0.0.1:%d/path" % self.second_port
 
         response = self.fetch(path)
         self.assertEqual(response.request.url, path)
 
     def tearDown(self):
         self.second_server.stop()
         super().tearDown()
@@ -130,14 +130,17 @@
         self.assertEqual(len(result.errors), 1)
         self.assertIn("should be decorated", result.errors[0][1])
 
     @unittest.skipIf(
         platform.python_implementation() == "PyPy",
         "pypy destructor warnings cannot be silenced",
     )
+    @unittest.skipIf(
+        sys.version_info >= (3, 12), "py312 has its own check for test case returns"
+    )
     def test_undecorated_coroutine(self):
         class Test(AsyncTestCase):
             async def test_coro(self):
                 pass
 
         test = Test("test_coro")
         result = unittest.TestResult()
@@ -334,37 +337,9 @@
         try:
             test(self)
             self.fail("did not get expected exception")
         except ioloop.TimeoutError:
             self.finished = True
 
 
-class GetNewIOLoopTest(AsyncTestCase):
-    def get_new_ioloop(self):
-        # Use the current loop instead of creating a new one here.
-        return ioloop.IOLoop.current()
-
-    def setUp(self):
-        # This simulates the effect of an asyncio test harness like
-        # pytest-asyncio.
-        with ignore_deprecation():
-            try:
-                self.orig_loop = asyncio.get_event_loop()
-            except RuntimeError:
-                self.orig_loop = None  # type: ignore[assignment]
-        self.new_loop = asyncio.new_event_loop()
-        asyncio.set_event_loop(self.new_loop)
-        super().setUp()
-
-    def tearDown(self):
-        super().tearDown()
-        # AsyncTestCase must not affect the existing asyncio loop.
-        self.assertFalse(asyncio.get_event_loop().is_closed())
-        asyncio.set_event_loop(self.orig_loop)
-        self.new_loop.close()
-
-    def test_loop(self):
-        self.assertIs(self.io_loop.asyncio_loop, self.new_loop)  # type: ignore
-
-
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `tornado-6.2b2/tornado/test/twisted_test.py` & `tornado-6.3b1/tornado/test/twisted_test.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/test/util.py` & `tornado-6.3b1/tornado/test/util.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/test/util_test.py` & `tornado-6.3b1/tornado/test/util_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from io import StringIO
 import re
 import sys
 import datetime
 import unittest
 
-import tornado.escape
+import tornado
 from tornado.escape import utf8
 from tornado.util import (
     raise_exc_info,
     Configurable,
     exec_in,
     ArgReplacer,
     timedelta_to_seconds,
@@ -210,15 +210,15 @@
 
         obj = TestConfig3()
         self.assertIsInstance(obj, TestConfig3B)
 
 
 class UnicodeLiteralTest(unittest.TestCase):
     def test_unicode_escapes(self):
-        self.assertEqual(utf8(u"\u00e9"), b"\xc3\xa9")
+        self.assertEqual(utf8("\u00e9"), b"\xc3\xa9")
 
 
 class ExecInTest(unittest.TestCase):
     # TODO(bdarnell): make a version of this test for one of the new
     # future imports available in python 3.
     @unittest.skip("no testable future imports")
     def test_no_inherit_future(self):
@@ -272,24 +272,24 @@
 
 
 class ImportObjectTest(unittest.TestCase):
     def test_import_member(self):
         self.assertIs(import_object("tornado.escape.utf8"), utf8)
 
     def test_import_member_unicode(self):
-        self.assertIs(import_object(u"tornado.escape.utf8"), utf8)
+        self.assertIs(import_object("tornado.escape.utf8"), utf8)
 
     def test_import_module(self):
         self.assertIs(import_object("tornado.escape"), tornado.escape)
 
     def test_import_module_unicode(self):
         # The internal implementation of __import__ differs depending on
         # whether the thing being imported is a module or not.
         # This variant requires a byte string in python 2.
-        self.assertIs(import_object(u"tornado.escape"), tornado.escape)
+        self.assertIs(import_object("tornado.escape"), tornado.escape)
 
 
 class ReUnescapeTest(unittest.TestCase):
     def test_re_unescape(self):
         test_strings = ("/favicon.ico", "index.html", "Hello, World!", "!$@#%;")
         for string in test_strings:
             self.assertEqual(string, re_unescape(re.escape(string)))
```

### Comparing `tornado-6.2b2/tornado/test/web_test.py` & `tornado-6.3b1/tornado/test/web_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
 class HelloHandler(RequestHandler):
     def get(self):
         self.write("hello")
 
 
 class CookieTestRequestHandler(RequestHandler):
-    # stub out enough methods to make the secure_cookie functions work
+    # stub out enough methods to make the signed_cookie functions work
     def __init__(self, cookie_secret="0123456789", key_version=None):
         # don't call super.__init__
         self._cookies = {}  # type: typing.Dict[str, bytes]
         if key_version is None:
             self.application = ObjectDict(  # type: ignore
                 settings=dict(cookie_secret=cookie_secret)
             )
@@ -117,23 +117,23 @@
         self._cookies[name] = value
 
 
 # See SignedValueTest below for more.
 class SecureCookieV1Test(unittest.TestCase):
     def test_round_trip(self):
         handler = CookieTestRequestHandler()
-        handler.set_secure_cookie("foo", b"bar", version=1)
-        self.assertEqual(handler.get_secure_cookie("foo", min_version=1), b"bar")
+        handler.set_signed_cookie("foo", b"bar", version=1)
+        self.assertEqual(handler.get_signed_cookie("foo", min_version=1), b"bar")
 
     def test_cookie_tampering_future_timestamp(self):
         handler = CookieTestRequestHandler()
         # this string base64-encodes to '12345678'
-        handler.set_secure_cookie("foo", binascii.a2b_hex(b"d76df8e7aefc"), version=1)
+        handler.set_signed_cookie("foo", binascii.a2b_hex(b"d76df8e7aefc"), version=1)
         cookie = handler._cookies["foo"]
-        match = re.match(br"12345678\|([0-9]+)\|([0-9a-f]+)", cookie)
+        match = re.match(rb"12345678\|([0-9]+)\|([0-9a-f]+)", cookie)
         assert match is not None
         timestamp = match.group(1)
         sig = match.group(2)
         self.assertEqual(
             _create_signature_v1(
                 handler.application.settings["cookie_secret"],
                 "foo",
@@ -156,70 +156,70 @@
         )
         # tamper with the cookie
         handler._cookies["foo"] = utf8(
             "1234|5678%s|%s" % (to_basestring(timestamp), to_basestring(sig))
         )
         # it gets rejected
         with ExpectLog(gen_log, "Cookie timestamp in future"):
-            self.assertTrue(handler.get_secure_cookie("foo", min_version=1) is None)
+            self.assertTrue(handler.get_signed_cookie("foo", min_version=1) is None)
 
     def test_arbitrary_bytes(self):
         # Secure cookies accept arbitrary data (which is base64 encoded).
         # Note that normal cookies accept only a subset of ascii.
         handler = CookieTestRequestHandler()
-        handler.set_secure_cookie("foo", b"\xe9", version=1)
-        self.assertEqual(handler.get_secure_cookie("foo", min_version=1), b"\xe9")
+        handler.set_signed_cookie("foo", b"\xe9", version=1)
+        self.assertEqual(handler.get_signed_cookie("foo", min_version=1), b"\xe9")
 
 
 # See SignedValueTest below for more.
 class SecureCookieV2Test(unittest.TestCase):
     KEY_VERSIONS = {0: "ajklasdf0ojaisdf", 1: "aslkjasaolwkjsdf"}
 
     def test_round_trip(self):
         handler = CookieTestRequestHandler()
-        handler.set_secure_cookie("foo", b"bar", version=2)
-        self.assertEqual(handler.get_secure_cookie("foo", min_version=2), b"bar")
+        handler.set_signed_cookie("foo", b"bar", version=2)
+        self.assertEqual(handler.get_signed_cookie("foo", min_version=2), b"bar")
 
     def test_key_version_roundtrip(self):
         handler = CookieTestRequestHandler(
             cookie_secret=self.KEY_VERSIONS, key_version=0
         )
-        handler.set_secure_cookie("foo", b"bar")
-        self.assertEqual(handler.get_secure_cookie("foo"), b"bar")
+        handler.set_signed_cookie("foo", b"bar")
+        self.assertEqual(handler.get_signed_cookie("foo"), b"bar")
 
     def test_key_version_roundtrip_differing_version(self):
         handler = CookieTestRequestHandler(
             cookie_secret=self.KEY_VERSIONS, key_version=1
         )
-        handler.set_secure_cookie("foo", b"bar")
-        self.assertEqual(handler.get_secure_cookie("foo"), b"bar")
+        handler.set_signed_cookie("foo", b"bar")
+        self.assertEqual(handler.get_signed_cookie("foo"), b"bar")
 
     def test_key_version_increment_version(self):
         handler = CookieTestRequestHandler(
             cookie_secret=self.KEY_VERSIONS, key_version=0
         )
-        handler.set_secure_cookie("foo", b"bar")
+        handler.set_signed_cookie("foo", b"bar")
         new_handler = CookieTestRequestHandler(
             cookie_secret=self.KEY_VERSIONS, key_version=1
         )
         new_handler._cookies = handler._cookies
-        self.assertEqual(new_handler.get_secure_cookie("foo"), b"bar")
+        self.assertEqual(new_handler.get_signed_cookie("foo"), b"bar")
 
     def test_key_version_invalidate_version(self):
         handler = CookieTestRequestHandler(
             cookie_secret=self.KEY_VERSIONS, key_version=0
         )
-        handler.set_secure_cookie("foo", b"bar")
+        handler.set_signed_cookie("foo", b"bar")
         new_key_versions = self.KEY_VERSIONS.copy()
         new_key_versions.pop(0)
         new_handler = CookieTestRequestHandler(
             cookie_secret=new_key_versions, key_version=1
         )
         new_handler._cookies = handler._cookies
-        self.assertEqual(new_handler.get_secure_cookie("foo"), None)
+        self.assertEqual(new_handler.get_signed_cookie("foo"), None)
 
 
 class FinalReturnTest(WebTestCase):
     final_return = None  # type: Future
 
     def get_handlers(self):
         test = self
@@ -270,28 +270,28 @@
 class CookieTest(WebTestCase):
     def get_handlers(self):
         class SetCookieHandler(RequestHandler):
             def get(self):
                 # Try setting cookies with different argument types
                 # to ensure that everything gets encoded correctly
                 self.set_cookie("str", "asdf")
-                self.set_cookie("unicode", u"qwer")
+                self.set_cookie("unicode", "qwer")
                 self.set_cookie("bytes", b"zxcv")
 
         class GetCookieHandler(RequestHandler):
             def get(self):
                 cookie = self.get_cookie("foo", "default")
                 assert cookie is not None
                 self.write(cookie)
 
         class SetCookieDomainHandler(RequestHandler):
             def get(self):
                 # unicode domain and path arguments shouldn't break things
                 # either (see bug #285)
-                self.set_cookie("unicode_args", "blah", domain=u"foo.com", path=u"/foo")
+                self.set_cookie("unicode_args", "blah", domain="foo.com", path="/foo")
 
         class SetCookieSpecialCharHandler(RequestHandler):
             def get(self):
                 self.set_cookie("equals", "a=b")
                 self.set_cookie("semicolon", "a;b")
                 self.set_cookie("quote", 'a"b')
 
@@ -538,17 +538,17 @@
         )
 
     def test_group_encoding(self):
         # Path components and query arguments should be decoded the same way
         self.assertEqual(
             self.fetch_json("/group/%C3%A9?arg=%C3%A9"),
             {
-                u"path": u"/group/%C3%A9",
-                u"path_args": [u"\u00e9"],
-                u"args": {u"arg": [u"\u00e9"]},
+                "path": "/group/%C3%A9",
+                "path_args": ["\u00e9"],
+                "args": {"arg": ["\u00e9"]},
             },
         )
 
     def test_slashes(self):
         # Slashes may be escaped to appear as a single "directory" in the path,
         # but they are then unescaped when passed to the get() method.
         self.assertEqual(
@@ -581,15 +581,15 @@
 
         # Secure cookies return bytes because they can contain arbitrary
         # data, but regular cookies are native strings.
         if list(self.cookies.keys()) != ["asdf"]:
             raise Exception(
                 "unexpected values for cookie keys: %r" % self.cookies.keys()
             )
-        self.check_type("get_secure_cookie", self.get_secure_cookie("asdf"), bytes)
+        self.check_type("get_signed_cookie", self.get_signed_cookie("asdf"), bytes)
         self.check_type("get_cookie", self.get_cookie("asdf"), str)
 
         self.check_type("xsrf_token", self.xsrf_token, bytes)
         self.check_type("xsrf_form_html", self.xsrf_form_html(), str)
 
         self.check_type("reverse_url", self.reverse_url("typecheck", "foo"), str)
 
@@ -809,23 +809,21 @@
         ]
         for req_url in urls:
             response = self.fetch(req_url)
             response.rethrow()
             data = json_decode(response.body)
             self.assertEqual(
                 data,
-                {u"path": [u"unicode", u"\u00e9"], u"query": [u"unicode", u"\u00e9"]},
+                {"path": ["unicode", "\u00e9"], "query": ["unicode", "\u00e9"]},
             )
 
         response = self.fetch("/decode_arg/%C3%A9?foo=%C3%A9")
         response.rethrow()
         data = json_decode(response.body)
-        self.assertEqual(
-            data, {u"path": [u"bytes", u"c3a9"], u"query": [u"bytes", u"c3a9"]}
-        )
+        self.assertEqual(data, {"path": ["bytes", "c3a9"], "query": ["bytes", "c3a9"]})
 
     def test_decode_argument_invalid_unicode(self):
         # test that invalid unicode in URLs causes 400, not 500
         with ExpectLog(gen_log, ".*Invalid unicode.*"):
             response = self.fetch("/typecheck/invalid%FF")
             self.assertEqual(response.code, 400)
             response = self.fetch("/typecheck/invalid?foo=%FF")
@@ -839,23 +837,23 @@
         ]
         for req_url in urls:
             response = self.fetch(req_url)
             response.rethrow()
             data = json_decode(response.body)
             self.assertEqual(
                 data,
-                {u"path": [u"unicode", u"1 + 1"], u"query": [u"unicode", u"1 + 1"]},
+                {"path": ["unicode", "1 + 1"], "query": ["unicode", "1 + 1"]},
             )
 
     def test_reverse_url(self):
         self.assertEqual(self.app.reverse_url("decode_arg", "foo"), "/decode_arg/foo")
         self.assertEqual(self.app.reverse_url("decode_arg", 42), "/decode_arg/42")
         self.assertEqual(self.app.reverse_url("decode_arg", b"\xe9"), "/decode_arg/%E9")
         self.assertEqual(
-            self.app.reverse_url("decode_arg", u"\u00e9"), "/decode_arg/%C3%A9"
+            self.app.reverse_url("decode_arg", "\u00e9"), "/decode_arg/%C3%A9"
         )
         self.assertEqual(
             self.app.reverse_url("decode_arg", "1 + 1"), "/decode_arg/1%20%2B%201"
         )
 
     def test_uimodule_unescaped(self):
         response = self.fetch("/linkify")
@@ -888,16 +886,16 @@
 //]]>
 </script>
 <script src="/analytics.js"/>
 </body></html>""",  # noqa: E501
         )
 
     def test_optional_path(self):
-        self.assertEqual(self.fetch_json("/optional_path/foo"), {u"path": u"foo"})
-        self.assertEqual(self.fetch_json("/optional_path/"), {u"path": None})
+        self.assertEqual(self.fetch_json("/optional_path/foo"), {"path": "foo"})
+        self.assertEqual(self.fetch_json("/optional_path/"), {"path": None})
 
     def test_multi_header(self):
         response = self.fetch("/multi_header")
         self.assertEqual(response.headers["x-overwrite"], "2")
         self.assertEqual(response.headers.get_list("x-multi"), ["3", "4"])
 
     def test_redirect(self):
@@ -1588,15 +1586,15 @@
     def get_handlers(self):
         class EchoHandler(RequestHandler):
             def get(self, path):
                 self.write(path)
 
         return [
             ("/str/(?P<path>.*)", EchoHandler),
-            (u"/unicode/(?P<path>.*)", EchoHandler),
+            ("/unicode/(?P<path>.*)", EchoHandler),
         ]
 
     def test_named_urlspec_groups(self):
         response = self.fetch("/str/foo")
         self.assertEqual(response.body, b"foo")
 
         response = self.fetch("/unicode/bar")
@@ -2917,14 +2915,73 @@
                 method="POST",
                 body=urllib.parse.urlencode(dict(_xsrf=body_token)),
                 headers=self.cookie_headers(cookie_token),
             )
             self.assertEqual(response.code, 200)
 
 
+# A subset of the previous test with a different cookie name
+class XSRFCookieNameTest(SimpleHandlerTestCase):
+    class Handler(RequestHandler):
+        def get(self):
+            self.write(self.xsrf_token)
+
+        def post(self):
+            self.write("ok")
+
+    def get_app_kwargs(self):
+        return dict(
+            xsrf_cookies=True,
+            xsrf_cookie_name="__Host-xsrf",
+            xsrf_cookie_kwargs={"secure": True},
+        )
+
+    def setUp(self):
+        super().setUp()
+        self.xsrf_token = self.get_token()
+
+    def get_token(self, old_token=None):
+        if old_token is not None:
+            headers = self.cookie_headers(old_token)
+        else:
+            headers = None
+        response = self.fetch("/", headers=headers)
+        response.rethrow()
+        return native_str(response.body)
+
+    def cookie_headers(self, token=None):
+        if token is None:
+            token = self.xsrf_token
+        return {"Cookie": "__Host-xsrf=" + token}
+
+    def test_xsrf_fail_no_token(self):
+        with ExpectLog(gen_log, ".*'_xsrf' argument missing"):
+            response = self.fetch("/", method="POST", body=b"")
+        self.assertEqual(response.code, 403)
+
+    def test_xsrf_fail_body_no_cookie(self):
+        with ExpectLog(gen_log, ".*XSRF cookie does not match POST"):
+            response = self.fetch(
+                "/",
+                method="POST",
+                body=urllib.parse.urlencode(dict(_xsrf=self.xsrf_token)),
+            )
+        self.assertEqual(response.code, 403)
+
+    def test_xsrf_success_post_body(self):
+        response = self.fetch(
+            "/",
+            method="POST",
+            # Note that renaming the cookie doesn't rename the POST param
+            body=urllib.parse.urlencode(dict(_xsrf=self.xsrf_token)),
+            headers=self.cookie_headers(),
+        )
+        self.assertEqual(response.code, 200)
+
+
 class XSRFCookieKwargsTest(SimpleHandlerTestCase):
     class Handler(RequestHandler):
         def get(self):
             self.write(self.xsrf_token)
 
     def get_app_kwargs(self):
         return dict(
```

### Comparing `tornado-6.2b2/tornado/test/websocket_test.py` & `tornado-6.3b1/tornado/test/websocket_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import asyncio
 import functools
+import socket
 import traceback
 import typing
 import unittest
 
 from tornado.concurrent import Future
 from tornado import gen
 from tornado.httpclient import HTTPError, HTTPRequest
 from tornado.locks import Event
 from tornado.log import gen_log, app_log
+from tornado.netutil import Resolver
 from tornado.simple_httpclient import SimpleAsyncHTTPClient
 from tornado.template import DictLoader
 from tornado.testing import AsyncHTTPTestCase, gen_test, bind_unused_port, ExpectLog
 from tornado.web import Application, RequestHandler
 
 try:
     import tornado.websocket  # noqa: F401
@@ -337,24 +339,24 @@
         ws.write_message(b"hello \xe9", binary=True)
         response = yield ws.read_message()
         self.assertEqual(response, b"hello \xe9")
 
     @gen_test
     def test_unicode_message(self):
         ws = yield self.ws_connect("/echo")
-        ws.write_message(u"hello \u00e9")
+        ws.write_message("hello \u00e9")
         response = yield ws.read_message()
-        self.assertEqual(response, u"hello \u00e9")
+        self.assertEqual(response, "hello \u00e9")
 
     @gen_test
     def test_error_in_closed_client_write_message(self):
         ws = yield self.ws_connect("/echo")
         ws.close()
         with self.assertRaises(WebSocketClosedError):
-            ws.write_message(u"hello \u00e9")
+            ws.write_message("hello \u00e9")
 
     @gen_test
     def test_render_message(self):
         ws = yield self.ws_connect("/render")
         ws.write_message("hello")
         response = yield ws.read_message()
         self.assertEqual(response, "<b>hello</b>")
@@ -384,15 +386,15 @@
             yield self.ws_connect("/redirect")
 
     @gen_test
     def test_websocket_network_fail(self):
         sock, port = bind_unused_port()
         sock.close()
         with self.assertRaises(IOError):
-            with ExpectLog(gen_log, ".*"):
+            with ExpectLog(gen_log, ".*", required=False):
                 yield websocket_connect(
                     "ws://127.0.0.1:%d/" % port, connect_timeout=3600
                 )
 
     @gen_test
     def test_websocket_close_buffered_data(self):
         ws = yield websocket_connect("ws://127.0.0.1:%d/echo" % self.get_http_port())
@@ -535,14 +537,23 @@
 
         self.assertEqual(cm.exception.code, 403)
 
     @gen_test
     def test_check_origin_invalid_subdomains(self):
         port = self.get_http_port()
 
+        # CaresResolver may return ipv6-only results for localhost, but our
+        # server is only running on ipv4. Test for this edge case and skip
+        # the test if it happens.
+        addrinfo = yield Resolver().resolve("localhost", port)
+        families = set(addr[0] for addr in addrinfo)
+        if socket.AF_INET not in families:
+            self.skipTest("localhost does not resolve to ipv4")
+            return
+
         url = "ws://localhost:%d/echo" % port
         # Subdomains should be disallowed by default.  If we could pass a
         # resolver to websocket_connect we could test sibling domains as well.
         headers = {"Origin": "http://subtenant.localhost"}
 
         with self.assertRaises(HTTPError) as cm:
             yield websocket_connect(HTTPRequest(url, headers=headers))
```

### Comparing `tornado-6.2b2/tornado/testing.py` & `tornado-6.3b1/tornado/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,15 +131,16 @@
     This class also provides the (deprecated) `stop()` and `wait()`
     methods for a more manual style of testing. The test method itself
     must call ``self.wait()``, and asynchronous callbacks should call
     ``self.stop()`` to signal completion.
 
     By default, a new `.IOLoop` is constructed for each test and is available
     as ``self.io_loop``.  If the code being tested requires a
-    global `.IOLoop`, subclasses should override `get_new_ioloop` to return it.
+    reused global `.IOLoop`, subclasses should override `get_new_ioloop` to return it,
+    although this is deprecated as of Tornado 6.3.
 
     The `.IOLoop`'s ``start`` and ``stop`` methods should not be
     called directly.  Instead, use `self.stop <stop>` and `self.wait
     <wait>`.  Arguments passed to ``self.stop`` are returned from
     ``self.wait``.  It is possible to have multiple ``wait``/``stop``
     cycles in the same test.
 
@@ -158,25 +159,14 @@
         class MyTestCase2(AsyncTestCase):
             def test_http_fetch(self):
                 client = AsyncHTTPClient()
                 client.fetch("http://www.tornadoweb.org/", self.stop)
                 response = self.wait()
                 # Test contents of response
                 self.assertIn("FriendFeed", response.body)
-
-    .. deprecated:: 6.2
-
-       AsyncTestCase and AsyncHTTPTestCase are deprecated due to changes
-       in future versions of Python (after 3.10). The interfaces used
-       in this class are incompatible with the deprecation and intended
-       removal of certain methods related to the idea of a "current"
-       event loop while no event loop is actually running. Use
-       `unittest.IsolatedAsyncioTestCase` instead. Note that this class
-       does not emit DeprecationWarnings until better migration guidance
-       can be provided.
     """
 
     def __init__(self, methodName: str = "runTest") -> None:
         super().__init__(methodName)
         self.__stopped = False
         self.__running = False
         self.__failure = None  # type: Optional[_ExcInfoTuple]
@@ -189,57 +179,30 @@
         # make sure it's not an undecorated generator.
         setattr(self, methodName, _TestMethodWrapper(getattr(self, methodName)))
 
         # Not used in this class itself, but used by @gen_test
         self._test_generator = None  # type: Optional[Union[Generator, Coroutine]]
 
     def setUp(self) -> None:
-        setup_with_context_manager(self, warnings.catch_warnings())
-        warnings.filterwarnings(
-            "ignore",
-            message="There is no current event loop",
-            category=DeprecationWarning,
-            module=r"tornado\..*",
-        )
+        py_ver = sys.version_info
+        if ((3, 10, 0) <= py_ver < (3, 10, 9)) or ((3, 11, 0) <= py_ver <= (3, 11, 1)):
+            # Early releases in the Python 3.10 and 3.1 series had deprecation
+            # warnings that were later reverted; we must suppress them here.
+            setup_with_context_manager(self, warnings.catch_warnings())
+            warnings.filterwarnings(
+                "ignore",
+                message="There is no current event loop",
+                category=DeprecationWarning,
+                module=r"tornado\..*",
+            )
         super().setUp()
-        # NOTE: this code attempts to navigate deprecation warnings introduced
-        # in Python 3.10. The idea of an implicit current event loop is
-        # deprecated in that version, with the intention that tests like this
-        # explicitly create a new event loop and run on it. However, other
-        # packages such as pytest-asyncio (as of version 0.16.0) still rely on
-        # the implicit current event loop and we want to be compatible with them
-        # (even when run on 3.10, but not, of course, on the future version of
-        # python that removes the get/set_event_loop methods completely).
-        #
-        # Deprecation warnings were introduced inconsistently:
-        # asyncio.get_event_loop warns, but
-        # asyncio.get_event_loop_policy().get_event_loop does not. Similarly,
-        # none of the set_event_loop methods warn, although comments on
-        # https://bugs.python.org/issue39529 indicate that they are also
-        # intended for future removal.
-        #
-        # Therefore, we first attempt to access the event loop with the
-        # (non-warning) policy method, and if it fails, fall back to creating a
-        # new event loop. We do not have effective test coverage of the
-        # new event loop case; this will have to be watched when/if
-        # get_event_loop is actually removed.
-        self.should_close_asyncio_loop = False
-        try:
-            self.asyncio_loop = asyncio.get_event_loop_policy().get_event_loop()
-        except Exception:
-            self.asyncio_loop = asyncio.new_event_loop()
-            self.should_close_asyncio_loop = True
-
-        async def get_loop() -> IOLoop:
-            return self.get_new_ioloop()
-
-        self.io_loop = self.asyncio_loop.run_until_complete(get_loop())
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore", DeprecationWarning)
-            self.io_loop.make_current()
+        if type(self).get_new_ioloop is not AsyncTestCase.get_new_ioloop:
+            warnings.warn("get_new_ioloop is deprecated", DeprecationWarning)
+        self.io_loop = self.get_new_ioloop()
+        asyncio.set_event_loop(self.io_loop.asyncio_loop)  # type: ignore[attr-defined]
 
     def tearDown(self) -> None:
         # Native coroutines tend to produce warnings if they're not
         # allowed to run to completion. It's difficult to ensure that
         # this always happens in tests, so cancel any tasks that are
         # still pending by the time we get here.
         asyncio_loop = self.io_loop.asyncio_loop  # type: ignore
@@ -266,25 +229,21 @@
                 try:
                     f.result()
                 except asyncio.CancelledError:
                     pass
 
         # Clean up Subprocess, so it can be used again with a new ioloop.
         Subprocess.uninitialize()
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore", DeprecationWarning)
-            self.io_loop.clear_current()
+        asyncio.set_event_loop(None)
         if not isinstance(self.io_loop, _NON_OWNED_IOLOOPS):
             # Try to clean up any file descriptors left open in the ioloop.
             # This avoids leaks, especially when tests are run repeatedly
             # in the same process with autoreload (because curl does not
             # set FD_CLOEXEC on its file descriptors)
             self.io_loop.close(all_fds=True)
-        if self.should_close_asyncio_loop:
-            self.asyncio_loop.close()
         super().tearDown()
         # In case an exception escaped or the StackContext caught an exception
         # when there wasn't a wait() to re-raise it, do so here.
         # This is our last chance to raise an exception in a way that the
         # unittest machinery understands.
         self.__rethrow()
 
@@ -294,14 +253,17 @@
         By default, a new `.IOLoop` is created for each test.
         Subclasses may override this method to return
         `.IOLoop.current()` if it is not appropriate to use a new
         `.IOLoop` in each tests (for example, if there are global
         singletons using the default `.IOLoop`) or if a per-test event
         loop is being provided by another system (such as
         ``pytest-asyncio``).
+
+        .. deprecated:: 6.3
+           This method will be removed in Tornado 7.0.
         """
         return IOLoop(make_current=False)
 
     def _handle_exception(
         self, typ: Type[Exception], value: Exception, tb: TracebackType
     ) -> bool:
         if self.__failure is None:
@@ -431,18 +393,14 @@
         self.http_client.fetch(self.get_url('/'), self.stop)
         response = self.wait()
 
     which illustrates how AsyncTestCase can turn an asynchronous operation,
     like ``http_client.fetch()``, into a synchronous operation. If you need
     to do other asynchronous operations in tests, you'll probably need to use
     ``stop()`` and ``wait()`` yourself.
-
-    .. deprecated:: 6.2
-       `AsyncTestCase` and `AsyncHTTPTestCase` are deprecated due to changes
-       in Python 3.10; see comments on `AsyncTestCase` for more details.
     """
 
     def setUp(self) -> None:
         super().setUp()
         sock, port = bind_unused_port()
         self.__port = port
 
@@ -668,15 +626,15 @@
                 # exception back into it so the stack trace is replaced by the
                 # point where the test is stopped. The only reason the generator
                 # would not be running would be if it were cancelled, which means
                 # a native coroutine, so we can rely on the cr_running attribute.
                 if self._test_generator is not None and getattr(
                     self._test_generator, "cr_running", True
                 ):
-                    self._test_generator.throw(type(e), e)
+                    self._test_generator.throw(e)
                     # In case the test contains an overly broad except
                     # clause, we may get back here.
                 # Coroutine was stopped or didn't raise a useful stack trace,
                 # so re-raise the original exception which is better than nothing.
                 raise
 
         return post_coroutine
@@ -720,52 +678,68 @@
         logger: Union[logging.Logger, basestring_type],
         regex: str,
         required: bool = True,
         level: Optional[int] = None,
     ) -> None:
         """Constructs an ExpectLog context manager.
 
-        :param logger: Logger object (or name of logger) to watch.  Pass
-            an empty string to watch the root logger.
-        :param regex: Regular expression to match.  Any log entries on
-            the specified logger that match this regex will be suppressed.
-        :param required: If true, an exception will be raised if the end of
-            the ``with`` statement is reached without matching any log entries.
+        :param logger: Logger object (or name of logger) to watch.  Pass an
+            empty string to watch the root logger.
+        :param regex: Regular expression to match.  Any log entries on the
+            specified logger that match this regex will be suppressed.
+        :param required: If true, an exception will be raised if the end of the
+            ``with`` statement is reached without matching any log entries.
         :param level: A constant from the ``logging`` module indicating the
             expected log level. If this parameter is provided, only log messages
             at this level will be considered to match. Additionally, the
-            supplied ``logger`` will have its level adjusted if necessary
-            (for the duration of the ``ExpectLog`` to enable the expected
-            message.
+            supplied ``logger`` will have its level adjusted if necessary (for
+            the duration of the ``ExpectLog`` to enable the expected message.
 
         .. versionchanged:: 6.1
            Added the ``level`` parameter.
+
+        .. deprecated:: 6.3
+           In Tornado 7.0, only ``WARNING`` and higher logging levels will be
+           matched by default. To match ``INFO`` and lower levels, the ``level``
+           argument must be used. This is changing to minimize differences
+           between ``tornado.testing.main`` (which enables ``INFO`` logs by
+           default) and most other test runners (including those in IDEs)
+           which have ``INFO`` logs disabled by default.
         """
         if isinstance(logger, basestring_type):
             logger = logging.getLogger(logger)
         self.logger = logger
         self.regex = re.compile(regex)
         self.required = required
-        self.matched = False
+        # matched and deprecated_level_matched are a counter for the respective event.
+        self.matched = 0
+        self.deprecated_level_matched = 0
         self.logged_stack = False
         self.level = level
         self.orig_level = None  # type: Optional[int]
 
     def filter(self, record: logging.LogRecord) -> bool:
         if record.exc_info:
             self.logged_stack = True
         message = record.getMessage()
         if self.regex.match(message):
+            if self.level is None and record.levelno < logging.WARNING:
+                # We're inside the logging machinery here so generating a DeprecationWarning
+                # here won't be reported cleanly (if warnings-as-errors is enabled, the error
+                # just gets swallowed by the logging module), and even if it were it would
+                # have the wrong stack trace. Just remember this fact and report it in
+                # __exit__ instead.
+                self.deprecated_level_matched += 1
             if self.level is not None and record.levelno != self.level:
                 app_log.warning(
                     "Got expected log message %r at unexpected level (%s vs %s)"
                     % (message, logging.getLevelName(self.level), record.levelname)
                 )
                 return True
-            self.matched = True
+            self.matched += 1
             return False
         return True
 
     def __enter__(self) -> "ExpectLog":
         if self.level is not None and self.level < self.logger.getEffectiveLevel():
             self.orig_level = self.logger.level
             self.logger.setLevel(self.level)
@@ -779,14 +753,23 @@
         tb: Optional[TracebackType],
     ) -> None:
         if self.orig_level is not None:
             self.logger.setLevel(self.orig_level)
         self.logger.removeFilter(self)
         if not typ and self.required and not self.matched:
             raise Exception("did not get expected log message")
+        if (
+            not typ
+            and self.required
+            and (self.deprecated_level_matched >= self.matched)
+        ):
+            warnings.warn(
+                "ExpectLog matched at INFO or below without level argument",
+                DeprecationWarning,
+            )
 
 
 # From https://nedbatchelder.com/blog/201508/using_context_managers_in_test_setup.html
 def setup_with_context_manager(testcase: unittest.TestCase, cm: Any) -> Any:
     """Use a contextmanager to setUp a test case."""
     val = cm.__enter__()
     testcase.addCleanup(cm.__exit__, None, None, None)
```

### Comparing `tornado-6.2b2/tornado/util.py` & `tornado-6.3b1/tornado/util.py`

 * *Files identical despite different names*

### Comparing `tornado-6.2b2/tornado/web.py` & `tornado-6.3b1/tornado/web.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 <http://en.wikipedia.org/wiki/Push_technology#Long_polling>`_.
 
 Here is a simple "Hello, world" example app:
 
 .. testcode::
 
     import asyncio
-    import tornado.web
+    import tornado
 
     class MainHandler(tornado.web.RequestHandler):
         def get(self):
             self.write("Hello, world")
 
     async def main():
         application = tornado.web.Application([
@@ -87,18 +87,16 @@
 
 from tornado.concurrent import Future, future_set_result_unless_cancelled
 from tornado import escape
 from tornado import gen
 from tornado.httpserver import HTTPServer
 from tornado import httputil
 from tornado import iostream
-import tornado.locale
 from tornado import locale
 from tornado.log import access_log, app_log, gen_log
-import tornado.netutil
 from tornado import template
 from tornado.escape import utf8, _unicode
 from tornado.routing import (
     AnyMatches,
     DefaultHostMatches,
     HostMatches,
     ReversibleRouter,
@@ -162,15 +160,15 @@
 
 May be overridden by passing a ``version`` keyword argument.
 
 .. versionadded:: 3.2.1
 """
 
 DEFAULT_SIGNED_VALUE_MIN_VERSION = 1
-"""The oldest signed value accepted by `.RequestHandler.get_secure_cookie`.
+"""The oldest signed value accepted by `.RequestHandler.get_signed_cookie`.
 
 May be overridden by passing a ``min_version`` keyword argument.
 
 .. versionadded:: 3.2.1
 """
 
 
@@ -206,15 +204,15 @@
     path_args = None  # type: List[str]
     path_kwargs = None  # type: Dict[str, str]
 
     def __init__(
         self,
         application: "Application",
         request: httputil.HTTPServerRequest,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None:
         super().__init__()
 
         self.application = application
         self.request = request
         self._headers_written = False
         self._finished = False
@@ -599,29 +597,36 @@
         self,
         name: str,
         value: Union[str, bytes],
         domain: Optional[str] = None,
         expires: Optional[Union[float, Tuple, datetime.datetime]] = None,
         path: str = "/",
         expires_days: Optional[float] = None,
-        **kwargs: Any
+        # Keyword-only args start here for historical reasons.
+        *,
+        max_age: Optional[int] = None,
+        httponly: bool = False,
+        secure: bool = False,
+        samesite: Optional[str] = None,
     ) -> None:
         """Sets an outgoing cookie name/value with the given options.
 
         Newly-set cookies are not immediately visible via `get_cookie`;
         they are not present until the next request.
 
-        expires may be a numeric timestamp as returned by `time.time`,
+        Most arguments are passed directly to `http.cookies.Morsel` directly.
+        See https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Set-Cookie
+        for more information.
+
+        ``expires`` may be a numeric timestamp as returned by `time.time`,
         a time tuple as returned by `time.gmtime`, or a
-        `datetime.datetime` object.
+        `datetime.datetime` object. ``expires_days`` is provided as a convenience
+        to set an expiration time in days from today (if both are set, ``expires``
+        is used).
 
-        Additional keyword arguments are set on the cookies.Morsel
-        directly.
-        See https://docs.python.org/3/library/http.cookies.html#http.cookies.Morsel
-        for available attributes.
         """
         # The cookie library only accepts type str, in both python 2 and 3
         name = escape.native_str(name)
         value = escape.native_str(value)
         if re.search(r"[\x00-\x20]", name + value):
             # Don't let us accidentally inject bad stuff
             raise ValueError("Invalid cookie %r: %r" % (name, value))
@@ -637,104 +642,138 @@
             morsel["domain"] = domain
         if expires_days is not None and not expires:
             expires = datetime.datetime.utcnow() + datetime.timedelta(days=expires_days)
         if expires:
             morsel["expires"] = httputil.format_timestamp(expires)
         if path:
             morsel["path"] = path
-        for k, v in kwargs.items():
-            if k == "max_age":
-                k = "max-age"
-
-            # skip falsy values for httponly and secure flags because
-            # SimpleCookie sets them regardless
-            if k in ["httponly", "secure"] and not v:
-                continue
+        if max_age:
+            # Note change from _ to -.
+            morsel["max-age"] = str(max_age)
+        if httponly:
+            # Note that SimpleCookie ignores the value here. The presense of an
+            # httponly (or secure) key is treated as true.
+            morsel["httponly"] = True
+        if secure:
+            morsel["secure"] = True
+        if samesite:
+            morsel["samesite"] = samesite
 
-            morsel[k] = v
-
-    def clear_cookie(
-        self, name: str, path: str = "/", domain: Optional[str] = None
-    ) -> None:
+    def clear_cookie(self, name: str, **kwargs: Any) -> None:
         """Deletes the cookie with the given name.
 
-        Due to limitations of the cookie protocol, you must pass the same
-        path and domain to clear a cookie as were used when that cookie
-        was set (but there is no way to find out on the server side
-        which values were used for a given cookie).
+        This method accepts the same arguments as `set_cookie`, except for
+        ``expires`` and ``max_age``. Clearing a cookie requires the same
+        ``domain`` and ``path`` arguments as when it was set. In some cases the
+        ``samesite`` and ``secure`` arguments are also required to match. Other
+        arguments are ignored.
 
         Similar to `set_cookie`, the effect of this method will not be
         seen until the following request.
-        """
+
+        .. versionchanged:: 6.3
+
+           Now accepts all keyword arguments that ``set_cookie`` does.
+           The ``samesite`` and ``secure`` flags have recently become
+           required for clearing ``samesite="none"`` cookies.
+        """
+        for excluded_arg in ["expires", "max_age"]:
+            if excluded_arg in kwargs:
+                raise TypeError(
+                    f"clear_cookie() got an unexpected keyword argument '{excluded_arg}'"
+                )
         expires = datetime.datetime.utcnow() - datetime.timedelta(days=365)
-        self.set_cookie(name, value="", path=path, expires=expires, domain=domain)
+        self.set_cookie(name, value="", expires=expires, **kwargs)
 
-    def clear_all_cookies(self, path: str = "/", domain: Optional[str] = None) -> None:
-        """Deletes all the cookies the user sent with this request.
+    def clear_all_cookies(self, **kwargs: Any) -> None:
+        """Attempt to delete all the cookies the user sent with this request.
 
-        See `clear_cookie` for more information on the path and domain
-        parameters.
+        See `clear_cookie` for more information on keyword arguments. Due to
+        limitations of the cookie protocol, it is impossible to determine on the
+        server side which values are necessary for the ``domain``, ``path``,
+        ``samesite``, or ``secure`` arguments, this method can only be
+        successful if you consistently use the same values for these arguments
+        when setting cookies.
 
-        Similar to `set_cookie`, the effect of this method will not be
-        seen until the following request.
+        Similar to `set_cookie`, the effect of this method will not be seen
+        until the following request.
 
         .. versionchanged:: 3.2
 
            Added the ``path`` and ``domain`` parameters.
+
+        .. versionchanged:: 6.3
+
+           Now accepts all keyword arguments that ``set_cookie`` does.
+
+        .. deprecated:: 6.3
+
+           The increasingly complex rules governing cookies have made it
+           impossible for a ``clear_all_cookies`` method to work reliably
+           since all we know about cookies are their names. Applications
+           should generally use ``clear_cookie`` one at a time instead.
         """
         for name in self.request.cookies:
-            self.clear_cookie(name, path=path, domain=domain)
+            self.clear_cookie(name, **kwargs)
 
-    def set_secure_cookie(
+    def set_signed_cookie(
         self,
         name: str,
         value: Union[str, bytes],
         expires_days: Optional[float] = 30,
         version: Optional[int] = None,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None:
         """Signs and timestamps a cookie so it cannot be forged.
 
         You must specify the ``cookie_secret`` setting in your Application
         to use this method. It should be a long, random sequence of bytes
         to be used as the HMAC secret for the signature.
 
-        To read a cookie set with this method, use `get_secure_cookie()`.
+        To read a cookie set with this method, use `get_signed_cookie()`.
 
         Note that the ``expires_days`` parameter sets the lifetime of the
         cookie in the browser, but is independent of the ``max_age_days``
-        parameter to `get_secure_cookie`.
+        parameter to `get_signed_cookie`.
         A value of None limits the lifetime to the current browser session.
 
         Secure cookies may contain arbitrary byte values, not just unicode
         strings (unlike regular cookies)
 
         Similar to `set_cookie`, the effect of this method will not be
         seen until the following request.
 
         .. versionchanged:: 3.2.1
 
            Added the ``version`` argument.  Introduced cookie version 2
            and made it the default.
+
+        .. versionchanged:: 6.3
+
+           Renamed from ``set_secure_cookie`` to ``set_signed_cookie`` to
+           avoid confusion with other uses of "secure" in cookie attributes
+           and prefixes. The old name remains as an alias.
         """
         self.set_cookie(
             name,
             self.create_signed_value(name, value, version=version),
             expires_days=expires_days,
-            **kwargs
+            **kwargs,
         )
 
+    set_secure_cookie = set_signed_cookie
+
     def create_signed_value(
         self, name: str, value: Union[str, bytes], version: Optional[int] = None
     ) -> bytes:
         """Signs and timestamps a string so it cannot be forged.
 
-        Normally used via set_secure_cookie, but provided as a separate
+        Normally used via set_signed_cookie, but provided as a separate
         method for non-cookie uses.  To decode a value not stored
-        as a cookie use the optional value argument to get_secure_cookie.
+        as a cookie use the optional value argument to get_signed_cookie.
 
         .. versionchanged:: 3.2.1
 
            Added the ``version`` argument.  Introduced cookie version 2
            and made it the default.
         """
         self.require_setting("cookie_secret", "secure cookies")
@@ -745,60 +784,79 @@
                 raise Exception("key_version setting must be used for secret_key dicts")
             key_version = self.application.settings["key_version"]
 
         return create_signed_value(
             secret, name, value, version=version, key_version=key_version
         )
 
-    def get_secure_cookie(
+    def get_signed_cookie(
         self,
         name: str,
         value: Optional[str] = None,
         max_age_days: float = 31,
         min_version: Optional[int] = None,
     ) -> Optional[bytes]:
         """Returns the given signed cookie if it validates, or None.
 
         The decoded cookie value is returned as a byte string (unlike
         `get_cookie`).
 
         Similar to `get_cookie`, this method only returns cookies that
         were present in the request. It does not see outgoing cookies set by
-        `set_secure_cookie` in this handler.
+        `set_signed_cookie` in this handler.
 
         .. versionchanged:: 3.2.1
 
            Added the ``min_version`` argument.  Introduced cookie version 2;
            both versions 1 and 2 are accepted by default.
+
+         .. versionchanged:: 6.3
+
+           Renamed from ``get_secure_cookie`` to ``get_signed_cookie`` to
+           avoid confusion with other uses of "secure" in cookie attributes
+           and prefixes. The old name remains as an alias.
+
         """
         self.require_setting("cookie_secret", "secure cookies")
         if value is None:
             value = self.get_cookie(name)
         return decode_signed_value(
             self.application.settings["cookie_secret"],
             name,
             value,
             max_age_days=max_age_days,
             min_version=min_version,
         )
 
-    def get_secure_cookie_key_version(
+    get_secure_cookie = get_signed_cookie
+
+    def get_signed_cookie_key_version(
         self, name: str, value: Optional[str] = None
     ) -> Optional[int]:
         """Returns the signing key version of the secure cookie.
 
         The version is returned as int.
+
+        .. versionchanged:: 6.3
+
+           Renamed from ``get_secure_cookie_key_version`` to
+           ``set_signed_cookie_key_version`` to avoid confusion with other
+           uses of "secure" in cookie attributes and prefixes. The old name
+           remains as an alias.
+
         """
         self.require_setting("cookie_secret", "secure cookies")
         if value is None:
             value = self.get_cookie(name)
         if value is None:
             return None
         return get_signature_key_version(value)
 
+    get_secure_cookie_key_version = get_signed_cookie_key_version
+
     def redirect(
         self, url: str, permanent: bool = False, status: Optional[int] = None
     ) -> None:
         """Sends a redirect to the given (optionally relative) URL.
 
         If the ``status`` argument is specified, that value is used as the
         HTTP status code; otherwise either 301 (permanent) or 302
@@ -1317,25 +1375,25 @@
 
         * A subclass may override `get_current_user()`, which will be called
           automatically the first time ``self.current_user`` is accessed.
           `get_current_user()` will only be called once per request,
           and is cached for future access::
 
               def get_current_user(self):
-                  user_cookie = self.get_secure_cookie("user")
+                  user_cookie = self.get_signed_cookie("user")
                   if user_cookie:
                       return json.loads(user_cookie)
                   return None
 
         * It may be set as a normal variable, typically from an overridden
           `prepare()`::
 
               @gen.coroutine
               def prepare(self):
-                  user_id_cookie = self.get_secure_cookie("user_id")
+                  user_id_cookie = self.get_signed_cookie("user_id")
                   if user_id_cookie:
                       self.current_user = yield load_user(user_id_cookie)
 
         Note that `prepare()` may be a coroutine while `get_current_user()`
         may not, so the latter form is necessary if loading the user requires
         asynchronous operations.
 
@@ -1422,30 +1480,32 @@
                     ]
                 )
             else:
                 raise ValueError("unknown xsrf cookie version %d", output_version)
             if version is None:
                 if self.current_user and "expires_days" not in cookie_kwargs:
                     cookie_kwargs["expires_days"] = 30
-                self.set_cookie("_xsrf", self._xsrf_token, **cookie_kwargs)
+                cookie_name = self.settings.get("xsrf_cookie_name", "_xsrf")
+                self.set_cookie(cookie_name, self._xsrf_token, **cookie_kwargs)
         return self._xsrf_token
 
     def _get_raw_xsrf_token(self) -> Tuple[Optional[int], bytes, float]:
         """Read or generate the xsrf token in its raw form.
 
         The raw_xsrf_token is a tuple containing:
 
         * version: the version of the cookie from which this token was read,
           or None if we generated a new token in this request.
         * token: the raw token data; random (non-ascii) bytes.
         * timestamp: the time this token was generated (will not be accurate
           for version 1 cookies)
         """
         if not hasattr(self, "_raw_xsrf_token"):
-            cookie = self.get_cookie("_xsrf")
+            cookie_name = self.settings.get("xsrf_cookie_name", "_xsrf")
+            cookie = self.get_cookie(cookie_name)
             if cookie:
                 version, token, timestamp = self._decode_xsrf_token(cookie)
             else:
                 version, token, timestamp = None, None, None
             if token is None:
                 version = None
                 token = os.urandom(16)
@@ -1639,15 +1699,15 @@
         before completing the request.  The ``Etag`` header should be set
         (perhaps with `set_etag_header`) before calling this method.
         """
         computed_etag = utf8(self._headers.get("Etag", ""))
         # Find all weak and strong etag values from If-None-Match header
         # because RFC 7232 allows multiple etag values in a single header.
         etags = re.findall(
-            br'\*|(?:W/)?"[^"]*"', utf8(self.request.headers.get("If-None-Match", ""))
+            rb'\*|(?:W/)?"[^"]*"', utf8(self.request.headers.get("If-None-Match", ""))
         )
         if not computed_etag or not etags:
             return False
 
         match = False
         if etags[0] == b"*":
             match = True
@@ -1672,28 +1732,24 @@
                 raise HTTPError(405)
             self.path_args = [self.decode_argument(arg) for arg in args]
             self.path_kwargs = dict(
                 (k, self.decode_argument(v, name=k)) for (k, v) in kwargs.items()
             )
             # If XSRF cookies are turned on, reject form submissions without
             # the proper cookie
-            if (
-                self.request.method
-                not in (
-                    "GET",
-                    "HEAD",
-                    "OPTIONS",
-                )
-                and self.application.settings.get("xsrf_cookies")
-            ):
+            if self.request.method not in (
+                "GET",
+                "HEAD",
+                "OPTIONS",
+            ) and self.application.settings.get("xsrf_cookies"):
                 self.check_xsrf_cookie()
 
             result = self.prepare()
             if result is not None:
-                result = await result
+                result = await result  # type: ignore
             if self._prepared_future is not None:
                 # Tell the Application we've finished with prepare()
                 # and are ready for the body to arrive.
                 future_set_result_unless_cancelled(self._prepared_future, None)
             if self._finished:
                 return
 
@@ -1844,15 +1900,15 @@
       if the request has an empty body, ``data_received`` may not be called.
     * ``prepare`` and ``data_received`` may return Futures (such as via
       ``@gen.coroutine``, in which case the next method will not be called
       until those futures have completed.
     * The regular HTTP method (``post``, ``put``, etc) will be called after
       the entire body has been read.
 
-    See the `file receiver demo <https://github.com/tornadoweb/tornado/tree/master/demos/file_upload/>`_
+    See the `file receiver demo <https://github.com/tornadoweb/tornado/tree/stable/demos/file_upload/>`_
     for example usage.
     """  # noqa: E501
     if not issubclass(cls, RequestHandler):
         raise TypeError("expected subclass of RequestHandler, got %r", cls)
     cls._stream_request_body = True
     return cls
 
@@ -2042,15 +2098,15 @@
     """
 
     def __init__(
         self,
         handlers: Optional[_RuleList] = None,
         default_host: Optional[str] = None,
         transforms: Optional[List[Type["OutputTransform"]]] = None,
-        **settings: Any
+        **settings: Any,
     ) -> None:
         if transforms is None:
             self.transforms = []  # type: List[Type[OutputTransform]]
             if settings.get("compress_response") or settings.get("gzip"):
                 self.transforms.append(GZipContentEncoding)
         else:
             self.transforms = transforms
@@ -2102,15 +2158,15 @@
         port: int,
         address: Optional[str] = None,
         *,
         family: socket.AddressFamily = socket.AF_UNSPEC,
         backlog: int = tornado.netutil._DEFAULT_BACKLOG,
         flags: Optional[int] = None,
         reuse_port: bool = False,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> HTTPServer:
         """Starts an HTTP server for this application on the given port.
 
         This is a convenience alias for creating an `.HTTPServer` object and
         calling its listen method.  Keyword arguments not supported by
         `HTTPServer.listen <.TCPServer.listen>` are passed to the `.HTTPServer`
         constructor.  For advanced uses (e.g. multi-process mode), do not use
@@ -2389,15 +2445,15 @@
     """
 
     def __init__(
         self,
         status_code: int = 500,
         log_message: Optional[str] = None,
         *args: Any,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None:
         self.status_code = status_code
         self.log_message = log_message
         self.args = args
         self.reason = kwargs.get("reason", None)
         if log_message and not args:
             self.log_message = log_message.replace("%", "%%")
@@ -3437,15 +3493,15 @@
         return to_sign + signature
     else:
         raise ValueError("Unsupported version %d" % version)
 
 
 # A leading version number in decimal
 # with no leading zeros, followed by a pipe.
-_signed_value_version_re = re.compile(br"^([1-9][0-9]*)\|(.*)$")
+_signed_value_version_re = re.compile(rb"^([1-9][0-9]*)\|(.*)$")
 
 
 def _get_version(value: bytes) -> int:
     # Figures out what version value is.  Version 1 did not include an
     # explicit version field and started with arbitrary base64 data,
     # which makes this tricky.
     m = _signed_value_version_re.match(value)
```

### Comparing `tornado-6.2b2/tornado/websocket.py` & `tornado-6.3b1/tornado/websocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 """Implementation of the WebSocket protocol.
 
 `WebSockets <http://dev.w3.org/html5/websockets/>`_ allow for bidirectional
-communication between the browser and server.
-
-WebSockets are supported in the current versions of all major browsers,
-although older versions that do not support WebSockets are still in use
-(refer to http://caniuse.com/websockets for details).
+communication between the browser and server. WebSockets are supported in the
+current versions of all major browsers.
 
 This module implements the final version of the WebSocket protocol as
-defined in `RFC 6455 <http://tools.ietf.org/html/rfc6455>`_.  Certain
-browser versions (notably Safari 5.x) implemented an earlier draft of
-the protocol (known as "draft 76") and are not compatible with this module.
+defined in `RFC 6455 <http://tools.ietf.org/html/rfc6455>`_.
 
 .. versionchanged:: 4.0
    Removed support for the draft 76 protocol version.
 """
 
 import abc
 import asyncio
 import base64
 import hashlib
 import os
 import sys
 import struct
-import tornado.escape
-import tornado.web
+import tornado
 from urllib.parse import urlparse
 import zlib
 
 from tornado.concurrent import Future, future_set_result_unless_cancelled
 from tornado.escape import utf8, native_str, to_unicode
 from tornado import gen, httpclient, httputil
 from tornado.ioloop import IOLoop, PeriodicCallback
 from tornado.iostream import StreamClosedError, IOStream
 from tornado.log import gen_log, app_log
+from tornado.netutil import Resolver
 from tornado import simple_httpclient
 from tornado.queues import Queue
 from tornado.tcpclient import TCPClient
 from tornado.util import _websocket_mask
 
 from typing import (
     TYPE_CHECKING,
@@ -818,15 +813,15 @@
         self.mask_outgoing = mask_outgoing
         self.params = params
         self._final_frame = False
         self._frame_opcode = None
         self._masked_frame = None
         self._frame_mask = None  # type: Optional[bytes]
         self._frame_length = None
-        self._fragmented_message_buffer = None  # type: Optional[bytes]
+        self._fragmented_message_buffer = None  # type: Optional[bytearray]
         self._fragmented_message_opcode = None
         self._waiting = None  # type: object
         self._compression_options = params.compression_options
         self._decompressor = None  # type: Optional[_PerMessageDeflateDecompressor]
         self._compressor = None  # type: Optional[_PerMessageDeflateCompressor]
         self._frame_compressed = None  # type: Optional[bool]
         # The total uncompressed size of all messages received or sent.
@@ -1173,27 +1168,27 @@
                 self._abort()
                 return
         elif opcode == 0:  # continuation frame
             if self._fragmented_message_buffer is None:
                 # nothing to continue
                 self._abort()
                 return
-            self._fragmented_message_buffer += data
+            self._fragmented_message_buffer.extend(data)
             if is_final_frame:
                 opcode = self._fragmented_message_opcode
-                data = self._fragmented_message_buffer
+                data = bytes(self._fragmented_message_buffer)
                 self._fragmented_message_buffer = None
         else:  # start of new data message
             if self._fragmented_message_buffer is not None:
                 # can't start new message until the old one is finished
                 self._abort()
                 return
             if not is_final_frame:
                 self._fragmented_message_opcode = opcode
-                self._fragmented_message_buffer = data
+                self._fragmented_message_buffer = bytearray(data)
 
         if is_final_frame:
             handled_future = self._handle_message(opcode, data)
             if handled_future is not None:
                 await handled_future
 
     def _handle_message(self, opcode: int, data: bytes) -> "Optional[Future[None]]":
@@ -1358,14 +1353,15 @@
         request: httpclient.HTTPRequest,
         on_message_callback: Optional[Callable[[Union[None, str, bytes]], None]] = None,
         compression_options: Optional[Dict[str, Any]] = None,
         ping_interval: Optional[float] = None,
         ping_timeout: Optional[float] = None,
         max_message_size: int = _default_max_message_size,
         subprotocols: Optional[List[str]] = [],
+        resolver: Optional[Resolver] = None,
     ) -> None:
         self.connect_future = Future()  # type: Future[WebSocketClientConnection]
         self.read_queue = Queue(1)  # type: Queue[Union[None, str, bytes]]
         self.key = base64.b64encode(os.urandom(16))
         self._on_message_callback = on_message_callback
         self.close_code = None  # type: Optional[int]
         self.close_reason = None  # type: Optional[str]
@@ -1398,15 +1394,15 @@
             request.headers[
                 "Sec-WebSocket-Extensions"
             ] = "permessage-deflate; client_max_window_bits"
 
         # Websocket connection is currently unable to follow redirects
         request.follow_redirects = False
 
-        self.tcp_client = TCPClient()
+        self.tcp_client = TCPClient(resolver=resolver)
         super().__init__(
             None,
             request,
             lambda: None,
             self._on_http_response,
             104857600,
             self.tcp_client,
@@ -1584,14 +1580,15 @@
     connect_timeout: Optional[float] = None,
     on_message_callback: Optional[Callable[[Union[None, str, bytes]], None]] = None,
     compression_options: Optional[Dict[str, Any]] = None,
     ping_interval: Optional[float] = None,
     ping_timeout: Optional[float] = None,
     max_message_size: int = _default_max_message_size,
     subprotocols: Optional[List[str]] = None,
+    resolver: Optional[Resolver] = None,
 ) -> "Awaitable[WebSocketClientConnection]":
     """Client-side websocket support.
 
     Takes a url and returns a Future whose result is a
     `WebSocketClientConnection`.
 
     ``compression_options`` is interpreted in the same way as the
@@ -1627,14 +1624,17 @@
        arguments, which have the same meaning as in `WebSocketHandler`.
 
     .. versionchanged:: 5.0
        The ``io_loop`` argument (deprecated since version 4.1) has been removed.
 
     .. versionchanged:: 5.1
        Added the ``subprotocols`` argument.
+
+    .. versionchanged:: 6.3
+       Added the ``resolver`` argument.
     """
     if isinstance(url, httpclient.HTTPRequest):
         assert connect_timeout is None
         request = url
         # Copy and convert the headers dict/object (see comments in
         # AsyncHTTPClient.fetch)
         request.headers = httputil.HTTPHeaders(request.headers)
@@ -1648,11 +1648,12 @@
         request,
         on_message_callback=on_message_callback,
         compression_options=compression_options,
         ping_interval=ping_interval,
         ping_timeout=ping_timeout,
         max_message_size=max_message_size,
         subprotocols=subprotocols,
+        resolver=resolver,
     )
     if callback is not None:
         IOLoop.current().add_future(conn.connect_future, callback)
     return conn.connect_future
```

### Comparing `tornado-6.2b2/tornado/wsgi.py` & `tornado-6.3b1/tornado/wsgi.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,20 +23,23 @@
 the Tornado HTTP server. The reverse is not supported; the Tornado
 `.Application` and `.RequestHandler` classes are designed for use with
 the Tornado `.HTTPServer` and cannot be used in a generic WSGI
 container.
 
 """
 
-import sys
+import concurrent.futures
 from io import BytesIO
 import tornado
+import sys
 
+from tornado.concurrent import dummy_executor
 from tornado import escape
 from tornado import httputil
+from tornado.ioloop import IOLoop
 from tornado.log import access_log
 
 from typing import List, Tuple, Optional, Callable, Any, Dict, Text
 from types import TracebackType
 import typing
 
 if typing.TYPE_CHECKING:
@@ -50,28 +53,36 @@
 # here to minimize the temptation to use it in non-wsgi contexts.
 def to_wsgi_str(s: bytes) -> str:
     assert isinstance(s, bytes)
     return s.decode("latin1")
 
 
 class WSGIContainer(object):
-    r"""Makes a WSGI-compatible function runnable on Tornado's HTTP server.
+    r"""Makes a WSGI-compatible application runnable on Tornado's HTTP server.
 
     .. warning::
 
        WSGI is a *synchronous* interface, while Tornado's concurrency model
-       is based on single-threaded asynchronous execution.  This means that
-       running a WSGI app with Tornado's `WSGIContainer` is *less scalable*
-       than running the same app in a multi-threaded WSGI server like
-       ``gunicorn`` or ``uwsgi``.  Use `WSGIContainer` only when there are
-       benefits to combining Tornado and WSGI in the same process that
-       outweigh the reduced scalability.
+       is based on single-threaded *asynchronous* execution.  Many of Tornado's
+       distinguishing features are not available in WSGI mode, including efficient
+       long-polling and websockets. The primary purpose of `WSGIContainer` is
+       to support both WSGI applications and native Tornado ``RequestHandlers`` in
+       a single process. WSGI-only applications are likely to be better off
+       with a dedicated WSGI server such as ``gunicorn`` or ``uwsgi``.
+
+    Wrap a WSGI application in a `WSGIContainer` to make it implement the Tornado
+    `.HTTPServer` ``request_callback`` interface.  The `WSGIContainer` object can
+    then be passed to classes from the `tornado.routing` module,
+    `tornado.web.FallbackHandler`, or to `.HTTPServer` directly.
 
-    Wrap a WSGI function in a `WSGIContainer` and pass it to `.HTTPServer` to
-    run it. For example::
+    This class is intended to let other frameworks (Django, Flask, etc)
+    run on the Tornado HTTP server and I/O loop.
+
+    Realistic usage will be more complicated, but the simplest possible example uses a
+    hand-written WSGI application with `.HTTPServer`::
 
         def simple_app(environ, start_response):
             status = "200 OK"
             response_headers = [("Content-type", "text/plain")]
             start_response(status, response_headers)
             return [b"Hello world!\n"]
 
@@ -79,26 +90,54 @@
             container = tornado.wsgi.WSGIContainer(simple_app)
             http_server = tornado.httpserver.HTTPServer(container)
             http_server.listen(8888)
             await asyncio.Event().wait()
 
         asyncio.run(main())
 
-    This class is intended to let other frameworks (Django, web.py, etc)
-    run on the Tornado HTTP server and I/O loop.
+    The recommended pattern is to use the `tornado.routing` module to set up routing
+    rules between your WSGI application and, typically, a `tornado.web.Application`.
+    Alternatively, `tornado.web.Application` can be used as the top-level router
+    and `tornado.web.FallbackHandler` can embed a `WSGIContainer` within it.
+
+    If the ``executor`` argument is provided, the WSGI application will be executed
+    on that executor. This must be an instance of `concurrent.futures.Executor`,
+    typically a ``ThreadPoolExecutor`` (``ProcessPoolExecutor`` is not supported).
+    If no ``executor`` is given, the application will run on the event loop thread in
+    Tornado 6.3; this will change to use an internal thread pool by default in
+    Tornado 7.0.
 
-    The `tornado.web.FallbackHandler` class is often useful for mixing
-    Tornado and WSGI apps in the same server.  See
-    https://github.com/bdarnell/django-tornado-demo for a complete example.
+    .. warning::
+       By default, the WSGI application is executed on the event loop's thread. This
+       limits the server to one request at a time (per process), making it less scalable
+       than most other WSGI servers. It is therefore highly recommended that you pass
+       a ``ThreadPoolExecutor`` when constructing the `WSGIContainer`, after verifying
+       that your application is thread-safe. The default will change to use a
+       ``ThreadPoolExecutor`` in Tornado 7.0.
+
+    .. versionadded:: 6.3
+       The ``executor`` parameter.
+
+    .. deprecated:: 6.3
+       The default behavior of running the WSGI application on the event loop thread
+       is deprecated and will change in Tornado 7.0 to use a thread pool by default.
     """
 
-    def __init__(self, wsgi_application: "WSGIAppType") -> None:
+    def __init__(
+        self,
+        wsgi_application: "WSGIAppType",
+        executor: Optional[concurrent.futures.Executor] = None,
+    ) -> None:
         self.wsgi_application = wsgi_application
+        self.executor = dummy_executor if executor is None else executor
 
     def __call__(self, request: httputil.HTTPServerRequest) -> None:
+        IOLoop.current().spawn_callback(self.handle_request, request)
+
+    async def handle_request(self, request: httputil.HTTPServerRequest) -> None:
         data = {}  # type: Dict[str, Any]
         response = []  # type: List[bytes]
 
         def start_response(
             status: str,
             headers: List[Tuple[str, str]],
             exc_info: Optional[
@@ -109,23 +148,41 @@
                 ]
             ] = None,
         ) -> Callable[[bytes], Any]:
             data["status"] = status
             data["headers"] = headers
             return response.append
 
-        app_response = self.wsgi_application(
-            WSGIContainer.environ(request), start_response
+        loop = IOLoop.current()
+        app_response = await loop.run_in_executor(
+            self.executor,
+            self.wsgi_application,
+            self.environ(request),
+            start_response,
         )
         try:
-            response.extend(app_response)
-            body = b"".join(response)
+            app_response_iter = iter(app_response)
+
+            def next_chunk() -> Optional[bytes]:
+                try:
+                    return next(app_response_iter)
+                except StopIteration:
+                    # StopIteration is special and is not allowed to pass through
+                    # coroutines normally.
+                    return None
+
+            while True:
+                chunk = await loop.run_in_executor(self.executor, next_chunk)
+                if chunk is None:
+                    break
+                response.append(chunk)
         finally:
             if hasattr(app_response, "close"):
                 app_response.close()  # type: ignore
+        body = b"".join(response)
         if not data:
             raise Exception("WSGI app did not call start_response")
 
         status_code_str, reason = data["status"].split(" ", 1)
         status_code = int(status_code_str)
         headers = data["headers"]  # type: List[Tuple[str, str]]
         header_set = set(k.lower() for (k, v) in headers)
@@ -143,17 +200,20 @@
         for key, value in headers:
             header_obj.add(key, value)
         assert request.connection is not None
         request.connection.write_headers(start_line, header_obj, chunk=body)
         request.connection.finish()
         self._log(status_code, request)
 
-    @staticmethod
-    def environ(request: httputil.HTTPServerRequest) -> Dict[Text, Any]:
-        """Converts a `tornado.httputil.HTTPServerRequest` to a WSGI environment."""
+    def environ(self, request: httputil.HTTPServerRequest) -> Dict[Text, Any]:
+        """Converts a `tornado.httputil.HTTPServerRequest` to a WSGI environment.
+
+        .. versionchanged:: 6.3
+           No longer a static method.
+        """
         hostport = request.host.split(":")
         if len(hostport) == 2:
             host = hostport[0]
             port = int(hostport[1])
         else:
             host = request.host
             port = 443 if request.protocol == "https" else 80
@@ -168,15 +228,15 @@
             "SERVER_NAME": host,
             "SERVER_PORT": str(port),
             "SERVER_PROTOCOL": request.version,
             "wsgi.version": (1, 0),
             "wsgi.url_scheme": request.protocol,
             "wsgi.input": BytesIO(escape.utf8(request.body)),
             "wsgi.errors": sys.stderr,
-            "wsgi.multithread": False,
+            "wsgi.multithread": self.executor is not dummy_executor,
             "wsgi.multiprocess": True,
             "wsgi.run_once": False,
         }
         if "Content-Type" in request.headers:
             environ["CONTENT_TYPE"] = request.headers.pop("Content-Type")
         if "Content-Length" in request.headers:
             environ["CONTENT_LENGTH"] = request.headers.pop("Content-Length")
```

### Comparing `tornado-6.2b2/tornado.egg-info/PKG-INFO` & `tornado-6.3b1/tornado.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: tornado
-Version: 6.2b2
+Version: 6.3b1
 Summary: Tornado is a Python web framework and asynchronous networking library, originally developed at FriendFeed.
 Home-page: http://www.tornadoweb.org/
 Author: Facebook
 Author-email: python-tornado@googlegroups.com
-License: http://www.apache.org/licenses/LICENSE-2.0
+License: Apache-2.0
 Project-URL: Source, https://github.com/tornadoweb/tornado
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >= 3.7
+Requires-Python: >= 3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Tornado Web Server
 ==================
 
 .. image:: https://badges.gitter.im/Join%20Chat.svg
@@ -39,16 +39,15 @@
 ------------
 
 Here is a simple "Hello, world" example web app for Tornado:
 
 .. code-block:: python
 
     import asyncio
-
-    import tornado.web
+    import tornado
 
     class MainHandler(tornado.web.RequestHandler):
         def get(self):
             self.write("Hello, world")
 
     def make_app():
         return tornado.web.Application([
```

### Comparing `tornado-6.2b2/tornado.egg-info/SOURCES.txt` & `tornado-6.3b1/tornado.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -70,16 +70,14 @@
 docs/log.rst
 docs/netutil.rst
 docs/networking.rst
 docs/options.rst
 docs/process.rst
 docs/queues.rst
 docs/releases.rst
-docs/requirements.in
-docs/requirements.txt
 docs/routing.rst
 docs/tcpclient.rst
 docs/tcpserver.rst
 docs/template.rst
 docs/testing.rst
 docs/tornado.png
 docs/twisted.rst
@@ -142,14 +140,15 @@
 docs/releases/v6.0.0.rst
 docs/releases/v6.0.1.rst
 docs/releases/v6.0.2.rst
 docs/releases/v6.0.3.rst
 docs/releases/v6.0.4.rst
 docs/releases/v6.1.0.rst
 docs/releases/v6.2.0.rst
+docs/releases/v6.3.0.rst
 tornado/__init__.py
 tornado/_locale_data.py
 tornado/auth.py
 tornado/autoreload.py
 tornado/concurrent.py
 tornado/curl_httpclient.py
 tornado/escape.py
```

