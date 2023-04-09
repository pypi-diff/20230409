# Comparing `tmp/PyPtt-1.0.6.tar.gz` & `tmp/PyPtt-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPtt-1.0.6.tar", last modified: Sat Jan 28 06:08:50 2023, max compression
+gzip compressed data, was "PyPtt-1.0.7.tar", last modified: Sun Apr  9 09:46:25 2023, max compression
```

## Comparing `PyPtt-1.0.6.tar` & `PyPtt-1.0.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 06:08:50.638461 PyPtt-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-01-28 06:08:41.000000 PyPtt-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-01-28 06:08:41.000000 PyPtt-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-01-28 06:08:50.638461 PyPtt-1.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 06:08:50.638461 PyPtt-1.0.6/PyPtt/
--rw-r--r--   0 runner    (1001) docker     (123)    30672 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/PTT.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_call_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_change_pw.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_del_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_get_board_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_get_board_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_get_bottom_post_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_get_favourite_board.py
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_get_newest_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    22678 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_get_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_get_post_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_get_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_give_money.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_has_new_mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     7533 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_loginout.py
--rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_mark_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_reply_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_search_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_set_board_title.py
--rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/_api_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/check_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/connect_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    33897 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/lib_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    54737 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/screens.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-01-28 06:08:41.000000 PyPtt-1.0.6/PyPtt/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 06:08:50.638461 PyPtt-1.0.6/PyPtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-01-28 06:08:50.000000 PyPtt-1.0.6/PyPtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-01-28 06:08:50.000000 PyPtt-1.0.6/PyPtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-28 06:08:50.000000 PyPtt-1.0.6/PyPtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-28 06:08:50.000000 PyPtt-1.0.6/PyPtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-28 06:08:50.000000 PyPtt-1.0.6/PyPtt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-01-28 06:08:41.000000 PyPtt-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-28 06:08:50.638461 PyPtt-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-01-28 06:08:41.000000 PyPtt-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:46:25.868772 PyPtt-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-09 09:46:16.000000 PyPtt-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-09 09:46:16.000000 PyPtt-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-04-09 09:46:25.868772 PyPtt-1.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:46:25.868772 PyPtt-1.0.7/PyPtt/
+-rw-r--r--   0 runner    (1001) docker     (123)    30780 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/PTT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_call_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_change_pw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_del_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_get_board_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_get_board_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_get_bottom_post_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_get_favourite_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_get_newest_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22808 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_get_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_get_post_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_get_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_give_money.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_has_new_mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7533 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_loginout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_mark_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_reply_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_search_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_set_board_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/_api_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/check_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/connect_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33897 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/lib_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54737 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/screens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-09 09:46:16.000000 PyPtt-1.0.7/PyPtt/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 09:46:25.868772 PyPtt-1.0.7/PyPtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-04-09 09:46:25.000000 PyPtt-1.0.7/PyPtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-09 09:46:25.000000 PyPtt-1.0.7/PyPtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 09:46:25.000000 PyPtt-1.0.7/PyPtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-09 09:46:25.000000 PyPtt-1.0.7/PyPtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 09:46:25.000000 PyPtt-1.0.7/PyPtt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-09 09:46:16.000000 PyPtt-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 09:46:25.868772 PyPtt-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-09 09:46:16.000000 PyPtt-1.0.7/setup.py
```

### Comparing `PyPtt-1.0.6/LICENSE` & `PyPtt-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PKG-INFO` & `PyPtt-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPtt
-Version: 1.0.6
+Version: 1.0.7
 Summary: PyPtt
 Home-page: https://github.com/PyPtt/PyPtt
 Author: CodingMan
 Author-email: pttcodingman@gmail.com
 Keywords: PTT,crawler,bot,library,websockets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `PyPtt-1.0.6/PyPtt/PTT.py` & `PyPtt-1.0.7/PyPtt/PTT.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         if host in [data_type.HOST.PTT1, data_type.HOST.PTT2] and connect_mode is data_type.ConnectMode.TELNET:
             raise ValueError('[PyPtt] TELNET is not available on PTT1 and PTT2')
         self.config.connect_mode = connect_mode
 
         self.connect_core = connect_core.API(self.config)
         self._exist_board_list = []
         self._board_info_list = dict()
-        self._ModeratorList = dict()
+        self._moderators = dict()
         # self._last_throw_water_ball_time = 0
         self._thread_id = threading.get_ident()
         self._goto_board_list = []
         self._board_info_list = dict()
 
         self.logger.debug('ThreadID', self._thread_id)
 
@@ -424,15 +424,16 @@
         範例::
 
             import PyPtt
 
             ptt_bot = PyPtt.API()
             try:
                 # .. login ..
-                ptt_bot.comment(board='Test', comment_type=PyPtt.CommentType.PUSH, comment_content='PyPtt 程式推文測試', index=123)
+                ptt_bot.comment(board='Test', comment_type=PyPtt.CommentType.PUSH, content='Comment by index', index=123)
+                ptt_bot.comment(board='Test', comment_type=PyPtt.CommentType.PUSH, content='Comment by index', aid='17MrayxF')
                 # .. do something ..
             finally:
                 ptt_bot.logout()
 
         參考 :ref:`推文類型 <comment-type>`、:ref:`取得最新文章編號 <api-get-newest-index>`
         """
```

### Comparing `PyPtt-1.0.6/PyPtt/_api_bucket.py` & `PyPtt-1.0.7/PyPtt/_api_bucket.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/_api_call_status.py` & `PyPtt-1.0.7/PyPtt/_api_call_status.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/_api_change_pw.py` & `PyPtt-1.0.7/PyPtt/_api_change_pw.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/_api_comment.py` & `PyPtt-1.0.7/PyPtt/_api_comment.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,56 @@
+import collections
 import time
 
 from SingleLog import LogLevel
 
 from . import _api_util
 from . import check_value
 from . import command
 from . import connect_core
 from . import data_type
 from . import exceptions
 from . import i18n
 from . import lib_util
 from . import screens
 
+comment_option = [
+    None,
+    data_type.CommentType.PUSH,
+    data_type.CommentType.BOO,
+    data_type.CommentType.ARROW,
+]
+
 
 def _comment(api,
              board: str,
              push_type: data_type.CommentType,
              push_content: str,
              post_aid: str,
              post_index: int) -> None:
+
+    _api_util.goto_board(api, board)
+
     cmd_list = []
 
     if post_aid is not None:
-        cmd_list.append('#' + post_aid)
+        cmd_list.append(lib_util.check_aid(post_aid))
     elif post_index != 0:
         cmd_list.append(str(post_index))
+    else:
+        raise ValueError('post_aid and post_index cannot be None at the same time')
+
     cmd_list.append(command.enter)
     cmd_list.append(command.comment)
 
     cmd = ''.join(cmd_list)
 
     target_list = [
         connect_core.TargetUnit('您覺得這篇', log_level=LogLevel.DEBUG, break_detect=True),
+        connect_core.TargetUnit(f'→ {api.ptt_id}: ', log_level=LogLevel.DEBUG, break_detect=True),
         connect_core.TargetUnit('加註方式', log_level=LogLevel.DEBUG, break_detect=True),
         connect_core.TargetUnit('禁止快速連續推文', log_level=LogLevel.INFO, break_detect=True,
                                 exceptions_=exceptions.NoFastComment()),
         connect_core.TargetUnit('禁止短時間內大量推文', log_level=LogLevel.INFO, break_detect=True,
                                 exceptions_=exceptions.NoFastComment()),
         connect_core.TargetUnit('使用者不可發言', log_level=LogLevel.INFO, break_detect=True,
                                 exceptions_=exceptions.NoPermission(i18n.no_permission)),
@@ -44,47 +59,55 @@
     ]
 
     index = api.connect_core.send(
         cmd,
         target_list)
 
     if index == -1:
-        if post_aid is not None:
-            raise exceptions.NoSuchPost(board, post_aid)
-        else:
-            raise exceptions.NoSuchPost(board, post_index)
+        raise exceptions.UnknownError('unknown error in comment')
 
     api.logger.info(i18n.has_comment_permission)
 
     cmd_list = []
 
-    if index == 0:
+    if index == 0 or index == 1:
         push_option_line = api.connect_core.get_screen_queue()[-1]
         push_option_line = push_option_line.split('\n')[-1]
 
         api.logger.debug('comment option line', push_option_line)
 
-        enable_push = '值得推薦' in push_option_line
-        enable_boo = '給它噓聲' in push_option_line
-        enable_arrow = '只加→註解' in push_option_line
-
-        api.logger.debug('comment', enable_push)
-        api.logger.debug('Boo', enable_boo)
-        api.logger.debug('Arrow', enable_arrow)
-
-        if push_type == data_type.CommentType.PUSH and not enable_push:
-            push_type = data_type.CommentType.ARROW
-        elif push_type == data_type.CommentType.BOO and not enable_boo:
-            push_type = data_type.CommentType.ARROW
-        elif push_type == data_type.CommentType.ARROW and not enable_arrow:
-            push_type = data_type.CommentType.PUSH
-
-        cmd_list.append(str(push_type))
-    # elif index == 1:
-    #     push_type = data_type.push_type.ARROW
+        available_push_type = collections.defaultdict(lambda: False)
+        first_available_push_type = None
+
+        if '值得推薦' in push_option_line:
+            available_push_type[data_type.CommentType.PUSH] = True
+
+            if first_available_push_type is None:
+                first_available_push_type = data_type.CommentType.PUSH
+
+        if '只加→註解' in push_option_line:
+            available_push_type[data_type.CommentType.ARROW] = True
+
+            if first_available_push_type is None:
+                first_available_push_type = data_type.CommentType.ARROW
+
+        if '給它噓聲' in push_option_line:
+            available_push_type[data_type.CommentType.BOO] = True
+
+            if first_available_push_type is None:
+                first_available_push_type = data_type.CommentType.BOO
+
+        api.logger.debug('available_push_type', available_push_type)
+
+        if available_push_type[push_type] is False:
+            if first_available_push_type:
+                push_type = first_available_push_type
+
+        if True in available_push_type.values():
+            cmd_list.append(str(comment_option.index(push_type)))
 
     cmd_list.append(push_content)
     cmd_list.append(command.enter)
     cmd_list.append('y')
     cmd_list.append(command.enter)
 
     cmd = ''.join(cmd_list)
@@ -96,15 +119,14 @@
     api.connect_core.send(
         cmd,
         target_list)
 
 
 def comment(api, board: str, push_type: data_type.CommentType, push_content: str, post_aid: str,
             post_index: int) -> None:
-    _api_util.goto_board(api, board)
 
     if not api.is_registered_user:
         raise exceptions.UnregisteredUser(lib_util.get_current_func_name())
 
     if not api._is_login:
         raise exceptions.RequireLogin(i18n.require_login)
 
@@ -143,15 +165,14 @@
             api.logger.debug(i18n.push_aligned)
             max_push_length = 32
         else:
             api.logger.debug(i18n.not_push_aligned)
             max_push_length = 43 - len(api.ptt_id)
     else:
         api.logger.debug(i18n.not_record_ip)
-        #     推文對齊
         if board_info[data_type.BoardField.is_comment_aligned]:
             api.logger.debug(i18n.push_aligned)
             max_push_length = 46
         else:
             api.logger.debug(i18n.not_push_aligned)
             max_push_length = 58 - len(api.ptt_id)
```

### Comparing `PyPtt-1.0.6/PyPtt/_api_del_post.py` & `PyPtt-1.0.7/PyPtt/_api_del_post.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,20 @@
             raise exceptions.NoPermission(i18n.no_permission)
 
     _api_util.goto_board(api, board)
 
     cmd_list = []
 
     if post_aid is not None:
-        cmd_list.append('#' + post_aid)
+        cmd_list.append(lib_util.check_aid(post_aid))
     elif post_index != 0:
         cmd_list.append(str(post_index))
+    else:
+        raise ValueError('post_aid and post_index cannot be None at the same time')
+
     cmd_list.append(command.enter)
     cmd_list.append('d')
 
     cmd = ''.join(cmd_list)
 
     api.confirm = False
```

### Comparing `PyPtt-1.0.6/PyPtt/_api_get_board_info.py` & `PyPtt-1.0.7/PyPtt/_api_get_board_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -230,37 +230,14 @@
         target_list = [
             connect_core.TargetUnit(screens.Target.InBoard, break_detect=True)
         ]
         api.connect_core.send(
             cmd,
             target_list)
 
-    # board_info = data_type.BoardInfo(
-    #     boardname,
-    #     online_user,
-    #     mandarin_des,
-    #     moderators,
-    #     open_status,
-    #     into_top_ten_when_hide,
-    #     can_non_board_members_post,
-    #     can_reply_post,
-    #     self_del_post,
-    #     can_comment_post,
-    #     can_boo_post,
-    #     can_fast_push,
-    #     min_interval_between_comments,
-    #     is_comment_record_ip,
-    #     is_comment_aligned,
-    #     can_moderators_del_illegal_content,
-    #     does_tran_post_auto_recorded_and_require_post_permissions,
-    #     is_cool_mode,
-    #     is_require18,
-    #     require_login_time,
-    #     require_illegal_post,
-    #     post_kind_list)
     return {
         BoardField.board: boardname,
         BoardField.online_user: online_user,
         BoardField.mandarin_des: chinese_des,
         BoardField.moderators: moderators,
         BoardField.open_status: open_status,
         BoardField.into_top_ten_when_hide: into_top_ten_when_hide,
```

### Comparing `PyPtt-1.0.6/PyPtt/_api_get_board_list.py` & `PyPtt-1.0.7/PyPtt/_api_get_board_list.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/_api_get_bottom_post_list.py` & `PyPtt-1.0.7/PyPtt/_api_get_bottom_post_list.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/_api_get_favourite_board.py` & `PyPtt-1.0.7/PyPtt/_api_get_favourite_board.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/_api_get_newest_index.py` & `PyPtt-1.0.7/PyPtt/_api_get_newest_index.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/_api_get_post.py` & `PyPtt-1.0.7/PyPtt/_api_get_post.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from . import _api_util
 from . import check_value
 from . import command
 from . import connect_core
 from . import data_type
 from . import exceptions
 from . import i18n
+from . import lib_util
 from . import screens
 from .data_type import PostField, CommentField, NewIndex
 from .data_type import SearchType as st
 
 
 def get_post(api, board: str, aid: [str | None] = None, index: int = 0, search_list: [list | None] = None,
              search_type: data_type.SearchType = data_type.SearchType.NOPE,
@@ -107,15 +108,15 @@
     _api_util.goto_board(api, board)
 
     logger = DefaultLogger('get_post')
 
     cmd_list = []
 
     if post_aid is not None:
-        cmd_list.append('#' + post_aid)
+        cmd_list.append(lib_util.check_aid(post_aid))
 
     elif post_index != 0:
         if search_condition is not None:
             if search_type == data_type.SearchType.KEYWORD:
                 cmd_list.append('/')
             elif search_type == data_type.SearchType.AUTHOR:
                 cmd_list.append('a')
@@ -145,14 +146,16 @@
 
                 cmd_list.append(search_condition_)
                 cmd_list.append(command.enter)
 
         cmd_list.append(str(max(1, post_index - 100)))
         cmd_list.append(command.enter)
         cmd_list.append(str(post_index))
+    else:
+        raise ValueError('post_aid and post_index cannot be None at the same time')
 
     cmd_list.append(command.enter)
     cmd_list.append(command.query_post)
 
     cmd = ''.join(cmd_list)
 
     target_list = [
@@ -277,15 +280,14 @@
             PostField.pass_format_check: True,
             PostField.push_number: push_number})
         return post
 
     origin_post, has_control_code = _api_util.get_content(api)
 
     if origin_post is None:
-
         logger.info(i18n.post_deleted)
 
         post.update({
             PostField.board: board,
             PostField.aid: post_aid,
             PostField.index: post_index,
             PostField.author: post_author,
```

### Comparing `PyPtt-1.0.6/PyPtt/_api_get_post_index.py` & `PyPtt-1.0.7/PyPtt/_api_get_post_index.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/_api_get_time.py` & `PyPtt-1.0.7/PyPtt/_api_get_time.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/_api_get_user.py` & `PyPtt-1.0.7/PyPtt/_api_get_user.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/_api_give_money.py` & `PyPtt-1.0.7/PyPtt/_api_give_money.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/_api_has_new_mail.py` & `PyPtt-1.0.7/PyPtt/_api_has_new_mail.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/_api_loginout.py` & `PyPtt-1.0.7/PyPtt/_api_loginout.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/_api_mail.py` & `PyPtt-1.0.7/PyPtt/_api_mail.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/_api_mark_post.py` & `PyPtt-1.0.7/PyPtt/_api_mark_post.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,18 +79,16 @@
         board,
         check_moderator=True)
 
     _api_util.goto_board(api, board)
 
     cmd_list = []
     if post_aid is not None:
-        cmd_list.append('#' + post_aid)
-
+        cmd_list.append(lib_util.check_aid(post_aid))
         cmd_list.append(command.enter)
-
     elif post_index != 0:
         if search_condition is not None:
             if search_type == data_type.SearchType.KEYWORD:
                 cmd_list.append('/')
             elif search_type == data_type.SearchType.AUTHOR:
                 cmd_list.append('a')
             elif search_type == data_type.SearchType.COMMENT:
@@ -102,14 +100,16 @@
 
             cmd_list.append(search_condition)
             cmd_list.append(command.enter)
 
         cmd_list.append(str(post_index))
 
         cmd_list.append(command.enter)
+    else:
+        raise ValueError('post_aid and post_index cannot be None at the same time')
 
     if mark_type == data_type.MarkType.S:
         cmd_list.append('L')
     elif mark_type == data_type.MarkType.D:
         cmd_list.append('t')
     elif mark_type == data_type.MarkType.DELETE_D:
         cmd_list.append(command.ctrl_d)
```

### Comparing `PyPtt-1.0.6/PyPtt/_api_post.py` & `PyPtt-1.0.7/PyPtt/_api_post.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/_api_reply_post.py` & `PyPtt-1.0.7/PyPtt/_api_reply_post.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from . import _api_util
 from . import check_value
 from . import command
 from . import connect_core
 from . import data_type
 from . import exceptions
 from . import i18n
+from . import lib_util
 
 
 def reply_post(api, reply_to: data_type.ReplyTo, board: str, content: str, sign_file, post_aid: str,
                post_index: int) -> None:
     _api_util.one_thread(api)
 
     if not api._is_login:
@@ -45,17 +46,20 @@
     _api_util.check_board(api, board)
 
     _api_util.goto_board(api, board)
 
     cmd_list = []
 
     if post_aid is not None:
-        cmd_list.append('#' + post_aid)
+        cmd_list.append(lib_util.check_aid(post_aid))
     elif post_index != 0:
         cmd_list.append(str(post_index))
+    else:
+        raise ValueError('post_aid and post_index cannot be None at the same time')
+
     cmd_list.append(command.enter * 2)
     cmd_list.append('r')
 
     if reply_to == data_type.ReplyTo.BOARD:
         api.logger.info(i18n.reply_board)
         reply_target_unit = connect_core.TargetUnit('▲ 回應至', log_level=LogLevel.INFO, response='F' + command.enter)
     elif reply_to == data_type.ReplyTo.MAIL:
```

### Comparing `PyPtt-1.0.6/PyPtt/_api_search_user.py` & `PyPtt-1.0.7/PyPtt/_api_search_user.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/_api_set_board_title.py` & `PyPtt-1.0.7/PyPtt/_api_set_board_title.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/_api_util.py` & `PyPtt-1.0.7/PyPtt/_api_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,15 +465,15 @@
     if board.lower() not in api._exist_board_list:
         board_info = _api_get_board_info.get_board_info(api, board, get_post_kind=False, call_by_others=False)
         api._exist_board_list.append(board.lower())
         api._board_info_list[board.lower()] = board_info
 
         moderators = board_info[data_type.BoardField.moderators]
         moderators = [x.lower() for x in moderators]
-        api._ModeratorList[board.lower()] = moderators
+        api._moderators[board.lower()] = moderators
         api._board_info_list[board.lower()] = board_info
 
     if check_moderator:
-        if api.ptt_id.lower() not in api._ModeratorList[board.lower()]:
+        if api.ptt_id.lower() not in api._moderators[board.lower()]:
             raise exceptions.NeedModeratorPermission(board)
 
     return api._board_info_list[board.lower()]
```

### Comparing `PyPtt-1.0.6/PyPtt/check_value.py` & `PyPtt-1.0.7/PyPtt/check_value.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/command.py` & `PyPtt-1.0.7/PyPtt/command.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/config.py` & `PyPtt-1.0.7/PyPtt/config.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/connect_core.py` & `PyPtt-1.0.7/PyPtt/connect_core.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/data_type.py` & `PyPtt-1.0.7/PyPtt/data_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,26 +25,14 @@
     COMMENT = auto()
     # 搜尋標記      G
     MARK = auto()
     # 搜尋稿酬      A
     MONEY = auto()
 
 
-# class MailSearchType(IntEnum):
-#     """信件搜尋類型"""
-#
-#     NOPE = auto()
-#     # 搜尋關鍵字    / ?
-#     KEYWORD = auto()
-#     # 搜尋作者      a
-#     AUTHOR = auto()
-#     # 搜尋標記      G
-#     MARK = auto()
-
-
 class ReplyTo(AutoStrEnum):
     # 回文類型
 
     BOARD = auto()
     MAIL = auto()
     BOARD_MAIL = auto()
```

### Comparing `PyPtt-1.0.6/PyPtt/exceptions.py` & `PyPtt-1.0.7/PyPtt/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/i18n.py` & `PyPtt-1.0.7/PyPtt/i18n.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/lib_util.py` & `PyPtt-1.0.7/PyPtt/lib_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,28 +32,29 @@
     return len(haystack) - len(parts[-1]) - len(needle)
 
 
 def get_random_str(length) -> str:
     return ''.join(random.choices(string.hexdigits, k=length))
 
 
+# 演算法參考 https://www.ptt.cc/man/C_Chat/DE98/DFF5/DB61/M.1419434423.A.DF0.html
+# aid 字元表
+aid_table = '0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz-_'
+
+
 def get_aid_from_url(url: str) -> Tuple[str, str]:
     # 檢查是否為字串
     check_value.check_type(url, str, 'url')
 
     # 檢查是否符合 PTT BOARD 文章網址格式
     pattern = re.compile('https://www.ptt.cc/bbs/[-.\w]+/M.[\d]+.A[.\w]*.html')
     r = pattern.search(url)
     if r is None:
         raise ValueError('wrong parameter url must be www.ptt.cc post url')
 
-    # 演算法參考 https://www.ptt.cc/man/C_Chat/DE98/DFF5/DB61/M.1419434423.A.DF0.html
-    # aid 字元表
-    aid_table = '0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz-_'
-
     board = url[23:]
     board = board[:board.find('/')]
 
     temp = url[url.rfind('/') + 1:].split('.')
     # print(temp)
 
     id_0 = int(temp[1])  # dec
@@ -139,10 +140,30 @@
     text = text.replace('\r\n', random_tag)
     text = text.replace('\n', '\r\n')
     text = text.replace(random_tag, '\r\n')
 
     return text
 
 
+def check_aid(aid: str) -> str:
+    if aid is None:
+        raise ValueError('aid is None')
+
+    if not isinstance(aid, str):
+        raise TypeError('aid is not str')
+
+    if aid.startswith('#'):
+        aid = aid[1:]
+
+    if len(aid) != 8:
+        raise ValueError('aid is not valid')
+
+    # check the char of aid is in aid_table or not
+    for char in aid:
+        if char not in aid_table:
+            raise ValueError('aid is not valid')
+
+    return f'#{aid}'
+
+
 if __name__ == '__main__':
-    for _ in range(5):
-        print(get_random_str(10))
+    check_aid('#1aBzRW4z')
```

### Comparing `PyPtt-1.0.6/PyPtt/screens.py` & `PyPtt-1.0.7/PyPtt/screens.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt/service.py` & `PyPtt-1.0.7/PyPtt/service.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/PyPtt.egg-info/PKG-INFO` & `PyPtt-1.0.7/PyPtt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPtt
-Version: 1.0.6
+Version: 1.0.7
 Summary: PyPtt
 Home-page: https://github.com/PyPtt/PyPtt
 Author: CodingMan
 Author-email: pttcodingman@gmail.com
 Keywords: PTT,crawler,bot,library,websockets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `PyPtt-1.0.6/PyPtt.egg-info/SOURCES.txt` & `PyPtt-1.0.7/PyPtt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/README.md` & `PyPtt-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `PyPtt-1.0.6/setup.py` & `PyPtt-1.0.7/setup.py`

 * *Files identical despite different names*

